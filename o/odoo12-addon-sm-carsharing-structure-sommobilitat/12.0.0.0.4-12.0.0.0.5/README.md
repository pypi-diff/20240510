# Comparing `tmp/odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.4.tar.gz` & `tmp/odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.4.tar", last modified: Tue Apr 30 09:49:01 2024, max compression
+gzip compressed data, was "odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.5.tar", last modified: Fri May 10 10:50:54 2024, max compression
```

## Comparing `odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.4.tar` & `odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 jrobles   (1001) jrobles   (1001)        0 2024-04-30 09:49:01.150329 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.4/
--rw-rw-r--   0 jrobles   (1001) jrobles   (1001)      423 2024-04-30 09:49:01.150329 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.4/PKG-INFO
-drwxrwxr-x   0 jrobles   (1001) jrobles   (1001)        0 2024-04-30 09:49:01.146329 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.4/odoo/
-drwxrwxr-x   0 jrobles   (1001) jrobles   (1001)        0 2024-04-30 09:49:01.146329 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.4/odoo/addons/
-drwxrwxr-x   0 jrobles   (1001) jrobles   (1001)        0 2024-04-30 09:49:01.146329 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.4/odoo/addons/sm_carsharing_structure_sommobilitat/
--rw-rw-r--   0 jrobles   (1001) jrobles   (1001)       46 2024-04-30 09:15:18.000000 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.4/odoo/addons/sm_carsharing_structure_sommobilitat/__init__.py
--rw-rw-r--   0 jrobles   (1001) jrobles   (1001)      674 2024-04-30 09:15:18.000000 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.4/odoo/addons/sm_carsharing_structure_sommobilitat/__manifest__.py
-drwxrwxr-x   0 jrobles   (1001) jrobles   (1001)        0 2024-04-30 09:49:01.146329 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.4/odoo/addons/sm_carsharing_structure_sommobilitat/data/
--rw-rw-r--   0 jrobles   (1001) jrobles   (1001)     1312 2024-04-30 09:15:18.000000 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.4/odoo/addons/sm_carsharing_structure_sommobilitat/data/fleet_vehicle_state.xml
-drwxrwxr-x   0 jrobles   (1001) jrobles   (1001)        0 2024-04-30 09:49:01.150329 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.4/odoo/addons/sm_carsharing_structure_sommobilitat/models/
--rw-rw-r--   0 jrobles   (1001) jrobles   (1001)       87 2024-04-30 09:15:18.000000 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.4/odoo/addons/sm_carsharing_structure_sommobilitat/models/__init__.py
--rw-rw-r--   0 jrobles   (1001) jrobles   (1001)      215 2024-04-30 09:15:18.000000 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.4/odoo/addons/sm_carsharing_structure_sommobilitat/models/fleet_vehicle_state.py
--rw-rw-r--   0 jrobles   (1001) jrobles   (1001)     5914 2024-04-30 09:15:18.000000 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.4/odoo/addons/sm_carsharing_structure_sommobilitat/models/models_cs_car.py
-drwxrwxr-x   0 jrobles   (1001) jrobles   (1001)        0 2024-04-30 09:49:01.150329 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.4/odoo/addons/sm_carsharing_structure_sommobilitat/security/
--rw-rw-r--   0 jrobles   (1001) jrobles   (1001)       76 2023-12-19 17:24:31.000000 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.4/odoo/addons/sm_carsharing_structure_sommobilitat/security/ir.model.access.csv
-drwxrwxr-x   0 jrobles   (1001) jrobles   (1001)        0 2024-04-30 09:49:01.150329 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.4/odoo/addons/sm_carsharing_structure_sommobilitat/views/
--rw-rw-r--   0 jrobles   (1001) jrobles   (1001)      641 2024-04-30 09:15:18.000000 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.4/odoo/addons/sm_carsharing_structure_sommobilitat/views/fleet_vehicle_state_view.xml
--rw-rw-r--   0 jrobles   (1001) jrobles   (1001)    13779 2024-04-30 09:15:18.000000 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.4/odoo/addons/sm_carsharing_structure_sommobilitat/views/views_cs_car.xml
-drwxrwxr-x   0 jrobles   (1001) jrobles   (1001)        0 2024-04-30 09:49:01.150329 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.4/odoo12_addon_sm_carsharing_structure_sommobilitat.egg-info/
--rw-rw-r--   0 jrobles   (1001) jrobles   (1001)      423 2024-04-30 09:49:01.000000 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.4/odoo12_addon_sm_carsharing_structure_sommobilitat.egg-info/PKG-INFO
--rw-rw-r--   0 jrobles   (1001) jrobles   (1001)     1112 2024-04-30 09:49:01.000000 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.4/odoo12_addon_sm_carsharing_structure_sommobilitat.egg-info/SOURCES.txt
--rw-rw-r--   0 jrobles   (1001) jrobles   (1001)        1 2024-04-30 09:49:01.000000 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.4/odoo12_addon_sm_carsharing_structure_sommobilitat.egg-info/dependency_links.txt
--rw-rw-r--   0 jrobles   (1001) jrobles   (1001)        1 2024-04-30 09:49:01.000000 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.4/odoo12_addon_sm_carsharing_structure_sommobilitat.egg-info/not-zip-safe
--rw-rw-r--   0 jrobles   (1001) jrobles   (1001)      117 2024-04-30 09:49:01.000000 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.4/odoo12_addon_sm_carsharing_structure_sommobilitat.egg-info/requires.txt
--rw-rw-r--   0 jrobles   (1001) jrobles   (1001)        5 2024-04-30 09:49:01.000000 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.4/odoo12_addon_sm_carsharing_structure_sommobilitat.egg-info/top_level.txt
--rw-rw-r--   0 jrobles   (1001) jrobles   (1001)       67 2024-04-30 09:49:01.150329 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.4/setup.cfg
--rw-rw-r--   0 jrobles   (1001) jrobles   (1001)      100 2023-12-19 17:24:31.000000 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.4/setup.py
+drwxrwxr-x   0 jrobles   (1001) jrobles   (1001)        0 2024-05-10 10:50:54.405095 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.5/
+-rw-rw-r--   0 jrobles   (1001) jrobles   (1001)      423 2024-05-10 10:50:54.405095 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.5/PKG-INFO
+drwxrwxr-x   0 jrobles   (1001) jrobles   (1001)        0 2024-05-10 10:50:54.401095 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.5/odoo/
+drwxrwxr-x   0 jrobles   (1001) jrobles   (1001)        0 2024-05-10 10:50:54.401095 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.5/odoo/addons/
+drwxrwxr-x   0 jrobles   (1001) jrobles   (1001)        0 2024-05-10 10:50:54.401095 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.5/odoo/addons/sm_carsharing_structure_sommobilitat/
+-rw-rw-r--   0 jrobles   (1001) jrobles   (1001)       46 2024-04-30 09:15:18.000000 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.5/odoo/addons/sm_carsharing_structure_sommobilitat/__init__.py
+-rw-rw-r--   0 jrobles   (1001) jrobles   (1001)      674 2024-05-10 10:49:08.000000 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.5/odoo/addons/sm_carsharing_structure_sommobilitat/__manifest__.py
+drwxrwxr-x   0 jrobles   (1001) jrobles   (1001)        0 2024-05-10 10:50:54.401095 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.5/odoo/addons/sm_carsharing_structure_sommobilitat/data/
+-rw-rw-r--   0 jrobles   (1001) jrobles   (1001)     1312 2024-05-03 11:54:28.000000 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.5/odoo/addons/sm_carsharing_structure_sommobilitat/data/fleet_vehicle_state.xml
+drwxrwxr-x   0 jrobles   (1001) jrobles   (1001)        0 2024-05-10 10:50:54.405095 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.5/odoo/addons/sm_carsharing_structure_sommobilitat/models/
+-rw-rw-r--   0 jrobles   (1001) jrobles   (1001)       87 2024-05-03 11:54:28.000000 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.5/odoo/addons/sm_carsharing_structure_sommobilitat/models/__init__.py
+-rw-rw-r--   0 jrobles   (1001) jrobles   (1001)      215 2024-05-03 11:54:28.000000 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.5/odoo/addons/sm_carsharing_structure_sommobilitat/models/fleet_vehicle_state.py
+-rw-rw-r--   0 jrobles   (1001) jrobles   (1001)     7478 2024-05-10 10:49:08.000000 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.5/odoo/addons/sm_carsharing_structure_sommobilitat/models/models_cs_car.py
+drwxrwxr-x   0 jrobles   (1001) jrobles   (1001)        0 2024-05-10 10:50:54.405095 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.5/odoo/addons/sm_carsharing_structure_sommobilitat/security/
+-rw-rw-r--   0 jrobles   (1001) jrobles   (1001)       76 2023-12-19 17:24:31.000000 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.5/odoo/addons/sm_carsharing_structure_sommobilitat/security/ir.model.access.csv
+drwxrwxr-x   0 jrobles   (1001) jrobles   (1001)        0 2024-05-10 10:50:54.405095 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.5/odoo/addons/sm_carsharing_structure_sommobilitat/views/
+-rw-rw-r--   0 jrobles   (1001) jrobles   (1001)      641 2024-05-03 11:54:28.000000 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.5/odoo/addons/sm_carsharing_structure_sommobilitat/views/fleet_vehicle_state_view.xml
+-rw-rw-r--   0 jrobles   (1001) jrobles   (1001)    14640 2024-05-10 10:49:08.000000 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.5/odoo/addons/sm_carsharing_structure_sommobilitat/views/views_cs_car.xml
+drwxrwxr-x   0 jrobles   (1001) jrobles   (1001)        0 2024-05-10 10:50:54.405095 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.5/odoo12_addon_sm_carsharing_structure_sommobilitat.egg-info/
+-rw-rw-r--   0 jrobles   (1001) jrobles   (1001)      423 2024-05-10 10:50:54.000000 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.5/odoo12_addon_sm_carsharing_structure_sommobilitat.egg-info/PKG-INFO
+-rw-rw-r--   0 jrobles   (1001) jrobles   (1001)     1112 2024-05-10 10:50:54.000000 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.5/odoo12_addon_sm_carsharing_structure_sommobilitat.egg-info/SOURCES.txt
+-rw-rw-r--   0 jrobles   (1001) jrobles   (1001)        1 2024-05-10 10:50:54.000000 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.5/odoo12_addon_sm_carsharing_structure_sommobilitat.egg-info/dependency_links.txt
+-rw-rw-r--   0 jrobles   (1001) jrobles   (1001)        1 2024-04-30 09:49:01.000000 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.5/odoo12_addon_sm_carsharing_structure_sommobilitat.egg-info/not-zip-safe
+-rw-rw-r--   0 jrobles   (1001) jrobles   (1001)      117 2024-05-10 10:50:54.000000 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.5/odoo12_addon_sm_carsharing_structure_sommobilitat.egg-info/requires.txt
+-rw-rw-r--   0 jrobles   (1001) jrobles   (1001)        5 2024-05-10 10:50:54.000000 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.5/odoo12_addon_sm_carsharing_structure_sommobilitat.egg-info/top_level.txt
+-rw-rw-r--   0 jrobles   (1001) jrobles   (1001)       67 2024-05-10 10:50:54.405095 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.5/setup.cfg
+-rw-rw-r--   0 jrobles   (1001) jrobles   (1001)      100 2023-12-19 17:24:31.000000 odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.5/setup.py
```

### Comparing `odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.4/odoo/addons/sm_carsharing_structure_sommobilitat/__manifest__.py` & `odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.5/odoo/addons/sm_carsharing_structure_sommobilitat/__manifest__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     'summary': """
          Extra fields any enterprise would need to add to fleet vehicle""",
 
     'author': "Som Mobilitat",
     'website': "https://www.sommobilitat.coop",
 
     'category': '',
