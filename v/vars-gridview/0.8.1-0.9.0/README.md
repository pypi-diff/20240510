# Comparing `tmp/vars_gridview-0.8.1.tar.gz` & `tmp/vars_gridview-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vars_gridview-0.8.1.tar", max compression
+gzip compressed data, was "vars_gridview-0.9.0.tar", max compression
```

## Comparing `vars_gridview-0.8.1.tar` & `vars_gridview-0.9.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1104 2023-12-12 16:11:17.312857 vars_gridview-0.8.1/LICENSE
--rw-r--r--   0        0        0     1267 2023-12-12 16:11:17.312857 vars_gridview-0.8.1/README.md
--rw-r--r--   0        0        0     2400 2023-12-12 16:11:17.312857 vars_gridview-0.8.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-12 16:11:17.312857 vars_gridview-0.8.1/vars_gridview/__init__.py
--rw-r--r--   0        0        0      970 2023-12-12 16:11:17.312857 vars_gridview-0.8.1/vars_gridview/assets/base_query.sql
--rw-r--r--   0        0        0    17305 2023-12-12 16:11:17.312857 vars_gridview-0.8.1/vars_gridview/assets/gridview.ui
--rw-r--r--   0        0        0       90 2023-12-12 16:11:17.312857 vars_gridview-0.8.1/vars_gridview/assets/icons/README.md
--rw-r--r--   0        0        0    74956 2023-12-12 16:11:17.312857 vars_gridview-0.8.1/vars_gridview/assets/icons/VARSGridView.icns
--rw-r--r--   0        0        0     8595 2023-12-12 16:11:17.312857 vars_gridview-0.8.1/vars_gridview/assets/icons/VARSGridView.iconset/icon_128.png
--rw-r--r--   0        0        0     1568 2023-12-12 16:11:17.312857 vars_gridview-0.8.1/vars_gridview/assets/icons/VARSGridView.iconset/icon_16.png
--rw-r--r--   0        0        0    17436 2023-12-12 16:11:17.312857 vars_gridview-0.8.1/vars_gridview/assets/icons/VARSGridView.iconset/icon_256.png
--rw-r--r--   0        0        0     2475 2023-12-12 16:11:17.312857 vars_gridview-0.8.1/vars_gridview/assets/icons/VARSGridView.iconset/icon_32.png
--rw-r--r--   0        0        0    36456 2023-12-12 16:11:17.316857 vars_gridview-0.8.1/vars_gridview/assets/icons/VARSGridView.iconset/icon_512.png
--rw-r--r--   0        0        0     1283 2023-12-12 16:11:17.316857 vars_gridview-0.8.1/vars_gridview/assets/icons/gear-solid.svg
--rw-r--r--   0        0        0      480 2023-12-12 16:11:17.316857 vars_gridview-0.8.1/vars_gridview/assets/icons/magnifying-glass-solid.svg
--rw-r--r--   0        0        0    31829 2023-12-12 16:11:17.316857 vars_gridview-0.8.1/vars_gridview/assets/style/dark.qss
--rw-r--r--   0        0        0        0 2023-12-12 16:11:17.316857 vars_gridview-0.8.1/vars_gridview/lib/__init__.py
--rw-r--r--   0        0        0     5114 2023-12-12 16:11:17.316857 vars_gridview-0.8.1/vars_gridview/lib/annotation.py
--rw-r--r--   0        0        0     8475 2023-12-12 16:11:17.316857 vars_gridview-0.8.1/vars_gridview/lib/boxes.py
--rw-r--r--   0        0        0     5863 2023-12-12 16:11:17.316857 vars_gridview-0.8.1/vars_gridview/lib/cache.py
--rw-r--r--   0        0        0     1143 2023-12-12 16:11:17.316857 vars_gridview-0.8.1/vars_gridview/lib/constants.py
--rw-r--r--   0        0        0    39509 2023-12-12 16:11:17.316857 vars_gridview-0.8.1/vars_gridview/lib/image_mosaic.py
--rw-r--r--   0        0        0     1915 2023-12-12 16:11:17.316857 vars_gridview-0.8.1/vars_gridview/lib/log.py
--rw-r--r--   0        0        0     2086 2023-12-12 16:11:17.316857 vars_gridview-0.8.1/vars_gridview/lib/m3/__init__.py
--rw-r--r--   0        0        0     5566 2023-12-12 16:11:17.316857 vars_gridview-0.8.1/vars_gridview/lib/m3/clients.py
--rw-r--r--   0        0        0    10984 2023-12-12 16:11:17.316857 vars_gridview-0.8.1/vars_gridview/lib/m3/operations.py
--rw-r--r--   0        0        0      729 2023-12-12 16:11:17.316857 vars_gridview-0.8.1/vars_gridview/lib/raziel.py
--rw-r--r--   0        0        0     2660 2023-12-12 16:11:17.316857 vars_gridview-0.8.1/vars_gridview/lib/settings.py
--rw-r--r--   0        0        0     4670 2023-12-12 16:11:17.316857 vars_gridview-0.8.1/vars_gridview/lib/sort_methods.py
--rw-r--r--   0        0        0     3007 2023-12-12 16:11:17.316857 vars_gridview-0.8.1/vars_gridview/lib/sql.py
--rw-r--r--   0        0        0     2631 2023-12-12 16:11:17.316857 vars_gridview-0.8.1/vars_gridview/lib/util.py
--rw-r--r--   0        0        0    12257 2023-12-12 16:11:17.316857 vars_gridview-0.8.1/vars_gridview/lib/widgets.py
--rw-r--r--   0        0        0        0 2023-12-12 16:11:17.316857 vars_gridview-0.8.1/vars_gridview/scripts/__init__.py
--rw-r--r--   0        0        0    35708 2023-12-12 16:11:17.316857 vars_gridview-0.8.1/vars_gridview/scripts/run.py
--rw-r--r--   0        0        0     1464 2023-12-12 16:11:17.316857 vars_gridview-0.8.1/vars_gridview/ui/ConfirmationDialog.py
--rw-r--r--   0        0        0     1890 2023-12-12 16:11:17.316857 vars_gridview-0.8.1/vars_gridview/ui/FileSelectionLineEdit.py
--rw-r--r--   0        0        0     3598 2023-12-12 16:11:17.316857 vars_gridview-0.8.1/vars_gridview/ui/LoginDialog.py
--rw-r--r--   0        0        0    18701 2023-12-12 16:11:17.316857 vars_gridview-0.8.1/vars_gridview/ui/QueryDialog.py
--rw-r--r--   0        0        0     3586 2023-12-12 16:11:17.316857 vars_gridview-0.8.1/vars_gridview/ui/SortDialog.py
--rw-r--r--   0        0        0        0 2023-12-12 16:11:17.316857 vars_gridview-0.8.1/vars_gridview/ui/__init__.py
--rw-r--r--   0        0        0     3317 2023-12-12 16:11:17.316857 vars_gridview-0.8.1/vars_gridview/ui/settings/SettingsDialog.py
--rw-r--r--   0        0        0        0 2023-12-12 16:11:17.316857 vars_gridview-0.8.1/vars_gridview/ui/settings/__init__.py
--rw-r--r--   0        0        0      822 2023-12-12 16:11:17.316857 vars_gridview-0.8.1/vars_gridview/ui/settings/tabs/AbstractSettingsTab.py
--rw-r--r--   0        0        0     2611 2023-12-12 16:11:17.316857 vars_gridview-0.8.1/vars_gridview/ui/settings/tabs/AppearanceTab.py
--rw-r--r--   0        0        0     2543 2023-12-12 16:11:17.316857 vars_gridview-0.8.1/vars_gridview/ui/settings/tabs/CacheTab.py
--rw-r--r--   0        0        0     1053 2023-12-12 16:11:17.316857 vars_gridview-0.8.1/vars_gridview/ui/settings/tabs/M3Tab.py
--rw-r--r--   0        0        0     2994 2023-12-12 16:11:17.316857 vars_gridview-0.8.1/vars_gridview/ui/settings/tabs/SQLTab.py
--rw-r--r--   0        0        0     4566 2023-12-12 16:11:17.316857 vars_gridview-0.8.1/vars_gridview/ui/settings/tabs/VideoPlayerTab.py
--rw-r--r--   0        0        0        0 2023-12-12 16:11:17.316857 vars_gridview-0.8.1/vars_gridview/ui/settings/tabs/__init__.py
--rw-r--r--   0        0        0     2468 1970-01-01 00:00:00.000000 vars_gridview-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1104 2023-12-13 23:50:13.936178 vars_gridview-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1267 2023-12-13 23:50:13.936178 vars_gridview-0.9.0/README.md
+-rw-r--r--   0        0        0     2400 2023-12-13 23:50:13.936178 vars_gridview-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-13 23:50:13.936178 vars_gridview-0.9.0/vars_gridview/__init__.py
+-rw-r--r--   0        0        0      970 2023-12-13 23:50:13.936178 vars_gridview-0.9.0/vars_gridview/assets/base_query.sql
+-rw-r--r--   0        0        0    17965 2023-12-13 23:50:13.936178 vars_gridview-0.9.0/vars_gridview/assets/gridview.ui
+-rw-r--r--   0        0        0       90 2023-12-13 23:50:13.936178 vars_gridview-0.9.0/vars_gridview/assets/icons/README.md
+-rw-r--r--   0        0        0    74956 2023-12-13 23:50:13.936178 vars_gridview-0.9.0/vars_gridview/assets/icons/VARSGridView.icns
+-rw-r--r--   0        0        0     8595 2023-12-13 23:50:13.936178 vars_gridview-0.9.0/vars_gridview/assets/icons/VARSGridView.iconset/icon_128.png
+-rw-r--r--   0        0        0     1568 2023-12-13 23:50:13.936178 vars_gridview-0.9.0/vars_gridview/assets/icons/VARSGridView.iconset/icon_16.png
+-rw-r--r--   0        0        0    17436 2023-12-13 23:50:13.936178 vars_gridview-0.9.0/vars_gridview/assets/icons/VARSGridView.iconset/icon_256.png
+-rw-r--r--   0        0        0     2475 2023-12-13 23:50:13.936178 vars_gridview-0.9.0/vars_gridview/assets/icons/VARSGridView.iconset/icon_32.png
+-rw-r--r--   0        0        0    36456 2023-12-13 23:50:13.936178 vars_gridview-0.9.0/vars_gridview/assets/icons/VARSGridView.iconset/icon_512.png
+-rw-r--r--   0        0        0     1283 2023-12-13 23:50:13.936178 vars_gridview-0.9.0/vars_gridview/assets/icons/gear-solid.svg
+-rw-r--r--   0        0        0      480 2023-12-13 23:50:13.936178 vars_gridview-0.9.0/vars_gridview/assets/icons/magnifying-glass-solid.svg
+-rw-r--r--   0        0        0    31829 2023-12-13 23:50:13.936178 vars_gridview-0.9.0/vars_gridview/assets/style/dark.qss
+-rw-r--r--   0        0        0        0 2023-12-13 23:50:13.936178 vars_gridview-0.9.0/vars_gridview/lib/__init__.py
+-rw-r--r--   0        0        0     5114 2023-12-13 23:50:13.936178 vars_gridview-0.9.0/vars_gridview/lib/annotation.py
+-rw-r--r--   0        0        0     8475 2023-12-13 23:50:13.936178 vars_gridview-0.9.0/vars_gridview/lib/boxes.py
+-rw-r--r--   0        0        0     5863 2023-12-13 23:50:13.936178 vars_gridview-0.9.0/vars_gridview/lib/cache.py
+-rw-r--r--   0        0        0     1143 2023-12-13 23:50:13.936178 vars_gridview-0.9.0/vars_gridview/lib/constants.py
+-rw-r--r--   0        0        0    39598 2023-12-13 23:50:13.936178 vars_gridview-0.9.0/vars_gridview/lib/image_mosaic.py
+-rw-r--r--   0        0        0     1915 2023-12-13 23:50:13.936178 vars_gridview-0.9.0/vars_gridview/lib/log.py
+-rw-r--r--   0        0        0     2086 2023-12-13 23:50:13.936178 vars_gridview-0.9.0/vars_gridview/lib/m3/__init__.py
+-rw-r--r--   0        0        0     5566 2023-12-13 23:50:13.936178 vars_gridview-0.9.0/vars_gridview/lib/m3/clients.py
+-rw-r--r--   0        0        0    10984 2023-12-13 23:50:13.936178 vars_gridview-0.9.0/vars_gridview/lib/m3/operations.py
+-rw-r--r--   0        0        0      729 2023-12-13 23:50:13.936178 vars_gridview-0.9.0/vars_gridview/lib/raziel.py
+-rw-r--r--   0        0        0     2660 2023-12-13 23:50:13.940178 vars_gridview-0.9.0/vars_gridview/lib/settings.py
+-rw-r--r--   0        0        0     5305 2023-12-13 23:50:13.940178 vars_gridview-0.9.0/vars_gridview/lib/sort_methods.py
+-rw-r--r--   0        0        0     3007 2023-12-13 23:50:13.940178 vars_gridview-0.9.0/vars_gridview/lib/sql.py
+-rw-r--r--   0        0        0     2631 2023-12-13 23:50:13.940178 vars_gridview-0.9.0/vars_gridview/lib/util.py
+-rw-r--r--   0        0        0    12257 2023-12-13 23:50:13.940178 vars_gridview-0.9.0/vars_gridview/lib/widgets.py
+-rw-r--r--   0        0        0        0 2023-12-13 23:50:13.940178 vars_gridview-0.9.0/vars_gridview/scripts/__init__.py
+-rw-r--r--   0        0        0    36449 2023-12-13 23:50:13.940178 vars_gridview-0.9.0/vars_gridview/scripts/run.py
+-rw-r--r--   0        0        0     1464 2023-12-13 23:50:13.940178 vars_gridview-0.9.0/vars_gridview/ui/ConfirmationDialog.py
+-rw-r--r--   0        0        0     1890 2023-12-13 23:50:13.940178 vars_gridview-0.9.0/vars_gridview/ui/FileSelectionLineEdit.py
+-rw-r--r--   0        0        0     3598 2023-12-13 23:50:13.940178 vars_gridview-0.9.0/vars_gridview/ui/LoginDialog.py
+-rw-r--r--   0        0        0    18701 2023-12-13 23:50:13.940178 vars_gridview-0.9.0/vars_gridview/ui/QueryDialog.py
+-rw-r--r--   0        0        0     3749 2023-12-13 23:50:13.940178 vars_gridview-0.9.0/vars_gridview/ui/SortDialog.py
+-rw-r--r--   0        0        0        0 2023-12-13 23:50:13.940178 vars_gridview-0.9.0/vars_gridview/ui/__init__.py
+-rw-r--r--   0        0        0     3317 2023-12-13 23:50:13.940178 vars_gridview-0.9.0/vars_gridview/ui/settings/SettingsDialog.py
+-rw-r--r--   0        0        0        0 2023-12-13 23:50:13.940178 vars_gridview-0.9.0/vars_gridview/ui/settings/__init__.py
+-rw-r--r--   0        0        0      822 2023-12-13 23:50:13.940178 vars_gridview-0.9.0/vars_gridview/ui/settings/tabs/AbstractSettingsTab.py
+-rw-r--r--   0        0        0     2611 2023-12-13 23:50:13.940178 vars_gridview-0.9.0/vars_gridview/ui/settings/tabs/AppearanceTab.py
+-rw-r--r--   0        0        0     2543 2023-12-13 23:50:13.940178 vars_gridview-0.9.0/vars_gridview/ui/settings/tabs/CacheTab.py
+-rw-r--r--   0        0        0     1053 2023-12-13 23:50:13.940178 vars_gridview-0.9.0/vars_gridview/ui/settings/tabs/M3Tab.py
+-rw-r--r--   0        0        0     2994 2023-12-13 23:50:13.940178 vars_gridview-0.9.0/vars_gridview/ui/settings/tabs/SQLTab.py
+-rw-r--r--   0        0        0     4566 2023-12-13 23:50:13.940178 vars_gridview-0.9.0/vars_gridview/ui/settings/tabs/VideoPlayerTab.py
+-rw-r--r--   0        0        0        0 2023-12-13 23:50:13.940178 vars_gridview-0.9.0/vars_gridview/ui/settings/tabs/__init__.py
+-rw-r--r--   0        0        0     2468 1970-01-01 00:00:00.000000 vars_gridview-0.9.0/PKG-INFO
```

### Comparing `vars_gridview-0.8.1/LICENSE` & `vars_gridview-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.8.1/README.md` & `vars_gridview-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.8.1/pyproject.toml` & `vars_gridview-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vars-gridview"
-version = "0.8.1"
+version = "0.9.0"
 description = "VARS GridView is a tool for reviewing and correcting VARS localizations in bulk."
 authors = [
     "Kevin Barnard <kbarnard@mbari.org>",
     "Paul Roberts <proberts@mbari.org>"
 ]
 readme = "README.md"
 repository = "https://github.com/mbari-org/vars-gridview"
