# Comparing `tmp/odoo12_addon_vertical_carsharing_mail-12.0.0.0.3-py3-none-any.whl.zip` & `tmp/odoo12_addon_vertical_carsharing_mail-12.0.0.0.3.99.dev1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 3751 bytes, number of entries: 9
--rw-r--r--  2.0 unx       44 b- defN 21-Jul-12 16:17 odoo/addons/vertical_carsharing_mail/__init__.py
--rw-r--r--  2.0 unx      698 b- defN 21-Jul-23 09:21 odoo/addons/vertical_carsharing_mail/__manifest__.py
--rw-r--r--  2.0 unx     1416 b- defN 21-Jul-23 09:04 odoo/addons/vertical_carsharing_mail/data/vc_mail_data.xml
--rw-r--r--  2.0 unx       29 b- defN 21-Jul-12 16:17 odoo/addons/vertical_carsharing_mail/models/__init__.py
--rw-r--r--  2.0 unx      572 b- defN 21-Jul-12 16:17 odoo/addons/vertical_carsharing_mail/models/account_invoice.py
--rw-r--r--  2.0 unx      372 b- defN 21-Jul-23 09:23 odoo12_addon_vertical_carsharing_mail-12.0.0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Jul-23 09:23 odoo12_addon_vertical_carsharing_mail-12.0.0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 21-Jul-23 09:23 odoo12_addon_vertical_carsharing_mail-12.0.0.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      990 b- defN 21-Jul-23 09:23 odoo12_addon_vertical_carsharing_mail-12.0.0.0.3.dist-info/RECORD
-9 files, 4218 bytes uncompressed, 1959 bytes compressed:  53.6%
+Zip file size: 3757 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx       44 b- defN 23-Dec-19 17:24 odoo/addons/vertical_carsharing_mail/__init__.py
+-rw-rw-r--  2.0 unx      573 b- defN 23-Dec-19 17:24 odoo/addons/vertical_carsharing_mail/__manifest__.py
+-rw-rw-r--  2.0 unx     1416 b- defN 23-Dec-19 17:24 odoo/addons/vertical_carsharing_mail/data/vc_mail_data.xml
+-rw-rw-r--  2.0 unx       29 b- defN 23-Dec-19 17:24 odoo/addons/vertical_carsharing_mail/models/__init__.py
+-rw-rw-r--  2.0 unx      572 b- defN 23-Dec-19 17:24 odoo/addons/vertical_carsharing_mail/models/account_invoice.py
+-rw-rw-r--  2.0 unx      416 b- defN 24-May-10 10:52 odoo12_addon_vertical_carsharing_mail-12.0.0.0.3.99.dev1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-10 10:52 odoo12_addon_vertical_carsharing_mail-12.0.0.0.3.99.dev1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        5 b- defN 24-May-10 10:52 odoo12_addon_vertical_carsharing_mail-12.0.0.0.3.99.dev1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1022 b- defN 24-May-10 10:52 odoo12_addon_vertical_carsharing_mail-12.0.0.0.3.99.dev1.dist-info/RECORD
+9 files, 4169 bytes uncompressed, 1901 bytes compressed:  54.4%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: odoo/addons/vertical_carsharing_mail/models/__init__.py
 Comment: 
 
 Filename: odoo/addons/vertical_carsharing_mail/models/account_invoice.py
 Comment: 
 
-Filename: odoo12_addon_vertical_carsharing_mail-12.0.0.0.3.dist-info/METADATA
+Filename: odoo12_addon_vertical_carsharing_mail-12.0.0.0.3.99.dev1.dist-info/METADATA
 Comment: 
 
-Filename: odoo12_addon_vertical_carsharing_mail-12.0.0.0.3.dist-info/WHEEL
+Filename: odoo12_addon_vertical_carsharing_mail-12.0.0.0.3.99.dev1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo12_addon_vertical_carsharing_mail-12.0.0.0.3.dist-info/top_level.txt
+Filename: odoo12_addon_vertical_carsharing_mail-12.0.0.0.3.99.dev1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo12_addon_vertical_carsharing_mail-12.0.0.0.3.dist-info/RECORD
+Filename: odoo12_addon_vertical_carsharing_mail-12.0.0.0.3.99.dev1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/vertical_carsharing_mail/__manifest__.py

