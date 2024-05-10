# Comparing `tmp/sqlfactory-1.2.1.tar.gz` & `tmp/sqlfactory-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlfactory-1.2.1.tar", max compression
+gzip compressed data, was "sqlfactory-1.3.0.tar", max compression
```

## Comparing `sqlfactory-1.2.1.tar` & `sqlfactory-1.3.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1069 2024-05-09 12:56:55.085194 sqlfactory-1.2.1/LICENSE
--rw-r--r--   0        0        0     7889 2024-05-09 12:56:55.085194 sqlfactory-1.2.1/README.md
--rw-r--r--   0        0        0     1293 2024-05-09 12:56:55.721186 sqlfactory-1.2.1/pyproject.toml
--rw-r--r--   0        0        0      303 2024-05-09 12:56:55.085194 sqlfactory-1.2.1/sqlfactory/__init__.py
--rw-r--r--   0        0        0      324 2024-05-09 12:56:55.085194 sqlfactory-1.2.1/sqlfactory/condition/__init__.py
--rw-r--r--   0        0        0     5049 2024-05-09 12:56:55.085194 sqlfactory-1.2.1/sqlfactory/condition/base.py
--rw-r--r--   0        0        0     1787 2024-05-09 12:56:55.085194 sqlfactory-1.2.1/sqlfactory/condition/between.py
--rw-r--r--   0        0        0     4920 2024-05-09 12:56:55.085194 sqlfactory-1.2.1/sqlfactory/condition/in_condition.py
--rw-r--r--   0        0        0     1274 2024-05-09 12:56:55.085194 sqlfactory-1.2.1/sqlfactory/condition/like.py
--rw-r--r--   0        0        0     5510 2024-05-09 12:56:55.085194 sqlfactory-1.2.1/sqlfactory/condition/simple.py
--rw-r--r--   0        0        0       68 2024-05-09 12:56:55.085194 sqlfactory-1.2.1/sqlfactory/delete/__init__.py
--rw-r--r--   0        0        0     1951 2024-05-09 12:56:55.085194 sqlfactory-1.2.1/sqlfactory/delete/delete.py
--rw-r--r--   0        0        0     7691 2024-05-09 12:56:55.085194 sqlfactory-1.2.1/sqlfactory/entities.py
--rw-r--r--   0        0        0     7543 2024-05-09 12:56:55.085194 sqlfactory-1.2.1/sqlfactory/execute.py
--rw-r--r--   0        0        0        0 2024-05-09 12:56:55.117194 sqlfactory-1.2.1/sqlfactory/func/__init__.py
--rw-r--r--   0        0        0     2578 2024-05-09 12:56:55.085194 sqlfactory-1.2.1/sqlfactory/func/agg.py
--rw-r--r--   0        0        0      987 2024-05-09 12:56:55.085194 sqlfactory-1.2.1/sqlfactory/func/base.py
--rw-r--r--   0        0        0      979 2024-05-09 12:56:55.085194 sqlfactory-1.2.1/sqlfactory/func/control.py
--rw-r--r--   0        0        0    15497 2024-05-09 12:56:55.085194 sqlfactory-1.2.1/sqlfactory/func/datetime.py
--rw-r--r--   0        0        0     4359 2024-05-09 12:56:55.085194 sqlfactory-1.2.1/sqlfactory/func/enc.py
--rw-r--r--   0        0        0     4726 2024-05-09 12:56:55.085194 sqlfactory-1.2.1/sqlfactory/func/info.py
--rw-r--r--   0        0        0     4601 2024-05-09 12:56:55.089194 sqlfactory-1.2.1/sqlfactory/func/misc.py
--rw-r--r--   0        0        0     7156 2024-05-09 12:56:55.089194 sqlfactory-1.2.1/sqlfactory/func/numeric.py
--rw-r--r--   0        0        0     7741 2024-05-09 12:56:55.089194 sqlfactory-1.2.1/sqlfactory/func/str.py
--rw-r--r--   0        0        0       95 2024-05-09 12:56:55.089194 sqlfactory-1.2.1/sqlfactory/insert/__init__.py
--rw-r--r--   0        0        0     6828 2024-05-09 12:56:55.089194 sqlfactory-1.2.1/sqlfactory/insert/insert.py
--rw-r--r--   0        0        0      601 2024-05-09 12:56:55.089194 sqlfactory-1.2.1/sqlfactory/insert/values.py
--rw-r--r--   0        0        0      115 2024-05-09 12:56:55.089194 sqlfactory-1.2.1/sqlfactory/logger.py
--rw-r--r--   0        0        0      271 2024-05-09 12:56:55.089194 sqlfactory-1.2.1/sqlfactory/mixins/__init__.py
--rw-r--r--   0        0        0     3822 2024-05-09 12:56:55.089194 sqlfactory-1.2.1/sqlfactory/mixins/limit.py
--rw-r--r--   0        0        0     2498 2024-05-09 12:56:55.089194 sqlfactory-1.2.1/sqlfactory/mixins/order.py
--rw-r--r--   0        0        0      824 2024-05-09 12:56:55.089194 sqlfactory-1.2.1/sqlfactory/mixins/where.py
--rw-r--r--   0        0        0      244 2024-05-09 12:56:55.089194 sqlfactory-1.2.1/sqlfactory/select/__init__.py
--rw-r--r--   0        0        0     1200 2024-05-09 12:56:55.089194 sqlfactory-1.2.1/sqlfactory/select/aliased.py
--rw-r--r--   0        0        0     2115 2024-05-09 12:56:55.089194 sqlfactory-1.2.1/sqlfactory/select/column_list.py
--rw-r--r--   0        0        0     1846 2024-05-09 12:56:55.089194 sqlfactory-1.2.1/sqlfactory/select/join.py
--rw-r--r--   0        0        0     7502 2024-05-09 12:56:55.089194 sqlfactory-1.2.1/sqlfactory/select/select.py
--rw-r--r--   0        0        0     3861 2024-05-09 12:56:55.089194 sqlfactory-1.2.1/sqlfactory/statement.py
--rw-r--r--   0        0        0       68 2024-05-09 12:56:55.089194 sqlfactory-1.2.1/sqlfactory/update/__init__.py
--rw-r--r--   0        0        0     4867 2024-05-09 12:56:55.089194 sqlfactory-1.2.1/sqlfactory/update/update.py
--rw-r--r--   0        0        0     9002 1970-01-01 00:00:00.000000 sqlfactory-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-10 16:55:58.438267 sqlfactory-1.3.0/LICENSE
+-rw-r--r--   0        0        0     7889 2024-05-10 16:55:58.438267 sqlfactory-1.3.0/README.md
+-rw-r--r--   0        0        0     1293 2024-05-10 16:55:59.034259 sqlfactory-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      284 2024-05-10 16:55:58.438267 sqlfactory-1.3.0/sqlfactory/__init__.py
+-rw-r--r--   0        0        0      324 2024-05-10 16:55:58.438267 sqlfactory-1.3.0/sqlfactory/condition/__init__.py
+-rw-r--r--   0        0        0     5023 2024-05-10 16:55:58.438267 sqlfactory-1.3.0/sqlfactory/condition/base.py
+-rw-r--r--   0        0        0     1744 2024-05-10 16:55:58.438267 sqlfactory-1.3.0/sqlfactory/condition/between.py
+-rw-r--r--   0        0        0     4972 2024-05-10 16:55:58.438267 sqlfactory-1.3.0/sqlfactory/condition/in_condition.py
+-rw-r--r--   0        0        0     1239 2024-05-10 16:55:58.438267 sqlfactory-1.3.0/sqlfactory/condition/like.py
+-rw-r--r--   0        0        0     5475 2024-05-10 16:55:58.438267 sqlfactory-1.3.0/sqlfactory/condition/simple.py
+-rw-r--r--   0        0        0       68 2024-05-10 16:55:58.438267 sqlfactory-1.3.0/sqlfactory/delete/__init__.py
+-rw-r--r--   0        0        0     1935 2024-05-10 16:55:58.438267 sqlfactory-1.3.0/sqlfactory/delete/delete.py
+-rw-r--r--   0        0        0     8296 2024-05-10 16:55:58.438267 sqlfactory-1.3.0/sqlfactory/entities.py
+-rw-r--r--   0        0        0     6539 2024-05-10 16:55:58.438267 sqlfactory-1.3.0/sqlfactory/execute.py
+-rw-r--r--   0        0        0        0 2024-05-10 16:55:58.466267 sqlfactory-1.3.0/sqlfactory/func/__init__.py
+-rw-r--r--   0        0        0     2562 2024-05-10 16:55:58.438267 sqlfactory-1.3.0/sqlfactory/func/agg.py
+-rw-r--r--   0        0        0      987 2024-05-10 16:55:58.438267 sqlfactory-1.3.0/sqlfactory/func/base.py
+-rw-r--r--   0        0        0      979 2024-05-10 16:55:58.438267 sqlfactory-1.3.0/sqlfactory/func/control.py
+-rw-r--r--   0        0        0    15454 2024-05-10 16:55:58.438267 sqlfactory-1.3.0/sqlfactory/func/datetime.py
+-rw-r--r--   0        0        0     4359 2024-05-10 16:55:58.438267 sqlfactory-1.3.0/sqlfactory/func/enc.py
+-rw-r--r--   0        0        0     4699 2024-05-10 16:55:58.438267 sqlfactory-1.3.0/sqlfactory/func/info.py
+-rw-r--r--   0        0        0     4601 2024-05-10 16:55:58.438267 sqlfactory-1.3.0/sqlfactory/func/misc.py
+-rw-r--r--   0        0        0     7156 2024-05-10 16:55:58.438267 sqlfactory-1.3.0/sqlfactory/func/numeric.py
+-rw-r--r--   0        0        0     7741 2024-05-10 16:55:58.438267 sqlfactory-1.3.0/sqlfactory/func/str.py
+-rw-r--r--   0        0        0       95 2024-05-10 16:55:58.438267 sqlfactory-1.3.0/sqlfactory/insert/__init__.py
+-rw-r--r--   0        0        0     6735 2024-05-10 16:55:58.438267 sqlfactory-1.3.0/sqlfactory/insert/insert.py
+-rw-r--r--   0        0        0      601 2024-05-10 16:55:58.438267 sqlfactory-1.3.0/sqlfactory/insert/values.py
+-rw-r--r--   0        0        0      115 2024-05-10 16:55:58.438267 sqlfactory-1.3.0/sqlfactory/logger.py
+-rw-r--r--   0        0        0      271 2024-05-10 16:55:58.438267 sqlfactory-1.3.0/sqlfactory/mixins/__init__.py
+-rw-r--r--   0        0        0     3806 2024-05-10 16:55:58.438267 sqlfactory-1.3.0/sqlfactory/mixins/limit.py
+-rw-r--r--   0        0        0     2464 2024-05-10 16:55:58.438267 sqlfactory-1.3.0/sqlfactory/mixins/order.py
+-rw-r--r--   0        0        0      824 2024-05-10 16:55:58.438267 sqlfactory-1.3.0/sqlfactory/mixins/where.py
+-rw-r--r--   0        0        0      244 2024-05-10 16:55:58.438267 sqlfactory-1.3.0/sqlfactory/select/__init__.py
+-rw-r--r--   0        0        0     1115 2024-05-10 16:55:58.438267 sqlfactory-1.3.0/sqlfactory/select/aliased.py
+-rw-r--r--   0        0        0     2107 2024-05-10 16:55:58.438267 sqlfactory-1.3.0/sqlfactory/select/column_list.py
+-rw-r--r--   0        0        0     1830 2024-05-10 16:55:58.438267 sqlfactory-1.3.0/sqlfactory/select/join.py
+-rw-r--r--   0        0        0     7459 2024-05-10 16:55:58.438267 sqlfactory-1.3.0/sqlfactory/select/select.py
+-rw-r--r--   0        0        0     2644 2024-05-10 16:55:58.438267 sqlfactory-1.3.0/sqlfactory/statement.py
+-rw-r--r--   0        0        0       68 2024-05-10 16:55:58.438267 sqlfactory-1.3.0/sqlfactory/update/__init__.py
+-rw-r--r--   0        0        0     4700 2024-05-10 16:55:58.438267 sqlfactory-1.3.0/sqlfactory/update/update.py
+-rw-r--r--   0        0        0     9002 1970-01-01 00:00:00.000000 sqlfactory-1.3.0/PKG-INFO
```

### Comparing `sqlfactory-1.2.1/LICENSE` & `sqlfactory-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.2.1/README.md` & `sqlfactory-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.2.1/pyproject.toml` & `sqlfactory-1.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sqlfactory"
-version = "v1.2.1"
+version = "v1.3.0"
 description = "Convenient classes for building SQL queries in Python. Main purpose of this library is to ease construction of SQL queries in Python code. It is not an ORM (and don't intend to be), just a plain SQL query builder with syntax as similar to actual SQL as possible."
 authors = ["Michal Kuchta <niximor@gmail.com>"]
 readme = "README.md"
 packages = [{include = "sqlfactory"}]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Development Status :: 5 - Production/Stable",
