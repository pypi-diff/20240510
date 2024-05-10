# Comparing `tmp/nesiac-0.4.2.tar.gz` & `tmp/nesiac-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nesiac-0.4.2.tar", max compression
+gzip compressed data, was "nesiac-0.4.3.tar", max compression
```

## Comparing `nesiac-0.4.2.tar` & `nesiac-0.4.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1083 2023-10-02 08:31:55.251482 nesiac-0.4.2/LICENSE
--rw-r--r--   0        0        0       29 2023-10-04 05:55:42.315361 nesiac-0.4.2/nesiac/__main__.py
--rw-r--r--   0        0        0     2439 2023-10-10 06:45:44.270971 nesiac-0.4.2/nesiac/args.py
--rw-r--r--   0        0        0    10878 2023-10-10 06:48:30.252202 nesiac-0.4.2/nesiac/cli.py
--rw-r--r--   0        0        0     3852 2023-10-03 06:17:37.856792 nesiac-0.4.2/nesiac/ingest.py
--rw-r--r--   0        0        0        0 2023-09-13 12:41:35.006853 nesiac-0.4.2/nesiac/parsing/__init__.py
--rw-r--r--   0        0        0     1060 2023-10-03 06:17:47.362785 nesiac-0.4.2/nesiac/parsing/map_regions.py
--rw-r--r--   0        0        0     1106 2023-10-02 14:19:31.408745 nesiac-0.4.2/nesiac/parsing/objects.py
--rw-r--r--   0        0        0      139 2023-09-26 07:08:02.511833 nesiac-0.4.2/nesiac/parsing/program_headers.py
--rw-r--r--   0        0        0      146 2023-09-26 07:08:07.885854 nesiac-0.4.2/nesiac/parsing/section_headers.py
--rw-r--r--   0        0        0      659 2023-10-10 06:49:08.620977 nesiac-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     1695 2023-10-09 11:49:01.049934 nesiac-0.4.2/README.md
--rw-r--r--   0        0        0     2517 1970-01-01 00:00:00.000000 nesiac-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-05-10 13:21:40.331140 nesiac-0.4.3/LICENSE
+-rw-r--r--   0        0        0       29 2024-05-10 13:21:40.331140 nesiac-0.4.3/nesiac/__main__.py
+-rw-r--r--   0        0        0     2439 2024-05-10 13:21:40.331140 nesiac-0.4.3/nesiac/args.py
+-rw-r--r--   0        0        0    10878 2024-05-10 13:21:40.331140 nesiac-0.4.3/nesiac/cli.py
+-rw-r--r--   0        0        0     3852 2024-05-10 13:21:40.334662 nesiac-0.4.3/nesiac/ingest.py
+-rw-r--r--   0        0        0        0 2024-05-10 13:21:40.334662 nesiac-0.4.3/nesiac/parsing/__init__.py
+-rw-r--r--   0        0        0     1060 2024-05-10 13:21:40.335212 nesiac-0.4.3/nesiac/parsing/map_regions.py
+-rw-r--r--   0        0        0     1131 2024-05-10 13:27:30.943007 nesiac-0.4.3/nesiac/parsing/objects.py
+-rw-r--r--   0        0        0      139 2024-05-10 13:21:40.335212 nesiac-0.4.3/nesiac/parsing/program_headers.py
+-rw-r--r--   0        0        0      146 2024-05-10 13:21:40.335212 nesiac-0.4.3/nesiac/parsing/section_headers.py
+-rw-r--r--   0        0        0      654 2024-05-10 13:27:10.933019 nesiac-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     1695 2024-05-10 13:21:40.331140 nesiac-0.4.3/README.md
+-rw-r--r--   0        0        0     2563 1970-01-01 00:00:00.000000 nesiac-0.4.3/PKG-INFO
```

### Comparing `nesiac-0.4.2/LICENSE` & `nesiac-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nesiac-0.4.2/nesiac/args.py` & `nesiac-0.4.3/nesiac/args.py`

 * *Files identical despite different names*

### Comparing `nesiac-0.4.2/nesiac/cli.py` & `nesiac-0.4.3/nesiac/cli.py`

 * *Files identical despite different names*

### Comparing `nesiac-0.4.2/nesiac/ingest.py` & `nesiac-0.4.3/nesiac/ingest.py`

 * *Files identical despite different names*

### Comparing `nesiac-0.4.2/nesiac/parsing/map_regions.py` & `nesiac-0.4.3/nesiac/parsing/map_regions.py`

 * *Files identical despite different names*

### Comparing `nesiac-0.4.2/nesiac/parsing/objects.py` & `nesiac-0.4.3/nesiac/parsing/objects.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from dataclasses import dataclass
 import pathlib
 from elftools.elf.elffile import ELFFile, SymbolTableSection
