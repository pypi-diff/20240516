# Comparing `tmp/fa_signal_provider-1.1.27.tar.gz` & `tmp/fa-signal-provider-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fa_signal_provider-1.1.27.tar", last modified: Thu May 16 12:57:48 2024, max compression
+gzip compressed data, was "fa-signal-provider-1.1.9.tar", last modified: Thu Jan 18 16:41:40 2024, max compression
```

## Comparing `fa_signal_provider-1.1.27.tar` & `fa-signal-provider-1.1.9.tar`

### file list

```diff
@@ -1,24 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:57:48.398008 fa_signal_provider-1.1.27/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-16 12:57:31.000000 fa_signal_provider-1.1.27/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-16 12:57:48.398008 fa_signal_provider-1.1.27/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-16 12:57:31.000000 fa_signal_provider-1.1.27/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:57:48.394008 fa_signal_provider-1.1.27/fa_signal_provider.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-16 12:57:48.000000 fa_signal_provider-1.1.27/fa_signal_provider.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-16 12:57:48.000000 fa_signal_provider-1.1.27/fa_signal_provider.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 12:57:48.000000 fa_signal_provider-1.1.27/fa_signal_provider.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-16 12:57:48.000000 fa_signal_provider-1.1.27/fa_signal_provider.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 12:57:48.000000 fa_signal_provider-1.1.27/fa_signal_provider.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:57:48.394008 fa_signal_provider-1.1.27/fasignalprovider/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:57:31.000000 fa_signal_provider-1.1.27/fasignalprovider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-05-16 12:57:31.000000 fa_signal_provider-1.1.27/fasignalprovider/code.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-16 12:57:31.000000 fa_signal_provider-1.1.27/fasignalprovider/direction.py
--rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-05-16 12:57:31.000000 fa_signal_provider-1.1.27/fasignalprovider/event.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-16 12:57:31.000000 fa_signal_provider-1.1.27/fasignalprovider/order_type.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-16 12:57:31.000000 fa_signal_provider-1.1.27/fasignalprovider/side.py
--rw-r--r--   0 runner    (1001) docker     (127)     6905 2024-05-16 12:57:31.000000 fa_signal_provider-1.1.27/fasignalprovider/trading_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-16 12:57:45.000000 fa_signal_provider-1.1.27/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 12:57:48.398008 fa_signal_provider-1.1.27/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-16 12:57:31.000000 fa_signal_provider-1.1.27/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:57:48.394008 fa_signal_provider-1.1.27/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-05-16 12:57:31.000000 fa_signal_provider-1.1.27/tests/test_trading_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-16 12:57:31.000000 fa_signal_provider-1.1.27/tests/test_trading_signal_datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 16:41:40.178263 fa-signal-provider-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-18 16:41:19.000000 fa-signal-provider-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-01-18 16:41:40.178263 fa-signal-provider-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-01-18 16:41:19.000000 fa-signal-provider-1.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 16:41:40.178263 fa-signal-provider-1.1.9/fa_signal_provider.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-01-18 16:41:40.000000 fa-signal-provider-1.1.9/fa_signal_provider.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-01-18 16:41:40.000000 fa-signal-provider-1.1.9/fa_signal_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 16:41:40.000000 fa-signal-provider-1.1.9/fa_signal_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-01-18 16:41:40.000000 fa-signal-provider-1.1.9/fa_signal_provider.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-18 16:41:40.000000 fa-signal-provider-1.1.9/fa_signal_provider.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 16:41:40.178263 fa-signal-provider-1.1.9/fasignalprovider/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 16:41:19.000000 fa-signal-provider-1.1.9/fasignalprovider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-01-18 16:41:19.000000 fa-signal-provider-1.1.9/fasignalprovider/direction.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-01-18 16:41:19.000000 fa-signal-provider-1.1.9/fasignalprovider/side.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-01-18 16:41:19.000000 fa-signal-provider-1.1.9/fasignalprovider/trading_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-01-18 16:41:33.000000 fa-signal-provider-1.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 16:41:40.178263 fa-signal-provider-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-01-18 16:41:19.000000 fa-signal-provider-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 16:41:40.178263 fa-signal-provider-1.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-01-18 16:41:19.000000 fa-signal-provider-1.1.9/tests/test_trading_signal.py
```

### Comparing `fa_signal_provider-1.1.27/LICENSE` & `fa-signal-provider-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fa_signal_provider-1.1.27/PKG-INFO` & `fa-signal-provider-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fa-signal-provider
-Version: 1.1.27
+Version: 1.1.9
 Summary: A model library for all signal providers of Freya Alpha using python. It includes models to handle signal ingestion, signal status reports, profit & performance reports, etc.
 Author-email: Brayan Svan <hello@freya-alpha.com>
 Project-URL: Homepage, https://github.com/svabra/fa-signal-provider
 Keywords: finance,trading,models
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
@@ -15,15 +15,15 @@
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 
-# fa-signal-provider
+# fa-signal-provider-lib
 A model library for all signal providers of Freya Alpha using python. It includes models to handle signal ingestion, signal status reports, profit and performance reports, etc.
 
 ## Sponsors
 Freya Alpha,
 The Kára System,
 Spark & Hale Robotic Industries
