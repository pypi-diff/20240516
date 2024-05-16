# Comparing `tmp/hass_nabucasa-0.81.0.tar.gz` & `tmp/hass-nabucasa-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hass_nabucasa-0.81.0.tar", last modified: Thu May 16 13:59:11 2024, max compression
+gzip compressed data, was "dist/hass-nabucasa-0.9.tar", last modified: Thu Mar 21 15:12:51 2019, max compression
```

## Comparing `hass_nabucasa-0.81.0.tar` & `hass-nabucasa-0.9.tar`

### file list

```diff
@@ -1,43 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:59:11.619581 hass_nabucasa-0.81.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-16 13:59:04.000000 hass_nabucasa-0.81.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-16 13:59:11.619581 hass_nabucasa-0.81.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-16 13:59:04.000000 hass_nabucasa-0.81.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:59:11.611581 hass_nabucasa-0.81.0/hass_nabucasa/
--rw-r--r--   0 runner    (1001) docker     (127)    11971 2024-05-16 13:59:04.000000 hass_nabucasa-0.81.0/hass_nabucasa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-05-16 13:59:04.000000 hass_nabucasa-0.81.0/hass_nabucasa/account_link.py
--rw-r--r--   0 runner    (1001) docker     (127)    20510 2024-05-16 13:59:04.000000 hass_nabucasa-0.81.0/hass_nabucasa/acme.py
--rw-r--r--   0 runner    (1001) docker     (127)     8509 2024-05-16 13:59:04.000000 hass_nabucasa-0.81.0/hass_nabucasa/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-16 13:59:04.000000 hass_nabucasa-0.81.0/hass_nabucasa/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9507 2024-05-16 13:59:04.000000 hass_nabucasa-0.81.0/hass_nabucasa/cloud_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-16 13:59:04.000000 hass_nabucasa-0.81.0/hass_nabucasa/cloudhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-16 13:59:04.000000 hass_nabucasa-0.81.0/hass_nabucasa/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-05-16 13:59:04.000000 hass_nabucasa-0.81.0/hass_nabucasa/google_report_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-05-16 13:59:04.000000 hass_nabucasa-0.81.0/hass_nabucasa/iot.py
--rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-05-16 13:59:04.000000 hass_nabucasa-0.81.0/hass_nabucasa/iot_base.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:59:04.000000 hass_nabucasa-0.81.0/hass_nabucasa/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    22419 2024-05-16 13:59:04.000000 hass_nabucasa-0.81.0/hass_nabucasa/remote.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-16 13:59:04.000000 hass_nabucasa-0.81.0/hass_nabucasa/thingtalk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-05-16 13:59:04.000000 hass_nabucasa-0.81.0/hass_nabucasa/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    34339 2024-05-16 13:59:04.000000 hass_nabucasa-0.81.0/hass_nabucasa/voice.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:59:11.615581 hass_nabucasa-0.81.0/hass_nabucasa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-16 13:59:11.000000 hass_nabucasa-0.81.0/hass_nabucasa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-16 13:59:11.000000 hass_nabucasa-0.81.0/hass_nabucasa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 13:59:11.000000 hass_nabucasa-0.81.0/hass_nabucasa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 13:59:11.000000 hass_nabucasa-0.81.0/hass_nabucasa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-16 13:59:11.000000 hass_nabucasa-0.81.0/hass_nabucasa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-16 13:59:11.000000 hass_nabucasa-0.81.0/hass_nabucasa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-05-16 13:59:04.000000 hass_nabucasa-0.81.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 13:59:11.619581 hass_nabucasa-0.81.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:59:11.615581 hass_nabucasa-0.81.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-05-16 13:59:04.000000 hass_nabucasa-0.81.0/tests/test_account_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     7495 2024-05-16 13:59:04.000000 hass_nabucasa-0.81.0/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    12476 2024-05-16 13:59:04.000000 hass_nabucasa-0.81.0/tests/test_cloud_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-16 13:59:04.000000 hass_nabucasa-0.81.0/tests/test_cloudhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-05-16 13:59:04.000000 hass_nabucasa-0.81.0/tests/test_google_report_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    10078 2024-05-16 13:59:04.000000 hass_nabucasa-0.81.0/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)    10326 2024-05-16 13:59:04.000000 hass_nabucasa-0.81.0/tests/test_iot.py
--rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-05-16 13:59:04.000000 hass_nabucasa-0.81.0/tests/test_iot_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    30641 2024-05-16 13:59:04.000000 hass_nabucasa-0.81.0/tests/test_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-16 13:59:04.000000 hass_nabucasa-0.81.0/tests/test_thingtalk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-16 13:59:04.000000 hass_nabucasa-0.81.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-16 13:59:04.000000 hass_nabucasa-0.81.0/tests/test_voice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-03-21 15:12:51.000000 hass-nabucasa-0.9/
+-rw-r--r--   0 root         (0) root         (0)      909 2019-03-21 15:12:51.000000 hass-nabucasa-0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       39 2019-03-01 22:18:23.000000 hass-nabucasa-0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-03-21 15:12:51.000000 hass-nabucasa-0.9/hass_nabucasa/
+-rw-r--r--   0 root         (0) root         (0)     6232 2019-03-11 09:43:41.000000 hass-nabucasa-0.9/hass_nabucasa/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13557 2019-03-15 12:30:59.000000 hass-nabucasa-0.9/hass_nabucasa/acme.py
+-rw-r--r--   0 root         (0) root         (0)     6468 2019-03-11 09:43:41.000000 hass-nabucasa-0.9/hass_nabucasa/auth.py
+-rw-r--r--   0 root         (0) root         (0)     2199 2019-03-15 12:30:59.000000 hass-nabucasa-0.9/hass_nabucasa/client.py
+-rw-r--r--   0 root         (0) root         (0)     2260 2019-03-11 09:43:41.000000 hass-nabucasa-0.9/hass_nabucasa/cloud_api.py
+-rw-r--r--   0 root         (0) root         (0)     2283 2019-03-12 11:06:17.000000 hass-nabucasa-0.9/hass_nabucasa/cloudhooks.py
+-rw-r--r--   0 root         (0) root         (0)     1869 2019-03-15 13:15:14.000000 hass-nabucasa-0.9/hass_nabucasa/const.py
+-rw-r--r--   0 root         (0) root         (0)    10736 2019-03-15 12:30:59.000000 hass-nabucasa-0.9/hass_nabucasa/iot.py
+-rw-r--r--   0 root         (0) root         (0)    10439 2019-03-21 15:12:30.000000 hass-nabucasa-0.9/hass_nabucasa/remote.py
+-rw-r--r--   0 root         (0) root         (0)     2468 2019-03-15 12:30:59.000000 hass-nabucasa-0.9/hass_nabucasa/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-03-21 15:12:51.000000 hass-nabucasa-0.9/hass_nabucasa.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      909 2019-03-21 15:12:51.000000 hass-nabucasa-0.9/hass_nabucasa.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      488 2019-03-21 15:12:51.000000 hass-nabucasa-0.9/hass_nabucasa.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2019-03-21 15:12:51.000000 hass-nabucasa-0.9/hass_nabucasa.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2019-03-21 15:12:51.000000 hass-nabucasa-0.9/hass_nabucasa.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       78 2019-03-21 15:12:51.000000 hass-nabucasa-0.9/hass_nabucasa.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2019-03-21 15:12:51.000000 hass-nabucasa-0.9/hass_nabucasa.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      432 2019-03-21 15:12:51.000000 hass-nabucasa-0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1273 2019-03-21 15:12:30.000000 hass-nabucasa-0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `hass_nabucasa-0.81.0/hass_nabucasa/acme.py` & `hass-nabucasa-0.9/hass_nabucasa/acme.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,100 +1,78 @@
 """Handle ACME and local certificates."""
-
-from __future__ import annotations
-
 import asyncio
-import contextlib
-from datetime import datetime, timedelta
+from datetime import datetime
 import logging
 from pathlib import Path
-from typing import TYPE_CHECKING
+from typing import Optional
 import urllib
 
+import OpenSSL
 from acme import challenges, client, crypto_util, errors, messages
 import async_timeout
-from atomicwrites import atomic_write
 import attr
 from cryptography import x509
-from cryptography.hazmat.primitives import hashes, serialization
+from cryptography.hazmat.backends import default_backend
+from cryptography.hazmat.primitives import serialization, hashes
 from cryptography.hazmat.primitives.asymmetric import rsa
-from cryptography.x509.extensions import SubjectAlternativeName
 from cryptography.x509.oid import NameOID
 import josepy as jose
-import OpenSSL
 
 from . import cloud_api
-from .utils import utcnow
+from .utils import UTC
 
 FILE_ACCOUNT_KEY = "acme_account.pem"
 FILE_PRIVATE_KEY = "remote_private.pem"
 FILE_FULLCHAIN = "remote_fullchain.pem"
 FILE_REGISTRATION = "acme_reg.json"
 
 ACCOUNT_KEY_SIZE = 2048
 PRIVATE_KEY_SIZE = 2048
 USER_AGENT = "home-assistant-cloud"
 
 _LOGGER = logging.getLogger(__name__)
 
-if TYPE_CHECKING:
-    from . import Cloud, _ClientT
-
 
 class AcmeClientError(Exception):
     """Raise if a acme client error raise."""
 
 
 class AcmeChallengeError(AcmeClientError):
     """Raise if a challenge fails."""
 
 
-class AcmeJWSVerificationError(AcmeClientError):
-    """Raise if a JWS verification fails."""
-
-
 class AcmeNabuCasaError(AcmeClientError):
-    """Raise errors on nabucasa API."""
+    """Raise erros on nabucasa API."""
 
 
 @attr.s
 class ChallengeHandler:
     """Handle ACME data over a challenge."""
 
-    challenge = attr.ib(type=messages.ChallengeBody)
+    challenge = attr.ib(type=messages.ChallengeResource)
     order = attr.ib(type=messages.OrderResource)
     response = attr.ib(type=challenges.ChallengeResponse)
     validation = attr.ib(type=str)
 
 
 class AcmeHandler:
     """Class handle a local certification."""
 
-    def __init__(self, cloud: Cloud[_ClientT], domains: list[str], email: str) -> None:
+    def __init__(self, cloud, domain: str, email: str) -> None:
         """Initialize local ACME Handler."""
         self.cloud = cloud
-        self._acme_server = f"https://{cloud.acme_server}/directory"
-        self._account_jwk: jose.JWKRSA | None = None
-        self._acme_client: client.ClientV2 | None = None
-        self._x509: x509.Certificate | None = None
+        self._acme_server = cloud.acme_directory_server
+        self._account_jwk = None
+        self._acme_client = None
+        self._x509 = None
 
-        self._domains = domains
+        self._domain = domain
         self._email = email
 
     @property
-    def email(self) -> str:
-        """Return the email."""
-        return self._email
-
-    @property
-    def domains(self) -> list[str]:
-        """Return the domains."""
-        return self._domains
-
-    @property
     def path_account_key(self) -> Path:
         """Return path of account key."""
         return Path(self.cloud.path(FILE_ACCOUNT_KEY))
 
     @property
     def path_private_key(self) -> Path:
         """Return path of private key."""
@@ -114,47 +92,34 @@
     def certificate_available(self) -> bool:
         """Return True if a certificate is loaded."""
         return self._x509 is not None
 
     @property
     def is_valid_certificate(self) -> bool:
         """Validate date of a certificate and return True is valid."""
-        if (expire_date := self.expire_date) is None:
+        if not self._x509:
             return False
-        return expire_date > utcnow()
+        return self._x509.not_valid_after > datetime.utcnow()
 
     @property
-    def expire_date(self) -> datetime | None:
+    def expire_date(self) -> Optional[datetime]:
         """Return datetime of expire date for certificate."""
         if not self._x509:
             return None
-        return self._x509.not_valid_after_utc
+        return self._x509.not_valid_after.replace(tzinfo=UTC)
 
     @property
-    def common_name(self) -> str | None:
+    def common_name(self) -> Optional[str]:
         """Return CommonName of certificate."""
         if not self._x509:
             return None
-        return str(
-            self._x509.subject.get_attributes_for_oid(NameOID.COMMON_NAME)[0].value,
-        )
+        return self._x509.subject.get_attributes_for_oid(NameOID.COMMON_NAME)[0].value
 
     @property
-    def alternative_names(self) -> list[str] | None:
-        """Return alternative names of certificate."""
-        if not self._x509:
-            return None
-
-        alternative_names = self._x509.extensions.get_extension_for_class(
-            SubjectAlternativeName,
-        ).value
-        return [str(entry.value) for entry in alternative_names]
-
-    @property
-    def fingerprint(self) -> str | None:
+    def fingerprint(self) -> Optional[str]:
         """Return SHA1 hex string as fingerprint."""
         if not self._x509:
             return None
         fingerprint = self._x509.fingerprint(hashes.SHA1())
         return fingerprint.hex()
 
     def _generate_csr(self) -> bytes:
@@ -165,387 +130,250 @@
         else:
             _LOGGER.debug("create private keyfile: %s", self.path_private_key)
             key = OpenSSL.crypto.PKey()
             key.generate_key(OpenSSL.crypto.TYPE_RSA, PRIVATE_KEY_SIZE)
             key_pem = OpenSSL.crypto.dump_privatekey(OpenSSL.crypto.FILETYPE_PEM, key)
 
             self.path_private_key.write_bytes(key_pem)
-            self.path_private_key.chmod(0o600)
 
-        return crypto_util.make_csr(key_pem, self._domains)
+        return crypto_util.make_csr(key_pem, [self._domain])
 
     def _load_account_key(self) -> None:
         """Load or create account key."""
+        key = None
         if self.path_account_key.exists():
             _LOGGER.debug("Load account keyfile: %s", self.path_account_key)
             pem = self.path_account_key.read_bytes()
-            key = serialization.load_pem_private_key(pem, password=None)
+            key = serialization.load_pem_private_key(
+                pem, password=None, backend=default_backend()
+            )
 
         else:
             _LOGGER.debug("Create new RSA keyfile: %s", self.path_account_key)
             key = rsa.generate_private_key(
                 public_exponent=65537,
                 key_size=ACCOUNT_KEY_SIZE,
+                backend=default_backend(),
             )
 
             # Store it to file
             pem = key.private_bytes(
                 encoding=serialization.Encoding.PEM,
                 format=serialization.PrivateFormat.PKCS8,
                 encryption_algorithm=serialization.NoEncryption(),
             )
             self.path_account_key.write_bytes(pem)
             self.path_account_key.chmod(0o600)
 
-        if TYPE_CHECKING:
-            assert isinstance(key, rsa.RSAPrivateKey)
         self._account_jwk = jose.JWKRSA(key=jose.ComparableRSAKey(key))
 
     def _create_client(self) -> None:
         """Create new ACME client."""
         if self.path_registration_info.exists():
             _LOGGER.info("Load exists ACME registration")
             regr = messages.RegistrationResource.json_loads(
-                self.path_registration_info.read_text(encoding="utf-8"),
+                self.path_registration_info.read_text()
             )
 
             acme_url = urllib.parse.urlparse(self._acme_server)
             regr_url = urllib.parse.urlparse(regr.uri)
 
             if acme_url[0] != regr_url[0] or acme_url[1] != regr_url[1]:
                 _LOGGER.info("Reset new ACME registration")
                 self.path_registration_info.unlink()
                 self.path_account_key.unlink()
 
         # Make sure that account key is loaded
         self._load_account_key()
-        assert self._account_jwk is not None
 
         # Load a exists registration
         if self.path_registration_info.exists():
             try:
                 network = client.ClientNetwork(
-                    self._account_jwk,
-                    account=regr,
-                    user_agent=USER_AGENT,
+                    self._account_jwk, account=regr, user_agent=USER_AGENT
                 )
-                directory = client.ClientV2.get_directory(
-                    url=self._acme_server,
-                    net=network,
-                )
-                self._acme_client = client.ClientV2(directory=directory, net=network)
-            except (errors.Error, ValueError) as err:
-                # https://github.com/certbot/certbot/blob/63fb97d8dea73ba63964f69fac0b15acfed02b3e/acme/acme/client.py#L670
-                # The client raises ValueError for RequestException
-                raise AcmeClientError(f"Can't connect to ACME server: {err}") from err
+                directory = messages.Directory.from_json(network.get(self._acme_server).json())
+                self._acme_client = client.ClientV2(directory, net=network)
+            except errors.Error as err:
+                _LOGGER.error("Can't connect to ACME server: %s", err)
+                raise AcmeClientError()
             return
 
         # Create a new registration
         try:
             network = client.ClientNetwork(self._account_jwk, user_agent=USER_AGENT)
-            directory = client.ClientV2.get_directory(
-                url=self._acme_server,
-                net=network,
-            )
-            self._acme_client = client.ClientV2(directory=directory, net=network)
-        except (errors.Error, ValueError) as err:
-            raise AcmeClientError(f"Can't connect to ACME server: {err}") from err
+            directory = messages.Directory.from_json(network.get(self._acme_server).json())
+            self._acme_client = client.ClientV2(directory, net=network)
+        except errors.Error as err:
+            _LOGGER.error("Can't connect to ACME server: %s", err)
+            raise AcmeClientError()
 
         try:
             _LOGGER.info(
                 "Register a ACME account with TOS: %s",
                 self._acme_client.directory.meta.terms_of_service,
             )
             regr = self._acme_client.new_account(
                 messages.NewRegistration.from_data(
-                    email=self._email,
-                    terms_of_service_agreed=True,
-                ),
+                    email=self._email, terms_of_service_agreed=True
+                )
             )
         except errors.Error as err:
-            raise AcmeClientError(f"Can't register to ACME server: {err}") from err
+            _LOGGER.error("Can't register to ACME server: %s", err)
+            raise AcmeClientError()
 
         # Store registration info
-        self.path_registration_info.write_text(
-            regr.json_dumps_pretty(),
-            encoding="utf-8",
-        )
+        self.path_registration_info.write_text(regr.json_dumps_pretty())
         self.path_registration_info.chmod(0o600)
 
-    def _create_order(self, csr_pem: bytes) -> messages.OrderResource:
+    def _start_challenge(self, csr_pem: str) -> ChallengeHandler:
         """Initialize domain challenge and return token."""
         _LOGGER.info("Initialize challenge for a new ACME certificate")
-        assert self._acme_client is not None
         try:
-            return self._acme_client.new_order(csr_pem)
-        except (messages.Error, errors.Error) as err:
-            if (
-                isinstance(err, messages.Error)
-                and err.typ == "urn:ietf:params:acme:error:malformed"
-                and err.detail == "JWS verification error"
-            ):
-                raise AcmeJWSVerificationError(
-                    f"JWS verification failed: {err}",
-                ) from None
-            raise AcmeChallengeError(
-                f"Can't order a new ACME challenge: {err}",
-            ) from None
-
-    def _start_challenge(self, order: messages.OrderResource) -> list[ChallengeHandler]:
-        """Initialize domain challenge and return token."""
-        _LOGGER.info("Start challenge for a new ACME certificate")
+            order = self._acme_client.new_order(csr_pem)
+        except errors.Error as err:
+            _LOGGER.error("Can't order a new ACME challenge: %s", err)
+            raise AcmeChallengeError() from None
 
         # Find DNS challenge
         # pylint: disable=not-an-iterable
-        dns_challenges: list[messages.ChallengeBody] = []
+        dns_challenge = None
         for auth in order.authorizations:
             for challenge in auth.body.challenges:
                 if challenge.typ != "dns-01":
                     continue
-                dns_challenges.append(challenge)
-
-        if len(dns_challenges) == 0:
-            raise AcmeChallengeError("No pending ACME challenge")
+                dns_challenge = challenge
 
-        handlers = []
-
-        for dns_challenge in dns_challenges:
-            try:
-                response, validation = dns_challenge.response_and_validation(
-                    self._account_jwk,
-                )
-            except errors.Error as err:
-                raise AcmeChallengeError(
-                    f"Can't validate the new ACME challenge: {err}",
-                ) from None
-            handlers.append(
-                ChallengeHandler(dns_challenge, order, response, validation),
+        try:
+            response, validation = dns_challenge.response_and_validation(
+                self._account_jwk
             )
+        except errors.Error as err:
+            _LOGGER.error("Can't validate the new ACME challenge: %s", err)
+            raise AcmeChallengeError() from None
 
-        return handlers
+        return ChallengeHandler(dns_challenge, order, response, validation)
 
-    def _answer_challenge(self, handler: ChallengeHandler) -> None:
-        """Answer challenge."""
-        _LOGGER.info("Answer challenge for the new ACME certificate")
-        if TYPE_CHECKING:
-            assert self._acme_client is not None
+    def _finish_challenge(self, handler: ChallengeHandler) -> None:
+        """Wait until challenge is finished."""
+        _LOGGER.info("Finishing challenge for the new ACME certificate")
         try:
             self._acme_client.answer_challenge(handler.challenge, handler.response)
         except errors.Error as err:
-            raise AcmeChallengeError(f"Can't accept ACME challenge: {err}") from err
+            _LOGGER.error("Can't accept ACME challenge: %s", err)
+            raise AcmeChallengeError()
 
-    def _finish_challenge(self, order: messages.OrderResource) -> None:
-        """Wait until challenge is finished."""
-        # Wait until it's authorize and fetch certification
-        if TYPE_CHECKING:
-            assert self._acme_client is not None
-        deadline = datetime.now() + timedelta(seconds=90)
-        try:
-            order = self._acme_client.poll_authorizations(order, deadline)
-            order = self._acme_client.finalize_order(
-                order,
-                deadline,
-                fetch_alternative_chains=True,
-            )
+        try:
+            order = self._acme_client.poll_and_finalize(handler.order)
         except errors.Error as err:
-            raise AcmeChallengeError(f"Wait of ACME challenge fails: {err}") from err
-        except Exception:  # pylint: disable=broad-except
-            _LOGGER.exception("Unexpected exception while finalizing order")
-            raise AcmeChallengeError(
-                "Unexpected exception while finalizing order",
-            ) from None
+            _LOGGER.error("Wait of ACME challenge fails: %s", err)
+            raise AcmeChallengeError()
 
         # Cleanup the old stuff
         if self.path_fullchain.exists():
             _LOGGER.info("Renew old certificate: %s", self.path_fullchain)
             self.path_fullchain.unlink()
         else:
             _LOGGER.info("Create new certificate: %s", self.path_fullchain)
 
-        with atomic_write(self.path_fullchain, overwrite=True) as fp:
-            fp.write(order.fullchain_pem)
+        self.path_fullchain.write_text(order.fullchain_pem)
         self.path_fullchain.chmod(0o600)
 
     async def load_certificate(self) -> None:
         """Get x509 Cert-Object."""
         if self._x509 or not self.path_fullchain.exists():
             return
 
-        def _load_cert() -> x509.Certificate:
+        def _load_cert():
             """Load certificate in a thread."""
-            return x509.load_pem_x509_certificate(self.path_fullchain.read_bytes())
+            return x509.load_pem_x509_certificate(
+                self.path_fullchain.read_bytes(),
+                default_backend()
+            )
 
-        try:
-            self._x509 = await self.cloud.run_executor(_load_cert)
-        except Exception:  # pylint: disable=broad-except
-            _LOGGER.exception("Unexpected exception loading certificate")
+        self._x509 = await self.cloud.run_executor(_load_cert)
 
     def _revoke_certificate(self) -> None:
         """Revoke certificate."""
         if not self.path_fullchain.exists():
             _LOGGER.warning("Can't revoke not exists certificate")
             return
 
-        if self._acme_client is None:
-            _LOGGER.error("No acme client")
-            return
-
         fullchain = jose.ComparableX509(
             OpenSSL.crypto.load_certificate(
-                OpenSSL.crypto.FILETYPE_PEM,
-                self.path_fullchain.read_bytes(),
-            ),
+                OpenSSL.crypto.FILETYPE_PEM, self.path_fullchain.read_bytes()
+            )
         )
 
         _LOGGER.info("Revoke certificate")
         try:
-            # https://letsencrypt.org/docs/revoking/#specifying-a-reason-code
-            self._acme_client.revoke(fullchain, 4)
+            self._acme_client.revoke(fullchain, 0)
         except errors.ConflictError:
             pass
         except errors.Error as err:
-            # Ignore errors where certificate did not exist
-            if "No such certificate" in str(err):  # noqa: SIM114
-                pass
-            # Ignore errors where certificate has expired
-            elif "Certificate is expired" in str(err):  # noqa: SIM114
-                pass
-            # Ignore errors where unrecognized issuer (happens dev/prod switch)
-            elif "Certificate from unrecognized issuer" in str(err):
-                pass
-            else:
-                raise AcmeClientError(f"Can't revoke certificate: {err}") from err
+            _LOGGER.error("Can't revoke certificate: %s", err)
+            raise AcmeClientError() from None
+
+        self.path_fullchain.unlink()
+        self.path_private_key.unlink()
 
     def _deactivate_account(self) -> None:
         """Deactivate account."""
-        if not self.path_registration_info.exists() or self._acme_client is None:
+        if not self.path_registration_info.exists():
             return
 
         _LOGGER.info("Load exists ACME registration")
         regr = messages.RegistrationResource.json_loads(
-            self.path_registration_info.read_text(encoding="utf-8"),
+            self.path_registration_info.read_text()
         )
 
         try:
             self._acme_client.deactivate_registration(regr)
         except errors.Error as err:
-            raise AcmeClientError(f"Can't deactivate account: {err}") from err
+            _LOGGER.error("Can't deactivate account: %s", err)
+            raise AcmeClientError()
 
-    def _have_any_file(self) -> bool:
-        return (
-            self.path_registration_info.exists()
-            or self.path_account_key.exists()
-            or self.path_fullchain.exists()
-            or self.path_private_key.exists()
-        )
-
-    def _remove_files(self) -> None:
-        self.path_registration_info.unlink(missing_ok=True)
-        self.path_account_key.unlink(missing_ok=True)
-        self.path_fullchain.unlink(missing_ok=True)
-        self.path_private_key.unlink(missing_ok=True)
+        self.path_registration_info.unlink()
+        self.path_account_key.unlink()
 
     async def issue_certificate(self) -> None:
         """Create/Update certificate."""
         if not self._acme_client:
             await self.cloud.run_executor(self._create_client)
 
         # Initialize challenge / new certificate
         csr = await self.cloud.run_executor(self._generate_csr)
-        order = await self.cloud.run_executor(self._create_order, csr)
-        dns_challenges: list[ChallengeHandler] = await self.cloud.run_executor(
-            self._start_challenge,
-            order,
-        )
+        challenge = await self.cloud.run_executor(self._start_challenge, csr)
 
+        # Update DNS
         try:
-            for challenge in dns_challenges:
-                # Update DNS
-                try:
-                    async with async_timeout.timeout(30):
-                        resp = await cloud_api.async_remote_challenge_txt(
-                            self.cloud,
-                            challenge.validation,
-                        )
-                    assert resp.status in (200, 201)
-                except (TimeoutError, AssertionError):
-                    raise AcmeNabuCasaError(
-                        "Can't set challenge token to NabuCasa DNS!",
-                    ) from None
-
-                # Answer challenge
-                try:
-                    _LOGGER.info(
-                        "Waiting 60 seconds for publishing DNS to ACME provider",
-                    )
-                    await asyncio.sleep(60)
-                    await self.cloud.run_executor(self._answer_challenge, challenge)
-                except AcmeChallengeError as err:
-                    _LOGGER.error("Could not complete answer challenge - %s", err)
-                    # There is no point in continuing here
-                    break
-                except Exception:  # pylint: disable=broad-except
-                    _LOGGER.exception("Unexpected exception while answering challenge")
-                    # There is no point in continuing here
-                    break
-        finally:
-            try:
-                async with async_timeout.timeout(30):
-                    # We only need to cleanup for the last entry
-                    await cloud_api.async_remote_challenge_cleanup(
-                        self.cloud,
-                        dns_challenges[-1].validation,
-                    )
-            except TimeoutError:
-                _LOGGER.error("Failed to clean up challenge from NabuCasa DNS!")
+            async with async_timeout.timeout(15):
+                resp = await cloud_api.async_remote_challenge_txt(
+                    self.cloud, challenge.validation
+                )
+            assert resp.status == 200
+        except (asyncio.TimeoutError, AssertionError):
+            _LOGGER.error("Can't set challenge token to NabuCasa DNS!")
+            raise AcmeNabuCasaError() from None
 
         # Finish validation
         try:
-            await self.cloud.run_executor(self._finish_challenge, order)
-        except AcmeChallengeError as err:
-            raise AcmeNabuCasaError(f"Could not finish challenge - {err}") from err
-        await self.load_certificate()
+            _LOGGER.info("Wait 60sec for publishing DNS to ACME provider")
+            await asyncio.sleep(60)
+            await self.cloud.run_executor(self._finish_challenge, challenge)
+            await self.load_certificate()
+        finally:
+            await cloud_api.async_remote_challenge_cleanup(self.cloud, challenge.validation)
 
     async def reset_acme(self) -> None:
         """Revoke and deactivate acme certificate/account."""
         _LOGGER.info("Revoke and deactivate ACME user/certificate")
-        if (
-            self._acme_client is None
-            and self._account_jwk is None
-            and self._x509 is None
-            and not await self.cloud.run_executor(self._have_any_file)
-        ):
-            _LOGGER.info("ACME user/certificates already cleaned up")
-            return
-
         if not self._acme_client:
             await self.cloud.run_executor(self._create_client)
 
         try:
-            with contextlib.suppress(AcmeClientError):
-                await self.cloud.run_executor(self._revoke_certificate)
-            with contextlib.suppress(AcmeClientError):
-                await self.cloud.run_executor(self._deactivate_account)
+            await self.cloud.run_executor(self._revoke_certificate)
+            await self.cloud.run_executor(self._deactivate_account)
         finally:
             self._acme_client = None
             self._account_jwk = None
             self._x509 = None
-            await self.cloud.run_executor(self._remove_files)
-
-    async def hardening_files(self) -> None:
-        """Control permission on files."""
-
-        def _control() -> None:
-            # Set file permission to 0600
-            if self.path_account_key.exists():
-                self.path_account_key.chmod(0o600)
-            if self.path_registration_info.exists():
-                self.path_registration_info.chmod(0o600)
-            if self.path_fullchain.exists():
-                self.path_fullchain.chmod(0o600)
-            if self.path_private_key.exists():
-                self.path_private_key.chmod(0o600)
-
-        try:
-            await self.cloud.run_executor(_control)
-        except OSError:
-            _LOGGER.warning("Can't check and hardening file permission")
```