```

### Comparing `vars_gridview-0.8.1/vars_gridview/assets/base_query.sql` & `vars_gridview-0.9.0/vars_gridview/assets/base_query.sql`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.8.1/vars_gridview/assets/gridview.ui` & `vars_gridview-0.9.0/vars_gridview/assets/gridview.ui`

 * *Files 2% similar despite different names*

#### Comparing `vars_gridview-0.8.1/vars_gridview/assets/gridview.ui` & `vars_gridview-0.9.0/vars_gridview/assets/gridview.ui`

```diff
@@ -242,14 +242,31 @@
                     </property>
                     <property name="checked">
                       <bool>false</bool>
                     </property>
                   </widget>
                 </item>
                 <item>
+                  <widget class="QCheckBox" name="hideUnlabeled">
+                    <property name="font">
+                      <font>
+                        <pointsize>10</pointsize>
+                        <weight>75</weight>
+                        <bold>true</bold>
+                      </font>
+                    </property>
+                    <property name="text">
+                      <string>Hide Unverified</string>
+                    </property>
+                    <property name="checked">
+                      <bool>false</bool>
+                    </property>
+                  </widget>
+                </item>
+                <item>
                   <widget class="QPushButton" name="sortButton">
                     <property name="font">
                       <font>
                         <pointsize>10</pointsize>
                         <weight>75</weight>
                         <bold>true</bold>
                       </font>
```

