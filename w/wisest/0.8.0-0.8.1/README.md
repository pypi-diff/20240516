# Comparing `tmp/wisest-0.8.0-py3-none-any.whl.zip` & `tmp/wisest-0.8.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 6659 bytes, number of entries: 13
+Zip file size: 6660 bytes, number of entries: 13
 -rw-r--r--  2.0 unx      452 b- defN 80-Jan-01 00:00 wise/__init__.py
--rw-r--r--  2.0 unx     1252 b- defN 80-Jan-01 00:00 wise/cli.py
+-rw-r--r--  2.0 unx     1251 b- defN 80-Jan-01 00:00 wise/cli.py
 -rw-r--r--  2.0 unx      771 b- defN 80-Jan-01 00:00 wise/cost.py
 -rw-r--r--  2.0 unx      583 b- defN 80-Jan-01 00:00 wise/currency.py
 -rw-r--r--  2.0 unx     2157 b- defN 80-Jan-01 00:00 wise/method.py
--rw-r--r--  2.0 unx     3493 b- defN 80-Jan-01 00:00 wise/price.py
+-rw-r--r--  2.0 unx     3491 b- defN 80-Jan-01 00:00 wise/price.py
 -rw-r--r--  2.0 unx     1707 b- defN 80-Jan-01 00:00 wise/rate.py
 -rw-r--r--  2.0 unx       79 b- defN 80-Jan-01 00:00 wise/request.py
--rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 wisest-0.8.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      544 b- defN 80-Jan-01 00:00 wisest-0.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 wisest-0.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       37 b- defN 80-Jan-01 00:00 wisest-0.8.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      943 b- defN 16-Jan-01 00:00 wisest-0.8.0.dist-info/RECORD
-13 files, 13172 bytes uncompressed, 5117 bytes compressed:  61.2%
+-rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 wisest-0.8.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      544 b- defN 80-Jan-01 00:00 wisest-0.8.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 wisest-0.8.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       37 b- defN 80-Jan-01 00:00 wisest-0.8.1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      943 b- defN 16-Jan-01 00:00 wisest-0.8.1.dist-info/RECORD
+13 files, 13169 bytes uncompressed, 5118 bytes compressed:  61.1%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: wise/rate.py
 Comment: 
 
 Filename: wise/request.py
 Comment: 
 
-Filename: wisest-0.8.0.dist-info/LICENSE
+Filename: wisest-0.8.1.dist-info/LICENSE
 Comment: 
 
-Filename: wisest-0.8.0.dist-info/METADATA
+Filename: wisest-0.8.1.dist-info/METADATA
 Comment: 
 
-Filename: wisest-0.8.0.dist-info/WHEEL
+Filename: wisest-0.8.1.dist-info/WHEEL
 Comment: 
 
-Filename: wisest-0.8.0.dist-info/entry_points.txt
+Filename: wisest-0.8.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: wisest-0.8.0.dist-info/RECORD
+Filename: wisest-0.8.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wise/cli.py

```diff
@@ -7,15 +7,15 @@
 from .price import query_price
 
 
 @click.command()
 @click.argument("source-currency", type=click.STRING)
 @click.argument("target-amount", type=click.STRING)
 @click.argument("target-currency", type=click.STRING)
-@click.option("-i", "--pay-in-method", type=click.STRING, default="VISA_CREDIT")
+@click.option("-i", "--pay-in-method", type=click.STRING, default="GOOGLE_PAY")
 @click.option("-o", "--pay-out-method", type=click.STRING, default="BALANCE")
 def cli(
     source_currency: str,
     target_amount: str,
     target_currency: str,
     pay_in_method: str,
     pay_out_method: str,
```

## wise/price.py