### Comparing `hass_nabucasa-0.81.0/hass_nabucasa/cloudhooks.py` & `hass-nabucasa-0.9/hass_nabucasa/cloudhooks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,19 @@
 """Manage cloud cloudhooks."""
-
-from __future__ import annotations
-
-from typing import TYPE_CHECKING, Any
+from typing import Dict, Any
 
 import async_timeout
 
 from . import cloud_api
 
-if TYPE_CHECKING:
-    from . import Cloud, _ClientT
-
 
 class Cloudhooks:
     """Class to help manage cloudhooks."""
 
-    def __init__(self, cloud: Cloud[_ClientT]) -> None:
+    def __init__(self, cloud):
         """Initialize cloudhooks."""
         self.cloud = cloud
 
         cloud.iot.register_on_connect(self.async_publish_cloudhooks)
 
     async def async_publish_cloudhooks(self) -> None:
         """Inform the Relayer of the cloudhooks that we support."""
@@ -29,29 +23,28 @@
         cloudhooks = self.cloud.client.cloudhooks
         await self.cloud.iot.async_send_message(
             "webhook-register",
             {"cloudhook_ids": [info["cloudhook_id"] for info in cloudhooks.values()]},
             expect_answer=False,
         )
 
-    async def async_create(self, webhook_id: str, managed: bool) -> dict[str, Any]:
+    async def async_create(self, webhook_id: str, managed: bool) -> Dict[str, Any]:
         """Create a cloud webhook."""
         cloudhooks = self.cloud.client.cloudhooks
 
         if webhook_id in cloudhooks:
             raise ValueError("Hook is already enabled for the cloud.")
 
         if not self.cloud.iot.connected:
             raise ValueError("Cloud is not connected")
 
         # Create cloud hook
