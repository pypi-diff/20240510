# Comparing `tmp/pulumi_venafi-1.9.0a1712991486.tar.gz` & `tmp/pulumi_venafi-1.9.0a1713292049.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_venafi-1.9.0a1712991486.tar", last modified: Sat Apr 13 07:00:51 2024, max compression
+gzip compressed data, was "pulumi_venafi-1.9.0a1713292049.tar", last modified: Tue Apr 16 18:31:16 2024, max compression
```

## Comparing `pulumi_venafi-1.9.0a1712991486.tar` & `pulumi_venafi-1.9.0a1713292049.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:00:51.135194 pulumi_venafi-1.9.0a1712991486/
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-04-13 07:00:51.135194 pulumi_venafi-1.9.0a1712991486/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-13 07:00:45.000000 pulumi_venafi-1.9.0a1712991486/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:00:51.131194 pulumi_venafi-1.9.0a1712991486/pulumi_venafi/
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-13 07:00:45.000000 pulumi_venafi-1.9.0a1712991486/pulumi_venafi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-13 07:00:45.000000 pulumi_venafi-1.9.0a1712991486/pulumi_venafi/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    48936 2024-04-13 07:00:45.000000 pulumi_venafi-1.9.0a1712991486/pulumi_venafi/certificate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:00:51.131194 pulumi_venafi-1.9.0a1712991486/pulumi_venafi/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-13 07:00:45.000000 pulumi_venafi-1.9.0a1712991486/pulumi_venafi/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-13 07:00:45.000000 pulumi_venafi-1.9.0a1712991486/pulumi_venafi/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-13 07:00:45.000000 pulumi_venafi-1.9.0a1712991486/pulumi_venafi/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    11857 2024-04-13 07:00:45.000000 pulumi_venafi-1.9.0a1712991486/pulumi_venafi/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    23680 2024-04-13 07:00:45.000000 pulumi_venafi-1.9.0a1712991486/pulumi_venafi/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-13 07:00:45.000000 pulumi_venafi-1.9.0a1712991486/pulumi_venafi/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:00:45.000000 pulumi_venafi-1.9.0a1712991486/pulumi_venafi/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    53759 2024-04-13 07:00:45.000000 pulumi_venafi-1.9.0a1712991486/pulumi_venafi/ssh_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-04-13 07:00:45.000000 pulumi_venafi-1.9.0a1712991486/pulumi_venafi/ssh_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:00:51.135194 pulumi_venafi-1.9.0a1712991486/pulumi_venafi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-04-13 07:00:51.000000 pulumi_venafi-1.9.0a1712991486/pulumi_venafi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-13 07:00:51.000000 pulumi_venafi-1.9.0a1712991486/pulumi_venafi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 07:00:51.000000 pulumi_venafi-1.9.0a1712991486/pulumi_venafi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-13 07:00:51.000000 pulumi_venafi-1.9.0a1712991486/pulumi_venafi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-13 07:00:51.000000 pulumi_venafi-1.9.0a1712991486/pulumi_venafi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-13 07:00:45.000000 pulumi_venafi-1.9.0a1712991486/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 07:00:51.135194 pulumi_venafi-1.9.0a1712991486/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:31:16.673716 pulumi_venafi-1.9.0a1713292049/
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-04-16 18:31:16.673716 pulumi_venafi-1.9.0a1713292049/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-16 18:31:10.000000 pulumi_venafi-1.9.0a1713292049/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:31:16.669716 pulumi_venafi-1.9.0a1713292049/pulumi_venafi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-16 18:31:10.000000 pulumi_venafi-1.9.0a1713292049/pulumi_venafi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-16 18:31:10.000000 pulumi_venafi-1.9.0a1713292049/pulumi_venafi/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48561 2024-04-16 18:31:10.000000 pulumi_venafi-1.9.0a1713292049/pulumi_venafi/certificate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:31:16.669716 pulumi_venafi-1.9.0a1713292049/pulumi_venafi/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-16 18:31:10.000000 pulumi_venafi-1.9.0a1713292049/pulumi_venafi/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-16 18:31:10.000000 pulumi_venafi-1.9.0a1713292049/pulumi_venafi/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-04-16 18:31:10.000000 pulumi_venafi-1.9.0a1713292049/pulumi_venafi/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11820 2024-04-16 18:31:10.000000 pulumi_venafi-1.9.0a1713292049/pulumi_venafi/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23785 2024-04-16 18:31:10.000000 pulumi_venafi-1.9.0a1713292049/pulumi_venafi/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-16 18:31:10.000000 pulumi_venafi-1.9.0a1713292049/pulumi_venafi/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:31:10.000000 pulumi_venafi-1.9.0a1713292049/pulumi_venafi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    54543 2024-04-16 18:31:10.000000 pulumi_venafi-1.9.0a1713292049/pulumi_venafi/ssh_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-04-16 18:31:10.000000 pulumi_venafi-1.9.0a1713292049/pulumi_venafi/ssh_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:31:16.669716 pulumi_venafi-1.9.0a1713292049/pulumi_venafi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-04-16 18:31:16.000000 pulumi_venafi-1.9.0a1713292049/pulumi_venafi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-16 18:31:16.000000 pulumi_venafi-1.9.0a1713292049/pulumi_venafi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 18:31:16.000000 pulumi_venafi-1.9.0a1713292049/pulumi_venafi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-16 18:31:16.000000 pulumi_venafi-1.9.0a1713292049/pulumi_venafi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-16 18:31:16.000000 pulumi_venafi-1.9.0a1713292049/pulumi_venafi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-16 18:31:10.000000 pulumi_venafi-1.9.0a1713292049/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 18:31:16.673716 pulumi_venafi-1.9.0a1713292049/setup.cfg
```

### Comparing `pulumi_venafi-1.9.0a1712991486/PKG-INFO` & `pulumi_venafi-1.9.0a1713292049/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_venafi
-Version: 1.9.0a1712991486
+Version: 1.9.0a1713292049
 Summary: A Pulumi package for creating and managing venafi cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-venafi
 Keywords: pulumi,venafi
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_venafi-1.9.0a1712991486/README.md` & `pulumi_venafi-1.9.0a1713292049/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.9.0a1712991486/pulumi_venafi/__init__.py` & `pulumi_venafi-1.9.0a1713292049/pulumi_venafi/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.9.0a1712991486/pulumi_venafi/_utilities.py` & `pulumi_venafi-1.9.0a1713292049/pulumi_venafi/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.9.0a1712991486/pulumi_venafi/certificate.py` & `pulumi_venafi-1.9.0a1713292049/pulumi_venafi/certificate.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,43 +32,37 @@
                  san_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  san_ips: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  san_uris: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  valid_days: Optional[pulumi.Input[int]] = None):
         """
         The set of arguments for constructing a Certificate resource.
         :param pulumi.Input[str] common_name: The common name of the certificate.
-        :param pulumi.Input[str] algorithm: Key encryption algorithm, either `RSA` or `ECDSA`.
-               Defaults to `RSA`.
-        :param pulumi.Input[str] csr_origin: Whether key-pair generation will be `local` or `service` generated. Default is `local`.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_fields: Collection of Custom Field name-value pairs to
-               assign to the certificate.
+        :param pulumi.Input[str] algorithm: Key encryption algorithm, either RSA or ECDSA. Defaults to `RSA`.
+        :param pulumi.Input[str] csr_origin: Whether key-pair generation will be `local` or `service` generated. Default is 
+               `local`.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_fields: Collection of Custom Field name-value pairs to assign to the certificate.
         :param pulumi.Input[str] ecdsa_curve: ECDSA curve to use when generating a key
-        :param pulumi.Input[int] expiration_window: Number of hours before certificate expiry
-               to request a new certificate.  Defaults to `168`.
-        :param pulumi.Input[str] issuer_hint: Used with valid_days to indicate the target
-               issuer when using Trust Protection Platform.  Relevant values are: "DigiCert",
-               "Entrust", and "Microsoft".
+        :param pulumi.Input[int] expiration_window: Number of hours before certificate expiry to request a new certificate. 
+               Defaults to `168`.
+        :param pulumi.Input[str] issuer_hint: Used with `valid_days` to indicate the target issuer when using Trust Protection 
+               Platform. Relevant values are: `DigiCert`, `Entrust`, and `Microsoft`.
         :param pulumi.Input[str] key_password: The password used to encrypt the private key.
-        :param pulumi.Input[str] nickname: Use to specify a name for the new certificate object that will be created and placed in a policy. Only valid for TPP.
-        :param pulumi.Input[str] pkcs12: A base64-encoded PKCS#12 keystore secured by the `key_password`.
-               Useful when working with resources like
-               azurerm_key_vault_certificate.
+        :param pulumi.Input[str] nickname: Use to specify a name for the new certificate object that will be created and placed 
+               in a policy. Only valid for Trust Protection Platform.
+        :param pulumi.Input[str] pkcs12: A base64-encoded PKCS#12 keystore secured by the `key_password`. Useful when working with resources like 
+               azure key_vault_certificate.
         :param pulumi.Input[str] private_key_pem: The private key in PEM format.
-        :param pulumi.Input[int] rsa_bits: Number of bits to use when generating an RSA key.
-               Applies when `algorithm=RSA`.  Defaults to `2048`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] san_dns: List of DNS names to use as alternative
-               subjects of the certificate.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] san_emails: List of email addresses to use as
-               alternative subjects of the certificate.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] san_ips: List of IP addresses to use as alternative
-               subjects of the certificate.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] san_uris: List of Uniform Resource Identifiers (URIs) to use as alternative
-               subjects of the certificate.
-        :param pulumi.Input[int] valid_days: Desired number of days for which the new
-               certificate will be valid.
+        :param pulumi.Input[int] rsa_bits: Number of bits to use when generating an RSA key. Applies when algorithm is `RSA`. 
+               Defaults to `2048`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] san_dns: List of DNS names to use as alternative subjects of the certificate.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] san_emails: List of email addresses to use as alternative subjects of the certificate.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] san_ips: List of IP addresses to use as alternative subjects of the certificate.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] san_uris: List of Uniform Resource Identifiers (URIs) to use as alternative subjects of 
+               the certificate.
+        :param pulumi.Input[int] valid_days: Desired number of days for which the new certificate will be valid.
         """
         pulumi.set(__self__, "common_name", common_name)
         if algorithm is not None:
             pulumi.set(__self__, "algorithm", algorithm)
         if certificate_dn is not None:
             pulumi.set(__self__, "certificate_dn", certificate_dn)
         if csr_origin is not None:
@@ -116,16 +110,15 @@
     def common_name(self, value: pulumi.Input[str]):
         pulumi.set(self, "common_name", value)
 
     @property
     @pulumi.getter
     def algorithm(self) -> Optional[pulumi.Input[str]]:
         """
-        Key encryption algorithm, either `RSA` or `ECDSA`.
-        Defaults to `RSA`.
+        Key encryption algorithm, either RSA or ECDSA. Defaults to `RSA`.
         """
         return pulumi.get(self, "algorithm")
 
     @algorithm.setter
     def algorithm(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "algorithm", value)
 
@@ -138,15 +131,16 @@
     def certificate_dn(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "certificate_dn", value)
 
     @property
     @pulumi.getter(name="csrOrigin")
     def csr_origin(self) -> Optional[pulumi.Input[str]]:
         """
-        Whether key-pair generation will be `local` or `service` generated. Default is `local`.
+        Whether key-pair generation will be `local` or `service` generated. Default is 
+        `local`.
         """
         return pulumi.get(self, "csr_origin")
 
     @csr_origin.setter
     def csr_origin(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "csr_origin", value)
 
