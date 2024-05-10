# Comparing `tmp/pymonocypher-4.0.2.1.tar.gz` & `tmp/pymonocypher-4.0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymonocypher-4.0.2.1.tar", last modified: Wed May  8 21:51:01 2024, max compression
+gzip compressed data, was "pymonocypher-4.0.2.2.tar", last modified: Fri May 10 15:21:37 2024, max compression
```

## Comparing `pymonocypher-4.0.2.1.tar` & `pymonocypher-4.0.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:51:01.233281 pymonocypher-4.0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-05-08 21:50:55.000000 pymonocypher-4.0.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-08 21:50:55.000000 pymonocypher-4.0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-08 21:51:01.233281 pymonocypher-4.0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-08 21:50:55.000000 pymonocypher-4.0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   749610 2024-05-08 21:51:00.000000 pymonocypher-4.0.2.1/c_monocypher.c
--rw-r--r--   0 runner    (1001) docker     (127)   100271 2024-05-08 21:50:55.000000 pymonocypher-4.0.2.1/monocypher.c
--rw-r--r--   0 runner    (1001) docker     (127)    12175 2024-05-08 21:50:55.000000 pymonocypher-4.0.2.1/monocypher.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:51:01.233281 pymonocypher-4.0.2.1/pymonocypher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-08 21:51:01.000000 pymonocypher-4.0.2.1/pymonocypher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-08 21:51:01.000000 pymonocypher-4.0.2.1/pymonocypher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 21:51:01.000000 pymonocypher-4.0.2.1/pymonocypher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-08 21:51:01.000000 pymonocypher-4.0.2.1/pymonocypher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 21:51:01.000000 pymonocypher-4.0.2.1/pymonocypher.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-08 21:50:55.000000 pymonocypher-4.0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-08 21:51:01.233281 pymonocypher-4.0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-08 21:50:55.000000 pymonocypher-4.0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:51:01.233281 pymonocypher-4.0.2.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 21:50:55.000000 pymonocypher-4.0.2.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1873923 2024-05-08 21:50:55.000000 pymonocypher-4.0.2.1/test/blake2-kat.json
--rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-05-08 21:50:55.000000 pymonocypher-4.0.2.1/test/test_monocypher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:21:37.531598 pymonocypher-4.0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-05-10 15:21:31.000000 pymonocypher-4.0.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-10 15:21:31.000000 pymonocypher-4.0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-10 15:21:37.531598 pymonocypher-4.0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-10 15:21:31.000000 pymonocypher-4.0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   755033 2024-05-10 15:21:37.000000 pymonocypher-4.0.2.2/c_monocypher.c
+-rw-r--r--   0 runner    (1001) docker     (127)   100271 2024-05-10 15:21:31.000000 pymonocypher-4.0.2.2/monocypher.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12175 2024-05-10 15:21:31.000000 pymonocypher-4.0.2.2/monocypher.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:21:37.531598 pymonocypher-4.0.2.2/pymonocypher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-10 15:21:37.000000 pymonocypher-4.0.2.2/pymonocypher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-10 15:21:37.000000 pymonocypher-4.0.2.2/pymonocypher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 15:21:37.000000 pymonocypher-4.0.2.2/pymonocypher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 15:21:37.000000 pymonocypher-4.0.2.2/pymonocypher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-10 15:21:37.000000 pymonocypher-4.0.2.2/pymonocypher.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-10 15:21:31.000000 pymonocypher-4.0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-10 15:21:37.531598 pymonocypher-4.0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-10 15:21:31.000000 pymonocypher-4.0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:21:37.531598 pymonocypher-4.0.2.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 15:21:31.000000 pymonocypher-4.0.2.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1873923 2024-05-10 15:21:31.000000 pymonocypher-4.0.2.2/test/blake2-kat.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-05-10 15:21:31.000000 pymonocypher-4.0.2.2/test/test_monocypher.py
```

### Comparing `pymonocypher-4.0.2.1/LICENSE.txt` & `pymonocypher-4.0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pymonocypher-4.0.2.1/PKG-INFO` & `pymonocypher-4.0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonocypher
-Version: 4.0.2.1
+Version: 4.0.2.2
 Summary: Python ctypes bindings to the Monocypher library
 Home-page: https://github.com/jetperch/pymonocypher
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: BSD 2-clause
 Project-URL: Bug Reports, https://github.com/jetperch/pymonocypher/issues
 Project-URL: Source, https://github.com/jetperch/pymonocypher/
```

### Comparing `pymonocypher-4.0.2.1/README.md` & `pymonocypher-4.0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pymonocypher-4.0.2.1/c_monocypher.c` & `pymonocypher-4.0.2.2/c_monocypher.c`

 * *Files 2% similar despite different names*

```diff
@@ -1993,31 +1993,45 @@
 
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
 /* KeywordStringCheck.proto */
 static int __Pyx_CheckKeywordStrings(PyObject *kw, const char* function_name, int kw_allowed);
 
+/* PyObjectFormatSimple.proto */
+#if CYTHON_COMPILING_IN_PYPY
+    #define __Pyx_PyObject_FormatSimple(s, f) (\
+        likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
+        PyObject_Format(s, f))
+#elif PY_MAJOR_VERSION < 3
+    #define __Pyx_PyObject_FormatSimple(s, f) (\
+        likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
+        likely(PyString_CheckExact(s)) ? PyUnicode_FromEncodedObject(s, NULL, "strict") :\
+        PyObject_Format(s, f))
+#elif CYTHON_USE_TYPE_SLOTS
+    #define __Pyx_PyObject_FormatSimple(s, f) (\
+        likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
+        likely(PyLong_CheckExact(s)) ? PyLong_Type.tp_repr(s) :\
+        likely(PyFloat_CheckExact(s)) ? PyFloat_Type.tp_repr(s) :\
+        PyObject_Format(s, f))
+#else
+    #define __Pyx_PyObject_FormatSimple(s, f) (\
+        likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
+        PyObject_Format(s, f))
+#endif
+
 /* PyObjectSetAttrStr.proto */
 #if CYTHON_USE_TYPE_SLOTS
 #define __Pyx_PyObject_DelAttrStr(o,n) __Pyx_PyObject_SetAttrStr(o, n, NULL)
 static CYTHON_INLINE int __Pyx_PyObject_SetAttrStr(PyObject* obj, PyObject* attr_name, PyObject* value);
 #else
 #define __Pyx_PyObject_DelAttrStr(o,n)   PyObject_DelAttr(o,n)
 #define __Pyx_PyObject_SetAttrStr(o,n,v) PyObject_SetAttr(o,n,v)
 #endif
 
-/* PyIntBinop.proto */
-#if !CYTHON_COMPILING_IN_PYPY
-static PyObject* __Pyx_PyInt_MultiplyObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check);
-#else
-#define __Pyx_PyInt_MultiplyObjC(op1, op2, intval, inplace, zerodivision_check)\
-    (inplace ? PyNumber_InPlaceMultiply(op1, op2) : PyNumber_Multiply(op1, op2))
-#endif
-
 /* GetException.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
 static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
 #else
 static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
 #endif
@@ -2042,19 +2056,19 @@
 #define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
 static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
 #else
 #define __Pyx_ExceptionSave(type, value, tb)   PyErr_GetExcInfo(type, value, tb)
 #define __Pyx_ExceptionReset(type, value, tb)  PyErr_SetExcInfo(type, value, tb)
 #endif
 
-/* SliceObject.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GetSlice(
-        PyObject* obj, Py_ssize_t cstart, Py_ssize_t cstop,
-        PyObject** py_start, PyObject** py_stop, PyObject** py_slice,
-        int has_cstart, int has_cstop, int wraparound);
+/* ArgTypeTest.proto */
+#define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
+    ((likely(__Pyx_IS_TYPE(obj, type) | (none_allowed && (obj == Py_None)))) ? 1 :\
+        __Pyx__ArgTypeTest(obj, type, name, exact))
+static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
 
 /* PyDictVersioning.proto */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 #define __PYX_DICT_VERSION_INIT  ((PY_UINT64_T) -1)
 #define __PYX_GET_DICT_VERSION(dict)  (((PyDictObject*)(dict))->ma_version_tag)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)\
     (version_var) = __PYX_GET_DICT_VERSION(dict);\
@@ -2095,20 +2109,14 @@
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
-/* ArgTypeTest.proto */
-#define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
-    ((likely(__Pyx_IS_TYPE(obj, type) | (none_allowed && (obj == Py_None)))) ? 1 :\
-        __Pyx__ArgTypeTest(obj, type, name, exact))
-static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
-
 /* RaiseUnexpectedTypeError.proto */
 static int __Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj);
 
 /* PyObjectCallNoArg.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
 
 /* PyObjectGetMethod.proto */
@@ -2184,20 +2192,20 @@
 static PyObject* __pyx_convert__to_py_crypto_argon2_config(crypto_argon2_config s);
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_uint32_t(uint32_t value);
-
 /* CIntFromPy.proto */
 static CYTHON_INLINE uint32_t __Pyx_PyInt_As_uint32_t(PyObject *);
 
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_uint32_t(uint32_t value);
+
 /* CIntFromPy.proto */
 static CYTHON_INLINE size_t __Pyx_PyInt_As_size_t(PyObject *);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE uint8_t __Pyx_PyInt_As_uint8_t(PyObject *);
 
 /* FormatTypeName.proto */
@@ -2248,14 +2256,15 @@
 /* Module declarations from "libc.stdint" */
 
 /* Module declarations from "libc.string" */
 
 /* Module declarations from "libc.stdlib" */
 
 /* Module declarations from "monocypher" */
+static uint32_t __pyx_f_10monocypher__validate_u32(PyObject *, PyObject *); /*proto*/
 static PyObject *__Pyx_CFunc_f5947c__10monocypher_int__lParen__const_uint8_t__ptr____etc_to_py_1a_1b(int (*)(uint8_t const *, uint8_t const *)); /*proto*/
 /* #### Code section: typeinfo ### */
 /* #### Code section: before_global_var ### */
 #define __Pyx_MODULE_NAME "monocypher"
 extern int __pyx_module_is_main_monocypher;
 int __pyx_module_is_main_monocypher = 0;
 
@@ -2278,14 +2287,15 @@
 static const char __pyx_k__10[] = "*";
 static const char __pyx_k__60[] = "?";
 static const char __pyx_k_key[] = "key";
 static const char __pyx_k_mac[] = "mac";
 static const char __pyx_k_msg[] = "msg";
 static const char __pyx_k_sig[] = "sig";
 static const char __pyx_k_url[] = "__url__";
+static const char __pyx_k_bool[] = "bool";
 static const char __pyx_k_data[] = "data";
 static const char __pyx_k_hash[] = "hash";
 static const char __pyx_k_lock[] = "lock";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_salt[] = "salt";
 static const char __pyx_k_seed[] = "seed";
@@ -2313,15 +2323,15 @@
 static const char __pyx_k_public[] = "public";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_result[] = "result";
 static const char __pyx_k_return[] = "return";
 static const char __pyx_k_secret[] = "secret";
 static const char __pyx_k_unlock[] = "unlock";
 static const char __pyx_k_update[] = "update";
-static const char __pyx_k_4_0_2_1[] = "4.0.2.1";
+static const char __pyx_k_4_0_2_2[] = "4.0.2.2";
 static const char __pyx_k_Blake2b[] = "Blake2b";
 static const char __pyx_k_blake2b[] = "blake2b";
 static const char __pyx_k_default[] = "default";
 static const char __pyx_k_disable[] = "disable";
 static const char __pyx_k_license[] = "__license__";
 static const char __pyx_k_message[] = "message";
 static const char __pyx_k_secrets[] = "secrets";
@@ -2331,14 +2341,15 @@
 static const char __pyx_k_finalize[] = "finalize";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_nb_block[] = "nb_block";
 static const char __pyx_k_nb_lanes[] = "nb_lanes";
 static const char __pyx_k_password[] = "password";
 static const char __pyx_k_randbits[] = "randbits";
 static const char __pyx_k_setstate[] = "__setstate__";
+static const char __pyx_k_too_long[] = " too long: ";
 static const char __pyx_k_warnings[] = "warnings";
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_algorithm[] = "algorithm";
 static const char __pyx_k_copyright[] = "__copyright__";
 static const char __pyx_k_hash_size[] = "hash_size";
 static const char __pyx_k_isenabled[] = "isenabled";
 static const char __pyx_k_nb_blocks[] = "nb_blocks";
@@ -2390,22 +2401,23 @@
 static const char __pyx_k_Invalid_nonce_length[] = "Invalid nonce length ";
 static const char __pyx_k_invalid_nonce_length[] = "invalid nonce length";
 static const char __pyx_k_unsupported_method_s[] = "unsupported method: %s";
 static const char __pyx_k_Invalid_hidden_length[] = "Invalid hidden length ";
 static const char __pyx_k_Blake2b___reduce_cython[] = "Blake2b.__reduce_cython__";
 static const char __pyx_k_Blake2b___setstate_cython[] = "Blake2b.__setstate_cython__";
 static const char __pyx_k_generate_signing_key_pair[] = "generate_signing_key_pair";
+static const char __pyx_k_secret_key_length_invalid[] = "secret key length invalid";
 static const char __pyx_k_compute_signing_public_key[] = "compute_signing_public_key";
 static const char __pyx_k_joulescope_dev_jetperch_com[] = "joulescope-dev@jetperch.com";
 static const char __pyx_k_Pyx_CFunc_f5947c__10monocypher[] = "__Pyx_CFunc_f5947c__10monocypher_int__lParen__const_uint8_t__ptr____etc_to_py_1a_1b.<locals>.wrap";
 static const char __pyx_k_generate_key_exchange_key_pair[] = "generate_key_exchange_key_pair";
 static const char __pyx_k_Monocypher_library_Python_bindi[] = "\nMonocypher library Python bindings.\n\nMonocypher is an easy to use, easy to deploy, auditable crypto library\nwritten in portable C.\n";
 static const char __pyx_k_Pickling_of_struct_members_such[] = "Pickling of struct members such as self._ctx must be explicitly requested with @auto_pickle(True)";
 static const char __pyx_k_compute_key_exchange_public_key[] = "compute_key_exchange_public_key";
-static const char __pyx_k_Copyright_2018_2022_Jetperch_LLC[] = "Copyright 2018-2022 Jetperch LLC";
+static const char __pyx_k_Copyright_2018_2024_Jetperch_LLC[] = "Copyright 2018-2024 Jetperch LLC";
 static const char __pyx_k_IncrementalAuthenticatedEncrypti[] = "IncrementalAuthenticatedEncryption";
 static const char __pyx_k_Python_ctypes_bindings_to_the_Mo[] = "Python ctypes bindings to the Monocypher library";
 static const char __pyx_k_curve_point_is_unsuitable_for_hi[] = "curve point is unsuitable for hiding";
 static const char __pyx_k_https_github_com_jetperch_pymono[] = "https://github.com/jetperch/pymonocypher";
 static const char __pyx_k_IncrementalAuthenticatedEncrypti_2[] = "IncrementalAuthenticatedEncryption.lock";
 static const char __pyx_k_IncrementalAuthenticatedEncrypti_3[] = "IncrementalAuthenticatedEncryption.unlock";
 static const char __pyx_k_IncrementalAuthenticatedEncrypti_4[] = "IncrementalAuthenticatedEncryption.__reduce_cython__";
@@ -2482,22 +2494,22 @@
   #endif
   PyTypeObject *__pyx_ptype_10monocypher_IncrementalAuthenticatedEncryption;
   PyTypeObject *__pyx_ptype_10monocypher_Blake2b;
   PyTypeObject *__pyx_ptype___pyx_scope_struct____Pyx_CFunc_f5947c__10monocypher_int__lParen__const_uint8_t__ptr____etc_to_py_1a_1b;
   PyObject *__pyx_kp_u_16;
   PyObject *__pyx_kp_u_24;
   PyObject *__pyx_kp_u_32;
-  PyObject *__pyx_kp_u_4_0_2_1;
+  PyObject *__pyx_kp_u_4_0_2_2;
   PyObject *__pyx_kp_u_BSD_2_clause;
   PyObject *__pyx_n_s_Blake2b;
   PyObject *__pyx_n_s_Blake2b___reduce_cython;
   PyObject *__pyx_n_s_Blake2b___setstate_cython;
   PyObject *__pyx_n_s_Blake2b_finalize;
   PyObject *__pyx_n_s_Blake2b_update;
-  PyObject *__pyx_kp_u_Copyright_2018_2022_Jetperch_LLC;
+  PyObject *__pyx_kp_u_Copyright_2018_2024_Jetperch_LLC;
   PyObject *__pyx_n_s_IncrementalAuthenticatedEncrypti;
   PyObject *__pyx_n_s_IncrementalAuthenticatedEncrypti_2;
   PyObject *__pyx_n_s_IncrementalAuthenticatedEncrypti_3;
   PyObject *__pyx_n_s_IncrementalAuthenticatedEncrypti_4;
   PyObject *__pyx_n_s_IncrementalAuthenticatedEncrypti_5;
   PyObject *__pyx_kp_u_Invalid_curve_length;
   PyObject *__pyx_kp_u_Invalid_hidden_length;
@@ -2513,23 +2525,25 @@
   PyObject *__pyx_n_s_ValueError;
   PyObject *__pyx_n_s__10;
   PyObject *__pyx_kp_b__4;
   PyObject *__pyx_kp_u__4;
   PyObject *__pyx_n_s__60;
   PyObject *__pyx_n_s_a;
   PyObject *__pyx_n_s_ad;
+  PyObject *__pyx_n_u_ad;
   PyObject *__pyx_n_s_algorithm;
   PyObject *__pyx_n_s_argon2i_32;
   PyObject *__pyx_n_s_associated_data;
   PyObject *__pyx_n_s_asyncio_coroutines;
   PyObject *__pyx_n_s_author;
   PyObject *__pyx_n_s_author_email;
   PyObject *__pyx_n_s_b;
   PyObject *__pyx_n_s_binascii;
   PyObject *__pyx_n_s_blake2b;
+  PyObject *__pyx_n_s_bool;
   PyObject *__pyx_n_s_bytes;
   PyObject *__pyx_kp_s_c_monocypher_pyx;
   PyObject *__pyx_n_s_cfunc_to_py;
   PyObject *__pyx_n_s_chacha20;
   PyObject *__pyx_n_u_chacha20;
   PyObject *__pyx_n_s_cline_in_traceback;
   PyObject *__pyx_n_s_compute_key_exchange_public_key;
@@ -2563,14 +2577,15 @@
   PyObject *__pyx_n_s_initializing;
   PyObject *__pyx_n_s_inputs;
   PyObject *__pyx_kp_u_invalid_nonce_length;
   PyObject *__pyx_n_s_is_coroutine;
   PyObject *__pyx_kp_u_isenabled;
   PyObject *__pyx_kp_u_joulescope_dev_jetperch_com;
   PyObject *__pyx_n_s_key;
+  PyObject *__pyx_n_u_key;
   PyObject *__pyx_n_s_key_exchange;
   PyObject *__pyx_n_s_length;
   PyObject *__pyx_n_s_license;
   PyObject *__pyx_n_s_lock;
   PyObject *__pyx_n_s_mac;
   PyObject *__pyx_n_s_main;
   PyObject *__pyx_n_s_message;
@@ -2583,29 +2598,32 @@
   PyObject *__pyx_n_s_nb_iterations;
   PyObject *__pyx_n_s_nb_lanes;
   PyObject *__pyx_n_s_nb_passes;
   PyObject *__pyx_n_s_nonce;
   PyObject *__pyx_n_u_os;
   PyObject *__pyx_n_s_p;
   PyObject *__pyx_n_s_password;
+  PyObject *__pyx_n_u_password;
   PyObject *__pyx_n_s_plain_text;
   PyObject *__pyx_n_s_public;
   PyObject *__pyx_n_s_public_key;
   PyObject *__pyx_n_u_pymonocypher;
   PyObject *__pyx_n_s_pyx_state;
   PyObject *__pyx_n_s_randbits;
   PyObject *__pyx_n_s_reduce;
   PyObject *__pyx_n_s_reduce_cython;
   PyObject *__pyx_n_s_reduce_ex;
   PyObject *__pyx_n_s_result;
   PyObject *__pyx_n_s_return;
   PyObject *__pyx_n_s_rv;
   PyObject *__pyx_n_s_salt;
+  PyObject *__pyx_n_u_salt;
   PyObject *__pyx_n_s_secret;
   PyObject *__pyx_n_s_secret_key;
+  PyObject *__pyx_kp_u_secret_key_length_invalid;
   PyObject *__pyx_n_s_secrets;
   PyObject *__pyx_n_u_secrets;
   PyObject *__pyx_n_s_seed;
   PyObject *__pyx_n_s_self;
   PyObject *__pyx_n_s_setstate;
   PyObject *__pyx_n_s_setstate_cython;
   PyObject *__pyx_n_s_sig;
@@ -2614,14 +2632,15 @@
   PyObject *__pyx_n_s_signature_sign;
   PyObject *__pyx_n_s_spec;
   PyObject *__pyx_kp_s_stringsource;
   PyObject *__pyx_n_s_test;
   PyObject *__pyx_n_s_their_public_key;
   PyObject *__pyx_n_s_title;
   PyObject *__pyx_n_s_token_bytes;
+  PyObject *__pyx_kp_u_too_long;
   PyObject *__pyx_kp_s_tuple_bytes_bytes;
   PyObject *__pyx_n_s_tweak;
   PyObject *__pyx_n_s_unlock;
   PyObject *__pyx_kp_u_unsupported_method_s;
   PyObject *__pyx_n_s_update;
   PyObject *__pyx_n_s_url;
   PyObject *__pyx_kp_u_utf_8;
@@ -2632,21 +2651,21 @@
   PyObject *__pyx_n_s_wrap;
   PyObject *__pyx_n_s_your_secret_key;
   PyObject *__pyx_int_8;
   PyObject *__pyx_int_16;
   PyObject *__pyx_int_24;
   PyObject *__pyx_int_32;
   PyObject *__pyx_int_64;
-  PyObject *__pyx_int_1024;
+  PyObject *__pyx_int_4294967295;
   PyObject *__pyx_tuple_;
-  PyObject *__pyx_slice__8;
   PyObject *__pyx_tuple__3;
   PyObject *__pyx_tuple__5;
   PyObject *__pyx_tuple__6;
   PyObject *__pyx_tuple__7;
+  PyObject *__pyx_tuple__8;
   PyObject *__pyx_tuple__9;
   PyObject *__pyx_tuple__11;
   PyObject *__pyx_tuple__13;
   PyObject *__pyx_tuple__15;
   PyObject *__pyx_tuple__16;
   PyObject *__pyx_tuple__18;
   PyObject *__pyx_tuple__20;
@@ -2741,22 +2760,22 @@
   Py_CLEAR(clear_module_state->__pyx_ptype_10monocypher_Blake2b);
   Py_CLEAR(clear_module_state->__pyx_type_10monocypher_Blake2b);
   Py_CLEAR(clear_module_state->__pyx_ptype___pyx_scope_struct____Pyx_CFunc_f5947c__10monocypher_int__lParen__const_uint8_t__ptr____etc_to_py_1a_1b);
   Py_CLEAR(clear_module_state->__pyx_scope_struct____Pyx_CFunc_f5947c__10monocypher_int__lParen__const_uint8_t__ptr____etc_to_py_1a_1b);
   Py_CLEAR(clear_module_state->__pyx_kp_u_16);
   Py_CLEAR(clear_module_state->__pyx_kp_u_24);
   Py_CLEAR(clear_module_state->__pyx_kp_u_32);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_4_0_2_1);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_4_0_2_2);
   Py_CLEAR(clear_module_state->__pyx_kp_u_BSD_2_clause);
   Py_CLEAR(clear_module_state->__pyx_n_s_Blake2b);
   Py_CLEAR(clear_module_state->__pyx_n_s_Blake2b___reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_Blake2b___setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_Blake2b_finalize);
   Py_CLEAR(clear_module_state->__pyx_n_s_Blake2b_update);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_Copyright_2018_2022_Jetperch_LLC);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_Copyright_2018_2024_Jetperch_LLC);
   Py_CLEAR(clear_module_state->__pyx_n_s_IncrementalAuthenticatedEncrypti);
   Py_CLEAR(clear_module_state->__pyx_n_s_IncrementalAuthenticatedEncrypti_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_IncrementalAuthenticatedEncrypti_3);
   Py_CLEAR(clear_module_state->__pyx_n_s_IncrementalAuthenticatedEncrypti_4);
   Py_CLEAR(clear_module_state->__pyx_n_s_IncrementalAuthenticatedEncrypti_5);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Invalid_curve_length);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Invalid_hidden_length);
