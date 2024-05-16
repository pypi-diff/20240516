# Comparing `tmp/exegol-4.3.2.tar.gz` & `tmp/exegol-4.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exegol-4.3.2.tar", last modified: Mon Apr 15 19:22:20 2024, max compression
+gzip compressed data, was "exegol-4.3.3.tar", last modified: Thu May 16 01:32:29 2024, max compression
```

## Comparing `exegol-4.3.2.tar` & `exegol-4.3.3.tar`

### file list

```diff
@@ -1,750 +1,750 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.332595 exegol-4.3.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.332595 exegol-4.3.2/Exegol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-04-15 19:22:20.000000 exegol-4.3.2/Exegol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    40881 2024-04-15 19:22:20.000000 exegol-4.3.2/Exegol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 19:22:20.000000 exegol-4.3.2/Exegol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-15 19:22:20.000000 exegol-4.3.2/Exegol.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-15 19:22:20.000000 exegol-4.3.2/Exegol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 19:22:20.000000 exegol-4.3.2/Exegol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-15 19:21:51.000000 exegol-4.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-04-15 19:22:20.332595 exegol-4.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-04-15 19:21:51.000000 exegol-4.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.208594 exegol-4.3.2/exegol/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.324595 exegol-4.3.2/exegol/config/
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/config/ConstantConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/config/DataCache.py
--rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/config/EnvInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/config/UserConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.324595 exegol-4.3.2/exegol/console/
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/console/ConsoleFormat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/console/ExegolProgress.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/console/ExegolPrompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/console/LayerTextColumn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/console/MetaGitProgress.py
--rw-r--r--   0 runner    (1001) docker     (127)    26707 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/console/TUI.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/console/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.324595 exegol-4.3.2/exegol/console/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/console/cli/ExegolCompleter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/console/cli/ParametersManager.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/console/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.324595 exegol-4.3.2/exegol/console/cli/actions/
--rw-r--r--   0 runner    (1001) docker     (127)     7471 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/console/cli/actions/Command.py
--rw-r--r--   0 runner    (1001) docker     (127)    14442 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/console/cli/actions/ExegolParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)    17522 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/console/cli/actions/GenericParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/console/cli/actions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.324595 exegol-4.3.2/exegol/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/exceptions/ExegolExceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.324595 exegol-4.3.2/exegol/manager/
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/manager/ExegolController.py
--rw-r--r--   0 runner    (1001) docker     (127)    31118 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/manager/ExegolManager.py
--rw-r--r--   0 runner    (1001) docker     (127)    22083 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/manager/UpdateManager.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.328595 exegol-4.3.2/exegol/model/
--rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/model/CacheModels.py
--rw-r--r--   0 runner    (1001) docker     (127)    74813 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/model/ContainerConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    18282 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/model/ExegolContainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/model/ExegolContainerTemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)    33485 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/model/ExegolImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/model/ExegolModules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/model/MetaImages.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/model/SelectableInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.328595 exegol-4.3.2/exegol/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/utils/ContainerLogStream.py
--rw-r--r--   0 runner    (1001) docker     (127)     8069 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/utils/DataFileUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)    34554 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/utils/DockerUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4977 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/utils/ExeLog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/utils/FsUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20384 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/utils/GitUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20020 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/utils/GuiUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/utils/MetaSingleton.py
--rw-r--r--   0 runner    (1001) docker     (127)     8053 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/utils/WebUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/utils/argParse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.328595 exegol-4.3.2/exegol/utils/imgsync/
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/utils/imgsync/ImageScriptSync.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/utils/imgsync/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5110 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/utils/imgsync/entrypoint.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     2188 2024-04-15 19:21:51.000000 exegol-4.3.2/exegol/utils/imgsync/spawn.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.208594 exegol-4.3.2/exegol-docker-build/
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/ad.dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/light.dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/osint.dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.208594 exegol-4.3.2/exegol-docker-build/sources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.204594 exegol-4.3.2/exegol-docker-build/sources/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.208594 exegol-4.3.2/exegol-docker-build/sources/assets/bloodhound/
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/bloodhound/config.json
--rw-r--r--   0 runner    (1001) docker     (127)    58751 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/bloodhound/customqueries.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.208594 exegol-4.3.2/exegol-docker-build/sources/assets/bloodhound-ce/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/bloodhound-ce/bloodhound-ce
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/bloodhound-ce/bloodhound-ce-reset
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/bloodhound-ce/bloodhound-ce-stop
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/bloodhound-ce/bloodhound.config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.212594 exegol-4.3.2/exegol-docker-build/sources/assets/burpsuite/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/burpsuite/UserConfigCommunity.json
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/burpsuite/conf.json
--rwxr-xr-x   0 runner    (1001) docker     (127)     3005 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/burpsuite/trust-ca-burp.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.212594 exegol-4.3.2/exegol-docker-build/sources/assets/crackmapexec/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/crackmapexec/cme.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.212594 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/
--rw-r--r--   0 runner    (1001) docker     (127)   670539 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/Prof_XFCE_2_1.tar.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.212594 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/applications/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/applications/bloodhound.desktop
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/applications/burpsuite.desktop
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/applications/ghidra.desktop
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/applications/jd-gui.desktop
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/applications/maltego.desktop
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/applications/remmina.desktop
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/applications/wireshark.desktop
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.212594 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)       39 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/bin/desktop-restart
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/bin/desktop-start
--rwxr-xr-x   0 runner    (1001) docker     (127)       45 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/bin/desktop-stop
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.216594 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/bookmarks
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/config
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/docklike-2.rc
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/exegol.directory
--rw-r--r--   0 runner    (1001) docker     (127)    83326 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/wallpaper.png
--rw-r--r--   0 runner    (1001) docker     (127)   101362 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/wallpaper2.png
--rw-r--r--   0 runner    (1001) docker     (127)    91894 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/wallpaper3.png
--rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/xfce-applications.menu
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/xfce4-desktop.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/xfce4-panel.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/xsettings.xml
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/xstartup.conf
--rw-r--r--   0 runner    (1001) docker     (127)    81901 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/exegol_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.216594 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/wallpapers/
--rw-r--r--   0 runner    (1001) docker     (127)   117551 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/wallpapers/default.png
--rw-r--r--   0 runner    (1001) docker     (127)   123335 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/wallpapers/desert.png
--rw-r--r--   0 runner    (1001) docker     (127)   123905 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/wallpapers/forest.png
--rw-r--r--   0 runner    (1001) docker     (127)   123311 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/wallpapers/glacier.png
--rw-r--r--   0 runner    (1001) docker     (127)    78352 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/wallpapers/midnight.png
--rw-r--r--   0 runner    (1001) docker     (127)    75451 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/desktop/wallpapers/space.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.216594 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.216594 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/build_pipeline_tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/build_pipeline_tests/run_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/entrypoint.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)    11378 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/load_supported_setups.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.220595 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.220595 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/apt/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/apt/keys.list
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/apt/packages.list
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/apt/sources.list
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.220595 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/bloodhound/
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/bloodhound/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.220595 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/bloodhound/customqueries_merge/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/bloodhound/customqueries_merge/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.220595 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/bloodhound/customqueries_replacement/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/bloodhound/customqueries_replacement/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.220595 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/firefox/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/firefox/addons.txt
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/load_user_setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.220595 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/python3/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/python3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/supported_setups.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.220595 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/zsh/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/zsh/aliases
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/zsh/history
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/zsh/zshrc
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/exegol/start.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.224594 exegol-4.3.2/exegol-docker-build/sources/assets/firefox/
--rw-r--r--   0 runner    (1001) docker     (127)  1703936 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/firefox/places.sqlite
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/firefox/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/firefox/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/firefox/user-setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.224594 exegol-4.3.2/exegol-docker-build/sources/assets/grc/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/grc/conf.cme
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/grc/conf.describeTicket
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/grc/conf.getgpppassword
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/grc/conf.krbrelayx
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/grc/conf.ntlmrelayx
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/grc/conf.rbcd
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/grc/conf.secretsdump
--rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/grc/grc.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.224594 exegol-4.3.2/exegol-docker-build/sources/assets/logrotate/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/logrotate/exegol_vpn
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.224594 exegol-4.3.2/exegol-docker-build/sources/assets/netexec/
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/netexec/nxc.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.224594 exegol-4.3.2/exegol-docker-build/sources/assets/patches/
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/patches/cloudmapper.patch
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/patches/openssl.patch
--rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/patches/undefined-symbol-aesni-key.patch
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.224594 exegol-4.3.2/exegol-docker-build/sources/assets/proxychains/
--rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/proxychains/proxychains.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.224594 exegol-4.3.2/exegol-docker-build/sources/assets/python/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/python/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.228594 exegol-4.3.2/exegol-docker-build/sources/assets/shells/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.256595 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/LDAPWordlistHarvester
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/MurMurHash
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/PassTheCert
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/Xspear
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/_init
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/aircrack-ng
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/arsenal
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/bat
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/bettercap
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/blackbird
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/blazy
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/bloodhound
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/bloodhound-py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/bloodhound-quickwin
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/bolt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/bqm
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/brakeman
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/burpsuite
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/carbon14
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/cewl
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/checksec
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/cloudfail
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/cloudmapper
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/cloudsploit
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/clusterd
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/corscanner
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/crackhound
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/crackmapexec
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/cypheroth
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/darkarmour
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/dfscoerce
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/dnschef
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/drupwn
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/eaphammer
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/emacs-nox
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/empire
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/enyx
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/evil-winrm
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/extractbitlockerkeys
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/eyewitness
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/feroxbuster
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/finalrecon
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/finduncommonshares
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/fuxploider
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/fzf
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/gdb
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/geopincer
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/ghidra
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/ghunt
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/gittools
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/gmsadumper
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/gopherus
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/gpp-decrypt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/grc
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/h2csmuggler
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/haiti
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/havoc
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/httpmethods
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/ida
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/impacket
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/infoga
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/jd-gui
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/jdwp-shellifier
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/john-the-ripper
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/joomscan
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/jwt_tool
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/kadimus
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/kraken
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/krbrelayx
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/ldaprelayscan
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/ldapsearch-ad
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/libmspack
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/libnfc-crypto1-crack
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/linkedin2username
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/linkfinder
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/lnkup
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/manspider
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/metasploit
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/mfdread
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/mobsf
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/moodlescan
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/mousejack
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/neo4j
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/netexec
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/nmap
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/noPac
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/nosqlmap
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/ntlm_theft
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/ntlmv1-multi
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/oaburl
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/oneforall
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/pass-station
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/patator
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/pcredz
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/peepdf
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/petitpotam
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/photon
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/php
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/php_filter_chain_generator
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/phpggc
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/pkinittools
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/polenum
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/powershell
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/privexchange
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/proxmark3
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/proxychains
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/pth-tools
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/pwndb
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/pwnedornot
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/pyftpdlib
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/pygpoabuse
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/pykek
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/pylaps
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/pyrit
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/python3
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/pywhisker
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/pywsus
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/recondog
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/responder
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/routersploit
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/rsactftool
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/sccmhunter
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/sccmwtf
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/shadowcoerce
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/sherlock
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/simplyemail
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/smali
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/smuggler
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/soapui
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/spiderfoot
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/ssrfmap
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/starkiller
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/symfony-exploits
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/tailscale
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/targetedkerberoast
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/teamsphisher
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/testssl
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/theharvester
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/timing_attack
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/tls-map
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/tls-scanner
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/tomcatwardeployer
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/trid
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/trilium
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/username-anarchy
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/villain
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/volatility2
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/volatility3
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/weevely
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/whatweb
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/wifite
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/wpscan
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/xmllint
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/xsel
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/xsser
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/xsstrike
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/ysoserial
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/zerologon
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/zsteg
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/bashrc
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/exegol_shells_rc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.316595 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/GPOddity
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/LDAPWordlistHarvester
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/MurMurHash
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/PassTheCert
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/XSpear
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/_init
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/abuseACL
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/aclpwn
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/adb
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/adidnsdump
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/aircrack-ng
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/amass
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/amber
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/androguard
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/anew
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/apksigner
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/apktool
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/arjun
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/arsenal
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ascii
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/assetfinder
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/autorecon
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/avrdude
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/aws
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/azure-cli
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/bettercap
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/binwalk
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/blackbird
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/bloodhound
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/bloodhound-ce-py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/bloodhound-import
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/bloodhound-py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/bloodhound-quickwin
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/bloodyAD
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/bolt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/bqm
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/brakeman
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/bruteforce-luks
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/bully
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/burpsuite
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/buster
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/byp4xx
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/carbon14
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/censys
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/certipy
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/certsync
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/cewl
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/cewler
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/chainsaw
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/checksec
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/chisel
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/cloudfail
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/cloudmapper
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/cloudsplaining
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/clusterd
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/cmsmap
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/coercer
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/constellation
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/corscanner
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/cowpatty
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/crackhound
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/crackmapexec
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/crunch
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ctf-party
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/cupp
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/curl
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/cypheroth
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/darkarmour
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/dex2jar
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/dfscoerce
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/dirb
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/dirsearch
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/divideandscan
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/dnschef
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/dnsenum
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/dnsutils
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/dnsx
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/donpapi
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/dploot
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/droopescan
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/drupwn
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/eaphammer
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/empire
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/enum4linux-ng
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/enyx
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/evil-winrm
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/exif
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/exifprobe
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/exiftool
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/exiv2
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/extractbitlockerkeys
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/eyewitness
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/faketime
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/fcrackzip
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/fdisk
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/feroxbuster
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ffuf
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/fierce
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/finalrecon
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/findomain
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/finduncommonshares
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/firefox
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/foremost
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/freeipscanner
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/frida
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/fuxploider
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/gau
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/gdb
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/genusernames
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/geopincer
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/geowordlists
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/gf
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ghidra
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/git-dumper
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/github-email
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/gittools
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/gmsadumper
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/gobuster
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/goldencopy
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/gomapenum
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/gopherus
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/gosecretsdump
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/goshs
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/gowitness
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/gpp-decrypt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/gqrx
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/gron
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/h2csmuggler
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/h8mail
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/hackrf
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/haiti
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/hakrawler
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/hakrevdns
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/hashcat
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/hashonymize
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/havoc
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/hcxdumptool
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/hcxtools
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/hexedit
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/holehe
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/hping3
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/httpmethods
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/httprobe
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/httpx
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/hydra
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ida
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ignorant
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/imagemagick
--rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/impacket
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/infoga
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ipinfo
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/iptables
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/jackit
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/jadx
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/jd-gui
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/jdwp-shellifier
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/john-the-ripper
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/joomscan
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/jwt_tool
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/kadimus
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/keepwn
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/kerbrute
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/kiterunner
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/kraken
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/krbrelayx
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/kubectl
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ldapdomaindump
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ldaprelayscan
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ldapsearch
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ldapsearch-ad
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ldeep
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/legba
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/libmspack
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/libnfc
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/libnfc-crypto1-crack
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ligolo-ng
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/linkedin2username
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/linkfinder
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/lnkup
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/lsassy
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/maigret
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/maltego
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/manspider
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/masky
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/masscan
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/mfcuk
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/mfdread
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/mfoc
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/minicom
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/mitm6
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/mobsf
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/moodlescan
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/mousejack
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/msprobe
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/naabu
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/name-that-hash
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/nasm
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/nbtscan
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/neo4j
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/netdiscover
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/netexec
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ngrok
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/nmap
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/nmap-parse-output
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/noPac
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/notify
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ntlm_theft
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ntlmv1-multi
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ntpdate
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/nuclei
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/oaburl
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/objection
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/objectwalker
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/oneforall
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/onesixtyone
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/osrframework
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pass-station
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/patator
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pcredz
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pdfcrack
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/peepdf
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/petitpotam
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/phoneinfoga
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/photon
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/php_filter_chain_generator
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/phpggc
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pkcrack
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pkinittools
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/polenum
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/powershell
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pp-finder
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pre2k
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pretender
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/prips
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/privexchange
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/prowler
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/proxmark3
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/proxychains
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pth-tools
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pwncat
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pwndb
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pwnedornot
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pwninit
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pyftpdlib
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pygpoabuse
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pykek
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pylaps
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pymeta
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pypykatz
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pyrit
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pywerview
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pywhisker
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pywsus
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/radare2
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/rdesktop
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/reaver
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/recon-ng
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/recondog
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/responder
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/rlwrap
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/roastinthemiddle
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/robotstester
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/rsacracker
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/rsactftool
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/rsync
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/rtl-433
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ruler
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/rusthound
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/rustscan
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/rustscan-ce
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/samba
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/samdump2
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/sccmhunter
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/sccmwtf
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/scout
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/scrcpy
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/scrtdnsdump
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/searchsploit
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/semgrep
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/shadowcoerce
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/shellerator
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/shuffledns
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/simplyemail
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/sipvicious_svcrack
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/sliver
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/smali
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/smartbrute
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/smbclient
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/smbmap
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/smtp-user-enum
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/smuggler
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/snmp
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/spiderfoot
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/sprayhound
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/sqlmap
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ssh
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ssh-audit
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/sshuttle
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/sslscan
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/sslyze
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ssrfmap
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/steghide
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/stegolsb
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/stegosuite
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/strace
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/subfinder
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/sublist3r
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/swaks
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/symfony-exploits
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/tailscale
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/targetedkerberoast
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/tcpdump
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/teamsphisher
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/testdisk
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/testssl
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/theharvester
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/timing_attack
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/tls-map
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/tls-scanner
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/tomcatwardeployer
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/tor
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/toutatis
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/traceroute
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/trevorspray
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/trid
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/trilium
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/tshark
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/twint
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/uberfile
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/updog
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/username-anarchy
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/villain
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/volatility2
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/volatility3
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/wafw00f
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/waybackurls
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/webclientservicescanner
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/weevely
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/wfuzz
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/whatportis
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/whatweb
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/whois
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/wifite
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/windapsearch
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/wireshark
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/wpscan
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/wuzz
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/xfreerdp
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/xsrfprobe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/xsser
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/xsstrike
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/yalis
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/youtube-dl
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/ysoserial
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/zerologon
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/zipalign
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/zsteg
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/tmux.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/shells/zshrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.316595 exegol-4.3.2/exegol-docker-build/sources/assets/trilium/
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/trilium/config.ini
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/assets/trilium/trilium-manager.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/build_logs_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/code_compliance_check.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.316595 exegol-4.3.2/exegol-docker-build/sources/dockerfiles/
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/dockerfiles/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/dockerfiles/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/dockerfiles/ad.dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/dockerfiles/base.dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/dockerfiles/light.dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/dockerfiles/osint.dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/dockerfiles/web.dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.320595 exegol-4.3.2/exegol-docker-build/sources/install/
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/common.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (127)    68328 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_ad.sh
--rw-r--r--   0 runner    (1001) docker     (127)    21661 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_base.sh
--rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_c2.sh
--rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_cloud.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_code_analysis.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_cracking.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_crypto.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_desktop.sh
--rw-r--r--   0 runner    (1001) docker     (127)     5996 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_forensic.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_iot.sh
--rw-r--r--   0 runner    (1001) docker     (127)     9612 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_misc.sh
--rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_mobile.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_most_used.sh
--rw-r--r--   0 runner    (1001) docker     (127)    15455 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_network.sh
--rw-r--r--   0 runner    (1001) docker     (127)    27488 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_osint.sh
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_reverse.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_rfid.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_sdr.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_steganography.sh
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_voip.sh
--rw-r--r--   0 runner    (1001) docker     (127)    40434 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_web.sh
--rw-r--r--   0 runner    (1001) docker     (127)     6276 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_wifi.sh
--rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/sources/install/package_wordlists.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/web.dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-15 19:22:03.000000 exegol-4.3.2/exegol-docker-build/wifi.dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 19:22:20.332595 exegol-4.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-15 19:21:51.000000 exegol-4.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:22:20.332595 exegol-4.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-15 19:21:51.000000 exegol-4.3.2/tests/test_exegol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:29.107391 exegol-4.3.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:29.107391 exegol-4.3.3/Exegol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-05-16 01:32:28.000000 exegol-4.3.3/Exegol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    40881 2024-05-16 01:32:28.000000 exegol-4.3.3/Exegol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 01:32:28.000000 exegol-4.3.3/Exegol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-16 01:32:28.000000 exegol-4.3.3/Exegol.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-16 01:32:28.000000 exegol-4.3.3/Exegol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 01:32:28.000000 exegol-4.3.3/Exegol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-16 01:31:57.000000 exegol-4.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-05-16 01:32:29.107391 exegol-4.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-05-16 01:31:57.000000 exegol-4.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:28.967390 exegol-4.3.3/exegol/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:29.099391 exegol-4.3.3/exegol/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/config/ConstantConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/config/DataCache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9304 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/config/EnvInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/config/UserConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:29.099391 exegol-4.3.3/exegol/console/
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/console/ConsoleFormat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/console/ExegolProgress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/console/ExegolPrompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/console/LayerTextColumn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/console/MetaGitProgress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26707 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/console/TUI.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/console/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:29.099391 exegol-4.3.3/exegol/console/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/console/cli/ExegolCompleter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/console/cli/ParametersManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/console/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:29.103391 exegol-4.3.3/exegol/console/cli/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)     7471 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/console/cli/actions/Command.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14442 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/console/cli/actions/ExegolParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17522 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/console/cli/actions/GenericParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/console/cli/actions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:29.103391 exegol-4.3.3/exegol/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/exceptions/ExegolExceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:29.103391 exegol-4.3.3/exegol/manager/
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/manager/ExegolController.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30890 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/manager/ExegolManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22099 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/manager/UpdateManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:29.103391 exegol-4.3.3/exegol/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/model/CacheModels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75465 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/model/ContainerConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18282 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/model/ExegolContainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/model/ExegolContainerTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33485 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/model/ExegolImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/model/ExegolModules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/model/MetaImages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/model/SelectableInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:29.107391 exegol-4.3.3/exegol/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/utils/ContainerLogStream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8276 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/utils/DataFileUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34937 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/utils/DockerUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4977 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/utils/ExeLog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/utils/FsUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20395 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/utils/GitUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20122 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/utils/GuiUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/utils/MetaSingleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8053 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/utils/WebUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/utils/argParse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:29.107391 exegol-4.3.3/exegol/utils/imgsync/
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/utils/imgsync/ImageScriptSync.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/utils/imgsync/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5110 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/utils/imgsync/entrypoint.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2188 2024-05-16 01:31:57.000000 exegol-4.3.3/exegol/utils/imgsync/spawn.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:28.967390 exegol-4.3.3/exegol-docker-build/
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/ad.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/light.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/osint.dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:28.967390 exegol-4.3.3/exegol-docker-build/sources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:28.963390 exegol-4.3.3/exegol-docker-build/sources/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:28.971390 exegol-4.3.3/exegol-docker-build/sources/assets/bloodhound/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/bloodhound/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)    58751 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/bloodhound/customqueries.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:28.971390 exegol-4.3.3/exegol-docker-build/sources/assets/bloodhound-ce/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/bloodhound-ce/bloodhound-ce
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/bloodhound-ce/bloodhound-ce-reset
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/bloodhound-ce/bloodhound-ce-stop
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/bloodhound-ce/bloodhound.config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:28.971390 exegol-4.3.3/exegol-docker-build/sources/assets/burpsuite/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/burpsuite/UserConfigCommunity.json
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/burpsuite/conf.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3005 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/burpsuite/trust-ca-burp.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:28.971390 exegol-4.3.3/exegol-docker-build/sources/assets/crackmapexec/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/crackmapexec/cme.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:28.971390 exegol-4.3.3/exegol-docker-build/sources/assets/desktop/
+-rw-r--r--   0 runner    (1001) docker     (127)   670539 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/desktop/Prof_XFCE_2_1.tar.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:28.975390 exegol-4.3.3/exegol-docker-build/sources/assets/desktop/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/desktop/applications/bloodhound.desktop
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/desktop/applications/burpsuite.desktop
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/desktop/applications/ghidra.desktop
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/desktop/applications/jd-gui.desktop
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/desktop/applications/maltego.desktop
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/desktop/applications/remmina.desktop
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/desktop/applications/wireshark.desktop
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:28.975390 exegol-4.3.3/exegol-docker-build/sources/assets/desktop/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       39 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/desktop/bin/desktop-restart
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/desktop/bin/desktop-start
+-rwxr-xr-x   0 runner    (1001) docker     (127)       45 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/desktop/bin/desktop-stop
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:28.979390 exegol-4.3.3/exegol-docker-build/sources/assets/desktop/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/desktop/configuration/bookmarks
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/desktop/configuration/config
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/desktop/configuration/docklike-2.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/desktop/configuration/exegol.directory
+-rw-r--r--   0 runner    (1001) docker     (127)    83326 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/desktop/configuration/wallpaper.png
+-rw-r--r--   0 runner    (1001) docker     (127)   101362 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/desktop/configuration/wallpaper2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    91894 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/desktop/configuration/wallpaper3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/desktop/configuration/xfce-applications.menu
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/desktop/configuration/xfce4-desktop.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/desktop/configuration/xfce4-panel.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/desktop/configuration/xsettings.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/desktop/configuration/xstartup.conf
+-rw-r--r--   0 runner    (1001) docker     (127)    81901 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/desktop/exegol_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:28.979390 exegol-4.3.3/exegol-docker-build/sources/assets/desktop/wallpapers/
+-rw-r--r--   0 runner    (1001) docker     (127)   117551 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/desktop/wallpapers/default.png
+-rw-r--r--   0 runner    (1001) docker     (127)   123335 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/desktop/wallpapers/desert.png
+-rw-r--r--   0 runner    (1001) docker     (127)   123905 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/desktop/wallpapers/forest.png
+-rw-r--r--   0 runner    (1001) docker     (127)   123311 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/desktop/wallpapers/glacier.png
+-rw-r--r--   0 runner    (1001) docker     (127)    78352 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/desktop/wallpapers/midnight.png
+-rw-r--r--   0 runner    (1001) docker     (127)    75451 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/desktop/wallpapers/space.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:28.979390 exegol-4.3.3/exegol-docker-build/sources/assets/exegol/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:28.979390 exegol-4.3.3/exegol-docker-build/sources/assets/exegol/build_pipeline_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/exegol/build_pipeline_tests/run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/exegol/entrypoint.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11378 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/exegol/load_supported_setups.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:28.979390 exegol-4.3.3/exegol-docker-build/sources/assets/exegol/skel/
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/exegol/skel/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:28.983390 exegol-4.3.3/exegol-docker-build/sources/assets/exegol/skel/apt/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/exegol/skel/apt/keys.list
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/exegol/skel/apt/packages.list
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/exegol/skel/apt/sources.list
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:28.983390 exegol-4.3.3/exegol-docker-build/sources/assets/exegol/skel/bloodhound/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/exegol/skel/bloodhound/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:28.983390 exegol-4.3.3/exegol-docker-build/sources/assets/exegol/skel/bloodhound/customqueries_merge/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/exegol/skel/bloodhound/customqueries_merge/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:28.983390 exegol-4.3.3/exegol-docker-build/sources/assets/exegol/skel/bloodhound/customqueries_replacement/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/exegol/skel/bloodhound/customqueries_replacement/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:28.983390 exegol-4.3.3/exegol-docker-build/sources/assets/exegol/skel/firefox/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/exegol/skel/firefox/addons.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/exegol/skel/load_user_setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:28.983390 exegol-4.3.3/exegol-docker-build/sources/assets/exegol/skel/python3/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/exegol/skel/python3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/exegol/skel/supported_setups.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:28.983390 exegol-4.3.3/exegol-docker-build/sources/assets/exegol/skel/zsh/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/exegol/skel/zsh/aliases
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/exegol/skel/zsh/history
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/exegol/skel/zsh/zshrc
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/exegol/start.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:28.987390 exegol-4.3.3/exegol-docker-build/sources/assets/firefox/
+-rw-r--r--   0 runner    (1001) docker     (127)  1703936 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/firefox/places.sqlite
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/firefox/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/firefox/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/firefox/user-setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:28.987390 exegol-4.3.3/exegol-docker-build/sources/assets/grc/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/grc/conf.cme
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/grc/conf.describeTicket
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/grc/conf.getgpppassword
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/grc/conf.krbrelayx
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/grc/conf.ntlmrelayx
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/grc/conf.rbcd
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/grc/conf.secretsdump
+-rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/grc/grc.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:28.987390 exegol-4.3.3/exegol-docker-build/sources/assets/logrotate/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/logrotate/exegol_vpn
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:28.987390 exegol-4.3.3/exegol-docker-build/sources/assets/netexec/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/netexec/nxc.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:28.987390 exegol-4.3.3/exegol-docker-build/sources/assets/patches/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/patches/cloudmapper.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/patches/openssl.patch
+-rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/patches/undefined-symbol-aesni-key.patch
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:28.987390 exegol-4.3.3/exegol-docker-build/sources/assets/proxychains/
+-rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/proxychains/proxychains.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:28.991390 exegol-4.3.3/exegol-docker-build/sources/assets/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/python/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:28.991390 exegol-4.3.3/exegol-docker-build/sources/assets/shells/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:29.019391 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/LDAPWordlistHarvester
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/MurMurHash
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/PassTheCert
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/Xspear
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/_init
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/aircrack-ng
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/arsenal
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/bat
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/bettercap
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/blackbird
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/blazy
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/bloodhound
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/bloodhound-py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/bloodhound-quickwin
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/bolt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/bqm
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/brakeman
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/burpsuite
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/carbon14
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/cewl
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/checksec
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/cloudfail
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/cloudmapper
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/cloudsploit
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/clusterd
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/corscanner
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/crackhound
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/crackmapexec
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/cypheroth
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/darkarmour
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/dfscoerce
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/dnschef
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/drupwn
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/eaphammer
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/emacs-nox
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/empire
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/enyx
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/evil-winrm
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/extractbitlockerkeys
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/eyewitness
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/feroxbuster
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/finalrecon
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/finduncommonshares
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/fuxploider
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/fzf
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/gdb
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/geopincer
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/ghidra
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/ghunt
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/gittools
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/gmsadumper
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/gopherus
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/gpp-decrypt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/grc
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/h2csmuggler
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/haiti
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/havoc
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/httpmethods
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/ida
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/impacket
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/infoga
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/jd-gui
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/jdwp-shellifier
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/john-the-ripper
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/joomscan
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/jwt_tool
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/kadimus
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/kraken
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/krbrelayx
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/ldaprelayscan
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/ldapsearch-ad
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/libmspack
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/libnfc-crypto1-crack
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/linkedin2username
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/linkfinder
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/lnkup
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/manspider
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/metasploit
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/mfdread
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/mobsf
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/moodlescan
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/mousejack
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/neo4j
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/netexec
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/nmap
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/noPac
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/nosqlmap
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/ntlm_theft
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/ntlmv1-multi
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/oaburl
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/oneforall
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/pass-station
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/patator
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/pcredz
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/peepdf
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/petitpotam
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/photon
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/php
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/php_filter_chain_generator
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/phpggc
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/pkinittools
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/polenum
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/powershell
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/privexchange
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/proxmark3
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/proxychains
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/pth-tools
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/pwndb
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/pwnedornot
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/pyftpdlib
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/pygpoabuse
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/pykek
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/pylaps
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/pyrit
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/python3
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/pywhisker
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/pywsus
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/recondog
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/responder
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/routersploit
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/rsactftool
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/sccmhunter
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/sccmwtf
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/shadowcoerce
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/sherlock
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/simplyemail
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/smali
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/smuggler
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/soapui
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/spiderfoot
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/ssrfmap
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/starkiller
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/symfony-exploits
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/tailscale
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/targetedkerberoast
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/teamsphisher
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/testssl
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/theharvester
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/timing_attack
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/tls-map
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/tls-scanner
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/tomcatwardeployer
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/trid
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/trilium
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/username-anarchy
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/villain
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/volatility2
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/volatility3
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/weevely
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/whatweb
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/wifite
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/wpscan
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/xmllint
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/xsel
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/xsser
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/xsstrike
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/ysoserial
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/zerologon
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/zsteg
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/bashrc
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/exegol_shells_rc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:29.091391 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/GPOddity
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/LDAPWordlistHarvester
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/MurMurHash
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/PassTheCert
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/XSpear
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/_init
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/abuseACL
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/aclpwn
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/adb
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/adidnsdump
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/aircrack-ng
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/amass
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/amber
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/androguard
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/anew
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/apksigner
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/apktool
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/arjun
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/arsenal
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/ascii
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/assetfinder
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/autorecon
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/avrdude
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/aws
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/azure-cli
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/bettercap
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/binwalk
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/blackbird
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/bloodhound
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/bloodhound-ce-py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/bloodhound-import
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/bloodhound-py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/bloodhound-quickwin
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/bloodyAD
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/bolt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/bqm
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/brakeman
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/bruteforce-luks
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/bully
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/burpsuite
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/buster
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/byp4xx
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/carbon14
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/censys
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/certipy
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/certsync
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/cewl
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/cewler
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/chainsaw
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/checksec
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/chisel
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/cloudfail
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/cloudmapper
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/cloudsplaining
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/clusterd
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/cmsmap
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/coercer
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/constellation
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/corscanner
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/cowpatty
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/crackhound
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/crackmapexec
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/crunch
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/ctf-party
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/cupp
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/curl
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/cypheroth
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/darkarmour
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/dex2jar
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/dfscoerce
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/dirb
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/dirsearch
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/divideandscan
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/dnschef
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/dnsenum
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/dnsutils
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/dnsx
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/donpapi
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/dploot
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/droopescan
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/drupwn
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/eaphammer
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/empire
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/enum4linux-ng
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/enyx
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/evil-winrm
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/exif
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/exifprobe
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/exiftool
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/exiv2
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/extractbitlockerkeys
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/eyewitness
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/faketime
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/fcrackzip
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/fdisk
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/feroxbuster
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/ffuf
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/fierce
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/finalrecon
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/findomain
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/finduncommonshares
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/firefox
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/foremost
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/freeipscanner
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/frida
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/fuxploider
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/gau
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/gdb
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/genusernames
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/geopincer
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/geowordlists
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/gf
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/ghidra
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/git-dumper
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/github-email
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/gittools
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/gmsadumper
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/gobuster
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/goldencopy
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/gomapenum
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/gopherus
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/gosecretsdump
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/goshs
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/gowitness
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/gpp-decrypt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/gqrx
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/gron
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/h2csmuggler
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/h8mail
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/hackrf
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/haiti
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/hakrawler
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/hakrevdns
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/hashcat
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/hashonymize
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/havoc
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/hcxdumptool
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/hcxtools
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/hexedit
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/holehe
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/hping3
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/httpmethods
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/httprobe
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/httpx
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/hydra
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/ida
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/ignorant
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/imagemagick
+-rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/impacket
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/infoga
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/ipinfo
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/iptables
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/jackit
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/jadx
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/jd-gui
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/jdwp-shellifier
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/john-the-ripper
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/joomscan
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/jwt_tool
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/kadimus
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/keepwn
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/kerbrute
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/kiterunner
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/kraken
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/krbrelayx
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/kubectl
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/ldapdomaindump
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/ldaprelayscan
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/ldapsearch
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/ldapsearch-ad
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/ldeep
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/legba
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/libmspack
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/libnfc
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/libnfc-crypto1-crack
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/ligolo-ng
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/linkedin2username
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/linkfinder
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/lnkup
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/lsassy
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/maigret
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/maltego
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/manspider
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/masky
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/masscan
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/mfcuk
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/mfdread
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/mfoc
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/minicom
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/mitm6
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/mobsf
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/moodlescan
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/mousejack
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/msprobe
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/naabu
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/name-that-hash
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/nasm
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/nbtscan
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/neo4j
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/netdiscover
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/netexec
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/ngrok
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/nmap
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/nmap-parse-output
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/noPac
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/notify
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/ntlm_theft
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/ntlmv1-multi
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/ntpdate
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/nuclei
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/oaburl
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/objection
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/objectwalker
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/oneforall
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/onesixtyone
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/osrframework
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/pass-station
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/patator
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/pcredz
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/pdfcrack
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/peepdf
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/petitpotam
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/phoneinfoga
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/photon
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/php_filter_chain_generator
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/phpggc
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/pkcrack
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/pkinittools
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/polenum
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/powershell
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/pp-finder
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/pre2k
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/pretender
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/prips
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/privexchange
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/prowler
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/proxmark3
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/proxychains
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/pth-tools
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/pwncat
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/pwndb
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/pwnedornot
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/pwninit
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/pyftpdlib
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/pygpoabuse
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/pykek
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/pylaps
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/pymeta
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/pypykatz
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/pyrit
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/pywerview
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/pywhisker
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/pywsus
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/radare2
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/rdesktop
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/reaver
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/recon-ng
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/recondog
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/responder
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/rlwrap
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/roastinthemiddle
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/robotstester
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/rsacracker
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/rsactftool
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/rsync
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/rtl-433
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/ruler
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/rusthound
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/rustscan
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/rustscan-ce
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/samba
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/samdump2
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/sccmhunter
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/sccmwtf
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/scout
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/scrcpy
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/scrtdnsdump
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/searchsploit
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/semgrep
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/shadowcoerce
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/shellerator
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/shuffledns
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/simplyemail
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/sipvicious_svcrack
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/sliver
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/smali
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/smartbrute
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/smbclient
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/smbmap
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/smtp-user-enum
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/smuggler
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/snmp
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/spiderfoot
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/sprayhound
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/sqlmap
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/ssh
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/ssh-audit
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/sshuttle
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/sslscan
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/sslyze
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/ssrfmap
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/steghide
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/stegolsb
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/stegosuite
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/strace
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/subfinder
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/sublist3r
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/swaks
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/symfony-exploits
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/tailscale
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/targetedkerberoast
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/tcpdump
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/teamsphisher
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/testdisk
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/testssl
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/theharvester
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/timing_attack
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/tls-map
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/tls-scanner
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/tomcatwardeployer
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/tor
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/toutatis
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/traceroute
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/trevorspray
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/trid
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/trilium
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/tshark
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/twint
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/uberfile
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/updog
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/username-anarchy
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/villain
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/volatility2
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/volatility3
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/wafw00f
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/waybackurls
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/webclientservicescanner
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/weevely
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/wfuzz
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/whatportis
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/whatweb
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/whois
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/wifite
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/windapsearch
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/wireshark
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/wpscan
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/wuzz
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/xfreerdp
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/xsrfprobe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/xsser
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/xsstrike
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/yalis
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/youtube-dl
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/ysoserial
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/zerologon
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/zipalign
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/zsteg
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/tmux.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/shells/zshrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:29.091391 exegol-4.3.3/exegol-docker-build/sources/assets/trilium/
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/trilium/config.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/assets/trilium/trilium-manager.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/build_logs_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/code_compliance_check.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:29.091391 exegol-4.3.3/exegol-docker-build/sources/dockerfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/dockerfiles/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/dockerfiles/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/dockerfiles/ad.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/dockerfiles/base.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/dockerfiles/light.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/dockerfiles/osint.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/dockerfiles/web.dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:29.099391 exegol-4.3.3/exegol-docker-build/sources/install/
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/install/common.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/install/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    68328 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/install/package_ad.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    21661 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/install/package_base.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/install/package_c2.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/install/package_cloud.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/install/package_code_analysis.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/install/package_cracking.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/install/package_crypto.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/install/package_desktop.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     5996 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/install/package_forensic.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/install/package_iot.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     9612 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/install/package_misc.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/install/package_mobile.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/install/package_most_used.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    15455 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/install/package_network.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    27488 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/install/package_osint.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/install/package_reverse.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/install/package_rfid.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/install/package_sdr.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/install/package_steganography.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/install/package_voip.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    40434 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/install/package_web.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     6276 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/install/package_wifi.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/sources/install/package_wordlists.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/web.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-16 01:32:10.000000 exegol-4.3.3/exegol-docker-build/wifi.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 01:32:29.107391 exegol-4.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-16 01:31:57.000000 exegol-4.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:32:29.107391 exegol-4.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-16 01:31:57.000000 exegol-4.3.3/tests/test_exegol.py
```

### Comparing `exegol-4.3.2/Exegol.egg-info/PKG-INFO` & `exegol-4.3.3/Exegol.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Exegol
-Version: 4.3.2
+Version: 4.3.3
 Summary: Python wrapper to use Exegol, a container based fully featured and community-driven hacking environment.
 Home-page: https://github.com/ThePorgs/Exegol
 Author: Shutdown & Dramelac
 Author-email: nwodtuhs@pm.me
 License: GNU (GPLv3)
 Project-URL: Bug Reports, https://github.com/ThePorgs/Exegol/issues
 Project-URL: Source, https://github.com/ThePorgs/Exegol