-import cpp_demangle
+import cxxfilt
 import rust_demangler
 
+
 @dataclass(frozen=True)
 class ElfObject:
     addr: int
     size: int
     name: str
 
+
 def _demangle(input: str) -> str:
     try:
         rust_d = rust_demangler.demangle(input)
     except Exception:
         rust_d = None
     try:
-        cpp_d = cpp_demangle.demangle(input)
+        cpp_d = cxxfilt.demangle(input)
     except Exception:
         cpp_d = None
     return rust_d or cpp_d or input
 
 
 def from_elf(file: pathlib.Path) -> list[ElfObject]:
     outlist = []  # type: list[ElfObject]
@@ -28,10 +30,11 @@
         elf = ELFFile(in_f)
         symtab = elf.get_section_by_name(".symtab")
         if not isinstance(symtab, SymbolTableSection):
             return outlist
         for sym in symtab.iter_symbols():
             if sym.entry.st_info.type in ["STT_OBJECT", "STT_FUNC"]:
                 outlist.append(
-                    ElfObject(sym.entry.st_value, sym.entry.st_size, _demangle(sym.name))
+                    ElfObject(sym.entry.st_value, sym.entry.st_size,
+                              _demangle(sym.name))
                 )
     return outlist
```

### Comparing `nesiac-0.4.2/pyproject.toml` & `nesiac-0.4.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "nesiac"
-version = "0.4.2"
+version = "0.4.3"
 description = "Memory usage visualiser for embedded applications"
 authors = ["Eekle"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Eekle/Nesiac/"
 keywords = ["embedded", "elf", "binary", "memory"]
 classifiers = [
     "Topic :: Software Development :: Embedded Systems",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 rich = "^13.6.0"
 pyelftools = "^0.30"
-cpp-demangle = "^0.1.2"
+cxxfilt = "^0.3.0"
 rust-demangler = "^1.0"
 getchlib = "^1.0.12"
 
 [tool.poetry.scripts]
 nesiac = 'nesiac.cli:cli'
```

### Comparing `nesiac-0.4.2/README.md` & `nesiac-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `nesiac-0.4.2/PKG-INFO` & `nesiac-0.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: nesiac
-Version: 0.4.2
+Version: 0.4.3
 Summary: Memory usage visualiser for embedded applications
 Home-page: https://github.com/Eekle/Nesiac/
 License: MIT
 Keywords: embedded,elf,binary,memory
 Author: Eekle
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Embedded Systems
-Requires-Dist: cpp-demangle (>=0.1.2,<0.2.0)
+Requires-Dist: cxxfilt (>=0.3.0,<0.4.0)
 Requires-Dist: getchlib (>=1.0.12,<2.0.0)
 Requires-Dist: pyelftools (>=0.30,<0.31)
 Requires-Dist: rich (>=13.6.0,<14.0.0)
 Requires-Dist: rust-demangler (>=1.0,<2.0)
 Project-URL: Repository, https://github.com/Eekle/Nesiac/
 Description-Content-Type: text/markdown
```