@@ -2772,23 +2791,25 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_ValueError);
   Py_CLEAR(clear_module_state->__pyx_n_s__10);
   Py_CLEAR(clear_module_state->__pyx_kp_b__4);
   Py_CLEAR(clear_module_state->__pyx_kp_u__4);
   Py_CLEAR(clear_module_state->__pyx_n_s__60);
   Py_CLEAR(clear_module_state->__pyx_n_s_a);
   Py_CLEAR(clear_module_state->__pyx_n_s_ad);
+  Py_CLEAR(clear_module_state->__pyx_n_u_ad);
   Py_CLEAR(clear_module_state->__pyx_n_s_algorithm);
   Py_CLEAR(clear_module_state->__pyx_n_s_argon2i_32);
   Py_CLEAR(clear_module_state->__pyx_n_s_associated_data);
   Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
   Py_CLEAR(clear_module_state->__pyx_n_s_author);
   Py_CLEAR(clear_module_state->__pyx_n_s_author_email);
   Py_CLEAR(clear_module_state->__pyx_n_s_b);
   Py_CLEAR(clear_module_state->__pyx_n_s_binascii);
   Py_CLEAR(clear_module_state->__pyx_n_s_blake2b);
+  Py_CLEAR(clear_module_state->__pyx_n_s_bool);
   Py_CLEAR(clear_module_state->__pyx_n_s_bytes);
   Py_CLEAR(clear_module_state->__pyx_kp_s_c_monocypher_pyx);
   Py_CLEAR(clear_module_state->__pyx_n_s_cfunc_to_py);
   Py_CLEAR(clear_module_state->__pyx_n_s_chacha20);
   Py_CLEAR(clear_module_state->__pyx_n_u_chacha20);
   Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
   Py_CLEAR(clear_module_state->__pyx_n_s_compute_key_exchange_public_key);
@@ -2822,14 +2843,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_initializing);
   Py_CLEAR(clear_module_state->__pyx_n_s_inputs);
   Py_CLEAR(clear_module_state->__pyx_kp_u_invalid_nonce_length);
   Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
   Py_CLEAR(clear_module_state->__pyx_kp_u_isenabled);
   Py_CLEAR(clear_module_state->__pyx_kp_u_joulescope_dev_jetperch_com);
   Py_CLEAR(clear_module_state->__pyx_n_s_key);
+  Py_CLEAR(clear_module_state->__pyx_n_u_key);
   Py_CLEAR(clear_module_state->__pyx_n_s_key_exchange);
   Py_CLEAR(clear_module_state->__pyx_n_s_length);
   Py_CLEAR(clear_module_state->__pyx_n_s_license);
   Py_CLEAR(clear_module_state->__pyx_n_s_lock);
   Py_CLEAR(clear_module_state->__pyx_n_s_mac);
   Py_CLEAR(clear_module_state->__pyx_n_s_main);
   Py_CLEAR(clear_module_state->__pyx_n_s_message);
@@ -2842,29 +2864,32 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_nb_iterations);
   Py_CLEAR(clear_module_state->__pyx_n_s_nb_lanes);
   Py_CLEAR(clear_module_state->__pyx_n_s_nb_passes);
   Py_CLEAR(clear_module_state->__pyx_n_s_nonce);
   Py_CLEAR(clear_module_state->__pyx_n_u_os);
   Py_CLEAR(clear_module_state->__pyx_n_s_p);
   Py_CLEAR(clear_module_state->__pyx_n_s_password);
+  Py_CLEAR(clear_module_state->__pyx_n_u_password);
   Py_CLEAR(clear_module_state->__pyx_n_s_plain_text);
   Py_CLEAR(clear_module_state->__pyx_n_s_public);
   Py_CLEAR(clear_module_state->__pyx_n_s_public_key);
   Py_CLEAR(clear_module_state->__pyx_n_u_pymonocypher);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_state);
   Py_CLEAR(clear_module_state->__pyx_n_s_randbits);
   Py_CLEAR(clear_module_state->__pyx_n_s_reduce);
   Py_CLEAR(clear_module_state->__pyx_n_s_reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_reduce_ex);
   Py_CLEAR(clear_module_state->__pyx_n_s_result);
   Py_CLEAR(clear_module_state->__pyx_n_s_return);
   Py_CLEAR(clear_module_state->__pyx_n_s_rv);
   Py_CLEAR(clear_module_state->__pyx_n_s_salt);
+  Py_CLEAR(clear_module_state->__pyx_n_u_salt);
   Py_CLEAR(clear_module_state->__pyx_n_s_secret);
   Py_CLEAR(clear_module_state->__pyx_n_s_secret_key);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_secret_key_length_invalid);
   Py_CLEAR(clear_module_state->__pyx_n_s_secrets);
   Py_CLEAR(clear_module_state->__pyx_n_u_secrets);
   Py_CLEAR(clear_module_state->__pyx_n_s_seed);
   Py_CLEAR(clear_module_state->__pyx_n_s_self);
   Py_CLEAR(clear_module_state->__pyx_n_s_setstate);
   Py_CLEAR(clear_module_state->__pyx_n_s_setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_sig);
@@ -2873,14 +2898,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_signature_sign);
   Py_CLEAR(clear_module_state->__pyx_n_s_spec);
   Py_CLEAR(clear_module_state->__pyx_kp_s_stringsource);
   Py_CLEAR(clear_module_state->__pyx_n_s_test);
   Py_CLEAR(clear_module_state->__pyx_n_s_their_public_key);
   Py_CLEAR(clear_module_state->__pyx_n_s_title);
   Py_CLEAR(clear_module_state->__pyx_n_s_token_bytes);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_too_long);
   Py_CLEAR(clear_module_state->__pyx_kp_s_tuple_bytes_bytes);
   Py_CLEAR(clear_module_state->__pyx_n_s_tweak);
   Py_CLEAR(clear_module_state->__pyx_n_s_unlock);
   Py_CLEAR(clear_module_state->__pyx_kp_u_unsupported_method_s);
   Py_CLEAR(clear_module_state->__pyx_n_s_update);
   Py_CLEAR(clear_module_state->__pyx_n_s_url);
   Py_CLEAR(clear_module_state->__pyx_kp_u_utf_8);
@@ -2891,21 +2917,21 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_wrap);
   Py_CLEAR(clear_module_state->__pyx_n_s_your_secret_key);
   Py_CLEAR(clear_module_state->__pyx_int_8);
   Py_CLEAR(clear_module_state->__pyx_int_16);
   Py_CLEAR(clear_module_state->__pyx_int_24);
   Py_CLEAR(clear_module_state->__pyx_int_32);
   Py_CLEAR(clear_module_state->__pyx_int_64);
-  Py_CLEAR(clear_module_state->__pyx_int_1024);
+  Py_CLEAR(clear_module_state->__pyx_int_4294967295);
   Py_CLEAR(clear_module_state->__pyx_tuple_);
-  Py_CLEAR(clear_module_state->__pyx_slice__8);
   Py_CLEAR(clear_module_state->__pyx_tuple__3);
   Py_CLEAR(clear_module_state->__pyx_tuple__5);
   Py_CLEAR(clear_module_state->__pyx_tuple__6);
   Py_CLEAR(clear_module_state->__pyx_tuple__7);
+  Py_CLEAR(clear_module_state->__pyx_tuple__8);
   Py_CLEAR(clear_module_state->__pyx_tuple__9);
   Py_CLEAR(clear_module_state->__pyx_tuple__11);
   Py_CLEAR(clear_module_state->__pyx_tuple__13);
   Py_CLEAR(clear_module_state->__pyx_tuple__15);
   Py_CLEAR(clear_module_state->__pyx_tuple__16);
   Py_CLEAR(clear_module_state->__pyx_tuple__18);
   Py_CLEAR(clear_module_state->__pyx_tuple__20);
@@ -2978,22 +3004,22 @@
   Py_VISIT(traverse_module_state->__pyx_ptype_10monocypher_Blake2b);
   Py_VISIT(traverse_module_state->__pyx_type_10monocypher_Blake2b);
   Py_VISIT(traverse_module_state->__pyx_ptype___pyx_scope_struct____Pyx_CFunc_f5947c__10monocypher_int__lParen__const_uint8_t__ptr____etc_to_py_1a_1b);
   Py_VISIT(traverse_module_state->__pyx_scope_struct____Pyx_CFunc_f5947c__10monocypher_int__lParen__const_uint8_t__ptr____etc_to_py_1a_1b);
   Py_VISIT(traverse_module_state->__pyx_kp_u_16);
   Py_VISIT(traverse_module_state->__pyx_kp_u_24);
   Py_VISIT(traverse_module_state->__pyx_kp_u_32);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_4_0_2_1);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_4_0_2_2);
   Py_VISIT(traverse_module_state->__pyx_kp_u_BSD_2_clause);
   Py_VISIT(traverse_module_state->__pyx_n_s_Blake2b);
   Py_VISIT(traverse_module_state->__pyx_n_s_Blake2b___reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_Blake2b___setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_Blake2b_finalize);
   Py_VISIT(traverse_module_state->__pyx_n_s_Blake2b_update);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_Copyright_2018_2022_Jetperch_LLC);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_Copyright_2018_2024_Jetperch_LLC);
   Py_VISIT(traverse_module_state->__pyx_n_s_IncrementalAuthenticatedEncrypti);
   Py_VISIT(traverse_module_state->__pyx_n_s_IncrementalAuthenticatedEncrypti_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_IncrementalAuthenticatedEncrypti_3);
   Py_VISIT(traverse_module_state->__pyx_n_s_IncrementalAuthenticatedEncrypti_4);
   Py_VISIT(traverse_module_state->__pyx_n_s_IncrementalAuthenticatedEncrypti_5);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Invalid_curve_length);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Invalid_hidden_length);
@@ -3009,23 +3035,25 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_ValueError);
   Py_VISIT(traverse_module_state->__pyx_n_s__10);
   Py_VISIT(traverse_module_state->__pyx_kp_b__4);
   Py_VISIT(traverse_module_state->__pyx_kp_u__4);
   Py_VISIT(traverse_module_state->__pyx_n_s__60);
   Py_VISIT(traverse_module_state->__pyx_n_s_a);
   Py_VISIT(traverse_module_state->__pyx_n_s_ad);
+  Py_VISIT(traverse_module_state->__pyx_n_u_ad);
   Py_VISIT(traverse_module_state->__pyx_n_s_algorithm);
   Py_VISIT(traverse_module_state->__pyx_n_s_argon2i_32);
   Py_VISIT(traverse_module_state->__pyx_n_s_associated_data);
   Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
   Py_VISIT(traverse_module_state->__pyx_n_s_author);
   Py_VISIT(traverse_module_state->__pyx_n_s_author_email);
   Py_VISIT(traverse_module_state->__pyx_n_s_b);
   Py_VISIT(traverse_module_state->__pyx_n_s_binascii);
   Py_VISIT(traverse_module_state->__pyx_n_s_blake2b);
+  Py_VISIT(traverse_module_state->__pyx_n_s_bool);
   Py_VISIT(traverse_module_state->__pyx_n_s_bytes);
   Py_VISIT(traverse_module_state->__pyx_kp_s_c_monocypher_pyx);
   Py_VISIT(traverse_module_state->__pyx_n_s_cfunc_to_py);
   Py_VISIT(traverse_module_state->__pyx_n_s_chacha20);
   Py_VISIT(traverse_module_state->__pyx_n_u_chacha20);
   Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
   Py_VISIT(traverse_module_state->__pyx_n_s_compute_key_exchange_public_key);
@@ -3059,14 +3087,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_initializing);
   Py_VISIT(traverse_module_state->__pyx_n_s_inputs);
   Py_VISIT(traverse_module_state->__pyx_kp_u_invalid_nonce_length);
   Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
   Py_VISIT(traverse_module_state->__pyx_kp_u_isenabled);
   Py_VISIT(traverse_module_state->__pyx_kp_u_joulescope_dev_jetperch_com);
   Py_VISIT(traverse_module_state->__pyx_n_s_key);
+  Py_VISIT(traverse_module_state->__pyx_n_u_key);
   Py_VISIT(traverse_module_state->__pyx_n_s_key_exchange);
   Py_VISIT(traverse_module_state->__pyx_n_s_length);
   Py_VISIT(traverse_module_state->__pyx_n_s_license);
   Py_VISIT(traverse_module_state->__pyx_n_s_lock);
   Py_VISIT(traverse_module_state->__pyx_n_s_mac);
   Py_VISIT(traverse_module_state->__pyx_n_s_main);
   Py_VISIT(traverse_module_state->__pyx_n_s_message);
@@ -3079,29 +3108,32 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_nb_iterations);
   Py_VISIT(traverse_module_state->__pyx_n_s_nb_lanes);
   Py_VISIT(traverse_module_state->__pyx_n_s_nb_passes);
   Py_VISIT(traverse_module_state->__pyx_n_s_nonce);
   Py_VISIT(traverse_module_state->__pyx_n_u_os);
   Py_VISIT(traverse_module_state->__pyx_n_s_p);
   Py_VISIT(traverse_module_state->__pyx_n_s_password);
+  Py_VISIT(traverse_module_state->__pyx_n_u_password);
   Py_VISIT(traverse_module_state->__pyx_n_s_plain_text);
   Py_VISIT(traverse_module_state->__pyx_n_s_public);
   Py_VISIT(traverse_module_state->__pyx_n_s_public_key);
   Py_VISIT(traverse_module_state->__pyx_n_u_pymonocypher);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_state);
   Py_VISIT(traverse_module_state->__pyx_n_s_randbits);
   Py_VISIT(traverse_module_state->__pyx_n_s_reduce);
   Py_VISIT(traverse_module_state->__pyx_n_s_reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_reduce_ex);
   Py_VISIT(traverse_module_state->__pyx_n_s_result);
   Py_VISIT(traverse_module_state->__pyx_n_s_return);
   Py_VISIT(traverse_module_state->__pyx_n_s_rv);
   Py_VISIT(traverse_module_state->__pyx_n_s_salt);
+  Py_VISIT(traverse_module_state->__pyx_n_u_salt);
   Py_VISIT(traverse_module_state->__pyx_n_s_secret);
   Py_VISIT(traverse_module_state->__pyx_n_s_secret_key);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_secret_key_length_invalid);
   Py_VISIT(traverse_module_state->__pyx_n_s_secrets);
   Py_VISIT(traverse_module_state->__pyx_n_u_secrets);
   Py_VISIT(traverse_module_state->__pyx_n_s_seed);
   Py_VISIT(traverse_module_state->__pyx_n_s_self);
   Py_VISIT(traverse_module_state->__pyx_n_s_setstate);
   Py_VISIT(traverse_module_state->__pyx_n_s_setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_sig);
@@ -3110,14 +3142,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_signature_sign);
   Py_VISIT(traverse_module_state->__pyx_n_s_spec);
   Py_VISIT(traverse_module_state->__pyx_kp_s_stringsource);
   Py_VISIT(traverse_module_state->__pyx_n_s_test);
   Py_VISIT(traverse_module_state->__pyx_n_s_their_public_key);
   Py_VISIT(traverse_module_state->__pyx_n_s_title);
   Py_VISIT(traverse_module_state->__pyx_n_s_token_bytes);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_too_long);
   Py_VISIT(traverse_module_state->__pyx_kp_s_tuple_bytes_bytes);
   Py_VISIT(traverse_module_state->__pyx_n_s_tweak);
   Py_VISIT(traverse_module_state->__pyx_n_s_unlock);
   Py_VISIT(traverse_module_state->__pyx_kp_u_unsupported_method_s);
   Py_VISIT(traverse_module_state->__pyx_n_s_update);
   Py_VISIT(traverse_module_state->__pyx_n_s_url);
   Py_VISIT(traverse_module_state->__pyx_kp_u_utf_8);
@@ -3128,21 +3161,21 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_wrap);
   Py_VISIT(traverse_module_state->__pyx_n_s_your_secret_key);
   Py_VISIT(traverse_module_state->__pyx_int_8);
   Py_VISIT(traverse_module_state->__pyx_int_16);
   Py_VISIT(traverse_module_state->__pyx_int_24);
   Py_VISIT(traverse_module_state->__pyx_int_32);
   Py_VISIT(traverse_module_state->__pyx_int_64);
-  Py_VISIT(traverse_module_state->__pyx_int_1024);
+  Py_VISIT(traverse_module_state->__pyx_int_4294967295);
   Py_VISIT(traverse_module_state->__pyx_tuple_);
-  Py_VISIT(traverse_module_state->__pyx_slice__8);
   Py_VISIT(traverse_module_state->__pyx_tuple__3);
   Py_VISIT(traverse_module_state->__pyx_tuple__5);
   Py_VISIT(traverse_module_state->__pyx_tuple__6);
   Py_VISIT(traverse_module_state->__pyx_tuple__7);
+  Py_VISIT(traverse_module_state->__pyx_tuple__8);
   Py_VISIT(traverse_module_state->__pyx_tuple__9);
   Py_VISIT(traverse_module_state->__pyx_tuple__11);
   Py_VISIT(traverse_module_state->__pyx_tuple__13);
   Py_VISIT(traverse_module_state->__pyx_tuple__15);
   Py_VISIT(traverse_module_state->__pyx_tuple__16);
   Py_VISIT(traverse_module_state->__pyx_tuple__18);
   Py_VISIT(traverse_module_state->__pyx_tuple__20);
@@ -3231,22 +3264,22 @@
 #endif
 #define __pyx_ptype_10monocypher_IncrementalAuthenticatedEncryption __pyx_mstate_global->__pyx_ptype_10monocypher_IncrementalAuthenticatedEncryption
 #define __pyx_ptype_10monocypher_Blake2b __pyx_mstate_global->__pyx_ptype_10monocypher_Blake2b
 #define __pyx_ptype___pyx_scope_struct____Pyx_CFunc_f5947c__10monocypher_int__lParen__const_uint8_t__ptr____etc_to_py_1a_1b __pyx_mstate_global->__pyx_ptype___pyx_scope_struct____Pyx_CFunc_f5947c__10monocypher_int__lParen__const_uint8_t__ptr____etc_to_py_1a_1b
 #define __pyx_kp_u_16 __pyx_mstate_global->__pyx_kp_u_16
 #define __pyx_kp_u_24 __pyx_mstate_global->__pyx_kp_u_24
 #define __pyx_kp_u_32 __pyx_mstate_global->__pyx_kp_u_32
-#define __pyx_kp_u_4_0_2_1 __pyx_mstate_global->__pyx_kp_u_4_0_2_1
+#define __pyx_kp_u_4_0_2_2 __pyx_mstate_global->__pyx_kp_u_4_0_2_2
 #define __pyx_kp_u_BSD_2_clause __pyx_mstate_global->__pyx_kp_u_BSD_2_clause
 #define __pyx_n_s_Blake2b __pyx_mstate_global->__pyx_n_s_Blake2b
 #define __pyx_n_s_Blake2b___reduce_cython __pyx_mstate_global->__pyx_n_s_Blake2b___reduce_cython
 #define __pyx_n_s_Blake2b___setstate_cython __pyx_mstate_global->__pyx_n_s_Blake2b___setstate_cython
 #define __pyx_n_s_Blake2b_finalize __pyx_mstate_global->__pyx_n_s_Blake2b_finalize
 #define __pyx_n_s_Blake2b_update __pyx_mstate_global->__pyx_n_s_Blake2b_update
-#define __pyx_kp_u_Copyright_2018_2022_Jetperch_LLC __pyx_mstate_global->__pyx_kp_u_Copyright_2018_2022_Jetperch_LLC
+#define __pyx_kp_u_Copyright_2018_2024_Jetperch_LLC __pyx_mstate_global->__pyx_kp_u_Copyright_2018_2024_Jetperch_LLC
 #define __pyx_n_s_IncrementalAuthenticatedEncrypti __pyx_mstate_global->__pyx_n_s_IncrementalAuthenticatedEncrypti
 #define __pyx_n_s_IncrementalAuthenticatedEncrypti_2 __pyx_mstate_global->__pyx_n_s_IncrementalAuthenticatedEncrypti_2
 #define __pyx_n_s_IncrementalAuthenticatedEncrypti_3 __pyx_mstate_global->__pyx_n_s_IncrementalAuthenticatedEncrypti_3
 #define __pyx_n_s_IncrementalAuthenticatedEncrypti_4 __pyx_mstate_global->__pyx_n_s_IncrementalAuthenticatedEncrypti_4
 #define __pyx_n_s_IncrementalAuthenticatedEncrypti_5 __pyx_mstate_global->__pyx_n_s_IncrementalAuthenticatedEncrypti_5
 #define __pyx_kp_u_Invalid_curve_length __pyx_mstate_global->__pyx_kp_u_Invalid_curve_length
 #define __pyx_kp_u_Invalid_hidden_length __pyx_mstate_global->__pyx_kp_u_Invalid_hidden_length
@@ -3262,23 +3295,25 @@
 #define __pyx_n_s_ValueError __pyx_mstate_global->__pyx_n_s_ValueError
 #define __pyx_n_s__10 __pyx_mstate_global->__pyx_n_s__10
 #define __pyx_kp_b__4 __pyx_mstate_global->__pyx_kp_b__4
 #define __pyx_kp_u__4 __pyx_mstate_global->__pyx_kp_u__4
 #define __pyx_n_s__60 __pyx_mstate_global->__pyx_n_s__60
 #define __pyx_n_s_a __pyx_mstate_global->__pyx_n_s_a
 #define __pyx_n_s_ad __pyx_mstate_global->__pyx_n_s_ad
+#define __pyx_n_u_ad __pyx_mstate_global->__pyx_n_u_ad
 #define __pyx_n_s_algorithm __pyx_mstate_global->__pyx_n_s_algorithm
 #define __pyx_n_s_argon2i_32 __pyx_mstate_global->__pyx_n_s_argon2i_32
 #define __pyx_n_s_associated_data __pyx_mstate_global->__pyx_n_s_associated_data
 #define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
 #define __pyx_n_s_author __pyx_mstate_global->__pyx_n_s_author
 #define __pyx_n_s_author_email __pyx_mstate_global->__pyx_n_s_author_email
 #define __pyx_n_s_b __pyx_mstate_global->__pyx_n_s_b
 #define __pyx_n_s_binascii __pyx_mstate_global->__pyx_n_s_binascii
 #define __pyx_n_s_blake2b __pyx_mstate_global->__pyx_n_s_blake2b
+#define __pyx_n_s_bool __pyx_mstate_global->__pyx_n_s_bool
 #define __pyx_n_s_bytes __pyx_mstate_global->__pyx_n_s_bytes
 #define __pyx_kp_s_c_monocypher_pyx __pyx_mstate_global->__pyx_kp_s_c_monocypher_pyx
 #define __pyx_n_s_cfunc_to_py __pyx_mstate_global->__pyx_n_s_cfunc_to_py
 #define __pyx_n_s_chacha20 __pyx_mstate_global->__pyx_n_s_chacha20
 #define __pyx_n_u_chacha20 __pyx_mstate_global->__pyx_n_u_chacha20
 #define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
 #define __pyx_n_s_compute_key_exchange_public_key __pyx_mstate_global->__pyx_n_s_compute_key_exchange_public_key
@@ -3312,14 +3347,15 @@
 #define __pyx_n_s_initializing __pyx_mstate_global->__pyx_n_s_initializing
 #define __pyx_n_s_inputs __pyx_mstate_global->__pyx_n_s_inputs
 #define __pyx_kp_u_invalid_nonce_length __pyx_mstate_global->__pyx_kp_u_invalid_nonce_length
 #define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
 #define __pyx_kp_u_isenabled __pyx_mstate_global->__pyx_kp_u_isenabled
 #define __pyx_kp_u_joulescope_dev_jetperch_com __pyx_mstate_global->__pyx_kp_u_joulescope_dev_jetperch_com
 #define __pyx_n_s_key __pyx_mstate_global->__pyx_n_s_key
+#define __pyx_n_u_key __pyx_mstate_global->__pyx_n_u_key
 #define __pyx_n_s_key_exchange __pyx_mstate_global->__pyx_n_s_key_exchange
 #define __pyx_n_s_length __pyx_mstate_global->__pyx_n_s_length
 #define __pyx_n_s_license __pyx_mstate_global->__pyx_n_s_license
 #define __pyx_n_s_lock __pyx_mstate_global->__pyx_n_s_lock
 #define __pyx_n_s_mac __pyx_mstate_global->__pyx_n_s_mac
 #define __pyx_n_s_main __pyx_mstate_global->__pyx_n_s_main
 #define __pyx_n_s_message __pyx_mstate_global->__pyx_n_s_message
@@ -3332,29 +3368,32 @@
 #define __pyx_n_s_nb_iterations __pyx_mstate_global->__pyx_n_s_nb_iterations
 #define __pyx_n_s_nb_lanes __pyx_mstate_global->__pyx_n_s_nb_lanes
 #define __pyx_n_s_nb_passes __pyx_mstate_global->__pyx_n_s_nb_passes
 #define __pyx_n_s_nonce __pyx_mstate_global->__pyx_n_s_nonce
 #define __pyx_n_u_os __pyx_mstate_global->__pyx_n_u_os
 #define __pyx_n_s_p __pyx_mstate_global->__pyx_n_s_p
 #define __pyx_n_s_password __pyx_mstate_global->__pyx_n_s_password
