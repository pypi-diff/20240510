# Comparing `tmp/CTkSpinbox-1.3.0.tar.gz` & `tmp/ctkspinbox-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CTkSpinbox-1.3.0.tar", last modified: Wed Jan 31 12:56:54 2024, max compression
+gzip compressed data, was "ctkspinbox-1.4.0.tar", last modified: Fri May 10 18:19:00 2024, max compression
```

## Comparing `CTkSpinbox-1.3.0.tar` & `ctkspinbox-1.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-01-31 12:56:54.599339 CTkSpinbox-1.3.0/
--rw-rw-rw-   0        0        0     1078 2023-08-12 07:53:34.000000 CTkSpinbox-1.3.0/LICENSE
--rw-rw-rw-   0        0        0     4557 2024-01-31 12:56:54.599339 CTkSpinbox-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     4002 2024-01-31 12:44:26.000000 CTkSpinbox-1.3.0/README.md
--rw-rw-rw-   0        0        0      108 2023-08-10 16:32:04.000000 CTkSpinbox-1.3.0/pyproject.toml
--rw-rw-rw-   0        0        0      694 2024-01-31 12:56:54.599339 CTkSpinbox-1.3.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-01-31 12:56:54.482460 CTkSpinbox-1.3.0/src/
-drwxrwxrwx   0        0        0        0 2024-01-31 12:56:54.515511 CTkSpinbox-1.3.0/src/CTkSpinbox/
--rw-rw-rw-   0        0        0      132 2024-01-31 12:50:22.000000 CTkSpinbox-1.3.0/src/CTkSpinbox/__init__.py
--rw-rw-rw-   0        0        0     8261 2024-01-31 12:51:43.000000 CTkSpinbox-1.3.0/src/CTkSpinbox/ctkspinbox.py
-drwxrwxrwx   0        0        0        0 2024-01-31 12:56:54.596574 CTkSpinbox-1.3.0/src/CTkSpinbox.egg-info/
--rw-rw-rw-   0        0        0     4557 2024-01-31 12:56:54.000000 CTkSpinbox-1.3.0/src/CTkSpinbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2024-01-31 12:56:54.000000 CTkSpinbox-1.3.0/src/CTkSpinbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-31 12:56:54.000000 CTkSpinbox-1.3.0/src/CTkSpinbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-01-31 12:56:54.000000 CTkSpinbox-1.3.0/src/CTkSpinbox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 18:19:00.927311 ctkspinbox-1.4.0/
+-rw-rw-rw-   0        0        0     1078 2023-08-12 07:53:34.000000 ctkspinbox-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0     4557 2024-05-10 18:19:00.927311 ctkspinbox-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4002 2024-01-31 12:44:28.000000 ctkspinbox-1.4.0/README.md
+-rw-rw-rw-   0        0        0      108 2023-08-10 16:32:04.000000 ctkspinbox-1.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0      694 2024-05-10 18:19:00.929860 ctkspinbox-1.4.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-10 18:19:00.874551 ctkspinbox-1.4.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-10 18:19:00.903002 ctkspinbox-1.4.0/src/CTkSpinbox/
+-rw-rw-rw-   0        0        0      132 2024-05-10 17:08:11.000000 ctkspinbox-1.4.0/src/CTkSpinbox/__init__.py
+-rw-rw-rw-   0        0        0     8906 2024-05-10 17:16:19.000000 ctkspinbox-1.4.0/src/CTkSpinbox/ctkspinbox.py
+drwxrwxrwx   0        0        0        0 2024-05-10 18:19:00.926314 ctkspinbox-1.4.0/src/CTkSpinbox.egg-info/
+-rw-rw-rw-   0        0        0     4557 2024-05-10 18:19:00.000000 ctkspinbox-1.4.0/src/CTkSpinbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-05-10 18:19:00.000000 ctkspinbox-1.4.0/src/CTkSpinbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 18:19:00.000000 ctkspinbox-1.4.0/src/CTkSpinbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-10 18:19:00.000000 ctkspinbox-1.4.0/src/CTkSpinbox.egg-info/top_level.txt
```

### Comparing `CTkSpinbox-1.3.0/LICENSE` & `ctkspinbox-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CTkSpinbox-1.3.0/PKG-INFO` & `ctkspinbox-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkSpinbox
-Version: 1.3.0
+Version: 1.4.0
 Summary: A custom spinbox widget for customtkinter.
 Home-page: https://github.com/Sheikh-Rashdan/CTkSpinbox
 Author: Sheikh Rashdan
 Author-email: sheikhmohamedrashdan@gmail.com
 Project-URL: Bug Tracker, https://github.com/Sheikh-Rashdan/CTkSpinbox/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `CTkSpinbox-1.3.0/README.md` & `ctkspinbox-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `CTkSpinbox-1.3.0/setup.cfg` & `ctkspinbox-1.4.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2043 546b 5370 696e 626f 780d 0a76   = CTkSpinbox..v
-00000020: 6572 7369 6f6e 203d 2031 2e33 2e30 0d0a  ersion = 1.3.0..
+00000020: 6572 7369 6f6e 203d 2031 2e34 2e30 0d0a  ersion = 1.4.0..
 00000030: 6175 7468 6f72 203d 2053 6865 696b 6820  author = Sheikh 
 00000040: 5261 7368 6461 6e0d 0a61 7574 686f 725f  Rashdan..author_
 00000050: 656d 6169 6c20 3d20 7368 6569 6b68 6d6f  email = sheikhmo
 00000060: 6861 6d65 6472 6173 6864 616e 4067 6d61  hamedrashdan@gma
 00000070: 696c 2e63 6f6d 0d0a 6465 7363 7269 7074  il.com..descript
 00000080: 696f 6e20 3d20 4120 6375 7374 6f6d 2073  ion = A custom s
 00000090: 7069 6e62 6f78 2077 6964 6765 7420 666f  pinbox widget fo
