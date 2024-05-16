# Comparing `tmp/pypi_attestation_models-0.0.1rc2.tar.gz` & `tmp/pypi_attestation_models-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypi_attestation_models-0.0.1rc2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pypi_attestation_models-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pypi_attestation_models-0.0.1rc2.tar` & `pypi_attestation_models-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    10174 2024-05-08 12:07:00.973304 pypi_attestation_models-0.0.1rc2/LICENSE
--rw-r--r--   0        0        0     2892 2024-05-08 12:07:00.973304 pypi_attestation_models-0.0.1rc2/README.md
--rw-r--r--   0        0        0     2766 2024-05-08 12:07:00.973304 pypi_attestation_models-0.0.1rc2/pyproject.toml
--rw-r--r--   0        0        0      545 2024-05-08 12:07:00.973304 pypi_attestation_models-0.0.1rc2/src/pypi_attestation_models/__init__.py
--rw-r--r--   0        0        0     5886 2024-05-08 12:07:00.973304 pypi_attestation_models-0.0.1rc2/src/pypi_attestation_models/_impl.py
--rw-r--r--   0        0        0        0 2024-05-08 12:07:00.973304 pypi_attestation_models-0.0.1rc2/src/pypi_attestation_models/py.typed
--rw-r--r--   0        0        0     4434 1970-01-01 00:00:00.000000 pypi_attestation_models-0.0.1rc2/PKG-INFO
+-rw-r--r--   0        0        0    10174 2024-05-16 16:54:49.294142 pypi_attestation_models-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2939 2024-05-16 16:54:49.294142 pypi_attestation_models-0.0.2/README.md
+-rw-r--r--   0        0        0     2763 2024-05-16 16:54:49.294142 pypi_attestation_models-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      542 2024-05-16 16:54:49.294142 pypi_attestation_models-0.0.2/src/pypi_attestation_models/__init__.py
+-rw-r--r--   0        0        0     6092 2024-05-16 16:54:49.294142 pypi_attestation_models-0.0.2/src/pypi_attestation_models/_impl.py
+-rw-r--r--   0        0        0        0 2024-05-16 16:54:49.294142 pypi_attestation_models-0.0.2/src/pypi_attestation_models/py.typed
+-rw-r--r--   0        0        0     4475 1970-01-01 00:00:00.000000 pypi_attestation_models-0.0.2/PKG-INFO
```

### Comparing `pypi_attestation_models-0.0.1rc2/LICENSE` & `pypi_attestation_models-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pypi_attestation_models-0.0.1rc2/README.md` & `pypi_attestation_models-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 <!--- BADGES: START --->
 [![CI](https://github.com/trailofbits/pypi-attestation-models/actions/workflows/tests.yml/badge.svg)](https://github.com/trailofbits/pypi-attestation-models/actions/workflows/tests.yml)
 [![PyPI version](https://badge.fury.io/py/pypi-attestation-models.svg)](https://pypi.org/project/pypi-attestation-models)
 [![Packaging status](https://repology.org/badge/tiny-repos/python:pypi-attestation-models.svg)](https://repology.org/project/python:pypi-attestation-models/versions)
 <!--- BADGES: END --->
 
-A library to convert between Sigstore Bundles and PEP-740 Attestation objects
+A library to convert between Sigstore Bundles and [PEP 740] Attestation objects
 
 ## Installation
 
 ```bash
 python -m pip install pypi-attestation-models
 ```
 
 ## Usage
 
 See the full API documentation [here].
 
-
 ### Signing and verification
+
 Use these APIs to create a PEP 740-compliant `Attestation` object by signing a Python artifact
 (i.e: sdist or wheel files), and to verify an `Attestation` object against a Python artifact.
 
 ```python
 from pathlib import Path
 
 from pypi_attestation_models import Attestation, AttestationPayload
@@ -44,15 +44,14 @@
 
 # Verify an attestation against a Python artifact
 attestation_path = Path("test_package-0.0.1-py3-none-any.whl.attestation")
 attestation = Attestation.model_validate_json(attestation_path.read_bytes())
 verifier = Verifier.production()
 policy = policy.Identity(identity="example@gmail.com", issuer="https://accounts.google.com")
 attestation.verify(verifier, policy, attestation_path)
-
 ```
 
 ### Low-level model conversions
 These conversions assume that any Sigstore Bundle used as an input was created
 by signing an `AttestationPayload` object.
 ```python
 from pathlib import Path
@@ -71,8 +70,10 @@
 attestation_path = Path("attestation.json")
 with attestation_path.open("rb") as f:
     attestation = Attestation.model_validate_json(f.read())
 bundle = pypi_to_sigstore(attestation)
 print(bundle.to_json())
 ```
 
+[PEP 740]: https://peps.python.org/pep-0740/
+
 [here]: https://trailofbits.github.io/pypi-attestation-models
```

### Comparing `pypi_attestation_models-0.0.1rc2/pyproject.toml` & `pypi_attestation_models-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 authors = [
     { name = "Trail of Bits", email = "opensource@trailofbits.com" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
 ]
-dependencies = ["cryptography", "pydantic", "sigstore==3.0.0rc2"]
+dependencies = ["cryptography", "pydantic", "sigstore~=3.0.0"]
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 doc = ["pdoc"]
 test = ["pytest", "pytest-cov", "pretend", "coverage[toml]"]
 lint = [
     # NOTE: ruff is under active development, so we pin conservatively here
```

### Comparing `pypi_attestation_models-0.0.1rc2/src/pypi_attestation_models/__init__.py` & `pypi_attestation_models-0.0.2/src/pypi_attestation_models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """The `pypi-attestation-models` APIs."""
 
-__version__ = "0.0.1rc2"
+__version__ = "0.0.2"
 
 from ._impl import (
     Attestation,
     AttestationPayload,
     ConversionError,
     InvalidAttestationError,
     TransparencyLogEntry,
```

### Comparing `pypi_attestation_models-0.0.1rc2/src/pypi_attestation_models/_impl.py` & `pypi_attestation_models-0.0.2/src/pypi_attestation_models/_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 This module is NOT a public API, and is not considered stable.
 """
 
 from __future__ import annotations
 
 import binascii
 from base64 import b64decode, b64encode
-from hashlib import sha256
 from typing import TYPE_CHECKING, Annotated, Any, Literal, NewType
 
 import rfc8785
 import sigstore.errors
 from annotated_types import MinLen  # noqa: TCH002
 from cryptography import x509
 from cryptography.hazmat.primitives import serialization
 from pydantic import BaseModel
 from pydantic_core import ValidationError
+from sigstore._utils import _sha256_streaming
 from sigstore.models import Bundle, LogEntry
 
 if TYPE_CHECKING:
     from pathlib import Path  # pragma: no cover
 
     from sigstore.sign import Signer  # pragma: no cover
     from sigstore.verify import Verifier  # pragma: no cover
@@ -112,17 +112,22 @@
     """
     The SHA-256 digest of the distribution's contents, as a hexadecimal string.
     """
 
     @classmethod
     def from_dist(cls, dist: Path) -> AttestationPayload:
         """Create an `AttestationPayload` from a distribution file."""
+        with dist.open(mode="rb", buffering=0) as io:
+            # Replace this with `hashlib.file_digest()` once
+            # our minimum supported Python is >=3.11
+            digest = _sha256_streaming(io).hex()
+
         return AttestationPayload(
             distribution=dist.name,
-            digest=sha256(dist.read_bytes()).hexdigest(),
+            digest=digest,
         )
 
     def sign(self, signer: Signer) -> Attestation:
         """Create a PEP 740 attestation by signing this payload."""
         sigstore_bundle = signer.sign_artifact(bytes(self))
         return sigstore_to_pypi(sigstore_bundle)
```

### Comparing `pypi_attestation_models-0.0.1rc2/PKG-INFO` & `pypi_attestation_models-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pypi-attestation-models
-Version: 0.0.1rc2
+Version: 0.0.2
 Summary: A library to convert between Sigstore Bundles and PEP-740 Attestation objects
 Author-email: Trail of Bits <opensource@trailofbits.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: cryptography
 Requires-Dist: pydantic
-Requires-Dist: sigstore==3.0.0rc2
+Requires-Dist: sigstore~=3.0.0
 Requires-Dist: pypi-attestation-models[doc,test,lint] ; extra == "dev"
 Requires-Dist: twine ; extra == "dev"
 Requires-Dist: wheel ; extra == "dev"
 Requires-Dist: build ; extra == "dev"
 Requires-Dist: pdoc ; extra == "doc"
 Requires-Dist: ruff ~= 0.2 ; extra == "lint"
 Requires-Dist: mypy >= 1.0 ; extra == "lint"
@@ -38,28 +38,28 @@
 
 <!--- BADGES: START --->
 [![CI](https://github.com/trailofbits/pypi-attestation-models/actions/workflows/tests.yml/badge.svg)](https://github.com/trailofbits/pypi-attestation-models/actions/workflows/tests.yml)
 [![PyPI version](https://badge.fury.io/py/pypi-attestation-models.svg)](https://pypi.org/project/pypi-attestation-models)
 [![Packaging status](https://repology.org/badge/tiny-repos/python:pypi-attestation-models.svg)](https://repology.org/project/python:pypi-attestation-models/versions)
 <!--- BADGES: END --->
 
-A library to convert between Sigstore Bundles and PEP-740 Attestation objects
+A library to convert between Sigstore Bundles and [PEP 740] Attestation objects
 
 ## Installation
 
 ```bash
 python -m pip install pypi-attestation-models
 ```
 
 ## Usage
 
 See the full API documentation [here].
 
-
 ### Signing and verification
+
 Use these APIs to create a PEP 740-compliant `Attestation` object by signing a Python artifact
 (i.e: sdist or wheel files), and to verify an `Attestation` object against a Python artifact.
 
 ```python
 from pathlib import Path
 
 from pypi_attestation_models import Attestation, AttestationPayload
@@ -80,15 +80,14 @@
 
 # Verify an attestation against a Python artifact
 attestation_path = Path("test_package-0.0.1-py3-none-any.whl.attestation")
 attestation = Attestation.model_validate_json(attestation_path.read_bytes())
 verifier = Verifier.production()
 policy = policy.Identity(identity="example@gmail.com", issuer="https://accounts.google.com")
 attestation.verify(verifier, policy, attestation_path)
-
 ```
 
 ### Low-level model conversions
 These conversions assume that any Sigstore Bundle used as an input was created
 by signing an `AttestationPayload` object.
 ```python
 from pathlib import Path
@@ -107,9 +106,11 @@
 attestation_path = Path("attestation.json")
 with attestation_path.open("rb") as f:
     attestation = Attestation.model_validate_json(f.read())
 bundle = pypi_to_sigstore(attestation)
 print(bundle.to_json())
 ```
 
+[PEP 740]: https://peps.python.org/pep-0740/
+
 [here]: https://trailofbits.github.io/pypi-attestation-models
```

