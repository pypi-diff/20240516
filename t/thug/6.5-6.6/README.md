# Comparing `tmp/thug-6.5.tar.gz` & `tmp/thug-6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thug-6.5.tar", last modified: Thu Apr 11 14:03:15 2024, max compression
+gzip compressed data, was "thug-6.6.tar", last modified: Wed Apr 17 08:55:03 2024, max compression
```

## Comparing `thug-6.5.tar` & `thug-6.6.tar`

### file list

```diff
@@ -1,555 +1,547 @@
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.856458 thug-6.5/
--rw-r--r--   0 buffer    (1000) buffer    (1000)    17987 2022-11-28 09:02:06.000000 thug-6.5/LICENSE.txt
--rw-r--r--   0 buffer    (1000) buffer    (1000)      130 2023-01-12 15:47:27.000000 thug-6.5/MANIFEST.in
--rw-r--r--   0 buffer    (1000) buffer    (1000)     5613 2024-04-11 14:03:15.855458 thug-6.5/PKG-INFO
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2695 2024-01-19 09:00:07.000000 thug-6.5/README.rst
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3816 2024-04-11 13:56:54.000000 thug-6.5/pyproject.toml
--rw-r--r--   0 buffer    (1000) buffer    (1000)       38 2024-04-11 14:03:15.856458 thug-6.5/setup.cfg
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.735456 thug-6.5/thug/
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.737456 thug-6.5/thug/ActiveX/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     7458 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/ActiveX.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    47758 2024-04-11 13:56:54.000000 thug-6.5/thug/ActiveX/CLSID.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/ActiveX/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.764456 thug-6.5/thug/ActiveX/modules/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      323 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/AOLAttack.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      871 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/AcroPDF.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      610 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/AdodbRecordset.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2404 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/AdodbStream.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1275 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/AnswerWorks.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      948 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/AolAmpX.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      736 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/AolICQ.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      620 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/BaiduBar.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      498 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/BitDefender.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      360 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/CABrightStor.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      531 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/CGAgent.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      446 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/Comodo.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      652 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/ConnectAndEnterRoom.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      245 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/CreativeSoftAttack.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      408 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/DLinkMPEG.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      605 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/DPClient.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      411 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/DVRHOSTWeb.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      548 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/DirectShow.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      342 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/DivX.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1651 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/Domino.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1170 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/EnjoySAP.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      751 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/FacebookPhotoUploader.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3094 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/File.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      441 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/FileUploader.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2252 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/Folder.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      460 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/GLIEDown2.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      677 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/GatewayWeblaunch.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      383 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/Gogago.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      492 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/GomWeb.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2728 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/HPInfo.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      407 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/ICQToolbar.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      807 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/IMWebControl.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      413 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/InternetCleverSuite.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1750 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/JavaDeploymentToolkit.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      932 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/JetAudioDownloadFromMusicStore.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      368 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/Kingsoft.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      652 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/MSRICHTXT.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      411 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/MSVFP.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      457 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/MSXML2DOMDocument.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3549 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/MacrovisionFlexNet.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      295 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/MicrosoftWorks7Attack.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2119 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/MicrosoftXMLDOM.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     7787 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/MicrosoftXMLHTTP.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      430 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/Move.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      376 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/MyspaceUploader.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      520 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/NCTAudioFile2.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      972 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/NamoInstaller.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      547 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/NeoTracePro.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2210 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/NessusScanCtrl.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      945 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/OfficeOCX.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      919 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/OurgameGLWorld.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1066 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/PPlayer.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      462 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/PTZCamPanel.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      458 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/QuantumStreaming.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      447 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/QvodCtrl.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      712 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/RDSDataSpace.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2063 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/RealPlayer.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      285 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/RediffBolDownloaderAttack.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      684 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/RegistryPro.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      316 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/RisingScanner.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      412 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/RtspVaPgCtrl.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      980 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/SSReaderPdg2.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1032 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/ScriptingDictionary.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      342 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/ScriptingEncoder.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4975 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/ScriptingFileSystemObject.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1184 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/ShellApplication.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      298 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/Shockwave.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      390 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/ShockwaveFlash10.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      390 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/ShockwaveFlash11.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      390 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/ShockwaveFlash12.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      390 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/ShockwaveFlash9.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      274 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/SilverLight.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      752 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/SinaDLoader.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1165 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/SnapshotViewer.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      646 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/SonicWallNetExtenderAddRouteEntry.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      754 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/Spreadsheet.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      609 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/StormConfig.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2028 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/StormMps.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      480 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/StreamAudioChainCast.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      854 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/SymantecAppStream.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1949 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/SymantecBackupExec.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.764456 thug-6.5/thug/ActiveX/modules/System/
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.764456 thug-6.5/thug/ActiveX/modules/System/Collections/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      353 2024-04-11 13:56:54.000000 thug-6.5/thug/ActiveX/modules/System/Collections/ArrayList.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)       56 2024-04-11 13:56:54.000000 thug-6.5/thug/ActiveX/modules/System/Collections/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.765456 thug-6.5/thug/ActiveX/modules/System/IO/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      443 2024-04-11 13:56:54.000000 thug-6.5/thug/ActiveX/modules/System/IO/MemoryStream.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)       62 2024-04-11 13:56:54.000000 thug-6.5/thug/ActiveX/modules/System/IO/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.766456 thug-6.5/thug/ActiveX/modules/System/Runtime/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      134 2024-04-11 13:56:54.000000 thug-6.5/thug/ActiveX/modules/System/Runtime/Activator.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      173 2024-04-11 13:56:54.000000 thug-6.5/thug/ActiveX/modules/System/Runtime/Delegate.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.766456 thug-6.5/thug/ActiveX/modules/System/Runtime/Serialization/
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.766456 thug-6.5/thug/ActiveX/modules/System/Runtime/Serialization/Formatters/
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.767456 thug-6.5/thug/ActiveX/modules/System/Runtime/Serialization/Formatters/Binary/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      341 2024-04-11 13:56:54.000000 thug-6.5/thug/ActiveX/modules/System/Runtime/Serialization/Formatters/Binary/BinaryFormatter.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)       68 2024-04-11 13:56:54.000000 thug-6.5/thug/ActiveX/modules/System/Runtime/Serialization/Formatters/Binary/__init__.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)       50 2024-04-11 13:56:54.000000 thug-6.5/thug/ActiveX/modules/System/Runtime/Serialization/Formatters/__init__.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)       58 2024-04-11 13:56:54.000000 thug-6.5/thug/ActiveX/modules/System/Runtime/Serialization/__init__.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)       64 2024-04-11 13:56:54.000000 thug-6.5/thug/ActiveX/modules/System/Runtime/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.767456 thug-6.5/thug/ActiveX/modules/System/Security/
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.767456 thug-6.5/thug/ActiveX/modules/System/Security/Cryptography/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      323 2024-04-11 13:56:54.000000 thug-6.5/thug/ActiveX/modules/System/Security/Cryptography/FromBase64Transform.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)       76 2024-04-11 13:56:54.000000 thug-6.5/thug/ActiveX/modules/System/Security/Cryptography/__init__.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)       62 2024-04-11 13:56:54.000000 thug-6.5/thug/ActiveX/modules/System/Security/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.768456 thug-6.5/thug/ActiveX/modules/System/Text/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      388 2024-04-11 13:56:54.000000 thug-6.5/thug/ActiveX/modules/System/Text/ASCIIEncoding.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)       64 2024-04-11 13:56:54.000000 thug-6.5/thug/ActiveX/modules/System/Text/__init__.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      171 2024-04-11 13:56:54.000000 thug-6.5/thug/ActiveX/modules/System/__init__.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4792 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/TextStream.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      713 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/Toshiba.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      330 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/UUSeeUpdate.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      502 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/UniversalUpload.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1445 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/VLC.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      527 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/VisualStudioDTE80.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      493 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/VsaIDEDTE.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      493 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/VsmIDEDTE.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      815 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/WMEncProfileManager.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      132 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/WMP.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      257 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/WScriptCollection.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1279 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/WScriptExec.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1726 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/WScriptNetwork.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     8198 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/WScriptShell.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      218 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/WScriptShortcut.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      590 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/WebViewFolderIcon.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1358 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/WinNTSystemInfo.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      530 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/WinZip.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      145 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/WindowsMediaPlayer.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      921 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/XMLDOMParseError.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      888 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/XUpload.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      976 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/YahooJukebox.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      446 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/YahooMessengerCyft.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      939 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/YahooMessengerYVerInfo.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1102 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/YahooMessengerYwcvwr.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1660 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/ZenturiProgramCheckerAttack.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2079 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.768456 thug-6.5/thug/Analysis/
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/Analysis/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.768456 thug-6.5/thug/Analysis/awis/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3488 2024-01-17 12:09:54.000000 thug-6.5/thug/Analysis/awis/AWIS.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/Analysis/awis/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.769456 thug-6.5/thug/Analysis/context/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1609 2024-01-17 12:09:54.000000 thug-6.5/thug/Analysis/context/ContextAnalyzer.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/Analysis/context/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.769456 thug-6.5/thug/Analysis/favicon/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      394 2024-01-17 12:09:54.000000 thug-6.5/thug/Analysis/favicon/Favicon.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-09-11 08:32:02.000000 thug-6.5/thug/Analysis/favicon/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.770456 thug-6.5/thug/Analysis/honeyagent/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3980 2024-01-17 12:09:54.000000 thug-6.5/thug/Analysis/honeyagent/HoneyAgent.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/Analysis/honeyagent/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.770456 thug-6.5/thug/Analysis/screenshot/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1309 2024-01-17 12:09:54.000000 thug-6.5/thug/Analysis/screenshot/Screenshot.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/Analysis/screenshot/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.771456 thug-6.5/thug/Analysis/shellcode/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     8118 2024-01-17 12:09:54.000000 thug-6.5/thug/Analysis/shellcode/Shellcode.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/Analysis/shellcode/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.772456 thug-6.5/thug/Classifier/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     5394 2024-01-17 12:09:54.000000 thug-6.5/thug/Classifier/BaseClassifier.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2094 2024-01-17 12:09:54.000000 thug-6.5/thug/Classifier/CookieClassifier.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2147 2024-01-17 12:09:54.000000 thug-6.5/thug/Classifier/HTMLClassifier.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2057 2024-01-17 12:09:54.000000 thug-6.5/thug/Classifier/ImageClassifier.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1996 2024-01-17 12:09:54.000000 thug-6.5/thug/Classifier/JSClassifier.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2230 2024-01-17 12:09:54.000000 thug-6.5/thug/Classifier/SampleClassifier.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2070 2024-01-17 12:09:54.000000 thug-6.5/thug/Classifier/TextClassifier.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2318 2024-01-17 12:09:54.000000 thug-6.5/thug/Classifier/URLClassifier.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2002 2024-01-17 12:09:54.000000 thug-6.5/thug/Classifier/VBSClassifier.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/Classifier/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.781457 thug-6.5/thug/DOM/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2327 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/Alexa.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2236 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/AsyncPrefetcher.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2298 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/CCInterpreter.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      878 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/Chrome.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1302 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/ClipboardData.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      817 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/Components.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     5685 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/Console.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1113 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/Crypto.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    56116 2024-02-09 06:17:13.000000 thug-6.5/thug/DOM/DFT.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3511 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/External.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2831 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/HTMLInspector.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    10997 2024-02-22 09:16:59.000000 thug-6.5/thug/DOM/HTTPSession.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      932 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/HTTPSessionException.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3717 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/History.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3501 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/JSClass.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     8294 2024-02-09 06:17:13.000000 thug-6.5/thug/DOM/JSEngine.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4395 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/JSInspector.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     5971 2024-04-11 13:56:54.000000 thug-6.5/thug/DOM/JScriptEncode.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      752 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/LocalStorage.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4873 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/Location.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    18649 2024-02-09 06:17:13.000000 thug-6.5/thug/DOM/MIMEHandler.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      762 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/Map.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1195 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/MimeType.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4504 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/MimeTypes.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      782 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/MozConnection.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    13892 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/Navigator.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4191 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/Personality.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1231 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/Plugin.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1469 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/Plugins.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1064 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/SchemeHandler.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     5954 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/Screen.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      756 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/SessionStorage.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1775 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/Sidebar.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2830 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/Storage.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2805 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/UserProfile.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      766 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/Utils.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.782456 thug-6.5/thug/DOM/W3C/
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.788457 thug-6.5/thug/DOM/W3C/Core/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2172 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/Attr.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      266 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/CDATASection.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1245 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/CharacterData.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3760 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/ClassList.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      565 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/Comment.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1893 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/DOMException.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4988 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/DOMImplementation.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     8842 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/Document.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2422 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/DocumentFragment.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1512 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/DocumentType.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     9703 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/Element.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      458 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/Entity.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      501 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/EntityReference.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1295 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/NamedNodeMap.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    14383 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/Node.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      617 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/NodeList.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      341 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/NodeType.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      486 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/Notation.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      507 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/ProcessingInstruction.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      804 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/Text.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      939 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/__init__.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      362 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/abstractmethod.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      274 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/DOMParser.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1453 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/DOMTokenList.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.790457 thug-6.5/thug/DOM/W3C/Events/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      828 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Events/DocumentEvent.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4094 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Events/Event.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      477 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Events/EventException.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      274 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Events/EventListener.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     9365 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Events/EventTarget.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      389 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Events/HTMLEvent.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1174 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Events/MessageEvent.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2068 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Events/MouseEvent.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1557 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Events/MutationEvent.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1113 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Events/StorageEvent.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      634 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Events/UIEvent.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      628 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Events/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.791457 thug-6.5/thug/DOM/W3C/File/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2380 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/File/Blob.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1377 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/File/File.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)       74 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/File/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.813457 thug-6.5/thug/DOM/W3C/HTML/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      194 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/AudioTrackList.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      611 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/Dataset.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      374 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLAllCollection.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1878 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLAnchorElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      626 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLAppletElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      247 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLAudioElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      252 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLBRElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      289 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLBaseElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      329 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLBaseFontElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1484 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLBodyElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      561 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLButtonElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1278 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLCollection.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      265 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLDListElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      263 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLDirectoryElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      253 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLDivElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    16355 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLDocument.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      952 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLDocumentCompatibleInfo.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      412 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLDocumentCompatibleInfoCollection.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4438 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      332 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLFieldSetElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      320 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLFontElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      204 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLFormControlsCollection.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1689 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLFormElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      948 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLFrameElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      289 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLFrameSetElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      400 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLHRElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      258 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLHeadElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      257 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLHeadingElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      258 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLHtmlElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1219 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLIFrameElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1233 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLImageElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1330 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLInputElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      275 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLIsIndexElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      290 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLLIElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      366 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLLabelElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      367 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLLegendElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      532 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLLinkElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4236 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLMediaElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      264 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLMenuElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      651 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLMetaElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      292 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLModElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      373 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLOListElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2550 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLObjectElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      340 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLOptGroupElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      663 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLOptionElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      227 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLOptionsCollection.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      259 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLParagraphElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      364 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLParamElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      258 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLPreElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      253 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLQuoteElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      963 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLScriptElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1594 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLSelectElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      177 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLSpanElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      309 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLStyleElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      262 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLTableCaptionElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      893 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLTableCellElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      436 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLTableColElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4449 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLTableElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2865 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLTableRowElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2075 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLTableSectionElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1004 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLTextAreaElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      247 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLTitleElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      333 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLUListElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      654 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLVideoElement.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1042 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/TAnimateColor.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      281 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/TextTrackList.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      683 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/TimeRanges.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4769 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/__init__.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      462 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/attr_property.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      418 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/bool_property.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      463 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/form_property.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      841 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/text_property.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.813457 thug-6.5/thug/DOM/W3C/Style/
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.814457 thug-6.5/thug/DOM/W3C/Style/CSS/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1339 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Style/CSS/CSSStyleDeclaration.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      456 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Style/CSS/ElementCSSInlineStyle.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/Style/CSS/__init__.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/Style/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.814457 thug-6.5/thug/DOM/W3C/URL/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     5148 2024-02-09 06:17:13.000000 thug-6.5/thug/DOM/W3C/URL/URL.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2728 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/URL/URLSearchParams.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      104 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/URL/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.815457 thug-6.5/thug/DOM/W3C/Views/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      217 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/Views/AbstractView.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      211 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Views/DocumentView.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/Views/__init__.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)       34 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/__init__.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      365 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/w3c.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      829 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/WebStore.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    35463 2024-02-09 06:17:13.000000 thug-6.5/thug/DOM/Window.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/__init__.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4750 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/w3c_bindings.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.816457 thug-6.5/thug/Encoding/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      878 2024-01-17 12:09:54.000000 thug-6.5/thug/Encoding/Encoding.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/Encoding/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.816457 thug-6.5/thug/Java/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1109 2024-01-17 12:09:54.000000 thug-6.5/thug/Java/System.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/Java/__init__.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      763 2022-11-28 09:02:06.000000 thug-6.5/thug/Java/java.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      771 2022-11-28 09:02:06.000000 thug-6.5/thug/Java/lang.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.818457 thug-6.5/thug/Logging/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2493 2024-01-17 12:09:54.000000 thug-6.5/thug/Logging/BaseLogging.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3897 2024-01-17 12:09:54.000000 thug-6.5/thug/Logging/Features.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      902 2024-01-17 12:09:54.000000 thug-6.5/thug/Logging/LoggingModules.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4946 2024-01-17 12:09:54.000000 thug-6.5/thug/Logging/SampleLogging.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    15290 2024-02-09 06:17:13.000000 thug-6.5/thug/Logging/ThugLogging.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/Logging/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.820457 thug-6.5/thug/Logging/modules/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2479 2024-01-17 12:09:54.000000 thug-6.5/thug/Logging/modules/ElasticSearch.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1293 2024-01-17 12:09:54.000000 thug-6.5/thug/Logging/modules/ExploitGraph.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    13218 2024-01-17 12:09:54.000000 thug-6.5/thug/Logging/modules/JSON.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    10257 2024-01-17 12:09:54.000000 thug-6.5/thug/Logging/modules/Mapper.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    16005 2024-01-17 12:09:54.000000 thug-6.5/thug/Logging/modules/MongoDB.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)       47 2024-01-17 12:09:54.000000 thug-6.5/thug/Logging/modules/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.820457 thug-6.5/thug/Magic/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1592 2024-01-17 12:09:54.000000 thug-6.5/thug/Magic/Magic.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/Magic/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.820457 thug-6.5/thug/OS/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3503 2024-01-17 12:09:54.000000 thug-6.5/thug/OS/Windows.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/OS/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.821457 thug-6.5/thug/Plugins/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      956 2022-11-28 09:02:06.000000 thug-6.5/thug/Plugins/IPlugin.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3438 2024-01-17 12:09:54.000000 thug-6.5/thug/Plugins/ThugPlugins.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/Plugins/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.821457 thug-6.5/thug/Plugins/plugins/
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.822457 thug-6.5/thug/Plugins/plugins/POST-TestPlugin-999/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      878 2022-11-28 09:02:06.000000 thug-6.5/thug/Plugins/plugins/POST-TestPlugin-999/Handler.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/Plugins/plugins/POST-TestPlugin-999/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.822457 thug-6.5/thug/Plugins/plugins/PRE-TestPlugin-999/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      878 2022-11-28 09:02:06.000000 thug-6.5/thug/Plugins/plugins/PRE-TestPlugin-999/Handler.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/Plugins/plugins/PRE-TestPlugin-999/__init__.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/Plugins/plugins/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.824457 thug-6.5/thug/ThugAPI/
--rw-r--r--   0 buffer    (1000) buffer    (1000)    19217 2024-02-22 09:16:59.000000 thug-6.5/thug/ThugAPI/IThugAPI.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      787 2022-11-28 09:02:06.000000 thug-6.5/thug/ThugAPI/OpaqueFilter.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    16307 2024-02-22 09:16:59.000000 thug-6.5/thug/ThugAPI/ThugAPI.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)    10186 2024-02-22 09:16:59.000000 thug-6.5/thug/ThugAPI/ThugOpts.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4382 2024-01-17 12:09:54.000000 thug-6.5/thug/ThugAPI/ThugVulnModules.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1661 2024-01-17 12:09:54.000000 thug-6.5/thug/ThugAPI/Watchdog.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      147 2024-01-17 12:09:54.000000 thug-6.5/thug/ThugAPI/__init__.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)      341 2024-01-17 12:09:54.000000 thug-6.5/thug/ThugAPI/abstractmethod.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.825457 thug-6.5/thug/WebTracking/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3100 2024-01-17 12:09:54.000000 thug-6.5/thug/WebTracking/Cookies.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1176 2022-11-28 09:02:06.000000 thug-6.5/thug/WebTracking/WebStorage.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1594 2024-01-17 12:09:54.000000 thug-6.5/thug/WebTracking/WebTracking.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/WebTracking/__init__.py
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2203 2024-04-11 13:56:54.000000 thug-6.5/thug/__init__.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.826457 thug-6.5/thug/conf/
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.826457 thug-6.5/thug/conf/hooks/
--rw-r--r--   0 buffer    (1000) buffer    (1000)       45 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/hooks/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)      174 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/inspector.json
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.837458 thug-6.5/thug/conf/personalities/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      747 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/galaxy2chrome18.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      747 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/galaxy2chrome25.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      743 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/galaxy2chrome29.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      793 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/ipadchrome33.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      739 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/ipadchrome35.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      739 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/ipadchrome37.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      737 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/ipadchrome38.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      737 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/ipadchrome39.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      737 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/ipadchrome45.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      737 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/ipadchrome46.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      729 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/ipadchrome47.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      692 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/ipadsafari7.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      688 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/ipadsafari8.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      680 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/ipadsafari9.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      648 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/linuxchrome26.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      648 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/linuxchrome30.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      648 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/linuxchrome44.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      652 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/linuxchrome54.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      652 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/linuxchrome98.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      524 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/linuxfirefox19.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      524 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/linuxfirefox40.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      748 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/nexuschrome18.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      679 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/osx10chrome19.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      690 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/osx10chrome80.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      686 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/osx10chrome97.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      679 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/osx10safari5.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      682 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/osx11safari14.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      396 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/prefix_allocation.txt
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2851 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/win10edge20.json.review
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3826 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/win10ie110.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      782 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/win2kie60.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      915 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/win2kie80.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      686 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/win7chrome20.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      686 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/win7chrome40.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      686 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/win7chrome45.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      686 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/win7chrome49.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      579 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/win7firefox3.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3769 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/win7ie100.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3800 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/win7ie80.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3820 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/win7ie90.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      678 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/win7safari5.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      674 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/winxpchrome20.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      564 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/winxpfirefox12.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2876 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/winxpie60.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2896 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/winxpie61.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2871 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/winxpie70.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2968 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/winxpie80.json
--rw-r--r--   0 buffer    (1000) buffer    (1000)      666 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/winxpsafari5.json
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.837458 thug-6.5/thug/conf/plugins/
--rw-r--r--   0 buffer    (1000) buffer    (1000)       47 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/plugins/README
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.841457 thug-6.5/thug/conf/rules/
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.841457 thug-6.5/thug/conf/rules/cookieclassifier/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      117 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/cookieclassifier/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/cookieclassifier.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.841457 thug-6.5/thug/conf/rules/cookiefilter/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      105 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/cookiefilter/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/cookiefilter.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.841457 thug-6.5/thug/conf/rules/htmlclassifier/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      113 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/htmlclassifier/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/htmlclassifier.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.842457 thug-6.5/thug/conf/rules/htmlfilter/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      101 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/htmlfilter/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/htmlfilter.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.842457 thug-6.5/thug/conf/rules/imageclassifier/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      115 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/imageclassifier/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/imageclassifier.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.842457 thug-6.5/thug/conf/rules/imagefilter/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      103 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/imagefilter/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/imagefilter.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.842457 thug-6.5/thug/conf/rules/jsclassifier/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      245 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/jsclassifier/plugindetect.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/jsclassifier.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.843458 thug-6.5/thug/conf/rules/jsfilter/
--rw-r--r--   0 buffer    (1000) buffer    (1000)       97 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/jsfilter/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/jsfilter.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.843458 thug-6.5/thug/conf/rules/sampleclassifier/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      117 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/sampleclassifier/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/sampleclassifier.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.843458 thug-6.5/thug/conf/rules/samplefilter/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      105 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/samplefilter/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/samplefilter.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.843458 thug-6.5/thug/conf/rules/textclassifier/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      113 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/textclassifier/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/textclassifier.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.844457 thug-6.5/thug/conf/rules/textfilter/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      101 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/textfilter/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/textfilter.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.848458 thug-6.5/thug/conf/rules/urlclassifier/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      111 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlclassifier/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3005 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlclassifier/blackhole.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      418 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlclassifier/cool.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      766 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlclassifier/crimeboss.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      641 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlclassifier/critxpack.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1000 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlclassifier/fiesta.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      870 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlclassifier/g01pack.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      387 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlclassifier/impact.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      808 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlclassifier/neutrino.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      612 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlclassifier/nuclear.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      969 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlclassifier/popads.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      765 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlclassifier/redkit.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      427 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlclassifier/safepack.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      176 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlclassifier/sakura.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      478 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlclassifier/sofosfo.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)     2400 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlclassifier/styx.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      849 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlclassifier/sweetorange.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)      340 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlclassifier/tds.yar
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlclassifier.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.848458 thug-6.5/thug/conf/rules/urlfilter/
--rw-r--r--   0 buffer    (1000) buffer    (1000)       99 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlfilter/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlfilter.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.848458 thug-6.5/thug/conf/rules/vbsclassifier/
--rw-r--r--   0 buffer    (1000) buffer    (1000)      111 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/vbsclassifier/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/vbsclassifier.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.849458 thug-6.5/thug/conf/rules/vbsfilter/
--rw-r--r--   0 buffer    (1000) buffer    (1000)       99 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/vbsfilter/README
--rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/vbsfilter.yar
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.850458 thug-6.5/thug/conf/scripts/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     3837 2024-02-09 06:17:13.000000 thug-6.5/thug/conf/scripts/atob.js
--rw-r--r--   0 buffer    (1000) buffer    (1000)     1821 2024-02-09 06:17:13.000000 thug-6.5/thug/conf/scripts/btoa.js
--rw-r--r--   0 buffer    (1000) buffer    (1000)       69 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/scripts/date.js
--rw-r--r--   0 buffer    (1000) buffer    (1000)      197 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/scripts/eval.js
--rw-r--r--   0 buffer    (1000) buffer    (1000)       87 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/scripts/message-event.js
--rw-r--r--   0 buffer    (1000) buffer    (1000)      204 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/scripts/storage.js
--rw-r--r--   0 buffer    (1000) buffer    (1000)      753 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/scripts/thug.js
--rw-r--r--   0 buffer    (1000) buffer    (1000)      205 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/scripts/write.js
--rw-r--r--   0 buffer    (1000) buffer    (1000)      325 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/thug.conf
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.852458 thug-6.5/thug/thug.egg-info/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     4017 2022-12-08 08:47:59.000000 thug-6.5/thug/thug.egg-info/PKG-INFO
--rw-r--r--   0 buffer    (1000) buffer    (1000)    19264 2022-12-08 08:47:59.000000 thug-6.5/thug/thug.egg-info/SOURCES.txt
--rw-r--r--   0 buffer    (1000) buffer    (1000)        1 2022-12-08 08:47:59.000000 thug-6.5/thug/thug.egg-info/dependency_links.txt
--rw-r--r--   0 buffer    (1000) buffer    (1000)       40 2022-12-08 08:47:59.000000 thug-6.5/thug/thug.egg-info/entry_points.txt
--rw-r--r--   0 buffer    (1000) buffer    (1000)      486 2022-12-08 08:47:59.000000 thug-6.5/thug/thug.egg-info/requires.txt
--rw-r--r--   0 buffer    (1000) buffer    (1000)       91 2022-12-08 08:47:59.000000 thug-6.5/thug/thug.egg-info/top_level.txt
--rw-r--r--   0 buffer    (1000) buffer    (1000)        1 2022-12-07 11:50:03.000000 thug-6.5/thug/thug.egg-info/zip-safe
--rw-r--r--   0 buffer    (1000) buffer    (1000)    19877 2024-02-22 09:16:59.000000 thug-6.5/thug/thug.py
-drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.853458 thug-6.5/thug.egg-info/
--rw-r--r--   0 buffer    (1000) buffer    (1000)     5613 2024-04-11 14:03:15.000000 thug-6.5/thug.egg-info/PKG-INFO
--rw-r--r--   0 buffer    (1000) buffer    (1000)    17098 2024-04-11 14:03:15.000000 thug-6.5/thug.egg-info/SOURCES.txt
--rw-r--r--   0 buffer    (1000) buffer    (1000)        1 2024-04-11 14:03:15.000000 thug-6.5/thug.egg-info/dependency_links.txt
--rw-r--r--   0 buffer    (1000) buffer    (1000)       40 2024-04-11 14:03:15.000000 thug-6.5/thug.egg-info/entry_points.txt
--rw-r--r--   0 buffer    (1000) buffer    (1000)      763 2024-04-11 14:03:15.000000 thug-6.5/thug.egg-info/requires.txt
--rw-r--r--   0 buffer    (1000) buffer    (1000)       10 2024-04-11 14:03:15.000000 thug-6.5/thug.egg-info/top_level.txt
--rw-r--r--   0 buffer    (1000) buffer    (1000)        1 2024-04-11 14:03:15.000000 thug-6.5/thug.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.679699 thug-6.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    17987 2024-04-17 08:54:59.000000 thug-6.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-17 08:54:59.000000 thug-6.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-04-17 08:55:03.679699 thug-6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-17 08:54:59.000000 thug-6.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-17 08:54:59.000000 thug-6.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 08:55:03.679699 thug-6.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.603699 thug-6.6/thug/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.607699 thug-6.6/thug/ActiveX/
+-rw-r--r--   0 runner    (1001) docker     (127)     7458 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/ActiveX.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47758 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/CLSID.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.623699 thug-6.6/thug/ActiveX/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/AOLAttack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/AcroPDF.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/AdodbRecordset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/AdodbStream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/AnswerWorks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/AolAmpX.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/AolICQ.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/BaiduBar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/BitDefender.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/CABrightStor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/CGAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/Comodo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/ConnectAndEnterRoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/CreativeSoftAttack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/DLinkMPEG.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/DPClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/DVRHOSTWeb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/DirectShow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/DivX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/Domino.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/EnjoySAP.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/FacebookPhotoUploader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/File.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/FileUploader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/Folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/GLIEDown2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/GatewayWeblaunch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/Gogago.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/GomWeb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/HPInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/ICQToolbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/IMWebControl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/InternetCleverSuite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/JavaDeploymentToolkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/JetAudioDownloadFromMusicStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/Kingsoft.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/MSRICHTXT.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/MSVFP.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/MSXML2DOMDocument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/MacrovisionFlexNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/MicrosoftWorks7Attack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/MicrosoftXMLDOM.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/MicrosoftXMLHTTP.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/Move.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/MyspaceUploader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/NCTAudioFile2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/NamoInstaller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/NeoTracePro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/NessusScanCtrl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/OfficeOCX.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/OurgameGLWorld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/PPlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/PTZCamPanel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/QuantumStreaming.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/QvodCtrl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/RDSDataSpace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/RealPlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/RediffBolDownloaderAttack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/RegistryPro.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/RisingScanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/RtspVaPgCtrl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/SSReaderPdg2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/ScriptingDictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/ScriptingEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/ScriptingFileSystemObject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/ShellApplication.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/Shockwave.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/ShockwaveFlash10.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/ShockwaveFlash11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/ShockwaveFlash12.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/ShockwaveFlash9.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/SilverLight.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/SinaDLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/SnapshotViewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/SonicWallNetExtenderAddRouteEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/Spreadsheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/StormConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/StormMps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/StreamAudioChainCast.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/SymantecAppStream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/SymantecBackupExec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.623699 thug-6.6/thug/ActiveX/modules/System/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.623699 thug-6.6/thug/ActiveX/modules/System/Collections/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/System/Collections/ArrayList.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/System/Collections/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.623699 thug-6.6/thug/ActiveX/modules/System/IO/
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/System/IO/MemoryStream.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/System/IO/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.623699 thug-6.6/thug/ActiveX/modules/System/Runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/System/Runtime/Activator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/System/Runtime/Delegate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.623699 thug-6.6/thug/ActiveX/modules/System/Runtime/Serialization/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.623699 thug-6.6/thug/ActiveX/modules/System/Runtime/Serialization/Formatters/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.627699 thug-6.6/thug/ActiveX/modules/System/Runtime/Serialization/Formatters/Binary/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/System/Runtime/Serialization/Formatters/Binary/BinaryFormatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/System/Runtime/Serialization/Formatters/Binary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/System/Runtime/Serialization/Formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/System/Runtime/Serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/System/Runtime/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.627699 thug-6.6/thug/ActiveX/modules/System/Security/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.627699 thug-6.6/thug/ActiveX/modules/System/Security/Cryptography/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/System/Security/Cryptography/FromBase64Transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/System/Security/Cryptography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/System/Security/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.627699 thug-6.6/thug/ActiveX/modules/System/Text/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/System/Text/ASCIIEncoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/System/Text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/System/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/TextStream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/Toshiba.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/UUSeeUpdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/UniversalUpload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/VLC.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/VisualStudioDTE80.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/VsaIDEDTE.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/VsmIDEDTE.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/WMEncProfileManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/WMP.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/WScriptCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/WScriptExec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/WScriptNetwork.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8198 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/WScriptShell.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/WScriptShortcut.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/WebViewFolderIcon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/WinNTSystemInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/WinZip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/WindowsMediaPlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/XMLDOMParseError.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/XUpload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/YahooJukebox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/YahooMessengerCyft.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/YahooMessengerYVerInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/YahooMessengerYwcvwr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/ZenturiProgramCheckerAttack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-17 08:54:59.000000 thug-6.6/thug/ActiveX/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.627699 thug-6.6/thug/Analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:54:59.000000 thug-6.6/thug/Analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.627699 thug-6.6/thug/Analysis/awis/
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-04-17 08:54:59.000000 thug-6.6/thug/Analysis/awis/AWIS.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:54:59.000000 thug-6.6/thug/Analysis/awis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.627699 thug-6.6/thug/Analysis/context/
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-17 08:54:59.000000 thug-6.6/thug/Analysis/context/ContextAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:54:59.000000 thug-6.6/thug/Analysis/context/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.627699 thug-6.6/thug/Analysis/favicon/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-17 08:54:59.000000 thug-6.6/thug/Analysis/favicon/Favicon.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:54:59.000000 thug-6.6/thug/Analysis/favicon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.627699 thug-6.6/thug/Analysis/honeyagent/
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-17 08:54:59.000000 thug-6.6/thug/Analysis/honeyagent/HoneyAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:54:59.000000 thug-6.6/thug/Analysis/honeyagent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.627699 thug-6.6/thug/Analysis/screenshot/
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-17 08:54:59.000000 thug-6.6/thug/Analysis/screenshot/Screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:54:59.000000 thug-6.6/thug/Analysis/screenshot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.627699 thug-6.6/thug/Analysis/shellcode/
+-rw-r--r--   0 runner    (1001) docker     (127)     8118 2024-04-17 08:54:59.000000 thug-6.6/thug/Analysis/shellcode/Shellcode.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:54:59.000000 thug-6.6/thug/Analysis/shellcode/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.631699 thug-6.6/thug/Classifier/
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-04-17 08:54:59.000000 thug-6.6/thug/Classifier/BaseClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-17 08:54:59.000000 thug-6.6/thug/Classifier/CookieClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-17 08:54:59.000000 thug-6.6/thug/Classifier/HTMLClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-17 08:54:59.000000 thug-6.6/thug/Classifier/ImageClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-17 08:54:59.000000 thug-6.6/thug/Classifier/JSClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-17 08:54:59.000000 thug-6.6/thug/Classifier/SampleClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-17 08:54:59.000000 thug-6.6/thug/Classifier/TextClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-17 08:54:59.000000 thug-6.6/thug/Classifier/URLClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-17 08:54:59.000000 thug-6.6/thug/Classifier/VBSClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:54:59.000000 thug-6.6/thug/Classifier/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.635699 thug-6.6/thug/DOM/
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/Alexa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/AsyncPrefetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/CCInterpreter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/Chrome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/ClipboardData.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/Components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/Console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/Crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56116 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/DFT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/External.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/HTMLInspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10997 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/HTTPSession.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/HTTPSessionException.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/History.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/JSClass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8294 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/JSEngine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/JSInspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/JScriptEncode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/LocalStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/Location.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18649 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/MIMEHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/Map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/MimeType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/MimeTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/MozConnection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13892 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/Navigator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/Personality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/Plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/Plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/SchemeHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/Screen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/SessionStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/Sidebar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/Storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/UserProfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/Utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.635699 thug-6.6/thug/DOM/W3C/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.639699 thug-6.6/thug/DOM/W3C/Core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Core/Attr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Core/CDATASection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Core/CharacterData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Core/ClassList.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Core/Comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Core/DOMException.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Core/DOMImplementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8842 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Core/Document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Core/DocumentFragment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Core/DocumentType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9703 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Core/Element.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Core/Entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Core/EntityReference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Core/NamedNodeMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14383 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Core/Node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Core/NodeList.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Core/NodeType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Core/Notation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Core/ProcessingInstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Core/Text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Core/abstractmethod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/DOMParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/DOMTokenList.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.643699 thug-6.6/thug/DOM/W3C/Events/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Events/DocumentEvent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Events/Event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Events/EventException.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Events/EventListener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9365 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Events/EventTarget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Events/HTMLEvent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Events/MessageEvent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Events/MouseEvent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Events/MutationEvent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Events/StorageEvent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Events/UIEvent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Events/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.643699 thug-6.6/thug/DOM/W3C/File/
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/File/Blob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/File/File.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/File/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.651699 thug-6.6/thug/DOM/W3C/HTML/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/AudioTrackList.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/Dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLAllCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLAnchorElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLAppletElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLAudioElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLBRElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLBaseElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLBaseFontElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLBodyElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLButtonElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLDListElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLDirectoryElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLDivElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16355 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLDocument.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLDocumentCompatibleInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLDocumentCompatibleInfoCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLFieldSetElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLFontElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLFormControlsCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLFormElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLFrameElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLFrameSetElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLHRElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLHeadElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLHeadingElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLHtmlElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLIFrameElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLImageElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLInputElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLIsIndexElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLLIElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLLabelElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLLegendElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLLinkElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLMediaElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLMenuElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLMetaElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLModElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLOListElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLObjectElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLOptGroupElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLOptionElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLOptionsCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLParagraphElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLParamElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLPreElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLQuoteElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLScriptElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLSelectElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLSpanElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLStyleElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLTableCaptionElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLTableCellElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLTableColElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLTableElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLTableRowElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLTableSectionElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLTextAreaElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLTitleElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLUListElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/HTMLVideoElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/TAnimateColor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/TextTrackList.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/TimeRanges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/attr_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/bool_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/form_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/HTML/text_property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.651699 thug-6.6/thug/DOM/W3C/Style/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.655699 thug-6.6/thug/DOM/W3C/Style/CSS/
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Style/CSS/CSSStyleDeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Style/CSS/ElementCSSInlineStyle.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Style/CSS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Style/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.655699 thug-6.6/thug/DOM/W3C/URL/
+-rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/URL/URL.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/URL/URLSearchParams.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/URL/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.655699 thug-6.6/thug/DOM/W3C/Views/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Views/AbstractView.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Views/DocumentView.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/Views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/W3C/w3c.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/WebStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35463 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/Window.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-04-17 08:54:59.000000 thug-6.6/thug/DOM/w3c_bindings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.655699 thug-6.6/thug/Encoding/
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-17 08:54:59.000000 thug-6.6/thug/Encoding/Encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:54:59.000000 thug-6.6/thug/Encoding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.655699 thug-6.6/thug/Java/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-17 08:54:59.000000 thug-6.6/thug/Java/System.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:54:59.000000 thug-6.6/thug/Java/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-17 08:54:59.000000 thug-6.6/thug/Java/java.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-17 08:54:59.000000 thug-6.6/thug/Java/lang.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.655699 thug-6.6/thug/Logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-17 08:54:59.000000 thug-6.6/thug/Logging/BaseLogging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-17 08:54:59.000000 thug-6.6/thug/Logging/Features.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-17 08:54:59.000000 thug-6.6/thug/Logging/LoggingModules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-04-17 08:54:59.000000 thug-6.6/thug/Logging/SampleLogging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15290 2024-04-17 08:54:59.000000 thug-6.6/thug/Logging/ThugLogging.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:54:59.000000 thug-6.6/thug/Logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.655699 thug-6.6/thug/Logging/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-17 08:54:59.000000 thug-6.6/thug/Logging/modules/ElasticSearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-17 08:54:59.000000 thug-6.6/thug/Logging/modules/ExploitGraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13218 2024-04-17 08:54:59.000000 thug-6.6/thug/Logging/modules/JSON.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10257 2024-04-17 08:54:59.000000 thug-6.6/thug/Logging/modules/Mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16005 2024-04-17 08:54:59.000000 thug-6.6/thug/Logging/modules/MongoDB.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-17 08:54:59.000000 thug-6.6/thug/Logging/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.659699 thug-6.6/thug/Magic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-17 08:54:59.000000 thug-6.6/thug/Magic/Magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:54:59.000000 thug-6.6/thug/Magic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.659699 thug-6.6/thug/OS/
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-04-17 08:54:59.000000 thug-6.6/thug/OS/Windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:54:59.000000 thug-6.6/thug/OS/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.659699 thug-6.6/thug/Plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-17 08:54:59.000000 thug-6.6/thug/Plugins/IPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-17 08:54:59.000000 thug-6.6/thug/Plugins/ThugPlugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:54:59.000000 thug-6.6/thug/Plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.659699 thug-6.6/thug/Plugins/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.659699 thug-6.6/thug/Plugins/plugins/POST-TestPlugin-999/
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-17 08:54:59.000000 thug-6.6/thug/Plugins/plugins/POST-TestPlugin-999/Handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:54:59.000000 thug-6.6/thug/Plugins/plugins/POST-TestPlugin-999/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.659699 thug-6.6/thug/Plugins/plugins/PRE-TestPlugin-999/
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-17 08:54:59.000000 thug-6.6/thug/Plugins/plugins/PRE-TestPlugin-999/Handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:54:59.000000 thug-6.6/thug/Plugins/plugins/PRE-TestPlugin-999/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:54:59.000000 thug-6.6/thug/Plugins/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.659699 thug-6.6/thug/ThugAPI/
+-rw-r--r--   0 runner    (1001) docker     (127)    19217 2024-04-17 08:54:59.000000 thug-6.6/thug/ThugAPI/IThugAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-17 08:54:59.000000 thug-6.6/thug/ThugAPI/OpaqueFilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16307 2024-04-17 08:54:59.000000 thug-6.6/thug/ThugAPI/ThugAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10186 2024-04-17 08:54:59.000000 thug-6.6/thug/ThugAPI/ThugOpts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-04-17 08:54:59.000000 thug-6.6/thug/ThugAPI/ThugVulnModules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-17 08:54:59.000000 thug-6.6/thug/ThugAPI/Watchdog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-17 08:54:59.000000 thug-6.6/thug/ThugAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-17 08:54:59.000000 thug-6.6/thug/ThugAPI/abstractmethod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.659699 thug-6.6/thug/WebTracking/
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-17 08:54:59.000000 thug-6.6/thug/WebTracking/Cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-17 08:54:59.000000 thug-6.6/thug/WebTracking/WebStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-17 08:54:59.000000 thug-6.6/thug/WebTracking/WebTracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:54:59.000000 thug-6.6/thug/WebTracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-17 08:54:59.000000 thug-6.6/thug/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.659699 thug-6.6/thug/conf/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.659699 thug-6.6/thug/conf/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/hooks/README
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/inspector.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.667699 thug-6.6/thug/conf/personalities/
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/galaxy2chrome18.json
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/galaxy2chrome25.json
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/galaxy2chrome29.json
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/ipadchrome33.json
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/ipadchrome35.json
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/ipadchrome37.json
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/ipadchrome38.json
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/ipadchrome39.json
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/ipadchrome45.json
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/ipadchrome46.json
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/ipadchrome47.json
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/ipadsafari7.json
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/ipadsafari8.json
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/ipadsafari9.json
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/linuxchrome26.json
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/linuxchrome30.json
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/linuxchrome44.json
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/linuxchrome54.json
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/linuxchrome98.json
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/linuxfirefox19.json
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/linuxfirefox40.json
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/nexuschrome18.json
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/osx10chrome19.json
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/osx10chrome80.json
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/osx10chrome97.json
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/osx10safari5.json
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/osx11safari14.json
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/prefix_allocation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/win10edge20.json.review
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/win10ie110.json
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/win2kie60.json
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/win2kie80.json
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/win7chrome20.json
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/win7chrome40.json
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/win7chrome45.json
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/win7chrome49.json
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/win7firefox3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/win7ie100.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/win7ie80.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/win7ie90.json
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/win7safari5.json
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/winxpchrome20.json
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/winxpfirefox12.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/winxpie60.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/winxpie61.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/winxpie70.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/winxpie80.json
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/personalities/winxpsafari5.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.667699 thug-6.6/thug/conf/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/plugins/README
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.671699 thug-6.6/thug/conf/rules/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.671699 thug-6.6/thug/conf/rules/cookieclassifier/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/cookieclassifier/README
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/cookieclassifier.yar
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.671699 thug-6.6/thug/conf/rules/cookiefilter/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/cookiefilter/README
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/cookiefilter.yar
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.671699 thug-6.6/thug/conf/rules/htmlclassifier/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/htmlclassifier/README
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/htmlclassifier.yar
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.671699 thug-6.6/thug/conf/rules/htmlfilter/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/htmlfilter/README
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/htmlfilter.yar
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.671699 thug-6.6/thug/conf/rules/imageclassifier/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/imageclassifier/README
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/imageclassifier.yar
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.671699 thug-6.6/thug/conf/rules/imagefilter/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/imagefilter/README
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/imagefilter.yar
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.671699 thug-6.6/thug/conf/rules/jsclassifier/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/jsclassifier/plugindetect.yar
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/jsclassifier.yar
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.671699 thug-6.6/thug/conf/rules/jsfilter/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/jsfilter/README
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/jsfilter.yar
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.671699 thug-6.6/thug/conf/rules/sampleclassifier/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/sampleclassifier/README
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/sampleclassifier.yar
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.671699 thug-6.6/thug/conf/rules/samplefilter/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/samplefilter/README
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/samplefilter.yar
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.671699 thug-6.6/thug/conf/rules/textclassifier/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/textclassifier/README
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/textclassifier.yar
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.671699 thug-6.6/thug/conf/rules/textfilter/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/textfilter/README
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/textfilter.yar
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.675699 thug-6.6/thug/conf/rules/urlclassifier/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/urlclassifier/README
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/urlclassifier/blackhole.yar
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/urlclassifier/cool.yar
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/urlclassifier/crimeboss.yar
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/urlclassifier/critxpack.yar
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/urlclassifier/fiesta.yar
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/urlclassifier/g01pack.yar
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/urlclassifier/impact.yar
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/urlclassifier/neutrino.yar
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/urlclassifier/nuclear.yar
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/urlclassifier/popads.yar
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/urlclassifier/redkit.yar
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/urlclassifier/safepack.yar
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/urlclassifier/sakura.yar
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/urlclassifier/sofosfo.yar
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/urlclassifier/styx.yar
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/urlclassifier/sweetorange.yar
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/urlclassifier/tds.yar
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/urlclassifier.yar
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.675699 thug-6.6/thug/conf/rules/urlfilter/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/urlfilter/README
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/urlfilter.yar
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.675699 thug-6.6/thug/conf/rules/vbsclassifier/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/vbsclassifier/README
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/vbsclassifier.yar
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.675699 thug-6.6/thug/conf/rules/vbsfilter/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/vbsfilter/README
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/rules/vbsfilter.yar
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.675699 thug-6.6/thug/conf/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/scripts/atob.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/scripts/btoa.js
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/scripts/date.js
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/scripts/eval.js
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/scripts/message-event.js
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/scripts/storage.js
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/scripts/thug.js
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/scripts/write.js
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-17 08:54:59.000000 thug-6.6/thug/conf/thug.conf
+-rw-r--r--   0 runner    (1001) docker     (127)    19877 2024-04-17 08:54:59.000000 thug-6.6/thug/thug.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:55:03.675699 thug-6.6/thug.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-04-17 08:55:03.000000 thug-6.6/thug.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16870 2024-04-17 08:55:03.000000 thug-6.6/thug.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 08:55:03.000000 thug-6.6/thug.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-17 08:55:03.000000 thug-6.6/thug.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-17 08:55:03.000000 thug-6.6/thug.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-17 08:55:03.000000 thug-6.6/thug.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 08:55:03.000000 thug-6.6/thug.egg-info/zip-safe
```

### Comparing `thug-6.5/LICENSE.txt` & `thug-6.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `thug-6.5/PKG-INFO` & `thug-6.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thug
-Version: 6.5
+Version: 6.6
 Summary: Low-interaction honeyclient Thug
 Author-email: Angelo Dell'Aera <angelo.dellaera@honeynet.org>
 Maintainer-email: Angelo Dell'Aera <angelo.dellaera@honeynet.org>
 License: GPLv2
 Project-URL: homepage, https://github.com/buffer/thug
 Project-URL: documentation, https://thug-honeyclient.readthedocs.io/en/latest/
 Project-URL: bugs, https://github.com/buffer/thug/issues
@@ -45,17 +45,17 @@
 Requires-Dist: pysocks==1.7.1
 Requires-Dist: python-magic==0.4.27
 Requires-Dist: rarfile==4.2
 Requires-Dist: requests==2.31.0
 Requires-Dist: requests-futures==1.0.1
 Requires-Dist: setuptools>=65.5.1
 Requires-Dist: ssdeep==3.4
-Requires-Dist: stpyv8==12.3.219.16
+Requires-Dist: stpyv8==12.4.254.13
 Requires-Dist: yara-python==4.5.0
-Requires-Dist: zope.interface==6.2
+Requires-Dist: zope.interface==6.3
 Provides-Extra: elasticsearch
 Requires-Dist: elasticsearch; extra == "elasticsearch"
 Provides-Extra: exploitgraph
 Requires-Dist: pygraphviz; extra == "exploitgraph"
 Provides-Extra: image
 Requires-Dist: imgkit==1.1.0; extra == "image"
 Requires-Dist: pytesseract; extra == "image"
```

