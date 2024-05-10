# Comparing `tmp/avrotize-1.4.0.tar.gz` & `tmp/avrotize-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avrotize-1.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "avrotize-1.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `avrotize-1.4.0.tar` & `avrotize-1.4.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    26753 2024-05-08 18:17:46.279981 avrotize-1.4.0/README.md
--rw-r--r--   0        0        0     1673 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/__init__.py
--rw-r--r--   0        0        0       88 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/__main__.py
--rw-r--r--   0        0        0      411 2024-05-08 18:17:50.779965 avrotize-1.4.0/avrotize/_version.py
--rw-r--r--   0        0        0     8386 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/asn1toavro.py
--rw-r--r--   0        0        0    15557 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/avrotize.py
--rw-r--r--   0        0        0    43143 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/avrotocsharp.py
--rw-r--r--   0        0        0    50347 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/avrotojava.py
--rw-r--r--   0        0        0    12117 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/avrotojs.py
--rw-r--r--   0        0        0    18104 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/avrotojsons.py
--rw-r--r--   0        0        0     5155 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/avrotokusto.py
--rw-r--r--   0        0        0     5481 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/avrotoparquet.py
--rw-r--r--   0        0        0    22200 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/avrotoproto.py
--rw-r--r--   0        0        0    13101 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/avrotopython.py
--rw-r--r--   0        0        0    10166 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/avrotots.py
--rw-r--r--   0        0        0     9514 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/avrototsql.py
--rw-r--r--   0        0        0    16313 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/avrotoxsd.py
--rw-r--r--   0        0        0    13663 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/common.py
--rw-r--r--   0        0        0    19374 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/dependency_resolver.py
--rw-r--r--   0        0        0     1272 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/generic/generic.avsc
--rw-r--r--   0        0        0    95346 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/jsonstoavro.py
--rw-r--r--   0        0        0     2112 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/kconnect.json
--rw-r--r--   0        0        0     2537 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/kstructtoavro.py
--rw-r--r--   0        0        0    19742 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/proto2parser.py
--rw-r--r--   0        0        0    15536 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/proto3parser.py
--rw-r--r--   0        0        0     8722 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/prototoavro.py
--rw-r--r--   0        0        0     3390 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/prototypes/any.avsc
--rw-r--r--   0        0        0     6521 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/prototypes/api.avsc
--rw-r--r--   0        0        0     1629 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/prototypes/duration.avsc
--rw-r--r--   0        0        0     3558 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/prototypes/field_mask.avsc
--rw-r--r--   0        0        0     2394 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/prototypes/struct.avsc
--rw-r--r--   0        0        0      792 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/prototypes/timestamp.avsc
--rw-r--r--   0        0        0     6296 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/prototypes/type.avsc
--rw-r--r--   0        0        0     2571 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/prototypes/wrappers.avsc
--rw-r--r--   0        0        0    17371 2024-05-08 18:17:46.283981 avrotize-1.4.0/avrotize/xsdtoavro.py
--rw-r--r--   0        0        0     1138 2024-05-08 18:17:46.283981 avrotize-1.4.0/pyproject.toml
--rw-r--r--   0        0        0    27420 1970-01-01 00:00:00.000000 avrotize-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0    26753 2024-05-10 15:20:18.212851 avrotize-1.4.1/README.md
+-rw-r--r--   0        0        0     1673 2024-05-10 15:20:18.212851 avrotize-1.4.1/avrotize/__init__.py
+-rw-r--r--   0        0        0       88 2024-05-10 15:20:18.212851 avrotize-1.4.1/avrotize/__main__.py
+-rw-r--r--   0        0        0      411 2024-05-10 15:20:22.324847 avrotize-1.4.1/avrotize/_version.py
+-rw-r--r--   0        0        0     8386 2024-05-10 15:20:18.212851 avrotize-1.4.1/avrotize/asn1toavro.py
+-rw-r--r--   0        0        0    15557 2024-05-10 15:20:18.212851 avrotize-1.4.1/avrotize/avrotize.py
+-rw-r--r--   0        0        0    43154 2024-05-10 15:20:18.212851 avrotize-1.4.1/avrotize/avrotocsharp.py
+-rw-r--r--   0        0        0    58115 2024-05-10 15:20:18.212851 avrotize-1.4.1/avrotize/avrotojava.py
+-rw-r--r--   0        0        0    12117 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/avrotojs.py
+-rw-r--r--   0        0        0    18104 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/avrotojsons.py
+-rw-r--r--   0        0        0     5155 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/avrotokusto.py
+-rw-r--r--   0        0        0     5481 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/avrotoparquet.py
+-rw-r--r--   0        0        0    22200 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/avrotoproto.py
+-rw-r--r--   0        0        0    13360 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/avrotopython.py
+-rw-r--r--   0        0        0    10166 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/avrotots.py
+-rw-r--r--   0        0        0     9514 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/avrototsql.py
+-rw-r--r--   0        0        0    16313 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/avrotoxsd.py
+-rw-r--r--   0        0        0    13663 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/common.py
+-rw-r--r--   0        0        0    19374 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/dependency_resolver.py
+-rw-r--r--   0        0        0     1272 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/generic/generic.avsc
+-rw-r--r--   0        0        0    95346 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/jsonstoavro.py
+-rw-r--r--   0        0        0     2112 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/kconnect.json
+-rw-r--r--   0        0        0     2537 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/kstructtoavro.py
+-rw-r--r--   0        0        0    19742 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/proto2parser.py
+-rw-r--r--   0        0        0    15536 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/proto3parser.py
+-rw-r--r--   0        0        0     8722 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/prototoavro.py
+-rw-r--r--   0        0        0     3390 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/prototypes/any.avsc
+-rw-r--r--   0        0        0     6521 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/prototypes/api.avsc
+-rw-r--r--   0        0        0     1629 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/prototypes/duration.avsc
+-rw-r--r--   0        0        0     3558 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/prototypes/field_mask.avsc
+-rw-r--r--   0        0        0     2394 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/prototypes/struct.avsc
+-rw-r--r--   0        0        0      792 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/prototypes/timestamp.avsc
+-rw-r--r--   0        0        0     6296 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/prototypes/type.avsc
+-rw-r--r--   0        0        0     2571 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/prototypes/wrappers.avsc
+-rw-r--r--   0        0        0    17371 2024-05-10 15:20:18.216851 avrotize-1.4.1/avrotize/xsdtoavro.py
+-rw-r--r--   0        0        0     1138 2024-05-10 15:20:18.216851 avrotize-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0    27420 1970-01-01 00:00:00.000000 avrotize-1.4.1/PKG-INFO
```

### Comparing `avrotize-1.4.0/README.md` & `avrotize-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.0/avrotize/__init__.py` & `avrotize-1.4.1/avrotize/__init__.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.0/avrotize/asn1toavro.py` & `avrotize-1.4.1/avrotize/asn1toavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.0/avrotize/avrotize.py` & `avrotize-1.4.1/avrotize/avrotize.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.0/avrotize/avrotocsharp.py` & `avrotize-1.4.1/avrotize/avrotocsharp.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,15 +159,15 @@
         _ => throw new NotSupportedException("Data is not of a supported type for conversion to Stream")
     };
     if (contentType.MediaType.StartsWith("avro/binary") || contentType.MediaType.StartsWith("application/vnd.apache.avro+avro"))
     {
         var reader = new Avro.Specific.SpecificDatumReader<{type_name}>({type_name}.AvroSchema, {type_name}.AvroSchema);
         return reader.Read(new {type_name}(), new Avro.IO.BinaryDecoder(stream));
     }
