# Comparing `tmp/tg_signer-0.1.1.tar.gz` & `tmp/tg_signer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg_signer-0.1.1.tar", last modified: Thu May 16 07:07:21 2024, max compression
+gzip compressed data, was "tg_signer-0.1.2.tar", last modified: Thu May 16 07:50:07 2024, max compression
```

## Comparing `tg_signer-0.1.1.tar` & `tg_signer-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2024-05-16 07:07:21.987928 tg_signer-0.1.1/
--rw-r--r--   0 luming     (501) staff       (20)     1493 2024-01-07 10:02:22.000000 tg_signer-0.1.1/LICENSE
--rw-r--r--   0 luming     (501) staff       (20)     1148 2024-05-16 07:07:21.987868 tg_signer-0.1.1/PKG-INFO
--rw-r--r--   0 luming     (501) staff       (20)      595 2024-05-16 07:03:40.000000 tg_signer-0.1.1/README.md
--rw-r--r--   0 luming     (501) staff       (20)      979 2024-05-16 07:07:21.988188 tg_signer-0.1.1/setup.cfg
--rw-r--r--   0 luming     (501) staff       (20)       38 2024-01-07 10:02:22.000000 tg_signer-0.1.1/setup.py
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2024-05-16 07:07:21.986702 tg_signer-0.1.1/tg_signer/
--rw-r--r--   0 luming     (501) staff       (20)       22 2024-05-16 07:07:11.000000 tg_signer-0.1.1/tg_signer/__init__.py
--rw-r--r--   0 luming     (501) staff       (20)       66 2024-05-16 07:03:40.000000 tg_signer-0.1.1/tg_signer/__main__.py
--rw-r--r--   0 luming     (501) staff       (20)     8426 2024-05-16 07:03:40.000000 tg_signer-0.1.1/tg_signer/signer.py
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2024-05-16 07:07:21.987643 tg_signer-0.1.1/tg_signer.egg-info/
--rw-r--r--   0 luming     (501) staff       (20)     1148 2024-05-16 07:07:21.000000 tg_signer-0.1.1/tg_signer.egg-info/PKG-INFO
--rw-r--r--   0 luming     (501) staff       (20)      300 2024-05-16 07:07:21.000000 tg_signer-0.1.1/tg_signer.egg-info/SOURCES.txt
--rw-r--r--   0 luming     (501) staff       (20)        1 2024-05-16 07:07:21.000000 tg_signer-0.1.1/tg_signer.egg-info/dependency_links.txt
--rw-r--r--   0 luming     (501) staff       (20)       53 2024-05-16 07:07:21.000000 tg_signer-0.1.1/tg_signer.egg-info/entry_points.txt
--rw-r--r--   0 luming     (501) staff       (20)       18 2024-05-16 07:07:21.000000 tg_signer-0.1.1/tg_signer.egg-info/requires.txt
--rw-r--r--   0 luming     (501) staff       (20)       10 2024-05-16 07:07:21.000000 tg_signer-0.1.1/tg_signer.egg-info/top_level.txt
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2024-05-16 07:50:07.963207 tg_signer-0.1.2/
+-rw-r--r--   0 luming     (501) staff       (20)     1493 2024-01-07 10:02:22.000000 tg_signer-0.1.2/LICENSE
+-rw-r--r--   0 luming     (501) staff       (20)     1160 2024-05-16 07:50:07.963153 tg_signer-0.1.2/PKG-INFO
+-rw-r--r--   0 luming     (501) staff       (20)      607 2024-05-16 07:49:00.000000 tg_signer-0.1.2/README.md
+-rw-r--r--   0 luming     (501) staff       (20)      979 2024-05-16 07:50:07.965231 tg_signer-0.1.2/setup.cfg
+-rw-r--r--   0 luming     (501) staff       (20)       38 2024-01-07 10:02:22.000000 tg_signer-0.1.2/setup.py
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2024-05-16 07:50:07.961618 tg_signer-0.1.2/tg_signer/
+-rw-r--r--   0 luming     (501) staff       (20)       22 2024-05-16 07:49:56.000000 tg_signer-0.1.2/tg_signer/__init__.py
+-rw-r--r--   0 luming     (501) staff       (20)       66 2024-05-16 07:03:40.000000 tg_signer-0.1.2/tg_signer/__main__.py
+-rw-r--r--   0 luming     (501) staff       (20)     8557 2024-05-16 07:49:00.000000 tg_signer-0.1.2/tg_signer/signer.py
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2024-05-16 07:50:07.962982 tg_signer-0.1.2/tg_signer.egg-info/
+-rw-r--r--   0 luming     (501) staff       (20)     1160 2024-05-16 07:50:07.000000 tg_signer-0.1.2/tg_signer.egg-info/PKG-INFO
+-rw-r--r--   0 luming     (501) staff       (20)      300 2024-05-16 07:50:07.000000 tg_signer-0.1.2/tg_signer.egg-info/SOURCES.txt
+-rw-r--r--   0 luming     (501) staff       (20)        1 2024-05-16 07:50:07.000000 tg_signer-0.1.2/tg_signer.egg-info/dependency_links.txt
+-rw-r--r--   0 luming     (501) staff       (20)       53 2024-05-16 07:50:07.000000 tg_signer-0.1.2/tg_signer.egg-info/entry_points.txt
+-rw-r--r--   0 luming     (501) staff       (20)       18 2024-05-16 07:50:07.000000 tg_signer-0.1.2/tg_signer.egg-info/requires.txt
+-rw-r--r--   0 luming     (501) staff       (20)       10 2024-05-16 07:50:07.000000 tg_signer-0.1.2/tg_signer.egg-info/top_level.txt
```

### Comparing `tg_signer-0.1.1/LICENSE` & `tg_signer-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tg_signer-0.1.1/PKG-INFO` & `tg_signer-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-signer
-Version: 0.1.1
+Version: 0.1.2
 Summary: Telegram signer
 Home-page: https://github.com/amchii/tg-signer
 Author: Amchii
 Author-email: finethankuandyou@gmail.com
 License: BSD 3-Clause License
 Project-URL: Source, https://github.com/amchii/tg-signer
 Classifier: Intended Audience :: Developers
