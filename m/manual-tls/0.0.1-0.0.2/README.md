# Comparing `tmp/manual_tls-0.0.1.tar.gz` & `tmp/manual_tls-0.0.2.tar.gz`

## Comparing `manual_tls-0.0.1.tar` & `manual_tls-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rwxr-xr-x   0        0        0      897 2020-02-02 00:00:00.000000 manual_tls-0.0.1/client.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 manual_tls-0.0.1/manual_tls/__init__.py
--rwxr-xr-x   0        0        0    32155 2020-02-02 00:00:00.000000 manual_tls-0.0.1/manual_tls/manual_tls.py
--rwxr-xr-x   0        0        0     3299 2020-02-02 00:00:00.000000 manual_tls-0.0.1/.gitignore
--rwxr-xr-x   0        0        0     1105 2020-02-02 00:00:00.000000 manual_tls-0.0.1/LICENSE
--rwxr-xr-x   0        0        0     8441 2020-02-02 00:00:00.000000 manual_tls-0.0.1/README.md
--rwxr-xr-x   0        0        0      600 2020-02-02 00:00:00.000000 manual_tls-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 manual_tls-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1106 2020-02-02 00:00:00.000000 manual_tls-0.0.2/client.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 manual_tls-0.0.2/manual_tls/__init__.py
+-rwxr-xr-x   0        0        0    38465 2020-02-02 00:00:00.000000 manual_tls-0.0.2/manual_tls/manual_tls.py
+-rwxr-xr-x   0        0        0     3299 2020-02-02 00:00:00.000000 manual_tls-0.0.2/.gitignore
+-rwxr-xr-x   0        0        0     1105 2020-02-02 00:00:00.000000 manual_tls-0.0.2/LICENSE
+-rwxr-xr-x   0        0        0     8441 2020-02-02 00:00:00.000000 manual_tls-0.0.2/README.md
+-rwxr-xr-x   0        0        0      632 2020-02-02 00:00:00.000000 manual_tls-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     8834 2020-02-02 00:00:00.000000 manual_tls-0.0.2/PKG-INFO
```

### Comparing `manual_tls-0.0.1/manual_tls/manual_tls.py` & `manual_tls-0.0.2/manual_tls/manual_tls.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,98 @@
+import base64
+
 from abc import ABC, abstractmethod
+from enum import IntEnum
+from hashlib import sha256
+from ecdsa import VerifyingKey, SigningKey, NIST256p
+from ecdsa.util import sigdecode_der
 
 # in tls 1.3 the version tls 1.2 is sent for better compatibility
 LEGACY_TLS_VERSION = b"\x03\x03"
 TLS_AES_128_GCM_SHA256 = b"\x13\x01"
 
 CHANGE_CIPHER = b"\x14"
 ALERT = b"\x15"
 HANDSHAKE = b"\x16"
 APPLICATION_DATA = b"\x17"
 
