# Comparing `tmp/odoo12_addon_sm_teletacs-12.0.0.0.5-py2.py3-none-any.whl.zip` & `tmp/odoo12_addon_sm_teletacs-12.0.0.0.5.99.dev1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 5166 bytes, number of entries: 10
--rw-r--r--  2.0 unx       45 b- defN 22-Jun-28 13:09 odoo/addons/sm_teletacs/__init__.py
--rw-r--r--  2.0 unx      792 b- defN 23-Jan-19 13:18 odoo/addons/sm_teletacs/__manifest__.py
--rw-r--r--  2.0 unx       57 b- defN 22-Jun-28 13:09 odoo/addons/sm_teletacs/models/__init__.py
--rw-r--r--  2.0 unx     4474 b- defN 23-Jan-19 13:09 odoo/addons/sm_teletacs/models/models_smp_teletac.py
--rw-r--r--  2.0 unx      140 b- defN 22-Jun-28 13:09 odoo/addons/sm_teletacs/security/ir.model.access.csv
--rw-r--r--  2.0 unx     3876 b- defN 22-Jun-28 13:09 odoo/addons/sm_teletacs/views/views_teletac.xml
--rw-r--r--  2.0 unx      500 b- defN 23-Jan-19 13:19 odoo12_addon_sm_teletacs-12.0.0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jan-19 13:19 odoo12_addon_sm_teletacs-12.0.0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Jan-19 13:19 odoo12_addon_sm_teletacs-12.0.0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      988 b- defN 23-Jan-19 13:19 odoo12_addon_sm_teletacs-12.0.0.0.5.dist-info/RECORD
-10 files, 10987 bytes uncompressed, 3418 bytes compressed:  68.9%
+Zip file size: 5189 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx       45 b- defN 23-Dec-19 17:24 odoo/addons/sm_teletacs/__init__.py
+-rw-rw-r--  2.0 unx      613 b- defN 23-Dec-19 17:24 odoo/addons/sm_teletacs/__manifest__.py
+-rw-rw-r--  2.0 unx       57 b- defN 23-Dec-19 17:24 odoo/addons/sm_teletacs/models/__init__.py
+-rw-rw-r--  2.0 unx     5237 b- defN 23-Dec-19 17:24 odoo/addons/sm_teletacs/models/models_smp_teletac.py
+-rw-rw-r--  2.0 unx      140 b- defN 23-Dec-19 17:24 odoo/addons/sm_teletacs/security/ir.model.access.csv
+-rw-rw-r--  2.0 unx     3876 b- defN 23-Dec-19 17:24 odoo/addons/sm_teletacs/views/views_teletac.xml
+-rw-rw-r--  2.0 unx      507 b- defN 24-May-10 10:52 odoo12_addon_sm_teletacs-12.0.0.0.5.99.dev1.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 24-May-10 10:52 odoo12_addon_sm_teletacs-12.0.0.0.5.99.dev1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        5 b- defN 24-May-10 10:52 odoo12_addon_sm_teletacs-12.0.0.0.5.99.dev1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1020 b- defN 24-May-10 10:52 odoo12_addon_sm_teletacs-12.0.0.0.5.99.dev1.dist-info/RECORD
+10 files, 11610 bytes uncompressed, 3377 bytes compressed:  70.9%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: odoo/addons/sm_teletacs/security/ir.model.access.csv
 Comment: 
 
 Filename: odoo/addons/sm_teletacs/views/views_teletac.xml
 Comment: 
 
-Filename: odoo12_addon_sm_teletacs-12.0.0.0.5.dist-info/METADATA
+Filename: odoo12_addon_sm_teletacs-12.0.0.0.5.99.dev1.dist-info/METADATA
 Comment: 
 
-Filename: odoo12_addon_sm_teletacs-12.0.0.0.5.dist-info/WHEEL
+Filename: odoo12_addon_sm_teletacs-12.0.0.0.5.99.dev1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo12_addon_sm_teletacs-12.0.0.0.5.dist-info/top_level.txt
+Filename: odoo12_addon_sm_teletacs-12.0.0.0.5.99.dev1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo12_addon_sm_teletacs-12.0.0.0.5.dist-info/RECORD
+Filename: odoo12_addon_sm_teletacs-12.0.0.0.5.99.dev1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/sm_teletacs/__manifest__.py