### Comparing `vars_gridview-0.8.1/vars_gridview/assets/icons/VARSGridView.icns` & `vars_gridview-0.9.0/vars_gridview/assets/icons/VARSGridView.icns`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.8.1/vars_gridview/assets/icons/VARSGridView.iconset/icon_128.png` & `vars_gridview-0.9.0/vars_gridview/assets/icons/VARSGridView.iconset/icon_128.png`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.8.1/vars_gridview/assets/icons/VARSGridView.iconset/icon_16.png` & `vars_gridview-0.9.0/vars_gridview/assets/icons/VARSGridView.iconset/icon_16.png`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.8.1/vars_gridview/assets/icons/VARSGridView.iconset/icon_256.png` & `vars_gridview-0.9.0/vars_gridview/assets/icons/VARSGridView.iconset/icon_256.png`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.8.1/vars_gridview/assets/icons/VARSGridView.iconset/icon_32.png` & `vars_gridview-0.9.0/vars_gridview/assets/icons/VARSGridView.iconset/icon_32.png`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.8.1/vars_gridview/assets/icons/VARSGridView.iconset/icon_512.png` & `vars_gridview-0.9.0/vars_gridview/assets/icons/VARSGridView.iconset/icon_512.png`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.8.1/vars_gridview/assets/icons/gear-solid.svg` & `vars_gridview-0.9.0/vars_gridview/assets/icons/gear-solid.svg`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.8.1/vars_gridview/assets/style/dark.qss` & `vars_gridview-0.9.0/vars_gridview/assets/style/dark.qss`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.8.1/vars_gridview/lib/annotation.py` & `vars_gridview-0.9.0/vars_gridview/lib/annotation.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.8.1/vars_gridview/lib/boxes.py` & `vars_gridview-0.9.0/vars_gridview/lib/boxes.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.8.1/vars_gridview/lib/cache.py` & `vars_gridview-0.9.0/vars_gridview/lib/cache.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.8.1/vars_gridview/lib/constants.py` & `vars_gridview-0.9.0/vars_gridview/lib/constants.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.8.1/vars_gridview/lib/image_mosaic.py` & `vars_gridview-0.9.0/vars_gridview/lib/image_mosaic.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
         zoom: float = 1.0,
     ):
         super().__init__()
 
         self._rect_widgets: List[RectWidget] = []
         self.roi_map = {}
         self._hide_labeled = True
