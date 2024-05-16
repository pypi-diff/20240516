# Comparing `tmp/nostr_bots-0.0.2.tar.gz` & `tmp/nostr_bots-0.0.3.tar.gz`

## Comparing `nostr_bots-0.0.2.tar` & `nostr_bots-0.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 nostr_bots-0.0.2/.gitattributes
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 nostr_bots-0.0.2/.gitmodules
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 nostr_bots-0.0.2/run_bitcoin_bot.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 nostr_bots-0.0.2/run_echo_bot.py
--rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 nostr_bots-0.0.2/run_ip_bot.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 nostr_bots-0.0.2/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 nostr_bots-0.0.2/.idea/.gitignore
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 nostr_bots-0.0.2/.idea/misc.xml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 nostr_bots-0.0.2/.idea/modules.xml
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 nostr_bots-0.0.2/.idea/nostr_bots.iml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nostr_bots-0.0.2/.idea/vcs.xml
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 nostr_bots-0.0.2/.idea/workspace.xml
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 nostr_bots-0.0.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 nostr_bots-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nostr_bots-0.0.2/src/__init__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 nostr_bots-0.0.2/src/bots/__about__.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 nostr_bots-0.0.2/src/bots/__init__.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 nostr_bots-0.0.2/src/bots/acceptors.py
--rw-r--r--   0        0        0     7733 2020-02-02 00:00:00.000000 nostr_bots-0.0.2/src/bots/basic.py
--rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 nostr_bots-0.0.2/src/bots/bitcoind.py
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 nostr_bots-0.0.2/src/bots/util.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 nostr_bots-0.0.2/web/html/address.html
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 nostr_bots-0.0.2/web/html/list_transactions.html
--rw-r--r--   0        0        0     8876 2020-02-02 00:00:00.000000 nostr_bots-0.0.2/web/script/bot.js
--rw-r--r--   0        0        0   839290 2020-02-02 00:00:00.000000 nostr_bots-0.0.2/web/script/nostr.js
--rw-r--r--   0        0        0    33168 2020-02-02 00:00:00.000000 nostr_bots-0.0.2/web/script/qrcode.js
--rw-r--r--   0        0        0    19927 2020-02-02 00:00:00.000000 nostr_bots-0.0.2/web/script/qrcode.min.js
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 nostr_bots-0.0.2/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 nostr_bots-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 nostr_bots-0.0.2/README.md
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 nostr_bots-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 nostr_bots-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 nostr_bots-0.0.3/.gitattributes
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 nostr_bots-0.0.3/.gitmodules
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 nostr_bots-0.0.3/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 nostr_bots-0.0.3/.idea/.gitignore
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 nostr_bots-0.0.3/.idea/misc.xml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 nostr_bots-0.0.3/.idea/modules.xml
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 nostr_bots-0.0.3/.idea/nostr_bots.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nostr_bots-0.0.3/.idea/vcs.xml
+-rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 nostr_bots-0.0.3/.idea/workspace.xml
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 nostr_bots-0.0.3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 nostr_bots-0.0.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nostr_bots-0.0.3/src/__init__.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 nostr_bots-0.0.3/src/nostr_bots/__about__.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 nostr_bots-0.0.3/src/nostr_bots/__init__.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 nostr_bots-0.0.3/src/nostr_bots/acceptors.py
+-rw-r--r--   0        0        0     7733 2020-02-02 00:00:00.000000 nostr_bots-0.0.3/src/nostr_bots/basic.py
+-rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 nostr_bots-0.0.3/src/nostr_bots/bitcoind.py
+-rw-r--r--   0        0        0     4708 2020-02-02 00:00:00.000000 nostr_bots-0.0.3/src/nostr_bots/run_bitcoin_bot.py
+-rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 nostr_bots-0.0.3/src/nostr_bots/run_echo_bot.py
+-rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 nostr_bots-0.0.3/src/nostr_bots/run_ip_bot.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 nostr_bots-0.0.3/src/nostr_bots/util.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 nostr_bots-0.0.3/web/html/address.html
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 nostr_bots-0.0.3/web/html/list_transactions.html
+-rw-r--r--   0        0        0     8876 2020-02-02 00:00:00.000000 nostr_bots-0.0.3/web/script/bot.js
+-rw-r--r--   0        0        0   839290 2020-02-02 00:00:00.000000 nostr_bots-0.0.3/web/script/nostr.js
+-rw-r--r--   0        0        0    33168 2020-02-02 00:00:00.000000 nostr_bots-0.0.3/web/script/qrcode.js
+-rw-r--r--   0        0        0    19927 2020-02-02 00:00:00.000000 nostr_bots-0.0.3/web/script/qrcode.min.js
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 nostr_bots-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 nostr_bots-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 nostr_bots-0.0.3/README.md
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 nostr_bots-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 nostr_bots-0.0.3/PKG-INFO
```

### Comparing `nostr_bots-0.0.2/run_bitcoin_bot.py` & `nostr_bots-0.0.3/src/nostr_bots/run_bitcoin_bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import sys
 from pathlib import Path
 from monstr.exception import ConfigurationError
 from monstr.client.client import Client, ClientPool
 from monstr.util import util_funcs
 from monstr.encrypt import Keys
 from monstr.signing import BasicKeySigner