+#define __pyx_n_u_password __pyx_mstate_global->__pyx_n_u_password
 #define __pyx_n_s_plain_text __pyx_mstate_global->__pyx_n_s_plain_text
 #define __pyx_n_s_public __pyx_mstate_global->__pyx_n_s_public
 #define __pyx_n_s_public_key __pyx_mstate_global->__pyx_n_s_public_key
 #define __pyx_n_u_pymonocypher __pyx_mstate_global->__pyx_n_u_pymonocypher
 #define __pyx_n_s_pyx_state __pyx_mstate_global->__pyx_n_s_pyx_state
 #define __pyx_n_s_randbits __pyx_mstate_global->__pyx_n_s_randbits
 #define __pyx_n_s_reduce __pyx_mstate_global->__pyx_n_s_reduce
 #define __pyx_n_s_reduce_cython __pyx_mstate_global->__pyx_n_s_reduce_cython
 #define __pyx_n_s_reduce_ex __pyx_mstate_global->__pyx_n_s_reduce_ex
 #define __pyx_n_s_result __pyx_mstate_global->__pyx_n_s_result
 #define __pyx_n_s_return __pyx_mstate_global->__pyx_n_s_return
 #define __pyx_n_s_rv __pyx_mstate_global->__pyx_n_s_rv
 #define __pyx_n_s_salt __pyx_mstate_global->__pyx_n_s_salt
+#define __pyx_n_u_salt __pyx_mstate_global->__pyx_n_u_salt
 #define __pyx_n_s_secret __pyx_mstate_global->__pyx_n_s_secret
 #define __pyx_n_s_secret_key __pyx_mstate_global->__pyx_n_s_secret_key
+#define __pyx_kp_u_secret_key_length_invalid __pyx_mstate_global->__pyx_kp_u_secret_key_length_invalid
 #define __pyx_n_s_secrets __pyx_mstate_global->__pyx_n_s_secrets
 #define __pyx_n_u_secrets __pyx_mstate_global->__pyx_n_u_secrets
 #define __pyx_n_s_seed __pyx_mstate_global->__pyx_n_s_seed
 #define __pyx_n_s_self __pyx_mstate_global->__pyx_n_s_self
 #define __pyx_n_s_setstate __pyx_mstate_global->__pyx_n_s_setstate
 #define __pyx_n_s_setstate_cython __pyx_mstate_global->__pyx_n_s_setstate_cython
 #define __pyx_n_s_sig __pyx_mstate_global->__pyx_n_s_sig
@@ -3363,14 +3402,15 @@
 #define __pyx_n_s_signature_sign __pyx_mstate_global->__pyx_n_s_signature_sign
 #define __pyx_n_s_spec __pyx_mstate_global->__pyx_n_s_spec
 #define __pyx_kp_s_stringsource __pyx_mstate_global->__pyx_kp_s_stringsource
 #define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
 #define __pyx_n_s_their_public_key __pyx_mstate_global->__pyx_n_s_their_public_key
 #define __pyx_n_s_title __pyx_mstate_global->__pyx_n_s_title
 #define __pyx_n_s_token_bytes __pyx_mstate_global->__pyx_n_s_token_bytes
+#define __pyx_kp_u_too_long __pyx_mstate_global->__pyx_kp_u_too_long
 #define __pyx_kp_s_tuple_bytes_bytes __pyx_mstate_global->__pyx_kp_s_tuple_bytes_bytes
 #define __pyx_n_s_tweak __pyx_mstate_global->__pyx_n_s_tweak
 #define __pyx_n_s_unlock __pyx_mstate_global->__pyx_n_s_unlock
 #define __pyx_kp_u_unsupported_method_s __pyx_mstate_global->__pyx_kp_u_unsupported_method_s
 #define __pyx_n_s_update __pyx_mstate_global->__pyx_n_s_update
 #define __pyx_n_s_url __pyx_mstate_global->__pyx_n_s_url
 #define __pyx_kp_u_utf_8 __pyx_mstate_global->__pyx_kp_u_utf_8
@@ -3381,21 +3421,21 @@
 #define __pyx_n_s_wrap __pyx_mstate_global->__pyx_n_s_wrap
 #define __pyx_n_s_your_secret_key __pyx_mstate_global->__pyx_n_s_your_secret_key
 #define __pyx_int_8 __pyx_mstate_global->__pyx_int_8
 #define __pyx_int_16 __pyx_mstate_global->__pyx_int_16
 #define __pyx_int_24 __pyx_mstate_global->__pyx_int_24
 #define __pyx_int_32 __pyx_mstate_global->__pyx_int_32
 #define __pyx_int_64 __pyx_mstate_global->__pyx_int_64
-#define __pyx_int_1024 __pyx_mstate_global->__pyx_int_1024
+#define __pyx_int_4294967295 __pyx_mstate_global->__pyx_int_4294967295
 #define __pyx_tuple_ __pyx_mstate_global->__pyx_tuple_
-#define __pyx_slice__8 __pyx_mstate_global->__pyx_slice__8
 #define __pyx_tuple__3 __pyx_mstate_global->__pyx_tuple__3
 #define __pyx_tuple__5 __pyx_mstate_global->__pyx_tuple__5
 #define __pyx_tuple__6 __pyx_mstate_global->__pyx_tuple__6
 #define __pyx_tuple__7 __pyx_mstate_global->__pyx_tuple__7
+#define __pyx_tuple__8 __pyx_mstate_global->__pyx_tuple__8
 #define __pyx_tuple__9 __pyx_mstate_global->__pyx_tuple__9
 #define __pyx_tuple__11 __pyx_mstate_global->__pyx_tuple__11
 #define __pyx_tuple__13 __pyx_mstate_global->__pyx_tuple__13
 #define __pyx_tuple__15 __pyx_mstate_global->__pyx_tuple__15
 #define __pyx_tuple__16 __pyx_mstate_global->__pyx_tuple__16
 #define __pyx_tuple__18 __pyx_mstate_global->__pyx_tuple__18
 #define __pyx_tuple__20 __pyx_mstate_global->__pyx_tuple__20
@@ -6691,15 +6731,127 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "monocypher.pyx":317
  * 
  * 
