# Comparing `tmp/aepi-0.8.3.1.tar.gz` & `tmp/aepi-0.8.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aepi-0.8.3.1.tar", last modified: Wed May  8 21:58:25 2024, max compression
+gzip compressed data, was "aepi-0.8.3.2.tar", last modified: Fri May 10 15:16:19 2024, max compression
```

## Comparing `aepi-0.8.3.1.tar` & `aepi-0.8.3.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:58:25.143995 aepi-0.8.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-08 21:58:15.000000 aepi-0.8.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9864 2024-05-08 21:58:25.143995 aepi-0.8.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8742 2024-05-08 21:58:15.000000 aepi-0.8.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-08 21:58:15.000000 aepi-0.8.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-08 21:58:25.143995 aepi-0.8.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:58:25.139995 aepi-0.8.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:58:25.143995 aepi-0.8.3.1/src/AEPi/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-08 21:58:15.000000 aepi-0.8.3.1/src/AEPi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-05-08 21:58:15.000000 aepi-0.8.3.1/src/AEPi/codec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:58:25.143995 aepi-0.8.3.1/src/AEPi/codecs/
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-08 21:58:15.000000 aepi-0.8.3.1/src/AEPi/codecs/EtcPakCodec.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-08 21:58:15.000000 aepi-0.8.3.1/src/AEPi/codecs/RawCodec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-08 21:58:15.000000 aepi-0.8.3.1/src/AEPi/codecs/Tex2ImgCodec.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-08 21:58:15.000000 aepi-0.8.3.1/src/AEPi/codecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-05-08 21:58:15.000000 aepi-0.8.3.1/src/AEPi/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-05-08 21:58:15.000000 aepi-0.8.3.1/src/AEPi/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:58:25.143995 aepi-0.8.3.1/src/AEPi/image/
--rw-r--r--   0 runner    (1001) docker     (127)    18996 2024-05-08 21:58:15.000000 aepi-0.8.3.1/src/AEPi/image/AEI.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-08 21:58:15.000000 aepi-0.8.3.1/src/AEPi/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-08 21:58:15.000000 aepi-0.8.3.1/src/AEPi/image/texture.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:58:25.143995 aepi-0.8.3.1/src/AEPi/lib/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-08 21:58:15.000000 aepi-0.8.3.1/src/AEPi/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-08 21:58:15.000000 aepi-0.8.3.1/src/AEPi/lib/binaryio.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-08 21:58:15.000000 aepi-0.8.3.1/src/AEPi/lib/imageOps.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-08 21:58:15.000000 aepi-0.8.3.1/src/AEPi/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:58:25.143995 aepi-0.8.3.1/src/AEPi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9864 2024-05-08 21:58:25.000000 aepi-0.8.3.1/src/AEPi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-08 21:58:25.000000 aepi-0.8.3.1/src/AEPi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 21:58:25.000000 aepi-0.8.3.1/src/AEPi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-08 21:58:25.000000 aepi-0.8.3.1/src/AEPi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-08 21:58:25.000000 aepi-0.8.3.1/src/AEPi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:16:19.754202 aepi-0.8.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-10 15:16:07.000000 aepi-0.8.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9864 2024-05-10 15:16:19.754202 aepi-0.8.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8742 2024-05-10 15:16:07.000000 aepi-0.8.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-10 15:16:07.000000 aepi-0.8.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-10 15:16:19.754202 aepi-0.8.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:16:19.750202 aepi-0.8.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:16:19.754202 aepi-0.8.3.2/src/AEPi/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-10 15:16:07.000000 aepi-0.8.3.2/src/AEPi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-05-10 15:16:07.000000 aepi-0.8.3.2/src/AEPi/codec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:16:19.754202 aepi-0.8.3.2/src/AEPi/codecs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-10 15:16:07.000000 aepi-0.8.3.2/src/AEPi/codecs/EtcPakCodec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-10 15:16:07.000000 aepi-0.8.3.2/src/AEPi/codecs/RawCodec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-10 15:16:07.000000 aepi-0.8.3.2/src/AEPi/codecs/Tex2ImgCodec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-10 15:16:07.000000 aepi-0.8.3.2/src/AEPi/codecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-05-10 15:16:07.000000 aepi-0.8.3.2/src/AEPi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-05-10 15:16:07.000000 aepi-0.8.3.2/src/AEPi/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:16:19.754202 aepi-0.8.3.2/src/AEPi/image/
+-rw-r--r--   0 runner    (1001) docker     (127)    18996 2024-05-10 15:16:07.000000 aepi-0.8.3.2/src/AEPi/image/AEI.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-10 15:16:07.000000 aepi-0.8.3.2/src/AEPi/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-10 15:16:07.000000 aepi-0.8.3.2/src/AEPi/image/texture.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:16:19.754202 aepi-0.8.3.2/src/AEPi/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-10 15:16:07.000000 aepi-0.8.3.2/src/AEPi/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-10 15:16:07.000000 aepi-0.8.3.2/src/AEPi/lib/binaryio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-10 15:16:07.000000 aepi-0.8.3.2/src/AEPi/lib/imageOps.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-10 15:16:07.000000 aepi-0.8.3.2/src/AEPi/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:16:19.754202 aepi-0.8.3.2/src/AEPi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9864 2024-05-10 15:16:19.000000 aepi-0.8.3.2/src/AEPi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-10 15:16:19.000000 aepi-0.8.3.2/src/AEPi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 15:16:19.000000 aepi-0.8.3.2/src/AEPi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-10 15:16:19.000000 aepi-0.8.3.2/src/AEPi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-10 15:16:19.000000 aepi-0.8.3.2/src/AEPi.egg-info/top_level.txt
```

### Comparing `aepi-0.8.3.1/LICENSE` & `aepi-0.8.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aepi-0.8.3.1/PKG-INFO` & `aepi-0.8.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AEPi
-Version: 0.8.3.1
+Version: 0.8.3.2
 Summary: Read and write Abyss Engine Image (AEI) files from python, for Galaxy on Fire 2
 Home-page: https://github.com/Trimatix/AEPi
 Author: Jasper Law
 Author-email: trimatix.music@gmail.com
 Project-URL: Bug Tracker, https://github.com/Trimatix/AEPi/issues
 Keywords: game,python,galaxy-on-fire,image-compression,image-conversion,game-mod-tool,abyss-engine
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: AEPi Version: 0.8.3.1 Summary: Read and write Abyss
+Metadata-Version: 2.1 Name: AEPi Version: 0.8.3.2 Summary: Read and write Abyss
 Engine Image (AEI) files from python, for Galaxy on Fire 2 Home-page: https://
 github.com/Trimatix/AEPi Author: Jasper Law Author-email:
 trimatix.music@gmail.com Project-URL: Bug Tracker, https://github.com/Trimatix/
 AEPi/issues Keywords: game,python,galaxy-on-fire,image-compression,image-
 conversion,game-mod-tool,abyss-engine Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `aepi-0.8.3.1/README.md` & `aepi-0.8.3.2/README.md`

 * *Files identical despite different names*

