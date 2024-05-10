# Comparing `tmp/mkm-1.0.2.tar.gz` & `tmp/mkm-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mkm-1.0.2.tar", last modified: Thu Nov  2 05:02:22 2023, max compression
+gzip compressed data, was "dist/mkm-2.0.0.tar", last modified: Fri May 10 15:34:28 2024, max compression
```

## Comparing `mkm-1.0.2.tar` & `mkm-2.0.0.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-11-02 05:02:22.000000 mkm-1.0.2/
--rw-r--r--   0 moky       (501) staff       (20)     7513 2023-11-02 05:02:22.000000 mkm-1.0.2/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)     5732 2021-01-31 04:25:19.000000 mkm-1.0.2/README.md
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-11-02 05:02:22.000000 mkm-1.0.2/mkm/
--rw-r--r--   0 moky       (501) staff       (20)     2141 2023-10-28 14:11:44.000000 mkm-1.0.2/mkm/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     2422 2023-01-31 05:17:07.000000 mkm-1.0.2/mkm/address.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-11-02 05:02:22.000000 mkm-1.0.2/mkm/crypto/
--rw-r--r--   0 moky       (501) staff       (20)     2274 2023-10-13 09:19:03.000000 mkm-1.0.2/mkm/crypto/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     2376 2023-10-06 09:53:47.000000 mkm-1.0.2/mkm/crypto/asymmetric.py
--rw-r--r--   0 moky       (501) staff       (20)     3221 2023-10-06 09:52:42.000000 mkm-1.0.2/mkm/crypto/cryptography.py
--rw-r--r--   0 moky       (501) staff       (20)     3095 2023-09-13 06:54:31.000000 mkm-1.0.2/mkm/crypto/digest.py
--rw-r--r--   0 moky       (501) staff       (20)     6918 2023-10-09 11:50:37.000000 mkm-1.0.2/mkm/crypto/factory.py
--rw-r--r--   0 moky       (501) staff       (20)     3299 2023-10-06 10:59:46.000000 mkm-1.0.2/mkm/crypto/private.py
--rw-r--r--   0 moky       (501) staff       (20)     2743 2023-10-06 10:59:46.000000 mkm-1.0.2/mkm/crypto/public.py
--rw-r--r--   0 moky       (501) staff       (20)     3172 2023-10-06 10:59:54.000000 mkm-1.0.2/mkm/crypto/symmetric.py
--rw-r--r--   0 moky       (501) staff       (20)     9225 2023-10-11 03:07:30.000000 mkm-1.0.2/mkm/factory.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-11-02 05:02:22.000000 mkm-1.0.2/mkm/format/
--rw-r--r--   0 moky       (501) staff       (20)     2570 2023-10-10 08:16:58.000000 mkm-1.0.2/mkm/format/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3729 2023-10-06 06:18:36.000000 mkm-1.0.2/mkm/format/data.py
--rw-r--r--   0 moky       (501) staff       (20)     4729 2023-10-09 10:31:57.000000 mkm-1.0.2/mkm/format/encode.py
--rw-r--r--   0 moky       (501) staff       (20)     6489 2023-10-28 14:13:24.000000 mkm-1.0.2/mkm/format/factory.py
--rw-r--r--   0 moky       (501) staff       (20)     6192 2023-10-12 15:55:17.000000 mkm-1.0.2/mkm/format/file.py
--rw-r--r--   0 moky       (501) staff       (20)     3956 2023-10-06 06:18:32.000000 mkm-1.0.2/mkm/format/object.py
--rw-r--r--   0 moky       (501) staff       (20)     2599 2023-10-06 06:18:51.000000 mkm-1.0.2/mkm/format/string.py
--rw-r--r--   0 moky       (501) staff       (20)     2860 2023-01-31 05:17:07.000000 mkm-1.0.2/mkm/identifier.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-11-02 05:02:22.000000 mkm-1.0.2/mkm/protocol/
--rw-r--r--   0 moky       (501) staff       (20)     1876 2023-10-28 14:11:44.000000 mkm-1.0.2/mkm/protocol/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4071 2023-10-09 10:59:55.000000 mkm-1.0.2/mkm/protocol/address.py
--rw-r--r--   0 moky       (501) staff       (20)     5277 2023-10-09 11:36:26.000000 mkm-1.0.2/mkm/protocol/identifier.py
--rw-r--r--   0 moky       (501) staff       (20)     6437 2023-10-28 14:40:37.000000 mkm-1.0.2/mkm/protocol/meta.py
--rw-r--r--   0 moky       (501) staff       (20)     4447 2023-06-01 12:49:50.000000 mkm-1.0.2/mkm/protocol/network.py
--rw-r--r--   0 moky       (501) staff       (20)     3456 2022-12-12 09:54:19.000000 mkm-1.0.2/mkm/protocol/tai.py
--rw-r--r--   0 moky       (501) staff       (20)     4959 2023-10-28 14:18:28.000000 mkm-1.0.2/mkm/protocol/tai_doc.py
--rw-r--r--   0 moky       (501) staff       (20)     2780 2023-06-01 12:49:27.000000 mkm-1.0.2/mkm/protocol/version.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-11-02 05:02:22.000000 mkm-1.0.2/mkm/types/
--rw-r--r--   0 moky       (501) staff       (20)     1633 2023-10-06 14:22:35.000000 mkm-1.0.2/mkm/types/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3716 2023-10-09 10:47:08.000000 mkm-1.0.2/mkm/types/converter.py
--rw-r--r--   0 moky       (501) staff       (20)     8464 2023-10-09 15:36:51.000000 mkm-1.0.2/mkm/types/dictionary.py
--rw-r--r--   0 moky       (501) staff       (20)    25301 2023-06-09 15:45:23.000000 mkm-1.0.2/mkm/types/string.py
--rw-r--r--   0 moky       (501) staff       (20)     5297 2023-10-06 09:10:41.000000 mkm-1.0.2/mkm/types/wrapper.py
--rw-r--r--   0 moky       (501) staff       (20)     7070 2023-10-14 03:27:54.000000 mkm-1.0.2/mkm/types/x.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-11-02 05:02:22.000000 mkm-1.0.2/mkm.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)     7513 2023-11-02 05:02:22.000000 mkm-1.0.2/mkm.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      835 2023-11-02 05:02:22.000000 mkm-1.0.2/mkm.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2023-11-02 05:02:22.000000 mkm-1.0.2/mkm.egg-info/dependency_links.txt
--rw-r--r--   0 moky       (501) staff       (20)        4 2023-11-02 05:02:22.000000 mkm-1.0.2/mkm.egg-info/top_level.txt
--rw-r--r--   0 moky       (501) staff       (20)       38 2023-11-02 05:02:22.000000 mkm-1.0.2/setup.cfg
--rw-r--r--   0 moky       (501) staff       (20)      908 2023-10-28 14:06:36.000000 mkm-1.0.2/setup.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:34:28.000000 mkm-2.0.0/
+-rw-r--r--   0 moky       (501) staff       (20)     7513 2024-05-10 15:34:28.000000 mkm-2.0.0/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)     5732 2021-01-31 04:25:19.000000 mkm-2.0.0/README.md
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:34:28.000000 mkm-2.0.0/mkm/
+-rw-r--r--   0 moky       (501) staff       (20)     2141 2023-10-28 14:11:44.000000 mkm-2.0.0/mkm/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     2422 2023-01-31 05:17:07.000000 mkm-2.0.0/mkm/address.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:34:28.000000 mkm-2.0.0/mkm/crypto/
+-rw-r--r--   0 moky       (501) staff       (20)     2274 2023-10-13 09:19:03.000000 mkm-2.0.0/mkm/crypto/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     2376 2023-10-06 09:53:47.000000 mkm-2.0.0/mkm/crypto/asymmetric.py
+-rw-r--r--   0 moky       (501) staff       (20)     3221 2023-10-06 09:52:42.000000 mkm-2.0.0/mkm/crypto/cryptography.py
+-rw-r--r--   0 moky       (501) staff       (20)     3095 2023-09-13 06:54:31.000000 mkm-2.0.0/mkm/crypto/digest.py
+-rw-r--r--   0 moky       (501) staff       (20)     6918 2023-10-09 11:50:37.000000 mkm-2.0.0/mkm/crypto/factory.py
+-rw-r--r--   0 moky       (501) staff       (20)     3299 2023-10-06 10:59:46.000000 mkm-2.0.0/mkm/crypto/private.py
+-rw-r--r--   0 moky       (501) staff       (20)     2743 2023-10-06 10:59:46.000000 mkm-2.0.0/mkm/crypto/public.py
+-rw-r--r--   0 moky       (501) staff       (20)     3172 2023-10-06 10:59:54.000000 mkm-2.0.0/mkm/crypto/symmetric.py
+-rw-r--r--   0 moky       (501) staff       (20)     9225 2023-10-11 03:07:30.000000 mkm-2.0.0/mkm/factory.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:34:28.000000 mkm-2.0.0/mkm/format/
+-rw-r--r--   0 moky       (501) staff       (20)     2570 2023-10-10 08:16:58.000000 mkm-2.0.0/mkm/format/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3729 2023-10-06 06:18:36.000000 mkm-2.0.0/mkm/format/data.py
+-rw-r--r--   0 moky       (501) staff       (20)     4729 2023-10-09 10:31:57.000000 mkm-2.0.0/mkm/format/encode.py
+-rw-r--r--   0 moky       (501) staff       (20)     6489 2023-10-28 14:13:24.000000 mkm-2.0.0/mkm/format/factory.py
+-rw-r--r--   0 moky       (501) staff       (20)     6192 2023-10-12 15:55:17.000000 mkm-2.0.0/mkm/format/file.py
+-rw-r--r--   0 moky       (501) staff       (20)     3956 2023-10-06 06:18:32.000000 mkm-2.0.0/mkm/format/object.py
+-rw-r--r--   0 moky       (501) staff       (20)     2599 2023-10-06 06:18:51.000000 mkm-2.0.0/mkm/format/string.py
+-rw-r--r--   0 moky       (501) staff       (20)     2860 2023-01-31 05:17:07.000000 mkm-2.0.0/mkm/identifier.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:34:28.000000 mkm-2.0.0/mkm/protocol/
+-rw-r--r--   0 moky       (501) staff       (20)     1876 2023-10-28 14:11:44.000000 mkm-2.0.0/mkm/protocol/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4071 2023-10-09 10:59:55.000000 mkm-2.0.0/mkm/protocol/address.py
+-rw-r--r--   0 moky       (501) staff       (20)     5277 2023-10-09 11:36:26.000000 mkm-2.0.0/mkm/protocol/identifier.py
+-rw-r--r--   0 moky       (501) staff       (20)     6437 2023-10-28 14:40:37.000000 mkm-2.0.0/mkm/protocol/meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     4447 2023-06-01 12:49:50.000000 mkm-2.0.0/mkm/protocol/network.py
+-rw-r--r--   0 moky       (501) staff       (20)     3456 2022-12-12 09:54:19.000000 mkm-2.0.0/mkm/protocol/tai.py
+-rw-r--r--   0 moky       (501) staff       (20)     5016 2023-12-04 10:46:14.000000 mkm-2.0.0/mkm/protocol/tai_doc.py
+-rw-r--r--   0 moky       (501) staff       (20)     2780 2023-06-01 12:49:27.000000 mkm-2.0.0/mkm/protocol/version.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:34:28.000000 mkm-2.0.0/mkm/types/
+-rw-r--r--   0 moky       (501) staff       (20)     1670 2024-05-06 09:47:14.000000 mkm-2.0.0/mkm/types/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3796 2024-05-06 08:24:42.000000 mkm-2.0.0/mkm/types/converter.py
+-rw-r--r--   0 moky       (501) staff       (20)     2744 2024-05-06 09:42:27.000000 mkm-2.0.0/mkm/types/copier.py
+-rw-r--r--   0 moky       (501) staff       (20)     8489 2024-05-06 09:46:42.000000 mkm-2.0.0/mkm/types/dictionary.py
+-rw-r--r--   0 moky       (501) staff       (20)    25301 2023-06-09 15:45:23.000000 mkm-2.0.0/mkm/types/string.py
+-rw-r--r--   0 moky       (501) staff       (20)     5295 2024-05-06 09:50:48.000000 mkm-2.0.0/mkm/types/wrapper.py
+-rw-r--r--   0 moky       (501) staff       (20)     7070 2023-10-14 03:27:54.000000 mkm-2.0.0/mkm/types/x.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:34:28.000000 mkm-2.0.0/mkm.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)     7513 2024-05-10 15:34:28.000000 mkm-2.0.0/mkm.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      855 2024-05-10 15:34:28.000000 mkm-2.0.0/mkm.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2024-05-10 15:34:28.000000 mkm-2.0.0/mkm.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)        4 2024-05-10 15:34:28.000000 mkm-2.0.0/mkm.egg-info/top_level.txt
+-rw-r--r--   0 moky       (501) staff       (20)       38 2024-05-10 15:34:28.000000 mkm-2.0.0/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)      908 2024-05-10 15:34:08.000000 mkm-2.0.0/setup.py
```

### Comparing `mkm-1.0.2/PKG-INFO` & `mkm-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkm
-Version: 1.0.2
+Version: 2.0.0
 Summary: A common identity module
 Home-page: https://github.com/dimchat/mkm-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # Ming Ke Ming (名可名) -- Account Module (Python)
