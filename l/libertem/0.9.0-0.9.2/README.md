# Comparing `tmp/libertem-0.9.0.tar.gz` & `tmp/libertem-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libertem-0.9.0.tar", last modified: Thu Feb 17 15:59:02 2022, max compression
+gzip compressed data, was "libertem-0.9.2.tar", last modified: Thu Apr 28 17:30:33 2022, max compression
```

## Comparing `libertem-0.9.0.tar` & `libertem-0.9.2.tar`

### file list

```diff
@@ -1,574 +1,575 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.156690 libertem-0.9.0/
--rw-r--r--   0 root         (0) root         (0)    35149 2022-02-16 12:09:30.000000 libertem-0.9.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      125 2022-02-16 12:09:30.000000 libertem-0.9.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    10657 2022-02-17 15:59:02.156690 libertem-0.9.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9331 2022-02-16 12:09:30.000000 libertem-0.9.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:01.935692 libertem-0.9.0/client/
--rw-r--r--   0 root         (0) root         (0)     8275 2022-02-16 12:09:30.000000 libertem-0.9.0/client/.eslintrc.js
--rw-r--r--   0 root         (0) root         (0)      285 2022-02-16 12:09:30.000000 libertem-0.9.0/client/.gitignore
--rw-r--r--   0 root         (0) root         (0)     9483 2022-02-16 12:09:30.000000 libertem-0.9.0/client/README.md
--rw-r--r--   0 root         (0) root         (0)  1958343 2022-02-16 12:09:30.000000 libertem-0.9.0/client/package-lock.json
--rw-r--r--   0 root         (0) root         (0)     1685 2022-02-16 12:09:30.000000 libertem-0.9.0/client/package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:01.936692 libertem-0.9.0/client/public/
--rw-r--r--   0 root         (0) root         (0)    15086 2022-02-16 12:09:30.000000 libertem-0.9.0/client/public/favicon.ico
--rw-r--r--   0 root         (0) root         (0)     1589 2022-02-16 12:09:30.000000 libertem-0.9.0/client/public/index.html
--rw-r--r--   0 root         (0) root         (0)      295 2022-02-16 12:09:30.000000 libertem-0.9.0/client/public/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:01.943692 libertem-0.9.0/client/src/
--rw-r--r--   0 root         (0) root         (0)     2524 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/About.tsx
--rw-r--r--   0 root         (0) root         (0)      274 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/App.test.tsx
--rw-r--r--   0 root         (0) root         (0)      816 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/App.tsx
--rw-r--r--   0 root         (0) root         (0)      846 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/Menu.tsx
--rw-r--r--   0 root         (0) root         (0)      767 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/actions.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:01.944692 libertem-0.9.0/client/src/analysis/
--rw-r--r--   0 root         (0) root         (0)     1307 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/analysis/actions.ts
--rw-r--r--   0 root         (0) root         (0)     2987 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/analysis/reducers.ts
--rw-r--r--   0 root         (0) root         (0)      268 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/analysis/types.ts
--rw-r--r--   0 root         (0) root         (0)       58 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/basicTypes.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:01.946692 libertem-0.9.0/client/src/browser/
--rw-r--r--   0 root         (0) root         (0)     1616 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/browser/actions.ts
--rw-r--r--   0 root         (0) root         (0)      494 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/browser/api.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:01.950692 libertem-0.9.0/client/src/browser/components/
--rw-r--r--   0 root         (0) root         (0)     1145 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/browser/components/BrowserWrapper.tsx
--rw-r--r--   0 root         (0) root         (0)     3206 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/browser/components/FileBrowser.tsx
--rw-r--r--   0 root         (0) root         (0)     3645 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/browser/components/FileBrowserEntry.tsx
--rw-r--r--   0 root         (0) root         (0)     1079 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/browser/components/FileBrowserHeader.tsx
--rw-r--r--   0 root         (0) root         (0)      987 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/browser/components/FileEntry.tsx
--rw-r--r--   0 root         (0) root         (0)      970 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/browser/components/FolderEntry.tsx
--rw-r--r--   0 root         (0) root         (0)     3487 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/browser/components/PathBar.tsx
--rw-r--r--   0 root         (0) root         (0)      947 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/browser/components/PathDropDownItem.tsx
--rw-r--r--   0 root         (0) root         (0)      990 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/browser/components/PathInput.tsx
--rw-r--r--   0 root         (0) root         (0)     1864 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/browser/components/RecentFiles.tsx
--rw-r--r--   0 root         (0) root         (0)     2083 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/browser/reducers.ts
--rw-r--r--   0 root         (0) root         (0)     2773 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/browser/sagas.ts
--rw-r--r--   0 root         (0) root         (0)      348 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/browser/types.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:01.952692 libertem-0.9.0/client/src/channel/
--rw-r--r--   0 root         (0) root         (0)     2892 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/channel/actions.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:01.953692 libertem-0.9.0/client/src/channel/components/
--rw-r--r--   0 root         (0) root         (0)      459 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/channel/components/ChannelConnecting.tsx
--rw-r--r--   0 root         (0) root         (0)      397 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/channel/components/ChannelShutdown.tsx
--rw-r--r--   0 root         (0) root         (0)     2141 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/channel/components/ChannelStatus.tsx
--rw-r--r--   0 root         (0) root         (0)     4099 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/channel/messages.ts
--rw-r--r--   0 root         (0) root         (0)     1084 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/channel/reducers.ts
--rw-r--r--   0 root         (0) root         (0)     7858 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/channel/sagas.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:01.955692 libertem-0.9.0/client/src/cluster/
--rw-r--r--   0 root         (0) root         (0)      855 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/cluster/actions.ts
--rw-r--r--   0 root         (0) root         (0)      656 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/cluster/api.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:01.957692 libertem-0.9.0/client/src/cluster/components/
--rw-r--r--   0 root         (0) root         (0)     2699 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/cluster/components/ClusterConnectionForm.tsx
--rw-r--r--   0 root         (0) root         (0)     1570 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/cluster/components/GPUSelector.tsx
--rw-r--r--   0 root         (0) root         (0)     3559 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/cluster/components/LocalConnectionForm.tsx
--rw-r--r--   0 root         (0) root         (0)     1490 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/cluster/components/TCPConnectionForm.tsx
--rw-r--r--   0 root         (0) root         (0)     1086 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/cluster/reducers.ts
--rw-r--r--   0 root         (0) root         (0)     1615 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/cluster/sagas.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:01.958692 libertem-0.9.0/client/src/clusterStatus/
--rw-r--r--   0 root         (0) root         (0)      440 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/clusterStatus/api.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:01.959692 libertem-0.9.0/client/src/clusterStatus/components/
--rw-r--r--   0 root         (0) root         (0)     2564 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/clusterStatus/components/Cluster.tsx
--rw-r--r--   0 root         (0) root         (0)     2207 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/clusterStatus/components/LocalStatus.tsx
--rw-r--r--   0 root         (0) root         (0)      371 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/clusterStatus/components/NotConnected.tsx
--rw-r--r--   0 root         (0) root         (0)     4498 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/clusterStatus/components/TCPStatus.tsx
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:01.963692 libertem-0.9.0/client/src/compoundAnalysis/
--rw-r--r--   0 root         (0) root         (0)     2150 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/compoundAnalysis/actions.ts
--rw-r--r--   0 root         (0) root         (0)     1916 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/compoundAnalysis/api.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:01.971692 libertem-0.9.0/client/src/compoundAnalysis/components/
--rw-r--r--   0 root         (0) root         (0)    13884 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/compoundAnalysis/components/CenterOfMassAnalysis.tsx
--rw-r--r--   0 root         (0) root         (0)     7633 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/compoundAnalysis/components/Clustering.tsx
--rw-r--r--   0 root         (0) root         (0)     4394 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/compoundAnalysis/components/DefaultFrameView.tsx
--rw-r--r--   0 root         (0) root         (0)     3837 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/compoundAnalysis/components/DiskMaskAnalysis.tsx
--rw-r--r--   0 root         (0) root         (0)     8493 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/compoundAnalysis/components/Download.tsx
--rw-r--r--   0 root         (0) root         (0)     4496 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/compoundAnalysis/components/FEM.tsx
--rw-r--r--   0 root         (0) root         (0)     7148 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/compoundAnalysis/components/FFTAnalysis.tsx
--rw-r--r--   0 root         (0) root         (0)     2005 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/compoundAnalysis/components/FFTFramePicker.tsx
--rw-r--r--   0 root         (0) root         (0)     3020 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/compoundAnalysis/components/FFTFrameView.tsx
--rw-r--r--   0 root         (0) root         (0)      910 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/compoundAnalysis/components/FFTSumFrames.tsx
--rw-r--r--   0 root         (0) root         (0)     1911 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/compoundAnalysis/components/FramePicker.tsx
--rw-r--r--   0 root         (0) root         (0)      639 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/compoundAnalysis/components/JustSum.tsx
--rw-r--r--   0 root         (0) root         (0)      957 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/compoundAnalysis/components/ModeSelector.tsx
--rw-r--r--   0 root         (0) root         (0)     3416 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/compoundAnalysis/components/PointSelectionAnalysis.tsx
--rw-r--r--   0 root         (0) root         (0)     4643 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/compoundAnalysis/components/RadialFourierAnalysis.tsx
--rw-r--r--   0 root         (0) root         (0)     4477 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/compoundAnalysis/components/RingMaskAnalysis.tsx
--rw-r--r--   0 root         (0) root         (0)     1740 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/compoundAnalysis/components/Toolbar.tsx
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:01.971692 libertem-0.9.0/client/src/compoundAnalysis/components/base/
--rw-r--r--   0 root         (0) root         (0)      898 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/compoundAnalysis/components/base/Analysis.tsx
--rw-r--r--   0 root         (0) root         (0)      412 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/compoundAnalysis/components/base/AnalysisList.tsx
--rw-r--r--   0 root         (0) root         (0)     1173 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/compoundAnalysis/components/base/AnalysisSelect.tsx
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:01.973692 libertem-0.9.0/client/src/compoundAnalysis/components/layouts/
--rw-r--r--   0 root         (0) root         (0)     1907 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/compoundAnalysis/components/layouts/AnalysisLayoutThreeCol.tsx
--rw-r--r--   0 root         (0) root         (0)     1162 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/compoundAnalysis/components/layouts/AnalysisLayoutTwoCol.tsx
--rw-r--r--   0 root         (0) root         (0)     1954 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/compoundAnalysis/components/layouts/AnalysisLayoutTwoRes.tsx
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:01.973692 libertem-0.9.0/client/src/compoundAnalysis/components/roi/
--rw-r--r--   0 root         (0) root         (0)     1942 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/compoundAnalysis/components/roi/DiskROI.tsx
--rw-r--r--   0 root         (0) root         (0)     1943 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/compoundAnalysis/components/roi/RectROI.tsx
--rw-r--r--   0 root         (0) root         (0)     1243 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/compoundAnalysis/components/roi/RoiPicker.tsx
--rw-r--r--   0 root         (0) root         (0)      392 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/compoundAnalysis/getMetadata.tsx
--rw-r--r--   0 root         (0) root         (0)     2703 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/compoundAnalysis/helpers.ts
--rw-r--r--   0 root         (0) root         (0)     2579 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/compoundAnalysis/reducers.ts
--rw-r--r--   0 root         (0) root         (0)    10390 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/compoundAnalysis/sagas.ts
--rw-r--r--   0 root         (0) root         (0)     3894 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/compoundAnalysis/types.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:01.976692 libertem-0.9.0/client/src/config/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:01.976692 libertem-0.9.0/client/src/config/__tests__/
--rw-r--r--   0 root         (0) root         (0)      594 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/config/__tests__/helpers.ts
--rw-r--r--   0 root         (0) root         (0)      675 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/config/__tests__/reducers.ts
--rw-r--r--   0 root         (0) root         (0)      713 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/config/actions.ts
--rw-r--r--   0 root         (0) root         (0)      389 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/config/api.ts
--rw-r--r--   0 root         (0) root         (0)     1949 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/config/helpers.ts
--rw-r--r--   0 root         (0) root         (0)     3273 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/config/reducers.ts
--rw-r--r--   0 root         (0) root         (0)     2481 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/config/sagas.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:01.979692 libertem-0.9.0/client/src/dataset/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:01.980692 libertem-0.9.0/client/src/dataset/__tests__/
--rw-r--r--   0 root         (0) root         (0)     2773 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/dataset/__tests__/validate.ts
--rw-r--r--   0 root         (0) root         (0)     1699 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/dataset/actions.ts
--rw-r--r--   0 root         (0) root         (0)      893 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/dataset/api.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:01.988692 libertem-0.9.0/client/src/dataset/components/
--rw-r--r--   0 root         (0) root         (0)      887 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/dataset/components/AddAnalysis.tsx
--rw-r--r--   0 root         (0) root         (0)     3282 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/dataset/components/BLOParamsForm.tsx
--rw-r--r--   0 root         (0) root         (0)     1237 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/dataset/components/BackendSelectionDropdown.tsx
--rw-r--r--   0 root         (0) root         (0)     3431 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/dataset/components/Dataset.tsx
--rw-r--r--   0 root         (0) root         (0)     1454 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/dataset/components/DatasetInfo.tsx
--rw-r--r--   0 root         (0) root         (0)     1152 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/dataset/components/DatasetList.tsx
--rw-r--r--   0 root         (0) root         (0)     9992 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/dataset/components/DatasetOpen.tsx
--rw-r--r--   0 root         (0) root         (0)      884 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/dataset/components/DatasetOpenSpinner.tsx
--rw-r--r--   0 root         (0) root         (0)     1478 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/dataset/components/DatasetParams.tsx
--rw-r--r--   0 root         (0) root         (0)      833 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/dataset/components/DatasetToolbar.tsx
--rw-r--r--   0 root         (0) root         (0)      856 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/dataset/components/DatasetTypeSelect.tsx
--rw-r--r--   0 root         (0) root         (0)     3241 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/dataset/components/EMPADParamsForm.tsx
--rw-r--r--   0 root         (0) root         (0)     3240 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/dataset/components/FRMS6ParamsForm.tsx
--rw-r--r--   0 root         (0) root         (0)     4261 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/dataset/components/HDF5ParamsForm.tsx
--rw-r--r--   0 root         (0) root         (0)     3238 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/dataset/components/K2ISParamsForm.tsx
--rw-r--r--   0 root         (0) root         (0)     3284 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/dataset/components/MIBParamsForm.tsx
--rw-r--r--   0 root         (0) root         (0)     2759 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/dataset/components/MRCParamsForm.tsx
--rw-r--r--   0 root         (0) root         (0)     3418 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/dataset/components/RawFileParamsForm.tsx
--rw-r--r--   0 root         (0) root         (0)     3036 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/dataset/components/Reshape.tsx
--rw-r--r--   0 root         (0) root         (0)     3284 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/dataset/components/SEQParamsForm.tsx
--rw-r--r--   0 root         (0) root         (0)     2690 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/dataset/components/SERParamsForm.tsx
--rw-r--r--   0 root         (0) root         (0)     3312 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/dataset/components/TVIPSParamsForm.tsx
--rw-r--r--   0 root         (0) root         (0)     3012 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/dataset/components/TupleInput.tsx
--rw-r--r--   0 root         (0) root         (0)     1105 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/dataset/components/TupleInputPart.tsx
--rw-r--r--   0 root         (0) root         (0)     5736 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/dataset/helpers.ts
--rw-r--r--   0 root         (0) root         (0)     3603 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/dataset/reducers.ts
--rw-r--r--   0 root         (0) root         (0)     4432 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/dataset/sagas.ts
--rw-r--r--   0 root         (0) root         (0)      639 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/dataset/types.ts
--rw-r--r--   0 root         (0) root         (0)     1825 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/dataset/validate.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:01.990692 libertem-0.9.0/client/src/errors/
--rw-r--r--   0 root         (0) root         (0)      534 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/errors/actions.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:01.991692 libertem-0.9.0/client/src/errors/components/
--rw-r--r--   0 root         (0) root         (0)      726 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/errors/components/Error.tsx
--rw-r--r--   0 root         (0) root         (0)     1165 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/errors/components/ErrorList.tsx
--rw-r--r--   0 root         (0) root         (0)      395 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/errors/helpers.ts
--rw-r--r--   0 root         (0) root         (0)     1696 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/errors/reducers.ts
--rw-r--r--   0 root         (0) root         (0)        0 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/errors/sagas.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:01.994692 libertem-0.9.0/client/src/helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:01.995692 libertem-0.9.0/client/src/helpers/__tests__/
--rw-r--r--   0 root         (0) root         (0)      926 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/helpers/__tests__/reducerHelpers.ts
--rw-r--r--   0 root         (0) root         (0)     1029 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/helpers/actionHelpers.ts
--rw-r--r--   0 root         (0) root         (0)     1102 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/helpers/apiHelpers.ts
--rw-r--r--   0 root         (0) root         (0)      444 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/helpers/hooks.ts
--rw-r--r--   0 root         (0) root         (0)      714 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/helpers/index.ts
--rw-r--r--   0 root         (0) root         (0)       59 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/helpers/props.ts
--rw-r--r--   0 root         (0) root         (0)     3259 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/helpers/reducerHelpers.ts
--rw-r--r--   0 root         (0) root         (0)     1355 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/helpers/svg.ts
--rw-r--r--   0 root         (0) root         (0)      227 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/helpers/types.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:01.995692 libertem-0.9.0/client/src/images/
--rw-r--r--   0 root         (0) root         (0)    11743 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/images/LiberTEM logo-medium.png
--rw-r--r--   0 root         (0) root         (0)      837 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/index.tsx
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:01.996692 libertem-0.9.0/client/src/job/
--rw-r--r--   0 root         (0) root         (0)      429 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/job/actions.ts
--rw-r--r--   0 root         (0) root         (0)      577 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/job/api.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:01.999692 libertem-0.9.0/client/src/job/components/
--rw-r--r--   0 root         (0) root         (0)     1523 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/job/components/PlaceholderImage.tsx
--rw-r--r--   0 root         (0) root         (0)     1712 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/job/components/Result.tsx
--rw-r--r--   0 root         (0) root         (0)      177 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/job/components/ResultImage.module.css
--rw-r--r--   0 root         (0) root         (0)      696 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/job/components/ResultImage.tsx
--rw-r--r--   0 root         (0) root         (0)     4486 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/job/components/ResultList.tsx
--rw-r--r--   0 root         (0) root         (0)      168 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/job/components/Selectors.tsx
--rw-r--r--   0 root         (0) root         (0)     3276 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/job/reducers.ts
--rw-r--r--   0 root         (0) root         (0)      816 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/job/types.ts
--rw-r--r--   0 root         (0) root         (0)    15174 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/messages.ts
--rw-r--r--   0 root         (0) root         (0)       40 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/react-app-env.d.ts
--rw-r--r--   0 root         (0) root         (0)     4526 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/registerServiceWorker.ts
--rw-r--r--   0 root         (0) root         (0)      592 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/sagas.ts
--rw-r--r--   0 root         (0) root         (0)      195 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/setupProxy.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:01.999692 libertem-0.9.0/client/src/shutdown/
--rw-r--r--   0 root         (0) root         (0)      227 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/shutdown/api.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:01.999692 libertem-0.9.0/client/src/shutdown/components/
--rw-r--r--   0 root         (0) root         (0)     2785 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/shutdown/components/ShutdownButton.tsx
--rw-r--r--   0 root         (0) root         (0)     1025 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/store.ts
--rw-r--r--   0 root         (0) root         (0)        0 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/vendor.d.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.004692 libertem-0.9.0/client/src/widgets/
--rw-r--r--   0 root         (0) root         (0)      453 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/widgets/BusySpinner.tsx
--rw-r--r--   0 root         (0) root         (0)      432 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/widgets/BusyWrapper.tsx
--rw-r--r--   0 root         (0) root         (0)      366 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/widgets/Disk.tsx
--rw-r--r--   0 root         (0) root         (0)     7306 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/widgets/DraggableHandle.tsx
--rw-r--r--   0 root         (0) root         (0)     2460 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/widgets/HandleParent.tsx
--rw-r--r--   0 root         (0) root         (0)      753 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/widgets/Rect.tsx
--rw-r--r--   0 root         (0) root         (0)      707 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/widgets/Ring.tsx
--rw-r--r--   0 root         (0) root         (0)      329 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/widgets/compose.tsx
--rw-r--r--   0 root         (0) root         (0)     1276 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/widgets/constraints.ts
--rw-r--r--   0 root         (0) root         (0)     1167 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/widgets/kbdHandler.ts
--rw-r--r--   0 root         (0) root         (0)      239 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/widgets/styles.ts
--rw-r--r--   0 root         (0) root         (0)      351 2022-02-16 12:09:30.000000 libertem-0.9.0/client/src/widgets/types.ts
--rw-r--r--   0 root         (0) root         (0)      576 2022-02-16 12:09:30.000000 libertem-0.9.0/client/tsconfig.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.004692 libertem-0.9.0/client/types/
--rw-r--r--   0 root         (0) root         (0)      937 2022-02-16 12:09:30.000000 libertem-0.9.0/client/types/react-window.d.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:01.907693 libertem-0.9.0/libertem/
--rw-r--r--   0 root         (0) root         (0)       53 2022-02-17 15:59:01.910693 libertem-0.9.0/libertem/_baked_revision.py
--rw-r--r--   0 root         (0) root         (0)       82 2022-02-16 12:09:30.000000 libertem-0.9.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      546 2022-02-17 15:59:02.157690 libertem-0.9.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     6681 2022-02-16 12:09:30.000000 libertem-0.9.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:01.919692 libertem-0.9.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.009692 libertem-0.9.0/src/libertem/
--rw-r--r--   0 root         (0) root         (0)      323 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.014691 libertem-0.9.0/src/libertem/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      344 2022-02-16 12:39:43.000000 libertem-0.9.0/src/libertem/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)      163 2022-02-16 12:39:43.000000 libertem-0.9.0/src/libertem/__pycache__/__version__.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    42813 2022-02-16 12:39:45.000000 libertem-0.9.0/src/libertem/__pycache__/api.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)      380 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/__pycache__/exceptions.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    11654 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/__pycache__/masks.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)      508 2022-02-16 12:39:43.000000 libertem-0.9.0/src/libertem/__pycache__/versioning.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)      746 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/__pycache__/warnings.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)       22 2022-02-17 15:47:41.000000 libertem-0.9.0/src/libertem/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.024691 libertem-0.9.0/src/libertem/analysis/
--rw-r--r--   0 root         (0) root         (0)      877 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/analysis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.035691 libertem-0.9.0/src/libertem/analysis/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      916 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/analysis/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     2717 2022-02-16 12:39:47.000000 libertem-0.9.0/src/libertem/analysis/__pycache__/apply_fft_mask.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    12578 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/analysis/__pycache__/base.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     7174 2022-02-16 12:39:47.000000 libertem-0.9.0/src/libertem/analysis/__pycache__/clust.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    18301 2022-02-16 12:39:47.000000 libertem-0.9.0/src/libertem/analysis/__pycache__/com.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     3182 2022-02-16 12:39:47.000000 libertem-0.9.0/src/libertem/analysis/__pycache__/disk.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     2888 2022-02-16 12:39:47.000000 libertem-0.9.0/src/libertem/analysis/__pycache__/fem.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    13853 2022-02-16 12:39:47.000000 libertem-0.9.0/src/libertem/analysis/__pycache__/fullmatch.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)      627 2022-02-16 12:39:47.000000 libertem-0.9.0/src/libertem/analysis/__pycache__/getroi.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    17165 2022-02-16 12:39:47.000000 libertem-0.9.0/src/libertem/analysis/__pycache__/gridmatching.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     3238 2022-02-16 12:39:47.000000 libertem-0.9.0/src/libertem/analysis/__pycache__/helper.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     7941 2022-02-16 12:39:47.000000 libertem-0.9.0/src/libertem/analysis/__pycache__/masks.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     3099 2022-02-16 12:39:47.000000 libertem-0.9.0/src/libertem/analysis/__pycache__/point.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    10082 2022-02-16 12:39:47.000000 libertem-0.9.0/src/libertem/analysis/__pycache__/radialfourier.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     6310 2022-02-16 12:39:47.000000 libertem-0.9.0/src/libertem/analysis/__pycache__/raw.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     2584 2022-02-16 12:39:47.000000 libertem-0.9.0/src/libertem/analysis/__pycache__/rawfft.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     3098 2022-02-16 12:39:47.000000 libertem-0.9.0/src/libertem/analysis/__pycache__/ring.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     3105 2022-02-16 12:39:47.000000 libertem-0.9.0/src/libertem/analysis/__pycache__/sd.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     5332 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/analysis/__pycache__/sum.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     2777 2022-02-16 12:39:47.000000 libertem-0.9.0/src/libertem/analysis/__pycache__/sumfft.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     2489 2022-02-16 12:39:47.000000 libertem-0.9.0/src/libertem/analysis/__pycache__/sumsig.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     2030 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/analysis/apply_fft_mask.py
--rw-r--r--   0 root         (0) root         (0)    11471 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/analysis/base.py
--rw-r--r--   0 root         (0) root         (0)     7864 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/analysis/clust.py
--rw-r--r--   0 root         (0) root         (0)    22450 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/analysis/com.py
--rw-r--r--   0 root         (0) root         (0)     2371 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/analysis/disk.py
--rw-r--r--   0 root         (0) root         (0)     2200 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/analysis/fem.py
--rw-r--r--   0 root         (0) root         (0)    16383 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/analysis/fullmatch.py
--rw-r--r--   0 root         (0) root         (0)      669 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/analysis/getroi.py
--rw-r--r--   0 root         (0) root         (0)    18296 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/analysis/gridmatching.py
--rw-r--r--   0 root         (0) root         (0)     2593 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/analysis/helper.py
--rw-r--r--   0 root         (0) root         (0)     7319 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/analysis/masks.py
--rw-r--r--   0 root         (0) root         (0)     2145 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/analysis/point.py
--rw-r--r--   0 root         (0) root         (0)    12805 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/analysis/radialfourier.py
--rw-r--r--   0 root         (0) root         (0)     5522 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/analysis/raw.py
--rw-r--r--   0 root         (0) root         (0)     2008 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/analysis/rawfft.py
--rw-r--r--   0 root         (0) root         (0)     2385 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/analysis/ring.py
--rw-r--r--   0 root         (0) root         (0)     2659 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/analysis/sd.py
--rw-r--r--   0 root         (0) root         (0)     4987 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/analysis/sum.py
--rw-r--r--   0 root         (0) root         (0)     2280 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/analysis/sumfft.py
--rw-r--r--   0 root         (0) root         (0)     1687 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/analysis/sumsig.py
--rw-r--r--   0 root         (0) root         (0)    49144 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/api.py
--rw-r--r--   0 root         (0) root         (0)      165 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/cli_tweaks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.039691 libertem-0.9.0/src/libertem/common/
--rw-r--r--   0 root         (0) root         (0)     1151 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/common/LICENSE
--rw-r--r--   0 root         (0) root         (0)       80 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.041691 libertem-0.9.0/src/libertem/common/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      242 2022-02-16 12:39:45.000000 libertem-0.9.0/src/libertem/common/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     2272 2022-02-16 12:39:45.000000 libertem-0.9.0/src/libertem/common/__pycache__/backend.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    22758 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/common/__pycache__/buffers.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     6694 2022-02-16 12:39:47.000000 libertem-0.9.0/src/libertem/common/__pycache__/container.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)      878 2022-02-16 12:39:45.000000 libertem-0.9.0/src/libertem/common/__pycache__/math.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     6637 2022-02-16 12:39:45.000000 libertem-0.9.0/src/libertem/common/__pycache__/shape.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    11764 2022-02-16 12:39:45.000000 libertem-0.9.0/src/libertem/common/__pycache__/slice.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     2754 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/common/backend.py
--rw-r--r--   0 root         (0) root         (0)    23927 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/common/buffers.py
--rw-r--r--   0 root         (0) root         (0)     8911 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/common/container.py
--rw-r--r--   0 root         (0) root         (0)      766 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/common/math.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.042691 libertem-0.9.0/src/libertem/common/numba/
--rw-r--r--   0 root         (0) root         (0)     5523 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/common/numba/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.043691 libertem-0.9.0/src/libertem/common/numba/__pycache__/
--rw-r--r--   0 root         (0) root         (0)     4297 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/common/numba/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     4712 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/common/numba/__pycache__/cache.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     5905 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/common/numba/cache.py
--rw-r--r--   0 root         (0) root         (0)     5434 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/common/shape.py
--rw-r--r--   0 root         (0) root         (0)    12476 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/common/slice.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.043691 libertem-0.9.0/src/libertem/contrib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.044691 libertem-0.9.0/src/libertem/contrib/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      779 2022-02-16 13:34:18.000000 libertem-0.9.0/src/libertem/contrib/__pycache__/daskadapter.cpython-38.pyc
--rw-r--r--   0 root         (0) root         (0)      777 2022-02-16 12:34:51.000000 libertem-0.9.0/src/libertem/contrib/__pycache__/daskadapter.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)      698 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/contrib/daskadapter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.046691 libertem-0.9.0/src/libertem/corrections/
--rw-r--r--   0 root         (0) root         (0)       64 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/corrections/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.047691 libertem-0.9.0/src/libertem/corrections/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      215 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/corrections/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     1066 2022-02-16 12:39:47.000000 libertem-0.9.0/src/libertem/corrections/__pycache__/coordinates.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     7038 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/corrections/__pycache__/corrset.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     8409 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/corrections/__pycache__/detector.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)      810 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/corrections/coordinates.py
--rw-r--r--   0 root         (0) root         (0)    10366 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/corrections/corrset.py
--rw-r--r--   0 root         (0) root         (0)    11538 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/corrections/detector.py
--rw-r--r--   0 root         (0) root         (0)      109 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.052691 libertem-0.9.0/src/libertem/executor/
--rw-r--r--   0 root         (0) root         (0)        0 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/executor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.054691 libertem-0.9.0/src/libertem/executor/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      145 2022-02-16 12:39:44.000000 libertem-0.9.0/src/libertem/executor/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    15943 2022-02-16 12:39:45.000000 libertem-0.9.0/src/libertem/executor/__pycache__/base.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     6054 2022-02-16 12:39:45.000000 libertem-0.9.0/src/libertem/executor/__pycache__/concurrent.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    20442 2022-02-16 12:39:44.000000 libertem-0.9.0/src/libertem/executor/__pycache__/dask.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    15699 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/executor/__pycache__/delayed.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     3154 2022-02-16 12:39:45.000000 libertem-0.9.0/src/libertem/executor/__pycache__/inline.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     1975 2022-02-16 12:39:45.000000 libertem-0.9.0/src/libertem/executor/__pycache__/integration.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     6114 2022-02-16 12:39:45.000000 libertem-0.9.0/src/libertem/executor/__pycache__/scheduler.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    13307 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/executor/base.py
--rw-r--r--   0 root         (0) root         (0)     3309 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/executor/cli.py
--rw-r--r--   0 root         (0) root         (0)     5308 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/executor/concurrent.py
--rw-r--r--   0 root         (0) root         (0)    22579 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/executor/dask.py
--rw-r--r--   0 root         (0) root         (0)    17893 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/executor/delayed.py
--rw-r--r--   0 root         (0) root         (0)     2569 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/executor/inline.py
--rw-r--r--   0 root         (0) root         (0)     2563 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/executor/integration.py
--rw-r--r--   0 root         (0) root         (0)     3506 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/executor/scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.056691 libertem-0.9.0/src/libertem/executor/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/executor/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.058691 libertem-0.9.0/src/libertem/executor/utils/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      151 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/executor/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     7850 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/executor/utils/__pycache__/dask_buffer.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     6285 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/executor/utils/__pycache__/dask_inplace.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     9234 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/executor/utils/__pycache__/delayed_unpack.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     7683 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/executor/utils/dask_buffer.py
--rw-r--r--   0 root         (0) root         (0)     7648 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/executor/utils/dask_inplace.py
--rw-r--r--   0 root         (0) root         (0)    10183 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/executor/utils/delayed_unpack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.060691 libertem-0.9.0/src/libertem/io/
--rw-r--r--   0 root         (0) root         (0)     1151 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/LICENSE
--rw-r--r--   0 root         (0) root         (0)        0 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.061691 libertem-0.9.0/src/libertem/io/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      139 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/io/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     1480 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/io/__pycache__/utils.cpython-39.pyc
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.069691 libertem-0.9.0/src/libertem/io/dataset/
--rw-r--r--   0 root         (0) root         (0)     5726 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/dataset/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.077691 libertem-0.9.0/src/libertem/io/dataset/__pycache__/
--rw-r--r--   0 root         (0) root         (0)     5443 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/io/dataset/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     8002 2022-02-16 12:39:49.000000 libertem-0.9.0/src/libertem/io/dataset/__pycache__/blo.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    19877 2022-02-16 12:39:47.000000 libertem-0.9.0/src/libertem/io/dataset/__pycache__/cached.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     9877 2022-02-16 12:39:47.000000 libertem-0.9.0/src/libertem/io/dataset/__pycache__/cluster.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    21540 2022-02-16 12:39:50.000000 libertem-0.9.0/src/libertem/io/dataset/__pycache__/dask.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    10507 2022-02-16 12:39:49.000000 libertem-0.9.0/src/libertem/io/dataset/__pycache__/dm.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     8743 2022-02-16 12:39:49.000000 libertem-0.9.0/src/libertem/io/dataset/__pycache__/empad.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    20542 2022-02-16 12:39:49.000000 libertem-0.9.0/src/libertem/io/dataset/__pycache__/frms6.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    23751 2022-02-16 12:39:49.000000 libertem-0.9.0/src/libertem/io/dataset/__pycache__/hdf5.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    34341 2022-02-16 12:39:49.000000 libertem-0.9.0/src/libertem/io/dataset/__pycache__/k2is.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    10765 2022-02-16 12:39:49.000000 libertem-0.9.0/src/libertem/io/dataset/__pycache__/memory.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    33199 2022-02-16 12:39:47.000000 libertem-0.9.0/src/libertem/io/dataset/__pycache__/mib.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     8240 2022-02-16 12:39:49.000000 libertem-0.9.0/src/libertem/io/dataset/__pycache__/mrc.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     7620 2022-02-16 12:39:47.000000 libertem-0.9.0/src/libertem/io/dataset/__pycache__/raw.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    18639 2022-02-16 12:39:49.000000 libertem-0.9.0/src/libertem/io/dataset/__pycache__/seq.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    10309 2022-02-16 12:39:49.000000 libertem-0.9.0/src/libertem/io/dataset/__pycache__/ser.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    13560 2022-02-16 12:39:49.000000 libertem-0.9.0/src/libertem/io/dataset/__pycache__/tvips.cpython-39.pyc
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.082691 libertem-0.9.0/src/libertem/io/dataset/base/
--rw-r--r--   0 root         (0) root         (0)     1271 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/dataset/base/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.089691 libertem-0.9.0/src/libertem/io/dataset/base/__pycache__/
--rw-r--r--   0 root         (0) root         (0)     1312 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/io/dataset/base/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     5300 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/io/dataset/base/__pycache__/backend.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    11278 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/io/dataset/base/__pycache__/backend_buffered.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     1922 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/io/dataset/base/__pycache__/backend_direct.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    11264 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/io/dataset/base/__pycache__/backend_mmap.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     1576 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/io/dataset/base/__pycache__/coordinates.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    10961 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/io/dataset/base/__pycache__/dataset.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     5547 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/io/dataset/base/__pycache__/decode.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)      325 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/io/dataset/base/__pycache__/exceptions.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     5585 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/io/dataset/base/__pycache__/file.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     3522 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/io/dataset/base/__pycache__/fileset.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     4490 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/io/dataset/base/__pycache__/meta.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     9157 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/io/dataset/base/__pycache__/partition.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     2099 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/io/dataset/base/__pycache__/roi.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     7865 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/io/dataset/base/__pycache__/tiling.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    14230 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/io/dataset/base/__pycache__/tiling_scheme.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     2479 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/io/dataset/base/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     5117 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/dataset/base/backend.py
--rw-r--r--   0 root         (0) root         (0)    15021 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/dataset/base/backend_buffered.py
--rw-r--r--   0 root         (0) root         (0)     1347 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/dataset/base/backend_direct.py
--rw-r--r--   0 root         (0) root         (0)    12823 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/dataset/base/backend_mmap.py
--rw-r--r--   0 root         (0) root         (0)     1535 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/dataset/base/coordinates.py
--rw-r--r--   0 root         (0) root         (0)    10241 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/dataset/base/dataset.py
--rw-r--r--   0 root         (0) root         (0)     5044 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/dataset/base/decode.py
--rw-r--r--   0 root         (0) root         (0)       44 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/dataset/base/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     5680 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/dataset/base/file.py
--rw-r--r--   0 root         (0) root         (0)     3159 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/dataset/base/fileset.py
--rw-r--r--   0 root         (0) root         (0)     4217 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/dataset/base/meta.py
--rw-r--r--   0 root         (0) root         (0)     8726 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/dataset/base/partition.py
--rw-r--r--   0 root         (0) root         (0)     1845 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/dataset/base/roi.py
--rw-r--r--   0 root         (0) root         (0)    11867 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/dataset/base/tiling.py
--rw-r--r--   0 root         (0) root         (0)    17722 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/dataset/base/tiling_scheme.py
--rw-r--r--   0 root         (0) root         (0)     2232 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/dataset/base/utils.py
--rw-r--r--   0 root         (0) root         (0)     8726 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/dataset/blo.py
--rw-r--r--   0 root         (0) root         (0)    18746 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/dataset/cached.py
--rw-r--r--   0 root         (0) root         (0)     8456 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/dataset/cluster.py
--rw-r--r--   0 root         (0) root         (0)    21163 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/dataset/dask.py
--rw-r--r--   0 root         (0) root         (0)    10195 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/dataset/dm.py
--rw-r--r--   0 root         (0) root         (0)     9356 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/dataset/empad.py
--rw-r--r--   0 root         (0) root         (0)    23589 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/dataset/frms6.py
--rw-r--r--   0 root         (0) root         (0)    28043 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/dataset/hdf5.py
--rw-r--r--   0 root         (0) root         (0)    37600 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/dataset/k2is.py
--rw-r--r--   0 root         (0) root         (0)    13036 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/dataset/memory.py
--rw-r--r--   0 root         (0) root         (0)    44457 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/dataset/mib.py
--rw-r--r--   0 root         (0) root         (0)     7380 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/dataset/mrc.py
--rw-r--r--   0 root         (0) root         (0)     8609 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/dataset/raw.py
--rw-r--r--   0 root         (0) root         (0)    23010 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/dataset/seq.py
--rw-r--r--   0 root         (0) root         (0)    10454 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/dataset/ser.py
--rw-r--r--   0 root         (0) root         (0)    17844 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/dataset/tvips.py
--rw-r--r--   0 root         (0) root         (0)      491 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/direct.py
--rw-r--r--   0 root         (0) root         (0)     3242 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/fs.py
--rw-r--r--   0 root         (0) root         (0)     1717 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.090691 libertem-0.9.0/src/libertem/io/writers/
--rw-r--r--   0 root         (0) root         (0)        0 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/writers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.091691 libertem-0.9.0/src/libertem/io/writers/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      147 2022-02-16 12:39:48.000000 libertem-0.9.0/src/libertem/io/writers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     4120 2022-02-16 12:39:48.000000 libertem-0.9.0/src/libertem/io/writers/__pycache__/base.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     4264 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/writers/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.092691 libertem-0.9.0/src/libertem/io/writers/results/
--rw-r--r--   0 root         (0) root         (0)        0 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/writers/results/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.093691 libertem-0.9.0/src/libertem/io/writers/results/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      155 2022-02-16 12:39:48.000000 libertem-0.9.0/src/libertem/io/writers/results/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     2838 2022-02-16 12:39:48.000000 libertem-0.9.0/src/libertem/io/writers/results/__pycache__/base.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     5371 2022-02-16 12:39:48.000000 libertem-0.9.0/src/libertem/io/writers/results/__pycache__/formats.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     1801 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/writers/results/base.py
--rw-r--r--   0 root         (0) root         (0)     2996 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/io/writers/results/formats.py
--rw-r--r--   0 root         (0) root         (0)    13962 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/masks.py
--rw-r--r--   0 root         (0) root         (0)      536 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/preload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.097691 libertem-0.9.0/src/libertem/udf/
--rw-r--r--   0 root         (0) root         (0)     2696 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/udf/FEM.py
--rw-r--r--   0 root         (0) root         (0)      349 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/udf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.102691 libertem-0.9.0/src/libertem/udf/__pycache__/
--rw-r--r--   0 root         (0) root         (0)     3059 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/udf/__pycache__/FEM.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)      470 2022-02-16 12:39:45.000000 libertem-0.9.0/src/libertem/udf/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     2115 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/udf/__pycache__/auto.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    71195 2022-02-16 12:39:45.000000 libertem-0.9.0/src/libertem/udf/__pycache__/base.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     4189 2022-02-16 12:39:47.000000 libertem-0.9.0/src/libertem/udf/__pycache__/crystallinity.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     6012 2022-02-16 12:39:47.000000 libertem-0.9.0/src/libertem/udf/__pycache__/holography.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     2478 2022-02-16 12:39:50.000000 libertem-0.9.0/src/libertem/udf/__pycache__/logsum.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     7236 2022-02-16 12:39:47.000000 libertem-0.9.0/src/libertem/udf/__pycache__/masks.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     2371 2022-02-16 12:39:47.000000 libertem-0.9.0/src/libertem/udf/__pycache__/raw.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    12890 2022-02-16 12:39:47.000000 libertem-0.9.0/src/libertem/udf/__pycache__/stddev.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     2197 2022-02-16 12:39:47.000000 libertem-0.9.0/src/libertem/udf/__pycache__/sum.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     1283 2022-02-16 12:39:47.000000 libertem-0.9.0/src/libertem/udf/__pycache__/sumsigudf.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     1826 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/udf/auto.py
--rw-r--r--   0 root         (0) root         (0)    74248 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/udf/base.py
--rw-r--r--   0 root         (0) root         (0)     4268 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/udf/crystallinity.py
--rw-r--r--   0 root         (0) root         (0)     7396 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/udf/holography.py
--rw-r--r--   0 root         (0) root         (0)     1619 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/udf/logsum.py
--rw-r--r--   0 root         (0) root         (0)     7952 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/udf/masks.py
--rw-r--r--   0 root         (0) root         (0)     2281 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/udf/raw.py
--rw-r--r--   0 root         (0) root         (0)    14913 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/udf/stddev.py
--rw-r--r--   0 root         (0) root         (0)     1316 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/udf/sum.py
--rw-r--r--   0 root         (0) root         (0)      791 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/udf/sumsigudf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.105691 libertem-0.9.0/src/libertem/utils/
--rw-r--r--   0 root         (0) root         (0)     4665 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.107691 libertem-0.9.0/src/libertem/utils/__pycache__/
--rw-r--r--   0 root         (0) root         (0)     4826 2022-02-16 12:39:45.000000 libertem-0.9.0/src/libertem/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     7639 2022-02-16 12:39:45.000000 libertem-0.9.0/src/libertem/utils/__pycache__/async_utils.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     1841 2022-02-16 12:39:45.000000 libertem-0.9.0/src/libertem/utils/__pycache__/devices.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     4706 2022-02-16 12:39:47.000000 libertem-0.9.0/src/libertem/utils/__pycache__/generate.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     7033 2022-02-16 12:39:45.000000 libertem-0.9.0/src/libertem/utils/__pycache__/threading.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     8361 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/utils/async_utils.py
--rw-r--r--   0 root         (0) root         (0)     1682 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/utils/devices.py
--rw-r--r--   0 root         (0) root         (0)     5171 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/utils/generate.py
--rw-r--r--   0 root         (0) root         (0)     9956 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/utils/threading.py
--rw-r--r--   0 root         (0) root         (0)      351 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/versioning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.109691 libertem-0.9.0/src/libertem/viz/
--rw-r--r--   0 root         (0) root         (0)      848 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/viz/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.111691 libertem-0.9.0/src/libertem/viz/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      739 2022-02-16 12:39:48.000000 libertem-0.9.0/src/libertem/viz/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     9870 2022-02-16 12:39:49.000000 libertem-0.9.0/src/libertem/viz/__pycache__/base.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     3964 2022-02-16 12:39:50.000000 libertem-0.9.0/src/libertem/viz/__pycache__/bqp.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     3627 2022-02-16 12:39:50.000000 libertem-0.9.0/src/libertem/viz/__pycache__/gms.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     3765 2022-02-16 12:39:50.000000 libertem-0.9.0/src/libertem/viz/__pycache__/mpl.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    10612 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/viz/base.py
--rw-r--r--   0 root         (0) root         (0)     4320 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/viz/bqp.py
--rw-r--r--   0 root         (0) root         (0)     3497 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/viz/gms.py
--rw-r--r--   0 root         (0) root         (0)     3695 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/viz/mpl.py
--rw-r--r--   0 root         (0) root         (0)      473 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/warnings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.118691 libertem-0.9.0/src/libertem/web/
--rw-r--r--   0 root         (0) root         (0)        0 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.121690 libertem-0.9.0/src/libertem/web/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      140 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/web/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     1728 2022-02-16 12:39:46.000000 libertem-0.9.0/src/libertem/web/__pycache__/messageconverter.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     6681 2022-02-16 12:39:47.000000 libertem-0.9.0/src/libertem/web/__pycache__/messages.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     2280 2022-02-16 12:39:47.000000 libertem-0.9.0/src/libertem/web/__pycache__/models.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     4293 2022-02-16 12:39:47.000000 libertem-0.9.0/src/libertem/web/__pycache__/rpc.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)    16039 2022-02-16 12:39:47.000000 libertem-0.9.0/src/libertem/web/__pycache__/state.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     7081 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/analysis.py
--rw-r--r--   0 root         (0) root         (0)     1511 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/base.py
--rw-r--r--   0 root         (0) root         (0)      985 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/browse.py
--rw-r--r--   0 root         (0) root         (0)     2471 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.123690 libertem-0.9.0/src/libertem/web/client/
--rw-r--r--   0 root         (0) root         (0)     1365 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/client/asset-manifest.json
--rw-r--r--   0 root         (0) root         (0)    15086 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/client/favicon.ico
--rw-r--r--   0 root         (0) root         (0)     2199 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/client/index.html
--rw-r--r--   0 root         (0) root         (0)      295 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/client/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:01.928692 libertem-0.9.0/src/libertem/web/client/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.129690 libertem-0.9.0/src/libertem/web/client/static/css/
--rw-r--r--   0 root         (0) root         (0)   579793 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/client/static/css/2.42a8572e.chunk.css
--rw-r--r--   0 root         (0) root         (0)  1404626 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/client/static/css/2.42a8572e.chunk.css.map
--rw-r--r--   0 root         (0) root         (0)      295 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/client/static/css/main.c0d8de42.chunk.css
--rw-r--r--   0 root         (0) root         (0)      448 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/client/static/css/main.c0d8de42.chunk.css.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.139690 libertem-0.9.0/src/libertem/web/client/static/js/
--rw-r--r--   0 root         (0) root         (0)   668351 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/client/static/js/2.6b575192.chunk.js
--rw-r--r--   0 root         (0) root         (0)     2093 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/client/static/js/2.6b575192.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)  3041745 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/client/static/js/2.6b575192.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)   152198 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/client/static/js/main.2e050bba.chunk.js
--rw-r--r--   0 root         (0) root         (0)   508286 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/client/static/js/main.2e050bba.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)     1585 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/client/static/js/runtime-main.fcac4e81.js
--rw-r--r--   0 root         (0) root         (0)     8298 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/client/static/js/runtime-main.fcac4e81.js.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.153690 libertem-0.9.0/src/libertem/web/client/static/media/
--rw-r--r--   0 root         (0) root         (0)    11743 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/client/static/media/LiberTEM logo-medium.2765b438.png
--rw-r--r--   0 root         (0) root         (0)    54488 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/client/static/media/brand-icons.278156e4.woff2
--rw-r--r--   0 root         (0) root         (0)    98404 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/client/static/media/brand-icons.65a2fb6d.ttf
--rw-r--r--   0 root         (0) root         (0)   507628 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/client/static/media/brand-icons.6729d297.svg
--rw-r--r--   0 root         (0) root         (0)    63728 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/client/static/media/brand-icons.cac87dc0.woff
--rw-r--r--   0 root         (0) root         (0)    98640 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/client/static/media/brand-icons.d68fa3e6.eot
--rw-r--r--   0 root         (0) root         (0)    28123 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/client/static/media/flags.99f63ae7.png
--rw-r--r--   0 root         (0) root         (0)    40148 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/client/static/media/icons.38c6d8ba.woff2
--rw-r--r--   0 root         (0) root         (0)    50524 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/client/static/media/icons.425399f8.woff
--rw-r--r--   0 root         (0) root         (0)   390837 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/client/static/media/icons.62d9dae4.svg
--rw-r--r--   0 root         (0) root         (0)   106004 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/client/static/media/icons.a01e3f2d.eot
--rw-r--r--   0 root         (0) root         (0)   105784 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/client/static/media/icons.c656b8ca.ttf
--rw-r--r--   0 root         (0) root         (0)    30928 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/client/static/media/outline-icons.53671035.ttf
--rw-r--r--   0 root         (0) root         (0)    12240 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/client/static/media/outline-icons.687a4990.woff2
--rw-r--r--   0 root         (0) root         (0)    31156 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/client/static/media/outline-icons.752905fa.eot
--rw-r--r--   0 root         (0) root         (0)   107201 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/client/static/media/outline-icons.9c4845b4.svg
--rw-r--r--   0 root         (0) root         (0)    14712 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/client/static/media/outline-icons.ddae9b1b.woff
--rw-r--r--   0 root         (0) root         (0)     1071 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/config.py
--rw-r--r--   0 root         (0) root         (0)     3573 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/connect.py
--rw-r--r--   0 root         (0) root         (0)     4201 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/dataset.py
--rw-r--r--   0 root         (0) root         (0)     9381 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/engine.py
--rw-r--r--   0 root         (0) root         (0)     2378 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/events.py
--rw-r--r--   0 root         (0) root         (0)     2385 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/generator.py
--rw-r--r--   0 root         (0) root         (0)     1564 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/jobs.py
--rw-r--r--   0 root         (0) root         (0)     1348 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/messageconverter.py
--rw-r--r--   0 root         (0) root         (0)     6696 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/messages.py
--rw-r--r--   0 root         (0) root         (0)     1156 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.154690 libertem-0.9.0/src/libertem/web/notebook_generator/
--rw-r--r--   0 root         (0) root         (0)        0 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/notebook_generator/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.155690 libertem-0.9.0/src/libertem/web/notebook_generator/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      159 2022-02-16 12:39:47.000000 libertem-0.9.0/src/libertem/web/notebook_generator/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     1664 2022-02-16 12:39:47.000000 libertem-0.9.0/src/libertem/web/notebook_generator/__pycache__/template.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)     4262 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/notebook_generator/code_template.py
--rw-r--r--   0 root         (0) root         (0)      514 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/notebook_generator/copy.py
--rw-r--r--   0 root         (0) root         (0)     1378 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/notebook_generator/notebook_generator.py
--rw-r--r--   0 root         (0) root         (0)     1323 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/notebook_generator/template.py
--rw-r--r--   0 root         (0) root         (0)     3300 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/rpc.py
--rw-r--r--   0 root         (0) root         (0)     7460 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/server.py
--rw-r--r--   0 root         (0) root         (0)      691 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/shutdown.py
--rw-r--r--   0 root         (0) root         (0)    13476 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/web/state.py
--rw-r--r--   0 root         (0) root         (0)     2488 2022-02-16 12:09:30.000000 libertem-0.9.0/src/libertem/win_tweaks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:59:02.011691 libertem-0.9.0/src/libertem.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10657 2022-02-17 15:59:01.000000 libertem-0.9.0/src/libertem.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    21094 2022-02-17 15:59:01.000000 libertem-0.9.0/src/libertem.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-02-17 15:59:01.000000 libertem-0.9.0/src/libertem.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2022-02-17 15:59:01.000000 libertem-0.9.0/src/libertem.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-02-16 12:09:35.000000 libertem-0.9.0/src/libertem.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      440 2022-02-17 15:59:01.000000 libertem-0.9.0/src/libertem.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2022-02-17 15:59:01.000000 libertem-0.9.0/src/libertem.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.712914 libertem-0.9.2/
+-rw-r--r--   0 root         (0) root         (0)    35149 2022-04-26 10:50:39.000000 libertem-0.9.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      125 2022-04-26 10:50:39.000000 libertem-0.9.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    10657 2022-04-28 17:30:33.712914 libertem-0.9.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9331 2022-04-28 17:22:40.000000 libertem-0.9.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.607915 libertem-0.9.2/client/
+-rw-r--r--   0 root         (0) root         (0)     8275 2022-04-26 10:50:39.000000 libertem-0.9.2/client/.eslintrc.js
+-rw-r--r--   0 root         (0) root         (0)      285 2022-04-26 10:50:39.000000 libertem-0.9.2/client/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     9483 2022-04-26 10:50:39.000000 libertem-0.9.2/client/README.md
+-rw-r--r--   0 root         (0) root         (0)  1958343 2022-04-28 17:22:40.000000 libertem-0.9.2/client/package-lock.json
+-rw-r--r--   0 root         (0) root         (0)     1685 2022-04-28 17:22:40.000000 libertem-0.9.2/client/package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.608915 libertem-0.9.2/client/public/
+-rw-r--r--   0 root         (0) root         (0)    15086 2022-04-26 10:50:39.000000 libertem-0.9.2/client/public/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)     1589 2022-04-26 10:50:39.000000 libertem-0.9.2/client/public/index.html
+-rw-r--r--   0 root         (0) root         (0)      295 2022-04-26 10:50:39.000000 libertem-0.9.2/client/public/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.610915 libertem-0.9.2/client/src/
+-rw-r--r--   0 root         (0) root         (0)     2524 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/About.tsx
+-rw-r--r--   0 root         (0) root         (0)      274 2022-04-28 17:22:40.000000 libertem-0.9.2/client/src/App.test.tsx
+-rw-r--r--   0 root         (0) root         (0)      816 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/App.tsx
+-rw-r--r--   0 root         (0) root         (0)      846 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/Menu.tsx
+-rw-r--r--   0 root         (0) root         (0)      767 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/actions.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.610915 libertem-0.9.2/client/src/analysis/
+-rw-r--r--   0 root         (0) root         (0)     1307 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/analysis/actions.ts
+-rw-r--r--   0 root         (0) root         (0)     2987 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/analysis/reducers.ts
+-rw-r--r--   0 root         (0) root         (0)      268 2022-04-28 17:22:40.000000 libertem-0.9.2/client/src/analysis/types.ts
+-rw-r--r--   0 root         (0) root         (0)       58 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/basicTypes.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.611915 libertem-0.9.2/client/src/browser/
+-rw-r--r--   0 root         (0) root         (0)     1616 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/browser/actions.ts
+-rw-r--r--   0 root         (0) root         (0)      494 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/browser/api.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.613915 libertem-0.9.2/client/src/browser/components/
+-rw-r--r--   0 root         (0) root         (0)     1145 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/browser/components/BrowserWrapper.tsx
+-rw-r--r--   0 root         (0) root         (0)     3206 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/browser/components/FileBrowser.tsx
+-rw-r--r--   0 root         (0) root         (0)     3645 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/browser/components/FileBrowserEntry.tsx
+-rw-r--r--   0 root         (0) root         (0)     1079 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/browser/components/FileBrowserHeader.tsx
+-rw-r--r--   0 root         (0) root         (0)      987 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/browser/components/FileEntry.tsx
+-rw-r--r--   0 root         (0) root         (0)      970 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/browser/components/FolderEntry.tsx
+-rw-r--r--   0 root         (0) root         (0)     3487 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/browser/components/PathBar.tsx
+-rw-r--r--   0 root         (0) root         (0)      947 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/browser/components/PathDropDownItem.tsx
+-rw-r--r--   0 root         (0) root         (0)      990 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/browser/components/PathInput.tsx
+-rw-r--r--   0 root         (0) root         (0)     1864 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/browser/components/RecentFiles.tsx
+-rw-r--r--   0 root         (0) root         (0)     2083 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/browser/reducers.ts
+-rw-r--r--   0 root         (0) root         (0)     2773 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/browser/sagas.ts
+-rw-r--r--   0 root         (0) root         (0)      348 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/browser/types.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.614915 libertem-0.9.2/client/src/channel/
+-rw-r--r--   0 root         (0) root         (0)     2892 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/channel/actions.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.614915 libertem-0.9.2/client/src/channel/components/
+-rw-r--r--   0 root         (0) root         (0)      459 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/channel/components/ChannelConnecting.tsx
+-rw-r--r--   0 root         (0) root         (0)      397 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/channel/components/ChannelShutdown.tsx
+-rw-r--r--   0 root         (0) root         (0)     2141 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/channel/components/ChannelStatus.tsx
+-rw-r--r--   0 root         (0) root         (0)     4099 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/channel/messages.ts
+-rw-r--r--   0 root         (0) root         (0)     1084 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/channel/reducers.ts
+-rw-r--r--   0 root         (0) root         (0)     7858 2022-04-28 17:22:40.000000 libertem-0.9.2/client/src/channel/sagas.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.615915 libertem-0.9.2/client/src/cluster/
+-rw-r--r--   0 root         (0) root         (0)      855 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/cluster/actions.ts
+-rw-r--r--   0 root         (0) root         (0)      656 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/cluster/api.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.617915 libertem-0.9.2/client/src/cluster/components/
+-rw-r--r--   0 root         (0) root         (0)     2699 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/cluster/components/ClusterConnectionForm.tsx
+-rw-r--r--   0 root         (0) root         (0)     1570 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/cluster/components/GPUSelector.tsx
+-rw-r--r--   0 root         (0) root         (0)     3559 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/cluster/components/LocalConnectionForm.tsx
+-rw-r--r--   0 root         (0) root         (0)     1490 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/cluster/components/TCPConnectionForm.tsx
+-rw-r--r--   0 root         (0) root         (0)     1086 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/cluster/reducers.ts
+-rw-r--r--   0 root         (0) root         (0)     1615 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/cluster/sagas.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.618915 libertem-0.9.2/client/src/clusterStatus/
+-rw-r--r--   0 root         (0) root         (0)      440 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/clusterStatus/api.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.618915 libertem-0.9.2/client/src/clusterStatus/components/
+-rw-r--r--   0 root         (0) root         (0)     2564 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/clusterStatus/components/Cluster.tsx
+-rw-r--r--   0 root         (0) root         (0)     2207 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/clusterStatus/components/LocalStatus.tsx
+-rw-r--r--   0 root         (0) root         (0)      371 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/clusterStatus/components/NotConnected.tsx
+-rw-r--r--   0 root         (0) root         (0)     4498 2022-04-28 17:22:40.000000 libertem-0.9.2/client/src/clusterStatus/components/TCPStatus.tsx
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.619915 libertem-0.9.2/client/src/compoundAnalysis/
+-rw-r--r--   0 root         (0) root         (0)     2150 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/compoundAnalysis/actions.ts
+-rw-r--r--   0 root         (0) root         (0)     1916 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/compoundAnalysis/api.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.621915 libertem-0.9.2/client/src/compoundAnalysis/components/
+-rw-r--r--   0 root         (0) root         (0)    13922 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/compoundAnalysis/components/CenterOfMassAnalysis.tsx
+-rw-r--r--   0 root         (0) root         (0)     7633 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/compoundAnalysis/components/Clustering.tsx
+-rw-r--r--   0 root         (0) root         (0)     4394 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/compoundAnalysis/components/DefaultFrameView.tsx
+-rw-r--r--   0 root         (0) root         (0)     3837 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/compoundAnalysis/components/DiskMaskAnalysis.tsx
+-rw-r--r--   0 root         (0) root         (0)     8493 2022-04-28 17:22:40.000000 libertem-0.9.2/client/src/compoundAnalysis/components/Download.tsx
+-rw-r--r--   0 root         (0) root         (0)     4496 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/compoundAnalysis/components/FEM.tsx
+-rw-r--r--   0 root         (0) root         (0)     7148 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/compoundAnalysis/components/FFTAnalysis.tsx
+-rw-r--r--   0 root         (0) root         (0)     2005 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/compoundAnalysis/components/FFTFramePicker.tsx
+-rw-r--r--   0 root         (0) root         (0)     3020 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/compoundAnalysis/components/FFTFrameView.tsx
+-rw-r--r--   0 root         (0) root         (0)      910 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/compoundAnalysis/components/FFTSumFrames.tsx
+-rw-r--r--   0 root         (0) root         (0)     1911 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/compoundAnalysis/components/FramePicker.tsx
+-rw-r--r--   0 root         (0) root         (0)      639 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/compoundAnalysis/components/JustSum.tsx
+-rw-r--r--   0 root         (0) root         (0)      957 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/compoundAnalysis/components/ModeSelector.tsx
+-rw-r--r--   0 root         (0) root         (0)     3416 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/compoundAnalysis/components/PointSelectionAnalysis.tsx
+-rw-r--r--   0 root         (0) root         (0)     4643 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/compoundAnalysis/components/RadialFourierAnalysis.tsx
+-rw-r--r--   0 root         (0) root         (0)     4477 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/compoundAnalysis/components/RingMaskAnalysis.tsx
+-rw-r--r--   0 root         (0) root         (0)     1740 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/compoundAnalysis/components/Toolbar.tsx
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.621915 libertem-0.9.2/client/src/compoundAnalysis/components/base/
+-rw-r--r--   0 root         (0) root         (0)      898 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/compoundAnalysis/components/base/Analysis.tsx
+-rw-r--r--   0 root         (0) root         (0)      412 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/compoundAnalysis/components/base/AnalysisList.tsx
+-rw-r--r--   0 root         (0) root         (0)     1173 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/compoundAnalysis/components/base/AnalysisSelect.tsx
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.622915 libertem-0.9.2/client/src/compoundAnalysis/components/layouts/
+-rw-r--r--   0 root         (0) root         (0)     1907 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/compoundAnalysis/components/layouts/AnalysisLayoutThreeCol.tsx
+-rw-r--r--   0 root         (0) root         (0)     1162 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/compoundAnalysis/components/layouts/AnalysisLayoutTwoCol.tsx
+-rw-r--r--   0 root         (0) root         (0)     1954 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/compoundAnalysis/components/layouts/AnalysisLayoutTwoRes.tsx
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.622915 libertem-0.9.2/client/src/compoundAnalysis/components/roi/
+-rw-r--r--   0 root         (0) root         (0)     1942 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/compoundAnalysis/components/roi/DiskROI.tsx
+-rw-r--r--   0 root         (0) root         (0)     1943 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/compoundAnalysis/components/roi/RectROI.tsx
+-rw-r--r--   0 root         (0) root         (0)     1243 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/compoundAnalysis/components/roi/RoiPicker.tsx
+-rw-r--r--   0 root         (0) root         (0)      392 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/compoundAnalysis/getMetadata.tsx
+-rw-r--r--   0 root         (0) root         (0)     2703 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/compoundAnalysis/helpers.ts
+-rw-r--r--   0 root         (0) root         (0)     2579 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/compoundAnalysis/reducers.ts
+-rw-r--r--   0 root         (0) root         (0)    10390 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/compoundAnalysis/sagas.ts
+-rw-r--r--   0 root         (0) root         (0)     3894 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/compoundAnalysis/types.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.623915 libertem-0.9.2/client/src/config/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.623915 libertem-0.9.2/client/src/config/__tests__/
+-rw-r--r--   0 root         (0) root         (0)      594 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/config/__tests__/helpers.ts
+-rw-r--r--   0 root         (0) root         (0)      675 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/config/__tests__/reducers.ts
+-rw-r--r--   0 root         (0) root         (0)      713 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/config/actions.ts
+-rw-r--r--   0 root         (0) root         (0)      389 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/config/api.ts
+-rw-r--r--   0 root         (0) root         (0)     1949 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/config/helpers.ts
+-rw-r--r--   0 root         (0) root         (0)     3273 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/config/reducers.ts
+-rw-r--r--   0 root         (0) root         (0)     2481 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/config/sagas.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.626915 libertem-0.9.2/client/src/dataset/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.626915 libertem-0.9.2/client/src/dataset/__tests__/
+-rw-r--r--   0 root         (0) root         (0)     2773 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/dataset/__tests__/validate.ts
+-rw-r--r--   0 root         (0) root         (0)     1699 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/dataset/actions.ts
+-rw-r--r--   0 root         (0) root         (0)      893 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/dataset/api.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.629915 libertem-0.9.2/client/src/dataset/components/
+-rw-r--r--   0 root         (0) root         (0)      887 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/dataset/components/AddAnalysis.tsx
+-rw-r--r--   0 root         (0) root         (0)     3282 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/dataset/components/BLOParamsForm.tsx
+-rw-r--r--   0 root         (0) root         (0)     1237 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/dataset/components/BackendSelectionDropdown.tsx
+-rw-r--r--   0 root         (0) root         (0)     3431 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/dataset/components/Dataset.tsx
+-rw-r--r--   0 root         (0) root         (0)     1454 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/dataset/components/DatasetInfo.tsx
+-rw-r--r--   0 root         (0) root         (0)     1152 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/dataset/components/DatasetList.tsx
+-rw-r--r--   0 root         (0) root         (0)     9992 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/dataset/components/DatasetOpen.tsx
+-rw-r--r--   0 root         (0) root         (0)      884 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/dataset/components/DatasetOpenSpinner.tsx
+-rw-r--r--   0 root         (0) root         (0)     1478 2022-04-28 17:22:40.000000 libertem-0.9.2/client/src/dataset/components/DatasetParams.tsx
+-rw-r--r--   0 root         (0) root         (0)      833 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/dataset/components/DatasetToolbar.tsx
+-rw-r--r--   0 root         (0) root         (0)      856 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/dataset/components/DatasetTypeSelect.tsx
+-rw-r--r--   0 root         (0) root         (0)     3241 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/dataset/components/EMPADParamsForm.tsx
+-rw-r--r--   0 root         (0) root         (0)     3240 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/dataset/components/FRMS6ParamsForm.tsx
+-rw-r--r--   0 root         (0) root         (0)     4261 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/dataset/components/HDF5ParamsForm.tsx
+-rw-r--r--   0 root         (0) root         (0)     3238 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/dataset/components/K2ISParamsForm.tsx
+-rw-r--r--   0 root         (0) root         (0)     3284 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/dataset/components/MIBParamsForm.tsx
+-rw-r--r--   0 root         (0) root         (0)     2759 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/dataset/components/MRCParamsForm.tsx
+-rw-r--r--   0 root         (0) root         (0)     3418 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/dataset/components/RawFileParamsForm.tsx
+-rw-r--r--   0 root         (0) root         (0)     3036 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/dataset/components/Reshape.tsx
+-rw-r--r--   0 root         (0) root         (0)     3284 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/dataset/components/SEQParamsForm.tsx
+-rw-r--r--   0 root         (0) root         (0)     2690 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/dataset/components/SERParamsForm.tsx
+-rw-r--r--   0 root         (0) root         (0)     3312 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/dataset/components/TVIPSParamsForm.tsx
+-rw-r--r--   0 root         (0) root         (0)     3012 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/dataset/components/TupleInput.tsx
+-rw-r--r--   0 root         (0) root         (0)     1105 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/dataset/components/TupleInputPart.tsx
+-rw-r--r--   0 root         (0) root         (0)     5736 2022-04-28 17:22:40.000000 libertem-0.9.2/client/src/dataset/helpers.ts
+-rw-r--r--   0 root         (0) root         (0)     3603 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/dataset/reducers.ts
+-rw-r--r--   0 root         (0) root         (0)     4432 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/dataset/sagas.ts
+-rw-r--r--   0 root         (0) root         (0)      639 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/dataset/types.ts
+-rw-r--r--   0 root         (0) root         (0)     1825 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/dataset/validate.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.630915 libertem-0.9.2/client/src/errors/
+-rw-r--r--   0 root         (0) root         (0)      534 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/errors/actions.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.630915 libertem-0.9.2/client/src/errors/components/
+-rw-r--r--   0 root         (0) root         (0)      726 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/errors/components/Error.tsx
+-rw-r--r--   0 root         (0) root         (0)     1165 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/errors/components/ErrorList.tsx
+-rw-r--r--   0 root         (0) root         (0)      395 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/errors/helpers.ts
+-rw-r--r--   0 root         (0) root         (0)     1696 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/errors/reducers.ts
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-28 17:22:40.000000 libertem-0.9.2/client/src/errors/sagas.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.632915 libertem-0.9.2/client/src/helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.632915 libertem-0.9.2/client/src/helpers/__tests__/
+-rw-r--r--   0 root         (0) root         (0)      926 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/helpers/__tests__/reducerHelpers.ts
+-rw-r--r--   0 root         (0) root         (0)     1029 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/helpers/actionHelpers.ts
+-rw-r--r--   0 root         (0) root         (0)     1102 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/helpers/apiHelpers.ts
+-rw-r--r--   0 root         (0) root         (0)      444 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/helpers/hooks.ts
+-rw-r--r--   0 root         (0) root         (0)      714 2022-04-28 17:22:40.000000 libertem-0.9.2/client/src/helpers/index.ts
+-rw-r--r--   0 root         (0) root         (0)       59 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/helpers/props.ts
+-rw-r--r--   0 root         (0) root         (0)     3259 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/helpers/reducerHelpers.ts
+-rw-r--r--   0 root         (0) root         (0)     1355 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/helpers/svg.ts
+-rw-r--r--   0 root         (0) root         (0)      227 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/helpers/types.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.632915 libertem-0.9.2/client/src/images/
+-rw-r--r--   0 root         (0) root         (0)    11743 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/images/LiberTEM logo-medium.png
+-rw-r--r--   0 root         (0) root         (0)      837 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/index.tsx
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.632915 libertem-0.9.2/client/src/job/
+-rw-r--r--   0 root         (0) root         (0)      429 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/job/actions.ts
+-rw-r--r--   0 root         (0) root         (0)      577 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/job/api.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.634915 libertem-0.9.2/client/src/job/components/
+-rw-r--r--   0 root         (0) root         (0)     1523 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/job/components/PlaceholderImage.tsx
+-rw-r--r--   0 root         (0) root         (0)     1712 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/job/components/Result.tsx
+-rw-r--r--   0 root         (0) root         (0)      177 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/job/components/ResultImage.module.css
+-rw-r--r--   0 root         (0) root         (0)      696 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/job/components/ResultImage.tsx
+-rw-r--r--   0 root         (0) root         (0)     4486 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/job/components/ResultList.tsx
+-rw-r--r--   0 root         (0) root         (0)      168 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/job/components/Selectors.tsx
+-rw-r--r--   0 root         (0) root         (0)     3276 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/job/reducers.ts
+-rw-r--r--   0 root         (0) root         (0)      816 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/job/types.ts
+-rw-r--r--   0 root         (0) root         (0)    15174 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/messages.ts
+-rw-r--r--   0 root         (0) root         (0)       40 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/react-app-env.d.ts
+-rw-r--r--   0 root         (0) root         (0)     4526 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/registerServiceWorker.ts
+-rw-r--r--   0 root         (0) root         (0)      592 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/sagas.ts
+-rw-r--r--   0 root         (0) root         (0)      195 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/setupProxy.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.634915 libertem-0.9.2/client/src/shutdown/
+-rw-r--r--   0 root         (0) root         (0)      227 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/shutdown/api.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.634915 libertem-0.9.2/client/src/shutdown/components/
+-rw-r--r--   0 root         (0) root         (0)     2785 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/shutdown/components/ShutdownButton.tsx
+-rw-r--r--   0 root         (0) root         (0)     1025 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/store.ts
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/vendor.d.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.636915 libertem-0.9.2/client/src/widgets/
+-rw-r--r--   0 root         (0) root         (0)      453 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/widgets/BusySpinner.tsx
+-rw-r--r--   0 root         (0) root         (0)      432 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/widgets/BusyWrapper.tsx
+-rw-r--r--   0 root         (0) root         (0)      366 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/widgets/Disk.tsx
+-rw-r--r--   0 root         (0) root         (0)     7306 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/widgets/DraggableHandle.tsx
+-rw-r--r--   0 root         (0) root         (0)     2460 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/widgets/HandleParent.tsx
+-rw-r--r--   0 root         (0) root         (0)      753 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/widgets/Rect.tsx
+-rw-r--r--   0 root         (0) root         (0)      707 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/widgets/Ring.tsx
+-rw-r--r--   0 root         (0) root         (0)      329 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/widgets/compose.tsx
+-rw-r--r--   0 root         (0) root         (0)     1276 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/widgets/constraints.ts
+-rw-r--r--   0 root         (0) root         (0)     1167 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/widgets/kbdHandler.ts
+-rw-r--r--   0 root         (0) root         (0)      239 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/widgets/styles.ts
+-rw-r--r--   0 root         (0) root         (0)      351 2022-04-26 10:50:39.000000 libertem-0.9.2/client/src/widgets/types.ts
+-rw-r--r--   0 root         (0) root         (0)      576 2022-04-26 10:50:39.000000 libertem-0.9.2/client/tsconfig.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.636915 libertem-0.9.2/client/types/
+-rw-r--r--   0 root         (0) root         (0)      937 2022-04-26 10:50:39.000000 libertem-0.9.2/client/types/react-window.d.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.590915 libertem-0.9.2/libertem/
+-rw-r--r--   0 root         (0) root         (0)       53 2022-04-28 17:30:33.593915 libertem-0.9.2/libertem/_baked_revision.py
+-rw-r--r--   0 root         (0) root         (0)       82 2022-04-26 10:50:39.000000 libertem-0.9.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      546 2022-04-28 17:30:33.713914 libertem-0.9.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     6681 2022-04-26 10:50:39.000000 libertem-0.9.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.599915 libertem-0.9.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.637915 libertem-0.9.2/src/libertem/
+-rw-r--r--   0 root         (0) root         (0)      323 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.639915 libertem-0.9.2/src/libertem/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      344 2022-04-28 17:13:56.000000 libertem-0.9.2/src/libertem/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)      166 2022-04-28 17:13:56.000000 libertem-0.9.2/src/libertem/__pycache__/__version__.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    42813 2022-04-28 17:13:58.000000 libertem-0.9.2/src/libertem/__pycache__/api.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)      380 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/__pycache__/exceptions.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    11654 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/__pycache__/masks.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)      508 2022-04-28 17:13:56.000000 libertem-0.9.2/src/libertem/__pycache__/versioning.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)      746 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/__pycache__/warnings.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)       22 2022-04-28 17:22:40.000000 libertem-0.9.2/src/libertem/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.641915 libertem-0.9.2/src/libertem/analysis/
+-rw-r--r--   0 root         (0) root         (0)      877 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/analysis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.644915 libertem-0.9.2/src/libertem/analysis/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      916 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/analysis/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     2717 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/analysis/__pycache__/apply_fft_mask.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    12578 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/analysis/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     7174 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/analysis/__pycache__/clust.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    18301 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/analysis/__pycache__/com.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     3182 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/analysis/__pycache__/disk.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     2888 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/analysis/__pycache__/fem.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    13853 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/analysis/__pycache__/fullmatch.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)      627 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/analysis/__pycache__/getroi.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    17165 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/analysis/__pycache__/gridmatching.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     3238 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/analysis/__pycache__/helper.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     7941 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/analysis/__pycache__/masks.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     3099 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/analysis/__pycache__/point.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    10082 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/analysis/__pycache__/radialfourier.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     6310 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/analysis/__pycache__/raw.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     2584 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/analysis/__pycache__/rawfft.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     3098 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/analysis/__pycache__/ring.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     3105 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/analysis/__pycache__/sd.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     5332 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/analysis/__pycache__/sum.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     2777 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/analysis/__pycache__/sumfft.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     2489 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/analysis/__pycache__/sumsig.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     2030 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/analysis/apply_fft_mask.py
+-rw-r--r--   0 root         (0) root         (0)    11471 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/analysis/base.py
+-rw-r--r--   0 root         (0) root         (0)     7864 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/analysis/clust.py
+-rw-r--r--   0 root         (0) root         (0)    22450 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/analysis/com.py
+-rw-r--r--   0 root         (0) root         (0)     2371 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/analysis/disk.py
+-rw-r--r--   0 root         (0) root         (0)     2200 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/analysis/fem.py
+-rw-r--r--   0 root         (0) root         (0)    16383 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/analysis/fullmatch.py
+-rw-r--r--   0 root         (0) root         (0)      669 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/analysis/getroi.py
+-rw-r--r--   0 root         (0) root         (0)    18296 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/analysis/gridmatching.py
+-rw-r--r--   0 root         (0) root         (0)     2593 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/analysis/helper.py
+-rw-r--r--   0 root         (0) root         (0)     7319 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/analysis/masks.py
+-rw-r--r--   0 root         (0) root         (0)     2145 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/analysis/point.py
+-rw-r--r--   0 root         (0) root         (0)    12805 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/analysis/radialfourier.py
+-rw-r--r--   0 root         (0) root         (0)     5522 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/analysis/raw.py
+-rw-r--r--   0 root         (0) root         (0)     2008 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/analysis/rawfft.py
+-rw-r--r--   0 root         (0) root         (0)     2385 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/analysis/ring.py
+-rw-r--r--   0 root         (0) root         (0)     2659 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/analysis/sd.py
+-rw-r--r--   0 root         (0) root         (0)     4987 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/analysis/sum.py
+-rw-r--r--   0 root         (0) root         (0)     2280 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/analysis/sumfft.py
+-rw-r--r--   0 root         (0) root         (0)     1687 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/analysis/sumsig.py
+-rw-r--r--   0 root         (0) root         (0)    49144 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/api.py
+-rw-r--r--   0 root         (0) root         (0)      165 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/cli_tweaks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.646915 libertem-0.9.2/src/libertem/common/
+-rw-r--r--   0 root         (0) root         (0)     1151 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/common/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       80 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.650915 libertem-0.9.2/src/libertem/common/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      242 2022-04-28 17:13:58.000000 libertem-0.9.2/src/libertem/common/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     2272 2022-04-28 17:13:58.000000 libertem-0.9.2/src/libertem/common/__pycache__/backend.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    22758 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/common/__pycache__/buffers.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     6694 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/common/__pycache__/container.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)      878 2022-04-28 17:13:58.000000 libertem-0.9.2/src/libertem/common/__pycache__/math.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     6637 2022-04-28 17:13:58.000000 libertem-0.9.2/src/libertem/common/__pycache__/shape.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    11764 2022-04-28 17:13:58.000000 libertem-0.9.2/src/libertem/common/__pycache__/slice.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     2754 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/common/backend.py
+-rw-r--r--   0 root         (0) root         (0)    23927 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/common/buffers.py
+-rw-r--r--   0 root         (0) root         (0)     8911 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/common/container.py
+-rw-r--r--   0 root         (0) root         (0)      766 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/common/math.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.651915 libertem-0.9.2/src/libertem/common/numba/
+-rw-r--r--   0 root         (0) root         (0)     5523 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/common/numba/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.652915 libertem-0.9.2/src/libertem/common/numba/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)     4297 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/common/numba/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     4712 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/common/numba/__pycache__/cache.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     5905 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/common/numba/cache.py
+-rw-r--r--   0 root         (0) root         (0)     5434 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/common/shape.py
+-rw-r--r--   0 root         (0) root         (0)    12476 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/common/slice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.652915 libertem-0.9.2/src/libertem/contrib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.653915 libertem-0.9.2/src/libertem/contrib/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      767 2022-04-28 17:29:49.000000 libertem-0.9.2/src/libertem/contrib/__pycache__/daskadapter.cpython-37.pyc
+-rw-r--r--   0 root         (0) root         (0)      779 2022-04-26 11:11:45.000000 libertem-0.9.2/src/libertem/contrib/__pycache__/daskadapter.cpython-38.pyc
+-rw-r--r--   0 root         (0) root         (0)      777 2022-04-26 11:49:13.000000 libertem-0.9.2/src/libertem/contrib/__pycache__/daskadapter.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)      698 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/contrib/daskadapter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.653915 libertem-0.9.2/src/libertem/corrections/
+-rw-r--r--   0 root         (0) root         (0)       64 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/corrections/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.653915 libertem-0.9.2/src/libertem/corrections/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      215 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/corrections/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     1066 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/corrections/__pycache__/coordinates.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     7038 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/corrections/__pycache__/corrset.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     8409 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/corrections/__pycache__/detector.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)      810 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/corrections/coordinates.py
+-rw-r--r--   0 root         (0) root         (0)    10366 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/corrections/corrset.py
+-rw-r--r--   0 root         (0) root         (0)    11538 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/corrections/detector.py
+-rw-r--r--   0 root         (0) root         (0)      109 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.654915 libertem-0.9.2/src/libertem/executor/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/executor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.656915 libertem-0.9.2/src/libertem/executor/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      145 2022-04-28 17:13:58.000000 libertem-0.9.2/src/libertem/executor/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    15943 2022-04-28 17:13:58.000000 libertem-0.9.2/src/libertem/executor/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     6054 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/executor/__pycache__/concurrent.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    20442 2022-04-28 17:13:58.000000 libertem-0.9.2/src/libertem/executor/__pycache__/dask.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    15699 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/executor/__pycache__/delayed.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     3154 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/executor/__pycache__/inline.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     1975 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/executor/__pycache__/integration.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     6114 2022-04-28 17:13:58.000000 libertem-0.9.2/src/libertem/executor/__pycache__/scheduler.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    13307 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/executor/base.py
+-rw-r--r--   0 root         (0) root         (0)     3309 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/executor/cli.py
+-rw-r--r--   0 root         (0) root         (0)     5308 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/executor/concurrent.py
+-rw-r--r--   0 root         (0) root         (0)    22579 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/executor/dask.py
+-rw-r--r--   0 root         (0) root         (0)    17893 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/executor/delayed.py
+-rw-r--r--   0 root         (0) root         (0)     2569 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/executor/inline.py
+-rw-r--r--   0 root         (0) root         (0)     2563 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/executor/integration.py
+-rw-r--r--   0 root         (0) root         (0)     3506 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/executor/scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.656915 libertem-0.9.2/src/libertem/executor/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/executor/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.657915 libertem-0.9.2/src/libertem/executor/utils/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      151 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/executor/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     7850 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/executor/utils/__pycache__/dask_buffer.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     6285 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/executor/utils/__pycache__/dask_inplace.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     9234 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/executor/utils/__pycache__/delayed_unpack.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     7683 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/executor/utils/dask_buffer.py
+-rw-r--r--   0 root         (0) root         (0)     7648 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/executor/utils/dask_inplace.py
+-rw-r--r--   0 root         (0) root         (0)    10183 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/executor/utils/delayed_unpack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.658915 libertem-0.9.2/src/libertem/io/
+-rw-r--r--   0 root         (0) root         (0)     1151 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/LICENSE
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.659915 libertem-0.9.2/src/libertem/io/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      139 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/io/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     1480 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/io/__pycache__/utils.cpython-39.pyc
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.663915 libertem-0.9.2/src/libertem/io/dataset/
+-rw-r--r--   0 root         (0) root         (0)     5726 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/dataset/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.665915 libertem-0.9.2/src/libertem/io/dataset/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)     5443 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/io/dataset/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     8002 2022-04-28 17:14:02.000000 libertem-0.9.2/src/libertem/io/dataset/__pycache__/blo.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    19877 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/io/dataset/__pycache__/cached.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     9877 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/io/dataset/__pycache__/cluster.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    21540 2022-04-28 17:14:02.000000 libertem-0.9.2/src/libertem/io/dataset/__pycache__/dask.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    10507 2022-04-28 17:14:01.000000 libertem-0.9.2/src/libertem/io/dataset/__pycache__/dm.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     8743 2022-04-28 17:14:01.000000 libertem-0.9.2/src/libertem/io/dataset/__pycache__/empad.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    20542 2022-04-28 17:14:02.000000 libertem-0.9.2/src/libertem/io/dataset/__pycache__/frms6.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    23751 2022-04-28 17:14:02.000000 libertem-0.9.2/src/libertem/io/dataset/__pycache__/hdf5.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    34341 2022-04-28 17:14:01.000000 libertem-0.9.2/src/libertem/io/dataset/__pycache__/k2is.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    10765 2022-04-28 17:14:02.000000 libertem-0.9.2/src/libertem/io/dataset/__pycache__/memory.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    33199 2022-04-28 17:14:01.000000 libertem-0.9.2/src/libertem/io/dataset/__pycache__/mib.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     8240 2022-04-28 17:14:02.000000 libertem-0.9.2/src/libertem/io/dataset/__pycache__/mrc.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     7620 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/io/dataset/__pycache__/raw.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    18639 2022-04-28 17:14:02.000000 libertem-0.9.2/src/libertem/io/dataset/__pycache__/seq.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    10309 2022-04-28 17:14:02.000000 libertem-0.9.2/src/libertem/io/dataset/__pycache__/ser.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    13560 2022-04-28 17:14:02.000000 libertem-0.9.2/src/libertem/io/dataset/__pycache__/tvips.cpython-39.pyc
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.667915 libertem-0.9.2/src/libertem/io/dataset/base/
+-rw-r--r--   0 root         (0) root         (0)     1271 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/dataset/base/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.669915 libertem-0.9.2/src/libertem/io/dataset/base/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)     1312 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/io/dataset/base/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     5300 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/io/dataset/base/__pycache__/backend.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    11278 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/io/dataset/base/__pycache__/backend_buffered.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     1922 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/io/dataset/base/__pycache__/backend_direct.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    11264 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/io/dataset/base/__pycache__/backend_mmap.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     1576 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/io/dataset/base/__pycache__/coordinates.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    10961 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/io/dataset/base/__pycache__/dataset.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     5547 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/io/dataset/base/__pycache__/decode.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)      325 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/io/dataset/base/__pycache__/exceptions.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     5585 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/io/dataset/base/__pycache__/file.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     3522 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/io/dataset/base/__pycache__/fileset.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     4490 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/io/dataset/base/__pycache__/meta.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     9157 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/io/dataset/base/__pycache__/partition.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     2099 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/io/dataset/base/__pycache__/roi.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     7865 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/io/dataset/base/__pycache__/tiling.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    14230 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/io/dataset/base/__pycache__/tiling_scheme.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     2479 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/io/dataset/base/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     5117 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/dataset/base/backend.py
+-rw-r--r--   0 root         (0) root         (0)    15021 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/dataset/base/backend_buffered.py
+-rw-r--r--   0 root         (0) root         (0)     1347 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/dataset/base/backend_direct.py
+-rw-r--r--   0 root         (0) root         (0)    12823 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/dataset/base/backend_mmap.py
+-rw-r--r--   0 root         (0) root         (0)     1535 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/dataset/base/coordinates.py
+-rw-r--r--   0 root         (0) root         (0)    10241 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/dataset/base/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     5044 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/dataset/base/decode.py
+-rw-r--r--   0 root         (0) root         (0)       44 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/dataset/base/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     5680 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/dataset/base/file.py
+-rw-r--r--   0 root         (0) root         (0)     3159 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/dataset/base/fileset.py
+-rw-r--r--   0 root         (0) root         (0)     4217 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/dataset/base/meta.py
+-rw-r--r--   0 root         (0) root         (0)     8726 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/dataset/base/partition.py
+-rw-r--r--   0 root         (0) root         (0)     1845 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/dataset/base/roi.py
+-rw-r--r--   0 root         (0) root         (0)    11867 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/dataset/base/tiling.py
+-rw-r--r--   0 root         (0) root         (0)    17722 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/dataset/base/tiling_scheme.py
+-rw-r--r--   0 root         (0) root         (0)     2232 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/dataset/base/utils.py
+-rw-r--r--   0 root         (0) root         (0)     8726 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/dataset/blo.py
+-rw-r--r--   0 root         (0) root         (0)    18746 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/dataset/cached.py
+-rw-r--r--   0 root         (0) root         (0)     8456 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/dataset/cluster.py
+-rw-r--r--   0 root         (0) root         (0)    21163 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/dataset/dask.py
+-rw-r--r--   0 root         (0) root         (0)    10195 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/dataset/dm.py
+-rw-r--r--   0 root         (0) root         (0)     9356 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/dataset/empad.py
+-rw-r--r--   0 root         (0) root         (0)    23589 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/dataset/frms6.py
+-rw-r--r--   0 root         (0) root         (0)    28043 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/dataset/hdf5.py
+-rw-r--r--   0 root         (0) root         (0)    37600 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/dataset/k2is.py
+-rw-r--r--   0 root         (0) root         (0)    13036 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/dataset/memory.py
+-rw-r--r--   0 root         (0) root         (0)    44457 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/dataset/mib.py
+-rw-r--r--   0 root         (0) root         (0)     7380 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/dataset/mrc.py
+-rw-r--r--   0 root         (0) root         (0)     8609 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/dataset/raw.py
+-rw-r--r--   0 root         (0) root         (0)    23010 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/dataset/seq.py
+-rw-r--r--   0 root         (0) root         (0)    10454 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/dataset/ser.py
+-rw-r--r--   0 root         (0) root         (0)    17844 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/dataset/tvips.py
+-rw-r--r--   0 root         (0) root         (0)      491 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/direct.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/fs.py
+-rw-r--r--   0 root         (0) root         (0)     1717 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.670915 libertem-0.9.2/src/libertem/io/writers/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/writers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.670915 libertem-0.9.2/src/libertem/io/writers/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      147 2022-04-28 17:14:01.000000 libertem-0.9.2/src/libertem/io/writers/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     4120 2022-04-28 17:14:01.000000 libertem-0.9.2/src/libertem/io/writers/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     4264 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/writers/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.670915 libertem-0.9.2/src/libertem/io/writers/results/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/writers/results/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.670915 libertem-0.9.2/src/libertem/io/writers/results/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      155 2022-04-28 17:14:01.000000 libertem-0.9.2/src/libertem/io/writers/results/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     2838 2022-04-28 17:14:01.000000 libertem-0.9.2/src/libertem/io/writers/results/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     5371 2022-04-28 17:14:01.000000 libertem-0.9.2/src/libertem/io/writers/results/__pycache__/formats.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     1801 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/writers/results/base.py
+-rw-r--r--   0 root         (0) root         (0)     2996 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/io/writers/results/formats.py
+-rw-r--r--   0 root         (0) root         (0)    13962 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/masks.py
+-rw-r--r--   0 root         (0) root         (0)      536 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/preload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.673915 libertem-0.9.2/src/libertem/udf/
+-rw-r--r--   0 root         (0) root         (0)     2696 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/udf/FEM.py
+-rw-r--r--   0 root         (0) root         (0)      349 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/udf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.676915 libertem-0.9.2/src/libertem/udf/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)     3059 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/udf/__pycache__/FEM.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)      470 2022-04-28 17:13:58.000000 libertem-0.9.2/src/libertem/udf/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     2115 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/udf/__pycache__/auto.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    71195 2022-04-28 17:13:58.000000 libertem-0.9.2/src/libertem/udf/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     4189 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/udf/__pycache__/crystallinity.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     6012 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/udf/__pycache__/holography.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     2478 2022-04-28 17:14:02.000000 libertem-0.9.2/src/libertem/udf/__pycache__/logsum.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     7236 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/udf/__pycache__/masks.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     2371 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/udf/__pycache__/raw.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    12890 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/udf/__pycache__/stddev.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     2197 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/udf/__pycache__/sum.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     1283 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/udf/__pycache__/sumsigudf.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     1826 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/udf/auto.py
+-rw-r--r--   0 root         (0) root         (0)    74248 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/udf/base.py
+-rw-r--r--   0 root         (0) root         (0)     4268 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/udf/crystallinity.py
+-rw-r--r--   0 root         (0) root         (0)     7396 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/udf/holography.py
+-rw-r--r--   0 root         (0) root         (0)     1619 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/udf/logsum.py
+-rw-r--r--   0 root         (0) root         (0)     7952 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/udf/masks.py
+-rw-r--r--   0 root         (0) root         (0)     2281 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/udf/raw.py
+-rw-r--r--   0 root         (0) root         (0)    14913 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/udf/stddev.py
+-rw-r--r--   0 root         (0) root         (0)     1316 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/udf/sum.py
+-rw-r--r--   0 root         (0) root         (0)      791 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/udf/sumsigudf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.677914 libertem-0.9.2/src/libertem/utils/
+-rw-r--r--   0 root         (0) root         (0)     4665 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.678915 libertem-0.9.2/src/libertem/utils/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)     4826 2022-04-28 17:13:58.000000 libertem-0.9.2/src/libertem/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     7639 2022-04-28 17:13:58.000000 libertem-0.9.2/src/libertem/utils/__pycache__/async_utils.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     1841 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/utils/__pycache__/devices.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     4706 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/utils/__pycache__/generate.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     7033 2022-04-28 17:13:58.000000 libertem-0.9.2/src/libertem/utils/__pycache__/threading.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     8361 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/utils/async_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1682 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/utils/devices.py
+-rw-r--r--   0 root         (0) root         (0)     5171 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/utils/generate.py
+-rw-r--r--   0 root         (0) root         (0)     9956 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/utils/threading.py
+-rw-r--r--   0 root         (0) root         (0)      351 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/versioning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.679915 libertem-0.9.2/src/libertem/viz/
+-rw-r--r--   0 root         (0) root         (0)      848 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/viz/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.680914 libertem-0.9.2/src/libertem/viz/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      739 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/viz/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     9870 2022-04-28 17:14:02.000000 libertem-0.9.2/src/libertem/viz/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     3964 2022-04-28 17:14:02.000000 libertem-0.9.2/src/libertem/viz/__pycache__/bqp.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     3627 2022-04-28 17:14:02.000000 libertem-0.9.2/src/libertem/viz/__pycache__/gms.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     3765 2022-04-28 17:14:02.000000 libertem-0.9.2/src/libertem/viz/__pycache__/mpl.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    10612 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/viz/base.py
+-rw-r--r--   0 root         (0) root         (0)     4320 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/viz/bqp.py
+-rw-r--r--   0 root         (0) root         (0)     3497 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/viz/gms.py
+-rw-r--r--   0 root         (0) root         (0)     3695 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/viz/mpl.py
+-rw-r--r--   0 root         (0) root         (0)      473 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/warnings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.682915 libertem-0.9.2/src/libertem/web/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.683915 libertem-0.9.2/src/libertem/web/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      140 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/web/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     1728 2022-04-28 17:13:59.000000 libertem-0.9.2/src/libertem/web/__pycache__/messageconverter.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     6681 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/web/__pycache__/messages.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     2280 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/web/__pycache__/models.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     4293 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/web/__pycache__/rpc.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    16039 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/web/__pycache__/state.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     7081 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/analysis.py
+-rw-r--r--   0 root         (0) root         (0)     1511 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/base.py
+-rw-r--r--   0 root         (0) root         (0)      985 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/browse.py
+-rw-r--r--   0 root         (0) root         (0)     2471 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.685914 libertem-0.9.2/src/libertem/web/client/
+-rw-r--r--   0 root         (0) root         (0)     1365 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/client/asset-manifest.json
+-rw-r--r--   0 root         (0) root         (0)    15086 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/client/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)     2199 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/client/index.html
+-rw-r--r--   0 root         (0) root         (0)      295 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/client/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.603915 libertem-0.9.2/src/libertem/web/client/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.689914 libertem-0.9.2/src/libertem/web/client/static/css/
+-rw-r--r--   0 root         (0) root         (0)   579793 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/client/static/css/2.42a8572e.chunk.css
+-rw-r--r--   0 root         (0) root         (0)  1404626 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/client/static/css/2.42a8572e.chunk.css.map
+-rw-r--r--   0 root         (0) root         (0)      295 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/client/static/css/main.c0d8de42.chunk.css
+-rw-r--r--   0 root         (0) root         (0)      448 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/client/static/css/main.c0d8de42.chunk.css.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.697914 libertem-0.9.2/src/libertem/web/client/static/js/
+-rw-r--r--   0 root         (0) root         (0)   668351 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/client/static/js/2.909ce721.chunk.js
+-rw-r--r--   0 root         (0) root         (0)     2093 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/client/static/js/2.909ce721.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)  3041745 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/client/static/js/2.909ce721.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)   152222 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/client/static/js/main.d79ffbf3.chunk.js
+-rw-r--r--   0 root         (0) root         (0)   508349 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/client/static/js/main.d79ffbf3.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)     1585 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/client/static/js/runtime-main.fcac4e81.js
+-rw-r--r--   0 root         (0) root         (0)     8298 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/client/static/js/runtime-main.fcac4e81.js.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.707914 libertem-0.9.2/src/libertem/web/client/static/media/
+-rw-r--r--   0 root         (0) root         (0)    11743 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/client/static/media/LiberTEM logo-medium.2765b438.png
+-rw-r--r--   0 root         (0) root         (0)    54488 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/client/static/media/brand-icons.278156e4.woff2
+-rw-r--r--   0 root         (0) root         (0)    98404 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/client/static/media/brand-icons.65a2fb6d.ttf
+-rw-r--r--   0 root         (0) root         (0)   507628 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/client/static/media/brand-icons.6729d297.svg
+-rw-r--r--   0 root         (0) root         (0)    63728 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/client/static/media/brand-icons.cac87dc0.woff
+-rw-r--r--   0 root         (0) root         (0)    98640 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/client/static/media/brand-icons.d68fa3e6.eot
+-rw-r--r--   0 root         (0) root         (0)    28123 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/client/static/media/flags.99f63ae7.png
+-rw-r--r--   0 root         (0) root         (0)    40148 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/client/static/media/icons.38c6d8ba.woff2
+-rw-r--r--   0 root         (0) root         (0)    50524 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/client/static/media/icons.425399f8.woff
+-rw-r--r--   0 root         (0) root         (0)   390837 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/client/static/media/icons.62d9dae4.svg
+-rw-r--r--   0 root         (0) root         (0)   106004 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/client/static/media/icons.a01e3f2d.eot
+-rw-r--r--   0 root         (0) root         (0)   105784 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/client/static/media/icons.c656b8ca.ttf
+-rw-r--r--   0 root         (0) root         (0)    30928 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/client/static/media/outline-icons.53671035.ttf
+-rw-r--r--   0 root         (0) root         (0)    12240 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/client/static/media/outline-icons.687a4990.woff2
+-rw-r--r--   0 root         (0) root         (0)    31156 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/client/static/media/outline-icons.752905fa.eot
+-rw-r--r--   0 root         (0) root         (0)   107201 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/client/static/media/outline-icons.9c4845b4.svg
+-rw-r--r--   0 root         (0) root         (0)    14712 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/client/static/media/outline-icons.ddae9b1b.woff
+-rw-r--r--   0 root         (0) root         (0)     1071 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/config.py
+-rw-r--r--   0 root         (0) root         (0)     3573 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/connect.py
+-rw-r--r--   0 root         (0) root         (0)     4201 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     9381 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/engine.py
+-rw-r--r--   0 root         (0) root         (0)     2378 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/events.py
+-rw-r--r--   0 root         (0) root         (0)     2385 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/generator.py
+-rw-r--r--   0 root         (0) root         (0)     1564 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/jobs.py
+-rw-r--r--   0 root         (0) root         (0)     1348 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/messageconverter.py
+-rw-r--r--   0 root         (0) root         (0)     6696 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/messages.py
+-rw-r--r--   0 root         (0) root         (0)     1156 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.710914 libertem-0.9.2/src/libertem/web/notebook_generator/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/notebook_generator/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.711914 libertem-0.9.2/src/libertem/web/notebook_generator/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      159 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/web/notebook_generator/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     1664 2022-04-28 17:14:00.000000 libertem-0.9.2/src/libertem/web/notebook_generator/__pycache__/template.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     4262 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/notebook_generator/code_template.py
+-rw-r--r--   0 root         (0) root         (0)      514 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/notebook_generator/copy.py
+-rw-r--r--   0 root         (0) root         (0)     1378 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/notebook_generator/notebook_generator.py
+-rw-r--r--   0 root         (0) root         (0)     1323 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/notebook_generator/template.py
+-rw-r--r--   0 root         (0) root         (0)     3300 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/rpc.py
+-rw-r--r--   0 root         (0) root         (0)     7460 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/server.py
+-rw-r--r--   0 root         (0) root         (0)      691 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/shutdown.py
+-rw-r--r--   0 root         (0) root         (0)    13476 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/web/state.py
+-rw-r--r--   0 root         (0) root         (0)     2488 2022-04-26 10:50:39.000000 libertem-0.9.2/src/libertem/win_tweaks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-28 17:30:33.638915 libertem-0.9.2/src/libertem.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10657 2022-04-28 17:30:33.000000 libertem-0.9.2/src/libertem.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    21154 2022-04-28 17:30:33.000000 libertem-0.9.2/src/libertem.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-04-28 17:30:33.000000 libertem-0.9.2/src/libertem.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2022-04-28 17:30:33.000000 libertem-0.9.2/src/libertem.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-04-26 10:50:46.000000 libertem-0.9.2/src/libertem.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      440 2022-04-28 17:30:33.000000 libertem-0.9.2/src/libertem.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2022-04-28 17:30:33.000000 libertem-0.9.2/src/libertem.egg-info/top_level.txt
```

### Comparing `libertem-0.9.0/LICENSE` & `libertem-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/PKG-INFO` & `libertem-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libertem
-Version: 0.9.0
+Version: 0.9.2
 Summary: Open pixelated STEM framework
 Home-page: https://libertem.github.io/LiberTEM/
 Author: the LiberTEM team
 Author-email: libertem-dev@googlegroups.com
 License: GPL v3
 Keywords: electron microscopy
 Platform: UNKNOWN
```

### Comparing `libertem-0.9.0/README.rst` & `libertem-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/.eslintrc.js` & `libertem-0.9.2/client/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/README.md` & `libertem-0.9.2/client/README.md`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/package-lock.json` & `libertem-0.9.2/client/package-lock.json`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/package.json` & `libertem-0.9.2/client/package.json`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/public/favicon.ico` & `libertem-0.9.2/client/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/public/index.html` & `libertem-0.9.2/client/public/index.html`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/About.tsx` & `libertem-0.9.2/client/src/About.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/App.tsx` & `libertem-0.9.2/client/src/App.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/Menu.tsx` & `libertem-0.9.2/client/src/Menu.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/actions.ts` & `libertem-0.9.2/client/src/actions.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/analysis/actions.ts` & `libertem-0.9.2/client/src/analysis/actions.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/analysis/reducers.ts` & `libertem-0.9.2/client/src/analysis/reducers.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/browser/actions.ts` & `libertem-0.9.2/client/src/browser/actions.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/browser/components/BrowserWrapper.tsx` & `libertem-0.9.2/client/src/browser/components/BrowserWrapper.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/browser/components/FileBrowser.tsx` & `libertem-0.9.2/client/src/browser/components/FileBrowser.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/browser/components/FileBrowserEntry.tsx` & `libertem-0.9.2/client/src/browser/components/FileBrowserEntry.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/browser/components/FileBrowserHeader.tsx` & `libertem-0.9.2/client/src/browser/components/FileBrowserHeader.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/browser/components/FileEntry.tsx` & `libertem-0.9.2/client/src/browser/components/FileEntry.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/browser/components/FolderEntry.tsx` & `libertem-0.9.2/client/src/browser/components/FolderEntry.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/browser/components/PathBar.tsx` & `libertem-0.9.2/client/src/browser/components/PathBar.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/browser/components/PathDropDownItem.tsx` & `libertem-0.9.2/client/src/browser/components/PathDropDownItem.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/browser/components/PathInput.tsx` & `libertem-0.9.2/client/src/browser/components/PathInput.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/browser/components/RecentFiles.tsx` & `libertem-0.9.2/client/src/browser/components/RecentFiles.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/browser/reducers.ts` & `libertem-0.9.2/client/src/browser/reducers.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/browser/sagas.ts` & `libertem-0.9.2/client/src/browser/sagas.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/channel/actions.ts` & `libertem-0.9.2/client/src/channel/actions.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/channel/components/ChannelStatus.tsx` & `libertem-0.9.2/client/src/channel/components/ChannelStatus.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/channel/messages.ts` & `libertem-0.9.2/client/src/channel/messages.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/channel/reducers.ts` & `libertem-0.9.2/client/src/channel/reducers.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/channel/sagas.ts` & `libertem-0.9.2/client/src/channel/sagas.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/cluster/actions.ts` & `libertem-0.9.2/client/src/cluster/actions.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/cluster/api.ts` & `libertem-0.9.2/client/src/cluster/api.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/cluster/components/ClusterConnectionForm.tsx` & `libertem-0.9.2/client/src/cluster/components/ClusterConnectionForm.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/cluster/components/GPUSelector.tsx` & `libertem-0.9.2/client/src/cluster/components/GPUSelector.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/cluster/components/LocalConnectionForm.tsx` & `libertem-0.9.2/client/src/cluster/components/LocalConnectionForm.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/cluster/components/TCPConnectionForm.tsx` & `libertem-0.9.2/client/src/cluster/components/TCPConnectionForm.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/cluster/reducers.ts` & `libertem-0.9.2/client/src/cluster/reducers.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/cluster/sagas.ts` & `libertem-0.9.2/client/src/cluster/sagas.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/clusterStatus/components/Cluster.tsx` & `libertem-0.9.2/client/src/clusterStatus/components/Cluster.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/clusterStatus/components/LocalStatus.tsx` & `libertem-0.9.2/client/src/clusterStatus/components/LocalStatus.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/clusterStatus/components/TCPStatus.tsx` & `libertem-0.9.2/client/src/clusterStatus/components/TCPStatus.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/compoundAnalysis/actions.ts` & `libertem-0.9.2/client/src/compoundAnalysis/actions.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/compoundAnalysis/api.ts` & `libertem-0.9.2/client/src/compoundAnalysis/api.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/compoundAnalysis/components/CenterOfMassAnalysis.tsx` & `libertem-0.9.2/client/src/compoundAnalysis/components/CenterOfMassAnalysis.tsx`

 * *Files 0% similar despite different names*

```diff
@@ -221,14 +221,15 @@
     const guessParameters = (ev: React.MouseEvent) => {
         setGuessing(true);
         const basePath = getApiBasePath();
         const url = `${basePath}compoundAnalyses/${compoundAnalysis.compoundAnalysis}/rpc/guess_parameters/`;
 
         fetch(url, {
             method: 'PUT',
+            body: JSON.stringify({}),
             credentials: "same-origin",
         }).then(req => req.json()).then((json) => {
             setGuessing(false);
             const response = json as GuessResponse;
             if(response.status === "ok") {
                 setFlipY(response.guess.flip_y);
                 setCx(response.guess.cx);
```

### Comparing `libertem-0.9.0/client/src/compoundAnalysis/components/Clustering.tsx` & `libertem-0.9.2/client/src/compoundAnalysis/components/Clustering.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/compoundAnalysis/components/DefaultFrameView.tsx` & `libertem-0.9.2/client/src/compoundAnalysis/components/DefaultFrameView.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/compoundAnalysis/components/DiskMaskAnalysis.tsx` & `libertem-0.9.2/client/src/compoundAnalysis/components/DiskMaskAnalysis.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/compoundAnalysis/components/Download.tsx` & `libertem-0.9.2/client/src/compoundAnalysis/components/Download.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/compoundAnalysis/components/FEM.tsx` & `libertem-0.9.2/client/src/compoundAnalysis/components/FEM.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/compoundAnalysis/components/FFTAnalysis.tsx` & `libertem-0.9.2/client/src/compoundAnalysis/components/FFTAnalysis.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/compoundAnalysis/components/FFTFramePicker.tsx` & `libertem-0.9.2/client/src/compoundAnalysis/components/FFTFramePicker.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/compoundAnalysis/components/FFTFrameView.tsx` & `libertem-0.9.2/client/src/compoundAnalysis/components/FFTFrameView.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/compoundAnalysis/components/FFTSumFrames.tsx` & `libertem-0.9.2/client/src/compoundAnalysis/components/FFTSumFrames.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/compoundAnalysis/components/FramePicker.tsx` & `libertem-0.9.2/client/src/compoundAnalysis/components/FramePicker.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/compoundAnalysis/components/JustSum.tsx` & `libertem-0.9.2/client/src/compoundAnalysis/components/JustSum.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/compoundAnalysis/components/ModeSelector.tsx` & `libertem-0.9.2/client/src/compoundAnalysis/components/ModeSelector.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/compoundAnalysis/components/PointSelectionAnalysis.tsx` & `libertem-0.9.2/client/src/compoundAnalysis/components/PointSelectionAnalysis.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/compoundAnalysis/components/RadialFourierAnalysis.tsx` & `libertem-0.9.2/client/src/compoundAnalysis/components/RadialFourierAnalysis.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/compoundAnalysis/components/RingMaskAnalysis.tsx` & `libertem-0.9.2/client/src/compoundAnalysis/components/RingMaskAnalysis.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/compoundAnalysis/components/Toolbar.tsx` & `libertem-0.9.2/client/src/compoundAnalysis/components/Toolbar.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/compoundAnalysis/components/base/Analysis.tsx` & `libertem-0.9.2/client/src/compoundAnalysis/components/base/Analysis.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/compoundAnalysis/components/base/AnalysisSelect.tsx` & `libertem-0.9.2/client/src/compoundAnalysis/components/base/AnalysisSelect.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/compoundAnalysis/components/layouts/AnalysisLayoutThreeCol.tsx` & `libertem-0.9.2/client/src/compoundAnalysis/components/layouts/AnalysisLayoutThreeCol.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/compoundAnalysis/components/layouts/AnalysisLayoutTwoCol.tsx` & `libertem-0.9.2/client/src/compoundAnalysis/components/layouts/AnalysisLayoutTwoCol.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/compoundAnalysis/components/layouts/AnalysisLayoutTwoRes.tsx` & `libertem-0.9.2/client/src/compoundAnalysis/components/layouts/AnalysisLayoutTwoRes.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/compoundAnalysis/components/roi/DiskROI.tsx` & `libertem-0.9.2/client/src/compoundAnalysis/components/roi/DiskROI.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/compoundAnalysis/components/roi/RectROI.tsx` & `libertem-0.9.2/client/src/compoundAnalysis/components/roi/RectROI.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/compoundAnalysis/components/roi/RoiPicker.tsx` & `libertem-0.9.2/client/src/compoundAnalysis/components/roi/RoiPicker.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/compoundAnalysis/helpers.ts` & `libertem-0.9.2/client/src/compoundAnalysis/helpers.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/compoundAnalysis/reducers.ts` & `libertem-0.9.2/client/src/compoundAnalysis/reducers.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/compoundAnalysis/sagas.ts` & `libertem-0.9.2/client/src/compoundAnalysis/sagas.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/compoundAnalysis/types.ts` & `libertem-0.9.2/client/src/compoundAnalysis/types.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/config/__tests__/helpers.ts` & `libertem-0.9.2/client/src/config/__tests__/helpers.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/config/__tests__/reducers.ts` & `libertem-0.9.2/client/src/config/__tests__/reducers.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/config/actions.ts` & `libertem-0.9.2/client/src/config/actions.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/config/helpers.ts` & `libertem-0.9.2/client/src/config/helpers.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/config/reducers.ts` & `libertem-0.9.2/client/src/config/reducers.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/config/sagas.ts` & `libertem-0.9.2/client/src/config/sagas.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/dataset/__tests__/validate.ts` & `libertem-0.9.2/client/src/dataset/__tests__/validate.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/dataset/actions.ts` & `libertem-0.9.2/client/src/dataset/actions.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/dataset/api.ts` & `libertem-0.9.2/client/src/dataset/api.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/dataset/components/AddAnalysis.tsx` & `libertem-0.9.2/client/src/dataset/components/AddAnalysis.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/dataset/components/BLOParamsForm.tsx` & `libertem-0.9.2/client/src/dataset/components/BLOParamsForm.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/dataset/components/BackendSelectionDropdown.tsx` & `libertem-0.9.2/client/src/dataset/components/BackendSelectionDropdown.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/dataset/components/Dataset.tsx` & `libertem-0.9.2/client/src/dataset/components/Dataset.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/dataset/components/DatasetInfo.tsx` & `libertem-0.9.2/client/src/dataset/components/DatasetInfo.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/dataset/components/DatasetList.tsx` & `libertem-0.9.2/client/src/dataset/components/DatasetList.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/dataset/components/DatasetOpen.tsx` & `libertem-0.9.2/client/src/dataset/components/DatasetOpen.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/dataset/components/DatasetOpenSpinner.tsx` & `libertem-0.9.2/client/src/dataset/components/DatasetOpenSpinner.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/dataset/components/DatasetParams.tsx` & `libertem-0.9.2/client/src/dataset/components/DatasetParams.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/dataset/components/DatasetToolbar.tsx` & `libertem-0.9.2/client/src/dataset/components/DatasetToolbar.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/dataset/components/DatasetTypeSelect.tsx` & `libertem-0.9.2/client/src/dataset/components/DatasetTypeSelect.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/dataset/components/EMPADParamsForm.tsx` & `libertem-0.9.2/client/src/dataset/components/EMPADParamsForm.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/dataset/components/FRMS6ParamsForm.tsx` & `libertem-0.9.2/client/src/dataset/components/FRMS6ParamsForm.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/dataset/components/HDF5ParamsForm.tsx` & `libertem-0.9.2/client/src/dataset/components/HDF5ParamsForm.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/dataset/components/K2ISParamsForm.tsx` & `libertem-0.9.2/client/src/dataset/components/K2ISParamsForm.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/dataset/components/MIBParamsForm.tsx` & `libertem-0.9.2/client/src/dataset/components/MIBParamsForm.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/dataset/components/MRCParamsForm.tsx` & `libertem-0.9.2/client/src/dataset/components/MRCParamsForm.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/dataset/components/RawFileParamsForm.tsx` & `libertem-0.9.2/client/src/dataset/components/RawFileParamsForm.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/dataset/components/Reshape.tsx` & `libertem-0.9.2/client/src/dataset/components/Reshape.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/dataset/components/SEQParamsForm.tsx` & `libertem-0.9.2/client/src/dataset/components/SEQParamsForm.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/dataset/components/SERParamsForm.tsx` & `libertem-0.9.2/client/src/dataset/components/SERParamsForm.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/dataset/components/TVIPSParamsForm.tsx` & `libertem-0.9.2/client/src/dataset/components/TVIPSParamsForm.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/dataset/components/TupleInput.tsx` & `libertem-0.9.2/client/src/dataset/components/TupleInput.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/dataset/components/TupleInputPart.tsx` & `libertem-0.9.2/client/src/dataset/components/TupleInputPart.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/dataset/helpers.ts` & `libertem-0.9.2/client/src/dataset/helpers.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/dataset/reducers.ts` & `libertem-0.9.2/client/src/dataset/reducers.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/dataset/sagas.ts` & `libertem-0.9.2/client/src/dataset/sagas.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/dataset/types.ts` & `libertem-0.9.2/client/src/dataset/types.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/dataset/validate.ts` & `libertem-0.9.2/client/src/dataset/validate.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/errors/actions.ts` & `libertem-0.9.2/client/src/errors/actions.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/errors/components/Error.tsx` & `libertem-0.9.2/client/src/errors/components/Error.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/errors/components/ErrorList.tsx` & `libertem-0.9.2/client/src/errors/components/ErrorList.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/errors/reducers.ts` & `libertem-0.9.2/client/src/errors/reducers.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/helpers/__tests__/reducerHelpers.ts` & `libertem-0.9.2/client/src/helpers/__tests__/reducerHelpers.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/helpers/actionHelpers.ts` & `libertem-0.9.2/client/src/helpers/actionHelpers.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/helpers/apiHelpers.ts` & `libertem-0.9.2/client/src/helpers/apiHelpers.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/helpers/index.ts` & `libertem-0.9.2/client/src/helpers/index.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/helpers/reducerHelpers.ts` & `libertem-0.9.2/client/src/helpers/reducerHelpers.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/helpers/svg.ts` & `libertem-0.9.2/client/src/helpers/svg.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/images/LiberTEM logo-medium.png` & `libertem-0.9.2/client/src/images/LiberTEM logo-medium.png`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/index.tsx` & `libertem-0.9.2/client/src/index.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/job/api.ts` & `libertem-0.9.2/client/src/job/api.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/job/components/PlaceholderImage.tsx` & `libertem-0.9.2/client/src/job/components/PlaceholderImage.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/job/components/Result.tsx` & `libertem-0.9.2/client/src/job/components/Result.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/job/components/ResultImage.tsx` & `libertem-0.9.2/client/src/job/components/ResultImage.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/job/components/ResultList.tsx` & `libertem-0.9.2/client/src/job/components/ResultList.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/job/reducers.ts` & `libertem-0.9.2/client/src/job/reducers.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/job/types.ts` & `libertem-0.9.2/client/src/job/types.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/messages.ts` & `libertem-0.9.2/client/src/messages.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/registerServiceWorker.ts` & `libertem-0.9.2/client/src/registerServiceWorker.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/sagas.ts` & `libertem-0.9.2/client/src/sagas.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/shutdown/components/ShutdownButton.tsx` & `libertem-0.9.2/client/src/shutdown/components/ShutdownButton.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/store.ts` & `libertem-0.9.2/client/src/store.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/widgets/DraggableHandle.tsx` & `libertem-0.9.2/client/src/widgets/DraggableHandle.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/widgets/HandleParent.tsx` & `libertem-0.9.2/client/src/widgets/HandleParent.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/widgets/Rect.tsx` & `libertem-0.9.2/client/src/widgets/Rect.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/widgets/Ring.tsx` & `libertem-0.9.2/client/src/widgets/Ring.tsx`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/widgets/constraints.ts` & `libertem-0.9.2/client/src/widgets/constraints.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/src/widgets/kbdHandler.ts` & `libertem-0.9.2/client/src/widgets/kbdHandler.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/tsconfig.json` & `libertem-0.9.2/client/tsconfig.json`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/client/types/react-window.d.ts` & `libertem-0.9.2/client/types/react-window.d.ts`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/setup.cfg` & `libertem-0.9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/setup.py` & `libertem-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/__pycache__/api.cpython-39.pyc` & `libertem-0.9.2/src/libertem/__pycache__/api.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 49144 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 f8bf 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 f8bf 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 2802 0000 6400  .....@...s(...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 6d07 5a07  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d08 5a08 6d09 5a09 6d0a 5a0a 0100 6400  m.Z.m.Z.m.Z...d.
 00000060: 6402 6c0b 6d0c 5a0c 0100 6400 6403 6c0d  d.l.m.Z...d.d.l.
 00000070: 5a0d 6400 6403 6c0e 5a0f 6400 6404 6c10  Z.d.d.l.Z.d.d.l.
```

### Comparing `libertem-0.9.0/src/libertem/__pycache__/masks.cpython-39.pyc` & `libertem-0.9.2/src/libertem/__pycache__/masks.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 13962 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 8a36 0000  a.......z..b.6..
+00000000: 610d 0d0a 0000 0000 7fce 6762 8a36 0000  a.........gb.6..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 2401 0000 6400  .....@...s$...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c04 5a05 6400 6402 6c06  ..d.d.l.Z.d.d.l.
 00000050: 6d07 5a08 0100 6400 6402 6c07 5a07 6400  m.Z...d.d.l.Z.d.
 00000060: 6403 6c09 6d0a 5a0a 0100 6501 6505 6a0b  d.l.m.Z...e.e.j.
 00000070: 6508 6a0c 6a0d 6508 6a0e 6a0f 6603 1900  e.j.j.e.j.j.f...
```

### Comparing `libertem-0.9.0/src/libertem/__pycache__/warnings.cpython-39.pyc` & `libertem-0.9.2/src/libertem/__pycache__/warnings.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 473 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 d901 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 d901 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 1800 0000 6400  .....@...s....d.
 00000030: 5a00 4700 6401 6402 8400 6402 6501 8303  Z.G.d.d...d.e...
 00000040: 5a02 6403 5300 2904 7af2 0a43 7573 746f  Z.d.S.).z..Custo
 00000050: 6d20 7761 726e 696e 6720 7375 6263 6c61  m warning subcla
 00000060: 7373 6573 2e20 5573 6566 756c 2066 6f72  sses. Useful for
 00000070: 2073 656c 6563 7469 7665 6c79 2066 696c   selectively fil
```

### Comparing `libertem-0.9.0/src/libertem/analysis/__init__.py` & `libertem-0.9.2/src/libertem/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/analysis/__pycache__/__init__.cpython-39.pyc` & `libertem-0.9.2/src/libertem/analysis/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 877 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 6d03 0000  a.......z..bm...
+00000000: 610d 0d0a 0000 0000 7fce 6762 6d03 0000  a.........gbm...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 c000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 0100 6400 6406 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6400 6407 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
```

### Comparing `libertem-0.9.0/src/libertem/analysis/__pycache__/apply_fft_mask.cpython-39.pyc` & `libertem-0.9.2/src/libertem/analysis/__pycache__/apply_fft_mask.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 2030 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 ee07 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 ee07 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 5a00 0000 6400  .....@...sZ...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6402 6403 6c04 6d05 0200 0100 6d06  ..d.d.l.m.....m.
 00000050: 5a07 0100 6400 6404 6c08 6d09 5a09 0100  Z...d.d.l.m.Z...
 00000060: 4700 6405 6406 8400 6406 6509 8303 5a0a  G.d.d...d.e...Z.
 00000070: 4700 6407 6408 8400 6408 6501 6409 640a  G.d.d...d.e.d.d.
```

### Comparing `libertem-0.9.0/src/libertem/analysis/__pycache__/base.cpython-39.pyc` & `libertem-0.9.2/src/libertem/analysis/__pycache__/base.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 11471 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 cf2c 0000  a.......z..b.,..
+00000000: 610d 0d0a 0000 0000 7fce 6762 cf2c 0000  a.........gb.,..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 ea00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 0100 6400  m.Z.m.Z.m.Z...d.
 00000060: 6403 6c0a 6d0b 5a0b 0100 6400 6404 6c0c  d.l.m.Z...d.d.l.
 00000070: 5a0d 6400 6405 6c0e 6d0f 5a0f 0100 6400  Z.d.d.l.m.Z...d.
```

### Comparing `libertem-0.9.0/src/libertem/analysis/__pycache__/clust.cpython-39.pyc` & `libertem-0.9.2/src/libertem/analysis/__pycache__/clust.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 7864 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 b81e 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 b81e 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 c000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a03 6400 6401 6c04 5a04 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c05 6d06 5a06 0100 6403 6404 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 0100 6400  m.Z.m.Z.m.Z...d.
 00000070: 6405 6c0b 6d0c 5a0c 0100 6400 6406 6c0d  d.l.m.Z...d.d.l.
```

### Comparing `libertem-0.9.0/src/libertem/analysis/__pycache__/com.cpython-39.pyc` & `libertem-0.9.2/src/libertem/analysis/__pycache__/com.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 22450 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 b257 0000  a.......z..b.W..
+00000000: 610d 0d0a 0000 0000 7fce 6762 b257 0000  a.........gb.W..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 6c01 0000 6400  .....@...sl...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 6d05 5a05  d.l.m.Z.m.Z.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 0100 6400 6401 6c0a 5a0b 6400 6403 6c0c  ..d.d.l.Z.d.d.l.
 00000070: 6d0d 5a0d 0100 6400 6404 6c0e 6d0f 5a0f  m.Z...d.d.l.m.Z.
```

### Comparing `libertem-0.9.0/src/libertem/analysis/__pycache__/disk.cpython-39.pyc` & `libertem-0.9.2/src/libertem/analysis/__pycache__/disk.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 2371 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 4309 0000  a.......z..bC...
+00000000: 610d 0d0a 0000 0000 7fce 6762 4309 0000  a.........gbC...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 0100 6403 6404 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6403 6405 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 4700 6406 6407 8400 6407 6507 8303  ..G.d.d...d.e...
 00000070: 5a08 4700 6408 6409 8400 6409 6505 640a  Z.G.d.d...d.e.d.
```

### Comparing `libertem-0.9.0/src/libertem/analysis/__pycache__/fem.cpython-39.pyc` & `libertem-0.9.2/src/libertem/analysis/__pycache__/fem.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 2200 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 9808 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 9808 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 6401 6c00 5a00 6402 6403 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 6d04 5a04 0100 6402 6404 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6401 6c07 6d08 0200  m.Z...d.d.l.m...
 00000060: 0100 6d09 5a09 0100 4700 6405 6406 8400  ..m.Z...G.d.d...
 00000070: 6406 6506 8303 5a0a 4700 6407 6408 8400  d.e...Z.G.d.d...
```

### Comparing `libertem-0.9.0/src/libertem/analysis/__pycache__/fullmatch.cpython-39.pyc` & `libertem-0.9.2/src/libertem/analysis/__pycache__/fullmatch.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 16383 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 ff3f 0000  a.......z..b.?..
+00000000: 610d 0d0a 0000 0000 7fce 6762 ff3f 0000  a.........gb.?..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7a00 0000 6400  .....@...sz...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a03 6400 6401 6c04 6d05 0200  d.l.Z.d.d.l.m...
 00000050: 0100 6d06 5a07 0100 6400 6402 6c08 6d09  ..m.Z...d.d.l.m.
 00000060: 5a09 6d0a 5a0a 0100 6500 a00b 650c a101  Z.m.Z...e...e...
 00000070: 5a0d 4700 6403 6404 8400 6404 650e 8303  Z.G.d.d...d.e...
```

### Comparing `libertem-0.9.0/src/libertem/analysis/__pycache__/getroi.cpython-39.pyc` & `libertem-0.9.2/src/libertem/analysis/__pycache__/getroi.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 669 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 9d02 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 9d02 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 1800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6403 8400  d.l.m.Z...d.d...
 00000040: 5a02 6404 5300 2905 e900 0000 0029 01da  Z.d.S.)......)..
 00000050: 056d 6173 6b73 6302 0000 0000 0000 0000  .masksc.........
 00000060: 0000 0005 0000 0008 0000 0043 0000 0073  ...........C...s
 00000070: 9e00 0000 6401 7c00 7601 7314 6402 7c00  ....d.|.v.s.d.|.
```

### Comparing `libertem-0.9.0/src/libertem/analysis/__pycache__/gridmatching.cpython-39.pyc` & `libertem-0.9.2/src/libertem/analysis/__pycache__/gridmatching.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 18296 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 7847 0000  a.......z..bxG..
+00000000: 610d 0d0a 0000 0000 7fce 6762 7847 0000  a.........gbxG..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7a00 0000 6400  .....@...sz...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 6d04 5a04 0100 4700 6403 6404 8400 6404  m.Z...G.d.d...d.
 00000050: 8302 5a05 4700 6405 6406 8400 6406 8302  ..Z.G.d.d...d...
 00000060: 5a06 4700 6407 6408 8400 6408 8302 5a07  Z.G.d.d...d...Z.
 00000070: 4700 6409 640a 8400 640a 6506 8303 5a08  G.d.d...d.e...Z.
```

### Comparing `libertem-0.9.0/src/libertem/analysis/__pycache__/helper.cpython-39.pyc` & `libertem-0.9.2/src/libertem/analysis/__pycache__/helper.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 2593 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 210a 0000  a.......z..b!...
+00000000: 610d 0d0a 0000 0000 7fce 6762 210a 0000  a.........gb!...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 4700 6403 6404 8400 6404  m.Z...G.d.d...d.
 00000050: 6503 8303 5a04 6405 5300 2906 e900 0000  e...Z.d.S.).....
 00000060: 0029 01da 084f 7074 696f 6e61 6c29 01da  .)...Optional)..
 00000070: 0c54 656d 706c 6174 6542 6173 6563 0000  .TemplateBasec..
```

### Comparing `libertem-0.9.0/src/libertem/analysis/__pycache__/masks.cpython-39.pyc` & `libertem-0.9.2/src/libertem/analysis/__pycache__/masks.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 7319 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 971c 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 971c 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6402 6403 6c04 6d05 5a05 0100 6402  ..d.d.l.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 4700 6405 6406  d.l.m.Z...G.d.d.
 00000060: 8400 6406 6501 8303 5a08 4700 6407 6408  ..d.e...Z.G.d.d.
 00000070: 8400 6408 6508 8303 5a09 4700 6409 640a  ..d.e...Z.G.d.d.
```

### Comparing `libertem-0.9.0/src/libertem/analysis/__pycache__/point.cpython-39.pyc` & `libertem-0.9.2/src/libertem/analysis/__pycache__/point.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 2145 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 6108 0000  a.......z..ba...
+00000000: 610d 0d0a 0000 0000 7fce 6762 6108 0000  a.........gba...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 5800 0000 6400  .....@...sX...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a03 6402 6403 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6402 6404 6c06 6d07 5a07 0100 4700  ..d.d.l.m.Z...G.
 00000060: 6405 6406 8400 6406 6507 8303 5a08 4700  d.d...d.e...Z.G.
 00000070: 6407 6408 8400 6408 6505 6409 640a 8d04  d.d...d.e.d.d...
```

### Comparing `libertem-0.9.0/src/libertem/analysis/__pycache__/radialfourier.cpython-39.pyc` & `libertem-0.9.2/src/libertem/analysis/__pycache__/radialfourier.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 12805 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 0532 0000  a.......z..b.2..
+00000000: 610d 0d0a 0000 0000 7fce 6762 0532 0000  a.........gb.2..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 ae00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6401 6c04  d.l.m.Z...d.d.l.
 00000050: 5a05 6400 6401 6c06 5a06 6400 6403 6c07  Z.d.d.l.Z.d.d.l.
 00000060: 6d08 5a08 0100 6400 6404 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6405 6406 6c0b 6d0c 5a0c 6d0d 5a0d  ..d.d.l.m.Z.m.Z.
```

### Comparing `libertem-0.9.0/src/libertem/analysis/__pycache__/raw.cpython-39.pyc` & `libertem-0.9.2/src/libertem/analysis/__pycache__/raw.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 5522 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 9215 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 9215 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 0100 6403 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 6403  m.Z.m.Z.m.Z...d.
 00000060: 6405 6c09 6d0a 5a0a 0100 4700 6406 6407  d.l.m.Z...G.d.d.
 00000070: 8400 6407 650a 8303 5a0b 4700 6408 6409  ..d.e...Z.G.d.d.
```

### Comparing `libertem-0.9.0/src/libertem/analysis/__pycache__/rawfft.cpython-39.pyc` & `libertem-0.9.2/src/libertem/analysis/__pycache__/rawfft.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 2008 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 d807 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 d807 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6403 6404 6c04 6d05 5a05 0100 6403  ..d.d.l.m.Z...d.
 00000050: 6405 6c06 6d07 5a07 0100 4700 6406 6407  d.l.m.Z...G.d.d.
 00000060: 8400 6407 6507 8303 5a08 4700 6408 6409  ..d.e...Z.G.d.d.
 00000070: 8400 6409 6505 640a 640b 8d04 5a09 6401  ..d.e.d.d...Z.d.
```

### Comparing `libertem-0.9.0/src/libertem/analysis/__pycache__/ring.cpython-39.pyc` & `libertem-0.9.2/src/libertem/analysis/__pycache__/ring.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 2385 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 5109 0000  a.......z..bQ...
+00000000: 610d 0d0a 0000 0000 7fce 6762 5109 0000  a.........gbQ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 0100 6403 6404 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6403 6405 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 4700 6406 6407 8400 6407 6507 8303  ..G.d.d...d.e...
 00000070: 5a08 4700 6408 6409 8400 6409 6505 640a  Z.G.d.d...d.e.d.
```

### Comparing `libertem-0.9.0/src/libertem/analysis/__pycache__/sd.cpython-39.pyc` & `libertem-0.9.2/src/libertem/analysis/__pycache__/sd.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 2659 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 630a 0000  a.......z..bc...
+00000000: 610d 0d0a 0000 0000 7fce 6762 630a 0000  a.........gbc...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
 00000030: 6401 6c00 5a00 6402 6403 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6401 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 0200 0100 6d07 5a08 0100 6400 6404  m.....m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 0100 6402 6405 6c0b 6d0c  l.m.Z...d.d.l.m.
 00000070: 5a0c 0100 4700 6406 6407 8400 6407 650c  Z...G.d.d...d.e.
```

### Comparing `libertem-0.9.0/src/libertem/analysis/__pycache__/sum.cpython-39.pyc` & `libertem-0.9.2/src/libertem/analysis/__pycache__/sum.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 4987 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 7b13 0000  a.......z..b{...
+00000000: 610d 0d0a 0000 0000 7fce 6762 7b13 0000  a.........gb{...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a02 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6404 6c07 6d08 5a08 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c09 6d0a 5a0a 0100 6402 6406 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 4700 6407 6408 8400 6408  m.Z...G.d.d...d.
@@ -253,15 +253,15 @@
 00000fc0: 017a 1353 756d 416e 616c 7973 6973 2e67  .z.SumAnalysis.g
 00000fd0: 6574 5f75 6466 6301 0000 0000 0000 0000  et_udfc.........
 00000fe0: 0000 0001 0000 0004 0000 0043 0000 0073  ...........C...s
 00000ff0: 1400 0000 7400 7c00 6a01 7c00 6a02 6a03  ....t.|.j.|.j.j.
 00001000: 6a04 6401 8d02 5300 2902 4e29 0272 0c00  j.d...S.).N).r..
 00001010: 0000 da05 7368 6170 6529 0572 0600 0000  ....shape).r....
 00001020: da0a 7061 7261 6d65 7465 7273 7227 0000  ..parametersr'..
-00001030: 0072 2a00 0000 5a03 6e61 7672 1100 0000  .r*...Z.navr....
+00001030: 0072 2a00 0000 da03 6e61 7672 1100 0000  .r*.....navr....
 00001040: 720e 0000 0072 0e00 0000 720f 0000 0072  r....r....r....r
 00001050: 0600 0000 6400 0000 7302 0000 0000 017a  ....d...s......z
 00001060: 1353 756d 416e 616c 7973 6973 2e67 6574  .SumAnalysis.get
 00001070: 5f72 6f69 6304 0000 0000 0000 0000 0000  _roic...........
 00001080: 0005 0000 0009 0000 0043 0000 0073 9200  .........C...s..
 00001090: 0000 6401 6402 6c00 6d01 7d04 0100 7c01  ..d.d.l.m.}...|.
 000010a0: 6403 1900 6a02 6a03 6a04 6404 6b02 723e  d...j.j.j.d.k.r>
@@ -276,30 +276,30 @@
 00001130: 7669 7375 616c 697a 655f 7369 6d70 6c65  visualize_simple
 00001140: 5a09 696e 7465 6e73 6974 7972 2300 0000  Z.intensityr#...
 00001150: 7a11 7375 6d20 6f66 2061 6c6c 2066 7261  z.sum of all fra
 00001160: 6d65 7354 4629 055a 0a6b 6579 5f70 7265  mesTF).Z.key_pre
 00001170: 6669 7872 1500 0000 da04 6465 7363 da06  fixr......desc..
 00001180: 6461 6d61 6765 5a0b 6465 6661 756c 745f  damageZ.default_
 00001190: 6c69 6e29 025a 0b6c 6f67 6172 6974 686d  lin).Z.logarithm
-000011a0: 6963 722e 0000 007a 0f69 6e74 656e 7369  icr....z.intensi
+000011a0: 6963 722f 0000 007a 0f69 6e74 656e 7369  icr/...z.intensi
 000011b0: 7479 205b 6c6f 675d 7a18 7375 6d20 6f66  ty [log]z.sum of
 000011c0: 2066 7261 6d65 7320 6c6f 672d 7363 616c   frames log-scal
 000011d0: 6564 2905 da08 7261 775f 6461 7461 5a0a  ed)...raw_dataZ.
 000011e0: 7669 7375 616c 697a 6564 da03 6b65 7972  visualized..keyr
-000011f0: 1500 0000 722d 0000 005a 0d69 6e74 656e  ....r-...Z.inten
+000011f0: 1500 0000 722e 0000 005a 0d69 6e74 656e  ....r....Z.inten
 00001200: 7369 7479 5f6c 696e 7a0f 696e 7465 6e73  sity_linz.intens
 00001210: 6974 7920 5b6c 696e 5d7a 1873 756d 206f  ity [lin]z.sum o
 00001220: 6620 6672 616d 6573 206c 696e 2d73 6361  f frames lin-sca
 00001230: 6c65 6429 095a 0c6c 6962 6572 7465 6d2e  led).Z.libertem.
-00001240: 7669 7a72 2c00 0000 da04 6461 7461 7225  vizr,.....datar%
+00001240: 7669 7a72 2d00 0000 da04 6461 7461 7225  vizr-.....datar%
 00001250: 0000 0072 2800 0000 7205 0000 005a 1367  ...r(...r....Z.g
 00001260: 6574 5f63 6f6d 706c 6578 5f72 6573 756c  et_complex_resul
 00001270: 7473 7220 0000 0072 0400 0000 2905 720d  tsr ...r....).r.
 00001280: 0000 005a 0b75 6466 5f72 6573 756c 7473  ...Z.udf_results
-00001290: 721a 0000 0072 2e00 0000 722c 0000 0072  r....r....r,...r
+00001290: 721a 0000 0072 2f00 0000 722d 0000 0072  r....r/...r-...r
 000012a0: 0e00 0000 720e 0000 0072 0f00 0000 da0f  ....r....r......
 000012b0: 6765 745f 7564 665f 7265 7375 6c74 7367  get_udf_resultsg
 000012c0: 0000 0073 3a00 0000 0001 0c01 1201 0201  ...s:...........
 000012d0: 0401 0801 0201 0201 0201 0201 02fa 04ff  ................
 000012e0: 040b 0201 0201 0801 0201 0a01 02fe 0404  ................
 000012f0: 06fa 0408 0a01 0201 0a01 02fe 0404 06fb  ................
 00001300: 04f7 7a1b 5375 6d41 6e61 6c79 7369 732e  ..z.SumAnalysis.
@@ -310,16 +310,16 @@
 00001350: 0363 6c73 720e 0000 0072 0e00 0000 720f  .clsr....r....r.
 00001360: 0000 00da 1367 6574 5f74 656d 706c 6174  .....get_templat
 00001370: 655f 6865 6c70 6572 8700 0000 7302 0000  e_helper....s...
 00001380: 0000 027a 1f53 756d 416e 616c 7973 6973  ...z.SumAnalysis
 00001390: 2e67 6574 5f74 656d 706c 6174 655f 6865  .get_template_he
 000013a0: 6c70 6572 4e29 0972 1d00 0000 721e 0000  lperN).r....r...
 000013b0: 0072 1f00 0000 da04 5459 5045 7229 0000  .r......TYPEr)..
-000013c0: 0072 0600 0000 7232 0000 00da 0b63 6c61  .r....r2.....cla
-000013d0: 7373 6d65 7468 6f64 7234 0000 0072 0e00  ssmethodr4...r..
+000013c0: 0072 0600 0000 7233 0000 00da 0b63 6c61  .r....r3.....cla
+000013d0: 7373 6d65 7468 6f64 7235 0000 0072 0e00  ssmethodr5...r..
 000013e0: 0000 720e 0000 0072 0e00 0000 720f 0000  ..r....r....r...
 000013f0: 0072 2200 0000 5b00 0000 730c 0000 0008  .r"...[...s.....
 00001400: 0104 0208 0608 0308 2002 0172 2200 0000  ........ ..r"...
 00001410: 5a0a 5355 4d5f 4652 414d 4553 2901 da03  Z.SUM_FRAMES)...
 00001420: 6964 5f29 10da 056e 756d 7079 7226 0000  id_)...numpyr&..
 00001430: 0072 1300 0000 da04 6261 7365 7203 0000  .r......baser...
 00001440: 0072 0400 0000 7205 0000 005a 186c 6962  .r....r....Z.lib
```

### Comparing `libertem-0.9.0/src/libertem/analysis/__pycache__/sumfft.cpython-39.pyc` & `libertem-0.9.2/src/libertem/analysis/__pycache__/sumfft.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 2280 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 e808 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 e808 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6403 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 0100 6403 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6406 6c09 5a0a 4700 6407 6408  ..d.d.l.Z.G.d.d.
 00000070: 8400 6408 6508 8303 5a0b 4700 6409 640a  ..d.e...Z.G.d.d.
```

### Comparing `libertem-0.9.0/src/libertem/analysis/__pycache__/sumsig.cpython-39.pyc` & `libertem-0.9.2/src/libertem/analysis/__pycache__/sumsig.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 1687 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 9706 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 9706 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 5a00 0000 6400  .....@...sZ...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6402 6403 6c04 6d05 0200 0100 6d06  ..d.d.l.m.....m.
 00000050: 5a06 0100 6400 6404 6c07 6d08 5a08 0100  Z...d.d.l.m.Z...
 00000060: 4700 6405 6406 8400 6406 6508 8303 5a09  G.d.d...d.e...Z.
 00000070: 4700 6407 6408 8400 6408 6501 6409 640a  G.d.d...d.e.d.d.
```

### Comparing `libertem-0.9.0/src/libertem/analysis/apply_fft_mask.py` & `libertem-0.9.2/src/libertem/analysis/apply_fft_mask.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/analysis/base.py` & `libertem-0.9.2/src/libertem/analysis/base.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/analysis/clust.py` & `libertem-0.9.2/src/libertem/analysis/clust.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/analysis/com.py` & `libertem-0.9.2/src/libertem/analysis/com.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/analysis/disk.py` & `libertem-0.9.2/src/libertem/analysis/disk.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/analysis/fem.py` & `libertem-0.9.2/src/libertem/analysis/fem.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/analysis/fullmatch.py` & `libertem-0.9.2/src/libertem/analysis/fullmatch.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/analysis/getroi.py` & `libertem-0.9.2/src/libertem/analysis/getroi.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/analysis/gridmatching.py` & `libertem-0.9.2/src/libertem/analysis/gridmatching.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/analysis/helper.py` & `libertem-0.9.2/src/libertem/analysis/helper.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/analysis/masks.py` & `libertem-0.9.2/src/libertem/analysis/masks.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/analysis/point.py` & `libertem-0.9.2/src/libertem/analysis/point.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/analysis/radialfourier.py` & `libertem-0.9.2/src/libertem/analysis/radialfourier.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/analysis/raw.py` & `libertem-0.9.2/src/libertem/analysis/raw.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/analysis/rawfft.py` & `libertem-0.9.2/src/libertem/analysis/rawfft.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/analysis/ring.py` & `libertem-0.9.2/src/libertem/analysis/ring.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/analysis/sd.py` & `libertem-0.9.2/src/libertem/analysis/sd.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/analysis/sum.py` & `libertem-0.9.2/src/libertem/analysis/sum.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/analysis/sumfft.py` & `libertem-0.9.2/src/libertem/analysis/sumfft.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/analysis/sumsig.py` & `libertem-0.9.2/src/libertem/analysis/sumsig.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/api.py` & `libertem-0.9.2/src/libertem/api.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/common/LICENSE` & `libertem-0.9.2/src/libertem/common/LICENSE`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/common/__pycache__/backend.cpython-39.pyc` & `libertem-0.9.2/src/libertem/common/__pycache__/backend.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 2754 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 c20a 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 c20a 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5600 0000 6400  .....@...sV...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6502 6503 1900 6403 9c01 6404 6405  ..e.e...d...d.d.
 00000050: 8404 5a04 6503 6406 9c01 6407 6408 8404  ..Z.e.d...d.d...
 00000060: 5a05 6409 640a 8400 5a06 6503 640b 9c01  Z.d.d...Z.e.d...
 00000070: 640c 640d 8404 5a07 640e 640f 8400 5a08  d.d...Z.d.d...Z.
```

### Comparing `libertem-0.9.0/src/libertem/common/__pycache__/buffers.cpython-39.pyc` & `libertem-0.9.2/src/libertem/common/__pycache__/buffers.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 23927 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 775d 0000  a.......z..bw]..
+00000000: 610d 0d0a 0000 0000 7fce 6762 775d 0000  a.........gbw]..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 a801 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6402 6c07 6d08 5a08 0100 6400 6403 6c09  d.l.m.Z...d.d.l.
 00000060: 5a09 6400 6403 6c0a 5a0a 6400 6404 6c0b  Z.d.d.l.Z.d.d.l.
 00000070: 6d0c 5a0c 0100 6400 6403 6c0d 5a0d 6400  m.Z...d.d.l.Z.d.
@@ -515,15 +515,15 @@
 00002020: 7374 206f 6620 6461 7461 7365 7420 7061  st of dataset pa
 00002030: 7274 6974 696f 6e73 2074 6f20 7468 6520  rtitions to the 
 00002040: 6275 6666 6572 2073 7563 6820 7468 6174  buffer such that
 00002050: 0a20 2020 2020 2020 2073 656c 662e 616c  .        self.al
 00002060: 6c6f 6361 7465 2829 2063 616e 206d 616b  locate() can mak
 00002070: 6520 7573 6520 6f66 2074 6865 2073 7472  e use of the str
 00002080: 7563 7475 7265 0a20 2020 2020 2020 204e  ucture.        N
-00002090: 2901 726f 0000 0029 0272 4f00 0000 5a0a  ).ro...).rO...Z.
+00002090: 2901 726f 0000 0029 0272 4f00 0000 da0a  ).ro...).rO.....
 000020a0: 7061 7274 6974 696f 6e73 721e 0000 0072  partitionsr....r
 000020b0: 1e00 0000 721f 0000 00da 0e61 6464 5f70  ....r......add_p
 000020c0: 6172 7469 7469 6f6e 73f1 0000 0073 0200  artitions....s..
 000020d0: 0000 0005 7a1c 4275 6666 6572 5772 6170  ....z.BufferWrap
 000020e0: 7065 722e 6164 645f 7061 7274 6974 696f  per.add_partitio
 000020f0: 6e73 6303 0000 0000 0000 0000 0000 0005  nsc.............
 00002100: 0000 0005 0000 0043 0000 0073 7e00 0000  .......C...s~...
@@ -554,20 +554,20 @@
 00002290: 6f6e 6303 0000 0000 0000 0000 0000 0004  onc.............
 000022a0: 0000 0005 0000 0043 0000 0073 4a00 0000  .......C...sJ...
 000022b0: 7c00 a000 7c02 a101 0100 6400 7d03 7c02  |...|.....d.}.|.
 000022c0: 6400 7501 7222 7401 a002 7c00 6a03 a101  d.u.r"t...|.j...
 000022d0: 7d03 7c00 a004 7c00 6a05 7c01 a006 a100  }.|...|.j.|.....
 000022e0: 7c03 a103 7c00 5f07 7c00 a008 a100 0100  |...|._.|.......
 000022f0: 7c01 7c00 5f09 6400 5300 7221 0000 0029  |.|._.d.S.r!...)
-00002300: 0a72 7a00 0000 7227 0000 0072 8000 0000  .rz...r'...r....
-00002310: 7270 0000 0072 8100 0000 7268 0000 00da  rp...r....rh....
+00002300: 0a72 7a00 0000 7227 0000 0072 8100 0000  .rz...r'...r....
+00002310: 7270 0000 0072 8200 0000 7268 0000 00da  rp...r....rh....
 00002320: 0b66 6c61 7474 656e 5f6e 6176 726d 0000  .flatten_navrm..
-00002330: 0072 8200 0000 726e 0000 0029 0472 4f00  .r....rn...).rO.
+00002330: 0072 8300 0000 726e 0000 0029 0472 4f00  .r....rn...).rO.
 00002340: 0000 5a0d 6461 7461 7365 745f 7368 6170  ..Z.dataset_shap
-00002350: 6572 7900 0000 7284 0000 0072 1e00 0000  ery...r....r....
+00002350: 6572 7900 0000 7285 0000 0072 1e00 0000  ery...r....r....
 00002360: 721e 0000 0072 1f00 0000 da0c 7365 745f  r....r......set_
 00002370: 7368 6170 655f 6473 0301 0000 730e 0000  shape_ds....s...
 00002380: 0000 010a 0104 0108 010c 0116 0108 017a  ...............z
 00002390: 1a42 7566 6665 7257 7261 7070 6572 2e73  .BufferWrapper.s
 000023a0: 6574 5f73 6861 7065 5f64 7363 0100 0000  et_shape_dsc....
 000023b0: 0000 0000 0000 0000 0100 0000 0100 0000  ................
 000023c0: 4300 0000 7306 0000 007c 006a 0053 0072  C...s....|.j.S.r
@@ -588,17 +588,17 @@
 000024b0: 4e72 0f00 0000 7210 0000 0072 1100 0000  Nr....r....r....
 000024c0: 7201 0000 00a9 0172 0c00 0000 7a10 756e  r......r....z.un
 000024d0: 6b6e 6f77 6e20 6b69 6e64 3a20 2573 2907  known kind: %s).
 000024e0: 7268 0000 0072 6600 0000 720f 0000 0072  rh...rf...r....r
 000024f0: 6700 0000 7210 0000 00da 036c 656e da0a  g...r......len..
 00002500: 5661 6c75 6545 7272 6f72 2905 724f 0000  ValueError).rO..
 00002510: 0072 7500 0000 da0a 6f72 6967 5f73 6861  .ru.....orig_sha
-00002520: 7065 7284 0000 00da 096e 6176 5f73 6861  per......nav_sha
+00002520: 7065 7285 0000 00da 096e 6176 5f73 6861  per......nav_sha
 00002530: 7065 721e 0000 0072 1e00 0000 721f 0000  per....r....r...
-00002540: 0072 8100 0000 1101 0000 7318 0000 0000  .r........s.....
+00002540: 0072 8200 0000 1101 0000 7318 0000 0000  .r........s.....
 00002550: 010a 0108 010c 0206 010a 010a 0110 010a  ................
 00002560: 010e 0106 0206 027a 1d42 7566 6665 7257  .......z.BufferW
 00002570: 7261 7070 6572 2e5f 7368 6170 655f 666f  rapper._shape_fo
 00002580: 725f 6b69 6e64 6301 0000 0000 0000 0000  r_kindc.........
 00002590: 0000 0004 0000 0006 0000 0043 0000 0073  ...........C...s
 000025a0: b000 0000 7c00 6a00 720e 7401 6401 8301  ....|.j.r.t.d...
 000025b0: 8201 7c00 6a02 6402 7500 7322 7c00 6a03  ..|.j.d.u.s"|.j.
@@ -642,15 +642,15 @@
 00002810: 2020 2020 2020 20fa 2543 6163 6865 2069         .%Cache i
 00002820: 7320 6e6f 7420 656d 7074 792c 2068 6173  s not empty, has
 00002830: 2074 6f20 6265 2066 6c75 7368 6564 4e72   to be flushedNr
 00002840: 0f00 0000 2903 da01 69da 0175 da01 5672  ....)...i..u..Vr
 00002850: 0100 0000 2902 da01 53da 0155 da00 7226  ....)...S..U..r&
 00002860: 0000 0029 0f72 7300 0000 da0c 5275 6e74  ...).rs.....Runt
 00002870: 696d 6545 7272 6f72 7270 0000 0072 6800  imeErrorrp...rh.
-00002880: 0000 726b 0000 0072 2a00 0000 7281 0000  ..rk...r*...r...
+00002880: 0000 726b 0000 0072 2a00 0000 7282 0000  ..rk...r*...r...
 00002890: 0072 6e00 0000 723b 0000 0072 2400 0000  .rn...r;...r$...
 000028a0: 7275 0000 0072 2700 0000 da04 6675 6c6c  ru...r'.....full
 000028b0: 7269 0000 0072 0f00 0000 2904 724f 0000  ri...r....).rO..
 000028c0: 0072 3b00 0000 da04 6669 6c6c da07 7772  .r;.....fill..wr
 000028d0: 6170 7065 7272 1e00 0000 721e 0000 0072  apperr....r....r
 000028e0: 1f00 0000 da04 6461 7461 2201 0000 731e  ......data"...s.
 000028f0: 0000 0000 0c06 0108 0114 0118 0110 010c  ................
@@ -722,15 +722,15 @@
 00002d10: 5772 6170 7065 722e 7768 6572 6563 0100  Wrapper.wherec..
 00002d20: 0000 0000 0000 0000 0000 0100 0000 0100  ................
 00002d30: 0000 4300 0000 7306 0000 007c 006a 0053  ..C...s....|.j.S
 00002d40: 0029 017a 410a 2020 2020 2020 2020 7265  .).zA.        re
 00002d50: 7475 726e 7320 7468 6520 2277 7261 7070  turns the "wrapp
 00002d60: 6564 222f 7265 7368 6170 6564 2061 7272  ed"/reshaped arr
 00002d70: 6179 2c20 7365 6520 6162 6f76 650a 2020  ay, see above.  
-00002d80: 2020 2020 2020 2901 7299 0000 0072 4e00        ).r....rN.
+00002d80: 2020 2020 2020 2901 729a 0000 0072 4e00        ).r....rN.
 00002d90: 0000 721e 0000 0072 1e00 0000 721f 0000  ..r....r....r...
 00002da0: 00da 095f 5f61 7272 6179 5f5f 7201 0000  ...__array__r...
 00002db0: 7302 0000 0000 047a 1742 7566 6665 7257  s......z.BufferW
 00002dc0: 7261 7070 6572 2e5f 5f61 7272 6179 5f5f  rapper.__array__
 00002dd0: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
 00002de0: 0004 0000 0043 0000 0073 5800 0000 7c00  .....C...sX...|.
 00002df0: 6a00 6401 7500 7212 7401 6402 8301 8201  j.d.u.r.t.d.....
@@ -752,25 +752,25 @@
 00002ef0: 6c6c 6f63 6174 696e 6720 6f6e 2064 6576  llocating on dev
 00002f00: 6963 650a 2020 2020 2020 2020 4e7a 1d63  ice.        Nz.c
 00002f10: 616e 6e6f 7420 616c 6c6f 6361 7465 3a20  annot allocate: 
 00002f20: 6e6f 2073 6861 7065 2073 6574 7a24 6361  no shape setz$ca
 00002f30: 6e6e 6f74 2061 6c6c 6f63 6174 653a 2064  nnot allocate: d
 00002f40: 6174 6120 6973 2061 6c72 6561 6479 2073  ata is already s
 00002f50: 6574 7212 0000 0072 2600 0000 2907 726d  etr....r&...).rm
-00002f60: 0000 0072 9500 0000 726b 0000 0072 6a00  ...r....rk...rj.
+00002f60: 0000 0072 9600 0000 726b 0000 0072 6a00  ...r....rk...rj.
 00002f70: 0000 7230 0000 0072 3200 0000 7269 0000  ..r0...r2...ri..
 00002f80: 0029 0372 4f00 0000 da03 6c69 625a 025f  .).rO.....libZ._
 00002f90: 7a72 1e00 0000 721e 0000 0072 1f00 0000  zr....r....r....
 00002fa0: da08 616c 6c6f 6361 7465 7801 0000 7310  ..allocatex...s.
 00002fb0: 0000 0000 080a 0108 010a 0108 0112 0108  ................
 00002fc0: 0204 017a 1642 7566 6665 7257 7261 7070  ...z.BufferWrapp
 00002fd0: 6572 2e61 6c6c 6f63 6174 6563 0100 0000  er.allocatec....
 00002fe0: 0000 0000 0000 0000 0100 0000 0200 0000  ................
 00002ff0: 4300 0000 730a 0000 007c 006a 0064 0075  C...s....|.j.d.u
-00003000: 0153 0072 2100 0000 729a 0000 0072 4e00  .S.r!...r....rN.
+00003000: 0153 0072 2100 0000 729b 0000 0072 4e00  .S.r!...r....rN.
 00003010: 0000 721e 0000 0072 1e00 0000 721f 0000  ..r....r....r...
 00003020: 00da 0868 6173 5f64 6174 618a 0100 0073  ...has_data....s
 00003030: 0200 0000 0001 7a16 4275 6666 6572 5772  ......z.BufferWr
 00003040: 6170 7065 722e 6861 735f 6461 7461 6301  apper.has_datac.
 00003050: 0000 0000 0000 0000 0000 0001 0000 0001  ................
 00003060: 0000 0043 0000 0073 0600 0000 7c00 6a00  ...C...s....|.j.
 00003070: 5300 7221 0000 0029 0172 7100 0000 724e  S.r!...).rq...rN
@@ -780,15 +780,15 @@
 000030b0: 6572 5772 6170 7065 722e 726f 695f 6973  erWrapper.roi_is
 000030c0: 5f7a 6572 6f63 0100 0000 0000 0000 0000  _zeroc..........
 000030d0: 0000 0100 0000 0200 0000 4300 0000 7314  ..........C...s.
 000030e0: 0000 0074 007c 006a 0183 0164 016b 027c  ...t.|.j...d.k.|
 000030f0: 005f 0264 0053 0072 5a00 0000 2903 720a  ._.d.S.rZ...).r.
 00003100: 0000 0072 6d00 0000 7271 0000 0072 4e00  ...rm...rq...rN.
 00003110: 0000 721e 0000 0072 1e00 0000 721f 0000  ..r....r....r...
-00003120: 0072 8200 0000 9101 0000 7302 0000 0000  .r........s.....
+00003120: 0072 8300 0000 9101 0000 7302 0000 0000  .r........s.....
 00003130: 017a 2142 7566 6665 7257 7261 7070 6572  .z!BufferWrapper
 00003140: 2e5f 7570 6461 7465 5f72 6f69 5f69 735f  ._update_roi_is_
 00003150: 7a65 726f 6302 0000 0000 0000 0000 0000  zeroc...........
 00003160: 0002 0000 0003 0000 0043 0000 0073 1e00  .........C...s..
 00003170: 0000 7c00 6a00 6401 7500 7210 7c01 6a01  ..|.j.d.u.r.|.j.
 00003180: 5300 7c01 6a01 a002 7c00 6a00 a101 5300  S.|.j...|.j...S.
 00003190: 2902 7ae8 0a20 2020 2020 2020 2047 6574  ).z..        Get
@@ -802,41 +802,41 @@
 00003210: 7373 6564 2220 6966 2061 2052 4f49 2069  ssed" if a ROI i
 00003220: 7320 7365 742c 2077 6520 6361 6e27 7420  s set, we can't 
 00003230: 6469 7265 6374 6c79 2069 6e64 6578 2061  directly index a
 00003240: 6e64 206d 7573 740a 2020 2020 2020 2020  nd must.        
 00003250: 6361 6c63 756c 6174 6520 6120 6e65 7720  calculate a new 
 00003260: 736c 6963 6520 6672 6f6d 2074 6865 2052  slice from the R
 00003270: 4f49 2e0a 2020 2020 2020 2020 4e29 0372  OI..        N).r
-00003280: 7000 0000 727e 0000 00da 0e61 646a 7573  p...r~.....adjus
+00003280: 7000 0000 727f 0000 00da 0e61 646a 7573  p...r......adjus
 00003290: 745f 666f 725f 726f 69a9 0272 4f00 0000  t_for_roi..rO...
-000032a0: 7283 0000 0072 1e00 0000 721e 0000 0072  r....r....r....r
+000032a0: 7284 0000 0072 1e00 0000 721e 0000 0072  r....r....r....r
 000032b0: 1f00 0000 da14 5f73 6c69 6365 5f66 6f72  ......_slice_for
 000032c0: 5f70 6172 7469 7469 6f6e 9401 0000 7306  _partition....s.
 000032d0: 0000 0000 070a 0106 017a 2242 7566 6665  .........z"Buffe
 000032e0: 7257 7261 7070 6572 2e5f 736c 6963 655f  rWrapper._slice_
 000032f0: 666f 725f 7061 7274 6974 696f 6e63 0200  for_partitionc..
 00003300: 0000 0000 0000 0000 0000 0200 0000 0200  ................
 00003310: 0000 4300 0000 7314 0000 007c 006a 0072  ..C...s....|.j.r
 00003320: 0e74 0164 0183 0182 017c 006a 0253 0029  .t.d.....|.j.S.)
-00003330: 024e 728e 0000 0029 0372 7300 0000 7295  .Nr....).rs...r.
+00003330: 024e 728f 0000 0029 0372 7300 0000 7296  .Nr....).rs...r.
 00003340: 0000 0072 6b00 0000 a902 724f 0000 00da  ...rk.....rO....
 00003350: 0764 6174 6173 6574 721e 0000 0072 1e00  .datasetr....r..
 00003360: 0000 721f 0000 00da 1467 6574 5f76 6965  ..r......get_vie
 00003370: 775f 666f 725f 6461 7461 7365 749f 0100  w_for_dataset...
 00003380: 0073 0600 0000 0001 0601 0801 7a22 4275  .s..........z"Bu
 00003390: 6666 6572 5772 6170 7065 722e 6765 745f  fferWrapper.get_
 000033a0: 7669 6577 5f66 6f72 5f64 6174 6173 6574  view_for_dataset
-000033b0: 2901 727e 0000 0063 0200 0000 0000 0000  ).r~...c........
+000033b0: 2901 727f 0000 0063 0200 0000 0000 0000  ).r....c........
 000033c0: 0000 0000 0400 0000 0300 0000 4300 0000  ............C...
 000033d0: 7330 0000 007c 01a0 00a1 007d 027c 006a  s0...|.....}.|.j
 000033e0: 017c 0219 007d 037c 036a 0274 037c 016a  .|...}.|.j.t.|.j
 000033f0: 0283 017c 006a 0417 006b 0273 2c4a 0082  ...|.j...k.s,J..
-00003400: 017c 0353 0072 2100 0000 2905 727f 0000  .|.S.r!...).r...
+00003400: 017c 0353 0072 2100 0000 2905 7280 0000  .|.S.r!...).r...
 00003410: 0072 6b00 0000 723b 0000 0072 6600 0000  .rk...r;...rf...
-00003420: 7276 0000 0029 0472 4f00 0000 727e 0000  rv...).rO...r~..
+00003420: 7276 0000 0029 0472 4f00 0000 727f 0000  rv...).rO...r...
 00003430: 005a 0a72 6561 6c5f 736c 6963 65da 0672  .Z.real_slice..r
 00003440: 6573 756c 7472 1e00 0000 721e 0000 0072  esultr....r....r
 00003450: 1f00 0000 da0a 5f67 6574 5f73 6c69 6365  ......_get_slice
 00003460: a401 0000 7308 0000 0000 0108 010a 031a  ....s...........
 00003470: 017a 1842 7566 6665 7257 7261 7070 6572  .z.BufferWrapper
 00003480: 2e5f 6765 745f 736c 6963 6563 0200 0000  ._get_slicec....
 00003490: 0000 0000 0000 0000 0200 0000 0500 0000  ................
@@ -847,19 +847,19 @@
 000034e0: 037c 016a 066a 07a1 0153 007c 006a 0264  .|.j.j...S.|.j.d
 000034f0: 046b 0272 527c 006a 0853 0064 0553 0029  .k.rR|.j.S.d.S.)
 00003500: 067a 520a 2020 2020 2020 2020 6765 7420  .zR.        get 
 00003510: 6120 7669 6577 2066 6f72 2061 2073 696e  a view for a sin
 00003520: 676c 6520 7061 7274 6974 696f 6e20 696e  gle partition in
 00003530: 2061 2077 686f 6c65 2d72 6573 756c 742d   a whole-result-
 00003540: 7369 7a65 6420 6275 6666 6572 0a20 2020  sized buffer.   
-00003550: 2020 2020 2072 8e00 0000 720f 0000 0072       r....r....r
+00003550: 2020 2020 2072 8f00 0000 720f 0000 0072       r....r....r
 00003560: 1000 0000 7211 0000 004e 2909 7273 0000  ....r....N).rs..
-00003570: 0072 9500 0000 7268 0000 0072 a800 0000  .r....rh...r....
-00003580: 72a3 0000 0072 0f00 0000 727e 0000 0072  r....r....r~...r
-00003590: 1000 0000 726b 0000 0072 a200 0000 721e  ....rk...r....r.
+00003570: 0072 9600 0000 7268 0000 0072 a900 0000  .r....rh...r....
+00003580: 72a4 0000 0072 0f00 0000 727f 0000 0072  r....r....r....r
+00003590: 1000 0000 726b 0000 0072 a300 0000 721e  ....rk...r....r.
 000035a0: 0000 0072 1e00 0000 721f 0000 00da 1667  ...r....r......g
 000035b0: 6574 5f76 6965 775f 666f 725f 7061 7274  et_view_for_part
 000035c0: 6974 696f 6eac 0100 0073 1000 0000 0004  ition....s......
 000035d0: 0601 0801 0a01 1201 0a01 0e01 0a01 7a24  ..............z$
 000035e0: 4275 6666 6572 5772 6170 7065 722e 6765  BufferWrapper.ge
 000035f0: 745f 7669 6577 5f66 6f72 5f70 6172 7469  t_view_for_parti
 00003600: 7469 6f6e 6304 0000 0000 0000 0000 0000  tionc...........
@@ -888,24 +888,24 @@
 00003770: 6564 2072 6573 756c 7420 666f 7220 6120  ed result for a 
 00003780: 7768 6f6c 6520 7061 7274 6974 696f 6e2c  whole partition,
 00003790: 0a20 2020 2020 2020 206e 6f74 2074 6865  .        not the
 000037a0: 2070 6172 7469 7469 6f6e 2069 7473 656c   partition itsel
 000037b0: 6621 290a 2020 2020 2020 2020 720c 0000  f!).        r...
 000037c0: 007a 2570 6172 7469 7469 6f6e 2073 6861  .z%partition sha
 000037d0: 7065 2073 686f 756c 6420 6265 2066 6c61  pe should be fla
-000037e0: 742c 2069 7320 2573 728e 0000 0072 1000  t, is %sr....r..
+000037e0: 742c 2069 7320 2573 728f 0000 0072 1000  t, is %sr....r..
 000037f0: 0000 720f 0000 0072 0100 0000 7211 0000  ..r....r....r...
 00003800: 004e 2911 723b 0000 00da 0464 696d 7372  .N).r;.....dimsr
-00003810: 1000 0000 7295 0000 0072 7300 0000 7268  ....r....rs...rh
-00003820: 0000 0072 a800 0000 da0a 7469 6c65 5f73  ...r......tile_s
-00003830: 6c69 6365 72a3 0000 0072 6c00 0000 da06  licer....rl.....
-00003840: 6f72 6967 696e da03 696e 7472 8a00 0000  origin..intr....
+00003810: 1000 0000 7296 0000 0072 7300 0000 7268  ....r....rs...rh
+00003820: 0000 0072 a900 0000 da0a 7469 6c65 5f73  ...r......tile_s
+00003830: 6c69 6365 72a4 0000 0072 6c00 0000 da06  licer....rl.....
+00003840: 6f72 6967 696e da03 696e 7472 8b00 0000  origin..intr....
 00003850: 7267 0000 0072 6b00 0000 7227 0000 00da  rg...rk...r'....
 00003860: 076e 6577 6178 6973 2907 724f 0000 0072  .newaxis).rO...r
-00003870: 8300 0000 da04 7469 6c65 da09 6672 616d  ......tile..fram
+00003870: 8400 0000 da04 7469 6c65 da09 6672 616d  ......tile..fram
 00003880: 655f 6964 78da 0f70 6172 7469 7469 6f6e  e_idx..partition
 00003890: 5f73 6c69 6365 da06 6f66 6673 6574 5a0a  _slice..offsetZ.
 000038a0: 7265 7375 6c74 5f69 6478 721e 0000 0072  result_idxr....r
 000038b0: 1e00 0000 721f 0000 00da 1267 6574 5f76  ....r......get_v
 000038c0: 6965 775f 666f 725f 6672 616d 65b9 0100  iew_for_frame...
 000038d0: 0073 2200 0000 0006 1601 0e01 0601 0801  .s".............
 000038e0: 0a01 0e01 0a01 0a01 0601 0602 0a03 1a02  ................
@@ -933,26 +933,26 @@
 00003a40: 6665 720a 2020 2020 2020 2020 2870 6172  fer.        (par
 00003a50: 7469 7469 6f6e 2d73 697a 6564 2068 6572  tition-sized her
 00003a60: 6520 6d65 616e 7320 7468 6520 7265 6475  e means the redu
 00003a70: 6365 6420 7265 7375 6c74 2066 6f72 2061  ced result for a
 00003a80: 2077 686f 6c65 2070 6172 7469 7469 6f6e   whole partition
 00003a90: 2c0a 2020 2020 2020 2020 6e6f 7420 7468  ,.        not th
 00003aa0: 6520 7061 7274 6974 696f 6e20 6974 7365  e partition itse
-00003ab0: 6c66 2129 0a20 2020 2020 2020 2072 8e00  lf!).        r..
+00003ab0: 6c66 2129 0a20 2020 2020 2020 2072 8f00  lf!).        r..
 00003ac0: 0000 7a26 6361 6e6e 6f74 2067 6574 2076  ..z&cannot get v
 00003ad0: 6965 7720 666f 7220 7469 6c65 2077 6974  iew for tile wit
 00003ae0: 6820 7a65 726f 2052 4f49 7210 0000 0072  h zero ROIr....r
 00003af0: 0f00 0000 7201 0000 0072 1100 0000 4e29  ....r....r....N)
-00003b00: 0e72 7300 0000 7295 0000 0072 a000 0000  .rs...r....r....
-00003b10: 728b 0000 0072 6800 0000 72a8 0000 0072  r....rh...r....r
-00003b20: ab00 0000 7210 0000 0072 a300 0000 726c  ....r....r....rl
-00003b30: 0000 0072 ac00 0000 723b 0000 0072 8a00  ...r....r;...r..
-00003b40: 0000 726b 0000 0029 0872 4f00 0000 7283  ..rk...).rO...r.
-00003b50: 0000 0072 af00 0000 72b1 0000 0072 ab00  ...r....r....r..
-00003b60: 0000 72b2 0000 005a 0c72 6573 756c 745f  ..r....Z.result_
+00003b00: 0e72 7300 0000 7296 0000 0072 a100 0000  .rs...r....r....
+00003b10: 728c 0000 0072 6800 0000 72a9 0000 0072  r....rh...r....r
+00003b20: ac00 0000 7210 0000 0072 a400 0000 726c  ....r....r....rl
+00003b30: 0000 0072 ad00 0000 723b 0000 0072 8b00  ...r....r;...r..
+00003b40: 0000 726b 0000 0029 0872 4f00 0000 7284  ..rk...).rO...r.
+00003b50: 0000 0072 b000 0000 72b2 0000 0072 ac00  ...r....r....r..
+00003b60: 0000 72b3 0000 005a 0c72 6573 756c 745f  ..r....Z.result_
 00003b70: 7374 6172 745a 0b72 6573 756c 745f 7374  startZ.result_st
 00003b80: 6f70 721e 0000 0072 1e00 0000 721f 0000  opr....r....r...
 00003b90: 00da 1167 6574 5f76 6965 775f 666f 725f  ...get_view_for_
 00003ba0: 7469 6c65 d601 0000 7326 0000 0000 0606  tile....s&......
 00003bb0: 0108 0106 0108 010a 010e 010a 010a 0106  ................
 00003bc0: 0106 0106 020a 010e 010e 0312 0112 010e  ................
 00003bd0: 010a 017a 1f42 7566 6665 7257 7261 7070  ...z.BufferWrapp
@@ -1002,20 +1002,20 @@
 00003e90: 2020 2d2d 2d2d 2d2d 2d0a 0a20 2020 2020    -------..     
 00003ea0: 2020 2076 6965 7720 3a20 6e70 2e6e 6461     view : np.nda
 00003eb0: 7272 6179 0a20 2020 2020 2020 2020 2020  rray.           
 00003ec0: 2056 6965 7720 696e 746f 2064 6174 6120   View into data 
 00003ed0: 6f72 2063 6f6e 7469 6775 6f75 7320 636f  or contiguous co
 00003ee0: 7079 2069 6620 6e65 6365 7373 6172 790a  py if necessary.
 00003ef0: 0a20 2020 2020 2020 2072 1000 0000 4e29  .        r....N)
-00003f00: 0a72 6800 0000 72ab 0000 00da 0b64 6973  .rh...r......dis
-00003f10: 6361 7264 5f6e 6176 7273 0000 0072 a800  card_navrs...r..
+00003f00: 0a72 6800 0000 72ac 0000 00da 0b64 6973  .rh...r......dis
+00003f10: 6361 7264 5f6e 6176 7273 0000 0072 a900  card_navrs...r..
 00003f20: 0000 7210 0000 00da 0566 6c61 6773 da0c  ..r......flags..
 00003f30: 635f 636f 6e74 6967 756f 7573 da04 636f  c_contiguous..co
-00003f40: 7079 72b4 0000 0029 0572 4f00 0000 7283  pyr....).rO...r.
-00003f50: 0000 0072 af00 0000 da03 6b65 7972 3a00  ...r......keyr:.
+00003f40: 7079 72b5 0000 0029 0572 4f00 0000 7284  pyr....).rO...r.
+00003f50: 0000 0072 b000 0000 da03 6b65 7972 3a00  ...r......keyr:.
 00003f60: 0000 721e 0000 0072 1e00 0000 721f 0000  ..r....r....r...
 00003f70: 00da 1c67 6574 5f63 6f6e 7469 6775 6f75  ...get_contiguou
 00003f80: 735f 7669 6577 5f66 6f72 5f74 696c 65f3  s_view_for_tile.
 00003f90: 0100 0073 1400 0000 0016 0a01 0a01 0a01  ...s............
 00003fa0: 0c02 0c03 0801 0801 0a01 0402 7a2a 4275  ............z*Bu
 00003fb0: 6666 6572 5772 6170 7065 722e 6765 745f  fferWrapper.get_
 00003fc0: 636f 6e74 6967 756f 7573 5f76 6965 775f  contiguous_view_
@@ -1039,18 +1039,18 @@
 000040e0: 797a 2e60 6b65 7960 2025 7220 7368 6f75  yz.`key` %r shou
 000040f0: 6c64 2062 6520 6469 736a 6f69 6e74 2077  ld be disjoint w
 00004100: 6974 6820 6578 6973 7469 6e67 206b 6579  ith existing key
 00004110: 737a 2a43 6f6e 7469 6775 6f75 7320 6361  sz*Contiguous ca
 00004120: 6368 6520 6e6f 7420 696d 706c 656d 656e  che not implemen
 00004130: 7465 6420 666f 7220 6b69 6e64 20da 012e  ted for kind ...
 00004140: 4e29 0972 6800 0000 7273 0000 00da 0569  N).rh...rs.....i
-00004150: 7465 6d73 727f 0000 0072 6b00 0000 7248  temsr....rk...rH
-00004160: 0000 00da 046b 6579 7372 9500 0000 7272  .....keysr....rr
+00004150: 7465 6d73 7280 0000 0072 6b00 0000 7248  temsr....rk...rH
+00004160: 0000 00da 046b 6579 7372 9600 0000 7272  .....keysr....rr
 00004170: 0000 0029 0572 4f00 0000 da05 6465 6275  ...).rO.....debu
-00004180: 6772 b900 0000 723a 0000 0072 3e00 0000  gr....r:...r>...
+00004180: 6772 ba00 0000 723a 0000 0072 3e00 0000  gr....r:...r>...
 00004190: 721e 0000 0072 1e00 0000 721f 0000 00da  r....r....r.....
 000041a0: 0566 6c75 7368 1802 0000 731a 0000 0000  .flush....s.....
 000041b0: 060a 0112 010c 010a 0114 0102 0106 ff06  ................
 000041c0: 030a 0206 0102 010c ff7a 1342 7566 6665  .........z.Buffe
 000041d0: 7257 7261 7070 6572 2e66 6c75 7368 6301  rWrapper.flushc.
 000041e0: 0000 0000 0000 0000 0000 0001 0000 0002  ................
 000041f0: 0000 0043 0000 0073 1000 0000 7400 7c00  ...C...s....t.|.
@@ -1073,15 +1073,15 @@
 00004300: 7874 7261 5f73 6861 7065 3d7b 7d3e a904  xtra_shape={}>..
 00004310: da06 666f 726d 6174 7268 0000 0072 6900  ..formatrh...ri.
 00004320: 0000 7267 0000 0072 4e00 0000 721e 0000  ..rg...rN...r...
 00004330: 0072 1e00 0000 721f 0000 00da 085f 5f72  .r....r......__r
 00004340: 6570 725f 5f33 0200 0073 0600 0000 0001  epr__3...s......
 00004350: 0401 0cff 7a16 4275 6666 6572 5772 6170  ....z.BufferWrap
 00004360: 7065 722e 5f5f 7265 7072 5f5f 7a0c 6e74  per.__repr__z.nt
-00004370: 2e41 7272 6179 4c69 6b65 2902 7299 0000  .ArrayLike).r...
+00004370: 2e41 7272 6179 4c69 6b65 2902 729a 0000  .ArrayLike).r...
 00004380: 0072 1700 0000 6302 0000 0000 0000 0000  .r....c.........
 00004390: 0000 0004 0000 0006 0000 0043 0000 0073  ...........C...s
 000043a0: 7e00 0000 7c00 6a00 6401 7500 7218 7c00  ~...|.j.d.u.r.|.
 000043b0: 6a01 7d02 7c00 6a02 7d03 6e10 7c00 6a00  j.}.|.j.}.n.|.j.
 000043c0: 6a03 7d02 7c00 6a00 6a04 7d03 7c01 6a04  j.}.|.j.j.}.|.j.
 000043d0: 7c03 6b03 724a 7405 6402 7c03 9b00 6403  |.k.rJt.d.|...d.
 000043e0: 7c01 6a04 9b00 6404 9d05 8301 8201 7c01  |.j...d.......|.
@@ -1100,20 +1100,20 @@
 000044b0: 2061 6e79 2061 7272 6179 2d6c 696b 6520   any array-like 
 000044c0: 6f62 6a65 6374 0a0a 2020 2020 2020 2020  object..        
 000044d0: 5769 6c6c 2070 6572 666f 726d 2063 6865  Will perform che
 000044e0: 636b 696e 6720 666f 7220 7368 6170 6520  cking for shape 
 000044f0: 616e 6420 6474 7970 652e 0a20 2020 2020  and dtype..     
 00004500: 2020 204e 7a1a 6474 7970 6520 6d69 736d     Nz.dtype mism
 00004510: 6174 6368 3a20 6275 6666 6572 2069 7320  atch: buffer is 
-00004520: 7a0a 2c20 6461 7461 2069 7320 72bc 0000  z., data is r...
+00004520: 7a0a 2c20 6461 7461 2069 7320 72bd 0000  z., data is r...
 00004530: 007a 1a53 6861 7065 206d 6973 6d61 7463  .z.Shape mismatc
 00004540: 683a 2062 7566 6665 7220 6973 2029 0872  h: buffer is ).r
 00004550: 6b00 0000 726d 0000 0072 6900 0000 723b  k...rm...ri...r;
-00004560: 0000 0072 2400 0000 728b 0000 0072 7200  ...r$...r....rr.
-00004570: 0000 7273 0000 0029 0472 4f00 0000 7299  ..rs...).rO...r.
+00004560: 0000 0072 2400 0000 728c 0000 0072 7200  ...r$...r....rr.
+00004570: 0000 7273 0000 0029 0472 4f00 0000 729a  ..rs...).rO...r.
 00004580: 0000 0072 3b00 0000 7224 0000 0072 1e00  ...r;...r$...r..
 00004590: 0000 721e 0000 0072 1f00 0000 da0d 7265  ..r....r......re
 000045a0: 706c 6163 655f 6172 7261 7938 0200 0073  place_array8...s
 000045b0: 1600 0000 0009 0a01 0601 0802 0801 0801  ................
 000045c0: 0a01 1801 0a01 1801 0801 7a1b 4275 6666  ..........z.Buff
 000045d0: 6572 5772 6170 7065 722e 7265 706c 6163  erWrapper.replac
 000045e0: 655f 6172 7261 7963 0100 0000 0000 0000  e_arrayc........
@@ -1133,25 +1133,25 @@
 000046c0: 6c74 5f62 7566 6665 725f 7479 7065 4e02  lt_buffer_typeN.
 000046d0: 0000 7302 0000 0000 067a 2042 7566 6665  ..s......z Buffe
 000046e0: 7257 7261 7070 6572 2e72 6573 756c 745f  rWrapper.result_
 000046f0: 6275 6666 6572 5f74 7970 6529 0472 1e00  buffer_type).r..
 00004700: 0000 7264 0000 004e 4e29 014e 2901 4e29  ..rd...NN).N).N)
 00004710: 014e 2901 4e29 0146 2927 725c 0000 0072  .N).N).F)'r\...r
 00004720: 5d00 0000 725e 0000 0072 5f00 0000 7250  ]...r^...r_...rP
-00004730: 0000 0072 7a00 0000 727b 0000 0072 8600  ...rz...r{...r..
-00004740: 0000 7288 0000 00da 0870 726f 7065 7274  ..r......propert
-00004750: 7972 3b00 0000 7281 0000 0072 9900 0000  yr;...r....r....
+00004730: 0000 0072 7a00 0000 727c 0000 0072 8700  ...rz...r|...r..
+00004740: 0000 7289 0000 00da 0870 726f 7065 7274  ..r......propert
+00004750: 7972 3b00 0000 7282 0000 0072 9a00 0000  yr;...r....r....
 00004760: 7224 0000 0072 0400 0000 7227 0000 0072  r$...r....r'...r
-00004770: 3500 0000 729b 0000 0072 7500 0000 7276  5...r....ru...rv
-00004780: 0000 0072 7700 0000 729c 0000 0072 9e00  ...rw...r....r..
-00004790: 0000 729f 0000 0072 a000 0000 7282 0000  ..r....r....r...
-000047a0: 0072 a300 0000 72a6 0000 0072 0b00 0000  .r....r....r....
-000047b0: 72a8 0000 0072 a900 0000 72b3 0000 0072  r....r....r....r
-000047c0: b400 0000 72ba 0000 0072 c000 0000 72c1  ....r....r....r.
-000047d0: 0000 0072 c400 0000 72c5 0000 0072 c700  ...r....r....r..
+00004770: 3500 0000 729c 0000 0072 7500 0000 7276  5...r....ru...rv
+00004780: 0000 0072 7700 0000 729d 0000 0072 9f00  ...rw...r....r..
+00004790: 0000 72a0 0000 0072 a100 0000 7283 0000  ..r....r....r...
+000047a0: 0072 a400 0000 72a7 0000 0072 0b00 0000  .r....r....r....
+000047b0: 72a9 0000 0072 aa00 0000 72b4 0000 0072  r....r....r....r
+000047c0: b500 0000 72bb 0000 0072 c100 0000 72c2  ....r....r....r.
+000047d0: 0000 0072 c500 0000 72c6 0000 0072 c800  ...r....r....r..
 000047e0: 0000 721e 0000 0072 1e00 0000 721e 0000  ..r....r....r...
 000047f0: 0072 1f00 0000 7263 0000 00a8 0000 0073  .r....rc.......s
 00004800: 4e00 0000 0801 0433 1010 0805 0807 0a0b  N......3........
 00004810: 0a09 0201 0a04 0a11 0201 0a23 0201 0a08  ...........#....
 00004820: 0201 1607 0201 0a08 0201 0a08 0201 0a08  ................
 00004830: 0806 0a12 0803 0201 0a03 0803 080b 0805  ................
 00004840: 0e08 080d 081d 081d 0825 0a15 0806 0805  .........%......
@@ -1177,115 +1177,115 @@
 00004980: 2020 7468 6174 2061 7265 206f 6e6c 7920    that are only 
 00004990: 6d61 7465 7269 616c 697a 6564 2069 6e20  materialized in 
 000049a0: 3a63 6f64 653a 6055 4446 2e67 6574 5f72  :code:`UDF.get_r
 000049b0: 6573 756c 7473 602e 0a20 2020 204e 6302  esults`..    Nc.
 000049c0: 0000 0000 0000 0000 0000 0002 0000 0001  ................
 000049d0: 0000 0043 0000 0073 0400 0000 6400 5300  ...C...s....d.S.
 000049e0: 7221 0000 0072 1e00 0000 2902 724f 0000  r!...r....).rO..
-000049f0: 0072 9d00 0000 721e 0000 0072 1e00 0000  .r....r....r....
-00004a00: 721f 0000 0072 9e00 0000 5d02 0000 7302  r....r....]...s.
+000049f0: 0072 9e00 0000 721e 0000 0072 1e00 0000  .r....r....r....
+00004a00: 721f 0000 0072 9f00 0000 5d02 0000 7302  r....r....]...s.
 00004a10: 0000 0000 017a 2150 6c61 6365 686f 6c64  .....z!Placehold
 00004a20: 6572 4275 6666 6572 5772 6170 7065 722e  erBufferWrapper.
 00004a30: 616c 6c6f 6361 7465 6301 0000 0000 0000  allocatec.......
 00004a40: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
 00004a50: 0073 0400 0000 6401 5300 7265 0000 0072  .s....d.S.re...r
 00004a60: 1e00 0000 724e 0000 0072 1e00 0000 721e  ....rN...r....r.
-00004a70: 0000 0072 1f00 0000 729f 0000 0060 0200  ...r....r....`..
+00004a70: 0000 0072 1f00 0000 72a0 0000 0060 0200  ...r....r....`..
 00004a80: 0073 0200 0000 0001 7a21 506c 6163 6568  .s......z!Placeh
 00004a90: 6f6c 6465 7242 7566 6665 7257 7261 7070  olderBufferWrapp
 00004aa0: 6572 2e68 6173 5f64 6174 6163 0100 0000  er.has_datac....
 00004ab0: 0000 0000 0000 0000 0100 0000 0100 0000  ................
 00004ac0: 4300 0000 7304 0000 0064 0053 0072 2100  C...s....d.S.r!.
 00004ad0: 0000 721e 0000 0072 4e00 0000 721e 0000  ..r....rN...r...
-00004ae0: 0072 1e00 0000 721f 0000 0072 c100 0000  .r....r....r....
+00004ae0: 0072 1e00 0000 721f 0000 0072 c200 0000  .r....r....r....
 00004af0: 6302 0000 7302 0000 0000 017a 1f50 6c61  c...s......z.Pla
 00004b00: 6365 686f 6c64 6572 4275 6666 6572 5772  ceholderBufferWr
 00004b10: 6170 7065 722e 6578 706f 7274 6302 0000  apper.exportc...
 00004b20: 0000 0000 0000 0000 0002 0000 0001 0000  ................
 00004b30: 0043 0000 0073 0400 0000 6400 5300 7221  .C...s....d.S.r!
-00004b40: 0000 0072 1e00 0000 72a2 0000 0072 1e00  ...r....r....r..
-00004b50: 0000 721e 0000 0072 1f00 0000 72a9 0000  ..r....r....r...
+00004b40: 0000 0072 1e00 0000 72a3 0000 0072 1e00  ...r....r....r..
+00004b50: 0000 721e 0000 0072 1f00 0000 72aa 0000  ..r....r....r...
 00004b60: 0066 0200 0073 0200 0000 0001 7a2f 506c  .f...s......z/Pl
 00004b70: 6163 6568 6f6c 6465 7242 7566 6665 7257  aceholderBufferW
 00004b80: 7261 7070 6572 2e67 6574 5f76 6965 775f  rapper.get_view_
 00004b90: 666f 725f 7061 7274 6974 696f 6e63 0400  for_partitionc..
 00004ba0: 0000 0000 0000 0000 0000 0400 0000 0100  ................
 00004bb0: 0000 4300 0000 7304 0000 0064 0053 0072  ..C...s....d.S.r
 00004bc0: 2100 0000 721e 0000 0029 0472 4f00 0000  !...r....).rO...
-00004bd0: 7283 0000 0072 af00 0000 72b0 0000 0072  r....r....r....r
-00004be0: 1e00 0000 721e 0000 0072 1f00 0000 72b3  ....r....r....r.
+00004bd0: 7284 0000 0072 b000 0000 72b1 0000 0072  r....r....r....r
+00004be0: 1e00 0000 721e 0000 0072 1f00 0000 72b4  ....r....r....r.
 00004bf0: 0000 0069 0200 0073 0200 0000 0001 7a2b  ...i...s......z+
 00004c00: 506c 6163 6568 6f6c 6465 7242 7566 6665  PlaceholderBuffe
 00004c10: 7257 7261 7070 6572 2e67 6574 5f76 6965  rWrapper.get_vie
 00004c20: 775f 666f 725f 6672 616d 6563 0300 0000  w_for_framec....
 00004c30: 0000 0000 0000 0000 0300 0000 0100 0000  ................
 00004c40: 4300 0000 7304 0000 0064 0053 0072 2100  C...s....d.S.r!.
-00004c50: 0000 721e 0000 00a9 0372 4f00 0000 7283  ..r......rO...r.
-00004c60: 0000 0072 af00 0000 721e 0000 0072 1e00  ...r....r....r..
-00004c70: 0000 721f 0000 0072 b400 0000 6c02 0000  ..r....r....l...
+00004c50: 0000 721e 0000 00a9 0372 4f00 0000 7284  ..r......rO...r.
+00004c60: 0000 0072 b000 0000 721e 0000 0072 1e00  ...r....r....r..
+00004c70: 0000 721f 0000 0072 b500 0000 6c02 0000  ..r....r....l...
 00004c80: 7302 0000 0000 017a 2a50 6c61 6365 686f  s......z*Placeho
 00004c90: 6c64 6572 4275 6666 6572 5772 6170 7065  lderBufferWrappe
 00004ca0: 722e 6765 745f 7669 6577 5f66 6f72 5f74  r.get_view_for_t
 00004cb0: 696c 6563 0300 0000 0000 0000 0000 0000  ilec............
 00004cc0: 0300 0000 0100 0000 4300 0000 7304 0000  ........C...s...
 00004cd0: 0064 0053 0072 2100 0000 721e 0000 0072  .d.S.r!...r....r
-00004ce0: ca00 0000 721e 0000 0072 1e00 0000 721f  ....r....r....r.
-00004cf0: 0000 0072 ba00 0000 6f02 0000 7302 0000  ...r....o...s...
+00004ce0: cb00 0000 721e 0000 0072 1e00 0000 721f  ....r....r....r.
+00004cf0: 0000 0072 bb00 0000 6f02 0000 7302 0000  ...r....o...s...
 00004d00: 0000 017a 3550 6c61 6365 686f 6c64 6572  ...z5Placeholder
 00004d10: 4275 6666 6572 5772 6170 7065 722e 6765  BufferWrapper.ge
 00004d20: 745f 636f 6e74 6967 756f 7573 5f76 6965  t_contiguous_vie
 00004d30: 775f 666f 725f 7469 6c65 6301 0000 0000  w_for_tilec.....
 00004d40: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
 00004d50: 0000 0073 0c00 0000 7400 6401 8301 8201  ...s....t.d.....
 00004d60: 6400 5300 a902 4e7a 3a74 6869 7320 4275  d.S...Nz:this Bu
 00004d70: 6666 6572 5772 6170 7065 7220 646f 6573  fferWrapper does
 00004d80: 6e27 7420 6861 7665 2061 2076 616c 7565  n't have a value
 00004d90: 2061 7373 6f63 6961 7465 6420 7769 7468   associated with
-00004da0: 2069 74a9 0172 8b00 0000 724e 0000 0072   it..r....rN...r
-00004db0: 1e00 0000 721e 0000 0072 1f00 0000 7299  ....r....r....r.
+00004da0: 2069 74a9 0172 8c00 0000 724e 0000 0072   it..r....rN...r
+00004db0: 1e00 0000 721e 0000 0072 1f00 0000 729a  ....r....r....r.
 00004dc0: 0000 0072 0200 0073 0600 0000 0002 0201  ...r...s........
 00004dd0: 02ff 7a1d 506c 6163 6568 6f6c 6465 7242  ..z.PlaceholderB
 00004de0: 7566 6665 7257 7261 7070 6572 2e64 6174  ufferWrapper.dat
 00004df0: 6163 0100 0000 0000 0000 0000 0000 0100  ac..............
 00004e00: 0000 0200 0000 4300 0000 730c 0000 0074  ......C...s....t
-00004e10: 0064 0183 0182 0164 0053 0072 cb00 0000  .d.....d.S.r....
-00004e20: 72cc 0000 0072 4e00 0000 721e 0000 0072  r....rN...r....r
-00004e30: 1e00 0000 721f 0000 0072 9b00 0000 7802  ....r....r....x.
+00004e10: 0064 0183 0182 0164 0053 0072 cc00 0000  .d.....d.S.r....
+00004e20: 72cd 0000 0072 4e00 0000 721e 0000 0072  r....rN...r....r
+00004e30: 1e00 0000 721f 0000 0072 9c00 0000 7802  ....r....r....x.
 00004e40: 0000 7306 0000 0000 0202 0102 ff7a 2150  ..s..........z!P
 00004e50: 6c61 6365 686f 6c64 6572 4275 6666 6572  laceholderBuffer
 00004e60: 5772 6170 7065 722e 7261 775f 6461 7461  Wrapper.raw_data
 00004e70: 2901 4e29 0e72 5c00 0000 725d 0000 0072  ).N).r\...r]...r
-00004e80: 5e00 0000 725f 0000 0072 9e00 0000 729f  ^...r_...r....r.
-00004e90: 0000 0072 c100 0000 72a9 0000 0072 b300  ...r....r....r..
-00004ea0: 0000 72b4 0000 0072 ba00 0000 72c8 0000  ..r....r....r...
-00004eb0: 0072 9900 0000 729b 0000 0072 1e00 0000  .r....r....r....
+00004e80: 5e00 0000 725f 0000 0072 9f00 0000 72a0  ^...r_...r....r.
+00004e90: 0000 0072 c200 0000 72aa 0000 0072 b400  ...r....r....r..
+00004ea0: 0000 72b5 0000 0072 bb00 0000 72c9 0000  ..r....r....r...
+00004eb0: 0072 9a00 0000 729c 0000 0072 1e00 0000  .r....r....r....
 00004ec0: 721e 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
-00004ed0: c900 0000 5702 0000 7318 0000 0008 0104  ....W...s.......
+00004ed0: ca00 0000 5702 0000 7318 0000 0008 0104  ....W...s.......
 00004ee0: 050a 0308 0308 0308 0308 0308 0308 0302  ................
-00004ef0: 010a 0502 0172 c900 0000 6300 0000 0000  .....r....c.....
+00004ef0: 010a 0502 0172 ca00 0000 6300 0000 0000  .....r....c.....
 00004f00: 0000 0000 0000 0000 0000 0003 0000 0000  ................
 00004f10: 0000 0073 1c00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
 00004f20: 8700 6601 6401 6402 8408 5a03 8700 0400  ..f.d.d...Z.....
-00004f30: 5a04 5300 2903 72c6 0000 0063 0200 0000  Z.S.).r....c....
+00004f30: 5a04 5300 2903 72c7 0000 0063 0200 0000  Z.S.).r....c....
 00004f40: 0000 0000 0000 0000 0400 0000 0400 0000  ................
 00004f50: 0f00 0000 731c 0000 0074 0083 006a 017c  ....s....t...j.|
 00004f60: 0269 007c 03a4 018e 0101 007c 017c 005f  .i.|.......|.|._
 00004f70: 0264 0053 0072 2100 0000 2903 da05 7375  .d.S.r!...)...su
 00004f80: 7065 7272 5000 0000 726b 0000 0029 0472  perrP...rk...).r
-00004f90: 4f00 0000 7299 0000 00da 0461 7267 73da  O...r......args.
+00004f90: 4f00 0000 729a 0000 00da 0461 7267 73da  O...r......args.
 00004fa0: 066b 7761 7267 73a9 01da 095f 5f63 6c61  .kwargs....__cla
 00004fb0: 7373 5f5f 721e 0000 0072 1f00 0000 7250  ss__r....r....rP
 00004fc0: 0000 0080 0200 0073 0400 0000 0001 1201  .......s........
 00004fd0: 7a1e 5072 6561 6c6c 6f63 4275 6666 6572  z.PreallocBuffer
 00004fe0: 5772 6170 7065 722e 5f5f 696e 6974 5f5f  Wrapper.__init__
 00004ff0: 2905 725c 0000 0072 5d00 0000 725e 0000  ).r\...r]...r^..
 00005000: 0072 5000 0000 da0d 5f5f 636c 6173 7363  .rP.....__classc
 00005010: 656c 6c5f 5f72 1e00 0000 721e 0000 0072  ell__r....r....r
-00005020: d000 0000 721f 0000 0072 c600 0000 7f02  ....r....r......
-00005030: 0000 7302 0000 0008 0172 c600 0000 6300  ..s......r....c.
+00005020: d100 0000 721f 0000 0072 c700 0000 7f02  ....r....r......
+00005030: 0000 7302 0000 0008 0172 c700 0000 6300  ..s......r....c.
 00005040: 0000 0000 0000 0000 0000 0000 0000 0003  ................
 00005050: 0000 0040 0000 0073 2e00 0000 6500 5a01  ...@...s....e.Z.
 00005060: 6400 5a02 6401 6402 8400 5a03 6403 6404  d.Z.d.d...Z.d.d.
 00005070: 8400 5a04 640b 6406 6407 8401 5a05 6408  ..Z.d.d.d...Z.d.
 00005080: 6409 8400 5a06 640a 5300 290c da10 4175  d...Z.d.S.)...Au
 00005090: 7842 7566 6665 7257 7261 7070 6572 6303  xBufferWrapperc.
 000050a0: 0000 0000 0000 0000 0000 0007 0000 0005  ................
@@ -1316,35 +1316,35 @@
 00005230: 0a20 2020 2020 2020 2062 7920 7468 6973  .        by this
 00005240: 206d 6574 686f 642c 2074 6861 7420 6973   method, that is
 00005250: 2c20 6974 2073 686f 756c 6420 6861 7665  , it should have
 00005260: 2067 6c6f 6261 6c20 636f 6f72 6469 6e61   global coordina
 00005270: 7465 7320 7769 7468 6f75 740a 2020 2020  tes without.    
 00005280: 2020 2020 6861 7669 6e67 2074 6865 2052      having the R
 00005290: 4f49 2061 7070 6c69 6564 2e0a 2020 2020  OI applied..    
-000052a0: 2020 2020 5472 7c00 0000 4e72 1800 0000      Tr|...Nr....
+000052a0: 2020 2020 5472 7d00 0000 4e72 1800 0000      Tr}...Nr....
 000052b0: 4629 01da 0969 735f 676c 6f62 616c 7201  F)...is_globalr.
-000052c0: 0000 0029 0d72 6c00 0000 727e 0000 0072  ...).rl...r~...r
-000052d0: 7f00 0000 72d1 0000 0072 6800 0000 7267  ....r....rh...rg
+000052c0: 0000 0029 0d72 6c00 0000 727f 0000 0072  ...).rl...r....r
+000052d0: 8000 0000 72d2 0000 0072 6800 0000 7267  ....r....rh...rg
 000052e0: 0000 0072 6900 0000 722a 0000 0072 6b00  ...ri...r*...rk.
 000052f0: 0000 da0a 7365 745f 6275 6666 6572 727a  ....set_bufferrz
 00005300: 0000 0072 0a00 0000 723b 0000 0029 0772  ...r....r;...).r
-00005310: 4f00 0000 7283 0000 0072 7900 0000 da02  O...r....ry.....
-00005320: 7073 721d 0000 0072 8500 0000 da08 6e65  psr....r......ne
+00005310: 4f00 0000 7284 0000 0072 7900 0000 da02  O...r....ry.....
+00005320: 7073 721d 0000 0072 8600 0000 da08 6e65  psr....r......ne
 00005330: 775f 6461 7461 721e 0000 0072 1e00 0000  w_datar....r....
 00005340: 721f 0000 00da 116e 6577 5f66 6f72 5f70  r......new_for_p
 00005350: 6172 7469 7469 6f6e 8602 0000 7318 0000  artition....s...
 00005360: 0000 0f0a 010e 0114 0108 010e 0110 020a  ................
 00005370: 010e 010a 0112 010a 017a 2241 7578 4275  .........z"AuxBu
 00005380: 6666 6572 5772 6170 7065 722e 6e65 775f  fferWrapper.new_
 00005390: 666f 725f 7061 7274 6974 696f 6e63 0200  for_partitionc..
 000053a0: 0000 0000 0000 0000 0000 0200 0000 0200  ................
 000053b0: 0000 4300 0000 730c 0000 007c 006a 007c  ..C...s....|.j.|
 000053c0: 006a 0119 0053 0072 2100 0000 2902 726b  .j...S.r!...).rk
-000053d0: 0000 0072 7000 0000 72a4 0000 0072 1e00  ...rp...r....r..
-000053e0: 0000 721e 0000 0072 1f00 0000 72a6 0000  ..r....r....r...
+000053d0: 0000 0072 7000 0000 72a5 0000 0072 1e00  ...rp...r....r..
+000053e0: 0000 721e 0000 0072 1f00 0000 72a7 0000  ..r....r....r...
 000053f0: 00a3 0200 0073 0200 0000 0001 7a25 4175  .....s......z%Au
 00005400: 7842 7566 6665 7257 7261 7070 6572 2e67  xBufferWrapper.g
 00005410: 6574 5f76 6965 775f 666f 725f 6461 7461  et_view_for_data
 00005420: 7365 7454 6303 0000 0000 0000 0000 0000  setTc...........
 00005430: 0005 0000 0003 0000 0043 0000 0073 5200  .........C...sR.
 00005440: 0000 7c00 6a00 6401 7500 730e 4a00 8201  ..|.j.d.u.s.J...
 00005450: 7c01 6a01 7c00 6a02 6b02 731e 4a00 8201  |.j.|.j.k.s.J...
@@ -1365,59 +1365,59 @@
 00005540: 742c 2070 6c75 7320 6578 7472 615f 7368  t, plus extra_sh
 00005550: 6170 652c 2061 7320 6465 7465 726d 696e  ape, as determin
 00005560: 6564 2062 7920 7468 6520 606b 696e 6460  ed by the `kind`
 00005570: 2061 6e64 0a20 2020 2020 2020 2060 6578   and.        `ex
 00005580: 7472 615f 7368 6170 6560 2063 6f6e 7374  tra_shape` const
 00005590: 7275 6374 6f72 2061 7267 756d 656e 7473  ructor arguments
 000055a0: 2e0a 2020 2020 2020 2020 4e72 7800 0000  ..        Nrx...
-000055b0: 7289 0000 0029 0672 6b00 0000 7224 0000  r....).rk...r$..
+000055b0: 728a 0000 0029 0672 6b00 0000 7224 0000  r....).rk...r$..
 000055c0: 0072 6900 0000 7267 0000 0072 2a00 0000  .ri...rg...r*...
 000055d0: 726c 0000 0029 0572 4f00 0000 721d 0000  rl...).rO...r...
-000055e0: 0072 d400 0000 da05 6578 7472 6172 3b00  .r......extrar;.
+000055e0: 0072 d500 0000 da05 6578 7472 6172 3b00  .r......extrar;.
 000055f0: 0000 721e 0000 0072 1e00 0000 721f 0000  ..r....r....r...
-00005600: 0072 d500 0000 a602 0000 7310 0000 0000  .r........s.....
+00005600: 0072 d600 0000 a602 0000 7310 0000 0000  .r........s.....
 00005610: 080e 0110 0106 0104 010c 0108 010c 017a  ...............z
 00005620: 1b41 7578 4275 6666 6572 5772 6170 7065  .AuxBufferWrappe
 00005630: 722e 7365 745f 6275 6666 6572 6301 0000  r.set_bufferc...
 00005640: 0000 0000 0000 0000 0001 0000 0005 0000  ................
 00005650: 0043 0000 0073 1400 0000 6401 a000 7c00  .C...s....d...|.
 00005660: 6a01 7c00 6a02 7c00 6a03 a103 5300 2902  j.|.j.|.j...S.).
 00005670: 4e7a 323c 4175 7842 7566 6665 7257 7261  Nz2<AuxBufferWra
 00005680: 7070 6572 206b 696e 643d 7b7d 2064 7479  pper kind={} dty
 00005690: 7065 3d7b 7d20 6578 7472 615f 7368 6170  pe={} extra_shap
-000056a0: 653d 7b7d 3e72 c200 0000 724e 0000 0072  e={}>r....rN...r
-000056b0: 1e00 0000 721e 0000 0072 1f00 0000 72c4  ....r....r....r.
+000056a0: 653d 7b7d 3e72 c300 0000 724e 0000 0072  e={}>r....rN...r
+000056b0: 1e00 0000 721e 0000 0072 1f00 0000 72c5  ....r....r....r.
 000056c0: 0000 00b7 0200 0073 0600 0000 0001 0401  .......s........
 000056d0: 0cff 7a19 4175 7842 7566 6665 7257 7261  ..z.AuxBufferWra
 000056e0: 7070 6572 2e5f 5f72 6570 725f 5f4e 2901  pper.__repr__N).
 000056f0: 5429 0772 5c00 0000 725d 0000 0072 5e00  T).r\...r]...r^.
-00005700: 0000 72d8 0000 0072 a600 0000 72d5 0000  ..r....r....r...
-00005710: 0072 c400 0000 721e 0000 0072 1e00 0000  .r....r....r....
-00005720: 721e 0000 0072 1f00 0000 72d3 0000 0085  r....r....r.....
+00005700: 0000 72d9 0000 0072 a700 0000 72d6 0000  ..r....r....r...
+00005710: 0072 c500 0000 721e 0000 0072 1e00 0000  .r....r....r....
+00005720: 721e 0000 0072 1f00 0000 72d4 0000 0085  r....r....r.....
 00005730: 0200 0073 0800 0000 0801 081d 0803 0a11  ...s............
-00005740: 72d3 0000 0029 0172 1400 0000 292b 720e  r....).r....)+r.
+00005740: 72d4 0000 0029 0172 1400 0000 292b 720e  r....).r....)+r.
 00005750: 0000 0072 0200 0000 7203 0000 0072 0400  ...r....r....r..
 00005760: 0000 7205 0000 0072 0600 0000 7207 0000  ..r....r....r...
 00005770: 00da 1174 7970 696e 675f 6578 7465 6e73  ...typing_extens
 00005780: 696f 6e73 7208 0000 0072 1b00 0000 7219  ionsr....r....r.
 00005790: 0000 00da 0a63 6f6e 7465 7874 6c69 6272  .....contextlibr
 000057a0: 0900 0000 724b 0000 00da 056e 756d 7079  ....rK.....numpy
 000057b0: 7227 0000 00da 146c 6962 6572 7465 6d2e  r'.....libertem.
 000057c0: 636f 6d6d 6f6e 2e6d 6174 6872 0a00 0000  common.mathr....
 000057d0: 5a15 6c69 6265 7274 656d 2e63 6f6d 6d6f  Z.libertem.commo
 000057e0: 6e2e 736c 6963 6572 0b00 0000 da07 6261  n.slicer......ba
 000057f0: 636b 656e 6472 0d00 0000 da02 6e74 5a0a  ckendr......ntZ.
 00005800: 4275 6666 6572 4b69 6e64 5a0e 4275 6666  BufferKindZ.Buff
 00005810: 6572 4c6f 6361 7469 6f6e 5a09 4275 6666  erLocationZ.Buff
-00005820: 6572 5573 6572 ad00 0000 5a0a 4275 6666  erUser....Z.Buff
+00005820: 6572 5573 6572 ae00 0000 5a0a 4275 6666  erUser....Z.Buff
 00005830: 6572 5369 7a65 7220 0000 0072 2200 0000  erSizer ...r"...
 00005840: 7223 0000 0072 3500 0000 722d 0000 0072  r#...r5...r-...r
 00005850: 3200 0000 7239 0000 0072 3c00 0000 7248  2...r9...r<...rH
 00005860: 0000 0072 4900 0000 7260 0000 0072 6300  ...rI...r`...rc.
-00005870: 0000 72c9 0000 0072 c600 0000 72d3 0000  ..r....r....r...
+00005870: 0000 72ca 0000 0072 c700 0000 72d4 0000  ..r....r....r...
 00005880: 0072 1e00 0000 721e 0000 0072 1e00 0000  .r....r....r....
 00005890: 721f 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
 000058a0: 0000 0073 3e00 0000 2001 0c01 0801 0801  ...s>... .......
 000058b0: 0c01 0802 0802 0c01 0c01 0c02 0401 0c02  ................
 000058c0: 0801 0c01 0801 1403 1610 1006 1409 140a  ................
 000058d0: 1c0e 101c 1404 0e2c 0e0e 0e7f 007f 007f  .......,........
 000058e0: 0032 1028 1006                           .2.(..
```

### Comparing `libertem-0.9.0/src/libertem/common/__pycache__/container.cpython-39.pyc` & `libertem-0.9.2/src/libertem/common/__pycache__/container.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 8911 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 cf22 0000  a.......z..b."..
+00000000: 610d 0d0a 0000 0000 7fce 6762 cf22 0000  a.........gb."..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 8800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a04 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c05 5a06 6400 6401 6c07 5a07 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6402 6c08 6d09 5a09 0100 6400 6403 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 0100 6400  m.Z.m.Z.m.Z...d.
```

### Comparing `libertem-0.9.0/src/libertem/common/__pycache__/math.cpython-39.pyc` & `libertem-0.9.2/src/libertem/common/__pycache__/math.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 766 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 fe02 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 fe02 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 5a00 0000 6400  .....@...sZ...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 6505 6506 6504 6a07 6504  d.l.Z.e.e.e.j.e.
 00000050: 6a08 6504 6a09 6605 5a0a 6502 6505 6506  j.e.j.f.Z.e.e.e.
 00000060: 6504 6a07 6504 6a08 6504 6a09 6605 1900  e.j.e.j.e.j.f...
 00000070: 5a0b 6501 650b 1900 6403 9c01 6404 6405  Z.e.e...d...d.d.
```

### Comparing `libertem-0.9.0/src/libertem/common/__pycache__/shape.cpython-39.pyc` & `libertem-0.9.2/src/libertem/common/__pycache__/shape.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 5434 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 3a15 0000  a.......z..b:...
+00000000: 610d 0d0a 0000 0000 7fce 6762 3a15 0000  a.........gb:...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5600 0000 6400  .....@...sV...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 6d05 5a05  d.l.m.Z.m.Z.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 0100 4700 6403 6404 8400 6404 8302 5a0a  ..G.d.d...d...Z.
 00000070: 6508 650a 6506 650b 1900 6602 1900 5a0c  e.e.e.e...f...Z.
```

### Comparing `libertem-0.9.0/src/libertem/common/__pycache__/slice.cpython-39.pyc` & `libertem-0.9.2/src/libertem/common/__pycache__/slice.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 12476 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 bc30 0000  a.......z..b.0..
+00000000: 610d 0d0a 0000 0000 7fce 6762 bc30 0000  a.........gb.0..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 0100 6400 6401 6c09  m.Z.m.Z...d.d.l.
 00000060: 5a0a 6400 6403 6c0b 6d0c 5a0c 0100 6400  Z.d.d.l.m.Z...d.
 00000070: 6404 6c0d 6d0e 5a0e 6d0f 5a0f 0100 4700  d.l.m.Z.m.Z...G.
```

### Comparing `libertem-0.9.0/src/libertem/common/backend.py` & `libertem-0.9.2/src/libertem/common/backend.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/common/buffers.py` & `libertem-0.9.2/src/libertem/common/buffers.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/common/container.py` & `libertem-0.9.2/src/libertem/common/container.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/common/math.py` & `libertem-0.9.2/src/libertem/common/math.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/common/numba/__init__.py` & `libertem-0.9.2/src/libertem/common/numba/__init__.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/common/numba/__pycache__/__init__.cpython-39.pyc` & `libertem-0.9.2/src/libertem/common/numba/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 5523 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 9315 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 9315 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 ce00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a03 6400 6401 6c04 5a05 6402  d.l.Z.d.d.l.Z.d.
 00000050: 6403 6c06 6d07 5a07 6d08 5a08 0100 6500  d.l.m.Z.m.Z...e.
 00000060: a009 650a a101 5a0b 6501 6a0c 6404 6404  ..e...Z.e.j.d.d.
 00000070: 6405 8d02 6406 6407 8400 8301 5a0d 6501  d...d.d.....Z.e.
@@ -183,28 +183,28 @@
 00000b60: 6174 7269 7820 6f72 2073 6369 7079 2e73  atrix or scipy.s
 00000b70: 7061 7273 652e 6373 725f 6d61 7472 6978  parse.csr_matrix
 00000b80: 2c20 676f 7420 2913 7209 0000 0072 1f00  , got ).r....r..
 00000b90: 0000 da0a 5661 6c75 6545 7272 6f72 7216  ....ValueErrorr.
 00000ba0: 0000 0072 1700 0000 da0b 7265 7375 6c74  ...r......result
 00000bb0: 5f74 7970 65da 0a69 7369 6e73 7461 6e63  _type..isinstanc
 00000bc0: 65da 0573 6369 7079 da06 7370 6172 7365  e..scipy..sparse
-00000bd0: 5a0a 6373 635f 6d61 7472 6978 da0c 5f72  Z.csc_matrix.._r
+00000bd0: da0a 6373 635f 6d61 7472 6978 da0c 5f72  ..csc_matrix.._r
 00000be0: 6d61 746d 756c 5f63 7363 da04 6461 7461  matmul_csc..data
-00000bf0: 7224 0000 005a 0669 6e64 7074 725a 0a63  r$...Z.indptrZ.c
+00000bf0: 7224 0000 00da 0669 6e64 7074 72da 0a63  r$.....indptr..c
 00000c00: 7372 5f6d 6174 7269 78da 0c5f 726d 6174  sr_matrix.._rmat
 00000c10: 6d75 6c5f 6373 72da 0474 7970 65da 0154  mul_csr..type..T
 00000c20: da04 636f 7079 2903 7228 0000 005a 0c72  ..copy).r(...Z.r
 00000c30: 6967 6874 5f73 7061 7273 65da 0872 6573  ight_sparse..res
 00000c40: 756c 745f 7472 1100 0000 7211 0000 0072  ult_tr....r....r
 00000c50: 1200 0000 da07 726d 6174 6d75 6c43 0000  ......rmatmulC..
 00000c60: 0073 4800 0000 0019 0e01 1201 0e01 1201  .sH.............
 00000c70: 1401 0201 0201 12ff 06ff 0404 0401 1201  ................
 00000c80: 0afe 0605 0e01 0201 0201 0401 0401 0401  ................
 00000c90: 02fb 0807 0e01 0201 0201 0401 0401 0401  ................
-00000ca0: 02fb 0808 0201 0201 06ff 06ff 0404 7239  ..............r9
+00000ca0: 02fb 0808 0201 0201 06ff 06ff 0404 723c  ..............r<
 00000cb0: 0000 0029 03da 0866 6173 746d 6174 68da  ...)...fastmath.
 00000cc0: 0563 6163 6865 7206 0000 0063 0500 0000  .cacher....c....
 00000cd0: 0000 0000 0000 0000 0f00 0000 0700 0000  ................
 00000ce0: 4300 0000 739c 0000 007c 006a 0064 0119  C...s....|.j.d..
 00000cf0: 007d 0574 0174 027c 0383 0164 0218 0083  .}.t.t.|...d....
 00000d00: 0144 005d 7c7d 067c 037c 0619 007d 077c  .D.]|}.|.|...}.|
 00000d10: 037c 0664 0217 0019 007c 0718 007d 087c  .|.d.....|...}.|
@@ -220,17 +220,17 @@
 00000db0: 2a00 0000 722b 0000 0072 2c00 0000 da09  *...r+...r,.....
 00000dc0: 6c65 6674 5f72 6f77 73da 0c72 6967 6874  left_rows..right
 00000dd0: 5f63 6f6c 756d 6eda 066f 6666 7365 74da  _column..offset.
 00000de0: 0569 7465 6d73 7219 0000 0072 1e00 0000  .itemsr....r....
 00000df0: da09 7269 6768 745f 726f 77da 0b72 6967  ..right_row..rig
 00000e00: 6874 5f76 616c 7565 da08 6c65 6674 5f72  ht_value..left_r
 00000e10: 6f77 da03 746d 7072 1100 0000 7211 0000  ow..tmpr....r...
-00000e20: 0072 1200 0000 7232 0000 0082 0000 0073  .r....r2.......s
+00000e20: 0072 1200 0000 7233 0000 0082 0000 0073  .r....r3.......s
 00000e30: 1800 0000 0002 0a01 1401 0801 1001 0801  ................
-00000e40: 0c01 0801 0801 0801 0c01 1001 7232 0000  ............r2..
+00000e40: 0c01 0801 0801 0801 0c01 1001 7233 0000  ............r3..
 00000e50: 0063 0500 0000 0000 0000 0000 0000 1000  .c..............
 00000e60: 0000 0700 0000 4300 0000 73c2 0000 007c  ......C...s....|
 00000e70: 006a 0064 0119 007d 0574 016a 027c 0566  .j.d...}.t.j.|.f
 00000e80: 017c 006a 0364 028d 027d 0674 0474 057c  .|.j.d...}.t.t.|
 00000e90: 0383 0164 0318 0083 0144 005d 907d 077c  ...d.....D.].}.|
 00000ea0: 037c 0719 007d 087c 037c 0764 0317 0019  .|...}.|.|.d....
 00000eb0: 007c 0818 007d 097c 0964 016b 0472 2c7c  .|...}.|.d.k.r,|
@@ -242,28 +242,28 @@
 00000f10: 007d 0f7c 047c 0c7c 0e66 0205 0019 007c  .}.|.|.|.f.....|
 00000f20: 0f37 0003 003c 0071 9471 7071 2c64 0053  .7...<.q.qpq,d.S
 00000f30: 0029 044e 7201 0000 0072 2700 0000 7202  .).Nr....r'...r.
 00000f40: 0000 0029 0672 1f00 0000 7216 0000 00da  ...).r....r.....
 00000f50: 0565 6d70 7479 7215 0000 0072 0800 0000  .emptyr....r....
 00000f60: 7209 0000 0029 1072 2800 0000 7229 0000  r....).r(...r)..
 00000f70: 0072 2a00 0000 722b 0000 0072 2c00 0000  .r*...r+...r,...
-00000f80: 723c 0000 005a 0672 6f77 6275 6672 4000  r<...Z.rowbufr@.
-00000f90: 0000 723e 0000 0072 3f00 0000 7219 0000  ..r>...r?...r...
-00000fa0: 0072 1e00 0000 723d 0000 0072 4100 0000  .r....r=...rA...
-00000fb0: 7242 0000 0072 4300 0000 7211 0000 0072  rB...rC...r....r
-00000fc0: 1100 0000 7212 0000 0072 3400 0000 9200  ....r....r4.....
+00000f80: 723f 0000 005a 0672 6f77 6275 6672 4300  r?...Z.rowbufrC.
+00000f90: 0000 7241 0000 0072 4200 0000 7219 0000  ..rA...rB...r...
+00000fa0: 0072 1e00 0000 7240 0000 0072 4400 0000  .r....r@...rD...
+00000fb0: 7245 0000 0072 4600 0000 7211 0000 0072  rE...rF...r....r
+00000fc0: 1100 0000 7212 0000 0072 3700 0000 9200  ....r....r7.....
 00000fd0: 0000 731c 0000 0000 020a 0112 0114 0108  ..s.............
 00000fe0: 0110 0108 0118 010c 0108 0108 0108 010c  ................
-00000ff0: 010c 0172 3400 0000 2914 da07 6c6f 6767  ...r4...)...logg
-00001000: 696e 67da 056e 756d 6261 5a0c 7363 6970  ing..numbaZ.scip
+00000ff0: 010c 0172 3700 0000 2914 da07 6c6f 6767  ...r7...)...logg
+00001000: 696e 67da 056e 756d 6261 da0c 7363 6970  ing..numba..scip
 00001010: 792e 7370 6172 7365 7230 0000 00da 056e  y.sparser0.....n
-00001020: 756d 7079 7216 0000 0072 3b00 0000 7203  umpyr....r;...r.
+00001020: 756d 7079 7216 0000 0072 3e00 0000 7203  umpyr....r>...r.
 00001030: 0000 0072 0400 0000 da09 6765 744c 6f67  ...r......getLog
 00001040: 6765 72da 085f 5f6e 616d 655f 5fda 066c  ger..__name__..l
 00001050: 6f67 6765 72da 046e 6a69 7472 1300 0000  ogger..njitr....
 00001060: 721a 0000 0072 2300 0000 7225 0000 0072  r....r#...r%...r
-00001070: 3900 0000 7232 0000 0072 3400 0000 7211  9...r2...r4...r.
+00001070: 3c00 0000 7233 0000 0072 3700 0000 7211  <...r3...r7...r.
 00001080: 0000 0072 1100 0000 7211 0000 0072 1200  ...r....r....r..
 00001090: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
 000010a0: 7324 0000 0008 0208 0108 0108 0210 020a  s$..............
 000010b0: 030c 010a 0c0c 010a 0d0c 010a 0d0c 010a  ................
 000010c0: 0d08 3f0e 010a 0f0e 01                   ..?......
```

### Comparing `libertem-0.9.0/src/libertem/common/numba/__pycache__/cache.cpython-39.pyc` & `libertem-0.9.2/src/libertem/common/numba/__pycache__/cache.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 5905 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 1117 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 1117 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000d 0000 0040 0000 0073 9401 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6502 a003 6504 a101 5a05  d.l.Z.e...e...Z.
 00000050: 6400 6401 6c06 5a06 7a30 6400 6402 6c07  d.d.l.Z.z0d.d.l.
 00000060: 6d08 5a08 0100 6400 6403 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6404 6c0b 6d0c 5a0c 6d0d 5a0d  ..d.d.l.m.Z.m.Z.
```

### Comparing `libertem-0.9.0/src/libertem/common/numba/cache.py` & `libertem-0.9.2/src/libertem/common/numba/cache.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/common/shape.py` & `libertem-0.9.2/src/libertem/common/shape.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/common/slice.py` & `libertem-0.9.2/src/libertem/common/slice.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/contrib/__pycache__/daskadapter.cpython-38.pyc` & `libertem-0.9.2/src/libertem/contrib/__pycache__/daskadapter.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 698 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 7ae9 0c62 ba02 0000  U.......z..b....
+00000000: 550d 0d0a 0000 0000 7fce 6762 ba02 0000  U.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 1e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a00 6405  d.l.Z.d.d.l.Z.d.
 00000040: 6403 6404 8401 5a02 6401 5300 2906 e900  d.d...Z.d.S.)...
 00000050: 0000 004e da07 666c 6f61 7433 3263 0300  ...N..float32c..
 00000060: 0000 0000 0000 0000 0000 0800 0000 0900  ................
 00000070: 0000 4300 0000 7384 0000 0067 007d 0369  ..C...s....g.}.i
```

### Comparing `libertem-0.9.0/src/libertem/contrib/__pycache__/daskadapter.cpython-39.pyc` & `libertem-0.9.2/src/libertem/contrib/__pycache__/daskadapter.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 698 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 ba02 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 ba02 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 1e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a00 6405  d.l.Z.d.d.l.Z.d.
 00000040: 6403 6404 8401 5a02 6401 5300 2906 e900  d.d...Z.d.S.)...
 00000050: 0000 004e da07 666c 6f61 7433 3263 0300  ...N..float32c..
 00000060: 0000 0000 0000 0000 0000 0800 0000 0900  ................
 00000070: 0000 4300 0000 7384 0000 0067 007d 0369  ..C...s....g.}.i
```

### Comparing `libertem-0.9.0/src/libertem/contrib/daskadapter.py` & `libertem-0.9.2/src/libertem/contrib/daskadapter.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/corrections/__pycache__/coordinates.cpython-39.pyc` & `libertem-0.9.2/src/libertem/corrections/__pycache__/coordinates.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 810 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 2a03 0000  a.......z..b*...
+00000000: 610d 0d0a 0000 0000 7fce 6762 2a03 0000  a.........gb*...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
 00000030: 6401 6c00 5a01 6402 6403 8400 5a02 6404  d.l.Z.d.d...Z.d.
 00000040: 6405 8400 5a03 6406 6407 8400 5a04 6408  d...Z.d.d...Z.d.
 00000050: 6409 8400 5a05 640a 640b 8400 5a06 640c  d...Z.d.d...Z.d.
 00000060: 640d 8400 5a07 6401 5300 290e e900 0000  d...Z.d.S.).....
 00000070: 004e 6301 0000 0000 0000 0000 0000 0001  .Nc.............
```

### Comparing `libertem-0.9.0/src/libertem/corrections/__pycache__/corrset.cpython-39.pyc` & `libertem-0.9.2/src/libertem/corrections/__pycache__/corrset.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 10366 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 7e28 0000  a.......z..b~(..
+00000000: 610d 0d0a 0000 0000 7fce 6762 7e28 0000  a.........gb~(..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 8200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a04 6400 6401 6c05  ..d.d.l.Z.d.d.l.
 00000050: 5a05 6400 6401 6c06 5a07 6400 6403 6c08  Z.d.d.l.Z.d.d.l.
 00000060: 6d09 5a09 0100 6400 6404 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 6d0c 5a0c 0100 6405 6406 8400 5a0d 6407  m.Z...d.d...Z.d.
```

### Comparing `libertem-0.9.0/src/libertem/corrections/__pycache__/detector.cpython-39.pyc` & `libertem-0.9.2/src/libertem/corrections/__pycache__/detector.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 11538 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 122d 0000  a.......z..b.-..
+00000000: 610d 0d0a 0000 0000 7fce 6762 122d 0000  a.........gb.-..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 b800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a03 6400 6402 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c08 6d09 5a09 6d0a 5a0a 0100 6502  d.l.m.Z.m.Z...e.
 00000070: 6a0b 6405 6405 6406 8d02 6407 6408 8400  j.d.d.d...d.d...
```

### Comparing `libertem-0.9.0/src/libertem/corrections/coordinates.py` & `libertem-0.9.2/src/libertem/corrections/coordinates.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/corrections/corrset.py` & `libertem-0.9.2/src/libertem/corrections/corrset.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/corrections/detector.py` & `libertem-0.9.2/src/libertem/corrections/detector.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/executor/__pycache__/base.cpython-39.pyc` & `libertem-0.9.2/src/libertem/executor/__pycache__/base.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 13307 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 fb33 0000  a.......z..b.3..
+00000000: 610d 0d0a 0000 0000 7fce 6762 fb33 0000  a.........gb.3..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 0e01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 6d05 5a05 6d06 5a06 6d07 5a07 6d08 5a08  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6400 6403 6c0b  m.Z.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6400 6404 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `libertem-0.9.0/src/libertem/executor/__pycache__/concurrent.cpython-39.pyc` & `libertem-0.9.2/src/libertem/executor/__pycache__/concurrent.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 5308 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 bc14 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 bc14 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 ae00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a04 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c05 6d06 5a06 6d07 5a07 0100 6403  d.l.m.Z.m.Z...d.
 00000060: 6404 6c08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 0100 6400 6405 6c0e  m.Z.m.Z...d.d.l.
```

### Comparing `libertem-0.9.0/src/libertem/executor/__pycache__/dask.cpython-39.pyc` & `libertem-0.9.2/src/libertem/executor/__pycache__/dask.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 22579 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 3358 0000  a.......z..b3X..
+00000000: 610d 0d0a 0000 0000 7fce 6762 3358 0000  a.........gb3X..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000a 0000 0040 0000 0073 4801 0000 6400  .....@...sH...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 6400 6401 6c04  ..d.d.l.Z.d.d.l.
 00000050: 5a04 6400 6401 6c05 5a05 6400 6403 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000070: 0100 6400 6404 6c0b 6d0c 5a0d 0100 6400  ..d.d.l.m.Z...d.
```

### Comparing `libertem-0.9.0/src/libertem/executor/__pycache__/delayed.cpython-39.pyc` & `libertem-0.9.2/src/libertem/executor/__pycache__/delayed.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 17893 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 e545 0000  a.......z..b.E..
+00000000: 610d 0d0a 0000 0000 7fce 6762 e545 0000  a.........gb.E..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5e01 0000 6400  .....@...s^...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 0100 6400 6403 6c08 5a08 6400  m.Z...d.d.l.Z.d.
 00000060: 6404 6c09 6d0a 5a0a 6d0b 5a0b 0100 6400  d.l.m.Z.m.Z...d.
 00000070: 6403 6c0c 5a0d 6400 6403 6c0e 5a0e 6400  d.l.Z.d.d.l.Z.d.
```

### Comparing `libertem-0.9.0/src/libertem/executor/__pycache__/inline.cpython-39.pyc` & `libertem-0.9.2/src/libertem/executor/__pycache__/inline.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 2569 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 090a 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 090a 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6c00 0000 6400  .....@...sl...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a03 6400 6402 6c04 5a04 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c05 5a05 6403 6404 6c06 6d07 5a07  d.l.Z.d.d.l.m.Z.
 00000060: 6d08 5a08 6d09 5a09 0100 6403 6405 6c0a  m.Z.m.Z...d.d.l.
 00000070: 6d0b 5a0b 6d0c 5a0c 0100 6400 6406 6c0d  m.Z.m.Z...d.d.l.
```

### Comparing `libertem-0.9.0/src/libertem/executor/__pycache__/integration.cpython-39.pyc` & `libertem-0.9.2/src/libertem/executor/__pycache__/integration.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 2563 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 030a 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 030a 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a01 6400 6401 6c03 6d04 5a05  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6402 6403 6c01 6d06 5a06 0100 6402  ..d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 0100 6402 6405 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 0100 6406 6407 8400 5a0b 6401  m.Z...d.d...Z.d.
```

### Comparing `libertem-0.9.0/src/libertem/executor/__pycache__/scheduler.cpython-39.pyc` & `libertem-0.9.2/src/libertem/executor/__pycache__/scheduler.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 3506 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 b20d 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 b20d 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 8302 5a02 4700 6404 6405 8400  ..d...Z.G.d.d...
 00000050: 6405 8302 5a03 4700 6406 6407 8400 6407  d...Z.G.d.d...d.
 00000060: 8302 5a04 6408 5300 2909 e900 0000 0029  ..Z.d.S.)......)
 00000070: 01da 0b64 6566 6175 6c74 6469 6374 6300  ...defaultdictc.
```

### Comparing `libertem-0.9.0/src/libertem/executor/base.py` & `libertem-0.9.2/src/libertem/executor/base.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/executor/cli.py` & `libertem-0.9.2/src/libertem/executor/cli.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/executor/concurrent.py` & `libertem-0.9.2/src/libertem/executor/concurrent.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/executor/dask.py` & `libertem-0.9.2/src/libertem/executor/dask.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/executor/delayed.py` & `libertem-0.9.2/src/libertem/executor/delayed.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/executor/inline.py` & `libertem-0.9.2/src/libertem/executor/inline.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/executor/integration.py` & `libertem-0.9.2/src/libertem/executor/integration.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/executor/scheduler.py` & `libertem-0.9.2/src/libertem/executor/scheduler.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/executor/utils/__pycache__/dask_buffer.cpython-39.pyc` & `libertem-0.9.2/src/libertem/executor/utils/__pycache__/dask_buffer.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 7683 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 031e 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 031e 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7800 0000 6400  .....@...sx...d.
 00000030: 6401 6c00 6d01 5a02 0100 6400 6401 6c03  d.l.m.Z...d.d.l.
 00000040: 5a04 6402 6403 6c05 6d06 5a06 0100 6402  Z.d.d.l.m.Z...d.
 00000050: 6404 6c07 6d08 5a08 0100 6402 6405 6c09  d.l.m.Z...d.d.l.
 00000060: 6d0a 5a0a 0100 6406 6407 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
 00000070: 0100 4700 6408 6409 8400 6409 650a 8303  ..G.d.d...d.e...
```

### Comparing `libertem-0.9.0/src/libertem/executor/utils/__pycache__/dask_inplace.cpython-39.pyc` & `libertem-0.9.2/src/libertem/executor/utils/__pycache__/dask_inplace.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 7648 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 e01d 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 e01d 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4a00 0000 6400  .....@...sJ...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a03 6501 6403 6404  Z.d.d.l.Z.e.d.d.
 00000050: 6701 8302 5a04 4700 6405 6406 8400 6406  g...Z.G.d.d...d.
 00000060: 8302 5a05 6407 6408 8400 5a06 6409 640a  ..Z.d.d...Z.d.d.
 00000070: 8400 5a07 6402 5300 290b e900 0000 0029  ..Z.d.S.)......)
```

### Comparing `libertem-0.9.0/src/libertem/executor/utils/__pycache__/delayed_unpack.cpython-39.pyc` & `libertem-0.9.2/src/libertem/executor/utils/__pycache__/delayed_unpack.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 10183 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 c727 0000  a.......z..b.'..
+00000000: 610d 0d0a 0000 0000 7fce 6762 c727 0000  a.........gb.'..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000a 0000 0040 0000 0073 f601 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 0100 6504  m.Z.m.Z.m.Z...e.
 00000050: 6507 6502 6503 6701 6503 6505 6501 6501  e.e.e.g.e.e.e.e.
 00000060: 6602 1900 1900 6602 1900 6602 1900 6402  f.....f...f...d.
 00000070: 9c01 6403 6404 8404 5a08 6504 6507 6502  ..d.d...Z.e.e.e.
```

### Comparing `libertem-0.9.0/src/libertem/executor/utils/dask_buffer.py` & `libertem-0.9.2/src/libertem/executor/utils/dask_buffer.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/executor/utils/dask_inplace.py` & `libertem-0.9.2/src/libertem/executor/utils/dask_inplace.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/executor/utils/delayed_unpack.py` & `libertem-0.9.2/src/libertem/executor/utils/delayed_unpack.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/io/LICENSE` & `libertem-0.9.2/src/libertem/io/LICENSE`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/io/__pycache__/utils.cpython-39.pyc` & `libertem-0.9.2/src/libertem/io/__pycache__/utils.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 1717 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 b506 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 b506 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 8200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 7a14 6400 6404 6c07 5a07  m.Z...z.d.d.l.Z.
 00000060: 6405 6406 8400 5a08 5700 6e1e 0400 6509  d.d...Z.W.n...e.
 00000070: 795a 0100 0100 0100 6400 6407 6c0a 6d08  yZ......d.d.l.m.
@@ -75,15 +75,15 @@
 000004a0: 6173 745f 7369 7a65 da03 7265 7372 0e00  ast_size..resr..
 000004b0: 0000 720e 0000 0072 0f00 0000 da13 6765  ..r....r......ge
 000004c0: 745f 7061 7274 6974 696f 6e5f 7368 6170  t_partition_shap
 000004d0: 6514 0000 0073 2000 0000 0014 0801 0402  e....s .........
 000004e0: 0801 0402 1402 1201 0a01 0c01 0801 0602  ................
 000004f0: 0801 1201 0a01 0602 2001 7222 0000 0029  ........ .r"...)
 00000500: 014e 290d da06 7479 7069 6e67 7202 0000  .N)...typingr...
-00000510: 0072 0300 0000 5a0f 6c69 6265 7274 656d  .r....Z.libertem
+00000510: 0072 0300 0000 da0f 6c69 6265 7274 656d  .r......libertem
 00000520: 2e63 6f6d 6d6f 6e72 0400 0000 da14 6c69  .commonr......li
 00000530: 6265 7274 656d 2e63 6f6d 6d6f 6e2e 6d61  bertem.common.ma
 00000540: 7468 7205 0000 0072 0600 0000 7210 0000  thr....r....r...
 00000550: 00da 134d 6f64 756c 654e 6f74 466f 756e  ...ModuleNotFoun
 00000560: 6445 7272 6f72 5a13 6c69 6265 7274 656d  dErrorZ.libertem
 00000570: 2e77 696e 5f74 7765 616b 7372 1900 0000  .win_tweaksr....
 00000580: 7222 0000 0072 0e00 0000 720e 0000 0072  r"...r....r....r
```

### Comparing `libertem-0.9.0/src/libertem/io/dataset/__init__.py` & `libertem-0.9.2/src/libertem/io/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/io/dataset/__pycache__/__init__.cpython-39.pyc` & `libertem-0.9.2/src/libertem/io/dataset/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 5726 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 5e16 0000  a.......z..b^...
+00000000: 610d 0d0a 0000 0000 7fce 6762 5e16 0000  a.........gb^...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000f 0000 0040 0000 0073 ae01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 6d06 5a06 0100 6400 6404 6c07  m.Z.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6400 6405 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6406 6407 6408 6409 640a 640b 640c  ..d.d.d.d.d.d.d.
```

### Comparing `libertem-0.9.0/src/libertem/io/dataset/__pycache__/blo.cpython-39.pyc` & `libertem-0.9.2/src/libertem/io/dataset/__pycache__/blo.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 8726 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 1622 0000  a.......z..b."..
+00000000: 610d 0d0a 0000 0000 7fce 6762 1622 0000  a.........gb."..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a03 6400 6402 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c06 6d07 5a07 0100 6404  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `libertem-0.9.0/src/libertem/io/dataset/__pycache__/cached.cpython-39.pyc` & `libertem-0.9.2/src/libertem/io/dataset/__pycache__/cached.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 18746 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 3a49 0000  a.......z..b:I..
+00000000: 610d 0d0a 0000 0000 7fce 6762 3a49 0000  a.........gb:I..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 f000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6402 6c06 6d07 5a07 0100 6400 6401 6c08  d.l.m.Z...d.d.l.
 00000070: 5a09 6403 6404 6c0a 6d0b 5a0b 6d0c 5a0c  Z.d.d.l.m.Z.m.Z.
```

### Comparing `libertem-0.9.0/src/libertem/io/dataset/__pycache__/cluster.cpython-39.pyc` & `libertem-0.9.2/src/libertem/io/dataset/__pycache__/cluster.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 8456 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 0821 0000  a.......z..b.!..
+00000000: 610d 0d0a 0000 0000 7fce 6762 0821 0000  a.........gb.!..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6401 6c04  d.l.m.Z...d.d.l.
 00000050: 5a05 6400 6403 6c06 6d07 5a07 0100 6404  Z.d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 0100 6404  m.Z.m.Z.m.Z...d.
```

### Comparing `libertem-0.9.0/src/libertem/io/dataset/__pycache__/dask.cpython-39.pyc` & `libertem-0.9.2/src/libertem/io/dataset/__pycache__/dask.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 21163 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 ab52 0000  a.......z..b.R..
+00000000: 610d 0d0a 0000 0000 7fce 6762 ab52 0000  a.........gb.R..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5e01 0000 6400  .....@...s^...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a03 6400 6401 6c04 6d05 5a06  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6402 6c07 6d08 5a08 6d09 5a09  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6400 6403 6c0a 6d0b 5a0b 6d0c 5a0c  ..d.d.l.m.Z.m.Z.
 00000070: 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f 6d10 5a10  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `libertem-0.9.0/src/libertem/io/dataset/__pycache__/dm.cpython-39.pyc` & `libertem-0.9.2/src/libertem/io/dataset/__pycache__/dm.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 10195 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 d327 0000  a.......z..b.'..
+00000000: 610d 0d0a 0000 0000 7fce 6762 d327 0000  a.........gb.'..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 ec00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c04 6d05 5a05 0100 6400 6401 6c06  d.l.m.Z...d.d.l.
 00000060: 5a07 6400 6403 6c08 6d09 5a09 0100 6400  Z.d.d.l.m.Z...d.
 00000070: 6404 6c0a 6d0b 5a0b 0100 6400 6405 6c0c  d.l.m.Z...d.d.l.
```

### Comparing `libertem-0.9.0/src/libertem/io/dataset/__pycache__/empad.cpython-39.pyc` & `libertem-0.9.2/src/libertem/io/dataset/__pycache__/empad.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 9356 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 8c24 0000  a.......z..b.$..
+00000000: 610d 0d0a 0000 0000 7fce 6762 8c24 0000  a.........gb.$..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 6d03 5a04 0100 6400 6401 6c05  d.l.m.Z...d.d.l.
 00000050: 5a06 6400 6402 6c07 6d08 5a08 0100 6400  Z.d.d.l.m.Z...d.
 00000060: 6403 6c09 6d0a 5a0a 0100 6400 6404 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6405 6406 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `libertem-0.9.0/src/libertem/io/dataset/__pycache__/frms6.cpython-39.pyc` & `libertem-0.9.2/src/libertem/io/dataset/__pycache__/frms6.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 23589 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 255c 0000  a.......z..b%\..
+00000000: 610d 0d0a 0000 0000 7fce 6762 255c 0000  a.........gb%\..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000a 0000 0040 0000 0073 4002 0000 6400  .....@...s@...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000050: 6d04 5a04 0100 6400 6401 6c05 5a05 6400  m.Z...d.d.l.Z.d.
 00000060: 6401 6c06 5a06 6400 6401 6c07 5a07 6400  d.l.Z.d.d.l.Z.d.
 00000070: 6401 6c08 5a08 6400 6401 6c09 5a09 6400  d.l.Z.d.d.l.Z.d.
@@ -208,18 +208,18 @@
 00000cf0: 0d4e 7a1b 436f 756c 6420 6e6f 7420 6669  .Nz.Could not fi
 00000d00: 6e64 202e 6864 7220 6669 6c65 207b 7d5a  nd .hdr file {}Z
 00000d10: 0f6d 6561 7375 7265 6d65 6e74 496e 666f  .measurementInfo
 00000d20: 7a33 6d65 6173 7572 656d 656e 7449 6e66  z3measurementInf
 00000d30: 6f20 6d69 7373 696e 6720 6672 6f6d 202e  o missing from .
 00000d40: 6864 7220 6669 6c65 207b 7d2c 2068 6176  hdr file {}, hav
 00000d50: 653a 207b 7d3e 0400 0000 5a0a 6461 726b  e: {}>....Z.dark
-00000d60: 6672 616d 6573 da0c 7369 676e 616c 6672  frames..signalfr
-00000d70: 616d 6573 5a15 6477 656c 6c74 696d 656d  amesZ.dwelltimem
-00000d80: 6963 726f 7365 636f 6e64 73da 0467 6169  icroseconds..gai
-00000d90: 6e63 0100 0000 0000 0000 0000 0000 0200  nc..............
+00000d60: 6672 616d 6573 5a15 6477 656c 6c74 696d  framesZ.dwelltim
+00000d70: 656d 6963 726f 7365 636f 6e64 73da 0467  emicroseconds..g
+00000d80: 6169 6eda 0c73 6967 6e61 6c66 7261 6d65  ain..signalframe
+00000d90: 7363 0100 0000 0000 0000 0000 0000 0200  sc..............
 00000da0: 0000 0300 0000 7300 0000 7316 0000 007c  ......s...s....|
 00000db0: 005d 0e7d 0174 007c 0183 0156 0001 0071  .].}.t.|...V...q
 00000dc0: 0264 0053 00a9 014e a901 da03 696e 7429  .d.S...N....int)
 00000dd0: 0272 3900 0000 da01 7072 3800 0000 7238  .r9.....pr8...r8
 00000de0: 0000 0072 3d00 0000 da09 3c67 656e 6578  ...r=.....<genex
 00000df0: 7072 3e9a 0000 00f3 0000 0000 7a24 5f72  pr>.........z$_r
 00000e00: 6561 645f 6461 7461 7365 745f 6864 722e  ead_dataset_hdr.
@@ -783,15 +783,15 @@
 000030e0: 0000 723d 0000 0072 a900 0000 cc01 0000  ..r=...r........
 000030f0: 7304 0000 0006 0202 ff7a 2f46 524d 5336  s........z/FRMS6
 00003100: 4461 7461 5365 742e 5f64 6f5f 696e 6974  DataSet._do_init
 00003110: 6961 6c69 7a65 2e3c 6c6f 6361 6c73 3e2e  ialize.<locals>.
 00003120: 3c6c 6973 7463 6f6d 703e 7201 0000 0072  <listcomp>r....r
 00003130: 1c00 0000 721b 0000 0072 2b00 0000 7269  ....r....r+...ri
 00003140: 0000 0072 f900 0000 720a 0000 0072 1600  ...r....r....r..
-00003150: 0000 725f 0000 0072 6700 0000 7a1d 7369  ..r_...rg...z.si
+00003150: 0000 7260 0000 0072 6700 0000 7a1d 7369  ..r`...rg...z.si
 00003160: 675f 7368 6170 6520 6d75 7374 2062 6520  g_shape must be 
 00003170: 6f66 2073 697a 653a 2025 73da 0766 6c6f  of size: %s..flo
 00003180: 6174 3332 da0e 7261 775f 6672 616d 655f  at32..raw_frame_
 00003190: 7369 7a65 a901 da08 7369 675f 6469 6d73  size....sig_dims
 000031a0: 2906 da09 7261 775f 6474 7970 6572 7d00  )...raw_dtyper}.
 000031b0: 0000 da08 6d65 7461 6461 7461 724d 0000  ....metadatarM..
 000031c0: 0072 3300 0000 da0b 696d 6167 655f 636f  .r3.....image_co
@@ -1121,15 +1121,15 @@
 00004600: 0102 0102 0102 0106 0102 0102 0102 0102  ................
 00004610: f904 ff04 0b0a 0108 0102 0102 0102 0102  ................
 00004620: fd7a 1946 524d 5336 4461 7461 5365 742e  .z.FRMS6DataSet.
 00004630: 5f67 6574 5f66 696c 6573 6574 6301 0000  _get_filesetc...
 00004640: 0000 0000 0000 0000 0001 0000 0004 0000  ................
 00004650: 0043 0000 0073 1000 0000 7400 7c00 6a01  .C...s....t.|.j.
 00004660: 7c00 6a02 6401 8d02 5300 2902 4e29 02da  |.j.d...S.).N)..
-00004670: 0464 6172 6b72 6000 0000 2903 7206 0000  .darkr`...).r...
+00004670: 0464 6172 6b72 5f00 0000 2903 7206 0000  .darkr_...).r...
 00004680: 0072 0901 0000 722b 0100 0072 1701 0000  .r....r+...r....
 00004690: 7238 0000 0072 3800 0000 723d 0000 00da  r8...r8...r=....
 000046a0: 1367 6574 5f63 6f72 7265 6374 696f 6e5f  .get_correction_
 000046b0: 6461 7461 9d02 0000 7308 0000 0000 0102  data....s.......
 000046c0: 0104 0104 fe7a 2046 524d 5336 4461 7461  .....z FRMS6Data
 000046d0: 5365 742e 6765 745f 636f 7272 6563 7469  Set.get_correcti
 000046e0: 6f6e 5f64 6174 6163 0100 0000 0000 0000  on_datac........
```

### Comparing `libertem-0.9.0/src/libertem/io/dataset/__pycache__/hdf5.cpython-39.pyc` & `libertem-0.9.2/src/libertem/io/dataset/__pycache__/hdf5.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 28043 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 8b6d 0000  a.......z..b.m..
+00000000: 610d 0d0a 0000 0000 7fce 6762 8b6d 0000  a.........gb.m..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 1a01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 6400 6401 6c04  ..d.d.l.Z.d.d.l.
 00000050: 5a04 6400 6401 6c05 5a05 6400 6401 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 5a07 6400 6401 6c08 5a08 6400 6403 6c09  Z.d.d.l.Z.d.d.l.
 00000070: 6d0a 5a0a 0100 6400 6404 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
@@ -618,16 +618,16 @@
 00002690: 721c 0000 0072 1c00 0000 7221 0000 00da  r....r....r!....
 000026a0: 1167 6574 5f6d 7367 5f63 6f6e 7665 7274  .get_msg_convert
 000026b0: 6572 2401 0000 7302 0000 0000 027a 1b48  er$...s......z.H
 000026c0: 3544 6174 6153 6574 2e67 6574 5f6d 7367  5DataSet.get_msg
 000026d0: 5f63 6f6e 7665 7274 6572 6301 0000 0000  _converterc.....
 000026e0: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
 000026f0: 0000 0073 0800 0000 6800 6401 a301 5300  ...s....h.d...S.
-00002700: 2902 4e3e 0400 0000 da02 6835 5a04 6873  ).N>......h5Z.hs
-00002710: 7079 da04 6864 6635 5a03 6e78 7372 1c00  py..hdf5Z.nxsr..
+00002700: 2902 4e3e 0400 0000 da02 6835 da04 6864  ).N>......h5..hd
+00002710: 6635 5a04 6873 7079 5a03 6e78 7372 1c00  f5Z.hspyZ.nxsr..
 00002720: 0000 7297 0000 0072 1c00 0000 721c 0000  ..r....r....r...
 00002730: 0072 2100 0000 da18 6765 745f 7375 7070  .r!.....get_supp
 00002740: 6f72 7465 645f 6578 7465 6e73 696f 6e73  orted_extensions
 00002750: 2801 0000 7302 0000 0000 027a 2248 3544  (...s......z"H5D
 00002760: 6174 6153 6574 2e67 6574 5f73 7570 706f  ataSet.get_suppo
 00002770: 7274 6564 5f65 7874 656e 7369 6f6e 7363  rted_extensionsc
 00002780: 0100 0000 0000 0000 0000 0000 0100 0000  ................
```

### Comparing `libertem-0.9.0/src/libertem/io/dataset/__pycache__/k2is.cpython-39.pyc` & `libertem-0.9.2/src/libertem/io/dataset/__pycache__/k2is.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 37600 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 e092 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 e092 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 1402 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6401 6c06 5a06 6400 6401 6c07 5a08 6400  d.l.Z.d.d.l.Z.d.
 00000070: 6401 6c09 5a09 6400 6402 6c0a 6d0b 5a0b  d.l.Z.d.d.l.m.Z.
```

### Comparing `libertem-0.9.0/src/libertem/io/dataset/__pycache__/memory.cpython-39.pyc` & `libertem-0.9.2/src/libertem/io/dataset/__pycache__/memory.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 13036 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 ec32 0000  a.......z..b.2..
+00000000: 610d 0d0a 0000 0000 7fce 6762 ec32 0000  a.........gb.2..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 1601 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 0100 6400  d.l.m.Z.m.Z...d.
 00000050: 6401 6c05 5a05 6400 6401 6c06 5a07 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6403 6c08 6d09 5a09 0100 6400 6404 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6400 6405 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
```

### Comparing `libertem-0.9.0/src/libertem/io/dataset/__pycache__/mib.cpython-39.pyc` & `libertem-0.9.2/src/libertem/io/dataset/__pycache__/mib.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 44457 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 a9ad 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 a9ad 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 5803 0000 6400  .....@...sX...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d02 5a02 6d03 5a03 0100 6400  d.l.m.Z.m.Z...d.
 00000050: 6401 6c04 5a04 6400 6403 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000060: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 0100 6400 6404 6c0d  m.Z.m.Z...d.d.l.
```

### Comparing `libertem-0.9.0/src/libertem/io/dataset/__pycache__/mrc.cpython-39.pyc` & `libertem-0.9.2/src/libertem/io/dataset/__pycache__/mrc.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 7380 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 d41c 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 d41c 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 ea00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6406  ..d.d.l.m.Z...d.
 00000070: 6407 6c0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  d.l.m.Z.m.Z.m.Z.
```

### Comparing `libertem-0.9.0/src/libertem/io/dataset/__pycache__/raw.cpython-39.pyc` & `libertem-0.9.2/src/libertem/io/dataset/__pycache__/raw.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 8609 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 a121 0000  a.......z..b.!..
+00000000: 610d 0d0a 0000 0000 7fce 6762 a121 0000  a.........gb.!..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a03 6400 6402 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c08 6d09 5a09 0100 6405 6406 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `libertem-0.9.0/src/libertem/io/dataset/__pycache__/seq.cpython-39.pyc` & `libertem-0.9.2/src/libertem/io/dataset/__pycache__/seq.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 23010 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 e259 0000  a.......z..b.Y..
+00000000: 610d 0d0a 0000 0000 7fce 6762 e259 0000  a.........gb.Y..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 001b 0000 0040 0000 0073 0e02 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6401 6c05 6d06 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6401 6c08 5a09 6400 6401 6c0a 5a0a 6400  d.l.Z.d.d.l.Z.d.
 00000070: 6403 6c0b 6d0c 5a0c 0100 6400 6404 6c0d  d.l.m.Z...d.d.l.
```

### Comparing `libertem-0.9.0/src/libertem/io/dataset/__pycache__/ser.cpython-39.pyc` & `libertem-0.9.2/src/libertem/io/dataset/__pycache__/ser.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 10454 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 d628 0000  a.......z..b.(..
+00000000: 610d 0d0a 0000 0000 7fce 6762 d628 0000  a.........gb.(..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 e800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a05 6400 6402 6c06 6d07 5a07  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6400 6403 6c08 6d09 5a09 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6404 6c0a 6d0b 5a0b 6d0c 5a0c 0100 6400  d.l.m.Z.m.Z...d.
```

### Comparing `libertem-0.9.0/src/libertem/io/dataset/__pycache__/tvips.cpython-39.pyc` & `libertem-0.9.2/src/libertem/io/dataset/__pycache__/tvips.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 17844 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 b445 0000  a.......z..b.E..
+00000000: 610d 0d0a 0000 0000 7fce 6762 b445 0000  a.........gb.E..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 f001 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a03 6400 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6400 6403 6c05 6d06 5a06 6d07 5a07  Z.d.d.l.m.Z.m.Z.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 0100 6400 6402 6c0d 5a0e 6400  m.Z...d.d.l.Z.d.
```

### Comparing `libertem-0.9.0/src/libertem/io/dataset/base/__init__.py` & `libertem-0.9.2/src/libertem/io/dataset/base/__init__.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/io/dataset/base/__pycache__/__init__.cpython-39.pyc` & `libertem-0.9.2/src/libertem/io/dataset/base/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 1271 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 f704 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 f704 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 f800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 0100 6400 6404 6c08  m.Z.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6406 6c0c 6d0d 5a0d 0100 6400  ..d.d.l.m.Z...d.
```

### Comparing `libertem-0.9.0/src/libertem/io/dataset/base/__pycache__/backend.cpython-39.pyc` & `libertem-0.9.2/src/libertem/io/dataset/base/__pycache__/backend.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 5117 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 fd13 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 fd13 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6401 6c05  m.Z.m.Z...d.d.l.
 00000050: 5a05 6400 6401 6c06 5a07 6403 6404 6c08  Z.d.d.l.Z.d.d.l.
 00000060: 6d09 5a09 0100 6500 a00a 650b a101 5a0c  m.Z...e...e...Z.
 00000070: 4700 6405 6406 8400 6406 8302 5a0d 4700  G.d.d...d...Z.G.
```

### Comparing `libertem-0.9.0/src/libertem/io/dataset/base/__pycache__/backend_buffered.cpython-39.pyc` & `libertem-0.9.2/src/libertem/io/dataset/base/__pycache__/backend_buffered.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 15021 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 ad3a 0000  a.......z..b.:..
+00000000: 610d 0d0a 0000 0000 7fce 6762 ad3a 0000  a.........gb.:..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 1401 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6401 6c04  d.l.m.Z...d.d.l.
 00000050: 5a05 6400 6401 6c06 5a06 6400 6403 6c07  Z.d.d.l.Z.d.d.l.
 00000060: 6d08 5a08 0100 6400 6401 6c09 5a09 6400  m.Z...d.d.l.Z.d.
 00000070: 6404 6c0a 6d0b 5a0b 0100 6400 6405 6c0c  d.l.m.Z...d.d.l.
@@ -684,15 +684,15 @@
 00002ab0: 0000 00da 146c 6962 6572 7465 6d2e 636f  .....libertem.co
 00002ac0: 6d6d 6f6e 2e6d 6174 6872 0400 0000 5a20  mmon.mathr....Z 
 00002ad0: 6c69 6265 7274 656d 2e69 6f2e 6461 7461  libertem.io.data
 00002ae0: 7365 742e 6261 7365 2e62 6163 6b65 6e64  set.base.backend
 00002af0: 7205 0000 0072 0600 0000 5a20 6c69 6265  r....r....Z libe
 00002b00: 7274 656d 2e69 6f2e 6461 7461 7365 742e  rtem.io.dataset.
 00002b10: 6261 7365 2e66 696c 6573 6574 7207 0000  base.filesetr...
-00002b20: 005a 0f6c 6962 6572 7465 6d2e 636f 6d6d  .Z.libertem.comm
+00002b20: 00da 0f6c 6962 6572 7465 6d2e 636f 6d6d  ...libertem.comm
 00002b30: 6f6e 7208 0000 0072 0900 0000 da17 6c69  onr....r......li
 00002b40: 6265 7274 656d 2e63 6f6d 6d6f 6e2e 6275  bertem.common.bu
 00002b50: 6666 6572 7372 0a00 0000 720b 0000 00da  ffersr....r.....
 00002b60: 156c 6962 6572 7465 6d2e 636f 6d6d 6f6e  .libertem.common
 00002b70: 2e6e 756d 6261 720d 0000 00da 0674 696c  .numbar......til
 00002b80: 696e 6772 0f00 0000 7228 0000 0072 1000  ingr....r(...r..
 00002b90: 0000 728c 0000 0072 2c00 0000 da04 6e6a  ..r....r,.....nj
```

### Comparing `libertem-0.9.0/src/libertem/io/dataset/base/__pycache__/backend_direct.cpython-39.pyc` & `libertem-0.9.2/src/libertem/io/dataset/base/__pycache__/backend_direct.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 1347 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 4305 0000  a.......z..bC...
+00000000: 610d 0d0a 0000 0000 7fce 6762 4305 0000  a.........gbC...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 3800 0000 6400  .....@...s8...d.
 00000030: 6401 6c00 5a00 6402 6403 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6402 6404 6c03 6d04 5a04 0100 4700  ..d.d.l.m.Z...G.
 00000050: 6405 6406 8400 6406 6502 6407 6408 8d04  d.d...d.e.d.d...
 00000060: 5a05 6401 5300 2909 e900 0000 004e e901  Z.d.S.)......N..
 00000070: 0000 0029 01da 0949 4f42 6163 6b65 6e64  ...)...IOBackend
```

### Comparing `libertem-0.9.0/src/libertem/io/dataset/base/__pycache__/backend_mmap.cpython-39.pyc` & `libertem-0.9.2/src/libertem/io/dataset/base/__pycache__/backend_mmap.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 12823 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 1732 0000  a.......z..b.2..
+00000000: 610d 0d0a 0000 0000 7fce 6762 1732 0000  a.........gb.2..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 0a01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a05 6400 6402 6c06 6d07 5a07  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6400 6401 6c08 5a08 6400 6403 6c09  ..d.d.l.Z.d.d.l.
 00000070: 6d0a 5a0a 0100 6400 6404 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
@@ -683,17 +683,17 @@
 00002aa0: 0000 00da 056e 756d 6261 da14 6c69 6265  .....numba..libe
 00002ab0: 7274 656d 2e63 6f6d 6d6f 6e2e 6d61 7468  rtem.common.math
 00002ac0: 7203 0000 005a 206c 6962 6572 7465 6d2e  r....Z libertem.
 00002ad0: 696f 2e64 6174 6173 6574 2e62 6173 652e  io.dataset.base.
 00002ae0: 6261 636b 656e 6472 0400 0000 7205 0000  backendr....r...
 00002af0: 005a 206c 6962 6572 7465 6d2e 696f 2e64  .Z libertem.io.d
 00002b00: 6174 6173 6574 2e62 6173 652e 6669 6c65  ataset.base.file
-00002b10: 7365 7472 0600 0000 5a0f 6c69 6265 7274  setr....Z.libert
+00002b10: 7365 7472 0600 0000 da0f 6c69 6265 7274  setr......libert
 00002b20: 656d 2e63 6f6d 6d6f 6e72 0700 0000 7208  em.commonr....r.
-00002b30: 0000 005a 176c 6962 6572 7465 6d2e 636f  ...Z.libertem.co
+00002b30: 0000 00da 176c 6962 6572 7465 6d2e 636f  .....libertem.co
 00002b40: 6d6d 6f6e 2e62 7566 6665 7273 7209 0000  mmon.buffersr...
 00002b50: 00da 156c 6962 6572 7465 6d2e 636f 6d6d  ...libertem.comm
 00002b60: 6f6e 2e6e 756d 6261 720b 0000 00da 0674  on.numbar......t
 00002b70: 696c 696e 6772 0d00 0000 7223 0000 0072  ilingr....r#...r
 00002b80: 0e00 0000 728b 0000 0072 2700 0000 da04  ....r....r'.....
 00002b90: 6e6a 6974 7233 0000 0072 3400 0000 7249  njitr3...r4...rI
 00002ba0: 0000 0072 5300 0000 723a 0000 0072 2400  ...rS...r:...r$.
```

### Comparing `libertem-0.9.0/src/libertem/io/dataset/base/__pycache__/coordinates.cpython-39.pyc` & `libertem-0.9.2/src/libertem/io/dataset/base/__pycache__/coordinates.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 1535 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 ff05 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 ff05 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 4a00 0000 6400  .....@...sJ...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c04 6d05 5a05 6d06 5a06  ..d.d.l.m.Z.m.Z.
 00000050: 0100 6400 6404 6c07 6d08 5a08 0100 6408  ..d.d.l.m.Z...d.
 00000060: 6506 6505 6501 6a09 6405 9c03 6406 6407  e.e.e.j.d...d.d.
 00000070: 8405 5a0a 6401 5300 2909 e900 0000 004e  ..Z.d.S.)......N
@@ -85,15 +85,15 @@
 00000540: 745f 636f 6f72 6469 6e61 7465 7308 0000  t_coordinates...
 00000550: 0073 2a00 0000 0011 0601 0601 0801 0801  .s*.............
 00000560: 1001 0e01 0801 1201 0401 0401 1401 02fe  ................
 00000570: 0204 02fb 0808 0c01 1601 0a01 0a01 1601  ................
 00000580: 7225 0000 0029 014e 290b da05 6e75 6d70  r%...).N)...nump
 00000590: 7972 1200 0000 da14 6c69 6265 7274 656d  yr......libertem
 000005a0: 2e63 6f6d 6d6f 6e2e 6d61 7468 7202 0000  .common.mathr...
-000005b0: 005a 0f6c 6962 6572 7465 6d2e 636f 6d6d  .Z.libertem.comm
+000005b0: 00da 0f6c 6962 6572 7465 6d2e 636f 6d6d  ...libertem.comm
 000005c0: 6f6e 7203 0000 0072 0400 0000 da18 6c69  onr....r......li
 000005d0: 6265 7274 656d 2e69 6f2e 6461 7461 7365  bertem.io.datase
 000005e0: 742e 6261 7365 7205 0000 00da 076e 6461  t.baser......nda
 000005f0: 7272 6179 7225 0000 0072 2300 0000 7223  rrayr%...r#...r#
 00000600: 0000 0072 2300 0000 7224 0000 00da 083c  ...r#...r$.....<
 00000610: 6d6f 6475 6c65 3e01 0000 0073 0800 0000  module>....s....
 00000620: 0802 0c01 1001 0c03                      ........
```

### Comparing `libertem-0.9.0/src/libertem/io/dataset/base/__pycache__/dataset.cpython-39.pyc` & `libertem-0.9.2/src/libertem/io/dataset/base/__pycache__/dataset.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 10241 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 0128 0000  a.......z..b.(..
+00000000: 610d 0d0a 0000 0000 7fce 6762 0128 0000  a.........gb.(..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 d200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c00 6d01 5a01  d.l.Z.d.d.l.m.Z.
 00000040: 6d02 5a02 6d03 5a03 0100 6400 6401 6c04  m.Z.m.Z...d.d.l.
 00000050: 5a05 6400 6403 6c06 6d07 5a07 0100 6400  Z.d.d.l.m.Z...d.
 00000060: 6404 6c08 6d09 5a09 0100 6400 6405 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6400 6406 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
@@ -670,15 +670,15 @@
 000029d0: 0700 0000 7259 0000 0072 0800 0000 7209  ....rY...r....r.
 000029e0: 0000 005a 1d6c 6962 6572 7465 6d2e 7765  ...Z.libertem.we
 000029f0: 622e 6d65 7373 6167 6563 6f6e 7665 7274  b.messageconvert
 00002a00: 6572 720a 0000 00da 1c6c 6962 6572 7465  err......liberte
 00002a10: 6d2e 636f 7272 6563 7469 6f6e 732e 636f  m.corrections.co
 00002a20: 7272 7365 7472 0c00 0000 da09 7061 7274  rrsetr......part
 00002a30: 6974 696f 6e72 0e00 0000 720f 0000 00da  itionr....r.....
-00002a40: 0d54 5950 455f 4348 4543 4b49 4e47 5a16  .TYPE_CHECKINGZ.
+00002a40: 0d54 5950 455f 4348 4543 4b49 4e47 da16  .TYPE_CHECKING..
 00002a50: 6c69 6265 7274 656d 2e65 7865 6375 746f  libertem.executo
 00002a60: 722e 6261 7365 7210 0000 0072 1100 0000  r.baser....r....
 00002a70: 7212 0000 0072 1300 0000 da02 6e74 7215  r....r......ntr.
 00002a80: 0000 0072 7e00 0000 721f 0000 0072 1f00  ...r~...r....r..
 00002a90: 0000 721f 0000 0072 2000 0000 da08 3c6d  ..r....r .....<m
 00002aa0: 6f64 756c 653e 0100 0000 7322 0000 0008  odule>....s"....
 00002ab0: 0114 0208 010c 020c 010c 0110 010c 010c  ................
```

### Comparing `libertem-0.9.0/src/libertem/io/dataset/base/__pycache__/decode.cpython-39.pyc` & `libertem-0.9.2/src/libertem/io/dataset/base/__pycache__/decode.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 5044 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 b413 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 b413 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6001 0000 6400  .....@...s`...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a03 6503 6a04 6402 6403 6404  d.l.Z.e.j.d.d.d.
 00000050: 8d02 6405 6406 8400 8301 5a05 6503 6a04  ..d.d.....Z.e.j.
 00000060: 6402 6403 6404 8d02 6407 6408 8400 8301  d.d.d...d.d.....
 00000070: 5a06 6503 6a04 6402 6403 6404 8d02 6409  Z.e.j.d.d.d...d.
```

### Comparing `libertem-0.9.0/src/libertem/io/dataset/base/__pycache__/file.cpython-39.pyc` & `libertem-0.9.2/src/libertem/io/dataset/base/__pycache__/file.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 5680 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 3016 0000  a.......z..b0...
+00000000: 610d 0d0a 0000 0000 7fce 6762 3016 0000  a.........gb0...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a04 6400 6403 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000050: 0100 4700 6404 6405 8400 6405 6501 8303  ..G.d.d...d.e...
 00000060: 5a07 4700 6406 6407 8400 6407 8302 5a08  Z.G.d.d...d...Z.
 00000070: 6402 5300 2908 e900 0000 0029 02da 0a4e  d.S.)......)...N
```

### Comparing `libertem-0.9.0/src/libertem/io/dataset/base/__pycache__/fileset.cpython-39.pyc` & `libertem-0.9.2/src/libertem/io/dataset/base/__pycache__/fileset.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 3159 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 570c 0000  a.......z..bW...
+00000000: 610d 0d0a 0000 0000 7fce 6762 570c 0000  a.........gbW...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 6c03 6d04 5a04 0100 6402 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6402 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6402 6406 6c09 6d0a 5a0a 0100 4700  ..d.d.l.m.Z...G.
 00000070: 6407 6408 8400 6408 8302 5a0b 6401 5300  d.d...d...Z.d.S.
```

### Comparing `libertem-0.9.0/src/libertem/io/dataset/base/__pycache__/meta.cpython-39.pyc` & `libertem-0.9.2/src/libertem/io/dataset/base/__pycache__/meta.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 4217 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 7910 0000  a.......z..by...
+00000000: 610d 0d0a 0000 0000 7fce 6762 7910 0000  a.........gby...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c04 5a04 6400 6402 6c05  ..d.d.l.Z.d.d.l.
 00000050: 5a06 6400 6403 6c07 6d08 5a08 0100 6503  Z.d.d.l.m.Z...e.
 00000060: 7240 6400 6404 6c05 6d00 5a09 0100 4700  r@d.d.l.m.Z...G.
 00000070: 6405 6406 8400 6406 8302 5a0a 4700 6407  d.d...d...Z.G.d.
```

### Comparing `libertem-0.9.0/src/libertem/io/dataset/base/__pycache__/partition.cpython-39.pyc` & `libertem-0.9.2/src/libertem/io/dataset/base/__pycache__/partition.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 8726 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 1622 0000  a.......z..b."..
+00000000: 610d 0d0a 0000 0000 7fce 6762 1622 0000  a.........gb."..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a04 6400 6403 6c05  ..d.d.l.Z.d.d.l.
 00000050: 6d06 5a06 6d07 5a07 0100 6400 6404 6c08  m.Z.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6405 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6405 6407 6c0c 6d0d 5a0d 0100 6405  ..d.d.l.m.Z...d.
@@ -554,15 +554,15 @@
 00002290: 6173 7363 656c 6c5f 5f72 1300 0000 7213  asscell__r....r.
 000022a0: 0000 0072 6000 0000 7214 0000 0072 5600  ...r`...r....rV.
 000022b0: 0000 7600 0000 7320 0000 0008 0104 1c00  ..v...s ........
 000022c0: fc02 0104 0106 0102 0106 fc10 1608 0408  ................
 000022d0: 080a 1e0a 0a08 040e 0310 2b72 5600 0000  ..........+rV...
 000022e0: 2919 7230 0000 00da 0674 7970 696e 6772  ).r0.....typingr
 000022f0: 0200 0000 da05 6e75 6d70 7972 6b00 0000  ......numpyrk...
-00002300: 5a0f 6c69 6265 7274 656d 2e63 6f6d 6d6f  Z.libertem.commo
+00002300: da0f 6c69 6265 7274 656d 2e63 6f6d 6d6f  ..libertem.commo
 00002310: 6e72 0300 0000 7204 0000 00da 146c 6962  nr....r......lib
 00002320: 6572 7465 6d2e 636f 7272 6563 7469 6f6e  ertem.correction
 00002330: 7372 0500 0000 da06 7469 6c69 6e67 7207  sr......tilingr.
 00002340: 0000 0072 4100 0000 7208 0000 0072 1c00  ...rA...r....r..
 00002350: 0000 7209 0000 0072 5700 0000 720a 0000  ..r....rW...r...
 00002360: 00da 0072 0b00 0000 da06 6465 636f 6465  ...r......decode
 00002370: 720c 0000 0072 0d00 0000 721a 0000 0072  r....r....r....r
```

### Comparing `libertem-0.9.0/src/libertem/io/dataset/base/__pycache__/roi.cpython-39.pyc` & `libertem-0.9.2/src/libertem/io/dataset/base/__pycache__/roi.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 1845 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 3507 0000  a.......z..b5...
+00000000: 610d 0d0a 0000 0000 7fce 6762 3507 0000  a.........gb5...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 0100 6500 6a05 6403  d.l.m.Z...e.j.d.
 00000050: 6404 8d01 640a 6405 6406 8401 8301 5a06  d...d.d.d.....Z.
 00000060: 6504 6407 9c01 6408 6409 8404 5a07 6401  e.d...d.d...Z.d.
 00000070: 5300 290b e900 0000 004e 2901 da05 536c  S.)......N)...Sl
```

### Comparing `libertem-0.9.0/src/libertem/io/dataset/base/__pycache__/tiling.cpython-39.pyc` & `libertem-0.9.2/src/libertem/io/dataset/base/__pycache__/tiling.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 11867 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 5b2e 0000  a.......z..b[...
+00000000: 610d 0d0a 0000 0000 7fce 6762 5b2e 0000  a.........gb[...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a04 0100 6400 6401 6c05  d.l.m.Z...d.d.l.
 00000050: 5a06 6400 6403 6c07 6d08 5a09 6d0a 5a0a  Z.d.d.l.m.Z.m.Z.
 00000060: 0100 6404 6405 6c0b 6d0c 5a0c 0100 6500  ..d.d.l.m.Z...e.
 00000070: a00d 650e a101 5a0f 6501 6a10 6406 6407  ..e...Z.e.j.d.d.
```

### Comparing `libertem-0.9.0/src/libertem/io/dataset/base/__pycache__/tiling_scheme.cpython-39.pyc` & `libertem-0.9.2/src/libertem/io/dataset/base/__pycache__/tiling_scheme.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 17722 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 3a45 0000  a.......z..b:E..
+00000000: 610d 0d0a 0000 0000 7fce 6762 3a45 0000  a.........gb:E..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 e000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 6d05 5a05 6d06 5a06 6d07 5a07 6d08 5a08  m.Z.m.Z.m.Z.m.Z.
 00000060: 0100 6400 6403 6c09 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6401 6c0b 5a0c 6400 6404 6c0d 6d0e 5a0e  d.l.Z.d.d.l.m.Z.
@@ -405,15 +405,15 @@
 00001940: 696e 746f 2073 697a 6520 2564 7201 0000  into size %dr...
 00001950: 007a 0e54 6865 2074 696c 6573 6861 7065  .z.The tileshape
 00001960: 207a 2120 6973 2069 6e63 6f6d 7061 7469   z! is incompati
 00001970: 626c 6520 7769 7468 2062 6173 6520 7368  ble with base sh
 00001980: 6170 6520 7a0e 2069 6e20 6469 6d65 6e73  ape z. in dimens
 00001990: 696f 6e20 da01 2e29 0ada 0361 6e79 da03  ion ...)...any..
 000019a0: 7a69 7072 2100 0000 da03 6d61 7872 0b00  zipr!.....maxr..
-000019b0: 0000 da13 6765 745f 6578 636c 7564 6564  ....get_excluded
+000019b0: 0000 5a13 6765 745f 6578 636c 7564 6564  ..Z.get_excluded
 000019c0: 5f70 6978 656c 73da 0877 6172 6e69 6e67  _pixels..warning
 000019d0: 73da 0477 6172 6eda 0572 616e 6765 723c  s..warn..ranger<
 000019e0: 0000 0029 0c72 2200 0000 722b 0000 0072  ...).r"...r+...r
 000019f0: 5400 0000 722c 0000 0072 5500 0000 7256  T...r,...rU...rV
 00001a00: 0000 0072 5700 0000 7258 0000 00da 0973  ...rW...rX.....s
 00001a10: 6967 5f73 6861 7065 da07 7369 7a65 5f70  ig_shape..size_p
 00001a20: 78da 076d 6573 7361 6765 da03 6469 6d72  x..message..dimr
@@ -510,78 +510,78 @@
 00001fd0: 6620 696e 7465 7265 7374 0a0a 2020 2020  f interest..    
 00001fe0: 2020 2020 636f 7272 6563 7469 6f6e 7320      corrections 
 00001ff0: 3a20 436f 7272 6563 7469 6f6e 5365 740a  : CorrectionSet.
 00002000: 2020 2020 2020 2020 2020 2020 436f 7272              Corr
 00002010: 6563 7469 6f6e 2073 6574 2074 6f20 636f  ection set to co
 00002020: 6e73 6964 6572 2069 6e20 6e65 676f 7469  nsider in negoti
 00002030: 6174 696f 6e0a 2020 2020 2020 2020 2903  ation.        ).
-00002040: 726b 0000 0072 6900 0000 7258 0000 0063  rk...ri...rX...c
+00002040: 726a 0000 0072 6800 0000 7258 0000 0063  rj...rh...rX...c
 00002050: 0100 0000 0000 0000 0000 0000 0200 0000  ................
 00002060: 0600 0000 1300 0000 7318 0000 0067 007c  ........s....g.|
 00002070: 005d 107d 0188 01a0 007c 0188 00a1 0291  .].}.....|......
 00002080: 0271 0453 0072 2400 0000 2901 da0e 5f67  .q.S.r$...)..._g
 00002090: 6574 5f6d 696e 5f64 6570 7468 a902 723f  et_min_depth..r?
-000020a0: 0000 00da 0375 6466 2902 726a 0000 0072  .....udf).rj...r
+000020a0: 0000 00da 0375 6466 2902 7269 0000 0072  .....udf).ri...r
 000020b0: 2200 0000 7224 0000 0072 2500 0000 da0a  "...r$...r%.....
 000020c0: 3c6c 6973 7463 6f6d 703e 0c01 0000 7304  <listcomp>....s.
 000020d0: 0000 0006 0202 ff7a 294e 6567 6f74 6961  .......z)Negotia
 000020e0: 746f 722e 6765 745f 7363 6865 6d65 2e3c  tor.get_scheme.<
 000020f0: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
 00002100: 703e 6301 0000 0000 0000 0000 0000 0002  p>c.............
 00002110: 0000 0009 0000 0013 0000 0073 1e00 0000  ...........s....
 00002120: 6700 7c00 5d16 7d01 8804 a000 8802 7c01  g.|.].}.......|.
 00002130: 8803 8800 8801 a105 9102 7104 5300 7224  ..........q.S.r$
 00002140: 0000 0029 01da 095f 6765 745f 7369 7a65  ...)..._get_size
-00002150: 726d 0000 00a9 0572 6a00 0000 7257 0000  rm.....rj...rW..
+00002150: 726c 0000 00a9 0572 6900 0000 7257 0000  rl.....ri...rW..
 00002160: 0072 5500 0000 7256 0000 0072 2200 0000  .rU...rV...r"...
-00002170: 7224 0000 0072 2500 0000 726f 0000 0015  r$...r%...ro....
+00002170: 7224 0000 0072 2500 0000 726e 0000 0015  r$...r%...rn....
 00002180: 0100 0073 0800 0000 0604 02fd 0401 0aff  ...s............
-00002190: 7211 0000 004e 2903 da0a 7469 6c65 5f73  r....N)...tile_s
-000021a0: 6861 7065 7264 0000 0072 5700 0000 2902  haperd...rW...).
+00002190: 7211 0000 004e 2903 5a0a 7469 6c65 5f73  r....N).Z.tile_s
+000021a0: 6861 7065 7263 0000 0072 5700 0000 2902  haperc...rW...).
 000021b0: da10 636f 6e74 6169 6e69 6e67 5f73 6861  ..containing_sha
 000021c0: 7065 722c 0000 0072 1900 0000 2901 7219  per,...r....).r.
-000021d0: 0000 0029 0372 7300 0000 722c 0000 00da  ...).rs...r,....
+000021d0: 0000 0029 0372 7100 0000 722c 0000 00da  ...).rq...r,....
 000021e0: 0b6d 696e 5f66 6163 746f 7273 7a1f 7469  .min_factorsz.ti
 000021f0: 6c65 7368 6170 6520 6265 666f 7265 2061  leshape before a
 00002200: 646a 7573 746d 656e 743a 2025 72a9 0172  djustment: %r..r
-00002210: 6b00 0000 7a1e 7469 6c65 7368 6170 6520  k...z.tileshape 
+00002210: 6a00 0000 7a1e 7469 6c65 7368 6170 6520  j...z.tileshape 
 00002220: 6166 7465 7220 6164 6a75 7374 6d65 6e74  after adjustment
-00002230: 3a20 2572 7228 0000 0029 0872 7400 0000  : %rr(...).rt...
+00002230: 3a20 2572 7228 0000 0029 0872 7200 0000  : %rr(...).rr...
 00002240: da07 6661 6374 6f72 7372 1600 0000 722c  ..factorsr....r,
-00002250: 0000 0072 6500 0000 da0f 6675 6c6c 5f62  ...re.....full_b
+00002250: 0000 0072 6400 0000 da0f 6675 6c6c 5f62  ...rd.....full_b
 00002260: 6173 655f 7368 6170 65da 0b6e 6565 645f  ase_shape..need_
 00002270: 6465 636f 6465 722d 0000 0029 0472 1600  decoder-...).r..
 00002280: 0000 7217 0000 0072 1800 0000 7223 0000  ..r....r....r#..
 00002290: 0029 1a72 4800 0000 7247 0000 0072 5600  .).rH...rG...rV.
 000022a0: 0000 5a10 6765 745f 6d69 6e5f 7369 675f  ..Z.get_min_sig_
-000022b0: 7369 7a65 722b 0000 0072 2f00 0000 7278  sizer+...r/...rx
+000022b0: 7369 7a65 722b 0000 0072 2f00 0000 7276  sizer+...r/...rv
 000022c0: 0000 00da 105f 6765 745f 696f 5f6d 6178  ....._get_io_max
 000022d0: 5f73 697a 6572 5f00 0000 da0f 5f67 6574  _sizer_....._get
 000022e0: 5f62 6173 655f 7368 6170 65da 0b5f 6765  _base_shape.._ge
 000022f0: 745f 696e 7465 6e74 da03 6d69 6eda 1068  t_intent..min..h
-00002300: 6176 655f 636f 7272 6563 7469 6f6e 73da  ave_corrections.
+00002300: 6176 655f 636f 7272 6563 7469 6f6e 735a  ave_correctionsZ
 00002310: 1061 646a 7573 745f 7469 6c65 7368 6170  .adjust_tileshap
 00002320: 6572 2e00 0000 da12 5f67 6574 5f73 6361  er......_get_sca
 00002330: 6c65 5f66 6163 746f 7273 da11 5f73 6361  le_factors.._sca
 00002340: 6c65 5f62 6173 655f 7368 6170 6572 0b00  le_base_shaper..
 00002350: 0000 da03 6c6f 6772 2300 0000 725e 0000  ....logr#...r^..
-00002360: 0072 6800 0000 7214 0000 0072 3800 0000  .rh...r....r8...
+00002360: 0072 6700 0000 7214 0000 0072 3800 0000  .rg...r....r8...
 00002370: 7209 0000 0072 2000 0000 291a 7222 0000  r....r ...).r"..
 00002380: 00da 0475 6466 73da 0764 6174 6173 6574  ...udfs..dataset
-00002390: 7269 0000 0072 6a00 0000 726b 0000 0072  ri...rj...rk...r
+00002390: 7268 0000 0072 6900 0000 726a 0000 0072  rh...ri...rj...r
 000023a0: 5800 0000 5a0c 6d69 6e5f 7369 675f 7369  X...Z.min_sig_si
-000023b0: 7a65 7254 0000 0072 7800 0000 da06 6465  zerT...rx.....de
+000023b0: 7a65 7254 0000 0072 7600 0000 5a06 6465  zerT...rv...Z.de
 000023c0: 7074 6873 722d 0000 0072 1800 0000 da05  pthsr-...r......
-000023d0: 7369 7a65 7372 2c00 0000 7265 0000 0072  sizesr,...re...r
-000023e0: 7400 0000 5a0e 6d69 6e5f 6261 7365 5f73  t...Z.min_base_s
+000023d0: 7369 7a65 7372 2c00 0000 7264 0000 0072  sizesr,...rd...r
+000023e0: 7200 0000 5a0e 6d69 6e5f 6261 7365 5f73  r...Z.min_base_s
 000023f0: 6861 7065 da09 6d61 785f 6465 7074 6872  hape..max_depthr
-00002400: 7700 0000 7273 0000 0072 7600 0000 7216  w...rs...rv...r.
+00002400: 7500 0000 7271 0000 0072 7400 0000 7216  u...rq...rt...r.
 00002410: 0000 005a 0e74 696c 6573 6861 7065 5f6f  ...Z.tileshape_o
 00002420: 7269 67da 0262 7372 5900 0000 7224 0000  rig..bsrY...r$..
-00002430: 0072 7100 0000 7225 0000 00da 0a67 6574  .rq...r%.....get
+00002430: 0072 7000 0000 7225 0000 00da 0a67 6574  .rp...r%.....get
 00002440: 5f73 6368 656d 65da 0000 0073 8a00 0000  _scheme....s....
 00002450: 0025 0c05 0801 0803 1002 1002 0c02 02fe  .%..............
 00002460: 0604 0801 1002 0a02 1204 02fc 0606 0801  ................
 00002470: 0a02 0801 0802 1003 0401 0201 0601 02fd  ................
 00002480: 0607 0401 0201 0201 02fd 0606 0c03 1201  ................
 00002490: 0a01 0402 0c01 0e02 0402 0401 0201 0201  ................
 000024a0: 0201 02fc 0606 0c01 0406 0e01 1201 0e04  ................
@@ -592,17 +592,17 @@
 000024f0: 6563 0500 0000 0000 0000 0000 0000 0600  ec..............
 00002500: 0000 0300 0000 4300 0000 732a 0000 007c  ......C...s*...|
 00002510: 0472 1a7c 01a0 00a1 007d 057c 0564 0075  .r.|.....}.|.d.u
 00002520: 0072 2664 017d 056e 0c7c 0374 017c 0283  .r&d.}.n.|.t.|..
 00002530: 0114 007d 057c 0553 00a9 024e 6900 0010  ...}.|.S...Ni...
 00002540: 0029 02da 0f67 6574 5f6d 6178 5f69 6f5f  .)...get_max_io_
 00002550: 7369 7a65 720b 0000 0029 0672 2200 0000  sizer....).r"...
-00002560: 7283 0000 0072 6a00 0000 7256 0000 0072  r....rj...rV...r
-00002570: 7800 0000 7255 0000 0072 2400 0000 7224  x...rU...r$...r$
-00002580: 0000 0072 2500 0000 7279 0000 0069 0100  ...r%...ry...i..
+00002560: 7280 0000 0072 6900 0000 7256 0000 0072  r....ri...rV...r
+00002570: 7600 0000 7255 0000 0072 2400 0000 7224  v...rU...r$...r$
+00002580: 0000 0072 2500 0000 7277 0000 0069 0100  ...r%...rw...i..
 00002590: 0073 0c00 0000 0001 0401 0801 0801 0602  .s..............
 000025a0: 0c01 7a1b 4e65 676f 7469 6174 6f72 2e5f  ..z.Negotiator._
 000025b0: 6765 745f 696f 5f6d 6178 5f73 697a 6563  get_io_max_sizec
 000025c0: 0500 0000 0000 0000 0000 0000 0c00 0000  ................
 000025d0: 0800 0000 4300 0000 730e 0100 0074 00a0  ....C...s....t..
 000025e0: 0164 017c 017c 027c 037c 04a1 0501 0074  .d.|.|.|.|.....t
 000025f0: 027c 0183 0174 027c 0283 016b 0273 264a  .|...t.|...k.s&J
@@ -643,25 +643,25 @@
 00002820: 2400 0000 7224 0000 0072 2500 0000 725b  $...r$...r%...r[
 00002830: 0000 0080 0100 0073 0400 0000 0402 06ff  .......s........
 00002840: 7a30 4e65 676f 7469 6174 6f72 2e5f 6765  z0Negotiator._ge
 00002850: 745f 7363 616c 655f 6661 6374 6f72 732e  t_scale_factors.
 00002860: 3c6c 6f63 616c 733e 2e3c 6765 6e65 7870  <locals>.<genexp
 00002870: 723e 7a1a 5f67 6574 5f73 6361 6c65 5f66  r>z._get_scale_f
 00002880: 6163 746f 7273 206f 7574 3a20 2572 290d  actors out: %r).
-00002890: 7281 0000 0072 2300 0000 723c 0000 0072  r....r#...r<...r
-000028a0: 3400 0000 722e 0000 0072 5e00 0000 7280  4...r....r^...r.
-000028b0: 0000 0072 0b00 0000 7263 0000 0072 5100  ...r....rc...rQ.
+00002890: 727e 0000 0072 2300 0000 723c 0000 0072  r~...r#...r<...r
+000028a0: 3400 0000 722e 0000 0072 5e00 0000 727d  4...r....r^...r}
+000028b0: 0000 0072 0b00 0000 7262 0000 0072 5100  ...r....rb...rQ.
 000028c0: 0000 da04 6d61 7468 da05 666c 6f6f 7272  ....math..floorr
 000028d0: 5f00 0000 290c 7222 0000 0072 2b00 0000  _...).r"...r+...
-000028e0: 7273 0000 0072 2c00 0000 7274 0000 0072  rs...r,...rt...r
-000028f0: 7600 0000 5a0b 6d61 785f 6661 6374 6f72  v...Z.max_factor
+000028e0: 7271 0000 0072 2c00 0000 7272 0000 0072  rq...r,...rr...r
+000028f0: 7400 0000 5a0b 6d61 785f 6661 6374 6f72  t...Z.max_factor
 00002900: 735a 0c70 7265 6c69 6d5f 7368 6170 65da  sZ.prelim_shape.
 00002910: 0472 6573 7472 3900 0000 5a0a 6d61 785f  .restr9...Z.max_
 00002920: 6661 6374 6f72 da06 6661 6374 6f72 7224  factor..factorr$
-00002930: 0000 0072 2400 0000 7225 0000 0072 7f00  ...r$...r%...r..
+00002930: 0000 0072 2400 0000 7225 0000 0072 7c00  ...r$...r%...r|.
 00002940: 0000 7201 0000 733c 0000 0000 0504 0102  ..r...s<........
 00002950: 0108 fe04 0414 0108 0110 0208 0108 0208  ................
 00002960: fe08 040c 010c 0108 0104 0110 0108 0116  ................
 00002970: 010c 0108 0108 0104 0108 010c 011a 0104  ................
 00002980: 0102 0102 fe04 047a 1d4e 6567 6f74 6961  .......z.Negotia
 00002990: 746f 722e 5f67 6574 5f73 6361 6c65 5f66  tor._get_scale_f
 000029a0: 6163 746f 7273 6303 0000 0000 0000 0000  actorsc.........
@@ -670,28 +670,28 @@
 000029d0: 6b02 7314 4a00 8201 7401 6401 6402 8400  k.s.J...t.d.d...
 000029e0: 7402 7c02 7c01 8302 4400 8301 8301 5300  t.|.|...D.....S.
 000029f0: 2903 4e63 0100 0000 0000 0000 0000 0000  ).Nc............
 00002a00: 0300 0000 0300 0000 7300 0000 731a 0000  ........s...s...
 00002a10: 007c 005d 125c 027d 017d 027c 017c 0214  .|.].\.}.}.|.|..
 00002a20: 0056 0001 0071 0264 0053 0072 3a00 0000  .V...q.d.S.r:...
 00002a30: 7224 0000 0029 0372 3f00 0000 da01 6672  r$...).r?.....fr
-00002a40: 8700 0000 7224 0000 0072 2400 0000 7225  ....r$...r$...r%
+00002a40: 8300 0000 7224 0000 0072 2400 0000 7225  ....r$...r$...r%
 00002a50: 0000 0072 5b00 0000 9a01 0000 7304 0000  ...r[.......s...
 00002a60: 0004 0206 ff7a 2f4e 6567 6f74 6961 746f  .....z/Negotiato
 00002a70: 722e 5f73 6361 6c65 5f62 6173 655f 7368  r._scale_base_sh
 00002a80: 6170 652e 3c6c 6f63 616c 733e 2e3c 6765  ape.<locals>.<ge
 00002a90: 6e65 7870 723e 2903 723c 0000 0072 2e00  nexpr>).r<...r..
 00002aa0: 0000 725e 0000 0029 0372 2200 0000 7257  ..r^...).r"...rW
-00002ab0: 0000 0072 7600 0000 7224 0000 0072 2400  ...rv...r$...r$.
-00002ac0: 0000 7225 0000 0072 8000 0000 9801 0000  ..r%...r........
+00002ab0: 0000 0072 7400 0000 7224 0000 0072 2400  ...rt...r$...r$.
+00002ac0: 0000 7225 0000 0072 7d00 0000 9801 0000  ..r%...r}.......
 00002ad0: 7308 0000 0000 0114 0108 0208 fe7a 1c4e  s............z.N
 00002ae0: 6567 6f74 6961 746f 722e 5f73 6361 6c65  egotiator._scale
 00002af0: 5f62 6173 655f 7368 6170 6563 0100 0000  _base_shapec....
 00002b00: 0000 0000 0000 0000 0100 0000 0100 0000  ................
-00002b10: 4300 0000 7304 0000 0064 0153 0072 8900  C...s....d.S.r..
+00002b10: 4300 0000 7304 0000 0064 0153 0072 8500  C...s....d.S.r..
 00002b20: 0000 7224 0000 0072 3d00 0000 7224 0000  ..r$...r=...r$..
 00002b30: 0072 2400 0000 7225 0000 00da 115f 6765  .r$...r%....._ge
 00002b40: 745f 6465 6661 756c 745f 7369 7a65 9f01  t_default_size..
 00002b50: 0000 7302 0000 0000 027a 1c4e 6567 6f74  ..s......z.Negot
 00002b60: 6961 746f 722e 5f67 6574 5f64 6566 6175  iator._get_defau
 00002b70: 6c74 5f73 697a 6563 0200 0000 0000 0000  lt_sizec........
 00002b80: 0000 0000 0500 0000 0400 0000 4300 0000  ............C...
@@ -700,17 +700,17 @@
 00002bb0: 046a 05a1 027d 047c 047c 026a 0675 0072  .j...}.|.|.j.u.r
 00002bc0: 347c 00a0 07a1 007d 047c 0453 0029 044e  4|.....}.|.S.).N
 00002bd0: 7201 0000 0072 0d00 0000 da0a 746f 7461  r....r......tota
 00002be0: 6c5f 7369 7a65 2908 da0c 6c69 6265 7274  l_size)...libert
 00002bf0: 656d 2e75 6466 720e 0000 00da 1667 6574  em.udfr......get
 00002c00: 5f74 696c 696e 675f 7072 6566 6572 656e  _tiling_preferen
 00002c10: 6365 73da 0367 6574 7248 0000 00da 0369  ces..getrH.....i
-00002c20: 6e66 5a12 5449 4c45 5f53 495a 455f 4245  nfZ.TILE_SIZE_BE
-00002c30: 5354 5f46 4954 7291 0000 0029 0572 2200  ST_FITr....).r".
-00002c40: 0000 726e 0000 0072 0e00 0000 da09 7564  ..rn...r......ud
+00002c20: 6e66 da12 5449 4c45 5f53 495a 455f 4245  nf..TILE_SIZE_BE
+00002c30: 5354 5f46 4954 728d 0000 0029 0572 2200  ST_FITr....).r".
+00002c40: 0000 726d 0000 0072 0e00 0000 da09 7564  ..rm...r......ud
 00002c50: 665f 7072 6566 7372 2c00 0000 7224 0000  f_prefsr,...r$..
 00002c60: 0072 2400 0000 7225 0000 00da 125f 6765  .r$...r%....._ge
 00002c70: 745f 7564 665f 7369 7a65 5f70 7265 66a3  t_udf_size_pref.
 00002c80: 0100 0073 0c00 0000 0001 0c01 0801 0e01  ...s............
 00002c90: 0a01 0801 7a1d 4e65 676f 7469 6174 6f72  ....z.Negotiator
 00002ca0: 2e5f 6765 745f 7564 665f 7369 7a65 5f70  ._get_udf_size_p
 00002cb0: 7265 6672 4400 0000 6302 0000 0000 0000  refrD...c.......
@@ -721,170 +721,170 @@
 00002d00: 7230 6405 7d02 7400 6406 6402 8400 7c01  r0d.}.t.d.d...|.
 00002d10: 4400 8301 8301 7246 6407 7d02 7c02 6400  D.....rFd.}.|.d.
 00002d20: 7501 7352 4a00 8201 7c02 5300 2908 4e63  u.sRJ...|.S.).Nc
 00002d30: 0100 0000 0000 0000 0000 0000 0200 0000  ................
 00002d40: 0300 0000 7300 0000 731a 0000 007c 005d  ....s...s....|.]
 00002d50: 127d 017c 01a0 00a1 0064 006b 0256 0001  .}.|.....d.k.V..
 00002d60: 0071 0264 0153 0029 0272 1300 0000 4ea9  .q.d.S.).r....N.
-00002d70: 01da 0a67 6574 5f6d 6574 686f 6472 6d00  ...get_methodrm.
+00002d70: 01da 0a67 6574 5f6d 6574 686f 6472 6c00  ...get_methodrl.
 00002d80: 0000 7224 0000 0072 2400 0000 7225 0000  ..r$...r$...r%..
 00002d90: 0072 5b00 0000 ad01 0000 7304 0000 0004  .r[.......s.....
 00002da0: 0202 ff7a 294e 6567 6f74 6961 746f 722e  ...z)Negotiator.
 00002db0: 5f67 6574 5f69 6e74 656e 742e 3c6c 6f63  _get_intent.<loc
 00002dc0: 616c 733e 2e3c 6765 6e65 7870 723e 7213  als>.<genexpr>r.
 00002dd0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
 00002de0: 0200 0000 0300 0000 7300 0000 731a 0000  ........s...s...
 00002df0: 007c 005d 127d 017c 01a0 00a1 0064 006b  .|.].}.|.....d.k
 00002e00: 0256 0001 0071 0264 0153 0029 0272 1200  .V...q.d.S.).r..
-00002e10: 0000 4e72 9900 0000 726d 0000 0072 2400  ..Nr....rm...r$.
+00002e10: 0000 4e72 9600 0000 726c 0000 0072 2400  ..Nr....rl...r$.
 00002e20: 0000 7224 0000 0072 2500 0000 725b 0000  ..r$...r%...r[..
 00002e30: 00b2 0100 0073 0400 0000 0402 02ff 7212  .....s........r.
 00002e40: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
 00002e50: 0200 0000 0300 0000 7300 0000 731a 0000  ........s...s...
 00002e60: 007c 005d 127d 017c 01a0 00a1 0064 006b  .|.].}.|.....d.k
 00002e70: 0256 0001 0071 0264 0153 0029 0272 1100  .V...q.d.S.).r..
-00002e80: 0000 4e72 9900 0000 726d 0000 0072 2400  ..Nr....rm...r$.
+00002e80: 0000 4e72 9600 0000 726c 0000 0072 2400  ..Nr....rl...r$.
 00002e90: 0000 7224 0000 0072 2500 0000 725b 0000  ..r$...r%...r[..
 00002ea0: 00b7 0100 0073 0400 0000 0402 02ff 7211  .....s........r.
 00002eb0: 0000 0029 0172 5d00 0000 2903 7222 0000  ...).r]...).r"..
-00002ec0: 0072 8200 0000 7218 0000 0072 2400 0000  .r....r....r$...
-00002ed0: 7224 0000 0072 2500 0000 727b 0000 00ab  r$...r%...r{....
+00002ec0: 0072 7f00 0000 7218 0000 0072 2400 0000  .r....r....r$...
+00002ed0: 7224 0000 0072 2500 0000 7279 0000 00ab  r$...r%...ry....
 00002ee0: 0100 0073 1e00 0000 0001 0401 0802 02fe  ...s............
 00002ef0: 0804 0401 0802 02fe 0804 0401 0802 02fe  ................
 00002f00: 0804 0401 0c01 7a16 4e65 676f 7469 6174  ......z.Negotiat
 00002f10: 6f72 2e5f 6765 745f 696e 7465 6e74 2901  or._get_intent).
-00002f20: 726a 0000 0063 0600 0000 0000 0000 0000  rj...c..........
+00002f20: 7269 0000 0063 0600 0000 0000 0000 0000  ri...c..........
 00002f30: 0000 0b00 0000 0400 0000 4300 0000 7386  ..........C...s.
 00002f40: 0000 007c 02a0 00a1 007d 067c 0374 0174  ...|.....}.|.t.t
 00002f50: 027c 0483 0183 0114 007d 077c 0374 0174  .|.......}.|.t.t
 00002f60: 027c 046a 0383 0183 0114 007d 087c 0664  .|.j.......}.|.d
 00002f70: 016b 0272 4274 047c 00a0 05a1 007c 0883  .k.rBt.|.....|..
 00002f80: 027d 096e 407c 0664 026b 0272 507c 077d  .}.n@|.d.k.rP|.}
 00002f90: 096e 327c 0664 036b 0272 827c 00a0 067c  .n2|.d.k.r.|...|
 00002fa0: 02a1 017d 0974 077c 097c 0183 027d 097c  ...}.t.|.|...}.|
 00002fb0: 0374 017c 0583 0114 007d 0a74 047c 0a7c  .t.|.....}.t.|.|
 00002fc0: 0983 027d 097c 0953 0029 047a 3a0a 2020  ...}.|.S.).z:.  
 00002fd0: 2020 2020 2020 4361 6c63 756c 6174 6520        Calculate 
 00002fe0: 7468 6520 6d61 7869 6d75 6d20 7469 6c65  the maximum tile
 00002ff0: 2073 697a 6520 696e 2062 7974 6573 0a20   size in bytes. 
 00003000: 2020 2020 2020 2072 1200 0000 7211 0000         r....r...
-00003010: 0072 1300 0000 2908 729a 0000 0072 0b00  .r....).r....r..
+00003010: 0072 1300 0000 2908 7297 0000 0072 0b00  .r....).r....r..
 00003020: 0000 722e 0000 0072 2f00 0000 725f 0000  ..r....r/...r_..
-00003030: 0072 9100 0000 7298 0000 0072 7c00 0000  .r....r....r|...
-00003040: 290b 7222 0000 0072 5500 0000 726e 0000  ).r"...rU...rn..
-00003050: 0072 5600 0000 726a 0000 0072 5700 0000  .rV...rj...rW...
+00003030: 0072 8d00 0000 7295 0000 0072 7a00 0000  .r....r....rz...
+00003040: 290b 7222 0000 0072 5500 0000 726d 0000  ).r"...rU...rm..
+00003050: 0072 5600 0000 7269 0000 0072 5700 0000  .rV...ri...rW...
 00003060: da0a 7564 665f 6d65 7468 6f64 7230 0000  ..udf_methodr0..
 00003070: 005a 1270 6172 7469 7469 6f6e 5f73 697a  .Z.partition_siz
 00003080: 655f 7369 6772 2c00 0000 5a09 6261 7365  e_sigr,...Z.base
 00003090: 5f73 697a 6572 2400 0000 7224 0000 0072  _sizer$...r$...r
-000030a0: 2500 0000 7270 0000 00bf 0100 0073 1a00  %...rp.......s..
+000030a0: 2500 0000 726f 0000 00bf 0100 0073 1a00  %...ro.......s..
 000030b0: 0000 0004 0801 1001 1201 0801 1001 0801  ................
 000030c0: 0601 0802 0a03 0a04 0c01 0a01 7a14 4e65  ............z.Ne
 000030d0: 676f 7469 6174 6f72 2e5f 6765 745f 7369  gotiator._get_si
-000030e0: 7a65 720e 0000 0072 0f00 0000 2904 7282  zer....r....).r.
-000030f0: 0000 0072 8300 0000 726a 0000 0072 6b00  ...r....rj...rk.
+000030e0: 7a65 720e 0000 0072 0f00 0000 2904 727f  zer....r....).r.
+000030f0: 0000 0072 8000 0000 7269 0000 0072 6a00  ...r....ri...rj.
 00003100: 0000 6305 0000 0000 0000 0000 0000 0007  ..c.............
 00003110: 0000 0004 0000 0043 0000 0073 4600 0000  .......C...sF...
 00003120: 6401 6402 8400 7c01 4400 8301 7d05 7400  d.d...|.D...}.t.
 00003130: 6403 6404 8400 7c05 4400 8301 8301 7228  d.d...|.D.....r(
 00003140: 7c03 6a01 7d06 6e1a 7402 7c02 6a03 7c04  |.j.}.n.t.|.j.|.
 00003150: 6405 8d01 7c03 6a01 6a04 6406 8d02 6a01  d...|.j.j.d...j.
 00003160: 7d06 7c06 5300 2907 4e63 0100 0000 0000  }.|.S.).Nc......
 00003170: 0000 0000 0000 0200 0000 0400 0000 5300  ..............S.
 00003180: 0000 7314 0000 0067 007c 005d 0c7d 017c  ..s....g.|.].}.|
 00003190: 01a0 00a1 0091 0271 0453 0072 2400 0000  .......q.S.r$...
-000031a0: 7299 0000 0072 6d00 0000 7224 0000 0072  r....rm...r$...r
-000031b0: 2400 0000 7225 0000 0072 6f00 0000 de01  $...r%...ro.....
+000031a0: 7296 0000 0072 6c00 0000 7224 0000 0072  r....rl...r$...r
+000031b0: 2400 0000 7225 0000 0072 6e00 0000 de01  $...r%...rn.....
 000031c0: 0000 7304 0000 0006 0202 ff7a 2e4e 6567  ..s........z.Neg
 000031d0: 6f74 6961 746f 722e 5f67 6574 5f62 6173  otiator._get_bas
 000031e0: 655f 7368 6170 652e 3c6c 6f63 616c 733e  e_shape.<locals>
 000031f0: 2e3c 6c69 7374 636f 6d70 3e63 0100 0000  .<listcomp>c....
 00003200: 0000 0000 0000 0000 0200 0000 0300 0000  ................
 00003210: 7300 0000 731e 0000 007c 005d 167d 017c  s...s....|.].}.|
 00003220: 0164 006b 0270 147c 0164 016b 0256 0001  .d.k.p.|.d.k.V..
 00003230: 0071 0264 0253 0029 0372 1200 0000 7211  .q.d.S.).r....r.
 00003240: 0000 004e 7224 0000 0029 0272 3f00 0000  ...Nr$...).r?...
 00003250: da01 6d72 2400 0000 7224 0000 0072 2500  ..mr$...r$...r%.
 00003260: 0000 725b 0000 00e2 0100 0072 4200 0000  ..r[.......rB...
 00003270: 7a2d 4e65 676f 7469 6174 6f72 2e5f 6765  z-Negotiator._ge
 00003280: 745f 6261 7365 5f73 6861 7065 2e3c 6c6f  t_base_shape.<lo
 00003290: 6361 6c73 3e2e 3c67 656e 6578 7072 3e72  cals>.<genexpr>r
-000032a0: 7500 0000 7228 0000 0029 0572 5d00 0000  u...r(...).r]...
+000032a0: 7300 0000 7228 0000 0029 0572 5d00 0000  s...r(...).r]...
 000032b0: 722f 0000 0072 0900 0000 5a0e 6765 745f  r/...r....Z.get_
 000032c0: 6261 7365 5f73 6861 7065 7220 0000 0029  base_shaper ...)
-000032d0: 0772 2200 0000 7282 0000 0072 8300 0000  .r"...r....r....
-000032e0: 726a 0000 0072 6b00 0000 da07 6d65 7468  rj...rk.....meth
+000032d0: 0772 2200 0000 727f 0000 0072 8000 0000  .r"...r....r....
+000032e0: 7269 0000 0072 6a00 0000 da07 6d65 7468  ri...rj.....meth
 000032f0: 6f64 7372 5700 0000 7224 0000 0072 2400  odsrW...r$...r$.
-00003300: 0000 7225 0000 0072 7a00 0000 d701 0000  ..r%...rz.......
+00003300: 0000 7225 0000 0072 7800 0000 d701 0000  ..r%...rx.......
 00003310: 7314 0000 0000 0706 0202 fe06 0412 0108  s...............
 00003320: 0302 010a 0106 fe08 047a 1a4e 6567 6f74  .........z.Negot
 00003330: 6961 746f 722e 5f67 6574 5f62 6173 655f  iator._get_base_
-00003340: 7368 6170 6529 0372 6e00 0000 726a 0000  shape).rn...rj..
+00003340: 7368 6170 6529 0372 6d00 0000 7269 0000  shape).rm...ri..
 00003350: 0072 2700 0000 6303 0000 0000 0000 0000  .r'...c.........
 00003360: 0000 0006 0000 0004 0000 0043 0000 0073  ...........C...s
 00003370: 4800 0000 6401 6402 6c00 6d01 7d03 0100  H...d.d.l.m.}...
 00003380: 7c01 a002 a100 7d04 7c04 a003 6403 7c03  |.....}.|...d.|.
 00003390: 6a04 a102 7d05 7c05 7c03 6a04 7500 7230  j...}.|.|.j.u.r0
 000033a0: 6404 7d05 7c05 7c02 6401 1900 6b04 7244  d.}.|.|.d...k.rD
 000033b0: 7c02 6401 1900 7d05 7c05 5300 2905 4e72  |.d...}.|.S.).Nr
 000033c0: 0100 0000 720d 0000 0072 2d00 0000 e920  ....r....r-.... 
-000033d0: 0000 0029 0572 9300 0000 720e 0000 0072  ...).r....r....r
-000033e0: 9400 0000 7295 0000 005a 1254 494c 455f  ....r....Z.TILE_
+000033d0: 0000 0029 0572 8f00 0000 720e 0000 0072  ...).r....r....r
+000033e0: 9000 0000 7291 0000 00da 1254 494c 455f  ....r......TILE_
 000033f0: 4445 5054 485f 4445 4641 554c 5429 0672  DEPTH_DEFAULT).r
-00003400: 2200 0000 726e 0000 0072 6a00 0000 720e  "...rn...rj...r.
-00003410: 0000 0072 9700 0000 722d 0000 0072 2400  ...r....r-...r$.
+00003400: 2200 0000 726d 0000 0072 6900 0000 720e  "...rm...ri...r.
+00003410: 0000 0072 9400 0000 722d 0000 0072 2400  ...r....r-...r$.
 00003420: 0000 7224 0000 0072 2500 0000 da13 5f67  ..r$...r%....._g
 00003430: 6574 5f75 6466 5f64 6570 7468 5f70 7265  et_udf_depth_pre
 00003440: 66ec 0100 0073 1000 0000 0001 0c01 0801  f....s..........
 00003450: 0e01 0a01 0401 0c01 0801 7a1e 4e65 676f  ..........z.Nego
 00003460: 7469 6174 6f72 2e5f 6765 745f 7564 665f  tiator._get_udf_
 00003470: 6465 7074 685f 7072 6566 6303 0000 0000  depth_prefc.....
 00003480: 0000 0000 0000 0004 0000 0004 0000 0043  ...............C
 00003490: 0000 0073 3000 0000 7c01 a000 a100 7d03  ...s0...|.....}.
 000034a0: 7c03 6401 6b02 7218 7c02 6402 1900 5300  |.d.k.r.|.d...S.
 000034b0: 7c03 6403 6b02 722c 7c00 a001 7c01 7c02  |.d.k.r,|...|.|.
 000034c0: a102 5300 6404 5300 2905 4e72 1100 0000  ..S.d.S.).Nr....
 000034d0: 7201 0000 0072 1300 0000 7219 0000 0029  r....r....r....)
-000034e0: 0272 9a00 0000 729f 0000 0029 0472 2200  .r....r....).r".
-000034f0: 0000 726e 0000 0072 6a00 0000 729b 0000  ..rn...rj...r...
+000034e0: 0272 9700 0000 729d 0000 0029 0472 2200  .r....r....).r".
+000034f0: 0000 726d 0000 0072 6900 0000 7298 0000  ..rm...ri...r...
 00003500: 0072 2400 0000 7224 0000 0072 2500 0000  .r$...r$...r%...
-00003510: 726c 0000 00f6 0100 0073 0c00 0000 0001  rl.......s......
+00003510: 726b 0000 00f6 0100 0073 0c00 0000 0001  rk.......s......
 00003520: 0802 0801 0801 0801 0c01 7a19 4e65 676f  ..........z.Nego
 00003530: 7469 6174 6f72 2e5f 6765 745f 6d69 6e5f  tiator._get_min_
 00003540: 6465 7074 6829 024e 4e29 014e 291a 724c  depth).NN).N).rL
 00003550: 0000 0072 4d00 0000 724e 0000 00da 075f  ...rM...rN....._
 00003560: 5f64 6f63 5f5f 7205 0000 0072 5100 0000  _doc__r....rQ...
-00003570: 7204 0000 0072 0800 0000 7268 0000 0072  r....r....rh...r
+00003570: 7204 0000 0072 0800 0000 7267 0000 0072  r....r....rg...r
 00003580: 0900 0000 7248 0000 00da 076e 6461 7272  ....rH.....ndarr
-00003590: 6179 7214 0000 0072 8800 0000 7279 0000  ayr....r....ry..
-000035a0: 0072 7f00 0000 7280 0000 0072 9100 0000  .r....r....r....
-000035b0: 7298 0000 0072 4f00 0000 727b 0000 0072  r....rO...r{...r
-000035c0: 7000 0000 7202 0000 0072 7a00 0000 729f  p...r....rz...r.
-000035d0: 0000 0072 6c00 0000 7224 0000 0072 2400  ...rl...r$...r$.
+00003590: 6179 7214 0000 0072 8400 0000 7277 0000  ayr....r....rw..
+000035a0: 0072 7c00 0000 727d 0000 0072 8d00 0000  .r|...r}...r....
+000035b0: 7295 0000 0072 4f00 0000 7279 0000 0072  r....rO...ry...r
+000035c0: 6f00 0000 7202 0000 0072 7800 0000 729d  o...r....rx...r.
+000035d0: 0000 0072 6b00 0000 7224 0000 0072 2400  ...rk...r$...r$.
 000035e0: 0000 7224 0000 0072 2500 0000 7253 0000  ..r$...r%...rS..
 000035f0: 00ab 0000 0073 4200 0000 0801 0409 0a01  .....sB.........
 00003600: 0a01 0201 0201 0201 0a01 06f8 0c2d 0001  .............-..
 00003610: 00f9 0204 0201 0201 0801 0601 02f8 0c7f  ................
 00003620: 0010 0809 0a26 0807 0804 0808 0e14 0e1a  .....&..........
 00003630: 0601 0201 0201 08fb 0c15 120a 7253 0000  ............rS..
-00003640: 0029 2072 8c00 0000 da07 6c6f 6767 696e  .) r......loggin
-00003650: 6772 6100 0000 720c 0000 0072 0200 0000  gra...r....r....
+00003640: 0029 2072 8800 0000 da07 6c6f 6767 696e  .) r......loggin
+00003650: 6772 6000 0000 720c 0000 0072 0200 0000  gr`...r....r....
 00003660: 7203 0000 0072 0400 0000 7205 0000 0072  r....r....r....r
 00003670: 0600 0000 da11 7479 7069 6e67 5f65 7874  ......typing_ext
 00003680: 656e 7369 6f6e 7372 0700 0000 da05 6e75  ensionsr......nu
 00003690: 6d70 7972 4800 0000 da14 6c69 6265 7274  mpyrH.....libert
 000036a0: 656d 2e63 6f72 7265 6374 696f 6e73 7208  em.correctionsr.
-000036b0: 0000 005a 0f6c 6962 6572 7465 6d2e 636f  ...Z.libertem.co
+000036b0: 0000 00da 0f6c 6962 6572 7465 6d2e 636f  .....libertem.co
 000036c0: 6d6d 6f6e 7209 0000 0072 0a00 0000 da14  mmonr....r......
 000036d0: 6c69 6265 7274 656d 2e63 6f6d 6d6f 6e2e  libertem.common.
-000036e0: 6d61 7468 720b 0000 00da 026e 74da 116c  mathr......nt..l
+000036e0: 6d61 7468 720b 0000 00da 026e 745a 116c  mathr......ntZ.l
 000036f0: 6962 6572 7465 6d2e 7564 662e 6261 7365  ibertem.udf.base
 00003700: 720e 0000 00da 186c 6962 6572 7465 6d2e  r......libertem.
 00003710: 696f 2e64 6174 6173 6574 2e62 6173 6572  io.dataset.baser
 00003720: 0f00 0000 7210 0000 00da 0967 6574 4c6f  ....r......getLo
-00003730: 6767 6572 724c 0000 0072 8100 0000 724f  ggerrL...r....rO
+00003730: 6767 6572 724c 0000 0072 7e00 0000 724f  ggerrL...r~...rO
 00003740: 0000 0072 1400 0000 7253 0000 0072 2400  ...r....rS...r$.
 00003750: 0000 7224 0000 0072 2400 0000 7225 0000  ..r$...r$...r%..
 00003760: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
 00003770: 2200 0000 0801 0801 0801 1c01 0c02 0802  "...............
 00003780: 0c01 1001 0c02 0401 0c01 0c01 1002 0a02  ................
 00003790: 1a03 0e7f 0015                           ......
```

### Comparing `libertem-0.9.0/src/libertem/io/dataset/base/__pycache__/utils.cpython-39.pyc` & `libertem-0.9.2/src/libertem/io/dataset/base/__pycache__/utils.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 2232 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 b808 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 b808 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2400 0000 6400  .....@...s$...d.
 00000030: 6401 6c00 5a00 6500 6a01 6402 1900 5a02  d.l.Z.e.j.d...Z.
 00000040: 4700 6403 6404 8400 6404 8302 5a03 6401  G.d.d...d...Z.d.
 00000050: 5300 2905 e900 0000 004e 2902 4eda 0846  S.)......N).N..F
 00000060: 696c 6554 7265 6563 0000 0000 0000 0000  ileTreec........
 00000070: 0000 0000 0000 0000 0700 0000 4000 0000  ............@...
```

### Comparing `libertem-0.9.0/src/libertem/io/dataset/base/backend.py` & `libertem-0.9.2/src/libertem/io/dataset/base/backend.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/io/dataset/base/backend_buffered.py` & `libertem-0.9.2/src/libertem/io/dataset/base/backend_buffered.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/io/dataset/base/backend_direct.py` & `libertem-0.9.2/src/libertem/io/dataset/base/backend_direct.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/io/dataset/base/backend_mmap.py` & `libertem-0.9.2/src/libertem/io/dataset/base/backend_mmap.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/io/dataset/base/coordinates.py` & `libertem-0.9.2/src/libertem/io/dataset/base/coordinates.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/io/dataset/base/dataset.py` & `libertem-0.9.2/src/libertem/io/dataset/base/dataset.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/io/dataset/base/decode.py` & `libertem-0.9.2/src/libertem/io/dataset/base/decode.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/io/dataset/base/file.py` & `libertem-0.9.2/src/libertem/io/dataset/base/file.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/io/dataset/base/fileset.py` & `libertem-0.9.2/src/libertem/io/dataset/base/fileset.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/io/dataset/base/meta.py` & `libertem-0.9.2/src/libertem/io/dataset/base/meta.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/io/dataset/base/partition.py` & `libertem-0.9.2/src/libertem/io/dataset/base/partition.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/io/dataset/base/roi.py` & `libertem-0.9.2/src/libertem/io/dataset/base/roi.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/io/dataset/base/tiling.py` & `libertem-0.9.2/src/libertem/io/dataset/base/tiling.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/io/dataset/base/tiling_scheme.py` & `libertem-0.9.2/src/libertem/io/dataset/base/tiling_scheme.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/io/dataset/base/utils.py` & `libertem-0.9.2/src/libertem/io/dataset/base/utils.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/io/dataset/blo.py` & `libertem-0.9.2/src/libertem/io/dataset/blo.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/io/dataset/cached.py` & `libertem-0.9.2/src/libertem/io/dataset/cached.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/io/dataset/cluster.py` & `libertem-0.9.2/src/libertem/io/dataset/cluster.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/io/dataset/dask.py` & `libertem-0.9.2/src/libertem/io/dataset/dask.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/io/dataset/dm.py` & `libertem-0.9.2/src/libertem/io/dataset/dm.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/io/dataset/empad.py` & `libertem-0.9.2/src/libertem/io/dataset/empad.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/io/dataset/frms6.py` & `libertem-0.9.2/src/libertem/io/dataset/frms6.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/io/dataset/hdf5.py` & `libertem-0.9.2/src/libertem/io/dataset/hdf5.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/io/dataset/k2is.py` & `libertem-0.9.2/src/libertem/io/dataset/k2is.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/io/dataset/memory.py` & `libertem-0.9.2/src/libertem/io/dataset/memory.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/io/dataset/mib.py` & `libertem-0.9.2/src/libertem/io/dataset/mib.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/io/dataset/mrc.py` & `libertem-0.9.2/src/libertem/io/dataset/mrc.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/io/dataset/raw.py` & `libertem-0.9.2/src/libertem/io/dataset/raw.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/io/dataset/seq.py` & `libertem-0.9.2/src/libertem/io/dataset/seq.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/io/dataset/ser.py` & `libertem-0.9.2/src/libertem/io/dataset/ser.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/io/dataset/tvips.py` & `libertem-0.9.2/src/libertem/io/dataset/tvips.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/io/fs.py` & `libertem-0.9.2/src/libertem/io/fs.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/io/utils.py` & `libertem-0.9.2/src/libertem/io/utils.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/io/writers/__pycache__/base.cpython-39.pyc` & `libertem-0.9.2/src/libertem/io/writers/__pycache__/base.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 4264 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 a810 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 a810 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a04 4700  d.l.Z.d.d.l.Z.G.
 00000050: 6402 6403 8400 6403 8302 5a05 6401 5300  d.d...d...Z.d.S.
 00000060: 2904 e900 0000 004e 6300 0000 0000 0000  )......Nc.......
 00000070: 0000 0000 0000 0000 0002 0000 0040 0000  .............@..
```

### Comparing `libertem-0.9.0/src/libertem/io/writers/base.py` & `libertem-0.9.2/src/libertem/io/writers/base.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/io/writers/results/__pycache__/base.cpython-39.pyc` & `libertem-0.9.2/src/libertem/io/writers/results/__pycache__/base.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 1801 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 0907 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 0907 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 4700 6403 6404  d.l.m.Z...G.d.d.
 00000050: 8400 6404 6505 8303 5a06 4700 6405 6406  ..d.e...Z.G.d.d.
 00000060: 8400 6406 6506 6407 8d03 5a07 6408 5300  ..d.e.d...Z.d.S.
 00000070: 2909 e900 0000 0029 02da 0454 7970 65da  )......)...Type.
```

### Comparing `libertem-0.9.0/src/libertem/io/writers/results/__pycache__/formats.cpython-39.pyc` & `libertem-0.9.2/src/libertem/io/writers/results/__pycache__/formats.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 2996 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 b40b 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 b40b 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7c00 0000 6400  .....@...s|...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 0100 6403 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 4700 6405 6406 8400 6406  m.Z...G.d.d...d.
 00000060: 6506 8303 5a07 4700 6407 6408 8400 6408  e...Z.G.d.d...d.
 00000070: 6506 8303 5a08 4700 6409 640a 8400 640a  e...Z.G.d.d...d.
```

### Comparing `libertem-0.9.0/src/libertem/io/writers/results/base.py` & `libertem-0.9.2/src/libertem/io/writers/results/base.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/io/writers/results/formats.py` & `libertem-0.9.2/src/libertem/io/writers/results/formats.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/masks.py` & `libertem-0.9.2/src/libertem/masks.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/preload.py` & `libertem-0.9.2/src/libertem/preload.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/udf/FEM.py` & `libertem-0.9.2/src/libertem/udf/FEM.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/udf/__pycache__/FEM.cpython-39.pyc` & `libertem-0.9.2/src/libertem/udf/__pycache__/FEM.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 2696 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 880a 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 880a 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3e00 0000 6400  .....@...s>...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c04 6d05 5a05 0100 4700  ..d.d.l.m.Z...G.
 00000050: 6404 6405 8400 6405 6505 8303 5a06 6408  d.d...d.e...Z.d.
 00000060: 6406 6407 8401 5a07 6401 5300 2909 e900  d.d...Z.d.S.)...
 00000070: 0000 004e 2901 da13 5f6d 616b 655f 6369  ...N)..._make_ci
```

### Comparing `libertem-0.9.0/src/libertem/udf/__pycache__/auto.cpython-39.pyc` & `libertem-0.9.2/src/libertem/udf/__pycache__/auto.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 1826 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 2207 0000  a.......z..b"...
+00000000: 610d 0d0a 0000 0000 7fce 6762 2207 0000  a.........gb"...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 0100 6500 a005 6506  d.l.m.Z...e...e.
 00000050: a101 5a07 4700 6403 6404 8400 6404 6504  ..Z.G.d.d...d.e.
 00000060: 8303 5a08 6401 5300 2905 e900 0000 004e  ..Z.d.S.)......N
 00000070: 2901 da03 5544 4663 0000 0000 0000 0000  )...UDFc........
```

### Comparing `libertem-0.9.0/src/libertem/udf/__pycache__/base.cpython-39.pyc` & `libertem-0.9.2/src/libertem/udf/__pycache__/base.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 74248 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 0822 0100  a.......z..b."..
+00000000: 610d 0d0a 0000 0000 7fce 6762 0822 0100  a.........gb."..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 9403 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0e 5a0e 6d0f 5a0f 6d10 5a10 6d11 5a11  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `libertem-0.9.0/src/libertem/udf/__pycache__/crystallinity.cpython-39.pyc` & `libertem-0.9.2/src/libertem/udf/__pycache__/crystallinity.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 4268 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 ac10 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 ac10 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3e00 0000 6400  .....@...s>...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c04 6d05 5a05 0100 4700  ..d.d.l.m.Z...G.
 00000050: 6404 6405 8400 6405 6505 8303 5a06 6409  d.d...d.e...Z.d.
 00000060: 6407 6408 8401 5a07 6401 5300 290a e900  d.d...Z.d.S.)...
 00000070: 0000 004e 2901 da13 5f6d 616b 655f 6369  ...N)..._make_ci
```

### Comparing `libertem-0.9.0/src/libertem/udf/__pycache__/holography.cpython-39.pyc` & `libertem-0.9.2/src/libertem/udf/__pycache__/holography.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 7396 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 e41c 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 e41c 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c04 6d05 5a05 0100 640b  ..d.d.l.m.Z...d.
 00000050: 6405 6406 8401 5a06 6407 6408 8400 5a07  d.d...Z.d.d...Z.
 00000060: 4700 6409 640a 8400 640a 6505 8303 5a08  G.d.d...d.e...Z.
 00000070: 6401 5300 290c e900 0000 004e 2901 da04  d.S.)......N)...
```

### Comparing `libertem-0.9.0/src/libertem/udf/__pycache__/logsum.cpython-39.pyc` & `libertem-0.9.2/src/libertem/udf/__pycache__/logsum.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 1619 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 5306 0000  a.......z..bS...
+00000000: 610d 0d0a 0000 0000 7fce 6762 5306 0000  a.........gbS...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 0100 4700 6403 6404 8400 6404 6503 8303  ..G.d.d...d.e...
 00000050: 5a04 6407 6405 6406 8401 5a05 6401 5300  Z.d.d.d...Z.d.S.
 00000060: 2908 e900 0000 004e 2901 da03 5544 4663  )......N)...UDFc
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `libertem-0.9.0/src/libertem/udf/__pycache__/masks.cpython-39.pyc` & `libertem-0.9.2/src/libertem/udf/__pycache__/masks.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 7952 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 101f 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 101f 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 4700 6405 6406  d.l.m.Z...G.d.d.
 00000060: 8400 6406 6503 8303 5a08 6401 5300 2907  ..d.e...Z.d.S.).
 00000070: e900 0000 004e 2901 da03 5544 4629 01da  .....N)...UDF)..
```

### Comparing `libertem-0.9.0/src/libertem/udf/__pycache__/raw.cpython-39.pyc` & `libertem-0.9.2/src/libertem/udf/__pycache__/raw.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 2281 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 e908 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 e908 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6500 a007 6508 a101 5a09  m.Z...e...e...Z.
 00000060: 4700 6404 6405 8400 6405 6506 8303 5a0a  G.d.d...d.e...Z.
 00000070: 6401 5300 2906 e900 0000 004e 2901 da04  d.S.)......N)...
```

### Comparing `libertem-0.9.0/src/libertem/udf/__pycache__/stddev.cpython-39.pyc` & `libertem-0.9.2/src/libertem/udf/__pycache__/stddev.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 14913 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 413a 0000  a.......z..bA:..
+00000000: 610d 0d0a 0000 0000 7fce 6762 413a 0000  a.........gbA:..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 a400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a03 6400 6402 6c04 5a04 6400 6403 6c05  Z.d.d.l.Z.d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6504 6a09 6405 6405 6405 6406 8d03  ..e.j.d.d.d.d...
 00000070: 6407 6408 8400 8301 5a0a 6504 6a09 6405  d.d.....Z.e.j.d.
```

### Comparing `libertem-0.9.0/src/libertem/udf/__pycache__/sum.cpython-39.pyc` & `libertem-0.9.2/src/libertem/udf/__pycache__/sum.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 1316 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 2405 0000  a.......z..b$...
+00000000: 610d 0d0a 0000 0000 7fce 6762 2405 0000  a.........gb$...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2800 0000 6400  .....@...s(...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 0100 4700 6403 6404 8400 6404 6503 8303  ..G.d.d...d.e...
 00000050: 5a04 6401 5300 2905 e900 0000 004e 2901  Z.d.S.)......N).
 00000060: da03 5544 4663 0000 0000 0000 0000 0000  ..UDFc..........
 00000070: 0000 0000 0000 0400 0000 0000 0000 734a  ..............sJ
```

### Comparing `libertem-0.9.0/src/libertem/udf/__pycache__/sumsigudf.cpython-39.pyc` & `libertem-0.9.2/src/libertem/udf/__pycache__/sumsigudf.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 791 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 1703 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 1703 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3000 0000 6400  .....@...s0...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 0100 4700 6403 6404 8400 6404 6503 8303  ..G.d.d...d.e...
 00000050: 5a04 6405 6406 8400 5a05 6401 5300 2907  Z.d.d...Z.d.S.).
 00000060: e900 0000 004e 2901 da03 5544 4663 0000  .....N)...UDFc..
 00000070: 0000 0000 0000 0000 0000 0000 0000 0200  ................
```

### Comparing `libertem-0.9.0/src/libertem/udf/auto.py` & `libertem-0.9.2/src/libertem/udf/auto.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/udf/base.py` & `libertem-0.9.2/src/libertem/udf/base.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/udf/crystallinity.py` & `libertem-0.9.2/src/libertem/udf/crystallinity.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/udf/holography.py` & `libertem-0.9.2/src/libertem/udf/holography.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/udf/logsum.py` & `libertem-0.9.2/src/libertem/udf/logsum.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/udf/masks.py` & `libertem-0.9.2/src/libertem/udf/masks.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/udf/raw.py` & `libertem-0.9.2/src/libertem/udf/raw.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/udf/stddev.py` & `libertem-0.9.2/src/libertem/udf/stddev.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/udf/sum.py` & `libertem-0.9.2/src/libertem/udf/sum.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/udf/sumsigudf.py` & `libertem-0.9.2/src/libertem/udf/sumsigudf.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/utils/__init__.py` & `libertem-0.9.2/src/libertem/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/utils/__pycache__/__init__.cpython-39.pyc` & `libertem-0.9.2/src/libertem/utils/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 4665 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 3912 0000  a.......z..b9...
+00000000: 610d 0d0a 0000 0000 7fce 6762 3912 0000  a.........gb9...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 6401 6c00 5a01 6402 6403 8400 5a02 6404  d.l.Z.d.d...Z.d.
 00000040: 6405 8400 5a03 6406 6407 8400 5a04 6408  d...Z.d.d...Z.d.
 00000050: 6409 8400 5a05 640a 640b 8400 5a06 640c  d...Z.d.d...Z.d.
 00000060: 640d 8400 5a07 640e 640f 8400 5a08 6410  d...Z.d.d...Z.d.
 00000070: 6411 8400 5a09 6412 6413 8400 5a0a 6401  d...Z.d.d...Z.d.
@@ -59,23 +59,23 @@
 000003a0: 7465 7369 616e 2076 6563 746f 7273 0a0a  tesian vectors..
 000003b0: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
 000003c0: 2d2d 2d2d 2d2d 2d0a 0a20 2020 2050 6f6c  -------..    Pol
 000003d0: 6172 2076 6563 746f 7220 6173 206e 756d  ar vector as num
 000003e0: 7079 2e6e 6461 7272 6179 206f 6620 7475  py.ndarray of tu
 000003f0: 706c 6573 205b 2872 312c 2070 6869 3129  ples [(r1, phi1)
 00000400: 2c20 2872 322c 2070 6869 3229 2c20 2e2e  , (r2, phi2), ..
-00000410: 2e5d 0a20 2020 20e9 ffff ffff a901 5a04  .].    .......Z.
+00000410: 2e5d 0a20 2020 20e9 ffff ffff a901 da04  .].    .........
 00000420: 6178 6973 7204 0000 0072 0200 0000 2906  axisr....r....).
-00000430: 7205 0000 005a 066c 696e 616c 67da 046e  r....Z.linalg..n
+00000430: 7205 0000 00da 066c 696e 616c 67da 046e  r......linalg..n
 00000440: 6f72 6dda 0761 7263 7461 6e32 7208 0000  orm..arctan2r...
 00000450: 0072 0900 0000 2903 5a09 6361 7274 6573  .r....).Z.cartes
 00000460: 6961 6eda 0264 73da 0661 6c70 6861 7372  ian..ds..alphasr
 00000470: 0c00 0000 720c 0000 0072 0d00 0000 da0a  ....r....r......
 00000480: 6d61 6b65 5f70 6f6c 6172 1b00 0000 7306  make_polar....s.
-00000490: 0000 0000 0e10 0214 0172 1500 0000 6304  .........r....c.
+00000490: 0000 0000 0e10 0214 0172 1700 0000 6304  .........r....c.
 000004a0: 0000 0000 0000 0000 0000 0006 0000 0003  ................
 000004b0: 0000 0043 0000 0073 2800 0000 7c02 7c01  ...C...s(...|.|.
 000004c0: 1400 7c03 7c00 1400 1800 7d04 7c03 7c01  ..|.|.....}.|.|.
 000004d0: 1400 7c02 7c00 1400 1700 7d05 7c05 7c04  ..|.|.....}.|.|.
 000004e0: 6602 5300 2901 611c 0300 000a 2020 2020  f.S.).a.....    
 000004f0: 526f 7461 7465 2077 6974 6820 7072 652d  Rotate with pre-
 00000500: 6361 6c63 756c 6174 6564 2065 6e74 7269  calculated entri
@@ -128,15 +128,15 @@
 000007f0: 7273 696f 6e61 6464 6564 3a3a 2030 2e36  rsionadded:: 0.6
 00000800: 2e30 0a20 2020 2072 0c00 0000 2906 da01  .0.    r....)...
 00000810: 79da 0178 da09 636f 735f 616e 676c 65da  y..x..cos_angle.
 00000820: 0973 696e 5f61 6e67 6c65 5a03 725f 785a  .sin_angleZ.r_xZ
 00000830: 0372 5f79 720c 0000 0072 0c00 0000 720d  .r_yr....r....r.
 00000840: 0000 00da 0e72 6f74 6174 655f 7072 6563  .....rotate_prec
 00000850: 616c 632f 0000 0073 0600 0000 001b 1001  alc/...s........
-00000860: 1001 721a 0000 0063 0300 0000 0000 0000  ..r....c........
+00000860: 1001 721c 0000 0063 0300 0000 0000 0000  ..r....c........
 00000870: 0000 0000 0300 0000 0500 0000 4300 0000  ............C...
 00000880: 7316 0000 0074 007c 007c 0174 016a 0264  s....t.|.|.t.j.d
 00000890: 011b 007c 0214 0083 0353 0029 0261 5e02  ...|.....S.).a^.
 000008a0: 0000 0a20 2020 2052 6f74 6174 6520 6279  ...    Rotate by
 000008b0: 2061 6e67 6c65 2069 6e20 6465 6772 6565   angle in degree
 000008c0: 730a 0a20 2020 2054 6865 2072 6f74 6174  s..    The rotat
 000008d0: 696f 6e20 666f 6c6c 6f77 7320 6874 7470  ion follows http
@@ -171,19 +171,19 @@
 00000aa0: 206e 756d 7079 2e6e 6461 7272 6179 0a20   numpy.ndarray. 
 00000ab0: 2020 2020 2020 2059 2061 6e64 2058 2063         Y and X c
 00000ac0: 6f6d 706f 6e65 6e74 7320 6f66 2072 6f74  omponents of rot
 00000ad0: 6174 6564 2076 6563 746f 7228 7329 0a0a  ated vector(s)..
 00000ae0: 2020 2020 2e2e 2076 6572 7369 6f6e 6164      .. versionad
 00000af0: 6465 643a 3a20 302e 362e 300a 2020 2020  ded:: 0.6.0.    
 00000b00: e9b4 0000 0029 03da 0a72 6f74 6174 655f  .....)...rotate_
-00000b10: 7261 6472 0500 0000 da02 7069 2903 7216  radr......pi).r.
-00000b20: 0000 0072 1700 0000 da07 6465 6772 6565  ...r......degree
+00000b10: 7261 6472 0500 0000 da02 7069 2903 7218  radr......pi).r.
+00000b20: 0000 0072 1900 0000 da07 6465 6772 6565  ...r......degree
 00000b30: 7372 0c00 0000 720c 0000 0072 0d00 0000  sr....r....r....
 00000b40: da0a 726f 7461 7465 5f64 6567 4f00 0000  ..rotate_degO...
-00000b50: 7302 0000 0000 1972 1f00 0000 6303 0000  s......r....c...
+00000b50: 7302 0000 0000 1972 2100 0000 6303 0000  s......r!...c...
 00000b60: 0000 0000 0000 0000 0003 0000 0007 0000  ................
 00000b70: 0043 0000 0073 1c00 0000 7400 7c00 7c01  .C...s....t.|.|.
 00000b80: 7401 a002 7c02 a101 7401 a003 7c02 a101  t...|...t...|...
 00000b90: 6401 8d04 5300 2902 615e 0200 000a 2020  d...S.).a^....  
 00000ba0: 2020 526f 7461 7465 2062 7920 616e 676c    Rotate by angl
 00000bb0: 6520 696e 2072 6164 6961 6e73 0a0a 2020  e in radians..  
 00000bc0: 2020 5468 6520 726f 7461 7469 6f6e 2066    The rotation f
@@ -217,21 +217,21 @@
 00000d80: 3d3d 3d3d 3d3d 3d0a 2020 2020 792c 2078  =======.    y, x
 00000d90: 203a 2066 6c6f 6174 206f 7220 6e75 6d70   : float or nump
 00000da0: 792e 6e64 6172 7261 790a 2020 2020 2020  y.ndarray.      
 00000db0: 2020 5920 616e 6420 5820 636f 6d70 6f6e    Y and X compon
 00000dc0: 656e 7473 206f 6620 726f 7461 7465 6420  ents of rotated 
 00000dd0: 7665 6374 6f72 2873 290a 0a20 2020 202e  vector(s)..    .
 00000de0: 2e20 7665 7273 696f 6e61 6464 6564 3a3a  . versionadded::
-00000df0: 2030 2e36 2e30 0a20 2020 2029 0272 1800   0.6.0.    ).r..
-00000e00: 0000 7219 0000 0029 0472 1a00 0000 7205  ..r....).r....r.
+00000df0: 2030 2e36 2e30 0a20 2020 2029 0272 1a00   0.6.0.    ).r..
+00000e00: 0000 721b 0000 0029 0472 1c00 0000 7205  ..r....).r....r.
 00000e10: 0000 0072 0600 0000 7207 0000 0029 0372  ...r....r....).r
-00000e20: 1600 0000 7217 0000 00da 0772 6164 6961  ....r......radia
+00000e20: 1800 0000 7219 0000 00da 0772 6164 6961  ....r......radia
 00000e30: 6e73 720c 0000 0072 0c00 0000 720d 0000  nsr....r....r...
-00000e40: 0072 1c00 0000 6b00 0000 7302 0000 0000  .r....k...s.....
-00000e50: 1972 1c00 0000 6301 0000 0000 0000 0000  .r....c.........
+00000e40: 0072 1e00 0000 6b00 0000 7302 0000 0000  .r....k...s.....
+00000e50: 1972 1e00 0000 6301 0000 0000 0000 0000  .r....c.........
 00000e60: 0000 0003 0000 0004 0000 0043 0000 0073  ...........C...s
 00000e70: 6000 0000 7c00 6a00 7d01 7401 7c01 8301  `...|.j.}.t.|...
 00000e80: 6401 6b02 722c 7c01 6402 1900 6403 6b02  d.k.r,|.d...d.k.
 00000e90: 722c 7402 a003 7c00 6a04 a101 7d02 6e30  r,t...|.j...}.n0
 00000ea0: 7401 7c01 8301 6403 6b02 724a 7c01 6404  t.|...d.k.rJ|.d.
 00000eb0: 1900 6403 6b02 724a 7c00 7d02 6e12 7405  ..d.k.rJ|.}.n.t.
 00000ec0: 6405 7406 7c00 6a00 8301 1600 8301 8201  d.t.|.j.........
@@ -244,59 +244,59 @@
 00000f30: 0500 0000 da0b 636f 6e63 6174 656e 6174  ......concatenat
 00000f40: 6572 0900 0000 da0a 5661 6c75 6545 7272  er......ValueErr
 00000f50: 6f72 da03 7374 7229 03da 0769 6e64 6963  or..str)...indic
 00000f60: 6573 da01 73da 0672 6573 756c 7472 0c00  es..s..resultr..
 00000f70: 0000 720c 0000 0072 0d00 0000 da12 7265  ..r....r......re
 00000f80: 6775 6c61 7269 7a65 5f69 6e64 6963 6573  gularize_indices
 00000f90: 8700 0000 7312 0000 0000 0106 0218 010e  ....s...........
-00000fa0: 0218 0106 0202 010c ff04 0272 2b00 0000  ...........r+...
+00000fa0: 0218 0106 0202 010c ff04 0272 2d00 0000  ...........r-...
 00000fb0: 6307 0000 0000 0000 0000 0000 0009 0000  c...............
 00000fc0: 0005 0000 0043 0000 0073 3400 0000 7400  .....C...s4...t.
 00000fd0: 7c06 8301 7d06 7401 7c02 7c03 7c04 7c06  |...}.t.|.|.|.|.
 00000fe0: 8304 7d07 7402 7c07 7c05 7c00 7c01 8304  ..}.t.|.|.|.|...
 00000ff0: 7d08 7c06 7c08 1900 7c07 7c08 1900 6602  }.|.|...|.|...f.
-00001000: 5300 2901 4e29 0372 2b00 0000 da0b 6361  S.).N).r+.....ca
+00001000: 5300 2901 4e29 0372 2d00 0000 da0b 6361  S.).N).r-.....ca
 00001010: 6c63 5f63 6f6f 7264 73da 0c77 6974 6869  lc_coords..withi
 00001020: 6e5f 6672 616d 6529 09da 0266 79da 0266  n_frame)...fy..f
 00001030: 78da 047a 6572 6fda 0161 da01 62da 0172  x..zero..a..b..r
-00001040: 7228 0000 00da 0570 6561 6b73 da08 7365  r(.....peaks..se
+00001040: 722a 0000 00da 0570 6561 6b73 da08 7365  r*.....peaks..se
 00001050: 6c65 6374 6f72 720c 0000 0072 0c00 0000  lectorr....r....
 00001060: 720d 0000 00da 0b66 7261 6d65 5f70 6561  r......frame_pea
 00001070: 6b73 9500 0000 7308 0000 0000 0108 010e  ks....s.........
-00001080: 010e 0172 3600 0000 6304 0000 0000 0000  ...r6...c.......
+00001080: 010e 0172 3800 0000 6304 0000 0000 0000  ...r8...c.......
 00001090: 0000 0000 0005 0000 0005 0000 0043 0000  .............C..
 000010a0: 0073 1e00 0000 7400 a001 7c01 7c02 6602  .s....t...|.|.f.
 000010b0: a101 7d04 7c00 7400 a002 7c03 7c04 a102  ..}.|.t...|.|...
 000010c0: 1700 5300 2901 7a45 0a20 2020 2043 616c  ..S.).zE.    Cal
 000010d0: 6375 6c61 7465 2063 6f6f 7264 696e 6174  culate coordinat
 000010e0: 6573 2066 726f 6d20 6c61 7474 6963 6520  es from lattice 
 000010f0: 7665 6374 6f72 7320 612c 2062 2061 6e64  vectors a, b and
 00001100: 2069 6e64 6963 6573 0a20 2020 2029 0372   indices.    ).r
 00001110: 0500 0000 7208 0000 00da 0364 6f74 2905  ....r......dot).
-00001120: 7230 0000 0072 3100 0000 7232 0000 0072  r0...r1...r2...r
-00001130: 2800 0000 5a0c 636f 6566 6669 6369 656e  (...Z.coefficien
+00001120: 7232 0000 0072 3300 0000 7234 0000 0072  r2...r3...r4...r
+00001130: 2a00 0000 da0c 636f 6566 6669 6369 656e  *.....coefficien
 00001140: 7473 720c 0000 0072 0c00 0000 720d 0000  tsr....r....r...
-00001150: 0072 2c00 0000 9c00 0000 7304 0000 0000  .r,.......s.....
-00001160: 040e 0172 2c00 0000 6304 0000 0000 0000  ...r,...c.......
+00001150: 0072 2e00 0000 9c00 0000 7304 0000 0000  .r........s.....
+00001160: 040e 0172 2e00 0000 6304 0000 0000 0000  ...r....c.......
 00001170: 0000 0000 0005 0000 0005 0000 0043 0000  .............C..
 00001180: 0073 2c00 0000 7c00 7c01 7c01 6602 6b05  .s,...|.|.|.f.k.
 00001190: 7c00 7c02 7c01 1800 7c03 7c01 1800 6602  |.|.|...|.|...f.
 000011a0: 6b00 1400 7d04 7c04 6a00 6401 6402 8d01  k...}.|.j.d.d...
 000011b0: 5300 2903 7a5e 0a20 2020 2052 6574 7572  S.).z^.    Retur
 000011c0: 6e20 6120 626f 6f6c 6561 6e20 7665 6374  n a boolean vect
 000011d0: 6f72 2069 6e64 6963 6174 696e 6720 7065  or indicating pe
 000011e0: 616b 7320 7468 6174 2061 7265 2077 6974  aks that are wit
 000011f0: 6869 6e20 2872 2c20 7229 2061 6e64 2028  hin (r, r) and (
 00001200: 6679 202d 2072 2c20 6678 202d 2072 290a  fy - r, fx - r).
 00001210: 2020 2020 720f 0000 0072 1000 0000 2901      r....r....).
-00001220: da03 616c 6c29 0572 3400 0000 7233 0000  ..all).r4...r3..
-00001230: 0072 2e00 0000 722f 0000 0072 3500 0000  .r....r/...r5...
+00001220: da03 616c 6c29 0572 3600 0000 7235 0000  ..all).r6...r5..
+00001230: 0072 3000 0000 7231 0000 0072 3700 0000  .r0...r1...r7...
 00001240: 720c 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
-00001250: 2d00 0000 a400 0000 7304 0000 0000 0420  -.......s...... 
-00001260: 0172 2d00 0000 290b da05 6e75 6d70 7972  .r-...)...numpyr
-00001270: 0500 0000 720e 0000 0072 1500 0000 721a  ....r....r....r.
-00001280: 0000 0072 1f00 0000 721c 0000 0072 2b00  ...r....r....r+.
-00001290: 0000 7236 0000 0072 2c00 0000 722d 0000  ..r6...r,...r-..
+00001250: 2f00 0000 a400 0000 7304 0000 0000 0420  /.......s...... 
+00001260: 0172 2f00 0000 290b da05 6e75 6d70 7972  .r/...)...numpyr
+00001270: 0500 0000 720e 0000 0072 1700 0000 721c  ....r....r....r.
+00001280: 0000 0072 2100 0000 721e 0000 0072 2d00  ...r!...r....r-.
+00001290: 0000 7238 0000 0072 2e00 0000 722f 0000  ..r8...r....r/..
 000012a0: 0072 0c00 0000 720c 0000 0072 0c00 0000  .r....r....r....
 000012b0: 720d 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
 000012c0: 0000 0073 1200 0000 0808 0812 0814 0820  ...s........... 
 000012d0: 081c 081c 080e 0807 0808                 ..........
```

### Comparing `libertem-0.9.0/src/libertem/utils/__pycache__/async_utils.cpython-39.pyc` & `libertem-0.9.2/src/libertem/utils/__pycache__/async_utils.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 8361 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 a920 0000  a.......z..b. ..
+00000000: 610d 0d0a 0000 0000 7fce 6762 a920 0000  a.........gb. ..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 2801 0000 6400  .....@...s(...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c04 6d05 5a05 6d06 5a06 6d07 5a07  d.l.m.Z.m.Z.m.Z.
 00000060: 6d08 5a08 6d09 5a09 0100 6400 6403 6c0a  m.Z.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6509 6404 8301 5a0c 4700  m.Z...e.d...Z.G.
```

### Comparing `libertem-0.9.0/src/libertem/utils/__pycache__/devices.cpython-39.pyc` & `libertem-0.9.2/src/libertem/utils/__pycache__/devices.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 1682 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 9206 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 9206 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000a 0000 0040 0000 0073 9800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a04 6501  d.l.Z.d.d.l.Z.e.
 00000050: a005 6506 a101 5a07 7a0c 6400 6401 6c08  ..e...Z.z.d.d.l.
 00000060: 5a08 5700 6e4c 0400 6509 794c 0100 0100  Z.W.nL..e.yL....
 00000070: 0100 6401 5a08 5900 6e38 0400 650a 7982  ..d.Z.Y.n8..e.y.
```

### Comparing `libertem-0.9.0/src/libertem/utils/__pycache__/generate.cpython-39.pyc` & `libertem-0.9.2/src/libertem/utils/__pycache__/generate.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 5171 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 3314 0000  a.......z..b3...
+00000000: 610d 0d0a 0000 0000 7fce 6762 3314 0000  a.........gb3...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 6d08 5a08 6d09 5a09  d.l.m.Z.m.Z.m.Z.
 00000060: 0100 6400 6401 6c0a 6d0b 5a0c 0100 6414  ..d.d.l.m.Z...d.
 00000070: 6408 6409 8401 5a0d 6415 640e 640f 8401  d.d...Z.d.d.d...
@@ -50,27 +50,27 @@
 00000310: 00da 0270 69da 056d 6772 6964 7206 0000  ...pi..mgridr...
 00000320: 00da 057a 6572 6f73 da07 666c 6f61 7433  ...zeros..float3
 00000330: 32da 066c 696e 616c 67da 046e 6f72 6dda  2..linalg..norm.
 00000340: 036d 6178 da03 6c65 6eda 0965 6e75 6d65  .max..len..enume
 00000350: 7261 7465 da01 6dda 0863 6972 6375 6c61  rate..m..circula
 00000360: 7229 0f72 0c00 0000 720d 0000 0072 0e00  r).r....r....r..
 00000370: 0000 720f 0000 0072 1000 0000 7212 0000  ..r....r....r...
-00000380: 0072 1c00 0000 5a09 616c 6c5f 6571 7561  .r....Z.all_equa
+00000380: 0072 1c00 0000 da09 616c 6c5f 6571 7561  .r......all_equa
 00000390: 6cda 066d 6172 6769 6eda 0570 6561 6b73  l..margin..peaks
 000003a0: da04 6461 7461 da05 6469 7374 73da 076d  ..data..dists..m
-000003b0: 6178 5f76 616c da01 69da 0170 a900 7232  ax_val..i..p..r2
+000003b0: 6178 5f76 616c da01 69da 0170 a900 7233  ax_val..i..p..r3
 000003c0: 0000 00fa 332f 617a 702f 6167 656e 742f  ....3/azp/agent/
 000003d0: 5f77 6f72 6b2f 312f 732f 7372 632f 6c69  _work/1/s/src/li
 000003e0: 6265 7274 656d 2f75 7469 6c73 2f67 656e  bertem/utils/gen
 000003f0: 6572 6174 652e 7079 da0a 6362 6564 5f66  erate.py..cbed_f
 00000400: 7261 6d65 0900 0000 733a 0000 0000 0308  rame....s:......
 00000410: 0110 010a 0108 010c 010a 0108 011a 010a  ................
 00000420: 0108 0116 0108 0104 011a 0216 0214 011a  ................
 00000430: 0210 0106 0106 0106 0102 0102 0102 0102  ................
-00000440: fa04 071e f908 0972 3400 0000 e700 0000  .......r4.......
+00000440: fa04 071e f908 0972 3500 0000 e700 0000  .......r5.......
 00000450: 0000 408f 40e7 0000 0000 0000 1440 e700  ..@.@........@..
 00000460: 0000 0000 00f0 3fe7 0000 0000 0000 3e40  ......?.......>@
 00000470: 6308 0000 0000 0000 0000 0000 000e 0000  c...............
 00000480: 000a 0000 0043 0000 0073 0a01 0000 7c00  .....C...s....|.
 00000490: 6a00 7c01 6a00 6b02 7314 7401 6401 8301  j.|.j.k.s.t.d...
 000004a0: 8201 7c01 6a00 5c02 7d08 7d09 7402 a003  ..|.j.\.}.}.t...
 000004b0: 7402 a004 7c09 a101 7402 a004 7c08 a101  t...|...t...|...
@@ -167,15 +167,15 @@
 00000a60: 6f6c 6f3a 206e 702e 6e64 6172 7261 792c  olo: np.ndarray,
 00000a70: 2032 640a 2020 2020 2020 2020 686f 6c6f   2d.        holo
 00000a80: 6772 616d 2069 6d61 6765 0a20 2020 207a  gram image.    z
 00000a90: 3a41 6d70 6c69 7475 6465 2061 6e64 2070  :Amplitude and p
 00000aa0: 6861 7365 2073 686f 756c 6420 6265 2032  hase should be 2
 00000ab0: 6420 6172 7261 7973 206f 6620 7468 6520  d arrays of the 
 00000ac0: 7361 6d65 2073 6861 7065 2e67 0000 0000  same shape.g....
-00000ad0: 0080 6640 7209 0000 0072 3700 0000 6700  ..f@r....r7...g.
+00000ad0: 0080 6640 7209 0000 0072 3800 0000 6700  ..f@r....r8...g.
 00000ae0: 0000 0000 0000 407a 3770 6f69 7373 6f6e  ......@z7poisson
 00000af0: 5f6e 6f69 7365 2070 6172 616d 6574 6572  _noise parameter
 00000b00: 2073 686f 756c 6420 6265 2066 6c6f 6174   should be float
 00000b10: 206f 7220 696e 7420 6f72 204e 6f6e 652e   or int or None.
 00000b20: 7a38 6761 7573 7369 616e 5f6e 6f69 7365  z8gaussian_noise
 00000b30: 2070 6172 616d 6574 6572 2073 686f 756c   parameter shoul
 00000b40: 6420 6265 2066 6c6f 6174 206f 7220 696e  d be float or in
@@ -189,35 +189,35 @@
 00000bc0: 0000 0029 0eda 0361 6d70 da03 7068 69da  ...)...amp..phi.
 00000bd0: 0663 6f75 6e74 73da 0873 616d 706c 696e  .counts..samplin
 00000be0: 67da 0a76 6973 6962 696c 6974 795a 0766  g..visibilityZ.f
 00000bf0: 5f61 6e67 6c65 5a0e 6761 7573 7369 616e  _angleZ.gaussian
 00000c00: 5f6e 6f69 7365 5a0d 706f 6973 736f 6e5f  _noiseZ.poisson_
 00000c10: 6e6f 6973 65da 0273 79da 0273 78da 0178  noise..sy..sx..x
 00000c20: da01 795a 0468 6f6c 6f5a 0b6e 6f69 7365  ..yZ.holoZ.noise
-00000c30: 5f73 6361 6c65 7232 0000 0072 3200 0000  _scaler2...r2...
-00000c40: 7233 0000 00da 0e68 6f6c 6f67 7261 6d5f  r3.....hologram_
+00000c30: 5f73 6361 6c65 7233 0000 0072 3300 0000  _scaler3...r3...
+00000c40: 7234 0000 00da 0e68 6f6c 6f67 7261 6d5f  r4.....hologram_
 00000c50: 6672 616d 652d 0000 0073 2c00 0000 0033  frame-...s,....3
 00000c60: 0c01 0801 0a01 1c01 0e02 1a01 1e01 1aff  ................
 00000c70: 0202 02fe 04ff 0805 0401 0e01 0801 0801  ................
-00000c80: 1402 0601 0e01 0801 0a02 724d 0000 0063  ..........rM...c
+00000c80: 1402 0601 0e01 0801 0a02 724e 0000 0063  ..........rN...c
 00000c90: 0200 0000 0000 0000 0000 0000 0300 0000  ................
 00000ca0: 0600 0000 4300 0000 732e 0000 0074 006a  ....C...s....t.j
 00000cb0: 0164 0164 0274 027c 0083 0174 027c 0183  .d.d.t.|...t.|..
 00000cc0: 0114 0074 006a 0364 038d 047d 027c 02a0  ...t.j.d...}.|..
 00000cd0: 047c 007c 0117 00a1 0153 0029 044e e905  .|.|.....S.).N..
 00000ce0: 0000 00e9 1e00 0000 2904 da05 7374 6172  ........)...star
 00000cf0: 74da 0473 746f 70da 036e 756d 7215 0000  t..stop..numr...
 00000d00: 0029 0572 1e00 0000 da08 6c69 6e73 7061  .).r......linspa
 00000d10: 6365 7203 0000 0072 2300 0000 da07 7265  cer....r#.....re
 00000d20: 7368 6170 6529 03da 086e 6176 5f64 696d  shape)...nav_dim
-00000d30: 73da 0873 6967 5f64 696d 7372 2d00 0000  s..sig_dimsr-...
-00000d40: 7232 0000 0072 3200 0000 7233 0000 00da  r2...r2...r3....
+00000d30: 73da 0873 6967 5f64 696d 7372 2e00 0000  s..sig_dimsr....
+00000d40: 7233 0000 0072 3300 0000 7234 0000 00da  r3...r3...r4....
 00000d50: 0d67 7261 6469 656e 745f 6461 7461 7900  .gradient_datay.
 00000d60: 0000 7308 0000 0000 0104 0116 ff06 0372  ..s............r
-00000d70: 5700 0000 6302 0000 0000 0000 0000 0000  W...c...........
+00000d70: 5800 0000 6302 0000 0000 0000 0000 0000  X...c...........
 00000d80: 0007 0000 0006 0000 0003 0000 0073 ae00  .............s..
 00000d90: 0000 7c01 6401 6b02 720c 6402 5300 7400  ..|.d.k.r.d.S.t.
 00000da0: 6a01 7c00 7402 6403 8d02 7d02 7403 7404  j.|.t.d...}.t.t.
 00000db0: 7c00 8301 8301 4400 5d2a 8900 7405 8700  |.....D.]*..t...
 00000dc0: 6601 6404 6405 8408 7403 7404 7c00 8301  f.d.d...t.t.|...
 00000dd0: 8301 4400 8301 8301 7d03 6406 7c02 7c03  ..D.....}.d.|.|.
 00000de0: 3c00 7126 6700 7d04 7404 7c04 8301 7c01  <.q&g.}.t.|...|.
@@ -237,59 +237,59 @@
 00000ec0: 6e74 2064 6174 6173 6574 0a20 2020 2072  nt dataset.    r
 00000ed0: 0100 0000 4e72 1400 0000 6301 0000 0000  ....Nr....c.....
 00000ee0: 0000 0000 0000 0002 0000 0003 0000 0033  ...............3
 00000ef0: 0000 0073 2200 0000 7c00 5d1a 7d01 7c01  ...s"...|.].}.|.
 00000f00: 8800 6b03 7216 7400 6400 8301 6e02 6401  ..k.r.t.d...n.d.
 00000f10: 5600 0100 7102 6400 5300 2902 4e29 0272  V...q.d.S.).N).r
 00000f20: 0100 0000 7216 0000 00a9 01da 0573 6c69  ....r........sli
-00000f30: 6365 2902 da02 2e30 7230 0000 00a9 01da  ce)....0r0......
-00000f40: 0364 696d 7232 0000 0072 3300 0000 da09  .dimr2...r3.....
+00000f30: 6365 2902 da02 2e30 7231 0000 00a9 01da  ce)....0r1......
+00000f40: 0364 696d 7233 0000 0072 3400 0000 da09  .dimr3...r4.....
 00000f50: 3c67 656e 6578 7072 3e8d 0000 00f3 0000  <genexpr>.......
 00000f60: 0000 7a21 6578 636c 7564 655f 7069 7865  ..z!exclude_pixe
 00000f70: 6c73 2e3c 6c6f 6361 6c73 3e2e 3c67 656e  ls.<locals>.<gen
 00000f80: 6578 7072 3e46 6301 0000 0000 0000 0000  expr>Fc.........
 00000f90: 0000 0002 0000 0005 0000 0073 0000 0073  ...........s...s
 00000fa0: 2200 0000 7c00 5d1a 7d01 7400 6a01 6a02  "...|.].}.t.j.j.
 00000fb0: 6400 7c01 6400 1800 6401 8d02 5600 0100  d.|.d...d...V...
 00000fc0: 7102 6402 5300 2903 7213 0000 0029 02da  q.d.S.).r....)..
 00000fd0: 036c 6f77 da04 6869 6768 4e29 0372 1e00  .low..highN).r..
-00000fe0: 0000 7242 0000 00da 0772 616e 6469 6e74  ..rB.....randint
-00000ff0: 2902 725a 0000 00da 0173 7232 0000 0072  ).rZ.....sr2...r
-00001000: 3200 0000 7233 0000 0072 5d00 0000 9300  2...r3...r].....
-00001010: 0000 725e 0000 0063 0100 0000 0000 0000  ..r^...c........
+00000fe0: 0000 7243 0000 00da 0772 616e 6469 6e74  ..rC.....randint
+00000ff0: 2902 725b 0000 00da 0173 7233 0000 0072  ).r[.....sr3...r
+00001000: 3300 0000 7234 0000 0072 5e00 0000 9300  3...r4...r^.....
+00001010: 0000 725f 0000 0063 0100 0000 0000 0000  ..r_...c........
 00001020: 0000 0000 0200 0000 0500 0000 7300 0000  ............s...
 00001030: 7320 0000 007c 005d 187d 0174 007c 0164  s ...|.].}.t.|.d
 00001040: 0018 007c 0164 0117 0083 0256 0001 0071  ...|.d.....V...q
 00001050: 0264 0253 0029 0372 1300 0000 7209 0000  .d.S.).r....r...
-00001060: 004e 7258 0000 0029 0272 5a00 0000 da01  .NrX...).rZ.....
-00001070: 6572 3200 0000 7232 0000 0072 3300 0000  er2...r2...r3...
-00001080: 725d 0000 0096 0000 0072 5e00 0000 2909  r].......r^...).
+00001060: 004e 7259 0000 0029 0272 5b00 0000 da01  .NrY...).r[.....
+00001070: 6572 3300 0000 7233 0000 0072 3400 0000  er3...r3...r4...
+00001080: 725e 0000 0096 0000 0072 5f00 0000 2909  r^.......r_...).
 00001090: 721e 0000 00da 046f 6e65 73da 0462 6f6f  r......ones..boo
 000010a0: 6cda 0572 616e 6765 7227 0000 00da 0574  l..ranger'.....t
 000010b0: 7570 6c65 da06 6170 7065 6e64 721f 0000  uple..appendr...
-000010c0: 00da 0154 2907 7256 0000 005a 0c6e 756d  ...T).rV...Z.num
+000010c0: 00da 0154 2907 7257 0000 005a 0c6e 756d  ...T).rW...Z.num
 000010d0: 5f65 7863 6c75 6465 645a 0866 7265 655f  _excludedZ.free_
 000010e0: 6d61 70da 0873 656c 6563 746f 72da 0765  map..selector..e
 000010f0: 7863 6c75 6465 5a0c 6578 636c 7564 655f  xcludeZ.exclude_
 00001100: 6974 656d 5a09 6b6e 6f63 6b5f 6f75 7472  itemZ.knock_outr
-00001110: 3200 0000 725b 0000 0072 3300 0000 da0e  2...r[...r3.....
+00001110: 3300 0000 725c 0000 0072 3400 0000 da0e  3...r\...r4.....
 00001120: 6578 636c 7564 655f 7069 7865 6c73 8000  exclude_pixels..
 00001130: 0000 731c 0000 0000 0608 0104 020e 0310  ..s.............
 00001140: 011e 010a 0204 020c 0112 0108 010a 0112  ................
-00001150: 030a 0472 6c00 0000 2909 7207 0000 0072  ...rl...).r....r
+00001150: 030a 0472 6d00 0000 2909 7207 0000 0072  ...rm...).r....r
 00001160: 0700 0000 4e4e 4e4e 7208 0000 0046 4e29  ....NNNNr....FN)
-00001170: 0672 3500 0000 7236 0000 0072 3700 0000  .r5...r6...r7...
-00001180: 7238 0000 004e 4e29 11da 056e 756d 7079  r8...NN)...numpy
+00001170: 0672 3600 0000 7237 0000 0072 3800 0000  .r6...r7...r8...
+00001180: 7239 0000 004e 4e29 11da 056e 756d 7079  r9...NN)...numpy
 00001190: 721e 0000 005a 1573 6369 7079 2e6e 6469  r....Z.scipy.ndi
 000011a0: 6d61 6765 2e66 696c 7465 7273 7202 0000  mage.filtersr...
 000011b0: 00da 146c 6962 6572 7465 6d2e 636f 6d6d  ...libertem.comm
 000011c0: 6f6e 2e6d 6174 6872 0300 0000 da0e 6c69  on.mathr......li
 000011d0: 6265 7274 656d 2e75 7469 6c73 7204 0000  bertem.utilsr...
 000011e0: 0072 0500 0000 7206 0000 00da 0e6c 6962  .r....r......lib
 000011f0: 6572 7465 6d2e 6d61 736b 73da 056d 6173  ertem.masks..mas
-00001200: 6b73 7229 0000 0072 3400 0000 724d 0000  ksr)...r4...rM..
-00001210: 0072 5700 0000 726c 0000 0072 3200 0000  .rW...rl...r2...
-00001220: 7232 0000 0072 3200 0000 7233 0000 00da  r2...r2...r3....
+00001200: 6b73 7229 0000 0072 3500 0000 724e 0000  ksr)...r5...rN..
+00001210: 0072 5800 0000 726d 0000 0072 3300 0000  .rX...rm...r3...
+00001220: 7233 0000 0072 3300 0000 7234 0000 00da  r3...r3...r4....
 00001230: 083c 6d6f 6475 6c65 3e01 0000 0073 2000  .<module>....s .
 00001240: 0000 0801 0c02 0c01 1401 0c04 0001 00fe  ................
 00001250: 0a25 0001 0001 0001 0001 0001 00fa 0a4c  .%.............L
 00001260: 0807                                     ..
```

### Comparing `libertem-0.9.0/src/libertem/utils/__pycache__/threading.cpython-39.pyc` & `libertem-0.9.2/src/libertem/utils/__pycache__/threading.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 9956 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 e426 0000  a.......z..b.&..
+00000000: 610d 0d0a 0000 0000 7fce 6762 e426 0000  a.........gb.&..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 e200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 6400 6401 6c04  ..d.d.l.Z.d.d.l.
 00000050: 5a04 6400 6401 6c05 5a05 6500 a006 6507  Z.d.d.l.Z.e...e.
 00000060: a101 5a08 6505 a009 a100 5a0a 6401 610b  ..Z.e.....Z.d.a.
 00000070: 6401 610c 6401 610d 6400 610e 6401 610f  d.a.d.a.d.a.d.a.
```

### Comparing `libertem-0.9.0/src/libertem/utils/async_utils.py` & `libertem-0.9.2/src/libertem/utils/async_utils.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/utils/devices.py` & `libertem-0.9.2/src/libertem/utils/devices.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/utils/generate.py` & `libertem-0.9.2/src/libertem/utils/generate.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/utils/threading.py` & `libertem-0.9.2/src/libertem/utils/threading.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/viz/__init__.py` & `libertem-0.9.2/src/libertem/viz/__init__.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/viz/__pycache__/__init__.cpython-39.pyc` & `libertem-0.9.2/src/libertem/viz/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 848 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 5003 0000  a.......z..bP...
+00000000: 610d 0d0a 0000 0000 7fce 6762 5003 0000  a.........gbP...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6402 6403 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 6d07 5a07 6d08 5a08 0100 6700 6404 a201  m.Z.m.Z...g.d...
 00000060: 5a09 6501 8300 6501 6405 6406 8d01 6501  Z.e...e.d.d...e.
 00000070: 6402 6402 6407 6407 6408 6409 8d05 6502  d.d.d.d.d.d...e.
```

### Comparing `libertem-0.9.0/src/libertem/viz/__pycache__/base.cpython-39.pyc` & `libertem-0.9.2/src/libertem/viz/__pycache__/base.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 10612 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 7429 0000  a.......z..bt)..
+00000000: 610d 0d0a 0000 0000 7fce 6762 7429 0000  a.........gbt)..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 c400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 6400 6403 6c04  ..d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 6d06 5a06 0100 6400 6401 6c07  m.Z.m.Z...d.d.l.
 00000060: 5a08 6400 6404 6c09 6d0a 5a0a 6d0b 5a0b  Z.d.d.l.m.Z.m.Z.
 00000070: 0100 6400 6405 6c0c 6d0d 5a0d 0100 6400  ..d.d.l.m.Z...d.
```

### Comparing `libertem-0.9.0/src/libertem/viz/__pycache__/bqp.cpython-39.pyc` & `libertem-0.9.2/src/libertem/viz/__pycache__/bqp.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 4320 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 e010 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 e010 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 6c03 6d04 5a04 0100 6500 a005 6506  d.l.m.Z...e...e.
 00000050: a101 5a07 4700 6404 6405 8400 6405 6504  ..Z.G.d.d...d.e.
 00000060: 8303 5a08 6401 5300 2906 e900 0000 004e  ..Z.d.S.)......N
 00000070: e901 0000 0029 01da 0a4c 6976 6532 4450  .....)...Live2DP
```

### Comparing `libertem-0.9.0/src/libertem/viz/__pycache__/gms.cpython-39.pyc` & `libertem-0.9.2/src/libertem/viz/__pycache__/gms.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 3497 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 a90d 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 a90d 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3000 0000 6400  .....@...s0...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 6c03 6d04 5a04 0100 4700 6404 6405  d.l.m.Z...G.d.d.
 00000050: 8400 6405 6504 8303 5a05 6401 5300 2906  ..d.e...Z.d.S.).
 00000060: e900 0000 004e e901 0000 0029 01da 0a4c  .....N.....)...L
 00000070: 6976 6532 4450 6c6f 7463 0000 0000 0000  ive2DPlotc......
```

### Comparing `libertem-0.9.0/src/libertem/viz/__pycache__/mpl.cpython-39.pyc` & `libertem-0.9.2/src/libertem/viz/__pycache__/mpl.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 3695 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 6f0e 0000  a.......z..bo...
+00000000: 610d 0d0a 0000 0000 7fce 6762 6f0e 0000  a.........gbo...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4e00 0000 6400  .....@...sN...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a03 6400 6401 6c04 6d05 5a06  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6402 6403 6c07 6d08 5a08 0100 6500  ..d.d.l.m.Z...e.
 00000060: a009 650a a101 5a0b 4700 6404 6405 8400  ..e...Z.G.d.d...
 00000070: 6405 6508 8303 5a0c 6401 5300 2906 e900  d.e...Z.d.S.)...
```

### Comparing `libertem-0.9.0/src/libertem/viz/base.py` & `libertem-0.9.2/src/libertem/viz/base.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/viz/bqp.py` & `libertem-0.9.2/src/libertem/viz/bqp.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/viz/gms.py` & `libertem-0.9.2/src/libertem/viz/gms.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/viz/mpl.py` & `libertem-0.9.2/src/libertem/viz/mpl.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/__pycache__/messageconverter.cpython-39.pyc` & `libertem-0.9.2/src/libertem/web/__pycache__/messageconverter.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 1348 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 4405 0000  a.......z..bD...
+00000000: 610d 0d0a 0000 0000 7fce 6762 4405 0000  a.........gbD...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2a00 0000 6400  .....@...s*...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a03 4700 6403 6404 8400 6404  d.l.Z.G.d.d...d.
 00000050: 8302 5a04 6402 5300 2905 e900 0000 0029  ..Z.d.S.)......)
 00000060: 02da 0444 6963 74da 084f 7074 696f 6e61  ...Dict..Optiona
 00000070: 6c4e 6300 0000 0000 0000 0000 0000 0000  lNc.............
```

### Comparing `libertem-0.9.0/src/libertem/web/__pycache__/messages.cpython-39.pyc` & `libertem-0.9.2/src/libertem/web/__pycache__/messages.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 6696 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 281a 0000  a.......z..b(...
+00000000: 610d 0d0a 0000 0000 7fce 6762 281a 0000  a.........gb(...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2a00 0000 6400  .....@...s*...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 4700 6403 6404 8400 6404  m.Z...G.d.d...d.
 00000050: 8302 5a04 6405 5300 2906 e901 0000 0029  ..Z.d.S.)......)
 00000060: 01da 0b53 6861 7265 6453 7461 7465 2901  ...SharedState).
 00000070: da10 4d65 7373 6167 6543 6f6e 7665 7274  ..MessageConvert
```

### Comparing `libertem-0.9.0/src/libertem/web/__pycache__/models.cpython-39.pyc` & `libertem-0.9.2/src/libertem/web/__pycache__/models.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 1156 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 8404 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 8404 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 dc00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 0100 6401  m.Z.m.Z.m.Z...d.
 00000050: 6403 6c07 6d08 5a08 0100 6502 7254 6401  d.l.m.Z...e.rTd.
 00000060: 6404 6c09 6d0a 5a0a 0100 6401 6405 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6401 6406 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `libertem-0.9.0/src/libertem/web/__pycache__/rpc.cpython-39.pyc` & `libertem-0.9.2/src/libertem/web/__pycache__/rpc.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 3300 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 e40c 0000  a.......z..b....
+00000000: 610d 0d0a 0000 0000 7fce 6762 e40c 0000  a.........gb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 c000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6401 6c06 5a06 6400 6401 6c07 5a07 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6403 6c08 6d09 5a09 0100 6404 6405 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 0100 6502  m.Z.m.Z.m.Z...e.
```

### Comparing `libertem-0.9.0/src/libertem/web/__pycache__/state.cpython-39.pyc` & `libertem-0.9.2/src/libertem/web/__pycache__/state.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 13476 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 a434 0000  a.......z..b.4..
+00000000: 610d 0d0a 0000 0000 7fce 6762 a434 0000  a.........gb.4..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 1401 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6402 6c06 6d07 5a07 0100 6400 6403 6c08  d.l.m.Z...d.d.l.
 00000070: 6d09 5a09 0100 6400 6404 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
```

### Comparing `libertem-0.9.0/src/libertem/web/analysis.py` & `libertem-0.9.2/src/libertem/web/analysis.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/base.py` & `libertem-0.9.2/src/libertem/web/base.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/browse.py` & `libertem-0.9.2/src/libertem/web/browse.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/cli.py` & `libertem-0.9.2/src/libertem/web/cli.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/client/asset-manifest.json` & `libertem-0.9.2/src/libertem/web/client/asset-manifest.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7542016806722689%*

 * *Differences: {"'entrypoints'": "{insert: [(2, 'static/js/2.909ce721.chunk.js'), (4, "*

 * *                  "'static/js/main.d79ffbf3.chunk.js')], delete: [4, 2]}",*

 * * "'files'": "{'main.js': './static/static/js/main.d79ffbf3.chunk.js', 'main.js.map': "*

 * *            "'./static/static/js/main.d79ffbf3.chunk.js.map', 'static/js/2.909ce721.chunk.js': "*

 * *            "'./static/static/js/2.909ce721.chunk.js', 'static/js/2.909ce721.chunk.js.map': "*

 * *            "'./static/static/js/2.909ce721.chunk.js.map', "*

 * *            "'static/js/2 […]*

```diff
@@ -1,25 +1,25 @@
 {
     "entrypoints": [
         "static/js/runtime-main.fcac4e81.js",
         "static/css/2.42a8572e.chunk.css",
-        "static/js/2.6b575192.chunk.js",
+        "static/js/2.909ce721.chunk.js",
         "static/css/main.c0d8de42.chunk.css",
-        "static/js/main.2e050bba.chunk.js"
+        "static/js/main.d79ffbf3.chunk.js"
     ],
     "files": {
         "index.html": "./static/index.html",
         "main.css": "./static/static/css/main.c0d8de42.chunk.css",
-        "main.js": "./static/static/js/main.2e050bba.chunk.js",
-        "main.js.map": "./static/static/js/main.2e050bba.chunk.js.map",
+        "main.js": "./static/static/js/main.d79ffbf3.chunk.js",
+        "main.js.map": "./static/static/js/main.d79ffbf3.chunk.js.map",
         "runtime-main.js": "./static/static/js/runtime-main.fcac4e81.js",
         "runtime-main.js.map": "./static/static/js/runtime-main.fcac4e81.js.map",
         "static/css/2.42a8572e.chunk.css": "./static/static/css/2.42a8572e.chunk.css",
         "static/css/2.42a8572e.chunk.css.map": "./static/static/css/2.42a8572e.chunk.css.map",
         "static/css/main.c0d8de42.chunk.css.map": "./static/static/css/main.c0d8de42.chunk.css.map",
-        "static/js/2.6b575192.chunk.js": "./static/static/js/2.6b575192.chunk.js",
-        "static/js/2.6b575192.chunk.js.LICENSE.txt": "./static/static/js/2.6b575192.chunk.js.LICENSE.txt",
-        "static/js/2.6b575192.chunk.js.map": "./static/static/js/2.6b575192.chunk.js.map",
+        "static/js/2.909ce721.chunk.js": "./static/static/js/2.909ce721.chunk.js",
+        "static/js/2.909ce721.chunk.js.LICENSE.txt": "./static/static/js/2.909ce721.chunk.js.LICENSE.txt",
+        "static/js/2.909ce721.chunk.js.map": "./static/static/js/2.909ce721.chunk.js.map",
         "static/media/LiberTEM logo-medium.2765b438.png": "./static/static/media/LiberTEM logo-medium.2765b438.png",
         "static/media/semantic.min.css": "./static/static/media/outline-icons.ddae9b1b.woff"
     }
 }
```

### Comparing `libertem-0.9.0/src/libertem/web/client/favicon.ico` & `libertem-0.9.2/src/libertem/web/client/favicon.ico`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/client/index.html` & `libertem-0.9.2/src/libertem/web/client/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><meta charset="utf-8"><meta name="viewport" content="width=device-width,initial-scale=1,shrink-to-fit=no"><meta name="theme-color" content="#000000"><link rel="shortcut icon" href="./static/favicon.ico"><title>LiberTEM</title><link href="./static/static/css/2.42a8572e.chunk.css" rel="stylesheet"><link href="./static/static/css/main.c0d8de42.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,i=t[0],a=t[1],c=t[2],p=0,s=[];p<i.length;p++)l=i[p],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in a)Object.prototype.hasOwnProperty.call(a,n)&&(e[n]=a[n]);for(f&&f(t);s.length;)s.shift()();return u.push.apply(u,c||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,i=1;i<r.length;i++){var a=r[i];0!==o[a]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./static/";var i=this["webpackJsonplibertem-client"]=this["webpackJsonplibertem-client"]||[],a=i.push.bind(i);i.push=t,i=i.slice();for(var c=0;c<i.length;c++)t(i[c]);var f=a;r()}([])</script><script src="./static/static/js/2.6b575192.chunk.js"></script><script src="./static/static/js/main.2e050bba.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><meta charset="utf-8"><meta name="viewport" content="width=device-width,initial-scale=1,shrink-to-fit=no"><meta name="theme-color" content="#000000"><link rel="shortcut icon" href="./static/favicon.ico"><title>LiberTEM</title><link href="./static/static/css/2.42a8572e.chunk.css" rel="stylesheet"><link href="./static/static/css/main.c0d8de42.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,i=t[0],a=t[1],c=t[2],p=0,s=[];p<i.length;p++)l=i[p],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in a)Object.prototype.hasOwnProperty.call(a,n)&&(e[n]=a[n]);for(f&&f(t);s.length;)s.shift()();return u.push.apply(u,c||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,i=1;i<r.length;i++){var a=r[i];0!==o[a]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./static/";var i=this["webpackJsonplibertem-client"]=this["webpackJsonplibertem-client"]||[],a=i.push.bind(i);i.push=t,i=i.slice();for(var c=0;c<i.length;c++)t(i[c]);var f=a;r()}([])</script><script src="./static/static/js/2.909ce721.chunk.js"></script><script src="./static/static/js/main.d79ffbf3.chunk.js"></script></body></html>
```

### Comparing `libertem-0.9.0/src/libertem/web/client/static/css/2.42a8572e.chunk.css` & `libertem-0.9.2/src/libertem/web/client/static/css/2.42a8572e.chunk.css`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/client/static/css/2.42a8572e.chunk.css.map` & `libertem-0.9.2/src/libertem/web/client/static/css/2.42a8572e.chunk.css.map`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/client/static/js/2.6b575192.chunk.js` & `libertem-0.9.2/src/libertem/web/client/static/js/2.909ce721.chunk.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 2.6b575192.chunk.js.LICENSE.txt */
+/*! For license information please see 2.909ce721.chunk.js.LICENSE.txt */
 (this["webpackJsonplibertem-client"] = this["webpackJsonplibertem-client"] || []).push([
     [2],
     [function(e, t, n) {
         "use strict";
         e.exports = n(241)
     }, function(e, t, n) {
         "use strict";
@@ -31535,8 +31535,8 @@
                 }, t
             }(n(207).a);
         b.handledProps = ["as", "checked", "className", "defaultChecked", "defaultIndeterminate", "disabled", "fitted", "id", "indeterminate", "label", "name", "onChange", "onClick", "onMouseDown", "onMouseUp", "radio", "readOnly", "slider", "tabIndex", "toggle", "type", "value"], b.propTypes = {}, b.defaultProps = {
             type: "checkbox"
         }, b.autoControlledProps = ["checked", "indeterminate"]
     }]
 ]);
-//# sourceMappingURL=2.6b575192.chunk.js.map
+//# sourceMappingURL=2.909ce721.chunk.js.map
```

### Comparing `libertem-0.9.0/src/libertem/web/client/static/js/2.6b575192.chunk.js.LICENSE.txt` & `libertem-0.9.2/src/libertem/web/client/static/js/2.909ce721.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/client/static/js/2.6b575192.chunk.js.map` & `libertem-0.9.2/src/libertem/web/client/static/js/2.909ce721.chunk.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'file'": "'static/js/2.909ce721.chunk.js'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "static/js/2.6b575192.chunk.js",
+    "file": "static/js/2.909ce721.chunk.js",
     "names": [
         "module",
         "exports",
         "require",
         "_extends",
         "Object",
```

### Comparing `libertem-0.9.0/src/libertem/web/client/static/js/main.2e050bba.chunk.js` & `libertem-0.9.2/src/libertem/web/client/static/js/main.d79ffbf3.chunk.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -2841,14 +2841,15 @@
                                 icon: !0,
                                 onClick: function(e) {
                                     Q(!0);
                                     var n = Xe(),
                                         a = "".concat(n, "compoundAnalyses/").concat(t.compoundAnalysis, "/rpc/guess_parameters/");
                                     fetch(a, {
                                         method: "PUT",
+                                        body: JSON.stringify({}),
                                         credentials: "same-origin"
                                     }).then((function(e) {
                                         return e.json()
                                     })).then((function(e) {
                                         Q(!1);
                                         var t = e;
                                         "ok" === t.status ? (A(t.guess.flip_y), h(t.guess.cx), x(t.guess.cy), D(t.guess.scan_rotation.toString())) : console.error(t.message)
@@ -8697,8 +8698,8 @@
             }), document.getElementById("root")), wc.run(mc)
         }
     },
     [
         [301, 1, 2]
     ]
 ]);
-//# sourceMappingURL=main.2e050bba.chunk.js.map
+//# sourceMappingURL=main.d79ffbf3.chunk.js.map
```

### Comparing `libertem-0.9.0/src/libertem/web/client/static/js/main.2e050bba.chunk.js.map` & `libertem-0.9.2/src/libertem/web/client/static/js/main.d79ffbf3.chunk.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8561576354679803%*

 * *Differences: {"'file'": "'static/js/main.d79ffbf3.chunk.js'",*

 * * "'mappings'": "'6GACAA,EAAOC,QAAU,CAAC,QAAU,6BAA6B,SAAW,gC,4CCExDC,E,mHCeL,SAASC,EAAqCC,EAASC,EAAaC,GACvE,YAAaC,IAATD,QAAkCC,IAAZF,EACf,CAAED,aACOG,IAATD,EACA,CAAEF,OAAMC,WAER,CAAED,OAAMC,UAASC,S,SDrBpBJ,K,sCAAAA,E,0BAAAA,E,gCAAAA,E,8BAAAA,E,uBAAAA,M,KASL,IEVKA,EFUCM,EAAU,CACnBC,aAAc,kBAAMN,EAAaD,EAAYQ,gBAC7CC,QAAS,SAACC,GAAD,OAAkCT,EAAaD,EAAYW,QAAS,CAAED,YAC/EE,WAAY,kBAAMX,EAAaD,EAAYa,aAC3CC,UAAW,SAACJ,GAAD,OAAmCT,EAAaD,EAAYe,UAAW,CAAEL,YACpFM,MAAO,SAACC,EA […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.2e050bba.chunk.js",
-    "mappings": "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",
+    "file": "static/js/main.d79ffbf3.chunk.js",
+    "mappings": "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",
     "names": [
         "module",
         "exports",
         "ActionTypes",
         "createAction",
         "type",
         "payload",
@@ -1472,15 +1472,15 @@
         "import * as React from \"react\";\nimport { getPathArc } from \"../helpers/svg\";\nimport { defaultMaskStyles } from \"./styles\";\n\nexport interface RingProps {\n    imageWidth: number,\n    cx: number,\n    cy: number,\n    ri: number,\n    ro: number,\n}\n\nconst Ring: React.FC<RingProps> = ({ imageWidth, cx, cy, ri, ro }) => {\n    // see also: https://stackoverflow.com/a/37883328/540644\n    const pathSpecs = [\n        getPathArc({ x: cx + .5, y: cy + .5 }, 90, 90, ro),\n        getPathArc({ x: cx + .5, y: cy + .5 }, 90, 90, ri)\n    ]\n    const pathSpec = pathSpecs.join(' ');\n\n    return (\n        <path d={pathSpec} fillRule=\"evenodd\" style={{ ...defaultMaskStyles(imageWidth) }} />\n    );\n}\n\nexport default Ring;\n",
         "import * as React from \"react\";\nimport { useState } from \"react\";\nimport { useDispatch } from \"react-redux\";\nimport { AnalysisTypes } from \"../../messages\";\nimport { HandleRenderFunction } from \"../../widgets/types\";\nimport * as compoundAnalysisActions from \"../actions\";\nimport useFramePicker from \"./FramePicker\";\nimport ModeSelector from \"./ModeSelector\";\nimport { useDiskROI } from \"./roi/DiskROI\";\nimport { useRectROI } from \"./roi/RectROI\";\nimport { useRoiPicker } from \"./roi/RoiPicker\";\n\n\nexport enum DefaultModes {\n    SUM = \"SUM\",\n    SD = \"SD\",\n    PICK = \"PICK\",\n}\n\nexport enum DefaultRois {\n    ALL = \"ALL\",\n    DISK = \"DISK\",\n    RECT = \"RECT\",\n}\n\nconst useDefaultFrameView = ({\n    scanWidth, scanHeight, compoundAnalysisId, doAutoStart,\n}: {\n    scanWidth: number, scanHeight: number, compoundAnalysisId: string,\n    doAutoStart: boolean,\n}) => {\n    const availableModes = [\n        {\n            text: \"Average\",\n            value: DefaultModes.SUM,\n        },\n        {\n            text: \"Standard Deviation\",\n            value: DefaultModes.SD,\n        },\n        {\n            text: \"Pick\",\n            value: DefaultModes.PICK,\n        },\n    ]\n\n    const availableRois = [\n        {\n            text: \"All\",\n            value: DefaultRois.ALL,\n        },\n        {\n            text: \"Disk\",\n            value: DefaultRois.DISK,\n        },\n        {\n            text: \"Rect\",\n            value: DefaultRois.RECT,\n        },\n    ]\n\n    const [frameMode, setMode] = useState(DefaultModes.SUM);\n    const [roi, setRoi] = useState(DefaultRois.ALL);\n\n    const dispatch = useDispatch();\n\n    const updateFrameMode = (newMode: string) => {\n        dispatch(compoundAnalysisActions.Actions.enableAutoStart(compoundAnalysisId));\n        setMode(newMode as DefaultModes);\n    }\n\n    const updateRoi = (newRoi: string) => {\n        dispatch(compoundAnalysisActions.Actions.enableAutoStart(compoundAnalysisId));\n        setRoi(newRoi as DefaultRois);\n    }\n\n    const frameModeSelector = <ModeSelector modes={availableModes} currentMode={frameMode} onModeChange={updateFrameMode} label=\"Mode\" />\n\n    let roiSelector = <ModeSelector modes={availableRois} currentMode={roi} onModeChange={updateRoi} label=\"ROI\" />\n\n    if (frameMode === DefaultModes.PICK) {\n        roiSelector = <></>;\n    }\n\n    const [cx, setCx] = React.useState(Math.floor(scanWidth / 2));\n    const [cy, setCy] = React.useState(Math.floor(scanHeight / 2));\n\n    const { coords: pickCoords, handles: pickHandles } = useFramePicker({\n        enabled: frameMode === DefaultModes.PICK,\n        scanWidth, scanHeight,\n        analysisIndex: 0,\n        compoundAnalysisId,\n        cx, cy, setCx, setCy\n    });\n\n    const { rectRoiHandles, rectRoiWidgets, rectRoiParameters } = useRectROI({ scanHeight, scanWidth })\n    const { diskRoiHandles, diskRoiWidgets, diskRoiParameters } = useDiskROI({ scanHeight, scanWidth })\n\n    const nullHandles: HandleRenderFunction = () => null\n    let handles = nullHandles;\n\n    let widgets;\n    let params = { roi: {} };\n    switch (roi) {\n        case DefaultRois.DISK:\n            handles = diskRoiHandles;\n            widgets = diskRoiWidgets;\n            params = diskRoiParameters;\n            break;\n        case DefaultRois.RECT:\n            handles = rectRoiHandles;\n            widgets = rectRoiWidgets;\n            params = rectRoiParameters;\n            break;\n    }\n\n    switch (frameMode) {\n        case DefaultModes.PICK:\n            handles = pickHandles;\n            widgets = undefined;\n            break;\n    }\n\n    useRoiPicker({\n        enabled: frameMode === DefaultModes.SD && doAutoStart,\n        scanWidth, scanHeight,\n        analysisIndex: 0,\n        compoundAnalysisId,\n        roiParameters: params,\n        analysisType: AnalysisTypes.SD_FRAMES\n    })\n\n    useRoiPicker({\n        enabled: frameMode === DefaultModes.SUM && doAutoStart,\n        scanWidth, scanHeight,\n        analysisIndex: 0,\n        compoundAnalysisId,\n        roiParameters: params,\n        analysisType: AnalysisTypes.SUM_FRAMES,\n    })\n\n    const frameViewTitle = (\n        frameMode !== DefaultModes.PICK ? null : <>Pick: x={pickCoords.cx}, y={pickCoords.cy} &emsp;</>\n    )\n\n    return {\n        frameViewTitle,\n        frameModeSelector: (<>{frameModeSelector} {roiSelector}</>),\n        roiSelector,\n        handles,\n        widgets,\n    }\n}\n\nexport default useDefaultFrameView;\n",
         "import React from \"react\";\nimport { useDispatch } from \"react-redux\";\nimport { AnalysisParameters, AnalysisTypes } from \"../../messages\";\nimport { inRectConstraint } from \"../../widgets/constraints\";\nimport DraggableHandle from \"../../widgets/DraggableHandle\";\nimport { HandleRenderFunction } from \"../../widgets/types\";\nimport * as compoundAnalysisActions from \"../actions\";\n\nconst useFramePicker = ({\n    enabled, scanWidth, scanHeight, analysisIndex, compoundAnalysisId, cx, cy, setCx, setCy\n}: {\n    enabled: boolean, scanWidth: number, scanHeight: number,\n    analysisIndex: number, compoundAnalysisId: string,\n    cx: number, cy: number, setCx: (newCx: number) => void, setCy: (newCy: number) => void,\n}) => {\n\n    const dispatch = useDispatch();\n\n    React.useEffect(() => {\n        if (enabled) {\n            const params: AnalysisParameters = {\n                x: cx,\n                y: cy,\n            };\n\n            dispatch(compoundAnalysisActions.Actions.run(compoundAnalysisId, analysisIndex, {\n                analysisType: AnalysisTypes.PICK_FRAME,\n                parameters: params,\n            }))\n        }\n    }, [compoundAnalysisId, cx, cy, enabled, analysisIndex, dispatch]);\n\n    const onPickChange = (pickX: number, pickY: number) => {\n        const newX = Math.round(pickX);\n        const newY = Math.round(pickY);\n        if (cx === newX && cy === newY) {\n            return;\n        }\n        setCx(newX);\n        setCy(newY);\n    }\n\n    const renderPickHandle: HandleRenderFunction = (onDragStart, onDrop) => (\n        <DraggableHandle x={cx} y={cy} withCross\n            imageWidth={scanWidth}\n            onDragMove={onPickChange}\n            parentOnDragStart={onDragStart}\n            parentOnDrop={onDrop}\n            constraint={inRectConstraint(scanWidth, scanHeight)} />\n    )\n\n    return { coords: { cx, cy }, handles: renderPickHandle };\n}\n\nexport default useFramePicker;",
         "import * as React from \"react\";\nimport { Dropdown, DropdownProps } from \"semantic-ui-react\";\n\n\ntype ModeOptions = Array<{\n    text: string;\n    value: string;\n}>;\n\ninterface ModeSelectorProps {\n    modes: ModeOptions,\n    currentMode: string,\n    onModeChange: (mode: string) => void,\n    label: string,\n}\n\nconst ModeSelector: React.FunctionComponent<ModeSelectorProps> = ({\n    modes, currentMode, onModeChange, label\n}) => {\n\n    const onChange = (e: React.SyntheticEvent, data: DropdownProps) => {\n        if(data.value !== undefined && typeof data.value === \"string\") {\n            onModeChange(data.value);\n        }\n    }\n\n    return (\n        <>\n            <div>\n                {label}:{' '}\n                <Dropdown\n                    inline\n                    options={modes}\n                    value={currentMode}\n                    onChange={onChange}\n                />\n            </div>\n        </>\n    )\n}\n\nexport default ModeSelector;",
         "import * as React from \"react\";\nimport { defaultMaskStyles } from \"./styles\";\n\nexport interface RectProps {\n    imageWidth: number,\n    imageHeight: number,\n    x: number,\n    y: number,\n    width: number,\n    height: number,\n}\n\nconst Rect: React.FC<RectProps> = ({ imageWidth, x, y, width, height }) => {\n    let ymin: number;\n    let xmin: number;\n    if (height*width > 0) {\n    ymin = Math.min(y, y+height);\n    xmin = Math.min(x, x+width);}\n    else if (height > 0 && width < 0) \n    {ymin = y;\n    xmin = x+width;}\n    else \n    {ymin = y+height;\n    xmin = x;}\n    return (\n        <rect x={xmin + .5} y={ymin + .5} width={Math.abs(width)} height={Math.abs(height)} style={{ ...defaultMaskStyles(imageWidth) }} />\n    );\n}\n\nexport default Rect;\n\n",
         "import { useState } from \"react\";\nimport { RectRoiParams } from \"../../../messages\";\nimport DraggableHandle from \"../../../widgets/DraggableHandle\";\nimport Rect from \"../../../widgets/Rect\";\nimport { HandleRenderFunction } from \"../../../widgets/types\";\n\n\n\nconst useRectROI = ({ scanWidth, scanHeight }: {\n    scanWidth: number;\n    scanHeight: number;\n}) => {\n    const minLength = Math.min(scanWidth, scanHeight);\n    const [x, setx] = useState(scanWidth / 2);\n    const [y, sety] = useState(scanHeight / 2);\n    const [width, setwidth] = useState(minLength / 8);\n    const [height, setheight] = useState(minLength / 8);\n\n\n    const rectRoiParameters: {roi: RectRoiParams} = {\n        roi: {\n            shape: \"rect\",\n            x,\n            y,\n            width,\n            height,\n        },\n    }\n\n\n    const handleCornerChange = (newx: number, newy: number) => {\n        setx(newx);\n        sety(newy);\n    };\n\n    const handleShapeChange = (newx: number, newy: number) => {\n        setwidth(newx - x);\n        setheight(newy - y);\n    };\n\n    const smthHandle = {\n        x: x + width,\n        y: y + height,\n    }\n\n    const rectRoiHandles: HandleRenderFunction = (handleDragStart, handleDrop) => (<>\n        <DraggableHandle x={x} y={y}\n            imageWidth={scanWidth}\n            onDragMove={handleCornerChange}\n            parentOnDragStart={handleDragStart}\n            parentOnDrop={handleDrop} />\n        <DraggableHandle x={smthHandle.x} y={smthHandle.y}\n            imageWidth={scanWidth}\n            onDragMove={handleShapeChange}\n            parentOnDragStart={handleDragStart}\n            parentOnDrop={handleDrop} />\n    </>);\n\n    const rectRoiWidgets = (\n        <Rect x={x} y={y} width={width} height={height}\n            imageWidth={scanWidth} imageHeight={scanHeight}\n        />\n    );\n\n    return {\n        rectRoiParameters,\n        rectRoiHandles,\n        rectRoiWidgets,\n    };\n};\n\nexport { useRectROI };\n\n",
         "import * as React from \"react\";\nimport { useDispatch } from \"react-redux\";\nimport { AnalysisTypes, FrameParams } from \"../../../messages\";\nimport * as analysisActions from \"../../actions\";\n\n\nconst useRoiPicker = ({ compoundAnalysisId, enabled, analysisIndex, roiParameters, analysisType }: {\n    scanWidth: number;\n    scanHeight: number;\n    enabled: boolean;\n    analysisIndex: number,\n    compoundAnalysisId: string;\n    roiParameters: FrameParams;\n    analysisType: AnalysisTypes.SD_FRAMES | AnalysisTypes.SUM_FRAMES\n}) => {\n    const dispatch = useDispatch();\n\n    React.useEffect(() => {\n        const handle = setTimeout(() => {\n            if (enabled) {\n                const analysisDetails = {\n                    analysisType,\n                    parameters: roiParameters,\n                };\n                dispatch(analysisActions.Actions.run(compoundAnalysisId, analysisIndex, analysisDetails))\n            }\n        }, 100);\n\n        return () => clearTimeout(handle);\n        // rules-of-hooks can't be statically validated here\n        // eslint-disable-next-line\n    }, [analysisType, compoundAnalysisId, enabled, analysisIndex, JSON.stringify(roiParameters), dispatch]);\n\n    return {\n    };\n};\n\nexport { useRoiPicker };\n\n",
-        "import * as React from \"react\";\nimport { useState } from \"react\";\nimport { useDispatch, useSelector } from \"react-redux\";\nimport { Button, Checkbox, Dropdown, DropdownProps, Form, Header, Icon, IconProps, Input, List, Modal, Popup } from \"semantic-ui-react\";\nimport { defaultDebounce, getEnumValues } from \"../../helpers\";\nimport { getApiBasePath } from \"../../helpers/apiHelpers\";\nimport ResultList from \"../../job/components/ResultList\";\nimport { AnalysisDetails, AnalysisTypes, CenterOfMassParams } from \"../../messages\";\nimport { RootReducer } from \"../../store\";\nimport { composeHandles } from \"../../widgets/compose\";\nimport { cbToRadius, inRectConstraint, keepOnCY, riConstraint, roConstraints } from \"../../widgets/constraints\";\nimport Disk from \"../../widgets/Disk\";\nimport { DraggableHandle } from \"../../widgets/DraggableHandle\";\nimport Ring from \"../../widgets/Ring\";\nimport { HandleRenderFunction } from \"../../widgets/types\";\nimport * as compoundAnalysisActions from \"../actions\";\nimport { haveDisplayResult } from \"../helpers\";\nimport { CompoundAnalysisProps } from \"../types\";\nimport useDefaultFrameView from \"./DefaultFrameView\";\nimport AnalysisLayoutTwoCol from \"./layouts/AnalysisLayoutTwoCol\";\nimport Toolbar from \"./Toolbar\";\n\nexport enum CoMMaskShapes {\n    DISK = \"DISK\",\n    RING = \"RING\",\n}\n\nexport const MaskShapeMetadata: { [s: string]: { [s: string]: string } } = {\n    [CoMMaskShapes.DISK]: {\n        label: \"Disk cut-off\",\n    },\n    [CoMMaskShapes.RING]: {\n        label: \"Annular CoM\",\n    }\n}\nconst maskShapeKeys = getEnumValues(CoMMaskShapes);\nconst maskShapeOptions = maskShapeKeys.map(t => ({\n    text: MaskShapeMetadata[CoMMaskShapes[t]].label,\n    value: CoMMaskShapes[t],\n}));\n\ninterface MaskShapeSelectorProps {\n    selectedShape: CoMMaskShapes,\n    handleChange: (e: React.SyntheticEvent, data: DropdownProps) => void,\n}\n\ntype GuessResponse = {\n    status: \"error\";\n    message: string;\n} | {\n    status: \"ok\";\n    guess: {\n        cx: number;\n        cy: number;\n        scan_rotation: number;\n        flip_y: boolean;\n    }\n}\n\n\nconst MaskShapeSelector: React.FC<MaskShapeSelectorProps> = ({ selectedShape, handleChange }) => (\n        <>\n            CoM mask shape:{' '}\n            <Dropdown inline options={maskShapeOptions}\n            value={selectedShape}\n            onChange={handleChange}\n            />\n        </>\n    )\n\nconst CenterOfMassAnalysis: React.FC<CompoundAnalysisProps> = ({ compoundAnalysis, dataset }) => {\n    const { shape } = dataset.params;\n    const [scanHeight, scanWidth, imageHeight, imageWidth] = shape;\n    const minLength = Math.min(imageWidth, imageHeight);\n    const [cx, setCx] = useState(imageWidth / 2);\n    const [cy, setCy] = useState(imageHeight / 2);\n    const [r, setR] = useState(minLength / 4);\n    const [flip_y, setFlipY] = useState(false);\n    const [scan_rotation, setScanRotation] = useState(\"0.0\");\n    const [ri, setRI] = useState(minLength / 8);\n    const [maskShape, setMaskShape] = useState(CoMMaskShapes.DISK)\n    const [guessing, setGuessing] = useState(false);\n\n    const dispatch = useDispatch();\n\n    const rHandle = {\n        x: cx - r,\n        y: cy,\n    }\n\n    const riHandle = {\n        x: cx - ri,\n        y: cy,\n    }\n\n    const handleCenterChange = defaultDebounce((newCx: number, newCy: number) => {\n        setCx(newCx);\n        setCy(newCy);\n    });\n    const handleRChange = defaultDebounce(setR);\n    const handleRIChange = defaultDebounce(setRI);\n\n    let rConstraint = keepOnCY(cy);\n    if (maskShape === CoMMaskShapes.RING) {\n        rConstraint = roConstraints(riHandle.x, cy);\n    }\n\n    let frameViewHandles: HandleRenderFunction = (handleDragStart, handleDrop) => (<>\n        <DraggableHandle x={cx} y={cy}\n            imageWidth={imageWidth}\n            onDragMove={handleCenterChange}\n            parentOnDragStart={handleDragStart}\n            parentOnDrop={handleDrop}\n            constraint={inRectConstraint(imageWidth, imageHeight)} />\n        <DraggableHandle x={rHandle.x} y={rHandle.y}\n            imageWidth={imageWidth}\n            onDragMove={cbToRadius(cx, cy, handleRChange)}\n            parentOnDragStart={handleDragStart}\n            parentOnDrop={handleDrop}\n            constraint={rConstraint} />\n    </>);\n\n    let frameViewWidgets = (<></>);\n\n    if (maskShape === CoMMaskShapes.DISK) {\n        frameViewWidgets = (\n            <Disk cx={cx} cy={cy} r={r}\n                imageWidth={imageWidth} />\n        );\n    } else if(maskShape === CoMMaskShapes.RING) {\n        frameViewWidgets = (\n            <Ring cx={cx} cy={cy} ro={r} ri={ri}\n                imageWidth={imageWidth} />\n        );\n        frameViewHandles = composeHandles(frameViewHandles, (handleDragStart, handleDrop)  => (\n            <>\n                <DraggableHandle x={riHandle.x} y={riHandle.y}\n                    imageWidth={imageWidth}\n                    onDragMove={cbToRadius(cx, cy, handleRIChange)}\n                    parentOnDragStart={handleDragStart}\n                    parentOnDrop={handleDrop}\n                    constraint={riConstraint(rHandle.x, cy)} />\n            </>\n        ));\n    }\n\n    const {\n        frameViewTitle, frameModeSelector,\n        handles: resultHandles, widgets: resultWidgets\n    } = useDefaultFrameView({\n        scanWidth,\n        scanHeight,\n        compoundAnalysisId: compoundAnalysis.compoundAnalysis,\n        doAutoStart: compoundAnalysis.doAutoStart,\n    })\n\n    const subtitle = <>{frameViewTitle} Disk: center=(x={cx.toFixed(2)}, y={cy.toFixed(2)}), r={r.toFixed(2)}</>;\n\n    let parsedScanRotation: number =  parseFloat(scan_rotation);\n    if (!parsedScanRotation) {\n        parsedScanRotation = 0.0;\n    }\n\n    const getDetails: (() => AnalysisDetails) = () => {\n        const parameters: CenterOfMassParams = {\n            shape: \"com\",\n            cx,\n            cy,\n            r,\n            flip_y,\n            scan_rotation: parsedScanRotation,\n        };\n        if (maskShape === CoMMaskShapes.RING) {\n            parameters.ri = ri;\n        }\n        return {\n            analysisType: AnalysisTypes.CENTER_OF_MASS,\n            parameters,\n        };\n    }\n\n    const runAnalysis = () => {\n        dispatch(compoundAnalysisActions.Actions.run(compoundAnalysis.compoundAnalysis, 1, getDetails()));\n    };\n\n    React.useEffect(() => {\n        dispatch(compoundAnalysisActions.Actions.setParams(\n            compoundAnalysis, 1, getDetails()\n        ));\n    }, [cx, cy, flip_y, scan_rotation, r, ri, maskShape]);\n\n    const analyses = useSelector((state: RootReducer) => state.analyses)\n    const jobs = useSelector((state: RootReducer) => state.jobs)\n\n    const haveResult = haveDisplayResult(\n        compoundAnalysis,\n        analyses,\n        jobs,\n        [1],\n    );\n\n    // NOTE: haveResult is not a dependency here, as we don't want to re-run directly\n    // after the results have become available.\n    React.useEffect(() => {\n        if (haveResult) {\n            runAnalysis();\n        }\n    }, [flip_y, scan_rotation]);\n\n    const updateFlipY = (e: React.ChangeEvent<HTMLInputElement>, { checked }: { checked: boolean }) => {\n        setFlipY(checked);\n    };\n\n    const updateScanRotation = (e: React.ChangeEvent<HTMLInputElement>, { value }: { value: string }) => {\n        if (value === \"-\") {\n            setScanRotation(\"-\");\n        }\n        setScanRotation(value);\n    };\n\n    const guessParameters = (ev: React.MouseEvent) => {\n        setGuessing(true);\n        const basePath = getApiBasePath();\n        const url = `${basePath}compoundAnalyses/${compoundAnalysis.compoundAnalysis}/rpc/guess_parameters/`;\n\n        fetch(url, {\n            method: 'PUT',\n            credentials: \"same-origin\",\n        }).then(req => req.json()).then((json) => {\n            setGuessing(false);\n            const response = json as GuessResponse;\n            if(response.status === \"ok\") {\n                setFlipY(response.guess.flip_y);\n                setCx(response.guess.cx);\n                setCy(response.guess.cy);\n                setScanRotation(response.guess.scan_rotation.toString());\n            } else {\n                // eslint-disable-next-line no-console\n                console.error(response.message);\n            }\n        }).catch(e => {\n            setGuessing(false);\n            // eslint-disable-next-line no-console\n            console.error(e)\n        });\n        ev.preventDefault();\n    }\n\n    const guessIconProps: IconProps = guessing ? { name: 'cog', loading: true } : { name: 'question' }\n\n    const toolbar = (\n        <Toolbar compoundAnalysis={compoundAnalysis} onApply={runAnalysis} busyIdxs={[1]} extra={\n            <Button icon onClick={guessParameters} disabled={guessing}>\n                <Icon {...guessIconProps} />\n                Guess parameters\n            </Button>\n        }/>\n    );\n\n\n    // TODO: debounce parameters\n    const comParams = (\n        <>\n            <Header>\n                <Modal trigger={\n                    <Header.Content>\n                        Parameters\n                        {' '}\n                        <Icon name=\"info circle\" size=\"small\" link />\n                    </Header.Content>\n                }>\n                    <Popup.Header>CoM / first moment parameters</Popup.Header>\n                    <Popup.Content>\n                        <Header>CoM mask shape</Header>\n                        <p>\n                            Select a shape that will be used to mask out the data:\n                        </p>\n                        <ul>\n                            <li><em>Annular CoM</em>: calculate the center of mass in a selected ring</li>\n                            <li><em>Disk cut-off</em>: calculate the center of mass in a selected disk</li>\n                        </ul>\n                        <Header>Flip in y direction</Header>\n                        <p>\n                            Flip the Y coordinate. Some detectors, for example Quantum\n                            Detectors Merlin, may have pixel (0, 0) at the lower\n                            left corner. This has to be corrected to get the sign of\n                            the y shift as well as curl and divergence right.\n                        </p>\n                        <Header>Rotation between scan and detector</Header>\n                        <p>\n                            The optics of an electron microscope can rotate the\n                            image. Furthermore, scan generators may allow\n                            scanning in arbitrary directions. This means that\n                            the x and y coordinates of the detector image are\n                            usually not parallel to the x and y scan\n                            coordinates. For interpretation of center of mass\n                            shifts, however, the shift vector in detector\n                            coordinates has to be put in relation to the\n                            position on the sample. This parameter can be used\n                            to rotate the detector coordinates to match the scan\n                            coordinate system. A positive value rotates the\n                            displacement vector clock-wise. That means if the\n                            detector seems rotated to the right relative to the\n                            scan, this value should be negative to counteract\n                            this rotation.\n                        </p>\n                        <p>\n                            Use either the numeric input or the slider to adjust\n                            the rotation angle.\n                        </p>\n                    </Popup.Content>\n                </Modal>\n            </Header>\n            <Form>\n                <List relaxed=\"very\">\n                    <List.Item>\n                        <List.Content>\n                            <MaskShapeSelector selectedShape={maskShape} handleChange={(e, data) => {\n                                setMaskShape(data.value as CoMMaskShapes)\n                            }} />\n                        </List.Content>\n                    </List.Item>\n                    <List.Item>\n                        <List.Content>\n                            <Form.Field control={Checkbox} label=\"Flip in y direction\" checked={flip_y} onChange={updateFlipY} />\n                        </List.Content>\n                    </List.Item>\n                    <List.Item>\n                        <List.Content>\n                            <Form.Field type=\"number\" control={Input} label=\"Rotation between scan and detector (deg)\" value={scan_rotation} onChange={updateScanRotation} />\n                            <Form.Field type=\"range\" min=\"-180\" max=\"180\" step=\"0.1\" control={Input} value={scan_rotation} onChange={updateScanRotation} />\n                        </List.Content>\n                    </List.Item>\n                </List>\n            </Form>\n        </>\n    );\n\n    return (\n        <AnalysisLayoutTwoCol\n            title=\"CoM / first moment analysis\" subtitle={subtitle}\n            left={<>\n                <ResultList\n                    extraHandles={frameViewHandles} extraWidgets={frameViewWidgets}\n                    analysisIndex={0} compoundAnalysis={compoundAnalysis.compoundAnalysis}\n                    width={imageWidth} height={imageHeight}\n                    selectors={frameModeSelector}\n                />\n            </>}\n            right={<>\n                <ResultList\n                    analysisIndex={1} compoundAnalysis={compoundAnalysis.compoundAnalysis}\n                    width={scanWidth} height={scanHeight}\n                    extraHandles={resultHandles}\n                    extraWidgets={resultWidgets}\n                />\n            </>}\n            toolbar={toolbar}\n            params={comParams}\n        />\n    );\n}\n\nexport default CenterOfMassAnalysis;\n",
+        "import * as React from \"react\";\nimport { useState } from \"react\";\nimport { useDispatch, useSelector } from \"react-redux\";\nimport { Button, Checkbox, Dropdown, DropdownProps, Form, Header, Icon, IconProps, Input, List, Modal, Popup } from \"semantic-ui-react\";\nimport { defaultDebounce, getEnumValues } from \"../../helpers\";\nimport { getApiBasePath } from \"../../helpers/apiHelpers\";\nimport ResultList from \"../../job/components/ResultList\";\nimport { AnalysisDetails, AnalysisTypes, CenterOfMassParams } from \"../../messages\";\nimport { RootReducer } from \"../../store\";\nimport { composeHandles } from \"../../widgets/compose\";\nimport { cbToRadius, inRectConstraint, keepOnCY, riConstraint, roConstraints } from \"../../widgets/constraints\";\nimport Disk from \"../../widgets/Disk\";\nimport { DraggableHandle } from \"../../widgets/DraggableHandle\";\nimport Ring from \"../../widgets/Ring\";\nimport { HandleRenderFunction } from \"../../widgets/types\";\nimport * as compoundAnalysisActions from \"../actions\";\nimport { haveDisplayResult } from \"../helpers\";\nimport { CompoundAnalysisProps } from \"../types\";\nimport useDefaultFrameView from \"./DefaultFrameView\";\nimport AnalysisLayoutTwoCol from \"./layouts/AnalysisLayoutTwoCol\";\nimport Toolbar from \"./Toolbar\";\n\nexport enum CoMMaskShapes {\n    DISK = \"DISK\",\n    RING = \"RING\",\n}\n\nexport const MaskShapeMetadata: { [s: string]: { [s: string]: string } } = {\n    [CoMMaskShapes.DISK]: {\n        label: \"Disk cut-off\",\n    },\n    [CoMMaskShapes.RING]: {\n        label: \"Annular CoM\",\n    }\n}\nconst maskShapeKeys = getEnumValues(CoMMaskShapes);\nconst maskShapeOptions = maskShapeKeys.map(t => ({\n    text: MaskShapeMetadata[CoMMaskShapes[t]].label,\n    value: CoMMaskShapes[t],\n}));\n\ninterface MaskShapeSelectorProps {\n    selectedShape: CoMMaskShapes,\n    handleChange: (e: React.SyntheticEvent, data: DropdownProps) => void,\n}\n\ntype GuessResponse = {\n    status: \"error\";\n    message: string;\n} | {\n    status: \"ok\";\n    guess: {\n        cx: number;\n        cy: number;\n        scan_rotation: number;\n        flip_y: boolean;\n    }\n}\n\n\nconst MaskShapeSelector: React.FC<MaskShapeSelectorProps> = ({ selectedShape, handleChange }) => (\n        <>\n            CoM mask shape:{' '}\n            <Dropdown inline options={maskShapeOptions}\n            value={selectedShape}\n            onChange={handleChange}\n            />\n        </>\n    )\n\nconst CenterOfMassAnalysis: React.FC<CompoundAnalysisProps> = ({ compoundAnalysis, dataset }) => {\n    const { shape } = dataset.params;\n    const [scanHeight, scanWidth, imageHeight, imageWidth] = shape;\n    const minLength = Math.min(imageWidth, imageHeight);\n    const [cx, setCx] = useState(imageWidth / 2);\n    const [cy, setCy] = useState(imageHeight / 2);\n    const [r, setR] = useState(minLength / 4);\n    const [flip_y, setFlipY] = useState(false);\n    const [scan_rotation, setScanRotation] = useState(\"0.0\");\n    const [ri, setRI] = useState(minLength / 8);\n    const [maskShape, setMaskShape] = useState(CoMMaskShapes.DISK)\n    const [guessing, setGuessing] = useState(false);\n\n    const dispatch = useDispatch();\n\n    const rHandle = {\n        x: cx - r,\n        y: cy,\n    }\n\n    const riHandle = {\n        x: cx - ri,\n        y: cy,\n    }\n\n    const handleCenterChange = defaultDebounce((newCx: number, newCy: number) => {\n        setCx(newCx);\n        setCy(newCy);\n    });\n    const handleRChange = defaultDebounce(setR);\n    const handleRIChange = defaultDebounce(setRI);\n\n    let rConstraint = keepOnCY(cy);\n    if (maskShape === CoMMaskShapes.RING) {\n        rConstraint = roConstraints(riHandle.x, cy);\n    }\n\n    let frameViewHandles: HandleRenderFunction = (handleDragStart, handleDrop) => (<>\n        <DraggableHandle x={cx} y={cy}\n            imageWidth={imageWidth}\n            onDragMove={handleCenterChange}\n            parentOnDragStart={handleDragStart}\n            parentOnDrop={handleDrop}\n            constraint={inRectConstraint(imageWidth, imageHeight)} />\n        <DraggableHandle x={rHandle.x} y={rHandle.y}\n            imageWidth={imageWidth}\n            onDragMove={cbToRadius(cx, cy, handleRChange)}\n            parentOnDragStart={handleDragStart}\n            parentOnDrop={handleDrop}\n            constraint={rConstraint} />\n    </>);\n\n    let frameViewWidgets = (<></>);\n\n    if (maskShape === CoMMaskShapes.DISK) {\n        frameViewWidgets = (\n            <Disk cx={cx} cy={cy} r={r}\n                imageWidth={imageWidth} />\n        );\n    } else if(maskShape === CoMMaskShapes.RING) {\n        frameViewWidgets = (\n            <Ring cx={cx} cy={cy} ro={r} ri={ri}\n                imageWidth={imageWidth} />\n        );\n        frameViewHandles = composeHandles(frameViewHandles, (handleDragStart, handleDrop)  => (\n            <>\n                <DraggableHandle x={riHandle.x} y={riHandle.y}\n                    imageWidth={imageWidth}\n                    onDragMove={cbToRadius(cx, cy, handleRIChange)}\n                    parentOnDragStart={handleDragStart}\n                    parentOnDrop={handleDrop}\n                    constraint={riConstraint(rHandle.x, cy)} />\n            </>\n        ));\n    }\n\n    const {\n        frameViewTitle, frameModeSelector,\n        handles: resultHandles, widgets: resultWidgets\n    } = useDefaultFrameView({\n        scanWidth,\n        scanHeight,\n        compoundAnalysisId: compoundAnalysis.compoundAnalysis,\n        doAutoStart: compoundAnalysis.doAutoStart,\n    })\n\n    const subtitle = <>{frameViewTitle} Disk: center=(x={cx.toFixed(2)}, y={cy.toFixed(2)}), r={r.toFixed(2)}</>;\n\n    let parsedScanRotation: number =  parseFloat(scan_rotation);\n    if (!parsedScanRotation) {\n        parsedScanRotation = 0.0;\n    }\n\n    const getDetails: (() => AnalysisDetails) = () => {\n        const parameters: CenterOfMassParams = {\n            shape: \"com\",\n            cx,\n            cy,\n            r,\n            flip_y,\n            scan_rotation: parsedScanRotation,\n        };\n        if (maskShape === CoMMaskShapes.RING) {\n            parameters.ri = ri;\n        }\n        return {\n            analysisType: AnalysisTypes.CENTER_OF_MASS,\n            parameters,\n        };\n    }\n\n    const runAnalysis = () => {\n        dispatch(compoundAnalysisActions.Actions.run(compoundAnalysis.compoundAnalysis, 1, getDetails()));\n    };\n\n    React.useEffect(() => {\n        dispatch(compoundAnalysisActions.Actions.setParams(\n            compoundAnalysis, 1, getDetails()\n        ));\n    }, [cx, cy, flip_y, scan_rotation, r, ri, maskShape]);\n\n    const analyses = useSelector((state: RootReducer) => state.analyses)\n    const jobs = useSelector((state: RootReducer) => state.jobs)\n\n    const haveResult = haveDisplayResult(\n        compoundAnalysis,\n        analyses,\n        jobs,\n        [1],\n    );\n\n    // NOTE: haveResult is not a dependency here, as we don't want to re-run directly\n    // after the results have become available.\n    React.useEffect(() => {\n        if (haveResult) {\n            runAnalysis();\n        }\n    }, [flip_y, scan_rotation]);\n\n    const updateFlipY = (e: React.ChangeEvent<HTMLInputElement>, { checked }: { checked: boolean }) => {\n        setFlipY(checked);\n    };\n\n    const updateScanRotation = (e: React.ChangeEvent<HTMLInputElement>, { value }: { value: string }) => {\n        if (value === \"-\") {\n            setScanRotation(\"-\");\n        }\n        setScanRotation(value);\n    };\n\n    const guessParameters = (ev: React.MouseEvent) => {\n        setGuessing(true);\n        const basePath = getApiBasePath();\n        const url = `${basePath}compoundAnalyses/${compoundAnalysis.compoundAnalysis}/rpc/guess_parameters/`;\n\n        fetch(url, {\n            method: 'PUT',\n            body: JSON.stringify({}),\n            credentials: \"same-origin\",\n        }).then(req => req.json()).then((json) => {\n            setGuessing(false);\n            const response = json as GuessResponse;\n            if(response.status === \"ok\") {\n                setFlipY(response.guess.flip_y);\n                setCx(response.guess.cx);\n                setCy(response.guess.cy);\n                setScanRotation(response.guess.scan_rotation.toString());\n            } else {\n                // eslint-disable-next-line no-console\n                console.error(response.message);\n            }\n        }).catch(e => {\n            setGuessing(false);\n            // eslint-disable-next-line no-console\n            console.error(e)\n        });\n        ev.preventDefault();\n    }\n\n    const guessIconProps: IconProps = guessing ? { name: 'cog', loading: true } : { name: 'question' }\n\n    const toolbar = (\n        <Toolbar compoundAnalysis={compoundAnalysis} onApply={runAnalysis} busyIdxs={[1]} extra={\n            <Button icon onClick={guessParameters} disabled={guessing}>\n                <Icon {...guessIconProps} />\n                Guess parameters\n            </Button>\n        }/>\n    );\n\n\n    // TODO: debounce parameters\n    const comParams = (\n        <>\n            <Header>\n                <Modal trigger={\n                    <Header.Content>\n                        Parameters\n                        {' '}\n                        <Icon name=\"info circle\" size=\"small\" link />\n                    </Header.Content>\n                }>\n                    <Popup.Header>CoM / first moment parameters</Popup.Header>\n                    <Popup.Content>\n                        <Header>CoM mask shape</Header>\n                        <p>\n                            Select a shape that will be used to mask out the data:\n                        </p>\n                        <ul>\n                            <li><em>Annular CoM</em>: calculate the center of mass in a selected ring</li>\n                            <li><em>Disk cut-off</em>: calculate the center of mass in a selected disk</li>\n                        </ul>\n                        <Header>Flip in y direction</Header>\n                        <p>\n                            Flip the Y coordinate. Some detectors, for example Quantum\n                            Detectors Merlin, may have pixel (0, 0) at the lower\n                            left corner. This has to be corrected to get the sign of\n                            the y shift as well as curl and divergence right.\n                        </p>\n                        <Header>Rotation between scan and detector</Header>\n                        <p>\n                            The optics of an electron microscope can rotate the\n                            image. Furthermore, scan generators may allow\n                            scanning in arbitrary directions. This means that\n                            the x and y coordinates of the detector image are\n                            usually not parallel to the x and y scan\n                            coordinates. For interpretation of center of mass\n                            shifts, however, the shift vector in detector\n                            coordinates has to be put in relation to the\n                            position on the sample. This parameter can be used\n                            to rotate the detector coordinates to match the scan\n                            coordinate system. A positive value rotates the\n                            displacement vector clock-wise. That means if the\n                            detector seems rotated to the right relative to the\n                            scan, this value should be negative to counteract\n                            this rotation.\n                        </p>\n                        <p>\n                            Use either the numeric input or the slider to adjust\n                            the rotation angle.\n                        </p>\n                    </Popup.Content>\n                </Modal>\n            </Header>\n            <Form>\n                <List relaxed=\"very\">\n                    <List.Item>\n                        <List.Content>\n                            <MaskShapeSelector selectedShape={maskShape} handleChange={(e, data) => {\n                                setMaskShape(data.value as CoMMaskShapes)\n                            }} />\n                        </List.Content>\n                    </List.Item>\n                    <List.Item>\n                        <List.Content>\n                            <Form.Field control={Checkbox} label=\"Flip in y direction\" checked={flip_y} onChange={updateFlipY} />\n                        </List.Content>\n                    </List.Item>\n                    <List.Item>\n                        <List.Content>\n                            <Form.Field type=\"number\" control={Input} label=\"Rotation between scan and detector (deg)\" value={scan_rotation} onChange={updateScanRotation} />\n                            <Form.Field type=\"range\" min=\"-180\" max=\"180\" step=\"0.1\" control={Input} value={scan_rotation} onChange={updateScanRotation} />\n                        </List.Content>\n                    </List.Item>\n                </List>\n            </Form>\n        </>\n    );\n\n    return (\n        <AnalysisLayoutTwoCol\n            title=\"CoM / first moment analysis\" subtitle={subtitle}\n            left={<>\n                <ResultList\n                    extraHandles={frameViewHandles} extraWidgets={frameViewWidgets}\n                    analysisIndex={0} compoundAnalysis={compoundAnalysis.compoundAnalysis}\n                    width={imageWidth} height={imageHeight}\n                    selectors={frameModeSelector}\n                />\n            </>}\n            right={<>\n                <ResultList\n                    analysisIndex={1} compoundAnalysis={compoundAnalysis.compoundAnalysis}\n                    width={scanWidth} height={scanHeight}\n                    extraHandles={resultHandles}\n                    extraWidgets={resultWidgets}\n                />\n            </>}\n            toolbar={toolbar}\n            params={comParams}\n        />\n    );\n}\n\nexport default CenterOfMassAnalysis;\n",
         "import { useState } from \"react\";\n\nimport { FrameParams } from \"../../../messages\";\nimport { cbToRadius, inRectConstraint, keepOnCY } from \"../../../widgets/constraints\";\nimport Disk from \"../../../widgets/Disk\";\nimport DraggableHandle from \"../../../widgets/DraggableHandle\";\nimport { HandleRenderFunction } from \"../../../widgets/types\";\n\nconst useDiskROI = ({ scanWidth, scanHeight }: {\n    scanWidth: number;\n    scanHeight: number;\n}) => {\n    const minLength = Math.min(scanWidth, scanHeight);\n    const [cx, setCx] = useState(scanWidth / 2);\n    const [cy, setCy] = useState(scanHeight / 2);\n    const [r, setR] = useState(minLength / 8);\n\n\n    const diskRoiParameters: FrameParams = {\n        roi: {\n            shape: \"disk\",\n            cx,\n            cy,\n            r,\n        },\n    }\n\n\n    const handleCenterChange = (newCx: number, newCy: number) => {\n        setCx(newCx);\n        setCy(newCy);\n    };\n\n    const handleRChange = (newR: number) => {\n        setR(newR);\n    };\n\n    const rHandle = {\n        x: cx - r,\n        y: cy,\n    }\n\n    const diskRoiHandles: HandleRenderFunction = (handleDragStart, handleDrop) => (<>\n        <DraggableHandle x={cx} y={cy}\n            imageWidth={scanWidth}\n            onDragMove={handleCenterChange}\n            parentOnDragStart={handleDragStart}\n            parentOnDrop={handleDrop}\n            constraint={inRectConstraint(scanWidth, scanHeight)} />\n        <DraggableHandle x={rHandle.x} y={rHandle.y}\n            imageWidth={scanWidth}\n            onDragMove={cbToRadius(cx, cy, handleRChange)}\n            parentOnDragStart={handleDragStart}\n            parentOnDrop={handleDrop}\n            constraint={keepOnCY(cy)} />\n    </>);\n\n    const diskRoiWidgets = (\n        <Disk cx={cx} cy={cy} r={r}\n            imageWidth={scanWidth}\n        />\n    );\n\n    return {\n        diskRoiParameters,\n        diskRoiHandles,\n        diskRoiWidgets,\n    };\n};\n\nexport { useDiskROI };\n\n",
         "import * as React from \"react\";\nimport { Grid, Header, Icon, Segment } from \"semantic-ui-react\";\n\ninterface AnalysisLayoutTwoColProps {\n    title: string,\n    subtitle: React.ReactNode,\n    left: React.ReactNode,\n    right: React.ReactNode,\n    toolbar?: React.ReactNode,\n    params?: React.ReactNode,\n}\n\ntype MergedProps = AnalysisLayoutTwoColProps;\n\nconst AnalysisLayoutTwoCol: React.FC<MergedProps> = ({\n    title, subtitle,\n    left, right,\n    toolbar,\n    params,\n}) => (\n    <>\n        <Header as='h3' attached=\"top\">\n            <Icon name=\"cog\" />\n            <Header.Content>{title}</Header.Content>\n        </Header>\n        <Segment attached>\n            <Grid columns={2}>\n                <Grid.Row>\n                    <Grid.Column>\n                        {left}\n                        <p>{subtitle}</p>\n                    </Grid.Column>\n                    <Grid.Column>\n                        {right}\n                    </Grid.Column>\n                </Grid.Row>\n            </Grid>\n        </Segment>\n        {params === null ? params : <Segment attached>{params}</Segment>}\n        {toolbar}\n    </>\n)\n\nexport default AnalysisLayoutTwoCol\n",
         "import { genericDelete, genericPut, getApiBasePath } from \"../helpers/apiHelpers\";\nimport { AnalysisDetails, CompoundAnalysisDetails, CopyNotebookResponse, CreateAnalysisResponse, CreateCompoundAnalysisResponse, CreateOrUpdateAnalysisRequest, CreateOrUpdateCompoundAnalysisRequest, RemoveAnalysisResponse, RemoveCompoundAnalysisResponse } from \"../messages\";\n\nexport const createOrUpdateAnalysis = async (\n    compoundAnalysisId: string,\n    analysisId: string, dataset: string, details: AnalysisDetails\n): Promise<CreateAnalysisResponse> => {\n    const payload: CreateOrUpdateAnalysisRequest = {\n        dataset,\n        details,\n    };\n    return await genericPut(`compoundAnalyses/${compoundAnalysisId}/analyses/${analysisId}/`, payload);\n}\n\nexport const removeAnalysis = async (compoundAnalysisId: string, analysisId: string): Promise<RemoveAnalysisResponse> => (\n    await genericDelete(`compoundAnalyses/${compoundAnalysisId}/analyses/${analysisId}/`)\n);\n\nexport const createOrUpdateCompoundAnalysis = async (\n    compoundAnalysisId: string,\n    dataset: string,\n    details: CompoundAnalysisDetails,\n): Promise<CreateCompoundAnalysisResponse> => {\n    const payload: CreateOrUpdateCompoundAnalysisRequest = {\n        dataset,\n        details,\n    };\n    return await genericPut(`compoundAnalyses/${compoundAnalysisId}/`, payload);\n}\n\nexport const removeCompoundAnalysis = async (compoundAnalysisId: string): Promise<RemoveCompoundAnalysisResponse> => (\n    await genericDelete(`compoundAnalyses/${compoundAnalysisId}/`)\n);\n\nexport const getNotebook = async (compoundAnalysisId: string): Promise<CopyNotebookResponse> => {\n    const basePath = getApiBasePath();\n    const url = `${basePath}compoundAnalyses/${compoundAnalysisId}/copy/notebook/`;\n    const r = await fetch(url, {\n        method: 'GET',\n        credentials: \"same-origin\",\n    });\n    return await (r.json() as Promise<CopyNotebookResponse>);\n}\n",
         "import { AnalysisTypes } from \"../messages\";\nimport { CompoundAnalysisMetadata, CompoundAnalysisMetadataItem } from \"./types\";\n// keyof typeof: https://stackoverflow.com/a/42623905/540644\nexport const getMetadata = (typeName: keyof typeof AnalysisTypes): CompoundAnalysisMetadataItem => {\n    const type: AnalysisTypes = AnalysisTypes[typeName];\n    return CompoundAnalysisMetadata[type];\n};\n",
         "import * as React from \"react\";\nimport { useEffect, useState } from \"react\";\nimport { useDispatch, useSelector } from \"react-redux\";\nimport { Button, Dropdown, DropdownProps, Header, Icon, Modal, Segment, Tab } from \"semantic-ui-react\";\nimport { AnalysisState } from \"../../analysis/types\";\nimport { dispatchGenericError } from \"../../errors/helpers\";\nimport { writeClipboard } from \"../../helpers\";\nimport { getApiBasePath } from \"../../helpers/apiHelpers\";\nimport { JobStatus } from \"../../job/types\";\nimport { CopyAnalysis } from \"../../messages\";\nimport { RootReducer } from \"../../store\";\nimport { getNotebook } from '../api';\nimport { getMetadata } from \"../getMetadata\";\nimport { CompoundAnalysisState } from \"../types\";\n\ninterface DownloadItemsProps {\n    compoundAnalysis: CompoundAnalysisState,\n    currentFormat: string,\n}\n\nconst DownloadItems: React.FC<DownloadItemsProps> = ({\n    compoundAnalysis, currentFormat\n}) => {\n\n    const basePath = getApiBasePath();\n    const downloadUrl = (analysisId: string) => (\n        `${basePath}compoundAnalyses/${compoundAnalysis.compoundAnalysis}/analyses/${analysisId}/download/${currentFormat}/`\n    )\n\n    const analysesById = useSelector((state: RootReducer) => state.analyses.byId);\n    const jobsById = useSelector((state: RootReducer) => state.jobs.byId);\n\n    const analyses = compoundAnalysis.details.analyses.map(analysis => analysesById[analysis]).filter(analysis =>\n        analysis.jobs.some(jobId => jobsById[jobId].status === JobStatus.SUCCESS)\n    );\n\n    const getAnalysisDescription = (analysis: AnalysisState) => getMetadata(analysis.details.analysisType).desc;\n\n    const getDownloadChannels = (analysis: AnalysisState) => {\n        if (!analysis.displayedJob) {\n            return [];\n        }\n        return jobsById[analysis.displayedJob].results.filter(\n            result => result.description.includeInDownload\n        ).map(\n            result => result.description.title\n        )\n    }\n\n    return (\n        <ul>\n            {analyses.map((analysis) => (\n                <li key={analysis.id}>\n                    <a href={downloadUrl(analysis.id)}>\n                        {getAnalysisDescription(analysis)} (channels: {getDownloadChannels(analysis).join(\", \")})\n                        </a>\n                </li>\n            ))}\n        </ul>\n    )\n}\n\ninterface CopyScriptsProps {\n    compoundAnalysis: CompoundAnalysisState,\n}\n\nconst CopyScripts: React.FC<CopyScriptsProps> = ({ compoundAnalysis }) => {\n    const initialAnalysis: CopyAnalysis[] = [\n        {\n            analysis: \"\",\n            plot: [\"\"],\n        },\n    ];\n\n    const [notebook, setNotebook] = useState({\n        dependency: \"\",\n        initial_setup: \"\",\n        ctx: \"\",\n        dataset: \"\",\n        analysis: initialAnalysis,\n    });\n\n    const dispatch = useDispatch();\n\n    const cell = (code: string) => {\n        const copy = () => {\n            writeClipboard(code, dispatch);\n        };\n\n        return (\n            <Segment padded>\n                <Button floated={\"right\"} icon={\"copy\"} onClick={copy} />\n                <pre>{code}</pre>\n            </Segment>\n        );\n    };\n\n    const copyCompleteNotebook = () => {\n        const firstPart = [notebook.dependency, notebook.initial_setup, notebook.ctx, notebook.dataset].join(\"\\n\\n\");\n        const joinCode = (analysis: CopyAnalysis) => `${analysis.analysis}\\n${analysis.plot.join(\"\\n\\n\")}`\n        const secondPart = notebook.analysis.map(joinCode).join(\"\\n\\n\");\n        writeClipboard(`${firstPart}\\n\\n${secondPart}`, dispatch);\n    };\n\n    useEffect(() => {\n        getNotebook(compoundAnalysis.compoundAnalysis).then(CurrentNotebook => {\n            setNotebook({\n                dependency: CurrentNotebook.dependency,\n                initial_setup: CurrentNotebook.initial_setup,\n                ctx: CurrentNotebook.ctx,\n                dataset: CurrentNotebook.dataset,\n                analysis: CurrentNotebook.analysis,\n            });\n        }).catch(() => dispatchGenericError(\"could not get notebook\", dispatch))\n    }, [compoundAnalysis.compoundAnalysis]);\n\n    return (\n        <>\n            <Segment clearing>\n                <Header floated={\"left\"}>Notebook</Header>\n                <Button icon labelPosition=\"left\" floated={\"right\"} onClick={copyCompleteNotebook}>\n                    <Icon name=\"copy\" />\n                    Complete notebook\n                </Button>\n            </Segment>\n            <Modal.Content scrolling>\n                {[notebook.dependency, notebook.initial_setup, notebook.ctx, notebook.dataset].map(cell)}\n                {notebook.analysis.map(analysis => (\n                    <>\n                        {cell(analysis.analysis)}\n                        {analysis.plot.map(cell)}\n                    </>\n                ))}\n            </Modal.Content>\n        </>\n    );\n};\n\ninterface DownloadScriptsProps {\n    compoundAnalysis: CompoundAnalysisState,\n}\n\nconst DownloadScripts: React.FC<DownloadScriptsProps> = ({ compoundAnalysis }) => {\n    const basePath = getApiBasePath();\n    const downloadUrl = `${basePath}compoundAnalyses/${compoundAnalysis.compoundAnalysis}/download/notebook/`;\n\n    return (\n        <ul>\n            <li>\n                <a href={downloadUrl}>notebook corresponding to analysis</a>\n            </li>\n        </ul>\n    );\n};\n\ninterface DownloadProps {\n    compoundAnalysis: CompoundAnalysisState,\n}\n\ntype FormatOptions = Array<{\n    text: string;\n    value: string;\n}>;\n\ninterface DownloadResultItemProps {\n    formatOptions: FormatOptions,\n    onFormatChange: (e: React.SyntheticEvent, data: DropdownProps) => void,\n    currentFormat: string,\n    compoundAnalysis: CompoundAnalysisState,\n}\n\nconst DownloadResultItem: React.FC<DownloadResultItemProps> = ({\n    formatOptions, onFormatChange, currentFormat, compoundAnalysis,\n}) => (\n    <Tab.Pane>\n        <Header >\n            Download Results, format: <Dropdown inline options={formatOptions} onChange={onFormatChange} value={currentFormat} />\n        </Header>\n        <Header as=\"h3\">Available results:</Header>\n        <DownloadItems compoundAnalysis={compoundAnalysis} currentFormat={currentFormat} />\n    </Tab.Pane>\n);\n\ninterface DownloadNotebookItemProps {\n    compoundAnalysis: CompoundAnalysisState,\n}\n\nconst DownloadNotebookItem: React.FC<DownloadNotebookItemProps> = ({\n    compoundAnalysis\n}) => (\n    <Tab.Pane>\n        <Header as=\"h3\">Available scripts: </Header>\n        <DownloadScripts compoundAnalysis={compoundAnalysis} />\n    </Tab.Pane>\n);\n\ninterface CopyNotebookItemProps {\n    compoundAnalysis: CompoundAnalysisState,\n}\n\nconst CopyNotebookItem: React.FC<CopyNotebookItemProps> = ({\n    compoundAnalysis,\n}) => (\n    <Tab.Pane>\n        <CopyScripts compoundAnalysis={compoundAnalysis} />\n    </Tab.Pane>\n);\n\nconst Download: React.FC<DownloadProps> = ({ compoundAnalysis }) => {\n    const formats = useSelector((state: RootReducer) => state.config.resultFileFormats);\n    const formatOptions: FormatOptions = Object.keys(formats).map(identifier => ({\n        value: identifier,\n        text: formats[identifier].description,\n    }));\n\n    const [currentFormat, setFormat] = useState(formatOptions[0]?.value);\n\n    // we may be called before the config is completely loaded, so we\n    // need to set the format after the list of formats is available\n    React.useEffect(() => {\n        if (formatOptions.length !== 0 && !currentFormat) {\n            setFormat(formatOptions[0].value);\n        }\n    }, [formatOptions, currentFormat])\n\n    const onFormatChange = (e: React.SyntheticEvent, data: DropdownProps) => {\n        if(data.value) {\n            setFormat(data.value.toString());\n        }\n    }\n\n    const panes = [\n        {\n            menuItem: \"Download result\",\n            render: () => <DownloadResultItem formatOptions={formatOptions} onFormatChange={onFormatChange} currentFormat={currentFormat} compoundAnalysis={compoundAnalysis} />\n        },\n        {\n            menuItem: \"Download notebook\",\n            render: () => <DownloadNotebookItem compoundAnalysis={compoundAnalysis} />,\n        },\n        {\n            menuItem: \"Copy notebook\",\n            render: () => <CopyNotebookItem compoundAnalysis={compoundAnalysis} />,\n        },\n    ];\n\n\n    return (\n        <Modal trigger={\n            <Button icon>\n                <Icon name='download' />\n                Download\n            </Button>\n        }>\n            <Tab panes={panes} />\n        </Modal>\n    );\n}\n\nexport default Download;",
         "import * as React from \"react\";\nimport { useDispatch, useSelector } from \"react-redux\";\nimport { Button, Icon, IconProps, Segment } from \"semantic-ui-react\";\nimport { RootReducer } from \"../../store\";\nimport * as analysisActions from \"../actions\";\nimport { getAnalysisStatus } from \"../helpers\";\nimport { CompoundAnalysisState } from \"../types\";\nimport Download from \"./Download\";\n\ninterface ToolbarProps {\n    compoundAnalysis: CompoundAnalysisState,\n    busyIdxs: number[],\n    extra?: React.ReactNode,\n    onApply: () => void,\n}\n\n\ntype MergedProps = ToolbarProps;\n\nconst Toolbar: React.FC<MergedProps> = ({ busyIdxs, onApply, compoundAnalysis, extra }) => {\n    const dispatch = useDispatch();\n    const handleRemove = () => dispatch(analysisActions.Actions.remove(compoundAnalysis.compoundAnalysis));\n    const analyses = useSelector((state: RootReducer) => state.analyses);\n    const jobs = useSelector((state: RootReducer) => state.jobs);\n    const status = getAnalysisStatus(\n        compoundAnalysis, analyses, jobs,\n        busyIdxs\n    );\n    const running = status === \"busy\";\n    const applyIconProps: IconProps = running ? { name: 'cog', loading: true } : { name: 'check' }\n\n    return (\n        <Segment attached=\"bottom\">\n            <Button.Group>\n                <Button primary onClick={onApply} icon>\n                    <Icon {...applyIconProps} />\n                    Apply\n                </Button>\n                <Download compoundAnalysis={compoundAnalysis} />\n                <Button onClick={handleRemove} icon>\n                    <Icon name='remove' />\n                    Remove\n                </Button>\n                {extra}\n            </Button.Group>\n        </Segment>\n    );\n}\n\nexport default Toolbar;\n",
         "import { AnalysisReducerState } from \"../analysis/reducers\";\nimport { JobReducerState } from \"../job/reducers\";\nimport { JobRunning } from \"../job/types\";\nimport { CompoundAnalysisState } from \"./types\";\n\nexport const getAnalysisStatus = (\n    compoundAnalysis: CompoundAnalysisState,\n    analyses: AnalysisReducerState,\n    jobs: JobReducerState,\n    analysisIdxsToInclude: number[] = []\n): \"idle\" | \"busy\" => {\n    let filteredAnalyses = compoundAnalysis.details.analyses;\n\n    if (analysisIdxsToInclude.length > 0) {\n        filteredAnalyses = filteredAnalyses.filter((analysisId: string, idx: number) => analysisIdxsToInclude.indexOf(idx) !== -1)\n    }\n\n    return filteredAnalyses.reduce((prevValue: \"idle\" | \"busy\", analysisId: string) => {\n        const analysis = analyses.byId[analysisId];\n        if(!analysis) {\n            return prevValue; // no analysis, so \"all jobs\" are done\n        }\n        analysis.jobs.forEach((jobId) => {\n            if (!jobs.byId[jobId]) {\n                // eslint-disable-next-line no-console\n                console.error(`could not find job id ${jobId} for analysis ${analysisId}`);\n            }\n        });\n        const allDone = analysis.jobs.every(\n            jobId => jobs.byId[jobId] ? jobs.byId[jobId].running === JobRunning.DONE : true\n        );\n        return allDone ? prevValue : \"busy\";\n    }, \"idle\");\n}\n\n\n/**\n * Check if there is a finished job that is being displayed\n * \n * @param compoundAnalysis \n * @param analyses \n * @param jobs \n * @param analysisIdxsToInclude \n * @returns true iff all displayedJobs of the given analyses are DONE (also false if there are no analyses or displayed jobs)\n */\nexport const haveDisplayResult = (\n    compoundAnalysis: CompoundAnalysisState,\n    analyses: AnalysisReducerState,\n    jobs: JobReducerState,\n    analysisIdxsToInclude: number[] = []\n): boolean => {\n    let filteredAnalyses = compoundAnalysis.details.analyses;\n\n    if (analysisIdxsToInclude.length > 0) {\n        filteredAnalyses = filteredAnalyses.filter((analysisId: string, idx: number) => analysisIdxsToInclude.indexOf(idx) !== -1)\n    }\n\n    if (filteredAnalyses.length === 0) {\n        return false;\n    }\n\n    return filteredAnalyses.reduce((prevValue: boolean, analysisId: string) => {\n        const analysis = analyses.byId[analysisId];\n        if (!analysis) {\n            return false; // no analysis, so we don't have a result\n        }\n        if (!analysis.displayedJob) {\n            return false;\n        }\n        const displayedJob = jobs.byId[analysis.displayedJob];\n        if (!displayedJob) {\n            return false;\n        }\n\n        return displayedJob.running === JobRunning.DONE && prevValue;\n    }, true);\n}\n",
```

### Comparing `libertem-0.9.0/src/libertem/web/client/static/js/runtime-main.fcac4e81.js` & `libertem-0.9.2/src/libertem/web/client/static/js/runtime-main.fcac4e81.js`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/client/static/js/runtime-main.fcac4e81.js.map` & `libertem-0.9.2/src/libertem/web/client/static/js/runtime-main.fcac4e81.js.map`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/client/static/media/LiberTEM logo-medium.2765b438.png` & `libertem-0.9.2/src/libertem/web/client/static/media/LiberTEM logo-medium.2765b438.png`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/client/static/media/brand-icons.278156e4.woff2` & `libertem-0.9.2/src/libertem/web/client/static/media/brand-icons.278156e4.woff2`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/client/static/media/brand-icons.65a2fb6d.ttf` & `libertem-0.9.2/src/libertem/web/client/static/media/brand-icons.65a2fb6d.ttf`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/client/static/media/brand-icons.6729d297.svg` & `libertem-0.9.2/src/libertem/web/client/static/media/brand-icons.6729d297.svg`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/client/static/media/brand-icons.cac87dc0.woff` & `libertem-0.9.2/src/libertem/web/client/static/media/brand-icons.cac87dc0.woff`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/client/static/media/brand-icons.d68fa3e6.eot` & `libertem-0.9.2/src/libertem/web/client/static/media/brand-icons.d68fa3e6.eot`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/client/static/media/flags.99f63ae7.png` & `libertem-0.9.2/src/libertem/web/client/static/media/flags.99f63ae7.png`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/client/static/media/icons.38c6d8ba.woff2` & `libertem-0.9.2/src/libertem/web/client/static/media/icons.38c6d8ba.woff2`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/client/static/media/icons.425399f8.woff` & `libertem-0.9.2/src/libertem/web/client/static/media/icons.425399f8.woff`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/client/static/media/icons.62d9dae4.svg` & `libertem-0.9.2/src/libertem/web/client/static/media/icons.62d9dae4.svg`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/client/static/media/icons.a01e3f2d.eot` & `libertem-0.9.2/src/libertem/web/client/static/media/icons.a01e3f2d.eot`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/client/static/media/icons.c656b8ca.ttf` & `libertem-0.9.2/src/libertem/web/client/static/media/icons.c656b8ca.ttf`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/client/static/media/outline-icons.53671035.ttf` & `libertem-0.9.2/src/libertem/web/client/static/media/outline-icons.53671035.ttf`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/client/static/media/outline-icons.687a4990.woff2` & `libertem-0.9.2/src/libertem/web/client/static/media/outline-icons.687a4990.woff2`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/client/static/media/outline-icons.752905fa.eot` & `libertem-0.9.2/src/libertem/web/client/static/media/outline-icons.752905fa.eot`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/client/static/media/outline-icons.9c4845b4.svg` & `libertem-0.9.2/src/libertem/web/client/static/media/outline-icons.9c4845b4.svg`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/client/static/media/outline-icons.ddae9b1b.woff` & `libertem-0.9.2/src/libertem/web/client/static/media/outline-icons.ddae9b1b.woff`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/config.py` & `libertem-0.9.2/src/libertem/web/config.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/connect.py` & `libertem-0.9.2/src/libertem/web/connect.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/dataset.py` & `libertem-0.9.2/src/libertem/web/dataset.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/engine.py` & `libertem-0.9.2/src/libertem/web/engine.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/events.py` & `libertem-0.9.2/src/libertem/web/events.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/generator.py` & `libertem-0.9.2/src/libertem/web/generator.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/jobs.py` & `libertem-0.9.2/src/libertem/web/jobs.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/messageconverter.py` & `libertem-0.9.2/src/libertem/web/messageconverter.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/messages.py` & `libertem-0.9.2/src/libertem/web/messages.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/models.py` & `libertem-0.9.2/src/libertem/web/models.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/notebook_generator/__pycache__/template.cpython-39.pyc` & `libertem-0.9.2/src/libertem/web/notebook_generator/__pycache__/template.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Feb 16 12:09:30 2022 UTC, .py size: 1323 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7ae9 0c62 2b05 0000  a.......z..b+...
+00000000: 610d 0d0a 0000 0000 7fce 6762 2b05 0000  a.........gb+...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 4700 6403 6404 8400 6404 8302 5a03  ..G.d.d...d...Z.
 00000050: 6401 5300 2905 e900 0000 004e 2901 da08  d.S.)......N)...
 00000060: 5465 6d70 6c61 7465 6300 0000 0000 0000  Templatec.......
 00000070: 0000 0000 0000 0000 0002 0000 0040 0000  .............@..
```

### Comparing `libertem-0.9.0/src/libertem/web/notebook_generator/code_template.py` & `libertem-0.9.2/src/libertem/web/notebook_generator/code_template.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/notebook_generator/copy.py` & `libertem-0.9.2/src/libertem/web/notebook_generator/copy.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/notebook_generator/notebook_generator.py` & `libertem-0.9.2/src/libertem/web/notebook_generator/notebook_generator.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/notebook_generator/template.py` & `libertem-0.9.2/src/libertem/web/notebook_generator/template.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/rpc.py` & `libertem-0.9.2/src/libertem/web/rpc.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/server.py` & `libertem-0.9.2/src/libertem/web/server.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/shutdown.py` & `libertem-0.9.2/src/libertem/web/shutdown.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/web/state.py` & `libertem-0.9.2/src/libertem/web/state.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem/win_tweaks.py` & `libertem-0.9.2/src/libertem/win_tweaks.py`

 * *Files identical despite different names*

### Comparing `libertem-0.9.0/src/libertem.egg-info/PKG-INFO` & `libertem-0.9.2/src/libertem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libertem
-Version: 0.9.0
+Version: 0.9.2
 Summary: Open pixelated STEM framework
 Home-page: https://libertem.github.io/LiberTEM/
 Author: the LiberTEM team
 Author-email: libertem-dev@googlegroups.com
 License: GPL v3
 Keywords: electron microscopy
 Platform: UNKNOWN
```

### Comparing `libertem-0.9.0/src/libertem.egg-info/SOURCES.txt` & `libertem-0.9.2/src/libertem.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -260,14 +260,15 @@
 src/libertem/common/__pycache__/shape.cpython-39.pyc
 src/libertem/common/__pycache__/slice.cpython-39.pyc
 src/libertem/common/numba/__init__.py
 src/libertem/common/numba/cache.py
 src/libertem/common/numba/__pycache__/__init__.cpython-39.pyc
 src/libertem/common/numba/__pycache__/cache.cpython-39.pyc
 src/libertem/contrib/daskadapter.py
+src/libertem/contrib/__pycache__/daskadapter.cpython-37.pyc
 src/libertem/contrib/__pycache__/daskadapter.cpython-38.pyc
 src/libertem/contrib/__pycache__/daskadapter.cpython-39.pyc
 src/libertem/corrections/__init__.py
 src/libertem/corrections/coordinates.py
 src/libertem/corrections/corrset.py
 src/libertem/corrections/detector.py
 src/libertem/corrections/__pycache__/__init__.cpython-39.pyc
@@ -457,19 +458,19 @@
 src/libertem/web/client/favicon.ico
 src/libertem/web/client/index.html
 src/libertem/web/client/manifest.json
 src/libertem/web/client/static/css/2.42a8572e.chunk.css
 src/libertem/web/client/static/css/2.42a8572e.chunk.css.map
 src/libertem/web/client/static/css/main.c0d8de42.chunk.css
 src/libertem/web/client/static/css/main.c0d8de42.chunk.css.map
-src/libertem/web/client/static/js/2.6b575192.chunk.js
-src/libertem/web/client/static/js/2.6b575192.chunk.js.LICENSE.txt
-src/libertem/web/client/static/js/2.6b575192.chunk.js.map
-src/libertem/web/client/static/js/main.2e050bba.chunk.js
-src/libertem/web/client/static/js/main.2e050bba.chunk.js.map
+src/libertem/web/client/static/js/2.909ce721.chunk.js
+src/libertem/web/client/static/js/2.909ce721.chunk.js.LICENSE.txt
+src/libertem/web/client/static/js/2.909ce721.chunk.js.map
+src/libertem/web/client/static/js/main.d79ffbf3.chunk.js
+src/libertem/web/client/static/js/main.d79ffbf3.chunk.js.map
 src/libertem/web/client/static/js/runtime-main.fcac4e81.js
 src/libertem/web/client/static/js/runtime-main.fcac4e81.js.map
 src/libertem/web/client/static/media/LiberTEM logo-medium.2765b438.png
 src/libertem/web/client/static/media/brand-icons.278156e4.woff2
 src/libertem/web/client/static/media/brand-icons.65a2fb6d.ttf
 src/libertem/web/client/static/media/brand-icons.6729d297.svg
 src/libertem/web/client/static/media/brand-icons.cac87dc0.woff
```