@@ -159,16 +153,15 @@
     def csr_pem(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "csr_pem", value)
 
     @property
     @pulumi.getter(name="customFields")
     def custom_fields(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        Collection of Custom Field name-value pairs to
-        assign to the certificate.
+        Collection of Custom Field name-value pairs to assign to the certificate.
         """
         return pulumi.get(self, "custom_fields")
 
     @custom_fields.setter
     def custom_fields(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "custom_fields", value)
 
@@ -184,30 +177,29 @@
     def ecdsa_curve(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ecdsa_curve", value)
 
     @property
     @pulumi.getter(name="expirationWindow")
     def expiration_window(self) -> Optional[pulumi.Input[int]]:
         """
-        Number of hours before certificate expiry
-        to request a new certificate.  Defaults to `168`.
+        Number of hours before certificate expiry to request a new certificate. 
+        Defaults to `168`.
         """
         return pulumi.get(self, "expiration_window")
 
     @expiration_window.setter
     def expiration_window(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "expiration_window", value)
 
     @property
     @pulumi.getter(name="issuerHint")
     def issuer_hint(self) -> Optional[pulumi.Input[str]]:
         """
-        Used with valid_days to indicate the target
-        issuer when using Trust Protection Platform.  Relevant values are: "DigiCert",
-        "Entrust", and "Microsoft".
+        Used with `valid_days` to indicate the target issuer when using Trust Protection 
+        Platform. Relevant values are: `DigiCert`, `Entrust`, and `Microsoft`.
         """
         return pulumi.get(self, "issuer_hint")
 
     @issuer_hint.setter
     def issuer_hint(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "issuer_hint", value)
 
@@ -223,29 +215,29 @@
     def key_password(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "key_password", value)
 
     @property
     @pulumi.getter
     def nickname(self) -> Optional[pulumi.Input[str]]:
         """
-        Use to specify a name for the new certificate object that will be created and placed in a policy. Only valid for TPP.
+        Use to specify a name for the new certificate object that will be created and placed 
+        in a policy. Only valid for Trust Protection Platform.
         """
         return pulumi.get(self, "nickname")
 
     @nickname.setter
     def nickname(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "nickname", value)
 
     @property
     @pulumi.getter
     def pkcs12(self) -> Optional[pulumi.Input[str]]:
         """
-        A base64-encoded PKCS#12 keystore secured by the `key_password`.
-        Useful when working with resources like
-        azurerm_key_vault_certificate.
+        A base64-encoded PKCS#12 keystore secured by the `key_password`. Useful when working with resources like 
+        azure key_vault_certificate.
         """
         return pulumi.get(self, "pkcs12")
 
     @pkcs12.setter
     def pkcs12(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "pkcs12", value)
 
@@ -261,81 +253,77 @@
     def private_key_pem(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "private_key_pem", value)
 
     @property
     @pulumi.getter(name="rsaBits")
     def rsa_bits(self) -> Optional[pulumi.Input[int]]:
         """
-        Number of bits to use when generating an RSA key.
-        Applies when `algorithm=RSA`.  Defaults to `2048`.
+        Number of bits to use when generating an RSA key. Applies when algorithm is `RSA`. 
+        Defaults to `2048`.
         """
         return pulumi.get(self, "rsa_bits")
 
     @rsa_bits.setter
     def rsa_bits(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "rsa_bits", value)
 
     @property
     @pulumi.getter(name="sanDns")
     def san_dns(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of DNS names to use as alternative
-        subjects of the certificate.
+        List of DNS names to use as alternative subjects of the certificate.
         """
         return pulumi.get(self, "san_dns")
 
     @san_dns.setter
     def san_dns(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "san_dns", value)
 
     @property
     @pulumi.getter(name="sanEmails")
     def san_emails(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of email addresses to use as
-        alternative subjects of the certificate.
+        List of email addresses to use as alternative subjects of the certificate.
         """
         return pulumi.get(self, "san_emails")
 
     @san_emails.setter
     def san_emails(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "san_emails", value)
 
     @property
     @pulumi.getter(name="sanIps")
     def san_ips(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of IP addresses to use as alternative
-        subjects of the certificate.
+        List of IP addresses to use as alternative subjects of the certificate.
         """
         return pulumi.get(self, "san_ips")
 
     @san_ips.setter
     def san_ips(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "san_ips", value)
 
     @property
     @pulumi.getter(name="sanUris")
     def san_uris(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of Uniform Resource Identifiers (URIs) to use as alternative
-        subjects of the certificate.
+        List of Uniform Resource Identifiers (URIs) to use as alternative subjects of 
+        the certificate.
         """
         return pulumi.get(self, "san_uris")
 
     @san_uris.setter
     def san_uris(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "san_uris", value)
 
     @property
     @pulumi.getter(name="validDays")
     def valid_days(self) -> Optional[pulumi.Input[int]]:
         """
-        Desired number of days for which the new
-        certificate will be valid.
+        Desired number of days for which the new certificate will be valid.
         """
         return pulumi.get(self, "valid_days")
 
     @valid_days.setter
     def valid_days(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "valid_days", value)
 
@@ -362,47 +350,40 @@
                  san_dns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  san_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  san_ips: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  san_uris: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  valid_days: Optional[pulumi.Input[int]] = None):
         """
         Input properties used for looking up and filtering Certificate resources.
-        :param pulumi.Input[str] algorithm: Key encryption algorithm, either `RSA` or `ECDSA`.
-               Defaults to `RSA`.
+        :param pulumi.Input[str] algorithm: Key encryption algorithm, either RSA or ECDSA. Defaults to `RSA`.
         :param pulumi.Input[str] certificate: The X509 certificate in PEM format.
-        :param pulumi.Input[str] chain: The trust chain of X509 certificate authority certificates in PEM format
-               concatenated together.
+        :param pulumi.Input[str] chain: The trust chain of X509 certificate authority certificates in PEM format concatenated together.
         :param pulumi.Input[str] common_name: The common name of the certificate.
-        :param pulumi.Input[str] csr_origin: Whether key-pair generation will be `local` or `service` generated. Default is `local`.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_fields: Collection of Custom Field name-value pairs to
-               assign to the certificate.
+        :param pulumi.Input[str] csr_origin: Whether key-pair generation will be `local` or `service` generated. Default is 
+               `local`.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_fields: Collection of Custom Field name-value pairs to assign to the certificate.
         :param pulumi.Input[str] ecdsa_curve: ECDSA curve to use when generating a key
-        :param pulumi.Input[int] expiration_window: Number of hours before certificate expiry
-               to request a new certificate.  Defaults to `168`.
-        :param pulumi.Input[str] issuer_hint: Used with valid_days to indicate the target
-               issuer when using Trust Protection Platform.  Relevant values are: "DigiCert",
-               "Entrust", and "Microsoft".
+        :param pulumi.Input[int] expiration_window: Number of hours before certificate expiry to request a new certificate. 
+               Defaults to `168`.
+        :param pulumi.Input[str] issuer_hint: Used with `valid_days` to indicate the target issuer when using Trust Protection 
+               Platform. Relevant values are: `DigiCert`, `Entrust`, and `Microsoft`.
         :param pulumi.Input[str] key_password: The password used to encrypt the private key.
-        :param pulumi.Input[str] nickname: Use to specify a name for the new certificate object that will be created and placed in a policy. Only valid for TPP.
-        :param pulumi.Input[str] pkcs12: A base64-encoded PKCS#12 keystore secured by the `key_password`.
-               Useful when working with resources like
-               azurerm_key_vault_certificate.
+        :param pulumi.Input[str] nickname: Use to specify a name for the new certificate object that will be created and placed 
+               in a policy. Only valid for Trust Protection Platform.
+        :param pulumi.Input[str] pkcs12: A base64-encoded PKCS#12 keystore secured by the `key_password`. Useful when working with resources like 
+               azure key_vault_certificate.
         :param pulumi.Input[str] private_key_pem: The private key in PEM format.
-        :param pulumi.Input[int] rsa_bits: Number of bits to use when generating an RSA key.
-               Applies when `algorithm=RSA`.  Defaults to `2048`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] san_dns: List of DNS names to use as alternative
-               subjects of the certificate.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] san_emails: List of email addresses to use as
-               alternative subjects of the certificate.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] san_ips: List of IP addresses to use as alternative
-               subjects of the certificate.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] san_uris: List of Uniform Resource Identifiers (URIs) to use as alternative
-               subjects of the certificate.
-        :param pulumi.Input[int] valid_days: Desired number of days for which the new
-               certificate will be valid.
+        :param pulumi.Input[int] rsa_bits: Number of bits to use when generating an RSA key. Applies when algorithm is `RSA`. 
+               Defaults to `2048`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] san_dns: List of DNS names to use as alternative subjects of the certificate.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] san_emails: List of email addresses to use as alternative subjects of the certificate.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] san_ips: List of IP addresses to use as alternative subjects of the certificate.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] san_uris: List of Uniform Resource Identifiers (URIs) to use as alternative subjects of 
+               the certificate.
+        :param pulumi.Input[int] valid_days: Desired number of days for which the new certificate will be valid.
         """
         if algorithm is not None:
             pulumi.set(__self__, "algorithm", algorithm)
         if certificate is not None:
             pulumi.set(__self__, "certificate", certificate)
         if certificate_dn is not None:
             pulumi.set(__self__, "certificate_dn", certificate_dn)
@@ -443,16 +424,15 @@
         if valid_days is not None:
             pulumi.set(__self__, "valid_days", valid_days)
 
     @property
     @pulumi.getter
     def algorithm(self) -> Optional[pulumi.Input[str]]:
         """
-        Key encryption algorithm, either `RSA` or `ECDSA`.
-        Defaults to `RSA`.
+        Key encryption algorithm, either RSA or ECDSA. Defaults to `RSA`.
         """
         return pulumi.get(self, "algorithm")
 
     @algorithm.setter
     def algorithm(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "algorithm", value)
 
@@ -477,16 +457,15 @@
     def certificate_dn(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "certificate_dn", value)
 
     @property
     @pulumi.getter
     def chain(self) -> Optional[pulumi.Input[str]]:
         """
-        The trust chain of X509 certificate authority certificates in PEM format
-        concatenated together.
+        The trust chain of X509 certificate authority certificates in PEM format concatenated together.
         """
         return pulumi.get(self, "chain")
 
     @chain.setter
     def chain(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "chain", value)
 
@@ -502,15 +481,16 @@
     def common_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "common_name", value)
 
     @property
     @pulumi.getter(name="csrOrigin")
     def csr_origin(self) -> Optional[pulumi.Input[str]]:
         """
-        Whether key-pair generation will be `local` or `service` generated. Default is `local`.
+        Whether key-pair generation will be `local` or `service` generated. Default is 
+        `local`.
         """
         return pulumi.get(self, "csr_origin")
 
     @csr_origin.setter
     def csr_origin(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "csr_origin", value)
 
@@ -523,16 +503,15 @@
     def csr_pem(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "csr_pem", value)
 
     @property
     @pulumi.getter(name="customFields")
     def custom_fields(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        Collection of Custom Field name-value pairs to
-        assign to the certificate.
+        Collection of Custom Field name-value pairs to assign to the certificate.
         """
         return pulumi.get(self, "custom_fields")
 
     @custom_fields.setter
     def custom_fields(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "custom_fields", value)
 