### Comparing `aepi-0.8.3.1/pyproject.toml` & `aepi-0.8.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aepi-0.8.3.1/setup.cfg` & `aepi-0.8.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `aepi-0.8.3.1/src/AEPi/codec.py` & `aepi-0.8.3.2/src/AEPi/codec.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from .constants import CompressionFormat, CompressionQuality
 from .exceptions import UnsupportedCompressionFormatException
 
 class ImageCodecAdaptor(ABC):
     @classmethod
     def compress(cls, im: Image, format: CompressionFormat, quality: Optional[CompressionQuality]) -> bytes:
-        """Compress a BGRA image into format `format`, with quality `quality`
+        """Compress an RGB(A) image into format `format`, with quality `quality`
 
         :param im: The image to compress
         :type im: Image
         :param format: The compression format
         :type format: CompressionFormat
         :param quality: The compression quality
         :type quality: CompressionQuality
@@ -20,25 +20,25 @@
         :rtype: bytes
         """
         raise NotImplementedError(f"Codec {cls.__name__} is not capable of compression")
 
 
     @classmethod
     def decompress(cls, fp: bytes, format: CompressionFormat, width: int, height: int, quality: Optional[CompressionQuality]) -> Image:
-        """Decompress a `format`-compressed BGRA image into a BGRA Image.
+        """Decompress a `format`-compressed RGB(A) image into a RGB(A) Image.
 
         :param fp: The compressed image to decompress
         :type im: bytes
         :param format: The compression format
         :type format: CompressionFormat
         :param width: The width of the image
         :type width: int
         :param height: The height of the image
         :type height: int
-        :return: `fp`, decompressed into a BGRA image
+        :return: `fp`, decompressed into a RGB(A) image
         :rtype: Image
         """
         raise NotImplementedError(f"Codec {cls.__name__} is not capable of decompression")
 
 
 compressors: Dict[CompressionFormat, Type[ImageCodecAdaptor]] = {}
 decompressors: Dict[CompressionFormat, Type[ImageCodecAdaptor]] = {}
