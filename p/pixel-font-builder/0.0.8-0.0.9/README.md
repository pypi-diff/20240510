# Comparing `tmp/pixel-font-builder-0.0.8.tar.gz` & `tmp/pixel-font-builder-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixel-font-builder-0.0.8.tar", last modified: Fri Jul 28 12:23:34 2023, max compression
+gzip compressed data, was "pixel-font-builder-0.0.9.tar", last modified: Tue Aug  8 13:09:47 2023, max compression
```

## Comparing `pixel-font-builder-0.0.8.tar` & `pixel-font-builder-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:23:34.417937 pixel-font-builder-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-28 12:23:24.000000 pixel-font-builder-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-28 12:23:34.417937 pixel-font-builder-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-07-28 12:23:24.000000 pixel-font-builder-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-28 12:23:24.000000 pixel-font-builder-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 12:23:34.417937 pixel-font-builder-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:23:34.413936 pixel-font-builder-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:23:34.413936 pixel-font-builder-0.0.8/src/pixel_font_builder/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-28 12:23:24.000000 pixel-font-builder-0.0.8/src/pixel_font_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-28 12:23:24.000000 pixel-font-builder-0.0.8/src/pixel_font_builder/bdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-07-28 12:23:24.000000 pixel-font-builder-0.0.8/src/pixel_font_builder/font.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-28 12:23:24.000000 pixel-font-builder-0.0.8/src/pixel_font_builder/glyph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-28 12:23:24.000000 pixel-font-builder-0.0.8/src/pixel_font_builder/info.py
--rw-r--r--   0 runner    (1001) docker     (123)    14280 2023-07-28 12:23:24.000000 pixel-font-builder-0.0.8/src/pixel_font_builder/opentype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:23:34.417937 pixel-font-builder-0.0.8/src/pixel_font_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-28 12:23:34.000000 pixel-font-builder-0.0.8/src/pixel_font_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-28 12:23:34.000000 pixel-font-builder-0.0.8/src/pixel_font_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 12:23:34.000000 pixel-font-builder-0.0.8/src/pixel_font_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-28 12:23:34.000000 pixel-font-builder-0.0.8/src/pixel_font_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-28 12:23:34.000000 pixel-font-builder-0.0.8/src/pixel_font_builder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:23:34.417937 pixel-font-builder-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-28 12:23:24.000000 pixel-font-builder-0.0.8/tests/test_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:09:47.851312 pixel-font-builder-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-08 13:09:35.000000 pixel-font-builder-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-08-08 13:09:47.851312 pixel-font-builder-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-08-08 13:09:35.000000 pixel-font-builder-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-08-08 13:09:35.000000 pixel-font-builder-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 13:09:47.851312 pixel-font-builder-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:09:47.851312 pixel-font-builder-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:09:47.851312 pixel-font-builder-0.0.9/src/pixel_font_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-08-08 13:09:35.000000 pixel-font-builder-0.0.9/src/pixel_font_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-08-08 13:09:35.000000 pixel-font-builder-0.0.9/src/pixel_font_builder/bdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-08-08 13:09:35.000000 pixel-font-builder-0.0.9/src/pixel_font_builder/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-08-08 13:09:35.000000 pixel-font-builder-0.0.9/src/pixel_font_builder/glyph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-08-08 13:09:35.000000 pixel-font-builder-0.0.9/src/pixel_font_builder/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-08-08 13:09:35.000000 pixel-font-builder-0.0.9/src/pixel_font_builder/opentype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:09:47.851312 pixel-font-builder-0.0.9/src/pixel_font_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-08-08 13:09:47.000000 pixel-font-builder-0.0.9/src/pixel_font_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-08 13:09:47.000000 pixel-font-builder-0.0.9/src/pixel_font_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 13:09:47.000000 pixel-font-builder-0.0.9/src/pixel_font_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-08 13:09:47.000000 pixel-font-builder-0.0.9/src/pixel_font_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-08 13:09:47.000000 pixel-font-builder-0.0.9/src/pixel_font_builder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:09:47.851312 pixel-font-builder-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-08 13:09:35.000000 pixel-font-builder-0.0.9/tests/test_.py
```

### Comparing `pixel-font-builder-0.0.8/LICENSE` & `pixel-font-builder-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pixel-font-builder-0.0.8/PKG-INFO` & `pixel-font-builder-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixel-font-builder
-Version: 0.0.8
+Version: 0.0.9
 Summary: A library that helps create pixel style fonts.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/pixel-font-builder
 Project-URL: source, https://github.com/TakWolf/pixel-font-builder
 Project-URL: issues, https://github.com/TakWolf/pixel-font-builder/issues
