# Comparing `tmp/telegram_wallet_pay-0.5.0.tar.gz` & `tmp/telegram_wallet_pay-0.6.0.tar.gz`

## Comparing `telegram_wallet_pay-0.5.0.tar` & `telegram_wallet_pay-0.6.0.tar`

### file list

```diff
@@ -1,46 +1,48 @@
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/.editorconfig
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/Makefile
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/codecov.yaml
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/examples/00_create_order.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/examples/01_get_order_preview.py
--rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/examples/02_bot_example.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/examples/03_webhook_handler_example.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/__init__.py
--rw-r--r--   0        0        0     7277 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/client.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/errors.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/enums/__init__.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/enums/currency.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/enums/order_status.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/enums/request_status.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/enums/webhook_message_type.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/__init__.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/_default.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/create_order_request.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/create_order_response.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/get_order_preview_response.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/get_order_reconciliation_list_response.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/money_amount.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/order_amount.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/order_amount_response.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/order_preview.py
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/order_reconciliation_item.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/order_reconciliation_list.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/payment_option.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/webhook_message.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/webhook_payload.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/tools/__init__.py
--rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/tools/fastapi.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/tools/signature.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/telegram_wallet_pay/tools/text.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/tests/conftest.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/tests/samples.py
--rw-r--r--   0        0        0     6608 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/tests/test_client.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/tests/test_schemas.py
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/tests/test_tools/test_fastapi.py
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/tests/test_tools/test_signature.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/.gitignore
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/README.md
--rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     5321 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/.editorconfig
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/Makefile
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/codecov.yaml
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/examples/00_create_order.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/examples/01_get_order_preview.py
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/examples/02_bot_example.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/examples/03_webhook_handler_example.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/__init__.py
+-rw-r--r--   0        0        0     7277 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/client.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/constants.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/errors.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/enums/__init__.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/enums/button_name.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/enums/currency.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/enums/order_status.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/enums/request_status.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/enums/webhook_message_type.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/__init__.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/_default.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/create_order_request.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/create_order_response.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/get_order_preview_response.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/get_order_reconciliation_list_response.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/money_amount.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/order_amount.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/order_amount_response.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/order_preview.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/order_reconciliation_item.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/order_reconciliation_list.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/payment_option.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/webhook_message.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/webhook_payload.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/tools/__init__.py
+-rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/tools/fastapi.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/tools/signature.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/telegram_wallet_pay/tools/text.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/tests/conftest.py
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/tests/samples.py
+-rw-r--r--   0        0        0     6608 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/tests/test_client.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/tests/test_schemas.py
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/tests/test_tools/test_fastapi.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/tests/test_tools/test_signature.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/.gitignore
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/README.md
+-rw-r--r--   0        0        0     4298 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.6.0/PKG-INFO
```

### Comparing `telegram_wallet_pay-0.5.0/examples/00_create_order.py` & `telegram_wallet_pay-0.6.0/examples/00_create_order.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 async def main() -> None:
     """Create order."""
     wallet = TelegramWalletPay(TOKEN)
 
     # create your first order
     response = await wallet.create_order(
         amount=40,
-        currency_code="RUB",
+        currency_code="EUR",
         description="TestPayment",
         external_id=str(uuid4()),
         timeout_seconds=5 * 60,
         customer_telegram_user_id=66812456,
     )
 
     # let's print creation response
```

### Comparing `telegram_wallet_pay-0.5.0/examples/02_bot_example.py` & `telegram_wallet_pay-0.6.0/examples/02_bot_example.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from aiogram.enums import ParseMode
 from aiogram.types import InlineKeyboardButton, Message
 from aiogram.utils.keyboard import InlineKeyboardBuilder
 
 # install Telegram Wallet Pay API client library:
 #   pip install telegram-wallet-pay
 from telegram_wallet_pay import TelegramWalletPay
+from telegram_wallet_pay.enums import ButtonName
 
 # store TELEGRAM_BOT_API_TOKEN to your .env
 # bot token can be issued via https://t.me/BotFather
 TELEGRAM_BOT_API_TOKEN = getenv("TELEGRAM_BOT_API_TOKEN")
 
 # store TELEGRAM_WALLET_PAY_TOKEN to your .env
 # wallet token can be issued via https://pay.wallet.tg/
