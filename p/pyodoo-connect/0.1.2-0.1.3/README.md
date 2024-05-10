# Comparing `tmp/pyodoo_connect-0.1.2.tar.gz` & `tmp/pyodoo_connect-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyodoo_connect-0.1.2.tar", last modified: Thu May  9 09:59:54 2024, max compression
+gzip compressed data, was "pyodoo_connect-0.1.3.tar", last modified: Fri May 10 21:19:00 2024, max compression
```

## Comparing `pyodoo_connect-0.1.2.tar` & `pyodoo_connect-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:59:54.773068 pyodoo_connect-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-09 09:59:42.000000 pyodoo_connect-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-05-09 09:59:54.773068 pyodoo_connect-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-05-09 09:59:42.000000 pyodoo_connect-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:59:54.773068 pyodoo_connect-0.1.2/pyodoo_connect/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-09 09:59:42.000000 pyodoo_connect-0.1.2/pyodoo_connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7242 2024-05-09 09:59:42.000000 pyodoo_connect-0.1.2/pyodoo_connect/odoo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-05-09 09:59:42.000000 pyodoo_connect-0.1.2/pyodoo_connect/proxies.py
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-09 09:59:42.000000 pyodoo_connect-0.1.2/pyodoo_connect/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:59:54.773068 pyodoo_connect-0.1.2/pyodoo_connect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-05-09 09:59:54.000000 pyodoo_connect-0.1.2/pyodoo_connect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-09 09:59:54.000000 pyodoo_connect-0.1.2/pyodoo_connect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 09:59:54.000000 pyodoo_connect-0.1.2/pyodoo_connect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-09 09:59:54.000000 pyodoo_connect-0.1.2/pyodoo_connect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-09 09:59:42.000000 pyodoo_connect-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-09 09:59:54.773068 pyodoo_connect-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-09 09:59:42.000000 pyodoo_connect-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:59:54.773068 pyodoo_connect-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-09 09:59:42.000000 pyodoo_connect-0.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-09 09:59:42.000000 pyodoo_connect-0.1.2/tests/test_odoo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:19:00.322440 pyodoo_connect-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-10 21:18:48.000000 pyodoo_connect-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-05-10 21:19:00.322440 pyodoo_connect-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-10 21:18:48.000000 pyodoo_connect-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:19:00.322440 pyodoo_connect-0.1.3/pyodoo_connect/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-10 21:18:48.000000 pyodoo_connect-0.1.3/pyodoo_connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7242 2024-05-10 21:18:48.000000 pyodoo_connect-0.1.3/pyodoo_connect/odoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-05-10 21:18:48.000000 pyodoo_connect-0.1.3/pyodoo_connect/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-10 21:18:48.000000 pyodoo_connect-0.1.3/pyodoo_connect/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:19:00.322440 pyodoo_connect-0.1.3/pyodoo_connect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-05-10 21:19:00.000000 pyodoo_connect-0.1.3/pyodoo_connect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-10 21:19:00.000000 pyodoo_connect-0.1.3/pyodoo_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 21:19:00.000000 pyodoo_connect-0.1.3/pyodoo_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-10 21:19:00.000000 pyodoo_connect-0.1.3/pyodoo_connect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-10 21:18:48.000000 pyodoo_connect-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-10 21:19:00.322440 pyodoo_connect-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-10 21:18:48.000000 pyodoo_connect-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:19:00.322440 pyodoo_connect-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-10 21:18:48.000000 pyodoo_connect-0.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-10 21:18:48.000000 pyodoo_connect-0.1.3/tests/test_odoo.py
```

### Comparing `pyodoo_connect-0.1.2/LICENSE` & `pyodoo_connect-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodoo_connect-0.1.2/PKG-INFO` & `pyodoo_connect-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodoo_connect
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python package to interact with Odoo via JSON-RPC.
 Home-page: https://github.com/fasilwdr/pyodoo_connector
 Author: Fasil
 Author-email: Fasil <fasilwdr@hotmail.com>
 License: MIT License
         
         Copyright (c) [2024] [Fasil]
