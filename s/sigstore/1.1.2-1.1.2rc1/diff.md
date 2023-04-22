# Comparing `tmp/sigstore-1.1.2.tar.gz` & `tmp/sigstore-1.1.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigstore-1.1.2.tar", last modified: Sat Apr 22 22:26:08 2023, max compression
+gzip compressed data, was "sigstore-1.1.2rc1.tar", last modified: Wed Mar 15 21:25:46 2023, max compression
```

## Comparing `sigstore-1.1.2.tar` & `sigstore-1.1.2rc1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    11358 2023-04-22 22:25:55.252449 sigstore-1.1.2/LICENSE
--rw-r--r--   0        0        0    20574 2023-04-22 22:25:55.252449 sigstore-1.1.2/README.md
--rw-r--r--   0        0        0     4125 2023-04-22 22:25:55.256449 sigstore-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      955 2023-04-22 22:25:55.256449 sigstore-1.1.2/sigstore/__init__.py
--rw-r--r--   0        0        0      726 2023-04-22 22:25:55.256449 sigstore-1.1.2/sigstore/__main__.py
--rw-r--r--   0        0        0    34542 2023-04-22 22:25:55.256449 sigstore-1.1.2/sigstore/_cli.py
--rw-r--r--   0        0        0      738 2023-04-22 22:25:55.256449 sigstore-1.1.2/sigstore/_internal/__init__.py
--rw-r--r--   0        0        0      774 2023-04-22 22:25:55.256449 sigstore-1.1.2/sigstore/_internal/ctfe.py
--rw-r--r--   0        0        0      833 2023-04-22 22:25:55.256449 sigstore-1.1.2/sigstore/_internal/fulcio/__init__.py
--rw-r--r--   0        0        0    11677 2023-04-22 22:25:55.256449 sigstore-1.1.2/sigstore/_internal/fulcio/client.py
--rw-r--r--   0        0        0     3891 2023-04-22 22:25:55.256449 sigstore-1.1.2/sigstore/_internal/keyring.py
--rw-r--r--   0        0        0     4544 2023-04-22 22:25:55.256449 sigstore-1.1.2/sigstore/_internal/merkle.py
--rw-r--r--   0        0        0     2576 2023-04-22 22:25:55.256449 sigstore-1.1.2/sigstore/_internal/oidc/__init__.py
--rw-r--r--   0        0        0    15958 2023-04-22 22:25:55.256449 sigstore-1.1.2/sigstore/_internal/oidc/oauth.py
--rw-r--r--   0        0        0      687 2023-04-22 22:25:55.256449 sigstore-1.1.2/sigstore/_internal/rekor/__init__.py
--rw-r--r--   0        0        0     9313 2023-04-22 22:25:55.256449 sigstore-1.1.2/sigstore/_internal/rekor/client.py
--rw-r--r--   0        0        0     9162 2023-04-22 22:25:55.256449 sigstore-1.1.2/sigstore/_internal/sct.py
--rw-r--r--   0        0        0     1513 2023-04-22 22:25:55.256449 sigstore-1.1.2/sigstore/_internal/set.py
--rw-r--r--   0        0        0    11045 2023-04-22 22:25:55.256449 sigstore-1.1.2/sigstore/_internal/tuf.py
--rw-r--r--   0        0        0     1247 2023-04-22 22:25:55.256449 sigstore-1.1.2/sigstore/_store/__init__.py
--rw-r--r--   0        0        0     6388 2023-04-22 22:25:55.256449 sigstore-1.1.2/sigstore/_store/root.json
--rw-r--r--   0        0        0     1876 2023-04-22 22:25:55.256449 sigstore-1.1.2/sigstore/_store/staging-root.json
--rw-r--r--   0        0        0     5171 2023-04-22 22:25:55.256449 sigstore-1.1.2/sigstore/_utils.py
--rw-r--r--   0        0        0     2874 2023-04-22 22:25:55.256449 sigstore-1.1.2/sigstore/errors.py
--rw-r--r--   0        0        0     8120 2023-04-22 22:25:55.256449 sigstore-1.1.2/sigstore/oidc.py
--rw-r--r--   0        0        0     8732 2023-04-22 22:25:55.256449 sigstore-1.1.2/sigstore/sign.py
--rw-r--r--   0        0        0     4679 2023-04-22 22:25:55.256449 sigstore-1.1.2/sigstore/transparency.py
--rw-r--r--   0        0        0     1932 2023-04-22 22:25:55.256449 sigstore-1.1.2/sigstore/verify/__init__.py
--rw-r--r--   0        0        0    10469 2023-04-22 22:25:55.256449 sigstore-1.1.2/sigstore/verify/models.py
--rw-r--r--   0        0        0     9824 2023-04-22 22:25:55.256449 sigstore-1.1.2/sigstore/verify/policy.py
--rw-r--r--   0        0        0    10444 2023-04-22 22:25:55.256449 sigstore-1.1.2/sigstore/verify/verifier.py
--rw-r--r--   0        0        0    22860 1970-01-01 00:00:00.000000 sigstore-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-03-15 21:25:33.169977 sigstore-1.1.2rc1/LICENSE
+-rw-r--r--   0        0        0    20574 2023-03-15 21:25:33.169977 sigstore-1.1.2rc1/README.md
+-rw-r--r--   0        0        0     4125 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/pyproject.toml
+-rw-r--r--   0        0        0      958 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/__init__.py
+-rw-r--r--   0        0        0      726 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/__main__.py
+-rw-r--r--   0        0        0    34542 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/_cli.py
+-rw-r--r--   0        0        0      738 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/_internal/__init__.py
+-rw-r--r--   0        0        0      774 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/_internal/ctfe.py
+-rw-r--r--   0        0        0      833 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/_internal/fulcio/__init__.py
+-rw-r--r--   0        0        0    11677 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/_internal/fulcio/client.py
+-rw-r--r--   0        0        0     3395 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/_internal/keyring.py
+-rw-r--r--   0        0        0     4544 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/_internal/merkle.py
+-rw-r--r--   0        0        0     2576 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/_internal/oidc/__init__.py
+-rw-r--r--   0        0        0    15958 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/_internal/oidc/oauth.py
+-rw-r--r--   0        0        0      687 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/_internal/rekor/__init__.py
+-rw-r--r--   0        0        0     9313 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/_internal/rekor/client.py
+-rw-r--r--   0        0        0     8229 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/_internal/sct.py
+-rw-r--r--   0        0        0     1513 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/_internal/set.py
+-rw-r--r--   0        0        0     7790 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/_internal/tuf.py
+-rw-r--r--   0        0        0     1247 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/_store/__init__.py
+-rw-r--r--   0        0        0     6388 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/_store/root.json
+-rw-r--r--   0        0        0     2482 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/_store/staging-root.json
+-rw-r--r--   0        0        0     4481 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/_utils.py
+-rw-r--r--   0        0        0     2874 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/errors.py
+-rw-r--r--   0        0        0     8054 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/oidc.py
+-rw-r--r--   0        0        0     8732 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/sign.py
+-rw-r--r--   0        0        0     4679 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/transparency.py
+-rw-r--r--   0        0        0     1932 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/verify/__init__.py
+-rw-r--r--   0        0        0    10469 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/verify/models.py
+-rw-r--r--   0        0        0     9824 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/verify/policy.py
+-rw-r--r--   0        0        0    10444 2023-03-15 21:25:33.173977 sigstore-1.1.2rc1/sigstore/verify/verifier.py
+-rw-r--r--   0        0        0    22863 1970-01-01 00:00:00.000000 sigstore-1.1.2rc1/PKG-INFO
```

### Comparing `sigstore-1.1.2/LICENSE` & `sigstore-1.1.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `sigstore-1.1.2/README.md` & `sigstore-1.1.2rc1/README.md`

 * *Files identical despite different names*