@@ -15,27 +15,31 @@
 License-File: LICENSE
 Requires-Dist: pyrogram
 Requires-Dist: tgcrypto
 
 # Telegram Signer - Telegram每日自动签到
 
 ## Install
-`pip install -U tg-signer`
+```
+pip install -U tg-signer
+```
 
 ## Usage
 ```
 Usage: tg-signer <command>
 Available commands: list, login, run, reconfig
 e.g. tg-signer run
 ```
 #### Configure proxy(if necessary)
 use `TG_PROXY`
 
 e.g.:
-`export TG_PROXY=socks5://127.0.0.1:7890`
+```
+export TG_PROXY=socks5://127.0.0.1:7890
+```
 
 #### Run
 `tg-signer run`
 
 run `tree .signer` you will see:
 ```
 .signer
```

### Comparing `tg_signer-0.1.1/README.md` & `tg_signer-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 # Telegram Signer - Telegram每日自动签到
 
 ## Install
-`pip install -U tg-signer`
+```
+pip install -U tg-signer
+```
 
 ## Usage
 ```
 Usage: tg-signer <command>
 Available commands: list, login, run, reconfig
 e.g. tg-signer run
 ```
 #### Configure proxy(if necessary)
 use `TG_PROXY`
 
 e.g.:
-`export TG_PROXY=socks5://127.0.0.1:7890`
+```
+export TG_PROXY=socks5://127.0.0.1:7890
+```
 
 #### Run
 `tg-signer run`
 
 run `tree .signer` you will see:
 ```
 .signer
```

### Comparing `tg_signer-0.1.1/setup.cfg` & `tg_signer-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `tg_signer-0.1.1/tg_signer/signer.py` & `tg_signer-0.1.2/tg_signer/signer.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,38 +27,43 @@
     "tg-signer.log",
     maxBytes=1024 * 1024 * 3,
     backupCount=10,
     encoding="utf-8",
 )
 file_handler.setFormatter(formatter)
 logger.addHandler(file_handler)
-desktop_api_id = 611335
-desktop_api_hash = "d524b414d21f4d37f08684c1df41ac9c"
-root_dir = pathlib.Path(__file__).parent.absolute()
+root_dir = pathlib.Path(".").absolute()
 local_dir = root_dir / ".signer"
 
 