-        async with async_timeout.timeout(10):
+        with async_timeout.timeout(10):
             resp = await cloud_api.async_create_cloudhook(self.cloud)
 
-        resp.raise_for_status()
         data = await resp.json()
         cloudhook_id = data["cloudhook_id"]
         cloudhook_url = data["url"]
 
         # Store hook
         cloudhooks = dict(cloudhooks)
         hook = cloudhooks[webhook_id] = {
```

### Comparing `hass_nabucasa-0.81.0/hass_nabucasa/const.py` & `hass-nabucasa-0.9/hass_nabucasa/const.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 """Constants for the hass-nabucasa."""
-
-from __future__ import annotations
-
 CONFIG_DIR = ".cloud"
 
 REQUEST_TIMEOUT = 10
 
 MODE_PROD = "production"
 MODE_DEV = "development"
 
@@ -14,57 +11,45 @@
 STATE_DISCONNECTED = "disconnected"
 
 DISPATCH_REMOTE_CONNECT = "remote_connect"
 DISPATCH_REMOTE_DISCONNECT = "remote_disconnect"
 DISPATCH_REMOTE_BACKEND_UP = "remote_backend_up"
 DISPATCH_REMOTE_BACKEND_DOWN = "remote_backend_down"
 
-DEFAULT_SERVERS: dict[str, dict[str, str]] = {
-    "production": {
-        "account_link": "account-link.nabucasa.com",
-        "accounts": "accounts.nabucasa.com",
-        "acme": "acme-v02.api.letsencrypt.org",
-        "alexa": "alexa-api.nabucasa.com",
-        "cloudhook": "webhooks-api.nabucasa.com",
-        "relayer": "cloud.nabucasa.com",
-        "remotestate": "remotestate.nabucasa.com",
-        "servicehandlers": "servicehandlers.nabucasa.com",
-        "thingtalk": "thingtalk-api.nabucasa.com",
-    },
-    "development": {},
-}
-
-DEFAULT_VALUES: dict[str, dict[str, str]] = {
+SERVERS = {
     "production": {
         "cognito_client_id": "60i2uvhvbiref2mftj7rgcrt9u",
         "user_pool_id": "us-east-1_87ll5WOP8",
         "region": "us-east-1",
-    },
-    "development": {},
+        "relayer": "wss://cloud.nabucasa.com/websocket",
+        "google_actions_sync_url": (
+            "https://24ab3v80xd.execute-api.us-east-1."
+            "amazonaws.com/prod/smart_home_sync"
+        ),
+        "subscription_info_url": (
+            "https://stripe-api.nabucasa.com/payments/" "subscription_info"
+        ),
+        "cloudhook_create_url": "https://webhooks-api.nabucasa.com/generate",
+        "remote_api_url": "https://remote-sni-api.nabucasa.com",
+        "acme_directory_server": "https://acme-v02.api.letsencrypt.org/directory",
+    }
 }
 
 MESSAGE_EXPIRATION = """
 It looks like your Home Assistant Cloud subscription has expired. Please check
 your [account page](/config/cloud/account) to continue using the service.
 """
 
 MESSAGE_AUTH_FAIL = """
 You have been logged out of Home Assistant Cloud because we have been unable
 to verify your credentials. Please [log in](/config/cloud) again to continue
 using the service.
 """
 
 MESSAGE_REMOTE_READY = """
-Your remote access is now available.
-You can manage your connectivity on the
-[Cloud panel](/config/cloud) or with our [portal](https://account.nabucasa.com/).
+You remote access is now available.
+You can manage your connectivity on the [Cloud Panel](/config/cloud) or with our [Portal](https://remote.nabucasa.com/).
 """
 
 MESSAGE_REMOTE_SETUP = """
-Unable to create a certificate. We will automatically
-retry it and notify you when it's available.
-"""
-
-MESSAGE_LOAD_CERTIFICATE_FAILURE = """
-Unable to load the certificate. We will automatically
-recreate it and notify you when it's available.
+Unable to create a certificate. We will automatically retry it and notify you when it's available.
 """
```

### Comparing `hass_nabucasa-0.81.0/hass_nabucasa/iot_base.py` & `hass-nabucasa-0.9/hass_nabucasa/remote.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,335 +1,329 @@
-"""Base class to keep a websocket connection open to a server."""
-
-from __future__ import annotations
-
+"""Manage remote UI connections."""
 import asyncio
-from collections.abc import Awaitable, Callable
-import dataclasses
+from datetime import datetime, timedelta
 import logging
-import pprint
 import random
-from socket import gaierror
-from typing import TYPE_CHECKING, Any
+import ssl
+from typing import Optional
 
-from aiohttp import (
-    ClientError,
-    ClientWebSocketResponse,
-    WSMessage,
-    WSMsgType,
-    WSServerHandshakeError,
-    client_exceptions,
-    hdrs,
-)
+import async_timeout
+import attr
+from snitun.exceptions import SniTunConnectionError
+from snitun.utils.aes import generate_aes_keyset
+from snitun.utils.aiohttp_client import SniTunClientAioHttp
 
-from .auth import CloudError
-from .const import (
-    MESSAGE_EXPIRATION,
-    STATE_CONNECTED,
-    STATE_CONNECTING,
-    STATE_DISCONNECTED,
-)
-from .utils import gather_callbacks
+from . import cloud_api, utils, const
+from .acme import AcmeClientError, AcmeHandler
 
-if TYPE_CHECKING:
-    from . import Cloud, _ClientT
+_LOGGER = logging.getLogger(__name__)
 
 
-@dataclasses.dataclass
-class DisconnectReason:
-    """Disconnect reason."""
+class RemoteError(Exception):
+    """General remote error."""
 
-    clean: bool
-    reason: str
 
+class RemoteBackendError(RemoteError):
+    """Backend problem with nabucasa API."""
 
-class NotConnected(Exception):
-    """Exception raised when trying to handle unknown handler."""
 
+class RemoteNotConnected(RemoteError):
+    """Raise if a request need connection and we are not ready."""
 
-class BaseIoT:
-    """Class to manage the IoT connection."""
 
-    mark_connected_after_first_message = False
+@attr.s
+class SniTunToken:
+    """Handle snitun token."""
 
-    def __init__(self, cloud: Cloud[_ClientT]) -> None:
-        """Initialize the CloudIoT class."""
-        self.cloud = cloud
-        # The WebSocket client
-        self.client: ClientWebSocketResponse | None = None
-        # Scheduled sleep task till next connection retry
-        self.retry_task: asyncio.Task | None = None
-        # Boolean to indicate if we wanted the connection to close
-        self.close_requested: bool = False
-        # The current number of attempts to connect, impacts wait time
-        self.tries: int = 0
-        # Current state of the connection
-        self.state: str = STATE_DISCONNECTED
-        self._on_connect: list[Callable[[], Awaitable[None]]] = []
-        self._on_disconnect: list[Callable[[], Awaitable[None]]] = []
-        self._logger = logging.getLogger(self.package_name)
-        self._disconnect_event: asyncio.Event | None = None
-        self.last_disconnect_reason: DisconnectReason | None = None
+    fernet = attr.ib(type=bytes)
+    aes_key = attr.ib(type=bytes)
+    aes_iv = attr.ib(type=bytes)
+    valid = attr.ib(type=datetime)
+    throttling = attr.ib(type=int)
+
+
+@attr.s
+class Certificate:
+    """Handle certificate details."""
+
+    common_name = attr.ib(type=str)
+    expire_date = attr.ib(type=datetime)
+    fingerprint = attr.ib(type=str)
 
-    @property
-    def package_name(self) -> str:
-        """Return package name for logging."""
-        raise NotImplementedError
+
+class RemoteUI:
+    """Class to help manage remote connections."""
+
+    def __init__(self, cloud):
+        """Initialize cloudhooks."""
+        self.cloud = cloud
+        self._acme = None
+        self._snitun = None
+        self._snitun_server = None
+        self._instance_domain = None
+        self._reconnect_task = None
+        self._acme_task = None
+        self._token = None
+
+        # Register start/stop
+        cloud.iot.register_on_connect(self.load_backend)
+        cloud.iot.register_on_disconnect(self.close_backend)
 
     @property
-    def ws_heartbeat(self) -> float | None:
-        """Server to connect to."""
-        return None
+    def snitun_server(self) -> Optional[str]:
+        """Return connected snitun server."""
+        return self._snitun_server
 
     @property
-    def ws_server_url(self) -> str:
-        """Server to connect to."""
-        raise NotImplementedError
+    def instance_domain(self) -> Optional[str]:
+        """Return instance domain."""
+        return self._instance_domain
 
     @property
-    def require_subscription(self) -> bool:
-        """If the server requires a valid subscription."""
-        return True
-
-    def async_handle_message(self, msg: dict[str, Any]) -> None:
-        """Handle incoming message.
-
-        Run all async tasks in a wrapper to log appropriately.
-        """
-        raise NotImplementedError
-
-    # --- Do not override after this line ---
-
-    def register_on_connect(self, on_connect_cb: Callable[[], Awaitable[None]]) -> None:
-        """Register an async on_connect callback."""
-        self._on_connect.append(on_connect_cb)
-
-    def register_on_disconnect(
-        self,
-        on_disconnect_cb: Callable[[], Awaitable[None]],
-    ) -> None:
-        """Register an async on_disconnect callback."""
-        self._on_disconnect.append(on_disconnect_cb)
+    def is_connected(self) -> bool:
+        """Return true if we are ready to connect."""
+        if not self._snitun:
+            return False
+        return self._snitun.is_connected
 
     @property
-    def connected(self) -> bool:
-        """Return if we're currently connected."""
-        return self.state == STATE_CONNECTED
-
-    async def async_send_json_message(self, message: dict[str, Any]) -> None:
-        """Send a message.
-
-        Raises NotConnected if client not connected.
-        """
-        if self.state != STATE_CONNECTED or self.client is None:
-            raise NotConnected
+    def certificate(self) -> Optional[Certificate]:
+        """Return certificate details."""
+        if not self._acme or not self._acme.certificate_available:
+            return None
 
-        if self._logger.isEnabledFor(logging.DEBUG):
-            self._logger.debug("Publishing message:\n%s\n", pprint.pformat(message))
+        return Certificate(
+            self._acme.common_name, self._acme.expire_date, self._acme.fingerprint
+        )
 
-        await self.client.send_json(message)
+    async def _create_context(self) -> ssl.SSLContext:
+        """Create SSL context with acme certificate."""
+        context = utils.server_context_modern()
+
+        await self.cloud.run_executor(
+            context.load_cert_chain,
+            str(self._acme.path_fullchain),
+            str(self._acme.path_private_key),
+        )
 
-    async def connect(self) -> None:
-        """Connect to the IoT broker."""
-        if self.state != STATE_DISCONNECTED:
-            raise RuntimeError("Connect called while not disconnected")
-
-        self.close_requested = False
-        self.state = STATE_CONNECTING
-        self.tries = 0
-        self._disconnect_event = asyncio.Event()
+        return context
 
-        while True:
-            try:
-                self._logger.debug("Trying to connect")
-                await self._handle_connection()
-            except Exception:  # pylint: disable=broad-except
-                # Safety net. This should never hit.
-                # Still adding it here to make sure we can always reconnect
-                self._logger.exception("Unexpected error")
-
-            if self.state == STATE_CONNECTED:
-                await self._disconnected()
+    async def load_backend(self) -> None:
+        """Load backend details."""
+        if self._snitun:
+            return
 
-            if self.close_requested:
-                break
+        # Setup background task for ACME certification handler
+        if not self._acme_task:
+            self._acme_task = self.cloud.run_task(self._certificate_handler())
 
-            if self.require_subscription and self.cloud.subscription_expired:
-                break
+        # Load instance data from backend
+        try:
+            async with async_timeout.timeout(15):
+                resp = await cloud_api.async_remote_register(self.cloud)
+            assert resp.status == 200
+        except (asyncio.TimeoutError, AssertionError):
+            _LOGGER.error("Can't update remote details from Home Assistant cloud")
+            return
+        data = await resp.json()
 
-            self.state = STATE_CONNECTING
-            self.tries += 1
+        # Extract data
+        _LOGGER.debug("Retrieve instance data: %s", data)
+        domain = data["domain"]
+        email = data["email"]
+        server = data["server"]
+
+        # Set instance details for certificate
+        self._acme = AcmeHandler(self.cloud, domain, email)
+
+        # Load exists certificate
+        await self._acme.load_certificate()
+
+        # Domain changed / revoke CA
+        ca_domain = self._acme.common_name
+        if ca_domain is not None and ca_domain != domain:
+            _LOGGER.warning("Invalid certificate found: %s", ca_domain)
+            await self._acme.reset_acme()
 
+        # Issue a certificate
+        if not self._acme.is_valid_certificate:
             try:
-                await self._wait_retry()
-            except asyncio.CancelledError:
-                # Happens if disconnect called
-                break
-
-        self.state = STATE_DISCONNECTED
-        self._disconnect_event.set()
-        self._disconnect_event = None
-
-    async def _wait_retry(self) -> None:
-        """Wait until it's time till the next retry."""
-        # Sleep 2^tries + 0…tries*3 seconds between retries
-        self.retry_task = asyncio.create_task(
-            asyncio.sleep(2 ** min(9, self.tries) + random.randint(0, self.tries * 3)),
+                await self._acme.issue_certificate()
+            except AcmeClientError:
+                self.cloud.client.user_message(
+                    "cloud_remote_acme",
+                    "Home Assistant Cloud",
+                    const.MESSAGE_REMOTE_SETUP,
+                )
+                return
+            else:
+                self.cloud.client.user_message(
+                    "cloud_remote_acme",
+                    "Home Assistant Cloud",
+                    const.MESSAGE_REMOTE_READY,
+                )
+
+        # Setup snitun / aiohttp wrapper
+        context = await self._create_context()
+        self._snitun = SniTunClientAioHttp(
+            self.cloud.client.aiohttp_runner,
+            context,
+            snitun_server=server,
+            snitun_port=443,
         )
-        await self.retry_task
-        self.retry_task = None
 
-    async def _handle_connection(self) -> None:
-        """Connect to the IoT broker."""
-        try:
-            await self.cloud.auth.async_check_token()
-        except CloudError as err:
-            self._logger.warning(
-                "Cannot connect because unable to refresh token: %s",
-                err,
-            )
+        # Cache data
+        self._instance_domain = domain
+        self._snitun_server = server
+
+        await self._snitun.start()
+        self.cloud.client.dispatcher_message(const.DISPATCH_REMOTE_BACKEND_UP)
+
+        # Connect to remote is autostart enabled
+        if self.cloud.client.remote_autostart:
+            self.cloud.run_task(self.connect())
+
+    async def close_backend(self) -> None:
+        """Close connections and shutdown backend."""
+        # Close reconnect task
+        if self._reconnect_task:
+            self._reconnect_task.cancel()
+
+        # Close ACME certificate handler
+        if self._acme_task:
+            self._acme_task.cancel()
+
+        # Disconnect snitun
+        if self._snitun:
+            await self._snitun.stop()
+
+        # Cleanup
+        self._snitun = None
+        self._acme = None
+        self._token = None
+        self._instance_domain = None
+        self._snitun_server = None
+
+        self.cloud.client.dispatcher_message(const.DISPATCH_REMOTE_BACKEND_DOWN)
+
+    async def handle_connection_requests(self, caller_ip: str) -> None:
+        """Handle connection requests."""
+        if not self._snitun:
+            _LOGGER.error("Can't handle request-connection without backend")
+            raise RemoteNotConnected()
+
+        if self._snitun.is_connected:
             return
+        await self.connect()
 
-        if self.require_subscription and self.cloud.subscription_expired:
-            self._logger.debug("Cloud subscription expired. Cancelling connecting.")
-            self.cloud.client.user_message(
-                "cloud_subscription_expired",
-                "Home Assistant Cloud",
-                MESSAGE_EXPIRATION,
-            )
-            self.close_requested = True
+    async def _refresh_snitun_token(self) -> None:
+        """Handle snitun token."""
+        if self._token and self._token.valid > utils.utcnow():
+            _LOGGER.debug("Don't need refresh snitun token")
             return
 
-        disconnect_clean: bool = False
-        disconnect_reason: (
-            str
-            | WSServerHandshakeError
-            | ClientError
-            | ConnectionResetError
-            | gaierror
-            | None
-        ) = None
+        # Generate session token
+        aes_key, aes_iv = generate_aes_keyset()
         try:
-            self.client = await self.cloud.websession.ws_connect(
-                self.ws_server_url,
-                heartbeat=self.ws_heartbeat,
-                headers={
-                    hdrs.AUTHORIZATION: f"Bearer {self.cloud.id_token}",
-                    hdrs.USER_AGENT: self.cloud.client.client_name,
-                },
-            )
+            async with async_timeout.timeout(15):
+                resp = await cloud_api.async_remote_token(self.cloud, aes_key, aes_iv)
+            assert resp.status == 200
+        except (asyncio.TimeoutError, AssertionError):
+            raise RemoteBackendError() from None
+
+        data = await resp.json()
+        self._token = SniTunToken(
+            data["token"].encode(),
+            aes_key,
+            aes_iv,
+            utils.utc_from_timestamp(data["valid"]),
+            data["throttling"]
+        )
 
-            if not self.mark_connected_after_first_message:
-                await self._connected()
+    async def connect(self) -> None:
+        """Connect to snitun server."""
+        if not self._snitun:
+            _LOGGER.error("Can't handle request-connection without backend")
+            raise RemoteNotConnected()
 
-            while not self.client.closed:
-                msg: WSMessage | None | str = None
-                try:
-                    msg = await self.client.receive(55)
-                except TimeoutError:
-                    # This is logged as info instead of warning because when
-                    # this hits there is not really much that can be done about it.
-                    # But the context is still valuable to have while
-                    # troubleshooting.
-                    self._logger.info("Timeout while waiting to receive message")
-                    await self.client.ping()
-                    continue
+        # Check if we already connected
+        if self._snitun.is_connected:
+            return
 
-                if msg.type in (WSMsgType.CLOSE, WSMsgType.CLOSED, WSMsgType.CLOSING):
-                    disconnect_clean = self.state == STATE_CONNECTED
-                    disconnect_reason = f"Closed by server. {msg.extra} ({msg.data})"
-                    break
-
-                # Do this inside the loop because if 2 clients are connected,
-                # it can happen that we get connected with valid auth,
-                # but then server decides to drop our connection.
-                if self.state != STATE_CONNECTED:
-                    await self._connected()
-
-                if msg.type == WSMsgType.ERROR:
-                    disconnect_reason = "Connection error"
-                    break
-
-                if msg.type != WSMsgType.TEXT:
-                    disconnect_reason = f"Received non-Text message: {msg.type}"
-                    break
+        try:
+            await self._refresh_snitun_token()
+            await self._snitun.connect(
+                self._token.fernet, self._token.aes_key, self._token.aes_iv,
+                throttling=self._token.throttling
+            )
 
-                try:
-                    msg_content: dict[str, Any] = msg.json()
-                except ValueError:
-                    disconnect_reason = "Received invalid JSON."
-                    break
-
-                if self._logger.isEnabledFor(logging.DEBUG):
-                    self._logger.debug(
-                        "Received message:\n%s\n",
-                        pprint.pformat(msg_content),
-                    )
+            self.cloud.client.dispatcher_message(const.DISPATCH_REMOTE_CONNECT)
+        except SniTunConnectionError:
+            _LOGGER.error("Connection problem to snitun server")
+        except RemoteBackendError:
+            _LOGGER.error("Can't refresh the snitun token")
+        finally:
+            # start retry task
+            if not self._reconnect_task:
+                self._reconnect_task = self.cloud.run_task(self._reconnect_snitun())
 
-                try:
-                    self.async_handle_message(msg_content)
-                except Exception:  # pylint: disable=broad-except
-                    self._logger.exception("Unexpected error handling %s", msg_content)
-
-            if self.client.closed:
-                if self.close_requested:
-                    disconnect_clean = True
-                    disconnect_reason = "Close requested"
-                elif disconnect_reason is None:
-                    disconnect_reason = "Closed by server. Unknown reason"
-
-        except client_exceptions.WSServerHandshakeError as err:
-            if err.status == 401:
-                disconnect_reason = "Invalid auth."
-                self.close_requested = True
-                # Should we notify user?
-            else:
-                disconnect_reason = err
+    async def disconnect(self) -> None:
+        """Disconnect from snitun server."""
+        if not self._snitun:
+            _LOGGER.error("Can't handle request-connection without backend")
+            raise RemoteNotConnected()
+
+        # Stop reconnect task
+        if self._reconnect_task:
+            self._reconnect_task.cancel()
 
-        except (client_exceptions.ClientError, ConnectionResetError, gaierror) as err:
-            disconnect_reason = err
+        # Check if we already connected
+        if not self._snitun.is_connected:
+            return
+        await self._snitun.disconnect()
+        self.cloud.client.dispatcher_message(const.DISPATCH_REMOTE_DISCONNECT)
 
+    async def _reconnect_snitun(self) -> None:
+        """Reconnect after disconnect."""
+        try:
+            while True:
+                if self._snitun.is_connected:
+                    await self._snitun.wait()
+
+                self.cloud.client.dispatcher_message(const.DISPATCH_REMOTE_DISCONNECT)
+                await asyncio.sleep(random.randint(1, 15))
+                await self.connect()
         except asyncio.CancelledError:
-            disconnect_clean = True
-            disconnect_reason = "Connection Cancelled"
-
+            pass
         finally:
-            if self.client:
-                base_msg = "Connection closed"
-                await self.client.close()
-                self.client = None
-            else:
-                base_msg = "Unable to connect"
-            msg = f"{base_msg}: {disconnect_reason}"
-            self.last_disconnect_reason = DisconnectReason(disconnect_clean, msg)
+            _LOGGER.debug("Close remote UI reconnect guard")
+            self._reconnect_task = None
 
-            if self.close_requested or disconnect_clean:
-                self._logger.info(msg)
-            else:
-                self._logger.warning(msg)
+    async def _certificate_handler(self) -> None:
+        """Handle certification ACME Tasks."""
+        try:
+            while True:
+                await asyncio.sleep(utils.next_midnight())
 
-    async def disconnect(self) -> None:
-        """Disconnect the client."""
-        self.close_requested = True
+                # Backend not initialize / No certificate issue now
+                if not self._snitun:
+                    await self.load_backend()
+                    continue
+
+                # Renew certificate?
+                if self._acme.expire_date > utils.utcnow() + timedelta(days=14):
+                    continue
+
+                # Renew certificate
+                try:
+                    await self._acme.issue_certificate()
+                    await self.close_backend()
+                    await self.load_backend()
+                except AcmeClientError:
+                    _LOGGER.warning(
+                        "Renew of ACME certificate fails. Try it lager again"
+                    )
 
-        if self.client is not None:
-            await self.client.close()
-        elif self.retry_task is not None:
-            self.retry_task.cancel()
-
-        if self._disconnect_event is not None:
-            await self._disconnect_event.wait()
-
-    async def _connected(self) -> None:
-        """Handle connected."""
-        self.last_disconnect_reason = None
-        self.tries = 0
-        self.state = STATE_CONNECTED
-        self._logger.info("Connected")
-
-        if self._on_connect:
-            await gather_callbacks(self._logger, "on_connect", self._on_connect)
-
-    async def _disconnected(self) -> None:
-        """Handle connected."""
-        if self._on_disconnect:
-            await gather_callbacks(self._logger, "on_disconnect", self._on_disconnect)
+        except asyncio.CancelledError:
+            pass
+        finally:
+            self._acme_task = None
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hass_nabucasa-0.81.0/hass_nabucasa/utils.py` & `hass-nabucasa-0.9/hass_nabucasa/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,39 @@
 """Helper methods to handle the time in Home Assistant."""
-
-from __future__ import annotations
-
-import asyncio
-from collections.abc import Awaitable, Callable
 import datetime as dt
-from logging import Logger
 import ssl
-from typing import TypeVar
+from typing import Optional, Callable, TypeVar
 
-import ciso8601
+import pytz
 
-CALLABLE_T = TypeVar("CALLABLE_T", bound=Callable)  # pylint: disable=invalid-name
-UTC = dt.UTC
+CALLABLE_T = TypeVar("CALLABLE_T", bound=Callable)  # noqa pylint: disable=invalid-name
+DATE_STR_FORMAT = "%Y-%m-%d"
+UTC = pytz.utc
 
 
 def utcnow() -> dt.datetime:
     """Get now in UTC time."""
     return dt.datetime.now(UTC)
 
 
 def utc_from_timestamp(timestamp: float) -> dt.datetime:
     """Return a UTC time from a timestamp."""
-    return dt.datetime.fromtimestamp(timestamp, UTC)
+    return UTC.localize(dt.datetime.utcfromtimestamp(timestamp))
 
 
-def parse_date(dt_str: str) -> dt.date | None:
+def parse_date(dt_str: str) -> Optional[dt.date]:
     """Convert a date string to a date object."""
     try:
-        return ciso8601.parse_datetime(dt_str).date()
+        return dt.datetime.strptime(dt_str, DATE_STR_FORMAT).date()
     except ValueError:  # If dt_str did not match our format
         return None
 
 
 def server_context_modern() -> ssl.SSLContext:
-    """
-    Return an SSL context following the Mozilla recommendations.
-
+    """Return an SSL context following the Mozilla recommendations.
     TLS configuration follows the best-practice guidelines specified here:
     https://wiki.mozilla.org/Security/Server_Side_TLS
     Modern guidelines are followed.
     """
     context = ssl.SSLContext(ssl.PROTOCOL_TLS)  # pylint: disable=no-member
 
     context.options |= (
@@ -54,44 +47,28 @@
         context.options |= ssl.OP_NO_COMPRESSION
 
     context.set_ciphers(
         "ECDHE-ECDSA-AES256-GCM-SHA384:ECDHE-RSA-AES256-GCM-SHA384:"
         "ECDHE-ECDSA-CHACHA20-POLY1305:ECDHE-RSA-CHACHA20-POLY1305:"
         "ECDHE-ECDSA-AES128-GCM-SHA256:ECDHE-RSA-AES128-GCM-SHA256:"
         "ECDHE-ECDSA-AES256-SHA384:ECDHE-RSA-AES256-SHA384:"
-        "ECDHE-ECDSA-AES128-SHA256:ECDHE-RSA-AES128-SHA256",
+        "ECDHE-ECDSA-AES128-SHA256:ECDHE-RSA-AES128-SHA256"
     )
 
     return context
 
 
-def next_midnight() -> float:
+def next_midnight() -> int:
     """Return the seconds till next local midnight."""
     midnight = dt.datetime.now().replace(
-        hour=0,
-        minute=0,
-        second=0,
-        microsecond=0,
+        hour=0, minute=0, second=0, microsecond=0
     ) + dt.timedelta(days=1)
     return (midnight - dt.datetime.now()).total_seconds()
 
 
-async def gather_callbacks(
-    logger: Logger,
-    name: str,
-    callbacks: list[Callable[[], Awaitable[None]]],
-) -> None:
-    """Gather callbacks and log exceptions."""
-    results = await asyncio.gather(*[cb() for cb in callbacks], return_exceptions=True)
-    for result, callback in zip(results, callbacks, strict=False):
-        if not isinstance(result, Exception):
-            continue
-        logger.error("Unexpected error in %s %s", name, callback, exc_info=result)
-
-
 class Registry(dict):
     """Registry of items."""
 
     def register(self, name: str) -> Callable[[CALLABLE_T], CALLABLE_T]:
         """Return decorator to register item with a specific name."""
 
         def decorator(func: CALLABLE_T) -> CALLABLE_T:
```