### Comparing `sigstore-1.1.2/pyproject.toml` & `sigstore-1.1.2rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
   "bandit",
   "black",
   "isort",
   "interrogate",
   "mypy ~= 1.1",
   # NOTE(ww): ruff is under active development, so we pin conservatively here
   # and let Dependabot periodically perform this update.
-  "ruff < 0.0.262",
+  "ruff < 0.0.256",
   "types-requests",
   # Needed for protocol typing in 3.7; remove when our minimum Python is 3.8.
   "typing-extensions; python_version < '3.8'",
   # TODO(ww): Re-enable once dependency on types-cryptography is dropped.
   # See: https://github.com/python/typeshed/issues/8699
   # "types-pyOpenSSL",
 ]
```

### Comparing `sigstore-1.1.2/sigstore/__init__.py` & `sigstore-1.1.2rc1/sigstore/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 Otherwise, here are some quick starting points:
 
 * `sigstore.verify`: verifying of Sigstore signatures,
   including flexible policy control
 * `sigstore.sign`: creation of Sigstore signatures
 """
 
-__version__ = "1.1.2"
+__version__ = "1.1.2rc1"
```

### Comparing `sigstore-1.1.2/sigstore/__main__.py` & `sigstore-1.1.2rc1/sigstore/__main__.py`

 * *Files identical despite different names*

### Comparing `sigstore-1.1.2/sigstore/_cli.py` & `sigstore-1.1.2rc1/sigstore/_cli.py`

 * *Files identical despite different names*

### Comparing `sigstore-1.1.2/sigstore/_internal/__init__.py` & `sigstore-1.1.2rc1/sigstore/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstore-1.1.2/sigstore/_internal/ctfe.py` & `sigstore-1.1.2rc1/sigstore/_internal/ctfe.py`

 * *Files identical despite different names*

### Comparing `sigstore-1.1.2/sigstore/_internal/fulcio/__init__.py` & `sigstore-1.1.2rc1/sigstore/_internal/fulcio/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstore-1.1.2/sigstore/_internal/fulcio/client.py` & `sigstore-1.1.2rc1/sigstore/_internal/fulcio/client.py`

 * *Files identical despite different names*

### Comparing `sigstore-1.1.2/sigstore/_internal/keyring.py` & `sigstore-1.1.2rc1/sigstore/_internal/keyring.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,22 +20,15 @@
 from typing import List
 
 import cryptography.hazmat.primitives.asymmetric.padding as padding
 from cryptography.exceptions import InvalidSignature
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.asymmetric import ec, rsa
 
-from sigstore._utils import (
-    InvalidKeyError,
-    KeyID,
-    UnexpectedKeyFormatError,
-    key_id,
-    load_der_public_key,
-    load_pem_public_key,
-)
+from sigstore._utils import KeyID, key_id, load_pem_public_key
 
 
 class KeyringError(Exception):
     """
     Raised on failure by `Keyring.verify()`.
     """
 
@@ -47,44 +40,30 @@
     A specialization of `KeyringError`, indicating that the specified
     key ID wasn't found in the keyring.
     """
 
     pass
 
 
