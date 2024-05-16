# Comparing `tmp/document_image_utils-0.1.8.tar.gz` & `tmp/document_image_utils-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "document_image_utils-0.1.8.tar", max compression
+gzip compressed data, was "document_image_utils-0.1.9.tar", max compression
```

## Comparing `document_image_utils-0.1.8.tar` & `document_image_utils-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-03-12 20:00:48.000000 document_image_utils-0.1.8/document_image_utils/__init__.py
--rw-r--r--   0        0        0    11098 2024-05-14 19:43:48.244212 document_image_utils-0.1.8/document_image_utils/box.py
--rw-r--r--   0        0        0    18607 2024-05-14 19:50:06.529737 document_image_utils-0.1.8/document_image_utils/image.py
--rw-r--r--   0        0        0      505 2024-05-14 19:50:29.229792 document_image_utils-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      879 2024-03-15 17:34:42.000000 document_image_utils-0.1.8/README.md
--rw-r--r--   0        0        0     1351 1970-01-01 00:00:00.000000 document_image_utils-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-12 20:00:48.000000 document_image_utils-0.1.9/document_image_utils/__init__.py
+-rw-r--r--   0        0        0    11098 2024-05-14 19:43:48.244212 document_image_utils-0.1.9/document_image_utils/box.py
+-rw-r--r--   0        0        0    25140 2024-05-15 14:43:51.364569 document_image_utils-0.1.9/document_image_utils/image.py
+-rw-r--r--   0        0        0      505 2024-05-15 14:47:49.266181 document_image_utils-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      879 2024-03-15 17:34:42.000000 document_image_utils-0.1.9/README.md
+-rw-r--r--   0        0        0     1351 1970-01-01 00:00:00.000000 document_image_utils-0.1.9/PKG-INFO
```

### Comparing `document_image_utils-0.1.8/document_image_utils/box.py` & `document_image_utils-0.1.9/document_image_utils/box.py`

 * *Files identical despite different names*

### Comparing `document_image_utils-0.1.8/document_image_utils/image.py` & `document_image_utils-0.1.9/document_image_utils/image.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import os
+import time
+from typing import Union
 import cv2
 from .box import *
 from scipy import ndimage
 import numpy as np
 from scipy.signal import *
 from whittaker_eilers import WhittakerSmoother
 from matplotlib import pyplot as plt
@@ -76,53 +78,71 @@
                     pixel_set.append(pixels[i])
         # for same x coordinate, height difference cant be more than 5% of image height
         elif direction == 'none' and pixels[i][0] == pixel_set[-1][0] and (abs(pixels[i][1] - pixel_set[-1][1])/image_shape[0] <= 0.05):
             pixel_set.append(pixels[i])
     return pixel_set
 
 
-def calculate_rotation_direction(image_path:str,line_quantetization:int=200,crop_left:int=50,crop_right:int=0,crop_top:int=100,crop_bottom:int=100,debug:bool=False):
+def calculate_rotation_direction(image:Union[str,cv2.typing.MatLike],line_quantetization:int=200,crop_left:int=0,crop_right:int=0,crop_top:int=0,crop_bottom:int=0,debug:bool=False):
     '''Calculate rotation direction (counter-clockwise or clockwise)
     
     On left margin of image compare the groups of ordered black pixels by x coordinate
     If the largest group is x descending (from top to bottom) the direction is clockwise, else counter-clockwise
     If largest group is of same x coordinate, the direction is none'''
-    test_path = image_path.split('/')[:-1]
-    test_path = '/'.join(test_path)
-    if not os.path.exists(f'{test_path}/test'):
-        os.mkdir(f'{test_path}/test')
-    test_path = f'{test_path}/test/{image_path.split("/")[-1]}'
 
