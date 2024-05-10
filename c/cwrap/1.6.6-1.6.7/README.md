# Comparing `tmp/cwrap-1.6.6-py3-none-any.whl.zip` & `tmp/cwrap-1.6.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 16136 bytes, number of entries: 14
--rw-r--r--  2.0 unx     1875 b- defN 24-Mar-15 12:38 cwrap/__init__.py
--rw-r--r--  2.0 unx     5020 b- defN 24-Mar-15 12:38 cwrap/basecclass.py
--rw-r--r--  2.0 unx     5319 b- defN 24-Mar-15 12:38 cwrap/basecenum.py
--rw-r--r--  2.0 unx     2091 b- defN 24-Mar-15 12:38 cwrap/basecvalue.py
--rw-r--r--  2.0 unx     5948 b- defN 24-Mar-15 12:38 cwrap/cfile.py
--rw-r--r--  2.0 unx     3756 b- defN 24-Mar-15 12:38 cwrap/clib.py
--rw-r--r--  2.0 unx     1931 b- defN 24-Mar-15 12:38 cwrap/metacwrap.py
--rw-r--r--  2.0 unx    10013 b- defN 24-Mar-15 12:38 cwrap/prototype.py
--rw-r--r--  2.0 unx      411 b- defN 24-Mar-15 12:38 cwrap/version.py
--rw-r--r--  2.0 unx      674 b- defN 24-Mar-15 12:38 cwrap-1.6.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     1222 b- defN 24-Mar-15 12:38 cwrap-1.6.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-15 12:38 cwrap-1.6.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 24-Mar-15 12:38 cwrap-1.6.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1039 b- defN 24-Mar-15 12:38 cwrap-1.6.6.dist-info/RECORD
-14 files, 39397 bytes uncompressed, 14448 bytes compressed:  63.3%
+Zip file size: 15129 bytes, number of entries: 14
+-rw-r--r--  2.0 unx     1935 b- defN 24-May-10 12:04 cwrap/__init__.py
+-rw-r--r--  2.0 unx     4804 b- defN 24-May-10 12:04 cwrap/basecclass.py
+-rw-r--r--  2.0 unx     5119 b- defN 24-May-10 12:04 cwrap/basecenum.py
+-rw-r--r--  2.0 unx     2102 b- defN 24-May-10 12:04 cwrap/basecvalue.py
+-rw-r--r--  2.0 unx     3233 b- defN 24-May-10 12:04 cwrap/cfile.py
+-rw-r--r--  2.0 unx     3591 b- defN 24-May-10 12:04 cwrap/clib.py
+-rw-r--r--  2.0 unx     2017 b- defN 24-May-10 12:04 cwrap/metacwrap.py
+-rw-r--r--  2.0 unx     9228 b- defN 24-May-10 12:04 cwrap/prototype.py
+-rw-r--r--  2.0 unx      411 b- defN 24-May-10 12:04 cwrap/version.py
+-rw-r--r--  2.0 unx      674 b- defN 24-May-10 12:04 cwrap-1.6.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1203 b- defN 24-May-10 12:04 cwrap-1.6.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-10 12:04 cwrap-1.6.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 24-May-10 12:04 cwrap-1.6.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1038 b- defN 24-May-10 12:04 cwrap-1.6.7.dist-info/RECORD
+14 files, 35453 bytes uncompressed, 13441 bytes compressed:  62.1%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: cwrap/prototype.py
 Comment: 
 
 Filename: cwrap/version.py
 Comment: 
 
-Filename: cwrap-1.6.6.dist-info/LICENSE
+Filename: cwrap-1.6.7.dist-info/LICENSE
 Comment: 
 
-Filename: cwrap-1.6.6.dist-info/METADATA
+Filename: cwrap-1.6.7.dist-info/METADATA
 Comment: 
 
-Filename: cwrap-1.6.6.dist-info/WHEEL
+Filename: cwrap-1.6.7.dist-info/WHEEL
 Comment: 
 
-Filename: cwrap-1.6.6.dist-info/top_level.txt
+Filename: cwrap-1.6.7.dist-info/top_level.txt
 Comment: 
 
-Filename: cwrap-1.6.6.dist-info/RECORD
+Filename: cwrap-1.6.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cwrap/__init__.py

```diff
@@ -24,30 +24,40 @@
 
   cfile: This module implemenets the class CFILE which can be used to
      extract the underlying FILE pointer from a Python filehandle, to
      facilitate use of Python filehandles for functions expecting a
      FILE pointer.
 """
 
-try: from .version import version as __version__
-except ImportError: __version__ = '0.0.0'
+try:
+    from .version import version as __version__
+except ImportError:
+    __version__ = "0.0.0"
 
-__author__ = 'Statoil ASA'
-__copyright__ = 'Copyright 2016, Statoil ASA'
+__author__ = "Statoil ASA"
+__copyright__ = "Copyright 2016, Statoil ASA"
 __credits__ = __author__
-__license__ = 'GPL'
+__license__ = "GPL"
 __maintainer__ = __author__
-__email__ = 'fg_gpl@statoil.com'
-__status__ = 'Prototype'
+__email__ = "fg_gpl@statoil.com"
+__status__ = "Prototype"
 
 from .basecclass import BaseCClass
 from .basecenum import BaseCEnum
 from .basecvalue import BaseCValue
-
-from .cfile import CFILE, copen as open
-from .clib import load, lib_name
-
+from .cfile import CFILE
+from .cfile import copen as open
+from .clib import lib_name, load
 from .metacwrap import MetaCWrap
-from .prototype import REGISTERED_TYPES, Prototype, PrototypeError
+from .prototype import REGISTERED_TYPES, Prototype, PrototypeError  # noqa
 
-__all__ = ['BaseCClass', 'BaseCEnum', 'BaseCValue', 'CFILE', 'open',
-           'MetaCWrap', 'Prototype', 'load', 'lib_name']
+__all__ = [
+    "BaseCClass",
+    "BaseCEnum",
+    "BaseCValue",
+    "CFILE",
+    "open",
+    "MetaCWrap",
+    "Prototype",
+    "load",
+    "lib_name",
+]
```

