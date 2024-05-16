# Comparing `tmp/py_alpaca_api-0.3.5.tar.gz` & `tmp/py_alpaca_api-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_alpaca_api-0.3.5.tar", max compression
+gzip compressed data, was "py_alpaca_api-0.4.0.tar", max compression
```

## Comparing `py_alpaca_api-0.3.5.tar` & `py_alpaca_api-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1066 2024-05-11 23:37:32.674625 py_alpaca_api-0.3.5/LICENSE
--rw-r--r--   0        0        0    12576 2024-05-12 02:52:40.341369 py_alpaca_api-0.3.5/README.md
--rw-r--r--   0        0        0        0 2024-05-11 00:31:44.448417 py_alpaca_api-0.3.5/py_alpaca_api/__init__.py
--rw-r--r--   0        0        0     2143 2024-05-14 02:56:26.383431 py_alpaca_api-0.3.5/py_alpaca_api/alpaca.py
--rw-r--r--   0        0        0        0 2024-05-14 02:56:26.383431 py_alpaca_api-0.3.5/py_alpaca_api/src/__init__.py
--rw-r--r--   0        0        0     3292 2024-05-14 02:56:26.383431 py_alpaca_api-0.3.5/py_alpaca_api/src/account.py
--rw-r--r--   0        0        0     1947 2024-05-14 02:56:26.383431 py_alpaca_api-0.3.5/py_alpaca_api/src/asset.py
--rw-r--r--   0        0        0    19461 2024-05-14 02:56:26.383431 py_alpaca_api-0.3.5/py_alpaca_api/src/data_classes.py
--rw-r--r--   0        0        0     6618 2024-05-14 02:56:26.383431 py_alpaca_api-0.3.5/py_alpaca_api/src/history.py
--rw-r--r--   0        0        0     1046 2024-05-14 02:56:26.383431 py_alpaca_api-0.3.5/py_alpaca_api/src/market.py
--rw-r--r--   0        0        0    17950 2024-05-14 02:56:26.383431 py_alpaca_api-0.3.5/py_alpaca_api/src/order.py
--rw-r--r--   0        0        0    14431 2024-05-14 02:56:26.383431 py_alpaca_api-0.3.5/py_alpaca_api/src/position.py
--rw-r--r--   0        0        0     1279 2024-05-14 02:56:26.383431 py_alpaca_api-0.3.5/pyproject.toml
--rw-r--r--   0        0        0    13337 1970-01-01 00:00:00.000000 py_alpaca_api-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-11 23:37:32.674625 py_alpaca_api-0.4.0/LICENSE
+-rw-r--r--   0        0        0    17299 2024-05-15 03:25:08.684820 py_alpaca_api-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-11 00:31:44.448417 py_alpaca_api-0.4.0/py_alpaca_api/__init__.py
+-rw-r--r--   0        0        0     2326 2024-05-16 00:32:12.422600 py_alpaca_api-0.4.0/py_alpaca_api/alpaca.py
+-rw-r--r--   0        0        0        0 2024-05-14 02:56:26.383431 py_alpaca_api-0.4.0/py_alpaca_api/src/__init__.py
+-rw-r--r--   0        0        0     3025 2024-05-16 00:32:12.422600 py_alpaca_api-0.4.0/py_alpaca_api/src/account.py
+-rw-r--r--   0        0        0     2494 2024-05-16 00:32:12.422600 py_alpaca_api-0.4.0/py_alpaca_api/src/asset.py
+-rw-r--r--   0        0        0    20501 2024-05-16 00:32:12.422600 py_alpaca_api-0.4.0/py_alpaca_api/src/data_classes.py
+-rw-r--r--   0        0        0     7736 2024-05-16 00:32:12.422600 py_alpaca_api-0.4.0/py_alpaca_api/src/history.py
+-rw-r--r--   0        0        0     2102 2024-05-16 00:32:12.422600 py_alpaca_api-0.4.0/py_alpaca_api/src/market.py
+-rw-r--r--   0        0        0    18665 2024-05-16 00:32:12.422600 py_alpaca_api-0.4.0/py_alpaca_api/src/order.py
+-rw-r--r--   0        0        0    14954 2024-05-16 00:32:12.422600 py_alpaca_api-0.4.0/py_alpaca_api/src/position.py
+-rw-r--r--   0        0        0    21192 2024-05-16 00:32:12.422600 py_alpaca_api-0.4.0/py_alpaca_api/src/watchlist.py
+-rw-r--r--   0        0        0     1279 2024-05-16 00:32:12.422600 py_alpaca_api-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    18060 1970-01-01 00:00:00.000000 py_alpaca_api-0.4.0/PKG-INFO
```

### Comparing `py_alpaca_api-0.3.5/LICENSE` & `py_alpaca_api-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.3.5/py_alpaca_api/alpaca.py` & `py_alpaca_api-0.4.0/py_alpaca_api/alpaca.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,61 +1,63 @@
-from .src.account import Account
-from .src.asset import Asset
-from .src.history import History
-from .src.market import Market
-from .src.order import Order
-from .src.position import Position
-
-
-# PyAlpacaApi class
-class PyAlpacaApi:
-    def __init__(self, api_key: str, api_secret: str, api_paper: bool = True):
-        """Initialize PyAlpacaApi class
-
-        Parameters:
-        -----------
-        api_key:    Alpaca API Key
-                    A valid Alpaca API Key string required
-
-        api_secret: Alpaca API Secret
-                    A valid Alpaca API Secret string required
-
-        api_paper:  Alpaca Paper Trading
-                    Alpaca Paper Trading (default: True) bool
-
-        Raises:
-        -------
-        ValueError:
-            ValueError if API Key is not provided
-
-        ValueError:
-            ValueError if API Secret is not provided
-
-        Example:
-        --------
-        >>> PyAlpacaApi(api_key="API", api_secret="SECRET", api_paper=True)
-        PyAlpacaApi()
-        """  # noqa
-        # Check if API Key and Secret are provided
-        if not api_key:
-            raise ValueError("API Key is required")
-        if not api_secret:
-            raise ValueError("API Secret is required")
-        # Set the API Key and Secret
-        self.headers = {
-            "APCA-API-KEY-ID": api_key,
-            "APCA-API-SECRET-KEY": api_secret,
-        }
-        # Set the API URL's
-        if api_paper:
-            self.trade_url = "https://paper-api.alpaca.markets/v2"
-        else:
-            self.trade_url = "https://api.alpaca.markets/v2"
-
-        self.data_url = "https://data.alpaca.markets/v2"
-
-        self.account = Account(trade_url=self.trade_url, headers=self.headers)
-        self.asset = Asset(trade_url=self.trade_url, headers=self.headers)
-        self.history = History(data_url=self.data_url, headers=self.headers, asset=self.asset)
-        self.position = Position(trade_url=self.trade_url, headers=self.headers, account=self.account)
-        self.order = Order(trade_url=self.trade_url, headers=self.headers)
-        self.market = Market(trade_url=self.trade_url, headers=self.headers)
+from .src.account import Account
+from .src.asset import Asset
+from .src.history import History
+from .src.market import Market
+from .src.order import Order
+from .src.position import Position
+from .src.watchlist import Watchlist
+
+
+# PyAlpacaApi class
+class PyAlpacaApi:
+    def __init__(self, api_key: str, api_secret: str, api_paper: bool = True):
+        """Initialize PyAlpacaApi class
+
+        Parameters:
+        -----------
+        api_key:    Alpaca API Key
+                    A valid Alpaca API Key string required
+
+        api_secret: Alpaca API Secret
+                    A valid Alpaca API Secret string required
+
+        api_paper:  Alpaca Paper Trading
+                    Alpaca Paper Trading (default: True) bool
+
+        Raises:
+        -------
+        ValueError:
+            ValueError if API Key is not provided
+
+        ValueError:
+            ValueError if API Secret is not provided
+
+        Example:
+        --------
+        >>> PyAlpacaApi(api_key="API", api_secret="SECRET", api_paper=True)
+        PyAlpacaApi()
+        """  # noqa
+        # Check if API Key and Secret are provided
+        if not api_key:
+            raise ValueError("API Key is required")
+        if not api_secret:
+            raise ValueError("API Secret is required")
+        # Set the API Key and Secret
+        self.headers = {
+            "APCA-API-KEY-ID": api_key,
+            "APCA-API-SECRET-KEY": api_secret,
+        }
+        # Set the API URL's
+        if api_paper:
+            self.trade_url = "https://paper-api.alpaca.markets/v2"
+        else:
+            self.trade_url = "https://api.alpaca.markets/v2"
+
+        self.data_url = "https://data.alpaca.markets/v2"
+
+        self.account = Account(trade_url=self.trade_url, headers=self.headers)
+        self.asset = Asset(trade_url=self.trade_url, headers=self.headers)
+        self.history = History(data_url=self.data_url, headers=self.headers, asset=self.asset)
+        self.position = Position(trade_url=self.trade_url, headers=self.headers, account=self.account)
+        self.order = Order(trade_url=self.trade_url, headers=self.headers)
+        self.market = Market(trade_url=self.trade_url, headers=self.headers)
+        self.watchlist = Watchlist(trade_url=self.trade_url, headers=self.headers)
```

### Comparing `py_alpaca_api-0.3.5/py_alpaca_api/src/data_classes.py` & `py_alpaca_api-0.4.0/py_alpaca_api/src/data_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -288,14 +288,43 @@
     daytrade_count: int
     balance_asof: str
     crypto_tier: int
     intraday_adjustments: int
     pending_reg_taf_fees: float
 
 
