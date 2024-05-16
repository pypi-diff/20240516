# Comparing `tmp/wisest-0.8.1-py3-none-any.whl.zip` & `tmp/wisest-0.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 6660 bytes, number of entries: 13
+Zip file size: 6766 bytes, number of entries: 13
 -rw-r--r--  2.0 unx      452 b- defN 80-Jan-01 00:00 wise/__init__.py
--rw-r--r--  2.0 unx     1251 b- defN 80-Jan-01 00:00 wise/cli.py
+-rw-r--r--  2.0 unx     1368 b- defN 80-Jan-01 00:00 wise/cli.py
 -rw-r--r--  2.0 unx      771 b- defN 80-Jan-01 00:00 wise/cost.py
 -rw-r--r--  2.0 unx      583 b- defN 80-Jan-01 00:00 wise/currency.py
 -rw-r--r--  2.0 unx     2157 b- defN 80-Jan-01 00:00 wise/method.py
--rw-r--r--  2.0 unx     3491 b- defN 80-Jan-01 00:00 wise/price.py
+-rw-r--r--  2.0 unx     3696 b- defN 80-Jan-01 00:00 wise/price.py
 -rw-r--r--  2.0 unx     1707 b- defN 80-Jan-01 00:00 wise/rate.py
 -rw-r--r--  2.0 unx       79 b- defN 80-Jan-01 00:00 wise/request.py
--rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 wisest-0.8.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      544 b- defN 80-Jan-01 00:00 wisest-0.8.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 wisest-0.8.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       37 b- defN 80-Jan-01 00:00 wisest-0.8.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      943 b- defN 16-Jan-01 00:00 wisest-0.8.1.dist-info/RECORD
-13 files, 13169 bytes uncompressed, 5118 bytes compressed:  61.1%
+-rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 wisest-0.9.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      544 b- defN 80-Jan-01 00:00 wisest-0.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 wisest-0.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       37 b- defN 80-Jan-01 00:00 wisest-0.9.0.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      943 b- defN 16-Jan-01 00:00 wisest-0.9.0.dist-info/RECORD
+13 files, 13491 bytes uncompressed, 5224 bytes compressed:  61.3%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: wise/rate.py
 Comment: 
 
 Filename: wise/request.py
 Comment: 
 
-Filename: wisest-0.8.1.dist-info/LICENSE
+Filename: wisest-0.9.0.dist-info/LICENSE
 Comment: 
 
-Filename: wisest-0.8.1.dist-info/METADATA
+Filename: wisest-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: wisest-0.8.1.dist-info/WHEEL
+Filename: wisest-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: wisest-0.8.1.dist-info/entry_points.txt
+Filename: wisest-0.9.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: wisest-0.8.1.dist-info/RECORD
+Filename: wisest-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wise/cli.py

```diff
@@ -9,32 +9,35 @@
 
 @click.command()
 @click.argument("source-currency", type=click.STRING)
 @click.argument("target-amount", type=click.STRING)
 @click.argument("target-currency", type=click.STRING)
 @click.option("-i", "--pay-in-method", type=click.STRING, default="GOOGLE_PAY")
 @click.option("-o", "--pay-out-method", type=click.STRING, default="BALANCE")
+@click.option("--new", is_flag=True, type=click.BOOL)
 def cli(
     source_currency: str,
     target_amount: str,
     target_currency: str,
     pay_in_method: str,
     pay_out_method: str,
+    new: bool,
 ) -> None:
     sources = source_currency.split(",")
     amounts = [float(x) for x in target_amount.split(",")]
     targets = target_currency.split(",")
 
     prices = [
         query_price(
             source_currency=source,
             target_amount=float(amount),
             target_currency=target,
             pay_in_method=pay_in_method,
             pay_out_method=pay_out_method,
+            price_set_id=2593 if new else 2586,
         )
         for source, amount, target in tqdm(list(product(sources, amounts, targets)))
     ]
 
     # sort by total fee rate
     prices = sorted(prices, key=lambda p: p.variable_fee_percent)
```

## wise/price.py