- * def argon2i_32(nb_blocks, nb_iterations, password, salt, key=None, ad=None):             # <<<<<<<<<<<<<<
+ * cdef uint32_t _validate_u32(variable_name, value):             # <<<<<<<<<<<<<<
+ *     if value > 0xffff_ffff:
+ *         raise ValueError(f'{variable_name} too long: {value}')
+ */
+
+static uint32_t __pyx_f_10monocypher__validate_u32(PyObject *__pyx_v_variable_name, PyObject *__pyx_v_value) {
+  uint32_t __pyx_r;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  Py_ssize_t __pyx_t_3;
+  Py_UCS4 __pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
+  uint32_t __pyx_t_6;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("_validate_u32", 1);
+
+  /* "monocypher.pyx":318
+ * 
+ * cdef uint32_t _validate_u32(variable_name, value):
+ *     if value > 0xffff_ffff:             # <<<<<<<<<<<<<<
+ *         raise ValueError(f'{variable_name} too long: {value}')
+ *     return <uint32_t> value
+ */
+  __pyx_t_1 = PyObject_RichCompare(__pyx_v_value, __pyx_int_4294967295, Py_GT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 318, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 318, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (unlikely(__pyx_t_2)) {
+
+    /* "monocypher.pyx":319
+ * cdef uint32_t _validate_u32(variable_name, value):
+ *     if value > 0xffff_ffff:
+ *         raise ValueError(f'{variable_name} too long: {value}')             # <<<<<<<<<<<<<<
+ *     return <uint32_t> value
+ * 
+ */
+    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 319, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_3 = 0;
+    __pyx_t_4 = 127;
+    __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_v_variable_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 319, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_4 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_4) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_4;
+    __pyx_t_3 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
+    __Pyx_GIVEREF(__pyx_t_5);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_5);
+    __pyx_t_5 = 0;
+    __Pyx_INCREF(__pyx_kp_u_too_long);
+    __pyx_t_3 += 11;
+    __Pyx_GIVEREF(__pyx_kp_u_too_long);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_kp_u_too_long);
+    __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_v_value, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 319, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_4 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_4) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_4;
+    __pyx_t_3 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
+    __Pyx_GIVEREF(__pyx_t_5);
+    PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_t_5);
+    __pyx_t_5 = 0;
+    __pyx_t_5 = __Pyx_PyUnicode_Join(__pyx_t_1, 3, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 319, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 319, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_Raise(__pyx_t_1, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __PYX_ERR(0, 319, __pyx_L1_error)
+
+    /* "monocypher.pyx":318
+ * 
+ * cdef uint32_t _validate_u32(variable_name, value):
+ *     if value > 0xffff_ffff:             # <<<<<<<<<<<<<<
+ *         raise ValueError(f'{variable_name} too long: {value}')
+ *     return <uint32_t> value
+ */
+  }
+
+  /* "monocypher.pyx":320
+ *     if value > 0xffff_ffff:
+ *         raise ValueError(f'{variable_name} too long: {value}')
+ *     return <uint32_t> value             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_t_6 = __Pyx_PyInt_As_uint32_t(__pyx_v_value); if (unlikely((__pyx_t_6 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 320, __pyx_L1_error)
+  __pyx_r = ((uint32_t)__pyx_t_6);
+  goto __pyx_L0;
+
+  /* "monocypher.pyx":317
+ * 
+ * 
+ * cdef uint32_t _validate_u32(variable_name, value):             # <<<<<<<<<<<<<<
+ *     if value > 0xffff_ffff:
+ *         raise ValueError(f'{variable_name} too long: {value}')
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_AddTraceback("monocypher._validate_u32", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = -1;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "monocypher.pyx":323
+ * 
+ * 
+ * def argon2i_32(nb_blocks, nb_iterations, password, salt, key=None, ad=None) -> bytes:             # <<<<<<<<<<<<<<
  *     key = b'' if key is None else key
  *     ad = b'' if ad is None else ad
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_10monocypher_11argon2i_32(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
@@ -6766,64 +6918,64 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_nb_blocks)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 317, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 323, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_nb_iterations)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 317, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 323, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("argon2i_32", 0, 4, 6, 1); __PYX_ERR(0, 317, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("argon2i_32", 0, 4, 6, 1); __PYX_ERR(0, 323, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_password)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 317, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 323, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("argon2i_32", 0, 4, 6, 2); __PYX_ERR(0, 317, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("argon2i_32", 0, 4, 6, 2); __PYX_ERR(0, 323, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_salt)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 317, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 323, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("argon2i_32", 0, 4, 6, 3); __PYX_ERR(0, 317, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("argon2i_32", 0, 4, 6, 3); __PYX_ERR(0, 323, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_key);
           if (value) { values[4] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 317, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 323, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_ad);
           if (value) { values[5] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 317, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 323, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "argon2i_32") < 0)) __PYX_ERR(0, 317, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "argon2i_32") < 0)) __PYX_ERR(0, 323, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  6: values[5] = __Pyx_Arg_FASTCALL(__pyx_args, 5);
         CYTHON_FALLTHROUGH;
         case  5: values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
@@ -6840,15 +6992,15 @@
     __pyx_v_password = values[2];
     __pyx_v_salt = values[3];
     __pyx_v_key = values[4];
     __pyx_v_ad = values[5];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("argon2i_32", 0, 4, 6, __pyx_nargs); __PYX_ERR(0, 317, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("argon2i_32", 0, 4, 6, __pyx_nargs); __PYX_ERR(0, 323, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -6901,17 +7053,17 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("argon2i_32", 0);
   __Pyx_INCREF(__pyx_v_key);
   __Pyx_INCREF(__pyx_v_ad);
 
-  /* "monocypher.pyx":318
+  /* "monocypher.pyx":324
  * 
- * def argon2i_32(nb_blocks, nb_iterations, password, salt, key=None, ad=None):
+ * def argon2i_32(nb_blocks, nb_iterations, password, salt, key=None, ad=None) -> bytes:
  *     key = b'' if key is None else key             # <<<<<<<<<<<<<<
  *     ad = b'' if ad is None else ad
  * 
  */
   __pyx_t_2 = (__pyx_v_key == Py_None);
   if (__pyx_t_2) {
     __Pyx_INCREF(__pyx_kp_b__4);
@@ -6919,16 +7071,16 @@
   } else {
     __Pyx_INCREF(__pyx_v_key);
     __pyx_t_1 = __pyx_v_key;
   }
   __Pyx_DECREF_SET(__pyx_v_key, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "monocypher.pyx":319
- * def argon2i_32(nb_blocks, nb_iterations, password, salt, key=None, ad=None):
+  /* "monocypher.pyx":325
+ * def argon2i_32(nb_blocks, nb_iterations, password, salt, key=None, ad=None) -> bytes:
  *     key = b'' if key is None else key
  *     ad = b'' if ad is None else ad             # <<<<<<<<<<<<<<
  * 
  *     cdef crypto_argon2_config config;
  */
   __pyx_t_2 = (__pyx_v_ad == Py_None);
   if (__pyx_t_2) {
@@ -6937,181 +7089,194 @@
   } else {
     __Pyx_INCREF(__pyx_v_ad);
     __pyx_t_1 = __pyx_v_ad;
   }
   __Pyx_DECREF_SET(__pyx_v_ad, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "monocypher.pyx":322
+  /* "monocypher.pyx":328
  * 
  *     cdef crypto_argon2_config config;
  *     config.algorithm = 1             # <<<<<<<<<<<<<<
  *     config.nb_block = nb_blocks
  *     config.nb_passes = nb_iterations
  */
   __pyx_v_config.algorithm = 1;
 
-  /* "monocypher.pyx":323
+  /* "monocypher.pyx":329
  *     cdef crypto_argon2_config config;
  *     config.algorithm = 1
  *     config.nb_block = nb_blocks             # <<<<<<<<<<<<<<
  *     config.nb_passes = nb_iterations
  *     config.nb_lanes = 1
  */
-  __pyx_t_1 = __pyx_convert__to_py_crypto_argon2_config(__pyx_v_config); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 323, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert__to_py_crypto_argon2_config(__pyx_v_config); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 329, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_t_1, __pyx_n_s_nb_block, __pyx_v_nb_blocks) < 0) __PYX_ERR(0, 323, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_t_1, __pyx_n_s_nb_block, __pyx_v_nb_blocks) < 0) __PYX_ERR(0, 329, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "monocypher.pyx":324
+  /* "monocypher.pyx":330
  *     config.algorithm = 1
  *     config.nb_block = nb_blocks
  *     config.nb_passes = nb_iterations             # <<<<<<<<<<<<<<
  *     config.nb_lanes = 1
  * 
  */
-  __pyx_t_3 = __Pyx_PyInt_As_uint32_t(__pyx_v_nb_iterations); if (unlikely((__pyx_t_3 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 324, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_As_uint32_t(__pyx_v_nb_iterations); if (unlikely((__pyx_t_3 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 330, __pyx_L1_error)
   __pyx_v_config.nb_passes = __pyx_t_3;
 
-  /* "monocypher.pyx":325
+  /* "monocypher.pyx":331
  *     config.nb_block = nb_blocks
  *     config.nb_passes = nb_iterations
  *     config.nb_lanes = 1             # <<<<<<<<<<<<<<
  * 
  *     cdef crypto_argon2_inputs inputs;
  */
   __pyx_v_config.nb_lanes = 1;
 
-  /* "monocypher.pyx":328
+  /* "monocypher.pyx":334
  * 
  *     cdef crypto_argon2_inputs inputs;
  *     inputs.pass_ = password             # <<<<<<<<<<<<<<
- *     inputs.pass_size = len(password)
+ *     inputs.pass_size = _validate_u32('password', len(password))
  *     inputs.salt = salt
  */
-  __pyx_t_4 = __Pyx_PyObject_AsUString(__pyx_v_password); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 328, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_AsUString(__pyx_v_password); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 334, __pyx_L1_error)
   __pyx_v_inputs.pass = __pyx_t_4;
 
-  /* "monocypher.pyx":329
+  /* "monocypher.pyx":335
  *     cdef crypto_argon2_inputs inputs;
  *     inputs.pass_ = password
- *     inputs.pass_size = len(password)             # <<<<<<<<<<<<<<
+ *     inputs.pass_size = _validate_u32('password', len(password))             # <<<<<<<<<<<<<<
  *     inputs.salt = salt
- *     inputs.salt_size = len(salt)
+ *     inputs.salt_size = _validate_u32('salt', len(salt))
  */
-  __pyx_t_5 = PyObject_Length(__pyx_v_password); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 329, __pyx_L1_error)
-  __pyx_v_inputs.pass_size = __pyx_t_5;
+  __pyx_t_5 = PyObject_Length(__pyx_v_password); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 335, __pyx_L1_error)
+  __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 335, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_3 = __pyx_f_10monocypher__validate_u32(__pyx_n_u_password, __pyx_t_1); if (unlikely(__pyx_t_3 == ((uint32_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 335, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v_inputs.pass_size = __pyx_t_3;
 
-  /* "monocypher.pyx":330
+  /* "monocypher.pyx":336
  *     inputs.pass_ = password
- *     inputs.pass_size = len(password)
+ *     inputs.pass_size = _validate_u32('password', len(password))
  *     inputs.salt = salt             # <<<<<<<<<<<<<<
- *     inputs.salt_size = len(salt)
+ *     inputs.salt_size = _validate_u32('salt', len(salt))
  * 
  */
-  __pyx_t_6 = __Pyx_PyObject_AsUString(__pyx_v_salt); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 330, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_AsUString(__pyx_v_salt); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 336, __pyx_L1_error)
   __pyx_v_inputs.salt = __pyx_t_6;
 
-  /* "monocypher.pyx":331
- *     inputs.pass_size = len(password)
+  /* "monocypher.pyx":337
+ *     inputs.pass_size = _validate_u32('password', len(password))
  *     inputs.salt = salt
- *     inputs.salt_size = len(salt)             # <<<<<<<<<<<<<<
+ *     inputs.salt_size = _validate_u32('salt', len(salt))             # <<<<<<<<<<<<<<
  * 
  *     cdef crypto_argon2_extras extras;
  */
-  __pyx_t_5 = PyObject_Length(__pyx_v_salt); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 331, __pyx_L1_error)
-  __pyx_v_inputs.salt_size = __pyx_t_5;
+  __pyx_t_5 = PyObject_Length(__pyx_v_salt); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 337, __pyx_L1_error)
+  __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 337, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_3 = __pyx_f_10monocypher__validate_u32(__pyx_n_u_salt, __pyx_t_1); if (unlikely(__pyx_t_3 == ((uint32_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 337, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v_inputs.salt_size = __pyx_t_3;
 
-  /* "monocypher.pyx":334
+  /* "monocypher.pyx":340
  * 
  *     cdef crypto_argon2_extras extras;
  *     extras.key = key             # <<<<<<<<<<<<<<
- *     extras.key_size = len(key)
+ *     extras.key_size = _validate_u32('key', len(key))
  *     extras.ad = ad
  */
-  __pyx_t_7 = __Pyx_PyObject_AsUString(__pyx_v_key); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 334, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_AsUString(__pyx_v_key); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 340, __pyx_L1_error)
   __pyx_v_extras.key = __pyx_t_7;
 
-  /* "monocypher.pyx":335
+  /* "monocypher.pyx":341
  *     cdef crypto_argon2_extras extras;
  *     extras.key = key
- *     extras.key_size = len(key)             # <<<<<<<<<<<<<<
+ *     extras.key_size = _validate_u32('key', len(key))             # <<<<<<<<<<<<<<
  *     extras.ad = ad
- *     extras.ad_size = len(ad)
+ *     extras.ad_size = _validate_u32('ad', len(ad))
  */
-  __pyx_t_5 = PyObject_Length(__pyx_v_key); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 335, __pyx_L1_error)
-  __pyx_v_extras.key_size = __pyx_t_5;
+  __pyx_t_5 = PyObject_Length(__pyx_v_key); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 341, __pyx_L1_error)
+  __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 341, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_3 = __pyx_f_10monocypher__validate_u32(__pyx_n_u_key, __pyx_t_1); if (unlikely(__pyx_t_3 == ((uint32_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 341, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v_extras.key_size = __pyx_t_3;
 
-  /* "monocypher.pyx":336
+  /* "monocypher.pyx":342
  *     extras.key = key
- *     extras.key_size = len(key)
+ *     extras.key_size = _validate_u32('key', len(key))
  *     extras.ad = ad             # <<<<<<<<<<<<<<
- *     extras.ad_size = len(ad)
+ *     extras.ad_size = _validate_u32('ad', len(ad))
  * 
  */
-  __pyx_t_8 = __Pyx_PyObject_AsUString(__pyx_v_ad); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 336, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_AsUString(__pyx_v_ad); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 342, __pyx_L1_error)
   __pyx_v_extras.ad = __pyx_t_8;
 
-  /* "monocypher.pyx":337
- *     extras.key_size = len(key)
+  /* "monocypher.pyx":343
+ *     extras.key_size = _validate_u32('key', len(key))
  *     extras.ad = ad
- *     extras.ad_size = len(ad)             # <<<<<<<<<<<<<<
+ *     extras.ad_size = _validate_u32('ad', len(ad))             # <<<<<<<<<<<<<<
  * 
  *     hash = bytes(32)
  */
-  __pyx_t_5 = PyObject_Length(__pyx_v_ad); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 337, __pyx_L1_error)
-  __pyx_v_extras.ad_size = __pyx_t_5;
+  __pyx_t_5 = PyObject_Length(__pyx_v_ad); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 343, __pyx_L1_error)
+  __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 343, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_3 = __pyx_f_10monocypher__validate_u32(__pyx_n_u_ad, __pyx_t_1); if (unlikely(__pyx_t_3 == ((uint32_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 343, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v_extras.ad_size = __pyx_t_3;
 
-  /* "monocypher.pyx":339
- *     extras.ad_size = len(ad)
+  /* "monocypher.pyx":345
+ *     extras.ad_size = _validate_u32('ad', len(ad))
  * 
  *     hash = bytes(32)             # <<<<<<<<<<<<<<
- *     work_area = malloc(nb_blocks * 1024)
+ *     work_area = malloc((<size_t> nb_blocks) * (<size_t> 1024))
  *     try:
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 339, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 345, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_hash = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "monocypher.pyx":340
+  /* "monocypher.pyx":346
  * 
  *     hash = bytes(32)
- *     work_area = malloc(nb_blocks * 1024)             # <<<<<<<<<<<<<<
+ *     work_area = malloc((<size_t> nb_blocks) * (<size_t> 1024))             # <<<<<<<<<<<<<<
  *     try:
  *         crypto_argon2(hash, <uint32_t> len(hash), work_area, config, inputs, extras)
  */
-  __pyx_t_1 = __Pyx_PyInt_MultiplyObjC(__pyx_v_nb_blocks, __pyx_int_1024, 0x400, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 340, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_9 = __Pyx_PyInt_As_size_t(__pyx_t_1); if (unlikely((__pyx_t_9 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 340, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v_work_area = malloc(__pyx_t_9);
+  __pyx_t_9 = __Pyx_PyInt_As_size_t(__pyx_v_nb_blocks); if (unlikely((__pyx_t_9 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 346, __pyx_L1_error)
+  __pyx_v_work_area = malloc((((size_t)__pyx_t_9) * ((size_t)0x400)));
 
-  /* "monocypher.pyx":341
+  /* "monocypher.pyx":347
  *     hash = bytes(32)
- *     work_area = malloc(nb_blocks * 1024)
+ *     work_area = malloc((<size_t> nb_blocks) * (<size_t> 1024))
  *     try:             # <<<<<<<<<<<<<<
  *         crypto_argon2(hash, <uint32_t> len(hash), work_area, config, inputs, extras)
  *     finally:
  */
   /*try:*/ {
 
-    /* "monocypher.pyx":342
- *     work_area = malloc(nb_blocks * 1024)
+    /* "monocypher.pyx":348
+ *     work_area = malloc((<size_t> nb_blocks) * (<size_t> 1024))
  *     try:
  *         crypto_argon2(hash, <uint32_t> len(hash), work_area, config, inputs, extras)             # <<<<<<<<<<<<<<
  *     finally:
  *         free(work_area)
  */
-    __pyx_t_10 = __Pyx_PyBytes_AsWritableUString(__pyx_v_hash); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 342, __pyx_L4_error)
-    __pyx_t_5 = __Pyx_PyBytes_GET_SIZE(__pyx_v_hash); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 342, __pyx_L4_error)
+    __pyx_t_10 = __Pyx_PyBytes_AsWritableUString(__pyx_v_hash); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 348, __pyx_L4_error)
+    __pyx_t_5 = __Pyx_PyBytes_GET_SIZE(__pyx_v_hash); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 348, __pyx_L4_error)
     crypto_argon2(__pyx_t_10, ((uint32_t)__pyx_t_5), __pyx_v_work_area, __pyx_v_config, __pyx_v_inputs, __pyx_v_extras);
   }
 
-  /* "monocypher.pyx":344
+  /* "monocypher.pyx":350
  *         crypto_argon2(hash, <uint32_t> len(hash), work_area, config, inputs, extras)
  *     finally:
  *         free(work_area)             # <<<<<<<<<<<<<<
  *     crypto_wipe(password, len(password))
  *     return hash
  */
   /*finally:*/ {
@@ -7150,41 +7315,41 @@
       __pyx_t_14 = 0; __pyx_t_15 = 0; __pyx_t_16 = 0; __pyx_t_17 = 0; __pyx_t_18 = 0; __pyx_t_19 = 0;
       __pyx_lineno = __pyx_t_11; __pyx_clineno = __pyx_t_12; __pyx_filename = __pyx_t_13;
       goto __pyx_L1_error;
     }
     __pyx_L5:;
   }
 
-  /* "monocypher.pyx":345
+  /* "monocypher.pyx":351
  *     finally:
  *         free(work_area)
  *     crypto_wipe(password, len(password))             # <<<<<<<<<<<<<<
  *     return hash
  * 
  */
-  __pyx_t_10 = __Pyx_PyObject_AsWritableUString(__pyx_v_password); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 345, __pyx_L1_error)
-  __pyx_t_5 = PyObject_Length(__pyx_v_password); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 345, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_AsWritableUString(__pyx_v_password); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 351, __pyx_L1_error)
+  __pyx_t_5 = PyObject_Length(__pyx_v_password); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 351, __pyx_L1_error)
   crypto_wipe(__pyx_t_10, __pyx_t_5);
 
-  /* "monocypher.pyx":346
+  /* "monocypher.pyx":352
  *         free(work_area)
  *     crypto_wipe(password, len(password))
  *     return hash             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_hash);
   __pyx_r = __pyx_v_hash;
   goto __pyx_L0;
 
-  /* "monocypher.pyx":317
+  /* "monocypher.pyx":323
  * 
  * 
- * def argon2i_32(nb_blocks, nb_iterations, password, salt, key=None, ad=None):             # <<<<<<<<<<<<<<
+ * def argon2i_32(nb_blocks, nb_iterations, password, salt, key=None, ad=None) -> bytes:             # <<<<<<<<<<<<<<
  *     key = b'' if key is None else key
  *     ad = b'' if ad is None else ad
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -7195,18 +7360,18 @@
   __Pyx_XDECREF(__pyx_v_key);
   __Pyx_XDECREF(__pyx_v_ad);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "monocypher.pyx":349
+/* "monocypher.pyx":355
  * 
  * 
- * def compute_key_exchange_public_key(secret_key):             # <<<<<<<<<<<<<<
+ * def compute_key_exchange_public_key(secret_key: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     """Generate the public key for key exchange from the secret key.
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_10monocypher_13compute_key_exchange_public_key(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
@@ -7257,47 +7422,52 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_secret_key)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 349, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 355, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "compute_key_exchange_public_key") < 0)) __PYX_ERR(0, 349, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "compute_key_exchange_public_key") < 0)) __PYX_ERR(0, 355, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
-    __pyx_v_secret_key = values[0];
+    __pyx_v_secret_key = ((PyObject*)values[0]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("compute_key_exchange_public_key", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 349, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("compute_key_exchange_public_key", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 355, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("monocypher.compute_key_exchange_public_key", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_secret_key), (&PyBytes_Type), 0, "secret_key", 1))) __PYX_ERR(0, 355, __pyx_L1_error)
   __pyx_r = __pyx_pf_10monocypher_12compute_key_exchange_public_key(__pyx_self, __pyx_v_secret_key);
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
@@ -7312,53 +7482,53 @@
   uint8_t *__pyx_t_2;
   uint8_t const *__pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("compute_key_exchange_public_key", 1);
 
-  /* "monocypher.pyx":355
+  /* "monocypher.pyx":361
  *     :return: The 32-byte public key for :func:`key_exchange`.
  *     """
  *     public_key = bytes(32)             # <<<<<<<<<<<<<<
  *     crypto_x25519_public_key(public_key, secret_key)
  *     return public_key
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 355, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 361, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_public_key = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "monocypher.pyx":356
+  /* "monocypher.pyx":362
  *     """
  *     public_key = bytes(32)
  *     crypto_x25519_public_key(public_key, secret_key)             # <<<<<<<<<<<<<<
  *     return public_key
  * 
  */
-  __pyx_t_2 = __Pyx_PyBytes_AsWritableUString(__pyx_v_public_key); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 356, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyObject_AsUString(__pyx_v_secret_key); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(0, 356, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBytes_AsWritableUString(__pyx_v_public_key); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 362, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyBytes_AsUString(__pyx_v_secret_key); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(0, 362, __pyx_L1_error)
   crypto_x25519_public_key(__pyx_t_2, __pyx_t_3);
 
-  /* "monocypher.pyx":357
+  /* "monocypher.pyx":363
  *     public_key = bytes(32)
  *     crypto_x25519_public_key(public_key, secret_key)
  *     return public_key             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_public_key);
   __pyx_r = __pyx_v_public_key;
   goto __pyx_L0;
 
-  /* "monocypher.pyx":349
+  /* "monocypher.pyx":355
  * 
  * 
- * def compute_key_exchange_public_key(secret_key):             # <<<<<<<<<<<<<<
+ * def compute_key_exchange_public_key(secret_key: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     """Generate the public key for key exchange from the secret key.
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -7367,18 +7537,18 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_public_key);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "monocypher.pyx":360
+/* "monocypher.pyx":366
  * 
  * 
- * def key_exchange(your_secret_key, their_public_key):             # <<<<<<<<<<<<<<
+ * def key_exchange(your_secret_key: bytes, their_public_key: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     """Compute a shared secret based upon public-key crytography.
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_10monocypher_15key_exchange(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
@@ -7432,59 +7602,65 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_your_secret_key)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 360, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 366, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_their_public_key)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 360, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 366, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("key_exchange", 1, 2, 2, 1); __PYX_ERR(0, 360, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("key_exchange", 1, 2, 2, 1); __PYX_ERR(0, 366, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "key_exchange") < 0)) __PYX_ERR(0, 360, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "key_exchange") < 0)) __PYX_ERR(0, 366, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
-    __pyx_v_your_secret_key = values[0];
-    __pyx_v_their_public_key = values[1];
+    __pyx_v_your_secret_key = ((PyObject*)values[0]);
+    __pyx_v_their_public_key = ((PyObject*)values[1]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("key_exchange", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 360, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("key_exchange", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 366, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("monocypher.key_exchange", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_your_secret_key), (&PyBytes_Type), 0, "your_secret_key", 1))) __PYX_ERR(0, 366, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_their_public_key), (&PyBytes_Type), 0, "their_public_key", 1))) __PYX_ERR(0, 366, __pyx_L1_error)
   __pyx_r = __pyx_pf_10monocypher_14key_exchange(__pyx_self, __pyx_v_your_secret_key, __pyx_v_their_public_key);
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
@@ -7500,54 +7676,54 @@
   uint8_t const *__pyx_t_3;
   uint8_t const *__pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("key_exchange", 1);
 
-  /* "monocypher.pyx":368
+  /* "monocypher.pyx":374
  *         computed using their_secret_key and your_public_key.
  *     """
  *     p = bytes(32)             # <<<<<<<<<<<<<<
  *     crypto_x25519(p, your_secret_key, their_public_key)
  *     return p
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 368, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 374, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_p = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "monocypher.pyx":369
+  /* "monocypher.pyx":375
  *     """
  *     p = bytes(32)
  *     crypto_x25519(p, your_secret_key, their_public_key)             # <<<<<<<<<<<<<<
  *     return p
  * 
  */
-  __pyx_t_2 = __Pyx_PyBytes_AsWritableUString(__pyx_v_p); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 369, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyObject_AsUString(__pyx_v_your_secret_key); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(0, 369, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_AsUString(__pyx_v_their_public_key); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 369, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBytes_AsWritableUString(__pyx_v_p); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 375, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyBytes_AsUString(__pyx_v_your_secret_key); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(0, 375, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyBytes_AsUString(__pyx_v_their_public_key); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 375, __pyx_L1_error)
   crypto_x25519(__pyx_t_2, __pyx_t_3, __pyx_t_4);
 
-  /* "monocypher.pyx":370
+  /* "monocypher.pyx":376
  *     p = bytes(32)
  *     crypto_x25519(p, your_secret_key, their_public_key)
  *     return p             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_p);
   __pyx_r = __pyx_v_p;
   goto __pyx_L0;
 
-  /* "monocypher.pyx":360
+  /* "monocypher.pyx":366
  * 
  * 
- * def key_exchange(your_secret_key, their_public_key):             # <<<<<<<<<<<<<<
+ * def key_exchange(your_secret_key: bytes, their_public_key: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     """Compute a shared secret based upon public-key crytography.
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -7556,31 +7732,31 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_p);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "monocypher.pyx":373
+/* "monocypher.pyx":379
  * 
  * 
- * def compute_signing_public_key(secret_key):             # <<<<<<<<<<<<<<
+ * def compute_signing_public_key(secret_key: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     """Generate the public key from the secret key.
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_10monocypher_17compute_signing_public_key(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_10monocypher_16compute_signing_public_key, "Generate the public key from the secret key.\n\n    :param secret_key: The 32-byte secret key.\n    :return: The 32-byte public key.\n    ");
+PyDoc_STRVAR(__pyx_doc_10monocypher_16compute_signing_public_key, "Generate the public key from the secret key.\n\n    :param secret_key: The 64-byte secret key from generate_signing_key_pair.\n    :return: The 32-byte public key.\n    ");
 static PyMethodDef __pyx_mdef_10monocypher_17compute_signing_public_key = {"compute_signing_public_key", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_10monocypher_17compute_signing_public_key, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_10monocypher_16compute_signing_public_key};
 static PyObject *__pyx_pw_10monocypher_17compute_signing_public_key(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
@@ -7618,103 +7794,143 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_secret_key)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 373, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 379, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "compute_signing_public_key") < 0)) __PYX_ERR(0, 373, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "compute_signing_public_key") < 0)) __PYX_ERR(0, 379, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
-    __pyx_v_secret_key = values[0];
+    __pyx_v_secret_key = ((PyObject*)values[0]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("compute_signing_public_key", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 373, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("compute_signing_public_key", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 379, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("monocypher.compute_signing_public_key", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_secret_key), (&PyBytes_Type), 0, "secret_key", 1))) __PYX_ERR(0, 379, __pyx_L1_error)
   __pyx_r = __pyx_pf_10monocypher_16compute_signing_public_key(__pyx_self, __pyx_v_secret_key);
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_10monocypher_16compute_signing_public_key(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_secret_key) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
+  Py_ssize_t __pyx_t_1;
+  int __pyx_t_2;
+  PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("compute_signing_public_key", 1);
 
-  /* "monocypher.pyx":379
+  /* "monocypher.pyx":385
  *     :return: The 32-byte public key.
  *     """
+ *     if len(secret_key) != 64:             # <<<<<<<<<<<<<<
+ *         raise ValueError('secret key length invalid')
+ *     return secret_key[32:]
+ */
+  __pyx_t_1 = __Pyx_PyBytes_GET_SIZE(__pyx_v_secret_key); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 385, __pyx_L1_error)
+  __pyx_t_2 = (__pyx_t_1 != 64);
+  if (unlikely(__pyx_t_2)) {
+
+    /* "monocypher.pyx":386
+ *     """
+ *     if len(secret_key) != 64:
+ *         raise ValueError('secret key length invalid')             # <<<<<<<<<<<<<<
+ *     return secret_key[32:]
+ * 
+ */
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 386, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __PYX_ERR(0, 386, __pyx_L1_error)
+
+    /* "monocypher.pyx":385
+ *     :return: The 32-byte public key.
+ *     """
+ *     if len(secret_key) != 64:             # <<<<<<<<<<<<<<
+ *         raise ValueError('secret key length invalid')
+ *     return secret_key[32:]
+ */
+  }
+
+  /* "monocypher.pyx":387
+ *     if len(secret_key) != 64:
+ *         raise ValueError('secret key length invalid')
  *     return secret_key[32:]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_v_secret_key, 32, 0, NULL, NULL, &__pyx_slice__8, 1, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 379, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
+  __pyx_t_3 = PySequence_GetSlice(__pyx_v_secret_key, 32, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 387, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_r = ((PyObject*)__pyx_t_3);
+  __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "monocypher.pyx":373
+  /* "monocypher.pyx":379
  * 
  * 
- * def compute_signing_public_key(secret_key):             # <<<<<<<<<<<<<<
+ * def compute_signing_public_key(secret_key: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     """Generate the public key from the secret key.
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_3);
   __Pyx_AddTraceback("monocypher.compute_signing_public_key", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "monocypher.pyx":382
+/* "monocypher.pyx":390
  * 
  * 
- * def signature_sign(secret_key, message):             # <<<<<<<<<<<<<<
+ * def signature_sign(secret_key: bytes, message: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     """Cryptographically sign a messge.
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_10monocypher_19signature_sign(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
@@ -7768,59 +7984,65 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_secret_key)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 382, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 390, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_message)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 382, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 390, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("signature_sign", 1, 2, 2, 1); __PYX_ERR(0, 382, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("signature_sign", 1, 2, 2, 1); __PYX_ERR(0, 390, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "signature_sign") < 0)) __PYX_ERR(0, 382, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "signature_sign") < 0)) __PYX_ERR(0, 390, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
-    __pyx_v_secret_key = values[0];
-    __pyx_v_message = values[1];
+    __pyx_v_secret_key = ((PyObject*)values[0]);
+    __pyx_v_message = ((PyObject*)values[1]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("signature_sign", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 382, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("signature_sign", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 390, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("monocypher.signature_sign", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_secret_key), (&PyBytes_Type), 0, "secret_key", 1))) __PYX_ERR(0, 390, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_message), (&PyBytes_Type), 0, "message", 1))) __PYX_ERR(0, 390, __pyx_L1_error)
   __pyx_r = __pyx_pf_10monocypher_18signature_sign(__pyx_self, __pyx_v_secret_key, __pyx_v_message);
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
@@ -7837,55 +8059,55 @@
   uint8_t const *__pyx_t_4;
   Py_ssize_t __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("signature_sign", 1);
 
-  /* "monocypher.pyx":392
+  /* "monocypher.pyx":400
  *     https://pynacl.readthedocs.io/en/stable/signing/.
  *     """
  *     sig = bytes(64)             # <<<<<<<<<<<<<<
  *     crypto_eddsa_sign(sig, secret_key, message, len(message))
  *     return sig
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 392, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_sig = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "monocypher.pyx":393
+  /* "monocypher.pyx":401
  *     """
  *     sig = bytes(64)
  *     crypto_eddsa_sign(sig, secret_key, message, len(message))             # <<<<<<<<<<<<<<
  *     return sig
  * 
  */
-  __pyx_t_2 = __Pyx_PyBytes_AsWritableUString(__pyx_v_sig); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 393, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyObject_AsUString(__pyx_v_secret_key); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(0, 393, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_AsUString(__pyx_v_message); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 393, __pyx_L1_error)
-  __pyx_t_5 = PyObject_Length(__pyx_v_message); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 393, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBytes_AsWritableUString(__pyx_v_sig); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 401, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyBytes_AsUString(__pyx_v_secret_key); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(0, 401, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyBytes_AsUString(__pyx_v_message); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 401, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyBytes_GET_SIZE(__pyx_v_message); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 401, __pyx_L1_error)
   crypto_eddsa_sign(__pyx_t_2, __pyx_t_3, __pyx_t_4, __pyx_t_5);
 
-  /* "monocypher.pyx":394
+  /* "monocypher.pyx":402
  *     sig = bytes(64)
  *     crypto_eddsa_sign(sig, secret_key, message, len(message))
  *     return sig             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_sig);
   __pyx_r = __pyx_v_sig;
   goto __pyx_L0;
 
-  /* "monocypher.pyx":382
+  /* "monocypher.pyx":390
  * 
  * 
- * def signature_sign(secret_key, message):             # <<<<<<<<<<<<<<
+ * def signature_sign(secret_key: bytes, message: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     """Cryptographically sign a messge.
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -7894,18 +8116,18 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_sig);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "monocypher.pyx":397
+/* "monocypher.pyx":405
  * 
  * 
- * def signature_check(signature, public_key, message):             # <<<<<<<<<<<<<<
+ * def signature_check(signature, public_key, message) -> bool:             # <<<<<<<<<<<<<<
  *     """Verify the signature.
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_10monocypher_21signature_check(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
@@ -7962,55 +8184,55 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_signature)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 397, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 405, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_public_key)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 397, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 405, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("signature_check", 1, 3, 3, 1); __PYX_ERR(0, 397, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("signature_check", 1, 3, 3, 1); __PYX_ERR(0, 405, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_message)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 397, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 405, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("signature_check", 1, 3, 3, 2); __PYX_ERR(0, 397, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("signature_check", 1, 3, 3, 2); __PYX_ERR(0, 405, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "signature_check") < 0)) __PYX_ERR(0, 397, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "signature_check") < 0)) __PYX_ERR(0, 405, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 3)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
     }
     __pyx_v_signature = values[0];
     __pyx_v_public_key = values[1];
     __pyx_v_message = values[2];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("signature_check", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 397, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("signature_check", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 405, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -8042,36 +8264,36 @@
   Py_ssize_t __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("signature_check", 1);
 
-  /* "monocypher.pyx":407
+  /* "monocypher.pyx":415
  *         fails verification.
  *     """
  *     return 0 == crypto_eddsa_check(signature, public_key, message, len(message))             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_AsUString(__pyx_v_signature); if (unlikely((!__pyx_t_1) && PyErr_Occurred())) __PYX_ERR(0, 407, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_AsUString(__pyx_v_public_key); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 407, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyObject_AsUString(__pyx_v_message); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(0, 407, __pyx_L1_error)
-  __pyx_t_4 = PyObject_Length(__pyx_v_message); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 407, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyBool_FromLong((0 == crypto_eddsa_check(__pyx_t_1, __pyx_t_2, __pyx_t_3, __pyx_t_4))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 407, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_AsUString(__pyx_v_signature); if (unlikely((!__pyx_t_1) && PyErr_Occurred())) __PYX_ERR(0, 415, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_AsUString(__pyx_v_public_key); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 415, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_AsUString(__pyx_v_message); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(0, 415, __pyx_L1_error)
+  __pyx_t_4 = PyObject_Length(__pyx_v_message); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 415, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyBool_FromLong((0 == crypto_eddsa_check(__pyx_t_1, __pyx_t_2, __pyx_t_3, __pyx_t_4))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 415, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "monocypher.pyx":397
+  /* "monocypher.pyx":405
  * 
  * 
- * def signature_check(signature, public_key, message):             # <<<<<<<<<<<<<<
+ * def signature_check(signature, public_key, message) -> bool:             # <<<<<<<<<<<<<<
  *     """Verify the signature.
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_5);
@@ -8079,31 +8301,31 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "monocypher.pyx":410
+/* "monocypher.pyx":418
  * 
  * 
- * def generate_key(length=None, method=None):             # <<<<<<<<<<<<<<
+ * def generate_key(length=None, method=None) -> bytes:             # <<<<<<<<<<<<<<
  *     """Generate a random key.
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_10monocypher_23generate_key(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_10monocypher_22generate_key, "Generate a random key.\n\n    :param length: The key length.  None (default) is equivalent to 32.\n    :param method: The random number generation method which is one of:\n        * 'os': Use the platform's random number generator directly\n        * 'chacha20': Apply the ChaCha20 cipher to the platform's random\n          number generator to increase entropy (does not improve randomness).\n        * None: (default) equivalent to 'chacha20'.\n    :return: A key that is as secure as the random number generator of\n        your platform.  See the Python secrets module for details on the\n        randomness (https://docs.python.org/3/library/secrets.html).\n    ");
+PyDoc_STRVAR(__pyx_doc_10monocypher_22generate_key, "Generate a random key.\n\n    :param length: The key length.  None (default) is equivalent to 32.\n    :param method: The random number generation method which is one of:\n        * 'os': Use the platform's random number generator directly\n        * 'chacha20': Apply the ChaCha20 cipher to the platform's random\n          number generator to increase entropy (does not improve randomness).\n        * None: (default) equivalent to 'chacha20'.\n    :return: A key that is as secure as the random number generator of\n        your platform.  See the Python secrets module for details on the\n        randomness (https://docs.python.org/3/library/secrets.html).\n    :see: generate_signing_key_pair, generate_key_exchange_key_pair, elligator_key_pair\n\n    You should probably use the *_key_pair function for your\n    specific crypto usage.\n    ");
 static PyMethodDef __pyx_mdef_10monocypher_23generate_key = {"generate_key", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_10monocypher_23generate_key, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_10monocypher_22generate_key};
 static PyObject *__pyx_pw_10monocypher_23generate_key(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
@@ -8145,27 +8367,27 @@
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_length);
           if (value) { values[0] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 410, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 418, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_method);
           if (value) { values[1] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 410, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 418, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "generate_key") < 0)) __PYX_ERR(0, 410, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "generate_key") < 0)) __PYX_ERR(0, 418, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
@@ -8174,15 +8396,15 @@
       }
     }
     __pyx_v_length = values[0];
     __pyx_v_method = values[1];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("generate_key", 0, 0, 2, __pyx_nargs); __PYX_ERR(0, 410, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("generate_key", 0, 0, 2, __pyx_nargs); __PYX_ERR(0, 418, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -8219,80 +8441,80 @@
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("generate_key", 0);
   __Pyx_INCREF(__pyx_v_length);
 
-  /* "monocypher.pyx":423
- *         randomness (https://docs.python.org/3/library/secrets.html).
+  /* "monocypher.pyx":435
+ *     specific crypto usage.
  *     """
  *     length = 32 if length is None else int(length)             # <<<<<<<<<<<<<<
  *     if method in ['chacha20', None, '', 'default']:
  *         # Do not entirely trust the platform's random number generator
  */
   __pyx_t_2 = (__pyx_v_length == Py_None);
   if (__pyx_t_2) {
     __Pyx_INCREF(__pyx_int_32);
     __pyx_t_1 = __pyx_int_32;
   } else {
-    __pyx_t_3 = __Pyx_PyNumber_Int(__pyx_v_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 423, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyNumber_Int(__pyx_v_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 435, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_1 = __pyx_t_3;
     __pyx_t_3 = 0;
   }
   __Pyx_DECREF_SET(__pyx_v_length, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "monocypher.pyx":424
+  /* "monocypher.pyx":436
  *     """
  *     length = 32 if length is None else int(length)
  *     if method in ['chacha20', None, '', 'default']:             # <<<<<<<<<<<<<<
  *         # Do not entirely trust the platform's random number generator
  *         key = secrets.token_bytes(32)
  */
   __Pyx_INCREF(__pyx_v_method);
   __pyx_t_1 = __pyx_v_method;
-  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_chacha20, Py_EQ)); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 424, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_chacha20, Py_EQ)); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 436, __pyx_L1_error)
   if (!__pyx_t_4) {
   } else {
     __pyx_t_2 = __pyx_t_4;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, Py_None, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 424, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 424, __pyx_L1_error)
+  __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, Py_None, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 436, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 436, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (!__pyx_t_4) {
   } else {
     __pyx_t_2 = __pyx_t_4;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_kp_u__4, Py_EQ)); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 424, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_kp_u__4, Py_EQ)); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 436, __pyx_L1_error)
   if (!__pyx_t_4) {
   } else {
     __pyx_t_2 = __pyx_t_4;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_default, Py_EQ)); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 424, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_default, Py_EQ)); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 436, __pyx_L1_error)
   __pyx_t_2 = __pyx_t_4;
   __pyx_L4_bool_binop_done:;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_4 = __pyx_t_2;
   if (__pyx_t_4) {
 
-    /* "monocypher.pyx":426
+    /* "monocypher.pyx":438
  *     if method in ['chacha20', None, '', 'default']:
  *         # Do not entirely trust the platform's random number generator
  *         key = secrets.token_bytes(32)             # <<<<<<<<<<<<<<
  *         nonce = secrets.token_bytes(24)
  *         message = secrets.token_bytes(length)
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_secrets); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 426, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_secrets); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 438, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_token_bytes); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 426, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_token_bytes); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 438, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     __pyx_t_6 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
@@ -8305,31 +8527,31 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_int_32};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 426, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 438, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __pyx_v_key = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "monocypher.pyx":427
+    /* "monocypher.pyx":439
  *         # Do not entirely trust the platform's random number generator
  *         key = secrets.token_bytes(32)
  *         nonce = secrets.token_bytes(24)             # <<<<<<<<<<<<<<
  *         message = secrets.token_bytes(length)
  *         key = chacha20(key, nonce, message)
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_secrets); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 427, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_secrets); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 439, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_token_bytes); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 427, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_token_bytes); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 439, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_5 = NULL;
     __pyx_t_6 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
@@ -8342,31 +8564,31 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_int_24};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 427, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 439, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __pyx_v_nonce = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "monocypher.pyx":428
+    /* "monocypher.pyx":440
  *         key = secrets.token_bytes(32)
  *         nonce = secrets.token_bytes(24)
  *         message = secrets.token_bytes(length)             # <<<<<<<<<<<<<<
  *         key = chacha20(key, nonce, message)
  *     elif method in ['os', 'secrets']:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_secrets); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 428, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_secrets); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 440, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_token_bytes); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 428, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_token_bytes); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 440, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     __pyx_t_6 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
@@ -8379,29 +8601,29 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_length};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 428, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 440, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __pyx_v_message = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "monocypher.pyx":429
+    /* "monocypher.pyx":441
  *         nonce = secrets.token_bytes(24)
  *         message = secrets.token_bytes(length)
  *         key = chacha20(key, nonce, message)             # <<<<<<<<<<<<<<
  *     elif method in ['os', 'secrets']:
  *         key = secrets.token_bytes(length)
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_chacha20); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 429, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_chacha20); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 441, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_3 = NULL;
     __pyx_t_6 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_3)) {
@@ -8413,63 +8635,63 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[4] = {__pyx_t_3, __pyx_v_key, __pyx_v_nonce, __pyx_v_message};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_6, 3+__pyx_t_6);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 429, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 441, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __Pyx_DECREF_SET(__pyx_v_key, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "monocypher.pyx":424
+    /* "monocypher.pyx":436
  *     """
  *     length = 32 if length is None else int(length)
  *     if method in ['chacha20', None, '', 'default']:             # <<<<<<<<<<<<<<
  *         # Do not entirely trust the platform's random number generator
  *         key = secrets.token_bytes(32)
  */
     goto __pyx_L3;
   }
 
