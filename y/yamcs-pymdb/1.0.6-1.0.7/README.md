# Comparing `tmp/yamcs_pymdb-1.0.6.tar.gz` & `tmp/yamcs_pymdb-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yamcs_pymdb-1.0.6.tar", last modified: Tue Apr 16 07:57:04 2024, max compression
+gzip compressed data, was "yamcs_pymdb-1.0.7.tar", last modified: Thu May  9 22:32:47 2024, max compression
```

## Comparing `yamcs_pymdb-1.0.6.tar` & `yamcs_pymdb-1.0.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-16 07:57:04.134244 yamcs_pymdb-1.0.6/
--rw-r--r--   0 fdi        (503) staff       (20)     7652 2024-02-09 08:16:29.000000 yamcs_pymdb-1.0.6/LICENSE
--rw-r--r--   0 fdi        (503) staff       (20)       34 2024-02-09 08:18:18.000000 yamcs_pymdb-1.0.6/MANIFEST.in
--rw-r--r--   0 fdi        (503) staff       (20)     1915 2024-04-16 07:57:04.133983 yamcs_pymdb-1.0.6/PKG-INFO
--rw-r--r--   0 fdi        (503) staff       (20)     1007 2024-02-09 09:41:58.000000 yamcs_pymdb-1.0.6/README.md
--rw-r--r--   0 fdi        (503) staff       (20)       38 2024-04-16 07:57:04.134306 yamcs_pymdb-1.0.6/setup.cfg
--rw-r--r--   0 fdi        (503) staff       (20)     1244 2024-04-16 07:47:15.000000 yamcs_pymdb-1.0.6/setup.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-16 07:57:04.105446 yamcs_pymdb-1.0.6/src/
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-16 07:57:04.105254 yamcs_pymdb-1.0.6/src/yamcs/
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-16 07:57:04.115456 yamcs_pymdb-1.0.6/src/yamcs/pymdb/
--rw-r--r--   0 fdi        (503) staff       (20)      687 2024-03-14 22:48:46.000000 yamcs_pymdb-1.0.6/src/yamcs/pymdb/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)     4166 2024-03-22 09:18:23.000000 yamcs_pymdb-1.0.6/src/yamcs/pymdb/alarms.py
--rw-r--r--   0 fdi        (503) staff       (20)     6569 2024-04-05 11:18:43.000000 yamcs_pymdb-1.0.6/src/yamcs/pymdb/algorithms.py
--rw-r--r--   0 fdi        (503) staff       (20)     1173 2024-03-22 09:19:10.000000 yamcs_pymdb-1.0.6/src/yamcs/pymdb/ancillary.py
--rw-r--r--   0 fdi        (503) staff       (20)     1110 2024-02-23 15:50:36.000000 yamcs_pymdb-1.0.6/src/yamcs/pymdb/calibrators.py
--rw-r--r--   0 fdi        (503) staff       (20)     6049 2024-04-15 20:41:06.000000 yamcs_pymdb-1.0.6/src/yamcs/pymdb/ccsds.py
--rw-r--r--   0 fdi        (503) staff       (20)     4561 2024-03-28 20:39:32.000000 yamcs_pymdb-1.0.6/src/yamcs/pymdb/checks.py
--rw-r--r--   0 fdi        (503) staff       (20)    18698 2024-04-15 21:15:24.000000 yamcs_pymdb-1.0.6/src/yamcs/pymdb/commands.py
--rw-r--r--   0 fdi        (503) staff       (20)     7602 2024-04-15 21:22:33.000000 yamcs_pymdb-1.0.6/src/yamcs/pymdb/containers.py
--rw-r--r--   0 fdi        (503) staff       (20)     7999 2024-04-15 21:28:28.000000 yamcs_pymdb-1.0.6/src/yamcs/pymdb/csp.py
--rw-r--r--   0 fdi        (503) staff       (20)    18231 2024-03-28 12:30:59.000000 yamcs_pymdb-1.0.6/src/yamcs/pymdb/datatypes.py
--rw-r--r--   0 fdi        (503) staff       (20)     8370 2024-04-05 09:43:14.000000 yamcs_pymdb-1.0.6/src/yamcs/pymdb/encodings.py
--rw-r--r--   0 fdi        (503) staff       (20)       86 2024-01-04 13:44:01.000000 yamcs_pymdb-1.0.6/src/yamcs/pymdb/exceptions.py
--rw-r--r--   0 fdi        (503) staff       (20)     4045 2024-03-22 07:37:40.000000 yamcs_pymdb-1.0.6/src/yamcs/pymdb/expressions.py
--rw-r--r--   0 fdi        (503) staff       (20)    16520 2024-04-04 12:25:17.000000 yamcs_pymdb-1.0.6/src/yamcs/pymdb/parameters.py
--rw-r--r--   0 fdi        (503) staff       (20)     8350 2024-04-05 09:43:14.000000 yamcs_pymdb-1.0.6/src/yamcs/pymdb/systems.py
--rw-r--r--   0 fdi        (503) staff       (20)     4427 2024-04-05 09:50:48.000000 yamcs_pymdb-1.0.6/src/yamcs/pymdb/verifiers.py
--rw-r--r--   0 fdi        (503) staff       (20)    78883 2024-04-15 21:26:03.000000 yamcs_pymdb-1.0.6/src/yamcs/pymdb/xtce.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-16 07:57:04.133662 yamcs_pymdb-1.0.6/src/yamcs_pymdb.egg-info/
--rw-r--r--   0 fdi        (503) staff       (20)     1915 2024-04-16 07:57:04.000000 yamcs_pymdb-1.0.6/src/yamcs_pymdb.egg-info/PKG-INFO
--rw-r--r--   0 fdi        (503) staff       (20)      737 2024-04-16 07:57:04.000000 yamcs_pymdb-1.0.6/src/yamcs_pymdb.egg-info/SOURCES.txt
--rw-r--r--   0 fdi        (503) staff       (20)        1 2024-04-16 07:57:04.000000 yamcs_pymdb-1.0.6/src/yamcs_pymdb.egg-info/dependency_links.txt
--rw-r--r--   0 fdi        (503) staff       (20)        1 2023-12-13 14:35:06.000000 yamcs_pymdb-1.0.6/src/yamcs_pymdb.egg-info/not-zip-safe
--rw-r--r--   0 fdi        (503) staff       (20)        6 2024-04-16 07:57:04.000000 yamcs_pymdb-1.0.6/src/yamcs_pymdb.egg-info/top_level.txt
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-09 22:32:47.775059 yamcs_pymdb-1.0.7/
+-rw-r--r--   0 fdi        (503) staff       (20)     7652 2024-02-09 08:16:29.000000 yamcs_pymdb-1.0.7/LICENSE
+-rw-r--r--   0 fdi        (503) staff       (20)       34 2024-02-09 08:18:18.000000 yamcs_pymdb-1.0.7/MANIFEST.in
+-rw-r--r--   0 fdi        (503) staff       (20)     1915 2024-05-09 22:32:47.774726 yamcs_pymdb-1.0.7/PKG-INFO
+-rw-r--r--   0 fdi        (503) staff       (20)     1007 2024-02-09 09:41:58.000000 yamcs_pymdb-1.0.7/README.md
+-rw-r--r--   0 fdi        (503) staff       (20)       38 2024-05-09 22:32:47.775112 yamcs_pymdb-1.0.7/setup.cfg
+-rw-r--r--   0 fdi        (503) staff       (20)     1244 2024-05-09 22:25:02.000000 yamcs_pymdb-1.0.7/setup.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-09 22:32:47.744379 yamcs_pymdb-1.0.7/src/
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-09 22:32:47.744051 yamcs_pymdb-1.0.7/src/yamcs/
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-09 22:32:47.771254 yamcs_pymdb-1.0.7/src/yamcs/pymdb/
+-rw-r--r--   0 fdi        (503) staff       (20)      687 2024-03-14 22:48:46.000000 yamcs_pymdb-1.0.7/src/yamcs/pymdb/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)     4166 2024-03-22 09:18:23.000000 yamcs_pymdb-1.0.7/src/yamcs/pymdb/alarms.py
+-rw-r--r--   0 fdi        (503) staff       (20)     6569 2024-04-05 11:18:43.000000 yamcs_pymdb-1.0.7/src/yamcs/pymdb/algorithms.py
+-rw-r--r--   0 fdi        (503) staff       (20)     1173 2024-03-22 09:19:10.000000 yamcs_pymdb-1.0.7/src/yamcs/pymdb/ancillary.py
+-rw-r--r--   0 fdi        (503) staff       (20)     1110 2024-02-23 15:50:36.000000 yamcs_pymdb-1.0.7/src/yamcs/pymdb/calibrators.py
+-rw-r--r--   0 fdi        (503) staff       (20)     6049 2024-04-15 20:41:06.000000 yamcs_pymdb-1.0.7/src/yamcs/pymdb/ccsds.py
+-rw-r--r--   0 fdi        (503) staff       (20)     4561 2024-03-28 20:39:32.000000 yamcs_pymdb-1.0.7/src/yamcs/pymdb/checks.py
+-rw-r--r--   0 fdi        (503) staff       (20)    19695 2024-05-09 20:11:31.000000 yamcs_pymdb-1.0.7/src/yamcs/pymdb/commands.py
+-rw-r--r--   0 fdi        (503) staff       (20)     7716 2024-05-09 21:10:10.000000 yamcs_pymdb-1.0.7/src/yamcs/pymdb/containers.py
+-rw-r--r--   0 fdi        (503) staff       (20)     7999 2024-04-15 21:28:28.000000 yamcs_pymdb-1.0.7/src/yamcs/pymdb/csp.py
+-rw-r--r--   0 fdi        (503) staff       (20)    18235 2024-05-09 19:15:26.000000 yamcs_pymdb-1.0.7/src/yamcs/pymdb/datatypes.py
+-rw-r--r--   0 fdi        (503) staff       (20)     8370 2024-04-05 09:43:14.000000 yamcs_pymdb-1.0.7/src/yamcs/pymdb/encodings.py
+-rw-r--r--   0 fdi        (503) staff       (20)       86 2024-01-04 13:44:01.000000 yamcs_pymdb-1.0.7/src/yamcs/pymdb/exceptions.py
+-rw-r--r--   0 fdi        (503) staff       (20)     4045 2024-03-22 07:37:40.000000 yamcs_pymdb-1.0.7/src/yamcs/pymdb/expressions.py
+-rw-r--r--   0 fdi        (503) staff       (20)    16520 2024-04-04 12:25:17.000000 yamcs_pymdb-1.0.7/src/yamcs/pymdb/parameters.py
+-rw-r--r--   0 fdi        (503) staff       (20)     8350 2024-04-05 09:43:14.000000 yamcs_pymdb-1.0.7/src/yamcs/pymdb/systems.py
+-rw-r--r--   0 fdi        (503) staff       (20)     4427 2024-04-05 09:50:48.000000 yamcs_pymdb-1.0.7/src/yamcs/pymdb/verifiers.py
+-rw-r--r--   0 fdi        (503) staff       (20)    80080 2024-05-09 22:25:02.000000 yamcs_pymdb-1.0.7/src/yamcs/pymdb/xtce.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-09 22:32:47.774323 yamcs_pymdb-1.0.7/src/yamcs_pymdb.egg-info/
+-rw-r--r--   0 fdi        (503) staff       (20)     1915 2024-05-09 22:32:47.000000 yamcs_pymdb-1.0.7/src/yamcs_pymdb.egg-info/PKG-INFO
+-rw-r--r--   0 fdi        (503) staff       (20)      737 2024-05-09 22:32:47.000000 yamcs_pymdb-1.0.7/src/yamcs_pymdb.egg-info/SOURCES.txt
+-rw-r--r--   0 fdi        (503) staff       (20)        1 2024-05-09 22:32:47.000000 yamcs_pymdb-1.0.7/src/yamcs_pymdb.egg-info/dependency_links.txt
+-rw-r--r--   0 fdi        (503) staff       (20)        1 2023-12-13 14:35:06.000000 yamcs_pymdb-1.0.7/src/yamcs_pymdb.egg-info/not-zip-safe
+-rw-r--r--   0 fdi        (503) staff       (20)        6 2024-05-09 22:32:47.000000 yamcs_pymdb-1.0.7/src/yamcs_pymdb.egg-info/top_level.txt
```

### Comparing `yamcs_pymdb-1.0.6/LICENSE` & `yamcs_pymdb-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `yamcs_pymdb-1.0.6/PKG-INFO` & `yamcs_pymdb-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamcs-pymdb
-Version: 1.0.6
+Version: 1.0.7
 Summary: Generate XTCE for use with Yamcs
 Home-page: https://github.com/yamcs/pymdb
 Author: Space Applications Services
 Author-email: yamcs@spaceapplications.com
 License: LGPL
 Keywords: packet telemetry ccsds xtce yamcs
 Platform: Posix; MacOS X; Windows
```