-    'version': '12.0.0.0.4',
+    'version': '12.0.0.0.5',
 
     # any module necessary for this one to work correctly
     'depends': [
         'base',
         'vertical_carsharing',
         'fleet',
         'sm_carsharing_structure',
```

### Comparing `odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.4/odoo/addons/sm_carsharing_structure_sommobilitat/data/fleet_vehicle_state.xml` & `odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.5/odoo/addons/sm_carsharing_structure_sommobilitat/data/fleet_vehicle_state.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.4/odoo/addons/sm_carsharing_structure_sommobilitat/models/models_cs_car.py` & `odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.5/odoo/addons/sm_carsharing_structure_sommobilitat/models/models_cs_car.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 from odoo.tools.translate import _
 import logging
 
 class cs_car(models.Model):
     _name = 'fleet.vehicle'
     _inherit = 'fleet.vehicle'
 
+    def _get_default_state(self):
+        """ Overriden method originally in fleet module! """
+        state = self.env.ref('sm_carsharing_structure_sommobilitat.fleet_vehicle_state_active', raise_if_not_found=False)
+        return state if state and state.id else False
+    
+    
     battery_fee = fields.Selection([
         ('rent', _("Lloguer")),
         ('bougth', _("Compra")),
         ('no-quota', _("Sense Quota"))
     ], string=_("Bateria propietat"), default="rent")
     car_type = fields.Selection([
         ('fp', _("FP")),
@@ -63,26 +69,29 @@
     
     # Dades Vehicle
 
     sm_version = fields.Char(string=_("Versió"))
     tire_type = fields.Char(string=_("Mida rodes"))
     vehicle_license = fields.Char(string=_("Permís circulació"))
     technical_data = fields.Char(string=_("Fitxa tècnica"))
-    ownership = fields.Selection([
+    ownership = fields.Selection(
+        [
             ('owned', 'Owned'),
             ('lesed', 'Lessed'),
             ('rented', 'Rented'),
             ('customer', 'Customer')
         ],
+        default="owned",
         string="Propietat",
     )
     app_service = fields.Boolean(
         string=_("App Service")
     )
 
+
     # Dades Compra
 
     partner_id = fields.Many2one(
         'res.partner',
         string=_("Proveïdor/Concessionàri")
     )
     purchase_invoice_id = fields.Many2one(
@@ -106,14 +115,15 @@
     financing_end_finish = fields.Date(
       string="Data Finalització finançament"
     )
     financing_contract = fields.Char(
       string="Contracte de finançament"
     )
 
+
     # Dades Venda
 
     date_change_name = fields.Date()
     sale_invoice_id = fields.Many2one(
         'account.invoice',
         string="Factura"
     )
@@ -145,14 +155,15 @@
     )
     sale_email = fields.Char(
         string="Email",
         related="sale_partner_id.email",
         readonly=True,
     )
 
+
     # Altres
 
     barcelona_id_code = fields.Char(
         string=_("Codi identificatiu Barcelona"),
         related="live_card",
         store=True,
         readonly=False
@@ -162,14 +173,25 @@
     # Modalitat Servei
 
     contracte_actiu = fields.Many2one(
         'contract.contract',
         string="Contracte actiu"
     )
 
+    state_id = fields.Many2one(
+        'fleet.vehicle.state',
+        'State',
+        default=_get_default_state,
+        group_expand='_read_group_stage_ids',
+        track_visibility="onchange",
+        help='Current state of the vehicle',
+        ondelete="set null"
+    )
+
+
     @api.multi
     @api.onchange('state_id')
     def _onchange_state_id(self):
         for vehicle in self:
             if vehicle.state_id:
                 if vehicle.state_id.archived and vehicle.active:
                     vehicle.active = False
@@ -177,7 +199,37 @@
                     vehicle.active = True
 
     # Dades Propietari
     owner_partner_id = fields.Many2one(
         'res.partner',
         string="Propietari"
     )
+
+
+    @api.multi
+    @api.onchange('license_plate')
+    def _onchange_license_plate(self):
+        for vehicle in self:
+            if vehicle.license_plate:
+                vehicle.license_plate = vehicle.license_plate.replace(" ", "")
+    
+    # Mantenimiento
+
+    # Revisió anual després de compra: (fecha)
+    annual_revision_after_purchase_date = fields.Date(
+        string="Revisió anual després de compra",
+    )
+    # ITV després de compra: (Fecha)
+    itv_after_purchase_date = fields.Date(
+        string="ITV després de compra",
+    )
+    # % rodes davant després de compra: (Integer)
+    front_tire_percent_after_purchase = fields.Integer(
+        string="% rodes davant després de compra",
+    )
+    # % rodes darrera després de compra: (Integer)
+    rear_tire_percent_after_purchase = fields.Integer(
+        string="% rodes darrera després de compra",
+    )
+    document_last_itv = fields.Char(
+        string="Document ITV passada",
+    )
```

### Comparing `odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.4/odoo/addons/sm_carsharing_structure_sommobilitat/views/fleet_vehicle_state_view.xml` & `odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.5/odoo/addons/sm_carsharing_structure_sommobilitat/views/fleet_vehicle_state_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.4/odoo/addons/sm_carsharing_structure_sommobilitat/views/views_cs_car.xml` & `odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.5/odoo/addons/sm_carsharing_structure_sommobilitat/views/views_cs_car.xml`

 * *Files 6% similar despite different names*

#### Comparing `odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.4/odoo/addons/sm_carsharing_structure_sommobilitat/views/views_cs_car.xml` & `odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.5/odoo/addons/sm_carsharing_structure_sommobilitat/views/views_cs_car.xml`

```diff
@@ -5,15 +5,15 @@
       <field name="name">new_fleet_vehicle_form_view_unique</field>
       <field name="model">fleet.vehicle</field>
       <field name="type">form</field>
       <field name="priority">1</field>
       <field name="arch" type="xml">
         <form string="Vehicle">
           <header>
-            <field name="state_id" widget="statusbar" options="{'clickable': '1'}"/>
+            <field name="state_id" widget="statusbar" clickable="True" on_change="1" can_create="true" can_write="true" modifiers="{}"/>
           </header>
           <sheet>
             <div class="oe_button_box" name="button_box">
               <button name="open_assignation_logs" string="Drivers History" type="object" class="oe_stat_button" icon="fa-history"/>
               <button name="return_action_to_open" type="object" class="oe_stat_button" icon="fa-book" context="{'xml_id':'fleet_vehicle_log_contract_action', 'search_default_open': 1}" help="show the contract for this vehicle">
                 <field name="contract_count" widget="statinfo" string="Contracts"/>
               </button>
@@ -39,24 +39,33 @@
               <sup class="oe_edit_only" style="color: #00ad5f">Fleetio</sup>
               <h1>
                 <field name="model_id" placeholder="e.g. Model S"/>
               </h1>
               <label for="sm_version" class="oe_edit_only"/>
               <sup class="oe_edit_only" style="color: #00ad5f">Fleetio</sup>
               <h3>
-                <field name="sm_version" class="oe_inline" placeholder="e.g. 50 R135"/>
+                <field name="sm_version" class="oe_inline" placeholder="Intens R135"/>
               </h3>
               <label for="license_plate" class="oe_edit_only"/>
               <sup class="oe_edit_only" style="color: #00ad5f">Fleetio</sup>
               <h2>
-                <field name="license_plate" required="1" class="oe_inline" placeholder="e.g. PAE 326"/>
+                <field name="license_plate" required="1" class="oe_inline" placeholder="Sense espais 0000AAA"/>
               </h2>
               <label for="tag_ids" class="oe_edit_only"/>
               <field name="tag_ids" widget="many2many_tags" options="{'color_field': 'color', 'no_create_edit': True}"/>
             </div>
+            <group col="2" name="Service type" string="Modalitat Servei">
+              <group>
+                <field name="state_id" string="Estat"/>
+              </group>
+              <group>
+                <field name="analytic_account_id" required="1" string="Compte analític"/>
+                <field name="contracte_actiu" required="0" string="Contracte actiu"/>
+              </group>
+            </group>
             <group col="2" name="Vehicle Data" string="Dades vehicle">
               <group>
                 <field name="vin_sn" required="1" string="Bastidor"/>
                 <label for="odometer" string="Km actuals"/>
                 <div class="o_row">
                   <field name="odometer"/>
                   <field name="odometer_unit"/>
@@ -65,35 +74,36 @@
                 <field name="vehicle_type" required="1" string="Tipus"/>
                 <field name="color" required="1"/>
                 <field name="doors" required="1" string="Portes"/>
               </group>
               <group>
                 <field name="seats" string="Seients" required="1"/>
                 <field name="battery_size" required="1" string="Capacitat bateria"/>
-                <field name="tire_type" required="1"/>
+                <field name="tire_type" required="0"/>
                 <field name="acquisition_date" required="1"/>
                 <field name="vehicle_license"/>
                 <field name="technical_data"/>
               </group>
             </group>
             <group col="2" name="Ownership and Management" string="Propietat i gestió">
               <group>
-                <field name="ownership"/>
+                <field name="ownership" required="True"/>
                 <field name="app_service" string="Servei APP"/>
               </group>
               <group>
                 <!-- ᶠˡᵉᵉᵗⁱᵒ -->
               </group>
             </group>
             <group col="2" name="Propietary Data" string="Dades Propietari" attrs="{'invisible': [('ownership', '!=', 'customer')]}">
               <field name="owner_partner_id" string="Propietari" attrs="{'required': [('ownership', '=', 'customer')]}"/>
             </group>
             <group col="2" name="Purchase Data" string="Dades Compra" attrs="{'invisible': [('ownership', '=', 'customer')]}">
               <group>
-                <field name="partner_id" string="Proveïdor/Concessionàri" attrs="{'required': [('ownership', '!=', 'customer')]}"/>
+                <field name="partner_id" string="Proveïdor/Concessionàri"/>
+                <!-- attrs="{'required': [('ownership', '!=', 'customer')]}" -->
                 <field name="purchase_invoice_id" string="Factura"/>
                 <field name="bougth_date" string="Data de compra"/>
                 <field name="bought_price" string="Preu de compra" widget="monetary"/>
                 <field name="bougth_km" string="Km a la compra"/>
               </group>
               <group>
                 <field name="financing" string="Finançament"/>
@@ -120,21 +130,23 @@
               <group>
                 <field name="barcelona_id_code" string="Codi identificatiu Barcelona" readonly="0"/>
               </group>
               <group>
                 <field name="ivtm_status" string="Tramitada bonificació IVTMS"/>
               </group>
             </group>
-            <group col="2" name="Service type" string="Modalitat Servei">
+            <group col="2" name="Management" string="Mantenimiento">
               <group>
-                <field name="state_id" string="Estat"/>
+                <field name="annual_revision_after_purchase_date" string="Revisió anual després de compra" readonly="0"/>
+                <field name="itv_after_purchase_date" string="ITV després de compra" readonly="0"/>
               </group>
               <group>
-                <field name="analytic_account_id" required="1" string="Compte analític"/>
-                <field name="contracte_actiu" required="0" string="Contracte actiu"/>
+                <field name="front_tire_percent_after_purchase" string="% rodes davant després de compra"/>
+                <field name="rear_tire_percent_after_purchase" string="% rodes darrera després de compra"/>
+                <field name="document_last_itv" string="Document ITV passada"/>
               </group>
             </group>
           </sheet>
           <div class="oe_chatter">
             <field name="message_follower_ids" widget="mail_followers"/>
             <field name="activity_ids" widget="mail_activity"/>
             <field name="message_ids" widget="mail_thread" options="{&quot;thread_level&quot;: 1}"/>
```

### Comparing `odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.4/odoo12_addon_sm_carsharing_structure_sommobilitat.egg-info/SOURCES.txt` & `odoo12-addon-sm_carsharing_structure_sommobilitat-12.0.0.0.5/odoo12_addon_sm_carsharing_structure_sommobilitat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