```diff
@@ -32,23 +32,25 @@
     source_currency: str | None = Field(default=None, serialization_alias="sourceCurrency")
     target_amount: float | None = Field(default=None, serialization_alias="targetAmount")
     target_currency: str | None = Field(default=None, serialization_alias="targetCurrency")
     profile_id: str | None = Field(default=None, serialization_alias="profileId")
     profile_country: str | None = Field(default=None, serialization_alias="profileCountry")
     profile_type: str | None = Field(default=None, serialization_alias="profileType")
     markers: str | None = None
+    price_set_id: int | None = Field(default=None, serialization_alias="priceSetId")
 
     @field_validator("source_currency", "target_currency")
     @classmethod
     def upper(cls, s: str) -> str:
         return s.upper()
 
     def do(self) -> list[Price]:
         # https://wise.com/gb/pricing/receive
         # https://wise.com/gb/pricing/send-money
+        # https://wise.com/price-change/borderless-add
 
         resp = get(
             url="https://wise.com/gateway/v1/price",
             params=self.model_dump(exclude_none=True, by_alias=True),
         )
         resp.raise_for_status()
         return [Price.model_validate(data) for data in resp.json()]
@@ -70,20 +72,22 @@
 def query_price(
     source_amount: float | None = None,
     source_currency: str | None = None,
     target_amount: float | None = None,
     target_currency: str | None = None,
     pay_in_method: str = "GOOGLE_PAY",
     pay_out_method: str = "BALANCE",
+    price_set_id: int = 2586,
 ) -> Price:
     prices = PriceRequest(
         source_amount=source_amount,
         source_currency=source_currency,
         target_amount=target_amount,
         target_currency=target_currency,
+        price_set_id=price_set_id,
     ).do()
     price = find_price(
         prices,
         pay_in_method=pay_in_method,
         pay_out_method=pay_out_method,
     )
     return price
```

## Comparing `wisest-0.8.1.dist-info/LICENSE` & `wisest-0.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `wisest-0.8.1.dist-info/METADATA` & `wisest-0.9.0.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wisest
-Version: 0.8.1
+Version: 0.9.0
 Summary: 
 Author: narumi
 Author-email: toucans-cutouts0f@icloud.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

## Comparing `wisest-0.8.1.dist-info/RECORD` & `wisest-0.9.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 wise/__init__.py,sha256=uIH9gdfABknJMDYbFqSdOddBie4c3QjpWORlQaM3DGg,452
-wise/cli.py,sha256=8tWVnNEydUNXAi-5Un5V7PFVaNqV9cwopeN7MN-GEx0,1251
+wise/cli.py,sha256=16pfJKwmLQD-hP6jvpEPHj7I8iqfJV3G-YTU2HOg1p8,1368
 wise/cost.py,sha256=dGTtJSaGcBFk1dg8In12TkYK7coxkYTQ27X5U497yng,771
 wise/currency.py,sha256=V8AaX8jW3cfpRbT0MdSvbV8Sk25eW1Pv7jR-cMr7au8,583
 wise/method.py,sha256=zUVJvML08O_X2ifou0AKLe66RE8AM2i14Q7qAntpntY,2157
-wise/price.py,sha256=9VZ3szGbtVB5pMiI12b7YCTwTlRmccCRLrIosGcwDzQ,3491
+wise/price.py,sha256=64QblEsUScRRj8CRYYfWOd-EFJmhaDHBBdLp_i1lo5g,3696
 wise/rate.py,sha256=VuIZW2bhEm3Dx81cMJwh-ALyt11YCiOUYPU1aOtDIOU,1707
 wise/request.py,sha256=iqGS-XJLlBBG0Z6zh_QDuG0z0f4UY9E4Cme5-fUIxbQ,79
-wisest-0.8.1.dist-info/LICENSE,sha256=H2T3_RTgmcngMeC7p_SXT3GwBLkd2DaNgAZuxulcfiA,1066
-wisest-0.8.1.dist-info/METADATA,sha256=qI7DISJUC3xp226KonXAF1IaofJhxg3b0tUQpSf245w,544
-wisest-0.8.1.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-wisest-0.8.1.dist-info/entry_points.txt,sha256=rO-m_h4BsjihmPclwhVbvslynf-_HOeFpznjZLdKnEA,37
-wisest-0.8.1.dist-info/RECORD,,
+wisest-0.9.0.dist-info/LICENSE,sha256=H2T3_RTgmcngMeC7p_SXT3GwBLkd2DaNgAZuxulcfiA,1066
+wisest-0.9.0.dist-info/METADATA,sha256=TM0Xh7imLSvdEPvOKTAwg-PN5rCjDK87Ue4u7Dda2JA,544
+wisest-0.9.0.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+wisest-0.9.0.dist-info/entry_points.txt,sha256=rO-m_h4BsjihmPclwhVbvslynf-_HOeFpznjZLdKnEA,37
+wisest-0.9.0.dist-info/RECORD,,
```