-    if ( contentType.MediaType.StartsWith("avro/json") || contentType.MediaType.StartsWith("application/avro+json"))
+    if ( contentType.MediaType.StartsWith("avro/json") || contentType.MediaType.StartsWith("application/vnd.apache.avro+json"))
     {
         var reader = new Avro.Specific.SpecificDatumReader<{type_name}>({type_name}.AvroSchema, {type_name}.AvroSchema);
         return reader.Read(new {type_name}(), new Avro.IO.JsonDecoder({type_name}.AvroSchema, stream));
     }
 }    
 """
```

### Comparing `avrotize-1.4.0/avrotize/avrotojava.py` & `avrotize-1.4.1/avrotize/avrotojava.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 INDENT = '    '
 POM_CONTENT = """<?xml version="1.0" encoding="UTF-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0"
     xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
     xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
     <modelVersion>4.0.0</modelVersion>
-    <groupId>com.example</groupId>
-    <artifactId>demo</artifactId>
+    <groupId>{groupid}</groupId>
+    <artifactId>{artifactid}</artifactId>
     <version>1.0-SNAPSHOT</version>
     <properties>
         <maven.compiler.source>21</maven.compiler.source>
         <maven.compiler.target>21</maven.compiler.target>
     </properties>
     <dependencies>
         <dependency>
@@ -87,19 +87,26 @@
         e.printStackTrace();
     }
 }
 """
 
 
 JSON_FROMDATA_THROWS = \
-    ",JsonProcessingException"
+    ",JsonProcessingException, IOException"
 JSON_FROMDATA = \
     """
 if ( mediaType == "application/json") {
-    if (data instanceof JsonNode) {
+    if (data instanceof byte[]) {
+        ByteArrayInputStream stream = new ByteArrayInputStream((byte[]) data);
+        return (new ObjectMapper()).readValue(stream, {typeName}.class);
+    }
+    else if (data instanceof InputStream) {
+        return (new ObjectMapper()).readValue((InputStream)data, {typeName}.class);
+    }
+    else if (data instanceof JsonNode) {
         return (new ObjectMapper()).readValue(((JsonNode)data).toString(), {typeName}.class);
     }
     else if ( data instanceof String) {
         return (new ObjectMapper()).readValue(((String)data), {typeName}.class);
     }
     throw new UnsupportedOperationException("Data is not of a supported type for JSON conversion to {typeName}");
 }
@@ -111,33 +118,55 @@
     result = new ObjectMapper().writeValueAsBytes(this);
 }
 """
 
 AVRO_FROMDATA_THROWS = ",IOException"
 AVRO_FROMDATA = \
     """
