# Comparing `tmp/motionSegmentation-2.8.8.tar.gz` & `tmp/motionsegmentation-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motionSegmentation-2.8.8.tar", last modified: Wed Aug  4 08:15:58 2021, max compression
+gzip compressed data, was "motionsegmentation-2.9.0.tar", last modified: Thu May 16 06:41:22 2024, max compression
```

## Comparing `motionSegmentation-2.8.8.tar` & `motionsegmentation-2.9.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 yaplab    (1000) yaplab    (1000)        0 2021-08-04 08:15:58.281458 motionSegmentation-2.8.8/
--rw-rw-r--   0 yaplab    (1000) yaplab    (1000)      738 2021-08-04 08:15:58.281458 motionSegmentation-2.8.8/PKG-INFO
--rw-rw-r--   0 yaplab    (1000) yaplab    (1000)     3692 2021-08-04 08:05:24.000000 motionSegmentation-2.8.8/README.md
-drwxrwxr-x   0 yaplab    (1000) yaplab    (1000)        0 2021-08-04 08:15:58.281458 motionSegmentation-2.8.8/motionSegmentation/
--rw-rw-r--   0 yaplab    (1000) yaplab    (1000)   118580 2021-08-04 08:05:24.000000 motionSegmentation-2.8.8/motionSegmentation/BsplineFourier.py
--rw-rw-r--   0 yaplab    (1000) yaplab    (1000)    26970 2021-08-04 08:05:24.000000 motionSegmentation-2.8.8/motionSegmentation/__init__.py
--rw-rw-r--   0 yaplab    (1000) yaplab    (1000)    78666 2021-08-04 08:05:24.000000 motionSegmentation-2.8.8/motionSegmentation/bfSolver.py
--rw-rw-r--   0 yaplab    (1000) yaplab    (1000)    30300 2021-08-04 08:05:24.000000 motionSegmentation-2.8.8/motionSegmentation/motionCorrect.py
--rw-rw-r--   0 yaplab    (1000) yaplab    (1000)    28203 2021-08-04 08:05:24.000000 motionSegmentation-2.8.8/motionSegmentation/segment.py
-drwxrwxr-x   0 yaplab    (1000) yaplab    (1000)        0 2021-08-04 08:15:58.281458 motionSegmentation-2.8.8/motionSegmentation.egg-info/
--rw-rw-r--   0 yaplab    (1000) yaplab    (1000)      738 2021-08-04 08:15:58.000000 motionSegmentation-2.8.8/motionSegmentation.egg-info/PKG-INFO
--rw-rw-r--   0 yaplab    (1000) yaplab    (1000)      402 2021-08-04 08:15:58.000000 motionSegmentation-2.8.8/motionSegmentation.egg-info/SOURCES.txt
--rw-rw-r--   0 yaplab    (1000) yaplab    (1000)        1 2021-08-04 08:15:58.000000 motionSegmentation-2.8.8/motionSegmentation.egg-info/dependency_links.txt
--rw-rw-r--   0 yaplab    (1000) yaplab    (1000)       42 2021-08-04 08:15:58.000000 motionSegmentation-2.8.8/motionSegmentation.egg-info/requires.txt
--rw-rw-r--   0 yaplab    (1000) yaplab    (1000)       19 2021-08-04 08:15:58.000000 motionSegmentation-2.8.8/motionSegmentation.egg-info/top_level.txt
--rw-rw-r--   0 yaplab    (1000) yaplab    (1000)       79 2021-08-04 08:15:58.281458 motionSegmentation-2.8.8/setup.cfg
--rw-rw-r--   0 yaplab    (1000) yaplab    (1000)     1628 2021-08-04 08:05:24.000000 motionSegmentation-2.8.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 06:41:22.455507 motionsegmentation-2.9.0/
+-rw-rw-rw-   0        0        0     1067 2024-05-16 06:40:14.000000 motionsegmentation-2.9.0/LICENSE
+-rw-rw-rw-   0        0        0     5773 2024-05-16 06:41:22.455507 motionsegmentation-2.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3692 2024-05-16 06:40:14.000000 motionsegmentation-2.9.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 06:41:22.439869 motionsegmentation-2.9.0/motionSegmentation/
+-rw-rw-rw-   0        0        0   118580 2024-05-16 06:40:14.000000 motionsegmentation-2.9.0/motionSegmentation/BsplineFourier.py
+-rw-rw-rw-   0        0        0    30532 2024-05-16 06:40:14.000000 motionsegmentation-2.9.0/motionSegmentation/__init__.py
+-rw-rw-rw-   0        0        0    79657 2024-05-16 06:40:14.000000 motionsegmentation-2.9.0/motionSegmentation/bfSolver.py
+-rw-rw-rw-   0        0        0    30300 2024-05-16 06:40:14.000000 motionsegmentation-2.9.0/motionSegmentation/motionCorrect.py
+-rw-rw-rw-   0        0        0    28203 2024-05-16 06:40:14.000000 motionsegmentation-2.9.0/motionSegmentation/segment.py
+drwxrwxrwx   0        0        0        0 2024-05-16 06:41:22.455507 motionsegmentation-2.9.0/motionSegmentation.egg-info/
+-rw-rw-rw-   0        0        0     5773 2024-05-16 06:41:22.000000 motionsegmentation-2.9.0/motionSegmentation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      406 2024-05-16 06:41:22.000000 motionsegmentation-2.9.0/motionSegmentation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 06:41:22.000000 motionsegmentation-2.9.0/motionSegmentation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-05-16 06:41:22.000000 motionsegmentation-2.9.0/motionSegmentation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-16 06:41:22.000000 motionsegmentation-2.9.0/motionSegmentation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1159 2024-05-16 06:40:14.000000 motionsegmentation-2.9.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-16 06:41:22.455507 motionsegmentation-2.9.0/setup.cfg
```

### Comparing `motionSegmentation-2.8.8/README.md` & `motionsegmentation-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `motionSegmentation-2.8.8/motionSegmentation/BsplineFourier.py` & `motionsegmentation-2.9.0/motionSegmentation/BsplineFourier.py`

 * *Files identical despite different names*