@@ -95,15 +95,15 @@
 - Execute a Method on a Record
 ```python
 partner.action_archive()
 partner.update({'mobile': '12345678'})
 ```
 - Search for Records
 ```python
-partner_ids = odoo.env['res.partner'].search(domain=[('name', '=', 'Abigail Peterson')])
+partner_ids = odoo.env['res.partner'].search([('name', '=', 'Abigail Peterson')])
 print(partner_ids)
 #[50]
 ```
 - Read Records
 ```python
 print(partner.name)
 records = odoo.env['res.partner'].read(ids=partner_ids, fields=['name', 'email'])
@@ -115,29 +115,52 @@
 ```python
 new_partner_id = odoo.env['res.partner'].create({'name': 'New Partner', 'email': 'new@partner.com', 'is_company': True})
 print(new_partner_id)
 #100
 ```
 - Update Records
 ```python
+#These are the ways to update records
+partner.mobile = '+91 9746707744'
+partner.write({'mobile': '+91 9746707744'})
 odoo.env['res.partner'].write(ids=new_partner_id, values={'phone': '1234567890'})
 ```
+- Update Relation fields (One2many or Many2many)
+```python
+from pyodoo_connect import Command
+partner.category_id = [Command.set([5,6])]
+partner.write({'category_id': [Command.link([4,3])]})
+odoo.env['res.partner'].write(ids=new_partner_id, values={'category_id': [Command.create({'name': 'New Tag'})]})
+#All functions of Command can be used (create, update, delete, unlink, link, clear, set)
+```
 - Delete Records
 ```python
 odoo.env['res.partner'].unlink(ids=new_partner_id)
 ```
 - Download a QWeb Report
 ```python
 odoo.download_report(report_name='sale.report_saleorder', record_ids=[52], file_name='Sales Report')
 ```
 - Version
 ```python
 print(odoo.version)
 #17.0
 ```
+- With Context
+```python
+record_id = odoo.env['purchase.order'].browse(14)
+record_id.with_context({'send_rfq':True}).action_rfq_send()
+#or
+record_id.with_context(send_rfq=True).action_rfq_send()
+```
+- UID
+```python
+print(odoo.uid)
+#2
+```
 - User Context
 ```python
 print(odoo.env.context)
 #{'lang': 'en_US', 'tz': 'Europe/Brussels', 'uid': 2}
 ```
 - User Info
 ```python
```

### Comparing `pyodoo_connect-0.1.2/README.md` & `pyodoo_connect-0.1.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 - Execute a Method on a Record
 ```python
 partner.action_archive()
 partner.update({'mobile': '12345678'})
 ```
 - Search for Records
 ```python
-partner_ids = odoo.env['res.partner'].search(domain=[('name', '=', 'Abigail Peterson')])
+partner_ids = odoo.env['res.partner'].search([('name', '=', 'Abigail Peterson')])
 print(partner_ids)
 #[50]
 ```
 - Read Records
 ```python
 print(partner.name)
 records = odoo.env['res.partner'].read(ids=partner_ids, fields=['name', 'email'])
@@ -73,29 +73,52 @@
 ```python
 new_partner_id = odoo.env['res.partner'].create({'name': 'New Partner', 'email': 'new@partner.com', 'is_company': True})
 print(new_partner_id)
 #100
 ```
 - Update Records
 ```python
+#These are the ways to update records
+partner.mobile = '+91 9746707744'
+partner.write({'mobile': '+91 9746707744'})
 odoo.env['res.partner'].write(ids=new_partner_id, values={'phone': '1234567890'})
 ```
+- Update Relation fields (One2many or Many2many)
+```python
+from pyodoo_connect import Command
+partner.category_id = [Command.set([5,6])]
+partner.write({'category_id': [Command.link([4,3])]})
+odoo.env['res.partner'].write(ids=new_partner_id, values={'category_id': [Command.create({'name': 'New Tag'})]})
+#All functions of Command can be used (create, update, delete, unlink, link, clear, set)
+```
 - Delete Records
 ```python
 odoo.env['res.partner'].unlink(ids=new_partner_id)
 ```
 - Download a QWeb Report
 ```python
 odoo.download_report(report_name='sale.report_saleorder', record_ids=[52], file_name='Sales Report')
 ```
 - Version
 ```python
 print(odoo.version)
 #17.0
 ```
+- With Context
+```python
+record_id = odoo.env['purchase.order'].browse(14)
+record_id.with_context({'send_rfq':True}).action_rfq_send()
+#or
+record_id.with_context(send_rfq=True).action_rfq_send()
+```
+- UID
+```python
+print(odoo.uid)
+#2
+```
 - User Context
 ```python
 print(odoo.env.context)
 #{'lang': 'en_US', 'tz': 'Europe/Brussels', 'uid': 2}
 ```
 - User Info
 ```python