-class KeyringSignatureError(KeyringError):
-    """
-    Raised when `Keyring.verify()` is passed an invalid signature.
-    """
-
-
 class Keyring:
     """
     Represents a set of CT signing keys, each of which is a potentially
     valid signer for a Signed Certificate Timestamp (SCT).
 
     This structure exists to facilitate key rotation in a CT log.
     """
 
     def __init__(self, keys: List[bytes] = []):
         """
         Create a new `Keyring`, with `keys` as the initial set of signing
-        keys. These `keys` can be in either DER format or PEM encoded.
+        keys.
         """
         self._keyring = {}
         for key_bytes in keys:
-            key = None
-
-            try:
-                key = load_pem_public_key(key_bytes)
-            except UnexpectedKeyFormatError as e:
-                raise e
-            except InvalidKeyError:
-                key = load_der_public_key(key_bytes)
-
+            key = load_pem_public_key(key_bytes)
             self._keyring[key_id(key)] = key
 
     def add(self, key_pem: bytes) -> None:
         """
         Adds a PEM-encoded key to the current keyring.
         """
         key = load_pem_public_key(key_pem)
@@ -118,8 +97,8 @@
                     data=data,
                     signature_algorithm=ec.ECDSA(hashes.SHA256()),
                 )
             else:
                 # NOTE(ww): Unreachable without API misuse.
                 raise KeyringError(f"unsupported key type: {key}")
         except InvalidSignature as exc:
-            raise KeyringSignatureError("invalid signature") from exc
+            raise KeyringError("invalid signature") from exc
```

### Comparing `sigstore-1.1.2/sigstore/_internal/merkle.py` & `sigstore-1.1.2rc1/sigstore/_internal/merkle.py`

 * *Files identical despite different names*

### Comparing `sigstore-1.1.2/sigstore/_internal/oidc/__init__.py` & `sigstore-1.1.2rc1/sigstore/_internal/oidc/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstore-1.1.2/sigstore/_internal/oidc/oauth.py` & `sigstore-1.1.2rc1/sigstore/_internal/oidc/oauth.py`

 * *Files identical despite different names*

### Comparing `sigstore-1.1.2/sigstore/_internal/rekor/__init__.py` & `sigstore-1.1.2rc1/sigstore/_internal/rekor/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstore-1.1.2/sigstore/_internal/rekor/client.py` & `sigstore-1.1.2rc1/sigstore/_internal/rekor/client.py`

 * *Files identical despite different names*

### Comparing `sigstore-1.1.2/sigstore/_internal/sct.py` & `sigstore-1.1.2rc1/sigstore/_internal/sct.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,19 +28,15 @@
 from cryptography.x509.certificate_transparency import (
     LogEntryType,
     SignedCertificateTimestamp,
 )
 from cryptography.x509.oid import ExtendedKeyUsageOID
 
 from sigstore._internal.ctfe import CTKeyring