+class HandshakeType(IntEnum):
+    HELLO_REQUEST = 0
+    CLIENT_HELLO = 1
+    SERVER_HELLO = 2
+    HELLO_VERIFY_REQUEST = 3
+    NEW_SESSION_TICKET = 4
+    END_OF_EARLY_DATA = 5
+    HELLO_RETRY_REQUEST = 6
+    ENCRYPTED_EXTENSIONS = 8
+    CERTIFICATE = 11
+    SERVER_KEY_EXCHANGE = 12
+    CERTIFICATE_REQUEST = 13
+    SERVER_HELLO_DONE = 14
+    CERTIFICATE_VERIFY = 15
+    CLIENT_KEY_EXCHANGE = 16
+    FINISHED = 20
+    CERTIFICATE_URL = 21
+    CERTIFICATE_STATUS = 22
+    SUPPLEMENTAL_DATA = 23
+    KEY_UPDATE = 24
+    MESSAGE_HASH = 254
+
+class ExtensionType(IntEnum):
+    SERVER_NAME = 0                             # RFC 6066
+    MAX_FRAGMENT_LENGTH = 1                     # RFC 6066
+    STATUS_REQUEST = 5                          # RFC 6066
+    SUPPORTED_GROUPS = 10                       # RFC 8422, 7919
+    SIGNATURE_ALGORITHMS = 13                   # RFC 8446
+    USE_SRTP = 14                               # RFC 5764
+    HEARTBEAT = 15                              # RFC 6520
+    APPLICATION_LAYER_PROTOCOL_NEGOTIATION = 16 # RFC 7301
+    SIGNED_CERTIFICATE_TIMESTAMP = 18           # RFC 6962
+    CLIENT_CERTIFICATE_TYPE = 19                # RFC 7250
+    SERVER_CERTIFICATE_TYPE = 20                # RFC 7250
+    PADDING = 21                                # RFC 7685
+    PRE_SHARED_KEY = 41                         # RFC 8446
+    EARLY_DATA = 42                             # RFC 8446
+    SUPPORTED_VERSIONS = 43                     # RFC 8446
+    COOKIE = 44                                 # RFC 8446
+    PSK_KEY_EXCHANGE_MODES = 45                 # RFC 8446
+    CERTIFICATE_AUTHORITIES = 47                # RFC 8446
+    OID_FILTERS = 48                            # RFC 8446
+    POST_HANDSHAKE_AUTH = 49                    # RFC 8446
+    SIGNATURE_ALGORITHMS_CERT = 50              # RFC 8446
+    KEY_SHARE = 51                              # RFC 8446
+
+class SignatureScheme(IntEnum):
+    # RSASSA-PKCS1-v1_5 algorithms
+    RSA_PKCS1_SHA256 = 0X0401
+    RSA_PKCS1_SHA384 = 0X0501
+    RSA_PKCS1_SHA512 = 0X0601
+
+    # ECDSA algorithms
+    ECDSA_SECP256R1_SHA256 = 0X0403
+    ECDSA_SECP384R1_SHA384 = 0X0503
+    ECDSA_SECP521R1_SHA512 = 0X0603          
+
+    # RSASSA-PSS algorithms with public key OID rsaEncryption
+    RSA_PSS_RSAE_SHA256 = 0X0804
+    RSA_PSS_RSAE_SHA384 = 0X0805
+    RSA_PSS_RSAE_SHA512 = 0X0806
+
+    # EdDSA algorithms
+    ED25519 = 0X0807
+    ED448 = 0X0808
+
+    # RSASSA-PSS algorithms with public key OID RSASSA-PSS
+    RSA_PSS_PSS_SHA256 = 0X0809
+    RSA_PSS_PSS_SHA384 = 0X080A
+    RSA_PSS_PSS_SHA512 = 0X080B
+
+    # Legacy algorithms
+    RSA_PKCS1_SHA1 = 0X0201
+    ECDSA_SHA1 = 0X0203
 
 # BYTE MANIPULATION HELPERS
 def bytes_to_num(b):
     return int.from_bytes(b, "big")
 
 def num_to_bytes(num, bytes_len):
     return int.to_bytes(num, bytes_len, "big")
@@ -156,63 +236,29 @@
 def aes128_gcm_encrypt(key, msg, nonce, associated_data):
     encrypted_msg = aes128_ctr_encrypt(key, msg, nonce, counter_start_val=2)
 
     pretag = calc_pretag(key, encrypted_msg, associated_data)
     tag = aes128_ctr_encrypt(key, pretag, nonce, counter_start_val=1)
     return encrypted_msg + tag
 