### Comparing `yamcs_pymdb-1.0.6/README.md` & `yamcs_pymdb-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `yamcs_pymdb-1.0.6/setup.py` & `yamcs_pymdb-1.0.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with io.open("README.md", encoding="utf-8") as f:
     readme = f.read()
 
 setuptools.setup(
     name="yamcs-pymdb",
-    version="1.0.6",
+    version="1.0.7",
     description="Generate XTCE for use with Yamcs",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/yamcs/pymdb",
     author="Space Applications Services",
     author_email="yamcs@spaceapplications.com",
     license="LGPL",
```

### Comparing `yamcs_pymdb-1.0.6/src/yamcs/pymdb/__init__.py` & `yamcs_pymdb-1.0.7/src/yamcs/pymdb/__init__.py`

 * *Files identical despite different names*

### Comparing `yamcs_pymdb-1.0.6/src/yamcs/pymdb/alarms.py` & `yamcs_pymdb-1.0.7/src/yamcs/pymdb/alarms.py`

 * *Files identical despite different names*

### Comparing `yamcs_pymdb-1.0.6/src/yamcs/pymdb/algorithms.py` & `yamcs_pymdb-1.0.7/src/yamcs/pymdb/algorithms.py`

 * *Files identical despite different names*

### Comparing `yamcs_pymdb-1.0.6/src/yamcs/pymdb/ancillary.py` & `yamcs_pymdb-1.0.7/src/yamcs/pymdb/ancillary.py`

 * *Files identical despite different names*

### Comparing `yamcs_pymdb-1.0.6/src/yamcs/pymdb/calibrators.py` & `yamcs_pymdb-1.0.7/src/yamcs/pymdb/calibrators.py`

 * *Files identical despite different names*

### Comparing `yamcs_pymdb-1.0.6/src/yamcs/pymdb/ccsds.py` & `yamcs_pymdb-1.0.7/src/yamcs/pymdb/ccsds.py`

 * *Files identical despite different names*

### Comparing `yamcs_pymdb-1.0.6/src/yamcs/pymdb/checks.py` & `yamcs_pymdb-1.0.7/src/yamcs/pymdb/checks.py`

 * *Files identical despite different names*

### Comparing `yamcs_pymdb-1.0.6/src/yamcs/pymdb/commands.py` & `yamcs_pymdb-1.0.7/src/yamcs/pymdb/commands.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from collections.abc import Mapping, Sequence
 from enum import Enum, auto
-from typing import TYPE_CHECKING, Any, Literal
+from typing import TYPE_CHECKING, Any, Literal, Union
 
 from yamcs.pymdb.containers import ParameterEntry
 from yamcs.pymdb.datatypes import (
     AbsoluteTimeDataType,
     AggregateDataType,
     ArrayDataType,
     BinaryDataType,
@@ -490,14 +490,23 @@
         the most-significant bits are dropped.
         """
 
 
 CommandEntry = ArgumentEntry | ParameterEntry | FixedValueEntry
 
 
+class TransmissionConstraint:
+    def __init__(self, expression: Expression, *, timeout: float = 0):
+        self.expression: Expression = expression
+        """Expression that must be satisfied"""
+
+        self.timeout: float = timeout
+        """How long to wait for the constraint to be satisfied (in seconds)"""
+
+
 class Command:
     def __init__(
         self,
         system: System,
         name: str,
         *,
         aliases: Mapping[str, str] | None = None,
@@ -507,14 +516,17 @@
         abstract: bool = False,
         base: Command | str | None = None,
         assignments: Mapping[str, Any] | None = None,
         arguments: Sequence[Argument] | None = None,
         entries: Sequence[CommandEntry] | None = None,
         level: CommandLevel = CommandLevel.NORMAL,
         warning_message: str | None = None,
+        constraint: (
+            Union[TransmissionConstraint, Sequence[TransmissionConstraint]] | None
+        ) = None,
     ):
         self.name: str = name
         """Short name of this command"""
 
         self.system: System = system
         """System this command belongs to"""
 
@@ -530,14 +542,29 @@
         self.extra: dict[str, str] = dict(extra or {})
         """Arbitrary information, keyed by name"""
 
         self.abstract: bool = abstract
         self.base: Command | str | None = base
         self.assignments: dict[str, Any] = dict(assignments or {})
         self.arguments: list[Argument] = list(arguments or [])
+
+        constraints: list[TransmissionConstraint] = []
+        if isinstance(constraint, Sequence):
+            constraints = list(constraint)
+        elif isinstance(constraint, TransmissionConstraint):
+            constraints.append(constraint)
+        self.constraints = constraints
+        """
+        Constraints to check before sending the command.
+
+        A command is sent only when all constraints are satisfied. Constraints
+        are evaluated in order. Afterwards, also constraints from :attr:`base`
+        are checked.
+        """
+
         self._entries: list[CommandEntry] | None = (
             list(entries) if entries is not None else None
         )
 
         self.transferred_to_range_verifier: TransferredToRangeVerifier | None = None
         self.sent_from_range_verifier: SentFromRangeVerifier | None = None
         self.received_verifier: ReceivedVerifier | None = None
```

### Comparing `yamcs_pymdb-1.0.6/src/yamcs/pymdb/containers.py` & `yamcs_pymdb-1.0.7/src/yamcs/pymdb/containers.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,14 +142,17 @@
         included.
         """
 
         self.rate: float | None = rate
         """
         Expected rate in seconds.
 
+        For example, a rate of ``2`` means: "one update every 2 seconds" (not
+        "2 updates every second").
+
         This is used by Yamcs to determine parameter expiration. A parameter's
         realtime value is considered expired when ``1.9 * rate`` has passed
         without a new update (where ``1.9`` is a configurable tolerance multiplier).
 
         If ``None``, the contained parameters are not checked for expiration.
         """
```

### Comparing `yamcs_pymdb-1.0.6/src/yamcs/pymdb/csp.py` & `yamcs_pymdb-1.0.7/src/yamcs/pymdb/csp.py`

 * *Files identical despite different names*

### Comparing `yamcs_pymdb-1.0.6/src/yamcs/pymdb/datatypes.py` & `yamcs_pymdb-1.0.7/src/yamcs/pymdb/datatypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,15 @@
             units=units,
             encoding=encoding,
         )
 
         self.choices: Choices = choices
 
     def label_for(self, value: int):
-        if isinstance(self.choices, list):
+        if isinstance(self.choices, Sequence):
             for choice in self.choices:
                 if choice[0] == value:
                     return choice[1]
         else:
             for choice in self.choices:
                 if choice.value == value:
                     return choice.name
```

### Comparing `yamcs_pymdb-1.0.6/src/yamcs/pymdb/encodings.py` & `yamcs_pymdb-1.0.7/src/yamcs/pymdb/encodings.py`

 * *Files identical despite different names*

### Comparing `yamcs_pymdb-1.0.6/src/yamcs/pymdb/expressions.py` & `yamcs_pymdb-1.0.7/src/yamcs/pymdb/expressions.py`

 * *Files identical despite different names*

### Comparing `yamcs_pymdb-1.0.6/src/yamcs/pymdb/parameters.py` & `yamcs_pymdb-1.0.7/src/yamcs/pymdb/parameters.py`

 * *Files identical despite different names*

### Comparing `yamcs_pymdb-1.0.6/src/yamcs/pymdb/systems.py` & `yamcs_pymdb-1.0.7/src/yamcs/pymdb/systems.py`

 * *Files identical despite different names*

### Comparing `yamcs_pymdb-1.0.6/src/yamcs/pymdb/verifiers.py` & `yamcs_pymdb-1.0.7/src/yamcs/pymdb/verifiers.py`

 * *Files identical despite different names*

### Comparing `yamcs_pymdb-1.0.6/src/yamcs/pymdb/xtce.py` & `yamcs_pymdb-1.0.7/src/yamcs/pymdb/xtce.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,14 +235,28 @@
 
             for argument in command.arguments:
                 self.add_argument(args_el, command, argument)
 
         container_el = ET.SubElement(el, "CommandContainer")
         container_el.attrib["name"] = command.name
 
+        if command.constraints:
+            constraints_el = ET.SubElement(el, "TransmissionConstraintList")
+
+            for constraint in command.constraints:
+                constraint_el = ET.SubElement(constraints_el, "TransmissionConstraint")
+                constraint_el.attrib["timeOut"] = _to_isoduration(constraint.timeout)
+
+                expr_el = ET.SubElement(constraint_el, "BooleanExpression")
+                self.add_expression_condition(
+                    expr_el,
+                    system=command.system,
+                    expression=constraint.expression,
+                )
+
         self.add_command_entry_list(container_el, command)
 
         if command.base:
             base_el = ET.SubElement(container_el, "BaseContainer")
             base_el.attrib["containerRef"] = self.make_command_ref(
                 target=command.base,
                 start=command.system,
@@ -858,14 +872,24 @@
             # Always make a new type
             member_type_name = f"{name}__{member.name}"
 
             member_el = ET.SubElement(members_el, "Member")
             member_el.attrib["name"] = str(member.name)
             member_el.attrib["typeRef"] = member_type_name
 
+            if member.short_description:
+                member_el.attrib["shortDescription"] = member.short_description
+
+            if member.long_description:
+                ET.SubElement(member_el, "LongDescription").text = (
+                    member.long_description
+                )
+            if member.extra:
+                self.add_ancillary_data(member_el, member.extra)
+
             if isinstance(member, AbsoluteTimeMember):
                 self.add_absolute_time_parameter_type(
                     parent,
                     system,
                     name=member_type_name,
                     data_type=member,
                 )
@@ -1768,15 +1792,18 @@
             extra["Yamcs"] = "UseAsArchivingPartition"
 
         if extra:
             self.add_ancillary_data(el, extra)
 
         if container.rate is not None:
             rate_el = ET.SubElement(el, "DefaultRateInStream")
-            rate_el.attrib["maximumValue"] = _to_xml_value(container.rate)
+            # In XTCE this is expressed as 'x containers per second',
+            # whereas both Yamcs and PyMDB, employ '1 container every x seconds'
+            rate_el.attrib["minimumValue"] = _to_xml_value(1 / container.rate)
+            rate_el.attrib["basis"] = "perSecond"
 
         if container.bits is not None:
             encoding_el = ET.SubElement(el, "BinaryEncoding")
             size_el = ET.SubElement(encoding_el, "SizeInBits")
             fv_el = ET.SubElement(size_el, "FixedValue")
             fv_el.text = str(container.bits)
```

### Comparing `yamcs_pymdb-1.0.6/src/yamcs_pymdb.egg-info/PKG-INFO` & `yamcs_pymdb-1.0.7/src/yamcs_pymdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamcs-pymdb
-Version: 1.0.6
+Version: 1.0.7
 Summary: Generate XTCE for use with Yamcs
 Home-page: https://github.com/yamcs/pymdb
 Author: Space Applications Services
 Author-email: yamcs@spaceapplications.com
 License: LGPL
 Keywords: packet telemetry ccsds xtce yamcs
 Platform: Posix; MacOS X; Windows
```

### Comparing `yamcs_pymdb-1.0.6/src/yamcs_pymdb.egg-info/SOURCES.txt` & `yamcs_pymdb-1.0.7/src/yamcs_pymdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