```

### Comparing `exegol-4.3.2/Exegol.egg-info/SOURCES.txt` & `exegol-4.3.3/Exegol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/LICENSE` & `exegol-4.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/PKG-INFO` & `exegol-4.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Exegol
-Version: 4.3.2
+Version: 4.3.3
 Summary: Python wrapper to use Exegol, a container based fully featured and community-driven hacking environment.
 Home-page: https://github.com/ThePorgs/Exegol
 Author: Shutdown & Dramelac
 Author-email: nwodtuhs@pm.me
 License: GNU (GPLv3)
 Project-URL: Bug Reports, https://github.com/ThePorgs/Exegol/issues
 Project-URL: Source, https://github.com/ThePorgs/Exegol
```

### Comparing `exegol-4.3.2/README.md` & `exegol-4.3.3/README.md`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol/config/ConstantConfig.py` & `exegol-4.3.3/exegol/config/ConstantConfig.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import site
 from pathlib import Path
 
 
 class ConstantConfig:
     """Constant parameters information"""
     # Exegol Version
-    version: str = "4.3.2"
+    version: str = "4.3.3"
 
     # Exegol documentation link
     documentation: str = "https://exegol.rtfd.io/"
     discord: str = "https://discord.gg/cXThyp7D6P"
     # OS Dir full root path of exegol project
     src_root_path_obj: Path = Path(__file__).parent.parent.parent.resolve()
     # Path of the Dockerfile
@@ -19,15 +19,16 @@
     entrypoint_context_path_obj: Path
     # Path of the spawn.sh
     spawn_context_path_obj: Path
     # Exegol config directory
     exegol_config_path: Path = Path().home() / ".exegol"
     # Docker Desktop for mac config file
     docker_desktop_mac_config_path = Path().home() / "Library/Group Containers/group.com.docker/settings.json"
-    docker_desktop_windows_config_path = Path().home() / "AppData/Roaming/Docker/settings.json"
+    docker_desktop_windows_config_short_path = "AppData/Roaming/Docker/settings.json"
+    docker_desktop_windows_config_path = Path().home() / docker_desktop_windows_config_short_path
     # Install mode, check if Exegol has been git cloned or installed using pip package
     git_source_installation: bool = (src_root_path_obj / '.git').is_dir()
     pip_installed: bool = src_root_path_obj.name == "site-packages"
     # Dockerhub Exegol images repository
     DOCKER_HUB: str = "hub.docker.com"  # Don't handle docker login operations
     DOCKER_REGISTRY: str = "registry-1.docker.io"  # Don't handle docker login operations
     IMAGE_NAME: str = "nwodtuhs/exegol"
```

