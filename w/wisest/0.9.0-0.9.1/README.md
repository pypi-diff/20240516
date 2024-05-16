# Comparing `tmp/wisest-0.9.0-py3-none-any.whl.zip` & `tmp/wisest-0.9.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 6766 bytes, number of entries: 13
+Zip file size: 6768 bytes, number of entries: 13
 -rw-r--r--  2.0 unx      452 b- defN 80-Jan-01 00:00 wise/__init__.py
 -rw-r--r--  2.0 unx     1368 b- defN 80-Jan-01 00:00 wise/cli.py
--rw-r--r--  2.0 unx      771 b- defN 80-Jan-01 00:00 wise/cost.py
+-rw-r--r--  2.0 unx      786 b- defN 80-Jan-01 00:00 wise/cost.py
 -rw-r--r--  2.0 unx      583 b- defN 80-Jan-01 00:00 wise/currency.py
 -rw-r--r--  2.0 unx     2157 b- defN 80-Jan-01 00:00 wise/method.py
 -rw-r--r--  2.0 unx     3696 b- defN 80-Jan-01 00:00 wise/price.py
 -rw-r--r--  2.0 unx     1707 b- defN 80-Jan-01 00:00 wise/rate.py
 -rw-r--r--  2.0 unx       79 b- defN 80-Jan-01 00:00 wise/request.py
--rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 wisest-0.9.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      544 b- defN 80-Jan-01 00:00 wisest-0.9.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 wisest-0.9.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       37 b- defN 80-Jan-01 00:00 wisest-0.9.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      943 b- defN 16-Jan-01 00:00 wisest-0.9.0.dist-info/RECORD
-13 files, 13491 bytes uncompressed, 5224 bytes compressed:  61.3%
+-rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 wisest-0.9.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      544 b- defN 80-Jan-01 00:00 wisest-0.9.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 wisest-0.9.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       37 b- defN 80-Jan-01 00:00 wisest-0.9.1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      943 b- defN 16-Jan-01 00:00 wisest-0.9.1.dist-info/RECORD
+13 files, 13506 bytes uncompressed, 5226 bytes compressed:  61.3%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: wise/rate.py
 Comment: 
 
 Filename: wise/request.py
 Comment: 
 
-Filename: wisest-0.9.0.dist-info/LICENSE
+Filename: wisest-0.9.1.dist-info/LICENSE
 Comment: 
 
-Filename: wisest-0.9.0.dist-info/METADATA
+Filename: wisest-0.9.1.dist-info/METADATA
 Comment: 
 
-Filename: wisest-0.9.0.dist-info/WHEEL
+Filename: wisest-0.9.1.dist-info/WHEEL
 Comment: 
 
-Filename: wisest-0.9.0.dist-info/entry_points.txt
+Filename: wisest-0.9.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: wisest-0.9.0.dist-info/RECORD
+Filename: wisest-0.9.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wise/cost.py

```diff
@@ -4,13 +4,13 @@
 def print_cost(price: Price, card_fee_percent: float = 1.5, reward_rate: float = 0.1) -> None:
     card_fee = price.source_amount * card_fee_percent / 100
     wise_fee_percent = 100 * price.total / price.source_amount
     fee = card_fee + price.total
     fee_percent = 100 * fee / (price.source_amount + card_fee)
     cost_per_mile = fee / (price.source_amount * reward_rate)
     print(
-        f"Add {price.target_amount:.2f} { price.target_currency}"
-        f", pay {price.source_amount:.2f} {price.source_currency}"
-        f", wise fee: {price.total:.2f} {price.source_currency} ({wise_fee_percent:.2f}%)"
-        f", total fee: {fee:.2f} {price.source_currency} ({fee_percent:.2f}%)"
+        f"Add {price.target_amount: >10.2f} {price.target_currency}"
+        f", pay {price.source_amount: >10.2f} {price.source_currency}"
+        f", wise fee: {price.total: >10.2f} {price.source_currency} ({wise_fee_percent:.2f}%)"
+        f", total fee: {fee: >10.2f} {price.source_currency} ({fee_percent:.2f}%)"
         f", cost per mile: {cost_per_mile:.4f}"
     )
```

## Comparing `wisest-0.9.0.dist-info/LICENSE` & `wisest-0.9.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `wisest-0.9.0.dist-info/METADATA` & `wisest-0.9.1.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wisest
-Version: 0.9.0
+Version: 0.9.1
 Summary: 
 Author: narumi
 Author-email: toucans-cutouts0f@icloud.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

## Comparing `wisest-0.9.0.dist-info/RECORD` & `wisest-0.9.1.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 wise/__init__.py,sha256=uIH9gdfABknJMDYbFqSdOddBie4c3QjpWORlQaM3DGg,452
 wise/cli.py,sha256=16pfJKwmLQD-hP6jvpEPHj7I8iqfJV3G-YTU2HOg1p8,1368
-wise/cost.py,sha256=dGTtJSaGcBFk1dg8In12TkYK7coxkYTQ27X5U497yng,771
+wise/cost.py,sha256=eEY96I9a0Ephvy0eGjWv9yfJj2A8zGm2SH1mqO3lQzA,786
 wise/currency.py,sha256=V8AaX8jW3cfpRbT0MdSvbV8Sk25eW1Pv7jR-cMr7au8,583
 wise/method.py,sha256=zUVJvML08O_X2ifou0AKLe66RE8AM2i14Q7qAntpntY,2157
 wise/price.py,sha256=64QblEsUScRRj8CRYYfWOd-EFJmhaDHBBdLp_i1lo5g,3696
 wise/rate.py,sha256=VuIZW2bhEm3Dx81cMJwh-ALyt11YCiOUYPU1aOtDIOU,1707
 wise/request.py,sha256=iqGS-XJLlBBG0Z6zh_QDuG0z0f4UY9E4Cme5-fUIxbQ,79
-wisest-0.9.0.dist-info/LICENSE,sha256=H2T3_RTgmcngMeC7p_SXT3GwBLkd2DaNgAZuxulcfiA,1066
-wisest-0.9.0.dist-info/METADATA,sha256=TM0Xh7imLSvdEPvOKTAwg-PN5rCjDK87Ue4u7Dda2JA,544
-wisest-0.9.0.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-wisest-0.9.0.dist-info/entry_points.txt,sha256=rO-m_h4BsjihmPclwhVbvslynf-_HOeFpznjZLdKnEA,37
-wisest-0.9.0.dist-info/RECORD,,
+wisest-0.9.1.dist-info/LICENSE,sha256=H2T3_RTgmcngMeC7p_SXT3GwBLkd2DaNgAZuxulcfiA,1066
+wisest-0.9.1.dist-info/METADATA,sha256=zlZ6tG5NwzCgGalQAr2RTK1tJA4lQCocLN-6fmnujOc,544
+wisest-0.9.1.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+wisest-0.9.1.dist-info/entry_points.txt,sha256=rO-m_h4BsjihmPclwhVbvslynf-_HOeFpznjZLdKnEA,37
+wisest-0.9.1.dist-info/RECORD,,
```