-from bots.bitcoind import BitcoindBot, BitcoindRPC
-from src.bots.util import load_toml
-from bots.acceptors import AuthListAccept
+from nostr_bots.bitcoind import BitcoindBot, BitcoindRPC
+from src.nostr_bots.util import load_toml
+from nostr_bots.acceptors import AuthListAccept
 
 
 # working directory
 WORK_DIR = f'{Path.home()}/.nostrpy/'
 # config file
 CONFIG_FILE = f'bitcoin_bot.toml'
 # default relay
```

### Comparing `nostr_bots-0.0.2/run_echo_bot.py` & `nostr_bots-0.0.3/src/nostr_bots/run_echo_bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import sys
 from monstr.exception import ConfigurationError
 from monstr.client.client import Client, ClientPool
 from monstr.event.event import Event
 from monstr.util import util_funcs
 from monstr.encrypt import Keys
 from monstr.inbox import Inbox
-from bots.basic import BotEventHandler
+from nostr_bots.basic import BotEventHandler
 from monstr.signing import BasicKeySigner
 
 
 # default relay
 DEFAULT_RELAY = 'ws://localhost:8081'
 # default key - if None it'll be generated each run
 USE_KEY = 'nsec1fnyygyh57chwf7zhw3mwmrltc2hatfwn0hldtl4z5axv4netkjlsy0u220'
```

### Comparing `nostr_bots-0.0.2/run_ip_bot.py` & `nostr_bots-0.0.3/src/nostr_bots/run_ip_bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import sys
 from monstr.exception import ConfigurationError
 from monstr.client.client import Client, ClientPool
 from monstr.event.event import Event
 from monstr.util import util_funcs
 from monstr.encrypt import Keys
 from monstr.signing import BasicKeySigner
-from bots.basic import BotEventHandler
+from nostr_bots.basic import BotEventHandler
 
 
 # default relay
 DEFAULT_RELAY = 'ws://localhost:8081'
 # default key - if None it'll be generated each run
 USE_KEY = 'nsec1fnyygyh57chwf7zhw3mwmrltc2hatfwn0hldtl4z5axv4netkjlsy0u220'
 
@@ -76,15 +76,15 @@
 
     # actually create the bot
     bot = IPBot(signer=BasicKeySigner(keys),
                 clients=clients,
                 encrypt_kinds=[])
 
     # start the clients
-    print(f'monitoring for events from or to account {keys.public_key_hex()} on relays {relays}')
+    print(f'monitoring for events from or to account {keys.public_key_bech32()} on relays {relays}')
 
     def sigint_handler(signal, frame):
         clients.end()
         sys.exit(0)
 
     signal.signal(signal.SIGINT, sigint_handler)
