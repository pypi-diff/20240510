# Comparing `tmp/pulumi_tls-5.1.0a1715237163.tar.gz` & `tmp/pulumi_tls-5.1.0a1715306927.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_tls-5.1.0a1715237163.tar", last modified: Thu May  9 06:48:42 2024, max compression
+gzip compressed data, was "pulumi_tls-5.1.0a1715306927.tar", last modified: Fri May 10 02:17:45 2024, max compression
```

## Comparing `pulumi_tls-5.1.0a1715237163.tar` & `pulumi_tls-5.1.0a1715306927.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:48:42.977201 pulumi_tls-5.1.0a1715237163/
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-09 06:48:42.977201 pulumi_tls-5.1.0a1715237163/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-05-09 06:48:36.000000 pulumi_tls-5.1.0a1715237163/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:48:42.977201 pulumi_tls-5.1.0a1715237163/pulumi_tls/
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-09 06:48:36.000000 pulumi_tls-5.1.0a1715237163/pulumi_tls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14351 2024-05-09 06:48:36.000000 pulumi_tls-5.1.0a1715237163/pulumi_tls/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-09 06:48:36.000000 pulumi_tls-5.1.0a1715237163/pulumi_tls/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    20435 2024-05-09 06:48:36.000000 pulumi_tls-5.1.0a1715237163/pulumi_tls/cert_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:48:42.977201 pulumi_tls-5.1.0a1715237163/pulumi_tls/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-09 06:48:36.000000 pulumi_tls-5.1.0a1715237163/pulumi_tls/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-09 06:48:36.000000 pulumi_tls-5.1.0a1715237163/pulumi_tls/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-09 06:48:36.000000 pulumi_tls-5.1.0a1715237163/pulumi_tls/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-09 06:48:36.000000 pulumi_tls-5.1.0a1715237163/pulumi_tls/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-09 06:48:36.000000 pulumi_tls-5.1.0a1715237163/pulumi_tls/get_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-05-09 06:48:36.000000 pulumi_tls-5.1.0a1715237163/pulumi_tls/get_public_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    41155 2024-05-09 06:48:36.000000 pulumi_tls-5.1.0a1715237163/pulumi_tls/locally_signed_cert.py
--rw-r--r--   0 runner    (1001) docker     (127)    14909 2024-05-09 06:48:36.000000 pulumi_tls-5.1.0a1715237163/pulumi_tls/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22201 2024-05-09 06:48:36.000000 pulumi_tls-5.1.0a1715237163/pulumi_tls/private_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-05-09 06:48:36.000000 pulumi_tls-5.1.0a1715237163/pulumi_tls/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-09 06:48:36.000000 pulumi_tls-5.1.0a1715237163/pulumi_tls/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 06:48:36.000000 pulumi_tls-5.1.0a1715237163/pulumi_tls/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    50239 2024-05-09 06:48:36.000000 pulumi_tls-5.1.0a1715237163/pulumi_tls/self_signed_cert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:48:42.977201 pulumi_tls-5.1.0a1715237163/pulumi_tls.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-09 06:48:42.000000 pulumi_tls-5.1.0a1715237163/pulumi_tls.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-09 06:48:42.000000 pulumi_tls-5.1.0a1715237163/pulumi_tls.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 06:48:42.000000 pulumi_tls-5.1.0a1715237163/pulumi_tls.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 06:48:42.000000 pulumi_tls-5.1.0a1715237163/pulumi_tls.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-09 06:48:42.000000 pulumi_tls-5.1.0a1715237163/pulumi_tls.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-09 06:48:36.000000 pulumi_tls-5.1.0a1715237163/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 06:48:42.977201 pulumi_tls-5.1.0a1715237163/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:17:45.790933 pulumi_tls-5.1.0a1715306927/
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-10 02:17:45.790933 pulumi_tls-5.1.0a1715306927/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-05-10 02:17:39.000000 pulumi_tls-5.1.0a1715306927/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:17:45.786934 pulumi_tls-5.1.0a1715306927/pulumi_tls/
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-10 02:17:39.000000 pulumi_tls-5.1.0a1715306927/pulumi_tls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14351 2024-05-10 02:17:39.000000 pulumi_tls-5.1.0a1715306927/pulumi_tls/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-10 02:17:39.000000 pulumi_tls-5.1.0a1715306927/pulumi_tls/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20435 2024-05-10 02:17:39.000000 pulumi_tls-5.1.0a1715306927/pulumi_tls/cert_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:17:45.790933 pulumi_tls-5.1.0a1715306927/pulumi_tls/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-10 02:17:39.000000 pulumi_tls-5.1.0a1715306927/pulumi_tls/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-10 02:17:39.000000 pulumi_tls-5.1.0a1715306927/pulumi_tls/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-10 02:17:39.000000 pulumi_tls-5.1.0a1715306927/pulumi_tls/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-10 02:17:39.000000 pulumi_tls-5.1.0a1715306927/pulumi_tls/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-10 02:17:39.000000 pulumi_tls-5.1.0a1715306927/pulumi_tls/get_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-05-10 02:17:39.000000 pulumi_tls-5.1.0a1715306927/pulumi_tls/get_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36895 2024-05-10 02:17:39.000000 pulumi_tls-5.1.0a1715306927/pulumi_tls/locally_signed_cert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14909 2024-05-10 02:17:39.000000 pulumi_tls-5.1.0a1715306927/pulumi_tls/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22201 2024-05-10 02:17:39.000000 pulumi_tls-5.1.0a1715306927/pulumi_tls/private_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-05-10 02:17:39.000000 pulumi_tls-5.1.0a1715306927/pulumi_tls/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-10 02:17:39.000000 pulumi_tls-5.1.0a1715306927/pulumi_tls/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 02:17:39.000000 pulumi_tls-5.1.0a1715306927/pulumi_tls/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    45979 2024-05-10 02:17:39.000000 pulumi_tls-5.1.0a1715306927/pulumi_tls/self_signed_cert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:17:45.790933 pulumi_tls-5.1.0a1715306927/pulumi_tls.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-10 02:17:45.000000 pulumi_tls-5.1.0a1715306927/pulumi_tls.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-10 02:17:45.000000 pulumi_tls-5.1.0a1715306927/pulumi_tls.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 02:17:45.000000 pulumi_tls-5.1.0a1715306927/pulumi_tls.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-10 02:17:45.000000 pulumi_tls-5.1.0a1715306927/pulumi_tls.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-10 02:17:45.000000 pulumi_tls-5.1.0a1715306927/pulumi_tls.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-10 02:17:39.000000 pulumi_tls-5.1.0a1715306927/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 02:17:45.790933 pulumi_tls-5.1.0a1715306927/setup.cfg
```

### Comparing `pulumi_tls-5.1.0a1715237163/PKG-INFO` & `pulumi_tls-5.1.0a1715306927/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_tls
-Version: 5.1.0a1715237163
+Version: 5.1.0a1715306927
 Summary: A Pulumi package to create TLS resources in Pulumi programs.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-tls
 Keywords: pulumi,tls
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_tls-5.1.0a1715237163/README.md` & `pulumi_tls-5.1.0a1715306927/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1715237163/pulumi_tls/__init__.py` & `pulumi_tls-5.1.0a1715306927/pulumi_tls/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1715237163/pulumi_tls/_inputs.py` & `pulumi_tls-5.1.0a1715306927/pulumi_tls/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1715237163/pulumi_tls/_utilities.py` & `pulumi_tls-5.1.0a1715306927/pulumi_tls/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1715237163/pulumi_tls/cert_request.py` & `pulumi_tls-5.1.0a1715306927/pulumi_tls/cert_request.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1715237163/pulumi_tls/config/outputs.py` & `pulumi_tls-5.1.0a1715306927/pulumi_tls/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1715237163/pulumi_tls/config/vars.py` & `pulumi_tls-5.1.0a1715306927/pulumi_tls/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1715237163/pulumi_tls/get_certificate.py` & `pulumi_tls-5.1.0a1715306927/pulumi_tls/get_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1715237163/pulumi_tls/get_public_key.py` & `pulumi_tls-5.1.0a1715306927/pulumi_tls/get_public_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1715237163/pulumi_tls/locally_signed_cert.py` & `pulumi_tls-5.1.0a1715306927/pulumi_tls/locally_signed_cert.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,19 +25,14 @@
         """
         The set of arguments for constructing a LocallySignedCert resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] allowed_uses: List of key usages allowed for the issued certificate. Values are defined in [RFC 5280](https://datatracker.ietf.org/doc/html/rfc5280) and combine flags defined by both [Key Usages](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.3) and [Extended Key Usages](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.12). Accepted values: `any_extended`, `cert_signing`, `client_auth`, `code_signing`, `content_commitment`, `crl_signing`, `data_encipherment`, `decipher_only`, `digital_signature`, `email_protection`, `encipher_only`, `ipsec_end_system`, `ipsec_tunnel`, `ipsec_user`, `key_agreement`, `key_encipherment`, `microsoft_commercial_code_signing`, `microsoft_kernel_code_signing`, `microsoft_server_gated_crypto`, `netscape_server_gated_crypto`, `ocsp_signing`, `server_auth`, `timestamping`.
         :param pulumi.Input[str] ca_cert_pem: Certificate data of the Certificate Authority (CA) in [PEM (RFC 1421)](https://datatracker.ietf.org/doc/html/rfc1421) format.
         :param pulumi.Input[str] ca_private_key_pem: Private key of the Certificate Authority (CA) used to sign the certificate, in [PEM (RFC 1421)](https://datatracker.ietf.org/doc/html/rfc1421) format.
         :param pulumi.Input[str] cert_request_pem: Certificate request data in [PEM (RFC 1421)](https://datatracker.ietf.org/doc/html/rfc1421) format.
         :param pulumi.Input[int] validity_period_hours: Number of hours, after initial issuing, that the certificate will remain valid for.
-        :param pulumi.Input[int] early_renewal_hours: The resource will consider the certificate to have expired the given number of hours before its actual expiry time. This
-               can be useful to deploy an updated certificate in advance of the expiration of the current certificate. However, the old
-               certificate remains valid until its true expiration time, since this resource does not (and cannot) support certificate
-               revocation. Also, this advance update can only be performed should the Terraform configuration be applied during the
-               early renewal period. (default: `0`)
         :param pulumi.Input[bool] is_ca_certificate: Is the generated certificate representing a Certificate Authority (CA) (default: `false`).
         :param pulumi.Input[bool] set_subject_key_id: Should the generated certificate include a [subject key identifier](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.2) (default: `false`).
         """
         pulumi.set(__self__, "allowed_uses", allowed_uses)
         pulumi.set(__self__, "ca_cert_pem", ca_cert_pem)
         pulumi.set(__self__, "ca_private_key_pem", ca_private_key_pem)
         pulumi.set(__self__, "cert_request_pem", cert_request_pem)