-    direction = 'clockwise'
-    image = cv2.imread(image_path)
+    if isinstance(image,str):
+        image = cv2.imread(image)
+    else:
+        image = image
+
+    if not crop_left:
+        crop_left = round(image.shape[1]*0.05)
+    if not crop_right:
+        crop_right = round(image.shape[1]*0.05)
+    if not crop_top:
+        crop_top = round(image.shape[0]*0.05)
+    if not crop_bottom:
+        crop_bottom = round(image.shape[0]*0.05)
+
+
+    if debug:
+        test_path = '/'.join(image.split('/')[:-1]) if isinstance(image,str) else '.'
+        if not os.path.exists(f'{test_path}/test'):
+            os.mkdir(f'{test_path}/test')
+        test_img_name = image.split("/")[-1] if isinstance(image,str) else 'test'
+        test_path = f'{test_path}/test/{test_img_name}'
+
+    direction = 'None'
     # crop margin
     image = image[crop_top:image.shape[0]-crop_bottom,crop_left:image.shape[1]-crop_right]
     # grey scale
     gray = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
     # binarize, clean salt and pepper noise and dilate
     thresh = cv2.threshold(gray, 0, 255, cv2.THRESH_OTSU + cv2.THRESH_BINARY_INV)[1]
-    filtered = ndimage.median_filter(thresh, 10)
-    dilation = cv2.dilate(filtered, np.ones((0,10),np.uint8),iterations=3)
+    filtered = cv2.medianBlur(thresh, 3)
+    dilation = cv2.dilate(filtered, np.ones((0,20),np.uint8),iterations=3)
     transformed_image = dilation
 
     if debug:
         cv2.imwrite(f'{test_path}_thresh.png',thresh)
         cv2.imwrite(f'{test_path}_filtered.png',filtered)
         cv2.imwrite(f'{test_path}_dilation.png',dilation)
 
+
     # calculate sets
     pixels = []
     step = math.floor(transformed_image.shape[0]/line_quantetization)
 
     for y in range(0,transformed_image.shape[0], step):
         for x in range(transformed_image.shape[1]):
             if transformed_image[y][x] == 255:
                 pixels.append((x,y))
                 break
 
+
     if debug:
     # draw pixels
         copy_image = cv2.imread(f'{test_path}_dilation.png')
         for pixel in pixels:
             cv2.circle(copy_image, pixel, 7, (0,0,255), -1)
         cv2.imwrite(f'{test_path}_pixels.png',copy_image)
 
@@ -142,17 +162,19 @@
 
 
     # find biggest sets
     biggest_clockwise_set = max(clockwise_sets, key=len)
     biggest_counter_clockwise_set = max(counter_clockwise_sets, key=len)
     biggest_same_x_set = max(same_x_sets, key=len)
 
-    print('test','clockwise',len(biggest_clockwise_set))
-    print('counter_clockwise',len(biggest_counter_clockwise_set))
-    print('same_x',len(biggest_same_x_set))
+    if debug:
+        print('test','clockwise',len(biggest_clockwise_set))
+        print('counter_clockwise',len(biggest_counter_clockwise_set))
+        print('same_x',len(biggest_same_x_set))
+
     if debug:
         # draw biggest sets
         for pixel in biggest_clockwise_set:
             cv2.circle(image, pixel, 7, (0,0,255), -1)
         for pixel in biggest_counter_clockwise_set:
             cv2.circle(image, pixel, 7, (0,255,0), -1)
         for pixel in biggest_same_x_set:
@@ -292,15 +314,15 @@
 
 
 
 
 
 
 