+        self._hide_unlabeled = True
         self.hide_discarded = True
         self.hide_to_review = True
         self.n_columns = 0
         self._rect_clicked_slot = rect_clicked_slot
 
         # Initialize the graphics
         self._graphics_view: QtWidgets.QGraphicsView = graphics_view
@@ -646,15 +647,15 @@
         # Clear the graphics
         self._clear_graphics_layout()
 
         # Get the subset of rect widgets to render
         rect_widgets_to_render = [
             rw
             for rw in self._rect_widgets
-            if not (self._hide_labeled and rw.is_verified)
+            if (not rw.is_verified and not self._hide_unlabeled) or (rw.is_verified and not self._hide_labeled)
         ]
 
         # Hide all rect widgets that we aren't rendering
         rect_widgets_to_hide = [
             rw for rw in self._rect_widgets if rw not in rect_widgets_to_render
         ]
         for rw in rect_widgets_to_hide:
```

### Comparing `vars_gridview-0.8.1/vars_gridview/lib/log.py` & `vars_gridview-0.9.0/vars_gridview/lib/log.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.8.1/vars_gridview/lib/m3/__init__.py` & `vars_gridview-0.9.0/vars_gridview/lib/m3/__init__.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.8.1/vars_gridview/lib/m3/clients.py` & `vars_gridview-0.9.0/vars_gridview/lib/m3/clients.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.8.1/vars_gridview/lib/m3/operations.py` & `vars_gridview-0.9.0/vars_gridview/lib/m3/operations.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.8.1/vars_gridview/lib/raziel.py` & `vars_gridview-0.9.0/vars_gridview/lib/raziel.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.8.1/vars_gridview/lib/settings.py` & `vars_gridview-0.9.0/vars_gridview/lib/settings.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.8.1/vars_gridview/lib/sort_methods.py` & `vars_gridview-0.9.0/vars_gridview/lib/sort_methods.py`

 * *Files 4% similar despite different names*

```diff
@@ -183,13 +183,36 @@
 
         if depth is None:
             depth = 0.0
 
         return depth
 
 
