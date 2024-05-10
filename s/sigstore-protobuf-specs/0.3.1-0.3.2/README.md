# Comparing `tmp/sigstore_protobuf_specs-0.3.1.tar.gz` & `tmp/sigstore_protobuf_specs-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigstore_protobuf_specs-0.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sigstore_protobuf_specs-0.3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sigstore_protobuf_specs-0.3.1.tar` & `sigstore_protobuf_specs-0.3.2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0    11358 2024-04-02 17:45:06.452222 sigstore_protobuf_specs-0.3.1/LICENSE
--rw-r--r--   0        0        0      216 2024-04-02 17:45:06.452222 sigstore_protobuf_specs-0.3.1/README.md
--rw-r--r--   0        0        0     1191 2024-04-02 17:45:06.452222 sigstore_protobuf_specs-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-02 17:45:06.452222 sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 17:45:06.452222 sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/dev/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 17:45:06.452222 sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/dev/sigstore/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 17:45:06.452222 sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/dev/sigstore/bundle/__init__.py
--rw-r--r--   0        0        0     4571 2024-04-02 17:45:06.452222 sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/dev/sigstore/bundle/v1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 17:45:06.452222 sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/dev/sigstore/common/__init__.py
--rw-r--r--   0        0        0     9042 2024-04-02 17:45:06.452222 sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/dev/sigstore/common/v1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 17:45:06.452222 sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/dev/sigstore/events/__init__.py
--rw-r--r--   0        0        0     1763 2024-04-02 17:45:06.452222 sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/dev/sigstore/events/v1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 17:45:06.452222 sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/dev/sigstore/rekor/__init__.py
--rw-r--r--   0        0        0     6380 2024-04-02 17:45:06.452222 sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/dev/sigstore/rekor/v1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 17:45:06.456222 sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/dev/sigstore/trustroot/__init__.py
--rw-r--r--   0        0        0     8142 2024-04-02 17:45:06.456222 sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/dev/sigstore/trustroot/v1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 17:45:06.456222 sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/dev/sigstore/verification/__init__.py
--rw-r--r--   0        0        0     7370 2024-04-02 17:45:06.456222 sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/dev/sigstore/verification/v1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 17:45:06.456222 sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/google/__init__.py
--rw-r--r--   0        0        0     2114 2024-04-02 17:45:06.456222 sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/google/api/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 17:45:06.456222 sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/io/__init__.py
--rw-r--r--   0        0        0     1450 2024-04-02 17:45:06.456222 sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/io/intoto/__init__.py
--rw-r--r--   0        0        0     1366 1970-01-01 00:00:00.000000 sigstore_protobuf_specs-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-05-10 18:45:29.634791 sigstore_protobuf_specs-0.3.2/LICENSE
+-rw-r--r--   0        0        0      216 2024-05-10 18:45:29.634791 sigstore_protobuf_specs-0.3.2/README.md
+-rw-r--r--   0        0        0     1191 2024-05-10 18:45:29.634791 sigstore_protobuf_specs-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-10 18:45:29.634791 sigstore_protobuf_specs-0.3.2/sigstore_protobuf_specs/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 18:45:29.634791 sigstore_protobuf_specs-0.3.2/sigstore_protobuf_specs/dev/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 18:45:29.634791 sigstore_protobuf_specs-0.3.2/sigstore_protobuf_specs/dev/sigstore/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 18:45:29.634791 sigstore_protobuf_specs-0.3.2/sigstore_protobuf_specs/dev/sigstore/bundle/__init__.py
+-rw-r--r--   0        0        0     5020 2024-05-10 18:45:29.634791 sigstore_protobuf_specs-0.3.2/sigstore_protobuf_specs/dev/sigstore/bundle/v1/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 18:45:29.634791 sigstore_protobuf_specs-0.3.2/sigstore_protobuf_specs/dev/sigstore/common/__init__.py
+-rw-r--r--   0        0        0     8863 2024-05-10 18:45:29.634791 sigstore_protobuf_specs-0.3.2/sigstore_protobuf_specs/dev/sigstore/common/v1/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 18:45:29.634791 sigstore_protobuf_specs-0.3.2/sigstore_protobuf_specs/dev/sigstore/events/__init__.py
+-rw-r--r--   0        0        0     1763 2024-05-10 18:45:29.634791 sigstore_protobuf_specs-0.3.2/sigstore_protobuf_specs/dev/sigstore/events/v1/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 18:45:29.638791 sigstore_protobuf_specs-0.3.2/sigstore_protobuf_specs/dev/sigstore/rekor/__init__.py
+-rw-r--r--   0        0        0     6567 2024-05-10 18:45:29.638791 sigstore_protobuf_specs-0.3.2/sigstore_protobuf_specs/dev/sigstore/rekor/v1/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 18:45:29.638791 sigstore_protobuf_specs-0.3.2/sigstore_protobuf_specs/dev/sigstore/trustroot/__init__.py
+-rw-r--r--   0        0        0     9274 2024-05-10 18:45:29.638791 sigstore_protobuf_specs-0.3.2/sigstore_protobuf_specs/dev/sigstore/trustroot/v1/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 18:45:29.638791 sigstore_protobuf_specs-0.3.2/sigstore_protobuf_specs/dev/sigstore/verification/__init__.py
+-rw-r--r--   0        0        0     7370 2024-05-10 18:45:29.638791 sigstore_protobuf_specs-0.3.2/sigstore_protobuf_specs/dev/sigstore/verification/v1/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 18:45:29.638791 sigstore_protobuf_specs-0.3.2/sigstore_protobuf_specs/google/__init__.py
+-rw-r--r--   0        0        0     2114 2024-05-10 18:45:29.638791 sigstore_protobuf_specs-0.3.2/sigstore_protobuf_specs/google/api/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 18:45:29.638791 sigstore_protobuf_specs-0.3.2/sigstore_protobuf_specs/io/__init__.py
+-rw-r--r--   0        0        0     1450 2024-05-10 18:45:29.638791 sigstore_protobuf_specs-0.3.2/sigstore_protobuf_specs/io/intoto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 18:45:29.638791 sigstore_protobuf_specs-0.3.2/sigstore_protobuf_specs/py.typed
+-rw-r--r--   0        0        0     1366 1970-01-01 00:00:00.000000 sigstore_protobuf_specs-0.3.2/PKG-INFO
```

### Comparing `sigstore_protobuf_specs-0.3.1/LICENSE` & `sigstore_protobuf_specs-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sigstore_protobuf_specs-0.3.1/pyproject.toml` & `sigstore_protobuf_specs-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "sigstore-protobuf-specs"
-version = "0.3.1"
+version = "0.3.2"
 description = "A library for serializing and deserializing Sigstore messages"
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [
   { name = "Sigstore Authors", email = "sigstore-dev@googlegroups.com" },
 ]
 classifiers = [
```

### Comparing `sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/dev/sigstore/bundle/v1/__init__.py` & `sigstore_protobuf_specs-0.3.2/sigstore_protobuf_specs/dev/sigstore/bundle/v1/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,9 +105,15 @@
     dsse_envelope: "____io_intoto__.Envelope" = betterproto.message_field(
         4, group="content"
     )
     """
     A DSSE envelope can contain arbitrary payloads. Verifiers must verify that
     the payload type is a supported and expected type. This is part of the DSSE
     protocol which is defined here: <https://github.com/secure-systems-
-    lab/dsse/blob/master/protocol.md>
+    lab/dsse/blob/master/protocol.md> DSSE envelopes in a bundle MUST have
+    exactly one signture. This is a limitation from the DSSE spec, as it can
+    contain multiple signatures. There are two primary reasons: 1. It simplfies
+    the verification logic and policy 2. The bundle (currently) can only
+    contain a single    instance of the required verification materials During
+    verification a client MUST reject an envelope if the number of signatures
+    is not equal to one.
     """
```

### Comparing `sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/dev/sigstore/common/v1/__init__.py` & `sigstore_protobuf_specs-0.3.2/sigstore_protobuf_specs/dev/sigstore/common/v1/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,20 +138,15 @@
 
 
 @dataclass(eq=False, repr=False)
 class LogId(betterproto.Message):
     """LogId captures the identity of a transparency log."""
 
     key_id: bytes = betterproto.bytes_field(1)
-    """
-    The unique id of the log, represented as the SHA-256 hash of the log's
-    public key, calculated over the DER encoding of the key represented as
-    SubjectPublicKeyInfo. See https://www.rfc-
-    editor.org/rfc/rfc6962#section-3.2
-    """
+    """The unique identity of the log, represented by its public key."""
 
 
 @dataclass(eq=False, repr=False)
 class Rfc3161SignedTimestamp(betterproto.Message):
     """This message holds a RFC 3161 timestamp."""
 
     signed_timestamp: bytes = betterproto.bytes_field(1)
```

### Comparing `sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/dev/sigstore/events/v1/__init__.py` & `sigstore_protobuf_specs-0.3.2/sigstore_protobuf_specs/dev/sigstore/events/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/dev/sigstore/rekor/v1/__init__.py` & `sigstore_protobuf_specs-0.3.2/sigstore_protobuf_specs/dev/sigstore/rekor/v1/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,22 +24,25 @@
     version: str = betterproto.string_field(2)
     """The specific api version of the type."""
 
 
 @dataclass(eq=False, repr=False)
 class Checkpoint(betterproto.Message):
     """
-    The checkpoint MUST contain a signature of the tree head (root hash), size
-    of the tree and the transparency log's unique identifier (log ID). It MAY
-    also be followed by any optional data. The result is a string,  the format
-    is described here https://github.com/transparency-
-    dev/formats/blob/main/log/README.md The details are here https://github.com
-    /sigstore/rekor/blob/a6e58f72b6b18cc06cefe61808efd562b9726330/pkg/util/sign
-    ed_note.go#L114 The signature has the same format as
-    InclusionPromise.signed_entry_timestamp. See below for more details.
+    The checkpoint MUST contain an origin string as a unique log identifier,
+    the tree size, and the root hash. It MAY also be followed by optional data,
+    and clients MUST NOT assume optional data. The checkpoint MUST also contain
+    a signature over the root hash (tree head). The checkpoint MAY contain
+    additional signatures, but the first SHOULD be the signature from the log.
+    Checkpoint contents are concatenated with newlines into a single string.
+    The checkpoint format is described in https://github.com/transparency-
+    dev/formats/blob/main/log/README.md and
+    https://github.com/C2SP/C2SP/blob/main/tlog-checkpoint.md. An example
+    implementation can be found in
+    https://github.com/sigstore/rekor/blob/main/pkg/util/signed_note.go
     """
 
     envelope: str = betterproto.string_field(1)
 
 
 @dataclass(eq=False, repr=False)
 class InclusionProof(betterproto.Message):
```

### Comparing `sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/dev/sigstore/trustroot/v1/__init__.py` & `sigstore_protobuf_specs-0.3.2/sigstore_protobuf_specs/dev/sigstore/trustroot/v1/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,15 +29,35 @@
     public_key: "__common_v1__.PublicKey" = betterproto.message_field(3)
     """
     The public key used to verify signatures generated by the log. This
     attribute contains the signature algorithm used by the log.
     """
 
     log_id: "__common_v1__.LogId" = betterproto.message_field(4)
-    """The unique identifier for this transparency log."""
+    """
+    The unique identifier for this transparency log. Represented as the SHA-256
+    hash of the log's public key, calculated over the DER encoding of the key
+    represented as SubjectPublicKeyInfo. See https://www.rfc-
+    editor.org/rfc/rfc6962#section-3.2
+    """
+
+    checkpoint_key_id: "__common_v1__.LogId" = betterproto.message_field(5)
+    """
+    The checkpoint key identifier for the log used in a checkpoint. Optional,
+    not provided for logs that do not generate checkpoints. For logs that do
+    generate checkpoints, if not set, assume log_id equals checkpoint_key_id.
+    Follows the specification described here for ECDSA and Ed25519 signatures:
+    https://github.com/C2SP/C2SP/blob/main/signed-note.md#signatures For RSA
+    signatures, the key ID will match the ECDSA format, the hashed DER-encoded
+    SPKI public key. Publicly witnessed logs MUST NOT use RSA-signed
+    checkpoints, since witnesses do not support RSA signatures. This is
+    provided for convenience. Clients can also calculate the checkpoint key ID
+    given the log's public key. SHOULD be set for logs generating Ed25519
+    signatures. SHOULD be 4 bytes long, as a truncated hash.
+    """
 
 
 @dataclass(eq=False, repr=False)
 class CertificateAuthority(betterproto.Message):
     """
     CertificateAuthority enlists the information required to identify which CA
     to use and perform signature verification.
```

### Comparing `sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/dev/sigstore/verification/v1/__init__.py` & `sigstore_protobuf_specs-0.3.2/sigstore_protobuf_specs/dev/sigstore/verification/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/google/api/__init__.py` & `sigstore_protobuf_specs-0.3.2/sigstore_protobuf_specs/google/api/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstore_protobuf_specs-0.3.1/sigstore_protobuf_specs/io/intoto/__init__.py` & `sigstore_protobuf_specs-0.3.2/sigstore_protobuf_specs/io/intoto/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstore_protobuf_specs-0.3.1/PKG-INFO` & `sigstore_protobuf_specs-0.3.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigstore-protobuf-specs
-Version: 0.3.1
+Version: 0.3.2
 Summary: A library for serializing and deserializing Sigstore messages
 Author-email: Sigstore Authors <sigstore-dev@googlegroups.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
```