### Comparing `exegol-4.3.2/exegol/config/DataCache.py` & `exegol-4.3.3/exegol/config/DataCache.py`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol/config/EnvInfo.py` & `exegol-4.3.3/exegol/config/EnvInfo.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import os
 import platform
 from enum import Enum
 from pathlib import Path
-from typing import Optional, Any, List
+from typing import Optional, List, Dict
 
 from exegol.config.ConstantConfig import ConstantConfig
 from exegol.utils.ExeLog import logger
 
 
 class EnvInfo:
     """Class to identify the environment in which exegol runs to adapt
@@ -146,14 +146,19 @@
 
     @classmethod
     def isMacHost(cls) -> bool:
         """Return true if macOS is detected on the host"""
         return cls.getHostOs() == cls.HostOs.MAC
 
     @classmethod
+    def isLinuxHost(cls) -> bool:
+        """Return true if Linux is detected on the host"""
+        return cls.getHostOs() == cls.HostOs.LINUX
+
+    @classmethod
     def isWaylandAvailable(cls) -> bool:
         """Return true if wayland is detected on the host"""
         return cls.getDisplayServer() == cls.DisplayServer.WAYLAND or bool(os.getenv("WAYLAND_DISPLAY"))
 
     @classmethod
     def isDockerDesktop(cls) -> bool:
         """Return true if docker desktop is used on the host"""
@@ -181,33 +186,47 @@
             return cls.HostOs.WINDOWS
         elif cls.is_mac_shell:
             return cls.HostOs.MAC
         else:
             return "Unknown"
 
     @classmethod
-    def getDockerDesktopSettings(cls) -> Optional[Any]:
+    def getDockerDesktopSettings(cls) -> Dict:
         """Applicable only for docker desktop on macos"""
         if cls.isDockerDesktop():
             if cls.__docker_desktop_resource_config is None:
                 if cls.is_mac_shell:
                     path = ConstantConfig.docker_desktop_mac_config_path
                 elif cls.is_windows_shell:
                     path = ConstantConfig.docker_desktop_windows_config_path
                 else:
-                    return None
-                    # TODO support from WSL shell
+                    # Find docker desktop config
+                    config_file = list(Path("/mnt/c/Users").glob(f"*/{ConstantConfig.docker_desktop_windows_config_short_path}"))
+                    if len(config_file) == 0:
+                        return {}
+                    else:
+                        path = config_file[0]
+                        logger.debug(f"Docker desktop config found at {path}")
                 try:
                     with open(path, 'r') as docker_desktop_config:
                         cls.__docker_desktop_resource_config = json.load(docker_desktop_config)
                 except FileNotFoundError:
                     logger.warning(f"Docker Desktop configuration file not found: '{path}'")
-                    return None
+                    return {}
             return cls.__docker_desktop_resource_config
-        return None
+        return {}
 
     @classmethod
     def getDockerDesktopResources(cls) -> List[str]:
-        config = cls.getDockerDesktopSettings()
-        if config:
-            return config.get('filesharingDirectories', [])
-        return []
+        return cls.getDockerDesktopSettings().get('filesharingDirectories', [])
+
+    @classmethod
+    def isHostNetworkAvailable(cls) -> bool:
+        if cls.isLinuxHost():
+            return True
+        elif cls.isOrbstack():
+            return True
+        elif cls.isDockerDesktop():
+            res = cls.getDockerDesktopSettings().get('hostNetworkingEnabled', False)
+            return res if res is not None else False
+        logger.warning("Unknown or not supported environment for host network mode.")
+        return False
```

### Comparing `exegol-4.3.2/exegol/config/UserConfig.py` & `exegol-4.3.3/exegol/config/UserConfig.py`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol/console/ConsoleFormat.py` & `exegol-4.3.3/exegol/console/ConsoleFormat.py`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol/console/ExegolProgress.py` & `exegol-4.3.3/exegol/console/ExegolProgress.py`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol/console/LayerTextColumn.py` & `exegol-4.3.3/exegol/console/LayerTextColumn.py`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol/console/MetaGitProgress.py` & `exegol-4.3.3/exegol/console/MetaGitProgress.py`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol/console/TUI.py` & `exegol-4.3.3/exegol/console/TUI.py`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol/console/cli/ExegolCompleter.py` & `exegol-4.3.3/exegol/console/cli/ExegolCompleter.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from exegol.config.UserConfig import UserConfig
 from exegol.manager.UpdateManager import UpdateManager
 from exegol.utils.DockerUtils import DockerUtils
 
 
 def ContainerCompleter(prefix: str, parsed_args: Namespace, **kwargs) -> Tuple[str, ...]:
     """Function to dynamically load a container list for CLI autocompletion purpose"""
-    data = [c.name for c in DockerUtils.listContainers()]
+    data = [c.name for c in DockerUtils().listContainers()]
     for obj in data:
         # filter data if needed
         if prefix and not obj.lower().startswith(prefix.lower()):
             data.remove(obj)
     return tuple(data)
```

### Comparing `exegol-4.3.2/exegol/console/cli/ParametersManager.py` & `exegol-4.3.3/exegol/console/cli/ParametersManager.py`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol/console/cli/actions/Command.py` & `exegol-4.3.3/exegol/console/cli/actions/Command.py`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol/console/cli/actions/ExegolParameters.py` & `exegol-4.3.3/exegol/console/cli/actions/ExegolParameters.py`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol/console/cli/actions/GenericParameters.py` & `exegol-4.3.3/exegol/console/cli/actions/GenericParameters.py`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol/manager/ExegolController.py` & `exegol-4.3.3/exegol/manager/ExegolController.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 try:
     import docker
     import requests
     import git
 
     from exegol.utils.ExeLog import logger, ExeLog, console
+    from exegol.utils.DockerUtils import DockerUtils
     from exegol.console.cli.ParametersManager import ParametersManager
     from exegol.console.cli.actions.ExegolParameters import Command
+    from exegol.manager.ExegolManager import ExegolManager
 except ModuleNotFoundError as e:
     print("Mandatory dependencies are missing:", e)
     print("Please install them with python3 -m pip install --upgrade -r requirements.txt")
     exit(1)
 except ImportError as e:
     print("An error occurred while loading the dependencies!")
     print()
@@ -28,14 +30,17 @@
     # (ParametersManager must be loaded from ExegolController first to load every Command subclass)
     __action: Command = ParametersManager().getCurrentAction()
 
     @classmethod
     def call_action(cls):
         """Dynamically retrieve the main function corresponding to the action selected by the user
         and execute it on the main thread"""
+        ExegolManager.print_version()
+        DockerUtils()  # Init dockerutils
+        ExegolManager.print_debug_banner()
         # Check for missing parameters
         missing_params = cls.__action.check_parameters()
         if len(missing_params) == 0:
             # Fetch main operation function
             main_action = cls.__action()
             # Execute main function
             main_action()
```

### Comparing `exegol-4.3.2/exegol/manager/ExegolManager.py` & `exegol-4.3.3/exegol/manager/ExegolManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 
     # Runtime default configuration
     __interactive_mode = False
 
     @classmethod
     def info(cls):
         """Print a list of available images and containers on the current host"""
-        ExegolManager.print_version()
         if logger.isEnabledFor(ExeLog.VERBOSE):
             logger.verbose("Listing user configurations")
             ExegolTUI.printTable(UserConfig().get_configs(), title="[not italic]:brain: [/not italic][gold3][g]User configurations[/g][/gold3]")
         if logger.isEnabledFor(ExeLog.ADVANCED):
             logger.verbose("Listing git repositories")
             ExegolTUI.printTable(UpdateManager.listGitStatus(), title="[not italic]:octopus: [/not italic][gold3][g]Project modules[/g][/gold3]")
         if bool(ParametersManager().containertag):
@@ -49,30 +48,29 @@
             container = cls.__loadOrCreateContainer(ParametersManager().containertag, must_exist=True)
             if container is not None:
                 assert type(container) is ExegolContainer
                 ExegolTUI.printContainerRecap(container)
         else:
             # Without any parameter, show all images and containers info
             # Fetch data
-            images = DockerUtils.listImages(include_version_tag=False)
-            containers = DockerUtils.listContainers()
+            images = DockerUtils().listImages(include_version_tag=False)
+            containers = DockerUtils().listContainers()
             # List and print images
             color = ConsoleFormat.getArchColor(ParametersManager().arch)
             logger.verbose(f"Listing local and remote Exegol images (filtering for architecture [{color}]{ParametersManager().arch}[/{color}])")
             ExegolTUI.printTable(images)
             # List and print containers
             logger.verbose("Listing local Exegol containers")
             logger.raw(f"[bold blue][*][/bold blue] Number of Exegol containers: {len(containers)}{os.linesep}",
                        markup=True)
             ExegolTUI.printTable(containers)
 
     @classmethod
     def start(cls):
         """Create and/or start an exegol container to finally spawn an interactive shell"""
-        ExegolManager.print_version()
         logger.info("Starting exegol")
         # Check if the first positional parameter have been supplied
         cls.__interactive_mode = not bool(ParametersManager().containertag)
         if not cls.__interactive_mode:
             logger.info("Arguments supplied with the command, skipping interactive mode")
         container = cls.__loadOrCreateContainer()
         assert container is not None and type(container) is ExegolContainer
@@ -82,15 +80,14 @@
         container.start()
         container.spawnShell()
 
     @classmethod
     def exec(cls):
         """Create and/or start an exegol container to execute a specific command.
         The execution can be seen in console output or be relayed in the background as a daemon."""
-        ExegolManager.print_version()
         logger.info("Starting exegol")
         if ParametersManager().tmp:
             container = cls.__createTmpContainer(ParametersManager().selector)
             if not ParametersManager().daemon:
                 container.exec(command=ParametersManager().exec, as_daemon=False, is_tmp=True)
                 container.stop(timeout=2)
             else:
@@ -99,61 +96,56 @@
         else:
             container = cast(ExegolContainer, cls.__loadOrCreateContainer(override_container=ParametersManager().selector))
             container.exec(command=ParametersManager().exec, as_daemon=ParametersManager().daemon)
 
     @classmethod
     def stop(cls):
         """Stop an exegol container"""
-        ExegolManager.print_version()
         logger.info("Stopping exegol")
         container = cls.__loadOrCreateContainer(multiple=True, must_exist=True)
         assert container is not None and type(container) is list
         for c in container:
             c.stop(timeout=5)
 
     @classmethod
     def restart(cls):
         """Stop and start an exegol container"""
-        ExegolManager.print_version()
         container = cast(ExegolContainer, cls.__loadOrCreateContainer(must_exist=True))
         if container:
             container.stop(timeout=5)
             container.start()
             logger.success(f"Container [green]{container.name}[/green] successfully restarted!")
             container.spawnShell()
 
     @classmethod
     def install(cls):
         """Pull or build a docker exegol image"""
-        ExegolManager.print_version()
         try:
             if not ExegolModules().isExegolResourcesReady():
                 raise CancelOperation
         except CancelOperation:
             # Error during installation, skipping operation
             logger.warning("Exegol resources have not been downloaded, the feature cannot be enabled")
         UpdateManager.updateImage(install_mode=True)
 
     @classmethod
     def update(cls):
         """Update python wrapper (git installation required) and Pull a docker exegol image"""
-        ExegolManager.print_version()
         if ParametersManager().offline_mode:
             logger.critical("It's not possible to update Exegol in offline mode. Please retry later with an internet connection.")
         if not ParametersManager().skip_git:
             UpdateManager.updateWrapper()
             UpdateManager.updateImageSource()
             UpdateManager.updateResources()
         if not ParametersManager().skip_images:
             UpdateManager.updateImage()
 
     @classmethod
     def uninstall(cls):
         """Remove an exegol image"""
-        ExegolManager.print_version()
         logger.info("Uninstalling an exegol image")
         # Set log level to verbose in order to show every image installed including the outdated.
         if not logger.isEnabledFor(ExeLog.VERBOSE):
             logger.setLevel(ExeLog.VERBOSE)
         images = cls.__loadOrInstallImage(multiple=True, must_exist=True)
         assert type(images) is list
         if len(images) == 0:
@@ -161,20 +153,19 @@
         all_name = ", ".join([x.getName() for x in images])
         if not ParametersManager().force_mode and not Confirm(
                 f"Are you sure you want to [red]permanently remove[/red] the following images? [orange3][ {all_name} ][/orange3]",
                 default=False):
             logger.error("Aborting operation.")
             return
         for img in images:
-            DockerUtils.removeImage(img)
+            DockerUtils().removeImage(img)
 
     @classmethod
     def remove(cls):
         """Remove an exegol container"""
-        ExegolManager.print_version()
         logger.info("Removing an exegol container")
         containers = cls.__loadOrCreateContainer(multiple=True, must_exist=True)
         assert type(containers) is list
         if len(containers) == 0:
             logger.error("No containers were selected. Exiting.")
             return
         all_name = ", ".join([x.name for x in containers])
@@ -183,15 +174,15 @@
                 default=False):
             logger.error("Aborting operation.")
             return
         for c in containers:
             c.remove()
             # If the image used is deprecated, it must be deleted after the removal of its container
             if c.image.isLocked() and UserConfig().auto_remove_images:
-                DockerUtils.removeImage(c.image, upgrade_mode=True)
+                DockerUtils().removeImage(c.image, upgrade_mode=True)
 
     @classmethod
     def print_version(cls):
         """Show exegol version (and context configuration on debug mode)"""
 
         logger.raw(f"[bold blue][*][/bold blue] Exegol is currently in version {UpdateManager.display_current_version()}{os.linesep}",
                    level=logging.INFO, markup=True)
@@ -206,14 +197,18 @@
         if 'a' in ConstantConfig.version:
             logger.empty_line()
             logger.warning("You are currently using an [red]Alpha[/red] version of Exegol, which may be unstable. "
                            "This version is a work in progress and bugs are expected.")
         elif 'b' in ConstantConfig.version:
             logger.empty_line()
             logger.warning("You are currently using a [orange3]Beta[/orange3] version of Exegol, which may be unstable.")
+
+    @classmethod
+    def print_debug_banner(cls):
+        """Print header debug info"""
         logger.debug(f"Pip installation: {boolFormatter(ConstantConfig.pip_installed)}")
         logger.debug(f"Git source installation: {boolFormatter(ConstantConfig.git_source_installation)}")
         logger.debug(f"Host OS: {EnvInfo.getHostOs().value} [bright_black]({EnvInfo.getDockerEngine().value})[/bright_black]")
         logger.debug(f"Arch: {EnvInfo.arch}")
         if EnvInfo.arch != EnvInfo.raw_arch:
             logger.debug(f"Raw arch: {EnvInfo.raw_arch}")
         if EnvInfo.isWindowsHost():
@@ -261,17 +256,17 @@
                     image_selection = cast(Union[Optional[ExegolImage], List[ExegolImage]],
                                            cls.__interactiveSelection(ExegolImage, multiple, must_exist))
                 else:
                     # Select image by tag name (non-interactive)
                     if multiple:
                         image_selection = []
                         for image_tag in image_tags:
-                            image_selection.append(DockerUtils.getInstalledImage(image_tag))
+                            image_selection.append(DockerUtils().getInstalledImage(image_tag))
                     else:
-                        image_selection = DockerUtils.getInstalledImage(image_tag)
+                        image_selection = DockerUtils().getInstalledImage(image_tag)
             except ObjectNotFound:
                 # ObjectNotFound is raised when the image_tag provided by the user does not match any existing image.
                 if image_tag is not None:
                     logger.warning(f"The image named '{image_tag}' has not been found.")
                 # If the user's selected image have not been found,
                 # offer to build a local image with this name
                 # (only if must_exist is not set)
@@ -338,17 +333,17 @@
                     logger.error(f"The selected image '{check_img[i].getName()}' is not installed.")
                     # If one of the image is not install, return False to restart the selection
                     return False, None
                 else:
                     # Check if the selected image is installed and install it
                     logger.warning("The selected image is not installed.")
                     # Download remote image
-                    if DockerUtils.downloadImage(check_img[i], install_mode=True):
+                    if DockerUtils().downloadImage(check_img[i], install_mode=True):
                         # Select installed image
-                        check_img[i] = DockerUtils.getInstalledImage(check_img[i].getName())
+                        check_img[i] = DockerUtils().getInstalledImage(check_img[i].getName())
                     else:
                         logger.error("This image cannot be installed.")
                         return False, None
 
         if reverse_type and not multiple:
             # Restoration of the original type
             return True, check_img[0]
@@ -377,27 +372,27 @@
                 # Try to find the corresponding container
                 if multiple:
                     cls.__container = []
                     assert container_tags is not None
                     # test each user tag
                     for container_tag in container_tags:
                         try:
-                            cls.__container.append(DockerUtils.getContainer(container_tag))
+                            cls.__container.append(DockerUtils().getContainer(container_tag))
                         except ObjectNotFound:
                             # on multi select, an object not found is not critical
                             if must_exist:
                                 # If the selected tag doesn't match any container, print an alert and continue
                                 logger.warning(f"The container named '{container_tag}' has not been found")
                             else:
                                 # If there is a multi select without must_exist flag, raise an error
                                 # because multi container creation is not supported
                                 raise NotImplemented
                 else:
                     assert container_tag is not None
-                    cls.__container = DockerUtils.getContainer(container_tag)
+                    cls.__container = DockerUtils().getContainer(container_tag)
         except (ObjectNotFound, IndexError):
             # ObjectNotFound is raised when the container_tag provided by the user does not match any existing container.
             # IndexError is raise when no container exist (raised from TUI interactive selection)
             # Create container
             if must_exist:
                 logger.warning(f"The container named '{container_tag}' has not been found")
                 return [] if multiple else None
@@ -413,18 +408,18 @@
             Union[ExegolImage, ExegolContainer, Sequence[ExegolImage], Sequence[ExegolContainer]]:
         """Interactive object selection process, depending on object_type.
         object_type can be ExegolImage or ExegolContainer."""
         object_list: Sequence[SelectableInterface]
         # Object listing depending on the type
         if object_type is ExegolContainer:
             # List all images available
-            object_list = DockerUtils.listContainers()
+            object_list = DockerUtils().listContainers()
         elif object_type is ExegolImage:
             # List all images available
-            object_list = DockerUtils.listInstalledImages() if must_exist else DockerUtils.listImages()
+            object_list = DockerUtils().listInstalledImages() if must_exist else DockerUtils().listImages()
         else:
             logger.critical("Unknown object type during interactive selection. Exiting.")
             raise Exception
         # Interactive choice with TUI
         user_selection: Union[SelectableInterface, Sequence[SelectableInterface], str]
         if multiple:
             user_selection = ExegolTUI.multipleSelectFromTable(object_list, object_type=object_type)
@@ -513,15 +508,15 @@
                 command_options = model.config.interactiveConfig(model.name)
                 ExegolTUI.printContainerRecap(model)
             logger.info(f"Command line of the configuration: "
                         f"[green]exegol start {model.name} {model.image.getName()} {' '.join(command_options)}[/green]")
             logger.info("To use exegol [orange3]without interaction[/orange3], "
                         "read CLI options with [green]exegol start -h[/green]")
 
-        container = DockerUtils.createContainer(model)
+        container = DockerUtils().createContainer(model)
         container.postCreateSetup()
         return container
 
     @classmethod
     def __createTmpContainer(cls, image_name: Optional[str] = None) -> ExegolContainer:
         """Create a temporary ExegolContainer with custom entrypoint"""
         logger.verbose("Configuring new exegol container")
@@ -537,17 +532,17 @@
         # Workspace must be disabled for temporary container because host directory is never deleted
         config.disableDefaultWorkspace()
         name = f"tmp-{binascii.b2a_hex(os.urandom(4)).decode('ascii')}"
         image: ExegolImage = cast(ExegolImage, cls.__loadOrInstallImage(override_image=image_name))
         model = ExegolContainerTemplate(name, config, image, hostname=ParametersManager().hostname)
 
         # Mount entrypoint as a volume (because in tmp mode the container is created with run instead of create method)
-        model.config.addVolume(str(ConstantConfig.entrypoint_context_path_obj), "/.exegol/entrypoint.sh", must_exist=True, read_only=True)
+        model.config.addVolume(ConstantConfig.entrypoint_context_path_obj, "/.exegol/entrypoint.sh", must_exist=True, read_only=True)
 
-        container = DockerUtils.createContainer(model, temporary=True)
+        container = DockerUtils().createContainer(model, temporary=True)
         container.postCreateSetup(is_temporary=True)
         return container
 
     @classmethod
     def __checkUselessParameters(cls):
         """Checks if the container creation parameters have not been filled in when the container already existed"""
         # Get defaults parameters
```

### Comparing `exegol-4.3.2/exegol/manager/UpdateManager.py` & `exegol-4.3.3/exegol/manager/UpdateManager.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,17 +29,17 @@
         image_args = ParametersManager().imagetag
         # Select image
         if image_args is not None and tag is None:
             tag = image_args
         if tag is None:
             # Filter for updatable images
             if install_mode:
-                available_images = [i for i in DockerUtils.listImages() if not i.isLocked()]
+                available_images = [i for i in DockerUtils().listImages() if not i.isLocked()]
             else:
-                available_images = [i for i in DockerUtils.listImages() if i.isInstall() and not i.isUpToDate() and not i.isLocked()]
+                available_images = [i for i in DockerUtils().listImages() if i.isInstall() and not i.isUpToDate() and not i.isLocked()]
                 if len(available_images) == 0:
                     logger.success("All images already installed are up to date!")
                     return None
             try:
                 # Interactive selection
                 selected_image = ExegolTUI.selectFromTable(available_images,
                                                            object_type=ExegolImage,
@@ -51,40 +51,40 @@
                     # either the user does not have internet,
                     # or the image repository has been changed and no docker image is available
                     logger.critical("Exegol can't be installed offline")
                 return None
         else:
             try:
                 # Find image by name
-                selected_image = DockerUtils.getImage(tag)
+                selected_image = DockerUtils().getImage(tag)
             except ObjectNotFound:
                 # If the image do not exist, ask to build it
                 if install_mode:
                     return cls.__askToBuild(tag)
                 else:
                     logger.error(f"Image '{tag}' was not found. If you wanted to build a local image, you can use the 'install' action instead.")
                     return None
 
         if selected_image is not None and type(selected_image) is ExegolImage:
             # Update existing ExegolImage
-            if DockerUtils.downloadImage(selected_image, install_mode):
+            if DockerUtils().downloadImage(selected_image, install_mode):
                 sync_result = None
                 # Name comparison allow detecting images without version tag
                 if not selected_image.isVersionSpecific() and selected_image.getName() != selected_image.getLatestVersionName():
                     with console.status(f"Synchronizing version tag information. Please wait.", spinner_style="blue"):
                         # Download associated version tag.
-                        sync_result = DockerUtils.downloadVersionTag(selected_image)
+                        sync_result = DockerUtils().downloadVersionTag(selected_image)
                     # Detect if an error have been triggered during the download
                     if type(sync_result) is str:
                         logger.error(f"Error while downloading version tag, {sync_result}")
                         sync_result = None
                 # if version tag have been successfully download, returning ExegolImage from docker response
                 if sync_result is not None and type(sync_result) is ExegolImage:
                     return sync_result
-                return DockerUtils.getInstalledImage(selected_image.getName())
+                return DockerUtils().getInstalledImage(selected_image.getName())
         elif type(selected_image) is str:
             # Build a new image using TUI selected name, confirmation has already been requested by TUI
             return cls.buildAndLoad(selected_image)
         else:
             # Unknown use case
             logger.critical(f"Unknown selected image type: {type(selected_image)}. Exiting.")
         return cast(Optional[ExegolImage], selected_image)
@@ -364,22 +364,22 @@
                 logger.error(f"Build profile {build_profile} not found.")
         if build_dockerfile is None:
             build_profile, build_dockerfile = cast(Tuple[str, str], ExegolTUI.selectFromList(profiles,
                                                                                              subject="a build profile",
                                                                                              title="[not italic]:dog: [/not italic][gold3]Profile[/gold3]"))
         logger.debug(f"Using {build_profile} build profile ({build_dockerfile})")
         # Docker Build
-        DockerUtils.buildImage(tag=build_name, build_profile=build_profile, build_dockerfile=build_dockerfile, dockerfile_path=build_path.as_posix())
+        DockerUtils().buildImage(tag=build_name, build_profile=build_profile, build_dockerfile=build_dockerfile, dockerfile_path=build_path.as_posix())
         return build_name
 
     @classmethod
     def buildAndLoad(cls, tag: str):
         """Build an image and load it"""
         build_name = cls.__buildSource(tag)
-        return DockerUtils.getInstalledImage(build_name)
+        return DockerUtils().getInstalledImage(build_name)
 
     @classmethod
     def listBuildProfiles(cls, profiles_path: Path = ConstantConfig.build_context_path_obj) -> Dict:
         """List every build profiles available locally
         Return a dict of options {"key = profile name": "value = dockerfile full name"}"""
         # Default stable profile
         profiles = {}
```

### Comparing `exegol-4.3.2/exegol/model/CacheModels.py` & `exegol-4.3.3/exegol/model/CacheModels.py`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol/model/ContainerConfig.py` & `exegol-4.3.3/exegol/model/ContainerConfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -384,15 +384,15 @@
                     logger.warning(f"Graphical X11 interface sharing could not be enabled: {e}")
             else:
                 logger.warning("X11 cannot be shared, only wayland, some graphical applications might not work...")
             if wayland_available:
                 try:
                     host_path = GuiUtils.getWaylandSocketPath()
                     if host_path is not None:
-                        self.addVolume(host_path.as_posix(), f"/tmp/{host_path.name}", must_exist=True)
+                        self.addVolume(host_path, f"/tmp/{host_path.name}", must_exist=True)
                         self.addEnv("XDG_SESSION_TYPE", "wayland")
                         self.addEnv("XDG_RUNTIME_DIR", "/tmp")
                         self.addEnv("WAYLAND_DISPLAY", GuiUtils.getWaylandEnv())
                         self.__gui_engine.append("Wayland")
                 except CancelOperation as e:
                     logger.warning(f"Graphical Wayland interface sharing could not be enabled: {e}")
             # TODO support pulseaudio
@@ -419,15 +419,15 @@
         if EnvInfo.is_windows_shell:
             logger.warning("Timezone sharing is not supported from a Windows shell. Skipping.")
             return
         elif EnvInfo.isMacHost():
             # On Orbstack /etc cannot be shared + we should test how Orbstack handle symlink
             # With docker desktop, symlink are resolved as full path on container creation. When tzdata is updated on the host, the container can no longer be started because the files of the previous package version are missing.
             # TODO Test if env var can be used as replacement
-            logger.warning("Timezone sharing on Mac isn't supported for instability issues. Skipping.")
+            logger.warning("Timezone sharing on Mac is not supported (for stability reasons). Skipping.")
             return
         if not self.__share_timezone:
             logger.verbose("Config: Enabling host timezones")
             # Try to share /etc/timezone (deprecated old timezone file)
             try:
                 self.addVolume("/etc/timezone", "/etc/timezone", read_only=True, must_exist=True)
                 logger.verbose("Volume was successfully added for [magenta]/etc/timezone[/magenta]")
@@ -455,20 +455,19 @@
             self.__share_timezone = False
             logger.verbose("Config: Disabling host timezones")
             self.removeVolume("/etc/timezone")
             self.removeVolume("/etc/localtime")
 
     def enableMyResources(self):
         """Procedure to enable shared volume feature"""
-        # TODO test my resources cross shell source (WSL / PSH) on Windows
         if not self.__my_resources:
             logger.verbose("Config: Enabling my-resources volume")
             self.__my_resources = True
             # Adding volume config
-            self.addVolume(str(UserConfig().my_resources_path), '/opt/my-resources', enable_sticky_group=True, force_sticky_group=True)
+            self.addVolume(UserConfig().my_resources_path, '/opt/my-resources', enable_sticky_group=True, force_sticky_group=True)
 
     def __disableMyResources(self):
         """Procedure to disable shared volume feature (Only for interactive config)"""
         if self.__my_resources:
             logger.verbose("Config: Disabling my-resources volume")
             self.__my_resources = False
             self.removeVolume(container_path='/opt/my-resources')
@@ -483,15 +482,15 @@
             except CancelOperation:
                 # Error during installation, skipping operation
                 logger.warning("Exegol resources have not been downloaded, the feature cannot be enabled")
                 return False
             logger.verbose("Config: Enabling exegol resources volume")
             self.__exegol_resources = True
             # Adding volume config
-            self.addVolume(str(UserConfig().exegol_resources_path), '/opt/resources')
+            self.addVolume(UserConfig().exegol_resources_path, '/opt/resources')
         return True
 
     def disableExegolResources(self):
         """Procedure to disable exegol resources volume feature (Only for interactive config)"""
         if self.__exegol_resources:
             logger.verbose("Config: Disabling exegol resources volume")
             self.__exegol_resources = False
@@ -678,21 +677,21 @@
         vpn_path = Path(config_path if config_path else ParametersManager().vpn).expanduser()
 
         logger.debug(f"Adding VPN from: {str(vpn_path.absolute())}")
         self.__vpn_path = vpn_path
         if vpn_path.is_file():
             self.__checkVPNConfigDNS(vpn_path)
             # Configure VPN with single file
-            self.addVolume(str(vpn_path.absolute()), "/.exegol/vpn/config/client.ovpn", read_only=True)
+            self.addVolume(vpn_path, "/.exegol/vpn/config/client.ovpn", read_only=True)
             ovpn_parameters.append("--config /.exegol/vpn/config/client.ovpn")
         else:
             # Configure VPN with directory
             logger.verbose("Folder detected for VPN configuration. "
                            "Only the first *.ovpn file will be automatically launched when the container starts.")
-            self.addVolume(str(vpn_path.absolute()), "/.exegol/vpn/config", read_only=True)
+            self.addVolume(vpn_path, "/.exegol/vpn/config", read_only=True)
             vpn_filename = None
             # Try to find the config file in order to configure the autostart command of the container
             for file in vpn_path.glob('*.ovpn'):
                 logger.info(f"Using VPN config: {file}")
                 self.__checkVPNConfigDNS(file)
                 # Get filename only to match the future container path
                 vpn_filename = file.name
@@ -708,15 +707,15 @@
         vpn_auth = None
         if input_vpn_auth is not None:
             vpn_auth = Path(input_vpn_auth).expanduser()
 
         if vpn_auth is not None:
             if vpn_auth.is_file():
                 logger.info(f"Adding VPN credentials from: {str(vpn_auth.absolute())}")
-                self.addVolume(str(vpn_auth.absolute()), "/.exegol/vpn/auth/creds.txt", read_only=True)
+                self.addVolume(vpn_auth, "/.exegol/vpn/auth/creds.txt", read_only=True)
                 ovpn_parameters.append("--auth-user-pass /.exegol/vpn/auth/creds.txt")
             else:
                 # Supply a directory instead of a file for VPN authentication is not supported.
                 logger.critical(
                     f"The path provided to the VPN connection credentials ({str(vpn_auth)}) does not lead to a file. Aborting operation.")
 
         return ' '.join(ovpn_parameters)
@@ -834,18 +833,21 @@
         """Set container's network mode, true for host, false for bridge"""
         if host_mode is None:
             host_mode = True
         if len(self.__ports) > 0 and host_mode:
             logger.warning("Host mode cannot be set with NAT ports configured. Disabling the shared network mode.")
             host_mode = False
         if EnvInfo.isDockerDesktop() and host_mode:
-            logger.warning("Docker desktop (Windows & macOS) does not support sharing of host network interfaces.")
-            logger.verbose("Official doc: https://docs.docker.com/network/host/")
-            logger.info("To share network ports between the host and exegol, use the [bright_blue]--port[/bright_blue] parameter.")
-            host_mode = False
+            if not EnvInfo.isHostNetworkAvailable():
+                logger.warning("Host network mode for Docker desktop (Windows & macOS) is not available.")
+                logger.verbose("Official doc: https://docs.docker.com/network/drivers/host/#docker-desktop")
+                logger.info("To share network ports between the host and exegol, use the [bright_blue]--port[/bright_blue] parameter.")
+                host_mode = False
+            else:
+                logger.warning("Docker desktop host network mode is enabled but in beta. Everything might not work as you expect.")
         self.__network_host = host_mode
 
     def setPrivileged(self, status: bool = True):
         """Set container as privileged"""
         logger.verbose(f"Config: Setting container privileged as {status}")
         if status:
             logger.warning("Setting container as privileged (this exposes the host to security risks)")
@@ -964,33 +966,35 @@
         return self.__share_timezone
 
     def isWorkspaceCustom(self) -> bool:
         """Return if the workspace have a custom host volume"""
         return bool(self.__workspace_custom_path)
 
     def addVolume(self,
-                  host_path: str,
+                  host_path: Union[str, Path],
                   container_path: str,
                   must_exist: bool = False,
                   read_only: bool = False,
                   enable_sticky_group: bool = False,
                   force_sticky_group: bool = False,
                   volume_type: str = 'bind'):
         """Add a volume to the container configuration.
         When the host path does not exist (neither file nor folder):
         if must_exist is set, an CancelOperation exception will be thrown.
         Otherwise, a folder will attempt to be created at the specified path.
         if set_sticky_group is set (on a Linux host), the permission setgid will be added to every folder on the volume."""
         # The creation of the directory is ignored when it is a path to the remote drive