@@ -44,15 +45,15 @@
         customer_telegram_user_id=message.from_user.id,
     )
     order = wallet_response.data
 
     # prepare keyboard
     keyboard = InlineKeyboardBuilder()
     wallet_button = InlineKeyboardButton(
-        text="👛 Pay via Wallet",
+        text=ButtonName.PAY_VIA_WALLET,
         url=order.pay_link,
     )
     keyboard.add(wallet_button)
 
     # send answer message with prepared content and keyboard markup
     await message.answer(
         text=f"{header}\n{body}",
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `telegram_wallet_pay-0.5.0/examples/03_webhook_handler_example.py` & `telegram_wallet_pay-0.6.0/examples/03_webhook_handler_example.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.5.0/telegram_wallet_pay/client.py` & `telegram_wallet_pay-0.6.0/telegram_wallet_pay/client.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/__init__.py` & `telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/create_order_request.py` & `telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/create_order_request.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/create_order_response.py` & `telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/create_order_response.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/order_preview.py` & `telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/order_reconciliation_item.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,26 +3,32 @@
 
 from pydantic import Field
 
 from telegram_wallet_pay.enums import Currency, OrderStatus
 
 from ._default import DefaultModel
 from .money_amount import MoneyAmount
+from .payment_option import PaymentOption
 
 
-class OrderPreview(DefaultModel):
-    id: str
-    status: OrderStatus
-    number: str
+class OrderReconciliationItem(DefaultModel):
+    id: int
+    status: Literal[
+        OrderStatus.ACTIVE,
+        OrderStatus.EXPIRED,
+        OrderStatus.PAID,
+        OrderStatus.CANCELLED,
+    ]
     amount: MoneyAmount
     auto_conversion_currency: Optional[
         Literal[
             Currency.TON,
             Currency.BTC,
             Currency.USDT,
         ]
     ] = None
+    external_id: str
+    customer_telegram_user_id: Optional[int] = None
     created_datetime: datetime = Field(alias="createdDateTime")
     expiration_datetime: datetime = Field(alias="expirationDateTime")
-    completed_datetime: Optional[datetime] = Field(None, alias="completedDateTime")
-    pay_link: str
-    direct_pay_link: str
+    payment_datetime: Optional[datetime] = Field(None, alias="paymentDateTime")
+    selected_payment_option: Optional[PaymentOption] = None
```

### Comparing `telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/order_reconciliation_item.py` & `telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/order_preview.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,27 +3,31 @@
 
 from pydantic import Field
 
 from telegram_wallet_pay.enums import Currency, OrderStatus
 
 from ._default import DefaultModel
 from .money_amount import MoneyAmount
-from .payment_option import PaymentOption
 
 
-class OrderReconciliationItem(DefaultModel):
-    id: int
-    status: OrderStatus
+class OrderPreview(DefaultModel):
+    id: str
+    status: Literal[
+        OrderStatus.ACTIVE,
+        OrderStatus.EXPIRED,
+        OrderStatus.PAID,
+        OrderStatus.CANCELLED,
+    ]
+    number: str
     amount: MoneyAmount
     auto_conversion_currency: Optional[
         Literal[
             Currency.TON,
             Currency.BTC,
             Currency.USDT,
         ]
     ] = None
-    external_id: str
-    customer_telegram_user_id: Optional[int] = None
     created_datetime: datetime = Field(alias="createdDateTime")
     expiration_datetime: datetime = Field(alias="expirationDateTime")
-    payment_datetime: Optional[datetime] = Field(None, alias="paymentDateTime")
-    selected_payment_option: Optional[PaymentOption] = None
+    completed_datetime: Optional[datetime] = Field(None, alias="completedDateTime")
+    pay_link: str
+    direct_pay_link: str
```

### Comparing `telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/webhook_message.py` & `telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/webhook_message.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from datetime import datetime
-from typing import Iterator, List
+from typing import Iterator, List, Literal
 
 from pydantic import Field
 
 from telegram_wallet_pay.enums import WebhookMessageType
 
 from ._default import DefaultModel, DefaultRootModel
 from .webhook_payload import WebhookPayload
 
 
 class WebhookMessage(DefaultModel):
     event_datetime: datetime = Field(alias="eventDateTime")
     event_id: int
-    type: WebhookMessageType
+    type: Literal[
+        WebhookMessageType.ORDER_PAID,
+        WebhookMessageType.ORDER_FAILED,
+    ]
     payload: WebhookPayload
 
 
 class WebhookMessages(DefaultRootModel):
     root: List[WebhookMessage]
 
     def __iter__(self) -> Iterator[WebhookMessage]:  # type: ignore[override]
```

### Comparing `telegram_wallet_pay-0.5.0/telegram_wallet_pay/schemas/webhook_payload.py` & `telegram_wallet_pay-0.6.0/telegram_wallet_pay/schemas/webhook_payload.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.5.0/telegram_wallet_pay/tools/fastapi.py` & `telegram_wallet_pay-0.6.0/telegram_wallet_pay/tools/fastapi.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.5.0/telegram_wallet_pay/tools/signature.py` & `telegram_wallet_pay-0.6.0/telegram_wallet_pay/tools/signature.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.5.0/tests/conftest.py` & `telegram_wallet_pay-0.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.5.0/tests/samples.py` & `telegram_wallet_pay-0.6.0/tests/samples.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ORDER_AMOUNT = {
-    "currencyCode": "RUB",
+    "currencyCode": "EUR",
     "amount": "40.00",
 }
 
 SELECTED_PAYMENT_OPTION = {
     "amount": {
         "currencyCode": "TON",
         "amount": "0.069848094",
@@ -31,14 +31,15 @@
 WEBHOOK_MESSAGE_ORDER_PAID = {
     "eventDateTime": "2024-04-21T15:04:24.092Z",
     "eventId": 10829789207553,
     "type": "ORDER_PAID",
     "payload": WEBHOOK_PAYLOAD,
 }
 
+# noinspection SpellCheckingInspection
 WEBHOOK_MESSAGE_ORDER_FAILED = {
     "eventId": 11044361216001,
     "eventDateTime": "2024-05-01T07:53:56.000991Z",
     "payload": {
         "id": 11000119772673,
         "number": "LVDPW6K8",
         "status": "EXPIRED",
```

### Comparing `telegram_wallet_pay-0.5.0/tests/test_client.py` & `telegram_wallet_pay-0.6.0/tests/test_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     OrderReconciliationList,
 )
 
 ORDER_PREVIEW = OrderPreview(
     id="",
     status="ACTIVE",
     number="",
-    amount=MoneyAmount(currency_code="RUB", amount="42.0"),
+    amount=MoneyAmount(currency_code="EUR", amount="42.0"),
     created_datetime=datetime.now(),
     expiration_datetime=datetime.now(),
     pay_link="",
     direct_pay_link="",
 )
 
 CREATE_ORDER_RESPONSE = CreateOrderResponse(
@@ -40,15 +40,15 @@
     message="",
     data=ORDER_PREVIEW,
 )
 
 ORDER_RECONCILIATION_ITEM = OrderReconciliationItem(
     id=42,
     status="EXPIRED",
-    amount=MoneyAmount(currency_code="RUB", amount="42.0"),
+    amount=MoneyAmount(currency_code="EUR", amount="42.0"),
     external_id="",
     created_datetime=datetime.now(),
     expiration_datetime=datetime.now(),
 )
 
 GET_ORDERS_LIST_RESPONSE = GetOrderReconciliationListResponse(
     status="SUCCESS",
```

### Comparing `telegram_wallet_pay-0.5.0/tests/test_schemas.py` & `telegram_wallet_pay-0.6.0/tests/test_schemas.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     MoneyAmount,
     PaymentOption,
     WebhookMessage,
     WebhookMessages,
     WebhookPayload,
 )
 
-money_amount = MoneyAmount(currency_code="RUB", amount="42")
+money_amount = MoneyAmount(currency_code="EUR", amount="42")
 payment_option = PaymentOption(
     amount=money_amount,
     amount_fee=money_amount,
     amount_net=money_amount,
     exchange_rate="",
 )
 webhook_payload = WebhookPayload(
```

### Comparing `telegram_wallet_pay-0.5.0/tests/test_tools/test_fastapi.py` & `telegram_wallet_pay-0.6.0/tests/test_tools/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.5.0/tests/test_tools/test_signature.py` & `telegram_wallet_pay-0.6.0/tests/test_tools/test_signature.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Union
 
 import pytest
 from telegram_wallet_pay.tools import compute_signature
 
 
+# noinspection SpellCheckingInspection
 @pytest.mark.parametrize(
     "body",
     [
         (
             '[{"eventDateTime":"2023-07-28T10:20:17.681338Z",'
             '"eventId":10030477545046017,"type":"ORDER_PAID","payload":{'
             '"id":10030467668508673,"number":"XYTNJP2O","customData":"in exercitation '
```

### Comparing `telegram_wallet_pay-0.5.0/.gitignore` & `telegram_wallet_pay-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.5.0/README.md` & `telegram_wallet_pay-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 async def main() -> None:
     """Create order."""
     wallet = TelegramWalletPay(TOKEN)
 
     # create your first order
     response = await wallet.create_order(
         amount=40,
-        currency_code="RUB",
+        currency_code="EUR",
         description="TestPayment",
         external_id=str(uuid4()),
         timeout_seconds=5 * 60,
         customer_telegram_user_id=66812456,
     )
 
     # let's print creation response
```

### Comparing `telegram_wallet_pay-0.5.0/pyproject.toml` & `telegram_wallet_pay-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -51,25 +51,26 @@
 ]
 
 [project.optional-dependencies]
 dev = [
     "ruff>=0,<1",
     "mypy>=1,<2",
     "pre-commit>=3,<4",
-    "fastapi>=0.110,<1",
+    "fastapi-slim>=0.111,<1",
     "uvicorn>=0.29,<1",
     "httpx>=0.27,<1",
+    "aiogram>=3.6,<4"
 ]
 test = [
     "coverage>=7,<8",
     "pytest>=8,<9",
     "pytest-asyncio>=0,<1",
     "pytest-cov>=5,<6",
     "aresponses>=3,<4",
-    "fastapi>=0.110,<1",
+    "fastapi-slim>=0.111,<1",
     "httpx>=0.27,<1",
 ]
 
 
 [project.urls]
 Repository = "https://github.com/Olegt0rr/TelegramWalletPay"
 Documentation = "https://docs.wallet.tg/pay/"
```

### Comparing `telegram_wallet_pay-0.5.0/PKG-INFO` & `telegram_wallet_pay-0.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: telegram-wallet-pay
-Version: 0.5.0
+Version: 0.6.0
 Summary: Async client for Telegram Wallet Pay API
 Project-URL: Repository, https://github.com/Olegt0rr/TelegramWalletPay
 Project-URL: Documentation, https://docs.wallet.tg/pay/
 Author-email: Oleg Abramov <oleg@trueweb.app>
 Maintainer-email: Oleg Abramov <oleg@trueweb.app>
 License-Expression: MIT
 Keywords: API,Pay,Telegram,Wallet,async
@@ -28,24 +28,25 @@
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: aiohttp<4,>=3.8
 Requires-Dist: certifi>=2023
 Requires-Dist: pydantic<3,>=2.4
 Provides-Extra: dev
-Requires-Dist: fastapi<1,>=0.110; extra == 'dev'
+Requires-Dist: aiogram<4,>=3.6; extra == 'dev'
+Requires-Dist: fastapi-slim<1,>=0.111; extra == 'dev'
 Requires-Dist: httpx<1,>=0.27; extra == 'dev'
 Requires-Dist: mypy<2,>=1; extra == 'dev'
 Requires-Dist: pre-commit<4,>=3; extra == 'dev'
 Requires-Dist: ruff<1,>=0; extra == 'dev'
 Requires-Dist: uvicorn<1,>=0.29; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: aresponses<4,>=3; extra == 'test'
 Requires-Dist: coverage<8,>=7; extra == 'test'
-Requires-Dist: fastapi<1,>=0.110; extra == 'test'
+Requires-Dist: fastapi-slim<1,>=0.111; extra == 'test'
 Requires-Dist: httpx<1,>=0.27; extra == 'test'
 Requires-Dist: pytest-asyncio<1,>=0; extra == 'test'
 Requires-Dist: pytest-cov<6,>=5; extra == 'test'
 Requires-Dist: pytest<9,>=8; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Telegram Wallet Pay
@@ -92,15 +93,15 @@
 async def main() -> None:
     """Create order."""
     wallet = TelegramWalletPay(TOKEN)
 
     # create your first order
     response = await wallet.create_order(
         amount=40,
-        currency_code="RUB",
+        currency_code="EUR",
         description="TestPayment",
         external_id=str(uuid4()),
         timeout_seconds=5 * 60,
         customer_telegram_user_id=66812456,
     )
 
     # let's print creation response
```