+def localization_meta_sort(key: str, default: Any) -> SortMethod:
+    """
+    Decorator factory for creating a sort method that sorts by a localization meta key.
+    
+    Args:
+        key: The localization meta key to sort by.
+        default: The default value to use if the key is not present.
+    """
+    def decorator(cls):
+        class LocalizationMetaSort(SortMethod):
+            NAME = cls.NAME
+
+            @staticmethod
+            def key(rect: RectWidget) -> Any:
+                return rect.localization.meta.get(key, default)
+
+        return LocalizationMetaSort
+    
+    return decorator
+
+
+@localization_meta_sort("verifier", "")
 class VerifierSort(SortMethod):
     NAME = "Verifier"
 
-    @staticmethod
-    def key(rect: RectWidget) -> str:
-        return rect.localization.meta.get("verifier", "")
+
+@localization_meta_sort("confidence", 0.0)
+class ConfidenceSort(SortMethod):
+    NAME = "Confidence"
```

### Comparing `vars_gridview-0.8.1/vars_gridview/lib/sql.py` & `vars_gridview-0.9.0/vars_gridview/lib/sql.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.8.1/vars_gridview/lib/util.py` & `vars_gridview-0.9.0/vars_gridview/lib/util.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.8.1/vars_gridview/lib/widgets.py` & `vars_gridview-0.9.0/vars_gridview/lib/widgets.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.8.1/vars_gridview/scripts/run.py` & `vars_gridview-0.9.0/vars_gridview/scripts/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,39 +111,48 @@
         self.sharktopoda_client = None  # Sharktopoda client
         self.sharktopoda_connected = (
             False  # Whether the Sharktopoda client is connected
         )
 
         self.cache_controller = CacheController()
 