-
-# CRYPTOGRAPHIC HASH FUNCTIONS AND MESSAGE AUTHENTICATION CODES
-SHA256_K = [
-    0x428a2f98, 0x71374491, 0xb5c0fbcf, 0xe9b5dba5, 0x3956c25b, 0x59f111f1, 0x923f82a4, 0xab1c5ed5,
-    0xd807aa98, 0x12835b01, 0x243185be, 0x550c7dc3, 0x72be5d74, 0x80deb1fe, 0x9bdc06a7, 0xc19bf174,
-    0xe49b69c1, 0xefbe4786, 0x0fc19dc6, 0x240ca1cc, 0x2de92c6f, 0x4a7484aa, 0x5cb0a9dc, 0x76f988da,
-    0x983e5152, 0xa831c66d, 0xb00327c8, 0xbf597fc7, 0xc6e00bf3, 0xd5a79147, 0x06ca6351, 0x14292967,
-    0x27b70a85, 0x2e1b2138, 0x4d2c6dfc, 0x53380d13, 0x650a7354, 0x766a0abb, 0x81c2c92e, 0x92722c85,
-    0xa2bfe8a1, 0xa81a664b, 0xc24b8b70, 0xc76c51a3, 0xd192e819, 0xd6990624, 0xf40e3585, 0x106aa070,
-    0x19a4c116, 0x1e376c08, 0x2748774c, 0x34b0bcb5, 0x391c0cb3, 0x4ed8aa4a, 0x5b9cca4f, 0x682e6ff3,
-    0x748f82ee, 0x78a5636f, 0x84c87814, 0x8cc70208, 0x90befffa, 0xa4506ceb, 0xbef9a3f7, 0xc67178f2
-]
-
-
-def sha256(msg):
-    msg += b"\x80" + b"\x00" * ((64-(len(msg) + 1 + 8)) % 64) + num_to_bytes(len(msg)*8, 8)
-
-    ss = [0x6a09e667, 0xbb67ae85, 0x3c6ef372, 0xa54ff53a, 0x510e527f, 0x9b05688c, 0x1f83d9ab, 0x5be0cd19]
-    for pos in range(0, len(msg), 64):
-        chunk = msg[pos:pos + 64]
-
-        w = [bytes_to_num(chunk[4*i:4*i+4]) for i in range(16)]
-        for i in range(16, 64):
-            a = rotr(w[i-15], 7) ^ rotr(w[i-15], 18) ^ (w[i-15] >> 3)
-            b = rotr(w[i-2], 17) ^ rotr(w[i-2], 19) ^ (w[i-2] >> 10)
-            w.append((a + b + w[i-16] + w[i-7]) & 0xffffffff)
-
-        s = ss.copy()
-        for i in range(64):
-            c = (s[4] & s[5]) ^ ((s[4] ^ 0xffffffff) & s[6])
-            t = SHA256_K[i] + s[7] + c + w[i] + (rotr(s[4], 6) ^ rotr(s[4], 11) ^ rotr(s[4], 25))
-            q = rotr(s[0], 2) ^ rotr(s[0], 13) ^ rotr(s[0], 22)
-            m = (s[0] & s[1]) ^ (s[0] & s[2]) ^ (s[1] & s[2])
-            s = [(q + m + t) & 0xffffffff, s[0], s[1], s[2], (s[3] + t) & 0xffffffff, s[4], s[5], s[6]]
-
-        ss = [(ss[i] + s[i]) & 0xffffffff for i in range(8)]
-    return b"".join(num_to_bytes(a, 4) for a in ss)
-
+def one_shot_sha256(data):
+    m = sha256()
+    m.update(data)
+    return m.digest()
 
 def hmac_sha256(key, data):
     BLOCK_SIZE = 512 // 8
     IPAD = b"\x36" * BLOCK_SIZE
     OPAD = b"\x5c" * BLOCK_SIZE
 
     if len(key) <= BLOCK_SIZE:
         key += b"\x00" * (BLOCK_SIZE - len(key))
     else:
-        key = sha256(key)
-    return sha256(xor(key, OPAD) + sha256(xor(key, IPAD) + data))
+        key = one_shot_sha256(key)
+    return one_shot_sha256(xor(key, OPAD) + one_shot_sha256(xor(key, IPAD) + data))
 
 
 def derive_secret(label, key, data, hash_len):
     full_label = b"tls13 " + label
     packed_data = (num_to_bytes(hash_len, 2) + num_to_bytes(len(full_label), 1) +
                 full_label + num_to_bytes(len(data), 1) + data)
 
@@ -276,28 +322,67 @@
 
     data = msg_type + LEGACY_TLS_VERSION + num_to_bytes(len(payload), 2)
     msg = aes128_gcm_decrypt(key, payload, nonce, associated_data=data)
 
     msg_type, msg_data = msg[-1:], msg[:-1]
     return msg_type, msg_data
 