-  /* "monocypher.pyx":430
+  /* "monocypher.pyx":442
  *         message = secrets.token_bytes(length)
  *         key = chacha20(key, nonce, message)
  *     elif method in ['os', 'secrets']:             # <<<<<<<<<<<<<<
  *         key = secrets.token_bytes(length)
  *     else:
  */
   __Pyx_INCREF(__pyx_v_method);
   __pyx_t_1 = __pyx_v_method;
-  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_os, Py_EQ)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 430, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_os, Py_EQ)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 442, __pyx_L1_error)
   if (!__pyx_t_2) {
   } else {
     __pyx_t_4 = __pyx_t_2;
     goto __pyx_L8_bool_binop_done;
   }
-  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_secrets, Py_EQ)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 430, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_secrets, Py_EQ)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 442, __pyx_L1_error)
   __pyx_t_4 = __pyx_t_2;
   __pyx_L8_bool_binop_done:;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_2 = __pyx_t_4;
   if (likely(__pyx_t_2)) {
 
-    /* "monocypher.pyx":431
+    /* "monocypher.pyx":443
  *         key = chacha20(key, nonce, message)
  *     elif method in ['os', 'secrets']:
  *         key = secrets.token_bytes(length)             # <<<<<<<<<<<<<<
  *     else:
  *         raise ValueError('unsupported method: %s' % method)
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_secrets); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 431, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_secrets); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 443, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_token_bytes); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 431, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_token_bytes); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 443, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_5 = NULL;
     __pyx_t_6 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
@@ -8482,66 +8704,67 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_v_length};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 431, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 443, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __pyx_v_key = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "monocypher.pyx":430
+    /* "monocypher.pyx":442
  *         message = secrets.token_bytes(length)
  *         key = chacha20(key, nonce, message)
  *     elif method in ['os', 'secrets']:             # <<<<<<<<<<<<<<
  *         key = secrets.token_bytes(length)
  *     else:
  */
     goto __pyx_L3;
   }
 
-  /* "monocypher.pyx":433
+  /* "monocypher.pyx":445
  *         key = secrets.token_bytes(length)
  *     else:
  *         raise ValueError('unsupported method: %s' % method)             # <<<<<<<<<<<<<<
  *     return key
  * 
  */
   /*else*/ {
-    __pyx_t_1 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_unsupported_method_s, __pyx_v_method); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 433, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_unsupported_method_s, __pyx_v_method); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 445, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 433, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 445, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 433, __pyx_L1_error)
+    __PYX_ERR(0, 445, __pyx_L1_error)
   }
   __pyx_L3:;
 
-  /* "monocypher.pyx":434
+  /* "monocypher.pyx":446
  *     else:
  *         raise ValueError('unsupported method: %s' % method)
  *     return key             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
+  if (!(likely(PyBytes_CheckExact(__pyx_v_key))||((__pyx_v_key) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_v_key))) __PYX_ERR(0, 446, __pyx_L1_error)
   __Pyx_INCREF(__pyx_v_key);
-  __pyx_r = __pyx_v_key;
+  __pyx_r = ((PyObject*)__pyx_v_key);
   goto __pyx_L0;
 
-  /* "monocypher.pyx":410
+  /* "monocypher.pyx":418
  * 
  * 
- * def generate_key(length=None, method=None):             # <<<<<<<<<<<<<<
+ * def generate_key(length=None, method=None) -> bytes:             # <<<<<<<<<<<<<<
  *     """Generate a random key.
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -8555,25 +8778,25 @@
   __Pyx_XDECREF(__pyx_v_message);
   __Pyx_XDECREF(__pyx_v_length);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "monocypher.pyx":437
+/* "monocypher.pyx":449
  * 
  * 
- * def generate_signing_key_pair():             # <<<<<<<<<<<<<<
+ * def generate_signing_key_pair() -> tuple[bytes, bytes]:             # <<<<<<<<<<<<<<
  *     """Generate a new keypair for signing using default settings.
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_10monocypher_25generate_signing_key_pair(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-PyDoc_STRVAR(__pyx_doc_10monocypher_24generate_signing_key_pair, "Generate a new keypair for signing using default settings.\n\n    :return (secret, public).\n\n    To print a key, use the following code snippet:\n\n        import binascii\n        print(binascii.hexlify(key))\n    ");
+PyDoc_STRVAR(__pyx_doc_10monocypher_24generate_signing_key_pair, "Generate a new keypair for signing using default settings.\n\n    :return: (secret, public)\n\n    To print a key, use the following code snippet:\n\n        import binascii\n        print(binascii.hexlify(key))\n    ");
 static PyMethodDef __pyx_mdef_10monocypher_25generate_signing_key_pair = {"generate_signing_key_pair", (PyCFunction)__pyx_pw_10monocypher_25generate_signing_key_pair, METH_NOARGS, __pyx_doc_10monocypher_24generate_signing_key_pair};
 static PyObject *__pyx_pw_10monocypher_25generate_signing_key_pair(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused) {
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("generate_signing_key_pair (wrapper)", 0);
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
@@ -8597,48 +8820,48 @@
   int __pyx_t_6;
   uint8_t *__pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("generate_signing_key_pair", 1);
 
-  /* "monocypher.pyx":447
+  /* "monocypher.pyx":459
  *         print(binascii.hexlify(key))
  *     """
  *     secret = bytes(64)             # <<<<<<<<<<<<<<
  *     public = bytes(32)
  *     crypto_eddsa_key_pair(secret, public, generate_key())
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 447, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 459, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_secret = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "monocypher.pyx":448
+  /* "monocypher.pyx":460
  *     """
  *     secret = bytes(64)
  *     public = bytes(32)             # <<<<<<<<<<<<<<
  *     crypto_eddsa_key_pair(secret, public, generate_key())
  *     return secret, public
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 448, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 460, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_public = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "monocypher.pyx":449
+  /* "monocypher.pyx":461
  *     secret = bytes(64)
  *     public = bytes(32)
  *     crypto_eddsa_key_pair(secret, public, generate_key())             # <<<<<<<<<<<<<<
  *     return secret, public
  * 
  */
-  __pyx_t_2 = __Pyx_PyBytes_AsWritableUString(__pyx_v_secret); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 449, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyBytes_AsWritableUString(__pyx_v_public); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(0, 449, __pyx_L1_error)
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_generate_key); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 449, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBytes_AsWritableUString(__pyx_v_secret); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 461, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyBytes_AsWritableUString(__pyx_v_public); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(0, 461, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_generate_key); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 461, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   __pyx_t_6 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
@@ -8650,46 +8873,46 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_5, NULL};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_6, 0+__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 449, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 461, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
-  __pyx_t_7 = __Pyx_PyObject_AsWritableUString(__pyx_t_1); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 449, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_AsWritableUString(__pyx_t_1); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 461, __pyx_L1_error)
   crypto_eddsa_key_pair(__pyx_t_2, __pyx_t_3, __pyx_t_7);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "monocypher.pyx":450
+  /* "monocypher.pyx":462
  *     public = bytes(32)
  *     crypto_eddsa_key_pair(secret, public, generate_key())
  *     return secret, public             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 450, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 462, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_secret);
   __Pyx_GIVEREF(__pyx_v_secret);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_secret)) __PYX_ERR(0, 450, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_secret)) __PYX_ERR(0, 462, __pyx_L1_error);
   __Pyx_INCREF(__pyx_v_public);
   __Pyx_GIVEREF(__pyx_v_public);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_public)) __PYX_ERR(0, 450, __pyx_L1_error);
-  __pyx_r = __pyx_t_1;
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_public)) __PYX_ERR(0, 462, __pyx_L1_error);
+  __pyx_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "monocypher.pyx":437
+  /* "monocypher.pyx":449
  * 
  * 
- * def generate_signing_key_pair():             # <<<<<<<<<<<<<<
+ * def generate_signing_key_pair() -> tuple[bytes, bytes]:             # <<<<<<<<<<<<<<
  *     """Generate a new keypair for signing using default settings.
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -8701,25 +8924,25 @@
   __Pyx_XDECREF(__pyx_v_secret);
   __Pyx_XDECREF(__pyx_v_public);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "monocypher.pyx":453
+/* "monocypher.pyx":465
  * 
  * 
- * def generate_key_exchange_key_pair():             # <<<<<<<<<<<<<<
+ * def generate_key_exchange_key_pair() -> tuple[bytes, bytes]:             # <<<<<<<<<<<<<<
  *     """Generate a new keypair for key exchange using default settings.
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_10monocypher_27generate_key_exchange_key_pair(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-PyDoc_STRVAR(__pyx_doc_10monocypher_26generate_key_exchange_key_pair, "Generate a new keypair for key exchange using default settings.\n\n    :return (secret, public).\n    ");
+PyDoc_STRVAR(__pyx_doc_10monocypher_26generate_key_exchange_key_pair, "Generate a new keypair for key exchange using default settings.\n\n    :return: (secret, public)\n    ");
 static PyMethodDef __pyx_mdef_10monocypher_27generate_key_exchange_key_pair = {"generate_key_exchange_key_pair", (PyCFunction)__pyx_pw_10monocypher_27generate_key_exchange_key_pair, METH_NOARGS, __pyx_doc_10monocypher_26generate_key_exchange_key_pair};
 static PyObject *__pyx_pw_10monocypher_27generate_key_exchange_key_pair(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused) {
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("generate_key_exchange_key_pair (wrapper)", 0);
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
@@ -8740,22 +8963,22 @@
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("generate_key_exchange_key_pair", 1);
 
-  /* "monocypher.pyx":458
- *     :return (secret, public).
+  /* "monocypher.pyx":470
+ *     :return: (secret, public)
  *     """
  *     secret = generate_key()             # <<<<<<<<<<<<<<
  *     public = compute_key_exchange_public_key(secret)
  *     return secret, public
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_generate_key); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 458, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_generate_key); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 470, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
@@ -8767,29 +8990,29 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 458, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 470, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_v_secret = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "monocypher.pyx":459
+  /* "monocypher.pyx":471
  *     """
  *     secret = generate_key()
  *     public = compute_key_exchange_public_key(secret)             # <<<<<<<<<<<<<<
  *     return secret, public
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_compute_key_exchange_public_key); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 459, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_compute_key_exchange_public_key); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 471, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
@@ -8801,45 +9024,45 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_secret};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 459, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 471, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_v_public = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "monocypher.pyx":460
+  /* "monocypher.pyx":472
  *     secret = generate_key()
  *     public = compute_key_exchange_public_key(secret)
  *     return secret, public             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 460, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 472, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_secret);
   __Pyx_GIVEREF(__pyx_v_secret);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_secret)) __PYX_ERR(0, 460, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_secret)) __PYX_ERR(0, 472, __pyx_L1_error);
   __Pyx_INCREF(__pyx_v_public);
   __Pyx_GIVEREF(__pyx_v_public);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_public)) __PYX_ERR(0, 460, __pyx_L1_error);
-  __pyx_r = __pyx_t_1;
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_public)) __PYX_ERR(0, 472, __pyx_L1_error);
+  __pyx_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "monocypher.pyx":453
+  /* "monocypher.pyx":465
  * 
  * 
- * def generate_key_exchange_key_pair():             # <<<<<<<<<<<<<<
+ * def generate_key_exchange_key_pair() -> tuple[bytes, bytes]:             # <<<<<<<<<<<<<<
  *     """Generate a new keypair for key exchange using default settings.
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -8851,15 +9074,15 @@
   __Pyx_XDECREF(__pyx_v_secret);
   __Pyx_XDECREF(__pyx_v_public);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "monocypher.pyx":466
+/* "monocypher.pyx":478
  * 
  * 
  * def elligator_map(hidden: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     """Computes the point corresponding to a representative.
  * 
  */
 
@@ -8913,45 +9136,45 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_hidden)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 466, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 478, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "elligator_map") < 0)) __PYX_ERR(0, 466, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "elligator_map") < 0)) __PYX_ERR(0, 478, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_hidden = ((PyObject*)values[0]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("elligator_map", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 466, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("elligator_map", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 478, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("monocypher.elligator_map", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_hidden), (&PyBytes_Type), 0, "hidden", 1))) __PYX_ERR(0, 466, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_hidden), (&PyBytes_Type), 0, "hidden", 1))) __PYX_ERR(0, 478, __pyx_L1_error)
   __pyx_r = __pyx_pf_10monocypher_28elligator_map(__pyx_self, __pyx_v_hidden);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -8978,106 +9201,106 @@
   uint8_t *__pyx_t_7;
   uint8_t const *__pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("elligator_map", 1);
 
-  /* "monocypher.pyx":474
+  /* "monocypher.pyx":486
  *         the two most significant bits are ignored.
  *     """
  *     curve = bytes(32)             # <<<<<<<<<<<<<<
  *     if len(hidden) != 32:
  *         raise ValueError(f'Invalid hidden length {len(hidden)} != 32')
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 474, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 486, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_curve = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "monocypher.pyx":475
+  /* "monocypher.pyx":487
  *     """
  *     curve = bytes(32)
  *     if len(hidden) != 32:             # <<<<<<<<<<<<<<
  *         raise ValueError(f'Invalid hidden length {len(hidden)} != 32')
  *     crypto_elligator_map(curve, hidden)
  */
-  __pyx_t_2 = __Pyx_PyBytes_GET_SIZE(__pyx_v_hidden); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 475, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBytes_GET_SIZE(__pyx_v_hidden); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 487, __pyx_L1_error)
   __pyx_t_3 = (__pyx_t_2 != 32);
   if (unlikely(__pyx_t_3)) {
 
-    /* "monocypher.pyx":476
+    /* "monocypher.pyx":488
  *     curve = bytes(32)
  *     if len(hidden) != 32:
  *         raise ValueError(f'Invalid hidden length {len(hidden)} != 32')             # <<<<<<<<<<<<<<
  *     crypto_elligator_map(curve, hidden)
  *     return curve
  */
-    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 476, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 488, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_2 = 0;
     __pyx_t_4 = 127;
     __Pyx_INCREF(__pyx_kp_u_Invalid_hidden_length);
     __pyx_t_2 += 22;
     __Pyx_GIVEREF(__pyx_kp_u_Invalid_hidden_length);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_Invalid_hidden_length);
-    __pyx_t_5 = __Pyx_PyBytes_GET_SIZE(__pyx_v_hidden); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 476, __pyx_L1_error)
-    __pyx_t_6 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_t_5, 0, ' ', 'd'); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 476, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyBytes_GET_SIZE(__pyx_v_hidden); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 488, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_t_5, 0, ' ', 'd'); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 488, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_6);
     __Pyx_GIVEREF(__pyx_t_6);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_6);
     __pyx_t_6 = 0;
     __Pyx_INCREF(__pyx_kp_u_32);
     __pyx_t_2 += 6;
     __Pyx_GIVEREF(__pyx_kp_u_32);
     PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u_32);
-    __pyx_t_6 = __Pyx_PyUnicode_Join(__pyx_t_1, 3, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 476, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyUnicode_Join(__pyx_t_1, 3, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 488, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 476, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 488, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 476, __pyx_L1_error)
+    __PYX_ERR(0, 488, __pyx_L1_error)
 
-    /* "monocypher.pyx":475
+    /* "monocypher.pyx":487
  *     """
  *     curve = bytes(32)
  *     if len(hidden) != 32:             # <<<<<<<<<<<<<<
  *         raise ValueError(f'Invalid hidden length {len(hidden)} != 32')
  *     crypto_elligator_map(curve, hidden)
  */
   }
 
-  /* "monocypher.pyx":477
+  /* "monocypher.pyx":489
  *     if len(hidden) != 32:
  *         raise ValueError(f'Invalid hidden length {len(hidden)} != 32')
  *     crypto_elligator_map(curve, hidden)             # <<<<<<<<<<<<<<
  *     return curve
  * 
  */
-  __pyx_t_7 = __Pyx_PyBytes_AsWritableUString(__pyx_v_curve); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 477, __pyx_L1_error)
-  __pyx_t_8 = __Pyx_PyBytes_AsUString(__pyx_v_hidden); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 477, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyBytes_AsWritableUString(__pyx_v_curve); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 489, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyBytes_AsUString(__pyx_v_hidden); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 489, __pyx_L1_error)
   crypto_elligator_map(__pyx_t_7, __pyx_t_8);
 
-  /* "monocypher.pyx":478
+  /* "monocypher.pyx":490
  *         raise ValueError(f'Invalid hidden length {len(hidden)} != 32')
  *     crypto_elligator_map(curve, hidden)
  *     return curve             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_curve);
   __pyx_r = __pyx_v_curve;
   goto __pyx_L0;
 
-  /* "monocypher.pyx":466
+  /* "monocypher.pyx":478
  * 
  * 
  * def elligator_map(hidden: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     """Computes the point corresponding to a representative.
  * 
  */
 
@@ -9090,15 +9313,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_curve);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "monocypher.pyx":481
+/* "monocypher.pyx":493
  * 
  * 
  * def elligator_rev(curve: bytes, tweak=None) -> bytes:             # <<<<<<<<<<<<<<
  *     """Computes the representative of a point.
  * 
  */
 
@@ -9156,27 +9379,27 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_curve)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 481, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 493, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_tweak);
           if (value) { values[1] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 481, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 493, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "elligator_rev") < 0)) __PYX_ERR(0, 481, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "elligator_rev") < 0)) __PYX_ERR(0, 493, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         break;
@@ -9184,29 +9407,29 @@
       }
     }
     __pyx_v_curve = ((PyObject*)values[0]);
     __pyx_v_tweak = values[1];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("elligator_rev", 0, 1, 2, __pyx_nargs); __PYX_ERR(0, 481, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("elligator_rev", 0, 1, 2, __pyx_nargs); __PYX_ERR(0, 493, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("monocypher.elligator_rev", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_curve), (&PyBytes_Type), 0, "curve", 1))) __PYX_ERR(0, 481, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_curve), (&PyBytes_Type), 0, "curve", 1))) __PYX_ERR(0, 493, __pyx_L1_error)
   __pyx_r = __pyx_pf_10monocypher_30elligator_rev(__pyx_self, __pyx_v_curve, __pyx_v_tweak);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -9238,102 +9461,102 @@
   uint8_t __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("elligator_rev", 0);
   __Pyx_INCREF(__pyx_v_tweak);
 
-  /* "monocypher.pyx":492
+  /* "monocypher.pyx":504
  *         and try again.
  *     """
  *     hidden = bytes(32)             # <<<<<<<<<<<<<<
  *     if len(curve) != 32:
  *         raise ValueError(f'Invalid curve length {len(curve)} != 32')
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 492, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 504, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_hidden = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "monocypher.pyx":493
+  /* "monocypher.pyx":505
  *     """
  *     hidden = bytes(32)
  *     if len(curve) != 32:             # <<<<<<<<<<<<<<
  *         raise ValueError(f'Invalid curve length {len(curve)} != 32')
  *     if tweak is None:
  */
-  __pyx_t_2 = __Pyx_PyBytes_GET_SIZE(__pyx_v_curve); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 493, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBytes_GET_SIZE(__pyx_v_curve); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 505, __pyx_L1_error)
   __pyx_t_3 = (__pyx_t_2 != 32);
   if (unlikely(__pyx_t_3)) {
 
-    /* "monocypher.pyx":494
+    /* "monocypher.pyx":506
  *     hidden = bytes(32)
  *     if len(curve) != 32:
  *         raise ValueError(f'Invalid curve length {len(curve)} != 32')             # <<<<<<<<<<<<<<
  *     if tweak is None:
  *         tweak = secrets.randbits(8)
  */
-    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 494, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 506, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_2 = 0;
     __pyx_t_4 = 127;
     __Pyx_INCREF(__pyx_kp_u_Invalid_curve_length);
     __pyx_t_2 += 21;
     __Pyx_GIVEREF(__pyx_kp_u_Invalid_curve_length);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_Invalid_curve_length);
-    __pyx_t_5 = __Pyx_PyBytes_GET_SIZE(__pyx_v_curve); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 494, __pyx_L1_error)
-    __pyx_t_6 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_t_5, 0, ' ', 'd'); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 494, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyBytes_GET_SIZE(__pyx_v_curve); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 506, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_t_5, 0, ' ', 'd'); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 506, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_6);
     __Pyx_GIVEREF(__pyx_t_6);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_6);
     __pyx_t_6 = 0;
     __Pyx_INCREF(__pyx_kp_u_32);
     __pyx_t_2 += 6;
     __Pyx_GIVEREF(__pyx_kp_u_32);
     PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u_32);
-    __pyx_t_6 = __Pyx_PyUnicode_Join(__pyx_t_1, 3, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 494, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyUnicode_Join(__pyx_t_1, 3, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 506, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 494, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 506, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 494, __pyx_L1_error)
+    __PYX_ERR(0, 506, __pyx_L1_error)
 
-    /* "monocypher.pyx":493
+    /* "monocypher.pyx":505
  *     """
  *     hidden = bytes(32)
  *     if len(curve) != 32:             # <<<<<<<<<<<<<<
  *         raise ValueError(f'Invalid curve length {len(curve)} != 32')
  *     if tweak is None:
  */
   }
 
-  /* "monocypher.pyx":495
+  /* "monocypher.pyx":507
  *     if len(curve) != 32:
  *         raise ValueError(f'Invalid curve length {len(curve)} != 32')
  *     if tweak is None:             # <<<<<<<<<<<<<<
  *         tweak = secrets.randbits(8)
  *     rv = crypto_elligator_rev(hidden, curve, tweak)
  */
   __pyx_t_3 = (__pyx_v_tweak == Py_None);
   if (__pyx_t_3) {
 
-    /* "monocypher.pyx":496
+    /* "monocypher.pyx":508
  *         raise ValueError(f'Invalid curve length {len(curve)} != 32')
  *     if tweak is None:
  *         tweak = secrets.randbits(8)             # <<<<<<<<<<<<<<
  *     rv = crypto_elligator_rev(hidden, curve, tweak)
  *     if rv:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_secrets); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 496, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_secrets); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 508, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_randbits); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 496, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_randbits); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 508, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_t_6 = NULL;
     __pyx_t_8 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_7))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_7);
@@ -9346,87 +9569,87 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_int_8};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 496, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 508, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
     __Pyx_DECREF_SET(__pyx_v_tweak, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "monocypher.pyx":495
+    /* "monocypher.pyx":507
  *     if len(curve) != 32:
  *         raise ValueError(f'Invalid curve length {len(curve)} != 32')
  *     if tweak is None:             # <<<<<<<<<<<<<<
  *         tweak = secrets.randbits(8)
  *     rv = crypto_elligator_rev(hidden, curve, tweak)
  */
   }
 
-  /* "monocypher.pyx":497
+  /* "monocypher.pyx":509
  *     if tweak is None:
  *         tweak = secrets.randbits(8)
  *     rv = crypto_elligator_rev(hidden, curve, tweak)             # <<<<<<<<<<<<<<
  *     if rv:
  *         raise ValueError('curve point is unsuitable for hiding')
  */
