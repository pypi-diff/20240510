# Comparing `tmp/flexible_dict-1.2.3.tar.gz` & `tmp/flexible_dict-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flexible_dict-1.2.3.tar", last modified: Wed Apr 17 04:43:31 2024, max compression
+gzip compressed data, was "flexible_dict-2.0.0.tar", last modified: Thu May  9 12:39:05 2024, max compression
```

## Comparing `flexible_dict-1.2.3.tar` & `flexible_dict-2.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:43:31.837538 flexible_dict-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-17 04:43:31.837538 flexible_dict-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-17 04:43:27.000000 flexible_dict-1.2.3/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      117 2024-04-17 04:43:27.000000 flexible_dict-1.2.3/build.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:43:31.837538 flexible_dict-1.2.3/flexible_dict/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-17 04:43:27.000000 flexible_dict-1.2.3/flexible_dict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-17 04:43:27.000000 flexible_dict-1.2.3/flexible_dict/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-17 04:43:31.000000 flexible_dict-1.2.3/flexible_dict/_dist_ver.py
--rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-04-17 04:43:27.000000 flexible_dict-1.2.3/flexible_dict/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    26728 2024-04-17 04:43:27.000000 flexible_dict-1.2.3/flexible_dict/json_object.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:43:31.837538 flexible_dict-1.2.3/flexible_dict/script/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 04:43:27.000000 flexible_dict-1.2.3/flexible_dict/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-04-17 04:43:27.000000 flexible_dict-1.2.3/flexible_dict/script/class_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-17 04:43:27.000000 flexible_dict-1.2.3/flexible_dict/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:43:31.837538 flexible_dict-1.2.3/flexible_dict.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-17 04:43:31.000000 flexible_dict-1.2.3/flexible_dict.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-17 04:43:31.000000 flexible_dict-1.2.3/flexible_dict.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 04:43:31.000000 flexible_dict-1.2.3/flexible_dict.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-17 04:43:31.000000 flexible_dict-1.2.3/flexible_dict.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-17 04:43:27.000000 flexible_dict-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-17 04:43:27.000000 flexible_dict-1.2.3/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      359 2024-04-17 04:43:27.000000 flexible_dict-1.2.3/run_test.sh
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 04:43:31.837538 flexible_dict-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-17 04:43:27.000000 flexible_dict-1.2.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:39:05.159058 flexible_dict-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-09 12:39:05.159058 flexible_dict-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-09 12:38:56.000000 flexible_dict-2.0.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      117 2024-05-09 12:38:56.000000 flexible_dict-2.0.0/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:39:05.159058 flexible_dict-2.0.0/flexible_dict/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-09 12:38:56.000000 flexible_dict-2.0.0/flexible_dict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-09 12:38:56.000000 flexible_dict-2.0.0/flexible_dict/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-09 12:39:05.000000 flexible_dict-2.0.0/flexible_dict/_dist_ver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-05-09 12:38:56.000000 flexible_dict-2.0.0/flexible_dict/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26128 2024-05-09 12:38:56.000000 flexible_dict-2.0.0/flexible_dict/json_object.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:39:05.159058 flexible_dict-2.0.0/flexible_dict/script/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 12:38:56.000000 flexible_dict-2.0.0/flexible_dict/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-05-09 12:38:56.000000 flexible_dict-2.0.0/flexible_dict/script/class_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-09 12:38:56.000000 flexible_dict-2.0.0/flexible_dict/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:39:05.159058 flexible_dict-2.0.0/flexible_dict.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-09 12:39:05.000000 flexible_dict-2.0.0/flexible_dict.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-09 12:39:05.000000 flexible_dict-2.0.0/flexible_dict.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 12:39:05.000000 flexible_dict-2.0.0/flexible_dict.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-09 12:39:05.000000 flexible_dict-2.0.0/flexible_dict.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-09 12:38:56.000000 flexible_dict-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-09 12:38:56.000000 flexible_dict-2.0.0/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      359 2024-05-09 12:38:56.000000 flexible_dict-2.0.0/run_test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 12:39:05.159058 flexible_dict-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-09 12:38:56.000000 flexible_dict-2.0.0/tox.ini
```

### Comparing `flexible_dict-1.2.3/PKG-INFO` & `flexible_dict-2.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flexible_dict
-Version: 1.2.3
+Version: 2.0.0
 Summary: A flexible way to access dict data instead of built-in dict.
 Author-email: darkpeath <darkpeath@gmail.com>
 Project-URL: Homepage, https://github.com/darkpeath/flexible_dict
 Description-Content-Type: text/markdown
 Requires-Dist: dataclasses; python_version < "3.7"
 Requires-Dist: typing_extensions; python_version < "3.8"