+class Extension:
+    def __init__(self, type, value) -> None:
+        self.type = type
+        self.value = value    
+
+class Parser:    
+    def __init__(self, buffer : bytes, offset = 0) -> None:
+        self.buffer = buffer
+        self.offset = offset
+
+    def get_uint8(self):
+        v = self.buffer[self.offset]
+        self.offset += 1
+        return v
+
+    def get_uint16(self):
+        v = bytes_to_num(self.buffer[self.offset : self.offset + 2])
+        self.offset += 2
+        return v
+
+    def get_uint24(self):
+        v = bytes_to_num(self.buffer[self.offset : self.offset + 3])
+        self.offset += 3
+        return v
+
+    def get_data(self, len):
+        v = self.buffer[self.offset : self.offset + len]
+        self.offset += len
+        return v
+
+    def bytes_left(self):
+        return len(self.buffer) - self.offset
 
 class ManualComm(ABC):
     @abstractmethod
+    def prepare_send(self, data) -> None:
+        pass
+    
+    @abstractmethod
     def sendall(self, data) -> None:
         pass
 
     @abstractmethod
     def recv(self, bufsize: int) -> bytes:
         pass
 
 
 class ManualTls:
     def __init__(self, comm: ManualComm) -> None:
         self.comm = comm
+        self.server_certificate_type = 0
+        self.client_certificate_type = 0
+        self.signature_algorithms = []
     
     # NETWORK AND LOW LEVEL TLS PROTOCOL HELPERS
     def recv_num_bytes(self, num):
         ret = bytearray()
         while len(ret) < num:
             data = self.comm.recv(min(4096, num - len(ret)))
             if not data:
@@ -315,26 +400,38 @@
         #assert tls_version == LEGACY_TLS_VERSION
 
         rec_len = bytes_to_num(self.recv_num_bytes(2))
         rec = self.recv_num_bytes(rec_len)
         return rec_type, rec
 
 
+    def prepare_send_tls(self, rec_type, msg):
+        tls_record = rec_type + LEGACY_TLS_VERSION + num_to_bytes(len(msg), 2) + msg
+        self.comm.prepare_send(tls_record)
+        
     def send_tls(self, rec_type, msg):
         tls_record = rec_type + LEGACY_TLS_VERSION + num_to_bytes(len(msg), 2) + msg
         self.comm.sendall(tls_record)
 
 
     def recv_tls_and_decrypt(self, key, nonce, seq_num):
         rec_type, encrypted_msg = self.recv_tls()
         assert rec_type == APPLICATION_DATA
 
         msg_type, msg = do_authenticated_decryption(key, nonce, seq_num, APPLICATION_DATA, encrypted_msg)
+        print(f"Received handshake type: {msg[0]} ({HandshakeType(msg[0]).name})")
         return msg_type, msg
 
+    def parse_extension(self, buff, offset):
+        type = bytes_to_num(buff[offset : offset + 2])
+        len = bytes_to_num(buff[offset + 2 : offset + 4])
+        value = buff[offset + 4 : offset + 4 + len]
+        
+        return type, len, value
+
 
     # PACKET GENERATORS AND HANDLERS
     def gen_client_hello(self, client_random, ecdh_pubkey_x, ecdh_pubkey_y):
         CLIENT_HELLO = b"\x01"
 
         session_id = b""
         compression_method = b"\x00"  # no compression
@@ -469,77 +566,140 @@
         print(f"    Extensions len is {extensions_length}: {num_to_bytes(extensions_length, 2).hex()}")
         print(f"    Extension parsing was skipped, but public_ec_key is {public_ec_key.hex()}")
 
         return server_random, session_id, public_ec_key_x, public_ec_key_y
 
 
     def handle_encrypted_extensions(self, msg):
-        ENCRYPTED_EXTENSIONS = 0x8
-
-        assert msg[0] == ENCRYPTED_EXTENSIONS
+        assert msg[0] == HandshakeType.ENCRYPTED_EXTENSIONS
         extensions_length = bytes_to_num(msg[1:4])
         assert len(msg[4:]) >= extensions_length