```

### Comparing `CTkSpinbox-1.3.0/src/CTkSpinbox/ctkspinbox.py` & `ctkspinbox-1.4.0/src/CTkSpinbox/ctkspinbox.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 """
 Custom Spinbox For CustomTkinter
 Author : Sheikh Rashdan
-Version : 1.3
+Version : 1.4
 """
 
+'''CHANGELOG:
+ • 1.4:
+    - Fixed scrollwheel interaction when widget was disabled. (Reported By : RaymondWK)
+'''
+
 import customtkinter as ctk
 
 class CTkSpinbox(ctk.CTkFrame):
     def __init__(self,
                  master: any,
                  width: int = 100,                            # width of the frame
                  height: int = 40,                            # height of the frame
@@ -24,14 +29,15 @@
                  button_color: str = ('#BBB','#444'),
                  button_hover_color: str = ('#AAA', '#555'),
                  border_width: int = 2,
                  corner_radius: int = 5,
                  button_corner_radius: int = 5,
                  button_border_width: int = 2,
                  button_border_color: str = ('#AAA', '#555'),
+                 state: str = 'normal',
                  command: any = None):
         super().__init__(master,
                          height = height,
                          width = width,
                          fg_color = fg_color,
                          border_color = border_color,
                          border_width = border_width,
@@ -49,14 +55,15 @@
         self.font = font
         self.text_color = text_color
         self.button_color = button_color
         self.button_hover_color = button_hover_color
         self.button_corner_radius = button_corner_radius 
         self.button_border_width = button_border_width
         self.button_border_color = button_border_color
+        self.state = state
         self.command = command
 
         # counter label
         self.counter_var = ctk.IntVar(value = self.start_value)
         self.counter = ctk.CTkLabel(self,
                                     text = 'Error',
                                     textvariable = self.counter_var,
@@ -99,14 +106,18 @@
         self.decrement.grid(row = 0, column = 0, sticky = 'news', padx = (4,0), pady = 4)
         self.counter.grid(row = 0, column = 1, sticky = 'news', padx = 0, pady = 4)
         self.increment.grid(row = 0, column = 2, sticky = 'news', padx = (0,4), pady = 4)
 
         # scroll bind
         self.bind('<MouseWheel>', self.scroll)
 
+        # update state
+        if self.state == 'disabled':
+            self.disable()
+
     def decrement_counter(self):
         self.counter_var.set(max(self.min_value, self.counter_var.get()-self.step_value))
         if self.variable:
             self.variable.set(self.counter_var.get())
         if self.command:
             self.command(self.counter_var.get())
 
@@ -114,35 +125,38 @@
         self.counter_var.set(min(self.max_value, self.counter_var.get()+self.step_value))
         if self.variable:
             self.variable.set(self.counter_var.get())
         if self.command:
             self.command(self.counter_var.get())
 
     def scroll(self, scroll):
-        dirn = 1 if scroll.delta>0 else -1
-        if dirn == -1:
-            self.counter_var.set(max(self.min_value, self.counter_var.get()-self.scroll_value))
-        else:
-            self.counter_var.set(min(self.max_value, self.counter_var.get()+self.scroll_value))
-        if self.variable:
-            self.variable.set(self.counter_var.get())
-        if self.command:
-            self.command(self.counter_var.get())
+        if self.state == 'normal':
+            dirn = 1 if scroll.delta>0 else -1
+            if dirn == -1:
+                self.counter_var.set(max(self.min_value, self.counter_var.get()-self.scroll_value))
+            else:
+                self.counter_var.set(min(self.max_value, self.counter_var.get()+self.scroll_value))
+            if self.variable:
+                self.variable.set(self.counter_var.get())
+            if self.command:
+                self.command(self.counter_var.get())
 
     def get(self):
         return self.counter_var.get()
     
     def set(self, value):
         self.counter_var.set(max(min(value, self.max_value), self.min_value))
     
     def disable(self):
+        self.state = 'disabled'
         self.increment.configure(state = 'disabled')
         self.decrement.configure(state = 'disabled')
 
     def enable(self):
+        self.state = 'normal'
         self.increment.configure(state = 'enabled')
         self.decrement.configure(state = 'enabled')
 
     def bind(self, key, function, add = True):
 
         super().bind(key, function, add)
         self.counter.bind(key, function, add)
@@ -171,9 +185,15 @@
         for value in ['min_value', 'max_value', 'step_value', 'scroll_value', 'variable']:
             if value in kwargs:
                 new_value = kwargs.pop(value)
                 exec(f'self.{value} = {new_value}')
 
         if 'command' in kwargs:
             self.command = kwargs.pop('command')
+        elif 'state' in kwargs:
+            self.state = kwargs.pop('state')
+            if self.state == 'normal':
+                self.enable()
+            elif self.state == 'disabled':
+                self.disable()
 
         super().configure(**kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `CTkSpinbox-1.3.0/src/CTkSpinbox.egg-info/PKG-INFO` & `ctkspinbox-1.4.0/src/CTkSpinbox.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkSpinbox
-Version: 1.3.0
+Version: 1.4.0
 Summary: A custom spinbox widget for customtkinter.
 Home-page: https://github.com/Sheikh-Rashdan/CTkSpinbox
 Author: Sheikh Rashdan
 Author-email: sheikhmohamedrashdan@gmail.com
 Project-URL: Bug Tracker, https://github.com/Sheikh-Rashdan/CTkSpinbox/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