+        self._sort_method = RecordedTimestampSort
+
         # Connect signals to slots
         self.ui.discardButton.clicked.connect(self.delete)
         self.ui.clearSelections.clicked.connect(self.clear_selected)
         self.ui.labelSelectedButton.clicked.connect(self.label_selected)
         self.ui.verifySelectedButton.clicked.connect(self.verify_selected)
         self.ui.unverifySelectedButton.clicked.connect(self.unverify_selected)
         self.ui.zoomSpinBox.valueChanged.connect(self.update_zoom)
         # self.ui.sortMethod.currentTextChanged.connect(self.update_layout)
         self.ui.hideLabeled.stateChanged.connect(self.update_layout)
+        self.ui.hideUnlabeled.stateChanged.connect(self.update_layout)
         self.ui.styleComboBox.currentTextChanged.connect(self._style_gui)
         self.ui.openVideo.clicked.connect(self.open_video)
         self.ui.sortButton.clicked.connect(self._sort_widgets)
 
         self._settings = SettingsManager.get_instance()
         self._settings.label_font_size.valueChanged.connect(self.update_layout)
 
         self.settings_dialog = SettingsDialog(
             self._setup_sharktopoda_client,
             self.sharktopodaConnected,
             self._clear_cache,
             parent=self,
         )
 
-        self.ui.roiGraphicsView.viewport().setAttribute(QtCore.Qt.WidgetAttribute.WA_AcceptTouchEvents, False)
-        self.ui.roiDetailGraphicsView.viewport().setAttribute(QtCore.Qt.WidgetAttribute.WA_AcceptTouchEvents, False)
+        self.sort_dialog = SortDialog(parent=self)
+
+        self.ui.roiGraphicsView.viewport().setAttribute(
+            QtCore.Qt.WidgetAttribute.WA_AcceptTouchEvents, False
+        )
+        self.ui.roiDetailGraphicsView.viewport().setAttribute(
+            QtCore.Qt.WidgetAttribute.WA_AcceptTouchEvents, False
+        )
 
         self._launch()
 
     @property
     def loaded(self):
         return self.image_mosaic is not None and self.box_handler is not None
 
@@ -374,24 +383,25 @@
             QtWidgets.QMessageBox.warning(
                 self,
                 "Not Loaded",
                 "No results are loaded, so sorting cannot be performed.",
             )
             return
 
-        # Show a sort dialog
-        sort_dialog = SortDialog(parent=self)
-        ok = sort_dialog.exec()
+        # Show the sort dialog
+        ok = self.sort_dialog.exec()
         if not ok:
             return