### Comparing `motionSegmentation-2.8.8/motionSegmentation/__init__.py` & `motionsegmentation-2.9.0/motionSegmentation/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -165,28 +165,40 @@
 Author: w.x.chan@gmail.com    04Aug2021                - v2.8.8   
                                 -added imgfmt to simpleSolver 
                                 - added automatic anchor
                         -bfSolver version 2.8.0
                         -BsplineFourier version 2.7.14
                         -motionCorrect version 2.7.8
                         -segment verion 2.7.19
+Author: w.x.chan@gmail.com    17Sep2021                - v2.8.9   
+                                -added changeGreyscaleFormat in simpleSolver
+                        -bfSolver version 2.8.0
+                        -BsplineFourier version 2.7.14
+                        -motionCorrect version 2.7.8
+                        -segment verion 2.7.19
+Author: w.x.chan@gmail.com    13May2024                - v2.9.0   
+                                -added multiresolution level for time (multiTimeRes)
+                        -bfSolver version 2.8.0
+                        -BsplineFourier version 2.7.14
+                        -motionCorrect version 2.7.8
+                        -segment verion 2.7.19
 Requirements:
     autoD
     numpy
     re
     scipy
     BsplineFourier
     pickle (optional)
     nfft
 
 Known Bug:
     HSV color format not supported
 All rights reserved.
 '''
-_version='2.8.8'
+_version='2.9.0'
 import logging
 logger = logging.getLogger('motionSegmentation v'+_version)
 logger.info('motionSegmentation version '+_version)
 
 import os
 import sys
 import numpy as np
@@ -194,30 +206,34 @@
 import motionSegmentation.BsplineFourier as BsplineFourier
 import motionSegmentation.bfSolver as bfSolver
 import motionSegmentation.segment as segment
 from skimage.segmentation import watershed
 import medImgProc as mip
 import medImgProc.processFunc as pf
 import time
+try:
+    import trimesh
+except:
+    pass
 
-def simpleSolver(savePath,startstep=1,endstep=7,fileScale=None,getCompoundTimeList=None,compoundSchemeList=None,fftLagrangian=True,pngFileFormat=None,period=None,maskImg=True,anchor=None,bgrid=4.,finalShape=None,fourierTerms=4,twoD=False,imgfmt=None):
+def simpleSolver(savePath,startstep=1,endstep=7,fileScale=None,getCompoundTimeList=None,compoundSchemeList=None,fftLagrangian=True,pngFileFormat=None,period=None,maskImg=True,anchor=None,bgrid=4.,finalShape=None,fourierTerms=4,twoD=False,imgfmt=None,multiTimeRes=0):
     '''
     step 1: load image
     step 2: create mask
     step 3: Registrations
     step 4: initialize BSF using fft
     step 5: solve BSF
     step 6: regrid to time
     setp 7: compute compound
     '''
     logging.info(savePath)
     allTime=[]
     allTimeHeader=""
-    imregPath=savePath+'/transform/'
     regfile_general='t{0:d}to{1:d}_0.txt'
+    imregPath=savePath+'/transform/'
     saveName='RMSmotion_smooth'
     if anchor is None:
         anchor=[]
     if fileScale is None:
         try:
             fileScale=np.loadtxt(imregPath+'fileScale.txt')
         except:
@@ -249,22 +265,24 @@
         else:
             image=mip.loadStack(savePath+'/'+pngFileFormat,dimension=['t','z'],n=1)
             image.dimlen['x']=imagedim[0]
             image.dimlen['y']=imagedim[1]
             image.dimlen['z']=imagedim[2]
             image.dimlen['t']=1.
             image.rearrangeDim(['t','z','y','x'])
+        if 'RGB' in image.dim:
+            image.changeGreyscaleFormat(colorFormat='RGB')
         if imgfmt is not None:
             image.data=image.data.astype(imgfmt)
         image.save(savePath+'/img')
         
     if startstep<=2 and endstep>=2:
         if maskImg:
             image=mip.load(savePath+'/img')
-            maskImg=image.clone()
+            maskImage=image.clone()
             mask=np.zeros(image.data.shape)
             mask[image.data==0]=1
             mask=np.prod(mask,axis=0)
             if twoD:
                 mask=np.tile(mask,(image.data.shape[0],1,1))
                 border=np.ones(mask.shape[1:]).astype(bool)
                 border[tuple([slice(1,-1)]*len(mask.shape[1:]))]=False
@@ -286,39 +304,36 @@
                         ws=watershed(mask[t,z])
                         for n in range(ws.max()):
                             if np.count_nonzero(ws==n)>0:
                                if mask[t,z][ws==n].mean()>=0.5 and not(np.any(border*ws==n)):
                                     mask[t,z][ws==n]=0
                         mask[t,z]=segment.detectNonregularBoundary(image.data[t,z].copy(),iterations=30,initArray=mask[t,z])
                         mask[t,z]=morphology.binary_erosion(mask[t,z],iterations=2,border_value=0)
-            maskImg.data=mask
-            maskImg.save(savePath+'/maskBorderImg')
-    
-    
+            maskImage.data=mask
+            maskImage.save(savePath+'/maskBorderImg')
+  
     if startstep<=3 and endstep>=3:
         image=mip.load(savePath+'/img')
         timestepNo=image.data.shape[0]
-        timeList=np.arange(timestepNo)
-        timestep=timeList[1]
         if maskImg:
             if type(maskImg)==str:
-                maskImg=mip.load(savePath+'/'+maskImg).data
+                maskImage=mip.load(savePath+'/'+maskImg).data
             else:
-                maskImg=mip.load(savePath+'/maskBorderImg').data.astype(float)
+                maskImage=mip.load(savePath+'/maskBorderImg').data.astype(float)
         else:
-            maskImg=None
+            maskImage=None
         startTime=time.process_time()
         if twoD:
             setOrigin=(0.,0.)
         else:
             setOrigin=(0.,0.,0.)
         if fftLagrangian:
-            pf.TmapRegister(image,savePath=savePath,origin=setOrigin,bgrid=bgrid,bweight=1.,rms=True,startTime=0,scaleImg=fileScale,maskArray=maskImg,twoD=twoD,cyclic=False)
+            pf.TmapRegister(image,savePath=savePath,origin=setOrigin,bgrid=bgrid,bweight=1.,rms=True,startTime=0,scaleImg=fileScale,maskArray=maskImage,twoD=twoD,cyclic=False)
         else:
-            pf.TmapRegister(image,savePath=savePath,origin=setOrigin,bgrid=bgrid,bweight=1.,rms=True,startTime=0,scaleImg=fileScale,maskArray=maskImg,twoD=twoD,cyclic=True)
+            pf.TmapRegister(image,savePath=savePath,origin=setOrigin,bgrid=bgrid,bweight=1.,rms=True,startTime=0,scaleImg=fileScale,maskArray=maskImage,twoD=twoD,cyclic=True)
         if anchor is not None:
             for n in range(len(anchor)):
                 if len(anchor[n])==4:
                     image1=mip.load(anchor[n][2])
                     image2=mip.load(anchor[n][3])
                     pf.TmapRegister_img2img(image1,image2,savePath=savePath,fileName='manual_'+regfile_general[:-4].format(anchor[n][0],anchor[n][1]),scaleImg=fileScale,rms=True,bgrid=bgrid,bweight=1.,twoD=twoD)
         regTime=time.process_time()-startTime
@@ -326,51 +341,88 @@
         allTimeHeader+="registrationTime,"
         
     if startstep<=4 and endstep>=4:
         image=mip.load(savePath+'/img')
         timestepNo=image.data.shape[0]
         timeList=np.arange(timestepNo)
         timestep=timeList[1]
-        timeMapList=[]
-        fileList=[]
-        for n in range(timestepNo-1):
-            timeMapList.append([timeList[n],timeList[n+1]])
-            fileList.append(imregPath+regfile_general.format(n,n+1))
-        timeMapList.append([timeList[-1],timeList[0]])
-        fileList.append(imregPath+regfile_general.format(timestepNo-1,0))
-    
-        timeMapList.append([timeList[0],timeList[-1]])
-        fileList.append(imregPath+regfile_general.format(0,timestepNo-1))
-        for n in range(timestepNo-1,0,-1):
-            timeMapList.append([timeList[n],timeList[n-1]])
-            fileList.append(imregPath+regfile_general.format(n,n-1))
-    
-        timeMapList2=[]
-        fileList2=[]
-        for n in range(timestepNo):
-            if n!=0:
-                timeMapList2.append([0,timeList[n]])
-                fileList2.append(imregPath+regfile_general.format(0,n))
-        if period is None:
-            period=timestep*timestepNo
-        
-        solver=bfSolver.bfSolver()
-        startTime=time.process_time()###
-        if fftLagrangian:
-            solver.addBsplineFile(fileList2+fileList[:timestepNo-1],timeMapList=timeMapList2+timeMapList[:timestepNo-1],fileScale=fileScale)
-            solver.initialize(shape=finalShape,period=period,fourierTerms=fourierTerms,spacingDivision=2.)
-            solver.estimateInitialwithRefTime(timestepNo-1,OrderedBsplinesList2=range(timestepNo-1,2*(timestepNo-1)),spacingDivision=2.,gap=0)
+        if multiTimeRes>0:
+            if period is None:
+                period=timestepNo
+            os.makedirs(savePath+'/multiTimeRes',exist_ok=True)
+            image=image.data[::2]
+            image.dimlen['t']=image.dimlen['t']*2
+            image.save(savePath+'/multiTimeRes/img')
+            if maskImg:
+                if type(maskImg)==str:
+                    maskImage=mip.load(savePath+'/'+maskImg)
+                else:
+                    maskImage=mip.load(savePath+'/maskBorderImg')
+                maskImage=maskImage.data[::2]
+                maskImage.dimlen['t']=maskImage.dimlen['t']*2
+                if type(maskImg)==str:
+                    maskImage.save(savePath+'/multiTimeRes/'+maskImg)
+                else:
+                    maskImage.save(savePath+'/multiTimeRes/maskBorderImg')
+            simpleSolver_dict={'fileScale':fileScale,
+                              'getCompoundTimeList':None,
+                              'compoundSchemeList':None,
+                              'fftLagrangian':fftLagrangian,
+                              'pngFileFormat':None,
+                              'period':period,
+                              'maskImg':maskImg,
+                              'anchor':None,
+                              'bgrid':bgrid,
+                              'finalShape':finalShape,
+                              'fourierTerms':fourierTerms,
+                              'twoD':twoD,
+                              'imgfmt':imgfmt,
+                              'multiTimeRes':multiTimeRes-1}
+            simpleSolver(savePath+'/multiTimeRes',startstep=3,endstep=5,**simpleSolver_dict)
+            bsFourier=BsplineFourier.BsplineFourier(savePath+'/multiTimeRes/'+saveName+'_f'+str(fourierTerms)+'.txt')
+            bsFourier.writeCoef(savePath+'/'+saveName+'_fft.txt')
+            del bsFourier
         else:
-            solver.addBsplineFile(fileList,timeMapList=timeMapList,fileScale=fileScale)
-            solver.initialize(shape=finalShape,period=period,fourierTerms=fourierTerms,spacingDivision=2.)
-            solver.estimateInitialwithRefTime(timestepNo-1,OrderedBsplinesList2=range(timestepNo,len(fileList)-1),spacingDivision=2.,gap=0,forwardbackward=True)
-        mtinitTime=time.process_time()-startTime
-        solver.bsFourier.writeCoef(savePath+'/'+saveName+'_fft.txt')
-        allTime.append(mtinitTime)
-        allTimeHeader+="motiontrackinginitTime,"
+            timeMapList=[]
+            fileList=[]
+            for n in range(timestepNo-1):
+                timeMapList.append([timeList[n],timeList[n+1]])
+                fileList.append(imregPath+regfile_general.format(n,n+1))
+            timeMapList.append([timeList[-1],timeList[0]])
+            fileList.append(imregPath+regfile_general.format(timestepNo-1,0))
+    
+            timeMapList.append([timeList[0],timeList[-1]])
+            fileList.append(imregPath+regfile_general.format(0,timestepNo-1))
+            for n in range(timestepNo-1,0,-1):
+                timeMapList.append([timeList[n],timeList[n-1]])
+                fileList.append(imregPath+regfile_general.format(n,n-1))
+    
+            timeMapList2=[]
+            fileList2=[]
+            for n in range(timestepNo):
+                if n!=0:
+                    timeMapList2.append([0,timeList[n]])
+                    fileList2.append(imregPath+regfile_general.format(0,n))
+            if period is None:
+                period=timestep*timestepNo
+        
+            solver=bfSolver.bfSolver()
+            startTime=time.process_time()###
+            if fftLagrangian:
+                solver.addBsplineFile(fileList2+fileList[:timestepNo-1],timeMapList=timeMapList2+timeMapList[:timestepNo-1],fileScale=fileScale)
+                solver.initialize(shape=finalShape,period=period,fourierTerms=fourierTerms,spacingDivision=2.)
+                solver.estimateInitialwithRefTime(timestepNo-1,OrderedBsplinesList2=range(timestepNo-1,2*(timestepNo-1)),spacingDivision=2.,gap=0)
+            else:
+                solver.addBsplineFile(fileList,timeMapList=timeMapList,fileScale=fileScale)
+                solver.initialize(shape=finalShape,period=period,fourierTerms=fourierTerms,spacingDivision=2.)
+                solver.estimateInitialwithRefTime(timestepNo-1,OrderedBsplinesList2=range(timestepNo,len(fileList)-1),spacingDivision=2.,gap=0,forwardbackward=True)
+            mtinitTime=time.process_time()-startTime
+            solver.bsFourier.writeCoef(savePath+'/'+saveName+'_fft.txt')
+            allTime.append(mtinitTime)
+            allTimeHeader+="motiontrackinginitTime,"
     
     if startstep<=5 and endstep>=5:
         image=mip.load(savePath+'/img')
         timestepNo=image.data.shape[0]
         timeList=np.arange(timestepNo)
         timestep=timeList[1]
         timeMapList=[]
@@ -458,40 +510,40 @@
     if startstep<=7 and endstep>=7:
         allTime=[]
         allTimeHeader=""
         image=mip.load(savePath+'/img')
         image.data=image.data.astype(float)
         timestepNo=image.data.shape[0]
         if maskImg:
-            maskImg=mip.load(savePath+'/maskBorderImg')
-            maskImg.data=maskImg.data.astype(float)
+            maskImage=mip.load(savePath+'/maskBorderImg')
+            maskImage.data=maskImage.data.astype(float)
         
         syncTime=[]
         syncMaskTime=[]
         SACTime=[]
         maxTime=[]
         meanTime=[]
         waveletTime=[]
         SACmaxTime=[]
         SACmeanTime=[]
         for t in getCompoundTimeList:
             
             syncImg=image.clone()
             if maskImg:
-                syncMask=maskImg.clone()
+                syncMask=maskImage.clone()
             syncMaskTime.append([])
             syncTime.append([])
             for t2 in range(image.data.shape[0]):
                 if t2!=t:
                     startTime=time.process_time()###
                     syncImg.data[t2]=pf.transform_img2img(image.data[t2].copy(),savePath+r'/bsfTransform/t'+str(t)+'to'+str(t2)+'.txt',savePath=savePath+'/'+str(t),scale=np.array([image.dimlen['x'],image.dimlen['y'],image.dimlen['z']]))
                     syncTime[-1].append(time.process_time()-startTime)###
                     if maskImg:
                         startTime=time.process_time()###
-                        syncMask.data[t2]=pf.transform_img2img(maskImg.data[t2].copy(),savePath+r'/bsfTransform/t'+str(t)+'to'+str(t2)+'.txt',savePath=savePath+'/'+str(t),scale=np.array([maskImg.dimlen['x'],maskImg.dimlen['y'],maskImg.dimlen['z']]))
+                        syncMask.data[t2]=pf.transform_img2img(maskImage.data[t2].copy(),savePath+r'/bsfTransform/t'+str(t)+'to'+str(t2)+'.txt',savePath=savePath+'/'+str(t),scale=np.array([maskImage.dimlen['x'],maskImage.dimlen['y'],maskImage.dimlen['z']]))
                         syncMaskTime[-1].append(time.process_time()-startTime)###
             syncTime[-1]=np.sum(syncTime[-1])
             syncMaskTime[-1]=np.sum(syncMaskTime[-1])
             syncImg.save(savePath+'/SRimg_sync_t'+str(t))
             
             if maskImg:
                 syncMask.data=np.maximum(0,np.minimum(1,syncMask.data))
@@ -536,8 +588,23 @@
                         compoundImg.data[np.isnan(compoundImg.data)]=0
                     compoundImg.save(savePath+'/SRimg_'+compoundstr+'_t'+str(t))
 
     
         allTime=np.array([np.mean(syncTime),np.mean(syncMaskTime),np.mean(SACTime),np.mean(SACTime)+np.mean(SACmaxTime),np.mean(SACTime)+np.mean(SACmeanTime),np.mean(maxTime),np.mean(meanTime),np.mean(waveletTime)])
         allTime=allTime/np.prod(image.data.shape[1:])*(10.**6.)
         np.savetxt(savePath+'/computationalTime.txt',allTime.reshape((1,-1)),header='syncTime,syncMaskTime,SACTime,SACmaxTime,SACmeanTime,maxTime,meanTime,waveletTime\n'+' microsecond per pixel ,image shape = '+repr(image.data.shape))
-    
+
+def get_stls(savePath,bsf_file,file_scale,stl_file,getTimeList=None):
+    mesh=trimesh.load_mesh(stl_file) 
+    os.makedirs(savePath,exist_ok=True)
+    #solver=bfSolver.bfSolver()
+    #solver.loadSamplingResults(os.path.join(casePath,training_folder,bsf_file[:-4]+'_samplingResults.txt'))
+    bsf=BsplineFourier(bsf_file)#.regridToTime(solver.points,solver.pointsCoef,stl_time)
+    stl0_coords=np.array(mesh.vertices)[:,0:3]
+    if getTimeList is None:
+        getTimeList=range(int(bsf.spacing[-1]))
+    for n in getTimeList:
+        new_coords=stl0_coords+bsf.getVector(np.concatenate((stl0_coords,stl0_coords[...,0:1]*0.+n),axis=-1))
+        mesh.vertices[:]=new_coords[:]
+        mesh.export(os.path.join(savePath,'t'+str(n)+'.stl'))
+        
+
```

### Comparing `motionSegmentation-2.8.8/motionSegmentation/bfSolver.py` & `motionsegmentation-2.9.0/motionSegmentation/bfSolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -347,16 +347,35 @@
         '''
         if method=='pointbypoint':
             sampleCoefList,rmsList=self.solve_pointbypoint(maxError=maxError,tRef=tRef,maxIteration=maxIteration,convergence=convergence,reportevery=reportevery,tempSave=tempSave,resume=resume)
             if type(rmsBasedWeighted)==type(None):
                 rmsweight=None
             else:
                 rmsweight=rmsBasedWeighted(rmsList)