```

### Comparing `flexible_dict-1.2.3/README.md` & `flexible_dict-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `flexible_dict-1.2.3/flexible_dict/__main__.py` & `flexible_dict-2.0.0/flexible_dict/__main__.py`

 * *Files identical despite different names*

### Comparing `flexible_dict-1.2.3/flexible_dict/adapter.py` & `flexible_dict-2.0.0/flexible_dict/adapter.py`

 * *Files identical despite different names*

### Comparing `flexible_dict-1.2.3/flexible_dict/json_object.py` & `flexible_dict-2.0.0/flexible_dict/json_object.py`

 * *Files 9% similar despite different names*

```diff
@@ -89,41 +89,45 @@
     key: str = MISSING
 
     # access control
     readable: bool = True
     writeable: bool = True
     deletable: bool = True
 
-    # default value setting
-    default: Any = None     # default value when the key not exists
-    default_factory: Callable[[dict], Any] = MISSING     # a function to get a value from the dict
-
-    # decide what scope the field belong to
-    static: bool = False    # a class property
-    exclude: bool = False   # exclude from dict key and mark as object property
-
-    # # if set as false, an exception will be raised when the key not exists
-    check_exist_before_delete: bool = True
-
+    # default value when init the dict
+    init_default: Any = MISSING
+    # a function to build default value when init the dict
+    init_default_factory: Callable[[], Any] = MISSING
+
+    # default value when access an absent key
+    getter_default: Any = MISSING
+    # a function to build default value when access an absent key
+    getter_default_factory0: Callable[[], Any] = MISSING
+    # a function to get value for the dict when access an absent key
+    getter_default_factory1: Callable[[dict], Any] = MISSING
+    
     # functions to cast value type when write or read dict
     encoder: Union[_ENCODER_TYPE, Literal['auto'], None] = 'auto'    # cast value type when write to dict
     decoder: Union[_DECODER_TYPE, None] = 'auto'    # cast value type when read from dict
 
+    # if set as false, an exception will be raised when the key not exists
+    check_exist_before_delete: bool = True
+
     # auto detect value
-    name: str = None
-    type: Any = None
-    _field_type: _FIELD_BASE = _FIELD_DICTKEY
+    name: str = dataclasses.field(init=False, default=None)
+    type: Any = dataclasses.field(init=False, default=None)
+    _field_type: _FIELD_BASE = dataclasses.field(init=False, default=_FIELD_DICTKEY)
 
     # additional metadata
     metadata: Dict[Any, Any] = dataclasses.field(default_factory=dict)
 
 @dataclasses.dataclass
 class ProcessorConfig:
-    # default value config on the class for field without init value
-    default_field_value: Any = None
+    # default value when access an absent key in class scope
+    getter_default: Any = MISSING
 
     # auto set encoder and decoder for field
     adapter_detector: AdapterDetector = dataclasses.field(default_factory=AdapterDetector)
 
     # whether to create a new __init__ function
     create_init_func: bool = True
 
@@ -160,45 +164,70 @@
             # Theoretically this can happen if someone writes
             # a custom string to cls.__module__.  In which case
             # such dataclass won't be fully introspectable
             # (w.r.t. typing.get_type_hints) but will still function
             # correctly.
             self.globals = {}
 
+    def _create_fn(self, name: str, args: List[str], body: List[str], *,
+                   _globals: Dict[str, Any] = None,
+                   _locals: Dict[str, Any] = None,
+                   return_type: Optional[Type] = MISSING):
+        _globals = _globals or self.globals or {}
+
+        # Note that we mutate locals when exec() is called.  Caller
+        # beware!  The only callers are internal to this module, so no
+        # worries about external callers.
+        if _locals is None:
+            _locals = {}
+        if 'BUILTINS' not in _locals:
+            _locals['BUILTINS'] = builtins
+        return_annotation = ''
+        if return_type is not MISSING:
+            _locals['_return_type'] = return_type
+            return_annotation = '->_return_type'
+        args = ','.join(args)
+        body = '\n'.join(f'  {b}' for b in body)
+
+        # Compute the text of the entire function.
+        txt = f' def {name}({args}){return_annotation}:\n{body}'
+
+        local_vars = ', '.join(_locals.keys())
+        txt = f"def __create_fn__({local_vars}):\n{txt}\n return {name}"
+
+        ns = {}
+        exec(txt, _globals, ns)
+        return ns['__create_fn__'](**_locals)
+
     @staticmethod
     def is_missing(value: Any) -> bool:
         return value is MISSING
 
     @staticmethod
     def _is_classvar(a_type, typing):
         return dataclasses._is_classvar(a_type, typing)
 
     @staticmethod
-    def _is_objectvar(a_type, module):
-        # The module we're checking against is the module we're currently in.
-        return (a_type is module.ObjectVar or type(a_type) is module.ObjectVar)
-
-    @staticmethod
     def _is_type(annotation, cls, a_module, a_type, is_type_predicate):
         return dataclasses._is_type(annotation, cls, a_module, a_type, is_type_predicate)
 
     def get_field(self, cls, a_name, a_type) -> Field:
         """
         Return a Field object for this field name and type.
         """
         # If the default value isn't derived from Field, then it's only a
         # normal default value.  Convert it to a Field().
-        default = getattr(cls, a_name, self.config.default_field_value)
+        default = getattr(cls, a_name, MISSING)
         if isinstance(default, Field):
             f = default
         else:
             if isinstance(default, types.MemberDescriptorType):
                 # This is a field in __slots__, so it has no default value.
-                default = self.config.default_field_value
-            f = Field(default=default)
+                default = MISSING
+            f = Field(init_default=default)
 
         # Only at this point do we know the name and the type.  Set them.
         f.name = a_name
         f.type = a_type
 
         # If missing key, set as name.
         if self.is_missing(f.key):
@@ -226,49 +255,36 @@
         typing = sys.modules.get('typing')
         if typing:
             if (self._is_classvar(a_type, typing)
                     or (isinstance(f.type, str)
                         and self._is_type(f.type, cls, typing, typing.ClassVar, self._is_classvar))):
                 f._field_type = _FIELD_CLASSVAR
 
-        # If the type is ObjectVar, or if it's a matching string annotation,
-        # then it's an ObjectVar.
-        if f._field_type is _FIELD_DICTKEY:
-            # The module we're checking against is the module we're currently in.
-            module = sys.modules[__name__]
-            if (self._is_objectvar(a_type, module)
-                    or (isinstance(f.type, str)
-                        and self._is_type(f.type, cls, dataclasses, dataclasses.InitVar, self._is_objectvar))):
-                f._field_type = _FIELD_OBJECTVAR
-
         # Validations for individual fields.  This is delayed until now,
         # instead of in the Field() constructor, since only here do we
         # know the field name, which allows for better error reporting.
 
         # Special restrictions for ClassVar.
         if f._field_type is _FIELD_CLASSVAR:
-            if not self.is_missing(f.default_factory):
+            if not self.is_missing(f.init_default_factory):
                 raise TypeError(f'field {f.name} cannot have a default factory')
             # Should I check for other field settings? default_factory
             # seems the most serious to check for.  Maybe add others.  For
             # example, how about init=False (or really,
             # init=<not-the-default-init-value>)?  It makes no sense for
             # ClassVar and InitVar to specify init=<anything>.
 
         # For real fields, disallow mutable defaults for known types.
-        if (f._field_type in (_FIELD_DICTKEY, _FIELD_OBJECTVAR)
-                and isinstance(f.default, (list, dict, set))):
-            raise ValueError(f'mutable default {type(f.default)} for field '
-                             f'{f.name} is not allowed: use default_factory')
-
-        # Set value if f is ClassVar or ObjectVar.
-        if f._field_type is _FIELD_CLASSVAR:
-            f.static = True
-        if f._field_type is _FIELD_OBJECTVAR:
-            f.exclude = True
+        if f._field_type in (_FIELD_DICTKEY, _FIELD_OBJECTVAR):
+            if isinstance(f.getter_default, (list, dict, set)):
+                raise ValueError(f'mutable getter_default {type(f.getter_default)} for field '
+                                 f'{f.name} is not allowed: use getter_default_factory0 or getter_default_factory1')
+            if isinstance(f.init_default, (list, dict, set)):
+                raise ValueError(f'mutable init_default {type(f.init_default)} for field '
+                                 f'{f.name} is not allowed: use init_default_factory')
 
         # if encoder/decoder set auto, detect whether an encoder/decoder is needed
         if f.encoder == 'auto':
             f.encoder = self.config.adapter_detector.detect_encoder(f.type)
         if f.decoder == 'auto':
             f.decoder = self.config.adapter_detector.detect_decoder(f.type)
 
@@ -287,62 +303,94 @@
         # Never overwrites an existing attribute.  Returns True if the
         # attribute already exists.
         if name in cls.__dict__:
             return True
         setattr(cls, name, value)
         return False
 
-    def build_getter(self, field: Field) -> Callable[[dict], Any]:
-        if not self.is_missing(field.default):
-            if callable(field.decoder):
-                def getter(d):
-                    if field.key in d:
-                        return field.decoder(d[field.key])
-                    return field.default
-            else:
-                def getter(d):
-                    return d.get(field.key, field.default)
-        elif not self.is_missing(field.default_factory):
-            if callable(field.decoder):
-                def getter(d):
-                    if field.key in d:
-                        return field.decoder(d[field.key])
-                    return field.default_factory(d)
-            else:
-                def getter(d):
-                    if field.key in d:
-                        return d[field.key]
-                    return field.default_factory(d)
+    def build_getter(self, field: Field, *, method_name='getter', var_dict='_d', var_key='_key',
+                     var_decoder='_decoder', var_default='_default') -> Callable[[dict], Any]:
+        _locals: dict = {
+            var_key: field.key,
+        }
+
+        should_decode = callable(field.decoder)
+        if should_decode:
+            _locals[var_decoder] = field.decoder
+
+        if field.getter_default is not MISSING:
+            default_type, default_value = 0, field.getter_default
+        elif field.getter_default_factory0 is not MISSING:
+            default_type, default_value = 1, field.getter_default_factory0
+        elif field.getter_default_factory1 is not MISSING:
+            default_type, default_value = 2, field.getter_default_factory1
+        elif self.config.getter_default is not MISSING:
+            default_type, default_value = 0, self.config.getter_default
         else:
-            if callable(field.decoder):
-                def getter(d):
-                    return field.decoder(d[field.key])
+            default_type, default_value = -2, None
+
+        def gen_body_lines() -> List[str]:
+            if default_type == -2:
+                # if no default defined, just get key value and decode
+                if should_decode:
+                    return [f"return {var_decoder}({var_dict}[{var_key}])"]
+                return [f"return {var_dict}[{var_key}]"]
+            lines = [f"if {var_key} in {var_dict}:"]
+            if should_decode:
+                lines.append(f" return {var_decoder}({var_dict}[{var_key}])")
             else:
-                def getter(d):
-                    return d[field.key]
-        return getter
-
-    def build_setter(self, field: Field) -> Callable[[dict, Any], Any]:
-        if callable(field.encoder):
-            def setter(d, value):
-                d[field.key] = field.encoder(value)
+                lines.append(f" return {var_dict}[{var_key}]")
+            _locals[var_default] = default_value
+            if default_type == 0:
+                lines.append(f"return {var_default}")
+            elif default_type == 1:
+                lines.append(f"return {var_default}()")
+            else:
+                assert default_type == 2
+                lines.append(f"return {var_default}({var_dict})")
+            return lines
+
+        body_lines = gen_body_lines()
+
+        return self._create_fn(method_name, [var_dict], body_lines, _locals=_locals)
+
+    def build_setter(self, field: Field, *, method_name='setter', var_dict='_d', var_value='_value',
+                     var_key='_key', var_encoder='_encoder') -> Callable[[dict, Any], Any]:
+        _locals: dict = {
+            var_key: field.key,
+        }
+
+        should_encode = callable(field.encoder)
+        if should_encode:
+            _locals[var_encoder] = field.encoder
+
+        if should_encode:
+            body_lines = [f"{var_dict}[{var_key}] = {var_encoder}({var_value})"]
         else:
-            def setter(d, value):
-                d[field.key] = value
-        return setter
+            body_lines = [f"{var_dict}[{var_key}] = {var_value}"]
+
+        return self._create_fn(method_name, [var_dict, var_value], body_lines, _locals=_locals)
+
+    def build_deleter(self, field: Field, *, method_name='deleter', var_dict='_d',
+                      var_key='_key') -> Callable[[dict], Any]:
+        _locals: dict = {
+            var_key: field.key,
+        }
 
-    def build_deleter(self, field: Field) -> Callable[[dict], Any]:
         if field.check_exist_before_delete:
-            def deleter(d):
-                if field.key in d:
-                    d.pop(field.key)
+            body_lines = [
+                f"if {var_key} in {var_dict}:",
+                f" {var_dict}.pop({var_key})",
+            ]
         else:
-            def deleter(d):
-                d.pop(field.key)
-        return deleter
+            body_lines = [
+                f"{var_dict}.pop({var_key})",
+            ]
+
+        return self._create_fn(method_name, [var_dict], body_lines, _locals=_locals)
 
     def build_property(self, field: Field) -> property:
         return property(fget=self.build_getter(field) if field.readable else None,
                         fset=self.build_setter(field) if field.writeable else None,
                         fdel=self.build_deleter(field) if field.deletable else None)
 
     def add_base(self):
@@ -391,30 +439,23 @@
         cls_annotations = cls.__dict__.get('__annotations__', {})
 
         # Now find fields in our class.  While doing so, validate some
         # things, and set the default values (as class attributes) where
         # we can.
         for name, a_type in cls_annotations.items():
             field = self.get_field(cls, name, a_type)
-            if field.static:
-                # It's not suggested to define a class field in this way.
-                if self.is_missing(field.default):
-                    delattr(cls, name)
-                else:
-                    setattr(cls, name, field.default)
-            elif field.exclude:
-                if self.is_missing(field.default) and self.is_missing(field.default_factory):
-                    delattr(cls, name)
-                elif not self.is_missing(field.default):
-                    # Actually it should be set to the obj when init,
-                    # this is a temp way to set as a class value.
-                    setattr(cls, name, field.default)
-                else:
-                    # Rare situation should set a dynamic default value.
-                    raise ValueError("not allowed to specify a factory.")
+            if field._field_type is _FIELD_CLASSVAR:
+                # It's not suggested to define a class field like `a: ClassVar[int] = Field(init_default=1)`.
+                # better to define like `a: ClassVar[int] = 1`.
+                # But deal field here just in case.
+                if isinstance(getattr(cls, field.name, None), Field):
+                    if self.is_missing(field.init_default):
+                        delattr(cls, name)
+                    else:
+                        setattr(cls, name, field.init_default)
             else:
                 setattr(cls, name, self.build_property(field))
                 fields[name] = field
 
         # Do we have any Field members that don't also have annotations?
         for name, value in cls.__dict__.items():
             if isinstance(value, Field) and name not in cls_annotations:
@@ -422,104 +463,76 @@
 
         # Remember all of the fields on our class (including bases).  This
         # also marks this class as being a json_object.
         setattr(cls, _FIELDS, fields)
 
         self.fields = fields
 
-    def _create_fn(self, name: str, args: List[str], body: List[str], *,
-                   _globals: Dict[str, Any] = None,
-                   _locals: Dict[str, Any] = None,
-                   return_type: Optional[Type] = MISSING):
-        _globals = _globals or self.globals or {}
-
-        # Note that we mutate locals when exec() is called.  Caller
-        # beware!  The only callers are internal to this module, so no
-        # worries about external callers.
-        if _locals is None:
-            _locals = {}
-        if 'BUILTINS' not in _locals:
-            _locals['BUILTINS'] = builtins
-        return_annotation = ''
-        if return_type is not MISSING:
-            _locals['_return_type'] = return_type
-            return_annotation = '->_return_type'
-        args = ','.join(args)
-        body = '\n'.join(f'  {b}' for b in body)
-
-        # Compute the text of the entire function.
-        txt = f' def {name}({args}){return_annotation}:\n{body}'
-
-        local_vars = ', '.join(_locals.keys())
-        txt = f"def __create_fn__({local_vars}):\n{txt}\n return {name}"
-
-        ns = {}
-        exec(txt, _globals, ns)
-        return ns['__create_fn__'](**_locals)
-
     @staticmethod
     def _field_assign(frozen, name, value, self_name):
         # If we're a frozen class, then assign to our fields in __init__
         # via object.__setattr__.  Otherwise, just use a simple
         # assignment.
         #
         # self_name is what "self" is called in this function: don't
         # hard-code "self", since that might be a field name.
         if frozen:
             return f'BUILTINS.object.__setattr__({self_name},{name!r},{value})'
         return f'{self_name}.{name}={value}'
 
     def _init_fn(self, fields: List[Field], self_name: str, d_name='_', ds_name='__', kwargs_name='___'):
-        # fields contains both real fields and InitVar pseudo-fields.
-
-        locals: dict = {
+        _locals: dict = {
             'MISSING': MISSING,
             'dict': dict,
         }
-        locals.update((f'_type_{f.name}', f.type) for f in fields)
-        locals.update((f'_key_{f.name}', f.key) for f in fields)
+        _locals.update((f'_type_{f.name}', f.type) for f in fields)
+        _locals.update((f'_key_{f.name}', f.key) for f in fields)
 
         # all args
         args = [self_name, f'*{ds_name}:dict'] + [f'{f.name}:_type_{f.name}=MISSING' for f in fields]
         if kwargs_name:
             args.append(f'**{kwargs_name}')
 
+        # default values
+        body_lines = []
+        for f in fields:
+            if not self.is_missing(f.init_default):
+                _locals[f'_default_{f.name}'] = f.init_default
+                body_lines.append(f"{self_name}[_key_{f.name}] = _default_{f.name}")
+            elif not self.is_missing(f.init_default_factory):
+                _locals[f'_default_{f.name}'] = f.init_default_factory
+                body_lines.append(f"{self_name}[_key_{f.name}] = _default_{f.name}()")
+
         # update by given dicts
-        body_lines = [
+        body_lines.extend([
             f"for {d_name} in {ds_name}:",
             f" {self_name}.update({d_name})",
-        ]
+        ])
 
         # update by kwargs
         if kwargs_name:
             body_lines.append(f"{self_name}.update({kwargs_name})")
 
         # update by name
         for f in fields:
             if f._field_type is _FIELD_DICTKEY:
                 # value stored in dict would be correctly encoded by setting with `.`
                 body_lines.extend([
                     f"if {f.name} is not MISSING:",
                     f" {self_name}.{f.name} = {f.name}",
                     f"elif _key_{f.name} in {self_name}:",
-                    f" {self_name}.{f.name} = {self_name}[_key_{f.name}]"
+                    f" {self_name}.{f.name} = {self_name}[_key_{f.name}]",
                 ])
             elif f._field_type is _FIELD_CLASSVAR:
                 body_lines.extend([
                     f"if {f.name} is not MISSING:",
                     f" {self_name}.{f.name} = {f.name}",
                 ])
 
-        # body lines would not be empty
-        # If no body lines, use 'pass'.
-        # if not body_lines:
-        #     body_lines = ['pass']
-
-        return self._create_fn('__init__', args, body_lines,
-                               _locals=locals, return_type=None)
+        return self._create_fn('__init__', args, body_lines, _locals=_locals)
 
     def add_init_func(self):
         """
         add __init__ function
         """
         # Include InitVars and regular fields (so, not ClassVars).
         allowed_field_types = (
@@ -636,23 +649,23 @@
     def __call__(self, cls: type = None) -> Type[dict]:
         if cls is not None:
             self._reset(cls)
         self._process()
         return self.cls
 
 def json_object(_cls=None, processor=JsonObjectClassProcessor, config=None,
-                default_field_value=None, adapter_detector: AdapterDetector = None,
+                getter_default=None, adapter_detector: AdapterDetector = None,
                 create_init_func=True, create_iter_func=True, iter_func_name='field_items',
                 **kwargs):
     """
     a decorator to mark a class as json format
     """
     if config is None:
         config = ProcessorConfig(
-            default_field_value=default_field_value,
+            getter_default=getter_default,
             adapter_detector=adapter_detector or AdapterDetector(),
             create_init_func=create_init_func,
             create_iter_func=create_iter_func,
             iter_func_name=iter_func_name,
             **kwargs
         )
 
@@ -666,54 +679,7 @@
     if _cls is None:
         # We're called with parens.
         return wrap
 
     # We're called as @json_object without parens.
     return wrap(_cls)
 
-# Another way to define a json_object class, just inherit this class.
-class JsonObject(dict):
-    def __init_subclass__(cls):
-        warnings.warn("Use decorator `json_object()` instead", DeprecationWarning)
-        super().__init_subclass__()
-        JsonObjectClassProcessor()(cls)
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        fields = getattr(self, _FIELDS, {})
-        for f in fields.values():
-            if callable(f.encoder):
-                value = self.get(f.key)
-                self[f.key] = f.encoder(value)
-
-    def field_items(self) -> Iterable[Tuple[str, Any]]:
-        """
-        iter of defined field values
-        """
-        # one should not define a field use the reserved name
-        fields = getattr(self, _FIELDS, {})
-        for name, field in fields.items():
-            if field.key in self:
-                yield name, self[field.key]
-
-    @property
-    def _iter_field_items_only(self) -> bool:
-        """
-        determine output of method items(): if `True`, same as field_items(); else same as dict.items()
-        """
-        return False
-
-    def items(self) -> Iterable[Tuple[str, Any]]:
-        if self._iter_field_items_only:
-            return self.field_items()
-        return super().items()
-
-    @classmethod
-    def from_dict(cls, d: Dict[str, Any]) -> 'JsonObject':
-        """
-        This method can be overwritten for custom use.
-        """
-        return cls(d)
-
-    @classmethod
-    def from_list(cls, li: List[Dict[str, Any]]) -> List['JsonObject']:
-        return [cls.from_dict(x) for x in li]
```

### Comparing `flexible_dict-1.2.3/flexible_dict/script/class_builder.py` & `flexible_dict-2.0.0/flexible_dict/script/class_builder.py`

 * *Files identical despite different names*

### Comparing `flexible_dict-1.2.3/flexible_dict.egg-info/PKG-INFO` & `flexible_dict-2.0.0/flexible_dict.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flexible_dict
-Version: 1.2.3
+Version: 2.0.0
 Summary: A flexible way to access dict data instead of built-in dict.
 Author-email: darkpeath <darkpeath@gmail.com>
 Project-URL: Homepage, https://github.com/darkpeath/flexible_dict
 Description-Content-Type: text/markdown
 Requires-Dist: dataclasses; python_version < "3.7"
 Requires-Dist: typing_extensions; python_version < "3.8"
```

### Comparing `flexible_dict-1.2.3/pyproject.toml` & `flexible_dict-2.0.0/pyproject.toml`

 * *Files identical despite different names*