## cwrap/basecclass.py

```diff
@@ -10,150 +10,145 @@
 #  ERT is distributed in the hope that it will be useful, but WITHOUT ANY
 #  WARRANTY; without even the implied warranty of MERCHANTABILITY or
 #  FITNESS FOR A PARTICULAR PURPOSE.
 #
 #  See the GNU General Public License at <http://www.gnu.org/licenses/gpl.html>
 #  for more details.
 
-from __future__ import (absolute_import, division,
-                        print_function, unicode_literals)
-
-import six
-
 import ctypes
+
 from .metacwrap import MetaCWrap
 
-@six.add_metaclass(MetaCWrap)
-class BaseCClass(object):
+
+class BaseCClass(metaclass=MetaCWrap):
     namespaces = {}
 
     def __init__(self, c_pointer, parent=None, is_reference=False):
         if not c_pointer:
             raise ValueError("Must have a valid (not null) pointer value!")
 
         if c_pointer < 0:
-            raise ValueError("The pointer value is negative! This may be correct, but usually is not!")
+            raise ValueError(
+                "The pointer value is negative! This may be correct, but usually is not!"
+            )
 
         self.__c_pointer = c_pointer
         self.__parent = parent
         self.__is_reference = is_reference
 
     def __new__(cls, *more, **kwargs):
-        obj = super(BaseCClass, cls).__new__(cls)
+        obj = super().__new__(cls)
         obj.__c_pointer = None
         obj.__parent = None
         obj.__is_reference = False
 
         return obj
 
     def is_initialized(self):
         return self._address() is not None
 
     def _address(self):
         return self.__c_pointer
 
     def _ad_str(self):
-        return 'at 0x%x' % self._address()
+        return f"at 0x{self._address():x}"
 
     @classmethod
     def from_param(cls, c_class_object):
         if c_class_object is not None and not isinstance(c_class_object, BaseCClass):
             raise ValueError("c_class_object must be a BaseCClass instance!")
 
         if c_class_object is None:
             return ctypes.c_void_p()
-        else:
-            return ctypes.c_void_p(c_class_object.__c_pointer)
+
+        return ctypes.c_void_p(c_class_object.__c_pointer)
 
     @classmethod
     def createPythonObject(cls, c_pointer):
         if c_pointer is not None:
             new_obj = cls.__new__(cls)
-            BaseCClass.__init__(new_obj, c_pointer=c_pointer, parent=None, is_reference=False)
+            BaseCClass.__init__(
+                new_obj, c_pointer=c_pointer, parent=None, is_reference=False
+            )
             return new_obj
         else:
             return None
 
     @classmethod
     def createCReference(cls, c_pointer, parent=None):
         if c_pointer is not None:
             new_obj = cls.__new__(cls)
-            BaseCClass.__init__(new_obj, c_pointer=c_pointer, parent=parent, is_reference=True)
+            BaseCClass.__init__(
+                new_obj, c_pointer=c_pointer, parent=parent, is_reference=True
+            )
             return new_obj
         else:
             return None
 
     @classmethod
     def storageType(cls):
         return ctypes.c_void_p
 
     def convertToCReference(self, parent):
         self.__is_reference = True
         self.__parent = parent
 
-
     def setParent(self, parent=None):
         if self.__is_reference:
             self.__parent = parent
         else:
             raise UserWarning("Can only set parent on reference types!")
 
         return self
 
     def isReference(self):
-        """ @rtype: bool """
+        """@rtype: bool"""
         return self.__is_reference
 
     def parent(self):
         return self.__parent
 
     def __eq__(self, other):
         # This is the last resort comparison function; it will do a
         # plain pointer comparison on the underlying C object; or
         # Python is-same-object comparison.
         if isinstance(other, BaseCClass):
             return self.__c_pointer == other.__c_pointer
         else:
-            return super(BaseCClass , self) == other
+            return super() == other
 
     def __hash__(self):
         # Similar to last resort comparison; this returns the hash of the
         # underlying C pointer.
         return hash(self.__c_pointer)
 
     def free(self):
         raise NotImplementedError("A BaseCClass requires a free method implementation!")
 
-    def _create_repr(self, args = ''):
+    def _create_repr(self, args=""):
         """Representation on the form (e.g.) 'EclFile(...) at 0x1729'."""
-        return "{0}({1}) {2}".format(self.__class__.__name__, args, self._ad_str())
+        return f"{self.__class__.__name__}({args}) {self._ad_str()}"
 
     def __repr__(self):
         """Representation on the form (e.g.) 'EclFile(...) at 0x1729'."""
         return self._create_repr()
 
     def __del__(self):
-        if self.free is not None:
-            if not self.__is_reference:
-                # Important to check the c_pointer; in the case of failed object creation
-                # we can have a Python object with c_pointer == None.
-                if self.__c_pointer:
-                    self.free()
+        if self.free is not None and not self.__is_reference and self.__c_pointer:
+            # Important to check the c_pointer; in the case of failed object creation
+            # we can have a Python object with c_pointer == None.
+            self.free()
 
     def _invalidateCPointer(self):
         self.__c_pointer = None
 
-
     def __bool__(self):
         """The BaseCClass instance will evaluate to true if it is bound to an
         underlying C object, otherwise it will evaluate to False. More
         elaborate bool tests should be implemented in the derived
         class.
         """
-        if self.__c_pointer:
-            return True
-        else:
-            return False
 
+        return bool(self.__c_pointer)
 
     def __nonzero__(self):
-        return self.__bool__( )
+        return self.__bool__()
```