-if ( mediaType == "application/avro") {
-    DatumReader<{typeName}> reader = new SpecificDatumReader<>({typeName}.class);
-    Decoder decoder = DecoderFactory.get().binaryDecoder((byte[])data, null);
-    return reader.read(null, decoder);
+if ( mediaType == "avro/binary" || mediaType == "application/vnd.apache.avro+avro") {
+    DatumReader<{typeName}> reader = new SpecificDatumReader<{typeName}>({typeName}.AvroSchema);
+    if (data instanceof byte[]) {
+        return reader.read(new {typeName}(), DecoderFactory.get().binaryDecoder((byte[])data, null));
+    } else if (data instanceof InputStream) {
+        return reader.read(new {typeName}(), DecoderFactory.get().binaryDecoder((InputStream)data, null));
+    }
+    throw new UnsupportedOperationException("Data is not of a supported type for Avro conversion to {typeName}");
+} else if ( mediaType == "avro/json" || mediaType == "application/vnd.apache.avro+json") {
+    DatumReader<{typeName}> reader = new SpecificDatumReader<{typeName}>({typeName}.AvroSchema);
+    if (data instanceof byte[]) {
+        return reader.read(new {typeName}(), DecoderFactory.get().jsonDecoder({typeName}.AvroSchema, new ByteArrayInputStream((byte[])data)));
+    } else if (data instanceof InputStream) {
+        return reader.read(new {typeName}(), DecoderFactory.get().jsonDecoder({typeName}.AvroSchema, (InputStream)data));
+    } else if (data instanceof String) {
+        return reader.read(new {typeName}(), DecoderFactory.get().jsonDecoder({typeName}.AvroSchema, (String)data));
+    }
+    throw new UnsupportedOperationException("Data is not of a supported type for Avro conversion to {typeName}");
 }
 """
 
 
 AVRO_TOBYTEARRAY_THROWS = ",IOException"
 AVRO_TOBYTEARRAY = \
     """
-if ( mediaType == "application/avro") {
-    DatumWriter<{typeName}> writer = new SpecificDatumWriter<>({typeName}.class);
+if ( mediaType == "avro/binary" || mediaType == "application/vnd.apache.avro+avro") {
+    DatumWriter<{typeName}> writer = new SpecificDatumWriter<{typeName}>({typeName}.AvroSchema);
     ByteArrayOutputStream out = new ByteArrayOutputStream();
     Encoder encoder = EncoderFactory.get().binaryEncoder(out, null);
     writer.write(this, encoder);
     encoder.flush();
     result = out.toByteArray();
 }
+else if ( mediaType == "avro/json" || mediaType == "application/vnd.apache.avro+json") {
+    DatumWriter<{typeName}> writer = new SpecificDatumWriter<{typeName}>({typeName}.AvroSchema);
+    ByteArrayOutputStream out = new ByteArrayOutputStream();
+    Encoder encoder = EncoderFactory.get().jsonEncoder({typeName}.AvroSchema, out);
+    writer.write(this, encoder);
+    encoder.flush();
+    result = out.toByteArray();
+}
 """
 
 
 JsonNode = Dict[str, 'JsonNode'] | List['JsonNode'] | str | None
 
 
 def flatten_type_name(name: str) -> str:
@@ -166,33 +195,36 @@
 
     def __init__(self, base_package: str = '') -> None:
         self.base_package = base_package.replace('.', '/')
         self.output_dir = os.getcwd()
         self.avro_annotation = False
         self.jackson_annotations = False
         self.pascal_properties = False
-        self.generated_types: Dict[str,str] = {}
+        self.generated_types_avro_namespace: Dict[str,str] = {}
+        self.generated_types_java_package: Dict[str,str] = {}
 
     def concat_package(self, package: str, name: str) -> str:
         """Concatenates package and name using a dot separator"""
         return f"{package.lower()}.{name}" if package else name
 
     class JavaType:
         """Java type definition"""
 
         def __init__(self, type_name: str, union_types: List['AvroToJava.JavaType'] | None = None, is_class: bool = False, is_enum: bool = False) -> None:
             self.type_name = type_name
             self.union_types = union_types
             self.is_class = is_class
             self.is_enum = is_enum
 
-    def safe_identifier(self, name: str) -> str:
+    def safe_identifier(self, name: str, class_name: str = '') -> str:
         """Converts a name to a safe Java identifier"""
         if is_java_reserved_word(name):
             return f"_{name}"
+        if class_name and name == class_name:
+            return f"{name}_"
         return name
     
     def map_primitive_to_java(self, avro_type: str, is_optional: bool) -> JavaType:
         """Maps Avro primitive types to Java types"""
         optional_mapping = {
             'null': 'Void',
             'boolean': 'Boolean',
@@ -213,17 +245,18 @@
             'bytes': 'byte[]',
             'string': 'String',
         }
         if '.' in avro_type:
             type_name = avro_type.split('.')[-1]
             package_name = '.'.join(avro_type.split('.')[:-1]).lower()
             avro_type = self.concat_package(package_name, type_name)
-        if avro_type in self.generated_types:
-            kind = self.generated_types[avro_type]
-            return AvroToJava.JavaType(avro_type, is_class=kind=="class", is_enum=kind=="enum")
+        if avro_type in self.generated_types_avro_namespace:
+            kind = self.generated_types_avro_namespace[avro_type]
+            qualified_class_name = self.concat_package(self.base_package, avro_type)
+            return AvroToJava.JavaType(qualified_class_name, is_class=kind=="class", is_enum=kind=="enum")
         else:
             return AvroToJava.JavaType(required_mapping.get(avro_type, avro_type) if not is_optional else optional_mapping.get(avro_type, avro_type))
     
     def is_java_primitive(self, java_type: JavaType) -> bool:
         """Checks if a Java type is a primitive type"""
         return java_type.type_name in [
             'void', 'boolean', 'int', 'long', 'float', 'double', 'byte[]', 'String',
@@ -298,35 +331,53 @@
         return AvroToJava.JavaType('Object')
 
     def generate_class(self, avro_schema: Dict, parent_package: str, write_file: bool) -> JavaType:
         """ Generates a Java class from an Avro record schema """
         class_definition = ''
         if 'doc' in avro_schema:
             class_definition += f"/** {avro_schema['doc']} */\n"
-        package = self.concat_package(self.base_package, avro_schema.get('namespace', parent_package)).replace('.', '/').lower()
+        namespace = avro_schema.get('namespace', parent_package)
+        if not 'namespace' in avro_schema:
+            avro_schema['namespace'] = namespace
+        package = self.concat_package(self.base_package, namespace).replace('.', '/').lower()
         class_name = self.safe_identifier(avro_schema['name'])
-        self.generated_types[self.concat_package(avro_schema.get('namespace', parent_package),avro_schema['name'])] = "class"
-        fields_str = [self.generate_property(class_name,
-            field, avro_schema.get('namespace', parent_package)) for field in avro_schema.get('fields', [])]
+        namespace_qualified_name = self.concat_package(namespace,avro_schema['name'])
+        qualified_class_name = self.concat_package(package.replace('/', '.'), class_name)
+        if namespace_qualified_name in self.generated_types_avro_namespace:
+            return AvroToJava.JavaType(qualified_class_name, is_class=True)
+        self.generated_types_avro_namespace[namespace_qualified_name] = "class"
+        self.generated_types_java_package[qualified_class_name] = "class"
+        fields_str = [self.generate_property(class_name, field, namespace) for field in avro_schema.get('fields', [])]
         class_body = "\n".join(fields_str)
         class_definition += f"public class {class_name}"
         if self.avro_annotation:
             class_definition += " implements SpecificRecord"
         class_definition += " {\n"
+        class_definition += f"{INDENT}public {class_name}() {{}}\n"
         class_definition += class_body
+        
+        if self.avro_annotation:
+            class_definition += f"\n{INDENT}public {class_name}(GenericData.Record record) {{\n"
+            class_definition += f"{INDENT*2}for( int i = 0; i < record.getSchema().getFields().size(); i++ ) {{\n"
+            class_definition += f"{INDENT*3}this.put(i, record.get(i));\n"
+            class_definition += f"{INDENT*2}}}\n"
+            class_definition += f"{INDENT}}}\n"
+        
         if self.avro_annotation:
             avro_schema_json = json.dumps(avro_schema)
             avro_schema_json = avro_schema_json.replace('"', '§')
             avro_schema_json = f"\"+\n{INDENT}\"".join(
                 [avro_schema_json[i:i+80] for i in range(0, len(avro_schema_json), 80)])
             avro_schema_json = avro_schema_json.replace('§', '\\"')
             class_definition += f"\n\n{INDENT}public static Schema AvroSchema = new Schema.Parser().parse(\n{INDENT}\"{avro_schema_json}\");\n"
+            if self.jackson_annotations:
+                class_definition += f"\n{INDENT}@JsonIgnore"
             class_definition += f"\n{INDENT}@Override\n{INDENT}public Schema getSchema(){{ return AvroSchema; }}\n"
-            class_definition += self.generate_get_method(avro_schema.get('fields', []), package)
-            class_definition += self.generate_put_method(class_name, avro_schema.get('fields', []), package)
+            class_definition += self.generate_avro_get_method(class_name, avro_schema.get('fields', []), namespace)
+            class_definition += self.generate_avro_put_method(class_name, avro_schema.get('fields', []), namespace)
 
         # emit toByteArray method
         class_definition += f"\n\n{INDENT}/**\n{INDENT} * Converts the object to a byte array\n{INDENT} * @param contentType the content type of the byte array\n{INDENT} * @return the byte array\n{INDENT} */\n"
         class_definition += f"\n\n{INDENT}public byte[] toByteArray(String contentType) throws UnsupportedOperationException" + \
             f"{ JSON_TOBYTEARRAY_THROWS if self.jackson_annotations else '' }" + \
             f"{ AVRO_TOBYTEARRAY_THROWS if self.avro_annotation else '' }  {{"
         if self.jackson_annotations or self.avro_annotation:
@@ -357,22 +408,21 @@
                 AVRO_FROMDATA.strip().replace("{typeName}", class_name).split("\n"))
         if self.jackson_annotations:
             class_definition += f'\n{INDENT*2}'+f'\n{INDENT*2}'.join(
                 JSON_FROMDATA.strip().replace("{typeName}", class_name).split("\n"))
         class_definition += f"\n{INDENT*2}throw new UnsupportedOperationException(\"Unsupported media type \"+ contentType);\n{INDENT}}}"
         
         if self.jackson_annotations:
-            class_definition += self.create_is_json_match_method(avro_schema, avro_schema.get('namespace', parent_package), class_name)
+            class_definition += self.create_is_json_match_method(avro_schema, avro_schema.get('namespace', namespace), class_name)
 
         class_definition += "\n}"
 
         if write_file:
             self.write_to_file(package, class_name, class_definition)
-        type_name = self.concat_package(package.replace('/', '.'), class_name)
-        return AvroToJava.JavaType(type_name, is_class=True)
+        return AvroToJava.JavaType(qualified_class_name, is_class=True)
     
     def create_is_json_match_method(self, avro_schema, parent_namespace, class_name) -> str:
         """ Generates the isJsonMatch method for Jackson """
         predicates = ''
         class_definition = ''
         class_definition += f"\n\n{INDENT}/**\n{INDENT} * Checks if the JSON node matches the schema\n{INDENT}"
         class_definition += f"\n{INDENT}@param node The JSON node to check */"
@@ -442,16 +492,16 @@
             class_definition += f"({node_check}.isObject())"   
         elif field_type.type_name.startswith("List<"):
             items_type = field_type.type_name[5:-1]
             pred = f"Predicate<JsonNode> val{field_name_js} = (JsonNode n) -> n.isArray() && !n.elements().hasNext() || "
             pred_test = self.predicate_test(items_type)
             if pred_test:
                 pred += "n.elements().next()" + pred_test
-            elif items_type in self.generated_types:
-                kind = self.generated_types[items_type]
+            elif items_type in self.generated_types_java_package:
+                kind = self.generated_types_java_package[items_type]
                 if kind == "enum":
                     pred += f"n.elements().next().isTextual() && Enum.valueOf({items_type}.class, n.elements().next().asText()) != null"
                 else:
                     pred += f"{items_type}.isJsonMatch(n.elements().next())"
             else:
                 pred += "true"
             predicates += pred + ";"
@@ -459,16 +509,16 @@
         elif field_type.type_name.startswith("Map<"):
             comma_offset = field_type.type_name.find(',')+1
             values_type = field_type.type_name[comma_offset:-1]
             pred = f"Predicate<JsonNode> val{field_name_js} = (JsonNode n) -> n.isObject() && !n.elements().hasNext() || "
             pred_test = self.predicate_test(values_type)
             if pred_test:
                 pred += "n.elements().next()" + pred_test
-            elif values_type in self.generated_types:
-                kind = self.generated_types[values_type]
+            elif values_type in self.generated_types_java_package:
+                kind = self.generated_types_java_package[values_type]
                 if kind == "enum":
                     pred += f"n.elements().next().isTextual() && Enum.valueOf({values_type}.class, n.elements().next().asText()) != null"
                 else:
                     pred += f"{values_type}.isJsonMatch(n.elements().next())"
             else:
                 pred += "true"
             predicates += pred + ";"
@@ -478,15 +528,15 @@
         elif field_type.is_enum:
             class_definition += f"(node.get(\"{field_name_js}\").isTextual() && Enum.valueOf({field_type.type_name}.class, node.get(\"{field_name_js}\").asText()) != null)"
         else:
             is_union = False
             field_union = pascal(field_name) + 'Union'
             if field_type == field_union:
                 field_union = class_name + "." + pascal(field_name) + 'Union'
-                type_kind = self.generated_types[field_union] if field_union in self.generated_types else "class"
+                type_kind = self.generated_types_avro_namespace[field_union] if field_union in self.generated_types_avro_namespace else "class"
                 if type_kind == "union":
                     is_union = True
                     class_definition += f"({node_check}.isObject() && {field_type.type_name}.isJsonMatch(node.get(\"{field_name_js}\")))"
             if not is_union:
                 class_definition += f"(node.has(\"{field_name_js}\"))"
         return predicates, class_definition
 
@@ -550,77 +600,92 @@
         elif field_type.is_enum:
             class_definition += f"({null_check} || ({node_check}.isTextual() && Enum.valueOf({field_type.type_name}.class, {element_name}.asText()) != null))"
         else:
             is_union = False
             field_union = pascal(element_name) + 'Union'
             if field_type == field_union:
                 field_union = class_name + "." + pascal(element_name) + 'Union'
-                type_kind = self.generated_types[field_union] if field_union in self.generated_types else "class"
+                type_kind = self.generated_types_avro_namespace[field_union] if field_union in self.generated_types_avro_namespace else "class"
                 if type_kind == "union":
                     is_union = True
                     class_definition += f"({null_check} || {field_type}.isJsonMatch({element_name}))"
             if not is_union:
                 class_definition += f"({node_check}.isObject()){f' || {null_check}' if is_optional else ''}"
 
         return class_definition
 
-    def generate_get_method(self, fields: List[Dict], parent_package: str) -> str:
+    def generate_avro_get_method(self, class_name: str, fields: List[Dict], parent_package: str) -> str:
         """ Generates the get method for SpecificRecord """
         get_method = f"\n{INDENT}@Override\n{INDENT}public Object get(int field$) {{\n"
         get_method += f"{INDENT * 2}switch (field$) {{\n"
         for index, field in enumerate(fields):
             field_name = pascal(field['name']) if self.pascal_properties else field['name']
-            field_name = self.safe_identifier(field_name)
-            get_method += f"{INDENT * 3}case {index}: return this.{field_name};\n"
+            field_name = self.safe_identifier(field_name, class_name)
+            field_type = self.convert_avro_type_to_java(class_name, field_name, field['type'], parent_package)
+            if field_type.type_name in self.generated_types_avro_namespace and self.generated_types_avro_namespace[field_type.type_name] == "union":
+                get_method += f"{INDENT * 3}case {index}: return this.{field_name}!=null?this.{field_name}.toObject():null;\n"
+            else:
+                get_method += f"{INDENT * 3}case {index}: return this.{field_name};\n"
         get_method += f"{INDENT * 3}default: throw new AvroRuntimeException(\"Bad index: \" + field$);\n"
         get_method += f"{INDENT * 2}}}\n{INDENT}}}\n"
         return get_method
 
-    def generate_put_method(self, class_name: str, fields: List[Dict], parent_package: str) -> str:
+    def generate_avro_put_method(self, class_name: str, fields: List[Dict], parent_package: str) -> str:
         """ Generates the put method for SpecificRecord """
         suppress_unchecked = False
         put_method = f"\n{INDENT}@Override\n{INDENT}public void put(int field$, Object value$) {{\n"
         put_method += f"{INDENT * 2}switch (field$) {{\n"
         for index, field in enumerate(fields):
             field_name = pascal(field['name']) if self.pascal_properties else field['name']
-            field_name = self.safe_identifier(field_name)
-            java_type = self.convert_avro_type_to_java(class_name, field_name, field['type'], parent_package)
-            if java_type.type_name.startswith("List<") or java_type.type_name.startswith("Map<"):
+            field_name = self.safe_identifier(field_name, class_name)
+            field_type = self.convert_avro_type_to_java(class_name, field_name, field['type'], parent_package)
+            if field_type.type_name.startswith("List<") or field_type.type_name.startswith("Map<"):
                 suppress_unchecked = True
-            put_method += f"{INDENT * 3}case {index}: this.{field_name} = ({java_type.type_name})value$; break;\n"
+            if field_type.type_name in self.generated_types_avro_namespace and self.generated_types_avro_namespace[field_type.type_name] == "union":
+                put_method += f"{INDENT * 3}case {index}: this.{field_name} = new {field_type.type_name}((GenericData.Record)value$); break;\n"
+            else:
+                if field_type.type_name == 'String':
+                    put_method += f"{INDENT * 3}case {index}: this.{field_name} = value$.toString(); break;\n"
+                else:
+                    put_method += f"{INDENT * 3}case {index}: this.{field_name} = ({field_type.type_name})value$; break;\n"
         put_method += f"{INDENT * 3}default: throw new AvroRuntimeException(\"Bad index: \" + field$);\n"
         put_method += f"{INDENT * 2}}}\n{INDENT}}}\n"
         if suppress_unchecked:
             put_method = f"\n{INDENT}@SuppressWarnings(\"unchecked\"){put_method}"
         return put_method
 
     def generate_enum(self, avro_schema: Dict, parent_package: str, write_file: bool) -> JavaType:
         """ Generates a Java enum from an Avro enum schema """
         enum_definition = ''
         if 'doc' in avro_schema:
             enum_definition += f"/** {avro_schema['doc']} */\n"
+            
+        package = self.concat_package(self.base_package, avro_schema.get('namespace', parent_package)).replace('.', '/').lower()       
         enum_name = self.safe_identifier(avro_schema['name'])
-        self.generated_types[self.concat_package(avro_schema.get('namespace', parent_package),avro_schema['name'])] = "enum"
-        package = self.concat_package(self.base_package, avro_schema.get('namespace', parent_package)).replace('.', '/').lower()        
+        type_name = self.concat_package(package.replace('/', '.'), enum_name)
+        self.generated_types_avro_namespace[self.concat_package(avro_schema.get('namespace', parent_package),avro_schema['name'])] = "enum"
+        self.generated_types_java_package[type_name] = "enum"       
         symbols = avro_schema.get('symbols', [])
         symbols_str = ', '.join(symbols)
         enum_definition += f"public enum {enum_name} {{\n"
         enum_definition += f"{INDENT}{symbols_str};\n"
         enum_definition += "}\n"
         if write_file:
             self.write_to_file(package, enum_name, enum_definition)
-        type_name = self.concat_package(package.replace('/', '.'), enum_name)
         return AvroToJava.JavaType(type_name, is_enum=True)
     
-    def generate_embedded_union_class_jackson(self, class_name: str, field_name: str, avro_type: List, parent_namespace: str, write_file: bool) -> str:
+    def generate_embedded_union_class_jackson(self, class_name: str, field_name: str, avro_type: List, parent_package: str, write_file: bool) -> str:
         """ Generates an embedded Union Class for Java using Jackson """
         class_definition_ctors = class_definition_decls = class_definition_read = class_definition_write = class_definition = ''
+        class_definition_toobject = class_definition_fromobjectctor = class_definition_genericrecordctor = ''
+        
         list_is_json_match: List[str] = []
         union_class_name = class_name + pascal(field_name) + 'Union'
-        union_types: List[AvroToJava.JavaType] = [self.convert_avro_type_to_java(class_name, field_name + "Option" + str(i), t, parent_namespace) for i, t in enumerate(avro_type)]
+        package = self.concat_package(self.base_package, parent_package).replace('.', '/').lower()
+        union_types: List[AvroToJava.JavaType] = [self.convert_avro_type_to_java(class_name, field_name + "Option" + str(i), t, parent_package) for i, t in enumerate(avro_type)]
         for i, union_type in enumerate(union_types):
             # we need the nullable version (wrapper) of all primitive types
             if self.is_java_primitive(union_type):
                 union_type = self.map_primitive_to_java(union_type.type_name, True)
             union_variable_name = union_type.type_name
             is_dict = is_list = False
             if union_type.type_name.startswith("Map<"):
@@ -633,24 +698,38 @@
                 is_list = True
                 union_variable_name = flatten_type_name(union_type.type_name)
             elif union_type.type_name == "byte[]":
                 union_variable_name = "Bytes"
             else:
                 union_variable_name = union_type.type_name.rsplit('.', 1)[-1]
             
-            union_variable_name = self.safe_identifier(union_variable_name)
+            union_variable_name = self.safe_identifier(union_variable_name, class_name)
 
             # Constructor for each type
             class_definition_ctors += \
                 f"{INDENT*1}public {union_class_name}({union_type.type_name} {union_variable_name}) {{\n{INDENT*2}this._{camel(union_variable_name)} = {union_variable_name};\n{INDENT*1}}}\n"
 
             # Declarations
             class_definition_decls += \
                 f"{INDENT*1}private {union_type.type_name} _{camel(union_variable_name)};\n" + \
                 f"{INDENT*1}public {union_type.type_name} get{union_variable_name}() {{ return _{camel(union_variable_name)}; }}\n";
+                
+            class_definition_toobject += f"{INDENT*2}if (_{camel(union_variable_name)} != null) {{\n{INDENT*3}return _{camel(union_variable_name)};\n{INDENT*2}}}\n"
+            
+            if self.avro_annotation and union_type.is_class:            
+                class_definition_genericrecordctor += f"{INDENT*2}if ( {union_type.type_name}.AvroSchema.getName().equals(record.getSchema().getName()) && {union_type.type_name}.AvroSchema.getNamespace().equals(record.getSchema().getNamespace()) ) {{"
+                class_definition_genericrecordctor += f"\n{INDENT*3}this._{camel(union_variable_name)} = new {union_type.type_name}(record);\n{INDENT*3}return;\n{INDENT*2}}}\n"
+            
+            # there can only be one list and one map in the union, so we don't need to differentiate this any further
+            if is_list:
+                class_definition_fromobjectctor += f"{INDENT*2}if (obj instanceof List<?>) {{\n{INDENT*3}this._{camel(union_variable_name)} = ({union_type.type_name})obj;\n{INDENT*3}return;\n{INDENT*2}}}\n"
+            elif is_dict:
+                class_definition_fromobjectctor += f"{INDENT*2}if (obj instanceof Map<?,?>) {{\n{INDENT*3}this._{camel(union_variable_name)} = ({union_type.type_name})obj;\n{INDENT*3}return;\n{INDENT*2}}}\n"
+            else:
+                class_definition_fromobjectctor += f"{INDENT*2}if (obj instanceof {union_type.type_name}) {{\n{INDENT*3}this._{camel(union_variable_name)} = ({union_type.type_name})obj;\n{INDENT*3}return;\n{INDENT*2}}}\n"
 
             # Read method logic
             if is_dict:
                 class_definition_read += f"{INDENT*3}if (node.isObject()) {{\n{INDENT*4}{union_type.type_name} map = mapper.readValue(node.toString(), new TypeReference<{union_type.type_name}>(){{}});\n{INDENT*3}return new {union_class_name}(map);\n{INDENT*3}}}\n"
             elif is_list:
                 class_definition_read += f"{INDENT*3}if (node.isArray()) {{\n{INDENT*4}{union_type.type_name} list = mapper.readValue(node.toString(), new TypeReference<{union_type.type_name}>(){{}});\n{INDENT*4}return new {union_class_name}(list);\n{INDENT*3}}}\n"
             elif self.is_java_primitive(union_type):
@@ -673,56 +752,70 @@
             else:
                 if union_type.is_enum:
                     class_definition_read += f"{INDENT*3}if (node.isTextual()) {{\n{INDENT*4}return new {union_class_name}(Enum.valueOf({union_type.type_name}.class, node.asText()));\n{INDENT*3}}}\n"
                 else:
                     class_definition_read += f"{INDENT*3}if (node.isObject() && {union_type.type_name}.isJsonMatch(node)) {{\n{INDENT*4}return new {union_class_name}(mapper.readValue(node.toString(), {union_type.type_name}.class));\n{INDENT*3}}}\n"
                 
             # Write method logic
-            class_definition_write += f"{INDENT*3}{union_type.type_name} {camel(union_variable_name)}Value = value.get{union_variable_name}();\n{INDENT*3}if ({camel(union_variable_name)}Value != null) {{\n{INDENT*4}generator.writeObject({camel(union_variable_name)}Value);\n{INDENT*3}}}\n"
+            class_definition_write += f"{INDENT*3}{union_type.type_name} {camel(union_variable_name)}Value = value.get{union_variable_name}();\n{INDENT*3}if ({camel(union_variable_name)}Value != null) {{\n{INDENT*4}generator.writeObject({camel(union_variable_name)}Value);\n{INDENT*4}return;\n{INDENT*3}}}\n"
 
             # JSON match method logic
             gij = self.get_is_json_match_clause_type("node", class_name, union_type)
             if gij:
                 list_is_json_match.append(gij)
 
         class_definition =  f"@JsonSerialize(using = {union_class_name}.Serializer.class)\n"
         class_definition += f"@JsonDeserialize(using = {union_class_name}.Deserializer.class)\n"
         class_definition += f"public class {union_class_name} {{\n"
         class_definition += class_definition_decls
-        class_definition += f"{INDENT}public " + union_class_name + "() {}\n"
+        class_definition += f"\n{INDENT}public " + union_class_name + "() {}\n"
+        if self.avro_annotation:
+            class_definition += f"\n{INDENT}public {union_class_name}(GenericData.Record record) {{\n"
+            class_definition += class_definition_genericrecordctor
+            class_definition += f"{INDENT*2}throw new UnsupportedOperationException(\"No record type is set in the union\");\n"
+            class_definition += f"{INDENT}}}\n"
+        class_definition += f"\n{INDENT}public {union_class_name}(Object obj) {{\n"
+        class_definition += class_definition_fromobjectctor
+        class_definition += f"{INDENT*2}throw new UnsupportedOperationException(\"No record type is set in the union\");\n"
+        class_definition += f"{INDENT}}}\n"
         class_definition += class_definition_ctors
-        class_definition += f"{INDENT}public static class Serializer extends JsonSerializer<" + union_class_name + "> {\n"
+        class_definition += f"\n{INDENT}public Object toObject() {{\n"
+        class_definition += class_definition_toobject
+        class_definition += f"{INDENT*2}throw new UnsupportedOperationException(\"No record type is set in the union\");\n"
+        class_definition += f"{INDENT}}}\n"
+        class_definition += f"\n{INDENT}public static class Serializer extends JsonSerializer<" + union_class_name + "> {\n"
         class_definition += f"{INDENT*2}@Override\n"
         class_definition += f"{INDENT*2}public void serialize(" + union_class_name + " value, JsonGenerator generator, SerializerProvider serializers) throws IOException {\n"
         class_definition += class_definition_write
         class_definition += f"{INDENT*3}throw new UnsupportedOperationException(\"No record type is set in the union\");\n"
         class_definition += f"{INDENT*2}}}\n{INDENT}}}\n"
-        class_definition += f"{INDENT}public static class Deserializer extends JsonDeserializer<" + union_class_name + "> {\n"
+        class_definition += f"\n{INDENT}public static class Deserializer extends JsonDeserializer<" + union_class_name + "> {\n"
         class_definition += f"{INDENT*2}@Override\n"
         class_definition += f"{INDENT*2}public " + union_class_name + " deserialize(JsonParser p, DeserializationContext ctxt) throws IOException, JsonProcessingException {\n"
         class_definition += f"{INDENT*3}ObjectMapper mapper = (ObjectMapper) p.getCodec();\n"
         class_definition += f"{INDENT*3}JsonNode node = mapper.readTree(p);\n"
         class_definition += class_definition_read
         class_definition += f"{INDENT*3}throw new UnsupportedOperationException(\"No record type matched the JSON data\");\n"
         class_definition += f"{INDENT*2}}}\n{INDENT}}}\n"
-        class_definition += f"{INDENT*1}public static boolean isJsonMatch(JsonNode node) {{\n"
+        class_definition += f"\n{INDENT*1}public static boolean isJsonMatch(JsonNode node) {{\n"
         class_definition += f"{INDENT*2}return " + " || ".join(list_is_json_match) + ";\n"
         class_definition += f"{INDENT*1}}}\n}}\n"
 
         if write_file:
-            self.write_to_file(parent_namespace, union_class_name, class_definition)
-        self.generated_types[union_class_name] = "union"  # Track union types
+            self.write_to_file(package, union_class_name, class_definition)
+        self.generated_types_avro_namespace[union_class_name] = "union"  # Track union types
+        self.generated_types_java_package[union_class_name] = "union"  # Track union types
         return union_class_name
 
 
     def generate_property(self, class_name: str, field: Dict, parent_package: str) -> str:
         """ Generates a Java property definition """
         field_name = pascal(field['name']) if self.pascal_properties else field['name']
         field_type = self.convert_avro_type_to_java(class_name, field_name, field['type'], parent_package)
-        safe_field_name = self.safe_identifier(field_name)
+        safe_field_name = self.safe_identifier(field_name, class_name)
         property_def = ''
         if 'doc' in field:
             property_def += f"{INDENT}/** {field['doc']} */\n"
         if self.jackson_annotations:
             property_def += f"{INDENT}@JsonProperty(\"{field['name']}\")\n"
         property_def += f"{INDENT}private {field_type.type_name} {safe_field_name};\n"
         property_def += f"{INDENT}public {field_type.type_name} get{pascal(field_name)}() {{ return {safe_field_name}; }}\n"
@@ -769,14 +862,16 @@
                     file.write("import java.time.Duration;\n")
                     
             if self.avro_annotation:
                 if 'AvroRuntimeException' in definition:
                     file.write("import org.apache.avro.AvroRuntimeException;\n")
                 if 'Schema' in definition:
                     file.write("import org.apache.avro.Schema;\n")
+                if 'GenericData' in definition:
+                    file.write("import org.apache.avro.generic.GenericData;\n")
                 if 'DatumReader' in definition:
                     file.write("import org.apache.avro.io.DatumReader;\n")
                 if 'DatumWriter' in definition:
                     file.write("import org.apache.avro.io.DatumWriter;\n")
                 if 'DecoderFactory' in definition:
                     file.write("import org.apache.avro.io.DecoderFactory;\n")
                 if 'EncoderFactory' in definition:
@@ -785,16 +880,14 @@
                     file.write("import org.apache.avro.specific.SpecificDatumReader;\n")
                 if 'SpecificDatumWriter' in definition:
                     file.write("import org.apache.avro.specific.SpecificDatumWriter;\n")
                 if 'SpecificRecord' in definition:
                     file.write("import org.apache.avro.specific.SpecificRecord;\n")
                 if 'Encoder' in definition:
                     file.write("import org.apache.avro.io.Encoder;\n")
-                if 'Decoder' in definition:
-                    file.write("import org.apache.avro.io.Decoder;\n")            
             if self.jackson_annotations:
                 if 'JsonNode' in definition:
                     file.write("import com.fasterxml.jackson.databind.JsonNode;\n")
                 if 'ObjectMapper' in definition:
                     file.write("import com.fasterxml.jackson.databind.ObjectMapper;\n")
                 if 'JsonSerialize' in definition:
                     file.write("import com.fasterxml.jackson.databind.annotation.JsonSerialize;\n")
@@ -806,14 +899,16 @@
                     file.write("import com.fasterxml.jackson.databind.SerializerProvider;\n")
                 if 'JsonDeserializer' in definition:
                     file.write("import com.fasterxml.jackson.databind.JsonDeserializer;\n")
                 if 'DeserializationContext' in definition:
                     file.write("import com.fasterxml.jackson.databind.DeserializationContext;\n")
                 if 'JsonParser' in definition:
                     file.write("import com.fasterxml.jackson.core.JsonParser;\n")
+                if 'JsonIgnore' in definition:
+                    file.write("import com.fasterxml.jackson.annotation.JsonIgnore;\n")
                 if 'JsonProperty' in definition:
                     file.write("import com.fasterxml.jackson.annotation.JsonProperty;\n")
                 if 'JsonProcessingException' in definition:
                     file.write("import com.fasterxml.jackson.core.JsonProcessingException;\n")
                 if 'JsonGenerator' in definition:
                     file.write("import com.fasterxml.jackson.core.JsonGenerator;\n")
                 if 'TypeReference' in definition:
@@ -840,23 +935,26 @@
         """Converts Avro schema to Java"""
         if not isinstance(schema, list):
             schema = [schema]
         if not os.path.exists(output_dir):
             os.makedirs(output_dir, exist_ok=True)
         pom_path = os.path.join(output_dir, "pom.xml")
         if not os.path.exists(pom_path):
+            package_elements = self.base_package.split('.') if self.base_package else ["com", "example"]
+            groupid = '.'.join(package_elements[:-1]) if len(package_elements) > 1 else package_elements[0]
+            artifactid = package_elements[-1]
             with open(pom_path, 'w', encoding='utf-8') as file:
-                file.write(POM_CONTENT)
+                file.write(POM_CONTENT.format(groupid=groupid, artifactid=artifactid))
         output_dir = os.path.join(
             output_dir, "src/main/java".replace('/', os.sep))
         if not os.path.exists(output_dir):
             os.makedirs(output_dir, exist_ok=True)
         self.output_dir = output_dir
         for avro_schema in (x for x in schema if isinstance(x, dict)):
-            self.generate_class_or_enum(avro_schema, self.base_package)
+            self.generate_class_or_enum(avro_schema, '')
 
     def convert(self, avro_schema_path: str, output_dir: str):
         """Converts Avro schema to Java"""
         with open(avro_schema_path, 'r', encoding='utf-8') as file:
             schema = json.load(file)
         self.convert_schema(schema, output_dir)
```

### Comparing `avrotize-1.4.0/avrotize/avrotojs.py` & `avrotize-1.4.1/avrotize/avrotojs.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.0/avrotize/avrotojsons.py` & `avrotize-1.4.1/avrotize/avrotojsons.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.0/avrotize/avrotokusto.py` & `avrotize-1.4.1/avrotize/avrotokusto.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.0/avrotize/avrotoparquet.py` & `avrotize-1.4.1/avrotize/avrotoparquet.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.0/avrotize/avrotoproto.py` & `avrotize-1.4.1/avrotize/avrotoproto.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.0/avrotize/avrotopython.py` & `avrotize-1.4.1/avrotize/avrotopython.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,15 +200,16 @@
         directory_path = os.path.join(self.output_dir, package.replace('.', '/').replace('/', os.sep).lower())
         if not os.path.exists(directory_path):
             os.makedirs(directory_path, exist_ok=True)
         
         # drop an __init.py__ file in all directories along the path above output_dir
         package_name = package
         while package_name:
-            init_file_path = os.path.join(directory_path, '__init__.py')
+            package_directory_path = os.path.join(self.output_dir, package_name.replace('.', '/').replace('/', os.sep).lower())
+            init_file_path = os.path.join(package_directory_path, '__init__.py')
             if not os.path.exists(init_file_path):
                 with open(init_file_path, 'w', encoding='utf-8') as file:
                     file.write('')
             if '.' in package_name:
                 package_name = package_name.rsplit('.', 1)[0]
             else:
                 package_name = ''
@@ -224,14 +225,16 @@
             if references:
                 file.write(f'from typing import {",".join(references)}\n')
             file.write('\n'+definition)
 
     def convert_schemas(self, avro_schemas: List, output_dir: str):
         """ Converts Avro schema to Python data classes"""
         self.output_dir = output_dir
+        with open(os.path.join(self.output_dir, "__init__.py"), 'w', encoding='utf-8') as file:
+            file.write('')
         for avro_schema in avro_schemas:
             if avro_schema['type'] == 'enum':
                 self.generate_enum(avro_schema, self.base_package, write_file=True)
             elif avro_schema['type'] == 'record':
                 self.generate_class(avro_schema, self.base_package, write_file=True)
     
     def convert(self, avro_schema_path: str, output_dir: str):
```

### Comparing `avrotize-1.4.0/avrotize/avrotots.py` & `avrotize-1.4.1/avrotize/avrotots.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.0/avrotize/avrototsql.py` & `avrotize-1.4.1/avrotize/avrototsql.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.0/avrotize/avrotoxsd.py` & `avrotize-1.4.1/avrotize/avrotoxsd.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.0/avrotize/common.py` & `avrotize-1.4.1/avrotize/common.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.0/avrotize/dependency_resolver.py` & `avrotize-1.4.1/avrotize/dependency_resolver.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.0/avrotize/generic/generic.avsc` & `avrotize-1.4.1/avrotize/generic/generic.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.0/avrotize/jsonstoavro.py` & `avrotize-1.4.1/avrotize/jsonstoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.0/avrotize/kconnect.json` & `avrotize-1.4.1/avrotize/kconnect.json`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.0/avrotize/kstructtoavro.py` & `avrotize-1.4.1/avrotize/kstructtoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.0/avrotize/proto2parser.py` & `avrotize-1.4.1/avrotize/proto2parser.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.0/avrotize/proto3parser.py` & `avrotize-1.4.1/avrotize/proto3parser.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.0/avrotize/prototoavro.py` & `avrotize-1.4.1/avrotize/prototoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.0/avrotize/prototypes/any.avsc` & `avrotize-1.4.1/avrotize/prototypes/any.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.0/avrotize/prototypes/api.avsc` & `avrotize-1.4.1/avrotize/prototypes/api.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.0/avrotize/prototypes/duration.avsc` & `avrotize-1.4.1/avrotize/prototypes/duration.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.0/avrotize/prototypes/field_mask.avsc` & `avrotize-1.4.1/avrotize/prototypes/field_mask.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.0/avrotize/prototypes/struct.avsc` & `avrotize-1.4.1/avrotize/prototypes/struct.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.0/avrotize/prototypes/timestamp.avsc` & `avrotize-1.4.1/avrotize/prototypes/timestamp.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.0/avrotize/prototypes/type.avsc` & `avrotize-1.4.1/avrotize/prototypes/type.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.0/avrotize/prototypes/wrappers.avsc` & `avrotize-1.4.1/avrotize/prototypes/wrappers.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.0/avrotize/xsdtoavro.py` & `avrotize-1.4.1/avrotize/xsdtoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.0/pyproject.toml` & `avrotize-1.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `avrotize-1.4.0/PKG-INFO` & `avrotize-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avrotize
-Version: 1.4.0
+Version: 1.4.1
 Summary: Tools to convert from and to Avro Schema from various other schema languages.
 Author-email: Clemens Vasters <clemensv@microsoft.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