```diff
@@ -52,15 +52,15 @@
         )
         resp.raise_for_status()
         return [Price.model_validate(data) for data in resp.json()]
 
 
 def find_price(
     prices: list[Price],
-    pay_in_method: str = "VISA_CREDIT",
+    pay_in_method: str = "GOOGLE_PAY",
     pay_out_method: str = "BALANCE",
 ) -> Price:
     for price in prices:
         if price.pay_in_method == pay_in_method.upper() and price.pay_out_method == pay_out_method.upper():
             return price
 
     msg = f"Price not found for pay_in_method={pay_in_method} and pay_out_method={pay_out_method}"
@@ -68,15 +68,15 @@
 
 
 def query_price(
     source_amount: float | None = None,
     source_currency: str | None = None,
     target_amount: float | None = None,
     target_currency: str | None = None,
-    pay_in_method: str = "VISA_CREDIT",
+    pay_in_method: str = "GOOGLE_PAY",
     pay_out_method: str = "BALANCE",
 ) -> Price:
     prices = PriceRequest(
         source_amount=source_amount,
         source_currency=source_currency,
         target_amount=target_amount,
         target_currency=target_currency,
```

## Comparing `wisest-0.8.0.dist-info/LICENSE` & `wisest-0.8.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `wisest-0.8.0.dist-info/METADATA` & `wisest-0.8.1.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wisest
-Version: 0.8.0
+Version: 0.8.1
 Summary: 
 Author: narumi
 Author-email: toucans-cutouts0f@icloud.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

## Comparing `wisest-0.8.0.dist-info/RECORD` & `wisest-0.8.1.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 wise/__init__.py,sha256=uIH9gdfABknJMDYbFqSdOddBie4c3QjpWORlQaM3DGg,452
-wise/cli.py,sha256=P8oPhiC-kQ8krQrJ1osu685F0uzqLgRXmyYgWI3QV2c,1252
+wise/cli.py,sha256=8tWVnNEydUNXAi-5Un5V7PFVaNqV9cwopeN7MN-GEx0,1251
 wise/cost.py,sha256=dGTtJSaGcBFk1dg8In12TkYK7coxkYTQ27X5U497yng,771
 wise/currency.py,sha256=V8AaX8jW3cfpRbT0MdSvbV8Sk25eW1Pv7jR-cMr7au8,583
 wise/method.py,sha256=zUVJvML08O_X2ifou0AKLe66RE8AM2i14Q7qAntpntY,2157
-wise/price.py,sha256=-A9RJKQVkkl-acyFltJNUoyf3zURJRIXqCF3q2tOPxQ,3493
+wise/price.py,sha256=9VZ3szGbtVB5pMiI12b7YCTwTlRmccCRLrIosGcwDzQ,3491
 wise/rate.py,sha256=VuIZW2bhEm3Dx81cMJwh-ALyt11YCiOUYPU1aOtDIOU,1707
 wise/request.py,sha256=iqGS-XJLlBBG0Z6zh_QDuG0z0f4UY9E4Cme5-fUIxbQ,79
-wisest-0.8.0.dist-info/LICENSE,sha256=H2T3_RTgmcngMeC7p_SXT3GwBLkd2DaNgAZuxulcfiA,1066
-wisest-0.8.0.dist-info/METADATA,sha256=FXwP1N3QOThRln6BSE34_g-LnW__b7D-sMuF4b2XOfo,544
-wisest-0.8.0.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-wisest-0.8.0.dist-info/entry_points.txt,sha256=rO-m_h4BsjihmPclwhVbvslynf-_HOeFpznjZLdKnEA,37
-wisest-0.8.0.dist-info/RECORD,,
+wisest-0.8.1.dist-info/LICENSE,sha256=H2T3_RTgmcngMeC7p_SXT3GwBLkd2DaNgAZuxulcfiA,1066
+wisest-0.8.1.dist-info/METADATA,sha256=qI7DISJUC3xp226KonXAF1IaofJhxg3b0tUQpSf245w,544
+wisest-0.8.1.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+wisest-0.8.1.dist-info/entry_points.txt,sha256=rO-m_h4BsjihmPclwhVbvslynf-_HOeFpznjZLdKnEA,37
+wisest-0.8.1.dist-info/RECORD,,
```