```

### Comparing `mkm-1.0.2/README.md` & `mkm-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `mkm-1.0.2/mkm/__init__.py` & `mkm-2.0.0/mkm/__init__.py`

 * *Files identical despite different names*

### Comparing `mkm-1.0.2/mkm/address.py` & `mkm-2.0.0/mkm/address.py`

 * *Files identical despite different names*

### Comparing `mkm-1.0.2/mkm/crypto/__init__.py` & `mkm-2.0.0/mkm/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `mkm-1.0.2/mkm/crypto/asymmetric.py` & `mkm-2.0.0/mkm/crypto/asymmetric.py`

 * *Files identical despite different names*

### Comparing `mkm-1.0.2/mkm/crypto/cryptography.py` & `mkm-2.0.0/mkm/crypto/cryptography.py`

 * *Files identical despite different names*

### Comparing `mkm-1.0.2/mkm/crypto/digest.py` & `mkm-2.0.0/mkm/crypto/digest.py`

 * *Files identical despite different names*

### Comparing `mkm-1.0.2/mkm/crypto/factory.py` & `mkm-2.0.0/mkm/crypto/factory.py`

 * *Files identical despite different names*

### Comparing `mkm-1.0.2/mkm/crypto/private.py` & `mkm-2.0.0/mkm/crypto/private.py`

 * *Files identical despite different names*