@@ -47,15 +47,15 @@
 
 def supportsFormats(
         compresses: Optional[Iterable[CompressionFormat]] = None,
         decompresses: Optional[Iterable[CompressionFormat]] = None,
         both: Optional[Iterable[CompressionFormat]] = None
     ):
     """Class decorator marking an image codec as able to compress/decompress images into the given compression formats.
-    The codec class must assume that BGRA is passed, and return BGRA.
+    The codec class must assume that RGB(A) is passed, and return RGB(A).
 
     ```py
     supportsFormats(
         compresses=[format1],
         decompresses=[format1]
     )
     ```
```

### Comparing `aepi-0.8.3.1/src/AEPi/codecs/EtcPakCodec.py` & `aepi-0.8.3.2/src/AEPi/codecs/EtcPakCodec.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 from typing import Optional
-from typing import Optional
+
 from PIL.Image import Image
 from contextlib import nullcontext
+
 from ..codec import ImageCodecAdaptor, supportsFormats
 from ..constants import CompressionFormat, CompressionQuality
 from ..exceptions import DependancyMissingException
 
 try:
     import etcpak
 except ImportError as e:
     raise DependancyMissingException("EtcPakCodec", "etcpak", e)
 
 
 @supportsFormats(compresses=[
     CompressionFormat.DXT5,
-    CompressionFormat.ETC1
+    CompressionFormat.ETC1,
+    CompressionFormat.ETC2
 ])
 class EtcPakCodec(ImageCodecAdaptor):
     @classmethod
     def compress(cls, im: Image, format: CompressionFormat, quality: Optional[CompressionQuality]) -> bytes:
         imageIn, ctx = cls._ensureRgba(im)
         with ctx:
             if format is CompressionFormat.DXT5:
                 return etcpak.compress_to_dxt5(imageIn.tobytes(), imageIn.width, imageIn.height) # type: ignore[reportUnknownVariableType]
 
             elif format is CompressionFormat.ETC1:
                 return etcpak.compress_to_etc1(imageIn.tobytes(), imageIn.width, imageIn.height) # type: ignore[reportUnknownVariableType]
             
+            elif format is CompressionFormat.ETC2:
+                # etcpak does provide a function for etc2 compression, but it produces almost completely black images
+                # ETC2 is backwards compatible with ETC1, so as a stopgap we'll just compress as etc1
+                # https://www.khronos.org/assets/uplo...pengl-es-bof/Ericsson-ETC2-SIGGRAPH_Aug12.pdf
+                return etcpak.compress_to_etc1(imageIn.tobytes(), imageIn.width, imageIn.height) # type: ignore[reportUnknownVariableType]
+            
         raise ValueError(f"Codec {EtcPakCodec.__name__} does not support format {format.name}")
     
     
     @classmethod
     def _ensureRgba(cls, im: Image):
         converted = im.mode != "RGBA"
         if converted:
```

### Comparing `aepi-0.8.3.1/src/AEPi/codecs/RawCodec.py` & `aepi-0.8.3.2/src/AEPi/codecs/RawCodec.py`

 * *Files identical despite different names*

### Comparing `aepi-0.8.3.1/src/AEPi/constants.py` & `aepi-0.8.3.2/src/AEPi/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,14 +98,15 @@
 FORMAT_BITCOUNTS[CompressionFormat.DXT1] = 4
 FORMAT_BITCOUNTS[CompressionFormat.DXT3] = 8
 FORMAT_BITCOUNTS[CompressionFormat.DXT5] = 8
 FORMAT_BITCOUNTS[CompressionFormat.ETC1] = 4
 FORMAT_BITCOUNTS[CompressionFormat.ETC2] = 8 # ?
 
 BGR_FORMATS.add(CompressionFormat.ETC1)
+BGR_FORMATS.add(CompressionFormat.ETC2)
 
 MIPMAPPABLE_FORMATS.add(CompressionFormat.PVRTC12A)
 MIPMAPPABLE_FORMATS.add(CompressionFormat.PVRTC14A)
 MIPMAPPABLE_FORMATS.add(CompressionFormat.ATC)
 MIPMAPPABLE_FORMATS.add(CompressionFormat.DXT1)
 MIPMAPPABLE_FORMATS.add(CompressionFormat.DXT3)
 MIPMAPPABLE_FORMATS.add(CompressionFormat.DXT5)
```

### Comparing `aepi-0.8.3.1/src/AEPi/exceptions.py` & `aepi-0.8.3.2/src/AEPi/exceptions.py`

 * *Files identical despite different names*

### Comparing `aepi-0.8.3.1/src/AEPi/image/AEI.py` & `aepi-0.8.3.2/src/AEPi/image/AEI.py`

 * *Files identical despite different names*

### Comparing `aepi-0.8.3.1/src/AEPi/image/texture.py` & `aepi-0.8.3.2/src/AEPi/image/texture.py`

 * *Files identical despite different names*

### Comparing `aepi-0.8.3.1/src/AEPi/lib/binaryio.py` & `aepi-0.8.3.2/src/AEPi/lib/binaryio.py`

 * *Files identical despite different names*

### Comparing `aepi-0.8.3.1/src/AEPi/lib/imageOps.py` & `aepi-0.8.3.2/src/AEPi/lib/imageOps.py`

 * *Files identical despite different names*

### Comparing `aepi-0.8.3.1/src/AEPi.egg-info/PKG-INFO` & `aepi-0.8.3.2/src/AEPi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AEPi
-Version: 0.8.3.1
+Version: 0.8.3.2
 Summary: Read and write Abyss Engine Image (AEI) files from python, for Galaxy on Fire 2
 Home-page: https://github.com/Trimatix/AEPi
 Author: Jasper Law
 Author-email: trimatix.music@gmail.com
 Project-URL: Bug Tracker, https://github.com/Trimatix/AEPi/issues
 Keywords: game,python,galaxy-on-fire,image-compression,image-conversion,game-mod-tool,abyss-engine
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: AEPi Version: 0.8.3.1 Summary: Read and write Abyss
+Metadata-Version: 2.1 Name: AEPi Version: 0.8.3.2 Summary: Read and write Abyss
 Engine Image (AEI) files from python, for Galaxy on Fire 2 Home-page: https://
 github.com/Trimatix/AEPi Author: Jasper Law Author-email:
 trimatix.music@gmail.com Project-URL: Bug Tracker, https://github.com/Trimatix/
 AEPi/issues Keywords: game,python,galaxy-on-fire,image-compression,image-
 conversion,game-mod-tool,abyss-engine Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `aepi-0.8.3.1/src/AEPi.egg-info/SOURCES.txt` & `aepi-0.8.3.2/src/AEPi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