@@ -38,27 +38,42 @@
 from examples import outputs_dir
 from pixel_font_builder import FontBuilder, Glyph, StyleName, SerifMode, WidthMode, opentype
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 def main():
-    builder = FontBuilder(
-        size=12,
-        ascent=10,
-        descent=-2,
-        x_height=5,
-        cap_height=7,
-    )
+    builder = FontBuilder()
+
+    builder.metrics.size = 12
+    builder.metrics.ascent = 10
+    builder.metrics.descent = -2
+    builder.metrics.x_height = 5
+    builder.metrics.cap_height = 7
+
+    builder.meta_infos.version = '1.0.0'
+    builder.meta_infos.family_name = 'My Pixel'
+    builder.meta_infos.style_name = StyleName.REGULAR
+    builder.meta_infos.serif_mode = SerifMode.SANS_SERIF
+    builder.meta_infos.width_mode = WidthMode.MONOSPACED
+    builder.meta_infos.manufacturer = 'Pixel Font Studio'
+    builder.meta_infos.designer = 'TakWolf'
+    builder.meta_infos.description = 'A demo pixel font.'
+    builder.meta_infos.copyright_info = 'Copyright (c) TakWolf'
+    builder.meta_infos.license_info = 'This Font Software is licensed under the SIL Open Font License, Version 1.1.'
+    builder.meta_infos.vendor_url = 'https://github.com/TakWolf/pixel-font-builder'
+    builder.meta_infos.designer_url = 'https://takwolf.com'
+    builder.meta_infos.license_url = 'https://scripts.sil.org/OFL'
+    builder.meta_infos.sample_text = 'Hello World!'
 
     builder.character_mapping.update({
         ord('A'): 'CAP_LETTER_A',
     })
 
