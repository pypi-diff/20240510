# Comparing `tmp/justatestwithcpp-0.1.1.tar.gz` & `tmp/justatestwithcpp-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "justatestwithcpp-0.1.1.tar", max compression
+gzip compressed data, was "justatestwithcpp-0.1.2.tar", max compression
```

## Comparing `justatestwithcpp-0.1.1.tar` & `justatestwithcpp-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2024-05-10 12:01:15.238184 justatestwithcpp-0.1.1/README.md
--rw-r--r--   0        0        0      203 2024-05-10 12:03:30.912670 justatestwithcpp-0.1.1/justatestwithcpp/.rendered.somecode.cpp
--rw-r--r--   0        0        0       24 2024-05-10 12:10:10.263635 justatestwithcpp-0.1.1/justatestwithcpp/__init__.py
--rw-r--r--   0        0        0      117 2024-05-10 12:04:22.591792 justatestwithcpp-0.1.1/justatestwithcpp/a.py
--rw-r--r--   0        0        0      228 2024-05-10 12:03:09.972985 justatestwithcpp-0.1.1/justatestwithcpp/somecode.cpp
--rwxr-xr-x   0        0        0  2427610 2024-05-10 12:03:35.164603 justatestwithcpp-0.1.1/justatestwithcpp/somecode.cpython-311-x86_64-linux-gnu.so
--rw-r--r--   0        0        0      287 2024-05-10 12:10:19.967374 justatestwithcpp-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      408 1970-01-01 00:00:00.000000 justatestwithcpp-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-10 12:01:15.238184 justatestwithcpp-0.1.2/README.md
+-rw-r--r--   0        0        0      203 2024-05-10 12:12:03.240544 justatestwithcpp-0.1.2/justatestwithcpp/.rendered.somecode.cpp
+-rw-r--r--   0        0        0       18 2024-05-10 12:18:15.403324 justatestwithcpp-0.1.2/justatestwithcpp/__init__.py
+-rw-r--r--   0        0        0      127 2024-05-10 12:18:06.399303 justatestwithcpp-0.1.2/justatestwithcpp/a.py
+-rw-r--r--   0        0        0      228 2024-05-10 12:03:09.972985 justatestwithcpp-0.1.2/justatestwithcpp/somecode.cpp
+-rwxr-xr-x   0        0        0  2427636 2024-05-10 12:12:07.340429 justatestwithcpp-0.1.2/justatestwithcpp/somecode.cpython-311-x86_64-linux-gnu.so
+-rw-r--r--   0        0        0      287 2024-05-10 12:18:46.211365 justatestwithcpp-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      408 1970-01-01 00:00:00.000000 justatestwithcpp-0.1.2/PKG-INFO
```

### Comparing `justatestwithcpp-0.1.1/justatestwithcpp/somecode.cpython-311-x86_64-linux-gnu.so` & `justatestwithcpp-0.1.2/justatestwithcpp/somecode.cpython-311-x86_64-linux-gnu.so`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 0% similar despite different names*

#### readelf --wide --file-header {}

```diff
@@ -6,15 +6,15 @@
   OS/ABI:                            UNIX - GNU
   ABI Version:                       0
   Type:                              DYN (Shared object file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
   Entry point address:               0x0
   Start of program headers:          64 (bytes into file)
-  Start of section headers:          2424944 (bytes into file)
+  Start of section headers:          2424960 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           56 (bytes)
   Number of program headers:         11
   Size of section headers:           64 (bytes)
   Number of section headers:         40
   Section header string table index: 39
```

#### readelf --wide --sections {}

```diff
@@ -1,8 +1,8 @@
-There are 40 section headers, starting at offset 0x250070:
+There are 40 section headers, starting at offset 0x250080:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .note.gnu.property NOTE            00000000000002a8 0002a8 000020 00   A  0   0  8
   [ 2] .note.gnu.build-id NOTE            00000000000002c8 0002c8 000024 00   A  0   0  4
   [ 3] .gnu.hash         GNU_HASH        00000000000002f0 0002f0 0000b0 00   A  4   0  8
@@ -32,18 +32,18 @@
   [27] .bss              NOBITS          000000000001e560 01d548 0000a0 00  WA  0   0 32
   [28] .comment          PROGBITS        0000000000000000 01d548 00002b 01  MS  0   0  1
   [29] .debug_aranges    PROGBITS        0000000000000000 01d573 000600 00      0   0  1
   [30] .debug_info       PROGBITS        0000000000000000 01db73 0de31b 00      0   0  1
   [31] .debug_abbrev     PROGBITS        0000000000000000 0fbe8e 002081 00      0   0  1
   [32] .debug_line       PROGBITS        0000000000000000 0fdf0f 01dddb 00      0   0  1
   [33] .debug_str        PROGBITS        0000000000000000 11bcea 0d7a06 01  MS  0   0  1
-  [34] .debug_line_str   PROGBITS        0000000000000000 1f36f0 000b57 01  MS  0   0  1
-  [35] .debug_loclists   PROGBITS        0000000000000000 1f4247 0488f5 00      0   0  1
-  [36] .debug_rnglists   PROGBITS        0000000000000000 23cb3c 00c88e 00      0   0  1
-  [37] .symtab           SYMTAB          0000000000000000 2493d0 0022f8 18     38 167  8
-  [38] .strtab           STRTAB          0000000000000000 24b6c8 004808 00      0   0  1
-  [39] .shstrtab         STRTAB          0000000000000000 24fed0 00019c 00      0   0  1
+  [34] .debug_line_str   PROGBITS        0000000000000000 1f36f0 000b6b 01  MS  0   0  1
+  [35] .debug_loclists   PROGBITS        0000000000000000 1f425b 0488f5 00      0   0  1
+  [36] .debug_rnglists   PROGBITS        0000000000000000 23cb50 00c88e 00      0   0  1
+  [37] .symtab           SYMTAB          0000000000000000 2493e0 0022f8 18     38 167  8
+  [38] .strtab           STRTAB          0000000000000000 24b6d8 004808 00      0   0  1
+  [39] .shstrtab         STRTAB          0000000000000000 24fee0 00019c 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   R (retain), D (mbind), l (large), p (processor specific)
```

#### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: f286e768d467d6ad080cb61a7650b687869d8dc9
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 185066115121b19647d397a75527ca8b8f35620f
```

#### readelf --wide --debug-dump=rawline {}

```diff
@@ -25,201 +25,201 @@
   Opcode 9 has 1 arg
   Opcode 10 has 0 args
   Opcode 11 has 0 args
   Opcode 12 has 1 arg
 
  The Directory Table (offset 0x22, lines 19, columns 1):
   Entry	Name
-  0	(line_strp)	(offset: 0x3a): /home/pietro/Desktop/cpp-py
-  1	(line_strp)	(offset: 0x56): /home/pietro/Desktop/cpp-py/cpp_py
-  2	(line_strp)	(offset: 0x79): /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/detail
-  3	(line_strp)	(offset: 0xec): /home/linuxbrew/.linuxbrew/opt/python@3.11/include/python3.11
-  4	(line_strp)	(offset: 0x12a): /usr/include/c++/11/bits
-  5	(line_strp)	(offset: 0x143): /usr/include/c++/11/ext
-  6	(line_strp)	(offset: 0x15b): /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/detail/../detail
-  7	(line_strp)	(offset: 0x1d8): /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/detail/../detail/..
-  8	(line_strp)	(offset: 0x258): /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11
-  9	(line_strp)	(offset: 0x2c4): /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/detail/..
-  10	(line_strp)	(offset: 0x33a): /usr/include/c++/11
-  11	(line_strp)	(offset: 0x34e): /home/linuxbrew/.linuxbrew/opt/python@3.11/include/python3.11/cpython
-  12	(line_strp)	(offset: 0x394): /usr/include/x86_64-linux-gnu/bits
-  13	(line_strp)	(offset: 0x3b7): /usr/include
-  14	(line_strp)	(offset: 0x3c4): /usr/lib/gcc/x86_64-linux-gnu/11/include
-  15	(line_strp)	(offset: 0x3ed): /usr/include/x86_64-linux-gnu/sys
-  16	(line_strp)	(offset: 0x40f): /usr/include/x86_64-linux-gnu/bits/types
-  17	(line_strp)	(offset: 0x438): /usr/include/x86_64-linux-gnu/c++/11/bits
-  18	(line_strp)	(offset: 0x462): /usr/include/c++/11/debug
+  0	(line_strp)	(offset: 0x44): /home/pietro/Desktop/cpp-py
+  1	(line_strp)	(offset: 0x60): /home/pietro/Desktop/cpp-py/justatestwithcpp
+  2	(line_strp)	(offset: 0x8d): /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/detail
+  3	(line_strp)	(offset: 0x100): /home/linuxbrew/.linuxbrew/opt/python@3.11/include/python3.11
+  4	(line_strp)	(offset: 0x13e): /usr/include/c++/11/bits
+  5	(line_strp)	(offset: 0x157): /usr/include/c++/11/ext
+  6	(line_strp)	(offset: 0x16f): /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/detail/../detail
+  7	(line_strp)	(offset: 0x1ec): /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/detail/../detail/..
+  8	(line_strp)	(offset: 0x26c): /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11
+  9	(line_strp)	(offset: 0x2d8): /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/detail/..
+  10	(line_strp)	(offset: 0x34e): /usr/include/c++/11
+  11	(line_strp)	(offset: 0x362): /home/linuxbrew/.linuxbrew/opt/python@3.11/include/python3.11/cpython
+  12	(line_strp)	(offset: 0x3a8): /usr/include/x86_64-linux-gnu/bits
+  13	(line_strp)	(offset: 0x3cb): /usr/include
+  14	(line_strp)	(offset: 0x3d8): /usr/lib/gcc/x86_64-linux-gnu/11/include
+  15	(line_strp)	(offset: 0x401): /usr/include/x86_64-linux-gnu/sys
+  16	(line_strp)	(offset: 0x423): /usr/include/x86_64-linux-gnu/bits/types
+  17	(line_strp)	(offset: 0x44c): /usr/include/x86_64-linux-gnu/c++/11/bits
+  18	(line_strp)	(offset: 0x476): /usr/include/c++/11/debug
 
  The File Name Table (offset 0x75, lines 165, columns 2):
   Entry	Dir	Name
-  0	(udata)	1	(line_strp)	(offset: 0x23): .rendered.somecode.cpp
-  1	(udata)	2	(line_strp)	(offset: 0x47c): class.h
-  2	(udata)	3	(line_strp)	(offset: 0x6d3): object.h
-  3	(udata)	1	(line_strp)	(offset: 0x23): .rendered.somecode.cpp
-  4	(udata)	4	(line_strp)	(offset: 0x484): shared_ptr_base.h
-  5	(udata)	4	(line_strp)	(offset: 0x7ba): allocator.h
-  6	(udata)	5	(line_strp)	(offset: 0x496): new_allocator.h
-  7	(udata)	4	(line_strp)	(offset: 0x4a6): allocated_ptr.h
-  8	(udata)	4	(line_strp)	(offset: 0x4b6): move.h
-  9	(udata)	4	(line_strp)	(offset: 0x4bd): alloc_traits.h
-  10	(udata)	6	(line_strp)	(offset: 0x4cc): common.h
-  11	(udata)	7	(line_strp)	(offset: 0x4d5): pytypes.h
-  12	(udata)	4	(line_strp)	(offset: 0x4df): shared_ptr.h
-  13	(udata)	5	(line_strp)	(offset: 0x4ec): atomicity.h
-  14	(udata)	4	(line_strp)	(offset: 0x4f8): hashtable.h
-  15	(udata)	4	(line_strp)	(offset: 0x504): hashtable_policy.h
-  16	(udata)	4	(line_strp)	(offset: 0x517): functional_hash.h
-  17	(udata)	4	(line_strp)	(offset: 0x529): stl_function.h
-  18	(udata)	4	(line_strp)	(offset: 0x538): stl_vector.h
-  19	(udata)	4	(line_strp)	(offset: 0x545): stl_pair.h
-  20	(udata)	4	(line_strp)	(offset: 0x550): basic_string.h
-  21	(udata)	4	(line_strp)	(offset: 0x55f): char_traits.h
-  22	(udata)	8	(line_strp)	(offset: 0x56d): pybind11.h
-  23	(udata)	9	(line_strp)	(offset: 0x578): attr.h
-  24	(udata)	4	(line_strp)	(offset: 0x57f): unique_ptr.h
-  25	(udata)	10	(line_strp)	(offset: 0x58c): tuple
-  26	(udata)	10	(line_strp)	(offset: 0x592): typeinfo
-  27	(udata)	4	(line_strp)	(offset: 0x59b): basic_string.tcc
-  28	(udata)	4	(line_strp)	(offset: 0x5ac): stl_iterator_base_funcs.h
-  29	(udata)	4	(line_strp)	(offset: 0x5c6): vector.tcc
-  30	(udata)	4	(line_strp)	(offset: 0x5d1): stl_bvector.h
-  31	(udata)	4	(line_strp)	(offset: 0x5df): stl_algobase.h
-  32	(udata)	10	(line_strp)	(offset: 0x5ee): typeindex
-  33	(udata)	4	(line_strp)	(offset: 0x5f8): stl_iterator.h
-  34	(udata)	4	(line_strp)	(offset: 0x607): charconv.h
-  35	(udata)	6	(line_strp)	(offset: 0x612): internals.h
-  36	(udata)	6	(line_strp)	(offset: 0x61e): typeid.h
-  37	(udata)	6	(line_strp)	(offset: 0x627): type_caster_base.h
-  38	(udata)	9	(line_strp)	(offset: 0x63a): cast.h
-  39	(udata)	5	(line_strp)	(offset: 0x4bd): alloc_traits.h
-  40	(udata)	4	(line_strp)	(offset: 0x641): forward_list.h
-  41	(udata)	4	(line_strp)	(offset: 0x650): exception_ptr.h
-  42	(udata)	4	(line_strp)	(offset: 0x660): stl_construct.h
-  43	(udata)	4	(line_strp)	(offset: 0x670): stl_uninitialized.h
-  44	(udata)	4	(line_strp)	(offset: 0x684): unordered_map.h
-  45	(udata)	4	(line_strp)	(offset: 0x694): unordered_set.h
-  46	(udata)	4	(line_strp)	(offset: 0x6a4): forward_list.tcc
-  47	(udata)	8	(line_strp)	(offset: 0x6b5): gil.h
-  48	(udata)	4	(line_strp)	(offset: 0x829): exception.h
-  49	(udata)	10	(line_strp)	(offset: 0x6bb): new
-  50	(udata)	11	(line_strp)	(offset: 0x6bf): tupleobject.h
-  51	(udata)	11	(line_strp)	(offset: 0x6cd): methodobject.h
-  52	(udata)	12	(line_strp)	(offset: 0x6dc): string_fortified.h
-  53	(udata)	9	(line_strp)	(offset: 0x6ef): options.h
-  54	(udata)	13	(line_strp)	(offset: 0x556): string.h
-  55	(udata)	10	(line_strp)	(offset: 0x6f9): array
-  56	(udata)	14	(line_strp)	(offset: 0x6ff): stddef.h
-  57	(udata)	13	(line_strp)	(offset: 0x708): stdlib.h
-  58	(udata)	12	(line_strp)	(offset: 0x7a5): types.h
-  59	(udata)	15	(line_strp)	(offset: 0x7a5): types.h
-  60	(udata)	16	(line_strp)	(offset: 0x711): clock_t.h
-  61	(udata)	16	(line_strp)	(offset: 0x71b): time_t.h
-  62	(udata)	12	(line_strp)	(offset: 0x724): stdint-intn.h
-  63	(udata)	12	(line_strp)	(offset: 0x732): pthreadtypes.h
-  64	(udata)	10	(line_strp)	(offset: 0x741): cstdlib
-  65	(udata)	4	(line_strp)	(offset: 0x749): std_abs.h
-  66	(udata)	4	(line_strp)	(offset: 0x753): cpp_type_traits.h
-  67	(udata)	10	(line_strp)	(offset: 0x765): cmath
-  68	(udata)	10	(line_strp)	(offset: 0x76b): cstddef
-  69	(udata)	10	(line_strp)	(offset: 0x773): cstring
-  70	(udata)	10	(line_strp)	(offset: 0x77b): type_traits
-  71	(udata)	17	(line_strp)	(offset: 0x787): c++config.h
-  72	(udata)	4	(line_strp)	(offset: 0x793): stl_iterator_base_types.h
-  73	(udata)	18	(line_strp)	(offset: 0x7ad): debug.h
-  74	(udata)	4	(line_strp)	(offset: 0x7b5): uses_allocator.h
-  75	(udata)	10	(line_strp)	(offset: 0x7c6): utility
-  76	(udata)	10	(line_strp)	(offset: 0x7ce): cwchar
-  77	(udata)	10	(line_strp)	(offset: 0x7d5): cstdint
-  78	(udata)	10	(line_strp)	(offset: 0x7dd): clocale
-  79	(udata)	10	(line_strp)	(offset: 0x7e5): cstdio
-  80	(udata)	10	(line_strp)	(offset: 0x7ec): initializer_list
-  81	(udata)	4	(line_strp)	(offset: 0x7fd): stringfwd.h
-  82	(udata)	4	(line_strp)	(offset: 0x809): enable_special_members.h
-  83	(udata)	4	(line_strp)	(offset: 0x822): nested_exception.h
-  84	(udata)	4	(line_strp)	(offset: 0x835): std_function.h
-  85	(udata)	10	(line_strp)	(offset: 0x844): functional
-  86	(udata)	4	(line_strp)	(offset: 0x84f): refwrap.h
-  87	(udata)	10	(line_strp)	(offset: 0x859): ctime
-  88	(udata)	10	(line_strp)	(offset: 0x85f): chrono
-  89	(udata)	10	(line_strp)	(offset: 0x866): system_error
-  90	(udata)	4	(line_strp)	(offset: 0x873): std_mutex.h
-  91	(udata)	4	(line_strp)	(offset: 0x87f): ptr_traits.h
-  92	(udata)	10	(line_strp)	(offset: 0x88c): stdexcept
-  93	(udata)	4	(line_strp)	(offset: 0x896): hash_bytes.h
-  94	(udata)	4	(line_strp)	(offset: 0x8a3): functexcept.h
-  95	(udata)	12	(line_strp)	(offset: 0x8b1): stdlib-float.h
-  96	(udata)	12	(line_strp)	(offset: 0x8c0): stdlib-bsearch.h
-  97	(udata)	12	(line_strp)	(offset: 0x708): stdlib.h
-  98	(udata)	4	(line_strp)	(offset: 0x8d1): predefined_ops.h
-  99	(udata)	5	(line_strp)	(offset: 0x8e2): concurrence.h
-  100	(udata)	5	(line_strp)	(offset: 0x8f0): aligned_buffer.h
-  101	(udata)	5	(line_strp)	(offset: 0x757): type_traits.h
-  102	(udata)	10	(line_strp)	(offset: 0x708): stdlib.h
-  103	(udata)	0	(line_strp)	(offset: 0x901): <built-in>
-  104	(udata)	16	(line_strp)	(offset: 0x90c): __mbstate_t.h
-  105	(udata)	16	(line_strp)	(offset: 0x91a): __fpos64_t.h
-  106	(udata)	16	(line_strp)	(offset: 0x927): __FILE.h
-  107	(udata)	16	(line_strp)	(offset: 0x930): struct_FILE.h
-  108	(udata)	16	(line_strp)	(offset: 0x929): FILE.h
-  109	(udata)	13	(line_strp)	(offset: 0x93e): stdio.h
-  110	(udata)	13	(line_strp)	(offset: 0x946): unistd.h
-  111	(udata)	16	(line_strp)	(offset: 0x94f): wint_t.h
-  112	(udata)	16	(line_strp)	(offset: 0x90e): mbstate_t.h
-  113	(udata)	12	(line_strp)	(offset: 0x958): stdint-uintn.h
-  114	(udata)	13	(line_strp)	(offset: 0x967): stdint.h
-  115	(udata)	3	(line_strp)	(offset: 0x970): pyport.h
-  116	(udata)	13	(line_strp)	(offset: 0x979): math.h
-  117	(udata)	10	(line_strp)	(offset: 0x979): math.h
-  118	(udata)	16	(line_strp)	(offset: 0x980): struct_tm.h
-  119	(udata)	3	(line_strp)	(offset: 0x98c): pytypedefs.h
-  120	(udata)	3	(line_strp)	(offset: 0x999): moduleobject.h
-  121	(udata)	3	(line_strp)	(offset: 0x6cd): methodobject.h
-  122	(udata)	3	(line_strp)	(offset: 0x9a8): descrobject.h
-  123	(udata)	11	(line_strp)	(offset: 0x6d3): object.h
-  124	(udata)	11	(line_strp)	(offset: 0x9b6): code.h
-  125	(udata)	11	(line_strp)	(offset: 0x9bd): pystate.h
-  126	(udata)	3	(line_strp)	(offset: 0x9c7): pybuffer.h
-  127	(udata)	3	(line_strp)	(offset: 0x9d2): bytearrayobject.h
-  128	(udata)	3	(line_strp)	(offset: 0x9e4): floatobject.h
-  129	(udata)	11	(line_strp)	(offset: 0x9f2): listobject.h
-  130	(udata)	3	(line_strp)	(offset: 0x9ff): dictobject.h
-  131	(udata)	11	(line_strp)	(offset: 0xa0c): classobject.h
-  132	(udata)	3	(line_strp)	(offset: 0xa1a): pycapsule.h
-  133	(udata)	11	(line_strp)	(offset: 0xa26): traceback.h
-  134	(udata)	3	(line_strp)	(offset: 0x9bd): pystate.h
-  135	(udata)	3	(line_strp)	(offset: 0xa32): pyerrors.h
-  136	(udata)	3	(line_strp)	(offset: 0xa3d): pythread.h
-  137	(udata)	11	(line_strp)	(offset: 0xa3d): pythread.h
-  138	(udata)	13	(line_strp)	(offset: 0xa48): wchar.h
-  139	(udata)	12	(line_strp)	(offset: 0xa50): wchar2.h
-  140	(udata)	17	(line_strp)	(offset: 0xa59): atomic_word.h
-  141	(udata)	15	(line_strp)	(offset: 0xa67): single_threaded.h
-  142	(udata)	13	(line_strp)	(offset: 0xa79): locale.h
-  143	(udata)	12	(line_strp)	(offset: 0xa82): stdio2.h
-  144	(udata)	12	(line_strp)	(offset: 0x93e): stdio.h
-  145	(udata)	6	(line_strp)	(offset: 0xa8b): descr.h
-  146	(udata)	7	(line_strp)	(offset: 0xa93): buffer_info.h
-  147	(udata)	8	(line_strp)	(offset: 0xaa1): typing.h
-  148	(udata)	4	(line_strp)	(offset: 0xaaa): cxxabi_init_exception.h
-  149	(udata)	10	(line_strp)	(offset: 0xac2): cxxabi.h
-  150	(udata)	13	(line_strp)	(offset: 0xacb): time.h
-  151	(udata)	3	(line_strp)	(offset: 0xad2): modsupport.h
-  152	(udata)	3	(line_strp)	(offset: 0xadf): longobject.h
-  153	(udata)	3	(line_strp)	(offset: 0xaec): abstract.h
-  154	(udata)	3	(line_strp)	(offset: 0xaf7): pymem.h
-  155	(udata)	3	(line_strp)	(offset: 0xaff): objimpl.h
-  156	(udata)	3	(line_strp)	(offset: 0xb09): weakrefobject.h
-  157	(udata)	3	(line_strp)	(offset: 0xb19): unicodeobject.h
-  158	(udata)	3	(line_strp)	(offset: 0x6bf): tupleobject.h
-  159	(udata)	3	(line_strp)	(offset: 0xb29): ceval.h
-  160	(udata)	3	(line_strp)	(offset: 0xb31): bytesobject.h
-  161	(udata)	11	(line_strp)	(offset: 0xb3f): pyframe.h
-  162	(udata)	3	(line_strp)	(offset: 0xb3f): pyframe.h
-  163	(udata)	3	(line_strp)	(offset: 0x9f2): listobject.h
-  164	(udata)	3	(line_strp)	(offset: 0xb49): pylifecycle.h
+  0	(udata)	1	(line_strp)	(offset: 0x2d): .rendered.somecode.cpp
+  1	(udata)	2	(line_strp)	(offset: 0x490): class.h
+  2	(udata)	3	(line_strp)	(offset: 0x6e7): object.h
+  3	(udata)	1	(line_strp)	(offset: 0x2d): .rendered.somecode.cpp
+  4	(udata)	4	(line_strp)	(offset: 0x498): shared_ptr_base.h
+  5	(udata)	4	(line_strp)	(offset: 0x7ce): allocator.h
+  6	(udata)	5	(line_strp)	(offset: 0x4aa): new_allocator.h
+  7	(udata)	4	(line_strp)	(offset: 0x4ba): allocated_ptr.h
+  8	(udata)	4	(line_strp)	(offset: 0x4ca): move.h
+  9	(udata)	4	(line_strp)	(offset: 0x4d1): alloc_traits.h
+  10	(udata)	6	(line_strp)	(offset: 0x4e0): common.h
+  11	(udata)	7	(line_strp)	(offset: 0x4e9): pytypes.h
+  12	(udata)	4	(line_strp)	(offset: 0x4f3): shared_ptr.h
+  13	(udata)	5	(line_strp)	(offset: 0x500): atomicity.h
+  14	(udata)	4	(line_strp)	(offset: 0x50c): hashtable.h
+  15	(udata)	4	(line_strp)	(offset: 0x518): hashtable_policy.h
+  16	(udata)	4	(line_strp)	(offset: 0x52b): functional_hash.h
+  17	(udata)	4	(line_strp)	(offset: 0x53d): stl_function.h
+  18	(udata)	4	(line_strp)	(offset: 0x54c): stl_vector.h
+  19	(udata)	4	(line_strp)	(offset: 0x559): stl_pair.h
+  20	(udata)	4	(line_strp)	(offset: 0x564): basic_string.h
+  21	(udata)	4	(line_strp)	(offset: 0x573): char_traits.h
+  22	(udata)	8	(line_strp)	(offset: 0x581): pybind11.h
+  23	(udata)	9	(line_strp)	(offset: 0x58c): attr.h
+  24	(udata)	4	(line_strp)	(offset: 0x593): unique_ptr.h
+  25	(udata)	10	(line_strp)	(offset: 0x5a0): tuple
+  26	(udata)	10	(line_strp)	(offset: 0x5a6): typeinfo
+  27	(udata)	4	(line_strp)	(offset: 0x5af): basic_string.tcc
+  28	(udata)	4	(line_strp)	(offset: 0x5c0): stl_iterator_base_funcs.h
+  29	(udata)	4	(line_strp)	(offset: 0x5da): vector.tcc
+  30	(udata)	4	(line_strp)	(offset: 0x5e5): stl_bvector.h
+  31	(udata)	4	(line_strp)	(offset: 0x5f3): stl_algobase.h
+  32	(udata)	10	(line_strp)	(offset: 0x602): typeindex
+  33	(udata)	4	(line_strp)	(offset: 0x60c): stl_iterator.h
+  34	(udata)	4	(line_strp)	(offset: 0x61b): charconv.h
+  35	(udata)	6	(line_strp)	(offset: 0x626): internals.h
+  36	(udata)	6	(line_strp)	(offset: 0x632): typeid.h
+  37	(udata)	6	(line_strp)	(offset: 0x63b): type_caster_base.h
+  38	(udata)	9	(line_strp)	(offset: 0x64e): cast.h
+  39	(udata)	5	(line_strp)	(offset: 0x4d1): alloc_traits.h
+  40	(udata)	4	(line_strp)	(offset: 0x655): forward_list.h
+  41	(udata)	4	(line_strp)	(offset: 0x664): exception_ptr.h
+  42	(udata)	4	(line_strp)	(offset: 0x674): stl_construct.h
+  43	(udata)	4	(line_strp)	(offset: 0x684): stl_uninitialized.h
+  44	(udata)	4	(line_strp)	(offset: 0x698): unordered_map.h
+  45	(udata)	4	(line_strp)	(offset: 0x6a8): unordered_set.h
+  46	(udata)	4	(line_strp)	(offset: 0x6b8): forward_list.tcc
+  47	(udata)	8	(line_strp)	(offset: 0x6c9): gil.h
+  48	(udata)	4	(line_strp)	(offset: 0x83d): exception.h
+  49	(udata)	10	(line_strp)	(offset: 0x6cf): new
+  50	(udata)	11	(line_strp)	(offset: 0x6d3): tupleobject.h
+  51	(udata)	11	(line_strp)	(offset: 0x6e1): methodobject.h
+  52	(udata)	12	(line_strp)	(offset: 0x6f0): string_fortified.h
+  53	(udata)	9	(line_strp)	(offset: 0x703): options.h
+  54	(udata)	13	(line_strp)	(offset: 0x56a): string.h
+  55	(udata)	10	(line_strp)	(offset: 0x70d): array
+  56	(udata)	14	(line_strp)	(offset: 0x713): stddef.h
+  57	(udata)	13	(line_strp)	(offset: 0x71c): stdlib.h
+  58	(udata)	12	(line_strp)	(offset: 0x7b9): types.h
+  59	(udata)	15	(line_strp)	(offset: 0x7b9): types.h
+  60	(udata)	16	(line_strp)	(offset: 0x725): clock_t.h
+  61	(udata)	16	(line_strp)	(offset: 0x72f): time_t.h
+  62	(udata)	12	(line_strp)	(offset: 0x738): stdint-intn.h
+  63	(udata)	12	(line_strp)	(offset: 0x746): pthreadtypes.h
+  64	(udata)	10	(line_strp)	(offset: 0x755): cstdlib
+  65	(udata)	4	(line_strp)	(offset: 0x75d): std_abs.h
+  66	(udata)	4	(line_strp)	(offset: 0x767): cpp_type_traits.h
+  67	(udata)	10	(line_strp)	(offset: 0x779): cmath
+  68	(udata)	10	(line_strp)	(offset: 0x77f): cstddef
+  69	(udata)	10	(line_strp)	(offset: 0x787): cstring
+  70	(udata)	10	(line_strp)	(offset: 0x78f): type_traits
+  71	(udata)	17	(line_strp)	(offset: 0x79b): c++config.h
+  72	(udata)	4	(line_strp)	(offset: 0x7a7): stl_iterator_base_types.h
+  73	(udata)	18	(line_strp)	(offset: 0x7c1): debug.h
+  74	(udata)	4	(line_strp)	(offset: 0x7c9): uses_allocator.h
+  75	(udata)	10	(line_strp)	(offset: 0x7da): utility
+  76	(udata)	10	(line_strp)	(offset: 0x7e2): cwchar
+  77	(udata)	10	(line_strp)	(offset: 0x7e9): cstdint
+  78	(udata)	10	(line_strp)	(offset: 0x7f1): clocale
+  79	(udata)	10	(line_strp)	(offset: 0x7f9): cstdio
+  80	(udata)	10	(line_strp)	(offset: 0x800): initializer_list
+  81	(udata)	4	(line_strp)	(offset: 0x811): stringfwd.h
+  82	(udata)	4	(line_strp)	(offset: 0x81d): enable_special_members.h
+  83	(udata)	4	(line_strp)	(offset: 0x836): nested_exception.h
+  84	(udata)	4	(line_strp)	(offset: 0x849): std_function.h
+  85	(udata)	10	(line_strp)	(offset: 0x858): functional
+  86	(udata)	4	(line_strp)	(offset: 0x863): refwrap.h
+  87	(udata)	10	(line_strp)	(offset: 0x86d): ctime
+  88	(udata)	10	(line_strp)	(offset: 0x873): chrono
+  89	(udata)	10	(line_strp)	(offset: 0x87a): system_error
+  90	(udata)	4	(line_strp)	(offset: 0x887): std_mutex.h
+  91	(udata)	4	(line_strp)	(offset: 0x893): ptr_traits.h
+  92	(udata)	10	(line_strp)	(offset: 0x8a0): stdexcept
+  93	(udata)	4	(line_strp)	(offset: 0x8aa): hash_bytes.h
+  94	(udata)	4	(line_strp)	(offset: 0x8b7): functexcept.h
+  95	(udata)	12	(line_strp)	(offset: 0x8c5): stdlib-float.h
+  96	(udata)	12	(line_strp)	(offset: 0x8d4): stdlib-bsearch.h
+  97	(udata)	12	(line_strp)	(offset: 0x71c): stdlib.h
+  98	(udata)	4	(line_strp)	(offset: 0x8e5): predefined_ops.h
+  99	(udata)	5	(line_strp)	(offset: 0x8f6): concurrence.h
+  100	(udata)	5	(line_strp)	(offset: 0x904): aligned_buffer.h
+  101	(udata)	5	(line_strp)	(offset: 0x76b): type_traits.h
+  102	(udata)	10	(line_strp)	(offset: 0x71c): stdlib.h
+  103	(udata)	0	(line_strp)	(offset: 0x915): <built-in>
+  104	(udata)	16	(line_strp)	(offset: 0x920): __mbstate_t.h
+  105	(udata)	16	(line_strp)	(offset: 0x92e): __fpos64_t.h
+  106	(udata)	16	(line_strp)	(offset: 0x93b): __FILE.h
+  107	(udata)	16	(line_strp)	(offset: 0x944): struct_FILE.h
+  108	(udata)	16	(line_strp)	(offset: 0x93d): FILE.h
+  109	(udata)	13	(line_strp)	(offset: 0x952): stdio.h
+  110	(udata)	13	(line_strp)	(offset: 0x95a): unistd.h
+  111	(udata)	16	(line_strp)	(offset: 0x963): wint_t.h
+  112	(udata)	16	(line_strp)	(offset: 0x922): mbstate_t.h
+  113	(udata)	12	(line_strp)	(offset: 0x96c): stdint-uintn.h
+  114	(udata)	13	(line_strp)	(offset: 0x97b): stdint.h
+  115	(udata)	3	(line_strp)	(offset: 0x984): pyport.h
+  116	(udata)	13	(line_strp)	(offset: 0x98d): math.h
+  117	(udata)	10	(line_strp)	(offset: 0x98d): math.h
+  118	(udata)	16	(line_strp)	(offset: 0x994): struct_tm.h
+  119	(udata)	3	(line_strp)	(offset: 0x9a0): pytypedefs.h
+  120	(udata)	3	(line_strp)	(offset: 0x9ad): moduleobject.h
+  121	(udata)	3	(line_strp)	(offset: 0x6e1): methodobject.h
+  122	(udata)	3	(line_strp)	(offset: 0x9bc): descrobject.h
+  123	(udata)	11	(line_strp)	(offset: 0x6e7): object.h
+  124	(udata)	11	(line_strp)	(offset: 0x9ca): code.h
+  125	(udata)	11	(line_strp)	(offset: 0x9d1): pystate.h
+  126	(udata)	3	(line_strp)	(offset: 0x9db): pybuffer.h
+  127	(udata)	3	(line_strp)	(offset: 0x9e6): bytearrayobject.h
+  128	(udata)	3	(line_strp)	(offset: 0x9f8): floatobject.h
+  129	(udata)	11	(line_strp)	(offset: 0xa06): listobject.h
+  130	(udata)	3	(line_strp)	(offset: 0xa13): dictobject.h
+  131	(udata)	11	(line_strp)	(offset: 0xa20): classobject.h
+  132	(udata)	3	(line_strp)	(offset: 0xa2e): pycapsule.h
+  133	(udata)	11	(line_strp)	(offset: 0xa3a): traceback.h
+  134	(udata)	3	(line_strp)	(offset: 0x9d1): pystate.h
+  135	(udata)	3	(line_strp)	(offset: 0xa46): pyerrors.h
+  136	(udata)	3	(line_strp)	(offset: 0xa51): pythread.h
+  137	(udata)	11	(line_strp)	(offset: 0xa51): pythread.h
+  138	(udata)	13	(line_strp)	(offset: 0xa5c): wchar.h
+  139	(udata)	12	(line_strp)	(offset: 0xa64): wchar2.h
+  140	(udata)	17	(line_strp)	(offset: 0xa6d): atomic_word.h
+  141	(udata)	15	(line_strp)	(offset: 0xa7b): single_threaded.h
+  142	(udata)	13	(line_strp)	(offset: 0xa8d): locale.h
+  143	(udata)	12	(line_strp)	(offset: 0xa96): stdio2.h
+  144	(udata)	12	(line_strp)	(offset: 0x952): stdio.h
+  145	(udata)	6	(line_strp)	(offset: 0xa9f): descr.h
+  146	(udata)	7	(line_strp)	(offset: 0xaa7): buffer_info.h
+  147	(udata)	8	(line_strp)	(offset: 0xab5): typing.h
+  148	(udata)	4	(line_strp)	(offset: 0xabe): cxxabi_init_exception.h
+  149	(udata)	10	(line_strp)	(offset: 0xad6): cxxabi.h
+  150	(udata)	13	(line_strp)	(offset: 0xadf): time.h
+  151	(udata)	3	(line_strp)	(offset: 0xae6): modsupport.h
+  152	(udata)	3	(line_strp)	(offset: 0xaf3): longobject.h
+  153	(udata)	3	(line_strp)	(offset: 0xb00): abstract.h
+  154	(udata)	3	(line_strp)	(offset: 0xb0b): pymem.h
+  155	(udata)	3	(line_strp)	(offset: 0xb13): objimpl.h
+  156	(udata)	3	(line_strp)	(offset: 0xb1d): weakrefobject.h
+  157	(udata)	3	(line_strp)	(offset: 0xb2d): unicodeobject.h
+  158	(udata)	3	(line_strp)	(offset: 0x6d3): tupleobject.h
+  159	(udata)	3	(line_strp)	(offset: 0xb3d): ceval.h
+  160	(udata)	3	(line_strp)	(offset: 0xb45): bytesobject.h
+  161	(udata)	11	(line_strp)	(offset: 0xb53): pyframe.h
+  162	(udata)	3	(line_strp)	(offset: 0xb53): pyframe.h
+  163	(udata)	3	(line_strp)	(offset: 0xa06): listobject.h
+  164	(udata)	3	(line_strp)	(offset: 0xb5d): pylifecycle.h
 
  Line Number Statements:
   [0x000003ae]  Set column to 99
   [0x000003b0]  Extended opcode 2: set Address to 0x72b0
   [0x000003bb]  Advance Line by 47 to 48
   [0x000003bd]  Copy
   [0x000003be]  Set is_stmt to 0
```

#### readelf --wide --debug-dump=info {}

```diff
@@ -5,16 +5,16 @@
    Version:       5
    Unit Type:     DW_UT_compile (1)
    Abbrev Offset: 0
    Pointer Size:  8
  <0><c>: Abbrev Number: 318 (DW_TAG_compile_unit)
     <e>   DW_AT_producer    : (strp) (offset: 0x9bfa8): GNU C++11 11.4.0 -mtune=generic -march=x86-64 -g -O3 -std=c++11 -fPIC -fvisibility=hidden -fasynchronous-unwind-tables -fstack-protector-strong -fstack-clash-protection -fcf-protection
     <12>   DW_AT_language    : (data1) 26	(C++11)
-    <13>   DW_AT_name        : (line_strp) (offset: 0): /home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp
-    <17>   DW_AT_comp_dir    : (line_strp) (offset: 0x3a): /home/pietro/Desktop/cpp-py
+    <13>   DW_AT_name        : (line_strp) (offset: 0): /home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp
+    <17>   DW_AT_comp_dir    : (line_strp) (offset: 0x44): /home/pietro/Desktop/cpp-py
     <1b>   DW_AT_ranges      : (sec_offset) 0xc49f
     <1f>   DW_AT_low_pc      : (addr) 0
     <27>   DW_AT_stmt_list   : (sec_offset) 0
  <1><2b>: Abbrev Number: 115 (DW_TAG_base_type)
     <2c>   DW_AT_byte_size   : (data1) 16
     <2d>   DW_AT_encoding    : (data1) 7	(unsigned)
     <2e>   DW_AT_name        : (strp) (offset: 0x608de): __int128 unsigned
```

#### strings --all --bytes=8 {}

```diff
@@ -10212,17 +10212,17 @@
 _ZN8pybind116detail8accessorINS0_17accessor_policies10tuple_itemEED2Ev
 _ZNSt5arrayIPKSt9type_infoLm1EE6rbeginEv
 ~index_error
 _ZNSt8__detail21_Hashtable_ebo_helperILi0ESt8equal_toIPK7_objectELb1EE6_M_getEv
 _ZNSt18unordered_multimapIPKvPN8pybind116detail8instanceESt4hashIS1_ESt8equal_toIS1_ESaISt4pairIKS1_S5_EEE6insertESt16initializer_listISC_E
 rebind<_object* (*)(_object*, _typeobject*)>
 _ZNKSt8__detail10_Hash_nodeIP7_objectLb0EE7_M_nextEv
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp
 /home/pietro/Desktop/cpp-py
-/home/pietro/Desktop/cpp-py/cpp_py
+/home/pietro/Desktop/cpp-py/justatestwithcpp
 /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/detail
 /home/linuxbrew/.linuxbrew/opt/python@3.11/include/python3.11
 /usr/include/c++/11/bits
 /usr/include/c++/11/ext
 /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/detail/../detail
 /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/detail/../detail/..
 /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11
@@ -10737,9 +10737,9 @@
 .debug_info
 .debug_abbrev
 .debug_line
 .debug_str
 .debug_line_str
 .debug_loclists
 .debug_rnglists
-[["/home/pietro/Desktop/cpp-py/cpp_py/somecode.cpp"], "9035d4c3db017ba12773d0182adab301"]Y
+[["/home/pietro/Desktop/cpp-py/justatestwithcpp/somecode.cpp"], "9035d4c3db017ba12773d0182adab301"]c
 cppimport
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -233,20 +233,20 @@
 	lea    0x20(%rsp),%rdi
 	call   6920 <pybind11::handle::dec_ref() const & [clone .isra.0]>
 	lea    0x28(%rsp),%rdi
 	call   6920 <pybind11::handle::dec_ref() const & [clone .isra.0]>
 	mov    %rbp,%rdi
 	mov    %r12,%rax
 PyInit_somecode.cold():
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:10 (discriminator 9)
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:10 (discriminator 9)
 	cmp    $0x1,%rax
 PyInit_somecode():
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:10 (discriminator 9)
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:10 (discriminator 9)
 	je     656d <PyInit_somecode.cold+0xa6>
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:10
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:10
 	cmp    $0x2,%rax
 	je     65cc <PyInit_somecode.cold+0x105>
 	mov    %rdi,%rbp
 	jmp    65ba <PyInit_somecode.cold+0xf3>
 pybind11::object::~object():
 /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/detail/../detail/../pytypes.h:370
 	mov    %rbx,%rdi
@@ -259,81 +259,81 @@
 /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/pybind11.h:1318
 	mov    %rax,%r12
 	mov    %rbp,%rdi
 	call   5c90 <__cxa_free_exception@plt>
 	mov    %r12,%rdi
 	call   61d0 <_Unwind_Resume@plt>
 PyInit_somecode():
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:10 (discriminator 12)
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:10 (discriminator 12)
 	call   5b40 <__cxa_begin_catch@plt>
 	mov    0x17a5f(%rip),%rdx        
 pybind11::error_already_set::restore():
 /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/detail/../detail/../pytypes.h:749 (discriminator 12)
 	mov    0x8(%rax),%rdi
 PyInit_somecode():
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:10 (discriminator 12)
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:10 (discriminator 12)
 	mov    (%rdx),%rbp
 pybind11::error_already_set::restore():
 /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/detail/../detail/../pytypes.h:749 (discriminator 12)
 	call   b900 <pybind11::detail::error_fetch_and_normalize::restore()>
 pybind11::raise_from(pybind11::error_already_set&, _object*, char const*):
 /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/detail/../detail/../pytypes.h:820
 	lea    0x12839(%rip),%rsi        
 	mov    %rbp,%rdi
 	call   8130 <pybind11::raise_from(_object*, char const*)>
 PyInit_somecode():
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:10 (discriminator 15)
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:10 (discriminator 15)
 	call   6100 <__cxa_end_catch@plt>
 pybind11::handle::dec_ref() const &:
 /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/detail/../detail/../pytypes.h:274
 	mov    0x10(%rsp),%rdi
 PyInit_somecode():
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:10
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:10
 	xor    %eax,%eax
 	jmp    7187 <PyInit_somecode+0x227>
 	endbr64
 pybind11::object::~object():
 /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/detail/../detail/../pytypes.h:370
 	mov    %rax,%rbp
 	jmp    65ba <PyInit_somecode.cold+0xf3>
 	endbr64
 PyInit_somecode():
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:10
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:10
 	mov    %rax,%rbp
 	call   6100 <__cxa_end_catch@plt>
 pybind11::object::~object():
 /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/detail/../detail/../pytypes.h:370 (discriminator 17)
 	lea    0x10(%rsp),%rdi
 	call   6920 <pybind11::handle::dec_ref() const & [clone .isra.0]>
 	mov    %rbp,%rdi
 	call   61d0 <_Unwind_Resume@plt>
 PyInit_somecode():
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:10 (discriminator 13)
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:10 (discriminator 13)
 	call   5b40 <__cxa_begin_catch@plt>
 	mov    %rax,%rdi
 	mov    (%rax),%rax
 	call   *0x10(%rax)
 	mov    %rax,%rsi
 pybind11::set_error(pybind11::handle const&, char const*):
 /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/detail/../detail/../pytypes.h:339 (discriminator 13)
 	mov    0x179f4(%rip),%rax        
 	mov    (%rax),%rdi
 	call   5e80 <PyErr_SetString@plt>
 PyInit_somecode():
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:10 (discriminator 19)
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:10 (discriminator 19)
 	call   6100 <__cxa_end_catch@plt>
 pybind11::handle::dec_ref() const &:
 /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/detail/../detail/../pytypes.h:274 (discriminator 19)
 	mov    0x10(%rsp),%rdi
 PyInit_somecode():
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:10 (discriminator 19)
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:10 (discriminator 19)
 	xor    %eax,%eax
 	jmp    7187 <PyInit_somecode+0x227>
 	endbr64
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:10
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:10
 	mov    %rax,%rbp
 	call   6100 <__cxa_end_catch@plt>
 	jmp    65ba <PyInit_somecode.cold+0xf3>
 PyInit_somecode.cold():
 	nopl   0x0(%rax,%rax,1)
 
 0000000000006610 <deregister_tm_clones>:
@@ -392,20 +392,20 @@
 frame_dummy():
 	endbr64
 	jmp    6640 <register_tm_clones>
 	nopl   0x0(%rax)
 
 00000000000066d0 <square(int)>:
 square(int):
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:6
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:6
 	endbr64
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:7
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:7
 	mov    %edi,%eax
 	imul   %edi,%eax
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:8
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:8
 	ret
 	nopw   0x0(%rax,%rax,1)
 
 00000000000066e0 <std::_Hashtable<_typeobject*, std::pair<_typeobject* const, std::vector<pybind11::detail::type_info*, std::allocator<pybind11::detail::type_info*> > >, std::allocator<std::pair<_typeobject* const, std::vector<pybind11::detail::type_info*, std::allocator<pybind11::detail::type_info*> > > >, std::__detail::_Select1st, std::equal_to<_typeobject*>, std::hash<_typeobject*>, std::__detail::_Mod_range_hashing, std::__detail::_Default_ranged_hash, std::__detail::_Prime_rehash_policy, std::__detail::_Hashtable_traits<false, false, true> >::_M_erase(std::integral_constant<bool, true>, _typeobject* const&) [clone .isra.0]>:
 std::_Hashtable<_typeobject*, std::pair<_typeobject* const, std::vector<pybind11::detail::type_info*, std::allocator<pybind11::detail::type_info*> > >, std::allocator<std::pair<_typeobject* const, std::vector<pybind11::detail::type_info*, std::allocator<pybind11::detail::type_info*> > > >, std::__detail::_Select1st, std::equal_to<_typeobject*>, std::hash<_typeobject*>, std::__detail::_Mod_range_hashing, std::__detail::_Default_ranged_hash, std::__detail::_Prime_rehash_policy, std::__detail::_Hashtable_traits<false, false, true> >::_M_erase(std::integral_constant<bool, true>, _typeobject* const&):
 /usr/include/c++/11/bits/hashtable.h:2194
 	push   %r13
@@ -1541,15 +1541,15 @@
 	jmp    64a4 <pybind11::detail::all_type_info_populate(_typeobject*, std::vector<pybind11::detail::type_info*, std::allocator<pybind11::detail::type_info*> >&) [clone .isra.0] [clone .cold]+0xa>
 pybind11::detail::all_type_info_populate(_typeobject*, std::vector<pybind11::detail::type_info*, std::allocator<pybind11::detail::type_info*> >&) [clone .isra.0]:
 /usr/include/c++/11/bits/stl_vector.h:680
 	nopl   0x0(%rax,%rax,1)
 
 0000000000006f60 <PyInit_somecode>:
 PyInit_somecode():
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:10
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:10
 	endbr64
 	push   %r15
 	push   %r14
 	push   %r13
 	lea    0x11e3f(%rip),%r13        
 	push   %r12
 	push   %rbp
@@ -1562,20 +1562,20 @@
 	mov    $0x4,%edx
 	mov    %r13,%rsi
 	mov    %rax,%rdi
 	mov    %rax,%r12
 	call   5b80 <strncmp@plt>
 	test   %eax,%eax
 	jne    71b8 <PyInit_somecode+0x258>
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:10 (discriminator 3)
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:10 (discriminator 3)
 	movzbl 0x4(%r12),%eax
 	sub    $0x30,%eax
 	cmp    $0x9,%al
 	jbe    71b8 <PyInit_somecode+0x258>
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:10 (discriminator 5)
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:10 (discriminator 5)
 	call   c6f0 <pybind11::detail::get_internals()>
 pybind11::module_::create_extension_module(char const*, char const*, PyModuleDef*):
 /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/pybind11.h:1314 (discriminator 5)
 	pxor   %xmm0,%xmm0
 	lea    0x11deb(%rip),%rax        
 /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/pybind11.h:1315 (discriminator 5)
 	mov    $0x3f5,%esi
@@ -1735,43 +1735,43 @@
 PyInit_somecode():
 /home/linuxbrew/.linuxbrew/opt/python@3.11/include/python3.11/object.h:537
 	subq   $0x1,(%rdi)
 Py_DECREF():
 /home/linuxbrew/.linuxbrew/opt/python@3.11/include/python3.11/object.h:537
 	je     7218 <PyInit_somecode+0x2b8>
 PyInit_somecode():
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:10
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:10
 	mov    0x10(%rsp),%rax
 	mov    %rax,%rdi
 /home/linuxbrew/.linuxbrew/opt/python@3.11/include/python3.11/object.h:601 (discriminator 21)
 	test   %rdi,%rdi
 Py_XDECREF():
 /home/linuxbrew/.linuxbrew/opt/python@3.11/include/python3.11/object.h:601 (discriminator 21)
 	je     7192 <PyInit_somecode+0x232>
 PyInit_somecode():
 /home/linuxbrew/.linuxbrew/opt/python@3.11/include/python3.11/object.h:537
 	subq   $0x1,(%rdi)
 Py_DECREF():
 /home/linuxbrew/.linuxbrew/opt/python@3.11/include/python3.11/object.h:537
 	je     7200 <PyInit_somecode+0x2a0>
 PyInit_somecode():
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:10
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:10
 	mov    0x38(%rsp),%rdx
 	sub    %fs:0x28,%rdx
 	jne    725b <PyInit_somecode+0x2fb>
 	add    $0x48,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
 	nopl   (%rax)
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:10 (discriminator 4)
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:10 (discriminator 4)
 	mov    0x16e19(%rip),%rax        
 	mov    %r12,%rcx
 	mov    %r13,%rdx
 	lea    0x10e64(%rip),%rsi        
 	mov    (%rax),%rdi
 	xor    %eax,%eax
 	call   5c60 <PyErr_Format@plt>
@@ -1819,15 +1819,15 @@
 pybind11::module_::create_extension_module(char const*, char const*, PyModuleDef*):
 /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/pybind11.h:1317
 	call   60c0 <PyErr_Occurred@plt>
 	test   %rax,%rax
 	je     64c7 <PyInit_somecode.cold>
 	jmp    64d3 <PyInit_somecode.cold+0xc>
 PyInit_somecode():
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:10
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:10
 	call   5e50 <__stack_chk_fail@plt>
 	endbr64
 pybind11::object::~object():
 /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/detail/../detail/../pytypes.h:370
 	mov    %rax,%rbp
 	mov    %rdx,%r12
 	lea    0x18(%rsp),%rbx
@@ -1850,28 +1850,28 @@
 	jmp    6521 <PyInit_somecode.cold+0x5a>
 PyInit_somecode():
 	cs nopw 0x0(%rax,%rax,1)
 	nopl   0x0(%rax,%rax,1)
 
 00000000000072b0 <pybind11_static_get>:
 pybind11_static_get():
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:48
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:48
 	endbr64
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:49
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:49
 	mov    0x16c7d(%rip),%rax        
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:48
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:48
 	mov    %rdx,%rsi
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:49
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:49
 	mov    0x110(%rax),%rax
 	jmp    *%rax
 	nopw   0x0(%rax,%rax,1)
 
 00000000000072d0 <pybind11_static_set>:
 pybind11_static_set():
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:53
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:53
 	endbr64
 /home/linuxbrew/.linuxbrew/opt/python@3.11/include/python3.11/object.h:133
 	mov    0x8(%rsi),%rax
 /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/detail/class.h:54
 	testb  $0x80,0xab(%rax)
 	cmove  %rax,%rsi
 /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/detail/class.h:55
@@ -1964,24 +1964,24 @@
 /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/detail/../detail/common.h:1020
 	mov    %rbp,%rdi
 	pop    %rbp
 	jmp    5dc0 <operator delete(void*)@plt>
 
 00000000000073b0 <pybind11_meta_getattro>:
 pybind11_meta_getattro():
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:173
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:173
 	endbr64
 	push   %r12
 	mov    %rsi,%r12
 	push   %rbp
 	mov    %rdi,%rbp
 	sub    $0x8,%rsp
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:174
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:174
 	call   6190 <_PyType_Lookup@plt>
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:175
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:175
 	test   %rax,%rax
 	je     73d8 <pybind11_meta_getattro+0x28>
 	mov    0x16aee(%rip),%rdx        
 	cmp    %rdx,0x8(%rax)
 	je     73f8 <pybind11_meta_getattro+0x48>
 /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/detail/class.h:179 (discriminator 4)
 	mov    0x16b29(%rip),%rax        
@@ -3138,23 +3138,23 @@
 	pop    %r13
 	ret
 	ret
 	nopl   0x0(%rax)
 
 0000000000007cc0 <pybind11_object_init>:
 pybind11_object_init():
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:372
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:372
 	endbr64
 	push   %r13
 	push   %r12
 	push   %rbp
 	push   %rbx
 	sub    $0x68,%rsp
 pybind11::detail::get_fully_qualified_tp_name[abi:cxx11](_typeobject*):
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:30
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:30
 	mov    %fs:0x28,%rax
 	mov    %rax,0x58(%rsp)
 	mov    0x8(%rdi),%rax
 std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_Alloc_hider::_Alloc_hider(char*, std::allocator<char> const&):
 /usr/include/c++/11/bits/basic_string.h:165
 	lea    0x40(%rsp),%rbx
 	mov    %rbx,0x30(%rsp)
@@ -13555,57 +13555,57 @@
 	jmp    ddda <pybind11::capsule::initialize_with_void_ptr_destructor(void const*, char const*, void (*)(void*))::{lambda(_object*)#1}::_FUN(_object*)+0x1aa>
 pybind11::capsule::initialize_with_void_ptr_destructor(void const*, char const*, void (*)(void*))::{lambda(_object*)#1}::_FUN(_object*):
 	cs nopw 0x0(%rax,%rax,1)
 	nop
 
 000000000000ddf0 <pybind11_meta_setattro>:
 pybind11_meta_setattro():
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:136
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:136
 	endbr64
 	push   %r15
 	push   %r14
 	push   %r13
 	mov    %rdx,%r13
 	push   %r12
 	mov    %rsi,%r12
 	push   %rbp
 	mov    %rdi,%rbp
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:139
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:139
 	call   6190 <_PyType_Lookup@plt>
 	mov    %rax,%r14
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:145
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:145
 	call   c6f0 <pybind11::detail::get_internals()>
 	mov    0x1b0(%rax),%r15
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:148
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:148
 	test   %r14,%r14
 	je     de24 <pybind11_meta_setattro+0x34>
 	test   %r13,%r13
 	jne    de50 <pybind11_meta_setattro+0x60>
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:163
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:163
 	mov    0x100dd(%rip),%rax        
 	mov    %r13,%rdx
 	mov    %r12,%rsi
 	mov    %rbp,%rdi
 	mov    0x98(%rax),%rax
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:165
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:165
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:163
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:163
 	jmp    *%rax
 	cs nopw 0x0(%rax,%rax,1)
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:147
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:147
 	mov    %r15,%rsi
 	mov    %r14,%rdi
 	call   5bc0 <PyObject_IsInstance@plt>
 	test   %eax,%eax
 	je     de24 <pybind11_meta_setattro+0x34>
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:148 (discriminator 3)
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:148 (discriminator 3)
 	mov    %r15,%rsi
 	mov    %r13,%rdi
 	call   5bc0 <PyObject_IsInstance@plt>
 	test   %eax,%eax
 	jne    de24 <pybind11_meta_setattro+0x34>
 /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/detail/class.h:152
 	mov    0x8(%r14),%rax
@@ -13615,22 +13615,22 @@
 	mov    0x118(%rax),%rax
 	jmp    de3b <pybind11_meta_setattro+0x4b>
 	cs nopw 0x0(%rax,%rax,1)
 	xchg   %ax,%ax
 
 000000000000de90 <pybind11::detail::deregister_instance_impl(void*, pybind11::detail::instance*)>:
 pybind11::detail::deregister_instance_impl(void*, pybind11::detail::instance*):
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:316
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:316
 	endbr64
 	push   %r12
 	mov    %rdi,%r12
 	push   %rbp
 	push   %rbx
 	mov    %rsi,%rbx
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:317
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:317
 	call   c6f0 <pybind11::detail::get_internals()>
 std::__detail::_Mod_range_hashing::operator()(unsigned long, unsigned long) const:
 /usr/include/c++/11/bits/hashtable_policy.h:430
 	xor    %edx,%edx
 std::_Hashtable<void const*, std::pair<void const* const, pybind11::detail::instance*>, std::allocator<std::pair<void const* const, pybind11::detail::instance*> >, std::__detail::_Select1st, std::equal_to<void const*>, std::hash<void const*>, std::__detail::_Mod_range_hashing, std::__detail::_Default_ranged_hash, std::__detail::_Prime_rehash_policy, std::__detail::_Hashtable_traits<false, false, false> >::_M_bucket_index(unsigned long) const:
 /usr/include/c++/11/bits/hashtable.h:795
 	mov    0x78(%rax),%r8
@@ -18855,28 +18855,28 @@
 	jmp    11074 <pybind11::cpp_function::initialize_generic(std::unique_ptr<pybind11::detail::function_record, pybind11::cpp_function::InitializingFunctionRecordDeleter>&&, char const*, std::type_info const* const*, unsigned long)+0x2324>
 pybind11::cpp_function::initialize_generic(std::unique_ptr<pybind11::detail::function_record, pybind11::cpp_function::InitializingFunctionRecordDeleter>&&, char const*, std::type_info const* const*, unsigned long):
 	cs nopw 0x0(%rax,%rax,1)
 	nopl   (%rax)
 
 0000000000011170 <pybind11_meta_dealloc>:
 pybind11_meta_dealloc():
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:207
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:207
 	endbr64
 	push   %r15
 	push   %r14
 	push   %r13
 	push   %r12
 	push   %rbp
 	mov    %rdi,%rbp
 	push   %rbx
 	sub    $0x38,%rsp
 	mov    %fs:0x28,%rax
 	mov    %rax,0x28(%rsp)
 	xor    %eax,%eax
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:209
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:209
 	call   c6f0 <pybind11::detail::get_internals()>
 std::__detail::_Mod_range_hashing::operator()(unsigned long, unsigned long) const:
 /usr/include/c++/11/bits/hashtable_policy.h:430
 	xor    %edx,%edx
 std::_Hashtable<_typeobject*, std::pair<_typeobject* const, std::vector<pybind11::detail::type_info*, std::allocator<pybind11::detail::type_info*> > >, std::allocator<std::pair<_typeobject* const, std::vector<pybind11::detail::type_info*, std::allocator<pybind11::detail::type_info*> > > >, std::__detail::_Select1st, std::equal_to<_typeobject*>, std::hash<_typeobject*>, std::__detail::_Mod_range_hashing, std::__detail::_Default_ranged_hash, std::__detail::_Prime_rehash_policy, std::__detail::_Hashtable_traits<false, false, true> >::_M_bucket_index(unsigned long) const:
 /usr/include/c++/11/bits/hashtable.h:795
 	mov    0x40(%rax),%rdi
@@ -20274,27 +20274,27 @@
 	call   61d0 <_Unwind_Resume@plt>
 pybind11::detail::instance::allocate_layout():
 	cs nopw 0x0(%rax,%rax,1)
 	nop
 
 0000000000011da0 <pybind11_object_new>:
 pybind11_object_new():
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:365
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:365
 	endbr64
 	push   %r12
 pybind11::detail::make_new_instance(_typeobject*):
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:355
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:355
 	xor    %esi,%esi
 	call   *0x130(%rdi)
 	mov    %rax,%r12
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:358
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:358
 	mov    %rax,%rdi
 	call   11970 <pybind11::detail::instance::allocate_layout()>
 pybind11_object_new():
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:367
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:367
 	mov    %r12,%rax
 	pop    %r12
 	ret
 	nop
 
 0000000000011dc0 <pybind11::detail::all_type_info(_typeobject*)>:
 pybind11::detail::all_type_info(_typeobject*):
@@ -20657,30 +20657,30 @@
 	mov    %rbp,%rdi
 	call   61d0 <_Unwind_Resume@plt>
 pybind11::detail::all_type_info(_typeobject*):
 	nopl   0x0(%rax)
 
 00000000000120f0 <pybind11_meta_call>:
 pybind11_meta_call():
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:183
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:183
 	endbr64
 	push   %r15
 	push   %r14
 	push   %r13
 	push   %r12
 	push   %rbp
 	push   %rbx
 	sub    $0x48,%rsp
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:186
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:186
 	mov    %fs:0x28,%rax
 	mov    %rax,0x38(%rsp)
 	mov    0xbdf1(%rip),%rax        
 	call   *0x80(%rax)
 	mov    %rax,0x8(%rsp)
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:187
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:187
 	test   %rax,%rax
 	je     121f5 <pybind11_meta_call+0x105>
 pybind11::detail::values_and_holders::values_and_holders(_object*):
 /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/detail/../detail/type_caster_base.h:340
 	mov    0x8(%rax),%rdi
 	call   11dc0 <pybind11::detail::all_type_info(_typeobject*)>
 __gnu_cxx::__normal_iterator<pybind11::detail::type_info* const*, std::vector<pybind11::detail::type_info*, std::allocator<pybind11::detail::type_info*> > >::__normal_iterator(pybind11::detail::type_info* const* const&):
@@ -25740,28 +25740,28 @@
 	jmp    1501c <pybind11::cpp_function::dispatcher(_object*, _object*, _object*)+0x281c>
 pybind11::cpp_function::dispatcher(_object*, _object*, _object*):
 	cs nopw 0x0(%rax,%rax,1)
 	nopl   (%rax)
 
 00000000000157d0 <pybind11::detail::traverse_offset_bases(void*, pybind11::detail::type_info const*, pybind11::detail::instance*, bool (*)(void*, pybind11::detail::instance*))>:
 pybind11::detail::traverse_offset_bases(void*, pybind11::detail::type_info const*, pybind11::detail::instance*, bool (*)(void*, pybind11::detail::instance*)):
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:295
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:295
 	endbr64
 	push   %r15
 	push   %r14
 	push   %r13
 	push   %r12
 	push   %rbp
 	push   %rbx
 	sub    $0x158,%rsp
 	mov    %rdi,0xb0(%rsp)
 	mov    %rsi,0x78(%rsp)
 	mov    %rdx,0x38(%rsp)
 	mov    %rcx,0x40(%rsp)
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:296
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:296
 	mov    %fs:0x28,%rax
 	mov    %rax,0x148(%rsp)
 	mov    (%rsi),%rax
 	mov    0x150(%rax),%rbp
 pybind11::object::object(pybind11::handle, pybind11::object::borrowed_t):
 /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/detail/../detail/../pytypes.h:441
 	mov    %rbp,0x110(%rsp)
@@ -26484,15 +26484,15 @@
 	mov    %rax,%rbp
 	jmp    15fba <pybind11::detail::traverse_offset_bases(void*, pybind11::detail::type_info const*, pybind11::detail::instance*, bool (*)(void*, pybind11::detail::instance*))+0x7ea>
 pybind11::detail::traverse_offset_bases(void*, pybind11::detail::type_info const*, pybind11::detail::instance*, bool (*)(void*, pybind11::detail::instance*)):
 	nopw   0x0(%rax,%rax,1)
 
 0000000000016030 <pybind11::detail::clear_instance(_object*)>:
 pybind11::detail::clear_instance(_object*):
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:405
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:405
 	endbr64
 	push   %r15
 	push   %r14
 	push   %r13
 	push   %r12
 	mov    %rdi,%r12
 	push   %rbp
@@ -28316,15 +28316,15 @@
 	mov    %rax,%rbp
 	jmp    16f9e <pybind11::detail::clear_instance(_object*)+0xf6e>
 pybind11::detail::clear_instance(_object*):
 	nopl   0x0(%rax,%rax,1)
 
 0000000000016fe0 <pybind11_object_dealloc>:
 pybind11_object_dealloc():
-/home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp:444
+/home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp:444
 	endbr64
 	push   %r12
 	push   %rbp
 	mov    %rdi,%rbp
 	sub    $0x8,%rsp
 /home/linuxbrew/.linuxbrew/opt/python@3.11/include/python3.11/object.h:133
 	mov    0x8(%rdi),%r12
```

#### readelf --wide --decompress --string-dump=.debug_line_str {}

```diff
@@ -1,165 +1,165 @@
 
 String dump of section '.debug_line_str':
-  [     0]  /home/pietro/Desktop/cpp-py/cpp_py/.rendered.somecode.cpp
-  [    3a]  /home/pietro/Desktop/cpp-py
-  [    56]  /home/pietro/Desktop/cpp-py/cpp_py
-  [    79]  /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/detail
-  [    ec]  /home/linuxbrew/.linuxbrew/opt/python@3.11/include/python3.11
-  [   12a]  /usr/include/c++/11/bits
-  [   143]  /usr/include/c++/11/ext
-  [   15b]  /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/detail/../detail
-  [   1d8]  /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/detail/../detail/..
-  [   258]  /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11
-  [   2c4]  /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/detail/..
-  [   33a]  /usr/include/c++/11
-  [   34e]  /home/linuxbrew/.linuxbrew/opt/python@3.11/include/python3.11/cpython
-  [   394]  /usr/include/x86_64-linux-gnu/bits
-  [   3b7]  /usr/include
-  [   3c4]  /usr/lib/gcc/x86_64-linux-gnu/11/include
-  [   3ed]  /usr/include/x86_64-linux-gnu/sys
-  [   40f]  /usr/include/x86_64-linux-gnu/bits/types
-  [   438]  /usr/include/x86_64-linux-gnu/c++/11/bits
-  [   462]  /usr/include/c++/11/debug
-  [   47c]  class.h
-  [   484]  shared_ptr_base.h
-  [   496]  new_allocator.h
-  [   4a6]  allocated_ptr.h
-  [   4b6]  move.h
-  [   4bd]  alloc_traits.h
-  [   4cc]  common.h
-  [   4d5]  pytypes.h
-  [   4df]  shared_ptr.h
-  [   4ec]  atomicity.h
-  [   4f8]  hashtable.h
-  [   504]  hashtable_policy.h
-  [   517]  functional_hash.h
-  [   529]  stl_function.h
-  [   538]  stl_vector.h
-  [   545]  stl_pair.h
-  [   550]  basic_string.h
-  [   55f]  char_traits.h
-  [   56d]  pybind11.h
-  [   578]  attr.h
-  [   57f]  unique_ptr.h
-  [   58c]  tuple
-  [   592]  typeinfo
-  [   59b]  basic_string.tcc
-  [   5ac]  stl_iterator_base_funcs.h
-  [   5c6]  vector.tcc
-  [   5d1]  stl_bvector.h
-  [   5df]  stl_algobase.h
-  [   5ee]  typeindex
-  [   5f8]  stl_iterator.h
-  [   607]  charconv.h
-  [   612]  internals.h
-  [   61e]  typeid.h
-  [   627]  type_caster_base.h
-  [   63a]  cast.h
-  [   641]  forward_list.h
-  [   650]  exception_ptr.h
-  [   660]  stl_construct.h
-  [   670]  stl_uninitialized.h
-  [   684]  unordered_map.h
-  [   694]  unordered_set.h
-  [   6a4]  forward_list.tcc
-  [   6b5]  gil.h
-  [   6bb]  new
-  [   6bf]  tupleobject.h
-  [   6cd]  methodobject.h
-  [   6dc]  string_fortified.h
-  [   6ef]  options.h
-  [   6f9]  array
-  [   6ff]  stddef.h
-  [   708]  stdlib.h
-  [   711]  clock_t.h
-  [   71b]  time_t.h
-  [   724]  stdint-intn.h
-  [   732]  pthreadtypes.h
-  [   741]  cstdlib
-  [   749]  std_abs.h
-  [   753]  cpp_type_traits.h
-  [   765]  cmath
-  [   76b]  cstddef
-  [   773]  cstring
-  [   77b]  type_traits
-  [   787]  c++config.h
-  [   793]  stl_iterator_base_types.h
-  [   7ad]  debug.h
-  [   7b5]  uses_allocator.h
-  [   7c6]  utility
-  [   7ce]  cwchar
-  [   7d5]  cstdint
-  [   7dd]  clocale
-  [   7e5]  cstdio
-  [   7ec]  initializer_list
-  [   7fd]  stringfwd.h
-  [   809]  enable_special_members.h
-  [   822]  nested_exception.h
-  [   835]  std_function.h
-  [   844]  functional
-  [   84f]  refwrap.h
-  [   859]  ctime
-  [   85f]  chrono
-  [   866]  system_error
-  [   873]  std_mutex.h
-  [   87f]  ptr_traits.h
-  [   88c]  stdexcept
-  [   896]  hash_bytes.h
-  [   8a3]  functexcept.h
-  [   8b1]  stdlib-float.h
-  [   8c0]  stdlib-bsearch.h
-  [   8d1]  predefined_ops.h
-  [   8e2]  concurrence.h
-  [   8f0]  aligned_buffer.h
-  [   901]  <built-in>
-  [   90c]  __mbstate_t.h
-  [   91a]  __fpos64_t.h
-  [   927]  __FILE.h
-  [   930]  struct_FILE.h
-  [   93e]  stdio.h
-  [   946]  unistd.h
-  [   94f]  wint_t.h
-  [   958]  stdint-uintn.h
-  [   967]  stdint.h
-  [   970]  pyport.h
-  [   979]  math.h
-  [   980]  struct_tm.h
-  [   98c]  pytypedefs.h
-  [   999]  moduleobject.h
-  [   9a8]  descrobject.h
-  [   9b6]  code.h
-  [   9bd]  pystate.h
-  [   9c7]  pybuffer.h
-  [   9d2]  bytearrayobject.h
-  [   9e4]  floatobject.h
-  [   9f2]  listobject.h
-  [   9ff]  dictobject.h
-  [   a0c]  classobject.h
-  [   a1a]  pycapsule.h
-  [   a26]  traceback.h
-  [   a32]  pyerrors.h
-  [   a3d]  pythread.h
-  [   a48]  wchar.h
-  [   a50]  wchar2.h
-  [   a59]  atomic_word.h
-  [   a67]  single_threaded.h
-  [   a79]  locale.h
-  [   a82]  stdio2.h
-  [   a8b]  descr.h
-  [   a93]  buffer_info.h
-  [   aa1]  typing.h
-  [   aaa]  cxxabi_init_exception.h
-  [   ac2]  cxxabi.h
-  [   acb]  time.h
-  [   ad2]  modsupport.h
-  [   adf]  longobject.h
-  [   aec]  abstract.h
-  [   af7]  pymem.h
-  [   aff]  objimpl.h
-  [   b09]  weakrefobject.h
-  [   b19]  unicodeobject.h
-  [   b29]  ceval.h
-  [   b31]  bytesobject.h
-  [   b3f]  pyframe.h
-  [   b49]  pylifecycle.h
+  [     0]  /home/pietro/Desktop/cpp-py/justatestwithcpp/.rendered.somecode.cpp
+  [    44]  /home/pietro/Desktop/cpp-py
+  [    60]  /home/pietro/Desktop/cpp-py/justatestwithcpp
+  [    8d]  /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/detail
+  [   100]  /home/linuxbrew/.linuxbrew/opt/python@3.11/include/python3.11
+  [   13e]  /usr/include/c++/11/bits
+  [   157]  /usr/include/c++/11/ext
+  [   16f]  /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/detail/../detail
+  [   1ec]  /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/detail/../detail/..
+  [   26c]  /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11
+  [   2d8]  /home/linuxbrew/.linuxbrew/Cellar/python@3.11/3.11.5/lib/python3.11/site-packages/pybind11/include/pybind11/detail/..
+  [   34e]  /usr/include/c++/11
+  [   362]  /home/linuxbrew/.linuxbrew/opt/python@3.11/include/python3.11/cpython
+  [   3a8]  /usr/include/x86_64-linux-gnu/bits
+  [   3cb]  /usr/include
+  [   3d8]  /usr/lib/gcc/x86_64-linux-gnu/11/include
+  [   401]  /usr/include/x86_64-linux-gnu/sys
+  [   423]  /usr/include/x86_64-linux-gnu/bits/types
+  [   44c]  /usr/include/x86_64-linux-gnu/c++/11/bits
+  [   476]  /usr/include/c++/11/debug
+  [   490]  class.h
+  [   498]  shared_ptr_base.h
+  [   4aa]  new_allocator.h
+  [   4ba]  allocated_ptr.h
+  [   4ca]  move.h
+  [   4d1]  alloc_traits.h
+  [   4e0]  common.h
+  [   4e9]  pytypes.h
+  [   4f3]  shared_ptr.h
+  [   500]  atomicity.h
+  [   50c]  hashtable.h
+  [   518]  hashtable_policy.h
+  [   52b]  functional_hash.h
+  [   53d]  stl_function.h
+  [   54c]  stl_vector.h
+  [   559]  stl_pair.h
+  [   564]  basic_string.h
+  [   573]  char_traits.h
+  [   581]  pybind11.h
+  [   58c]  attr.h
+  [   593]  unique_ptr.h
+  [   5a0]  tuple
+  [   5a6]  typeinfo
+  [   5af]  basic_string.tcc
+  [   5c0]  stl_iterator_base_funcs.h
+  [   5da]  vector.tcc
+  [   5e5]  stl_bvector.h
+  [   5f3]  stl_algobase.h
+  [   602]  typeindex
+  [   60c]  stl_iterator.h
+  [   61b]  charconv.h
+  [   626]  internals.h
+  [   632]  typeid.h
+  [   63b]  type_caster_base.h
+  [   64e]  cast.h
+  [   655]  forward_list.h
+  [   664]  exception_ptr.h
+  [   674]  stl_construct.h
+  [   684]  stl_uninitialized.h
+  [   698]  unordered_map.h
+  [   6a8]  unordered_set.h
+  [   6b8]  forward_list.tcc
+  [   6c9]  gil.h
+  [   6cf]  new
+  [   6d3]  tupleobject.h
+  [   6e1]  methodobject.h
+  [   6f0]  string_fortified.h
+  [   703]  options.h
+  [   70d]  array
+  [   713]  stddef.h
+  [   71c]  stdlib.h
+  [   725]  clock_t.h
+  [   72f]  time_t.h
+  [   738]  stdint-intn.h
+  [   746]  pthreadtypes.h
+  [   755]  cstdlib
+  [   75d]  std_abs.h
+  [   767]  cpp_type_traits.h
+  [   779]  cmath
+  [   77f]  cstddef
+  [   787]  cstring
+  [   78f]  type_traits
+  [   79b]  c++config.h
+  [   7a7]  stl_iterator_base_types.h
+  [   7c1]  debug.h
+  [   7c9]  uses_allocator.h
+  [   7da]  utility
+  [   7e2]  cwchar
+  [   7e9]  cstdint
+  [   7f1]  clocale
+  [   7f9]  cstdio
+  [   800]  initializer_list
+  [   811]  stringfwd.h
+  [   81d]  enable_special_members.h
+  [   836]  nested_exception.h
+  [   849]  std_function.h
+  [   858]  functional
+  [   863]  refwrap.h
+  [   86d]  ctime
+  [   873]  chrono
+  [   87a]  system_error
+  [   887]  std_mutex.h
+  [   893]  ptr_traits.h
+  [   8a0]  stdexcept
+  [   8aa]  hash_bytes.h
+  [   8b7]  functexcept.h
+  [   8c5]  stdlib-float.h
+  [   8d4]  stdlib-bsearch.h
+  [   8e5]  predefined_ops.h
+  [   8f6]  concurrence.h
+  [   904]  aligned_buffer.h
+  [   915]  <built-in>
+  [   920]  __mbstate_t.h
+  [   92e]  __fpos64_t.h
+  [   93b]  __FILE.h
+  [   944]  struct_FILE.h
+  [   952]  stdio.h
+  [   95a]  unistd.h
+  [   963]  wint_t.h
+  [   96c]  stdint-uintn.h
+  [   97b]  stdint.h
+  [   984]  pyport.h
+  [   98d]  math.h
+  [   994]  struct_tm.h
+  [   9a0]  pytypedefs.h
+  [   9ad]  moduleobject.h
+  [   9bc]  descrobject.h
+  [   9ca]  code.h
+  [   9d1]  pystate.h
+  [   9db]  pybuffer.h
+  [   9e6]  bytearrayobject.h
+  [   9f8]  floatobject.h
+  [   a06]  listobject.h
+  [   a13]  dictobject.h
+  [   a20]  classobject.h
+  [   a2e]  pycapsule.h
+  [   a3a]  traceback.h
+  [   a46]  pyerrors.h
+  [   a51]  pythread.h
+  [   a5c]  wchar.h
+  [   a64]  wchar2.h
+  [   a6d]  atomic_word.h
+  [   a7b]  single_threaded.h
+  [   a8d]  locale.h
+  [   a96]  stdio2.h
+  [   a9f]  descr.h
+  [   aa7]  buffer_info.h
+  [   ab5]  typing.h
+  [   abe]  cxxabi_init_exception.h
+  [   ad6]  cxxabi.h
+  [   adf]  time.h
+  [   ae6]  modsupport.h
+  [   af3]  longobject.h
+  [   b00]  abstract.h
+  [   b0b]  pymem.h
+  [   b13]  objimpl.h
+  [   b1d]  weakrefobject.h
+  [   b2d]  unicodeobject.h
+  [   b3d]  ceval.h
+  [   b45]  bytesobject.h
+  [   b53]  pyframe.h
+  [   b5d]  pylifecycle.h
```