```

### Comparing `fa_signal_provider-1.1.27/README.md` & `fa-signal-provider-1.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# fa-signal-provider
+# fa-signal-provider-lib
 A model library for all signal providers of Freya Alpha using python. It includes models to handle signal ingestion, signal status reports, profit and performance reports, etc.
 
 ## Sponsors
 Freya Alpha,
 The Kára System,
 Spark & Hale Robotic Industries
```

### Comparing `fa_signal_provider-1.1.27/fa_signal_provider.egg-info/PKG-INFO` & `fa-signal-provider-1.1.9/fa_signal_provider.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fa-signal-provider
-Version: 1.1.27
+Version: 1.1.9
 Summary: A model library for all signal providers of Freya Alpha using python. It includes models to handle signal ingestion, signal status reports, profit & performance reports, etc.
 Author-email: Brayan Svan <hello@freya-alpha.com>
 Project-URL: Homepage, https://github.com/svabra/fa-signal-provider
 Keywords: finance,trading,models
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
@@ -15,15 +15,15 @@
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 
-# fa-signal-provider
+# fa-signal-provider-lib
 A model library for all signal providers of Freya Alpha using python. It includes models to handle signal ingestion, signal status reports, profit and performance reports, etc.
 
 ## Sponsors
 Freya Alpha,
 The Kára System,
 Spark & Hale Robotic Industries
```

### Comparing `fa_signal_provider-1.1.27/fasignalprovider/trading_signal.py` & `fa-signal-provider-1.1.9/fasignalprovider/trading_signal.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,137 +1,91 @@
 from pydantic import BaseModel, Field, field_validator
-
-# from typing import Optional
+from typing import Optional
 from datetime import datetime
 from fasignalprovider.direction import Direction
-from fasignalprovider.order_type import OrderType
 from fasignalprovider.side import Side
 
 
 class TradingSignal(BaseModel):
     """
     A trading signal represents a suggestion to buy or sell. It is issued by a signal supplier
     (manually or algorithmically). It must have a correlating id to a trade.
     """
 