```

### Comparing `sqlfactory-1.2.1/sqlfactory/condition/base.py` & `sqlfactory-1.3.0/sqlfactory/condition/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 
 from __future__ import annotations
 
 from abc import ABC
 from collections.abc import Iterable
 from typing import Any
 
-from ..statement import StatementWithArgs, ConditionalStatement, Statement
+from ..statement import ConditionalStatement, Statement
+
 StatementOrColumn = str | Statement
 
 
-class ConditionBase(StatementWithArgs, ConditionalStatement, ABC):
+class ConditionBase(Statement, ConditionalStatement, ABC):
     """
     Generic condition interface, that can be chained with other conditions using & or | operators. All condition
     classes should inherit from this one, as there are checks through the library for instances of this class.
     """
     def __and__(self, other: ConditionBase) -> And:
         if isinstance(self, And):
             out = self
```

### Comparing `sqlfactory-1.2.1/sqlfactory/condition/between.py` & `sqlfactory-1.3.0/sqlfactory/condition/between.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """BETWEEN condition generator"""
 
 from typing import Any
 
 from .base import Condition, StatementOrColumn
 from ..entities import Column
-from ..statement import Statement, StatementWithArgs
+from ..statement import Statement
 
 
 # pylint: disable=too-few-public-methods  # As everything is handled by base classes.
 class Between(Condition):
     # pylint: disable=duplicate-code  # It does not make sense to generalize two-row statement used on two places.
     """
     Provides generation for following syntax:
@@ -27,27 +27,27 @@
         upper_bound_s = "%s"
 
         if not isinstance(column, Statement):
             column = Column(column)
 
         args = []
 
-        if isinstance(column, StatementWithArgs):
+        if isinstance(column, Statement):
             args.extend(column.args)
 
         if isinstance(lower_bound, Statement):
             lower_bound_s = str(lower_bound)
-            if isinstance(lower_bound, StatementWithArgs):
+            if isinstance(lower_bound, Statement):
                 args.extend(lower_bound.args)
         else:
             args.append(lower_bound)
 
         if isinstance(upper_bound, Statement):
             upper_bound_s = str(upper_bound)
-            if isinstance(upper_bound, StatementWithArgs):
+            if isinstance(upper_bound, Statement):
                 args.extend(upper_bound.args)
         else:
             args.append(upper_bound)
 
         super().__init__(
             f"{str(column)} {'NOT ' if negative else ''}BETWEEN {lower_bound_s} AND {upper_bound_s}",
             *args
```

### Comparing `sqlfactory-1.2.1/sqlfactory/condition/in_condition.py` & `sqlfactory-1.3.0/sqlfactory/condition/in_condition.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """IN condition, used for checking whether column value is in given list of values."""
 
 from collections.abc import Collection
 from typing import overload, Any
 
-from ..entities import Column
-from ..statement import StatementWithArgs, Statement
 from .base import Condition, StatementOrColumn
+from ..entities import Column
+from ..statement import Statement
 
 
 # pylint: disable=too-few-public-methods   # Everything is handled by super classes.
 class In(Condition):
     """
     IN condition:
 