## cwrap/basecenum.py

```diff
@@ -10,41 +10,36 @@
 #  cwrap is distributed in the hope that it will be useful, but WITHOUT ANY
 #  WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 #  A PARTICULAR PURPOSE.
 #
 #  See the GNU General Public License at <http://www.gnu.org/licenses/gpl.html>
 #  for more details.
 
-from __future__ import absolute_import, division, print_function, unicode_literals
-
 import ctypes
 
-import six
-
 from .metacwrap import MetaCWrap
 
 
-@six.add_metaclass(MetaCWrap)
-class BaseCEnum(object):
+class BaseCEnum(metaclass=MetaCWrap):
     enum_namespace = {}
 
     def __init__(self, *args, **kwargs):
         if not self in self.enum_namespace[self.__class__]:
             raise NotImplementedError("Can not be instantiated directly!")
 
     def __new__(cls, *args, **kwargs):
         if len(args) == 1:
             enum = cls.__resolveEnum(args[0])
 
             if enum is None:
-                raise ValueError("Unknown enum value: %i" % args[0])
+                raise ValueError(f"Unknown enum value: {args[0]}")
 
             return enum
         else:
-            obj = super(BaseCEnum, cls).__new__(cls, *args)
+            obj = super().__new__(cls, *args)
             obj.name = None
             obj.value = None
             return obj
 
     @classmethod
     def from_param(cls, c_class_object):
         if not isinstance(c_class_object, BaseCEnum):
@@ -53,15 +48,15 @@
 
     @classmethod
     def from_string(cls, name):
         for enum in cls.enum_namespace[cls]:
             if enum.name == name:
                 return enum
 
-        raise ValueError("No such enum:%s" % name)
+        raise ValueError(f"No such enum: {name}")
 
     @classmethod
     def addEnum(cls, name, value):
         name = str(name)
         if not isinstance(value, int):
             raise ValueError("Value must be an integer!")
 
@@ -98,15 +93,15 @@
     def __str__(self):
         return self.name
 
     def __repr__(self):
         cn = self.__class__.__name__
         na = self.name
         va = self.value
-        return '%s(name = "%s", value = %s)' % (cn, na, va)
+        return f'{cn}(name = "{na}", value = {va})'
 
     def __add__(self, other):
         self.__assertOtherIsSameType(other)
         value = self.value + other.value
         return self.__resolveOrCreateEnum(value)
 
     def __or__(self, other):
@@ -122,25 +117,25 @@
     def __and__(self, other):
         self.__assertOtherIsSameType(other)
         value = self.value & other.value
         return self.__resolveOrCreateEnum(value)
 
     def __int__(self):
         return self.value
-    
+
     def __index__(self):
         return self.value
 
     def __contains__(self, item):
         return self & item == item
 
     @classmethod
     def __createEnum(cls, value):
         enum = cls.__new__(cls)
-        enum.name = "Unnamed '%s' enum with value: %i" % (str(cls.__name__), value)
+        enum.name = f"Unnamed '{cls.__name__}' enum with value: {value}"
         enum.value = value
         return enum
 
     @classmethod
     def __resolveOrCreateEnum(cls, value):
         enum = cls.__resolveEnum(value)
 
@@ -155,28 +150,24 @@
             if enum.value == value:
                 return enum
         return None
 
     def __assertOtherIsSameType(self, other):
         assert isinstance(
             other, self.__class__
-        ), "Can only operate on enums of same type: %s =! %s" % (
-            self.__class__.__name__,
-            other.__class__.__name__,
-        )
+        ), f"Can only operate on enums of same type: {self.__class__.__name__} =! {other.__class__.__name__}"
 
     @classmethod
     def populateEnum(cls, library, enum_provider_function):
         try:
             func = getattr(library, enum_provider_function)
-        except AttributeError:
+        except AttributeError as err:
             raise ValueError(
-                "Could not find enum description function: %s - can not load enum: %s."
-                % (enum_provider_function, cls.__name__)
-            )
+                f"Could not find enum description function: {enum_provider_function} - can not load enum: {cls.__name__}."
+            ) from err
 
         func.restype = ctypes.c_char_p
         func.argtypes = [ctypes.c_int, ctypes.POINTER(ctypes.c_int)]
 
         index = 0
         while True:
             value = ctypes.c_int()
```

## cwrap/basecvalue.py