-        method = sort_dialog.method
+        method = self.sort_dialog.method
         if method is None:
             return
 
-        self.image_mosaic.sort_rect_widgets(method)
+        self._sort_method = method
+        self.image_mosaic.sort_rect_widgets(self._sort_method)
+
         self.image_mosaic.render_mosaic()
 
     def _do_query(self):
         """
         Perform a query based on the filter string.
         """
         # Show a query dialog
@@ -416,17 +426,18 @@
             self.verifier,
             zoom=self.ui.zoomSpinBox.value() / 100,
         )
 
         self.image_mosaic.hide_discarded = False
         self.image_mosaic.hide_to_review = False
         self.image_mosaic._hide_labeled = self.ui.hideLabeled.isChecked()
+        self.image_mosaic._hide_unlabeled = self.ui.hideUnlabeled.isChecked()
 
-        default_sort_method = RecordedTimestampSort
-        self.image_mosaic.sort_rect_widgets(default_sort_method)
+        self.sort_dialog.clear()
+        self.image_mosaic.sort_rect_widgets(self._sort_method)
         self.image_mosaic.render_mosaic()
 
         # Show some stats about the images and annotations
         self.statusBar().showMessage(
             "Loaded "
             + str(self.image_mosaic.n_images)
             + " images and "
@@ -585,14 +596,17 @@
         if opt == QtWidgets.QMessageBox.StandardButton.Yes:
             # Apply labels to all selected localizations, push to VARS
             self.image_mosaic.label_selected(remapped_concept, part)
 
             # Update the label of the selected localization in the image view (if necessary)
             self.box_handler.update_labels()
 
+            # Render the mosaic
+            self.image_mosaic.render_mosaic()
+
     def verify_selected(self):
         """
         Verify the selected localizations.
         """
         to_verify = self.image_mosaic.get_selected()
         if len(to_verify) > 1:
             opt = QtWidgets.QMessageBox.question(
@@ -603,14 +617,16 @@
             )
         else:
             opt = QtWidgets.QMessageBox.StandardButton.Yes
 
         if opt == QtWidgets.QMessageBox.StandardButton.Yes:
             self.image_mosaic.verify_selected()
 
+            self.image_mosaic.render_mosaic()
+
     def unverify_selected(self):
         """
         Unverify the selected localizations.
         """
         to_unverify = self.image_mosaic.get_selected()
         if len(to_unverify) > 1:
             opt = QtWidgets.QMessageBox.question(
@@ -621,14 +637,16 @@
             )
         else:
             opt = QtWidgets.QMessageBox.StandardButton.Yes
 
         if opt == QtWidgets.QMessageBox.StandardButton.Yes:
             self.image_mosaic.unverify_selected()
 
+            self.image_mosaic.render_mosaic()
+
     @QtCore.pyqtSlot()
     def delete(self):
         if not self.loaded:
             QtWidgets.QMessageBox.warning(
                 self,
                 "Not Loaded",
                 "No results are loaded, so deletions cannot be performed.",
@@ -647,31 +665,33 @@
         if opt == QtWidgets.QMessageBox.StandardButton.Yes:
             self.image_mosaic.delete_selected()
             self.box_handler.roi_detail.clear()
             self.box_handler.clear()
             self.ui.annotationXML.clear()
             self.ui.imageInfoList.clear()
 
+            self.image_mosaic.render_mosaic()
+
     @QtCore.pyqtSlot()
     def clear_selected(self):
         if not self.loaded:
             return
 
         self.image_mosaic.clear_selected()
 
     @QtCore.pyqtSlot()
     def update_layout(self):
         if not self.loaded:
             return
 
-        # method = self.ui.sortMethod.currentData()
         self.image_mosaic.hide_discarded = False
         self.image_mosaic.hide_to_review = False
         self.image_mosaic._hide_labeled = self.ui.hideLabeled.isChecked()
-        # self.image_mosaic.sort_rect_widgets(method)
+        self.image_mosaic._hide_unlabeled = self.ui.hideUnlabeled.isChecked()
+
         self.image_mosaic.render_mosaic()
 
     @QtCore.pyqtSlot(int)
     def update_zoom(self, zoom):
         if not self.loaded:
             return
 
@@ -687,15 +707,22 @@
             ctrl = event.modifiers() & QtCore.Qt.KeyboardModifier.ControlModifier
             shift = event.modifiers() & QtCore.Qt.KeyboardModifier.ShiftModifier
         else:
             ctrl = False
             shift = False
 
         # Save information to VARS for any moved/resized boxes
-        self.box_handler.save_all(self.verifier)
+        try:
+            self.box_handler.save_all(self.verifier)
+        except Exception as e:
+            LOGGER.error(f"Could not save localizations: {e}")
+            QtWidgets.QMessageBox.critical(
+                self, "Error", f"An error occurred while saving localizations: {e}"
+            )
+            return
 
         # Select the widget
         if shift:
             self.image_mosaic.select_range(self.last_selected_rect, rect)
         elif ctrl and rect.is_selected:
             self.image_mosaic.deselect(rect)
         else:
@@ -848,15 +875,15 @@
                 video_reference_uuid, annotation_milliseconds
             )
             self.sharktopoda_client.clear_localizations(video_reference_uuid)
             self.sharktopoda_client.add_localizations(
                 video_reference_uuid, [localization]
             )
             self.sharktopoda_client.show(video_reference_uuid)
-            
+
             # If on macOS, call the open command to bring Sharktopoda to the front
             if sys.platform == "darwin":
                 try:
                     os.system(f"open -a {constants.SHARKTOPODA_APP_NAME}")
                 except Exception as e:
                     LOGGER.warning(f"Could not open Sharktopoda: {e}")
```

### Comparing `vars_gridview-0.8.1/vars_gridview/ui/ConfirmationDialog.py` & `vars_gridview-0.9.0/vars_gridview/ui/ConfirmationDialog.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.8.1/vars_gridview/ui/FileSelectionLineEdit.py` & `vars_gridview-0.9.0/vars_gridview/ui/FileSelectionLineEdit.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.8.1/vars_gridview/ui/LoginDialog.py` & `vars_gridview-0.9.0/vars_gridview/ui/LoginDialog.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.8.1/vars_gridview/ui/QueryDialog.py` & `vars_gridview-0.9.0/vars_gridview/ui/QueryDialog.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.8.1/vars_gridview/ui/SortDialog.py` & `vars_gridview-0.9.0/vars_gridview/ui/SortDialog.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,15 @@
             sm.HeightSort,
             sm.AreaSort,
             sm.MeanIntensitySort,
             sm.MeanHueSort,
             sm.RegionMeanHueSort,
             sm.DepthSort,
             sm.VerifierSort,
+            sm.ConfidenceSort,
         ]
 
         self.setWindowTitle("Sort")
         self.setLayout(QVBoxLayout())
 
         self._add_method_button = QPushButton("Add")
         self._add_method_button.clicked.connect(self._add_method)