### Comparing `mkm-1.0.2/mkm/crypto/public.py` & `mkm-2.0.0/mkm/crypto/public.py`

 * *Files identical despite different names*

### Comparing `mkm-1.0.2/mkm/crypto/symmetric.py` & `mkm-2.0.0/mkm/crypto/symmetric.py`

 * *Files identical despite different names*

### Comparing `mkm-1.0.2/mkm/factory.py` & `mkm-2.0.0/mkm/factory.py`

 * *Files identical despite different names*

### Comparing `mkm-1.0.2/mkm/format/__init__.py` & `mkm-2.0.0/mkm/format/__init__.py`

 * *Files identical despite different names*

### Comparing `mkm-1.0.2/mkm/format/data.py` & `mkm-2.0.0/mkm/format/data.py`

 * *Files identical despite different names*

### Comparing `mkm-1.0.2/mkm/format/encode.py` & `mkm-2.0.0/mkm/format/encode.py`

 * *Files identical despite different names*

### Comparing `mkm-1.0.2/mkm/format/factory.py` & `mkm-2.0.0/mkm/format/factory.py`

 * *Files identical despite different names*

### Comparing `mkm-1.0.2/mkm/format/file.py` & `mkm-2.0.0/mkm/format/file.py`

 * *Files identical despite different names*