-  __pyx_t_9 = __Pyx_PyBytes_AsWritableUString(__pyx_v_hidden); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 497, __pyx_L1_error)
-  __pyx_t_10 = __Pyx_PyBytes_AsUString(__pyx_v_curve); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 497, __pyx_L1_error)
-  __pyx_t_11 = __Pyx_PyInt_As_uint8_t(__pyx_v_tweak); if (unlikely((__pyx_t_11 == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 497, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyBytes_AsWritableUString(__pyx_v_hidden); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 509, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyBytes_AsUString(__pyx_v_curve); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 509, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_As_uint8_t(__pyx_v_tweak); if (unlikely((__pyx_t_11 == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 509, __pyx_L1_error)
   __pyx_v_rv = crypto_elligator_rev(__pyx_t_9, __pyx_t_10, __pyx_t_11);
 
-  /* "monocypher.pyx":498
+  /* "monocypher.pyx":510
  *         tweak = secrets.randbits(8)
  *     rv = crypto_elligator_rev(hidden, curve, tweak)
  *     if rv:             # <<<<<<<<<<<<<<
  *         raise ValueError('curve point is unsuitable for hiding')
  *     return hidden
  */
   __pyx_t_3 = (__pyx_v_rv != 0);
   if (unlikely(__pyx_t_3)) {
 
-    /* "monocypher.pyx":499
+    /* "monocypher.pyx":511
  *     rv = crypto_elligator_rev(hidden, curve, tweak)
  *     if rv:
  *         raise ValueError('curve point is unsuitable for hiding')             # <<<<<<<<<<<<<<
  *     return hidden
  * 
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 499, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 511, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 499, __pyx_L1_error)
+    __PYX_ERR(0, 511, __pyx_L1_error)
 
-    /* "monocypher.pyx":498
+    /* "monocypher.pyx":510
  *         tweak = secrets.randbits(8)
  *     rv = crypto_elligator_rev(hidden, curve, tweak)
  *     if rv:             # <<<<<<<<<<<<<<
  *         raise ValueError('curve point is unsuitable for hiding')
  *     return hidden
  */
   }
 
-  /* "monocypher.pyx":500
+  /* "monocypher.pyx":512
  *     if rv:
  *         raise ValueError('curve point is unsuitable for hiding')
  *     return hidden             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_hidden);
   __pyx_r = __pyx_v_hidden;
   goto __pyx_L0;
 
-  /* "monocypher.pyx":481
+  /* "monocypher.pyx":493
  * 
  * 
  * def elligator_rev(curve: bytes, tweak=None) -> bytes:             # <<<<<<<<<<<<<<
  *     """Computes the representative of a point.
  * 
  */
 
@@ -9441,15 +9664,15 @@
   __Pyx_XDECREF(__pyx_v_hidden);
   __Pyx_XDECREF(__pyx_v_tweak);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "monocypher.pyx":503
+/* "monocypher.pyx":515
  * 
  * 
  * def elligator_key_pair(seed: bytes = None) -> tuple[bytes, bytes]:             # <<<<<<<<<<<<<<
  *     """Generate a key pair.
  * 
  */
 
@@ -9503,48 +9726,48 @@
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_seed);
           if (value) { values[0] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 503, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 515, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "elligator_key_pair") < 0)) __PYX_ERR(0, 503, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "elligator_key_pair") < 0)) __PYX_ERR(0, 515, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_seed = ((PyObject*)values[0]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("elligator_key_pair", 0, 0, 1, __pyx_nargs); __PYX_ERR(0, 503, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("elligator_key_pair", 0, 0, 1, __pyx_nargs); __PYX_ERR(0, 515, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("monocypher.elligator_key_pair", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_seed), (&PyBytes_Type), 1, "seed", 1))) __PYX_ERR(0, 503, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_seed), (&PyBytes_Type), 1, "seed", 1))) __PYX_ERR(0, 515, __pyx_L1_error)
   __pyx_r = __pyx_pf_10monocypher_32elligator_key_pair(__pyx_self, __pyx_v_seed);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -9576,58 +9799,58 @@
   uint8_t *__pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("elligator_key_pair", 0);
   __Pyx_INCREF(__pyx_v_seed);
 
-  /* "monocypher.pyx":513
+  /* "monocypher.pyx":525
  *         * secret_key: The generated 32-byte little endian secret key.
  *     """
  *     hidden = bytes(32)             # <<<<<<<<<<<<<<
  *     secret_key = bytes(32)
  *     if seed is None:
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 513, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 525, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_hidden = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "monocypher.pyx":514
+  /* "monocypher.pyx":526
  *     """
  *     hidden = bytes(32)
  *     secret_key = bytes(32)             # <<<<<<<<<<<<<<
  *     if seed is None:
  *         seed = secrets.token_bytes(32)
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 514, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 526, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_secret_key = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "monocypher.pyx":515
+  /* "monocypher.pyx":527
  *     hidden = bytes(32)
  *     secret_key = bytes(32)
  *     if seed is None:             # <<<<<<<<<<<<<<
  *         seed = secrets.token_bytes(32)
  *     elif len(seed) != 32:
  */
   __pyx_t_2 = (__pyx_v_seed == ((PyObject*)Py_None));
   if (__pyx_t_2) {
 
-    /* "monocypher.pyx":516
+    /* "monocypher.pyx":528
  *     secret_key = bytes(32)
  *     if seed is None:
  *         seed = secrets.token_bytes(32)             # <<<<<<<<<<<<<<
  *     elif len(seed) != 32:
  *         raise ValueError(f'Invalid seed length {len(seed)} != 32')
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_secrets); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 516, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_secrets); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 528, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_token_bytes); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 516, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_token_bytes); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 528, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     __pyx_t_5 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
@@ -9640,131 +9863,131 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_int_32};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 516, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 528, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
-    if (!(likely(PyBytes_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_t_1))) __PYX_ERR(0, 516, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_t_1))) __PYX_ERR(0, 528, __pyx_L1_error)
     __Pyx_DECREF_SET(__pyx_v_seed, ((PyObject*)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "monocypher.pyx":515
+    /* "monocypher.pyx":527
  *     hidden = bytes(32)
  *     secret_key = bytes(32)
  *     if seed is None:             # <<<<<<<<<<<<<<
  *         seed = secrets.token_bytes(32)
  *     elif len(seed) != 32:
  */
     goto __pyx_L3;
   }
 
-  /* "monocypher.pyx":517
+  /* "monocypher.pyx":529
  *     if seed is None:
  *         seed = secrets.token_bytes(32)
  *     elif len(seed) != 32:             # <<<<<<<<<<<<<<
  *         raise ValueError(f'Invalid seed length {len(seed)} != 32')
  *     crypto_elligator_key_pair(hidden, secret_key, seed)
  */
   if (unlikely(__pyx_v_seed == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 517, __pyx_L1_error)
+    __PYX_ERR(0, 529, __pyx_L1_error)
   }
-  __pyx_t_6 = __Pyx_PyBytes_GET_SIZE(__pyx_v_seed); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 517, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyBytes_GET_SIZE(__pyx_v_seed); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 529, __pyx_L1_error)
   __pyx_t_2 = (__pyx_t_6 != 32);
   if (unlikely(__pyx_t_2)) {
 
-    /* "monocypher.pyx":518
+    /* "monocypher.pyx":530
  *         seed = secrets.token_bytes(32)
  *     elif len(seed) != 32:
  *         raise ValueError(f'Invalid seed length {len(seed)} != 32')             # <<<<<<<<<<<<<<
  *     crypto_elligator_key_pair(hidden, secret_key, seed)
  *     return hidden, secret_key
  */
-    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 518, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 530, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_6 = 0;
     __pyx_t_7 = 127;
     __Pyx_INCREF(__pyx_kp_u_Invalid_seed_length);
     __pyx_t_6 += 20;
     __Pyx_GIVEREF(__pyx_kp_u_Invalid_seed_length);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_Invalid_seed_length);
     if (unlikely(__pyx_v_seed == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-      __PYX_ERR(0, 518, __pyx_L1_error)
+      __PYX_ERR(0, 530, __pyx_L1_error)
     }
-    __pyx_t_8 = __Pyx_PyBytes_GET_SIZE(__pyx_v_seed); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(0, 518, __pyx_L1_error)
-    __pyx_t_4 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_t_8, 0, ' ', 'd'); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 518, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyBytes_GET_SIZE(__pyx_v_seed); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(0, 530, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_t_8, 0, ' ', 'd'); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 530, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_6 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
     __pyx_t_4 = 0;
     __Pyx_INCREF(__pyx_kp_u_32);
     __pyx_t_6 += 6;
     __Pyx_GIVEREF(__pyx_kp_u_32);
     PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u_32);
-    __pyx_t_4 = __Pyx_PyUnicode_Join(__pyx_t_1, 3, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 518, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyUnicode_Join(__pyx_t_1, 3, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 530, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 518, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 530, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 518, __pyx_L1_error)
+    __PYX_ERR(0, 530, __pyx_L1_error)
 
-    /* "monocypher.pyx":517
+    /* "monocypher.pyx":529
  *     if seed is None:
  *         seed = secrets.token_bytes(32)
  *     elif len(seed) != 32:             # <<<<<<<<<<<<<<
  *         raise ValueError(f'Invalid seed length {len(seed)} != 32')
  *     crypto_elligator_key_pair(hidden, secret_key, seed)
  */
   }
   __pyx_L3:;
 
-  /* "monocypher.pyx":519
+  /* "monocypher.pyx":531
  *     elif len(seed) != 32:
  *         raise ValueError(f'Invalid seed length {len(seed)} != 32')
  *     crypto_elligator_key_pair(hidden, secret_key, seed)             # <<<<<<<<<<<<<<
  *     return hidden, secret_key
  */
-  __pyx_t_9 = __Pyx_PyBytes_AsWritableUString(__pyx_v_hidden); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 519, __pyx_L1_error)
-  __pyx_t_10 = __Pyx_PyBytes_AsWritableUString(__pyx_v_secret_key); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 519, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyBytes_AsWritableUString(__pyx_v_hidden); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 531, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyBytes_AsWritableUString(__pyx_v_secret_key); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 531, __pyx_L1_error)
   if (unlikely(__pyx_v_seed == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-    __PYX_ERR(0, 519, __pyx_L1_error)
+    __PYX_ERR(0, 531, __pyx_L1_error)
   }
-  __pyx_t_11 = __Pyx_PyBytes_AsWritableUString(__pyx_v_seed); if (unlikely((!__pyx_t_11) && PyErr_Occurred())) __PYX_ERR(0, 519, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyBytes_AsWritableUString(__pyx_v_seed); if (unlikely((!__pyx_t_11) && PyErr_Occurred())) __PYX_ERR(0, 531, __pyx_L1_error)
   crypto_elligator_key_pair(__pyx_t_9, __pyx_t_10, __pyx_t_11);
 
-  /* "monocypher.pyx":520
+  /* "monocypher.pyx":532
  *         raise ValueError(f'Invalid seed length {len(seed)} != 32')
  *     crypto_elligator_key_pair(hidden, secret_key, seed)
  *     return hidden, secret_key             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 520, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 532, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_hidden);
   __Pyx_GIVEREF(__pyx_v_hidden);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_hidden)) __PYX_ERR(0, 520, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_hidden)) __PYX_ERR(0, 532, __pyx_L1_error);
   __Pyx_INCREF(__pyx_v_secret_key);
   __Pyx_GIVEREF(__pyx_v_secret_key);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_secret_key)) __PYX_ERR(0, 520, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_secret_key)) __PYX_ERR(0, 532, __pyx_L1_error);
   __pyx_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "monocypher.pyx":503
+  /* "monocypher.pyx":515
  * 
  * 
  * def elligator_key_pair(seed: bytes = None) -> tuple[bytes, bytes]:             # <<<<<<<<<<<<<<
  *     """Generate a key pair.
  * 
  */
 
@@ -10226,22 +10449,22 @@
 /* #### Code section: pystring_table ### */
 
 static int __Pyx_CreateStringTabAndInitStrings(void) {
   __Pyx_StringTabEntry __pyx_string_tab[] = {
     {&__pyx_kp_u_16, __pyx_k_16, sizeof(__pyx_k_16), 0, 1, 0, 0},
     {&__pyx_kp_u_24, __pyx_k_24, sizeof(__pyx_k_24), 0, 1, 0, 0},
     {&__pyx_kp_u_32, __pyx_k_32, sizeof(__pyx_k_32), 0, 1, 0, 0},
-    {&__pyx_kp_u_4_0_2_1, __pyx_k_4_0_2_1, sizeof(__pyx_k_4_0_2_1), 0, 1, 0, 0},
+    {&__pyx_kp_u_4_0_2_2, __pyx_k_4_0_2_2, sizeof(__pyx_k_4_0_2_2), 0, 1, 0, 0},
     {&__pyx_kp_u_BSD_2_clause, __pyx_k_BSD_2_clause, sizeof(__pyx_k_BSD_2_clause), 0, 1, 0, 0},
     {&__pyx_n_s_Blake2b, __pyx_k_Blake2b, sizeof(__pyx_k_Blake2b), 0, 0, 1, 1},
     {&__pyx_n_s_Blake2b___reduce_cython, __pyx_k_Blake2b___reduce_cython, sizeof(__pyx_k_Blake2b___reduce_cython), 0, 0, 1, 1},
     {&__pyx_n_s_Blake2b___setstate_cython, __pyx_k_Blake2b___setstate_cython, sizeof(__pyx_k_Blake2b___setstate_cython), 0, 0, 1, 1},
     {&__pyx_n_s_Blake2b_finalize, __pyx_k_Blake2b_finalize, sizeof(__pyx_k_Blake2b_finalize), 0, 0, 1, 1},
     {&__pyx_n_s_Blake2b_update, __pyx_k_Blake2b_update, sizeof(__pyx_k_Blake2b_update), 0, 0, 1, 1},
-    {&__pyx_kp_u_Copyright_2018_2022_Jetperch_LLC, __pyx_k_Copyright_2018_2022_Jetperch_LLC, sizeof(__pyx_k_Copyright_2018_2022_Jetperch_LLC), 0, 1, 0, 0},
+    {&__pyx_kp_u_Copyright_2018_2024_Jetperch_LLC, __pyx_k_Copyright_2018_2024_Jetperch_LLC, sizeof(__pyx_k_Copyright_2018_2024_Jetperch_LLC), 0, 1, 0, 0},
     {&__pyx_n_s_IncrementalAuthenticatedEncrypti, __pyx_k_IncrementalAuthenticatedEncrypti, sizeof(__pyx_k_IncrementalAuthenticatedEncrypti), 0, 0, 1, 1},
     {&__pyx_n_s_IncrementalAuthenticatedEncrypti_2, __pyx_k_IncrementalAuthenticatedEncrypti_2, sizeof(__pyx_k_IncrementalAuthenticatedEncrypti_2), 0, 0, 1, 1},
     {&__pyx_n_s_IncrementalAuthenticatedEncrypti_3, __pyx_k_IncrementalAuthenticatedEncrypti_3, sizeof(__pyx_k_IncrementalAuthenticatedEncrypti_3), 0, 0, 1, 1},
     {&__pyx_n_s_IncrementalAuthenticatedEncrypti_4, __pyx_k_IncrementalAuthenticatedEncrypti_4, sizeof(__pyx_k_IncrementalAuthenticatedEncrypti_4), 0, 0, 1, 1},
     {&__pyx_n_s_IncrementalAuthenticatedEncrypti_5, __pyx_k_IncrementalAuthenticatedEncrypti_5, sizeof(__pyx_k_IncrementalAuthenticatedEncrypti_5), 0, 0, 1, 1},
     {&__pyx_kp_u_Invalid_curve_length, __pyx_k_Invalid_curve_length, sizeof(__pyx_k_Invalid_curve_length), 0, 1, 0, 0},
     {&__pyx_kp_u_Invalid_hidden_length, __pyx_k_Invalid_hidden_length, sizeof(__pyx_k_Invalid_hidden_length), 0, 1, 0, 0},
@@ -10257,23 +10480,25 @@
     {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
     {&__pyx_n_s__10, __pyx_k__10, sizeof(__pyx_k__10), 0, 0, 1, 1},
     {&__pyx_kp_b__4, __pyx_k__4, sizeof(__pyx_k__4), 0, 0, 0, 0},
     {&__pyx_kp_u__4, __pyx_k__4, sizeof(__pyx_k__4), 0, 1, 0, 0},
     {&__pyx_n_s__60, __pyx_k__60, sizeof(__pyx_k__60), 0, 0, 1, 1},
     {&__pyx_n_s_a, __pyx_k_a, sizeof(__pyx_k_a), 0, 0, 1, 1},
     {&__pyx_n_s_ad, __pyx_k_ad, sizeof(__pyx_k_ad), 0, 0, 1, 1},
+    {&__pyx_n_u_ad, __pyx_k_ad, sizeof(__pyx_k_ad), 0, 1, 0, 1},
     {&__pyx_n_s_algorithm, __pyx_k_algorithm, sizeof(__pyx_k_algorithm), 0, 0, 1, 1},
     {&__pyx_n_s_argon2i_32, __pyx_k_argon2i_32, sizeof(__pyx_k_argon2i_32), 0, 0, 1, 1},
     {&__pyx_n_s_associated_data, __pyx_k_associated_data, sizeof(__pyx_k_associated_data), 0, 0, 1, 1},
     {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
     {&__pyx_n_s_author, __pyx_k_author, sizeof(__pyx_k_author), 0, 0, 1, 1},
     {&__pyx_n_s_author_email, __pyx_k_author_email, sizeof(__pyx_k_author_email), 0, 0, 1, 1},
     {&__pyx_n_s_b, __pyx_k_b, sizeof(__pyx_k_b), 0, 0, 1, 1},
     {&__pyx_n_s_binascii, __pyx_k_binascii, sizeof(__pyx_k_binascii), 0, 0, 1, 1},
     {&__pyx_n_s_blake2b, __pyx_k_blake2b, sizeof(__pyx_k_blake2b), 0, 0, 1, 1},
+    {&__pyx_n_s_bool, __pyx_k_bool, sizeof(__pyx_k_bool), 0, 0, 1, 1},
     {&__pyx_n_s_bytes, __pyx_k_bytes, sizeof(__pyx_k_bytes), 0, 0, 1, 1},
     {&__pyx_kp_s_c_monocypher_pyx, __pyx_k_c_monocypher_pyx, sizeof(__pyx_k_c_monocypher_pyx), 0, 0, 1, 0},
     {&__pyx_n_s_cfunc_to_py, __pyx_k_cfunc_to_py, sizeof(__pyx_k_cfunc_to_py), 0, 0, 1, 1},
     {&__pyx_n_s_chacha20, __pyx_k_chacha20, sizeof(__pyx_k_chacha20), 0, 0, 1, 1},
     {&__pyx_n_u_chacha20, __pyx_k_chacha20, sizeof(__pyx_k_chacha20), 0, 1, 0, 1},
     {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
     {&__pyx_n_s_compute_key_exchange_public_key, __pyx_k_compute_key_exchange_public_key, sizeof(__pyx_k_compute_key_exchange_public_key), 0, 0, 1, 1},
@@ -10307,14 +10532,15 @@
     {&__pyx_n_s_initializing, __pyx_k_initializing, sizeof(__pyx_k_initializing), 0, 0, 1, 1},
     {&__pyx_n_s_inputs, __pyx_k_inputs, sizeof(__pyx_k_inputs), 0, 0, 1, 1},
     {&__pyx_kp_u_invalid_nonce_length, __pyx_k_invalid_nonce_length, sizeof(__pyx_k_invalid_nonce_length), 0, 1, 0, 0},
     {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
     {&__pyx_kp_u_isenabled, __pyx_k_isenabled, sizeof(__pyx_k_isenabled), 0, 1, 0, 0},
     {&__pyx_kp_u_joulescope_dev_jetperch_com, __pyx_k_joulescope_dev_jetperch_com, sizeof(__pyx_k_joulescope_dev_jetperch_com), 0, 1, 0, 0},
     {&__pyx_n_s_key, __pyx_k_key, sizeof(__pyx_k_key), 0, 0, 1, 1},
+    {&__pyx_n_u_key, __pyx_k_key, sizeof(__pyx_k_key), 0, 1, 0, 1},
     {&__pyx_n_s_key_exchange, __pyx_k_key_exchange, sizeof(__pyx_k_key_exchange), 0, 0, 1, 1},
     {&__pyx_n_s_length, __pyx_k_length, sizeof(__pyx_k_length), 0, 0, 1, 1},
     {&__pyx_n_s_license, __pyx_k_license, sizeof(__pyx_k_license), 0, 0, 1, 1},
     {&__pyx_n_s_lock, __pyx_k_lock, sizeof(__pyx_k_lock), 0, 0, 1, 1},
     {&__pyx_n_s_mac, __pyx_k_mac, sizeof(__pyx_k_mac), 0, 0, 1, 1},
     {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
     {&__pyx_n_s_message, __pyx_k_message, sizeof(__pyx_k_message), 0, 0, 1, 1},
@@ -10327,29 +10553,32 @@
     {&__pyx_n_s_nb_iterations, __pyx_k_nb_iterations, sizeof(__pyx_k_nb_iterations), 0, 0, 1, 1},
     {&__pyx_n_s_nb_lanes, __pyx_k_nb_lanes, sizeof(__pyx_k_nb_lanes), 0, 0, 1, 1},
     {&__pyx_n_s_nb_passes, __pyx_k_nb_passes, sizeof(__pyx_k_nb_passes), 0, 0, 1, 1},
     {&__pyx_n_s_nonce, __pyx_k_nonce, sizeof(__pyx_k_nonce), 0, 0, 1, 1},
     {&__pyx_n_u_os, __pyx_k_os, sizeof(__pyx_k_os), 0, 1, 0, 1},
     {&__pyx_n_s_p, __pyx_k_p, sizeof(__pyx_k_p), 0, 0, 1, 1},
     {&__pyx_n_s_password, __pyx_k_password, sizeof(__pyx_k_password), 0, 0, 1, 1},
+    {&__pyx_n_u_password, __pyx_k_password, sizeof(__pyx_k_password), 0, 1, 0, 1},
     {&__pyx_n_s_plain_text, __pyx_k_plain_text, sizeof(__pyx_k_plain_text), 0, 0, 1, 1},
     {&__pyx_n_s_public, __pyx_k_public, sizeof(__pyx_k_public), 0, 0, 1, 1},
     {&__pyx_n_s_public_key, __pyx_k_public_key, sizeof(__pyx_k_public_key), 0, 0, 1, 1},
     {&__pyx_n_u_pymonocypher, __pyx_k_pymonocypher, sizeof(__pyx_k_pymonocypher), 0, 1, 0, 1},
     {&__pyx_n_s_pyx_state, __pyx_k_pyx_state, sizeof(__pyx_k_pyx_state), 0, 0, 1, 1},
     {&__pyx_n_s_randbits, __pyx_k_randbits, sizeof(__pyx_k_randbits), 0, 0, 1, 1},
     {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
     {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
     {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
     {&__pyx_n_s_result, __pyx_k_result, sizeof(__pyx_k_result), 0, 0, 1, 1},
     {&__pyx_n_s_return, __pyx_k_return, sizeof(__pyx_k_return), 0, 0, 1, 1},
     {&__pyx_n_s_rv, __pyx_k_rv, sizeof(__pyx_k_rv), 0, 0, 1, 1},
     {&__pyx_n_s_salt, __pyx_k_salt, sizeof(__pyx_k_salt), 0, 0, 1, 1},
+    {&__pyx_n_u_salt, __pyx_k_salt, sizeof(__pyx_k_salt), 0, 1, 0, 1},
     {&__pyx_n_s_secret, __pyx_k_secret, sizeof(__pyx_k_secret), 0, 0, 1, 1},
     {&__pyx_n_s_secret_key, __pyx_k_secret_key, sizeof(__pyx_k_secret_key), 0, 0, 1, 1},
+    {&__pyx_kp_u_secret_key_length_invalid, __pyx_k_secret_key_length_invalid, sizeof(__pyx_k_secret_key_length_invalid), 0, 1, 0, 0},
     {&__pyx_n_s_secrets, __pyx_k_secrets, sizeof(__pyx_k_secrets), 0, 0, 1, 1},
     {&__pyx_n_u_secrets, __pyx_k_secrets, sizeof(__pyx_k_secrets), 0, 1, 0, 1},
     {&__pyx_n_s_seed, __pyx_k_seed, sizeof(__pyx_k_seed), 0, 0, 1, 1},
     {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
     {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
     {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
     {&__pyx_n_s_sig, __pyx_k_sig, sizeof(__pyx_k_sig), 0, 0, 1, 1},
@@ -10358,14 +10587,15 @@
     {&__pyx_n_s_signature_sign, __pyx_k_signature_sign, sizeof(__pyx_k_signature_sign), 0, 0, 1, 1},
     {&__pyx_n_s_spec, __pyx_k_spec, sizeof(__pyx_k_spec), 0, 0, 1, 1},
     {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
     {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
     {&__pyx_n_s_their_public_key, __pyx_k_their_public_key, sizeof(__pyx_k_their_public_key), 0, 0, 1, 1},
     {&__pyx_n_s_title, __pyx_k_title, sizeof(__pyx_k_title), 0, 0, 1, 1},
     {&__pyx_n_s_token_bytes, __pyx_k_token_bytes, sizeof(__pyx_k_token_bytes), 0, 0, 1, 1},
+    {&__pyx_kp_u_too_long, __pyx_k_too_long, sizeof(__pyx_k_too_long), 0, 1, 0, 0},
     {&__pyx_kp_s_tuple_bytes_bytes, __pyx_k_tuple_bytes_bytes, sizeof(__pyx_k_tuple_bytes_bytes), 0, 0, 1, 0},
     {&__pyx_n_s_tweak, __pyx_k_tweak, sizeof(__pyx_k_tweak), 0, 0, 1, 1},
     {&__pyx_n_s_unlock, __pyx_k_unlock, sizeof(__pyx_k_unlock), 0, 0, 1, 1},
     {&__pyx_kp_u_unsupported_method_s, __pyx_k_unsupported_method_s, sizeof(__pyx_k_unsupported_method_s), 0, 1, 0, 0},
     {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
     {&__pyx_n_s_url, __pyx_k_url, sizeof(__pyx_k_url), 0, 0, 1, 1},
     {&__pyx_kp_u_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 1, 0, 0},
@@ -10434,44 +10664,44 @@
  *     crypto_blake2b_keyed(hash, len(hash), key, len(key), msg, len(msg))
  *     return hash
  */
   __pyx_tuple__6 = PyTuple_Pack(1, __pyx_int_64); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 281, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "monocypher.pyx":339
- *     extras.ad_size = len(ad)
+  /* "monocypher.pyx":345
+ *     extras.ad_size = _validate_u32('ad', len(ad))
  * 
  *     hash = bytes(32)             # <<<<<<<<<<<<<<
- *     work_area = malloc(nb_blocks * 1024)
+ *     work_area = malloc((<size_t> nb_blocks) * (<size_t> 1024))
  *     try:
  */
-  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_int_32); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 339, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_int_32); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 345, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
-  /* "monocypher.pyx":379
- *     :return: The 32-byte public key.
+  /* "monocypher.pyx":386
  *     """
- *     return secret_key[32:]             # <<<<<<<<<<<<<<
- * 
+ *     if len(secret_key) != 64:
+ *         raise ValueError('secret key length invalid')             # <<<<<<<<<<<<<<
+ *     return secret_key[32:]
  * 
  */
-  __pyx_slice__8 = PySlice_New(__pyx_int_32, Py_None, Py_None); if (unlikely(!__pyx_slice__8)) __PYX_ERR(0, 379, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_slice__8);
-  __Pyx_GIVEREF(__pyx_slice__8);
+  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_secret_key_length_invalid); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 386, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__8);
+  __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "monocypher.pyx":499
+  /* "monocypher.pyx":511
  *     rv = crypto_elligator_rev(hidden, curve, tweak)
  *     if rv:
  *         raise ValueError('curve point is unsuitable for hiding')             # <<<<<<<<<<<<<<
  *     return hidden
  * 
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_curve_point_is_unsuitable_for_hi); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 499, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_curve_point_is_unsuitable_for_hi); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 511, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
   /* "monocypher.pyx":156
  * 
  * 
  * def wipe(data):             # <<<<<<<<<<<<<<
@@ -10614,157 +10844,157 @@
  * def __reduce_cython__(self):
  *     raise TypeError, "Pickling of struct members such as self._ctx must be explicitly requested with @auto_pickle(True)"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "Pickling of struct members such as self._ctx must be explicitly requested with @auto_pickle(True)"
  */
   __pyx_codeobj__35 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__35)) __PYX_ERR(1, 3, __pyx_L1_error)
 
-  /* "monocypher.pyx":317
+  /* "monocypher.pyx":323
  * 
  * 
- * def argon2i_32(nb_blocks, nb_iterations, password, salt, key=None, ad=None):             # <<<<<<<<<<<<<<
+ * def argon2i_32(nb_blocks, nb_iterations, password, salt, key=None, ad=None) -> bytes:             # <<<<<<<<<<<<<<
  *     key = b'' if key is None else key
  *     ad = b'' if ad is None else ad
  */
-  __pyx_tuple__36 = PyTuple_Pack(11, __pyx_n_s_nb_blocks, __pyx_n_s_nb_iterations, __pyx_n_s_password, __pyx_n_s_salt, __pyx_n_s_key, __pyx_n_s_ad, __pyx_n_s_config, __pyx_n_s_inputs, __pyx_n_s_extras, __pyx_n_s_hash, __pyx_n_s_work_area); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(0, 317, __pyx_L1_error)
+  __pyx_tuple__36 = PyTuple_Pack(11, __pyx_n_s_nb_blocks, __pyx_n_s_nb_iterations, __pyx_n_s_password, __pyx_n_s_salt, __pyx_n_s_key, __pyx_n_s_ad, __pyx_n_s_config, __pyx_n_s_inputs, __pyx_n_s_extras, __pyx_n_s_hash, __pyx_n_s_work_area); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(0, 323, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__36);
   __Pyx_GIVEREF(__pyx_tuple__36);
-  __pyx_codeobj__37 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__36, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_argon2i_32, 317, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__37)) __PYX_ERR(0, 317, __pyx_L1_error)
-  __pyx_tuple__38 = PyTuple_Pack(2, Py_None, Py_None); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(0, 317, __pyx_L1_error)
+  __pyx_codeobj__37 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__36, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_argon2i_32, 323, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__37)) __PYX_ERR(0, 323, __pyx_L1_error)
+  __pyx_tuple__38 = PyTuple_Pack(2, Py_None, Py_None); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(0, 323, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__38);
   __Pyx_GIVEREF(__pyx_tuple__38);
 
-  /* "monocypher.pyx":349
+  /* "monocypher.pyx":355
  * 
  * 
- * def compute_key_exchange_public_key(secret_key):             # <<<<<<<<<<<<<<
+ * def compute_key_exchange_public_key(secret_key: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     """Generate the public key for key exchange from the secret key.
  * 
  */
-  __pyx_tuple__39 = PyTuple_Pack(2, __pyx_n_s_secret_key, __pyx_n_s_public_key); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(0, 349, __pyx_L1_error)
+  __pyx_tuple__39 = PyTuple_Pack(2, __pyx_n_s_secret_key, __pyx_n_s_public_key); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(0, 355, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__39);
   __Pyx_GIVEREF(__pyx_tuple__39);
-  __pyx_codeobj__40 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__39, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_compute_key_exchange_public_key, 349, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__40)) __PYX_ERR(0, 349, __pyx_L1_error)
+  __pyx_codeobj__40 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__39, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_compute_key_exchange_public_key, 355, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__40)) __PYX_ERR(0, 355, __pyx_L1_error)
 
-  /* "monocypher.pyx":360
+  /* "monocypher.pyx":366
  * 
  * 
- * def key_exchange(your_secret_key, their_public_key):             # <<<<<<<<<<<<<<
+ * def key_exchange(your_secret_key: bytes, their_public_key: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     """Compute a shared secret based upon public-key crytography.
  * 
  */
-  __pyx_tuple__41 = PyTuple_Pack(3, __pyx_n_s_your_secret_key, __pyx_n_s_their_public_key, __pyx_n_s_p); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(0, 360, __pyx_L1_error)
+  __pyx_tuple__41 = PyTuple_Pack(3, __pyx_n_s_your_secret_key, __pyx_n_s_their_public_key, __pyx_n_s_p); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(0, 366, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__41);
   __Pyx_GIVEREF(__pyx_tuple__41);
-  __pyx_codeobj__42 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__41, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_key_exchange, 360, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__42)) __PYX_ERR(0, 360, __pyx_L1_error)
+  __pyx_codeobj__42 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__41, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_key_exchange, 366, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__42)) __PYX_ERR(0, 366, __pyx_L1_error)
 