@@ -35,46 +35,53 @@
 
     @overload
     def __init__(self, column: StatementOrColumn, values: Collection[Any], *, negative: bool = False):
         """Provides type definition for statement `column` IN (%s, %s, %s)"""
 
     # pylint: disable=consider-using-f-string, too-many-branches  # Yes, IN statement is rather complex.
     def __init__(
-            self, column: StatementOrColumn | tuple[StatementOrColumn, ...],
-            values: Collection[Any | tuple[Any, ...]], *, negative: bool = False
+            self,
+            column: StatementOrColumn | tuple[StatementOrColumn, ...],
+            values: Collection[Any | tuple[Any, ...]],
+            *,
+            negative: bool = False
     ):
         """
         :param column: Column to compare, or tuple of columns for multi-column comparison.
         :param values: Values to compare (list of values, or list of tuples of values).
         :param negative: Whether to perform negative comparison (NOT IN)
         """
         add_none = False
 
-        if None in values:
-            add_none = True
-            values = list(filter(lambda v: v is not None, values))
+        for value in values:
+            if value is None:
+                add_none = True
+                break
+
+        if add_none:
+            values = [value for value in values if value is not None]
 
         args = []
 
         if isinstance(column, tuple):
             column = tuple(Column(col) if not isinstance(col, Statement) else col for col in column)
         elif not isinstance(column, Statement):
             column = Column(column)
 
         if values:
             if isinstance(column, tuple):
                 for stmt in column:
-                    if isinstance(stmt, StatementWithArgs):
+                    if isinstance(stmt, Statement):
                         args.extend(stmt.args)
 
                 for value_tuple in values:
                     for value in value_tuple:
                         if not isinstance(value, Statement):
                             args.append(value)