@@ -105,14 +106,20 @@
             ]
             return sm.SortMethodGroup(*methods)
 
     def accept(self) -> None:
         self.method = self._get_method()
         super().accept()
 
+    def clear(self):
+        """
+        Clear the current sort methods from the dialog.
+        """
+        self._clear_methods()
+
 
 if __name__ == "__main__":
     # Test code, just show the dialog
     import sys
 
     from PyQt6.QtWidgets import QApplication
```

### Comparing `vars_gridview-0.8.1/vars_gridview/ui/settings/SettingsDialog.py` & `vars_gridview-0.9.0/vars_gridview/ui/settings/SettingsDialog.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.8.1/vars_gridview/ui/settings/tabs/AbstractSettingsTab.py` & `vars_gridview-0.9.0/vars_gridview/ui/settings/tabs/AbstractSettingsTab.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.8.1/vars_gridview/ui/settings/tabs/AppearanceTab.py` & `vars_gridview-0.9.0/vars_gridview/ui/settings/tabs/AppearanceTab.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.8.1/vars_gridview/ui/settings/tabs/CacheTab.py` & `vars_gridview-0.9.0/vars_gridview/ui/settings/tabs/CacheTab.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.8.1/vars_gridview/ui/settings/tabs/M3Tab.py` & `vars_gridview-0.9.0/vars_gridview/ui/settings/tabs/M3Tab.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.8.1/vars_gridview/ui/settings/tabs/SQLTab.py` & `vars_gridview-0.9.0/vars_gridview/ui/settings/tabs/SQLTab.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.8.1/vars_gridview/ui/settings/tabs/VideoPlayerTab.py` & `vars_gridview-0.9.0/vars_gridview/ui/settings/tabs/VideoPlayerTab.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.8.1/PKG-INFO` & `vars_gridview-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vars-gridview
-Version: 0.8.1
+Version: 0.9.0
 Summary: VARS GridView is a tool for reviewing and correcting VARS localizations in bulk.
 Home-page: https://github.com/mbari-org/vars-gridview
 License: MIT
 Keywords: VARS,localization,annotation
 Author: Kevin Barnard
 Author-email: kbarnard@mbari.org
 Requires-Python: >=3.8,<3.13
```