```

### Comparing `nostr_bots-0.0.2/.github/workflows/python-package.yml` & `nostr_bots-0.0.3/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `nostr_bots-0.0.2/.idea/inspectionProfiles/Project_Default.xml` & `nostr_bots-0.0.3/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `nostr_bots-0.0.2/src/bots/acceptors.py` & `nostr_bots-0.0.3/src/nostr_bots/acceptors.py`

 * *Files identical despite different names*

### Comparing `nostr_bots-0.0.2/src/bots/basic.py` & `nostr_bots-0.0.3/src/nostr_bots/basic.py`

 * *Files identical despite different names*

### Comparing `nostr_bots-0.0.2/src/bots/bitcoind.py` & `nostr_bots-0.0.3/src/nostr_bots/bitcoind.py`

 * *Files identical despite different names*

### Comparing `nostr_bots-0.0.2/src/bots/util.py` & `nostr_bots-0.0.3/src/nostr_bots/util.py`

 * *Files identical despite different names*

### Comparing `nostr_bots-0.0.2/web/html/address.html` & `nostr_bots-0.0.3/web/html/address.html`

 * *Files identical despite different names*

### Comparing `nostr_bots-0.0.2/web/html/list_transactions.html` & `nostr_bots-0.0.3/web/html/list_transactions.html`

 * *Files identical despite different names*

### Comparing `nostr_bots-0.0.2/web/script/bot.js` & `nostr_bots-0.0.3/web/script/bot.js`

 * *Files identical despite different names*

### Comparing `nostr_bots-0.0.2/web/script/nostr.js` & `nostr_bots-0.0.3/web/script/nostr.js`

 * *Files identical despite different names*

### Comparing `nostr_bots-0.0.2/web/script/qrcode.js` & `nostr_bots-0.0.3/web/script/qrcode.js`

 * *Files identical despite different names*

### Comparing `nostr_bots-0.0.2/web/script/qrcode.min.js` & `nostr_bots-0.0.3/web/script/qrcode.min.js`

 * *Files identical despite different names*

### Comparing `nostr_bots-0.0.2/LICENSE.txt` & `nostr_bots-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nostr_bots-0.0.2/README.md` & `nostr_bots-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nostr_bots-0.0.2/pyproject.toml` & `nostr_bots-0.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -22,20 +22,20 @@
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
     "monstr>=0.1.2"
 ]
 
 [project.urls]
-Documentation = "https://github.com/monty/bots#readme"
-Issues = "https://github.com/monty/bots/issues"
-Source = "https://github.com/monty/bots"
+Documentation = "https://github.com/monty/nostr_bots#readme"
+Issues = "https://github.com/monty/nostr_bots/issues"
+Source = "https://github.com/monty/nostr_bots"
 
 [tool.hatch.version]
-path = "src/bots/__about__.py"
+path = "src/nostr_bots/__about__.py"
 
 [tool.hatch.envs.types]
 extra-dependencies = [
   "mypy>=1.0.0",
 ]
 [tool.hatch.envs.types.scripts]
 check = "mypy --install-types --non-interactive {args:src/bots tests}"
```

### Comparing `nostr_bots-0.0.2/PKG-INFO` & `nostr_bots-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.3
 Name: nostr_bots
-Version: 0.0.2
+Version: 0.0.3
 Summary: simple bots for nostr using monstr
-Project-URL: Documentation, https://github.com/monty/bots#readme
-Project-URL: Issues, https://github.com/monty/bots/issues
-Project-URL: Source, https://github.com/monty/bots
+Project-URL: Documentation, https://github.com/monty/nostr_bots#readme
+Project-URL: Issues, https://github.com/monty/nostr_bots/issues
+Project-URL: Source, https://github.com/monty/nostr_bots
 Author-email: monty <monty@monty888.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

