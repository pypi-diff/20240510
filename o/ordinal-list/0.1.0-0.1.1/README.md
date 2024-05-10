# Comparing `tmp/ordinal_list-0.1.0-py3-none-any.whl.zip` & `tmp/ordinal_list-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 4570 bytes, number of entries: 6
--rw-r--r--  2.0 unx     2633 b- defN 24-May-09 18:38 ordinal_list/__init__.py
--rw-r--r--  2.0 unx     1082 b- defN 24-May-09 18:39 ordinal_list-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3789 b- defN 24-May-09 18:39 ordinal_list-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-09 18:39 ordinal_list-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 24-May-09 18:39 ordinal_list-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      492 b- defN 24-May-09 18:39 ordinal_list-0.1.0.dist-info/RECORD
-6 files, 8101 bytes uncompressed, 3676 bytes compressed:  54.6%
+Zip file size: 4569 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     2633 b- defN 24-May-09 18:47 ordinal_list/__init__.py
+-rw-r--r--  2.0 unx     1082 b- defN 24-May-09 18:47 ordinal_list-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3803 b- defN 24-May-09 18:47 ordinal_list-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-09 18:47 ordinal_list-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-May-09 18:47 ordinal_list-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      492 b- defN 24-May-09 18:47 ordinal_list-0.1.1.dist-info/RECORD
+6 files, 8115 bytes uncompressed, 3675 bytes compressed:  54.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: ordinal_list/__init__.py
 Comment: 
 
-Filename: ordinal_list-0.1.0.dist-info/LICENSE
+Filename: ordinal_list-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: ordinal_list-0.1.0.dist-info/METADATA
+Filename: ordinal_list-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: ordinal_list-0.1.0.dist-info/WHEEL
+Filename: ordinal_list-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: ordinal_list-0.1.0.dist-info/top_level.txt
+Filename: ordinal_list-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: ordinal_list-0.1.0.dist-info/RECORD
+Filename: ordinal_list-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ordinal_list-0.1.0.dist-info/LICENSE` & `ordinal_list-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ordinal_list-0.1.0.dist-info/METADATA` & `ordinal_list-0.1.1.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ordinal-list
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python library that uses ordinal numbers to work with lists.
 Author: Jimmy Jensen
 License: The MIT License (MIT)
         
         Copyright (c) [2024] [Jimmy Jensen]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -58,53 +58,53 @@
 This will download and install the latest version of Ordinal List from the Python Package Index (PyPI). After installation, you can import and use the library in your Python projects.
 
 ## Examples
 
 Here's how to get started with the Ordinal List library:
 
 ```python
->> from ordinal_list import OrdinalList
+>>> from ordinal_list import OrdinalList
 ```
 
 Create an OrdinalList with some fruits
 ```python
->> ordinal_list = OrdinalList(['apple', 'banana', 'cherry'])
+>>> ordinal_list = OrdinalList(["apple", "banana", "cherry"])
 ```
 Access elements using ordinal indices
 
 ```python
->> print(ordinal_list['1st'])
+>>> print(ordinal_list["1st"])
 apple
->> print(ordinal_list['2nd'])
+>>> print(ordinal_list["2nd"])
 banana
->> print(ordinal_list['3rd'])
+>>> print(ordinal_list["3rd"])
 cherry
->> print(ordinal_list['-1st'])
+>>> print(ordinal_list["-1st"])
 cherry
 ```
 
 Negative ordinals are also supported, as shown in the example above.
 
 If you try to access an element with an invalid ordinal, the library will raise a descriptive error:
 ```python
->> try:
->>    print(ordinal_list['0th']) # Invalid ordinal, will raise an error
->> except Exception as e:
->>    print(e)
+>>> try:
+>>>    print(ordinal_list["0th"]) # Invalid ordinal, will raise an error
+>>> except Exception as e:
+>>>    print(e)
 ```
 
 
 You can also set items using ordinal indices:
 
 ```python
->> ordinal_list['1st'] = 'strawberry'
->> print(ordinal_list['1st'])
+>>> ordinal_list["1st"] = "strawberry"
+>>> print(ordinal_list["1st"])
 strawberry
 ```
 
 And you can extend the list with more items:
 
 ```python
->> ordinal_list.extend(['kiwi', 'mango'])
->> print(ordinal_list['5th'])
+>>> ordinal_list.extend(["kiwi", "mango"])
+>>> print(ordinal_list["5th"])
 mango
 ```
```