+def get_api_config():
+    api_id = int(os.environ.get("TG_API_ID", 611335))
+    api_hash = os.environ.get("TG_API_HASH", "d524b414d21f4d37f08684c1df41ac9c")
+    return api_id, api_hash
+
+
 def get_proxy():
     if tg_proxy := os.environ.get("TG_PROXY"):
         r = parse.urlparse(tg_proxy)
         return {
             "scheme": r.scheme,
             "hostname": r.hostname,
             "port": r.port,
             "username": r.username,
             "password": r.password,
         }
 
 
 def get_client(name: str = "my_account", proxy=None):
     proxy = proxy or get_proxy()
+    api_id, api_hash = get_api_config()
     return Client(
         name,
-        desktop_api_id,
-        desktop_api_hash,
+        api_id,
+        api_hash,
         proxy=proxy,
     )
 
 
 app = get_client()
 
 
@@ -73,15 +78,15 @@
 
 
 @dataclasses.dataclass
 class SignConfig:
     chat_id: int
     sign_text: str
     sign_at: time
-    random_seconds: float | int
+    random_seconds: int
 
     def to_jsonable(self):
         return {
             "chat_id": self.chat_id,
             "sign_text": self.sign_text,
             "sign_at": self.sign_at.isoformat(),
             "random_seconds": self.random_seconds,
@@ -133,16 +138,16 @@
         if file.is_file():
             with open(file, "r") as f:
                 data = json.load(f)
             data.pop("_")
             user = User(
                 id=data["id"],
                 is_self=True,
-                first_name=data["first_name"],
-                last_name=data["last_name"],
+                first_name=data.get("first_name"),
+                last_name=data.get("last_name"),
             )
             return user
 
     def set_me(self, user: User):
         self.user = user
         with open(self.base_dir.joinpath("me.json"), "w") as fp:
             fp.write(str(user))
@@ -150,15 +155,15 @@
     def ask_for_config(self) -> "SignConfig":
         chat_id = int(input("Chat ID: "))
         sign_text = input("签到文本: ")
         sign_at_str = input("每日签到时间（如 06:00:00）: ")
         sign_at_str = sign_at_str.replace("：", ":").strip()
         sign_at = time.fromisoformat(sign_at_str)
         random_seconds_str = input("签到时间误差随机秒数（默认为0）: ") or "0"
-        random_seconds = float(random_seconds_str)
+        random_seconds = int(float(random_seconds_str))
         return SignConfig(chat_id, sign_text, sign_at, random_seconds)
 
     def reconfig(self):
         config = self.ask_for_config()
         with open(self.config_file, "w") as fp:
             json.dump(config.to_jsonable(), fp)
         return config
@@ -242,15 +247,15 @@
                             json.dump(sign_record, fp)
 
                     next_run = (now + timedelta(days=1)).replace(
                         hour=sign_at.hour,
                         minute=sign_at.minute,
                         second=sign_at.second,
                         microsecond=sign_at.microsecond,
-                    ) + timedelta(seconds=random.randint(0, config.random_seconds))
+                    ) + timedelta(seconds=random.randint(0, int(config.random_seconds)))
                     logger.info(f"下次运行时间: {next_run}")
                     await asyncio.sleep((next_run - now).total_seconds())
             except (OSError, errors.Unauthorized) as e:
                 logger.exception(e)
                 await asyncio.sleep(30)
```

### Comparing `tg_signer-0.1.1/tg_signer.egg-info/PKG-INFO` & `tg_signer-0.1.2/tg_signer.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-signer
-Version: 0.1.1
+Version: 0.1.2
 Summary: Telegram signer
 Home-page: https://github.com/amchii/tg-signer
 Author: Amchii
 Author-email: finethankuandyou@gmail.com
 License: BSD 3-Clause License
 Project-URL: Source, https://github.com/amchii/tg-signer
 Classifier: Intended Audience :: Developers
@@ -15,27 +15,31 @@
 License-File: LICENSE
 Requires-Dist: pyrogram
 Requires-Dist: tgcrypto
 
 # Telegram Signer - Telegram每日自动签到
 
 ## Install
-`pip install -U tg-signer`
+```
+pip install -U tg-signer
+```
 
 ## Usage
 ```
 Usage: tg-signer <command>
 Available commands: list, login, run, reconfig
 e.g. tg-signer run
 ```
 #### Configure proxy(if necessary)
 use `TG_PROXY`
 
 e.g.:
-`export TG_PROXY=socks5://127.0.0.1:7890`
+```
+export TG_PROXY=socks5://127.0.0.1:7890
+```
 
 #### Run
 `tg-signer run`
 
 run `tree .signer` you will see:
 ```
 .signer
```

