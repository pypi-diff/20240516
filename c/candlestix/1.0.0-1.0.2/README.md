# Comparing `tmp/candlestix-1.0.0-py3-none-any.whl.zip` & `tmp/candlestix-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8502 bytes, number of entries: 10
--rw-r--r--  2.0 unx     3755 b- defN 24-Mar-27 05:52 candlestix/__init__.py
+Zip file size: 8619 bytes, number of entries: 10
+-rw-r--r--  2.0 unx     4007 b- defN 24-May-16 08:21 candlestix/__init__.py
 -rw-r--r--  2.0 unx     6539 b- defN 24-May-11 09:28 candlestix/candle_loader.py
--rw-r--r--  2.0 unx     2244 b- defN 24-Mar-26 19:16 candlestix/candleconf.py
+-rw-r--r--  2.0 unx     2300 b- defN 24-May-16 08:06 candlestix/candleconf.py
 -rw-r--r--  2.0 unx      610 b- defN 24-Mar-27 03:47 candlestix/instrument.py
 -rw-r--r--  2.0 unx     2623 b- defN 24-Apr-28 07:19 candlestix/time.py
--rw-r--r--  2.0 unx     6461 b- defN 24-Mar-27 05:45 candlestix/upstox.py
--rw-r--r--  2.0 unx      118 b- defN 24-May-11 09:28 candlestix-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-11 09:28 candlestix-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 24-May-11 09:28 candlestix-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      785 b- defN 24-May-11 09:28 candlestix-1.0.0.dist-info/RECORD
-10 files, 23238 bytes uncompressed, 7170 bytes compressed:  69.1%
+-rw-r--r--  2.0 unx     6529 b- defN 24-May-16 08:19 candlestix/upstox.py
+-rw-r--r--  2.0 unx      118 b- defN 24-May-16 08:26 candlestix-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-16 08:26 candlestix-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-May-16 08:26 candlestix-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      785 b- defN 24-May-16 08:26 candlestix-1.0.2.dist-info/RECORD
+10 files, 23614 bytes uncompressed, 7287 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: candlestix/time.py
 Comment: 
 
 Filename: candlestix/upstox.py
 Comment: 
 
-Filename: candlestix-1.0.0.dist-info/METADATA
+Filename: candlestix-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: candlestix-1.0.0.dist-info/WHEEL
+Filename: candlestix-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: candlestix-1.0.0.dist-info/top_level.txt
+Filename: candlestix-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: candlestix-1.0.0.dist-info/RECORD
+Filename: candlestix-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## candlestix/__init__.py

```diff
@@ -75,24 +75,26 @@
             name = row[3]
             instrument_type = row[9]
             exchange_str = row[11]
 
             if ('%' in name or  # name contains '%'
                     bool(re.search(pattern_decimal_number, name)) or  # name contains a decimal number - 7.50
                     instrument_key in dup_check or  # duplicate check for instrument id
-                    instrument_type.lower() != 'equity'):  # type is not equity
+                    (instrument_type.lower() != 'equity' and instrument_type.lower() != 'index')):  # type is not equity
                 continue
 
             dup_check.add(instrument_key)
 
             exchange = Instrument.get_exchange_from_val(exchange_str)
+            if instrument_type.lower() == 'index':
+                symbol = name.upper().replace(' ', '_')  # Convert 'NIFTY 50' to 'NIFTY_50'
             inst = Instrument(symbol=symbol, instrument_key=instrument_key, name=name, exchange=exchange)
-            if exchange == Exchange.NSE:
+            if exchange == Exchange.NSE or exchange == Exchange.NSE_INDEX:
                 nse_lookup[symbol] = inst
-            elif exchange == Exchange.BSE:
+            elif exchange == Exchange.BSE or exchange == Exchange.BSE_INDEX:
                 bse_lookup[symbol] = inst
 
     # print(f'nse>> size={round(sys.getsizeof(nse_lookup)/1024,2)} kb, len={len(nse_lookup.keys())}')
     # print(f'bse>> size={round(sys.getsizeof(bse_lookup)/1024,2)} kb, len={len(bse_lookup.keys())}')
     logger.info("Data load COMPLETE for instruments.")
```

## candlestix/candleconf.py

```diff
@@ -50,14 +50,16 @@
     def from_name_str(s):
         return CandleLength.__members__.get(s)
 
 
 class Exchange(Enum):
     BSE = "BSE_EQ"
     NSE = 'NSE_EQ'
+    NSE_INDEX = 'NSE_INDEX'
+    BSE_INDEX = 'BSE_INDEX'
 
 
 class Constants:
     API_VERSION = '2.0'
     API_STATUS_ERROR = "error"
     API_STATUS_SUCCESS = "success"
```

## candlestix/upstox.py

```diff
@@ -130,13 +130,13 @@
 
         indices_to_delete.sort(reverse=True)
         print(indices_to_delete)
         for i in indices_to_delete:
             raw_ohlcv_candle_date.pop(i)
 
     def _fetch_instrument(self, symbol: str, exchange: Exchange) -> Instrument:
-        if exchange == Exchange.NSE:
+        if exchange == Exchange.NSE or exchange == Exchange.NSE_INDEX:
             return candlestix.nse_lookup.get(symbol)
-        elif exchange == Exchange.BSE:
+        elif exchange == Exchange.BSE or exchange == Exchange.BSE_INDEX:
             return candlestix.bse_lookup.get(symbol)
         else:
             return None
```