```

### Comparing `pyodoo_connect-0.1.2/pyodoo_connect/odoo.py` & `pyodoo_connect-0.1.3/pyodoo_connect/odoo.py`

 * *Files identical despite different names*

### Comparing `pyodoo_connect-0.1.2/pyodoo_connect/tools.py` & `pyodoo_connect-0.1.3/pyodoo_connect/tools.py`

 * *Files identical despite different names*

### Comparing `pyodoo_connect-0.1.2/pyodoo_connect.egg-info/PKG-INFO` & `pyodoo_connect-0.1.3/pyodoo_connect.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodoo_connect
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python package to interact with Odoo via JSON-RPC.
 Home-page: https://github.com/fasilwdr/pyodoo_connector
 Author: Fasil
 Author-email: Fasil <fasilwdr@hotmail.com>
 License: MIT License
         
         Copyright (c) [2024] [Fasil]
@@ -95,15 +95,15 @@
 - Execute a Method on a Record
 ```python
 partner.action_archive()
 partner.update({'mobile': '12345678'})
 ```
 - Search for Records
 ```python
-partner_ids = odoo.env['res.partner'].search(domain=[('name', '=', 'Abigail Peterson')])
+partner_ids = odoo.env['res.partner'].search([('name', '=', 'Abigail Peterson')])
 print(partner_ids)
 #[50]
 ```
 - Read Records
 ```python
 print(partner.name)
 records = odoo.env['res.partner'].read(ids=partner_ids, fields=['name', 'email'])
@@ -115,29 +115,52 @@
 ```python
 new_partner_id = odoo.env['res.partner'].create({'name': 'New Partner', 'email': 'new@partner.com', 'is_company': True})
 print(new_partner_id)
 #100
 ```
 - Update Records
 ```python
+#These are the ways to update records
+partner.mobile = '+91 9746707744'
+partner.write({'mobile': '+91 9746707744'})
 odoo.env['res.partner'].write(ids=new_partner_id, values={'phone': '1234567890'})
 ```
+- Update Relation fields (One2many or Many2many)
+```python
+from pyodoo_connect import Command
+partner.category_id = [Command.set([5,6])]
+partner.write({'category_id': [Command.link([4,3])]})
+odoo.env['res.partner'].write(ids=new_partner_id, values={'category_id': [Command.create({'name': 'New Tag'})]})
+#All functions of Command can be used (create, update, delete, unlink, link, clear, set)
+```
 - Delete Records
 ```python
 odoo.env['res.partner'].unlink(ids=new_partner_id)
 ```
 - Download a QWeb Report
 ```python
 odoo.download_report(report_name='sale.report_saleorder', record_ids=[52], file_name='Sales Report')
 ```
 - Version
 ```python
 print(odoo.version)
 #17.0
 ```
+- With Context
+```python
+record_id = odoo.env['purchase.order'].browse(14)
+record_id.with_context({'send_rfq':True}).action_rfq_send()
+#or
+record_id.with_context(send_rfq=True).action_rfq_send()
+```
+- UID
+```python
+print(odoo.uid)
+#2
+```
 - User Context
 ```python
 print(odoo.env.context)
 #{'lang': 'en_US', 'tz': 'Europe/Brussels', 'uid': 2}
 ```
 - User Info
 ```python
```

### Comparing `pyodoo_connect-0.1.2/pyproject.toml` & `pyodoo_connect-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyodoo_connect"
-version = "0.1.2"
+version = "0.1.3"
 description = "A Python package to interact with Odoo via JSON-RPC."
 authors = [{ name = "Fasil", email = "fasilwdr@hotmail.com" }]
 license = { file = "LICENSE" }
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `pyodoo_connect-0.1.2/setup.cfg` & `pyodoo_connect-0.1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyodoo_connect
-version = 0.1.2
+version = 0.1.3
 author = Fasil
 author_email = fasilwdr@hotmail.com
 description = A Python package to interact with Odoo via JSON-RPC.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/fasilwdr/pyodoo_connector
 classifiers =
```

### Comparing `pyodoo_connect-0.1.2/tests/test_odoo.py` & `pyodoo_connect-0.1.3/tests/test_odoo.py`

 * *Files identical despite different names*