-        # ignore the rest
+        
+        offset = 4
+        extensions_length = bytes_to_num(msg[offset:offset + 2])
+        offset += 2
+        while extensions_length > 0:
+            type, length, value = self.parse_extension(msg, offset)
+            offset += length + 4
+            extensions_length -= length + 4
+            
+            print(f"        Encrypted_Extension: {ExtensionType(type).name} - {value.hex()}")
+
+            if type == ExtensionType.SERVER_CERTIFICATE_TYPE:
+                self.server_certificate_type = value[0]
+            elif type == ExtensionType.CLIENT_CERTIFICATE_TYPE:
+                self.client_certificate_type = value[0]
+
+
+    def handle_cert_request(self, cert_request_data):
+        offset = 0
+        handshake_type = cert_request_data[offset]
+        offset += 1
+
+        assert handshake_type == HandshakeType.CERTIFICATE_REQUEST
+
+        extensions_length = bytes_to_num(cert_request_data[1:4])
+        offset += 3
+        assert len(cert_request_data[4:]) >= extensions_length
+
+        self.client_certificate_ctx = b""
+        context_len = cert_request_data[offset]
+        offset += 1
+        if context_len > 0:
+            self.client_certificate_ctx = cert_request_data[offset : offset+context_len]
+            offset += context_len
+        
+        extensions_length = bytes_to_num(cert_request_data[offset:offset + 2])
+        offset += 2
+        while extensions_length > 0:
+            type, length, value = self.parse_extension(cert_request_data, offset)
+            offset += length + 4
+            extensions_length -= length + 4
+            
+            print(f"        Cert_request_extension: {ExtensionType(type).name} - {value.hex()}")
+
+            if type == ExtensionType.SIGNATURE_ALGORITHMS:
+                sig_scheme_length = bytes_to_num(value[:2])
+                pos = 0
+                while pos < sig_scheme_length:
+                    alg = bytes_to_num(value[2 + pos : 2 + pos + 2])
+                    pos += 2
+                    self.signature_algorithms.append(alg)
 
+        for alg in self.signature_algorithms:
+            print(f"            Signature_alg: {hex(alg)} ({SignatureScheme(alg).name})")
 
-    def handle_server_cert(self, server_cert_data):
-        handshake_type = server_cert_data[0]
 
-        CERTIFICATE = 0x0b
-        assert handshake_type == CERTIFICATE
+    def handle_server_cert(self, server_cert_data):
+        p = Parser(server_cert_data)
+        
+        handshake_type = p.get_uint8()
+        assert handshake_type == HandshakeType.CERTIFICATE
 
-        certificate_field_len = bytes_to_num(server_cert_data[1:4])
+        certificate_field_len = p.get_uint24()
+        assert certificate_field_len == p.bytes_left()
 
         certificates = []
 
-        cert_string_left = server_cert_data[4: 4 + certificate_field_len]
-        while cert_string_left:
-            #cert_type = cert_string_left[0]
-            _ = cert_string_left[0]
-            cert_entry_len = bytes_to_num(cert_string_left[1:4])
-
-            cert_len = bytes_to_num(cert_string_left[4:7])
-
-            certificates.append(cert_string_left[7: 7 + cert_len])
-            cert_string_left = cert_string_left[4 + cert_entry_len:]
+        cert_request_context_length = p.get_uint8()
+        if cert_request_context_length > 0:
+            # not used now
+            _ = p.get_data(cert_request_context_length)
+
+        certificate_field_len = p.get_uint24()
+
+        while p.bytes_left() > 0:
+            cert_len = p.get_uint24()
+            cert = p.get_data(cert_len)
+            print(f"cert: {cert.hex()}")
+            certificates.append(cert)
+            
+            # skip extensions
+            ext_len = p.get_uint16()
+            if ext_len > 0:
+                _ = p.get_data(ext_len)
+            
         return certificates
 
-
     def handle_cert_verify(self, cert_verify_data, rsa, msgs_so_far):