```diff
@@ -10,38 +10,60 @@
 #  ERT is distributed in the hope that it will be useful, but WITHOUT ANY
 #  WARRANTY; without even the implied warranty of MERCHANTABILITY or
 #  FITNESS FOR A PARTICULAR PURPOSE.
 #
 #  See the GNU General Public License at <http://www.gnu.org/licenses/gpl.html>
 #  for more details.
 
-from __future__ import (absolute_import, division,
-                        print_function, unicode_literals)
-
-import six
-
-from ctypes import (pointer, c_long, c_int, c_bool, c_float, c_double, c_byte,
-                    c_short, c_char, c_ubyte, c_ushort, c_uint, c_ulong)
+from ctypes import (
+    c_bool,
+    c_byte,
+    c_char,
+    c_double,
+    c_float,
+    c_int,
+    c_long,
+    c_short,
+    c_ubyte,
+    c_uint,
+    c_ulong,
+    c_ushort,
+    pointer,
+)
 
 from .metacwrap import MetaCWrap
 
-@six.add_metaclass(MetaCWrap)
-class BaseCValue(object):
+
+class BaseCValue(metaclass=MetaCWrap):
     DATA_TYPE = None
-    LEGAL_TYPES = [c_byte, c_ubyte, c_short, c_ushort, c_int, c_uint, c_long, c_ulong, c_bool, c_char, c_float, c_double]
+    LEGAL_TYPES = [
+        c_byte,
+        c_ubyte,
+        c_short,
+        c_ushort,
+        c_int,
+        c_uint,
+        c_long,
+        c_ulong,
+        c_bool,
+        c_char,
+        c_float,
+        c_double,
+    ]
 
     def __init__(self, value):
-        super(BaseCValue, self).__init__()
+        super().__init__()
 
         if not self.DATA_TYPE in self.LEGAL_TYPES:
-            raise ValueError("DATA_TYPE must be one of these CTypes classes: %s" % BaseCValue.LEGAL_TYPES)
+            raise ValueError(
+                f"DATA_TYPE must be one of these CTypes classes: {BaseCValue.LEGAL_TYPES}"
+            )
 
         self.__value = self.cast(value)
 
-
     def value(self):
         return self.__value.value
 
     @classmethod
     def storageType(cls):
         return cls.type()
```

## cwrap/cfile.py

