# Comparing `tmp/tlvisuals-0.0.2.tar.gz` & `tmp/tlvisuals-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tlvisuals-0.0.2.tar", last modified: Mon Mar 18 02:04:43 2024, max compression
+gzip compressed data, was "tlvisuals-0.0.3.tar", last modified: Fri May 10 04:03:41 2024, max compression
```

## Comparing `tlvisuals-0.0.2.tar` & `tlvisuals-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-03-18 02:04:43.932410 tlvisuals-0.0.2/
--rw-rw-rw-   0        0        0     1091 2024-01-30 04:00:46.000000 tlvisuals-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      631 2024-03-18 02:04:43.927882 tlvisuals-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      155 2024-01-30 03:58:20.000000 tlvisuals-0.0.2/README.md
--rw-rw-rw-   0        0        0      560 2024-03-18 02:04:26.000000 tlvisuals-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-18 02:04:43.933412 tlvisuals-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-18 02:04:43.745576 tlvisuals-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-03-18 02:04:43.861515 tlvisuals-0.0.2/src/tlvisuals/
--rw-rw-rw-   0        0        0        0 2023-12-15 10:41:35.000000 tlvisuals-0.0.2/src/tlvisuals/__init__.py
--rw-rw-rw-   0        0        0     1839 2024-03-15 09:44:14.000000 tlvisuals-0.0.2/src/tlvisuals/__main__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 02:04:43.908520 tlvisuals-0.0.2/src/tlvisuals/output_builder/
--rw-rw-rw-   0        0        0        0 2023-12-15 10:41:35.000000 tlvisuals-0.0.2/src/tlvisuals/output_builder/__init__.py
--rw-rw-rw-   0        0        0     1905 2023-12-15 11:18:08.000000 tlvisuals-0.0.2/src/tlvisuals/output_builder/raw_format.py
-drwxrwxrwx   0        0        0        0 2024-03-18 02:04:43.923912 tlvisuals-0.0.2/src/tlvisuals/tests/
--rw-rw-rw-   0        0        0        0 2023-12-15 10:41:35.000000 tlvisuals-0.0.2/src/tlvisuals/tests/__init__.py
--rw-rw-rw-   0        0        0     1880 2023-12-15 10:41:35.000000 tlvisuals-0.0.2/src/tlvisuals/tests/test_bytegetter.py
--rw-rw-rw-   0        0        0     6903 2023-12-15 10:41:35.000000 tlvisuals-0.0.2/src/tlvisuals/tests/test_parser.py
--rw-rw-rw-   0        0        0     2670 2023-12-15 11:18:36.000000 tlvisuals-0.0.2/src/tlvisuals/tests/test_raw_format_output_builder.py
--rw-rw-rw-   0        0        0     1867 2023-12-15 10:50:55.000000 tlvisuals-0.0.2/src/tlvisuals/tlv.py
--rw-rw-rw-   0        0        0     8128 2024-03-15 10:26:45.000000 tlvisuals-0.0.2/src/tlvisuals/tlv_parser.py
-drwxrwxrwx   0        0        0        0 2024-03-18 02:04:43.926916 tlvisuals-0.0.2/src/tlvisuals.egg-info/
--rw-rw-rw-   0        0        0      631 2024-03-18 02:04:43.000000 tlvisuals-0.0.2/src/tlvisuals.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      525 2024-03-18 02:04:43.000000 tlvisuals-0.0.2/src/tlvisuals.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-18 02:04:43.000000 tlvisuals-0.0.2/src/tlvisuals.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-03-18 02:04:43.000000 tlvisuals-0.0.2/src/tlvisuals.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 04:03:41.908070 tlvisuals-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2024-01-30 04:00:46.000000 tlvisuals-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1498 2024-05-10 04:03:41.908070 tlvisuals-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1022 2024-05-10 03:49:29.000000 tlvisuals-0.0.3/README.md
+-rw-rw-rw-   0        0        0      560 2024-05-10 03:34:59.000000 tlvisuals-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-10 04:03:41.908070 tlvisuals-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-10 04:03:41.713097 tlvisuals-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-10 04:03:41.855548 tlvisuals-0.0.3/src/tlvisuals/
+-rw-rw-rw-   0        0        0        0 2023-12-15 10:41:35.000000 tlvisuals-0.0.3/src/tlvisuals/__init__.py
+-rw-rw-rw-   0        0        0     2276 2024-05-10 03:48:51.000000 tlvisuals-0.0.3/src/tlvisuals/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 04:03:41.871491 tlvisuals-0.0.3/src/tlvisuals/output_builder/
+-rw-rw-rw-   0        0        0        0 2023-12-15 10:41:35.000000 tlvisuals-0.0.3/src/tlvisuals/output_builder/__init__.py
+-rw-rw-rw-   0        0        0     2074 2024-05-10 03:37:22.000000 tlvisuals-0.0.3/src/tlvisuals/output_builder/raw_format.py
+drwxrwxrwx   0        0        0        0 2024-05-10 04:03:41.905048 tlvisuals-0.0.3/src/tlvisuals/tests/
+-rw-rw-rw-   0        0        0        0 2023-12-15 10:41:35.000000 tlvisuals-0.0.3/src/tlvisuals/tests/__init__.py
+-rw-rw-rw-   0        0        0     1880 2023-12-15 10:41:35.000000 tlvisuals-0.0.3/src/tlvisuals/tests/test_bytegetter.py
+-rw-rw-rw-   0        0        0     6903 2023-12-15 10:41:35.000000 tlvisuals-0.0.3/src/tlvisuals/tests/test_parser.py
+-rw-rw-rw-   0        0        0     2670 2024-05-10 03:39:20.000000 tlvisuals-0.0.3/src/tlvisuals/tests/test_raw_format_output_builder.py
+-rw-rw-rw-   0        0        0     1867 2023-12-15 10:50:55.000000 tlvisuals-0.0.3/src/tlvisuals/tlv.py
+-rw-rw-rw-   0        0        0     8128 2024-03-15 10:26:45.000000 tlvisuals-0.0.3/src/tlvisuals/tlv_parser.py
+drwxrwxrwx   0        0        0        0 2024-05-10 04:03:41.908070 tlvisuals-0.0.3/src/tlvisuals.egg-info/
+-rw-rw-rw-   0        0        0     1498 2024-05-10 04:03:41.000000 tlvisuals-0.0.3/src/tlvisuals.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      525 2024-05-10 04:03:41.000000 tlvisuals-0.0.3/src/tlvisuals.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 04:03:41.000000 tlvisuals-0.0.3/src/tlvisuals.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-10 04:03:41.000000 tlvisuals-0.0.3/src/tlvisuals.egg-info/top_level.txt
```

### Comparing `tlvisuals-0.0.2/LICENSE` & `tlvisuals-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tlvisuals-0.0.2/src/tlvisuals/__main__.py` & `tlvisuals-0.0.3/src/tlvisuals/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import argparse
+from argparse import RawTextHelpFormatter
 import sys
 import json
 from tlvisuals.tlv_parser import ByteGetter, TLVParser, DiagnosticsCollector, DerByteGetter
 from tlvisuals.output_builder.raw_format import RawFormatBuilder
 
 def main():
    parser = argparse.ArgumentParser(
       prog='TLVisuals',
       description='Prints TLV in a readable format. \
       Without options, app will read from standard input and assume the format is Hex in ASCII form, and output will be to standard output',
+      formatter_class=RawTextHelpFormatter
       )