-  /* "monocypher.pyx":373
+  /* "monocypher.pyx":379
  * 
  * 
- * def compute_signing_public_key(secret_key):             # <<<<<<<<<<<<<<
+ * def compute_signing_public_key(secret_key: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     """Generate the public key from the secret key.
  * 
  */
-  __pyx_tuple__43 = PyTuple_Pack(1, __pyx_n_s_secret_key); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(0, 373, __pyx_L1_error)
+  __pyx_tuple__43 = PyTuple_Pack(1, __pyx_n_s_secret_key); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(0, 379, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__43);
   __Pyx_GIVEREF(__pyx_tuple__43);
-  __pyx_codeobj__44 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__43, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_compute_signing_public_key, 373, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__44)) __PYX_ERR(0, 373, __pyx_L1_error)
+  __pyx_codeobj__44 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__43, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_compute_signing_public_key, 379, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__44)) __PYX_ERR(0, 379, __pyx_L1_error)
 
-  /* "monocypher.pyx":382
+  /* "monocypher.pyx":390
  * 
  * 
- * def signature_sign(secret_key, message):             # <<<<<<<<<<<<<<
+ * def signature_sign(secret_key: bytes, message: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     """Cryptographically sign a messge.
  * 
  */
-  __pyx_tuple__45 = PyTuple_Pack(3, __pyx_n_s_secret_key, __pyx_n_s_message, __pyx_n_s_sig); if (unlikely(!__pyx_tuple__45)) __PYX_ERR(0, 382, __pyx_L1_error)
+  __pyx_tuple__45 = PyTuple_Pack(3, __pyx_n_s_secret_key, __pyx_n_s_message, __pyx_n_s_sig); if (unlikely(!__pyx_tuple__45)) __PYX_ERR(0, 390, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__45);
   __Pyx_GIVEREF(__pyx_tuple__45);
-  __pyx_codeobj__46 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__45, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_signature_sign, 382, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__46)) __PYX_ERR(0, 382, __pyx_L1_error)
+  __pyx_codeobj__46 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__45, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_signature_sign, 390, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__46)) __PYX_ERR(0, 390, __pyx_L1_error)
 
-  /* "monocypher.pyx":397
+  /* "monocypher.pyx":405
  * 
  * 
- * def signature_check(signature, public_key, message):             # <<<<<<<<<<<<<<
+ * def signature_check(signature, public_key, message) -> bool:             # <<<<<<<<<<<<<<
  *     """Verify the signature.
  * 
  */
-  __pyx_tuple__47 = PyTuple_Pack(3, __pyx_n_s_signature, __pyx_n_s_public_key, __pyx_n_s_message); if (unlikely(!__pyx_tuple__47)) __PYX_ERR(0, 397, __pyx_L1_error)
+  __pyx_tuple__47 = PyTuple_Pack(3, __pyx_n_s_signature, __pyx_n_s_public_key, __pyx_n_s_message); if (unlikely(!__pyx_tuple__47)) __PYX_ERR(0, 405, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__47);
   __Pyx_GIVEREF(__pyx_tuple__47);
-  __pyx_codeobj__48 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__47, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_signature_check, 397, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__48)) __PYX_ERR(0, 397, __pyx_L1_error)
+  __pyx_codeobj__48 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__47, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_signature_check, 405, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__48)) __PYX_ERR(0, 405, __pyx_L1_error)
 
-  /* "monocypher.pyx":410
+  /* "monocypher.pyx":418
  * 
  * 
- * def generate_key(length=None, method=None):             # <<<<<<<<<<<<<<
+ * def generate_key(length=None, method=None) -> bytes:             # <<<<<<<<<<<<<<
  *     """Generate a random key.
  * 
  */
-  __pyx_tuple__49 = PyTuple_Pack(5, __pyx_n_s_length, __pyx_n_s_method, __pyx_n_s_key, __pyx_n_s_nonce, __pyx_n_s_message); if (unlikely(!__pyx_tuple__49)) __PYX_ERR(0, 410, __pyx_L1_error)
+  __pyx_tuple__49 = PyTuple_Pack(5, __pyx_n_s_length, __pyx_n_s_method, __pyx_n_s_key, __pyx_n_s_nonce, __pyx_n_s_message); if (unlikely(!__pyx_tuple__49)) __PYX_ERR(0, 418, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__49);
   __Pyx_GIVEREF(__pyx_tuple__49);
-  __pyx_codeobj__50 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__49, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_generate_key, 410, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__50)) __PYX_ERR(0, 410, __pyx_L1_error)
+  __pyx_codeobj__50 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__49, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_generate_key, 418, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__50)) __PYX_ERR(0, 418, __pyx_L1_error)
 
-  /* "monocypher.pyx":437
+  /* "monocypher.pyx":449
  * 
  * 
- * def generate_signing_key_pair():             # <<<<<<<<<<<<<<
+ * def generate_signing_key_pair() -> tuple[bytes, bytes]:             # <<<<<<<<<<<<<<
  *     """Generate a new keypair for signing using default settings.
  * 
  */
-  __pyx_tuple__51 = PyTuple_Pack(2, __pyx_n_s_secret, __pyx_n_s_public); if (unlikely(!__pyx_tuple__51)) __PYX_ERR(0, 437, __pyx_L1_error)
+  __pyx_tuple__51 = PyTuple_Pack(2, __pyx_n_s_secret, __pyx_n_s_public); if (unlikely(!__pyx_tuple__51)) __PYX_ERR(0, 449, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__51);
   __Pyx_GIVEREF(__pyx_tuple__51);
-  __pyx_codeobj__52 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__51, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_generate_signing_key_pair, 437, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__52)) __PYX_ERR(0, 437, __pyx_L1_error)
+  __pyx_codeobj__52 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__51, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_generate_signing_key_pair, 449, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__52)) __PYX_ERR(0, 449, __pyx_L1_error)
 
-  /* "monocypher.pyx":453
+  /* "monocypher.pyx":465
  * 
  * 
- * def generate_key_exchange_key_pair():             # <<<<<<<<<<<<<<
+ * def generate_key_exchange_key_pair() -> tuple[bytes, bytes]:             # <<<<<<<<<<<<<<
  *     """Generate a new keypair for key exchange using default settings.
  * 
  */
-  __pyx_codeobj__53 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__51, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_generate_key_exchange_key_pair, 453, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__53)) __PYX_ERR(0, 453, __pyx_L1_error)
+  __pyx_codeobj__53 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__51, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_generate_key_exchange_key_pair, 465, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__53)) __PYX_ERR(0, 465, __pyx_L1_error)
 
-  /* "monocypher.pyx":466
+  /* "monocypher.pyx":478
  * 
  * 
  * def elligator_map(hidden: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     """Computes the point corresponding to a representative.
  * 
  */
-  __pyx_tuple__54 = PyTuple_Pack(2, __pyx_n_s_hidden, __pyx_n_s_curve); if (unlikely(!__pyx_tuple__54)) __PYX_ERR(0, 466, __pyx_L1_error)
+  __pyx_tuple__54 = PyTuple_Pack(2, __pyx_n_s_hidden, __pyx_n_s_curve); if (unlikely(!__pyx_tuple__54)) __PYX_ERR(0, 478, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__54);
   __Pyx_GIVEREF(__pyx_tuple__54);
-  __pyx_codeobj__55 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__54, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_elligator_map, 466, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__55)) __PYX_ERR(0, 466, __pyx_L1_error)
+  __pyx_codeobj__55 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__54, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_elligator_map, 478, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__55)) __PYX_ERR(0, 478, __pyx_L1_error)
 
-  /* "monocypher.pyx":481
+  /* "monocypher.pyx":493
  * 
  * 
  * def elligator_rev(curve: bytes, tweak=None) -> bytes:             # <<<<<<<<<<<<<<
  *     """Computes the representative of a point.
  * 
  */
-  __pyx_tuple__56 = PyTuple_Pack(4, __pyx_n_s_curve, __pyx_n_s_tweak, __pyx_n_s_hidden, __pyx_n_s_rv); if (unlikely(!__pyx_tuple__56)) __PYX_ERR(0, 481, __pyx_L1_error)
+  __pyx_tuple__56 = PyTuple_Pack(4, __pyx_n_s_curve, __pyx_n_s_tweak, __pyx_n_s_hidden, __pyx_n_s_rv); if (unlikely(!__pyx_tuple__56)) __PYX_ERR(0, 493, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__56);
   __Pyx_GIVEREF(__pyx_tuple__56);
-  __pyx_codeobj__57 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__56, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_elligator_rev, 481, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__57)) __PYX_ERR(0, 481, __pyx_L1_error)
+  __pyx_codeobj__57 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__56, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_elligator_rev, 493, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__57)) __PYX_ERR(0, 493, __pyx_L1_error)
 
-  /* "monocypher.pyx":503
+  /* "monocypher.pyx":515
  * 
  * 
  * def elligator_key_pair(seed: bytes = None) -> tuple[bytes, bytes]:             # <<<<<<<<<<<<<<
  *     """Generate a key pair.
  * 
  */
-  __pyx_tuple__58 = PyTuple_Pack(3, __pyx_n_s_seed, __pyx_n_s_hidden, __pyx_n_s_secret_key); if (unlikely(!__pyx_tuple__58)) __PYX_ERR(0, 503, __pyx_L1_error)
+  __pyx_tuple__58 = PyTuple_Pack(3, __pyx_n_s_seed, __pyx_n_s_hidden, __pyx_n_s_secret_key); if (unlikely(!__pyx_tuple__58)) __PYX_ERR(0, 515, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__58);
   __Pyx_GIVEREF(__pyx_tuple__58);