```diff
@@ -11,164 +11,99 @@
 #  WARRANTY; without even the implied warranty of MERCHANTABILITY or
 #  FITNESS FOR A PARTICULAR PURPOSE.
 #
 #  See the GNU General Public License at <http://www.gnu.org/licenses/gpl.html>
 #  for more details.
 
 import os
-import six
-import sys
-from .prototype import Prototype
-from .basecclass import BaseCClass
 
+from .basecclass import BaseCClass
+from .clib import load as cwrapload
+from .prototype import Prototype
 
-if six.PY2:
-    import ctypes
 
-    def copen(filename, mode='r'):
-        """
-        This is a compatibility layer for functions taking FILE* pointers, and
-        should not be used unless absolutely needed.
-
-        In Python 2 this function is simply an alias for open. In Python 3,
-        however, it returns an instance of CWrapFile, a very light weight
-        wrapper around a FILE* instance.
-        """
-        return open(filename, mode)
-
-    class CFILE(BaseCClass):
-        """
-        Utility class to map a Python file handle <-> FILE* in C
-        """
-        TYPE_NAME = "FILE"
-
-        _as_file = Prototype(ctypes.pythonapi, "void* PyFile_AsFile(py_object)")
-
-        def __init__(self, py_file):
-            """
-            Takes a python file handle and looks up the underlying FILE *
-
-            The purpose of the CFILE class is to be able to use python
-            file handles when calling C functions which expect a FILE
-            pointer. A CFILE instance should be created based on the
-            Python file handle, and that should be passed to the function
-            expecting a FILE pointer.
-
-            The implementation is based on the ctypes object
-            pythonapi which is ctypes wrapping of the CPython api.
-
-              C-function:
-                 void fprintf_hello(FILE * stream , const char * msg);
-
-              Python wrapper:
-                 lib = clib.load( "lib.so" )
-                 fprintf_hello = Prototype(lib, "void fprintf_hello( FILE , char* )")
-
-              Python use:
-                 py_fileH = open("file.txt" , "w")
-                 fprintf_hello( CFILE( py_fileH ) , "Message ...")
-                 py_fileH.close()
-
-            If the supplied argument is not of type py_file the function
-            will raise a TypeException.
-
-            Examples: ecl.ecl.ecl_kw.EclKW.fprintf_grdecl()
-            """
-            c_ptr = self._as_file(py_file)
-            try:
-                super(CFILE, self).__init__(c_ptr)
-            except ValueError:
-                raise TypeError("Sorry - the supplied argument is not a valid "
-                                " Python file handle!")
-
-            self.py_file = py_file
-
-        def __del__(self):
-            pass
-
-
-if six.PY3:
-    from .clib import load as cwrapload
-
-    class LibcPrototype(Prototype):
-        # Load the c standard library (on Linux passsing None does the trick)
-        lib = cwrapload('msvcrt' if os.name == 'nt' else None)
-
-        def __init__(self, prototype, bind=False, allow_attribute_error=False):
-            super(LibcPrototype, self).__init__(
-                LibcPrototype.lib,
-                prototype,
-                bind=bind,
-                allow_attribute_error=allow_attribute_error)
-
-    def copen(filename, mode='r'):
-        """
-        This is a compatibility layer for functions taking FILE* pointers, and
-        should not be used unless absolutely needed.
-
-        In Python 2 this function is simply an alias for open. In Python 3,
-        however, it returns an instance of CWrapFile, a very lightweight
-        wrapper around a FILE* instance.
-        """
-        return CWrapFile(filename, mode)
-
-    class CWrapFile(BaseCClass):
-        """
-        This is a compatibility layer for functions taking FILE* pointers, and
-        should not be used unless absolutely needed.
-
-        CWrapFile is a very lightweight wrapper around FILE* instances. It is
-        meant be used inplace of python file objects that are to be passed to
-        foreign function calls under python 3.
-
-        Example:
-            with cwrap.open('filename', 'mode') as f:
-                foreign_function_call(f)
-        """
-
-        TYPE_NAME = "FILE"
-
-        _fopen = LibcPrototype("void* fopen (char*, char*)")
-        _fclose = LibcPrototype("int fclose (FILE)", bind=True)
-        _fflush = LibcPrototype("int fflush (FILE)", bind=True)
-
-        def __init__(self, fname, mode):
-            c_ptr = self._fopen(fname, mode)
-            self._mode = mode
-            self._fname = fname
-            self._closed = False
-
-            try:
-                super(CWrapFile, self).__init__(c_ptr)
-            except ValueError:
-                self._closed = True
-                raise IOError('Could not open file "{}" in mode {}'
-                              .format(fname, mode))
-
-        def close(self):
-            if not self._closed:
-                self._fflush()
-                cs = self._fclose()
-                if (cs != 0):
-                    raise IOError("Failed to close file")
-                self._closed = True
-
-        def __enter__(self):
-            return self
-
-        def __exit__(self, exc_type, exc_val, exc_tb):
-            self.close()
-            return exc_type is None
-
-        def free(self):
-            self.close()
-
-        def __del__(self):
-            self.close()
-
-    def CFILE(f):
-        if not isinstance(f, CWrapFile):
-            raise TypeError("This function requires the use of CWrapFile, "
-                            "not {} when running Python 3. See "
-                            "help(cwrap.open) for more info"
-                            .format(type(f).__name__))
-        return f
+class LibcPrototype(Prototype):
+    # Load the c standard library (on Linux passsing None does the trick)
+    lib = cwrapload("msvcrt" if os.name == "nt" else None)
+
+    def __init__(self, prototype, bind=False, allow_attribute_error=False):
+        super().__init__(
+            LibcPrototype.lib,
+            prototype,
+            bind=bind,
+            allow_attribute_error=allow_attribute_error,
+        )
+
+
+def copen(filename, mode="r"):
+    """
+    This is a compatibility layer for functions taking FILE* pointers, and
+    should not be used unless absolutely needed.
+
+    It returns an instance of CWrapFile, a very lightweight
+    wrapper around a FILE* instance.
+    """
+    return CWrapFile(filename, mode)
+
+
+class CWrapFile(BaseCClass):
+    """
+    This is a compatibility layer for functions taking FILE* pointers, and
+    should not be used unless absolutely needed.
+
+    CWrapFile is a very lightweight wrapper around FILE* instances. It is
+    meant be used inplace of python file objects that are to be passed to
+    foreign function calls under python 3.
+
+    Example:
+        with cwrap.open('filename', 'mode') as f:
+            foreign_function_call(f)
+    """
+
+    TYPE_NAME = "FILE"
+
+    _fopen = LibcPrototype("void* fopen (char*, char*)")
+    _fclose = LibcPrototype("int fclose (FILE)", bind=True)
+    _fflush = LibcPrototype("int fflush (FILE)", bind=True)
+
+    def __init__(self, fname, mode):
+        c_ptr = self._fopen(fname, mode)
+        self._mode = mode
+        self._fname = fname
+        self._closed = False
+
+        try:
+            super().__init__(c_ptr)
+        except ValueError as err:
+            self._closed = True
+            raise OSError(f'Could not open file "{fname}" in mode {mode}') from err
+
+    def close(self):
+        if not self._closed:
+            self._fflush()
+            cs = self._fclose()
+            if cs != 0:
+                raise OSError("Failed to close file")
+            self._closed = True
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.close()
+        return exc_type is None
+
+    def free(self):
+        self.close()
+
+    def __del__(self):
+        self.close()
+
+
+def CFILE(f):
+    if not isinstance(f, CWrapFile):
+        raise TypeError(
+            "This function requires the use of CWrapFile, "
+            f"not {type(f).__name__} when running Python 3. See "
+            "help(cwrap.open) for more info"
+        )
+    return f
```

## cwrap/clib.py