-from sigstore._internal.keyring import (
-    KeyringError,
-    KeyringLookupError,
-    KeyringSignatureError,
-)
+from sigstore._internal.keyring import KeyringError, KeyringLookupError
 from sigstore._utils import DERCert, KeyID, key_id
 from sigstore.errors import Error
 
 logger = logging.getLogger(__name__)
 
 
 def _pack_signed_entry(
@@ -142,76 +138,36 @@
 class InvalidSCTError(Error):
     """
     Raised during SCT verification if an SCT is invalid in some way.
     """
 
     def diagnostics(self) -> str:
         """Returns diagnostics for the error."""
-
-        ctx = f"\nContext: {self.__context__}" if self.__context__ else ""
-        return dedent(
-            f"""
-            SCT verification failed.
-
-            Additional context:
-
-            Message: {str(self)}
-            """
-            + ctx
-        )
-
-
-class InvalidSCTKeyError(InvalidSCTError):
-    """
-    Raised during SCT verification if the SCT can't be validated against the given keyring.
-
-    We specialize this error case, since it usually indicates one of
-    two conditions: either the current sigstore client is out-of-date,
-    or that the SCT is well-formed but invalid for the current configuration
-    (indicating that the user has asked for the wrong instance).
-    """
-
-    def diagnostics(self) -> str:
-        """Returns diagnostics for the error."""
-        return dedent(
-            f"""
+        # We specialize this error case, since it usually indicates one of
+        # two conditions: either the current sigstore client is out-of-date,
+        # or that the SCT is well-formed but invalid for the current configuration
+        # (indicating that the user has asked for the wrong instance).
+        if isinstance(self.__cause__, KeyringLookupError):
+            return dedent(
+                f"""
                 Invalid key ID in SCT: not found in current keyring.
 
                 This may be a result of an outdated `sigstore` installation.
 
                 Consider upgrading with:
 
                     python -m pip install --upgrade sigstore
 
                 Additional context:
 
                 {self.__cause__}
                 """
-        )
-
-
-class SCTSignatureError(InvalidSCTError):
-    """
-    Raised during SCT verification if the signature of the SCT is invalid.
-    """
-
-    def diagnostics(self) -> str:
-        """Returns diagnostics for the error."""
-        return dedent(
-            f"""
-            Invalid signature on SCT.
-
-            If validating a certificate, the certificate associated with this
-            SCT should not be trusted.
-
-            Additional context:
+            )
 
-            {self.__cause__}
-            """
-        )
+        return str(self)
 
 
 def verify_sct(
     sct: SignedCertificateTimestamp,
     cert: Certificate,
     chain: List[Certificate],
     ct_keyring: CTKeyring,
@@ -254,12 +210,12 @@
         # singular `opaque key_id[32]`. Cryptography's APIs don't bother
         # to expose this trivial single member, so we use the `log_id`
         # attribute directly.
         ct_keyring.verify(
             key_id=KeyID(sct.log_id), signature=sct.signature, data=digitally_signed
         )
     except KeyringLookupError as exc:
-        raise InvalidSCTKeyError from exc
-    except KeyringSignatureError as exc:
-        raise SCTSignatureError from exc
+        raise InvalidSCTError(
+            "Invalid key ID in SCT: not found in current keyring"
+        ) from exc
     except KeyringError as exc:
         raise InvalidSCTError from exc
```

### Comparing `sigstore-1.1.2/sigstore/_internal/set.py` & `sigstore-1.1.2rc1/sigstore/_internal/set.py`

 * *Files identical despite different names*

### Comparing `sigstore-1.1.2/sigstore/_store/__init__.py` & `sigstore-1.1.2rc1/sigstore/_store/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstore-1.1.2/sigstore/_store/root.json` & `sigstore-1.1.2rc1/sigstore/_store/root.json`

 * *Files identical despite different names*

### Comparing `sigstore-1.1.2/sigstore/_utils.py` & `sigstore-1.1.2rc1/sigstore/_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,16 +23,14 @@
 import sys
 from typing import IO, NewType, Union
 
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric import ec, rsa
 from cryptography.x509 import Certificate
 
-from sigstore.errors import Error
-
 if sys.version_info < (3, 11):
     import importlib_resources as resources
 else:
     from importlib import resources
 
 
 PublicKey = Union[rsa.RSAPublicKey, ec.EllipticCurvePublicKey]
@@ -55,60 +53,36 @@
 """
 KeyID = NewType("KeyID", bytes)
 """
 A newtype for `bytes` objects that contain a key id.
 """
 
 
-class InvalidKeyError(Error):
+class InvalidKey(Exception):
     """
     Raised when loading a key fails.
     """
 
     pass
 
 
-class UnexpectedKeyFormatError(InvalidKeyError):
-    """
-    Raised when loading a key produces a key of an unexpected type.
-    """
-
-    pass
-
-
 def load_pem_public_key(key_pem: bytes) -> PublicKey:
     """
     A specialization of `cryptography`'s `serialization.load_pem_public_key`
-    with a uniform exception type (`InvalidKeyError`) and additional restrictions
+    with a uniform exception type (`InvalidKey`) and additional restrictions
     on key validity (only RSA and ECDSA keys are valid).
     """
 
     try:
         key = serialization.load_pem_public_key(key_pem)
     except Exception as exc:
-        raise InvalidKeyError("could not load PEM-formatted public key") from exc
-
-    if not isinstance(key, (rsa.RSAPublicKey, ec.EllipticCurvePublicKey)):
-        raise UnexpectedKeyFormatError(f"invalid key format (not ECDSA or RSA): {key}")
-
-    return key
-
-
-def load_der_public_key(key_der: bytes) -> PublicKey:
-    """
-    The `load_pem_public_key` specialization, but DER.
-    """
-
-    try:
-        key = serialization.load_der_public_key(key_der)
-    except Exception as exc:
-        raise InvalidKeyError("could not load DER-formatted public key") from exc
+        raise InvalidKey("could not load PEM-formatted public key") from exc
 
     if not isinstance(key, (rsa.RSAPublicKey, ec.EllipticCurvePublicKey)):
-        raise UnexpectedKeyFormatError(f"invalid key format (not ECDSA or RSA): {key}")
+        raise InvalidKey(f"invalid key format (not ECDSA or RSA): {key}")
 
     return key
 
 
 def base64_encode_pem_cert(cert: Certificate) -> B64Str:
     """
     Returns a string containing a base64-encoded PEM-encoded X.509 certificate.
```

### Comparing `sigstore-1.1.2/sigstore/errors.py` & `sigstore-1.1.2rc1/sigstore/errors.py`

 * *Files identical despite different names*

### Comparing `sigstore-1.1.2/sigstore/oidc.py` & `sigstore-1.1.2rc1/sigstore/oidc.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 API for retrieving OIDC tokens.
 """
 
 from __future__ import annotations
 
 import logging
 import os
-import sys
 import time
 import urllib.parse
 import webbrowser
 from typing import NoReturn, Optional, cast
 
 import id
 import requests
@@ -122,20 +121,19 @@
 
         force_oob = os.getenv("SIGSTORE_OAUTH_FORCE_OOB") is not None
 
         code: str
         with _OAuthFlow(client_id, client_secret, self) as server:
             # Launch web browser
             if not force_oob and webbrowser.open(server.base_uri):
-                print("Waiting for browser interaction...", file=sys.stderr)
+                print("Waiting for browser interaction...")
             else:
                 server.enable_oob()
                 print(
-                    f"Go to the following link in a browser:\n\n\t{server.auth_endpoint}",
-                    file=sys.stderr,
+                    f"Go to the following link in a browser:\n\n\t{server.auth_endpoint}"
                 )
 
             if not server.is_oob():
                 # Wait until the redirect server populates the response
                 while server.auth_response is None:
                     time.sleep(0.1)
```

### Comparing `sigstore-1.1.2/sigstore/sign.py` & `sigstore-1.1.2rc1/sigstore/sign.py`

 * *Files identical despite different names*

### Comparing `sigstore-1.1.2/sigstore/transparency.py` & `sigstore-1.1.2rc1/sigstore/transparency.py`

 * *Files identical despite different names*

### Comparing `sigstore-1.1.2/sigstore/verify/__init__.py` & `sigstore-1.1.2rc1/sigstore/verify/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstore-1.1.2/sigstore/verify/models.py` & `sigstore-1.1.2rc1/sigstore/verify/models.py`

 * *Files identical despite different names*

### Comparing `sigstore-1.1.2/sigstore/verify/policy.py` & `sigstore-1.1.2rc1/sigstore/verify/policy.py`

 * *Files identical despite different names*

### Comparing `sigstore-1.1.2/sigstore/verify/verifier.py` & `sigstore-1.1.2rc1/sigstore/verify/verifier.py`

 * *Files identical despite different names*

### Comparing `sigstore-1.1.2/PKG-INFO` & `sigstore-1.1.2rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigstore
-Version: 1.1.2
+Version: 1.1.2rc1
 Summary: A tool for signing Python package distributions
 Author-email: Sigstore Authors <sigstore-dev@googlegroups.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
@@ -33,15 +33,15 @@
 Requires-Dist: sigstore[doc,test,lint] ; extra == "dev"
 Requires-Dist: pdoc ; extra == "doc"
 Requires-Dist: bandit ; extra == "lint"
 Requires-Dist: black ; extra == "lint"
 Requires-Dist: isort ; extra == "lint"
 Requires-Dist: interrogate ; extra == "lint"
 Requires-Dist: mypy ~= 1.1 ; extra == "lint"
-Requires-Dist: ruff < 0.0.262 ; extra == "lint"
+Requires-Dist: ruff < 0.0.256 ; extra == "lint"
 Requires-Dist: types-requests ; extra == "lint"
 Requires-Dist: typing-extensions ; extra == "lint" and ( python_version < '3.8')
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: pretend ; extra == "test"
 Requires-Dist: coverage[toml] ; extra == "test"
 Project-URL: Documentation, https://sigstore.github.io/sigstore-python/
```