### Comparing `thug-6.5/README.rst` & `thug-6.6/README.rst`

 * *Files identical despite different names*

### Comparing `thug-6.5/pyproject.toml` & `thug-6.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -54,17 +54,17 @@
     "pysocks==1.7.1",
     "python-magic==0.4.27",
     "rarfile==4.2",
     "requests==2.31.0",
     "requests-futures==1.0.1",
     "setuptools>=65.5.1",
     "ssdeep==3.4",
-    "stpyv8==12.3.219.16",
+    "stpyv8==12.4.254.13",
     "yara-python==4.5.0",
-    "zope.interface==6.2",
+    "zope.interface==6.3",
 ]
 keywords = [
     "honeyclient",
     "low-interaction",
     "client-honeypot",
     "security-tools",
 ]
```

### Comparing `thug-6.5/thug/ActiveX/ActiveX.py` & `thug-6.6/thug/ActiveX/ActiveX.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/CLSID.py` & `thug-6.6/thug/ActiveX/CLSID.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/AcroPDF.py` & `thug-6.6/thug/ActiveX/modules/AcroPDF.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/AdodbRecordset.py` & `thug-6.6/thug/ActiveX/modules/AdodbRecordset.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/AdodbStream.py` & `thug-6.6/thug/ActiveX/modules/AdodbStream.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/AnswerWorks.py` & `thug-6.6/thug/ActiveX/modules/AnswerWorks.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/AolAmpX.py` & `thug-6.6/thug/ActiveX/modules/AolAmpX.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/AolICQ.py` & `thug-6.6/thug/ActiveX/modules/AolICQ.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/BaiduBar.py` & `thug-6.6/thug/ActiveX/modules/BaiduBar.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/CGAgent.py` & `thug-6.6/thug/ActiveX/modules/CGAgent.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/ConnectAndEnterRoom.py` & `thug-6.6/thug/ActiveX/modules/ConnectAndEnterRoom.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/DPClient.py` & `thug-6.6/thug/ActiveX/modules/DPClient.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/DirectShow.py` & `thug-6.6/thug/ActiveX/modules/DirectShow.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/Domino.py` & `thug-6.6/thug/ActiveX/modules/Domino.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/EnjoySAP.py` & `thug-6.6/thug/ActiveX/modules/EnjoySAP.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/FacebookPhotoUploader.py` & `thug-6.6/thug/ActiveX/modules/FacebookPhotoUploader.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/File.py` & `thug-6.6/thug/ActiveX/modules/File.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/Folder.py` & `thug-6.6/thug/ActiveX/modules/Folder.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/GatewayWeblaunch.py` & `thug-6.6/thug/ActiveX/modules/GatewayWeblaunch.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/HPInfo.py` & `thug-6.6/thug/ActiveX/modules/HPInfo.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/IMWebControl.py` & `thug-6.6/thug/ActiveX/modules/IMWebControl.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/JavaDeploymentToolkit.py` & `thug-6.6/thug/ActiveX/modules/JavaDeploymentToolkit.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/JetAudioDownloadFromMusicStore.py` & `thug-6.6/thug/ActiveX/modules/JetAudioDownloadFromMusicStore.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/MSRICHTXT.py` & `thug-6.6/thug/ActiveX/modules/MSRICHTXT.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/MacrovisionFlexNet.py` & `thug-6.6/thug/ActiveX/modules/MacrovisionFlexNet.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/MicrosoftXMLDOM.py` & `thug-6.6/thug/ActiveX/modules/MicrosoftXMLDOM.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/MicrosoftXMLHTTP.py` & `thug-6.6/thug/ActiveX/modules/MicrosoftXMLHTTP.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/NCTAudioFile2.py` & `thug-6.6/thug/ActiveX/modules/NCTAudioFile2.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/NamoInstaller.py` & `thug-6.6/thug/ActiveX/modules/NamoInstaller.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/NeoTracePro.py` & `thug-6.6/thug/ActiveX/modules/NeoTracePro.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/NessusScanCtrl.py` & `thug-6.6/thug/ActiveX/modules/NessusScanCtrl.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/OfficeOCX.py` & `thug-6.6/thug/ActiveX/modules/OfficeOCX.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/OurgameGLWorld.py` & `thug-6.6/thug/ActiveX/modules/OurgameGLWorld.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/PPlayer.py` & `thug-6.6/thug/ActiveX/modules/PPlayer.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/RDSDataSpace.py` & `thug-6.6/thug/ActiveX/modules/RDSDataSpace.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/RealPlayer.py` & `thug-6.6/thug/ActiveX/modules/RealPlayer.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/RegistryPro.py` & `thug-6.6/thug/ActiveX/modules/RegistryPro.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/SSReaderPdg2.py` & `thug-6.6/thug/ActiveX/modules/SSReaderPdg2.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/ScriptingDictionary.py` & `thug-6.6/thug/ActiveX/modules/ScriptingDictionary.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/ScriptingFileSystemObject.py` & `thug-6.6/thug/ActiveX/modules/ScriptingFileSystemObject.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/ShellApplication.py` & `thug-6.6/thug/ActiveX/modules/ShellApplication.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/SinaDLoader.py` & `thug-6.6/thug/ActiveX/modules/SinaDLoader.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/SnapshotViewer.py` & `thug-6.6/thug/ActiveX/modules/SnapshotViewer.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/SonicWallNetExtenderAddRouteEntry.py` & `thug-6.6/thug/ActiveX/modules/SonicWallNetExtenderAddRouteEntry.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/Spreadsheet.py` & `thug-6.6/thug/ActiveX/modules/Spreadsheet.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/StormConfig.py` & `thug-6.6/thug/ActiveX/modules/StormConfig.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/StormMps.py` & `thug-6.6/thug/ActiveX/modules/StormMps.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/SymantecAppStream.py` & `thug-6.6/thug/ActiveX/modules/SymantecAppStream.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/SymantecBackupExec.py` & `thug-6.6/thug/ActiveX/modules/SymantecBackupExec.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/TextStream.py` & `thug-6.6/thug/ActiveX/modules/TextStream.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/Toshiba.py` & `thug-6.6/thug/ActiveX/modules/Toshiba.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/VLC.py` & `thug-6.6/thug/ActiveX/modules/VLC.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/VisualStudioDTE80.py` & `thug-6.6/thug/ActiveX/modules/VisualStudioDTE80.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/WMEncProfileManager.py` & `thug-6.6/thug/ActiveX/modules/WMEncProfileManager.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/WScriptExec.py` & `thug-6.6/thug/ActiveX/modules/WScriptExec.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/WScriptNetwork.py` & `thug-6.6/thug/ActiveX/modules/WScriptNetwork.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/WScriptShell.py` & `thug-6.6/thug/ActiveX/modules/WScriptShell.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/WebViewFolderIcon.py` & `thug-6.6/thug/ActiveX/modules/WebViewFolderIcon.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/WinNTSystemInfo.py` & `thug-6.6/thug/ActiveX/modules/WinNTSystemInfo.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/WinZip.py` & `thug-6.6/thug/ActiveX/modules/WinZip.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/XMLDOMParseError.py` & `thug-6.6/thug/ActiveX/modules/XMLDOMParseError.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/XUpload.py` & `thug-6.6/thug/ActiveX/modules/XUpload.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/YahooJukebox.py` & `thug-6.6/thug/ActiveX/modules/YahooJukebox.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/YahooMessengerYVerInfo.py` & `thug-6.6/thug/ActiveX/modules/YahooMessengerYVerInfo.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/YahooMessengerYwcvwr.py` & `thug-6.6/thug/ActiveX/modules/YahooMessengerYwcvwr.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/ZenturiProgramCheckerAttack.py` & `thug-6.6/thug/ActiveX/modules/ZenturiProgramCheckerAttack.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ActiveX/modules/__init__.py` & `thug-6.6/thug/ActiveX/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/Analysis/awis/AWIS.py` & `thug-6.6/thug/Analysis/awis/AWIS.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/Analysis/context/ContextAnalyzer.py` & `thug-6.6/thug/Analysis/context/ContextAnalyzer.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/Analysis/honeyagent/HoneyAgent.py` & `thug-6.6/thug/Analysis/honeyagent/HoneyAgent.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/Analysis/screenshot/Screenshot.py` & `thug-6.6/thug/Analysis/screenshot/Screenshot.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/Analysis/shellcode/Shellcode.py` & `thug-6.6/thug/Analysis/shellcode/Shellcode.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/Classifier/BaseClassifier.py` & `thug-6.6/thug/Classifier/BaseClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/Classifier/CookieClassifier.py` & `thug-6.6/thug/Classifier/CookieClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/Classifier/HTMLClassifier.py` & `thug-6.6/thug/Classifier/HTMLClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/Classifier/ImageClassifier.py` & `thug-6.6/thug/Classifier/ImageClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/Classifier/JSClassifier.py` & `thug-6.6/thug/Classifier/JSClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/Classifier/SampleClassifier.py` & `thug-6.6/thug/Classifier/SampleClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/Classifier/TextClassifier.py` & `thug-6.6/thug/Classifier/TextClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/Classifier/URLClassifier.py` & `thug-6.6/thug/Classifier/URLClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/Classifier/VBSClassifier.py` & `thug-6.6/thug/Classifier/VBSClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/Alexa.py` & `thug-6.6/thug/DOM/Alexa.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/AsyncPrefetcher.py` & `thug-6.6/thug/DOM/AsyncPrefetcher.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/CCInterpreter.py` & `thug-6.6/thug/DOM/CCInterpreter.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/Chrome.py` & `thug-6.6/thug/DOM/Chrome.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/ClipboardData.py` & `thug-6.6/thug/DOM/ClipboardData.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/Components.py` & `thug-6.6/thug/DOM/Components.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/Console.py` & `thug-6.6/thug/DOM/Console.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/Crypto.py` & `thug-6.6/thug/DOM/Crypto.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/DFT.py` & `thug-6.6/thug/DOM/DFT.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/External.py` & `thug-6.6/thug/DOM/External.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/HTMLInspector.py` & `thug-6.6/thug/DOM/HTMLInspector.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/HTTPSession.py` & `thug-6.6/thug/DOM/HTTPSession.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/HTTPSessionException.py` & `thug-6.6/thug/DOM/HTTPSessionException.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/History.py` & `thug-6.6/thug/DOM/History.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/JSClass.py` & `thug-6.6/thug/DOM/JSClass.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/JSEngine.py` & `thug-6.6/thug/DOM/JSEngine.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/JSInspector.py` & `thug-6.6/thug/DOM/JSInspector.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/JScriptEncode.py` & `thug-6.6/thug/DOM/JScriptEncode.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/LocalStorage.py` & `thug-6.6/thug/DOM/LocalStorage.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/Location.py` & `thug-6.6/thug/DOM/Location.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/MIMEHandler.py` & `thug-6.6/thug/DOM/MIMEHandler.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/Map.py` & `thug-6.6/thug/DOM/Map.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/MimeType.py` & `thug-6.6/thug/DOM/MimeType.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/MimeTypes.py` & `thug-6.6/thug/DOM/MimeTypes.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/MozConnection.py` & `thug-6.6/thug/DOM/MozConnection.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/Navigator.py` & `thug-6.6/thug/DOM/Navigator.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/Personality.py` & `thug-6.6/thug/DOM/Personality.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/Plugin.py` & `thug-6.6/thug/DOM/Plugin.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/Plugins.py` & `thug-6.6/thug/DOM/Plugins.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/SchemeHandler.py` & `thug-6.6/thug/DOM/SchemeHandler.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/Screen.py` & `thug-6.6/thug/DOM/Screen.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/SessionStorage.py` & `thug-6.6/thug/DOM/SessionStorage.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/Sidebar.py` & `thug-6.6/thug/DOM/Sidebar.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/Storage.py` & `thug-6.6/thug/DOM/Storage.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/UserProfile.py` & `thug-6.6/thug/DOM/UserProfile.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/Utils.py` & `thug-6.6/thug/DOM/Utils.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/Core/Attr.py` & `thug-6.6/thug/DOM/W3C/Core/Attr.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/Core/CharacterData.py` & `thug-6.6/thug/DOM/W3C/Core/CharacterData.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/Core/ClassList.py` & `thug-6.6/thug/DOM/W3C/Core/ClassList.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/Core/Comment.py` & `thug-6.6/thug/DOM/W3C/Core/Comment.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/Core/DOMException.py` & `thug-6.6/thug/DOM/W3C/Core/DOMException.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/Core/DOMImplementation.py` & `thug-6.6/thug/DOM/W3C/Core/DOMImplementation.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/Core/Document.py` & `thug-6.6/thug/DOM/W3C/Core/Document.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/Core/DocumentFragment.py` & `thug-6.6/thug/DOM/W3C/Core/DocumentFragment.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/Core/DocumentType.py` & `thug-6.6/thug/DOM/W3C/Core/DocumentType.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/Core/Element.py` & `thug-6.6/thug/DOM/W3C/Core/Element.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/Core/NamedNodeMap.py` & `thug-6.6/thug/DOM/W3C/Core/NamedNodeMap.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/Core/Node.py` & `thug-6.6/thug/DOM/W3C/Core/Node.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/Core/NodeList.py` & `thug-6.6/thug/DOM/W3C/Core/NodeList.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/Core/Text.py` & `thug-6.6/thug/DOM/W3C/Core/Text.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/Core/__init__.py` & `thug-6.6/thug/DOM/W3C/Core/__init__.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/DOMTokenList.py` & `thug-6.6/thug/DOM/W3C/DOMTokenList.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/Events/DocumentEvent.py` & `thug-6.6/thug/DOM/W3C/Events/DocumentEvent.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/Events/Event.py` & `thug-6.6/thug/DOM/W3C/Events/Event.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/Events/EventTarget.py` & `thug-6.6/thug/DOM/W3C/Events/EventTarget.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/Events/MessageEvent.py` & `thug-6.6/thug/DOM/W3C/Events/MessageEvent.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/Events/MouseEvent.py` & `thug-6.6/thug/DOM/W3C/Events/MouseEvent.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/Events/MutationEvent.py` & `thug-6.6/thug/DOM/W3C/Events/MutationEvent.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/Events/StorageEvent.py` & `thug-6.6/thug/DOM/W3C/Events/StorageEvent.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/Events/UIEvent.py` & `thug-6.6/thug/DOM/W3C/Events/UIEvent.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/Events/__init__.py` & `thug-6.6/thug/DOM/W3C/Events/__init__.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/File/Blob.py` & `thug-6.6/thug/DOM/W3C/File/Blob.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/File/File.py` & `thug-6.6/thug/DOM/W3C/File/File.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/HTML/Dataset.py` & `thug-6.6/thug/DOM/W3C/HTML/Dataset.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/HTML/HTMLAnchorElement.py` & `thug-6.6/thug/DOM/W3C/HTML/HTMLAnchorElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/HTML/HTMLAppletElement.py` & `thug-6.6/thug/DOM/W3C/HTML/HTMLAppletElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/HTML/HTMLBodyElement.py` & `thug-6.6/thug/DOM/W3C/HTML/HTMLBodyElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/HTML/HTMLButtonElement.py` & `thug-6.6/thug/DOM/W3C/HTML/HTMLButtonElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/HTML/HTMLCollection.py` & `thug-6.6/thug/DOM/W3C/HTML/HTMLCollection.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/HTML/HTMLDocument.py` & `thug-6.6/thug/DOM/W3C/HTML/HTMLDocument.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/HTML/HTMLDocumentCompatibleInfo.py` & `thug-6.6/thug/DOM/W3C/HTML/HTMLDocumentCompatibleInfo.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/HTML/HTMLElement.py` & `thug-6.6/thug/DOM/W3C/HTML/HTMLElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/HTML/HTMLFormElement.py` & `thug-6.6/thug/DOM/W3C/HTML/HTMLFormElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/HTML/HTMLFrameElement.py` & `thug-6.6/thug/DOM/W3C/HTML/HTMLFrameElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/HTML/HTMLIFrameElement.py` & `thug-6.6/thug/DOM/W3C/HTML/HTMLIFrameElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/HTML/HTMLImageElement.py` & `thug-6.6/thug/DOM/W3C/HTML/HTMLImageElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/HTML/HTMLInputElement.py` & `thug-6.6/thug/DOM/W3C/HTML/HTMLInputElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/HTML/HTMLLinkElement.py` & `thug-6.6/thug/DOM/W3C/HTML/HTMLLinkElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/HTML/HTMLMediaElement.py` & `thug-6.6/thug/DOM/W3C/HTML/HTMLMediaElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/HTML/HTMLMetaElement.py` & `thug-6.6/thug/DOM/W3C/HTML/HTMLMetaElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/HTML/HTMLObjectElement.py` & `thug-6.6/thug/DOM/W3C/HTML/HTMLObjectElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/HTML/HTMLOptionElement.py` & `thug-6.6/thug/DOM/W3C/HTML/HTMLOptionElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/HTML/HTMLScriptElement.py` & `thug-6.6/thug/DOM/W3C/HTML/HTMLScriptElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/HTML/HTMLSelectElement.py` & `thug-6.6/thug/DOM/W3C/HTML/HTMLSelectElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/HTML/HTMLTableCellElement.py` & `thug-6.6/thug/DOM/W3C/HTML/HTMLTableCellElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/HTML/HTMLTableElement.py` & `thug-6.6/thug/DOM/W3C/HTML/HTMLTableElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/HTML/HTMLTableRowElement.py` & `thug-6.6/thug/DOM/W3C/HTML/HTMLTableRowElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/HTML/HTMLTableSectionElement.py` & `thug-6.6/thug/DOM/W3C/HTML/HTMLTableSectionElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/HTML/HTMLTextAreaElement.py` & `thug-6.6/thug/DOM/W3C/HTML/HTMLTextAreaElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/HTML/HTMLVideoElement.py` & `thug-6.6/thug/DOM/W3C/HTML/HTMLVideoElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/HTML/TAnimateColor.py` & `thug-6.6/thug/DOM/W3C/HTML/TAnimateColor.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/HTML/TimeRanges.py` & `thug-6.6/thug/DOM/W3C/HTML/TimeRanges.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/HTML/__init__.py` & `thug-6.6/thug/DOM/W3C/HTML/__init__.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/HTML/text_property.py` & `thug-6.6/thug/DOM/W3C/HTML/text_property.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/Style/CSS/CSSStyleDeclaration.py` & `thug-6.6/thug/DOM/W3C/Style/CSS/CSSStyleDeclaration.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/URL/URL.py` & `thug-6.6/thug/DOM/W3C/URL/URL.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/W3C/URL/URLSearchParams.py` & `thug-6.6/thug/DOM/W3C/URL/URLSearchParams.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/WebStore.py` & `thug-6.6/thug/DOM/WebStore.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/Window.py` & `thug-6.6/thug/DOM/Window.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/DOM/w3c_bindings.py` & `thug-6.6/thug/DOM/w3c_bindings.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/Encoding/Encoding.py` & `thug-6.6/thug/Encoding/Encoding.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/Java/System.py` & `thug-6.6/thug/Java/System.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/Java/java.py` & `thug-6.6/thug/Java/java.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/Java/lang.py` & `thug-6.6/thug/Java/lang.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/Logging/BaseLogging.py` & `thug-6.6/thug/Logging/BaseLogging.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/Logging/Features.py` & `thug-6.6/thug/Logging/Features.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/Logging/LoggingModules.py` & `thug-6.6/thug/Logging/LoggingModules.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/Logging/SampleLogging.py` & `thug-6.6/thug/Logging/SampleLogging.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/Logging/ThugLogging.py` & `thug-6.6/thug/Logging/ThugLogging.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/Logging/modules/ElasticSearch.py` & `thug-6.6/thug/Logging/modules/ElasticSearch.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/Logging/modules/ExploitGraph.py` & `thug-6.6/thug/Logging/modules/ExploitGraph.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/Logging/modules/JSON.py` & `thug-6.6/thug/Logging/modules/JSON.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/Logging/modules/Mapper.py` & `thug-6.6/thug/Logging/modules/Mapper.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/Logging/modules/MongoDB.py` & `thug-6.6/thug/Logging/modules/MongoDB.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/Magic/Magic.py` & `thug-6.6/thug/Magic/Magic.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/OS/Windows.py` & `thug-6.6/thug/OS/Windows.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/Plugins/IPlugin.py` & `thug-6.6/thug/Plugins/IPlugin.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/Plugins/ThugPlugins.py` & `thug-6.6/thug/Plugins/ThugPlugins.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/Plugins/plugins/POST-TestPlugin-999/Handler.py` & `thug-6.6/thug/Plugins/plugins/POST-TestPlugin-999/Handler.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/Plugins/plugins/PRE-TestPlugin-999/Handler.py` & `thug-6.6/thug/Plugins/plugins/PRE-TestPlugin-999/Handler.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ThugAPI/IThugAPI.py` & `thug-6.6/thug/ThugAPI/IThugAPI.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ThugAPI/OpaqueFilter.py` & `thug-6.6/thug/ThugAPI/OpaqueFilter.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ThugAPI/ThugAPI.py` & `thug-6.6/thug/ThugAPI/ThugAPI.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ThugAPI/ThugOpts.py` & `thug-6.6/thug/ThugAPI/ThugOpts.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ThugAPI/ThugVulnModules.py` & `thug-6.6/thug/ThugAPI/ThugVulnModules.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/ThugAPI/Watchdog.py` & `thug-6.6/thug/ThugAPI/Watchdog.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/WebTracking/Cookies.py` & `thug-6.6/thug/WebTracking/Cookies.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/WebTracking/WebStorage.py` & `thug-6.6/thug/WebTracking/WebStorage.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/WebTracking/WebTracking.py` & `thug-6.6/thug/WebTracking/WebTracking.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/__init__.py` & `thug-6.6/thug/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import importlib.resources
 
 import appdirs
 