-    provider_signal_id: str = Field(
-        ...,
-        description="Mandatory. Provide us with your signal id. This correlation id is your own 'signal id' \
-            of your internal system. Your and our party will use it to inspect process errors. \
-            Do NOT mistaken this correlation id with the trade id.",
+    provider_id: str = Field(
+        ..., description="Your ID as a provider, who emitted the signal."
     )
-
-    provider_trade_id: str = Field(
+    strategy_id: str = Field(
         ...,
-        description="Mandatory. We describes a trade as a buy and a sell (not soley a buy OR a sell), \
-            which has a unique provider_trade_id (the same for both, respectively all of them). \
-            Every trade is expected to consist of at least one buy signal and at least one sell signal.\
-            Both have a unique provider_signal_id, but - again - share the same provider_trade_id. \
-            Thus, the provider_trade_id is mandatory for each signal sent. This will allow to create \
-            a multi-position-trade. \
-            \
-            E.g. one can send one long signal with a provider_trade_id 77 and another long signal a \
-            few hours later also with the provider_trade_id 77. Still, both signals require their \
-            unique provider_signal_id. Provided that the position_size_in_percentage is less than \
-            100 on the first one. \
-            All updates provided by Freya Alpha will hold the provider_trade_id and likely the provider_signal_id \
-            - if it concerns a signal itself.",
+        description="Provide the id of the strategy (you might have more than one algorithm), which is sending a signal.",
     )
-
-    provider_id: str = Field(
-        ..., description="Mandatory. Your ID as a provider, who emitted the signal."
+    provider_signal_id: Optional[str] = Field(
+        None,
+        description="You can use this correlation id as your own 'signal id' of your internal system. Do NOT mistaken this correlation id with the trade correlation id.",
     )
-    strategy_id: str = Field(
+    provider_trade_id: str = Field(
         ...,
-        description="Mandatory. Provide the id of the strategy (you might have more than one algorithm), which is sending a signal.",
+        description="FA Models describes a Trade as a buy and a sell (not soley a buy or a sell). Every trade is expected to consist of at least one buy order and at least one sell order. Thus, the provider_trade_id is mandatory if a provider wants to scale in and out on a fund-position. This will create a multi-position-trade. E.g. one can send one long signal with a provider_trade_id 77 and another long signal a few hours later also with the provider_trade_id 77. Provided that the position_size_in_percentage is less than 100 on the first one. All updates provided by the system will hold the trade id.",
     )
-
     is_hot_signal: bool = Field(
-        default=False,
-        description="Mandatory. By DEFAULT, every signal is marked as a COLD SIGNAL.  \
-            That is a paper-trading signal and will only be processed for forward-performance \
-            testing. Hot signals are suggested to be processed by the order engines - \
-            provided all other requirements for hot trading are fulfilled. Set this \
-            value to true to suggest a hot trade.",
-    )
-    market: str = Field(
-        ..., description="Mandatory. The market you want to trade. e.g. BTC/USDT"
+        default=True,
+        description="By default, every signal is marked as a cold signal. Thus, set to 0. That is a paper-trading signal and will only be processed for forward-performance testing. Hot signals are suggested to be processed by the order engines - provided all other requirements for hot trading are fulfilled. Set 1 (not true) to this value to suggest a hot trade.",
     )
-    data_source: str = Field(
+    market: str = Field(..., description="The market you want to trade. e.g. BTC/USDT")
+    exchange: str = Field(
         ...,
-        description="Mandatory. The source of data you based your decision on. E.g. Binance, CoinMarketCap,\
-            Chainlink, etc. This is to safeguard investments, which base on manipulated data sources.",
+        description="The exchange you pulled your data from - or - wish to trade on.",
     )
-    direction: Direction = Field(..., description="Mandatory. Simply LONG or SHORT.")
+    direction: Direction = Field(..., description="Simply LONG or SHORT.")
     side: Side = Field(
-        ..., description="Mandatory. Simply BUY (open trade) or SELL (close trade)."
-    )
-    order_type: OrderType = Field(
-        default=OrderType.LIMIT_ORDER,
-        description="Mandatory. Default is Limit Order. Please be careful with Markets Orders as slipage could be high.",
+        ..., description="Simply BUY (open trade) or SELL (close trade)."
     )
     price: float = Field(
-        ...,
-        description="Mandatory. The price to buy or sell. Used for the limit-order. If market-order is set, this price is a reference price only to avoid average slipage greater than 10%.",
-    )
-    tp: float = Field(
-        ...,
-        description="Mandatory. Take-profit in an absolute price. In case of a sell signal (limit order) the TP must equal the price.",
-    )
-    sl: float = Field(
-        ...,
-        description="Mandatory. Stop-loss in an absolute price. In case of a sell signal (limit order) the SL must equal the price.",
+        ..., description="The price to buy use for the limit-order or limit-stop-order"
     )
+    tp: float = Field(..., description="Take-profit in absolute price.")
+    sl: float = Field(..., description="Stop-loss in absolute price.")
     position_size_in_percentage: float = Field(
         default=100,
         description="Caution, if one chooses another value than 100, the system will create a multi-position-trade (for scaling-in and scaling-out on a trade). In addition, one has to provide a provider_trade_id in order for the system to create a multi-position-trade. Any consecutive trades (scale-in/out), need to have provide the same provider_trade_id. Percentage of the trade position this algortihm is allowed to trade. Default is 100%, which is 1 position of your fund's positions. Another number than 100, will assume this trade has multiple positions. If a signal provider has one partial position open and then closes it, it will also regard the trade as fully closed.",
     )
-    date_of_creation: int = Field(
-        description="Mandatory. The UTC POSIX date/time when the signal was created in the signal provider's system. Use the POSIX UTC date format. "
+    date_of_creation: datetime = Field(
+        default_factory=datetime.now,
+        description="The UTC datetime when the signal was created by the signal supplier.",
     )
 
     @field_validator(
         "provider_id",
         "strategy_id",
         "provider_signal_id",
         "provider_trade_id",
         "market",
-        "data_source",
+        "exchange",
     )
     def check_string_not_empty(cls, v):
         if not v or v.isspace():
-            raise ValueError("This field must not be empty.")
+            raise ValueError("This field must not be empty")
         return v
 
     @field_validator("price", "tp", "sl", "position_size_in_percentage")
     def check_positive_value(cls, v):
         if v <= 0:
-            raise ValueError("price must a positive number.")
+            raise ValueError("This field must be positive")
         return v
 
     @field_validator("is_hot_signal")
     def check_boolean(cls, v):
         if not isinstance(v, bool):
-            raise ValueError("is_hot_signal must be a boolean.")
+            raise ValueError("is_hot_signal must be a boolean")
         return v
 
     @field_validator("direction", "side")
     def check_enum(cls, v):
         if not isinstance(v, (Direction, Side)):
-            raise ValueError("Invalid value for direction or side.")
+            raise ValueError("Invalid value for direction or side")
         return v
 
     @field_validator("date_of_creation")
     def check_datetime(cls, v):
-        if not isinstance(v, int):
-            raise ValueError(f"date_of_creation must be an integer representing a POSIX timestamp in milliseconds, got type {type(v).__name__}")
-        
-        # # Assuming the value should be within a reasonable range, e.g., post-Unix epoch and not too far in the future
-        # # Unix epoch starts at 1970-01-01, which is 0 in POSIX time
-        # # Let's set an arbitrary upper limit for validation, e.g., January 1, 2030, for demonstration
-        # min_timestamp = 0  # This would be the Unix epoch start
-        # max_timestamp = 1893456000000  # Represents January 1, 2030, in milliseconds
-        # if not (min_timestamp <= v <= max_timestamp):
-        #     raise ValueError(f"date_of_creation must represent a date between 1970-01-01 and 2030-01-01, got {v}")
-
-        # # The value passes the check, return it
+        if not isinstance(v, datetime):
+            raise ValueError("date_of_creation must be a datetime object")
         return v
```

### Comparing `fa_signal_provider-1.1.27/pyproject.toml` & `fa-signal-provider-1.1.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=66.1.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fa-signal-provider"
-version = "1.1.27"
+version = "1.1.9"
 description = "A model library for all signal providers of Freya Alpha using python. It includes models to handle signal ingestion, signal status reports, profit & performance reports, etc."
 readme = "README.md"
 authors = [{ name = "Brayan Svan", email = "hello@freya-alpha.com" }]
 #license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python"
@@ -25,15 +25,15 @@
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/svabra/fa-signal-provider"
 
 [tool.bumpver]
-current_version = "1.1.27"
+current_version = "1.1.9"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fa_signal_provider-1.1.27/setup.py` & `fa-signal-provider-1.1.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,19 +20,17 @@
 #                 #     if obj.__module__ == module_name:
 #                 #         print(name)
 
 #         build.run(self)
 
 setup(
     name='fa-signal-provider',
-    # packages=find_packages(include=['fasignalprovider',
-    #                                 'fasignalprovider.com'
-    #                                 ], exclude=['tests*']),
-    packages=find_packages(exclude=['tests*']),
-    include_package_data=True # finds all modules within recursive folders with a __init__.py file.
+    packages=find_packages(include=['fasignalprovider',
+                                    'fasignalprovider.fund'
+                                    ], exclude=['tests*']),
     # packages=['fasignalprovider'],
     # package_dir={'fasignalprovider':'src'}
     #packages=find_packages(),
     #version='0.1.0',
     # description='The library describes the most common models used in trading systems.',
     # author='Brayan Svan',
     # license='MIT',
```