+@dataclass
+class WatchlistClass:
+    id: str
+    account_id: str
+    created_at: datetime
+    updated_at: datetime
+    name: str
+    assets: object
+
+
+def watchlist_class_from_dict(data_dict: dict) -> WatchlistClass:
+    return WatchlistClass(
+        id=str(data_dict["id"] if data_dict["id"] else ""),
+        account_id=str(data_dict["account_id"] if data_dict["account_id"] else ""),
+        created_at=(
+            datetime.strptime(data_dict["created_at"].split(".")[0].replace("T", " "), "%Y-%m-%d %H:%M:%S")
+            if data_dict["created_at"]
+            else datetime.date(0, 0, 0)
+        ),
+        updated_at=(
+            datetime.strptime(data_dict["updated_at"].split(".")[0].replace("T", " "), "%Y-%m-%d %H:%M:%S")
+            if data_dict["updated_at"]
+            else datetime.date(0, 0, 0)
+        ),
+        name=str(data_dict["name"] if data_dict["name"] else ""),
+        assets=[asset_class_from_dict(sym) for sym in data_dict["assets"] if len(data_dict["assets"]) > 0] if data_dict["assets"] else None,
+    )
+
+
 ############################################
 # Data Class Clock Conversion Functions
 ############################################
 def clock_class_from_dict(data_dict: dict) -> ClockClass:
     """Converts a dictionary to a ClockClass object.
 
     Parameters:
```

### Comparing `py_alpaca_api-0.3.5/py_alpaca_api/src/order.py` & `py_alpaca_api-0.4.0/py_alpaca_api/src/order.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,49 +3,86 @@
 import requests
 
 from .data_classes import OrderClass, order_class_from_dict
 
 
 class Order:
     def __init__(self, trade_url: str, headers: object) -> None:
+        """Initialize Order class
+
+        Parameters:
+        ___________
+        trade_url: str
+                Alpaca Trade API URL required
+
+        headers: object
+                API request headers required
+
+        Raises:
+        _______
+        ValueError: If trade URL is not provided
+
+        ValueError: If headers are not provided
+        """  # noqa
+
         self.trade_url = trade_url
         self.headers = headers
 
     #########################################################
     # \\\\\\\\\/////////  Get Order BY id \\\\\\\///////////#
     #########################################################
     def get_by_id(self, order_id: str, nested: bool = False) -> OrderClass:
         """Get order information by order ID
 
         Parameters:
         -----------
         order_id:   Order ID to get information
                     A valid order ID string required
 
-        nested:     Include nested information (default: False)
-                    Include nested information in the response (optional) bool
+        nested:     Include nested objects (default: False)
+                    Include nested objects (optional) bool
 
         Returns:
         --------
-        OrderClass: Order information as an OrderClass object with values:
-                    id, client_order_id, created_at, submitted_at, asset_id, symbol, asset_class, notional, qty, filled_qty, filled_avg_price,
-                    order_class, order_type
+        OrderClass: Order information as an OrderClass object
 
         Raises:
         -------
-        ValueError: 
-            ValueError if failed to get order information
-        
+        ValueError: If failed to get order information
+
         Example:
         --------
-        >>> get_order_by_id(order_id="ORDER_ID")
-        OrderClass(id='ORDER_ID', client_order_id='CLIENT_ORDER_ID', created_at='2021-10-01T00:00:00Z', \
-                submitted_at='2021-10-01 00:00:00', asset_id='ASSET_ID', symbol='AAPL', asset_class='us_equity', \
-                notional=1000.0, qty=10.0, filled_qty=10.0, filled_avg_price=100.0, order_class='simple', order_type='market')
+        >>> from py_alpaca_api import PyAlpacaApi
+            api = PyAlpacaApi(api_key="API", api_secret="SECRET", api_paper=True)
+            order = api.order.get_by_id(order_id="ORDER_ID")
+            print(order)
+
+        OrderClass(
+            id="ORDER_ID",
+            client_order_id="CLIENT_ORDER_ID",
+            created_at="2021-10-01T00:00:00Z",
+            submitted_at="2021-10-01 00:00:00",
+            asset_id="ASSET_ID",
+            symbol="AAPL",
+            asset_class="us_equity",
+            notional=1000.0,
+            qty=10.0,
+            filled_qty=10.0,
+            filled_avg_price=100.0,
+            order_class="simple",
+            order_type="market",
+            limit_price=None,
+            stop_price=None,
+            status="new",
+            side="buy",
+            time_in_force="day",
+            extended_hours=False
+        )
         """  # noqa
+
         # Parameters for the request
         params = {"nested": nested}
         # Alpaca API URL for order information
         url = f"{self.trade_url}/orders/{order_id}"
         # Get request to Alpaca API for order information
         response = requests.get(url, headers=self.headers, params=params)
         # Check if response is successful
@@ -72,22 +109,26 @@
 
         Returns:
         --------
         str:        Order cancellation confirmation message
 
         Raises:
         -------
-        Exception:
-            Exception if failed to cancel order
+        Exception:  If failed to cancel order
 
         Example:
         --------
-        >>> cancel_order_by_id(order_id="ORDER_ID")
-        'Order ORDER_ID has been cancelled'
+        >>> from py_alpaca_api import PyAlpacaApi
+            api = PyAlpacaApi(api_key="API", api_secret="SECRET", api_paper=True)
+            order = api.order.cancel_by_id(order_id="ORDER_ID")
+            print(order)
+
+        Order ORDER_ID has been cancelled
         """  # noqa