-    builder.add_glyph(Glyph(
+    builder.glyphs.append(Glyph(
         name='.notdef',
         advance_width=8,
         offset=(0, -2),
         data=[
             [1, 1, 1, 1, 1, 1, 1, 1],
             [1, 0, 0, 0, 0, 0, 0, 1],
             [1, 0, 0, 0, 0, 0, 0, 1],
@@ -69,15 +84,15 @@
             [1, 0, 0, 0, 0, 0, 0, 1],
             [1, 0, 0, 0, 0, 0, 0, 1],
             [1, 0, 0, 0, 0, 0, 0, 1],
             [1, 0, 0, 0, 0, 0, 0, 1],
             [1, 1, 1, 1, 1, 1, 1, 1],
         ],
     ))
-    builder.add_glyph(Glyph(
+    builder.glyphs.append(Glyph(
         name='CAP_LETTER_A',
         advance_width=8,
         offset=(0, -2),
         data=[
             [0, 0, 0, 1, 1, 0, 0, 0],
             [0, 0, 1, 0, 0, 1, 0, 0],
             [0, 0, 1, 0, 0, 1, 0, 0],
@@ -89,33 +104,18 @@
             [0, 1, 0, 0, 0, 0, 1, 0],
             [0, 1, 0, 0, 0, 0, 1, 0],
             [0, 0, 0, 0, 0, 0, 0, 0],
             [0, 0, 0, 0, 0, 0, 0, 0],
         ],
     ))
 
-    builder.meta_infos.version = '1.0.0'
-    builder.meta_infos.family_name = 'Demo Pixel'
-    builder.meta_infos.style_name = StyleName.REGULAR
-    builder.meta_infos.serif_mode = SerifMode.SANS_SERIF
-    builder.meta_infos.width_mode = WidthMode.MONOSPACED
-    builder.meta_infos.manufacturer = 'TakWolf Studio'
-    builder.meta_infos.designer = 'TakWolf'
-    builder.meta_infos.description = 'A demo pixel font.'
-    builder.meta_infos.copyright_info = 'Copyright (c) TakWolf'
-    builder.meta_infos.license_info = 'This Font Software is licensed under the SIL Open Font License, Version 1.1.'
-    builder.meta_infos.vendor_url = 'https://github.com/TakWolf/pixel-font-builder'
-    builder.meta_infos.designer_url = 'https://takwolf.com'
-    builder.meta_infos.license_url = 'https://scripts.sil.org/OFL'
-    builder.meta_infos.sample_text = 'Hello World!'
-
-    builder.save_otf(os.path.join(outputs_dir, 'demo.otf'))
-    builder.save_otf(os.path.join(outputs_dir, 'demo.woff2'), flavor=opentype.Flavor.WOFF2)
-    builder.save_ttf(os.path.join(outputs_dir, 'demo.ttf'))
-    builder.save_bdf(os.path.join(outputs_dir, 'demo.bdf'))
+    builder.save_otf(os.path.join(outputs_dir, 'my-pixel.otf'))
+    builder.save_otf(os.path.join(outputs_dir, 'my-pixel.woff2'), flavor=opentype.Flavor.WOFF2)
+    builder.save_ttf(os.path.join(outputs_dir, 'my-font.ttf'))
+    builder.save_bdf(os.path.join(outputs_dir, 'my-font.bdf'))
 
 
 if __name__ == '__main__':
     main()
 ```
 
 ## Dependencies
```

### Comparing `pixel-font-builder-0.0.8/README.md` & `pixel-font-builder-0.0.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -20,27 +20,42 @@
 from examples import outputs_dir
 from pixel_font_builder import FontBuilder, Glyph, StyleName, SerifMode, WidthMode, opentype
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 def main():
-    builder = FontBuilder(
-        size=12,
-        ascent=10,
-        descent=-2,
-        x_height=5,
-        cap_height=7,
-    )
+    builder = FontBuilder()
+
+    builder.metrics.size = 12
+    builder.metrics.ascent = 10
+    builder.metrics.descent = -2
+    builder.metrics.x_height = 5
+    builder.metrics.cap_height = 7
+
+    builder.meta_infos.version = '1.0.0'
+    builder.meta_infos.family_name = 'My Pixel'
+    builder.meta_infos.style_name = StyleName.REGULAR
+    builder.meta_infos.serif_mode = SerifMode.SANS_SERIF
+    builder.meta_infos.width_mode = WidthMode.MONOSPACED
+    builder.meta_infos.manufacturer = 'Pixel Font Studio'
+    builder.meta_infos.designer = 'TakWolf'
+    builder.meta_infos.description = 'A demo pixel font.'
+    builder.meta_infos.copyright_info = 'Copyright (c) TakWolf'
+    builder.meta_infos.license_info = 'This Font Software is licensed under the SIL Open Font License, Version 1.1.'
+    builder.meta_infos.vendor_url = 'https://github.com/TakWolf/pixel-font-builder'
+    builder.meta_infos.designer_url = 'https://takwolf.com'
+    builder.meta_infos.license_url = 'https://scripts.sil.org/OFL'
+    builder.meta_infos.sample_text = 'Hello World!'
 
     builder.character_mapping.update({
         ord('A'): 'CAP_LETTER_A',
     })
 
-    builder.add_glyph(Glyph(
+    builder.glyphs.append(Glyph(
         name='.notdef',
         advance_width=8,
         offset=(0, -2),
         data=[
             [1, 1, 1, 1, 1, 1, 1, 1],
             [1, 0, 0, 0, 0, 0, 0, 1],
             [1, 0, 0, 0, 0, 0, 0, 1],
@@ -51,15 +66,15 @@
             [1, 0, 0, 0, 0, 0, 0, 1],
             [1, 0, 0, 0, 0, 0, 0, 1],
             [1, 0, 0, 0, 0, 0, 0, 1],
             [1, 0, 0, 0, 0, 0, 0, 1],
             [1, 1, 1, 1, 1, 1, 1, 1],
         ],
     ))
-    builder.add_glyph(Glyph(
+    builder.glyphs.append(Glyph(
         name='CAP_LETTER_A',
         advance_width=8,
         offset=(0, -2),
         data=[
             [0, 0, 0, 1, 1, 0, 0, 0],
             [0, 0, 1, 0, 0, 1, 0, 0],
             [0, 0, 1, 0, 0, 1, 0, 0],
@@ -71,33 +86,18 @@
             [0, 1, 0, 0, 0, 0, 1, 0],
             [0, 1, 0, 0, 0, 0, 1, 0],
             [0, 0, 0, 0, 0, 0, 0, 0],
             [0, 0, 0, 0, 0, 0, 0, 0],
         ],
     ))
 
-    builder.meta_infos.version = '1.0.0'
-    builder.meta_infos.family_name = 'Demo Pixel'
-    builder.meta_infos.style_name = StyleName.REGULAR
-    builder.meta_infos.serif_mode = SerifMode.SANS_SERIF
-    builder.meta_infos.width_mode = WidthMode.MONOSPACED
-    builder.meta_infos.manufacturer = 'TakWolf Studio'
-    builder.meta_infos.designer = 'TakWolf'
-    builder.meta_infos.description = 'A demo pixel font.'
-    builder.meta_infos.copyright_info = 'Copyright (c) TakWolf'
-    builder.meta_infos.license_info = 'This Font Software is licensed under the SIL Open Font License, Version 1.1.'
-    builder.meta_infos.vendor_url = 'https://github.com/TakWolf/pixel-font-builder'
-    builder.meta_infos.designer_url = 'https://takwolf.com'
-    builder.meta_infos.license_url = 'https://scripts.sil.org/OFL'
-    builder.meta_infos.sample_text = 'Hello World!'
-
-    builder.save_otf(os.path.join(outputs_dir, 'demo.otf'))
-    builder.save_otf(os.path.join(outputs_dir, 'demo.woff2'), flavor=opentype.Flavor.WOFF2)
-    builder.save_ttf(os.path.join(outputs_dir, 'demo.ttf'))
-    builder.save_bdf(os.path.join(outputs_dir, 'demo.bdf'))
+    builder.save_otf(os.path.join(outputs_dir, 'my-pixel.otf'))
+    builder.save_otf(os.path.join(outputs_dir, 'my-pixel.woff2'), flavor=opentype.Flavor.WOFF2)
+    builder.save_ttf(os.path.join(outputs_dir, 'my-font.ttf'))
+    builder.save_bdf(os.path.join(outputs_dir, 'my-font.bdf'))
 
 
 if __name__ == '__main__':
     main()
 ```
 
 ## Dependencies
```

### Comparing `pixel-font-builder-0.0.8/pyproject.toml` & `pixel-font-builder-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pixel-font-builder"
-version = "0.0.8"
+version = "0.0.9"
 description = "A library that helps create pixel style fonts."
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.11"
 authors = [
     { name = "TakWolf" },
 ]
@@ -15,15 +15,15 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
-    "fonttools>=4.41.1",
+    "fonttools>=4.42.0",
     "Brotli>=1.0.9",
     "bdffont>=0.0.13",
 ]
 
 [project.urls]
 homepage = "https://github.com/TakWolf/pixel-font-builder"
 source = "https://github.com/TakWolf/pixel-font-builder"
```

### Comparing `pixel-font-builder-0.0.8/src/pixel_font_builder/glyph.py` & `pixel-font-builder-0.0.9/src/pixel_font_builder/glyph.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
             offset: tuple[int, int] = (0, 0),
             data: list[list[int]] = None,
     ):
         self.name = name
         self.advance_width = advance_width
         self.offset_x, self.offset_y = offset
         if data is None:
-            data = list[list[int]]()
+            data = []
         self.data = data
 
     @property
     def offset(self) -> tuple[int, int]:
         return self.offset_x, self.offset_y
 
     @offset.setter
```

### Comparing `pixel-font-builder-0.0.8/src/pixel_font_builder/opentype.py` & `pixel-font-builder-0.0.9/src/pixel_font_builder/opentype.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,34 +4,35 @@
 from fontTools.fontBuilder import FontBuilder
 from fontTools.misc.psCharStrings import T2CharString as OTFGlyph
 from fontTools.pens.t2CharStringPen import T2CharStringPen as OTFGlyphPen
 from fontTools.pens.ttGlyphPen import TTGlyphPen as TTFGlyphPen
 from fontTools.ttLib import TTCollection
 from fontTools.ttLib.tables._g_l_y_f import Glyph as TTFGlyph
 
-from pixel_font_builder import font
 from pixel_font_builder.glyph import Glyph
-from pixel_font_builder.info import MetaInfos
+from pixel_font_builder.info import Metrics, MetaInfos
 
 logger = logging.getLogger('pixel_font_builder.opentype')
 
 _CACHE_NAME_TAG = '_opentype_cache_tag'
 _CACHE_NAME_OUTLINES = '_opentype_cache_outlines'
 _CACHE_NAME_OTF_GLYPH = '_opentype_cache_otf_glyph'
 _CACHE_NAME_TTF_GLYPH = '_opentype_cache_ttf_glyph'
 
 
 class Configs:
     def __init__(
             self,
             px_to_units: int = 100,
             cff_family_name: str = None,
+            allow_fallback_cmap: bool = False,
     ):
         self.px_to_units = px_to_units
         self.cff_family_name = cff_family_name
+        self.allow_fallback_cmap = allow_fallback_cmap
 
 
 class Flavor(StrEnum):
     WOFF = 'woff'
     WOFF2 = 'woff2'
 
 
@@ -90,14 +91,30 @@
     if meta_infos.license_url is not None:
         name_strings['licenseInfoURL'] = meta_infos.license_url
     if meta_infos.sample_text is not None:
         name_strings['sampleText'] = meta_infos.sample_text
     return name_strings
 
 
+def _create_cff_font_infos(configs: Configs, meta_infos: MetaInfos) -> tuple[str, dict[str, str]]:
+    if configs.cff_family_name is not None:
+        cff_family_name = configs.cff_family_name
+    else:
+        cff_family_name = meta_infos.family_name
+    cff_ps_name = f'{cff_family_name.replace(" ", "-")}-{meta_infos.style_name}'
+    cff_font_infos = {
+        'FamilyName': cff_family_name,
+        'FullName': f'{cff_family_name} {meta_infos.style_name}',
+        'Weight': meta_infos.style_name,
+    }
+    if meta_infos.copyright_info is not None:
+        cff_font_infos['Notice'] = meta_infos.copyright_info
+    return cff_ps_name, cff_font_infos
+
+
 def _create_outlines(glyph_data: list[list[int]], px_to_units: int) -> list[list[tuple[int, int]]]:
     """
     将字形数据转换为轮廓数据，左上角原点坐标系
     """
     # 相邻像素分组
     point_group_list = []
     for y, glyph_data_row in enumerate(glyph_data):
@@ -178,27 +195,27 @@
             if (x == xl and x == xr) or (y == yl and y == yr):
                 solved_line_segment.pop()
             # 添加到轮廓
             outlines.append(solved_line_segment)
     return outlines
 
 
-def _create_glyph(outlines: list[list[tuple[int, int]]], glyph_context: Glyph, px_to_units: int, is_ttf: bool) -> OTFGlyph | TTFGlyph:
+def _create_glyph(glyph: Glyph, outlines: list[list[tuple[int, int]]], px_to_units: int, is_ttf: bool) -> OTFGlyph | TTFGlyph:
     if is_ttf:
         pen = TTFGlyphPen()
     else:
-        pen = OTFGlyphPen(glyph_context.advance_width * px_to_units, None)
+        pen = OTFGlyphPen(glyph.advance_width * px_to_units, None)
     if len(outlines) > 0:
         for outline_index, outline in enumerate(outlines):
             for point_index, point in enumerate(outline):
 
                 # 转换左上角原点坐标系为左下角原点坐标系
                 x, y = point
-                x += glyph_context.offset_x * px_to_units
-                y = (glyph_context.height + glyph_context.offset_y) * px_to_units - y
+                x += glyph.offset_x * px_to_units
+                y = (glyph.height + glyph.offset_y) * px_to_units - y
                 point = x, y
 
                 if point_index == 0:
                     pen.moveTo(point)
                 else:
                     pen.lineTo(point)
             if outline_index < len(outlines) - 1:
@@ -210,100 +227,98 @@
         pen.closePath()
     if is_ttf:
         return pen.glyph()
     else:
         return pen.getCharString()
 
 
-def _get_glyph_with_cache(glyph_context: Glyph, px_to_units: int, is_ttf: bool) -> OTFGlyph | TTFGlyph:
-    cache_tag = f'{glyph_context.advance_width}#{glyph_context.offset}#{glyph_context.data}'.replace(' ', '')
-    if getattr(glyph_context, _CACHE_NAME_TAG, None) != cache_tag:
-        setattr(glyph_context, _CACHE_NAME_OUTLINES, None)
-        setattr(glyph_context, _CACHE_NAME_OTF_GLYPH, None)
-        setattr(glyph_context, _CACHE_NAME_TTF_GLYPH, None)
-        setattr(glyph_context, _CACHE_NAME_TAG, cache_tag)
+def _get_glyph_with_cache(glyph: Glyph, px_to_units: int, is_ttf: bool) -> OTFGlyph | TTFGlyph:
+    cache_tag = f'{glyph.advance_width}#{glyph.offset}#{glyph.data}'.replace(' ', '')
+    if getattr(glyph, _CACHE_NAME_TAG, None) != cache_tag:
+        setattr(glyph, _CACHE_NAME_OUTLINES, None)
+        setattr(glyph, _CACHE_NAME_OTF_GLYPH, None)
+        setattr(glyph, _CACHE_NAME_TTF_GLYPH, None)
+        setattr(glyph, _CACHE_NAME_TAG, cache_tag)
 
-    outlines = getattr(glyph_context, _CACHE_NAME_OUTLINES, None)
+    outlines = getattr(glyph, _CACHE_NAME_OUTLINES, None)
     if outlines is None:
-        logger.debug("Create 'Outlines': %s", glyph_context.name)
-        outlines = _create_outlines(glyph_context.data, px_to_units)
-        setattr(glyph_context, _CACHE_NAME_OUTLINES, outlines)
+        logger.debug("Create 'Outlines': %s", glyph.name)
+        outlines = _create_outlines(glyph.data, px_to_units)
+        setattr(glyph, _CACHE_NAME_OUTLINES, outlines)
     else:
-        logger.debug("Use cached 'Outlines': %s", glyph_context.name)
+        logger.debug("Use cached 'Outlines': %s", glyph.name)
 
     cache_name_xtf_glyph = _CACHE_NAME_TTF_GLYPH if is_ttf else _CACHE_NAME_OTF_GLYPH
-    glyph = getattr(glyph_context, cache_name_xtf_glyph, None)
-    if glyph is None:
-        logger.debug("Create '%sGlyph': %s", 'TTF' if is_ttf else 'OTF', glyph_context.name)
-        glyph = _create_glyph(outlines, glyph_context, px_to_units, is_ttf)
-        setattr(glyph_context, cache_name_xtf_glyph, glyph)
+    xtf_glyph = getattr(glyph, cache_name_xtf_glyph, None)
+    if xtf_glyph is None:
+        logger.debug("Create '%sGlyph': %s", 'TTF' if is_ttf else 'OTF', glyph.name)
+        xtf_glyph = _create_glyph(glyph, outlines, px_to_units, is_ttf)
+        setattr(glyph, cache_name_xtf_glyph, xtf_glyph)
     else:
-        logger.debug("Use cached '%sGlyph': %s", 'TTF' if is_ttf else 'OTF', glyph_context.name)
-    return glyph
+        logger.debug("Use cached '%sGlyph': %s", 'TTF' if is_ttf else 'OTF', glyph.name)
+    return xtf_glyph
 
 
-def create_builder(context: 'font.FontBuilder', is_ttf: bool, flavor: Flavor = None) -> FontBuilder:
-    logger.debug("Create '%sBuilder': %s", 'TTF' if is_ttf else 'OTF', context.meta_infos.family_name)
-    context.check_ready()
-
-    units_per_em = context.size * context.opentype_configs.px_to_units
-    builder = FontBuilder(units_per_em, isTTF=is_ttf)
+def create_builder(
+        configs: Configs,
+        metrics: Metrics,
+        meta_infos: MetaInfos,
+        character_mapping: dict[int, str],
+        glyph_order: list[str],
+        name_to_glyph: dict[str, Glyph],
+        is_ttf: bool,
+        flavor: Flavor = None,
+) -> FontBuilder:
+    logger.debug("Create '%sBuilder': %s", 'TTF' if is_ttf else 'OTF', meta_infos.family_name)
+    builder = FontBuilder(metrics.size * configs.px_to_units, isTTF=is_ttf)
 
     logger.debug("Setup 'Name Strings'")
-    name_strings = _create_name_strings(context.meta_infos)
+    name_strings = _create_name_strings(meta_infos)
     builder.setupNameTable(name_strings)
 
-    logger.debug("Setup 'Glyph Order' and 'Glyphs'")
-    glyph_order = ['.notdef']
-    glyphs = {}
-    for glyph_context in context.get_glyphs():
-        if glyph_context.name != '.notdef':
-            glyph_order.append(glyph_context.name)
-        glyphs[glyph_context.name] = _get_glyph_with_cache(glyph_context, context.opentype_configs.px_to_units, is_ttf)
+    logger.debug("Setup 'Glyph Order'")
     builder.setupGlyphOrder(glyph_order)
+
+    logger.debug("Create 'Glyphs'")
+    xtf_glyphs = {}
+    for glyph_name, glyph in name_to_glyph.items():
+        xtf_glyphs[glyph_name] = _get_glyph_with_cache(glyph, configs.px_to_units, is_ttf)
     if is_ttf:
-        builder.setupGlyf(glyphs)
+        logger.debug("Setup 'Glyf'")
+        builder.setupGlyf(xtf_glyphs)
     else:
-        if context.opentype_configs.cff_family_name is not None:
-            cff_family_name = context.opentype_configs.cff_family_name
-        else:
-            cff_family_name = context.meta_infos.family_name
-        cff_ps_name = f'{cff_family_name.replace(" ", "-")}-{context.meta_infos.style_name}'
-        cff_font_infos = {
-            'FamilyName': cff_family_name,
-            'FullName': f'{cff_family_name} {context.meta_infos.style_name}',
-            'Weight': context.meta_infos.style_name,
-        }
-        if context.meta_infos.copyright_info is not None:
-            cff_font_infos['Notice'] = context.meta_infos.copyright_info
-        builder.setupCFF(cff_ps_name, cff_font_infos, glyphs, {})
+        logger.debug("Setup 'CFF'")
+        cff_ps_name, cff_font_infos = _create_cff_font_infos(configs, meta_infos)
+        builder.setupCFF(cff_ps_name, cff_font_infos, xtf_glyphs, {})
 
     logger.debug("Setup 'Character Mapping'")
-    builder.setupCharacterMap(context.character_mapping, allowFallback=True)
+    builder.setupCharacterMap(character_mapping, allowFallback=configs.allow_fallback_cmap)
 
     logger.debug("Setup 'Horizontal Metrics'")
     horizontal_metrics = {}
     for glyph_name in glyph_order:
-        advance_width = context.get_glyph(glyph_name).advance_width * context.opentype_configs.px_to_units
+        advance_width = name_to_glyph[glyph_name].advance_width * configs.px_to_units
         if is_ttf:
-            lsb = glyphs[glyph_name].xMin
+            lsb = xtf_glyphs[glyph_name].xMin
         else:
-            lsb = glyphs[glyph_name].calcBounds(None)[0]
+            lsb = xtf_glyphs[glyph_name].calcBounds(None)[0]
         horizontal_metrics[glyph_name] = advance_width, lsb
     builder.setupHorizontalMetrics(horizontal_metrics)
 
-    ascent = context.ascent * context.opentype_configs.px_to_units
-    descent = context.descent * context.opentype_configs.px_to_units
-    x_height = context.x_height * context.opentype_configs.px_to_units if context.x_height is not None else None
-    cap_height = context.cap_height * context.opentype_configs.px_to_units if context.cap_height is not None else None
+    ascent = metrics.ascent * configs.px_to_units
+    descent = metrics.descent * configs.px_to_units
+    x_height = metrics.x_height * configs.px_to_units if metrics.x_height is not None else None
+    cap_height = metrics.cap_height * configs.px_to_units if metrics.cap_height is not None else None
+
     logger.debug("Setup 'Horizontal Header'")
     builder.setupHorizontalHeader(
         ascent=ascent,
         descent=descent,
     )
+
     logger.debug("Setup 'OS2'")
     builder.setupOS2(
         sTypoAscender=ascent,
         sTypoDescender=descent,
         usWinAscent=ascent,
         usWinDescent=-descent,
         sxHeight=x_height,
@@ -317,12 +332,12 @@
         logger.debug("Setup 'Flavor': %s", flavor)
         builder.font.flavor = flavor
 
     logger.debug("Create '%sBuilder' finished", 'TTF' if is_ttf else 'OTF')
     return builder
 
 
-def create_collection_builder(context: 'font.FontCollectionBuilder', is_ttf: bool) -> TTCollection:
+def create_collection_builder(builders: list[FontBuilder]) -> TTCollection:
     collection_builder = TTCollection()
-    for font_context in context.font_builders:
-        collection_builder.fonts.append(create_builder(font_context, is_ttf).font)
+    for builder in builders:
+        collection_builder.fonts.append(builder.font)
     return collection_builder
```

### Comparing `pixel-font-builder-0.0.8/src/pixel_font_builder.egg-info/PKG-INFO` & `pixel-font-builder-0.0.9/src/pixel_font_builder.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixel-font-builder
-Version: 0.0.8
+Version: 0.0.9
 Summary: A library that helps create pixel style fonts.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/pixel-font-builder
 Project-URL: source, https://github.com/TakWolf/pixel-font-builder
 Project-URL: issues, https://github.com/TakWolf/pixel-font-builder/issues
@@ -38,27 +38,42 @@
 from examples import outputs_dir
 from pixel_font_builder import FontBuilder, Glyph, StyleName, SerifMode, WidthMode, opentype
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 def main():
-    builder = FontBuilder(
-        size=12,
-        ascent=10,
-        descent=-2,
-        x_height=5,
-        cap_height=7,
-    )
+    builder = FontBuilder()
+
+    builder.metrics.size = 12
+    builder.metrics.ascent = 10
+    builder.metrics.descent = -2
+    builder.metrics.x_height = 5
+    builder.metrics.cap_height = 7
+
+    builder.meta_infos.version = '1.0.0'
+    builder.meta_infos.family_name = 'My Pixel'
+    builder.meta_infos.style_name = StyleName.REGULAR
+    builder.meta_infos.serif_mode = SerifMode.SANS_SERIF
+    builder.meta_infos.width_mode = WidthMode.MONOSPACED
+    builder.meta_infos.manufacturer = 'Pixel Font Studio'
+    builder.meta_infos.designer = 'TakWolf'
+    builder.meta_infos.description = 'A demo pixel font.'
+    builder.meta_infos.copyright_info = 'Copyright (c) TakWolf'
+    builder.meta_infos.license_info = 'This Font Software is licensed under the SIL Open Font License, Version 1.1.'
+    builder.meta_infos.vendor_url = 'https://github.com/TakWolf/pixel-font-builder'
+    builder.meta_infos.designer_url = 'https://takwolf.com'
+    builder.meta_infos.license_url = 'https://scripts.sil.org/OFL'
+    builder.meta_infos.sample_text = 'Hello World!'
 
     builder.character_mapping.update({
         ord('A'): 'CAP_LETTER_A',
     })
 
-    builder.add_glyph(Glyph(
+    builder.glyphs.append(Glyph(
         name='.notdef',
         advance_width=8,
         offset=(0, -2),
         data=[
             [1, 1, 1, 1, 1, 1, 1, 1],
             [1, 0, 0, 0, 0, 0, 0, 1],
             [1, 0, 0, 0, 0, 0, 0, 1],
@@ -69,15 +84,15 @@
             [1, 0, 0, 0, 0, 0, 0, 1],
             [1, 0, 0, 0, 0, 0, 0, 1],
             [1, 0, 0, 0, 0, 0, 0, 1],
             [1, 0, 0, 0, 0, 0, 0, 1],
             [1, 1, 1, 1, 1, 1, 1, 1],
         ],
     ))
-    builder.add_glyph(Glyph(
+    builder.glyphs.append(Glyph(
         name='CAP_LETTER_A',
         advance_width=8,
         offset=(0, -2),
         data=[
             [0, 0, 0, 1, 1, 0, 0, 0],
             [0, 0, 1, 0, 0, 1, 0, 0],
             [0, 0, 1, 0, 0, 1, 0, 0],
@@ -89,33 +104,18 @@
             [0, 1, 0, 0, 0, 0, 1, 0],
             [0, 1, 0, 0, 0, 0, 1, 0],
             [0, 0, 0, 0, 0, 0, 0, 0],
             [0, 0, 0, 0, 0, 0, 0, 0],
         ],
     ))
 
-    builder.meta_infos.version = '1.0.0'
-    builder.meta_infos.family_name = 'Demo Pixel'
-    builder.meta_infos.style_name = StyleName.REGULAR
-    builder.meta_infos.serif_mode = SerifMode.SANS_SERIF
-    builder.meta_infos.width_mode = WidthMode.MONOSPACED
-    builder.meta_infos.manufacturer = 'TakWolf Studio'
-    builder.meta_infos.designer = 'TakWolf'
-    builder.meta_infos.description = 'A demo pixel font.'
-    builder.meta_infos.copyright_info = 'Copyright (c) TakWolf'
-    builder.meta_infos.license_info = 'This Font Software is licensed under the SIL Open Font License, Version 1.1.'
-    builder.meta_infos.vendor_url = 'https://github.com/TakWolf/pixel-font-builder'
-    builder.meta_infos.designer_url = 'https://takwolf.com'
-    builder.meta_infos.license_url = 'https://scripts.sil.org/OFL'
-    builder.meta_infos.sample_text = 'Hello World!'
-
-    builder.save_otf(os.path.join(outputs_dir, 'demo.otf'))
-    builder.save_otf(os.path.join(outputs_dir, 'demo.woff2'), flavor=opentype.Flavor.WOFF2)
-    builder.save_ttf(os.path.join(outputs_dir, 'demo.ttf'))
-    builder.save_bdf(os.path.join(outputs_dir, 'demo.bdf'))
+    builder.save_otf(os.path.join(outputs_dir, 'my-pixel.otf'))
+    builder.save_otf(os.path.join(outputs_dir, 'my-pixel.woff2'), flavor=opentype.Flavor.WOFF2)
+    builder.save_ttf(os.path.join(outputs_dir, 'my-font.ttf'))
+    builder.save_bdf(os.path.join(outputs_dir, 'my-font.bdf'))
 
 
 if __name__ == '__main__':
     main()
 ```
 
 ## Dependencies
```

