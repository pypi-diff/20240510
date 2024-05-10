# Comparing `tmp/odoo12_addon_sm_reports-12.0.0.0.3-py2.py3-none-any.whl.zip` & `tmp/odoo12_addon_sm_reports-12.0.0.0.3.99.dev1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 4368 bytes, number of entries: 11
--rw-r--r--  2.0 unx       20 b- defN 21-Oct-04 10:07 odoo/addons/sm_reports/__init__.py
--rw-r--r--  2.0 unx      663 b- defN 21-Oct-06 19:02 odoo/addons/sm_reports/__manifest__.py
--rw-r--r--  2.0 unx       30 b- defN 21-Oct-04 10:07 odoo/addons/sm_reports/models/__init__.py
--rw-r--r--  2.0 unx      267 b- defN 21-Oct-04 10:07 odoo/addons/sm_reports/models/models_sm_member.py
--rw-r--r--  2.0 unx      164 b- defN 21-Oct-06 17:54 odoo/addons/sm_reports/security/ir.model.access.csv
--rw-r--r--  2.0 unx     2000 b- defN 21-Oct-04 10:07 odoo/addons/sm_reports/views/default_template.xml
--rw-r--r--  2.0 unx      547 b- defN 21-Oct-04 10:07 odoo/addons/sm_reports/views/views_members.xml
--rw-r--r--  2.0 unx      402 b- defN 21-Oct-06 19:14 odoo12_addon_sm_reports-12.0.0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 21-Oct-06 19:14 odoo12_addon_sm_reports-12.0.0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 21-Oct-06 19:14 odoo12_addon_sm_reports-12.0.0.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1080 b- defN 21-Oct-06 19:14 odoo12_addon_sm_reports-12.0.0.0.3.dist-info/RECORD
-11 files, 5288 bytes uncompressed, 2470 bytes compressed:  53.3%
+-rw-rw-r--  2.0 unx       20 b- defN 23-Dec-19 17:24 odoo/addons/sm_reports/__init__.py
+-rw-rw-r--  2.0 unx      522 b- defN 23-Dec-19 17:24 odoo/addons/sm_reports/__manifest__.py
+-rw-rw-r--  2.0 unx       30 b- defN 23-Dec-19 17:24 odoo/addons/sm_reports/models/__init__.py
+-rw-rw-r--  2.0 unx      283 b- defN 23-Dec-19 17:24 odoo/addons/sm_reports/models/models_sm_member.py
+-rw-rw-r--  2.0 unx      164 b- defN 23-Dec-19 17:24 odoo/addons/sm_reports/security/ir.model.access.csv
+-rw-rw-r--  2.0 unx     2000 b- defN 23-Dec-19 17:24 odoo/addons/sm_reports/views/default_template.xml
+-rw-rw-r--  2.0 unx      547 b- defN 23-Dec-19 17:24 odoo/addons/sm_reports/views/views_members.xml
+-rw-rw-r--  2.0 unx      409 b- defN 24-May-10 10:52 odoo12_addon_sm_reports-12.0.0.0.3.99.dev1.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 24-May-10 10:52 odoo12_addon_sm_reports-12.0.0.0.3.99.dev1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        5 b- defN 24-May-10 10:52 odoo12_addon_sm_reports-12.0.0.0.3.99.dev1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1112 b- defN 24-May-10 10:52 odoo12_addon_sm_reports-12.0.0.0.3.99.dev1.dist-info/RECORD
+11 files, 5202 bytes uncompressed, 2406 bytes compressed:  53.7%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: odoo/addons/sm_reports/views/default_template.xml
 Comment: 
 
 Filename: odoo/addons/sm_reports/views/views_members.xml
 Comment: 
 
-Filename: odoo12_addon_sm_reports-12.0.0.0.3.dist-info/METADATA
+Filename: odoo12_addon_sm_reports-12.0.0.0.3.99.dev1.dist-info/METADATA
 Comment: 
 
-Filename: odoo12_addon_sm_reports-12.0.0.0.3.dist-info/WHEEL
+Filename: odoo12_addon_sm_reports-12.0.0.0.3.99.dev1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo12_addon_sm_reports-12.0.0.0.3.dist-info/top_level.txt
+Filename: odoo12_addon_sm_reports-12.0.0.0.3.99.dev1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo12_addon_sm_reports-12.0.0.0.3.dist-info/RECORD
+Filename: odoo12_addon_sm_reports-12.0.0.0.3.99.dev1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/sm_reports/__manifest__.py

```diff
@@ -1,28 +1,25 @@
 # -*- coding: utf-8 -*-
 {
-  'name': "sm_reports",
+    'name': "sm_reports",
 
-  'summary': """
+    'summary': """
     reporting engine for carsgharing system
   """,
 
-  'author': "Som Mobilitat",
-  'website': "https://www.sommobilitat.coop",
+    'author': "Som Mobilitat",
+    'website': "https://www.sommobilitat.coop",
 
-  # Categories can be used to filter modules in modules listing
-  # Check https://github.com/odoo/odoo/blob/11.0/odoo/addons/base/module/module_data.xml
-  # for the full list
-  'category': 'Uncategorized',
-  'version': '12.0.0.0.3',
+    'category': 'Uncategorized',
+    'version': '12.0.0.0.3',
 
-  # any module necessary for this one to work correctly
-  'depends': ['base'],
+    # any module necessary for this one to work correctly
+    'depends': ['base'],
 
-  # always loaded
-  'data': [
-    'views/default_template.xml',
-    'views/views_members.xml'
-  ],
-  # only loaded in demonstration mode
-  'demo': [],
+    # always loaded
+    'data': [
+        'views/default_template.xml',
+        'views/views_members.xml'
+    ],
+    # only loaded in demonstration mode
+    'demo': [],
 }
```

## odoo/addons/sm_reports/models/models_sm_member.py

```diff
@@ -1,9 +1,10 @@
 from odoo import models, fields, api
 from odoo.tools.translate import _
 
 
 class sm_reporting_member(models.Model):
-  _inherit = 'res.partner'
-  _name = 'res.partner'
+    _inherit = 'res.partner'
+    _name = 'res.partner'
 
-  reporting_related_member_id = fields.Many2one('res.partner', string=_("Reporting related member"))
+    reporting_related_member_id = fields.Many2one(
+        'res.partner', string=_("Reporting related member"))
```