+        elif method='pointbypoint_exact1':
+            sampleCoefList=self.solve_pointbypoint_exact1()
+            rmsweight=None
         self.bsFourier.regrid(self.points,sampleCoefList,weight=rmsweight,linearConstrainPoints=linearConstrainPoints,linearConstrainWeight=linearConstrainWeight)
         logger.info('BsplineFourier updated')
+    def solve_pointbypoint_exact1(self):
+        ''' 
+        Solves for the bsplineFourier with 1 cos coeficient only and bspline that goes starts from 0
+        '''
+        self.pointsCoef=[]
+        for m in range(len(self.pointsCoef),len(self.points)):
+            if self.bsplines[0].timeMap[0]!=0:
+                raise Exception("solver pointbypoint_exact1 is only avaliable for bspline maping from time 0.")
+            coef=self.bsFourier.getRefCoef(self.points[m])
+            V=np.array(self.bsplines[0].getVector(self.points[m]))
+            coscoef=V/(np.cos(2.*np.pi/self.bsFourier.spacing[-1]*self.bsplines[0].timeMap[1])-np.cos(2.*np.pi/self.bsFourier.spacing[-1]*self.bsplines[0].timeMap[0]))
+            coef[0]=0
+            coef[1]=coscoef
+            coef[2]=0
+            self.pointsCoef.append(coef.copy())
+        return self.pointsCoef
   
     def solve_pointbypoint(self,tRef=None,maxError=0.00001,maxIteration=1000,convergence=0.8,reportevery=1000,tempSave=None,resume=False,movAvgError=False,lmLambda_init=0.001,lmLambda_incrRatio=5.,lmLambda_max=float('inf'),lmLambda_min=0.00001):
         ''' 
         Solves for the bsplineFourier
         Parameters:
             maxError: float
                 maximum change in coefficients of bsplinefourier to consider converged
```

### Comparing `motionSegmentation-2.8.8/motionSegmentation/motionCorrect.py` & `motionsegmentation-2.9.0/motionSegmentation/motionCorrect.py`

 * *Files identical despite different names*

### Comparing `motionSegmentation-2.8.8/motionSegmentation/segment.py` & `motionsegmentation-2.9.0/motionSegmentation/segment.py`

 * *Files identical despite different names*