### Comparing `mkm-1.0.2/mkm/format/object.py` & `mkm-2.0.0/mkm/format/object.py`

 * *Files identical despite different names*

### Comparing `mkm-1.0.2/mkm/format/string.py` & `mkm-2.0.0/mkm/format/string.py`

 * *Files identical despite different names*

### Comparing `mkm-1.0.2/mkm/identifier.py` & `mkm-2.0.0/mkm/identifier.py`

 * *Files identical despite different names*

### Comparing `mkm-1.0.2/mkm/protocol/__init__.py` & `mkm-2.0.0/mkm/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `mkm-1.0.2/mkm/protocol/address.py` & `mkm-2.0.0/mkm/protocol/address.py`

 * *Files identical despite different names*

### Comparing `mkm-1.0.2/mkm/protocol/identifier.py` & `mkm-2.0.0/mkm/protocol/identifier.py`

 * *Files identical despite different names*

### Comparing `mkm-1.0.2/mkm/protocol/meta.py` & `mkm-2.0.0/mkm/protocol/meta.py`

 * *Files identical despite different names*

### Comparing `mkm-1.0.2/mkm/protocol/network.py` & `mkm-2.0.0/mkm/protocol/network.py`

 * *Files identical despite different names*

### Comparing `mkm-1.0.2/mkm/protocol/tai.py` & `mkm-2.0.0/mkm/protocol/tai.py`

 * *Files identical despite different names*

### Comparing `mkm-1.0.2/mkm/protocol/tai_doc.py` & `mkm-2.0.0/mkm/protocol/tai_doc.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             }
     """
 
     #
     #  Document types
     #
     VISA = 'visa'          # for user info (communicate key)
+    PROFILE = 'profile'    # for user profile (reserved)
     BULLETIN = 'bulletin'  # for group info (owner, assistants)
 
     @property
     @abstractmethod
     def type(self) -> Optional[str]:
         """
         Get document type