-        if volume_type == 'bind' and not host_path.startswith("\\\\"):
-            path = Path(host_path)
-            # TODO extend to docker desktop Windows
+        if volume_type == 'bind' and not (type(host_path) is str and host_path.startswith("\\\\")):
+            path: Path = host_path.absolute() if type(host_path) is Path else Path(host_path).absolute()
+            host_path = path.as_posix()
+            # Docker Desktop for Windows based on WSL2 don't have filesystem limitation
             if EnvInfo.isMacHost():
                 # Add support for /etc
-                path_match = str(path)
+                # TODO check if path_match + replace really useful , path_match rever used
+                path_match = host_path
                 if path_match.startswith("/opt/") and EnvInfo.isOrbstack():
                     msg = f"{EnvInfo.getDockerEngine().value} cannot mount directory from [magenta]/opt/[/magenta] host path."
                     if path_match.endswith("entrypoint.sh") or path_match.endswith("spawn.sh"):
                         msg += " Your exegol installation cannot be stored under this directory."
                         logger.critical(msg)
                     raise CancelOperation(msg)
                 if path_match.startswith("/etc/"):
@@ -1001,16 +1005,16 @@
                     match = False
                     # Find a match
                     for resource in EnvInfo.getDockerDesktopResources():
                         if path_match.startswith(resource):
                             match = True
                             break
                     if not match:
-                        logger.critical(f"Bind volume from {host_path} is not possible, Docker Desktop configuration is incorrect. "
-                                        f"You need to modify the config to share a parent directory in [magenta]Docker Desktop > Preferences > Resources > File Sharing[/magenta].")
+                        logger.error(f"Bind volume from {host_path} is not possible, Docker Desktop configuration is [red]incorrect[/red].")
+                        logger.critical(f"You need to modify the [green]Docker Desktop[/green] config and [green]add[/green] this path (or the root directory) in [magenta]Docker Desktop > Preferences > Resources > File Sharing[/magenta] configuration.")
             # Choose to update fs directory perms if available and depending on user choice
             # if force_sticky_group is set, user choice is bypassed, fs will be updated.
             execute_update_fs = force_sticky_group or (enable_sticky_group and (UserConfig().auto_update_workspace_fs ^ ParametersManager().update_fs_perms))
             try:
                 if not path.exists():
                     if must_exist:
                         raise CancelOperation(f"{host_path} does not exist on your host.")
@@ -1029,15 +1033,15 @@
                 if execute_update_fs:
                     # Apply perms update
                     FsUtils.setGidPermission(path)
                 elif enable_sticky_group:
                     # If user choose not to update, print tips
                     logger.warning(f"The file sharing permissions between the container and the host will not be applied automatically by Exegol. ("
                                    f"{'Currently enabled by default according to the user config' if UserConfig().auto_update_workspace_fs else 'Use the --update-fs option to enable the feature'})")
-        mount = Mount(container_path, host_path, read_only=read_only, type=volume_type)
+        mount = Mount(container_path, str(host_path), read_only=read_only, type=volume_type)
         self.__mounts.append(mount)
 
     def removeVolume(self, host_path: Optional[str] = None, container_path: Optional[str] = None) -> bool:
         """Remove a volume from the container configuration (Only before container creation)"""
         if host_path is None and container_path is None:
             # This is a dev problem
             raise ValueError('At least one parameter must be set')
@@ -1226,34 +1230,36 @@
         """
         return self.__username
 
     # ===== User parameter parsing section =====
 
     def addRawVolume(self, volume_string):
         """Add a volume to the container configuration from raw text input.
-        Expected format is: /source/path:/target/mount:rw"""
+        Expected format is one of:
+        /source/path:/target/mount:rw
+        C:\\source\\path:/target/mount:ro
+        ./relative/path:target/mount"""
         logger.debug(f"Parsing raw volume config: {volume_string}")
-        # TODO support relative path
-        parsing = re.match(r'^((\w:)?([\\/][\w .,:\-|()&;]*)+):(([\\/][\w .,\-|()&;]*)+)(:(ro|rw))?$',
-                           volume_string)
+        parsing = re.match(r'^((\w:|\.|~)?([\\/][\w .,:\-|()&;]*)+):(([\\/][\w .,\-|()&;]*)+)(:(ro|rw))?$', volume_string)
         if parsing:
             host_path = parsing.group(1)
             container_path = parsing.group(4)
             mode = parsing.group(7)
             if mode is None or mode == "rw":
                 readonly = False
             elif mode == "ro":
                 readonly = True
             else:
                 logger.error(f"Error on volume config, mode: {mode} not recognized.")
                 readonly = False
+            full_host_path = Path(host_path).expanduser()
             logger.debug(
-                f"Adding a volume from '{host_path}' to '{container_path}' as {'readonly' if readonly else 'read/write'}")
+                f"Adding a volume from '{full_host_path.as_posix()}' to '{container_path}' as {'readonly' if readonly else 'read/write'}")
             try:
-                self.addVolume(host_path, container_path, read_only=readonly)
+                self.addVolume(full_host_path, container_path, read_only=readonly)
             except CancelOperation as e:
                 logger.error(f"The following volume couldn't be created [magenta]{volume_string}[/magenta]. {e}")
                 if not Confirm("Do you want to continue without this volume ?", False):
                     exit(0)
         else:
             logger.critical(f"Volume '{volume_string}' cannot be parsed. Exiting.")
 
@@ -1451,16 +1457,16 @@
                f"Sysctls: {self.__sysctls}{os.linesep}" \
                f"X: {self.__enable_gui}{os.linesep}" \
                f"TTY: {self.tty}{os.linesep}" \
                f"Network host: {self.getNetworkMode()}{os.linesep}" \
                f"Ports: {self.__ports}{os.linesep}" \
                f"Share timezone: {self.__share_timezone}{os.linesep}" \
                f"Common resources: {self.__my_resources}{os.linesep}" \