-   parser.add_argument('-f', '--file')           # positional argument
-   parser.add_argument('-o', '--out')      # option that takes a value
-   parser.add_argument('-v', '--verbose',action='store_true')  # on/off flag
-   parser.add_argument('--input-format')  # inform formats: 'der', 'hextext'
+   parser.add_argument('-f', '--file', help="Parses input from specified FILE")
+   parser.add_argument('-o', '--out', help="Writes output to specified OUT file")
+   parser.add_argument('-v', '--verbose',action='store_true', help="Outputs more logs")  # on/off flag
+   parser.add_argument('--input-format', help="Specifies input format:\n -der: input is raw hex\notherwise assumed to be ascii hex")  # inform formats: 'der', 'hextext'
+   parser.add_argument('--output-format', help="Specifies output format:\n -interpretation: shows basic TLV flag interpretation")
    args = parser.parse_args()
    # print(args.file, args.out, args.verbose)
 
    # construct byte getter
    if args.file:
       if args.input_format and args.input_format == 'der':
          input_stream = open(args.file, 'rb')
@@ -36,15 +39,15 @@
    diags = DiagnosticsCollector()
    parser = TLVParser(diagnostic_collector=diags)
    parsed_tlvs = parser.parse_tlv(byte_getter)
    # for tlv in parsed_tlvs:
    #    print(json.dumps(tlv, indent=1))
 
    # build output