-        handshake_type = cert_verify_data[0]
-
-        CERTIFICATE_VERIFY = 0x0f
-        assert handshake_type == CERTIFICATE_VERIFY
-
-        cert_verify_len = bytes_to_num(cert_verify_data[1:4])
-        assert len(cert_verify_data[4:]) >= cert_verify_len
-
-        cert_verify_method = cert_verify_data[4:6]
-        signature_len = bytes_to_num(cert_verify_data[6:8])
-        signature = cert_verify_data[8: 8+signature_len]
+        p = Parser(cert_verify_data)
+        
+        handshake_type = p.get_uint8()
+        assert handshake_type == HandshakeType.CERTIFICATE_VERIFY
 
-        message = b" " * 64 + b"TLS 1.3, server CertificateVerify" + b"\x00" + sha256(msgs_so_far)
+        cert_verify_len = p.get_uint24()
+        assert cert_verify_len == p.bytes_left()
 
-        # try:
-        #     pss.new(rsa).verify(SHA256.new(message), signature)
-        # except ValueError:
-        #     return False
-        return True
+        algorithm = p.get_uint16()
+        print(f"        algorithm: {hex(algorithm)} ({SignatureScheme(algorithm).name})")
+        signature_len = p.get_uint16()
+        signature = p.get_data(signature_len)
+        print(f"        signature: {signature.hex()}")
+        print(f"        msgs_so_far: {msgs_so_far.hex()}")
+
+        tbs = b" " * 64 + b"TLS 1.3, server CertificateVerify" + b"\x00" + one_shot_sha256(msgs_so_far)
+
+        if algorithm == SignatureScheme.ECDSA_SECP256R1_SHA256:
+            pub_key = VerifyingKey.from_der(self.server_certs[0])
+            valid = pub_key.verify(signature, tbs, sha256, sigdecode=sigdecode_der)
+            return valid
+        else:
+            # not implemented
+            return True
 
 
     def handle_finished(self, finished_data, server_finished_key, msgs_so_far):
         handshake_type = finished_data[0]
 
-        FINISHED = 0x14
-        assert handshake_type == FINISHED
+        assert handshake_type == HandshakeType.FINISHED
 
         verify_data_len = bytes_to_num(finished_data[1:4])
         verify_data = finished_data[4:4+verify_data_len]
 
-        hmac_digest = hmac_sha256(server_finished_key, sha256(msgs_so_far))
+        hmac_digest = hmac_sha256(server_finished_key, one_shot_sha256(msgs_so_far))
         return verify_data == hmac_digest
 
 
     def gen_change_cipher(self):
         CHANGE_CIPHER_SPEC_MSG = b"\x01"
         return CHANGE_CIPHER_SPEC_MSG
 
@@ -547,14 +707,20 @@
     def gen_encrypted_finished(self, client_write_key, client_write_iv, client_seq_num, client_finish_val):
         FINISHED = b"\x14"
         msg = FINISHED + num_to_bytes(len(client_finish_val), 3) + client_finish_val
 
         return do_authenticated_encryption(client_write_key, client_write_iv, client_seq_num,
                                         HANDSHAKE, msg)
 
+    def generate_client_key(self):
+        self.client_key = SigningKey.generate(curve=NIST256p)
+        pub_key = self.client_key.verifying_key.to_string()
+        return pub_key[0:32], pub_key[32:64]
+
+
     def establish(self):
         print("Generating params for a client hello, the first message of TLS handshake")
         SECP256R1_P = 0xffffffff00000001000000000000000000000000ffffffffffffffffffffffff
         SECP256R1_A = 0xffffffff00000001000000000000000000000000fffffffffffffffffffffffc
         SECP256R1_G = (0x6b17d1f2e12c4247f8bce6e563a440f277037d812deb33a0f4a13945d898c296,
                     0x4fe342e2fe1a7f9b8ee7eb4a7c0f9e162bce33576b315ececbb6406837bf51f5)
 
@@ -588,23 +754,26 @@
         print(f"    Server ECDH public key: x={server_ecdh_pubkey_x} y={server_ecdh_pubkey_y}")
 
         ###########################
         print("Receiving a change cipher msg, all communication will be encrypted")
         rec_type, server_change_cipher = self.recv_tls()
         assert rec_type == CHANGE_CIPHER
 