-               f"Envs ({len(self.__envs)}): {self.__envs}{os.linesep}" \
-               f"Labels ({len(self.__labels)}): {self.__labels}{os.linesep}" \
-               f"Shares ({len(self.__mounts)}): {self.__mounts}{os.linesep}" \
-               f"Devices ({len(self.__devices)}): {self.__devices}{os.linesep}" \
+               f"Envs ({len(self.__envs)}): {os.linesep.join(self.__envs)}{os.linesep}" \
+               f"Labels ({len(self.__labels)}): {os.linesep.join(self.__labels)}{os.linesep}" \
+               f"Shares ({len(self.__mounts)}): {os.linesep.join([str(x) for x in self.__mounts])}{os.linesep}" \
+               f"Devices ({len(self.__devices)}): {os.linesep.join(self.__devices)}{os.linesep}" \
                f"VPN: {self.getVpnName()}"
 
     def printConfig(self):
         """Log current object state, debug only"""
         logger.info(f"Current container config :{os.linesep}{self}")
```

### Comparing `exegol-4.3.2/exegol/model/ExegolContainer.py` & `exegol-4.3.3/exegol/model/ExegolContainer.py`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol/model/ExegolContainerTemplate.py` & `exegol-4.3.3/exegol/model/ExegolContainerTemplate.py`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol/model/ExegolImage.py` & `exegol-4.3.3/exegol/model/ExegolImage.py`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol/model/ExegolModules.py` & `exegol-4.3.3/exegol/model/ExegolModules.py`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol/model/MetaImages.py` & `exegol-4.3.3/exegol/model/MetaImages.py`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol/utils/ContainerLogStream.py` & `exegol-4.3.3/exegol/utils/ContainerLogStream.py`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol/utils/DataFileUtils.py` & `exegol-4.3.3/exegol/utils/DataFileUtils.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,16 +83,20 @@
                     data = yaml.safe_load(file)
                 elif self.__file_type == "json":
                     data = json.load(file)
             except yaml.parser.ParserError:
                 logger.error("Error while parsing exegol config file ! Check for syntax error.")
             except JSONDecodeError:
                 logger.error(f"Error while parsing exegol data file {self._file_path} ! Check for syntax error.")
