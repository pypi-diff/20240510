# Comparing `tmp/pyescoapi-0.0.7.tar.gz` & `tmp/pyescoapi-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyescoapi-0.0.7.tar", last modified: Fri Apr 12 18:02:26 2024, max compression
+gzip compressed data, was "pyescoapi-0.0.9.tar", last modified: Thu Apr 18 15:54:54 2024, max compression
```

## Comparing `pyescoapi-0.0.7.tar` & `pyescoapi-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 18:02:26.009519 pyescoapi-0.0.7/
--rw-rw-rw-   0        0        0      514 2024-04-12 18:02:26.008518 pyescoapi-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       41 2024-04-10 15:22:40.000000 pyescoapi-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-12 18:02:25.964505 pyescoapi-0.0.7/pyEscoAPI/
--rw-rw-rw-   0        0        0      115 2024-04-10 15:22:40.000000 pyescoapi-0.0.7/pyEscoAPI/__init__.py
--rw-rw-rw-   0        0        0     5849 2024-04-12 18:00:25.000000 pyescoapi-0.0.7/pyEscoAPI/dataclasses.py
--rw-rw-rw-   0        0        0    78222 2024-04-12 18:00:25.000000 pyescoapi-0.0.7/pyEscoAPI/esco_api.py
-drwxrwxrwx   0        0        0        0 2024-04-12 18:02:26.006511 pyescoapi-0.0.7/pyEscoAPI.egg-info/
--rw-rw-rw-   0        0        0      514 2024-04-12 18:02:25.000000 pyescoapi-0.0.7/pyEscoAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2024-04-12 18:02:25.000000 pyescoapi-0.0.7/pyEscoAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 18:02:25.000000 pyescoapi-0.0.7/pyEscoAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-12 18:02:25.000000 pyescoapi-0.0.7/pyEscoAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-12 18:02:25.000000 pyescoapi-0.0.7/pyEscoAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      618 2024-04-12 18:00:25.000000 pyescoapi-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-12 18:02:26.009519 pyescoapi-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-12 18:02:26.005006 pyescoapi-0.0.7/tests/
--rw-rw-rw-   0        0        0     6346 2024-04-12 18:00:25.000000 pyescoapi-0.0.7/tests/test_client.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:54:54.523528 pyescoapi-0.0.9/
+-rw-rw-rw-   0        0        0      514 2024-04-18 15:54:54.522529 pyescoapi-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       41 2024-04-10 15:22:40.000000 pyescoapi-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 15:54:54.506970 pyescoapi-0.0.9/pyEscoAPI/
+-rw-rw-rw-   0        0        0      115 2024-04-10 15:22:40.000000 pyescoapi-0.0.9/pyEscoAPI/__init__.py
+-rw-rw-rw-   0        0        0     5849 2024-04-12 18:00:25.000000 pyescoapi-0.0.9/pyEscoAPI/dataclasses.py
+-rw-rw-rw-   0        0        0    81335 2024-04-18 15:52:28.000000 pyescoapi-0.0.9/pyEscoAPI/esco_api.py
+-rw-rw-rw-   0        0        0      215 2024-04-18 15:52:28.000000 pyescoapi-0.0.9/pyEscoAPI/exception.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:54:54.520529 pyescoapi-0.0.9/pyEscoAPI.egg-info/
+-rw-rw-rw-   0        0        0      514 2024-04-18 15:54:54.000000 pyescoapi-0.0.9/pyEscoAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2024-04-18 15:54:54.000000 pyescoapi-0.0.9/pyEscoAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 15:54:54.000000 pyescoapi-0.0.9/pyEscoAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-18 15:54:54.000000 pyescoapi-0.0.9/pyEscoAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-18 15:54:54.000000 pyescoapi-0.0.9/pyEscoAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      618 2024-04-18 15:53:45.000000 pyescoapi-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-18 15:54:54.523528 pyescoapi-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-18 15:54:54.520529 pyescoapi-0.0.9/tests/
+-rw-rw-rw-   0        0        0     6346 2024-04-12 18:00:25.000000 pyescoapi-0.0.9/tests/test_client.py
```

### Comparing `pyescoapi-0.0.7/PKG-INFO` & `pyescoapi-0.0.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyEscoAPI
-Version: 0.0.7
+Version: 0.0.9
 Summary: Python client for Esco API (Esco bolsa)
 Author-email: Codetria <hola@codetria.com>
 License: MIT License
 Keywords: Esco,API,bolsa,client,market,provider
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyescoapi-0.0.7/pyEscoAPI/dataclasses.py` & `pyescoapi-0.0.9/pyEscoAPI/dataclasses.py`

 * *Files identical despite different names*

### Comparing `pyescoapi-0.0.7/pyEscoAPI/esco_api.py` & `pyescoapi-0.0.9/pyEscoAPI/esco_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from http import HTTPMethod
 from typing import TypedDict, Optional
 
 import requests
 from requests import Response
 
 from pyEscoAPI.dataclasses import Persona, ComitenteData