-__version__ = "6.5"
+__version__ = "6.6"
 __jsengine__ = ""
 __jsengine_version__ = ""
 
 __global_configuration_path__ = "/etc/thug"
 __user_configuration_path__ = f"{appdirs.user_config_dir()}/thug"
 __package_configuration_path__ = os.path.join(importlib.resources.files("thug"), "conf")
 __configuration_path__ = __package_configuration_path__
```

### Comparing `thug-6.5/thug/conf/personalities/galaxy2chrome18.json` & `thug-6.6/thug/conf/personalities/galaxy2chrome18.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/galaxy2chrome25.json` & `thug-6.6/thug/conf/personalities/galaxy2chrome25.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/galaxy2chrome29.json` & `thug-6.6/thug/conf/personalities/galaxy2chrome29.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/ipadchrome33.json` & `thug-6.6/thug/conf/personalities/ipadchrome33.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/ipadchrome35.json` & `thug-6.6/thug/conf/personalities/ipadchrome35.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/ipadchrome37.json` & `thug-6.6/thug/conf/personalities/ipadchrome37.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/ipadchrome38.json` & `thug-6.6/thug/conf/personalities/ipadchrome38.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/ipadchrome39.json` & `thug-6.6/thug/conf/personalities/ipadchrome39.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/ipadchrome45.json` & `thug-6.6/thug/conf/personalities/ipadchrome45.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/ipadchrome46.json` & `thug-6.6/thug/conf/personalities/ipadchrome46.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/ipadchrome47.json` & `thug-6.6/thug/conf/personalities/ipadchrome47.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/ipadsafari7.json` & `thug-6.6/thug/conf/personalities/ipadsafari7.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/ipadsafari8.json` & `thug-6.6/thug/conf/personalities/ipadsafari8.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/ipadsafari9.json` & `thug-6.6/thug/conf/personalities/ipadsafari9.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/linuxchrome26.json` & `thug-6.6/thug/conf/personalities/linuxchrome26.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/linuxchrome30.json` & `thug-6.6/thug/conf/personalities/linuxchrome30.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/linuxchrome44.json` & `thug-6.6/thug/conf/personalities/linuxchrome44.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/linuxchrome54.json` & `thug-6.6/thug/conf/personalities/linuxchrome54.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/linuxchrome98.json` & `thug-6.6/thug/conf/personalities/linuxchrome98.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/linuxfirefox19.json` & `thug-6.6/thug/conf/personalities/linuxfirefox19.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/linuxfirefox40.json` & `thug-6.6/thug/conf/personalities/linuxfirefox40.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/nexuschrome18.json` & `thug-6.6/thug/conf/personalities/nexuschrome18.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/osx10chrome19.json` & `thug-6.6/thug/conf/personalities/osx10chrome19.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/osx10chrome80.json` & `thug-6.6/thug/conf/personalities/osx10chrome80.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/osx10chrome97.json` & `thug-6.6/thug/conf/personalities/osx10chrome97.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/osx10safari5.json` & `thug-6.6/thug/conf/personalities/osx10safari5.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/osx11safari14.json` & `thug-6.6/thug/conf/personalities/osx11safari14.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/win10edge20.json.review` & `thug-6.6/thug/conf/personalities/win10edge20.json.review`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/win10ie110.json` & `thug-6.6/thug/conf/personalities/win10ie110.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/win2kie60.json` & `thug-6.6/thug/conf/personalities/win2kie60.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/win2kie80.json` & `thug-6.6/thug/conf/personalities/win2kie80.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/win7chrome20.json` & `thug-6.6/thug/conf/personalities/win7chrome20.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/win7chrome40.json` & `thug-6.6/thug/conf/personalities/win7chrome40.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/win7chrome45.json` & `thug-6.6/thug/conf/personalities/win7chrome45.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/win7chrome49.json` & `thug-6.6/thug/conf/personalities/win7chrome49.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/win7firefox3.json` & `thug-6.6/thug/conf/personalities/win7firefox3.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/win7ie100.json` & `thug-6.6/thug/conf/personalities/win7ie100.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/win7ie80.json` & `thug-6.6/thug/conf/personalities/win7ie80.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/win7ie90.json` & `thug-6.6/thug/conf/personalities/win7ie90.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/win7safari5.json` & `thug-6.6/thug/conf/personalities/win7safari5.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/winxpchrome20.json` & `thug-6.6/thug/conf/personalities/winxpchrome20.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/winxpfirefox12.json` & `thug-6.6/thug/conf/personalities/winxpfirefox12.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/winxpie60.json` & `thug-6.6/thug/conf/personalities/winxpie60.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/winxpie61.json` & `thug-6.6/thug/conf/personalities/winxpie61.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/winxpie70.json` & `thug-6.6/thug/conf/personalities/winxpie70.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/winxpie80.json` & `thug-6.6/thug/conf/personalities/winxpie80.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/personalities/winxpsafari5.json` & `thug-6.6/thug/conf/personalities/winxpsafari5.json`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/rules/urlclassifier/blackhole.yar` & `thug-6.6/thug/conf/rules/urlclassifier/blackhole.yar`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/rules/urlclassifier/crimeboss.yar` & `thug-6.6/thug/conf/rules/urlclassifier/crimeboss.yar`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/rules/urlclassifier/critxpack.yar` & `thug-6.6/thug/conf/rules/urlclassifier/critxpack.yar`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/rules/urlclassifier/fiesta.yar` & `thug-6.6/thug/conf/rules/urlclassifier/fiesta.yar`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/rules/urlclassifier/g01pack.yar` & `thug-6.6/thug/conf/rules/urlclassifier/g01pack.yar`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/rules/urlclassifier/neutrino.yar` & `thug-6.6/thug/conf/rules/urlclassifier/neutrino.yar`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/rules/urlclassifier/nuclear.yar` & `thug-6.6/thug/conf/rules/urlclassifier/nuclear.yar`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/rules/urlclassifier/popads.yar` & `thug-6.6/thug/conf/rules/urlclassifier/popads.yar`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/rules/urlclassifier/redkit.yar` & `thug-6.6/thug/conf/rules/urlclassifier/redkit.yar`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/rules/urlclassifier/styx.yar` & `thug-6.6/thug/conf/rules/urlclassifier/styx.yar`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/rules/urlclassifier/sweetorange.yar` & `thug-6.6/thug/conf/rules/urlclassifier/sweetorange.yar`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/scripts/atob.js` & `thug-6.6/thug/conf/scripts/atob.js`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/scripts/btoa.js` & `thug-6.6/thug/conf/scripts/btoa.js`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/conf/scripts/thug.js` & `thug-6.6/thug/conf/scripts/thug.js`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug/thug.py` & `thug-6.6/thug/thug.py`

 * *Files identical despite different names*

### Comparing `thug-6.5/thug.egg-info/PKG-INFO` & `thug-6.6/thug.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thug
-Version: 6.5
+Version: 6.6
 Summary: Low-interaction honeyclient Thug
 Author-email: Angelo Dell'Aera <angelo.dellaera@honeynet.org>
 Maintainer-email: Angelo Dell'Aera <angelo.dellaera@honeynet.org>
 License: GPLv2
 Project-URL: homepage, https://github.com/buffer/thug
 Project-URL: documentation, https://thug-honeyclient.readthedocs.io/en/latest/
 Project-URL: bugs, https://github.com/buffer/thug/issues