-def rotate_image(image:str,line_quantetization:int=100,direction:str='auto',crop_left:int=50,crop_right:int=0,crop_top:int=100,crop_bottom:int=100,debug:bool=False):
+def rotate_image(image:str,line_quantetization:int=None,direction:str='auto',crop_left:int=0,crop_right:int=0,crop_top:int=0,crop_bottom:int=0,debug:bool=False):
     '''Finds the angle of the image and rotates it
     
     Based on the study by: W. Bieniecki, Sz. Grabowski, W. Rozenberg 
     
     Steps:
     1. Crop image
     2. Grey Scale image
@@ -316,38 +338,53 @@
 
     test_path = image.split('/')[:-1]
     test_path = '/'.join(test_path)
     if not os.path.exists(f'{test_path}/test'):
         os.mkdir(f'{test_path}/test')
     test_path = f'{test_path}/test/{image.split("/")[-1]}'
     
-    img = cv2.imread(image)
+    og_img = cv2.imread(image)
+    if not line_quantetization:
+        line_quantetization = round(og_img.shape[0]*0.1)
+
+    if not crop_left:
+        crop_left = round(og_img.shape[1]*0.05)
+    if not crop_right:
+        crop_right = round(og_img.shape[1]*0.05)
+    if not crop_top:
+        crop_top = round(og_img.shape[0]*0.05)
+    if not crop_bottom:
+        crop_bottom = round(og_img.shape[0]*0.05)
+
     # crop margin
-    img = img[crop_top:img.shape[0] - crop_bottom, crop_left:img.shape[1] - crop_right]
-    gray_img = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
+    cut_img = og_img[crop_top:og_img.shape[0] - crop_bottom, crop_left:og_img.shape[1] - crop_right]
+    gray_img = cv2.cvtColor(cut_img, cv2.COLOR_BGR2GRAY)
     binary_img = cv2.threshold(gray_img, 128, 255, cv2.THRESH_OTSU)
 
     # get first black pixel in each line of image
     ## analyses lines acording to line_quantetization
     pixels = []
     step = math.floor(binary_img[1].shape[0]/line_quantetization)
     for y in range(0,binary_img[1].shape[0], step):
         for x in range(binary_img[1].shape[1]):
             if binary_img[1][y][x] == 0:
                 pixels.append((x,y))
                 break
-    
+
     # estimate rotation direction
     if direction == 'auto' or direction not in ['clockwise', 'counter_clockwise']:
-        direction = calculate_rotation_direction(image,crop_left,crop_right,crop_top,crop_bottom, debug=debug)
-    print('direction',direction)
+        direction = calculate_rotation_direction(og_img,crop_left=crop_left,crop_right=crop_right,crop_top=crop_top,crop_bottom=crop_bottom, debug=debug)
+
+    if debug:
+        print('direction',direction)
 
     if direction == 'none':
         return cv2.imread(image)
 
+
     # make list of sets
     # each set is a list of pixels in x coordinates order (ascending or descending depending on rotation direction)
     sets = []
     for i in range(1,len(pixels)-1):
         new_set = create_vertical_aligned_pixel_set(pixels[i:], binary_img[1].shape, direction)
         sets.append(new_set)
 
@@ -355,59 +392,62 @@
     set = []
     # choose set with most elements
     for s in sets:
         if not set:
             set = s
         elif len(s) > len(set):
             set = s
-
-    print('set',len(set))
-    og_img = cv2.imread(image)
-
+    if debug:
+        print('set',len(set))
 
 
     new_set = pixels_set_remove_outliers(set,direction)
 
     if len(new_set) < 2:
-        return img
+        return og_img
     
     # get extreme points
     left_most_point = new_set[0]
     right_most_point = new_set[-1]
     
     # find angle
     angle = math.degrees(math.atan((right_most_point[1] - left_most_point[1]) / (right_most_point[0] - left_most_point[0])))
 
-    print('angle',angle)
+    if debug:
+        print('angle',angle)
 
     rotation_angle = 90 - abs(angle)
     if direction == 'counter_clockwise':
         rotation_angle = -rotation_angle
-    img = ndimage.rotate(og_img, rotation_angle,reshape=True,cval=255)
+
+    h,w = og_img.shape[:2]
+    center = (w // 2, h // 2)
+    rotation_matrix = cv2.getRotationMatrix2D(center, rotation_angle, 1)
+    rotated_img = cv2.warpAffine(og_img, rotation_matrix, (w, h),borderValue=(255, 255, 255))
 
 
     ## test images
     if debug:
-        cv2.imwrite(test_path + '_rotated.png', img)
-
+        cv2.imwrite(test_path + '_rotated.png', rotated_img)
+        img = og_img
         # draw points from set
         for p in set:
-            cv2.circle(og_img, (p[0]+50, p[1]), 7, (255, 0, 0), -1)
+            cv2.circle(img, (p[0]+50, p[1]), 7, (255, 0, 0), -1)
 
-        cv2.imwrite(test_path + '_points_1.png', og_img)
+        cv2.imwrite(test_path + '_points_1.png', img)
 
-        og_img = cv2.imread(image)
+        img = og_img
 
         # draw points from set
         for p in new_set:
-            cv2.circle(og_img, (p[0]+50, p[1]), 7, (255, 0, 0), -1)
+            cv2.circle(img, (p[0]+50, p[1]), 7, (255, 0, 0), -1)
 
-        cv2.imwrite(test_path + '_points.png', og_img)
+        cv2.imwrite(test_path + '_points.png', img)
 
-    return img
+    return rotated_img
         
 
 
 
 def divide_columns(image_path:str,method:str='WhittakerSmoother',logs:bool=False)->list[Box]:
     '''Get areas of columns based on black pixel frequency.\n
     Frequencies are then inverted to find white peaks.