+from pyEscoAPI.exception import PyEscoAPIError
 
 logger = logging.getLogger(f"{__name__}")
 
 
 class DomicilioDict(TypedDict):
     cod_pais: int
     cod_provincia: int
@@ -63,15 +64,15 @@
         }
         result: Response = req_call(**params)
         if 200 <= result.status_code <= 299:
             return result.json()
         else:
             if not error_message:
                 error_message = f"Error during endpoint call: {request_endpoint}. Code: {result.status_code}"
-            raise ConnectionRefusedError(error_message)
+            raise PyEscoAPIError(endpoint=request_endpoint, status_code=result.status_code, error_message=error_message)
 
     def __esco_login(self):
         req_body = {
             "userName": self.username,
             "password": self.password,
             "clientId": self.client_id
         }
@@ -1582,7 +1583,66 @@
         }
         self.__pre_connection()
         return self.__make_request(
             request_endpoint=f"/insert-cuenta-bancaria-comitente",
             request_body=req_body,
             request_method=HTTPMethod.POST
         )
+
+    def insert_comprobante_pago(
+            self,
+            cuenta: str,
+            moneda: str,
+            importe: decimal,
+            cuenta_contable: int,
+            fecha_concertacion: date = date.today(),
+            fecha_liquidacion: date = date.today(),
+            tp_cambio_mov_pais: int = 1,
+            cuenta_bancaria_comitente: int = None,
+            controla_saldo_monetario: bool = True,
+            num_referencia: int = None,
+            comentario: str = None,
+            id_origen: str = None,
+            es_echeq: bool = False,
+            numero_cheque: int = None
+    ):
+        """
+        Es un método que permite el ingreso de un Comprobante de Pago, este tipo de comprobante genera
+        un egreso monetario en la cuenta corriente de un cliente sin requerir una aprobacion posterior.
+        :param cuenta: Número de Comitente
+        :param moneda: Código de ISO de la moneda el movimiento.
+        :param importe: Importe de movimiento expresado en la moneda indicada.
+        :param cuenta_contable: Cuenta contable del agente donde se imputará el movimiento. Se debe ingresar el código interno de la cuenta contable.
+        :param fecha_concertacion: Fecha de concertación del recibo de cobro.
+        :param fecha_liquidacion: Fecha de liquidación del recibo de cobro.
+        :param tp_cambio_mov_pais: Tipo de Cambio para convertir el importe del recibo a la moneda local. 1 si es en moneda local.
+        :param cuenta_bancaria_comitente: Cuenta bancaria del cliente. Se debe ingresar el código interno. Es solo informativo, queda registrado solamente en el recibo de cobro.
+        :param controla_saldo_monetario: Indica si debe controlar el saldo monetario para hacer el egreso.
+        :param num_referencia: Nro de referencia del movimiento.
+        :param comentario: Comentario del movimiento
+        :param id_origen: Id de origen del movimiento
+        :param es_echeq: True is es un e-cheque.
+        :param numero_cheque: Si es un cheque, ingresar numero de cheque.s
+        :return:
+        """
+        req_body = {
+          "cuenta": cuenta,
+          "moneda": moneda,
+          "fechaConcertacion": fecha_concertacion.strftime("%Y-%m-%d"),
+          "fechaLiquidacion": fecha_liquidacion.strftime("%Y-%m-%d"),
+          "importe": importe,
+          "tpCambioMovPais": tp_cambio_mov_pais,
+          "cuentaContable": cuenta_contable,
+          "cuentaBancariaComitente": cuenta_bancaria_comitente,
+          "numReferencia": num_referencia,
+          "comentario": comentario,
+          "idOrigen": id_origen,
+          "controlaSaldoMonetario": controla_saldo_monetario,
+          "esEcheq": es_echeq,
+          "numeroCheque": numero_cheque
+        }
+        self.__pre_connection()
+        return self.__make_request(
+            request_endpoint=f"/insert-comprobante-pago",
+            request_body=req_body,
+            request_method=HTTPMethod.POST
+        )
```

### Comparing `pyescoapi-0.0.7/pyEscoAPI.egg-info/PKG-INFO` & `pyescoapi-0.0.9/pyEscoAPI.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyEscoAPI
-Version: 0.0.7
+Version: 0.0.9
 Summary: Python client for Esco API (Esco bolsa)
 Author-email: Codetria <hola@codetria.com>
 License: MIT License
 Keywords: Esco,API,bolsa,client,market,provider
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyescoapi-0.0.7/pyproject.toml` & `pyescoapi-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'pyEscoAPI'
-version = "0.0.7"
+version = "0.0.9"
 license = {text = "MIT License"}
 authors = [
   { name="Codetria", email="hola@codetria.com" },
 ]
 dependencies = [
     "requests==2.31.0"
 ]
```

### Comparing `pyescoapi-0.0.7/tests/test_client.py` & `pyescoapi-0.0.9/tests/test_client.py`

 * *Files identical despite different names*