-   output_builder = RawFormatBuilder()
+   output_builder = RawFormatBuilder(inline_interpretation = True if args.output_format == "interpretation" else False)
    out_str = output_builder.build(parsed_tlvs)
 
    # write to stream
    if args.out:
       with open(args.out, 'wt') as f:
          f.write(out_str)
    else:
```

### Comparing `tlvisuals-0.0.2/src/tlvisuals/output_builder/raw_format.py` & `tlvisuals-0.0.3/src/tlvisuals/output_builder/raw_format.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 
 
 
 from io import StringIO
 from tlvisuals.tlv import *
 
-
+"""
+   Prints TLVs with indentation and with interpretation 
+   of basic TLV flags if enabled
+"""
 class RawFormatBuilder:
-   def __init__(self, indent_size:int = 3,  indent:int = 0) -> None:
+   def __init__(self, indent_size:int = 3,  indent:int = 0, inline_interpretation: bool = True) -> None:
       self._indent_size = indent_size
       self._indent_str = ' ' * indent_size
       self._indent = indent
-      self._inline_interpretation = True
+      self._inline_interpretation = inline_interpretation
 
    def _add_indent(self, output: StringIO):
       for _ in range(0, self._indent):
          output.write(self._indent_str)
 
 
    def _build_primitive(self, tlv: TLV, output:StringIO):
@@ -40,15 +43,17 @@
       if not tlv.value is None:
          if tlv.tag.type == TagType.PRIMITIVE:
             self._build_primitive(tlv, output)
             output.write('\n')
          else:
             output.write('\n')
             self._build_constructed(tlv, output)
-      # output.write('\n')
+      else:
+         output.write('\n')
+
 
    def build_on_output(self, input: list[TLV], output: StringIO):
       for tlv in input:
          self._build_tlv(tlv, output)
 
    def build(self, input: list[TLV]) -> str:
       output = StringIO()
```

### Comparing `tlvisuals-0.0.2/src/tlvisuals/tests/test_bytegetter.py` & `tlvisuals-0.0.3/src/tlvisuals/tests/test_bytegetter.py`

 * *Files identical despite different names*

### Comparing `tlvisuals-0.0.2/src/tlvisuals/tests/test_parser.py` & `tlvisuals-0.0.3/src/tlvisuals/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `tlvisuals-0.0.2/src/tlvisuals/tests/test_raw_format_output_builder.py` & `tlvisuals-0.0.3/src/tlvisuals/tests/test_raw_format_output_builder.py`

 * *Files identical despite different names*

### Comparing `tlvisuals-0.0.2/src/tlvisuals/tlv.py` & `tlvisuals-0.0.3/src/tlvisuals/tlv.py`

 * *Files identical despite different names*

### Comparing `tlvisuals-0.0.2/src/tlvisuals/tlv_parser.py` & `tlvisuals-0.0.3/src/tlvisuals/tlv_parser.py`

 * *Files identical despite different names*

### Comparing `tlvisuals-0.0.2/src/tlvisuals.egg-info/SOURCES.txt` & `tlvisuals-0.0.3/src/tlvisuals.egg-info/SOURCES.txt`

 * *Files identical despite different names*