```diff
@@ -27,84 +27,86 @@
    GEO_LIB = ert.load("libert_geometry")
 
 Otherwise the standard operating system dependency resolve code will
 be invoked when loading libert_geometry, and that could in principle
 lead to loading a different version of libert_util.so
 """
 
-import platform
 import ctypes
 import os
+import platform
 
-so_extension = {"linux"  : "so",
-                "linux2" : "so",
-                "linux3" : "so",
-                "windows": "dll",
-                "darwin" : "dylib" }
+so_extension = {
+    "linux": "so",
+    "linux2": "so",
+    "linux3": "so",
+    "windows": "dll",
+    "darwin": "dylib",
+}
 
 
 # Passing None to the CDLL() function means to open a lib handle to
 # the current runnning process, i.e. like dlopen( NULL ). We must
 # special case this to avoid creating the bogus argument 'None.so'.
 
-def lib_name(lib , path = None , so_version = None, so_ext = None):
+
+def lib_name(lib, path=None, so_version=None, so_ext=None):
     if lib is None:
         return None
     else:
         platform_key = platform.system().lower()
         if so_version is None:
-            so_version = ''
+            so_version = ""
 
         if so_ext:
-            so_name = "%s.%s%s" % (lib, so_ext, so_version)
+            so_name = f"{lib}.{so_ext}{so_version}"
         elif platform_key == "darwin":
-            so_name = "%s%s.%s" % (lib, so_version, so_extension[ platform_key ])
+            so_name = f"{lib}{so_version}.{so_extension[platform_key]}"
         else:
-            so_name = "%s.%s%s" % (lib, so_extension[ platform_key ], so_version)
+            so_name = f"{lib}.{so_extension[platform_key]}{so_version}"
 
         if path:
-            return os.path.join( path , so_name )
+            return os.path.join(path, so_name)
         else:
             return so_name
 
 
-
-
-def load( lib, so_version = None, path = None, so_ext = None):
+def load(lib, so_version=None, path=None, so_ext=None):
     """Thin wrapper around the ctypes.CDLL function for loading shared
     library.
 
     If the path argument is non Null the function will first try to
     load with full path. If that fails it wil also try to load without
     a path component, invoking normal dlopen() semantics.
     """
 
     dll = None
-    lib_files = [ lib_name( lib, path = None, so_version = so_version ),
-                  lib_name( lib, path = None, so_version = so_version, so_ext = so_ext ),
-                  lib_name( lib, path = path, so_version = so_version ),
-                  lib_name( lib, path = path, so_version = so_version, so_ext = so_ext )
-                ]
+    lib_files = [
+        lib_name(lib, path=None, so_version=so_version),
+        lib_name(lib, path=None, so_version=so_version, so_ext=so_ext),
+        lib_name(lib, path=path, so_version=so_version),
+        lib_name(lib, path=path, so_version=so_version, so_ext=so_ext),
+    ]
 
     for lib_file in lib_files:
         try:
-            dll = ctypes.CDLL(lib_file , ctypes.RTLD_GLOBAL)
+            dll = ctypes.CDLL(lib_file, ctypes.RTLD_GLOBAL)
             return dll
         except Exception as exc:
             error = exc
 
-    error_msg = "\nFailed to load shared library:%s\n\ndlopen() error: %s\n" % (lib , error)
+    error_msg = f"\nFailed to load shared library:{lib}\n\ndlopen() error: {error}\n"
 
     LD_LIBRARY_PATH = os.getenv("LD_LIBRARY_PATH")
     if not LD_LIBRARY_PATH:
         LD_LIBRARY_PATH = ""
 
-    error_msg += """
+    error_msg += f"""
 The runtime linker has searched through the default location of shared
 libraries, and also the locations mentioned in your LD_LIBRARY_PATH
 variable. Your current LD_LIBRARY_PATH setting is:
 
-   LD_LIBRARY_PATH: %s
+   LD_LIBRARY_PATH: {LD_LIBRARY_PATH}
 
 You might need to update this variable?
-""" % LD_LIBRARY_PATH
+"""
     raise ImportError(error_msg)
```

## cwrap/metacwrap.py

```diff
@@ -11,48 +11,55 @@
 #  WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 #  A PARTICULAR PURPOSE.
 #
 #  See the GNU General Public License at <http://www.gnu.org/licenses/gpl.html>
 #  for more details.
 
 import re
-from types import MethodType
 
 from .prototype import Prototype
 
 
 def snakeCase(name):
-    s1 = re.sub('(.)([A-Z][a-z]+)', r'\1_\2', name)
-    return re.sub('([a-z0-9])([A-Z])', r'\1_\2', s1).lower()
+    s1 = re.sub("(.)([A-Z][a-z]+)", r"\1_\2", name)
+    return re.sub("([a-z0-9])([A-Z])", r"\1_\2", s1).lower()
 
 
 class MetaCWrap(type):
     def __init__(cls, name, bases, attrs):
-        super(MetaCWrap, cls).__init__(name, bases, attrs)
+        super().__init__(name, bases, attrs)
 
         is_return_type = False
         storage_type = None
 
-        if "TYPE_NAME" in attrs:
-            type_name = attrs["TYPE_NAME"]
-        else:
-            type_name = snakeCase(name)
+        type_name = attrs["TYPE_NAME"] if "TYPE_NAME" in attrs else snakeCase(name)
 
         if hasattr(cls, "DATA_TYPE") or hasattr(cls, "enums"):
             is_return_type = True
 
         if hasattr(cls, "storageType"):
             storage_type = cls.storageType()
 
-        Prototype.registerType(type_name, cls, is_return_type=is_return_type, storage_type=storage_type)
+        Prototype.registerType(
+            type_name, cls, is_return_type=is_return_type, storage_type=storage_type
+        )
 
         if hasattr(cls, "createCReference"):
-            Prototype.registerType("%s_ref" % type_name, cls.createCReference, is_return_type=True, storage_type=storage_type)
+            Prototype.registerType(
+                f"{type_name}_ref",
+                cls.createCReference,
+                is_return_type=True,
+                storage_type=storage_type,
+            )
 
         if hasattr(cls, "createPythonObject"):
-            Prototype.registerType("%s_obj" % type_name, cls.createPythonObject, is_return_type=True, storage_type=storage_type)
-
+            Prototype.registerType(
+                f"{type_name}_obj",
+                cls.createPythonObject,
+                is_return_type=True,
+                storage_type=storage_type,
+            )
 
         for key, attr in attrs.items():
             if isinstance(attr, Prototype):
                 attr.resolve()
                 attr.__name__ = key
```