-        self._raw_data = data
-        self._process_data()
+        if data is None:
+            logger.warning(f"Exegol was unable to load the file {self._file_path}. Restoring it to its original state.")
+            self._create_config_file()
+        else:
+            self._raw_data = data
+            self._process_data()
 
     def __load_config(self, data: dict, config_name: str, default: Union[bool, str],
                       choices: Optional[Set[str]] = None) -> Union[bool, str]:
         """
         Function to automatically load a data from a dict object. This function can handle limited choices and default value.
         If the parameter don't exist,a reset flag will be raised.
         :param data: Dict data to retrieve the value from
```

### Comparing `exegol-4.3.2/exegol/utils/DockerUtils.py` & `exegol-4.3.3/exegol/utils/DockerUtils.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,100 +18,102 @@
 from exegol.console.cli.ParametersManager import ParametersManager
 from exegol.exceptions.ExegolExceptions import ObjectNotFound
 from exegol.model.ExegolContainer import ExegolContainer
 from exegol.model.ExegolContainerTemplate import ExegolContainerTemplate
 from exegol.model.ExegolImage import ExegolImage
 from exegol.model.MetaImages import MetaImages
 from exegol.utils.ExeLog import logger, console, ExeLog
+from exegol.utils.MetaSingleton import MetaSingleton
 from exegol.utils.WebUtils import WebUtils
 
 
 # SDK Documentation : https://docker-py.readthedocs.io/en/stable/index.html
 
 
-class DockerUtils:
-    """Utility class between exegol and the Docker SDK"""
-    try:
-        # Connect Docker SDK to the local docker instance.
-        # Docker connection setting is loaded from the user environment variables.
-        __client: DockerClient = docker.from_env()
-        # Check if the docker daemon is serving linux container
-        __daemon_info = __client.info()
-        if __daemon_info.get("OSType", "linux").lower() != "linux":
-            logger.critical(
-                f"Docker daemon is not serving linux container ! Docker OS Type is: {__daemon_info.get('OSType', 'linux')}")
-        EnvInfo.initData(__daemon_info)
-    except DockerException as err:
-        if 'ConnectionRefusedError' in str(err):
-            logger.critical(f"Unable to connect to docker (from env config). Is docker running on your machine? Exiting.{os.linesep}"
-                            f"    Check documentation for help: https://exegol.readthedocs.io/en/latest/getting-started/faq.html#unable-to-connect-to-docker")
-        elif 'FileNotFoundError' in str(err):
-            logger.critical(f"Unable to connect to docker. Is docker installed on your machine? Exiting.{os.linesep}"
-                            f"    Check documentation for help: https://exegol.readthedocs.io/en/latest/getting-started/faq.html#unable-to-connect-to-docker")
-        else:
-            logger.error(err)
-            logger.critical(
-                "Unable to connect to docker (from env config). Is docker operational and accessible? on your machine? "
-                "Exiting.")
-    __images: Optional[List[ExegolImage]] = None
-    __containers: Optional[List[ExegolContainer]] = None
+class DockerUtils(metaclass=MetaSingleton):
+
+    def __init__(self):
+        """Utility class between exegol and the Docker SDK"""
+        try:
+            # Connect Docker SDK to the local docker instance.
+            # Docker connection setting is loaded from the user environment variables.
+            self.__client: DockerClient = docker.from_env()
+            # Check if the docker daemon is serving linux container
+            self.__daemon_info = self.__client.info()
+            if self.__daemon_info.get("OSType", "linux").lower() != "linux":
+                logger.critical(
+                    f"Docker daemon is not serving linux container ! Docker OS Type is: {self.__daemon_info.get('OSType', 'linux')}")
+            EnvInfo.initData(self.__daemon_info)
+        except DockerException as err:
+            if 'ConnectionRefusedError' in str(err):
+                logger.critical(f"Unable to connect to docker (from env config). Is docker running on your machine? Exiting.{os.linesep}"
+                                f"    Check documentation for help: https://exegol.readthedocs.io/en/latest/getting-started/faq.html#unable-to-connect-to-docker")
+            elif 'FileNotFoundError' in str(err):
+                logger.critical(f"Unable to connect to docker. Is docker installed on your machine? Exiting.{os.linesep}"
+                                f"    Check documentation for help: https://exegol.readthedocs.io/en/latest/getting-started/faq.html#unable-to-connect-to-docker")
+            elif 'PermissionError' in str(err):
+                logger.critical(f"Docker is installed on your host but you don't have the permission to interact with it. Exiting.{os.linesep}"
+                                f"    Check documentation for help: https://exegol.readthedocs.io/en/latest/getting-started/install.html#optional-run-exegol-with-appropriate-privileges")
+            else:
+                logger.error(err)
+                logger.critical(
+                    "Unable to connect to docker (from env config). Is docker operational and accessible? on your machine? "
+                    "Exiting.")
+        self.__images: Optional[List[ExegolImage]] = None
+        self.__containers: Optional[List[ExegolContainer]] = None
 
-    @classmethod
-    def clearCache(cls):
+    def clearCache(self):
         """Remove class's images and containers data cache
         Only needed if the list has to be updated in the same runtime at a later moment"""
-        cls.__containers = None
-        cls.__images = None
+        self.__containers = None
+        self.__images = None
 
-    @classmethod
-    def getDockerInfo(cls) -> dict:
+    def getDockerInfo(self) -> dict:
         """Fetch info from docker daemon"""
-        return cls.__daemon_info
+        return self.__daemon_info
 
     # # # Container Section # # #
 
-    @classmethod
-    def listContainers(cls) -> List[ExegolContainer]:
+    def listContainers(self) -> List[ExegolContainer]:
         """List available docker containers.
         Return a list of ExegolContainer"""
-        if cls.__containers is None:
-            cls.__containers = []
+        if self.__containers is None:
+            self.__containers = []
             try:
-                docker_containers = cls.__client.containers.list(all=True, filters={"name": "exegol-"})
+                docker_containers = self.__client.containers.list(all=True, filters={"name": "exegol-"})
             except APIError as err:
                 logger.debug(err)
                 logger.critical(err.explanation)
                 # Not reachable, critical logging will exit
                 return  # type: ignore
             except ReadTimeout:
                 logger.critical("Received a timeout error, Docker is busy... Unable to list containers, retry later.")
                 return  # type: ignore
             for container in docker_containers:
-                cls.__containers.append(ExegolContainer(container))
-        return cls.__containers
+                self.__containers.append(ExegolContainer(container))
+        return self.__containers
 
-    @classmethod
-    def createContainer(cls, model: ExegolContainerTemplate, temporary: bool = False) -> ExegolContainer:
+    def createContainer(self, model: ExegolContainerTemplate, temporary: bool = False) -> ExegolContainer:
         """Create an Exegol container from an ExegolContainerTemplate configuration.
         Return an ExegolContainer if the creation was successful."""
         logger.info("Creating new exegol container")
         model.prepare()
         logger.debug(model)
         # Preload docker volume before container creation
         for volume in model.config.getVolumes():
             if volume.get('Type', '?') == "volume":
-                docker_volume = cls.__loadDockerVolume(volume_path=volume['Source'], volume_name=volume['Target'])
+                docker_volume = self.__loadDockerVolume(volume_path=volume['Source'], volume_name=volume['Target'])
                 if docker_volume is None:
                     logger.warning(f"Error while creating docker volume '{volume['Target']}'")
         entrypoint, command = model.config.getEntrypointCommand()
         logger.debug(f"Entrypoint: {entrypoint}")
         logger.debug(f"Cmd: {command}")
         # The 'create' function must be called to create a container without starting it
         # in order to hot patch the entrypoint.sh with wrapper features (the container will be started after postCreateSetup)
-        docker_create_function = cls.__client.containers.create
+        docker_create_function = self.__client.containers.create
         docker_args = {"image": model.image.getDockerRef(),
                        "entrypoint": entrypoint,
                        "command": command,
                        "detach": True,
                        "name": model.container_name,
                        "hostname": model.config.hostname,
                        "extra_hosts": model.config.getExtraHost(),
@@ -126,28 +128,28 @@
                        "shm_size": model.config.shm_size,
                        "stdin_open": model.config.interactive,
                        "tty": model.config.tty,
                        "mounts": model.config.getVolumes(),
                        "working_dir": model.config.getWorkingDir()}
         if temporary:
             # Only the 'run' function support the "remove" parameter
-            docker_create_function = cls.__client.containers.run
+            docker_create_function = self.__client.containers.run
             docker_args["remove"] = temporary
             docker_args["auto_remove"] = temporary
         try:
             container = docker_create_function(**docker_args)
         except APIError as err:
             message = err.explanation.decode('utf-8').replace('[', '\\[') if type(err.explanation) is bytes else err.explanation
             if message is not None:
                 message = message.replace('[', '\\[')
                 logger.error(f"Docker error received: {message}")
             logger.debug(err)
             model.rollback()
             try:
-                container = cls.__client.containers.list(all=True, filters={"name": model.container_name})
+                container = self.__client.containers.list(all=True, filters={"name": model.container_name})
                 if container is not None and len(container) > 0:
                     for c in container:
                         if c.name == model.container_name:  # Search for exact match
                             container[0].remove()
                             logger.debug("Container removed")
             except Exception:
                 pass
@@ -158,64 +160,62 @@
             logger.success("Exegol container successfully created !")
         else:
             logger.critical("Unknown error while creating exegol container. Exiting.")
             # Not reachable, critical logging will exit
             return  # type: ignore
         return ExegolContainer(container, model)
 
-    @classmethod
-    def getContainer(cls, tag: str) -> ExegolContainer:
+    def getContainer(self, tag: str) -> ExegolContainer:
         """Get an ExegolContainer from tag name."""
         try:
             # Fetch potential container match from DockerSDK
-            container = cls.__client.containers.list(all=True, filters={"name": f"exegol-{tag}"})
+            container = self.__client.containers.list(all=True, filters={"name": f"exegol-{tag}"})
         except APIError as err:
             logger.debug(err)
             logger.critical(err.explanation)
             # Not reachable, critical logging will exit
             return  # type: ignore
         # Check if there is at least 1 result. If no container was found, raise ObjectNotFound.
         if container is None or len(container) == 0:
             # Handle case-insensitive OS
             if EnvInfo.isWindowsHost() or EnvInfo.isMacHost():
                 # First try to fetch the container as-is (for retroactive support with old container with uppercase characters)
                 # If the user's input didn't match any container, try to force the name in lowercase if not already tried
                 lowered_tag = tag.lower()
                 if lowered_tag != tag:
-                    return cls.getContainer(lowered_tag)
+                    return self.getContainer(lowered_tag)
             raise ObjectNotFound
         # Filter results with exact name matching
         for c in container:
             if c.name == f"exegol-{tag}":
                 # When the right container is found, select it and stop the search
                 return ExegolContainer(c)
         # When there is some close container's name,
         # docker may return some results but none of them correspond to the request.
         # In this case, ObjectNotFound is raised
         raise ObjectNotFound
 
     # # # Volumes Section # # #
 
-    @classmethod
-    def __loadDockerVolume(cls, volume_path: str, volume_name: str) -> Volume:
+    def __loadDockerVolume(self, volume_path: str, volume_name: str) -> Volume:
         """Load or create a docker volume for exegol containers
         (must be created before the container, SDK limitation)
         Return the docker volume object"""
         try:
             os.makedirs(volume_path, exist_ok=True)
         except PermissionError:
             logger.error("Unable to create the volume folder on the filesystem locally.")
             logger.critical(f"Insufficient permission to create the folder: {volume_path}")
         try:
             # Check if volume already exist
-            volume = cls.__client.volumes.get(volume_name)
+            volume = self.__client.volumes.get(volume_name)
             path = volume.attrs.get('Options', {}).get('device', '')
             if path != volume_path:
                 try:
-                    cls.__client.api.remove_volume(name=volume_name)
+                    self.__client.api.remove_volume(name=volume_name)
                     raise NotFound('Volume must be reloaded')
                 except APIError as e:
                     if e.status_code == 409:
                         logger.warning("The path of the volume specified by the user is not the same as in the existing docker volume. "
                                        "The user path will be [red]ignored[/red] as long as the docker volume already exists.")
                         logger.verbose("The volume is already used by some container and cannot be automatically removed.")
                         logger.debug(e.explanation)
@@ -225,18 +225,18 @@
                     logger.error(f"Received a timeout error, Docker is busy... Volume {volume_name} cannot be automatically removed. Please, retry later the following command:{os.linesep}"
                                  f"    [orange3]docker volume rm {volume_name}[/orange3]")
         except NotFound:
             try:
                 # Creating a docker volume bind to a host path
                 # Docker volume are more easily shared by container
                 # Docker volume can load data from container image on host's folder creation
-                volume = cls.__client.volumes.create(volume_name, driver="local",
-                                                     driver_opts={'o': 'bind',
-                                                                  'device': volume_path,
-                                                                  'type': 'none'})
+                volume = self.__client.volumes.create(volume_name, driver="local",
+                                                      driver_opts={'o': 'bind',
+                                                                   'device': volume_path,
+                                                                   'type': 'none'})
             except APIError as err:
                 logger.error(f"Error while creating docker volume '{volume_name}'.")
                 logger.debug(err)
                 logger.critical(err.explanation)
                 return None  # type: ignore
             except ReadTimeout:
                 logger.critical(f"Received a timeout error, Docker is busy... Volume {volume_name} cannot be created.")
@@ -247,47 +247,44 @@
         except ReadTimeout:
             logger.critical("Received a timeout error, Docker is busy... Unable to enumerate volume, retry later.")
             return None  # type: ignore
         return volume
 
     # # # Image Section # # #
 
-    @classmethod
-    def listImages(cls, include_version_tag: bool = False, include_locked: bool = False) -> List[ExegolImage]:
+    def listImages(self, include_version_tag: bool = False, include_locked: bool = False) -> List[ExegolImage]:
         """List available docker images.
         Return a list of ExegolImage"""
-        if cls.__images is None:
-            remote_images = cls.__listRemoteImages()
-            local_images = cls.__listLocalImages()
-            cls.__images = ExegolImage.mergeImages(remote_images, local_images)
-        result = cls.__images
+        if self.__images is None:
+            remote_images = self.__listRemoteImages()
+            local_images = self.__listLocalImages()
+            self.__images = ExegolImage.mergeImages(remote_images, local_images)
+        result = self.__images
         assert result is not None
         # Caching latest images
         DataCache().update_image_cache([img for img in result if not img.isVersionSpecific()])
         if not (logger.isEnabledFor(ExeLog.VERBOSE) or include_locked):
             # ToBeRemoved images are only shown in verbose mode
             result = [i for i in result if not i.isLocked()]
         if not include_version_tag:
             # Version specific images not installed are excluded by default
             result = [img for img in result if not img.isVersionSpecific() or img.isInstall()]
         return result
 
-    @classmethod
-    def listInstalledImages(cls) -> List[ExegolImage]:
+    def listInstalledImages(self) -> List[ExegolImage]:
         """List installed docker images.
         Return a list of ExegolImage"""
-        images = cls.listImages()
+        images = self.listImages()
         # Selecting only installed image
         return [img for img in images if img.isInstall()]
 
-    @classmethod
-    def getImage(cls, tag: str) -> ExegolImage:
+    def getImage(self, tag: str) -> ExegolImage:
         """Get an ExegolImage from tag name."""
         # Fetch every images available
-        images = cls.listImages(include_version_tag=True, include_locked=True)
+        images = self.listImages(include_version_tag=True, include_locked=True)
         match: Optional[ExegolImage] = None
         # Find a match
         for i in images:
             if i.getName() == tag:
                 # If there is a locked image keep it as default
                 if i.isLocked():
                     match = i
@@ -296,27 +293,26 @@
                     return i
         # If there is any match without lock (outdated) status, return the last outdated image found.
         if match is not None:
             return match
         # If there is no match at all, raise ObjectNotFound to handle the error
         raise ObjectNotFound
 
-    @classmethod
-    def getInstalledImage(cls, tag: str) -> ExegolImage:
+    def getInstalledImage(self, tag: str) -> ExegolImage:
         """Get an already installed ExegolImage from tag name."""
         try:
-            if cls.__images is None:
+            if self.__images is None:
                 try:
-                    docker_local_image = cls.__client.images.get(f"{ConstantConfig.IMAGE_NAME}:{tag}")
+                    docker_local_image = self.__client.images.get(f"{ConstantConfig.IMAGE_NAME}:{tag}")
                     # DockerSDK image get is an exact matching, no need to add more check
                 except APIError as err:
                     if err.status_code == 404:
                         # try to find it in recovery mode
                         logger.verbose("Unable to find your image. Trying to find in recovery mode.")
-                        recovery_images = cls.__findLocalRecoveryImages(include_untag=True)
+                        recovery_images = self.__findLocalRecoveryImages(include_untag=True)
                         match = []
                         for img in recovery_images:
                             if ExegolImage.parseAliasTagName(img) == tag:
                                 match.append(ExegolImage(docker_image=img))
                         if len(match) == 1:
                             return match[0]
                         elif len(match) > 1:
@@ -326,32 +322,31 @@
                         logger.critical(f"Error on image loading: {err}")
                         return  # type: ignore
                 except ReadTimeout:
                     logger.critical("Received a timeout error, Docker is busy... Unable to list images, retry later.")
                     return  # type: ignore
                 return ExegolImage(docker_image=docker_local_image).autoLoad()
             else:
-                for img in cls.__images:
+                for img in self.__images:
                     if img.getName() == tag:
                         if not img.isInstall() or not img.isUpToDate():
                             # Refresh local image status in case of installation/upgrade operations
-                            cls.__findImageMatch(img)
+                            self.__findImageMatch(img)
                         return img
         except ObjectNotFound:
             logger.critical(f"The desired image is not installed or do not exist ({ConstantConfig.IMAGE_NAME}:{tag}). Exiting.")
         return  # type: ignore
 
-    @classmethod
-    def __listLocalImages(cls, tag: Optional[str] = None) -> List[Image]:
+    def __listLocalImages(self, tag: Optional[str] = None) -> List[Image]:
         """List local docker images already installed.
         Return a list of docker images objects"""
         logger.debug("Fetching local image tags, digests (and other attributes)")
         try:
             image_name = ConstantConfig.IMAGE_NAME + ("" if tag is None else f":{tag}")
-            images = cls.__client.images.list(image_name, filters={"dangling": False})
+            images = self.__client.images.list(image_name, filters={"dangling": False})
         except APIError as err:
             logger.debug(err)
             logger.critical(err.explanation)
             # Not reachable, critical logging will exit
             return  # type: ignore
         except ReadTimeout:
             logger.critical("Received a timeout error, Docker is busy... Unable to list local images, retry later.")
@@ -363,35 +358,34 @@
             # len tags = 0 handle exegol <none> images (nightly image lost their tag after update)
             if len(img.attrs.get('RepoTags', [])) == 0 or \
                     ConstantConfig.IMAGE_NAME in [repo_tag.split(':')[0] for repo_tag in img.attrs.get("RepoTags", [])]:
                 result.append(img)
                 ids.add(img.id)
 
         # Try to find lost Exegol images
-        recovery_images = cls.__findLocalRecoveryImages()
+        recovery_images = self.__findLocalRecoveryImages()
         for img in recovery_images:
             # Docker can keep track of 2 images maximum with RepoTag or RepoDigests, after it's hard to track origin without labels, so this recovery option is "best effort"
             if img.id in ids:
                 # Skip image from other repo and image already found
                 logger.debug(f"Duplicate found in recovery mode! {img}")
                 continue
             else:
                 result.append(img)
                 ids.add(img.id)
         return result
 
-    @classmethod
-    def __findLocalRecoveryImages(cls, include_untag: bool = False) -> List[Image]:
+    def __findLocalRecoveryImages(self, include_untag: bool = False) -> List[Image]:
         """This method try to recovery untagged docker images.
         Set include_untag option to recover images with a valid RepoDigest (no not dangling) but without tag."""
         try:
             # Try to find lost Exegol images
-            recovery_images = cls.__client.images.list(filters={"dangling": True})
+            recovery_images = self.__client.images.list(filters={"dangling": True})
             if include_untag:
-                recovery_images += cls.__client.images.list(ConstantConfig.IMAGE_NAME, filters={"dangling": False})
+                recovery_images += self.__client.images.list(ConstantConfig.IMAGE_NAME, filters={"dangling": False})
         except APIError as err:
             logger.debug(f"Error occurred in recovery mode: {err}")
             return []
         except ReadTimeout:
             logger.critical("Received a timeout error, Docker is busy... Unable to enumerate lost images, retry later.")
             return  # type: ignore
         result = []
@@ -404,16 +398,15 @@
                 # Skip image from other repo and image already found
                 continue
             if img.labels.get('org.exegol.app', '') == "Exegol":
                 result.append(img)
                 id_list.add(img.id)
         return result
 
-    @classmethod
-    def __listRemoteImages(cls) -> List[MetaImages]:
+    def __listRemoteImages(self) -> List[MetaImages]:
         """List remote dockerhub images available.
         Return a list of ExegolImage"""
         logger.debug("Fetching remote image tags, digests and sizes")
         remote_results = []
         # Define max number of tags to download from dockerhub (in order to limit download time and discard historical versions)
         page_size = 20
         page_max = 2
@@ -439,110 +432,106 @@
                 for docker_images in docker_repo_response.get("results", []):
                     meta_image = MetaImages(docker_images)
                     remote_results.append(meta_image)
                 url = docker_repo_response.get("next")  # handle multiple page tags
         # Remove duplication (version specific / latest release)
         return remote_results
 
-    @classmethod
-    def __findImageMatch(cls, remote_image: ExegolImage):
+    def __findImageMatch(self, remote_image: ExegolImage):
         """From a Remote ExegolImage, try to find a local match (using Remote DigestID).
         This method is useful if the image repository name is also lost"""
         remote_id = remote_image.getLatestRemoteId()
         if not remote_id:
             logger.debug("Latest remote id is not available... Falling back to the current remote id.")
             remote_id = remote_image.getRemoteId()
         try:
-            docker_image = cls.__client.images.get(f"{ConstantConfig.IMAGE_NAME}@{remote_id}")
+            docker_image = self.__client.images.get(f"{ConstantConfig.IMAGE_NAME}@{remote_id}")
         except ImageNotFound:
             raise ObjectNotFound
         except ReadTimeout:
             logger.critical("Received a timeout error, Docker is busy... Unable to find a specific image, retry later.")
             return  # type: ignore
         remote_image.resetDockerImage()
         remote_image.setDockerObject(docker_image)
 
-    @classmethod
-    def downloadImage(cls, image: ExegolImage, install_mode: bool = False) -> bool:
+    def downloadImage(self, image: ExegolImage, install_mode: bool = False) -> bool:
         """Download/pull an ExegolImage"""
         if ParametersManager().offline_mode:
             logger.critical("It's not possible to download a docker image in offline mode ...")
             return False
         # Switch to install mode if the selected image is not already installed
         install_mode = install_mode or not image.isInstall()
         logger.info(f"{'Installing' if install_mode else 'Updating'} exegol image : {image.getName()}")
         name = image.updateCheck()
         if name is not None:
             logger.info(f"Pulling compressed image, starting a [cyan1]~{image.getDownloadSize()}[/cyan1] download :satellite:")
             logger.info(f"Once downloaded and uncompressed, the image will take [cyan1]~{image.getRealSizeRaw()}[/cyan1] on disk :floppy_disk:")
             logger.debug(f"Downloading {ConstantConfig.IMAGE_NAME}:{name} ({image.getArch()})")
             try:
                 ExegolTUI.downloadDockerLayer(
-                    cls.__client.api.pull(repository=ConstantConfig.IMAGE_NAME,
-                                          tag=name,
-                                          stream=True,
-                                          decode=True,
-                                          platform="linux/" + image.getArch()))
+                    self.__client.api.pull(repository=ConstantConfig.IMAGE_NAME,
+                                           tag=name,
+                                           stream=True,
+                                           decode=True,
+                                           platform="linux/" + image.getArch()))
                 logger.success(f"Image successfully {'installed' if install_mode else 'updated'}")
                 # Remove old image
                 if not install_mode and image.isInstall() and UserConfig().auto_remove_images:
-                    cls.removeImage(image, upgrade_mode=not install_mode)
+                    self.removeImage(image, upgrade_mode=not install_mode)
                 return True
             except APIError as err:
                 if err.status_code == 500:
                     logger.error(f"Error: {err.explanation}")
                     logger.error(f"Error while contacting docker registry. Aborting.")
                 elif err.status_code == 404:
                     logger.critical(f"The image has not been found on the docker registry: {err.explanation}")
                 else:
                     logger.debug(f"Error: {err}")
                     logger.critical(f"An error occurred while downloading this image: {err.explanation}")
             except ReadTimeout:
                 logger.critical(f"Received a timeout error, Docker is busy... Unable to download {name} image, retry later.")
         return False
 
-    @classmethod
-    def downloadVersionTag(cls, image: ExegolImage) -> Union[ExegolImage, str]:
+    def downloadVersionTag(self, image: ExegolImage) -> Union[ExegolImage, str]:
         """Pull a docker image for a specific version tag and return the corresponding ExegolImage"""
         if ParametersManager().offline_mode:
             logger.critical("It's not possible to download a docker image in offline mode ...")
             return ""
         try:
-            image = cls.__client.images.pull(repository=ConstantConfig.IMAGE_NAME,
-                                             tag=image.getLatestVersionName(),
-                                             platform="linux/" + image.getArch())
+            image = self.__client.images.pull(repository=ConstantConfig.IMAGE_NAME,
+                                              tag=image.getLatestVersionName(),
+                                              platform="linux/" + image.getArch())
             return ExegolImage(docker_image=image, isUpToDate=True)
         except APIError as err:
             if err.status_code == 500:
                 return f"error while contacting docker registry: {err.explanation}"
             elif err.status_code == 404:
                 return f"matching tag doesn't exist: {err.explanation}"
             else:
                 logger.debug(f"Error: {err}")
                 return f"en unknown error occurred while downloading this image : {err.explanation}"
         except ReadTimeout:
             logger.critical(f"Received a timeout error, Docker is busy... Unable to download an image tag, retry later the following command:{os.linesep}"
                             f"    [orange3]docker pull --platform linux/{image.getArch()} {ConstantConfig.IMAGE_NAME}:{image.getLatestVersionName()}[/orange3].")
             return  # type: ignore
 
-    @classmethod
-    def removeImage(cls, image: ExegolImage, upgrade_mode: bool = False) -> bool:
+    def removeImage(self, image: ExegolImage, upgrade_mode: bool = False) -> bool:
         """Remove an ExegolImage from disk"""
         tag = image.removeCheck()
         if tag is None:  # Skip removal if image is not installed locally.
             return False
         with console.status(f"Removing {'previous ' if upgrade_mode else ''}image [green]{image.getName()}[/green]...", spinner_style="blue"):
             try:
                 if not image.isVersionSpecific() and image.getInstalledVersionName() != image.getName() and not upgrade_mode:
                     # Docker can't remove multiple images at the same tag, version specific tag must be remove first
                     logger.debug(f"Removing image {image.getFullVersionName()}")
-                    if not cls.__remove_image(image.getFullVersionName()):
+                    if not self.__remove_image(image.getFullVersionName()):
                         logger.critical(f"An error occurred while removing this image : {image.getFullVersionName()}")
                 logger.debug(f"Removing image {image.getLocalId()} ({image.getFullVersionName() if upgrade_mode else image.getFullName()})")
-                if cls.__remove_image(image.getLocalId()):
+                if self.__remove_image(image.getLocalId()):
                     logger.verbose(f"Removing {'previous ' if upgrade_mode else ''}image [green]{image.getName()}[/green]...")
                     logger.success(f"{'Previous d' if upgrade_mode else 'D'}ocker image successfully removed.")
                     return True
             except APIError as err:
                 # Handle docker API error code
                 logger.verbose(err.explanation)
                 if err.status_code == 409:
@@ -554,46 +543,44 @@
                                      f"it is currently used by a container. Aborting.")
                 elif err.status_code == 404:
                     logger.error(f"This image doesn't exist locally {image.getLocalId()} ({image.getFullName()}). Aborting.")
                 else:
                     logger.critical(f"An error occurred while removing this image : {err}")
         return False
 
-    @classmethod
-    def __remove_image(cls, image_name: str) -> bool:
+    def __remove_image(self, image_name: str) -> bool:
         """
         Handle docker image removal with timeout support
         :param image_name: Name of the docker image to remove
         :return: True is removal successful and False otherwise
         """
         try:
-            cls.__client.images.remove(image_name, force=False, noprune=False)
+            self.__client.images.remove(image_name, force=False, noprune=False)
             return True
         except ReadTimeout:
             logger.warning("The deletion of the image has timeout. Docker is still processing the removal, please wait.")
             max_retry = 5
             wait_time = 5
             for i in range(5):
                 try:
-                    _ = cls.__client.images.get(image_name)
+                    _ = self.__client.images.get(image_name)
                     # DockerSDK image getter is an exact matching, no need to add more check
                 except APIError as err:
                     if err.status_code == 404:
                         return True
                     else:
                         logger.debug(f"Unexpected error after timeout: {err}")
                 except ReadTimeout:
-                    wait_time = wait_time + wait_time*i
-                    logger.info(f"Docker timeout again ({i+1}/{max_retry}). Next retry in {wait_time} seconds...")
+                    wait_time = wait_time + wait_time * i
+                    logger.info(f"Docker timeout again ({i + 1}/{max_retry}). Next retry in {wait_time} seconds...")
                     sleep(wait_time)  # Wait x seconds before retry
             logger.error(f"The deletion of the image '{image_name}' has timeout, the deletion may be incomplete.")
         return False
 
-    @classmethod
-    def buildImage(cls, tag: str, build_profile: Optional[str] = None, build_dockerfile: Optional[str] = None, dockerfile_path: str = ConstantConfig.build_context_path):
+    def buildImage(self, tag: str, build_profile: Optional[str] = None, build_dockerfile: Optional[str] = None, dockerfile_path: str = ConstantConfig.build_context_path):
         """Build a docker image from source"""
         if ParametersManager().offline_mode:
             logger.critical("It's not possible to build a docker image in offline mode. The build process need access to internet ...")
             return False
         logger.info(f"Building exegol image : {tag}")
         if build_profile is None or build_dockerfile is None:
             build_profile = "full"
@@ -604,25 +591,25 @@
         if EnvInfo.arch != ParametersManager().arch:
             logger.warning("Building an image for a different host architecture can cause unexpected problems and slowdowns!")
         try:
             # path is the directory full path where Dockerfile is.
             # tag is the name of the final build
             # dockerfile is the Dockerfile filename
             ExegolTUI.buildDockerImage(
-                cls.__client.api.build(path=dockerfile_path,
-                                       dockerfile=build_dockerfile,
-                                       tag=f"{ConstantConfig.IMAGE_NAME}:{tag}",
-                                       buildargs={"TAG": f"{build_profile}",
-                                                  "VERSION": "local",
-                                                  "BUILD_DATE": datetime.utcnow().strftime('%Y-%m-%dT%H:%M:%SZ')},
-                                       platform="linux/" + ParametersManager().arch,
-                                       rm=True,
-                                       forcerm=True,
-                                       pull=True,
-                                       decode=True))
+                self.__client.api.build(path=dockerfile_path,
+                                        dockerfile=build_dockerfile,
+                                        tag=f"{ConstantConfig.IMAGE_NAME}:{tag}",
+                                        buildargs={"TAG": f"{build_profile}",
+                                                   "VERSION": "local",
+                                                   "BUILD_DATE": datetime.utcnow().strftime('%Y-%m-%dT%H:%M:%SZ')},
+                                        platform="linux/" + ParametersManager().arch,
+                                        rm=True,
+                                        forcerm=True,
+                                        pull=True,
+                                        decode=True))
             logger.success(f"Exegol image successfully built")
         except APIError as err:
             logger.debug(f"Error: {err}")
             if err.status_code == 500:
                 logger.error(f"Error: {err.explanation}")
                 logger.error("Error while contacting docker hub. You probably don't have internet. Aborting.")
                 logger.debug(f"Error: {err}")
```

### Comparing `exegol-4.3.2/exegol/utils/ExeLog.py` & `exegol-4.3.3/exegol/utils/ExeLog.py`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol/utils/FsUtils.py` & `exegol-4.3.3/exegol/utils/FsUtils.py`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol/utils/GitUtils.py` & `exegol-4.3.3/exegol/utils/GitUtils.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
             return result
         for branch in self.__gitRemote.fetch():
             branch_parts = branch.name.split('/')
             if len(branch_parts) < 2:
                 logger.warning(f"Branch name is not correct: {branch.name}")
                 result.append(branch.name)
             else:
-                result.append(branch_parts[1])
+                result.append('/'.join(branch_parts[1:]))
         return result
 
     def safeCheck(self) -> bool:
         """Check the status of the local git repository,
         if there is pending change it is not safe to apply some operations"""
         assert self.isAvailable
         if self.__gitRepo is None or self.__gitRemote is None:
```

### Comparing `exegol-4.3.2/exegol/utils/GuiUtils.py` & `exegol-4.3.3/exegol/utils/GuiUtils.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,14 +150,15 @@
     def __checkDockerDesktopResourcesConfig() -> bool:
         """
             Check if Docker Desktop for macOS is configured correctly, allowing
             /tmp to be bind mounted into Docker containers, which is needed to
              mount /tmp/.X11-unix for display sharing.
              Return True if the configuration is correct and /tmp is part of the whitelisted resources
         """
+        # Function not used for now because the X11 socket cannot be used for now with Docker Desktop
         docker_config = EnvInfo.getDockerDesktopResources()
         logger.debug(f"Docker Desktop configuration filesharingDirectories: {docker_config}")
         return '/tmp' in docker_config
 
     @staticmethod
     def __isXQuartzInstalled() -> bool:
         return 'xquartz' in os.getenv('DISPLAY', "").lower()
```

### Comparing `exegol-4.3.2/exegol/utils/MetaSingleton.py` & `exegol-4.3.3/exegol/utils/MetaSingleton.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Generic singleton class
 from typing import Dict
 
 
+# Generic singleton class
 class MetaSingleton(type):
     """Metaclass to create a singleton class"""
     __instances: Dict[type, object] = {}
 
     def __call__(cls, *args, **kwargs) -> object:
         """Redirects each call to the current class to the corresponding single instance"""
         if cls not in MetaSingleton.__instances:
```

### Comparing `exegol-4.3.2/exegol/utils/WebUtils.py` & `exegol-4.3.3/exegol/utils/WebUtils.py`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol/utils/argParse.py` & `exegol-4.3.3/exegol/utils/argParse.py`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol/utils/imgsync/ImageScriptSync.py` & `exegol-4.3.3/exegol/utils/imgsync/ImageScriptSync.py`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol/utils/imgsync/entrypoint.sh` & `exegol-4.3.3/exegol/utils/imgsync/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol/utils/imgsync/spawn.sh` & `exegol-4.3.3/exegol/utils/imgsync/spawn.sh`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/Dockerfile` & `exegol-4.3.3/exegol-docker-build/Dockerfile`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/ad.dockerfile` & `exegol-4.3.3/exegol-docker-build/ad.dockerfile`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/light.dockerfile` & `exegol-4.3.3/exegol-docker-build/light.dockerfile`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/osint.dockerfile` & `exegol-4.3.3/exegol-docker-build/osint.dockerfile`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/bloodhound/config.json` & `exegol-4.3.3/exegol-docker-build/sources/assets/bloodhound/config.json`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/bloodhound/customqueries.json` & `exegol-4.3.3/exegol-docker-build/sources/assets/bloodhound/customqueries.json`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/bloodhound-ce/bloodhound-ce` & `exegol-4.3.3/exegol-docker-build/sources/assets/bloodhound-ce/bloodhound-ce`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/bloodhound-ce/bloodhound.config.json` & `exegol-4.3.3/exegol-docker-build/sources/assets/bloodhound-ce/bloodhound.config.json`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/burpsuite/conf.json` & `exegol-4.3.3/exegol-docker-build/sources/assets/burpsuite/conf.json`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/burpsuite/trust-ca-burp.sh` & `exegol-4.3.3/exegol-docker-build/sources/assets/burpsuite/trust-ca-burp.sh`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/desktop/Prof_XFCE_2_1.tar.gz` & `exegol-4.3.3/exegol-docker-build/sources/assets/desktop/Prof_XFCE_2_1.tar.gz`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/desktop/bin/desktop-start` & `exegol-4.3.3/exegol-docker-build/sources/assets/desktop/bin/desktop-start`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/config` & `exegol-4.3.3/exegol-docker-build/sources/assets/desktop/configuration/config`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/wallpaper.png` & `exegol-4.3.3/exegol-docker-build/sources/assets/desktop/configuration/wallpaper.png`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/wallpaper2.png` & `exegol-4.3.3/exegol-docker-build/sources/assets/desktop/configuration/wallpaper2.png`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/wallpaper3.png` & `exegol-4.3.3/exegol-docker-build/sources/assets/desktop/configuration/wallpaper3.png`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/xfce-applications.menu` & `exegol-4.3.3/exegol-docker-build/sources/assets/desktop/configuration/xfce-applications.menu`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/xfce4-desktop.xml` & `exegol-4.3.3/exegol-docker-build/sources/assets/desktop/configuration/xfce4-desktop.xml`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/xfce4-panel.xml` & `exegol-4.3.3/exegol-docker-build/sources/assets/desktop/configuration/xfce4-panel.xml`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/desktop/configuration/xsettings.xml` & `exegol-4.3.3/exegol-docker-build/sources/assets/desktop/configuration/xsettings.xml`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/desktop/exegol_logo.png` & `exegol-4.3.3/exegol-docker-build/sources/assets/desktop/exegol_logo.png`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/desktop/wallpapers/default.png` & `exegol-4.3.3/exegol-docker-build/sources/assets/desktop/wallpapers/default.png`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/desktop/wallpapers/desert.png` & `exegol-4.3.3/exegol-docker-build/sources/assets/desktop/wallpapers/desert.png`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/desktop/wallpapers/forest.png` & `exegol-4.3.3/exegol-docker-build/sources/assets/desktop/wallpapers/forest.png`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/desktop/wallpapers/glacier.png` & `exegol-4.3.3/exegol-docker-build/sources/assets/desktop/wallpapers/glacier.png`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/desktop/wallpapers/midnight.png` & `exegol-4.3.3/exegol-docker-build/sources/assets/desktop/wallpapers/midnight.png`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/desktop/wallpapers/space.png` & `exegol-4.3.3/exegol-docker-build/sources/assets/desktop/wallpapers/space.png`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/exegol/build_pipeline_tests/run_tests.py` & `exegol-4.3.3/exegol-docker-build/sources/assets/exegol/build_pipeline_tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/exegol/entrypoint.sh` & `exegol-4.3.3/exegol-docker-build/sources/assets/exegol/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/exegol/load_supported_setups.sh` & `exegol-4.3.3/exegol-docker-build/sources/assets/exegol/load_supported_setups.sh`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/README.md` & `exegol-4.3.3/exegol-docker-build/sources/assets/exegol/skel/README.md`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/bloodhound/README.md` & `exegol-4.3.3/exegol-docker-build/sources/assets/exegol/skel/bloodhound/README.md`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/load_user_setup.sh` & `exegol-4.3.3/exegol-docker-build/sources/assets/exegol/skel/load_user_setup.sh`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/exegol/skel/supported_setups.md` & `exegol-4.3.3/exegol-docker-build/sources/assets/exegol/skel/supported_setups.md`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/exegol/start.sh` & `exegol-4.3.3/exegol-docker-build/sources/assets/exegol/start.sh`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/firefox/places.sqlite` & `exegol-4.3.3/exegol-docker-build/sources/assets/firefox/places.sqlite`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/firefox/setup.py` & `exegol-4.3.3/exegol-docker-build/sources/assets/firefox/setup.py`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/firefox/user-setup.py` & `exegol-4.3.3/exegol-docker-build/sources/assets/firefox/user-setup.py`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/grc/conf.getgpppassword` & `exegol-4.3.3/exegol-docker-build/sources/assets/grc/conf.getgpppassword`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/grc/conf.ntlmrelayx` & `exegol-4.3.3/exegol-docker-build/sources/assets/grc/conf.ntlmrelayx`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/grc/conf.rbcd` & `exegol-4.3.3/exegol-docker-build/sources/assets/grc/conf.rbcd`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/grc/conf.secretsdump` & `exegol-4.3.3/exegol-docker-build/sources/assets/grc/conf.secretsdump`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/grc/grc.conf` & `exegol-4.3.3/exegol-docker-build/sources/assets/grc/grc.conf`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/patches/cloudmapper.patch` & `exegol-4.3.3/exegol-docker-build/sources/assets/patches/cloudmapper.patch`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/patches/undefined-symbol-aesni-key.patch` & `exegol-4.3.3/exegol-docker-build/sources/assets/patches/undefined-symbol-aesni-key.patch`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/proxychains/proxychains.conf` & `exegol-4.3.3/exegol-docker-build/sources/assets/proxychains/proxychains.conf`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/python/requirements.txt` & `exegol-4.3.3/exegol-docker-build/sources/assets/python/requirements.txt`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/_init` & `exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/_init`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/fzf` & `exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/fzf`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/metasploit` & `exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/metasploit`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/proxmark3` & `exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/proxmark3`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/pth-tools` & `exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/pth-tools`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/shells/aliases.d/responder` & `exegol-4.3.3/exegol-docker-build/sources/assets/shells/aliases.d/responder`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/shells/exegol_shells_rc` & `exegol-4.3.3/exegol-docker-build/sources/assets/shells/exegol_shells_rc`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/GPOddity` & `exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/GPOddity`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/bloodyAD` & `exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/bloodyAD`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/cloudsplaining` & `exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/cloudsplaining`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/crackmapexec` & `exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/crackmapexec`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/dploot` & `exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/dploot`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/hashcat` & `exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/hashcat`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/impacket` & `exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/impacket`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/kiterunner` & `exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/kiterunner`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/krbrelayx` & `exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/krbrelayx`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/netexec` & `exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/netexec`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/nmap` & `exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/nmap`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/nmap-parse-output` & `exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/nmap-parse-output`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pth-tools` & `exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/pth-tools`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/pywerview` & `exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/pywerview`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/responder` & `exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/responder`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/rsactftool` & `exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/rsactftool`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/sccmhunter` & `exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/sccmhunter`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/tls-map` & `exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/tls-map`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/volatility3` & `exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/volatility3`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/shells/history.d/wfuzz` & `exegol-4.3.3/exegol-docker-build/sources/assets/shells/history.d/wfuzz`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/shells/zshrc` & `exegol-4.3.3/exegol-docker-build/sources/assets/shells/zshrc`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/trilium/config.ini` & `exegol-4.3.3/exegol-docker-build/sources/assets/trilium/config.ini`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/assets/trilium/trilium-manager.sh` & `exegol-4.3.3/exegol-docker-build/sources/assets/trilium/trilium-manager.sh`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/build_logs_report.py` & `exegol-4.3.3/exegol-docker-build/sources/build_logs_report.py`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/code_compliance_check.py` & `exegol-4.3.3/exegol-docker-build/sources/code_compliance_check.py`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/dockerfiles/Dockerfile` & `exegol-4.3.3/exegol-docker-build/sources/dockerfiles/Dockerfile`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/dockerfiles/README.md` & `exegol-4.3.3/exegol-docker-build/sources/dockerfiles/README.md`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/dockerfiles/ad.dockerfile` & `exegol-4.3.3/exegol-docker-build/sources/dockerfiles/ad.dockerfile`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/dockerfiles/base.dockerfile` & `exegol-4.3.3/exegol-docker-build/sources/dockerfiles/base.dockerfile`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/dockerfiles/light.dockerfile` & `exegol-4.3.3/exegol-docker-build/sources/dockerfiles/light.dockerfile`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/dockerfiles/osint.dockerfile` & `exegol-4.3.3/exegol-docker-build/sources/dockerfiles/osint.dockerfile`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/dockerfiles/web.dockerfile` & `exegol-4.3.3/exegol-docker-build/sources/dockerfiles/web.dockerfile`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/install/common.sh` & `exegol-4.3.3/exegol-docker-build/sources/install/common.sh`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/install/entrypoint.sh` & `exegol-4.3.3/exegol-docker-build/sources/install/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/install/package_ad.sh` & `exegol-4.3.3/exegol-docker-build/sources/install/package_ad.sh`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/install/package_base.sh` & `exegol-4.3.3/exegol-docker-build/sources/install/package_base.sh`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/install/package_c2.sh` & `exegol-4.3.3/exegol-docker-build/sources/install/package_c2.sh`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/install/package_cloud.sh` & `exegol-4.3.3/exegol-docker-build/sources/install/package_cloud.sh`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/install/package_code_analysis.sh` & `exegol-4.3.3/exegol-docker-build/sources/install/package_code_analysis.sh`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/install/package_cracking.sh` & `exegol-4.3.3/exegol-docker-build/sources/install/package_cracking.sh`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/install/package_crypto.sh` & `exegol-4.3.3/exegol-docker-build/sources/install/package_crypto.sh`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/install/package_desktop.sh` & `exegol-4.3.3/exegol-docker-build/sources/install/package_desktop.sh`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/install/package_forensic.sh` & `exegol-4.3.3/exegol-docker-build/sources/install/package_forensic.sh`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/install/package_iot.sh` & `exegol-4.3.3/exegol-docker-build/sources/install/package_iot.sh`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/install/package_misc.sh` & `exegol-4.3.3/exegol-docker-build/sources/install/package_misc.sh`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/install/package_mobile.sh` & `exegol-4.3.3/exegol-docker-build/sources/install/package_mobile.sh`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/install/package_most_used.sh` & `exegol-4.3.3/exegol-docker-build/sources/install/package_most_used.sh`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/install/package_network.sh` & `exegol-4.3.3/exegol-docker-build/sources/install/package_network.sh`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/install/package_osint.sh` & `exegol-4.3.3/exegol-docker-build/sources/install/package_osint.sh`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/install/package_reverse.sh` & `exegol-4.3.3/exegol-docker-build/sources/install/package_reverse.sh`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/install/package_rfid.sh` & `exegol-4.3.3/exegol-docker-build/sources/install/package_rfid.sh`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/install/package_sdr.sh` & `exegol-4.3.3/exegol-docker-build/sources/install/package_sdr.sh`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/install/package_steganography.sh` & `exegol-4.3.3/exegol-docker-build/sources/install/package_steganography.sh`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/install/package_voip.sh` & `exegol-4.3.3/exegol-docker-build/sources/install/package_voip.sh`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/install/package_web.sh` & `exegol-4.3.3/exegol-docker-build/sources/install/package_web.sh`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/install/package_wifi.sh` & `exegol-4.3.3/exegol-docker-build/sources/install/package_wifi.sh`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/sources/install/package_wordlists.sh` & `exegol-4.3.3/exegol-docker-build/sources/install/package_wordlists.sh`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/web.dockerfile` & `exegol-4.3.3/exegol-docker-build/web.dockerfile`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/exegol-docker-build/wifi.dockerfile` & `exegol-4.3.3/exegol-docker-build/wifi.dockerfile`

 * *Files identical despite different names*

### Comparing `exegol-4.3.2/setup.py` & `exegol-4.3.3/setup.py`

 * *Files identical despite different names*