@@ -522,13 +562,161 @@
             for column in potential_columns:
                 c = Box({'left':column[0],'right':column[1],'top':0,'bottom':binarized.shape[0]})
                 columns.append(c)
         
 
     return columns
 
+
+
+
+def cut_document_margins(image_path:str, method:str='WhittakerSmoother', logs:bool=False)->Box:
+    '''
+    Cut document margins by analysing pixel frequency.
     
+    Margins should be great peaks of black pixels followed or preceded (depending on the side) by a great drop in frequency.'''
+
+    cut_document = None
+
+    methods = ['WhittakerSmoother','savgol_filter']
+    if method not in methods:
+        method = 'WhittakerSmoother'
+
+    if not os.path.exists(image_path):
+        print('Image not found')
+        return cut_document
+
+    image = cv2.imread(image_path)
+    cut_document = Box({'left':0,'right':image.shape[1],'top':0,'bottom':image.shape[0]})
+
+    # black and white
+    gray = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
+    # clean noise
+    se=cv2.getStructuringElement(cv2.MORPH_RECT , (8,8))
+    bg=cv2.morphologyEx(gray, cv2.MORPH_DILATE, se)
+    gray=cv2.divide(gray, bg, scale=255)
+    # binarize
+    binarized = cv2.threshold(gray, 0, 255, cv2.THRESH_BINARY_INV + cv2.THRESH_OTSU)[1]
+
+
+    # get frequency of black pixels per column
+    x_axis_freq = np.add.reduce(binarized, axis=0)
+
+    if x_axis_freq.any():
+
+        if method == 'WhittakerSmoother':
+            whittaker_smoother = WhittakerSmoother(lmbda=2e4, order=2, data_length = len(x_axis_freq))
+            x_axis_freq_smooth = whittaker_smoother.smooth(x_axis_freq)
+        elif method == 'savgol_filter':
+            x_axis_freq_smooth = savgol_filter(x_axis_freq, round(len(x_axis_freq)*0.1), 2)
+
+        x_axis_freq_smooth = [i if i > 0 else 0 for i in x_axis_freq_smooth ]
+
+
+        peaks,_ = find_peaks(x_axis_freq_smooth,prominence=0.2*(max(x_axis_freq_smooth)- min(x_axis_freq_smooth)))
+        
+
+        x_axis_freq_smooth = np.array(x_axis_freq_smooth)
+
+        # average of frequency
+        average_smooth_frequency = np.average(x_axis_freq_smooth)
+
+        if logs:
+            
+            # create 4 plots
+            plt.subplot(2, 2, 1)
+            plt.plot(peaks, x_axis_freq[peaks], "ob"); plt.plot(x_axis_freq); plt.legend(['prominence'])
+            plt.title('Frequency')
+
+
+            plt.subplot(2, 2, 2)
+            plt.plot(peaks, x_axis_freq_smooth[peaks], "ob"); plt.plot(x_axis_freq_smooth); plt.legend(['prominence'])
+            # average line
+            plt.plot([0,len(x_axis_freq_smooth)], [average_smooth_frequency, average_smooth_frequency], "r--");
+            plt.title('Frequency Smooth')
+
+            # binarized image
+            plt.subplot(2, 2, 3)
+            plt.imshow(binarized, cmap='gray')
+            plt.title('Binarized Image')
+
+            plt.show()
+
+        if logs:
+            print('Peaks',peaks)
+
+
+        if peaks.any():
+
+            # get left and right margins potential peaks
+                # they need to be between out of the 10% to 90% range of the x axis of the image
+            left_margin = peaks[0] if peaks[0] <= len(x_axis_freq_smooth)*0.1 else None
+            right_margin = None if len(peaks) == 1 else peaks[-1] if peaks[-1] >= len(x_axis_freq_smooth)*0.9 else None
+
+            if logs:
+                print('left margin',left_margin)
+                print('right margin',right_margin)
+
+            max_freq = max(x_axis_freq_smooth)
+            # check left margin
+            if left_margin:
+
+                # peak needs to be followed by a drop to less than 10% of max frequency
+                last_point = left_margin
+                i = last_point + 1
+                while i <= len(x_axis_freq_smooth)*0.1 and x_axis_freq_smooth[i] < x_axis_freq_smooth[last_point] :
+                    last_point = i
+                    i += 1
+
+
+                if logs:
+                    print('lowest point',last_point)
+                    print(x_axis_freq_smooth[last_point])
+
+                if x_axis_freq_smooth[last_point] <= max_freq*0.1:
+                    left_margin = last_point
+                else:
+                    left_margin = 0
+            else: 
+                left_margin = 0
+
+            # check right margin
+            if right_margin:
+
+                # peak needs to be preceded by a drop to less than 10% of max frequency
+                last_point = right_margin
+                i = last_point - 1
+                while i >= len(x_axis_freq_smooth)*0.9 and x_axis_freq_smooth[i] < x_axis_freq_smooth[last_point] :
+                    last_point = i
+                    i -= 1
+
+                if logs:
+                    print('lowest point',last_point)
+                    print(x_axis_freq_smooth[last_point])
+
+                if x_axis_freq_smooth[last_point] <= max_freq*0.1:
+                    right_margin = last_point
+                else:
+                    right_margin = len(x_axis_freq_smooth)
+            else: 
+                right_margin = len(x_axis_freq_smooth)
+
+            if logs:
+                print('Left margin',left_margin)
+                print('Right margin',right_margin)
+
+                # draw plot with left and right margins
+                plt.imshow(binarized, cmap='gray')
+
+                if left_margin:
+                    plt.plot([left_margin,left_margin], [0,binarized.shape[0]], "r--");
+                if right_margin:
+                    plt.plot([right_margin,right_margin], [0,binarized.shape[0]], "r--");
+                
 
+                plt.show()
 
 
+            cut_document = Box(left_margin,right_margin,0,binarized.shape[0])
 
+    return cut_document
```

### Comparing `document_image_utils-0.1.8/README.md` & `document_image_utils-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `document_image_utils-0.1.8/PKG-INFO` & `document_image_utils-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: document_image_utils
-Version: 0.1.8
+Version: 0.1.9
 Summary: Toolkit for document image processing
 Author: Gonçalo Afonso
 Author-email: brazafonso2001@gmail.com
 Requires-Python: >=3.10.11,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