@@ -548,30 +527,29 @@
     def ecdsa_curve(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ecdsa_curve", value)
 
     @property
     @pulumi.getter(name="expirationWindow")
     def expiration_window(self) -> Optional[pulumi.Input[int]]:
         """
-        Number of hours before certificate expiry
-        to request a new certificate.  Defaults to `168`.
+        Number of hours before certificate expiry to request a new certificate. 
+        Defaults to `168`.
         """
         return pulumi.get(self, "expiration_window")
 
     @expiration_window.setter
     def expiration_window(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "expiration_window", value)
 
     @property
     @pulumi.getter(name="issuerHint")
     def issuer_hint(self) -> Optional[pulumi.Input[str]]:
         """
-        Used with valid_days to indicate the target
-        issuer when using Trust Protection Platform.  Relevant values are: "DigiCert",
-        "Entrust", and "Microsoft".
+        Used with `valid_days` to indicate the target issuer when using Trust Protection 
+        Platform. Relevant values are: `DigiCert`, `Entrust`, and `Microsoft`.
         """
         return pulumi.get(self, "issuer_hint")
 
     @issuer_hint.setter
     def issuer_hint(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "issuer_hint", value)
 
@@ -587,29 +565,29 @@
     def key_password(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "key_password", value)
 
     @property
     @pulumi.getter
     def nickname(self) -> Optional[pulumi.Input[str]]:
         """
-        Use to specify a name for the new certificate object that will be created and placed in a policy. Only valid for TPP.
+        Use to specify a name for the new certificate object that will be created and placed 
+        in a policy. Only valid for Trust Protection Platform.
         """
         return pulumi.get(self, "nickname")
 
     @nickname.setter
     def nickname(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "nickname", value)
 
     @property
     @pulumi.getter
     def pkcs12(self) -> Optional[pulumi.Input[str]]:
         """
-        A base64-encoded PKCS#12 keystore secured by the `key_password`.
-        Useful when working with resources like
-        azurerm_key_vault_certificate.
+        A base64-encoded PKCS#12 keystore secured by the `key_password`. Useful when working with resources like 
+        azure key_vault_certificate.
         """
         return pulumi.get(self, "pkcs12")
 
     @pkcs12.setter
     def pkcs12(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "pkcs12", value)
 
@@ -625,81 +603,77 @@
     def private_key_pem(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "private_key_pem", value)
 
     @property
     @pulumi.getter(name="rsaBits")
     def rsa_bits(self) -> Optional[pulumi.Input[int]]:
         """
-        Number of bits to use when generating an RSA key.
-        Applies when `algorithm=RSA`.  Defaults to `2048`.
+        Number of bits to use when generating an RSA key. Applies when algorithm is `RSA`. 
+        Defaults to `2048`.
         """
         return pulumi.get(self, "rsa_bits")
 
     @rsa_bits.setter
     def rsa_bits(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "rsa_bits", value)
 
     @property
     @pulumi.getter(name="sanDns")
     def san_dns(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of DNS names to use as alternative
-        subjects of the certificate.
+        List of DNS names to use as alternative subjects of the certificate.
         """
         return pulumi.get(self, "san_dns")
 
     @san_dns.setter
     def san_dns(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "san_dns", value)
 
     @property
     @pulumi.getter(name="sanEmails")
     def san_emails(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of email addresses to use as
-        alternative subjects of the certificate.
+        List of email addresses to use as alternative subjects of the certificate.
         """
         return pulumi.get(self, "san_emails")
 
     @san_emails.setter
     def san_emails(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "san_emails", value)
 
     @property
     @pulumi.getter(name="sanIps")
     def san_ips(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of IP addresses to use as alternative
-        subjects of the certificate.
+        List of IP addresses to use as alternative subjects of the certificate.
         """
         return pulumi.get(self, "san_ips")
 
     @san_ips.setter
     def san_ips(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "san_ips", value)
 
     @property
     @pulumi.getter(name="sanUris")
     def san_uris(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of Uniform Resource Identifiers (URIs) to use as alternative
-        subjects of the certificate.
+        List of Uniform Resource Identifiers (URIs) to use as alternative subjects of 
+        the certificate.
         """
         return pulumi.get(self, "san_uris")
 
     @san_uris.setter
     def san_uris(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "san_uris", value)
 
     @property
     @pulumi.getter(name="validDays")
     def valid_days(self) -> Optional[pulumi.Input[int]]:
         """
-        Desired number of days for which the new
-        certificate will be valid.
+        Desired number of days for which the new certificate will be valid.
         """
         return pulumi.get(self, "valid_days")
 
     @valid_days.setter
     def valid_days(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "valid_days", value)
 
@@ -729,44 +703,38 @@
                  san_uris: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  valid_days: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
         Create a Certificate resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] algorithm: Key encryption algorithm, either `RSA` or `ECDSA`.
-               Defaults to `RSA`.
+        :param pulumi.Input[str] algorithm: Key encryption algorithm, either RSA or ECDSA. Defaults to `RSA`.
         :param pulumi.Input[str] common_name: The common name of the certificate.
-        :param pulumi.Input[str] csr_origin: Whether key-pair generation will be `local` or `service` generated. Default is `local`.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_fields: Collection of Custom Field name-value pairs to
-               assign to the certificate.
+        :param pulumi.Input[str] csr_origin: Whether key-pair generation will be `local` or `service` generated. Default is 
+               `local`.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_fields: Collection of Custom Field name-value pairs to assign to the certificate.
         :param pulumi.Input[str] ecdsa_curve: ECDSA curve to use when generating a key
-        :param pulumi.Input[int] expiration_window: Number of hours before certificate expiry
-               to request a new certificate.  Defaults to `168`.
-        :param pulumi.Input[str] issuer_hint: Used with valid_days to indicate the target
-               issuer when using Trust Protection Platform.  Relevant values are: "DigiCert",
-               "Entrust", and "Microsoft".
+        :param pulumi.Input[int] expiration_window: Number of hours before certificate expiry to request a new certificate. 
+               Defaults to `168`.
+        :param pulumi.Input[str] issuer_hint: Used with `valid_days` to indicate the target issuer when using Trust Protection 
+               Platform. Relevant values are: `DigiCert`, `Entrust`, and `Microsoft`.
         :param pulumi.Input[str] key_password: The password used to encrypt the private key.
-        :param pulumi.Input[str] nickname: Use to specify a name for the new certificate object that will be created and placed in a policy. Only valid for TPP.
-        :param pulumi.Input[str] pkcs12: A base64-encoded PKCS#12 keystore secured by the `key_password`.
-               Useful when working with resources like
-               azurerm_key_vault_certificate.
+        :param pulumi.Input[str] nickname: Use to specify a name for the new certificate object that will be created and placed 
+               in a policy. Only valid for Trust Protection Platform.
+        :param pulumi.Input[str] pkcs12: A base64-encoded PKCS#12 keystore secured by the `key_password`. Useful when working with resources like 
+               azure key_vault_certificate.
         :param pulumi.Input[str] private_key_pem: The private key in PEM format.
-        :param pulumi.Input[int] rsa_bits: Number of bits to use when generating an RSA key.
-               Applies when `algorithm=RSA`.  Defaults to `2048`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] san_dns: List of DNS names to use as alternative
-               subjects of the certificate.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] san_emails: List of email addresses to use as
-               alternative subjects of the certificate.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] san_ips: List of IP addresses to use as alternative
-               subjects of the certificate.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] san_uris: List of Uniform Resource Identifiers (URIs) to use as alternative
-               subjects of the certificate.
-        :param pulumi.Input[int] valid_days: Desired number of days for which the new
-               certificate will be valid.
+        :param pulumi.Input[int] rsa_bits: Number of bits to use when generating an RSA key. Applies when algorithm is `RSA`. 
+               Defaults to `2048`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] san_dns: List of DNS names to use as alternative subjects of the certificate.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] san_emails: List of email addresses to use as alternative subjects of the certificate.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] san_ips: List of IP addresses to use as alternative subjects of the certificate.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] san_uris: List of Uniform Resource Identifiers (URIs) to use as alternative subjects of 
+               the certificate.
+        :param pulumi.Input[int] valid_days: Desired number of days for which the new certificate will be valid.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: CertificateArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -874,47 +842,40 @@
         """
         Get an existing Certificate resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] algorithm: Key encryption algorithm, either `RSA` or `ECDSA`.
-               Defaults to `RSA`.
+        :param pulumi.Input[str] algorithm: Key encryption algorithm, either RSA or ECDSA. Defaults to `RSA`.
         :param pulumi.Input[str] certificate: The X509 certificate in PEM format.
-        :param pulumi.Input[str] chain: The trust chain of X509 certificate authority certificates in PEM format
-               concatenated together.
+        :param pulumi.Input[str] chain: The trust chain of X509 certificate authority certificates in PEM format concatenated together.
         :param pulumi.Input[str] common_name: The common name of the certificate.
-        :param pulumi.Input[str] csr_origin: Whether key-pair generation will be `local` or `service` generated. Default is `local`.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_fields: Collection of Custom Field name-value pairs to
-               assign to the certificate.
+        :param pulumi.Input[str] csr_origin: Whether key-pair generation will be `local` or `service` generated. Default is 
+               `local`.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] custom_fields: Collection of Custom Field name-value pairs to assign to the certificate.
         :param pulumi.Input[str] ecdsa_curve: ECDSA curve to use when generating a key
-        :param pulumi.Input[int] expiration_window: Number of hours before certificate expiry
-               to request a new certificate.  Defaults to `168`.
-        :param pulumi.Input[str] issuer_hint: Used with valid_days to indicate the target
-               issuer when using Trust Protection Platform.  Relevant values are: "DigiCert",
-               "Entrust", and "Microsoft".
+        :param pulumi.Input[int] expiration_window: Number of hours before certificate expiry to request a new certificate. 
+               Defaults to `168`.
+        :param pulumi.Input[str] issuer_hint: Used with `valid_days` to indicate the target issuer when using Trust Protection 
+               Platform. Relevant values are: `DigiCert`, `Entrust`, and `Microsoft`.
         :param pulumi.Input[str] key_password: The password used to encrypt the private key.
-        :param pulumi.Input[str] nickname: Use to specify a name for the new certificate object that will be created and placed in a policy. Only valid for TPP.
-        :param pulumi.Input[str] pkcs12: A base64-encoded PKCS#12 keystore secured by the `key_password`.
-               Useful when working with resources like
-               azurerm_key_vault_certificate.
+        :param pulumi.Input[str] nickname: Use to specify a name for the new certificate object that will be created and placed 
+               in a policy. Only valid for Trust Protection Platform.
+        :param pulumi.Input[str] pkcs12: A base64-encoded PKCS#12 keystore secured by the `key_password`. Useful when working with resources like 
+               azure key_vault_certificate.
         :param pulumi.Input[str] private_key_pem: The private key in PEM format.
-        :param pulumi.Input[int] rsa_bits: Number of bits to use when generating an RSA key.
-               Applies when `algorithm=RSA`.  Defaults to `2048`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] san_dns: List of DNS names to use as alternative
-               subjects of the certificate.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] san_emails: List of email addresses to use as
-               alternative subjects of the certificate.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] san_ips: List of IP addresses to use as alternative
-               subjects of the certificate.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] san_uris: List of Uniform Resource Identifiers (URIs) to use as alternative
-               subjects of the certificate.
-        :param pulumi.Input[int] valid_days: Desired number of days for which the new
-               certificate will be valid.
+        :param pulumi.Input[int] rsa_bits: Number of bits to use when generating an RSA key. Applies when algorithm is `RSA`. 
+               Defaults to `2048`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] san_dns: List of DNS names to use as alternative subjects of the certificate.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] san_emails: List of email addresses to use as alternative subjects of the certificate.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] san_ips: List of IP addresses to use as alternative subjects of the certificate.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] san_uris: List of Uniform Resource Identifiers (URIs) to use as alternative subjects of 
+               the certificate.
+        :param pulumi.Input[int] valid_days: Desired number of days for which the new certificate will be valid.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _CertificateState.__new__(_CertificateState)
 
         __props__.__dict__["algorithm"] = algorithm
         __props__.__dict__["certificate"] = certificate
@@ -939,16 +900,15 @@
         __props__.__dict__["valid_days"] = valid_days
         return Certificate(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def algorithm(self) -> pulumi.Output[Optional[str]]:
         """