+
         # Alpaca API URL for canceling an order
         url = f"{self.trade_url}/orders/{order_id}"
         # Delete request to Alpaca API for canceling an order
         response = requests.delete(url, headers=self.headers)
         # Check if response is successful
         if response.status_code == 204:
             # Convert JSON response to dictionary
@@ -105,17 +146,26 @@
 
         Returns:
         --------
         str:        Order cancellation confirmation message
 
         Raises:
         -------
-        Exception:
-            Exception if failed to cancel all orders
+        Exception:  If failed to cancel all orders
+
+        Example:
+        --------
+        >>> from py_alpaca_api import PyAlpacaApi
+            api = PyAlpacaApi(api_key="API", api_secret="SECRET", api_paper=True)
+            order = api.order.cancel_all()
+            print(order)
+
+        10 orders have been cancelled
         """  # noqa
+
         # Alpaca API URL for canceling all orders
         url = f"{self.trade_url}/orders"
         # Delete request to Alpaca API for canceling all orders
         response = requests.delete(url, headers=self.headers)
         # Check if response is successful
         if response.status_code == 207:
             # Convert JSON response to dictionary
@@ -134,30 +184,30 @@
         symbol: str,
         qty: float = None,
         notional: float = None,
         side: str = "buy",
         time_in_force: str = "day",
         extended_hours: bool = False,
     ) -> OrderClass:
-        """Submit a market order
+        """Submit a Market Order
 
         Parameters:
         -----------
         symbol:         Asset symbol to buy/sell
                         A valid asset symbol string required
-        
+
         qty:            Quantity of asset to buy/sell (default: None)
                         Quantity of asset to buy/sell (optional) float
 
         notional:       Notional value of asset to buy/sell (default: None)
                         Notional value of asset to buy/sell (optional) float
-                    
+
         side:           Order side (buy/sell) (default: buy)
                         Order side (buy/sell) (optional) str
-                    
+
         time_in_force:  Time in force options (day, gtc, opg, cls, ioc, fok) (default: day)
                         Time in force options (optional) str
 
         extended_hours: Extended hours trading (default: False)
                         Extended hours trading (optional) bool
 
         Returns:
@@ -171,24 +221,25 @@
         Raises:
         -------
         Exception: 
             Exception if failed to submit market order
 
         Example:
         --------
-        >>> market_order(symbol="AAPL", qty=10)
-        MarketOrderClass(id='ORDER_ID', client_order_id='CLIENT_ORDER_ID', created_at='2021-10-01T00:00:00Z', \
-                submitted_at='2021-10-01 00:00:00', asset_id='ASSET_ID', symbol='AAPL', asset_class='us_equity', \
-                notional=1000.0, qty=10.0, filled_qty=10.0, filled_avg_price=100.0, order_class='simple', order_type='market')
+        >>> from py_alpaca_api import PyAlpacaApi
+            api = PyAlpacaApi(api_key="API", api_secret="SECRET", api_paper=True)
+            order = api.order.market(symbol="AAPL", qty=10)
+            print(order)
 
-        >>> market_order(symbol="AAPL", notional=1000)
         MarketOrderClass(id='ORDER_ID', client_order_id='CLIENT_ORDER_ID', created_at='2021-10-01T00:00:00Z', \
                 submitted_at='2021-10-01 00:00:00', asset_id='ASSET_ID', symbol='AAPL', asset_class='us_equity', \
-                notional=1000.0, qty=10.0, filled_qty=10.0, filled_avg_price=100.0, order_class='simple', order_type='market')
+                notional=1000.0, qty=10.0, filled_qty=10.0, filled_avg_price=100.0, order_class='simple', order_type='market', \
+                limit_price=None, stop_price=None, status='new', side='buy', time_in_force='day', extended_hours=False)
         """  # noqa