@@ -45,17 +45,17 @@
 Requires-Dist: pysocks==1.7.1
 Requires-Dist: python-magic==0.4.27
 Requires-Dist: rarfile==4.2
 Requires-Dist: requests==2.31.0
 Requires-Dist: requests-futures==1.0.1
 Requires-Dist: setuptools>=65.5.1
 Requires-Dist: ssdeep==3.4
-Requires-Dist: stpyv8==12.3.219.16
+Requires-Dist: stpyv8==12.4.254.13
 Requires-Dist: yara-python==4.5.0
-Requires-Dist: zope.interface==6.2
+Requires-Dist: zope.interface==6.3
 Provides-Extra: elasticsearch
 Requires-Dist: elasticsearch; extra == "elasticsearch"
 Provides-Extra: exploitgraph
 Requires-Dist: pygraphviz; extra == "exploitgraph"
 Provides-Extra: image
 Requires-Dist: imgkit==1.1.0; extra == "image"
 Requires-Dist: pytesseract; extra == "image"
```

### Comparing `thug-6.5/thug.egg-info/SOURCES.txt` & `thug-6.6/thug.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -471,15 +471,8 @@
 thug/conf/scripts/atob.js
 thug/conf/scripts/btoa.js
 thug/conf/scripts/date.js
 thug/conf/scripts/eval.js
 thug/conf/scripts/message-event.js
 thug/conf/scripts/storage.js
 thug/conf/scripts/thug.js
-thug/conf/scripts/write.js
-thug/thug.egg-info/PKG-INFO
-thug/thug.egg-info/SOURCES.txt
-thug/thug.egg-info/dependency_links.txt
-thug/thug.egg-info/entry_points.txt
-thug/thug.egg-info/requires.txt
-thug/thug.egg-info/top_level.txt
-thug/thug.egg-info/zip-safe
+thug/conf/scripts/write.js
```

### Comparing `thug-6.5/thug.egg-info/requires.txt` & `thug-6.6/thug.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 pysocks==1.7.1
 python-magic==0.4.27
 rarfile==4.2
 requests==2.31.0
 requests-futures==1.0.1
 setuptools>=65.5.1
 ssdeep==3.4
-stpyv8==12.3.219.16
+stpyv8==12.4.254.13
 yara-python==4.5.0
-zope.interface==6.2
+zope.interface==6.3
 
 [:python_version < "3.10"]
 networkx==3.2.1
 
 [:python_version < "3.9"]
 importlib-resources==6.0.1
```