-  __pyx_codeobj__59 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__58, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_elligator_key_pair, 503, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__59)) __PYX_ERR(0, 503, __pyx_L1_error)
+  __pyx_codeobj__59 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__58, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_elligator_key_pair, 515, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__59)) __PYX_ERR(0, 515, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -10772,15 +11002,15 @@
 static CYTHON_SMALL_CODE int __Pyx_InitConstants(void) {
   if (__Pyx_CreateStringTabAndInitStrings() < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   __pyx_int_8 = PyInt_FromLong(8); if (unlikely(!__pyx_int_8)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_16 = PyInt_FromLong(16); if (unlikely(!__pyx_int_16)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_24 = PyInt_FromLong(24); if (unlikely(!__pyx_int_24)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_32 = PyInt_FromLong(32); if (unlikely(!__pyx_int_32)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_64 = PyInt_FromLong(64); if (unlikely(!__pyx_int_64)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_int_1024 = PyInt_FromLong(1024); if (unlikely(!__pyx_int_1024)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_4294967295 = PyInt_FromString((char *)"4294967295", 0, 0); if (unlikely(!__pyx_int_4294967295)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: init_globals ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
@@ -11237,31 +11467,31 @@
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_warnings, __pyx_t_2) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "monocypher.pyx":16
  * 
  * # also edit setup.py
- * __version__ = '4.0.2.1'   # also change setup.py             # <<<<<<<<<<<<<<
+ * __version__ = '4.0.2.2'   # also change setup.py             # <<<<<<<<<<<<<<
  * __title__ = 'pymonocypher'
  * __description__ = 'Python ctypes bindings to the Monocypher library'
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_version, __pyx_kp_u_4_0_2_1) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_version, __pyx_kp_u_4_0_2_2) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
 
   /* "monocypher.pyx":17
  * # also edit setup.py
- * __version__ = '4.0.2.1'   # also change setup.py
+ * __version__ = '4.0.2.2'   # also change setup.py
  * __title__ = 'pymonocypher'             # <<<<<<<<<<<<<<
  * __description__ = 'Python ctypes bindings to the Monocypher library'
  * __url__ = 'https://github.com/jetperch/pymonocypher'
  */
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_title, __pyx_n_u_pymonocypher) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
 
   /* "monocypher.pyx":18
- * __version__ = '4.0.2.1'   # also change setup.py
+ * __version__ = '4.0.2.2'   # also change setup.py
  * __title__ = 'pymonocypher'
  * __description__ = 'Python ctypes bindings to the Monocypher library'             # <<<<<<<<<<<<<<
  * __url__ = 'https://github.com/jetperch/pymonocypher'
  * __author__ = 'Jetperch LLC'
  */
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_description, __pyx_kp_u_Python_ctypes_bindings_to_the_Mo) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
 
@@ -11284,35 +11514,35 @@
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_author, __pyx_kp_u_Jetperch_LLC) < 0) __PYX_ERR(0, 20, __pyx_L1_error)
 
   /* "monocypher.pyx":21
  * __url__ = 'https://github.com/jetperch/pymonocypher'
  * __author__ = 'Jetperch LLC'
  * __author_email__ = 'joulescope-dev@jetperch.com'             # <<<<<<<<<<<<<<
  * __license__ = 'BSD 2-clause'
- * __copyright__ = 'Copyright 2018-2022 Jetperch LLC'
+ * __copyright__ = 'Copyright 2018-2024 Jetperch LLC'
  */
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_author_email, __pyx_kp_u_joulescope_dev_jetperch_com) < 0) __PYX_ERR(0, 21, __pyx_L1_error)
 
   /* "monocypher.pyx":22
  * __author__ = 'Jetperch LLC'
  * __author_email__ = 'joulescope-dev@jetperch.com'
  * __license__ = 'BSD 2-clause'             # <<<<<<<<<<<<<<
- * __copyright__ = 'Copyright 2018-2022 Jetperch LLC'
+ * __copyright__ = 'Copyright 2018-2024 Jetperch LLC'
  * 
  */
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_license, __pyx_kp_u_BSD_2_clause) < 0) __PYX_ERR(0, 22, __pyx_L1_error)
 
   /* "monocypher.pyx":23
  * __author_email__ = 'joulescope-dev@jetperch.com'
  * __license__ = 'BSD 2-clause'
- * __copyright__ = 'Copyright 2018-2022 Jetperch LLC'             # <<<<<<<<<<<<<<
+ * __copyright__ = 'Copyright 2018-2024 Jetperch LLC'             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_copyright, __pyx_kp_u_Copyright_2018_2022_Jetperch_LLC) < 0) __PYX_ERR(0, 23, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_copyright, __pyx_kp_u_Copyright_2018_2024_Jetperch_LLC) < 0) __PYX_ERR(0, 23, __pyx_L1_error)
 
   /* "monocypher.pyx":156
  * 
  * 
  * def wipe(data):             # <<<<<<<<<<<<<<
  *     """Wipe a bytes object from memory.
  * 
@@ -11465,189 +11695,240 @@
  *     raise TypeError, "Pickling of struct members such as self._ctx must be explicitly requested with @auto_pickle(True)"
  */
   __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_7Blake2b_9__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Blake2b___setstate_cython, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__35)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_2) < 0) __PYX_ERR(1, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "monocypher.pyx":317
+  /* "monocypher.pyx":323
  * 
  * 
- * def argon2i_32(nb_blocks, nb_iterations, password, salt, key=None, ad=None):             # <<<<<<<<<<<<<<
+ * def argon2i_32(nb_blocks, nb_iterations, password, salt, key=None, ad=None) -> bytes:             # <<<<<<<<<<<<<<
  *     key = b'' if key is None else key
  *     ad = b'' if ad is None else ad
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_11argon2i_32, 0, __pyx_n_s_argon2i_32, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__37)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 317, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 323, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__38);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_argon2i_32, __pyx_t_2) < 0) __PYX_ERR(0, 317, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 323, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_11argon2i_32, 0, __pyx_n_s_argon2i_32, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__37)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 323, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__38);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_argon2i_32, __pyx_t_3) < 0) __PYX_ERR(0, 323, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "monocypher.pyx":349
+  /* "monocypher.pyx":355
  * 
  * 
- * def compute_key_exchange_public_key(secret_key):             # <<<<<<<<<<<<<<
+ * def compute_key_exchange_public_key(secret_key: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     """Generate the public key for key exchange from the secret key.
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_13compute_key_exchange_public_key, 0, __pyx_n_s_compute_key_exchange_public_key, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__40)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 349, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 355, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_secret_key, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 355, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 355, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_13compute_key_exchange_public_key, 0, __pyx_n_s_compute_key_exchange_public_key, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__40)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 355, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_compute_key_exchange_public_key, __pyx_t_2) < 0) __PYX_ERR(0, 349, __pyx_L1_error)
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_compute_key_exchange_public_key, __pyx_t_2) < 0) __PYX_ERR(0, 355, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "monocypher.pyx":360
+  /* "monocypher.pyx":366
  * 
  * 
- * def key_exchange(your_secret_key, their_public_key):             # <<<<<<<<<<<<<<
+ * def key_exchange(your_secret_key: bytes, their_public_key: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     """Compute a shared secret based upon public-key crytography.
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_15key_exchange, 0, __pyx_n_s_key_exchange, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__42)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 360, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 366, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_key_exchange, __pyx_t_2) < 0) __PYX_ERR(0, 360, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_your_secret_key, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 366, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_their_public_key, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 366, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 366, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_15key_exchange, 0, __pyx_n_s_key_exchange, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__42)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 366, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_key_exchange, __pyx_t_3) < 0) __PYX_ERR(0, 366, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "monocypher.pyx":373
+  /* "monocypher.pyx":379
  * 
  * 
- * def compute_signing_public_key(secret_key):             # <<<<<<<<<<<<<<
+ * def compute_signing_public_key(secret_key: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     """Generate the public key from the secret key.
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_17compute_signing_public_key, 0, __pyx_n_s_compute_signing_public_key, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 373, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 379, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_secret_key, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 379, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 379, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_17compute_signing_public_key, 0, __pyx_n_s_compute_signing_public_key, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 379, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_compute_signing_public_key, __pyx_t_2) < 0) __PYX_ERR(0, 373, __pyx_L1_error)
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_compute_signing_public_key, __pyx_t_2) < 0) __PYX_ERR(0, 379, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "monocypher.pyx":382
+  /* "monocypher.pyx":390
  * 
  * 
- * def signature_sign(secret_key, message):             # <<<<<<<<<<<<<<
+ * def signature_sign(secret_key: bytes, message: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     """Cryptographically sign a messge.
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_19signature_sign, 0, __pyx_n_s_signature_sign, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__46)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 382, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 390, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_signature_sign, __pyx_t_2) < 0) __PYX_ERR(0, 382, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_secret_key, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 390, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_message, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 390, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 390, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_19signature_sign, 0, __pyx_n_s_signature_sign, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__46)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 390, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_signature_sign, __pyx_t_3) < 0) __PYX_ERR(0, 390, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "monocypher.pyx":397
+  /* "monocypher.pyx":405
  * 
  * 
- * def signature_check(signature, public_key, message):             # <<<<<<<<<<<<<<
+ * def signature_check(signature, public_key, message) -> bool:             # <<<<<<<<<<<<<<
  *     """Verify the signature.
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_21signature_check, 0, __pyx_n_s_signature_check, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__48)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 397, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 405, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_bool) < 0) __PYX_ERR(0, 405, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_21signature_check, 0, __pyx_n_s_signature_check, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__48)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 405, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_signature_check, __pyx_t_2) < 0) __PYX_ERR(0, 397, __pyx_L1_error)
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_signature_check, __pyx_t_2) < 0) __PYX_ERR(0, 405, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "monocypher.pyx":410
+  /* "monocypher.pyx":418
  * 
  * 
- * def generate_key(length=None, method=None):             # <<<<<<<<<<<<<<
+ * def generate_key(length=None, method=None) -> bytes:             # <<<<<<<<<<<<<<
  *     """Generate a random key.
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_23generate_key, 0, __pyx_n_s_generate_key, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__50)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 410, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 418, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__38);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_generate_key, __pyx_t_2) < 0) __PYX_ERR(0, 410, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 418, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_23generate_key, 0, __pyx_n_s_generate_key, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__50)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 418, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__38);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_generate_key, __pyx_t_3) < 0) __PYX_ERR(0, 418, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "monocypher.pyx":437
+  /* "monocypher.pyx":449
  * 
  * 
- * def generate_signing_key_pair():             # <<<<<<<<<<<<<<
+ * def generate_signing_key_pair() -> tuple[bytes, bytes]:             # <<<<<<<<<<<<<<
  *     """Generate a new keypair for signing using default settings.
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_25generate_signing_key_pair, 0, __pyx_n_s_generate_signing_key_pair, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__52)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 437, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 449, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_kp_s_tuple_bytes_bytes) < 0) __PYX_ERR(0, 449, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_25generate_signing_key_pair, 0, __pyx_n_s_generate_signing_key_pair, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__52)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 449, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_generate_signing_key_pair, __pyx_t_2) < 0) __PYX_ERR(0, 437, __pyx_L1_error)
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_generate_signing_key_pair, __pyx_t_2) < 0) __PYX_ERR(0, 449, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "monocypher.pyx":453
+  /* "monocypher.pyx":465
  * 
  * 
- * def generate_key_exchange_key_pair():             # <<<<<<<<<<<<<<
+ * def generate_key_exchange_key_pair() -> tuple[bytes, bytes]:             # <<<<<<<<<<<<<<
  *     """Generate a new keypair for key exchange using default settings.
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_27generate_key_exchange_key_pair, 0, __pyx_n_s_generate_key_exchange_key_pair, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__53)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 453, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 465, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_generate_key_exchange_key_pair, __pyx_t_2) < 0) __PYX_ERR(0, 453, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_kp_s_tuple_bytes_bytes) < 0) __PYX_ERR(0, 465, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_27generate_key_exchange_key_pair, 0, __pyx_n_s_generate_key_exchange_key_pair, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__53)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 465, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_generate_key_exchange_key_pair, __pyx_t_3) < 0) __PYX_ERR(0, 465, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "monocypher.pyx":466
+  /* "monocypher.pyx":478
  * 
  * 
  * def elligator_map(hidden: bytes) -> bytes:             # <<<<<<<<<<<<<<
  *     """Computes the point corresponding to a representative.
  * 
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 466, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_hidden, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 466, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 466, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_29elligator_map, 0, __pyx_n_s_elligator_map, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__55)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 466, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 478, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_elligator_map, __pyx_t_3) < 0) __PYX_ERR(0, 466, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_hidden, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 478, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 478, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_29elligator_map, 0, __pyx_n_s_elligator_map, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__55)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 478, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_elligator_map, __pyx_t_2) < 0) __PYX_ERR(0, 478, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "monocypher.pyx":481
+  /* "monocypher.pyx":493
  * 
  * 
  * def elligator_rev(curve: bytes, tweak=None) -> bytes:             # <<<<<<<<<<<<<<
  *     """Computes the representative of a point.
  * 
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 481, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_curve, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 481, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 481, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_31elligator_rev, 0, __pyx_n_s_elligator_rev, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__57)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 481, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 493, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__15);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_elligator_rev, __pyx_t_2) < 0) __PYX_ERR(0, 481, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_curve, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 493, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 493, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_31elligator_rev, 0, __pyx_n_s_elligator_rev, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__57)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 493, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__15);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_elligator_rev, __pyx_t_3) < 0) __PYX_ERR(0, 493, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "monocypher.pyx":503
+  /* "monocypher.pyx":515
  * 
  * 
  * def elligator_key_pair(seed: bytes = None) -> tuple[bytes, bytes]:             # <<<<<<<<<<<<<<
  *     """Generate a key pair.
  * 
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 503, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_seed, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 503, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_kp_s_tuple_bytes_bytes) < 0) __PYX_ERR(0, 503, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_33elligator_key_pair, 0, __pyx_n_s_elligator_key_pair, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__59)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 503, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 515, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__15);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_elligator_key_pair, __pyx_t_3) < 0) __PYX_ERR(0, 503, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_seed, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 515, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_kp_s_tuple_bytes_bytes) < 0) __PYX_ERR(0, 515, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10monocypher_33elligator_key_pair, 0, __pyx_n_s_elligator_key_pair, NULL, __pyx_n_s_monocypher, __pyx_d, ((PyObject *)__pyx_codeobj__59)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 515, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__15);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_elligator_key_pair, __pyx_t_2) < 0) __PYX_ERR(0, 515, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "monocypher.pyx":1
  * """             # <<<<<<<<<<<<<<
  * Monocypher library Python bindings.
  * 
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /*--- Wrapped vars code ---*/
   {
     PyObject* wrapped = __Pyx_CFunc_f5947c__10monocypher_int__lParen__const_uint8_t__ptr____etc_to_py_1a_1b(crypto_verify16);
     if (unlikely(!wrapped)) __PYX_ERR(0, 28, __pyx_L1_error)
     if (PyObject_SetAttrString(__pyx_m, "crypto_verify16", wrapped) < 0) __PYX_ERR(0, 28, __pyx_L1_error);
   }
@@ -14305,161 +14586,14 @@
     if (likely(tp->tp_setattr))
         return tp->tp_setattr(obj, PyString_AS_STRING(attr_name), value);
 #endif
     return PyObject_SetAttr(obj, attr_name, value);
 }
 #endif
 
-/* PyIntBinop */
-#if !CYTHON_COMPILING_IN_PYPY
-static PyObject* __Pyx_PyInt_MultiplyObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check) {
-    CYTHON_MAYBE_UNUSED_VAR(intval);
-    CYTHON_MAYBE_UNUSED_VAR(inplace);
-    CYTHON_UNUSED_VAR(zerodivision_check);
-    #if PY_MAJOR_VERSION < 3
-    if (likely(PyInt_CheckExact(op1))) {
-        const long b = intval;
-        long a = PyInt_AS_LONG(op1);
-        
-#ifdef HAVE_LONG_LONG
-            if (sizeof(PY_LONG_LONG) > sizeof(long)) {
-                PY_LONG_LONG result = (PY_LONG_LONG)a * (PY_LONG_LONG)b;
-                return (result >= LONG_MIN && result <= LONG_MAX) ?
-                    PyInt_FromLong((long)result) : PyLong_FromLongLong(result);
-            }
-#endif
-#if CYTHON_USE_TYPE_SLOTS
-            return PyInt_Type.tp_as_number->nb_multiply(op1, op2);
-#else
-            return PyNumber_Multiply(op1, op2);
-#endif
-    }
-    #endif
-    #if CYTHON_USE_PYLONG_INTERNALS
-    if (likely(PyLong_CheckExact(op1))) {
-        const long b = intval;
-        long a, x;
-#ifdef HAVE_LONG_LONG
-        const PY_LONG_LONG llb = intval;
-        PY_LONG_LONG lla, llx;
-#endif
-        if (unlikely(__Pyx_PyLong_IsZero(op1))) {
-            return __Pyx_NewRef(op1);
-        }
-        if (likely(__Pyx_PyLong_IsCompact(op1))) {
-            a = __Pyx_PyLong_CompactValue(op1);
-        } else {
-            const digit* digits = __Pyx_PyLong_Digits(op1);
-            const Py_ssize_t size = __Pyx_PyLong_SignedDigitCount(op1);
-            switch (size) {
-                case -2:
-                    if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT+30) {
-                        a = -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-                    #ifdef HAVE_LONG_LONG
-                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT+30) {
-                        lla = -(PY_LONG_LONG) (((((unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
-                        goto long_long;
-                    #endif
-                    }
-                    CYTHON_FALLTHROUGH;
-                case 2:
-                    if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT+30) {
-                        a = (long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-                    #ifdef HAVE_LONG_LONG
-                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT+30) {
-                        lla = (PY_LONG_LONG) (((((unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
-                        goto long_long;
-                    #endif
-                    }
-                    CYTHON_FALLTHROUGH;
-                case -3:
-                    if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT+30) {
-                        a = -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-                    #ifdef HAVE_LONG_LONG
-                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT+30) {
-                        lla = -(PY_LONG_LONG) (((((((unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
-                        goto long_long;
-                    #endif
-                    }
-                    CYTHON_FALLTHROUGH;
-                case 3:
-                    if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT+30) {
-                        a = (long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-                    #ifdef HAVE_LONG_LONG
-                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT+30) {
-                        lla = (PY_LONG_LONG) (((((((unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
-                        goto long_long;
-                    #endif
-                    }
-                    CYTHON_FALLTHROUGH;
-                case -4:
-                    if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT+30) {
-                        a = -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-                    #ifdef HAVE_LONG_LONG
-                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 4 * PyLong_SHIFT+30) {
-                        lla = -(PY_LONG_LONG) (((((((((unsigned PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
-                        goto long_long;
-                    #endif
-                    }
-                    CYTHON_FALLTHROUGH;
-                case 4:
-                    if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT+30) {
-                        a = (long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-                    #ifdef HAVE_LONG_LONG
-                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 4 * PyLong_SHIFT+30) {
-                        lla = (PY_LONG_LONG) (((((((((unsigned PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
-                        goto long_long;
-                    #endif
-                    }
-                    CYTHON_FALLTHROUGH;
-                default: return PyLong_Type.tp_as_number->nb_multiply(op1, op2);
-            }
-        }
-                CYTHON_UNUSED_VAR(a);
-                CYTHON_UNUSED_VAR(b);
-                #ifdef HAVE_LONG_LONG
-                lla = a;
-                goto long_long;
-                #else
-                return PyLong_Type.tp_as_number->nb_multiply(op1, op2);
-                #endif
-            return PyLong_FromLong(x);
-#ifdef HAVE_LONG_LONG
-        long_long:
-                llx = lla * llb;
-            return PyLong_FromLongLong(llx);
-#endif
-        
-        
-    }
-    #endif
-    if (PyFloat_CheckExact(op1)) {
-        const long b = intval;
-#if CYTHON_COMPILING_IN_LIMITED_API
-        double a = __pyx_PyFloat_AsDouble(op1);
-#else
-        double a = PyFloat_AS_DOUBLE(op1);
-#endif
-            double result;
-            
-            PyFPE_START_PROTECT("multiply", return NULL)
-            result = ((double)a) * (double)b;
-            PyFPE_END_PROTECT(result)
-            return PyFloat_FromDouble(result);
-    }
-    return (inplace ? PyNumber_InPlaceMultiply : PyNumber_Multiply)(op1, op2);
-}
-#endif
-
 /* GetException */
 #if CYTHON_FAST_THREAD_STATE
 static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
 #else
 static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
 #endif
 {
@@ -14683,116 +14817,39 @@
     Py_XDECREF(tmp_type);
     Py_XDECREF(tmp_value);
     Py_XDECREF(tmp_tb);
   #endif
 }
 #endif
 
-/* SliceObject */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GetSlice(PyObject* obj,
-        Py_ssize_t cstart, Py_ssize_t cstop,
-        PyObject** _py_start, PyObject** _py_stop, PyObject** _py_slice,
-        int has_cstart, int has_cstop, int wraparound) {
+/* ArgTypeTest */
+static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact)
+{
+    __Pyx_TypeName type_name;
     __Pyx_TypeName obj_type_name;
-#if CYTHON_USE_TYPE_SLOTS
-    PyMappingMethods* mp;
-#if PY_MAJOR_VERSION < 3
-    PySequenceMethods* ms = Py_TYPE(obj)->tp_as_sequence;
-    if (likely(ms && ms->sq_slice)) {
-        if (!has_cstart) {
-            if (_py_start && (*_py_start != Py_None)) {
-                cstart = __Pyx_PyIndex_AsSsize_t(*_py_start);
-                if ((cstart == (Py_ssize_t)-1) && PyErr_Occurred()) goto bad;
-            } else
-                cstart = 0;
-        }
-        if (!has_cstop) {
-            if (_py_stop && (*_py_stop != Py_None)) {
-                cstop = __Pyx_PyIndex_AsSsize_t(*_py_stop);
-                if ((cstop == (Py_ssize_t)-1) && PyErr_Occurred()) goto bad;
-            } else
-                cstop = PY_SSIZE_T_MAX;
-        }
-        if (wraparound && unlikely((cstart < 0) | (cstop < 0)) && likely(ms->sq_length)) {
-            Py_ssize_t l = ms->sq_length(obj);
-            if (likely(l >= 0)) {
-                if (cstop < 0) {
-                    cstop += l;
-                    if (cstop < 0) cstop = 0;
-                }
-                if (cstart < 0) {
-                    cstart += l;
-                    if (cstart < 0) cstart = 0;
-                }
-            } else {
-                if (!PyErr_ExceptionMatches(PyExc_OverflowError))
-                    goto bad;
-                PyErr_Clear();
-            }
-        }
-        return ms->sq_slice(obj, cstart, cstop);
+    if (unlikely(!type)) {
+        PyErr_SetString(PyExc_SystemError, "Missing type object");
+        return 0;
     }
-#else
-    CYTHON_UNUSED_VAR(wraparound);
-#endif
-    mp = Py_TYPE(obj)->tp_as_mapping;
-    if (likely(mp && mp->mp_subscript))
-#else
-    CYTHON_UNUSED_VAR(wraparound);
-#endif
-    {
-        PyObject* result;
-        PyObject *py_slice, *py_start, *py_stop;
-        if (_py_slice) {
-            py_slice = *_py_slice;
-        } else {
-            PyObject* owned_start = NULL;
-            PyObject* owned_stop = NULL;
-            if (_py_start) {
-                py_start = *_py_start;
-            } else {
-                if (has_cstart) {
-                    owned_start = py_start = PyInt_FromSsize_t(cstart);
-                    if (unlikely(!py_start)) goto bad;
-                } else
-                    py_start = Py_None;
-            }
-            if (_py_stop) {
-                py_stop = *_py_stop;
-            } else {
-                if (has_cstop) {
-                    owned_stop = py_stop = PyInt_FromSsize_t(cstop);
-                    if (unlikely(!py_stop)) {
-                        Py_XDECREF(owned_start);
-                        goto bad;
-                    }
-                } else
-                    py_stop = Py_None;
-            }
-            py_slice = PySlice_New(py_start, py_stop, Py_None);
-            Py_XDECREF(owned_start);
-            Py_XDECREF(owned_stop);
-            if (unlikely(!py_slice)) goto bad;
-        }
-#if CYTHON_USE_TYPE_SLOTS
-        result = mp->mp_subscript(obj, py_slice);
-#else
-        result = PyObject_GetItem(obj, py_slice);
-#endif
-        if (!_py_slice) {
-            Py_DECREF(py_slice);
-        }
-        return result;
+    else if (exact) {
+        #if PY_MAJOR_VERSION == 2
+        if ((type == &PyBaseString_Type) && likely(__Pyx_PyBaseString_CheckExact(obj))) return 1;
+        #endif
+    }
+    else {
+        if (likely(__Pyx_TypeCheck(obj, type))) return 1;
     }
+    type_name = __Pyx_PyType_GetName(type);
     obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
     PyErr_Format(PyExc_TypeError,
-        "'" __Pyx_FMT_TYPENAME "' object is unsliceable", obj_type_name);
+        "Argument '%.200s' has incorrect type (expected " __Pyx_FMT_TYPENAME
+        ", got " __Pyx_FMT_TYPENAME ")", name, type_name, obj_type_name);
+    __Pyx_DECREF_TypeName(type_name);
     __Pyx_DECREF_TypeName(obj_type_name);
-bad:
-    return NULL;
+    return 0;
 }
 
 /* PyDictVersioning */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj) {
     PyObject *dict = Py_TYPE(obj)->tp_dict;
     return likely(dict) ? __PYX_GET_DICT_VERSION(dict) : 0;
@@ -14856,41 +14913,14 @@
         return __Pyx_NewRef(result);
     }
     PyErr_Clear();
 #endif
     return __Pyx_GetBuiltinName(name);
 }
 
-/* ArgTypeTest */
-static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact)
-{
-    __Pyx_TypeName type_name;
-    __Pyx_TypeName obj_type_name;
-    if (unlikely(!type)) {
-        PyErr_SetString(PyExc_SystemError, "Missing type object");
-        return 0;
-    }
-    else if (exact) {
-        #if PY_MAJOR_VERSION == 2
-        if ((type == &PyBaseString_Type) && likely(__Pyx_PyBaseString_CheckExact(obj))) return 1;
-        #endif
-    }
-    else {
-        if (likely(__Pyx_TypeCheck(obj, type))) return 1;
-    }
-    type_name = __Pyx_PyType_GetName(type);
-    obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
-    PyErr_Format(PyExc_TypeError,
-        "Argument '%.200s' has incorrect type (expected " __Pyx_FMT_TYPENAME
-        ", got " __Pyx_FMT_TYPENAME ")", name, type_name, obj_type_name);
-    __Pyx_DECREF_TypeName(type_name);
-    __Pyx_DECREF_TypeName(obj_type_name);
-    return 0;
-}
-
 /* RaiseUnexpectedTypeError */
 static int
 __Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj)
 {
     __Pyx_TypeName obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
     PyErr_Format(PyExc_TypeError, "Expected %s, got " __Pyx_FMT_TYPENAME,
                  expected, obj_type_name);
@@ -16231,78 +16261,14 @@
     return (int) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int");
     return (int) -1;
 }
 
-/* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_uint32_t(uint32_t value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const uint32_t neg_one = (uint32_t) -1, const_zero = (uint32_t) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(uint32_t) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(uint32_t) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(uint32_t) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(uint32_t) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(uint32_t) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
-        return _PyLong_FromByteArray(bytes, sizeof(uint32_t),
-                                     little, !is_unsigned);
-#else
-        PyObject *from_bytes, *result = NULL;
-        PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
-        if (!from_bytes) return NULL;
-        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(uint32_t));
-        if (!py_bytes) goto limited_bad;
-        order_str = PyUnicode_FromString(little ? "little" : "big");
-        if (!order_str) goto limited_bad;
-        arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
-        if (!arg_tuple) goto limited_bad;
-        if (!is_unsigned) {
-            kwds = PyDict_New();
-            if (!kwds) goto limited_bad;
-            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
-        }
-        result = PyObject_Call(from_bytes, arg_tuple, kwds);
-        limited_bad:
-        Py_XDECREF(kwds);
-        Py_XDECREF(arg_tuple);
-        Py_XDECREF(order_str);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(from_bytes);
-        return result;
-#endif
-    }
-}
-
 /* CIntFromPy */
 static CYTHON_INLINE uint32_t __Pyx_PyInt_As_uint32_t(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const uint32_t neg_one = (uint32_t) -1, const_zero = (uint32_t) 0;
@@ -16568,14 +16534,78 @@
     return (uint32_t) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to uint32_t");
     return (uint32_t) -1;
 }
 
+/* CIntToPy */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_uint32_t(uint32_t value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const uint32_t neg_one = (uint32_t) -1, const_zero = (uint32_t) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(uint32_t) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(uint32_t) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(uint32_t) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(uint32_t) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(uint32_t) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
+        return _PyLong_FromByteArray(bytes, sizeof(uint32_t),
+                                     little, !is_unsigned);
+#else
+        PyObject *from_bytes, *result = NULL;
+        PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
+        if (!from_bytes) return NULL;
+        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(uint32_t));
+        if (!py_bytes) goto limited_bad;
+        order_str = PyUnicode_FromString(little ? "little" : "big");
+        if (!order_str) goto limited_bad;
+        arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
+        if (!arg_tuple) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
+        result = PyObject_Call(from_bytes, arg_tuple, kwds);
+        limited_bad:
+        Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
+        return result;
+#endif
+    }
+}
+
 /* CIntFromPy */
 static CYTHON_INLINE size_t __Pyx_PyInt_As_size_t(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const size_t neg_one = (size_t) -1, const_zero = (size_t) 0;
```

### Comparing `pymonocypher-4.0.2.1/monocypher.c` & `pymonocypher-4.0.2.2/monocypher.c`

 * *Files identical despite different names*

### Comparing `pymonocypher-4.0.2.1/monocypher.h` & `pymonocypher-4.0.2.2/monocypher.h`

 * *Files identical despite different names*

### Comparing `pymonocypher-4.0.2.1/pymonocypher.egg-info/PKG-INFO` & `pymonocypher-4.0.2.2/pymonocypher.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonocypher
-Version: 4.0.2.1
+Version: 4.0.2.2
 Summary: Python ctypes bindings to the Monocypher library
 Home-page: https://github.com/jetperch/pymonocypher
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: BSD 2-clause
 Project-URL: Bug Reports, https://github.com/jetperch/pymonocypher/issues
 Project-URL: Source, https://github.com/jetperch/pymonocypher/
```

### Comparing `pymonocypher-4.0.2.1/pyproject.toml` & `pymonocypher-4.0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pymonocypher-4.0.2.1/setup.py` & `pymonocypher-4.0.2.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # https://github.com/pypa/sampleproject
 
 
 import setuptools
 import os
 
 MYPATH = os.path.abspath(os.path.dirname(__file__))
-VERSION = '4.0.2.1'  # also change c_monocypher.pyx
+VERSION = '4.0.2.2'  # also change c_monocypher.pyx
 
 
 try:
     from Cython.Build import cythonize
     USE_CYTHON = os.path.isfile(os.path.join(MYPATH, 'c_monocypher.pyx'))
 except ImportError:
     USE_CYTHON = False
```

### Comparing `pymonocypher-4.0.2.1/test/blake2-kat.json` & `pymonocypher-4.0.2.2/test/blake2-kat.json`

 * *Files identical despite different names*

### Comparing `pymonocypher-4.0.2.1/test/test_monocypher.py` & `pymonocypher-4.0.2.2/test/test_monocypher.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,18 @@
         b_shared_secret = monocypher.key_exchange(b_private_secret, a_public_secret)
         a_shared_secret = monocypher.key_exchange(a_private_secret, b_public_secret)
         self.assertEqual(a_shared_secret, b_shared_secret)
 
     def test_generate_key(self):
         self.assertEqual(32, len(monocypher.generate_key()))
 
+    def test_compute_signing_public_key(self):
+        with self.assertRaises(ValueError):
+            monocypher.compute_signing_public_key(monocypher.generate_key())
+
     def test_elligator(self):
         hidden1, secret = monocypher.elligator_key_pair()
         curve1 = monocypher.elligator_map(hidden1)
         while True:
             try:
                 hidden2 = monocypher.elligator_rev(curve1)
                 break
```