-                        elif isinstance(value, StatementWithArgs):
+                        elif isinstance(value, Statement):
                             args.extend(value.args)
 
                 super().__init__(
                     "({}) {} ({})".format(
                         ", ".join(map(str, column)),
                         "IN" if not negative else "NOT IN ",
                         ", ".join(["(" + ", ".join([
@@ -87,39 +94,39 @@
             else:
                 in_stmt = "{} {} ({})".format(
                     str(column),
                     "IN" if not negative else "NOT IN",
                     ", ".join(["%s" if not isinstance(value, Statement) else str(value) for value in values])
                 )
 
-                if isinstance(column, StatementWithArgs):
+                if isinstance(column, Statement):
                     args.extend(column.args)
 
                 for value in values:
-                    if isinstance(value, StatementWithArgs):
+                    if isinstance(value, Statement):
                         args.extend(value.args)
                     elif not isinstance(value, Statement):
                         args.append(value)
 
                 if add_none:
-                    if isinstance(column, StatementWithArgs):
+                    if isinstance(column, Statement):
                         args.extend(column.args)
 
                     super().__init__(
                         f"({in_stmt} {'OR' if not negative else 'AND'} {str(column)} IS {'NOT ' if negative else ''}NULL)",
                         *args
                     )
                 else:
                     super().__init__(
                         in_stmt,
                         *args
                     )
         elif add_none:
             # This could happen only if there is just a one column, not multi-column statement.
-            if isinstance(column, StatementWithArgs):
+            if isinstance(column, Statement):
                 args.extend(column.args)
 
             super().__init__(
                 f"{str(column)} IS {'NOT ' if negative else ''}NULL",
                 *args
             )
         else:
```

### Comparing `sqlfactory-1.2.1/sqlfactory/condition/like.py` & `sqlfactory-1.3.0/sqlfactory/condition/like.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """LIKE statement"""
 
 from typing import Any
 
 from .base import Condition, StatementOrColumn
 from ..entities import Column
-from ..statement import Statement, StatementWithArgs
+from ..statement import Statement
 
 
 class Like(Condition):
     """
     SQL LIKE statement
 
     `column` LIKE %s
@@ -18,18 +18,18 @@
     """
     def __init__(self, column: StatementOrColumn, value: Any | Statement, negative: bool = False):
         args = []
 
         if not isinstance(column, Statement):
             column = Column(column)
 
-        if isinstance(column, StatementWithArgs):
+        if isinstance(column, Statement):
             args.extend(column.args)
 
-        if isinstance(value, StatementWithArgs):
+        if isinstance(value, Statement):
             args.extend(value.args)
         else:
             args.append(value)
 
         if isinstance(value, Statement):
             super().__init__(
                 f"{str(column)}{' NOT' if negative else ''} LIKE {str(value)}",
```

### Comparing `sqlfactory-1.2.1/sqlfactory/condition/simple.py` & `sqlfactory-1.3.0/sqlfactory/condition/simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Simple binary comparison conditions."""
 
 from typing import Any
 
 from .base import Condition, StatementOrColumn
-from ..statement import Statement, StatementWithArgs
+from ..statement import Statement
 
 
 # pylint: disable=too-few-public-methods  # As everything is handled in base classes.
 class SimpleCondition(Condition):
     # pylint: disable=duplicate-code  # It does not make sense to generalize two-row statement used on two places.
     """
     Simple condition comparing one column with given value, using specified operator.
@@ -21,18 +21,18 @@
         if not isinstance(column, Statement):
             # pylint: disable=import-outside-toplevel,cyclic-import
             from ..entities import Column
             column = Column(column)
 
         args = []
 
-        if isinstance(column, StatementWithArgs):
+        if isinstance(column, Statement):
             args.extend(column.args)
 
-        if isinstance(value, StatementWithArgs):
+        if isinstance(value, Statement):
             args.extend(value.args)
 
         elif not isinstance(value, Statement):
             args.append(value)
 
         if isinstance(value, Statement):
             super().__init__(
```

### Comparing `sqlfactory-1.2.1/sqlfactory/delete/delete.py` & `sqlfactory-1.3.0/sqlfactory/delete/delete.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """DELETE statement builder"""
 
 from typing import Any
 
 from ..entities import Table
 from ..condition.base import ConditionBase
-from ..execute import ExecutableStatementWithArgs
+from ..execute import ExecutableStatement
 from ..mixins.limit import WithLimit, Limit
 from ..mixins.order import WithOrder, OrderArg
 from ..mixins.where import WithWhere
 
 
 # pylint: disable=too-many-ancestors  # This is intentional, as this class is a combination of multiple mixins.
-class Delete(ExecutableStatementWithArgs, WithWhere['Delete'], WithOrder['Delete'], WithLimit['Delete']):
+class Delete(ExecutableStatement, WithWhere['Delete'], WithOrder['Delete'], WithLimit['Delete']):
     """
     DELETE statement
 
     >>> Delete("table", where=In("id", [1, 2, 3]))
     >>> "DELETE FROM `table` WHERE `id` IN (1,2,3)"
     """
     def __init__(
```

### Comparing `sqlfactory-1.2.1/sqlfactory/entities.py` & `sqlfactory-1.3.0/sqlfactory/entities.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,65 +1,24 @@
 """Classes representing database entities."""
 
 from __future__ import annotations
+
 from typing import Any
 
-from .statement import Statement, Raw, StatementWithArgs
 from .condition.simple import Gt, Ge, Eq, Lt, Le, Ne
+from .statement import Raw, Statement
 
 
-class Column(Statement):
+class Expression(Statement):
     """
-    Column (optionally with table and database) as statement.
+    Expression as statement
 
-    Provides shorthand for creating conditional SQL statements and arithmetic SQL statements. You can use Column
-    instance to directly create condition using simple operators (==, !=, <, <=, >, >=) or arithmetic operations
-    (+, -, *, /, %).
-
-    >>> Column("table.column") == 5
-    >>> # Produces Eq(Column("table.column"), 5)
-
-    >>> Column("table.column") + 5
-    >>> # Produces Raw("`table`.`column` + %s", 5)
+    Represents expression that can be used in SQL statements. It provides basic methods for creating complex
+    expressions by combining columns, functions and literals together to one arithmetic function.
     """
-    def __init__(self, column: str):
-        super().__init__()
-
-        self._column = column.split(".")
-        if len(self._column) > 3:
-            raise ValueError("Invalid column name (contains more than <database>.<table>.<column>).")
-
-    def __str__(self) -> str:
-        return ".".join(map(lambda x: f"`{x}`" if not x.startswith("`") else x, self._column))
-
-    @property
-    def column(self) -> str:
-        """Returns column part of the column name."""
-        return self._column[-1]
-
-    @property
-    def table(self) -> str | None:
-        """Returns table part of the column name, if specified. If column specification does not contain table name,
-        returns None."""
-        try:
-            return self._column[-2]
-        except IndexError:
-            return None
-
-    @property
-    def database(self) -> str | None:
-        """Returns database part of the column name, if specified. If column specification does not contain database
-        name, returns None."""
-        try:
-            return self._column[-3]
-        except IndexError:
-            return None
-
-    def __hash__(self):
-        return hash(str(self))
 
     def __gt__(self, other: Statement | Any) -> Gt:
         """Shorthand to produce conditional SQL statement <column> > <other>."""
         return Gt(self, other)
 
     def __ge__(self, other: Statement | Any) -> Ge:
         """Shorthand to produce conditional SQL statement <column> >= <other>."""
@@ -77,96 +36,162 @@
         """Shorthand to produce conditional SQL statement <column> = <other>."""
         return Eq(self, other)
 
     def __ne__(self, other: Statement | Any) -> Ne:
         """Shorthand to produce conditional SQL statement <column> != <other>."""
         return Ne(self, other)
 
-    def __add__(self, other) -> StatementWithArgs:
+    def __add__(self, other) -> Statement:
         return Raw(
             f"{str(self)} + {str(other) if isinstance(other, Statement) else '%s'}",
-            *other.args if isinstance(other, StatementWithArgs)
+            *self.args,
+            *other.args if isinstance(other, Statement)
             else [other] if not isinstance(other, Statement)
             else []
         )
 
-    def __sub__(self, other) -> StatementWithArgs:
+    def __sub__(self, other) -> Statement:
         return Raw(
             f"{str(self)} - {str(other) if isinstance(other, Statement) else '%s'}",
-            *other.args if isinstance(other, StatementWithArgs)
+            *self.args,
+            *other.args if isinstance(other, Statement)
             else [other] if not isinstance(other, Statement)
             else []
         )
 
-    def __mul__(self, other) -> StatementWithArgs:
+    def __mul__(self, other) -> Statement:
         return Raw(
             f"{str(self)} * {str(other) if isinstance(other, Statement) else '%s'}",
-            *other.args if isinstance(other, StatementWithArgs)
+            *self.args,
+            *other.args if isinstance(other, Statement)
             else [other] if not isinstance(other, Statement)
             else []
         )
 
-    def __truediv__(self, other) -> StatementWithArgs:
+    def __truediv__(self, other) -> Statement:
         return Raw(
             f"{str(self)} / {str(other) if isinstance(other, Statement) else '%s'}",
-            *other.args if isinstance(other, StatementWithArgs)
+            *self.args,
+            *other.args if isinstance(other, Statement)
             else [other] if not isinstance(other, Statement)
             else []
         )
 
-    def __mod__(self, other) -> StatementWithArgs:
+    def __mod__(self, other) -> Statement:
         return Raw(
             f"{str(self)} % {str(other) if isinstance(other, Statement) else '%s'}",
-            *other.args if isinstance(other, StatementWithArgs)
+            *self.args,
+            *other.args if isinstance(other, Statement)
             else [other] if not isinstance(other, Statement)
             else []
         )
 
-    def __and__(self, other) -> StatementWithArgs:
+    def __and__(self, other) -> Statement:
         return Raw(
             f"{str(self)} & {str(other) if isinstance(other, Statement) else '%s'}",
-            *other.args if isinstance(other, StatementWithArgs)
+            *self.args,
+            *other.args if isinstance(other, Statement)
             else [other] if not isinstance(other, Statement)
             else []
         )
 
-    def __or__(self, other) -> StatementWithArgs:
+    def __or__(self, other) -> Statement:
         return Raw(
             f"{str(self)} | {str(other) if isinstance(other, Statement) else '%s'}",
-            *other.args if isinstance(other, StatementWithArgs)
+            *self.args,
+            *other.args if isinstance(other, Statement)
             else [other] if not isinstance(other, Statement)
             else []
         )
 
-    def __xor__(self, other) -> StatementWithArgs:
+    def __xor__(self, other) -> Statement:
         return Raw(
             f"{str(self)} ^ {str(other) if isinstance(other, Statement) else '%s'}",
-            *other.args if isinstance(other, StatementWithArgs)
+            *self.args,
+            *other.args if isinstance(other, Statement)
             else [other] if not isinstance(other, Statement)
             else []
         )
 
     def __lshift__(self, other):
         return Raw(
             f"{str(self)} << {str(other) if isinstance(other, Statement) else '%s'}",
-            *other.args if isinstance(other, StatementWithArgs)
+            *self.args,
+            *other.args if isinstance(other, Statement)
             else [other] if not isinstance(other, Statement)
             else []
         )
 
     def __rshift__(self, other):
         return Raw(
             f"{str(self)} >> {str(other) if isinstance(other, Statement) else '%s'}",
-            *other.args if isinstance(other, StatementWithArgs)
+            *self.args,
+            *other.args if isinstance(other, Statement)
             else [other] if not isinstance(other, Statement)
             else []
         )
 
     def __neg__(self):
-        return Raw(f"~{str(self)}")
+        return Raw(f"~{str(self)}", *self.args)
+
+
+class Column(Expression):
+    """
+    Column (optionally with table and database) as statement.
+
+    Provides shorthand for creating conditional SQL statements and arithmetic SQL statements. You can use Column
+    instance to directly create condition using simple operators (==, !=, <, <=, >, >=) or arithmetic operations
+    (+, -, *, /, %).
+
+    >>> Column("table.column") == 5
+    >>> # Produces Eq(Column("table.column"), 5)
+
+    >>> Column("table.column") + 5
+    >>> # Produces Raw("`table`.`column` + %s", 5)
+    """
+    def __init__(self, column: str):
+        super().__init__()
+
+        self._column = column.split(".")
+        if len(self._column) > 3:
+            raise ValueError("Invalid column name (contains more than <database>.<table>.<column>).")
+
+    def __str__(self) -> str:
+        return ".".join(map(lambda x: f"`{x}`" if not x.startswith("`") else x, self._column))
+
+    @property
+    def column(self) -> str:
+        """Returns column part of the column name."""
+        return self._column[-1]
+
+    @property
+    def table(self) -> str | None:
+        """Returns table part of the column name, if specified. If column specification does not contain table name,
+        returns None."""
+        try:
+            return self._column[-2]
+        except IndexError:
+            return None
+
+    @property
+    def database(self) -> str | None:
+        """Returns database part of the column name, if specified. If column specification does not contain database
+        name, returns None."""
+        try:
+            return self._column[-3]
+        except IndexError:
+            return None
+
+    def __hash__(self):
+        return hash(str(self))
+
+    @property
+    def args(self) -> list[Any]:
+        """Column does not have any arguments."""
+        return []
 
 
 class Table(Statement):
     """
     Table (optionally with database) as statement
 
     By accessing Table's undefined attributes, instance of Column is returned. This allows to easily access columns of
@@ -204,10 +229,15 @@
         except IndexError:
             return None
 
     def __getattr__(self, name: str) -> Column:
         """Returns column of that table."""
         return Column(f"{'.'.join(self._table)}.{name}")
 
+    @property
+    def args(self) -> list[Any]:
+        """Table does not have any arguments."""
+        return []
+
 
 # Alias for column that can be passed as instance of column or as string.
 ColumnArg = Column | str
```

### Comparing `sqlfactory-1.2.1/sqlfactory/execute.py` & `sqlfactory-1.3.0/sqlfactory/execute.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Module containing definition of executable SQL statements base classes."""
 
 import inspect
 from abc import ABC
 from typing import Protocol, Any, overload
 
 from .logger import logger
-from .statement import Statement, StatementWithArgs, ConditionalStatement
+from .statement import Statement, ConditionalStatement
 
 
 # pylint: disable=too-few-public-methods, missing-function-docstring  # As this is just a protocol.
 class HasQueryWithTupleArgs(Protocol):
     """Protocol defining DB driver with query method that takes arguments as tuple."""
     def query(self, query: str, args: tuple[Any]): ...
 
@@ -101,35 +101,17 @@
         elif hasattr(trx, "execute"):
             call = trx.execute
         else:
             raise AttributeError("trx must define query() or execute() method.")
 
         sig = inspect.signature(call)
         if any(map(lambda p: p.kind == inspect.Parameter.VAR_POSITIONAL, sig.parameters.values())):
-            return call(str(self), *args)
+            return call(str(self), *self.args, *args)
 
-        return call(str(self), tuple(args))
-
-
-class ExecutableStatementWithArgs(StatementWithArgs, ExecutableStatement, ABC):
-    """
-    Base class of executable SQL statement with arguments that should be escaped.
-    """
-    def execute(self, trx: MaybeAsyncHasQueryOrExecute, *args):
-        """
-        Execute statement on db driver (db-agnostic, just expects method `query` or `execute` on given driver).
-        Passes staement arguments to the driver's method. Returns response of the driver's method.
-        This is just a shortland for calling driver.execute(str(self), *self.args).
-
-        :param trx: DB driver with query() or execute() method, which accepts either tuple as arguments,
-         or multiple arguments following the query.
-        :param args: Additional arguments to append to the end of argument list (you probably don't need this).
-        :return: The same as db driver's execute/query method. If driver is async, returns awaitable response.
-        """
-        return super().execute(trx, *self.args, *args)  # type: ignore
+        return call(str(self), tuple(self.args + list(args)))
 
 
 class ConditionalExecutableStatement(ExecutableStatement, ConditionalStatement, ABC):
     """
     Mixin that provides conditional execution of the statement (query will be executed only if statement is valid).
 
     This class is used for example for INSERT statements, to not execute empty INSERT. Or to not execute UPDATE
```

### Comparing `sqlfactory-1.2.1/sqlfactory/func/agg.py` & `sqlfactory-1.3.0/sqlfactory/func/agg.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Aggregate functions."""
 
 from typing import Literal
 
 from .base import Function
-from .. import Raw, StatementWithArgs
+from .. import Raw, Statement
 from ..entities import Column, ColumnArg
 
 
 # pylint: disable=too-few-public-methods
 class AggregateFunction(Function):
     """Base class for aggregate functions"""
     def __init__(self, agg: str, column: ColumnArg):
@@ -53,15 +53,15 @@
             column = Raw('*')
         elif isinstance(column, str):
             column = Column(column)
 
         if distinct:
             super().__init__(
                 "COUNT",
-                Raw(f"DISTINCT {str(column)}", *column.args if isinstance(column, StatementWithArgs) else [])
+                Raw(f"DISTINCT {str(column)}", *column.args if isinstance(column, Statement) else [])
             )
         else:
             super().__init__(
                 "COUNT",
                 column
             )
```

### Comparing `sqlfactory-1.2.1/sqlfactory/func/base.py` & `sqlfactory-1.3.0/sqlfactory/func/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Base classes for SQL functions"""
 
 from typing import Any
 
-from ..statement import StatementWithArgs, Statement
+from ..entities import Expression
+from ..statement import Statement
 
 
-class Function(StatementWithArgs):
+class Function(Expression):
     """Generic function with name and variable number of arguments."""
     def __init__(self, function: str, *args: Statement | Any):
         self.function = function
         self._args = args
 
     def _args_placeholders(self) -> list[str]:
         out: list[str] = []
@@ -25,13 +26,13 @@
     def __str__(self):
         return f"{self.function}({', '.join(self._args_placeholders())})"
 
     @property
     def args(self) -> list[Any]:
         out = []
         for arg in self._args:
-            if isinstance(arg, StatementWithArgs):
+            if isinstance(arg, Statement):
                 out.extend(arg.args)
             elif not isinstance(arg, Statement):
                 out.append(arg)
 
         return out
```

### Comparing `sqlfactory-1.2.1/sqlfactory/func/control.py` & `sqlfactory-1.3.0/sqlfactory/func/control.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.2.1/sqlfactory/func/datetime.py` & `sqlfactory-1.3.0/sqlfactory/func/datetime.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Date/Time SQL functions (https://mariadb.com/kb/en/date-time-functions/)."""
 from typing import Any, Literal
 
 from .base import Function
-from .. import StatementWithArgs, Statement, Raw
+from .. import Statement, Raw
 
 
 # pylint: disable=too-many-instance-attributes
-class Interval(StatementWithArgs):
+class Interval(Statement):
     """
     INTERVAL statement for DATE_ADD, DATE_SUB and similar functions.
     """
     _ATTRIBUTES = (
         "microsecond", "second", "minute", "hour", "day", "week", "month", "quarter", "year",
         "second_microsecond", "minute_microsecond", "minute_second", "hour_microsecond", "hour_second",
         "hour_minute", "day_microsecond", "day_second", "day_minute", "day_hour", "year_month"
@@ -76,15 +76,15 @@
         args = []
 
         for attr in reversed(self._ATTRIBUTES):
             value = getattr(self, attr)
             if value is None:
                 continue
 
-            if isinstance(value, StatementWithArgs):
+            if isinstance(value, Statement):
                 args.extend(value.args)
 
             elif not isinstance(value, Statement):
                 args.append(value)
 
         return args
 
@@ -262,15 +262,15 @@
 
 # pylint: disable=too-few-public-methods
 class Extract(Function):
     """
     Extracts part of date.
     """
     def __init__(self, unit: str, date: Any):
-        args = [date] if not isinstance(date, Statement) else date.args if isinstance(date, StatementWithArgs) else []
+        args = [date] if not isinstance(date, Statement) else date.args if isinstance(date, Statement) else []
         super().__init__(
             "EXTRACT",
             Raw(
                 f"{unit} FROM {str(date) if isinstance(date, Statement) else '%s'}",
                 *args
             )
         )
```

### Comparing `sqlfactory-1.2.1/sqlfactory/func/enc.py` & `sqlfactory-1.3.0/sqlfactory/func/enc.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.2.1/sqlfactory/func/info.py` & `sqlfactory-1.3.0/sqlfactory/func/info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Information functions (https://mariadb.com/kb/en/information-functions/)."""
 from typing import Any
 
 from .base import Function
-from .. import Statement, StatementWithArgs, Raw, Column
+from .. import Statement, Raw, Column
 
 
 # pylint: disable=too-few-public-methods
 class Benchmark(Function):
     """Executes an expression repeatedly."""
     def __init__(self, count: int, expression: Statement):
         super().__init__('BENCHMARK', count, expression)
@@ -43,15 +43,15 @@
 # pylint: disable=too-few-public-methods
 class Collate(Raw):
     """String with collation"""
     def __init__(self, expression: str | Statement, collation: str):
         super().__init__(
             f"{str(expression) if isinstance(expression, Statement) else '%s'} COLLATE {collation}",
             *(
-                expression.args if isinstance(expression, StatementWithArgs)
+                expression.args if isinstance(expression, Statement)
                 else [expression] if not isinstance(expression, Statement)
                 else []
             )
         )
 
 
 # pylint: disable=too-few-public-methods
```

### Comparing `sqlfactory-1.2.1/sqlfactory/func/misc.py` & `sqlfactory-1.3.0/sqlfactory/func/misc.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.2.1/sqlfactory/func/numeric.py` & `sqlfactory-1.3.0/sqlfactory/func/numeric.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.2.1/sqlfactory/func/str.py` & `sqlfactory-1.3.0/sqlfactory/func/str.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.2.1/sqlfactory/insert/insert.py` & `sqlfactory-1.3.0/sqlfactory/insert/insert.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from __future__ import annotations
 
 from collections.abc import Collection
 from typing import Any
 
 from .values import Values
 from ..entities import ColumnArg, Column, Table
-from ..execute import ExecutableStatementWithArgs, ConditionalExecutableStatement
-from ..statement import Statement, StatementWithArgs
+from ..execute import ConditionalExecutableStatement
+from ..statement import Statement
 
 
-class Insert(ConditionalExecutableStatement, ExecutableStatementWithArgs):
+class Insert(ConditionalExecutableStatement):
     """
     INSERT statement
 
     Statement is conditional, which means it won't be executed if no rows would be inserted (which throws SQL error).
 
     >>> Insert.into("table")("column1", "column2", "column3").values((1, 2, 3), (4, 5, 6))
     >>> "INSERT INTO `table` (`column1`, `column2`, `column3`) VALUES (1, 2, 3), (4, 5, 6)"
@@ -103,15 +103,15 @@
         >>> )
         """
         for column, stmt in kwargs.items():
             if not isinstance(column, Column):
                 column = Column(column)
 
             self._on_duplicate_key_update_set.append((column, str(stmt) if isinstance(stmt, Statement) else "%s"))
-            if isinstance(stmt, StatementWithArgs):
+            if isinstance(stmt, Statement):
                 self._on_duplicate_key_update_args.extend(stmt.args)
             elif not isinstance(stmt, Statement):
                 self._on_duplicate_key_update_args.append(stmt)
 
         return self
 
     # pylint: disable=invalid-name
@@ -165,15 +165,15 @@
 
     @property
     def args(self) -> list[Any]:
         out = []
 
         for row in self._values:
             for v in row:
-                if isinstance(v, StatementWithArgs):
+                if isinstance(v, Statement):
                     out.extend(v.args)
                 elif not isinstance(v, Statement):
                     out.append(v)
 
         out.extend(self._on_duplicate_key_update_args)
 
         return out
```

### Comparing `sqlfactory-1.2.1/sqlfactory/insert/values.py` & `sqlfactory-1.3.0/sqlfactory/insert/values.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.2.1/sqlfactory/mixins/limit.py` & `sqlfactory-1.3.0/sqlfactory/mixins/limit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """LIMIT statement"""
 
 from typing import TypeVar, Generic, overload
 
-from sqlfactory.statement import StatementWithArgs, ConditionalStatement
+from sqlfactory.statement import Statement, ConditionalStatement
 
 T = TypeVar("T")
 
 
-class Limit(ConditionalStatement, StatementWithArgs):
+class Limit(ConditionalStatement, Statement):
     """LIMIT statement"""
 
     @overload
     def __init__(self):
         """No LIMIT statement"""
 
     @overload
```

### Comparing `sqlfactory-1.2.1/sqlfactory/mixins/order.py` & `sqlfactory-1.3.0/sqlfactory/mixins/order.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """ORDER BY mixin for query generator"""
 
 from __future__ import annotations
+
 from enum import Enum
 from typing import Any, Generic, TypeVar, Collection, Literal
 
 from ..entities import Column, ColumnArg
-from ..statement import Statement, StatementWithArgs
+from ..statement import Statement
 
 
 class Direction(str, Enum):
     """Ordering direction as enum"""
     ASC = "ASC"
     DESC = "DESC"
 
 
 OrderColumn = ColumnArg | Statement
 
 
-class Order(list[tuple[OrderColumn, Direction | Literal['ASC', 'DESC']]], StatementWithArgs):
+class Order(list[tuple[OrderColumn, Direction | Literal['ASC', 'DESC']]], Statement):
     """ORDER BY statement as list of columns to use for ordering"""
     def __str__(self):
         if not self:
             return ""
 
         out = []
 
@@ -33,15 +34,15 @@
 
         return f"ORDER BY {', '.join(out)}"
 
     @property
     def args(self) -> list[Any]:
         out = []
         for column, _ in self:
-            if isinstance(column, StatementWithArgs):
+            if isinstance(column, Statement):
                 out.extend(column.args)
 
         return out
 
 
 T = TypeVar('T')
```

### Comparing `sqlfactory-1.2.1/sqlfactory/mixins/where.py` & `sqlfactory-1.3.0/sqlfactory/mixins/where.py`

 * *Files identical despite different names*

### Comparing `sqlfactory-1.2.1/sqlfactory/select/aliased.py` & `sqlfactory-1.3.0/sqlfactory/select/aliased.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 """Column / Statement aliasing support"""
 
 from typing import Any
 
 from sqlfactory.entities import ColumnArg, Column
-from sqlfactory.statement import StatementWithArgs, Statement
+from sqlfactory.statement import Statement
 
 
 # pylint: disable=too-few-public-methods
-class Aliased(StatementWithArgs):
+class Aliased(Statement):
     """Aliased generic statement. Only to be used in SELECT statement, where AS statement is only valid."""
     def __init__(self, statement: Statement | ColumnArg, alias: str = None):
         super().__init__()
         self._statement = statement if isinstance(statement, Statement) else Column(statement)
         self.alias = alias
 
     def __str__(self):
         if self.alias is None:
             return str(self._statement)
 
         return f"{str(self._statement)} AS `{self.alias}`"
 
     @property
     def args(self) -> list[Any]:
-        return self._statement.args if isinstance(self._statement, StatementWithArgs) else []
+        return self._statement.args
 
     def __getattr__(self, name):
         """Proxy to access attributes of inner (non-aliased) statement."""
         return getattr(self._statement, name)
 
 
 class SelectColumn(Aliased):
```

### Comparing `sqlfactory-1.2.1/sqlfactory/select/column_list.py` & `sqlfactory-1.3.0/sqlfactory/select/column_list.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 """Column list for usage in SELECT statement."""
 
 from __future__ import annotations
+
 from typing import Iterable, Any
 
 from sqlfactory.entities import ColumnArg, Column
-from sqlfactory.statement import StatementWithArgs, Statement
+from sqlfactory.statement import Statement
 
 
-class ColumnList(StatementWithArgs, list[Statement]):
+class ColumnList(Statement, list[Statement]):
     """
     Unique(ish) set of columns to be used in SELECT statement.
     """
     def __init__(self, iterable: Iterable[Statement | ColumnArg] = None):
         if iterable:
             super().__init__(map(
                 lambda i: Column(i) if not isinstance(i, Statement) else i,
                 iterable
             ))
         else:
             super().__init__()
 
     def __contains__(self, other: Statement):
-        """This needs custom implementation over default list.__contains__ because we need to compare Column objects,
-        which would generate Eq() instances instead of doing comparison."""
-        if isinstance(other, Column):
-            other = str(other)
+        """This needs custom implementation over default list.__contains__ because we need to compare Expression
+        objects, which would generate Eq() instances instead of doing comparison."""
+        if not isinstance(other, Statement):
+            raise AttributeError("ColumnList can only contain Statement objects.")
 
         for item in self:
-            if isinstance(item, Column):
-                item = str(item)
-
-            if item == other:
+            if str(item) == str(other) and item.args == other.args:
                 return True
 
         return False
 
     def add(self, element: Statement | str) -> ColumnList:
         """Add new columns to the set."""
         return self.append(element)
@@ -63,11 +61,11 @@
         return "[" + ", ".join(map(repr, self)) + "]"
 
     @property
     def args(self) -> list[Any]:
         out = []
 
         for item in self:
-            if isinstance(item, StatementWithArgs):
+            if isinstance(item, Statement):
                 out.extend(item.args)
 
         return out
```

### Comparing `sqlfactory-1.2.1/sqlfactory/select/join.py` & `sqlfactory-1.3.0/sqlfactory/select/join.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """JOIN statements for SQL queries."""
 
 from typing import Any
 
 from sqlfactory.entities import Table
 from sqlfactory.condition.base import ConditionBase
-from sqlfactory.statement import StatementWithArgs
+from sqlfactory.statement import Statement
 
 
-class Join(StatementWithArgs):
+class Join(Statement):
     """JOIN statement"""
     def __init__(self, table: str | Table, on: ConditionBase = None, alias: str = None):
         if isinstance(table, str):
             table = Table(table)
 
         self.table = table
         self.on = on
```

### Comparing `sqlfactory-1.2.1/sqlfactory/select/select.py` & `sqlfactory-1.3.0/sqlfactory/select/select.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from functools import reduce
 from typing import Any, overload
 
 from .column_list import ColumnList
 from .join import Join, LeftJoin
 from ..entities import ColumnArg, Table
 from ..condition.base import ConditionBase
-from ..execute import ExecutableStatementWithArgs
+from ..execute import ExecutableStatement
 from ..mixins.limit import WithLimit, Limit
 from ..mixins.order import WithOrder, OrderArg
 from ..mixins.where import WithWhere
-from ..statement import StatementWithArgs, Statement
+from ..statement import Statement
 
 
 # pylint: disable=too-many-ancestors  # Intentional, as this class is a combination of multiple mixins.
-class Select(ExecutableStatementWithArgs, WithWhere['Select'], WithOrder['Select'], WithLimit['Select']):
+class Select(ExecutableStatement, WithWhere['Select'], WithOrder['Select'], WithLimit['Select']):
     # pylint: disable=too-many-arguments  # Yes, SELECT is complex.
     """
     SELECT statement
 
     >>> (Select("column1", "column2", "column3", table="table_name")
     >>>     .where(Eq("column1", 1))
     >>>     .order_by("column2")
@@ -189,15 +189,15 @@
         if self._join:
             for join in self._join:
                 out.extend(join.args)
 
         return (
             out +
             reduce(
-                lambda acc, t: acc + (t.args if isinstance(t, StatementWithArgs) else []),
+                lambda acc, t: acc + (t.args if isinstance(t, Statement) else []),
                 self.table,
                 []
             ) +
             (self._where.args if self._where else []) +
             (self._group_by.args if self._group_by else []) +
             (self._having.args if self._having else []) +
             (self._order.args if self._order else []) +
```

### Comparing `sqlfactory-1.2.1/sqlfactory/statement.py` & `sqlfactory-1.3.0/sqlfactory/statement.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,85 +4,51 @@
 
 from abc import ABC, abstractmethod
 from typing import Any
 
 
 class Statement(ABC):
     """
-    Base class of serializable SQL statement. This class cannot hold any data, it is just an interface
-    for other classes to implement.
-
-    Everything that should be serialized to SQL should inherit from this class or it's subclasses, as many
-    checks in code are based on instance of this class.
-
-    To retrieve SQL statement, call str() on the instance.
-    """
-
-    @abstractmethod
-    def __str__(self) -> str:
-        """Return SQL statement representing the statement."""
-
-    def __repr__(self):
-        """Representation for debugging purposes, it is not used in SQL generation."""
-        return self.__str__()
-
-    def __hash__(self):
-        """Return hash of this statement to be able to use it in unique collections."""
-        return hash(str(self))
-
-    def __eq__(self, other: 'Statement'):
-        """Compares this statement to other."""
-        if not isinstance(other, Statement):
-            return False
-
-        return str(self) == str(other)
-
-
-class StatementWithArgs(Statement):
-    """
     Base class of serializable SQL statement with arguments that should be escaped. This class cannot hold any data,
     it is just an interface for other classes to implement.
 
     Any class that needs SQL argument substitution should inherit from this class, as there are checks that tests
     whether passed object is instance of this class.
 
     To retrieve SQL statement, call `str()` on the instance. To retrieve arguments, access `args` property.
     """
 
+    @abstractmethod
+    def __str__(self) -> str:
+        """Return SQL statement representing the statement."""
+
     @property
     @abstractmethod
     def args(self) -> list[Any]:
         """Return arguments representing `%s` placeholders in statement returned by `__str__()`. Number of items
         in returned list must match number of `%s` placeholders in string returned by calling `__str__()`."""
 
-    def __hash__(self):
+    def __hash__(self) -> int:
         """Return hash of this statement to be able to use it in unique collections."""
-        return super().__hash__() + sum(map(hash, self.args))
+        return hash(str(self)) + sum(map(hash, self.args))
 
-    def __eq__(self, other: 'StatementWithArgs'):
+    def __eq__(self, other: 'Statement') -> bool:
         """Compares this statement to other."""
-
-        # If other is not instance of StatementWithArgs (it is basic statement probably) and we have no args,
-        # we can compare it as normal statement.
-        if not isinstance(other, StatementWithArgs):
-            if not self.args:
-                return super().__eq__(other)
-
-            # If we have args and other does not, they are not equal.
+        if str(self) != str(other):
             return False
 
-        return self.args == other.args and super().__eq__(other)
+        return isinstance(other, Statement) and self.args == other.args
 
-    def __repr__(self):
-        """Representation of statement including the arguments."""
+    def __repr__(self) -> str:
+        """Representation of statement including the arguments, if any."""
         args = list(map(repr, self.args))
         if args:
-            return f"{super().__repr__()} with arguments [{', '.join(args)}]"
+            return f"{self.__str__()} with arguments [{', '.join(args)}]"
 
-        return super().__repr__()
+        return self.__str__()
 
 
 # pylint: disable=too-few-public-methods  # As this is just an interface.
 class ConditionalStatement(ABC):
     """
     Mixin that provides conditional execution of the statement (query will be executed only if statement is valid).
 
@@ -92,15 +58,15 @@
     @abstractmethod
     def __bool__(self) -> bool:
         """
         Return True if the statement should be executed.
         """
 
 
-class Raw(StatementWithArgs):
+class Raw(Statement):
     """
     RAW string statement (with optional args), that won't be processed in any way.
     """
 
     def __init__(self, sql: str, *args: Any):
         super().__init__()
         self._statement = sql
```

### Comparing `sqlfactory-1.2.1/sqlfactory/update/update.py` & `sqlfactory-1.3.0/sqlfactory/update/update.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 from __future__ import annotations
 
 from typing import Any, Optional
 
 from ..condition.base import ConditionBase
 from ..entities import ColumnArg, Column, Table
-from ..execute import ExecutableStatementWithArgs, ConditionalExecutableStatement
+from ..execute import ConditionalExecutableStatement
 from ..mixins.limit import WithLimit, Limit
 from ..mixins.where import WithWhere
-from ..statement import StatementWithArgs, Statement
+from ..statement import Statement
 
 
-class UpdateColumn(StatementWithArgs):
+class UpdateColumn(Statement):
     """
     Represents one field that should be updated.
     """
     def __init__(self, column: ColumnArg, value: Statement | Any):
         self._column = column if isinstance(column, Column) else Column(column)
         self._value = value
 
@@ -33,25 +33,22 @@
         return str(self._column) == str(other._column)
 
     @property
     def args(self) -> list[Any]:
         """
         Return arguments for the update statement.
         """
-        if isinstance(self._value, StatementWithArgs):
+        if isinstance(self._value, Statement):
             return self._value.args
 
-        if not isinstance(self._value, Statement):
-            return [self._value]
-
-        return []
+        return [self._value]
 
 
 # pylint: disable=too-many-ancestors  # This is intentional, as this class is a combination of multiple mixins.
-class Update(ExecutableStatementWithArgs, ConditionalExecutableStatement, WithWhere['Update'], WithLimit['Update']):
+class Update(ConditionalExecutableStatement, WithWhere['Update'], WithLimit['Update']):
     """
     Builds UPDATE statement SQL query.
 
     This is conditional SQL statement, so you can check whether it should be executed (would update any columns)
     by calling bool() on it. Also, if you are using execute() method of the statement, the execution won't be
     performed if bool() returns False.
```

### Comparing `sqlfactory-1.2.1/PKG-INFO` & `sqlfactory-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfactory
-Version: 1.2.1
+Version: 1.3.0
 Summary: Convenient classes for building SQL queries in Python. Main purpose of this library is to ease construction of SQL queries in Python code. It is not an ORM (and don't intend to be), just a plain SQL query builder with syntax as similar to actual SQL as possible.
 Author: Michal Kuchta
 Author-email: niximor@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