```diff
@@ -1,32 +1,29 @@
 # -*- coding: utf-8 -*-
 {
-  'name': "vertical_carsharing_mail",
+    'name': "vertical_carsharing_mail",
 
-  'summary': """
+    'summary': """
     Modules to manage mail templates""",
 
-  'author': "Som Mobilitat",
-  'website': "https://www.sommobilitat.coop",
+    'author': "Som Mobilitat",
+    'website': "https://www.sommobilitat.coop",
 
-  # Categories can be used to filter modules in modules listing
-  # Check https://github.com/odoo/odoo/blob/11.0/odoo/addons/base/module/module_data.xml
-  # for the full list
-  'category': 'vertical-carsharing',
-  'version': '12.0.0.0.3',
+    'category': 'vertical-carsharing',
+    'version': '12.0.0.0.3',
 
-  # any module necessary for this one to work correctly
-  'depends': [
-    'base',
-    'mail',
-    'account'
-  ],
+    # any module necessary for this one to work correctly
+    'depends': [
+        'base',
+        'mail',
+        'account'
+    ],
 
-  # always loaded
-  'data': [
-    'data/vc_mail_data.xml'
-  ],
-  # only loaded in demonstration mode
-  'demo': [
-    # 'demo/demo.xml',
-  ],
+    # always loaded
+    'data': [
+        'data/vc_mail_data.xml'
+    ],
+    # only loaded in demonstration mode
+    'demo': [
+        # 'demo/demo.xml',
+    ],
 }
```

## Comparing `odoo12_addon_vertical_carsharing_mail-12.0.0.0.3.dist-info/RECORD` & `odoo12_addon_vertical_carsharing_mail-12.0.0.0.3.99.dev1.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 odoo/addons/vertical_carsharing_mail/__init__.py,sha256=m9EwjQid0_uoD8cYfvb5nXUcNfwuHpJwwB2c3aAvtLo,44
-odoo/addons/vertical_carsharing_mail/__manifest__.py,sha256=oUw5BUZPKbGSzfAbJwYVCDPAYsEg1Xxa6g8I5uZUWgI,698
+odoo/addons/vertical_carsharing_mail/__manifest__.py,sha256=ZDOoSqc7Ey2FK3rR4kiVJH1sG3z6fDvAkU54Sfawbyg,573
 odoo/addons/vertical_carsharing_mail/data/vc_mail_data.xml,sha256=nBD7Sop6O5Wienww4nT3k5oyfitdYom03Ca18bpE7GA,1416
 odoo/addons/vertical_carsharing_mail/models/__init__.py,sha256=OhJy-jbUeeE8k5mKNnnEswiLmaRaIpe4DliD3Vmrx10,29
 odoo/addons/vertical_carsharing_mail/models/account_invoice.py,sha256=1mJOLqaZl3ZQDGM2qZasrwxZ6J26f8Y-DogxtUiavBo,572
-odoo12_addon_vertical_carsharing_mail-12.0.0.0.3.dist-info/METADATA,sha256=RWf_ypEROk7DIym6zgRDKaKTT7cVALIv8aUMzeCYf20,372
-odoo12_addon_vertical_carsharing_mail-12.0.0.0.3.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-odoo12_addon_vertical_carsharing_mail-12.0.0.0.3.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo12_addon_vertical_carsharing_mail-12.0.0.0.3.dist-info/RECORD,,
+odoo12_addon_vertical_carsharing_mail-12.0.0.0.3.99.dev1.dist-info/METADATA,sha256=xks7oc5Rj__8mmV31deSkyviRspI58Z4SCFuJfA9RUI,416
+odoo12_addon_vertical_carsharing_mail-12.0.0.0.3.99.dev1.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+odoo12_addon_vertical_carsharing_mail-12.0.0.0.3.99.dev1.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo12_addon_vertical_carsharing_mail-12.0.0.0.3.99.dev1.dist-info/RECORD,,
```