+
         # Alpaca API URL for submitting market order
         url = f"{self.trade_url}/orders"
         # Market order payload
         payload = {
             "symbol": symbol,
             "qty": qty if qty else None,
             "notional": round(notional, 2) if notional else None,
@@ -228,15 +279,15 @@
         Parameters:
         -----------
         symbol:         Asset symbol to buy/sell
                         A valid asset symbol string required
 
         limit_price:    Limit price for the order
                         Limit price for the order float required
-                
+
         qty:            Quantity of asset to buy/sell (default: None)
                         Quantity of asset to buy/sell (optional) float
 
         notional:       Notional value of asset to buy/sell (default: None)
                         Notional value of asset to buy/sell (optional) float
 
         side:           Order side (buy/sell) (default: buy)
@@ -247,38 +298,47 @@
 
         extended_hours: Extended hours trading (default: False)
                         Extended hours trading (optional) bool
 
         Returns:
         --------
         MarketOrderClass: Market order information as a MarketOrderClass object with
-                            values: id, client_order_id, created_at, submitted_at, asset_id, symbol, \
-                            asset_class, notional, qty, filled_qty, filled_avg_price, order_class, \
-                            order_type , limit_price, stop_price, filled_qty, filled_avg_price, \
-                            status, type, side, time_in_force, extended_hours
-        
+                            values: id, client_order_id, created_at, submitted_at, asset_id, symbol, asset_class, 
+                            notional, qty, filled_qty, filled_avg_price, order_class, order_type , limit_price, 
+                            stop_price, filled_qty, filled_avg_price, status, type, side, time_in_force, extended_hours
+
         Raises:
         -------
         Exception: 
             Exception if failed to submit limit order
-        
+
         Example:
         --------
-        >>> limit_order(symbol="AAPL", limit_price=100, qty=10)
+        >>> from py_alpaca_api import PyAlpacaApi
+            api = PyAlpacaApi(api_key="API", api_secret="SECRET", api_paper=True)
+            order = api.order.limit(symbol="AAPL", limit_price=100, qty=10)
+            print(order)
+
         MarketOrderClass(id='ORDER_ID', client_order_id='CLIENT_ORDER_ID', created_at='2021-10-01T00:00:00Z', \
                 submitted_at='2021-10-01 00:00:00', asset_id='ASSET_ID', symbol='AAPL', asset_class='us_equity', \
                 notional=1000.0, qty=10.0, filled_qty=10.0, filled_avg_price=100.0, order_class='simple', order_type='limit', \
                 limit_price=100.0, stop_price=None, status='new', side='buy', time_in_force='day', extended_hours=False)
 
-        >>> limit_order(symbol="AAPL", limit_price=100, notional=1000)
+        >>> from py_alpaca_api import PyAlpacaApi
+            api = PyAlpacaApi(api_key="API", api_secret="SECRET", api_paper=True)
+            order = api.order.limit(symbol="AAPL", limit_price=100, notional=1000)
+            print(order)
+
         MarketOrderClass(id='ORDER_ID', client_order_id='CLIENT_ORDER_ID', created_at='2021-10-01T00:00:00Z', \
                 submitted_at='2021-10-01 00:00:00', asset_id='ASSET_ID', symbol='AAPL', asset_class='us_equity', \
                 notional=1000.0, qty=10.0, filled_qty=10.0, filled_avg_price=100.0, order_class='simple', order_type='limit', \
                 limit_price=100.0, stop_price=None, status='new', side='buy', time_in_force='day', extended_hours=False)
+
         """  # noqa
+
         # Alpaca API URL for submitting market order
         url = f"{self.trade_url}/orders"
         # Market order payload
         payload = {
             "symbol": symbol,  # Asset symbol to buy/sell
             "limit_price": limit_price,  # Limit price for the order
             "qty": (qty if qty else None),  # Check if qty is provided, if not, set to None
@@ -325,46 +385,46 @@
 
         qty:            Quantity of asset to buy/sell
                         Quantity of asset to buy/sell float required
 
         side:           Order side (buy/sell) (default: buy)
                         Order side (buy/sell) (optional) str
 
-        time_in_force:  Time in force options (day, gtc, opg, cls, ioc, fok) (default: day) 
+        time_in_force:  Time in force options (day, gtc, opg, cls, ioc, fok) (default: day)
                         Time in force options (optional) str
 
-        extended_hours: Extended hours trading (default: False) 
+        extended_hours: Extended hours trading (default: False)
                         Extended hours trading (optional) bool
 
         Returns:
         --------
         MarketOrderClass: Market order information as a MarketOrderClass object with
                             values: id, client_order_id, created_at, submitted_at, asset_id, symbol, asset_class, 
                             notional, qty, filled_qty, filled_avg_price, order_class, order_type , limit_price, 
                             stop_price, filled_qty, filled_avg_price, status, type, side, time_in_force, extended_hours
 
-        Raises: 
+        Raises:
         -------
         Exception: 
             Exception if failed to submit stop order
 
-        Example:    
+        Example:
         --------
-        >>> stop_order(symbol="AAPL", stop_price=100, qty=10)
+        >>> from py_alpaca_api import PyAlpacaApi
+            api = PyAlpacaApi(api_key="API", api_secret="SECRET", api_paper=True)
+            order = api.order.stop(symbol="AAPL", stop_price=100, qty=10)
+            print(order)
+
         MarketOrderClass(id='ORDER_ID', client_order_id='CLIENT_ORDER_ID', created_at='2021-10-01T00:00:00Z', \
                 submitted_at='2021-10-01 00:00:00', asset_id='ASSET_ID', symbol='AAPL', asset_class='us_equity', \
                 notional=1000.0, qty=10.0, filled_qty=10.0, filled_avg_price=100.0, order_class='simple', order_type='stop', \
                 limit_price=None, stop_price=100.0, status='new', side='buy', time_in_force='day', extended_hours=False)
 
-        >>> stop_order(symbol="AAPL", stop_price=100, qty=10, side="sell")
-        MarketOrderClass(id='ORDER_ID', client_order_id='CLIENT_ORDER_ID', created_at='2021-10-01T00:00:00Z', \
-                submitted_at='2021-10-01 00:00:00', asset_id='ASSET_ID', symbol='AAPL', asset_class='us_equity', \
-                notional=1000.0, qty=10.0, filled_qty=10.0, filled_avg_price=100.0, order_class='simple', order_type='stop', \
-                limit_price=None, stop_price=100.0, status='new', side='sell', time_in_force='day', extended_hours=False)
         """  # noqa
+
         # Alpaca API URL for submitting market order
         url = f"{self.trade_url}/orders"
         # Market order payload
         payload = {
             "symbol": symbol,  # Asset symbol to buy/sell
             "stop_price": stop_price,  # Stop price for the order
             "qty": qty,  # Quantity of asset to buy/sell
```

### Comparing `py_alpaca_api-0.3.5/py_alpaca_api/src/position.py` & `py_alpaca_api-0.4.0/py_alpaca_api/src/position.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,41 +5,72 @@
 
 from .account import Account
 from .data_classes import PositionClass, position_class_from_dict
 
 
 class Position:
     def __init__(self, trade_url: str, headers: object, account: Account) -> None:
+        """Initialize Position class
+
+        Parameters:
+        ___________
+        trade_url: str
+                Alpaca Trade API URL required
+
+        headers: object
+                API request headers required
+
+        account: Account
+                Account object required
+
+        Raises:
+        _______
+        ValueError: If trade URL is not provided
+
+        ValueError: If headers are not provided
+
+        ValueError: If account is not provided
+
+        """  # noqa
+
         self.trade_url = trade_url
         self.headers = headers
         self.account = account
 
     ########################################################
     # \\\\\\\\\\\\\\\\\ Get Positions /////////////////////#
     ########################################################
     def get_all(self) -> pd.DataFrame:
-        """Get account positions, including cash
+        """Get all positions information from Alpaca API
 
         Returns:
         --------
-        DataFrame:  Account positions as a DataFrame with columns:
-                    asset_id, symbol, exchange, asset_class, qty, qty_available, side, market_value, cost_basis, profit_dol, profit_pct,
-                    intraday_profit_dol, intraday_profit_pct, portfolio_pct, current_price, lastday_price, change_today, asset_marginable
+        pd.DataFrame:   All positions information as a DataFrame with columns:
+                    asset_id, symbol, exchange, asset_class, avg_entry_price, qty, qty_available, side, market_value, cost_basis,
+                    profit_dol, profit_pct, intraday_profit_dol, intraday_profit_pct, portfolio_pct, current_price, lastday_price,
+                    change_today, asset_marginable
 
         Raises:
         -------
-        Exception:
-            Exception if failed to get account positions
+        Exception: If failed to get positions information
 
         Example:
         --------
-        >>> get_positions()
-            asset_id    symbol  exchange    asset_class qty qty_available   side    market_value    cost_basis  profit_dol  profit_pct  intraday_profit_dol intraday_profit_pct portfolio_pct   current_price   lastday_price   change_today    asset_marginable
-        0   ""          Cash    ""          ""          0   0               ""      1000.0          0.0         0.0         0.0         0.0                 0.0                 1.0             1.0             1.0             0.0             False
-        1   ASSET_ID    AAPL    NASDAQ      us_equity   10  10              long    1000.0          1000.0      0.0         0.0         0.0                 0.0                 0.0             100.0           100.0           0.0             True
+        >>> from py_alpaca_api import PyAlpacaApi
+            api = PyAlpacaApi(api_key="API", api_secret="SECRET", api_paper=True)
+            positions = api.position.get_all()
+            print(positions)
+
+        asset_id symbol exchange asset_class  avg_entry_price  qty  qty_available  side  market_value  cost_basis  profit_dol  profit_pct  \
+        0           Cash  Cash         Cash          0.0000  0.0            0.0  Cash       10000.0         0.0         0.0      0.000
+        1  ASSET_ID   AAPL   NASDAQ   us_equity        100.0000  10.0           10.0  long       1000.0      1000.0         0.0      0.000
+
+        intraday_profit_dol  intraday_profit_pct  portfolio_pct  current_price  lastday_price  change_today  asset_marginable
+        0                  0.0                0.000         1.0000            0.0            0.0           0.0             False
+        1                  0.0                0.000         0.1000          100.0          100.0           0.0              True
         """  # noqa
 
         # Url for positions
         url = f"{self.trade_url}/positions"
         # Get request to Alpaca API for positions
         response = requests.get(url, headers=self.headers)
         # Check if response is successful
@@ -123,56 +154,69 @@
 
         return pos_data_df
 
     ########################################################
     # \\\\\\\\\\\\\\\\\ Get Position //////////////////////#
     ########################################################
     def get(self, symbol: str = None, symbol_dict: dict = None) -> PositionClass:
-        """Get position information by symbol or symbol dictionary
+        """Get position information by symbol or asset ID
 
         Parameters:
         -----------
-        symbol:     Asset symbol to get position information
-                    A valid asset symbol string (e.g., AAPL, or asset_id) optional, not required if symbol_dict is provided
+        symbol:         Asset symbol to get position information
+                        A valid asset symbol string (optional) str
 
-        symbol_dict: Position information dictionary
-                    A valid position information dictionary optional, not required if symbol is provided
+        symbol_dict:    Asset symbol dictionary to get position information
+                        A valid asset symbol dictionary (optional) dict
 
         Returns:
         --------
-        PositionClass: Position information as a PositionClass object with values:
-                    asset_id, symbol, exchange, asset_class, qty, qty_available, side, market_value, cost_basis, profit_dol, profit_pct,
-                    intraday_profit_dol, intraday_profit_pct, portfolio_pct, current_price, lastday_price, change_today, asset_marginable
+        PositionClass:  Position information as a PositionClass object with attributes:
+                    asset_id, symbol, exchange, asset_class, avg_entry_price, qty, qty_available, side, market_value, cost_basis,
+                    profit_dol, profit_pct, intraday_profit_dol, intraday_profit_pct, portfolio_pct, current_price, lastday_price,
+                    change_today, asset_marginable
 
         Raises:
         -------
-        ValueError:
-            ValueError if symbol or symbol_dict is not provided
+        ValueError:     ValueError if symbol or symbol_dict is not provided
 
-        ValueError:
-            ValueError if both symbol and symbol_dict are provided
+        ValueError:     ValueError if both symbol and symbol_dict are provided
 
-        ValueError:
-            ValueError if failed to get position information
+        Exception:      Exception if failed to get position information
 
         Example:
         --------
-        >>> get_position(symbol="AAPL")
-        PositionClass(asset_id='ASSET_ID', symbol='AAPL', exchange='NASDAQ', asset_class='us_equity', qty=10.0, qty_available=10.0, \
-                    side='long', market_value=1000.0, cost_basis=1000.0, profit_dol=0.0, profit_pct=0.0, intraday_profit_dol=0.0, \
-                    intraday_profit_pct=0.0, portfolio_pct=1.0, current_price=100.0, lastday_price=100.0, change_today=0.0, asset_marginable=True)
-
-        >>> get_position(symbol_dict={"asset_id": "ASSET_ID", "symbol": "AAPL", "exchange": "NASDAQ", "asset_class": "us_equity", \
-                    "qty": 10.0, "qty_available": 10.0, "side": "long", "market_value": 1000.0, "cost_basis": 1000.0, "profit_dol": 0.0, \
-                    "profit_pct": 0.0, "intraday_profit_dol": 0.0, "intraday_profit_pct": 0.0, "portfolio_pct": 1.0, "current_price": 100.0, \
-                    "lastday_price": 100.0, "change_today": 0.0, "asset_marginable": True})
-        PositionClass(asset_id='ASSET_ID', symbol='AAPL', exchange='NASDAQ', asset_class='us_equity', qty=10.0, qty_available=10.0, \
-                    side='long', market_value=1000.0, cost_basis=1000.0, profit_dol=0.0, profit_pct=0.0, intraday_profit_dol=0.0, \
-                    intraday_profit_pct=0.0, portfolio_pct=1.0, current_price=100.0, lastday_price=100.0, change_today=0.0, asset_marginable=True)
+        >>> from py_alpaca_api import PyAlpacaApi
+            api = PyAlpacaApi(api_key="API", api_secret="SECRET", api_paper=True)
+            position = api.position.get(symbol="AAPL")
+            print(position)
+
+        PositionClass(
+            asset_id="375f6b6e-3b5f-4b2b-8f6b-2e6b2a6b2e6b",
+            symbol="AAPL",
+            exchange="NASDAQ",
+            asset_class="us_equity",
+            avg_entry_price=100.0,
+            qty=10.0,
+            qty_available=10.0,
+            side="long",
+            market_value=1000.0,
+            cost_basis=1000.0,
+            profit_dol=0.0,
+            profit_pct=0.0,
+            intraday_profit_dol=0.0,
+            intraday_profit_pct=0.0,
+            portfolio_pct=0.1,
+            current_price=100.0,
+            lastday_price=100.0,
+            change_today=0.0,
+            asset_marginable=True
+        )
         """  # noqa
+
         # Check if symbol or symbol_dict is provided
         if not symbol and not symbol_dict:
             # Raise ValueError if symbol or symbol_dict is not provided
             raise ValueError("Symbol or symbol_dict is required.")
         # Check if both symbol and symbol_dict are provided
         if symbol and symbol_dict:
             # Raise ValueError if both symbol and symbol_dict are provided
@@ -212,35 +256,39 @@
         # Return position information as a PositionClass object
         return position_class_from_dict(res_dict)
 
     ########################################################
     # \\\\\\\\\\\\\\\\ Close All Positions ////////////////#
     ########################################################
     def close_all(self, cancel_orders: bool = False) -> str:
-        """Close all positions
+        """Close all positions from Alpaca API
 
         Parameters:
         -----------
         cancel_orders:  Cancel open orders (default: False)
-                        Cancel open orders before closing positions (optional) bool
+                        Cancel open orders (optional) bool
 
         Returns:
         --------
-        str:            Position closing confirmation message
+        str:            Text message for closing all positions confirmation
 
         Raises:
         -------
-        Exception:
-            Exception if failed to close positions
+        Exception:      Exception if failed to close positions
 
         Example:
         --------
-        >>> close_all_positions()
-        '2 positions have been closed'
+        >>> from py_alpaca_api import PyAlpacaApi
+            api = PyAlpacaApi(api_key="API", api_secret="SECRET", api_paper=True)
+            message = api.position.close_all()
+            print(message)
+
+        '1 positions have been closed'
         """  # noqa
+
         # Url for positions
         url = f"{self.trade_url}/positions"
         # Parameters for the request
         params = {"cancel_orders": cancel_orders}
         # Delete request to Alpaca API for closing all positions
         response = requests.delete(url, headers=self.headers, params=params)
         # Check if response is successful
@@ -254,51 +302,50 @@
             res = json.loads(response.text)
             raise Exception(f'Failed to close positions. Response: {res["message"]}')
 
     ########################################################
     # \\\\\\\\\\\\\\\\\\ Close Position ///////////////////#
     ########################################################
     def close(self, symbol_or_id: str, qty: float = None, percentage: int = None) -> str:
-        """Close a position by symbol or asset ID
+        """Close position by symbol or asset ID from Alpaca API
 
         Parameters:
         -----------
         symbol_or_id:   Asset symbol or asset ID to close position
                         A valid asset symbol or asset ID string required
 
-        qty:            Quantity to close position (default: None)
+        qty:            Quantity to close position (optional)
                         Quantity to close position (optional) float
 
-        percentage:     Percentage to close position (default: None)
+        percentage:     Percentage to close position (optional)
                         Percentage to close position (optional) int
 
         Returns:
         --------
-        str:            Position closing confirmation message
+        str:            Text message for closing position confirmation
 
         Raises:
         -------
-        ValueError:
-            ValueError if quantity or percentage is not provided
+        ValueError:     ValueError if quantity or percentage is not provided
 
-        ValueError:
-            ValueError if both quantity and percentage are provided
+        ValueError:     ValueError if both quantity and percentage are provided
 
-        ValueError:
-            ValueError if percentage is not between 0 and 100
+        ValueError:     ValueError if percentage is not between 0 and 100
 
-        ValueError:
-            ValueError if symbol or asset_id is not provided
+        ValueError:     ValueError if symbol or asset_id is not provided
 
-        Exception:
-            Exception if failed to close position
+        Exception:      Exception if failed to close position
 
         Example:
         --------
-        >>> close_position(symbol_or_id="AAPL", qty=10)
+        >>> from py_alpaca_api import PyAlpacaApi
+            api = PyAlpacaApi(api_key="API", api_secret="SECRET", api_paper=True)
+            message = api.position.close(symbol_or_id="AAPL", qty=10)
+            print(message)
+
         'Position AAPL has been closed'
         """  # noqa
 
         # Check if quantity or percentage is provided
         if not qty and not percentage:
             raise ValueError("Quantity or percentage is required.")
         # Check if both quantity and percentage are provided
```

### Comparing `py_alpaca_api-0.3.5/pyproject.toml` & `py_alpaca_api-0.4.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-alpaca-api"
-version = "0.3.5"
+version = "0.4.0"
 description = "Python package, for communicating with Alpaca Markets REST API."
 authors = ["TexasCoding <jeff10278@me.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/TexasCoding/py-alpaca-api"
 repository = "https://github.com/TexasCoding/py-alpaca-api"
 documentation = "https://py-alpaca-api.readthedocs.io/en/latest/"
```

### Comparing `py_alpaca_api-0.3.5/PKG-INFO` & `py_alpaca_api-0.4.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,18 @@
-Metadata-Version: 2.1
-Name: py-alpaca-api
-Version: 0.3.5
-Summary: Python package, for communicating with Alpaca Markets REST API.
-Home-page: https://github.com/TexasCoding/py-alpaca-api
-License: MIT
-Keywords: alpaca,python
-Author: TexasCoding
-Author-email: jeff10278@me.com
-Requires-Python: >=3.12,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: numpy (>=1.26.4,<2.0.0)
-Requires-Dist: pandas (>=2.2.2,<3.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
-Project-URL: Documentation, https://py-alpaca-api.readthedocs.io/en/latest/
-Project-URL: Repository, https://github.com/TexasCoding/py-alpaca-api
-Description-Content-Type: text/markdown
-
 <p align="center">
   <img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" alt="project-logo">
 </p>
 <p align="center">
     <h1 align="center">PY-ALPACA-API</h1>
 </p>
 <p align="center">
-    <em>Unlock Alpacas Power with Seamless API Integration"</em>
+    <em>Empowering traders with precision and control.</em>
 </p>
 <p align="center">
+<img alt="GitHub Actions Workflow Status" src="https://img.shields.io/github/actions/workflow/status/TexasCoding/py-alpaca-api/.github%2Fworkflows%2Ftest-package.yml?logo=github">
 	<img src="https://img.shields.io/github/license/TexasCoding/py-alpaca-api?style=default&logo=opensourceinitiative&logoColor=white&color=0080ff" alt="license">
 	<img src="https://img.shields.io/github/last-commit/TexasCoding/py-alpaca-api?style=default&logo=git&logoColor=white&color=0080ff" alt="last-commit">
 	<img src="https://img.shields.io/github/languages/top/TexasCoding/py-alpaca-api?style=default&color=0080ff" alt="repo-top-language">
 	<img src="https://img.shields.io/github/languages/count/TexasCoding/py-alpaca-api?style=default&color=0080ff" alt="repo-language-count">
 <p>
 <p align="center">
 	<!-- default option, no dependency badges. -->
@@ -54,93 +35,134 @@
 - [License](#license)
 - [Acknowledgments](#acknowledgments)
 </details>
 <hr>
 
 ##  Overview
 
-The py-alpaca-api project is a Python library that simplifies interaction with the Alpaca API. It provides a robust interface, encapsulated in the `PyAlpacaApi` class, enabling developers to access Alpaca Market API trading functionalities effortlessly. By utilizing data classes for orders, assets, and accounts, the project abstracts away complexities, enhancing flexibility in processing API responses. With clear metadata management through Poetry, this project serves as a valuable tool for those looking to integrate Alpaca trading capabilities seamlessly into their applications.
-
-This project is still in development. New functionality will be added and updated daily. Hopefully this project will help make communicating with Alpaca Markets API, much easier for some. Any input or help would be appreciated.
+Py-alpaca-api is a robust Python library facilitating seamless interaction with the Alpaca Markets REST API. It empowers developers to manage accounts, assets, market data, orders, and positions efficiently. By leveraging key modules like position, order, and history, users can access historical market data, analyze trends, and make informed trading decisions. With a focus on modularity and ease of use, this open-source project delivers essential functionalities for enhancing trading platforms and enabling strategic decision-making within the financial realm.
 
 ---
 
 ##  Features
 
 |    |   Feature         | Description |
 |----|-------------------|---------------------------------------------------------------|
-| ⚙️  | **Architecture**  | Designed with a clear separation of concerns, utilizing data classes for enhanced abstraction and maintainability. Follows a modular approach to interact with the Alpaca API efficiently. |
-| 🔩 | **Code Quality**  | Maintains high code quality standards with consistent use of Python best practices. Codebase is well-formatted, follows PEP8 guidelines, and includes automated code formatting and linting with tools like black, flake8, and isort. |
-| 📄 | **Documentation** | Provides thorough documentation with a focus on API usage, setup instructions, and data class definitions. Utilizes Sphinx for generating documentation to support developers in understanding and integrating the project. |
-| 🔌 | **Integrations**  | Relies on key external dependencies such as requests for handling HTTP requests and numpy for numerical computations. Also integrates with pre-commit for code quality checks and pytest for testing. |
-| 🧩 | **Modularity**    | Emphasizes modularity and reusability with well-defined data classes that abstract API responses. Offers developers flexibility in handling different aspects of Alpaca trading functionalities. |
-| 🧪 | **Testing**       | Utilizes pytest as the primary testing framework along with requests-mock for mocking API requests. Ensures reliable testing for validating the behavior of the PyAlpacaApi class. |
-| ⚡️  | **Performance**   | Demonstrates efficiency in API communication and data processing. Optimizes speed by handling requests and responses effectively, contributing to overall performance. |
-| 🛡️ | **Security**      | Implements secure data handling by requiring Alpaca API Key and Secret for authentication. Employs measures to protect sensitive information and control access to the Alpaca trading functionalities. |
-| 📦 | **Dependencies**  | Depends on various libraries including requests, pandas, and numpy for API interactions, data processing, and numerical computations. Managed efficiently using Poetry for dependency management. |
-| 🚀 | **Scalability**   | Shows potential for scalability with its modular design and efficient data processing. Capable of handling increased traffic and load by abstracting API interactions and ensuring maintainability. |
+| ⚙️  | **Architecture**  | The project follows a modular architecture design, allowing for separate components such as Account, Asset, Market, and Order handling. It initializes with API Key, Secret, and Paper Trading options. |
+| 🔩 | **Code Quality**  | The codebase maintains good code quality with consistent style and formatting. It integrates tools like Black for code formatting and Flake8 for linting. |
+| 📄 | **Documentation** | The project has extensive documentation covering various modules such as Account, Asset, and History. It provides detailed explanations of methods, parameters, and usage instructions. |
+| 🔌 | **Integrations**  | Key integrations include requests for HTTP requests, pandas for data manipulation, and pytest for testing. It also leverages Alpaca Markets REST API for financial data interaction. |
+| 🧩 | **Modularity**    | The codebase is highly modular, with separate modules for different functionalities like Position, Order, and Market data retrieval. This promotes code reusability and maintainability. |
+| 🧪 | **Testing**       | The project utilizes pytest for unit testing and requests-mock for mocking HTTP requests. GitHub Actions automate testing workflows for ensuring code integrity. |
+| ⚡️  | **Performance**   | The codebase efficiently handles data retrieval and processing, ensuring smooth interaction with the Alpaca API endpoints. Performance optimizations are achieved through streamlined historical data retrieval and market status updates. |
+| 🛡️ | **Security**      | Security measures include handling authentication securely through API Key and Secret. The project emphasizes data protection and access control by managing account and asset information securely. |
+| 📦 | **Dependencies**  | Key external libraries and dependencies include requests, pandas, numpy for data manipulation, and pytest for testing. Additional tools like pre-commit and poetry enhance development workflows. |
 
 ---
 
 ##  Repository Structure
 
 ```sh
 └── py-alpaca-api/
     ├── .github
-    │   └── ISSUE_TEMPLATE
+    │   ├── ISSUE_TEMPLATE
+    │   │   ├── bug_report.md
+    │   │   ├── custom.md
+    │   │   └── feature_request.md
+    │   └── workflows
+    │       └── test-package.yml
     ├── CODE_OF_CONDUCT.md
+    ├── CONTRIBUTING.md
     ├── LICENSE
     ├── README.md
     ├── SECURITY.md
+    ├── docs
+    │   ├── Makefile
+    │   ├── make.bat
+    │   ├── rtd_requirements.txt
+    │   └── source
+    │       ├── conf.py
+    │       ├── index.md
+    │       └── notebooks
     ├── poetry.lock
     ├── py_alpaca_api
     │   ├── __init__.py
     │   ├── alpaca.py
     │   └── src
+    │       ├── __init__.py
+    │       ├── account.py
+    │       ├── asset.py
+    │       ├── data_classes.py
+    │       ├── history.py
+    │       ├── market.py
+    │       ├── order.py
+    │       └── position.py
     ├── pyproject.toml
+    ├── requirements.txt
     └── tests
         ├── __init__.py
-        └── test_alpaca.py
+        ├── test_account.py
+        ├── test_alpaca.py
+        ├── test_asset.py
+        ├── test_historical_data.py
+        ├── test_market.py
+        ├── test_orders.py
+        └── test_positions.py
 ```
 
 ---
 
 ##  Modules
 
 <details closed><summary>.</summary>
 
-| File                                                                                      | Summary                                                                                                                                                                                                                                                 |
-| ---                                                                                       | ---                                                                                                                                                                                                                                                     |
-| [pyproject.toml](https://github.com/TexasCoding/py-alpaca-api/blob/master/pyproject.toml) | Defines metadata and dependencies for py-alpaca-api. Manages project details, such as name, version, description, homepage, repository, and dependencies like pandas, requests, and numpy. Organizes development and testing dependencies using Poetry. |
+| File                                                                                          | Summary                                                                                                                                                                                                                |
+| ---                                                                                           | ---                                                                                                                                                                                                                    |
+| [requirements.txt](https://github.com/TexasCoding/py-alpaca-api/blob/master/requirements.txt) | Ensures Python dependencies are managed for the repository, restricting versions to specific ranges. Facilitates compatibility and stable functioning by defining required packages for the Alpaca API project.        |
+| [pyproject.toml](https://github.com/TexasCoding/py-alpaca-api/blob/master/pyproject.toml)     | Enables interaction with Alpaca Markets REST API. Manages account, asset, market data, orders, and positions. Supports Python 3.12, pandas, requests, and numpy. Integrates testing, linting, and documentation tools. |
 
 </details>
 
 <details closed><summary>py_alpaca_api</summary>
 
-| File                                                                                          | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
-| ---                                                                                           | ---                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
-| [alpaca.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/alpaca.py) | The `alpaca.py` file in the `py-alpaca-api` repository contains a class called `PyAlpacaApi`, designed to interact with the Alpaca API. This class facilitates communication by handling API requests and responses, leveraging data classes for account, asset, and order information. The constructor requires the Alpaca API Key and Secret, with an option to specify the usage of the Alpaca Paper Trading API. This component serves as a fundamental interface for developers to access and manage Alpaca trading functionalities within the broader project architecture. |
+| File                                                                                          | Summary                                                                                                                                                                                                                                         |
+| ---                                                                                           | ---                                                                                                                                                                                                                                             |
+| [alpaca.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/alpaca.py) | Defines PyAlpacaApi class, initializing with API Key, Secret, and Paper Trading option. Sets URLs based on trading mode and initializes Account, Asset, History, Position, Order, and Market objects for interacting with Alpaca API endpoints. |
 
 </details>
 
 <details closed><summary>py_alpaca_api.src</summary>
 
-| File                                                                                                          | Summary                                                                                                                                                                            |
-| ---                                                                                                           | ---                                                                                                                                                                                |
-| [data_classes.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/data_classes.py) | Defines data classes for Orders, Assets, and Accounts to map JSON data to Python objects. Abstracts data processing from API responses, enhancing flexibility and maintainability. |
+| File                                                                                                          | Summary                                                                                                                                                                                                                                                                                                                                                                                                          |
+| ---                                                                                                           | ---                                                                                                                                                                                                                                                                                                                                                                                                              |
+| [position.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/position.py)         | Retrieves and processes account positions from Alpaca API. Includes functions to get all positions as a DataFrame, retrieve a specific position, close all positions, and close a specific position by symbol or ID.                                                                                                                                                                                             |
+| [order.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/order.py)               | SummaryThis code file, `history.py`, plays a crucial role in the `py-alpaca-api` repository by providing essential functionalities related to historical market data retrieval and analysis within the Alpaca API ecosystem. By leveraging this module, developers can efficiently access and process historical data for strategic decision-making, enhancing the overall capabilities of the trading platform. |
+| [market.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/market.py)             | Retrieves market clock status via HTTP GET request, handling successful and failed responses. Integrated with Alpaca API for real-time market data.                                                                                                                                                                                                                                                              |
+| [history.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/history.py)           | Retrieve historical stock data from Alpaca API based on specified parameters. Validates asset information, handles timeframe conversions, sends API request with required parameters, and converts response to a structured DataFrame. Ensures error handling for data availability, asset validation, and API response.                                                                                         |
+| [data_classes.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/data_classes.py) | This code file, `data_classes.py`, plays a critical role in defining the data structures and classes essential for modeling various financial assets and market data within the `py-alpaca-api` repository. By encapsulating the core data elements and relationships, this module sets the foundation for consistent and organized representation of data throughout the project.                               |
+| [asset.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/asset.py)               | Retrieves asset information from the Alpaca API based on the provided symbol. Parses the response into an AssetClass object containing essential details like ID, exchange, status, and more. Signals errors if retrieval fails.                                                                                                                                                                                 |
+| [account.py](https://github.com/TexasCoding/py-alpaca-api/blob/master/py_alpaca_api/src/account.py)           | Retrieves account information from Alpaca API, mapping it to an AccountClass object in JSON format. Handles successful and failed responses gracefully within the repositorys modular architecture.                                                                                                                                                                                                              |
+
+</details>
+
+<details closed><summary>.github.workflows</summary>
+
+| File                                                                                                            | Summary                                                                                                                                                                                                                                              |
+| ---                                                                                                             | ---                                                                                                                                                                                                                                                  |
+| [test-package.yml](https://github.com/TexasCoding/py-alpaca-api/blob/master/.github/workflows/test-package.yml) | Tests package dependencies and ensures code integrity through automated workflows. Orchestrates testing for account, asset, historical data, market, orders, and positions modules. Facilitates CI/CD integration for robust repository maintenance. |
 
 </details>
 
 ---
 
 ##  Getting Started
 
 **System Requirements:**
 
-* **Python**: `version 3.12.3`
+* **Python**: `version x.y.z`
 
 ###  Installation
 
 <h4>From <code>source</code></h4>
 
 > 1. Clone the py-alpaca-api repository:
 >
@@ -150,61 +172,53 @@
 >
 > 2. Change to the project directory:
 > ```console
 > $ cd py-alpaca-api
 > ```
 >
 > 3. Install the dependencies:
-> Recommended way is to use poetry, to install all dependencies including dev
 > ```console
 > $ poetry install
 > ```
-> Using pip, this does not include -dev dependencies:
-> ```console
-> $ pip install -r requirements.txt
-> ```
 
 ###  Usage
 
-<h4>Include PyAlpacaAPI In Your App</h4>
+<h4>From <code>source</code></h4>
 
+> Run py-alpaca-api using the command below:
 > ```python
-> from py_alpaca_api.alpaca import PyAlpacaApi
->
-> api_key = 'your_api_key'
-> api_secret = 'your_api_secret'
->
-> alpaca = PyAlpacaApi(api_key=api_key, api_secret=api_secret, api_paper=True)
->
-> asset = alpaca.get_asset('AAPL')
->
-> print(asset)
+> from py_alpaca_api import PyAlpacaApi
+> api = PyAlpacaApi(api_key='YOUR_KEY', api_secret='YOUR_SECRET', api_paper=True)
+> positions = api.position.get_all()
+> orders = api.order.get_all()
+> # Create new order
+> order = api.order.market(symbol='AAPL', qty=1.034, side='buy')
 > ```
 
 ###  Tests
 
 > Run the test suite using the command below:
 > ```console
 > $ pytest
 > ```
 
 ---
 
 ##  Project Roadmap
 
-- [X] `► Adding all functionality from Alpaca's API`
+- [X] `► Create functionality for all Alpaca API resources`
 
 ---
 
 ##  Contributing
 
 Contributions are welcome! Here are several ways you can contribute:
 
 - **[Report Issues](https://github.com/TexasCoding/py-alpaca-api/issues)**: Submit bugs found or log feature requests for the `py-alpaca-api` project.
-- **[Submit Pull Requests](https://github.com/TexasCoding/py-alpaca-api/blob/master/CONTRIBUTING.md)**: Review open PRs, and submit your own PRs.
+- **[Submit Pull Requests](https://github.com/TexasCoding/py-alpaca-api/blob/main/CONTRIBUTING.md)**: Review open PRs, and submit your own PRs.
 - **[Join the Discussions](https://github.com/TexasCoding/py-alpaca-api/discussions)**: Share your insights, provide feedback, or ask questions.
 
 <details closed>
 <summary>Contributing Guidelines</summary>
 
 1. **Fork the Repository**: Start by forking the project repository to your github account.
 2. **Clone Locally**: Clone the forked repository to your local machine using a git client.
@@ -238,19 +252,18 @@
 </p>
 </details>
 
 ---
 
 ##  License
 
-This project is protected under the [MIT](https://choosealicense.com/licenses/mit/) License. For more details, refer to the [LICENSE](https://github.com/TexasCoding/py-alpaca-api/blob/master/LICENSE) file.
+This project is protected under the [SELECT-A-LICENSE](https://choosealicense.com/licenses) License. For more details, refer to the [LICENSE](https://choosealicense.com/licenses/) file.
 
 ---
 
 ##  Acknowledgments
 
-
+- List any resources, contributors, inspiration, etc. here.
 
 [**Return**](#-overview)
 
 ---
-
```