+        self.server_ecdh_pubkey_x = server_ecdh_pubkey_x
+        self.server_ecdh_pubkey_y = server_ecdh_pubkey_y
+
         our_secret_point_x = multiply_num_on_ec_point(our_ecdh_privkey, server_ecdh_pubkey_x, server_ecdh_pubkey_y,
                                                     SECP256R1_A, SECP256R1_P)[0]
         our_secret = num_to_bytes(our_secret_point_x, 32)
         print(f"    Our common ECDH secret is: {our_secret.hex()}, deriving keys")
 
         early_secret = hmac_sha256(key=b"", data=b"\x00" * 32)
-        preextractsec = derive_secret(b"derived", key=early_secret, data=sha256(b""), hash_len=32)
+        preextractsec = derive_secret(b"derived", key=early_secret, data=one_shot_sha256(b""), hash_len=32)
         handshake_secret = hmac_sha256(key=preextractsec, data=our_secret)
-        hello_hash = sha256(client_hello + server_hello)
+        hello_hash = one_shot_sha256(client_hello + server_hello)
         server_hs_secret = derive_secret(b"s hs traffic", key=handshake_secret, data=hello_hash, hash_len=32)
         server_write_key = derive_secret(b"key", key=server_hs_secret, data=b"", hash_len=16)
         server_write_iv = derive_secret(b"iv", key=server_hs_secret, data=b"", hash_len=12)
         server_finished_key = derive_secret(b"finished", key=server_hs_secret, data=b"", hash_len=32)
         client_hs_secret = derive_secret(b"c hs traffic", key=handshake_secret, data=hello_hash, hash_len=32)
         client_write_key = derive_secret(b"key", key=client_hs_secret, data=b"", hash_len=16)
         client_write_iv = derive_secret(b"iv", key=client_hs_secret, data=b"", hash_len=12)
@@ -620,72 +789,92 @@
 
         ###########################
         print("Receiving encrypted extensions")
         rec_type, encrypted_extensions = self.recv_tls_and_decrypt(server_write_key, server_write_iv, server_seq_num)
         assert rec_type == HANDSHAKE
         server_seq_num += 1
 
-        print(f"    Encrypted_extensions: {encrypted_extensions.hex()}, parsing skipped")
+        print(f"    Encrypted_extensions: {encrypted_extensions.hex()}")
         self.handle_encrypted_extensions(encrypted_extensions)
 
+        msgs_so_far = client_hello + server_hello + encrypted_extensions
+
         ###########################
         print("Receiving server certificates")
         rec_type, server_cert = self.recv_tls_and_decrypt(server_write_key, server_write_iv, server_seq_num)
         assert rec_type == HANDSHAKE
         server_seq_num += 1
 
-        certs = self.handle_server_cert(server_cert)
-        print(f"    Got {len(certs)} certs")
+        if server_cert[0] == HandshakeType.CERTIFICATE_REQUEST:
+            print(f"    Certificate_request: {server_cert.hex()}")
+
+            self.handle_cert_request(server_cert)
+            
+            msgs_so_far = msgs_so_far + server_cert
+            
+            rec_type, server_cert = self.recv_tls_and_decrypt(server_write_key, server_write_iv, server_seq_num)
+            assert rec_type == HANDSHAKE
+            server_seq_num += 1
+
+        print(f"    Certificate: {server_cert.hex()}")
+
+        self.server_certs = self.handle_server_cert(server_cert)
+        print(f"    Got {len(self.server_certs)} certs")
+
+        msgs_so_far = msgs_so_far + server_cert
 
         ###########################
         print("Receiving server verify certificate")
         rec_type, cert_verify = self.recv_tls_and_decrypt(server_write_key, server_write_iv, server_seq_num)
         assert rec_type == HANDSHAKE
         server_seq_num += 1
 
-        msgs_so_far = client_hello + server_hello + encrypted_extensions + server_cert
+        print(f"    Certificate_verify: {cert_verify.hex()}")
+
         cert_ok = self.handle_cert_verify(cert_verify, None, msgs_so_far)