```diff
@@ -4,22 +4,19 @@
 
     'summary': """
         Create extra expenses for carsharing usages""",
 
     'author': "Som Mobilitat",
     'website': "https://www.sommobilitat.coop",
 
-    # Categories can be used to filter modules in modules listing
-    # Check https://github.com/odoo/odoo/blob/11.0/odoo/addons/base/module/module_data.xml
-    # for the full list
     'category': 'vertical-carsharing',
     'version': '12.0.0.0.5',
 
     # any module necessary for this one to work correctly
-    'depends': ['base','vertical_carsharing','sm_partago_usage'],
+    'depends': ['base', 'vertical_carsharing', 'sm_partago_usage'],
 
     # always loaded
     'data': [
         # 'security/ir.model.access.csv',
         'views/views_teletac.xml'
     ],
     # only loaded in demonstration mode
```

## odoo/addons/sm_teletacs/models/models_smp_teletac.py

```diff
@@ -3,102 +3,113 @@
 from odoo import models, fields, api
 from odoo.tools.translate import _
 from odoo.addons.sm_maintenance.models.models_sm_resources import sm_resources
 from odoo.addons.sm_maintenance.models.models_sm_utils import sm_utils
 
 
 class smp_teletac(models.Model):
-  _name = 'smp.sm_teletac'
+    _name = 'smp.sm_teletac'
 
-  name = fields.Char(string=_("Name"), compute="_teletac_name")
-  date = fields.Date(string=_("Date"))
-  hour = fields.Char(string=_("Hour"))
-  description = fields.Char(string=_("Description"))
-  amount = fields.Float(string=_("Amount"))
-  discount = fields.Float(string=_("Discount"))
-  ttype = fields.Char(string=_("Type"))
-  license_plate = fields.Char(string=_("License Plate (car)"))
-  reservation_compute_id = fields.Many2one('smp.sm_reservation_compute', string=_("Related reservation"))
-  related_invoice_id = fields.Many2one('account.invoice', string=_("Related invoice"))
-  related_member_id = fields.Many2one('res.partner', string=_("Related member"),
-    compute="_get_related_member_id", store=True)
-  cs_user_type = fields.Char(string=_("cs user type"),
-    compute="_get_cs_user_type", store=True)
-  reservation_compute_invoiced = fields.Boolean(string=_("Compute invoiced"),
-    compute="_check_compute_invoiced", store=True)
-  reservation_compute_forgiven = fields.Boolean(string=_("Compute forgiven"),
-    compute="_check_compute_forgiven", store=True)
-
-  _order = "date desc"
-
-  @api.depends('date', 'hour', 'ttype', 'license_plate')
-  def _teletac_name(self):
-    for record in self:
-      record.name = str(record.date) + ' - ' + str(record.hour) + ' - ' + str(record.ttype) + ' - ' \
-        + str(record.license_plate)
-
-  @api.depends('reservation_compute_id', 'related_invoice_id')
-  def _check_compute_invoiced(self):
-    for record in self:
-      if record.reservation_compute_id.id:
-        record.reservation_compute_invoiced = record.reservation_compute_id.compute_invoiced
-      else:
-        record.reservation_compute_invoiced = False
-
-  @api.depends('reservation_compute_id', 'related_invoice_id')
-  def _check_compute_forgiven(self):
-    for record in self:
-      if record.reservation_compute_id.id:
-        record.reservation_compute_forgiven = record.reservation_compute_id.compute_forgiven
-      else:
-        record.reservation_compute_forgiven = False
-
-  @api.depends('reservation_compute_id')
-  def _get_related_member_id(self):
-    for record in self:
-      if record.reservation_compute_id.id:
-        record.related_member_id = record.reservation_compute_id.member_id
-      else:
-        record.related_member_id = False
-
-  @api.depends('related_member_id')
-  def _get_cs_user_type(self):
-    for record in self:
-      if record.reservation_compute_id.id:
-        record.cs_user_type = record.related_member_id.cs_user_type
-
-  @api.multi
-  def compute(self):
-    if self.env.context:
-      if 'active_ids' in self.env.context:
-        teletacs = self.env['smp.sm_teletac'].browse(self.env.context['active_ids'])
-        if teletacs.exists():
-          company = self.env.user.company_id
-          q_car_owner_group_index = company.sm_carsharing_api_credentials_admin_group
-          for teletac in teletacs:
-            car = self.env['smp.sm_car'].search([
-              ('license_plate', '=like', teletac.license_plate+"%"),
-              ('owner_group_index','=',q_car_owner_group_index)
-            ])
-            if car.exists():
-              query = [
-                ('current_car', 'like', car[0].name),
-                ('effectiveStartTime', '<=', str(sm_utils.local_to_utc_datetime(str(teletac.date) + ' ' + teletac.hour))),
-                ('effectiveEndTime', '>=', str(sm_utils.local_to_utc_datetime(str(teletac.date) + ' ' + teletac.hour)))
-              ]
-              computes = self.env['smp.sm_reservation_compute'].search(query)
-              if computes.exists():
-                teletac.write({
-                  'reservation_compute_id': computes[0].id
-                })
-    return sm_resources.getInstance().get_successful_action_message(self, _('Compute done successfully'), self._name)
-
-  @api.multi
-  def reset_state(self):
-    if self.env.context:
-      if 'active_ids' in self.env.context:
-        teletacs = self.env['smp.sm_teletac'].browse(self.env.context['active_ids'])
-        if teletacs.exists():
-          for teletac in teletacs:
-            teletac.related_invoice_id = None
-            teletac.invoice_report_id = None
-            teletac.reservation_compute_invoiced = False
+    name = fields.Char(string=_("Name"), compute="_teletac_name")
+    date = fields.Date(string=_("Date"))
+    hour = fields.Char(string=_("Hour"))
+    description = fields.Char(string=_("Description"))
+    amount = fields.Float(string=_("Amount"))
+    discount = fields.Float(string=_("Discount"))
+    ttype = fields.Char(string=_("Type"))
+    license_plate = fields.Char(string=_("License Plate (car)"))
+    reservation_compute_id = fields.Many2one(
+        'smp.sm_reservation_compute', string=_("Related reservation"))
+    related_invoice_id = fields.Many2one(
+        'account.invoice', string=_("Related invoice"))
+    related_member_id = fields.Many2one(
+        'res.partner', string=_("Related member"),
+        compute="_get_related_member_id", store=True)
+    cs_user_type = fields.Char(
+        string=_("cs user type"),
+        compute="_get_cs_user_type", store=True)
+    reservation_compute_invoiced = fields.Boolean(
+        string=_("Compute invoiced"),
+        compute="_check_compute_invoiced", store=True)
+    reservation_compute_forgiven = fields.Boolean(
+        string=_("Compute forgiven"),
+        compute="_check_compute_forgiven", store=True)
+
+    _order = "date desc"
+
+    @api.depends('date', 'hour', 'ttype', 'license_plate')
+    def _teletac_name(self):
+        for record in self:
+            record.name = str(record.date) + ' - ' + str(record.hour) + ' - ' + str(record.ttype) + ' - ' \
+                + str(record.license_plate)
+
+    @api.depends('reservation_compute_id', 'related_invoice_id')
+    def _check_compute_invoiced(self):
+        for record in self:
+            if record.reservation_compute_id.id:
+                record.reservation_compute_invoiced = record.reservation_compute_id.compute_invoiced
+            else:
+                record.reservation_compute_invoiced = False
+
+    @api.depends('reservation_compute_id', 'related_invoice_id')
+    def _check_compute_forgiven(self):
+        for record in self:
+            if record.reservation_compute_id.id:
+                record.reservation_compute_forgiven = record.reservation_compute_id.compute_forgiven
+            else:
+                record.reservation_compute_forgiven = False
+
+    @api.depends('reservation_compute_id')
+    def _get_related_member_id(self):
+        for record in self:
+            if record.reservation_compute_id.id:
+                record.related_member_id = record.reservation_compute_id.member_id
+            else:
+                record.related_member_id = False
+
+    @api.depends('related_member_id')
+    def _get_cs_user_type(self):
+        for record in self:
+            if record.reservation_compute_id.id:
+                record.cs_user_type = record.related_member_id.cs_user_type
+
+    @api.multi
+    def compute(self):
+        if self.env.context:
+            if 'active_ids' in self.env.context:
+                teletacs = self.env['smp.sm_teletac'].browse(
+                    self.env.context['active_ids'])
+                if teletacs.exists():
+                    company = self.env.user.company_id
+                    q_car_owner_group_index = company.sm_carsharing_api_credentials_admin_group
+                    for teletac in teletacs:
+                        car = self.env['smp.sm_car'].search([
+                            ('license_plate', '=like', teletac.license_plate+"%"),
+                            ('owner_group_index', '=', q_car_owner_group_index)
+                        ])
+                        if car.exists():
+                            query = [
+                                ('current_car', 'like', car[0].name),
+                                ('effectiveStartTime', '<=', str(sm_utils.local_to_utc_datetime(
+                                    str(teletac.date) + ' ' + teletac.hour))),
+                                ('effectiveEndTime', '>=', str(sm_utils.local_to_utc_datetime(
+                                    str(teletac.date) + ' ' + teletac.hour)))
+                            ]
+                            computes = self.env['smp.sm_reservation_compute'].search(
+                                query)
+                            if computes.exists():
+                                teletac.write({
+                                    'reservation_compute_id': computes[0].id
+                                })
+        return sm_resources.getInstance().get_successful_action_message(self, _('Compute done successfully'), self._name)
+
+    @api.multi
+    def reset_state(self):
+        if self.env.context:
+            if 'active_ids' in self.env.context:
+                teletacs = self.env['smp.sm_teletac'].browse(
+                    self.env.context['active_ids'])
+                if teletacs.exists():
+                    for teletac in teletacs:
+                        teletac.related_invoice_id = None
+                        teletac.invoice_report_id = None
+                        teletac.reservation_compute_invoiced = False
```