-        Key encryption algorithm, either `RSA` or `ECDSA`.
-        Defaults to `RSA`.
+        Key encryption algorithm, either RSA or ECDSA. Defaults to `RSA`.
         """
         return pulumi.get(self, "algorithm")
 
     @property
     @pulumi.getter
     def certificate(self) -> pulumi.Output[str]:
         """
@@ -961,16 +921,15 @@
     def certificate_dn(self) -> pulumi.Output[str]:
         return pulumi.get(self, "certificate_dn")
 
     @property
     @pulumi.getter
     def chain(self) -> pulumi.Output[str]:
         """
-        The trust chain of X509 certificate authority certificates in PEM format
-        concatenated together.
+        The trust chain of X509 certificate authority certificates in PEM format concatenated together.
         """
         return pulumi.get(self, "chain")
 
     @property
     @pulumi.getter(name="commonName")
     def common_name(self) -> pulumi.Output[str]:
         """
@@ -978,29 +937,29 @@
         """
         return pulumi.get(self, "common_name")
 
     @property
     @pulumi.getter(name="csrOrigin")
     def csr_origin(self) -> pulumi.Output[Optional[str]]:
         """
-        Whether key-pair generation will be `local` or `service` generated. Default is `local`.
+        Whether key-pair generation will be `local` or `service` generated. Default is 
+        `local`.
         """
         return pulumi.get(self, "csr_origin")
 
     @property
     @pulumi.getter(name="csrPem")
     def csr_pem(self) -> pulumi.Output[str]:
         return pulumi.get(self, "csr_pem")
 
     @property
     @pulumi.getter(name="customFields")
     def custom_fields(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
-        Collection of Custom Field name-value pairs to
-        assign to the certificate.
+        Collection of Custom Field name-value pairs to assign to the certificate.
         """
         return pulumi.get(self, "custom_fields")
 
     @property
     @pulumi.getter(name="ecdsaCurve")
     def ecdsa_curve(self) -> pulumi.Output[Optional[str]]:
         """
@@ -1008,26 +967,25 @@
         """
         return pulumi.get(self, "ecdsa_curve")
 
     @property
     @pulumi.getter(name="expirationWindow")
     def expiration_window(self) -> pulumi.Output[Optional[int]]:
         """
-        Number of hours before certificate expiry
-        to request a new certificate.  Defaults to `168`.
+        Number of hours before certificate expiry to request a new certificate. 
+        Defaults to `168`.
         """
         return pulumi.get(self, "expiration_window")
 
     @property
     @pulumi.getter(name="issuerHint")
     def issuer_hint(self) -> pulumi.Output[Optional[str]]:
         """
-        Used with valid_days to indicate the target
-        issuer when using Trust Protection Platform.  Relevant values are: "DigiCert",
-        "Entrust", and "Microsoft".
+        Used with `valid_days` to indicate the target issuer when using Trust Protection 
+        Platform. Relevant values are: `DigiCert`, `Entrust`, and `Microsoft`.
         """
         return pulumi.get(self, "issuer_hint")
 
     @property
     @pulumi.getter(name="keyPassword")
     def key_password(self) -> pulumi.Output[Optional[str]]:
         """
@@ -1035,25 +993,25 @@
         """
         return pulumi.get(self, "key_password")
 
     @property
     @pulumi.getter
     def nickname(self) -> pulumi.Output[Optional[str]]:
         """
-        Use to specify a name for the new certificate object that will be created and placed in a policy. Only valid for TPP.
+        Use to specify a name for the new certificate object that will be created and placed 
+        in a policy. Only valid for Trust Protection Platform.
         """
         return pulumi.get(self, "nickname")
 
     @property
     @pulumi.getter
     def pkcs12(self) -> pulumi.Output[str]:
         """
-        A base64-encoded PKCS#12 keystore secured by the `key_password`.
-        Useful when working with resources like
-        azurerm_key_vault_certificate.
+        A base64-encoded PKCS#12 keystore secured by the `key_password`. Useful when working with resources like 
+        azure key_vault_certificate.
         """
         return pulumi.get(self, "pkcs12")
 
     @property
     @pulumi.getter(name="privateKeyPem")
     def private_key_pem(self) -> pulumi.Output[str]:
         """
@@ -1061,57 +1019,53 @@
         """
         return pulumi.get(self, "private_key_pem")
 
     @property
     @pulumi.getter(name="rsaBits")
     def rsa_bits(self) -> pulumi.Output[Optional[int]]:
         """
-        Number of bits to use when generating an RSA key.
-        Applies when `algorithm=RSA`.  Defaults to `2048`.
+        Number of bits to use when generating an RSA key. Applies when algorithm is `RSA`. 
+        Defaults to `2048`.
         """
         return pulumi.get(self, "rsa_bits")
 
     @property
     @pulumi.getter(name="sanDns")
     def san_dns(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        List of DNS names to use as alternative
-        subjects of the certificate.
+        List of DNS names to use as alternative subjects of the certificate.
         """
         return pulumi.get(self, "san_dns")
 
     @property
     @pulumi.getter(name="sanEmails")
     def san_emails(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        List of email addresses to use as
-        alternative subjects of the certificate.
+        List of email addresses to use as alternative subjects of the certificate.
         """
         return pulumi.get(self, "san_emails")
 
     @property
     @pulumi.getter(name="sanIps")
     def san_ips(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        List of IP addresses to use as alternative
-        subjects of the certificate.
+        List of IP addresses to use as alternative subjects of the certificate.
         """
         return pulumi.get(self, "san_ips")
 
     @property
     @pulumi.getter(name="sanUris")
     def san_uris(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        List of Uniform Resource Identifiers (URIs) to use as alternative
-        subjects of the certificate.
+        List of Uniform Resource Identifiers (URIs) to use as alternative subjects of 
+        the certificate.
         """
         return pulumi.get(self, "san_uris")
 
     @property
     @pulumi.getter(name="validDays")
     def valid_days(self) -> pulumi.Output[Optional[int]]:
         """
-        Desired number of days for which the new
-        certificate will be valid.
+        Desired number of days for which the new certificate will be valid.
         """
         return pulumi.get(self, "valid_days")
```

### Comparing `pulumi_venafi-1.9.0a1712991486/pulumi_venafi/config/__init__.pyi` & `pulumi_venafi-1.9.0a1713292049/pulumi_venafi/config/__init__.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 devMode: Optional[bool]
 """
 When set to true, the resulting certificate will be issued by an ephemeral, no trust CA rather than enrolling using
 Venafi as a Service or Trust Protection Platform. Useful for development and testing.
 """
 
-idpJwt: Optional[str]
+externalJwt: Optional[str]
 """
 JWT of the identity provider associated to the Venafi Control Plane service account that is granting the access token
 """
 
 p12CertFilename: Optional[str]
 """
 Filename of PKCS#12 keystore containing a client certificate, private key, and chain certificates to authenticate to
```

### Comparing `pulumi_venafi-1.9.0a1712991486/pulumi_venafi/config/vars.py` & `pulumi_venafi-1.9.0a1713292049/pulumi_venafi/config/vars.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,19 +41,19 @@
         """
         When set to true, the resulting certificate will be issued by an ephemeral, no trust CA rather than enrolling using
         Venafi as a Service or Trust Protection Platform. Useful for development and testing.
         """
         return __config__.get_bool('devMode')
 
     @property
-    def idp_jwt(self) -> Optional[str]:
+    def external_jwt(self) -> Optional[str]:
         """
         JWT of the identity provider associated to the Venafi Control Plane service account that is granting the access token
         """
-        return __config__.get('idpJwt')
+        return __config__.get('externalJwt')
 
     @property
     def p12_cert_filename(self) -> Optional[str]:
         """
         Filename of PKCS#12 keystore containing a client certificate, private key, and chain certificates to authenticate to
         TLSPDC
         """
```

### Comparing `pulumi_venafi-1.9.0a1712991486/pulumi_venafi/policy.py` & `pulumi_venafi-1.9.0a1713292049/pulumi_venafi/policy.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,45 +14,45 @@
 @pulumi.input_type
 class PolicyArgs:
     def __init__(__self__, *,
                  policy_specification: Optional[pulumi.Input[str]] = None,
                  zone: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Policy resource.
-        :param pulumi.Input[str] policy_specification: The JSON-formatted certificate policy
-               specification as documented [here](https://github.com/Venafi/vcert/blob/master/README-POLICY-SPEC.md).
-               Typically read from a file using the `file` function.
-        :param pulumi.Input[str] zone: The *Trust Protection Plaform* policy folder or
-               *Venafi as a Service* application and issuing template.
+        :param pulumi.Input[str] policy_specification: The JSON-formatted certificate policy specification as documented 
+               [here](https://github.com/Venafi/vcert/blob/master/README-POLICY-SPEC.md). Typically read from a file using the `file`
+               function.
+        :param pulumi.Input[str] zone: The *Trust Protection Plaform* policy folder or *Venafi Control Plane* application and 
+               issuing template.
         """
         if policy_specification is not None:
             pulumi.set(__self__, "policy_specification", policy_specification)
         if zone is not None:
             pulumi.set(__self__, "zone", zone)
 
     @property
     @pulumi.getter(name="policySpecification")
     def policy_specification(self) -> Optional[pulumi.Input[str]]:
         """
-        The JSON-formatted certificate policy
-        specification as documented [here](https://github.com/Venafi/vcert/blob/master/README-POLICY-SPEC.md).
-        Typically read from a file using the `file` function.
+        The JSON-formatted certificate policy specification as documented 
+        [here](https://github.com/Venafi/vcert/blob/master/README-POLICY-SPEC.md). Typically read from a file using the `file`
+        function.
         """
         return pulumi.get(self, "policy_specification")
 
     @policy_specification.setter
     def policy_specification(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "policy_specification", value)
 
     @property
     @pulumi.getter
     def zone(self) -> Optional[pulumi.Input[str]]:
         """
-        The *Trust Protection Plaform* policy folder or
-        *Venafi as a Service* application and issuing template.
+        The *Trust Protection Plaform* policy folder or *Venafi Control Plane* application and 
+        issuing template.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "zone", value)
 
@@ -60,45 +60,45 @@
 @pulumi.input_type
 class _PolicyState:
     def __init__(__self__, *,
                  policy_specification: Optional[pulumi.Input[str]] = None,
                  zone: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Policy resources.
-        :param pulumi.Input[str] policy_specification: The JSON-formatted certificate policy
-               specification as documented [here](https://github.com/Venafi/vcert/blob/master/README-POLICY-SPEC.md).
-               Typically read from a file using the `file` function.
-        :param pulumi.Input[str] zone: The *Trust Protection Plaform* policy folder or
-               *Venafi as a Service* application and issuing template.
+        :param pulumi.Input[str] policy_specification: The JSON-formatted certificate policy specification as documented 
+               [here](https://github.com/Venafi/vcert/blob/master/README-POLICY-SPEC.md). Typically read from a file using the `file`
+               function.
+        :param pulumi.Input[str] zone: The *Trust Protection Plaform* policy folder or *Venafi Control Plane* application and 
+               issuing template.
         """
         if policy_specification is not None:
             pulumi.set(__self__, "policy_specification", policy_specification)
         if zone is not None:
             pulumi.set(__self__, "zone", zone)
 
     @property
     @pulumi.getter(name="policySpecification")
     def policy_specification(self) -> Optional[pulumi.Input[str]]:
         """
-        The JSON-formatted certificate policy
-        specification as documented [here](https://github.com/Venafi/vcert/blob/master/README-POLICY-SPEC.md).
-        Typically read from a file using the `file` function.
+        The JSON-formatted certificate policy specification as documented 
+        [here](https://github.com/Venafi/vcert/blob/master/README-POLICY-SPEC.md). Typically read from a file using the `file`
+        function.
         """
         return pulumi.get(self, "policy_specification")
 
     @policy_specification.setter
     def policy_specification(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "policy_specification", value)
 
     @property
     @pulumi.getter
     def zone(self) -> Optional[pulumi.Input[str]]:
         """
-        The *Trust Protection Plaform* policy folder or
-        *Venafi as a Service* application and issuing template.
+        The *Trust Protection Plaform* policy folder or *Venafi Control Plane* application and 
+        issuing template.
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "zone", value)
 
@@ -108,17 +108,16 @@
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  policy_specification: Optional[pulumi.Input[str]] = None,
                  zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Provides access to read and write certificate policy in Venafi. This can be used
-        to define a new policy (folder in *Trust Protection Platform*; application
-        and/or issuing template in *Venafi as a Service*).
+        Provides access to read and write certificate policy in Venafi. This can be used to define a new policy (folder in
+        *Trust Protection Platform*; application and issuing template in *Venafi Control Plane*).
 
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_venafi as venafi
@@ -127,52 +126,47 @@
             zone="My Business App\\\\Enterprise Trusted Certs",
             policy_specification=(lambda path: open(path).read())("/path-to/internal-policy.json"))
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
-        The `venafi_policy` resource supports the Terraform import
+        The `venafi_policy` resource supports the Terraform import method.
 
-        method.  When used, the `zone` and `policy_specification` resource arguments
+        When used, the `zone` and `policy_specification` resource arguments are not required since the zone is a required
 
-        are not required since the zone is a required parameter of the import method
+        parameter of the import method and the policy specification is populated from the existing infrastructure. Policy that
 
-        and the policy specification is populated from the existing infrastructure.
-
-        Policy that is successfully imported is also output to a file named after the
-
-        zone that was specified.
+        is successfully imported is also output to a file named after the zone that was specified.
 
         hcl
 
         resource "venafi_policy" "existing_policy" {}
 
         ```sh
         $ pulumi import venafi:index/policy:Policy existing_policy" "My Business App\\\\Enterprise Trusted Certs"
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] policy_specification: The JSON-formatted certificate policy
-               specification as documented [here](https://github.com/Venafi/vcert/blob/master/README-POLICY-SPEC.md).
-               Typically read from a file using the `file` function.
-        :param pulumi.Input[str] zone: The *Trust Protection Plaform* policy folder or
-               *Venafi as a Service* application and issuing template.
+        :param pulumi.Input[str] policy_specification: The JSON-formatted certificate policy specification as documented 
+               [here](https://github.com/Venafi/vcert/blob/master/README-POLICY-SPEC.md). Typically read from a file using the `file`
+               function.
+        :param pulumi.Input[str] zone: The *Trust Protection Plaform* policy folder or *Venafi Control Plane* application and 
+               issuing template.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[PolicyArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Provides access to read and write certificate policy in Venafi. This can be used
-        to define a new policy (folder in *Trust Protection Platform*; application
-        and/or issuing template in *Venafi as a Service*).
+        Provides access to read and write certificate policy in Venafi. This can be used to define a new policy (folder in
+        *Trust Protection Platform*; application and issuing template in *Venafi Control Plane*).
 
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_venafi as venafi
@@ -181,25 +175,21 @@
             zone="My Business App\\\\Enterprise Trusted Certs",
             policy_specification=(lambda path: open(path).read())("/path-to/internal-policy.json"))
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
-        The `venafi_policy` resource supports the Terraform import
-
-        method.  When used, the `zone` and `policy_specification` resource arguments
-
-        are not required since the zone is a required parameter of the import method
+        The `venafi_policy` resource supports the Terraform import method.
 
-        and the policy specification is populated from the existing infrastructure.
+        When used, the `zone` and `policy_specification` resource arguments are not required since the zone is a required
 
-        Policy that is successfully imported is also output to a file named after the
+        parameter of the import method and the policy specification is populated from the existing infrastructure. Policy that
 
-        zone that was specified.
+        is successfully imported is also output to a file named after the zone that was specified.
 
         hcl
 
         resource "venafi_policy" "existing_policy" {}
 
         ```sh
         $ pulumi import venafi:index/policy:Policy existing_policy" "My Business App\\\\Enterprise Trusted Certs"
@@ -248,40 +238,40 @@
         """
         Get an existing Policy resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] policy_specification: The JSON-formatted certificate policy
-               specification as documented [here](https://github.com/Venafi/vcert/blob/master/README-POLICY-SPEC.md).
-               Typically read from a file using the `file` function.
-        :param pulumi.Input[str] zone: The *Trust Protection Plaform* policy folder or
-               *Venafi as a Service* application and issuing template.
+        :param pulumi.Input[str] policy_specification: The JSON-formatted certificate policy specification as documented 
+               [here](https://github.com/Venafi/vcert/blob/master/README-POLICY-SPEC.md). Typically read from a file using the `file`
+               function.
+        :param pulumi.Input[str] zone: The *Trust Protection Plaform* policy folder or *Venafi Control Plane* application and 
+               issuing template.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _PolicyState.__new__(_PolicyState)
 
         __props__.__dict__["policy_specification"] = policy_specification
         __props__.__dict__["zone"] = zone
         return Policy(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="policySpecification")
     def policy_specification(self) -> pulumi.Output[Optional[str]]:
         """
-        The JSON-formatted certificate policy
-        specification as documented [here](https://github.com/Venafi/vcert/blob/master/README-POLICY-SPEC.md).
-        Typically read from a file using the `file` function.
+        The JSON-formatted certificate policy specification as documented 
+        [here](https://github.com/Venafi/vcert/blob/master/README-POLICY-SPEC.md). Typically read from a file using the `file`
+        function.
         """
         return pulumi.get(self, "policy_specification")
 
     @property
     @pulumi.getter
     def zone(self) -> pulumi.Output[Optional[str]]:
         """
-        The *Trust Protection Plaform* policy folder or
-        *Venafi as a Service* application and issuing template.
+        The *Trust Protection Plaform* policy folder or *Venafi Control Plane* application and 
+        issuing template.
         """
         return pulumi.get(self, "zone")
```

### Comparing `pulumi_venafi-1.9.0a1712991486/pulumi_venafi/provider.py` & `pulumi_venafi-1.9.0a1713292049/pulumi_venafi/provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 @pulumi.input_type
 class ProviderArgs:
     def __init__(__self__, *,
                  access_token: Optional[pulumi.Input[str]] = None,
                  api_key: Optional[pulumi.Input[str]] = None,
                  client_id: Optional[pulumi.Input[str]] = None,
                  dev_mode: Optional[pulumi.Input[bool]] = None,
-                 idp_jwt: Optional[pulumi.Input[str]] = None,
+                 external_jwt: Optional[pulumi.Input[str]] = None,
                  p12_cert_filename: Optional[pulumi.Input[str]] = None,
                  p12_cert_password: Optional[pulumi.Input[str]] = None,
                  skip_retirement: Optional[pulumi.Input[bool]] = None,
                  token_url: Optional[pulumi.Input[str]] = None,
                  tpp_password: Optional[pulumi.Input[str]] = None,
                  tpp_username: Optional[pulumi.Input[str]] = None,
                  trust_bundle: Optional[pulumi.Input[str]] = None,
@@ -31,15 +31,15 @@
         """
         The set of arguments for constructing a Provider resource.
         :param pulumi.Input[str] access_token: Access token for Venafi TLSPDC, user should use this for authentication
         :param pulumi.Input[str] api_key: API key for Venafi Control Plane. Example: 142231b7-cvb0-412e-886b-6aeght0bc93d
         :param pulumi.Input[str] client_id: application that will be using the token
         :param pulumi.Input[bool] dev_mode: When set to true, the resulting certificate will be issued by an ephemeral, no trust CA rather than enrolling using
                Venafi as a Service or Trust Protection Platform. Useful for development and testing.
-        :param pulumi.Input[str] idp_jwt: JWT of the identity provider associated to the Venafi Control Plane service account that is granting the access token
+        :param pulumi.Input[str] external_jwt: JWT of the identity provider associated to the Venafi Control Plane service account that is granting the access token
         :param pulumi.Input[str] p12_cert_filename: Filename of PKCS#12 keystore containing a client certificate, private key, and chain certificates to authenticate to
                TLSPDC
         :param pulumi.Input[str] p12_cert_password: Password for the PKCS#12 keystore declared in p12_cert
         :param pulumi.Input[bool] skip_retirement: When true, certificates will not be retired on Venafi platforms when terraform destroy is run. Default is false.
         :param pulumi.Input[str] token_url: Endpoint URL to request new Venafi Control Plane access tokens
         :param pulumi.Input[str] tpp_password: Password for WebSDK user. Example: password
         :param pulumi.Input[str] tpp_username: WebSDK user for Venafi TLSPDC. Example: admin
@@ -53,16 +53,16 @@
             pulumi.set(__self__, "access_token", access_token)
         if api_key is not None:
             pulumi.set(__self__, "api_key", api_key)
         if client_id is not None:
             pulumi.set(__self__, "client_id", client_id)
         if dev_mode is not None:
             pulumi.set(__self__, "dev_mode", dev_mode)
-        if idp_jwt is not None:
-            pulumi.set(__self__, "idp_jwt", idp_jwt)
+        if external_jwt is not None:
+            pulumi.set(__self__, "external_jwt", external_jwt)
         if p12_cert_filename is not None:
             pulumi.set(__self__, "p12_cert_filename", p12_cert_filename)
         if p12_cert_password is not None:
             pulumi.set(__self__, "p12_cert_password", p12_cert_password)
         if skip_retirement is not None:
             pulumi.set(__self__, "skip_retirement", skip_retirement)
         if token_url is not None:
@@ -130,24 +130,24 @@
         return pulumi.get(self, "dev_mode")
 
     @dev_mode.setter
     def dev_mode(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "dev_mode", value)
 
     @property
-    @pulumi.getter(name="idpJwt")
-    def idp_jwt(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="externalJwt")
+    def external_jwt(self) -> Optional[pulumi.Input[str]]:
         """
         JWT of the identity provider associated to the Venafi Control Plane service account that is granting the access token
         """
-        return pulumi.get(self, "idp_jwt")
+        return pulumi.get(self, "external_jwt")
 
-    @idp_jwt.setter
-    def idp_jwt(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "idp_jwt", value)
+    @external_jwt.setter
+    def external_jwt(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "external_jwt", value)
 
     @property
     @pulumi.getter(name="p12CertFilename")
     def p12_cert_filename(self) -> Optional[pulumi.Input[str]]:
         """
         Filename of PKCS#12 keystore containing a client certificate, private key, and chain certificates to authenticate to
         TLSPDC
@@ -268,15 +268,15 @@
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  access_token: Optional[pulumi.Input[str]] = None,
                  api_key: Optional[pulumi.Input[str]] = None,
                  client_id: Optional[pulumi.Input[str]] = None,
                  dev_mode: Optional[pulumi.Input[bool]] = None,
-                 idp_jwt: Optional[pulumi.Input[str]] = None,
+                 external_jwt: Optional[pulumi.Input[str]] = None,
                  p12_cert_filename: Optional[pulumi.Input[str]] = None,
                  p12_cert_password: Optional[pulumi.Input[str]] = None,
                  skip_retirement: Optional[pulumi.Input[bool]] = None,
                  token_url: Optional[pulumi.Input[str]] = None,
                  tpp_password: Optional[pulumi.Input[str]] = None,
                  tpp_username: Optional[pulumi.Input[str]] = None,
                  trust_bundle: Optional[pulumi.Input[str]] = None,
@@ -292,15 +292,15 @@
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] access_token: Access token for Venafi TLSPDC, user should use this for authentication
         :param pulumi.Input[str] api_key: API key for Venafi Control Plane. Example: 142231b7-cvb0-412e-886b-6aeght0bc93d
         :param pulumi.Input[str] client_id: application that will be using the token
         :param pulumi.Input[bool] dev_mode: When set to true, the resulting certificate will be issued by an ephemeral, no trust CA rather than enrolling using
                Venafi as a Service or Trust Protection Platform. Useful for development and testing.
-        :param pulumi.Input[str] idp_jwt: JWT of the identity provider associated to the Venafi Control Plane service account that is granting the access token
+        :param pulumi.Input[str] external_jwt: JWT of the identity provider associated to the Venafi Control Plane service account that is granting the access token
         :param pulumi.Input[str] p12_cert_filename: Filename of PKCS#12 keystore containing a client certificate, private key, and chain certificates to authenticate to
                TLSPDC
         :param pulumi.Input[str] p12_cert_password: Password for the PKCS#12 keystore declared in p12_cert
         :param pulumi.Input[bool] skip_retirement: When true, certificates will not be retired on Venafi platforms when terraform destroy is run. Default is false.
         :param pulumi.Input[str] token_url: Endpoint URL to request new Venafi Control Plane access tokens
         :param pulumi.Input[str] tpp_password: Password for WebSDK user. Example: password
         :param pulumi.Input[str] tpp_username: WebSDK user for Venafi TLSPDC. Example: admin
@@ -337,15 +337,15 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  access_token: Optional[pulumi.Input[str]] = None,
                  api_key: Optional[pulumi.Input[str]] = None,
                  client_id: Optional[pulumi.Input[str]] = None,
                  dev_mode: Optional[pulumi.Input[bool]] = None,
-                 idp_jwt: Optional[pulumi.Input[str]] = None,
+                 external_jwt: Optional[pulumi.Input[str]] = None,
                  p12_cert_filename: Optional[pulumi.Input[str]] = None,
                  p12_cert_password: Optional[pulumi.Input[str]] = None,
                  skip_retirement: Optional[pulumi.Input[bool]] = None,
                  token_url: Optional[pulumi.Input[str]] = None,
                  tpp_password: Optional[pulumi.Input[str]] = None,
                  tpp_username: Optional[pulumi.Input[str]] = None,
                  trust_bundle: Optional[pulumi.Input[str]] = None,
@@ -360,25 +360,25 @@
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProviderArgs.__new__(ProviderArgs)
 
             __props__.__dict__["access_token"] = None if access_token is None else pulumi.Output.secret(access_token)
             __props__.__dict__["api_key"] = None if api_key is None else pulumi.Output.secret(api_key)
             __props__.__dict__["client_id"] = client_id
             __props__.__dict__["dev_mode"] = pulumi.Output.from_input(dev_mode).apply(pulumi.runtime.to_json) if dev_mode is not None else None
-            __props__.__dict__["idp_jwt"] = None if idp_jwt is None else pulumi.Output.secret(idp_jwt)
+            __props__.__dict__["external_jwt"] = None if external_jwt is None else pulumi.Output.secret(external_jwt)
             __props__.__dict__["p12_cert_filename"] = p12_cert_filename
             __props__.__dict__["p12_cert_password"] = None if p12_cert_password is None else pulumi.Output.secret(p12_cert_password)
             __props__.__dict__["skip_retirement"] = pulumi.Output.from_input(skip_retirement).apply(pulumi.runtime.to_json) if skip_retirement is not None else None
             __props__.__dict__["token_url"] = None if token_url is None else pulumi.Output.secret(token_url)
             __props__.__dict__["tpp_password"] = None if tpp_password is None else pulumi.Output.secret(tpp_password)
             __props__.__dict__["tpp_username"] = tpp_username
             __props__.__dict__["trust_bundle"] = trust_bundle
             __props__.__dict__["url"] = url
             __props__.__dict__["zone"] = zone
-        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["accessToken", "apiKey", "idpJwt", "p12CertPassword", "tokenUrl", "tppPassword"])
+        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["accessToken", "apiKey", "externalJwt", "p12CertPassword", "tokenUrl", "tppPassword"])
         opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(Provider, __self__).__init__(
             'venafi',
             resource_name,
             __props__,
             opts)
 
@@ -403,20 +403,20 @@
     def client_id(self) -> pulumi.Output[Optional[str]]:
         """
         application that will be using the token
         """
         return pulumi.get(self, "client_id")
 
     @property
-    @pulumi.getter(name="idpJwt")
-    def idp_jwt(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="externalJwt")
+    def external_jwt(self) -> pulumi.Output[Optional[str]]:
         """
         JWT of the identity provider associated to the Venafi Control Plane service account that is granting the access token
         """
-        return pulumi.get(self, "idp_jwt")
+        return pulumi.get(self, "external_jwt")
 
     @property
     @pulumi.getter(name="p12CertFilename")
     def p12_cert_filename(self) -> pulumi.Output[Optional[str]]:
         """
         Filename of PKCS#12 keystore containing a client certificate, private key, and chain certificates to authenticate to
         TLSPDC
```

### Comparing `pulumi_venafi-1.9.0a1712991486/pulumi_venafi/ssh_certificate.py` & `pulumi_venafi-1.9.0a1713292049/pulumi_venafi/ssh_certificate.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,26 +30,34 @@
                  source_addresses: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  valid_hours: Optional[pulumi.Input[int]] = None,
                  windows: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a SshCertificate resource.
         :param pulumi.Input[str] key_id: The identifier of the requested SSH certificate.
         :param pulumi.Input[str] template: The SSH certificate issuing template.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] destination_addresses: A list of one or more valid IP or CIDR destination hosts where the certificate will authenticate.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] extensions: A list of key-value pairs that contain certificate extensions from the CA template for client certificates. Allowed values (case-sensitive): *permit-X11-forwarding, permit-agent-forwarding, permit-port-forwarding, permit-pty, permit-user-rc*
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] destination_addresses: A list of one or more valid IP or CIDR destination hosts where the 
+               certificate will authenticate.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] extensions: A list of key-value pairs that contain certificate extensions from the CA 
+               template for client certificates. Allowed values (case-sensitive): `permit-X11-forwarding`, `permit-agent-forwarding`,
+               `permit-port-forwarding`, `permit-pty`, `permit-user-rc`.
         :param pulumi.Input[str] folder: The DN of the policy folder where the SSH certificate object will be created.
         :param pulumi.Input[str] force_command: A command to run after successful login.
         :param pulumi.Input[str] key_passphrase: Passphrase for encrypting the private key.
-        :param pulumi.Input[int] key_size: Number of bits to use when creating a key pair. (e.g. 3072)
-        :param pulumi.Input[str] object_name: The friendly name of the SSH certificate object. When not specified the `key_id` is used for the friendly name. If the object already exists the old certificate is archived and the CA issues a new certificate.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] principal: [DEPRECATED] - (Optional, set of strings) Use "principals" instead. A list of user names for whom the requested certificate will be valid.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] principals: A list of user names for whom the requested certificate will be valid.
+        :param pulumi.Input[int] key_size: Number of bits to use when creating a key pair. (e.g. `3072`).
+        :param pulumi.Input[str] object_name: The friendly name of the SSH certificate object. When not specified the `key_id` 
+               is used for the friendly name. If the object already exists the old certificate is archived and the CA issues a new
+               certificate.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] principal: [DEPRECATED] - (Optional, set of strings) Use "principals" instead. A list of usernames for whom the 
+               requested certificate will be valid.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] principals: A list of usernames for whom the requested certificate will be valid.
         :param pulumi.Input[str] public_key: The OpenSSH formatted public key that will be used to generate the SSH certificate.
-        :param pulumi.Input[str] public_key_method: Specifies whether the public key will be "local" (default), "file" or "service" generated.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] source_addresses: A list of one or more valid IP or CIDR addresses that can use the SSH certificate.
+        :param pulumi.Input[str] public_key_method: Specifies whether the public key will be `local` (default), `file` or 
+               `service` generated.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] source_addresses: A list of one or more valid IP or CIDR addresses that can use the SSH 
+               certificate.
         :param pulumi.Input[int] valid_hours: Desired number of hours for which the certificate will be valid.
         :param pulumi.Input[bool] windows: Specifies whether the private key will use Windows/DOS style line breaks.
         """
         pulumi.set(__self__, "key_id", key_id)
         pulumi.set(__self__, "template", template)
         if destination_addresses is not None:
             pulumi.set(__self__, "destination_addresses", destination_addresses)
@@ -107,27 +115,30 @@
     def template(self, value: pulumi.Input[str]):
         pulumi.set(self, "template", value)
 
     @property
     @pulumi.getter(name="destinationAddresses")
     def destination_addresses(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of one or more valid IP or CIDR destination hosts where the certificate will authenticate.
+        A list of one or more valid IP or CIDR destination hosts where the 
+        certificate will authenticate.
         """
         return pulumi.get(self, "destination_addresses")
 
     @destination_addresses.setter
     def destination_addresses(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "destination_addresses", value)
 
     @property
     @pulumi.getter
     def extensions(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of key-value pairs that contain certificate extensions from the CA template for client certificates. Allowed values (case-sensitive): *permit-X11-forwarding, permit-agent-forwarding, permit-port-forwarding, permit-pty, permit-user-rc*
+        A list of key-value pairs that contain certificate extensions from the CA 
+        template for client certificates. Allowed values (case-sensitive): `permit-X11-forwarding`, `permit-agent-forwarding`,
+        `permit-port-forwarding`, `permit-pty`, `permit-user-rc`.
         """
         return pulumi.get(self, "extensions")
 
     @extensions.setter
     def extensions(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "extensions", value)
 
@@ -167,54 +178,57 @@
     def key_passphrase(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "key_passphrase", value)
 
     @property
     @pulumi.getter(name="keySize")
     def key_size(self) -> Optional[pulumi.Input[int]]:
         """
-        Number of bits to use when creating a key pair. (e.g. 3072)
+        Number of bits to use when creating a key pair. (e.g. `3072`).
         """
         return pulumi.get(self, "key_size")
 
     @key_size.setter
     def key_size(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "key_size", value)
 
     @property
     @pulumi.getter(name="objectName")
     def object_name(self) -> Optional[pulumi.Input[str]]:
         """
-        The friendly name of the SSH certificate object. When not specified the `key_id` is used for the friendly name. If the object already exists the old certificate is archived and the CA issues a new certificate.
+        The friendly name of the SSH certificate object. When not specified the `key_id` 
+        is used for the friendly name. If the object already exists the old certificate is archived and the CA issues a new
+        certificate.
         """
         return pulumi.get(self, "object_name")
 
     @object_name.setter
     def object_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "object_name", value)
 
     @property
     @pulumi.getter
     def principal(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        [DEPRECATED] - (Optional, set of strings) Use "principals" instead. A list of user names for whom the requested certificate will be valid.
+        [DEPRECATED] - (Optional, set of strings) Use "principals" instead. A list of usernames for whom the 
+        requested certificate will be valid.
         """
         warnings.warn("""This will be removed in the future. Use \"principals\" instead""", DeprecationWarning)
         pulumi.log.warn("""principal is deprecated: This will be removed in the future. Use \"principals\" instead""")
 
         return pulumi.get(self, "principal")
 
     @principal.setter
     def principal(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "principal", value)
 
     @property
     @pulumi.getter
     def principals(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of user names for whom the requested certificate will be valid.
+        A list of usernames for whom the requested certificate will be valid.
         """
         return pulumi.get(self, "principals")
 
     @principals.setter
     def principals(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "principals", value)
 
@@ -230,27 +244,29 @@
     def public_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "public_key", value)
 
     @property
     @pulumi.getter(name="publicKeyMethod")
     def public_key_method(self) -> Optional[pulumi.Input[str]]:
         """
-        Specifies whether the public key will be "local" (default), "file" or "service" generated.
+        Specifies whether the public key will be `local` (default), `file` or 
+        `service` generated.
         """
         return pulumi.get(self, "public_key_method")
 
     @public_key_method.setter
     def public_key_method(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "public_key_method", value)
 
     @property
     @pulumi.getter(name="sourceAddresses")
     def source_addresses(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of one or more valid IP or CIDR addresses that can use the SSH certificate.
+        A list of one or more valid IP or CIDR addresses that can use the SSH 
+        certificate.
         """
         return pulumi.get(self, "source_addresses")
 
     @source_addresses.setter
     def source_addresses(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "source_addresses", value)
 
@@ -306,31 +322,39 @@
                  valid_hours: Optional[pulumi.Input[int]] = None,
                  valid_to: Optional[pulumi.Input[str]] = None,
                  windows: Optional[pulumi.Input[bool]] = None):
         """
         Input properties used for looking up and filtering SshCertificate resources.
         :param pulumi.Input[str] certificate: The issued SSH certificate.
         :param pulumi.Input[str] certificate_type: Indicates whether the SSH certificate is for client or server authentication.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] destination_addresses: A list of one or more valid IP or CIDR destination hosts where the certificate will authenticate.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] extensions: A list of key-value pairs that contain certificate extensions from the CA template for client certificates. Allowed values (case-sensitive): *permit-X11-forwarding, permit-agent-forwarding, permit-port-forwarding, permit-pty, permit-user-rc*
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] destination_addresses: A list of one or more valid IP or CIDR destination hosts where the 
+               certificate will authenticate.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] extensions: A list of key-value pairs that contain certificate extensions from the CA 
+               template for client certificates. Allowed values (case-sensitive): `permit-X11-forwarding`, `permit-agent-forwarding`,
+               `permit-port-forwarding`, `permit-pty`, `permit-user-rc`.
         :param pulumi.Input[str] folder: The DN of the policy folder where the SSH certificate object will be created.
         :param pulumi.Input[str] force_command: A command to run after successful login.
         :param pulumi.Input[str] key_id: The identifier of the requested SSH certificate.
         :param pulumi.Input[str] key_passphrase: Passphrase for encrypting the private key.
-        :param pulumi.Input[int] key_size: Number of bits to use when creating a key pair. (e.g. 3072)
-        :param pulumi.Input[str] object_name: The friendly name of the SSH certificate object. When not specified the `key_id` is used for the friendly name. If the object already exists the old certificate is archived and the CA issues a new certificate.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] principal: [DEPRECATED] - (Optional, set of strings) Use "principals" instead. A list of user names for whom the requested certificate will be valid.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] principals: A list of user names for whom the requested certificate will be valid.
+        :param pulumi.Input[int] key_size: Number of bits to use when creating a key pair. (e.g. `3072`).
+        :param pulumi.Input[str] object_name: The friendly name of the SSH certificate object. When not specified the `key_id` 
+               is used for the friendly name. If the object already exists the old certificate is archived and the CA issues a new
+               certificate.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] principal: [DEPRECATED] - (Optional, set of strings) Use "principals" instead. A list of usernames for whom the 
+               requested certificate will be valid.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] principals: A list of usernames for whom the requested certificate will be valid.
         :param pulumi.Input[str] private_key: The private key for the SSH certificate if generated by Venafi.
         :param pulumi.Input[str] public_key: The OpenSSH formatted public key that will be used to generate the SSH certificate.
         :param pulumi.Input[str] public_key_fingerprint: The SHA256 fingerprint of the SSH certificate's public key.
-        :param pulumi.Input[str] public_key_method: Specifies whether the public key will be "local" (default), "file" or "service" generated.
+        :param pulumi.Input[str] public_key_method: Specifies whether the public key will be `local` (default), `file` or 
+               `service` generated.
         :param pulumi.Input[str] serial: The serial number of the SSH certificate.
         :param pulumi.Input[str] signing_ca: The SHA256 fingerprint of the CA that signed the SSH certificate.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] source_addresses: A list of one or more valid IP or CIDR addresses that can use the SSH certificate.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] source_addresses: A list of one or more valid IP or CIDR addresses that can use the SSH 
+               certificate.
         :param pulumi.Input[str] template: The SSH certificate issuing template.
         :param pulumi.Input[str] valid_from: The date the SSH certificate was issued.
         :param pulumi.Input[int] valid_hours: Desired number of hours for which the certificate will be valid.
         :param pulumi.Input[str] valid_to: The date the SSH certificate will expire.
         :param pulumi.Input[bool] windows: Specifies whether the private key will use Windows/DOS style line breaks.
         """
         if certificate is not None:
@@ -409,27 +433,30 @@
     def certificate_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "certificate_type", value)
 
     @property
     @pulumi.getter(name="destinationAddresses")
     def destination_addresses(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of one or more valid IP or CIDR destination hosts where the certificate will authenticate.
+        A list of one or more valid IP or CIDR destination hosts where the 
+        certificate will authenticate.
         """
         return pulumi.get(self, "destination_addresses")
 
     @destination_addresses.setter
     def destination_addresses(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "destination_addresses", value)
 
     @property
     @pulumi.getter
     def extensions(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of key-value pairs that contain certificate extensions from the CA template for client certificates. Allowed values (case-sensitive): *permit-X11-forwarding, permit-agent-forwarding, permit-port-forwarding, permit-pty, permit-user-rc*
+        A list of key-value pairs that contain certificate extensions from the CA 
+        template for client certificates. Allowed values (case-sensitive): `permit-X11-forwarding`, `permit-agent-forwarding`,
+        `permit-port-forwarding`, `permit-pty`, `permit-user-rc`.
         """
         return pulumi.get(self, "extensions")
 
     @extensions.setter
     def extensions(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "extensions", value)
 
@@ -481,54 +508,57 @@
     def key_passphrase(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "key_passphrase", value)
 
     @property
     @pulumi.getter(name="keySize")
     def key_size(self) -> Optional[pulumi.Input[int]]:
         """
-        Number of bits to use when creating a key pair. (e.g. 3072)
+        Number of bits to use when creating a key pair. (e.g. `3072`).
         """
         return pulumi.get(self, "key_size")
 
     @key_size.setter
     def key_size(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "key_size", value)
 
     @property
     @pulumi.getter(name="objectName")
     def object_name(self) -> Optional[pulumi.Input[str]]:
         """
-        The friendly name of the SSH certificate object. When not specified the `key_id` is used for the friendly name. If the object already exists the old certificate is archived and the CA issues a new certificate.
+        The friendly name of the SSH certificate object. When not specified the `key_id` 
+        is used for the friendly name. If the object already exists the old certificate is archived and the CA issues a new
+        certificate.
         """
         return pulumi.get(self, "object_name")
 
     @object_name.setter
     def object_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "object_name", value)
 
     @property
     @pulumi.getter
     def principal(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        [DEPRECATED] - (Optional, set of strings) Use "principals" instead. A list of user names for whom the requested certificate will be valid.
+        [DEPRECATED] - (Optional, set of strings) Use "principals" instead. A list of usernames for whom the 
+        requested certificate will be valid.
         """
         warnings.warn("""This will be removed in the future. Use \"principals\" instead""", DeprecationWarning)
         pulumi.log.warn("""principal is deprecated: This will be removed in the future. Use \"principals\" instead""")
 
         return pulumi.get(self, "principal")
 
     @principal.setter
     def principal(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "principal", value)
 
     @property
     @pulumi.getter
     def principals(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of user names for whom the requested certificate will be valid.
+        A list of usernames for whom the requested certificate will be valid.
         """
         return pulumi.get(self, "principals")
 
     @principals.setter
     def principals(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "principals", value)
 
@@ -568,15 +598,16 @@
     def public_key_fingerprint(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "public_key_fingerprint", value)
 
     @property
     @pulumi.getter(name="publicKeyMethod")
     def public_key_method(self) -> Optional[pulumi.Input[str]]:
         """
-        Specifies whether the public key will be "local" (default), "file" or "service" generated.
+        Specifies whether the public key will be `local` (default), `file` or 
+        `service` generated.
         """
         return pulumi.get(self, "public_key_method")
 
     @public_key_method.setter
     def public_key_method(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "public_key_method", value)
 
@@ -604,15 +635,16 @@
     def signing_ca(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "signing_ca", value)
 
     @property
     @pulumi.getter(name="sourceAddresses")
     def source_addresses(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of one or more valid IP or CIDR addresses that can use the SSH certificate.
+        A list of one or more valid IP or CIDR addresses that can use the SSH 
+        certificate.
         """
         return pulumi.get(self, "source_addresses")
 
     @source_addresses.setter
     def source_addresses(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "source_addresses", value)
 
@@ -718,27 +750,35 @@
             template="Sample SSH CA",
             valid_hours=24)
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] destination_addresses: A list of one or more valid IP or CIDR destination hosts where the certificate will authenticate.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] extensions: A list of key-value pairs that contain certificate extensions from the CA template for client certificates. Allowed values (case-sensitive): *permit-X11-forwarding, permit-agent-forwarding, permit-port-forwarding, permit-pty, permit-user-rc*
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] destination_addresses: A list of one or more valid IP or CIDR destination hosts where the 
+               certificate will authenticate.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] extensions: A list of key-value pairs that contain certificate extensions from the CA 
+               template for client certificates. Allowed values (case-sensitive): `permit-X11-forwarding`, `permit-agent-forwarding`,
+               `permit-port-forwarding`, `permit-pty`, `permit-user-rc`.
         :param pulumi.Input[str] folder: The DN of the policy folder where the SSH certificate object will be created.
         :param pulumi.Input[str] force_command: A command to run after successful login.
         :param pulumi.Input[str] key_id: The identifier of the requested SSH certificate.
         :param pulumi.Input[str] key_passphrase: Passphrase for encrypting the private key.