```

### Comparing `mkm-1.0.2/mkm/protocol/version.py` & `mkm-2.0.0/mkm/protocol/version.py`

 * *Files identical despite different names*

### Comparing `mkm-1.0.2/mkm/types/__init__.py` & `mkm-2.0.0/mkm/types/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,23 +20,24 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
 from .converter import Converter
+from .copier import Copier
 from .wrapper import Wrapper, Stringer, Mapper
 from .string import ConstantString  # , String
 from .dictionary import Dictionary
 
 from .x import URI, DateTime
 
 
 __all__ = [
 
     'URI', 'DateTime',
 
-    'Converter',
+    'Converter', 'Copier',
     'Wrapper', 'Stringer', 'Mapper',
     'ConstantString',  # 'String',
     'Dictionary',
 ]
```

### Comparing `mkm-1.0.2/mkm/types/converter.py` & `mkm-2.0.0/mkm/types/converter.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,14 +52,17 @@
             # exactly
             return value
         elif isinstance(value, int):
             return value != 0
         elif isinstance(value, float):
             return value != 0.0
         text = value if isinstance(value, str) else str(value)
+        text = text.strip()
+        if len(text) == 0:
+            return False
         lo = text.lower()
         return lo not in FALSE_LIST
         # return lo in TRUE_LIST
 
     @classmethod
     def get_int(cls, value: Any, default: Optional[int]) -> Optional[int]:
         if value is None:
```

### Comparing `mkm-1.0.2/mkm/types/dictionary.py` & `mkm-2.0.0/mkm/types/dictionary.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,21 +19,21 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
-import copy
 from typing import Any, Optional, Iterator, Tuple, Dict
 from typing import Mapping, ItemsView, KeysView, ValuesView
 
 from .x import DateTime
 from .string import Stringer
 from .converter import Converter
+from .copier import Copier
 from .wrapper import Mapper
 
 
 class Dictionary(Mapper):
     """
         Mutable Map Wrapper
         ~~~~~~~~~~~~~~~~~~~
@@ -51,15 +51,15 @@
     @property  # Override
     def dictionary(self) -> Dict:
         return self.__dictionary
 
     # Override
     def copy_dictionary(self, deep_copy: bool = False) -> Dict:
         if deep_copy:
-            copy.deepcopy(self.__dictionary)
+            return Copier.deep_copy(self.__dictionary)
         else:
             return self.__dictionary.copy()
 
     # Override
     def clear(self):
         """ D.clear() -> None.  Remove all items from D. """
         self.__dictionary.clear()
```

### Comparing `mkm-1.0.2/mkm/types/string.py` & `mkm-2.0.0/mkm/types/string.py`

 * *Files identical despite different names*

### Comparing `mkm-1.0.2/mkm/types/wrapper.py` & `mkm-2.0.0/mkm/types/wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,11 +172,11 @@
             dictionary[key] = naked
         return dictionary
 
     @classmethod
     def unwrap_list(cls, a) -> List[Any]:
         """ Unwrap values in the array """
         array = []
-        for value in a:
-            naked = cls.unwrap(value)
+        for item in a:
+            naked = cls.unwrap(item)
             array.append(naked)
         return array
```

### Comparing `mkm-1.0.2/mkm/types/x.py` & `mkm-2.0.0/mkm/types/x.py`

 * *Files identical despite different names*

### Comparing `mkm-1.0.2/mkm.egg-info/PKG-INFO` & `mkm-2.0.0/mkm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkm
-Version: 1.0.2
+Version: 2.0.0
 Summary: A common identity module
 Home-page: https://github.com/dimchat/mkm-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # Ming Ke Ming (名可名) -- Account Module (Python)
```

### Comparing `mkm-1.0.2/mkm.egg-info/SOURCES.txt` & `mkm-2.0.0/mkm.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,11 +29,12 @@
 mkm/protocol/meta.py
 mkm/protocol/network.py
 mkm/protocol/tai.py
 mkm/protocol/tai_doc.py
 mkm/protocol/version.py
 mkm/types/__init__.py
 mkm/types/converter.py
+mkm/types/copier.py
 mkm/types/dictionary.py
 mkm/types/string.py
 mkm/types/wrapper.py
 mkm/types/x.py
```

### Comparing `mkm-1.0.2/setup.py` & `mkm-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Common Identity Module for decentralized user identity authentication
 """
 
 import io
 
 from setuptools import setup, find_packages
 
-__version__ = '1.0.2'
+__version__ = '2.0.0'
 __author__ = 'Albert Moky'
 __contact__ = 'albert.moky@gmail.com'
 
 with io.open('README.md', 'r', encoding='utf-8') as fh:
     readme = fh.read()
 
 setup(
```