## Comparing `odoo12_addon_sm_teletacs-12.0.0.0.5.dist-info/RECORD` & `odoo12_addon_sm_teletacs-12.0.0.0.5.99.dev1.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 odoo/addons/sm_teletacs/__init__.py,sha256=Z0H-7tnW3JmMNtRFk_MxwVzutPYWpm0Ljnk9Fb4hEoc,45
-odoo/addons/sm_teletacs/__manifest__.py,sha256=clKfeLOWkBCk_HnxmIF_yB6rRLjWfGWj6r1OSdXjejI,792
+odoo/addons/sm_teletacs/__manifest__.py,sha256=in0AAsgX05Lo9YwxoctbXWRewzf7eE2qsi8LWu67fKY,613
 odoo/addons/sm_teletacs/models/__init__.py,sha256=KB0vDguCizQQufZRrOQ-Bi_Qq3CC1KqclV7GDDoFqxI,57
-odoo/addons/sm_teletacs/models/models_smp_teletac.py,sha256=8aiAHVhIaW2im7tQjmIJbPjexkmEAjN1SpObQ7xMGPU,4474
+odoo/addons/sm_teletacs/models/models_smp_teletac.py,sha256=eu7dytHJ8G8Ti1s8eofga0uVuqb-b4JasdHdSK4XoSs,5237
 odoo/addons/sm_teletacs/security/ir.model.access.csv,sha256=mPj3TkZIvKgk8vj8EKDxGwtbIZq3FLcD6a4h-lcY7NQ,140
 odoo/addons/sm_teletacs/views/views_teletac.xml,sha256=FUU6WhVKjwI1WG7FRjQxP2Z4dyXFnXTlTOgYhzgdmVE,3876
-odoo12_addon_sm_teletacs-12.0.0.0.5.dist-info/METADATA,sha256=GmKGxCkauYeZRStH69h4EupohjajzemsjDgLICaAE0Q,500
-odoo12_addon_sm_teletacs-12.0.0.0.5.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-odoo12_addon_sm_teletacs-12.0.0.0.5.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo12_addon_sm_teletacs-12.0.0.0.5.dist-info/RECORD,,
+odoo12_addon_sm_teletacs-12.0.0.0.5.99.dev1.dist-info/METADATA,sha256=TbLf49c-VQrxjgpEjv14C-1MM7crfMmRH8UPZ1ZYLrM,507
+odoo12_addon_sm_teletacs-12.0.0.0.5.99.dev1.dist-info/WHEEL,sha256=-G_t0oGuE7UD0DrSpVZnq1hHMBV9DD2XkS5v7XpmTnk,110
+odoo12_addon_sm_teletacs-12.0.0.0.5.99.dev1.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo12_addon_sm_teletacs-12.0.0.0.5.99.dev1.dist-info/RECORD,,
```