@@ -108,21 +103,14 @@
     @validity_period_hours.setter
     def validity_period_hours(self, value: pulumi.Input[int]):
         pulumi.set(self, "validity_period_hours", value)
 
     @property
     @pulumi.getter(name="earlyRenewalHours")
     def early_renewal_hours(self) -> Optional[pulumi.Input[int]]:
-        """
-        The resource will consider the certificate to have expired the given number of hours before its actual expiry time. This
-        can be useful to deploy an updated certificate in advance of the expiration of the current certificate. However, the old
-        certificate remains valid until its true expiration time, since this resource does not (and cannot) support certificate
-        revocation. Also, this advance update can only be performed should the Terraform configuration be applied during the
-        early renewal period. (default: `0`)
-        """
         return pulumi.get(self, "early_renewal_hours")
 
     @early_renewal_hours.setter
     def early_renewal_hours(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "early_renewal_hours", value)
 
     @property
@@ -170,19 +158,14 @@
         Input properties used for looking up and filtering LocallySignedCert resources.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] allowed_uses: List of key usages allowed for the issued certificate. Values are defined in [RFC 5280](https://datatracker.ietf.org/doc/html/rfc5280) and combine flags defined by both [Key Usages](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.3) and [Extended Key Usages](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.12). Accepted values: `any_extended`, `cert_signing`, `client_auth`, `code_signing`, `content_commitment`, `crl_signing`, `data_encipherment`, `decipher_only`, `digital_signature`, `email_protection`, `encipher_only`, `ipsec_end_system`, `ipsec_tunnel`, `ipsec_user`, `key_agreement`, `key_encipherment`, `microsoft_commercial_code_signing`, `microsoft_kernel_code_signing`, `microsoft_server_gated_crypto`, `netscape_server_gated_crypto`, `ocsp_signing`, `server_auth`, `timestamping`.
         :param pulumi.Input[str] ca_cert_pem: Certificate data of the Certificate Authority (CA) in [PEM (RFC 1421)](https://datatracker.ietf.org/doc/html/rfc1421) format.
         :param pulumi.Input[str] ca_key_algorithm: Name of the algorithm used when generating the private key provided in `ca_private_key_pem`.
         :param pulumi.Input[str] ca_private_key_pem: Private key of the Certificate Authority (CA) used to sign the certificate, in [PEM (RFC 1421)](https://datatracker.ietf.org/doc/html/rfc1421) format.
         :param pulumi.Input[str] cert_pem: Certificate data in PEM (RFC 1421).
         :param pulumi.Input[str] cert_request_pem: Certificate request data in [PEM (RFC 1421)](https://datatracker.ietf.org/doc/html/rfc1421) format.
-        :param pulumi.Input[int] early_renewal_hours: The resource will consider the certificate to have expired the given number of hours before its actual expiry time. This
-               can be useful to deploy an updated certificate in advance of the expiration of the current certificate. However, the old
-               certificate remains valid until its true expiration time, since this resource does not (and cannot) support certificate
-               revocation. Also, this advance update can only be performed should the Terraform configuration be applied during the
-               early renewal period. (default: `0`)
         :param pulumi.Input[bool] is_ca_certificate: Is the generated certificate representing a Certificate Authority (CA) (default: `false`).
         :param pulumi.Input[bool] ready_for_renewal: Is the certificate either expired (i.e. beyond the `validity_period_hours`) or ready for an early renewal (i.e. within the `early_renewal_hours`)?
         :param pulumi.Input[bool] set_subject_key_id: Should the generated certificate include a [subject key identifier](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.2) (default: `false`).
         :param pulumi.Input[str] validity_end_time: The time until which the certificate is invalid, expressed as an [RFC3339](https://tools.ietf.org/html/rfc3339) timestamp.
         :param pulumi.Input[int] validity_period_hours: Number of hours, after initial issuing, that the certificate will remain valid for.
         :param pulumi.Input[str] validity_start_time: The time after which the certificate is valid, expressed as an [RFC3339](https://tools.ietf.org/html/rfc3339) timestamp.
         """
@@ -284,21 +267,14 @@
     @cert_request_pem.setter
     def cert_request_pem(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cert_request_pem", value)
 
     @property
     @pulumi.getter(name="earlyRenewalHours")
     def early_renewal_hours(self) -> Optional[pulumi.Input[int]]:
-        """
-        The resource will consider the certificate to have expired the given number of hours before its actual expiry time. This
-        can be useful to deploy an updated certificate in advance of the expiration of the current certificate. However, the old
-        certificate remains valid until its true expiration time, since this resource does not (and cannot) support certificate
-        revocation. Also, this advance update can only be performed should the Terraform configuration be applied during the
-        early renewal period. (default: `0`)
-        """
         return pulumi.get(self, "early_renewal_hours")
 
     @early_renewal_hours.setter
     def early_renewal_hours(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "early_renewal_hours", value)
 
     @property
@@ -392,19 +368,14 @@
         Create a LocallySignedCert resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] allowed_uses: List of key usages allowed for the issued certificate. Values are defined in [RFC 5280](https://datatracker.ietf.org/doc/html/rfc5280) and combine flags defined by both [Key Usages](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.3) and [Extended Key Usages](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.12). Accepted values: `any_extended`, `cert_signing`, `client_auth`, `code_signing`, `content_commitment`, `crl_signing`, `data_encipherment`, `decipher_only`, `digital_signature`, `email_protection`, `encipher_only`, `ipsec_end_system`, `ipsec_tunnel`, `ipsec_user`, `key_agreement`, `key_encipherment`, `microsoft_commercial_code_signing`, `microsoft_kernel_code_signing`, `microsoft_server_gated_crypto`, `netscape_server_gated_crypto`, `ocsp_signing`, `server_auth`, `timestamping`.
         :param pulumi.Input[str] ca_cert_pem: Certificate data of the Certificate Authority (CA) in [PEM (RFC 1421)](https://datatracker.ietf.org/doc/html/rfc1421) format.
         :param pulumi.Input[str] ca_private_key_pem: Private key of the Certificate Authority (CA) used to sign the certificate, in [PEM (RFC 1421)](https://datatracker.ietf.org/doc/html/rfc1421) format.
         :param pulumi.Input[str] cert_request_pem: Certificate request data in [PEM (RFC 1421)](https://datatracker.ietf.org/doc/html/rfc1421) format.
-        :param pulumi.Input[int] early_renewal_hours: The resource will consider the certificate to have expired the given number of hours before its actual expiry time. This
-               can be useful to deploy an updated certificate in advance of the expiration of the current certificate. However, the old
-               certificate remains valid until its true expiration time, since this resource does not (and cannot) support certificate
-               revocation. Also, this advance update can only be performed should the Terraform configuration be applied during the
-               early renewal period. (default: `0`)
         :param pulumi.Input[bool] is_ca_certificate: Is the generated certificate representing a Certificate Authority (CA) (default: `false`).
         :param pulumi.Input[bool] set_subject_key_id: Should the generated certificate include a [subject key identifier](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.2) (default: `false`).
         :param pulumi.Input[int] validity_period_hours: Number of hours, after initial issuing, that the certificate will remain valid for.
         """
         ...
     @overload
     def __init__(__self__,
@@ -502,19 +473,14 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] allowed_uses: List of key usages allowed for the issued certificate. Values are defined in [RFC 5280](https://datatracker.ietf.org/doc/html/rfc5280) and combine flags defined by both [Key Usages](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.3) and [Extended Key Usages](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.12). Accepted values: `any_extended`, `cert_signing`, `client_auth`, `code_signing`, `content_commitment`, `crl_signing`, `data_encipherment`, `decipher_only`, `digital_signature`, `email_protection`, `encipher_only`, `ipsec_end_system`, `ipsec_tunnel`, `ipsec_user`, `key_agreement`, `key_encipherment`, `microsoft_commercial_code_signing`, `microsoft_kernel_code_signing`, `microsoft_server_gated_crypto`, `netscape_server_gated_crypto`, `ocsp_signing`, `server_auth`, `timestamping`.
         :param pulumi.Input[str] ca_cert_pem: Certificate data of the Certificate Authority (CA) in [PEM (RFC 1421)](https://datatracker.ietf.org/doc/html/rfc1421) format.
         :param pulumi.Input[str] ca_key_algorithm: Name of the algorithm used when generating the private key provided in `ca_private_key_pem`.
         :param pulumi.Input[str] ca_private_key_pem: Private key of the Certificate Authority (CA) used to sign the certificate, in [PEM (RFC 1421)](https://datatracker.ietf.org/doc/html/rfc1421) format.
         :param pulumi.Input[str] cert_pem: Certificate data in PEM (RFC 1421).
         :param pulumi.Input[str] cert_request_pem: Certificate request data in [PEM (RFC 1421)](https://datatracker.ietf.org/doc/html/rfc1421) format.
-        :param pulumi.Input[int] early_renewal_hours: The resource will consider the certificate to have expired the given number of hours before its actual expiry time. This
-               can be useful to deploy an updated certificate in advance of the expiration of the current certificate. However, the old
-               certificate remains valid until its true expiration time, since this resource does not (and cannot) support certificate
-               revocation. Also, this advance update can only be performed should the Terraform configuration be applied during the
-               early renewal period. (default: `0`)
         :param pulumi.Input[bool] is_ca_certificate: Is the generated certificate representing a Certificate Authority (CA) (default: `false`).
         :param pulumi.Input[bool] ready_for_renewal: Is the certificate either expired (i.e. beyond the `validity_period_hours`) or ready for an early renewal (i.e. within the `early_renewal_hours`)?
         :param pulumi.Input[bool] set_subject_key_id: Should the generated certificate include a [subject key identifier](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.2) (default: `false`).
         :param pulumi.Input[str] validity_end_time: The time until which the certificate is invalid, expressed as an [RFC3339](https://tools.ietf.org/html/rfc3339) timestamp.
         :param pulumi.Input[int] validity_period_hours: Number of hours, after initial issuing, that the certificate will remain valid for.
         :param pulumi.Input[str] validity_start_time: The time after which the certificate is valid, expressed as an [RFC3339](https://tools.ietf.org/html/rfc3339) timestamp.
         """
@@ -584,21 +550,14 @@
         Certificate request data in [PEM (RFC 1421)](https://datatracker.ietf.org/doc/html/rfc1421) format.
         """
         return pulumi.get(self, "cert_request_pem")
 
     @property
     @pulumi.getter(name="earlyRenewalHours")
     def early_renewal_hours(self) -> pulumi.Output[int]:
-        """
-        The resource will consider the certificate to have expired the given number of hours before its actual expiry time. This
-        can be useful to deploy an updated certificate in advance of the expiration of the current certificate. However, the old
-        certificate remains valid until its true expiration time, since this resource does not (and cannot) support certificate
-        revocation. Also, this advance update can only be performed should the Terraform configuration be applied during the
-        early renewal period. (default: `0`)
-        """
         return pulumi.get(self, "early_renewal_hours")
 
     @property
     @pulumi.getter(name="isCaCertificate")
     def is_ca_certificate(self) -> pulumi.Output[bool]:
         """
         Is the generated certificate representing a Certificate Authority (CA) (default: `false`).
```

### Comparing `pulumi_tls-5.1.0a1715237163/pulumi_tls/outputs.py` & `pulumi_tls-5.1.0a1715306927/pulumi_tls/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1715237163/pulumi_tls/private_key.py` & `pulumi_tls-5.1.0a1715306927/pulumi_tls/private_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1715237163/pulumi_tls/provider.py` & `pulumi_tls-5.1.0a1715306927/pulumi_tls/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1715237163/pulumi_tls/self_signed_cert.py` & `pulumi_tls-5.1.0a1715306927/pulumi_tls/self_signed_cert.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,19 +29,14 @@
                  uris: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a SelfSignedCert resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] allowed_uses: List of key usages allowed for the issued certificate. Values are defined in [RFC 5280](https://datatracker.ietf.org/doc/html/rfc5280) and combine flags defined by both [Key Usages](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.3) and [Extended Key Usages](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.12). Accepted values: `any_extended`, `cert_signing`, `client_auth`, `code_signing`, `content_commitment`, `crl_signing`, `data_encipherment`, `decipher_only`, `digital_signature`, `email_protection`, `encipher_only`, `ipsec_end_system`, `ipsec_tunnel`, `ipsec_user`, `key_agreement`, `key_encipherment`, `microsoft_commercial_code_signing`, `microsoft_kernel_code_signing`, `microsoft_server_gated_crypto`, `netscape_server_gated_crypto`, `ocsp_signing`, `server_auth`, `timestamping`.
         :param pulumi.Input[str] private_key_pem: Private key in PEM (RFC 1421) interpolation function.
         :param pulumi.Input[int] validity_period_hours: Number of hours, after initial issuing, that the certificate will remain valid for.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] dns_names: List of DNS names for which a certificate is being requested (i.e. certificate subjects).
-        :param pulumi.Input[int] early_renewal_hours: The resource will consider the certificate to have expired the given number of hours before its actual expiry time. This
-               can be useful to deploy an updated certificate in advance of the expiration of the current certificate. However, the old
-               certificate remains valid until its true expiration time, since this resource does not (and cannot) support certificate
-               revocation. Also, this advance update can only be performed should the Terraform configuration be applied during the
-               early renewal period. (default: `0`)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ip_addresses: List of IP addresses for which a certificate is being requested (i.e. certificate subjects).
         :param pulumi.Input[bool] is_ca_certificate: Is the generated certificate representing a Certificate Authority (CA) (default: `false`).
         :param pulumi.Input[bool] set_authority_key_id: Should the generated certificate include an [authority key identifier](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.1): for self-signed certificates this is the same value as the [subject key identifier](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.2) (default: `false`).
         :param pulumi.Input[bool] set_subject_key_id: Should the generated certificate include a [subject key identifier](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.2) (default: `false`).
         :param pulumi.Input['SelfSignedCertSubjectArgs'] subject: The subject for which a certificate is being requested. The acceptable arguments are all optional and their naming is based upon [Issuer Distinguished Names (RFC5280)](https://tools.ietf.org/html/rfc5280#section-4.1.2.4) section.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] uris: List of URIs for which a certificate is being requested (i.e. certificate subjects).
         """
@@ -112,21 +107,14 @@
     @dns_names.setter
     def dns_names(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "dns_names", value)
 
     @property
     @pulumi.getter(name="earlyRenewalHours")
     def early_renewal_hours(self) -> Optional[pulumi.Input[int]]:
-        """
-        The resource will consider the certificate to have expired the given number of hours before its actual expiry time. This
-        can be useful to deploy an updated certificate in advance of the expiration of the current certificate. However, the old
-        certificate remains valid until its true expiration time, since this resource does not (and cannot) support certificate
-        revocation. Also, this advance update can only be performed should the Terraform configuration be applied during the
-        early renewal period. (default: `0`)
-        """
         return pulumi.get(self, "early_renewal_hours")
 
     @early_renewal_hours.setter
     def early_renewal_hours(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "early_renewal_hours", value)
 
     @property
@@ -222,19 +210,14 @@
                  validity_period_hours: Optional[pulumi.Input[int]] = None,
                  validity_start_time: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering SelfSignedCert resources.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] allowed_uses: List of key usages allowed for the issued certificate. Values are defined in [RFC 5280](https://datatracker.ietf.org/doc/html/rfc5280) and combine flags defined by both [Key Usages](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.3) and [Extended Key Usages](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.12). Accepted values: `any_extended`, `cert_signing`, `client_auth`, `code_signing`, `content_commitment`, `crl_signing`, `data_encipherment`, `decipher_only`, `digital_signature`, `email_protection`, `encipher_only`, `ipsec_end_system`, `ipsec_tunnel`, `ipsec_user`, `key_agreement`, `key_encipherment`, `microsoft_commercial_code_signing`, `microsoft_kernel_code_signing`, `microsoft_server_gated_crypto`, `netscape_server_gated_crypto`, `ocsp_signing`, `server_auth`, `timestamping`.
         :param pulumi.Input[str] cert_pem: Certificate data in PEM (RFC 1421).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] dns_names: List of DNS names for which a certificate is being requested (i.e. certificate subjects).
-        :param pulumi.Input[int] early_renewal_hours: The resource will consider the certificate to have expired the given number of hours before its actual expiry time. This
-               can be useful to deploy an updated certificate in advance of the expiration of the current certificate. However, the old
-               certificate remains valid until its true expiration time, since this resource does not (and cannot) support certificate
-               revocation. Also, this advance update can only be performed should the Terraform configuration be applied during the
-               early renewal period. (default: `0`)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ip_addresses: List of IP addresses for which a certificate is being requested (i.e. certificate subjects).
         :param pulumi.Input[bool] is_ca_certificate: Is the generated certificate representing a Certificate Authority (CA) (default: `false`).
         :param pulumi.Input[str] key_algorithm: Name of the algorithm used when generating the private key provided in `private_key_pem`.
         :param pulumi.Input[str] private_key_pem: Private key in PEM (RFC 1421) interpolation function.
         :param pulumi.Input[bool] ready_for_renewal: Is the certificate either expired (i.e. beyond the `validity_period_hours`) or ready for an early renewal (i.e. within the `early_renewal_hours`)?
         :param pulumi.Input[bool] set_authority_key_id: Should the generated certificate include an [authority key identifier](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.1): for self-signed certificates this is the same value as the [subject key identifier](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.2) (default: `false`).
         :param pulumi.Input[bool] set_subject_key_id: Should the generated certificate include a [subject key identifier](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.2) (default: `false`).
@@ -312,21 +295,14 @@
     @dns_names.setter
     def dns_names(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "dns_names", value)
 
     @property
     @pulumi.getter(name="earlyRenewalHours")
     def early_renewal_hours(self) -> Optional[pulumi.Input[int]]:
-        """
-        The resource will consider the certificate to have expired the given number of hours before its actual expiry time. This
-        can be useful to deploy an updated certificate in advance of the expiration of the current certificate. However, the old
-        certificate remains valid until its true expiration time, since this resource does not (and cannot) support certificate
-        revocation. Also, this advance update can only be performed should the Terraform configuration be applied during the
-        early renewal period. (default: `0`)
-        """
         return pulumi.get(self, "early_renewal_hours")
 
     @early_renewal_hours.setter
     def early_renewal_hours(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "early_renewal_hours", value)
 
     @property
@@ -493,19 +469,14 @@
                  __props__=None):
         """
         Create a SelfSignedCert resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] allowed_uses: List of key usages allowed for the issued certificate. Values are defined in [RFC 5280](https://datatracker.ietf.org/doc/html/rfc5280) and combine flags defined by both [Key Usages](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.3) and [Extended Key Usages](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.12). Accepted values: `any_extended`, `cert_signing`, `client_auth`, `code_signing`, `content_commitment`, `crl_signing`, `data_encipherment`, `decipher_only`, `digital_signature`, `email_protection`, `encipher_only`, `ipsec_end_system`, `ipsec_tunnel`, `ipsec_user`, `key_agreement`, `key_encipherment`, `microsoft_commercial_code_signing`, `microsoft_kernel_code_signing`, `microsoft_server_gated_crypto`, `netscape_server_gated_crypto`, `ocsp_signing`, `server_auth`, `timestamping`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] dns_names: List of DNS names for which a certificate is being requested (i.e. certificate subjects).
-        :param pulumi.Input[int] early_renewal_hours: The resource will consider the certificate to have expired the given number of hours before its actual expiry time. This
-               can be useful to deploy an updated certificate in advance of the expiration of the current certificate. However, the old
-               certificate remains valid until its true expiration time, since this resource does not (and cannot) support certificate
-               revocation. Also, this advance update can only be performed should the Terraform configuration be applied during the
-               early renewal period. (default: `0`)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ip_addresses: List of IP addresses for which a certificate is being requested (i.e. certificate subjects).
         :param pulumi.Input[bool] is_ca_certificate: Is the generated certificate representing a Certificate Authority (CA) (default: `false`).
         :param pulumi.Input[str] private_key_pem: Private key in PEM (RFC 1421) interpolation function.
         :param pulumi.Input[bool] set_authority_key_id: Should the generated certificate include an [authority key identifier](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.1): for self-signed certificates this is the same value as the [subject key identifier](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.2) (default: `false`).
         :param pulumi.Input[bool] set_subject_key_id: Should the generated certificate include a [subject key identifier](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.2) (default: `false`).
         :param pulumi.Input[pulumi.InputType['SelfSignedCertSubjectArgs']] subject: The subject for which a certificate is being requested. The acceptable arguments are all optional and their naming is based upon [Issuer Distinguished Names (RFC5280)](https://tools.ietf.org/html/rfc5280#section-4.1.2.4) section.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] uris: List of URIs for which a certificate is being requested (i.e. certificate subjects).
@@ -610,19 +581,14 @@
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] allowed_uses: List of key usages allowed for the issued certificate. Values are defined in [RFC 5280](https://datatracker.ietf.org/doc/html/rfc5280) and combine flags defined by both [Key Usages](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.3) and [Extended Key Usages](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.12). Accepted values: `any_extended`, `cert_signing`, `client_auth`, `code_signing`, `content_commitment`, `crl_signing`, `data_encipherment`, `decipher_only`, `digital_signature`, `email_protection`, `encipher_only`, `ipsec_end_system`, `ipsec_tunnel`, `ipsec_user`, `key_agreement`, `key_encipherment`, `microsoft_commercial_code_signing`, `microsoft_kernel_code_signing`, `microsoft_server_gated_crypto`, `netscape_server_gated_crypto`, `ocsp_signing`, `server_auth`, `timestamping`.
         :param pulumi.Input[str] cert_pem: Certificate data in PEM (RFC 1421).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] dns_names: List of DNS names for which a certificate is being requested (i.e. certificate subjects).
-        :param pulumi.Input[int] early_renewal_hours: The resource will consider the certificate to have expired the given number of hours before its actual expiry time. This
-               can be useful to deploy an updated certificate in advance of the expiration of the current certificate. However, the old
-               certificate remains valid until its true expiration time, since this resource does not (and cannot) support certificate
-               revocation. Also, this advance update can only be performed should the Terraform configuration be applied during the
-               early renewal period. (default: `0`)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ip_addresses: List of IP addresses for which a certificate is being requested (i.e. certificate subjects).
         :param pulumi.Input[bool] is_ca_certificate: Is the generated certificate representing a Certificate Authority (CA) (default: `false`).
         :param pulumi.Input[str] key_algorithm: Name of the algorithm used when generating the private key provided in `private_key_pem`.
         :param pulumi.Input[str] private_key_pem: Private key in PEM (RFC 1421) interpolation function.
         :param pulumi.Input[bool] ready_for_renewal: Is the certificate either expired (i.e. beyond the `validity_period_hours`) or ready for an early renewal (i.e. within the `early_renewal_hours`)?
         :param pulumi.Input[bool] set_authority_key_id: Should the generated certificate include an [authority key identifier](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.1): for self-signed certificates this is the same value as the [subject key identifier](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.2) (default: `false`).
         :param pulumi.Input[bool] set_subject_key_id: Should the generated certificate include a [subject key identifier](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.2) (default: `false`).
@@ -677,21 +643,14 @@
         List of DNS names for which a certificate is being requested (i.e. certificate subjects).
         """
         return pulumi.get(self, "dns_names")
 
     @property
     @pulumi.getter(name="earlyRenewalHours")
     def early_renewal_hours(self) -> pulumi.Output[int]:
-        """
-        The resource will consider the certificate to have expired the given number of hours before its actual expiry time. This
-        can be useful to deploy an updated certificate in advance of the expiration of the current certificate. However, the old
-        certificate remains valid until its true expiration time, since this resource does not (and cannot) support certificate
-        revocation. Also, this advance update can only be performed should the Terraform configuration be applied during the
-        early renewal period. (default: `0`)
-        """
         return pulumi.get(self, "early_renewal_hours")
 
     @property
     @pulumi.getter(name="ipAddresses")
     def ip_addresses(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
         List of IP addresses for which a certificate is being requested (i.e. certificate subjects).
```

### Comparing `pulumi_tls-5.1.0a1715237163/pulumi_tls.egg-info/PKG-INFO` & `pulumi_tls-5.1.0a1715306927/pulumi_tls.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_tls
-Version: 5.1.0a1715237163
+Version: 5.1.0a1715306927
 Summary: A Pulumi package to create TLS resources in Pulumi programs.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-tls
 Keywords: pulumi,tls
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_tls-5.1.0a1715237163/pulumi_tls.egg-info/SOURCES.txt` & `pulumi_tls-5.1.0a1715306927/pulumi_tls.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1715237163/pyproject.toml` & `pulumi_tls-5.1.0a1715306927/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_tls"
   description = "A Pulumi package to create TLS resources in Pulumi programs."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "tls"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "5.1.0a1715237163"
+  version = "5.1.0a1715306927"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-tls"
 
 [build-system]
```