-        print("    Certificate verifying skipped")
+        print(f"    Certificate verifying ststus: {cert_ok}")
+        if not cert_ok:
+            raise Exception("Unable to verify server certificate!") 
 
         ###########################
         print("Receiving server finished")
         rec_type, finished = self.recv_tls_and_decrypt(server_write_key, server_write_iv, server_seq_num)
         assert rec_type == HANDSHAKE
         server_seq_num += 1
 
         msgs_so_far = msgs_so_far + cert_verify
         srv_finish_ok = self.handle_finished(finished, server_finished_key, msgs_so_far)
-        if not srv_finish_ok:
+        if srv_finish_ok:
             print("    Server sent valid finish handshake msg")
         else:
             print("    Warning: Server sent wrong handshake finished msg")
 
         ###########################
         print("Handshake: sending a change cipher msg")
-        self.send_tls(CHANGE_CIPHER, self.gen_change_cipher())
+        self.prepare_send_tls(CHANGE_CIPHER, self.gen_change_cipher())
 
         ###########################
         # All client messages beyond this point are encrypted
         msgs_so_far = msgs_so_far + finished
-        msgs_sha256 = sha256(msgs_so_far)
+        msgs_sha256 = one_shot_sha256(msgs_so_far)
         client_finish_val = hmac_sha256(client_finished_key, msgs_sha256)
 
         print("Handshake: sending an encrypted finished msg")
         encrypted_hangshake_msg = self.gen_encrypted_finished(client_write_key, client_write_iv, client_seq_num,
                                                         client_finish_val)
         print(f"    Client finish value {client_finish_val.hex()}")
         self.send_tls(APPLICATION_DATA, encrypted_hangshake_msg)
         client_seq_num += 1
 
         print("Handshake finished, regenerating secrets for application data")
 
         ###########################
         # rederive application secrets
-        msgs_so_far_hash = sha256(msgs_so_far)
-        premaster_secret = derive_secret(b"derived", data=sha256(b""), key=handshake_secret, hash_len=32)
+        msgs_so_far_hash = one_shot_sha256(msgs_so_far)
+        premaster_secret = derive_secret(b"derived", data=one_shot_sha256(b""), key=handshake_secret, hash_len=32)
         master_secret = hmac_sha256(key=premaster_secret, data=b"\x00" * 32)
         server_secret = derive_secret(b"s ap traffic", data=msgs_so_far_hash, key=master_secret, hash_len=32)
         self.server_write_key = derive_secret(b"key", data=b"", key=server_secret, hash_len=16)
         self.server_write_iv = derive_secret(b"iv", data=b"", key=server_secret, hash_len=12)
         client_secret = derive_secret(b"c ap traffic", data=msgs_so_far_hash, key=master_secret, hash_len=32)
         self.client_write_key = derive_secret(b"key", data=b"", key=client_secret, hash_len=16)
         self.client_write_iv = derive_secret(b"iv", data=b"", key=client_secret, hash_len=12)
```

### Comparing `manual_tls-0.0.1/.gitignore` & `manual_tls-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `manual_tls-0.0.1/LICENSE` & `manual_tls-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `manual_tls-0.0.1/README.md` & `manual_tls-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `manual_tls-0.0.1/pyproject.toml` & `manual_tls-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "manual_tls"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Alexander Bersenev / Adam Augustyn", email="watsug@gmail.com" },
 ]
 description = "A tiny TLS 1.3 pure Python implementation"
 readme = "README.md"
 requires-python = ">=3.8"
+dependencies = [
+  "ecdsa"
+]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `manual_tls-0.0.1/PKG-INFO` & `manual_tls-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.3
 Name: manual_tls
-Version: 0.0.1
+Version: 0.0.2
 Summary: A tiny TLS 1.3 pure Python implementation
 Project-URL: Homepage, https://github.com/watsug/manual-tls
 Project-URL: Issues, https://github.com/watsug/manual-tls
 Author-email: Alexander Bersenev / Adam Augustyn <watsug@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
+Requires-Dist: ecdsa
 Description-Content-Type: text/markdown
 
 # Manual TLS #
 
 Makes HTTPS connection with TLS 1.3 in 100% Python. The only used import is
 **socket**! All required crypto algorithms are implemented manually in a
 single file.
```