-        :param pulumi.Input[int] key_size: Number of bits to use when creating a key pair. (e.g. 3072)
-        :param pulumi.Input[str] object_name: The friendly name of the SSH certificate object. When not specified the `key_id` is used for the friendly name. If the object already exists the old certificate is archived and the CA issues a new certificate.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] principal: [DEPRECATED] - (Optional, set of strings) Use "principals" instead. A list of user names for whom the requested certificate will be valid.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] principals: A list of user names for whom the requested certificate will be valid.
+        :param pulumi.Input[int] key_size: Number of bits to use when creating a key pair. (e.g. `3072`).
+        :param pulumi.Input[str] object_name: The friendly name of the SSH certificate object. When not specified the `key_id` 
+               is used for the friendly name. If the object already exists the old certificate is archived and the CA issues a new
+               certificate.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] principal: [DEPRECATED] - (Optional, set of strings) Use "principals" instead. A list of usernames for whom the 
+               requested certificate will be valid.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] principals: A list of usernames for whom the requested certificate will be valid.
         :param pulumi.Input[str] public_key: The OpenSSH formatted public key that will be used to generate the SSH certificate.
-        :param pulumi.Input[str] public_key_method: Specifies whether the public key will be "local" (default), "file" or "service" generated.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] source_addresses: A list of one or more valid IP or CIDR addresses that can use the SSH certificate.
+        :param pulumi.Input[str] public_key_method: Specifies whether the public key will be `local` (default), `file` or 
+               `service` generated.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] source_addresses: A list of one or more valid IP or CIDR addresses that can use the SSH 
+               certificate.
         :param pulumi.Input[str] template: The SSH certificate issuing template.
         :param pulumi.Input[int] valid_hours: Desired number of hours for which the certificate will be valid.
         :param pulumi.Input[bool] windows: Specifies whether the private key will use Windows/DOS style line breaks.
         """
         ...
     @overload
     def __init__(__self__,
@@ -875,31 +915,39 @@
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] certificate: The issued SSH certificate.
         :param pulumi.Input[str] certificate_type: Indicates whether the SSH certificate is for client or server authentication.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] destination_addresses: A list of one or more valid IP or CIDR destination hosts where the certificate will authenticate.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] extensions: A list of key-value pairs that contain certificate extensions from the CA template for client certificates. Allowed values (case-sensitive): *permit-X11-forwarding, permit-agent-forwarding, permit-port-forwarding, permit-pty, permit-user-rc*
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] destination_addresses: A list of one or more valid IP or CIDR destination hosts where the 
+               certificate will authenticate.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] extensions: A list of key-value pairs that contain certificate extensions from the CA 
+               template for client certificates. Allowed values (case-sensitive): `permit-X11-forwarding`, `permit-agent-forwarding`,
+               `permit-port-forwarding`, `permit-pty`, `permit-user-rc`.
         :param pulumi.Input[str] folder: The DN of the policy folder where the SSH certificate object will be created.
         :param pulumi.Input[str] force_command: A command to run after successful login.
         :param pulumi.Input[str] key_id: The identifier of the requested SSH certificate.
         :param pulumi.Input[str] key_passphrase: Passphrase for encrypting the private key.
-        :param pulumi.Input[int] key_size: Number of bits to use when creating a key pair. (e.g. 3072)
-        :param pulumi.Input[str] object_name: The friendly name of the SSH certificate object. When not specified the `key_id` is used for the friendly name. If the object already exists the old certificate is archived and the CA issues a new certificate.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] principal: [DEPRECATED] - (Optional, set of strings) Use "principals" instead. A list of user names for whom the requested certificate will be valid.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] principals: A list of user names for whom the requested certificate will be valid.
+        :param pulumi.Input[int] key_size: Number of bits to use when creating a key pair. (e.g. `3072`).
+        :param pulumi.Input[str] object_name: The friendly name of the SSH certificate object. When not specified the `key_id` 
+               is used for the friendly name. If the object already exists the old certificate is archived and the CA issues a new
+               certificate.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] principal: [DEPRECATED] - (Optional, set of strings) Use "principals" instead. A list of usernames for whom the 
+               requested certificate will be valid.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] principals: A list of usernames for whom the requested certificate will be valid.
         :param pulumi.Input[str] private_key: The private key for the SSH certificate if generated by Venafi.
         :param pulumi.Input[str] public_key: The OpenSSH formatted public key that will be used to generate the SSH certificate.
         :param pulumi.Input[str] public_key_fingerprint: The SHA256 fingerprint of the SSH certificate's public key.
-        :param pulumi.Input[str] public_key_method: Specifies whether the public key will be "local" (default), "file" or "service" generated.
+        :param pulumi.Input[str] public_key_method: Specifies whether the public key will be `local` (default), `file` or 
+               `service` generated.
         :param pulumi.Input[str] serial: The serial number of the SSH certificate.
         :param pulumi.Input[str] signing_ca: The SHA256 fingerprint of the CA that signed the SSH certificate.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] source_addresses: A list of one or more valid IP or CIDR addresses that can use the SSH certificate.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] source_addresses: A list of one or more valid IP or CIDR addresses that can use the SSH 
+               certificate.
         :param pulumi.Input[str] template: The SSH certificate issuing template.
         :param pulumi.Input[str] valid_from: The date the SSH certificate was issued.
         :param pulumi.Input[int] valid_hours: Desired number of hours for which the certificate will be valid.
         :param pulumi.Input[str] valid_to: The date the SSH certificate will expire.
         :param pulumi.Input[bool] windows: Specifies whether the private key will use Windows/DOS style line breaks.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
@@ -948,23 +996,26 @@
         """
         return pulumi.get(self, "certificate_type")
 
     @property
     @pulumi.getter(name="destinationAddresses")
     def destination_addresses(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        A list of one or more valid IP or CIDR destination hosts where the certificate will authenticate.
+        A list of one or more valid IP or CIDR destination hosts where the 
+        certificate will authenticate.
         """
         return pulumi.get(self, "destination_addresses")
 
     @property
     @pulumi.getter
     def extensions(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        A list of key-value pairs that contain certificate extensions from the CA template for client certificates. Allowed values (case-sensitive): *permit-X11-forwarding, permit-agent-forwarding, permit-port-forwarding, permit-pty, permit-user-rc*
+        A list of key-value pairs that contain certificate extensions from the CA 
+        template for client certificates. Allowed values (case-sensitive): `permit-X11-forwarding`, `permit-agent-forwarding`,
+        `permit-port-forwarding`, `permit-pty`, `permit-user-rc`.
         """
         return pulumi.get(self, "extensions")
 
     @property
     @pulumi.getter
     def folder(self) -> pulumi.Output[Optional[str]]:
         """
@@ -996,42 +1047,45 @@
         """
         return pulumi.get(self, "key_passphrase")
 
     @property
     @pulumi.getter(name="keySize")
     def key_size(self) -> pulumi.Output[Optional[int]]:
         """
-        Number of bits to use when creating a key pair. (e.g. 3072)
+        Number of bits to use when creating a key pair. (e.g. `3072`).
         """
         return pulumi.get(self, "key_size")
 
     @property
     @pulumi.getter(name="objectName")
     def object_name(self) -> pulumi.Output[Optional[str]]:
         """
-        The friendly name of the SSH certificate object. When not specified the `key_id` is used for the friendly name. If the object already exists the old certificate is archived and the CA issues a new certificate.
+        The friendly name of the SSH certificate object. When not specified the `key_id` 
+        is used for the friendly name. If the object already exists the old certificate is archived and the CA issues a new
+        certificate.
         """
         return pulumi.get(self, "object_name")
 
     @property
     @pulumi.getter
     def principal(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        [DEPRECATED] - (Optional, set of strings) Use "principals" instead. A list of user names for whom the requested certificate will be valid.
+        [DEPRECATED] - (Optional, set of strings) Use "principals" instead. A list of usernames for whom the 
+        requested certificate will be valid.
         """
         warnings.warn("""This will be removed in the future. Use \"principals\" instead""", DeprecationWarning)
         pulumi.log.warn("""principal is deprecated: This will be removed in the future. Use \"principals\" instead""")
 
         return pulumi.get(self, "principal")
 
     @property
     @pulumi.getter
     def principals(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        A list of user names for whom the requested certificate will be valid.
+        A list of usernames for whom the requested certificate will be valid.
         """
         return pulumi.get(self, "principals")
 
     @property
     @pulumi.getter(name="privateKey")
     def private_key(self) -> pulumi.Output[str]:
         """
@@ -1055,15 +1109,16 @@
         """
         return pulumi.get(self, "public_key_fingerprint")
 
     @property
     @pulumi.getter(name="publicKeyMethod")
     def public_key_method(self) -> pulumi.Output[Optional[str]]:
         """
-        Specifies whether the public key will be "local" (default), "file" or "service" generated.
+        Specifies whether the public key will be `local` (default), `file` or 
+        `service` generated.
         """
         return pulumi.get(self, "public_key_method")
 
     @property
     @pulumi.getter
     def serial(self) -> pulumi.Output[str]:
         """
@@ -1079,15 +1134,16 @@
         """
         return pulumi.get(self, "signing_ca")
 
     @property
     @pulumi.getter(name="sourceAddresses")
     def source_addresses(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        A list of one or more valid IP or CIDR addresses that can use the SSH certificate.
+        A list of one or more valid IP or CIDR addresses that can use the SSH 
+        certificate.
         """
         return pulumi.get(self, "source_addresses")
 
     @property
     @pulumi.getter
     def template(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_venafi-1.9.0a1712991486/pulumi_venafi/ssh_config.py` & `pulumi_venafi-1.9.0a1713292049/pulumi_venafi/ssh_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.9.0a1712991486/pulumi_venafi.egg-info/PKG-INFO` & `pulumi_venafi-1.9.0a1713292049/pulumi_venafi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_venafi
-Version: 1.9.0a1712991486
+Version: 1.9.0a1713292049
 Summary: A Pulumi package for creating and managing venafi cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-venafi
 Keywords: pulumi,venafi
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_venafi-1.9.0a1712991486/pulumi_venafi.egg-info/SOURCES.txt` & `pulumi_venafi-1.9.0a1713292049/pulumi_venafi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.9.0a1712991486/pyproject.toml` & `pulumi_venafi-1.9.0a1713292049/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_venafi"
   description = "A Pulumi package for creating and managing venafi cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "venafi"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "1.9.0a1712991486"
+  version = "1.9.0a1713292049"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-venafi"
 
 [build-system]
```