## cwrap/prototype.py

```diff
@@ -16,73 +16,67 @@
 
 import ctypes
 import inspect
 import re
 import sys
 from types import MethodType
 
-import six
 
-
-class TypeDefinition(object):
+class TypeDefinition:
     def __init__(self, type_class_or_function, is_return_type, storage_type, errcheck):
         self.storage_type = storage_type
         self.is_return_type = is_return_type
         self.type_class_or_function = type_class_or_function
 
         # Note that errcheck (python name) can do more than error checking. See
         # toStr in the CStringHelper class.
         self.errcheck = errcheck
 
 
-if six.PY3:
-
-    class CStringHelper(object):
-        @classmethod
-        def from_param(cls, value):
-            if value is None:
-                return None
-            elif isinstance(value, bytes):
-                return value
-            elif isinstance(value, ctypes.Array):
-                return value
-            else:
-                e = value.encode()
-                return e
+class CStringHelper:
+    @classmethod
+    def from_param(cls, value):
+        if value is None:
+            return None
+        elif isinstance(value, (bytes, ctypes.Array)):
+            return value
+        else:
+            e = value.encode()
+            return e
 
-        @staticmethod
-        def toStr(result, func, arguments):
-            """
-            Transform a foreign char* type to str (if python 3).
-
-            ctypes functions have an attribute called errcheck that can not
-            only be used for error checking but also to alter the result. If
-            errcheck is defined, the value returned from that function is what
-            is returned from the foreign function call. In this case, C returns
-            strings in the form of zero-terminated char* strings. To use these
-            as python strings (str) they must be decoded.
-            """
-            if result is None or result == 0:
-                return None
-            return result.decode()
+    @staticmethod
+    def toStr(result, func, arguments):
+        """
+        Transform a foreign char* type to str.
+
+        ctypes functions have an attribute called errcheck that can not
+        only be used for error checking but also to alter the result. If
+        errcheck is defined, the value returned from that function is what
+        is returned from the foreign function call. In this case, C returns
+        strings in the form of zero-terminated char* strings. To use these
+        as python strings (str) they must be decoded.
+        """
+        if result is None or result == 0:
+            return None
+        return result.decode()
 
 
 REGISTERED_TYPES = {}
 """:type: dict[str,TypeDefinition]"""
 
 
 def _registerType(
     type_name,
     type_class_or_function,
     is_return_type=True,
     storage_type=None,
     errcheck=None,
 ):
     if type_name in REGISTERED_TYPES:
-        raise PrototypeError("Type: '%s' already registered!" % type_name)
+        raise PrototypeError(f"Type: '{type_name}' already registered!")
 
     REGISTERED_TYPES[type_name] = TypeDefinition(
         type_class_or_function, is_return_type, storage_type, errcheck
     )
 
 
 _registerType("void", None)
@@ -96,24 +90,22 @@
 _registerType("size_t", ctypes.c_size_t)
 _registerType("size_t*", ctypes.POINTER(ctypes.c_size_t))
 _registerType("bool", ctypes.c_bool)
 _registerType("bool*", ctypes.POINTER(ctypes.c_bool))
 _registerType("long", ctypes.c_long)
 _registerType("long*", ctypes.POINTER(ctypes.c_long))
 _registerType("char", ctypes.c_char)
-if six.PY2:
-    _registerType("char*", ctypes.c_char_p)
-    _registerType("char**", ctypes.POINTER(ctypes.c_char_p))
-if six.PY3:
-    _registerType(
-        "char*",
-        CStringHelper,
-        storage_type=ctypes.c_char_p,
-        errcheck=CStringHelper.toStr,
-    )
+
+
+_registerType(
+    "char*",
+    CStringHelper,
+    storage_type=ctypes.c_char_p,
+    errcheck=CStringHelper.toStr,
+)
 _registerType("float", ctypes.c_float)
 _registerType("float*", ctypes.POINTER(ctypes.c_float))
 _registerType("double", ctypes.c_double)
 _registerType("double*", ctypes.POINTER(ctypes.c_double))
 _registerType("py_object", ctypes.py_object)
 
 PROTOTYPE_PATTERN = (
@@ -123,19 +115,19 @@
 )
 
 
 class PrototypeError(Exception):
     pass
 
 
-class Prototype(object):
+class Prototype:
     pattern = re.compile(PROTOTYPE_PATTERN)
 
     def __init__(self, lib, prototype, bind=False, allow_attribute_error=False):
-        super(Prototype, self).__init__()
+        super().__init__()
         self._lib = lib
         self._prototype = prototype
         self._bind = bind
         self._func = None
         self.__name__ = prototype
         self._resolved = False
         self._allow_attribute_error = allow_attribute_error
@@ -147,54 +139,51 @@
         if type_name in REGISTERED_TYPES:
             type_definition = REGISTERED_TYPES[type_name]
             return (
                 type_definition.type_class_or_function,
                 type_definition.storage_type,
                 type_definition.errcheck,
             )
-        raise ValueError("Unknown type: %s" % type_name)
+        raise ValueError(f"Unknown type: {type_name}")
 
     def shouldBeBound(self):
         return self._bind
 
     def resolve(self):
         match = re.match(Prototype.pattern, self._prototype)
         if not match:
-            raise PrototypeError("Illegal prototype definition: %s\n" % self._prototype)
+            raise PrototypeError(f"Illegal prototype definition: {self._prototype}\n")
         else:
             restype = match.groupdict()["return"]
             function_name = match.groupdict()["function"]
             self.__name__ = function_name
             arguments = match.groupdict()["arguments"].split(",")
 
             try:
                 func = getattr(self._lib, function_name)
-            except AttributeError:
+            except AttributeError as err:
                 if self._allow_attribute_error:
                     return
                 raise PrototypeError(
-                    "Can not find function: %s in library: %s"
-                    % (function_name, self._lib)
-                )
+                    f"Can not find function: {function_name} in library: {self._lib}"
+                ) from err
 
             if (
                 not restype in REGISTERED_TYPES
                 or not REGISTERED_TYPES[restype].is_return_type
             ):
                 sys.stderr.write(
-                    "The type used as return type: %s is not registered as a return type.\n"
-                    % restype
+                    f"The type used as return type: {restype} is not registered as a return type.\n"
                 )
 
                 return_type, storage_type, errcheck = self._parseType(restype)
 
                 if inspect.isclass(return_type):
                     sys.stderr.write(
-                        "  Correct type may be: %s_ref or %s_obj.\n"
-                        % (restype, restype)
+                        f"  Correct type may be: {restype}_ref or {restype}_obj.\n"
                     )
 
                 return None
 
             return_type, storage_type, errcheck = self._parseType(restype)
 
             func.restype = return_type
@@ -223,15 +212,15 @@
     def __call__(self, *args):
         if not self._resolved:
             self.resolve()
             self._resolved = True
         if self._func is None:
             if self._allow_attribute_error:
                 raise NotImplementedError(
-                    "Function:%s has not been properly resolved" % self.__name__
+                    f"Function:{self.__name__} has not been properly resolved"
                 )
             else:
                 raise PrototypeError("Prototype has not been properly resolved")
         if self._bind and not args[0].is_initialized():
             raise ValueError(
                 "Called bound function with uninitialized object of type "
                 f"{type(args[0]).__name__}"
@@ -245,43 +234,33 @@
             # ArgumentError.message will look like this
             #   `argument 4: <type 'exceptions.TypeError'>: wrong type`
             # The only useful information here is the index of the argument
             errMsg = err.message if hasattr(err, "message") else str(err)
             tokens = re.split("[ :]", errMsg)
             argidx = int(tokens[1]) - 1  # it starts from 1
             raise TypeError(
-                (
-                    "Argument {argidx}: cannot create a {argtype} from the given "
-                    "value {actval} ({acttype})"
-                ).format(
-                    argtype=self._func.argtypes[argidx],
-                    argidx=argidx,
-                    actval=repr(args[argidx]),
-                    acttype=type(args[argidx]),
-                )
+                f"Argument {argidx}: cannot create a {self._func.argtypes[argidx]} from the given "
+                f"value {repr(args[argidx])} ({type(args[argidx])})"
             ) from err
 
     def __get__(self, instance, owner):
         if not self._resolved:
             self.resolve()
             self._resolved = True
         if self.shouldBeBound():
-            if six.PY2:
-                return MethodType(self, instance, owner)
-            if six.PY3:
-                return MethodType(self, instance)
+            return MethodType(self, instance)
         else:
             return self
 
     def __repr__(self):
         bound = ""
         if self.shouldBeBound():
             bound = ", bind=True"
 
-        return 'Prototype("%s"%s)' % (self._prototype, bound)
+        return f'Prototype("{self._prototype}"{bound})'
 
     @classmethod
     def registerType(
         cls, type_name, type_class_or_function, is_return_type=True, storage_type=None
     ):
         if storage_type is None and (inspect.isfunction(type_class_or_function)):
             storage_type = ctypes.c_void_p
```

## cwrap/version.py

```diff
@@ -8,9 +8,9 @@
     VERSION_TUPLE = object
 
 version: str
 __version__: str
 __version_tuple__: VERSION_TUPLE
 version_tuple: VERSION_TUPLE
 
-__version__ = version = '1.6.6'
-__version_tuple__ = version_tuple = (1, 6, 6)
+__version__ = version = '1.6.7'
+__version_tuple__ = version_tuple = (1, 6, 7)
```

## Comparing `cwrap-1.6.6.dist-info/LICENSE` & `cwrap-1.6.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cwrap-1.6.6.dist-info/METADATA` & `cwrap-1.6.7.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwrap
-Version: 1.6.6
+Version: 1.6.7
 Summary: cwrap - ctypes blanket
 Home-page: https://github.com/Statoil/cwrap
 Author: Statoil ASA
 Author-email: fg_gpl@statoil.com
 License: GPL-3.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,15 +18,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 License-File: LICENSE
-Requires-Dist: six
 
 
 =======
 cwrap
 =======
 
 Introduction
```

