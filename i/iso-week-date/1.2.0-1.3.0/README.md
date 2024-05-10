# Comparing `tmp/iso_week_date-1.2.0.tar.gz` & `tmp/iso_week_date-1.3.0.tar.gz`

## Comparing `iso_week_date-1.2.0.tar` & `iso_week_date-1.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 iso_week_date-1.2.0/iso_week_date/__init__.py
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 iso_week_date-1.2.0/iso_week_date/_patterns.py
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 iso_week_date-1.2.0/iso_week_date/_utils.py
--rw-r--r--   0        0        0     9472 2020-02-02 00:00:00.000000 iso_week_date-1.2.0/iso_week_date/base.py
--rw-r--r--   0        0        0    14494 2020-02-02 00:00:00.000000 iso_week_date-1.2.0/iso_week_date/isoweek.py
--rw-r--r--   0        0        0    10031 2020-02-02 00:00:00.000000 iso_week_date-1.2.0/iso_week_date/isoweekdate.py
--rw-r--r--   0        0        0    13908 2020-02-02 00:00:00.000000 iso_week_date-1.2.0/iso_week_date/mixin.py
--rw-r--r--   0        0        0    17271 2020-02-02 00:00:00.000000 iso_week_date-1.2.0/iso_week_date/pandas_utils.py
--rw-r--r--   0        0        0    17344 2020-02-02 00:00:00.000000 iso_week_date-1.2.0/iso_week_date/polars_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 iso_week_date-1.2.0/iso_week_date/py.typed
--rw-r--r--   0        0        0     5021 2020-02-02 00:00:00.000000 iso_week_date-1.2.0/iso_week_date/pydantic.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 iso_week_date-1.2.0/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 iso_week_date-1.2.0/LICENSE
--rw-r--r--   0        0        0     5886 2020-02-02 00:00:00.000000 iso_week_date-1.2.0/README.md
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 iso_week_date-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     9828 2020-02-02 00:00:00.000000 iso_week_date-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 iso_week_date-1.3.0/iso_week_date/__init__.py
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 iso_week_date-1.3.0/iso_week_date/_patterns.py
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 iso_week_date-1.3.0/iso_week_date/_utils.py
+-rw-r--r--   0        0        0    10740 2020-02-02 00:00:00.000000 iso_week_date-1.3.0/iso_week_date/base.py
+-rw-r--r--   0        0        0    15304 2020-02-02 00:00:00.000000 iso_week_date-1.3.0/iso_week_date/isoweek.py
+-rw-r--r--   0        0        0    10710 2020-02-02 00:00:00.000000 iso_week_date-1.3.0/iso_week_date/isoweekdate.py
+-rw-r--r--   0        0        0    14210 2020-02-02 00:00:00.000000 iso_week_date-1.3.0/iso_week_date/mixin.py
+-rw-r--r--   0        0        0    17542 2020-02-02 00:00:00.000000 iso_week_date-1.3.0/iso_week_date/pandas_utils.py
+-rw-r--r--   0        0        0    17591 2020-02-02 00:00:00.000000 iso_week_date-1.3.0/iso_week_date/polars_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 iso_week_date-1.3.0/iso_week_date/py.typed
+-rw-r--r--   0        0        0     5223 2020-02-02 00:00:00.000000 iso_week_date-1.3.0/iso_week_date/pydantic.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 iso_week_date-1.3.0/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 iso_week_date-1.3.0/LICENSE
+-rw-r--r--   0        0        0     5886 2020-02-02 00:00:00.000000 iso_week_date-1.3.0/README.md
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 iso_week_date-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     9849 2020-02-02 00:00:00.000000 iso_week_date-1.3.0/PKG-INFO
```

### Comparing `iso_week_date-1.2.0/iso_week_date/_patterns.py` & `iso_week_date-1.3.0/iso_week_date/_patterns.py`

 * *Files identical despite different names*

### Comparing `iso_week_date-1.2.0/iso_week_date/_utils.py` & `iso_week_date-1.3.0/iso_week_date/_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,28 @@
+from __future__ import annotations
+
+import re
 import sys
-from typing import Callable, Generic, Type, TypeVar, Union
+from importlib.metadata import version
+from typing import Callable, Generic, Tuple, Type, TypeVar
 
-if sys.version_info >= (3, 11):
-    from typing import Self  # pragma: no cover
-else:
-    from typing_extensions import Self  # pragma: no cover
+if sys.version_info >= (3, 11):  # pragma: no cover
+    from typing import Self
+else:  # pragma: no cover
+    from typing_extensions import Self
 
 
 T = TypeVar("T")
 R = TypeVar("R")
 
 
-class classproperty(Generic[T, R]):
-    """Decorator to create a class level property. It allows to define a property at the class level, which can be
-    accessed without creating an instance of the class.
+class classproperty(Generic[T, R]):  # noqa: N801
+    """Decorator to create a class level property.
+
+    It allows to define a property at the class level, which can be accessed without creating an instance of the class.
 
     Arguments:
         func: Function to be decorated.
 
     Examples:
     ```python
     class CustomClass:
@@ -31,41 +36,40 @@
     ```
     """
 
     def __init__(self: Self, func: Callable[[Type[T]], R]) -> None:
         """Initialize classproperty."""
         self.func = func
 
-    def __get__(self: Self, obj: Union[T, None], owner: Type[T]) -> R:
+    def __get__(self: Self, obj: T | None, owner: Type[T]) -> R:
         """Get the value of the class property.
 
         Arguments:
             obj: The instance of the class (ignored)
             owner: The class that owns the property
         """
         return self.func(owner)
 
 
 def format_err_msg(_fmt: str, _value: str) -> str:  # pragma: no cover
     """Format error message given a format and a value."""
-
     return (
         "Invalid isoweek date format. "
         f"Format must match the '{_fmt}' pattern, "
         "where:"
         "\n- YYYY is a year between 0001 and 9999"
         "\n- W is a literal character"
         "\n- NN is a week number between 1 and 53"
         "\n- D is a day number between 1 and 7"
         f"\n but found {_value}"
     )
 
 
 def p_of_year(year: int) -> int:
-    """Returns the day of the week of 31 December"""
+    """Returns the day of the week of 31 December."""
     return (year + year // 4 - year // 100 + year // 400) % 7
 
 
 def weeks_of_year(year: int) -> int:
     """Returns the max number of weeks in a year.
 
     From wikipedia section on [weeks per year](https://en.wikipedia.org/wiki/ISO_week_date#Weeks_per_year):
@@ -75,8 +79,14 @@
 
     Arguments:
         year: Ordinal year number
 
     Returns:
         Number of weeks in the year (either 52 or 53)
     """
-    return 52 + (p_of_year(year) == 4 or p_of_year(year - 1) == 3)
+    return 52 + (p_of_year(year) == 4 or p_of_year(year - 1) == 3)  # noqa: PLR2004
+
+
+def parse_version(module: str) -> Tuple[int, ...]:
+    """Parses a module version and return a tuple of integers."""
+    module_version = version(module).split(".")
+    return tuple(int(re.sub(r"\D", "", str(v))) for v in module_version)
```

### Comparing `iso_week_date-1.2.0/iso_week_date/base.py` & `iso_week_date-1.3.0/iso_week_date/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 from datetime import date, datetime, timedelta
 from enum import Enum
 from typing import ClassVar, Generator, Iterable, Literal, Type, TypeVar, Union, overload
 
 from iso_week_date._utils import classproperty, format_err_msg, weeks_of_year
 from iso_week_date.mixin import ComparatorMixin, ConverterMixin, IsoWeekProtocol, ParserMixin
 
-if sys.version_info >= (3, 11):
-    from typing import Self  # pragma: no cover
-else:
-    from typing_extensions import Self  # pragma: no cover
+if sys.version_info >= (3, 11):  # pragma: no cover
+    from typing import Self
+else:  # pragma: no cover
+    from typing_extensions import Self
 
-BaseIsoWeek_T = TypeVar("BaseIsoWeek_T", str, date, datetime, "BaseIsoWeek", covariant=True)
+BaseIsoWeek_T = TypeVar("BaseIsoWeek_T", str, date, datetime, "BaseIsoWeek", covariant=True)  # noqa: PLC0105
 
 
 class InclusiveEnum(str, Enum):
-    """Inclusive enum"""
+    """Enum describing the Inclusive values."""
 
     both = "both"
     left = "left"
     right = "right"
     neither = "neither"
 
 
@@ -72,33 +72,34 @@
 
         if not _match:
             raise ValueError(format_err_msg(cls._format, value))
 
         year, week = int(_match.group(1)), int(_match.group(2)[1:])
 
         if weeks_of_year(year) < week:
-            raise ValueError(f"Invalid week number. Year {year} has only {weeks_of_year(year)} weeks.")
+            msg = f"Invalid week number. Year {year} has only {weeks_of_year(year)} weeks."
+            raise ValueError(msg)
 
         return value
 
     def __repr__(self: Self) -> str:
         """Custom representation."""
         return f"{self.name}({self.value_}) with offset {self.offset_}"
 
     def __str__(self: Self) -> str:
         """String conversion operator, returns iso-week string value ignoring offset."""
         return self.value_
 
     @classproperty
-    def _compact_pattern(cls: Type[IsoWeekProtocol]) -> re.Pattern:
+    def _compact_pattern(cls: Type[IsoWeekProtocol]) -> re.Pattern:  # noqa: N805
         """Returns compiled compact pattern."""
         return re.compile(cls._pattern.pattern.replace(")-(", ")("))
 
     @classproperty
-    def _compact_format(cls: Type[IsoWeekProtocol]) -> str:
+    def _compact_format(cls: Type[IsoWeekProtocol]) -> str:  # noqa: N805
         """Returns compact format as string."""
         return cls._format.replace("-", "")
 
     @property
     def name(self: Self) -> str:
         """Returns class name."""
         return self.__class__.__name__
@@ -129,86 +130,131 @@
         IsoWeekDate("2023-W01-1").week  # 1
         ```
         """
         return int(self.value_[6:8])
 
     @property
     def quarter(self: Self) -> int:
-        """Returns quarter number as integer. The first three quarters have 13 weeks, while the last one has either 13
-        or 14 weeks depending on the year.
+        """Returns quarter number as integer.
+
+        The first three quarters have 13 weeks, while the last one has either 13 or 14 weeks depending on the year:
 
         - Q1: weeks from 1 to 13
         - Q2: weeks from 14 to 26
         - Q3: weeks from 27 to 39
         - Q4: weeks from 40 to 52 (or 53 if applicable)
 
         Examples:
         ```py
         from iso_week_date import IsoWeek, IsoWeekDate
 
         IsoWeek("2023-W01").quarter  # 1
         IsoWeekDate("2023-W52-1").quarter  # 4
         ```
         """
-
         return min((self.week - 1) // 13 + 1, 4)
 
     @overload
-    def __add__(self: Self, other: Union[int, timedelta]) -> Self:  # pragma: no cover
-        """Implementation of addition operator."""
-        ...
+    def __add__(self: Self, other: Union[int, timedelta]) -> Self: ...  # pragma: no cover
 
     @overload
-    def __add__(self: Self, other: Iterable[Union[int, timedelta]]) -> Generator[Self, None, None]:  # pragma: no cover
-        """Implementation of addition operator."""
-        ...
+    def __add__(
+        self: Self,
+        other: Iterable[Union[int, timedelta]],
+    ) -> Generator[Self, None, None]: ...  # pragma: no cover
+
+    @overload
+    def __add__(
+        self: Self,
+        other: Union[int, timedelta, Iterable[Union[int, timedelta]]],
+    ) -> Union[Self, Generator[Self, None, None]]: ...  # pragma: no cover
 
     @abstractmethod
     def __add__(
-        self: Self, other: Union[int, timedelta, Iterable[Union[int, timedelta]]]
+        self: Self,
+        other: Union[int, timedelta, Iterable[Union[int, timedelta]]],
     ) -> Union[Self, Generator[Self, None, None]]:  # pragma: no cover
         """Implementation of addition operator."""
         ...
 
     @overload
-    def __sub__(self: Self, other: Union[int, timedelta]) -> Self:  # pragma: no cover
-        """Annotation for subtraction with `int` and `timedelta`"""
-        ...
+    def __sub__(self: Self, other: Union[int, timedelta]) -> Self: ...  # pragma: no cover
 
     @overload
-    def __sub__(self: Self, other: Self) -> int:  # pragma: no cover
-        """Annotation for subtraction with other `BaseIsoWeek`"""
-        ...
+    def __sub__(self: Self, other: Self) -> int: ...  # pragma: no cover
 
     @overload
-    def __sub__(self: Self, other: Iterable[Union[int, timedelta]]) -> Generator[Self, None, None]:  # pragma: no cover
-        """Annotation for subtraction with other `BaseIsoWeek`"""
-        ...
+    def __sub__(
+        self: Self,
+        other: Iterable[Union[int, timedelta]],
+    ) -> Generator[Self, None, None]: ...  # pragma: no cover
 
     @overload
-    def __sub__(self: Self, other: Iterable[Self]) -> Generator[int, None, None]:  # pragma: no cover
-        """Annotation for subtraction with other `Self`"""
-        ...
+    def __sub__(self: Self, other: Iterable[Self]) -> Generator[int, None, None]: ...  # pragma: no cover
+
+    @overload
+    def __sub__(
+        self: Self,
+        other: Union[int, timedelta, Self, Iterable[Union[int, timedelta, Self]]],
+    ) -> Union[int, Self, Generator[Union[int, Self], None, None]]: ...  # pragma: no cover
 
     @abstractmethod
     def __sub__(
-        self: Self, other: Union[int, timedelta, Self, Iterable[Union[int, timedelta, Self]]]
+        self: Self,
+        other: Union[int, timedelta, Self, Iterable[Union[int, timedelta, Self]]],
     ) -> Union[int, Self, Generator[Union[int, Self], None, None]]:  # pragma: no cover
         """Implementation of subtraction operator."""
         ...
 
     def __next__(self: Self) -> Self:
         """Implementation of next operator."""
         return self + 1
 
+    @overload
     @classmethod
     def range(
         cls: Type[Self],
         start: BaseIsoWeek_T,
         end: BaseIsoWeek_T,
+        *,
+        step: int = 1,
+        inclusive: Literal["both", "left", "right", "neither"] = "both",
+        as_str: Literal[True],
+    ) -> Generator[str, None, None]: ...  # pragma: no cover
+
+    @overload
+    @classmethod
+    def range(
+        cls: Type[Self],
+        start: BaseIsoWeek_T,
+        end: BaseIsoWeek_T,
+        *,
+        step: int = 1,
+        inclusive: Literal["both", "left", "right", "neither"] = "both",
+        as_str: Literal[False],
+    ) -> Generator[Self, None, None]: ...  # pragma: no cover
+
+    @overload
+    @classmethod
+    def range(
+        cls: Type[Self],
+        start: BaseIsoWeek_T,
+        end: BaseIsoWeek_T,
+        *,
+        step: int = 1,
+        inclusive: Literal["both", "left", "right", "neither"] = "both",
+        as_str: bool = True,
+    ) -> Generator[Union[str, Self], None, None]: ...  # pragma: no cover
+
+    @classmethod
+    def range(
+        cls: Type[Self],
+        start: BaseIsoWeek_T,
+        end: BaseIsoWeek_T,
+        *,
         step: int = 1,
         inclusive: Literal["both", "left", "right", "neither"] = "both",
         as_str: bool = True,
     ) -> Generator[Union[str, Self], None, None]:
         """Generates `BaseIsoWeek` (or `str`) between `start` and `end` values with given `step`.
 
         `inclusive` parameter can be used to control inclusion of `start` and/or `end` week values.
@@ -243,29 +289,32 @@
             step=2,
             inclusive="both",
             as_str=True)
             )
         # ('2023-W01', '2023-W03', '2023-W05', '2023-W07')
         ```
         """
-
         _start = cls._cast(start)
         _end = cls._cast(end)
 
         if _start > _end:
-            raise ValueError(f"`start` must be before `end` value, found: {_start} > {_end}")
+            msg = f"`start` must be before `end` value, found: {_start} > {_end}"
+            raise ValueError(msg)
 
         if not isinstance(step, int):
-            raise TypeError(f"`step` must be integer, found {type(step)}")
+            msg = f"`step` must be integer, found {type(step)}"
+            raise TypeError(msg)
 
         if step < 1:
-            raise ValueError(f"`step` value must be greater than or equal to 1, found {step}")
+            msg = f"`step` value must be greater than or equal to 1, found {step}"
+            raise ValueError(msg)
 
         if inclusive not in _inclusive_values:
-            raise ValueError(f"Invalid `inclusive` value. Must be one of {_inclusive_values}")
+            msg = f"Invalid `inclusive` value. Must be one of {_inclusive_values}"
+            raise ValueError(msg)
 
         _delta = _end - _start
         range_start = 0 if inclusive in ("both", "left") else 1
         range_end = _delta + 1 if inclusive in ("both", "right") else _delta
 
         weeks_range: Generator[Union[str, Self], None, None] = (
             (_start + i).to_string() if as_str else _start + i for i in range(range_start, range_end, step)
```

### Comparing `iso_week_date-1.2.0/iso_week_date/isoweek.py` & `iso_week_date-1.3.0/iso_week_date/isoweek.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 from __future__ import annotations
 
 import sys
 from datetime import date, datetime, timedelta
-from typing import Any, Generator, Iterable, Tuple, TypeVar, Union, overload
+from typing import Any, Generator, Iterable, Literal, Tuple, TypeVar, Union, overload
 
 from iso_week_date._patterns import ISOWEEK__DATE_FORMAT, ISOWEEK__FORMAT, ISOWEEK_PATTERN
 from iso_week_date.base import BaseIsoWeek
 
-if sys.version_info >= (3, 11):
-    from typing import Self  # pragma: no cover
-else:
-    from typing_extensions import Self  # pragma: no cover
-
-if sys.version_info >= (3, 12):
-    from typing import override  # pragma: no cover
-else:
-    from typing_extensions import override  # pragma: no cover
+if sys.version_info >= (3, 11):  # pragma: no cover
+    from typing import Self
+else:  # pragma: no cover
+    from typing_extensions import Self
 
 IsoWeek_T = TypeVar("IsoWeek_T", date, datetime, str, "IsoWeek")
 
 
 class IsoWeek(BaseIsoWeek):
-    """Represents [ISO Week date](https://en.wikipedia.org/wiki/ISO_week_date) in the  _YYYY-WNN_ format and implements
-    methods to work directly with it instead of going back and forth between `date`, `datetime` and `str` objects.
+    """Represents [ISO Week date](https://en.wikipedia.org/wiki/ISO_week_date) in the  _YYYY-WNN_ format.
+
+    The class implements methods and functionalities to work directly with iso week format and avoid moving back and
+    forth between `date`, `datetime` and `str` objects.
 
     Attributes:
         value_: iso-week string of format "YYYY-WNN" where:
 
             - YYYY is between 0001 and 9999
             - W is a literal character
             - NN is between 01 and 53
@@ -47,16 +44,15 @@
 
         IsoWeek("2023-W01").days  # (date(2023, 1, 2), ..., date(2023, 1, 8))
         ```
         """
         return tuple(self.to_date(weekday) for weekday in range(1, 8))
 
     def nth(self: Self, n: int) -> date:
-        """Returns Nth day of the week using the ISO week weekday numbering convention
-        (1=First day, 2=Second day, ..., 7=Last day).
+        """Returns Nth day of the week using the ISO weekday numbering convention (1=First, 2=Second, ..., 7=Last day).
 
         !!! info
             Weekday is not the same as the day of the week. The weekday is an integer between 1 and 7.
 
         Arguments:
             n: Day number between 1 and 7.
 
@@ -71,24 +67,24 @@
         ```py
         from iso_week_date import IsoWeek
 
         IsoWeek("2023-W01").nth(1)  # date(2023, 1, 2)
         IsoWeek("2023-W01").nth(7)  # date(2023, 1, 8)
         ```
         """
-
         if not isinstance(n, int):
-            raise TypeError(f"`n` must be an integer, found {type(n)}")
+            msg = f"`n` must be an integer, found {type(n)}"
+            raise TypeError(msg)
         if n not in range(1, 8):
-            raise ValueError(f"`n` must be between 1 and 7, found {n}")
+            msg = f"`n` must be between 1 and 7, found {n}"
+            raise ValueError(msg)
 
         return self.days[n - 1]
 
-    @override
-    def to_datetime(self: Self, weekday: int = 1) -> datetime:  # type: ignore[override]
+    def to_datetime(self: Self, weekday: int = 1) -> datetime:
         """Converts `IsoWeek` to `datetime` object with the given weekday.
 
         If no weekday is provided then the first day of the week is used.
 
         !!! info
             Weekday is not the same as the day of the week. The weekday is an integer between 1 and 7.
 
@@ -107,24 +103,24 @@
         ```py
         from iso_week_date import IsoWeek
 
         IsoWeek("2023-W01").to_datetime()  # datetime.datetime(2023, 1, 2, 0, 0)
         IsoWeek("2023-W01").to_datetime(3)  # datetime.datetime(2023, 1, 4, 0, 0)
         ```
         """
-
         if not isinstance(weekday, int):
-            raise TypeError(f"`weekday` must be an integer between 1 and 7, found {type(weekday)}")
+            msg = f"`weekday` must be an integer between 1 and 7, found {type(weekday)}"
+            raise TypeError(msg)
         if weekday not in range(1, 8):
-            raise ValueError(f"Invalid `weekday`. Weekday must be between 1 and 7, found {weekday}")
+            msg = f"Invalid `weekday`. Weekday must be between 1 and 7, found {weekday}"
+            raise ValueError(msg)
 
-        return super().to_datetime(f"{self.value_}-{weekday}")
+        return super()._to_datetime(f"{self.value_}-{weekday}")
 
-    @override
-    def to_date(self: Self, weekday: int = 1) -> date:  # type: ignore[override]
+    def to_date(self: Self, weekday: int = 1) -> date:
         """Converts `IsoWeek` to `date` object with the given `weekday`.
 
         If no weekday is provided then the first day of the week is used.
 
         !!! info
             Weekday is not the same as the day of the week. The weekday is an integer between 1 and 7.
 
@@ -146,27 +142,35 @@
         IsoWeek("2023-W01").to_date()  # datetime.date(2023, 1, 2)
         IsoWeek("2023-W01").to_date(3)  # datetime.date(2023, 1, 4)
         ```
         """
         return self.to_datetime(weekday).date()
 
     @overload
-    def __add__(self: Self, other: Union[int, timedelta]) -> Self:  # pragma: no cover
-        """Implementation of addition operator."""
-        ...
+    def __add__(self: Self, other: Union[int, timedelta]) -> Self: ...  # pragma: no cover
 
     @overload
-    def __add__(self: Self, other: Iterable[Union[int, timedelta]]) -> Generator[Self, None, None]:  # pragma: no cover
-        """Implementation of addition operator."""
-        ...
+    def __add__(
+        self: Self,
+        other: Iterable[Union[int, timedelta]],
+    ) -> Generator[Self, None, None]: ...  # pragma: no cover
 
+    @overload
     def __add__(
-        self: Self, other: Union[int, timedelta, Iterable[Union[int, timedelta]]]
+        self: Self,
+        other: Union[int, timedelta, Iterable[Union[int, timedelta]]],
+    ) -> Union[Self, Generator[Self, None, None]]: ...  # pragma: no cover
+
+    def __add__(
+        self: Self,
+        other: Union[int, timedelta, Iterable[Union[int, timedelta]]],
     ) -> Union[Self, Generator[Self, None, None]]:
-        """It supports addition with the following types:
+        """Addition operation.
+
+        It supports addition with the following types:
 
         - `int`: interpreted as number of weeks to be added to the `IsoWeek` value.
         - `timedelta`: converts `IsoWeek` to datetime (first day of week), adds `timedelta` and converts back to
             `IsoWeek` object.
         - `Iterable` of `int` and/or `timedelta`: adds each element of the iterable to the `IsoWeek` value and returns
             a generator of `IsoWeek` objects.
 
@@ -187,50 +191,55 @@
         IsoWeek("2023-W01") + 1  # IsoWeek("2023-W02")
         IsoWeek("2023-W01") + timedelta(weeks=2)  # IsoWeek("2023-W03")
         IsoWeek("2023-W01") + timedelta(hours=1234) # IsoWeek("2023-W08")
 
         tuple(IsoWeek("2023-W01") + (1,2,3)) # (IsoWeek("2023-W02"), IsoWeek("2023-W03"), IsoWeek("2023-W04"))
         ```
         """
-
         if isinstance(other, int):
             return self.from_date(self.to_date() + timedelta(weeks=other))
         elif isinstance(other, timedelta):
             return self.from_datetime(self.to_datetime() + other)
         elif isinstance(other, Iterable) and all(isinstance(_other, (int, timedelta)) for _other in other):
             return (self + _other for _other in other)
         else:
-            raise TypeError(
-                f"Cannot add type {type(other)} to `IsoWeek`. " "Addition is supported with `int` and `timedelta` types"
+            msg = (
+                f"Cannot add type {type(other)} to `IsoWeek`. "
+                "Addition is supported with `int` and `timedelta` types",
             )
+            raise TypeError(msg)
 
     @overload
-    def __sub__(self: Self, other: Union[int, timedelta]) -> Self:  # pragma: no cover
-        """Annotation for subtraction with `int` and `timedelta`"""
-        ...
+    def __sub__(self: Self, other: Union[int, timedelta]) -> Self: ...  # pragma: no cover
 
     @overload
-    def __sub__(self: Self, other: Self) -> int:  # pragma: no cover
-        """Annotation for subtraction with other `BaseIsoWeek`"""
-        ...
+    def __sub__(self: Self, other: Self) -> int: ...  # pragma: no cover
 
     @overload
-    def __sub__(self: Self, other: Iterable[Union[int, timedelta]]) -> Generator[Self, None, None]:  # pragma: no cover
-        """Annotation for subtraction with other `BaseIsoWeek`"""
-        ...
+    def __sub__(
+        self: Self,
+        other: Iterable[Union[int, timedelta]],
+    ) -> Generator[Self, None, None]: ...  # pragma: no cover
 
     @overload
-    def __sub__(self: Self, other: Iterable[Self]) -> Generator[int, None, None]:  # pragma: no cover
-        """Annotation for subtraction with other `Self`"""
-        ...
+    def __sub__(self: Self, other: Iterable[Self]) -> Generator[int, None, None]: ...  # pragma: no cover
 
+    @overload
     def __sub__(
-        self: Self, other: Union[int, timedelta, Self, Iterable[Union[int, timedelta, Self]]]
+        self: Self,
+        other: Union[int, timedelta, Self, Iterable[Union[int, timedelta, Self]]],
+    ) -> Union[int, Self, Generator[Union[int, Self], None, None]]: ...  # pragma: no cover
+
+    def __sub__(
+        self: Self,
+        other: Union[int, timedelta, Self, Iterable[Union[int, timedelta, Self]]],
     ) -> Union[int, Self, Generator[Union[int, Self], None, None]]:
-        """It supports subtraction with the following types:
+        """Subtraction operation.
+
+        It supports subtraction with the following types:
 
         - `int`: interpreted as number of weeks to be subtracted to the `IsoWeek` value.
         - `timedelta`: converts `IsoWeek` to datetime (first day of week), subtract `timedelta` and converts back to
             `IsoWeek` object.
         - `IsoWeek`: will result in the difference between values in weeks (`int` type).
         - `Iterable` of `int`, `timedelta` and/or `IsoWeek`: subtracts each element of the iterable to the `IsoWeek`.
 
@@ -255,37 +264,64 @@
 
         tuple(IsoWeek("2023-W01") - (1,2,3))  # (IsoWeek("2022-W52"), IsoWeek("2022-W51"), IsoWeek("2022-W50"))
 
         IsoWeek("2023-W01") - IsoWeek("2022-W52")  # 1
         IsoWeek("2023-W01") - IsoWeek("2022-W51")  # 2
         ```
         """
-
         if isinstance(other, int):
             return self.from_date(self.to_date() - timedelta(weeks=other))
         if isinstance(other, timedelta):
             return self.from_datetime(self.to_datetime() - other)
         elif isinstance(other, IsoWeek) and self.offset_ == other.offset_:
             return (self.to_date() - other.to_date()).days // 7
         elif isinstance(other, Iterable) and all(isinstance(_other, (int, timedelta, IsoWeek)) for _other in other):
             return (self - _other for _other in other)
         else:
-            raise TypeError(
+            msg = (
                 f"Cannot subtract type {type(other)} to `IsoWeek`. "
                 "Subtraction is supported with `int`, `timedelta` and `IsoWeek` types"
             )
+            raise TypeError(msg)
+
+    @overload
+    def weeksout(
+        self: Self,
+        n_weeks: int,
+        *,
+        step: int = 1,
+        as_str: Literal[True],
+    ) -> Generator[str, None, None]: ...  # pragma: no cover
+
+    @overload
+    def weeksout(
+        self: Self,
+        n_weeks: int,
+        *,
+        step: int = 1,
+        as_str: Literal[False],
+    ) -> Generator[IsoWeek, None, None]: ...  # pragma: no cover
 
+    @overload
     def weeksout(
         self: Self,
         n_weeks: int,
+        *,
+        step: int = 1,
+        as_str: bool = True,
+    ) -> Generator[Union[str, IsoWeek], None, None]: ...  # pragma: no cover
+
+    def weeksout(
+        self: Self,
+        n_weeks: int,
+        *,
         step: int = 1,
         as_str: bool = True,
     ) -> Generator[Union[str, IsoWeek], None, None]:
-        """Generates range of `IsoWeek`s (or `str`s) from one week to `n_weeks` ahead of current `value`, with given
-        `step`.
+        """Generate range of `IsoWeek` (or `str`) from one to `n_weeks` ahead of current `value`, with given `step`.
 
         If `as_str` is flagged as `True`, it will return `str` values, otherwise it will return `IsoWeek` objects.
 
         Arguments:
             n_weeks: Number of weeks to be generated from current value.
             step: Step between weeks, must be positive integer.
             as_str: Whether to return str or IsoWeek object.
@@ -303,23 +339,25 @@
         iso = IsoWeek("2023-W01")
 
         tuple(iso.weeksout(4)) # ('2023-W02', '2023-W03', '2023-W04', '2023-W05')
         tuple(iso.weeksout(6, step=2))  # ('2023-W02', '2023-W04', '2023-W06')
         ```
         """
         if not isinstance(n_weeks, int):
-            raise TypeError(f"`n_weeks` must be an integer, found {type(n_weeks)} type")
+            msg = f"`n_weeks` must be an integer, found {type(n_weeks)} type"
+            raise TypeError(msg)
 
         if n_weeks <= 0:
-            raise ValueError(f"`n_weeks` must be strictly positive, found {n_weeks}")
+            msg = f"`n_weeks` must be strictly positive, found {n_weeks}"
+            raise ValueError(msg)
 
         start, end = (self + 1), (self + n_weeks)
-        return self.range(start, end, step, inclusive="both", as_str=as_str)
+        return self.range(start, end, step=step, inclusive="both", as_str=as_str)
 
-    def __contains__(self: Self, other: Any) -> bool:
+    def __contains__(self: Self, other: Any) -> bool:  # noqa: ANN401
         """Checks if self contains `other`.
 
         Arguments:
             other: `IsoWeek`, `date`, `datetime` or `str`.
 
         Returns:
             `True` if self week contains other, `False` otherwise.
@@ -336,28 +374,32 @@
         date(2023, 1, 2) in IsoWeek("2023-W01")  # True
         ```
         """
         if isinstance(other, (date, datetime, str, IsoWeek)):
             _other = self._cast(other)
             return self.__eq__(_other)
         else:
-            raise TypeError(f"Cannot compare type `{type(other)}` with IsoWeek")
+            msg = f"Cannot compare type `{type(other)}` with IsoWeek"
+            raise TypeError(msg)
 
     @overload
-    def contains(self: Self, other: IsoWeek_T) -> bool:  # pragma: no cover
-        """Annotation for `contains` method on `IsoWeek` possible types."""
-        ...
+    def contains(self: Self, other: IsoWeek_T) -> bool: ...  # pragma: no cover
 
     @overload
-    def contains(self: Self, other: Iterable[IsoWeek_T]) -> Tuple[bool]:  # pragma: no cover
-        """Annotation for `contains` method on `Iterator` of `IsoWeek` possible types."""
-        ...
+    def contains(self: Self, other: Iterable[IsoWeek_T]) -> Tuple[bool]: ...  # pragma: no cover
+
+    @overload
+    def contains(
+        self: Self,
+        other: Union[Any, Iterable[Any]],  # noqa: ANN401
+    ) -> Union[bool, Tuple[bool, ...]]: ...  # pragma: no cover
 
     def contains(self: Self, other: Union[Any, Iterable[Any]]) -> Union[bool, Tuple[bool, ...]]:
         """Checks if self contains `other`. `other` can be a single value or an iterable of values.
+
         In case of an iterable, the method returns a tuple of boolean values.
 
         Arguments:
             other: `IsoWeek`, `date`, `datetime` or `str`, or an iterable of those types.
 
         Returns:
             Boolean or iterable of booleans, where each boolean indicates whether self contains the corresponding value
@@ -376,8 +418,9 @@
         ```
         """
         if isinstance(other, (date, datetime, str, IsoWeek)):
             return other in self
         elif isinstance(other, Iterable):
             return tuple(_other in self for _other in other)
         else:
-            raise TypeError(f"Cannot compare type `{type(other)}` with `IsoWeek`")
+            msg = f"Cannot compare type `{type(other)}` with `IsoWeek`"
+            raise TypeError(msg)
```

### Comparing `iso_week_date-1.2.0/iso_week_date/isoweekdate.py` & `iso_week_date-1.3.0/iso_week_date/isoweekdate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 from __future__ import annotations
 
 import sys
 from datetime import date, datetime, timedelta
-from typing import Generator, Iterable, TypeVar, Union, overload
+from typing import Generator, Iterable, Literal, TypeVar, Union, overload
 
 from iso_week_date._patterns import ISOWEEKDATE__DATE_FORMAT, ISOWEEKDATE__FORMAT, ISOWEEKDATE_PATTERN
 from iso_week_date.base import BaseIsoWeek
 
-if sys.version_info >= (3, 11):
-    from typing import Self  # pragma: no cover
-else:
-    from typing_extensions import Self  # pragma: no cover
-
-if sys.version_info >= (3, 12):
-    from typing import override  # pragma: no cover
-else:
-    from typing_extensions import override  # pragma: no cover
+if sys.version_info >= (3, 11):  # pragma: no cover
+    from typing import Self
+else:  # pragma: no cover
+    from typing_extensions import Self
 
 IsoWeekDate_T = TypeVar("IsoWeekDate_T", date, datetime, str, "IsoWeekDate")
 
 
 class IsoWeekDate(BaseIsoWeek):
-    """Represents [ISO Week date](https://en.wikipedia.org/wiki/ISO_week_date) in the  _"YYYY-WNN-D"_ format and
-    implements methods to work directly with it instead of going back and forth between `date`, `datetime` and `str`
-    objects.
+    """Represents [ISO Week date](https://en.wikipedia.org/wiki/ISO_week_date) in the  _"YYYY-WNN-D"_ format.
+
+    The class implements methods and functionalities to work directly with iso week date format and avoid moving back
+    and forth between `date`, `datetime` and `str` objects.
 
     Attributes:
         value_: iso-week string of format "YYYY-WNN-D" where:
 
             - YYYY is between 0001 and 9999
             - W is a literal character
             - NN is between 01 and 53
@@ -67,34 +63,31 @@
         from iso_week_date import IsoWeekDate
 
         IsoWeekDate("2023-W01-1").isoweek  # "2023-W01"
         ```
         """
         return self.value_[:8]
 
-    @override
-    def to_datetime(self: Self) -> datetime:  # type: ignore[override]
+    def to_datetime(self: Self) -> datetime:
         """Converts `IsoWeekDate` to `datetime` object.
 
         Returns:
             `datetime` corresponding to the `IsoWeekDate`.
 
         Examples:
         ```py
         from iso_week_date import IsoWeekDate
 
         IsoWeekDate("2023-W01-1").to_datetime()  # datetime.datetime(2023, 1, 2, 0, 0)
         IsoWeekDate("2023-W01-3").to_datetime()  # datetime.datetime(2023, 1, 4, 0, 0)
         ```
         """
+        return super()._to_datetime(self.value_)
 
-        return super().to_datetime(self.value_)
-
-    @override
-    def to_date(self: Self) -> date:  # type: ignore[override]
+    def to_date(self: Self) -> date:
         """Converts `IsoWeekDate` to `date` object.
 
         Returns:
             `date` corresponding to the `IsoWeekDate`.
 
         Examples:
         ```py
@@ -103,27 +96,35 @@
         IsoWeekDate("2023-W01-1").to_date()  # datetime.date(2023, 1, 2)
         IsoWeekDate("2023-W01-3").to_date()  # datetime.date(2023, 1, 4)
         ```
         """
         return self.to_datetime().date()
 
     @overload
-    def __add__(self: Self, other: Union[int, timedelta]) -> Self:  # pragma: no cover
-        """Implementation of addition operator."""
-        ...
+    def __add__(self: Self, other: Union[int, timedelta]) -> Self: ...  # pragma: no cover
+
+    @overload
+    def __add__(
+        self: Self,
+        other: Iterable[Union[int, timedelta]],
+    ) -> Generator[Self, None, None]: ...  # pragma: no cover
 
     @overload
-    def __add__(self: Self, other: Iterable[Union[int, timedelta]]) -> Generator[Self, None, None]:  # pragma: no cover
-        """Implementation of addition operator."""
-        ...
+    def __add__(
+        self: Self,
+        other: Union[int, timedelta, Iterable[Union[int, timedelta]]],
+    ) -> Union[Self, Generator[Self, None, None]]: ...  # pragma: no cover
 
     def __add__(
-        self: Self, other: Union[int, timedelta, Iterable[Union[int, timedelta]]]
+        self: Self,
+        other: Union[int, timedelta, Iterable[Union[int, timedelta]]],
     ) -> Union[Self, Generator[Self, None, None]]:
-        """It supports addition with the following types:
+        """Addition operation.
+
+        It supports addition with the following types:
 
         - `int`: interpreted as number of days to be added to the `IsoWeekDate` value.
         - `timedelta`: converts `IsoWeekDate` to `datetime`, adds `timedelta` and converts back to `IsoWeekDate` object.
         - `Iterable` of `int` and/or `timedelta`: adds each element of the iterable to the `IsoWeekDate` value and
             returns a generator of `IsoWeekDate` objects.
 
         Arguments:
@@ -142,51 +143,55 @@
 
         IsoWeekDate("2023-W01-1") + 1  # IsoWeekDate("2023-W01-2")
         IsoWeekDate("2023-W01-1") + timedelta(weeks=2)  # IsoWeekDate("2023-W03-1")
 
         tuple(IsoWeekDate("2023-W01-1") + (1,2)) # (IsoWeekDate("2023-W01-2"), IsoWeekDate("2023-W01-3"))
         ```
         """
-
         if isinstance(other, int):
             return self.from_date(self.to_date() + timedelta(days=other))
         elif isinstance(other, timedelta):
             return self.from_datetime(self.to_datetime() + other)
         elif isinstance(other, Iterable) and all(isinstance(_other, (int, timedelta)) for _other in other):
             return (self + _other for _other in other)
         else:
-            raise TypeError(
+            msg = (
                 f"Cannot add type {type(other)} to `IsoWeekDate`. "
-                "Addition is supported with `int` and `timedelta` types"
+                "Addition is supported with `int` and `timedelta` types",
             )
+            raise TypeError(msg)
+
+    @overload
+    def __sub__(self: Self, other: Union[int, timedelta]) -> Self: ...  # pragma: no cover
 
     @overload
-    def __sub__(self: Self, other: Union[int, timedelta]) -> Self:  # pragma: no cover
-        """Annotation for subtraction with `int` and `timedelta`"""
-        ...
+    def __sub__(self: Self, other: Self) -> int: ...  # pragma: no cover
 
     @overload
-    def __sub__(self: Self, other: Self) -> int:  # pragma: no cover
-        """Annotation for subtraction with other `BaseIsoWeek`"""
-        ...
+    def __sub__(
+        self: Self,
+        other: Iterable[Union[int, timedelta]],
+    ) -> Generator[Self, None, None]: ...  # pragma: no cover
 
     @overload
-    def __sub__(self: Self, other: Iterable[Union[int, timedelta]]) -> Generator[Self, None, None]:  # pragma: no cover
-        """Annotation for subtraction with other `BaseIsoWeek`"""
-        ...
+    def __sub__(self: Self, other: Iterable[Self]) -> Generator[int, None, None]: ...  # pragma: no cover
 
     @overload
-    def __sub__(self: Self, other: Iterable[Self]) -> Generator[int, None, None]:  # pragma: no cover
-        """Annotation for subtraction with other `Self`"""
-        ...
+    def __sub__(
+        self: Self,
+        other: Union[int, timedelta, Self, Iterable[Union[int, timedelta, Self]]],
+    ) -> Union[int, Self, Generator[Union[int, Self], None, None]]: ...  # pragma: no cover
 
     def __sub__(
-        self: Self, other: Union[int, timedelta, Self, Iterable[Union[int, timedelta, Self]]]
+        self: Self,
+        other: Union[int, timedelta, Self, Iterable[Union[int, timedelta, Self]]],
     ) -> Union[int, Self, Generator[Union[int, Self], None, None]]:
-        """It supports subtraction with the following types:
+        """Subtraction operation.
+
+        It supports subtraction with the following types:
 
         - `int`: interpreted as number of days to be subtracted to the `IsoWeekDate` value.
         - `timedelta`: converts `IsoWeekDate` to `datetime`, subtracts `timedelta` and converts back to `IsoWeekDate`
             object.
         - `IsoWeekDate`: will result in the difference between values in days (`int` type).
         - `Iterable` of `int`, `timedelta` and/or `IsoWeekDate`: subtracts each element of the iterable to the
             `IsoWeekDate`.
@@ -212,37 +217,64 @@
 
         tuple(IsoWeekDate("2023-W01-1") - (1,2))  # (IsoWeekDate("2022-W52-7"), IsoWeekDate("2022-W52-6"))
 
         IsoWeekDate("2023-W01-1") - IsoWeekDate("2022-W52-3")  # 5
 
         ```
         """
-
         if isinstance(other, int):
             return self.from_date(self.to_date() - timedelta(days=other))
         if isinstance(other, timedelta):
             return self.from_datetime(self.to_datetime() - other)
         elif isinstance(other, IsoWeekDate) and self.offset_ == other.offset_:
             return (self.to_date() - other.to_date()).days
         elif isinstance(other, Iterable) and all(isinstance(_other, (int, timedelta, IsoWeekDate)) for _other in other):
             return (self - _other for _other in other)
         else:
-            raise TypeError(
+            msg = (
                 f"Cannot subtract type {type(other)} to `IsoWeekDate`. "
-                "Subtraction is supported with `int`, `timedelta` and `IsoWeekDate` types"
+                "Subtraction is supported with `int`, `timedelta` and `IsoWeekDate` types",
             )
+            raise TypeError(msg)
+
+    @overload
+    def daysout(
+        self: Self,
+        n_days: int,
+        *,
+        step: int = 1,
+        as_str: Literal[True],
+    ) -> Generator[str, None, None]: ...  # pragma: no cover
+
+    @overload
+    def daysout(
+        self: Self,
+        n_days: int,
+        *,
+        step: int = 1,
+        as_str: Literal[False],
+    ) -> Generator[IsoWeekDate, None, None]: ...  # pragma: no cover
+
+    @overload
+    def daysout(
+        self: Self,
+        n_days: int,
+        *,
+        step: int = 1,
+        as_str: bool = True,
+    ) -> Generator[Union[str, IsoWeekDate], None, None]: ...  # pragma: no cover
 
     def daysout(
         self: Self,
         n_days: int,
+        *,
         step: int = 1,
         as_str: bool = True,
     ) -> Generator[Union[str, IsoWeekDate], None, None]:
-        """Generates range of `IsoWeekDate`s (or `str`s) from one day to `n_days` ahead of current `value`, with given
-        `step`.
+        """Generate range of `IsoWeekDate` (or `str`) from one to `n_days` ahead of current `value`, with given `step`.
 
         If `as_str` is flagged as `True`, it will return `str` values, otherwise it will return `IsoWeekDate` objects.
 
         Arguments:
             n_days: Number of days to be generated from current value.
             step: Step between days, must be positive integer.
             as_str: Whether to return `str` or `IsoWeekDate` object.
@@ -260,14 +292,16 @@
         iso = IsoWeekDate("2023-W01-1")
 
         tuple(iso.daysout(3)) # ('2023-W01-2', '2023-W01-3', '2023-W01-4')
         tuple(iso.daysout(6, step=2)) # ('2023-W01-2', '2023-W01-4', '2023-W01-6')
         ```
         """
         if not isinstance(n_days, int):
-            raise TypeError(f"`n_weeks` must be integer, found {type(n_days)} type")
+            msg = f"`n_weeks` must be integer, found {type(n_days)} type"
+            raise TypeError(msg)
 
         if n_days <= 0:
-            raise ValueError(f"`n_weeks` must be strictly positive, found {n_days}")
+            msg = f"`n_weeks` must be strictly positive, found {n_days}"
+            raise ValueError(msg)
 
         start, end = (self + 1), (self + n_days)
-        return self.range(start, end, step, inclusive="both", as_str=as_str)
+        return self.range(start, end, step=step, inclusive="both", as_str=as_str)
```

### Comparing `iso_week_date-1.2.0/iso_week_date/mixin.py` & `iso_week_date-1.3.0/iso_week_date/mixin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,115 +1,123 @@
 from __future__ import annotations
 
-import re
 import sys
 from datetime import date, datetime, timedelta
-from typing import Any, ClassVar, Protocol, Tuple, Type, TypeVar, Union, runtime_checkable
+from typing import TYPE_CHECKING, ClassVar, Protocol, Tuple, Type, TypeVar, Union, runtime_checkable
 
 from iso_week_date._utils import classproperty, format_err_msg
 
-if sys.version_info >= (3, 11):
-    from typing import Self  # pragma: no cover
-else:
-    from typing_extensions import Self  # pragma: no cover
+if sys.version_info >= (3, 11):  # pragma: no cover
+    from typing import Self
+else:  # pragma: no cover
+    from typing_extensions import Self
+
+if TYPE_CHECKING:  # pragma: no cover
+    import re
 
 
 @runtime_checkable
 class IsoWeekProtocol(Protocol):  # pragma: no cover
     """Protocol for `BaseIsoWeek`."""
 
     value_: str
     _pattern: ClassVar[re.Pattern]
 
     _format: ClassVar[str]
     _date_format: ClassVar[str]
 
     offset_: ClassVar[timedelta] = timedelta(days=0)
 
-    def __init__(self, value: str) -> None:
-        """init takes a string value which will be validated."""
+    def __init__(self: Self, value: str) -> None:
+        """Init takes a string value which will be validated."""
         ...
 
     @property
     def name(self: Self) -> str:
-        """property that returns the class name."""
+        """Property that returns the class name."""
         ...
 
     @classmethod
     def _validate(cls: Type[IsoWeekProtocol], value: str) -> str:
-        """classmethod that validates the string passed as input."""
+        """Classmethod that validates the string passed as input."""
         ...
 
     @classproperty
-    def _compact_pattern(cls: Type[IsoWeekProtocol]) -> re.Pattern:
-        """classproperty that returns the compiled compact pattern."""
+    def _compact_pattern(cls: Type[IsoWeekProtocol]) -> re.Pattern:  # noqa: N805
+        """Classproperty that returns the compiled compact pattern."""
         ...
 
     @classproperty
-    def _compact_format(cls: Type[IsoWeekProtocol]) -> str:
-        """classproperty that returns the compact format as string."""
+    def _compact_format(cls: Type[IsoWeekProtocol]) -> str:  # noqa: N805
+        """Classproperty that returns the compact format as string."""
         ...
 
 
-IsoWeek_T = TypeVar("IsoWeek_T", bound=Union[str, date, datetime, IsoWeekProtocol], contravariant=True)
+IsoWeek_T_contra = TypeVar("IsoWeek_T_contra", bound=Union[str, date, datetime, IsoWeekProtocol], contravariant=True)
 
 
 class ParserMixin(IsoWeekProtocol):
-    """Mixin that implements `from_*` class methods to parse from:
+    """Mixin that handles conversion from types.
+
+    `ParserMixin` implements `from_*` (class) methods to parse from:
 
     - `str`: string matching `pattern`, will be validated.
     - `str`: string matching `compact_pattern`, will be validated.
     - `date`: casted to ISO Week `_date_format` using `.strftime()` method after applying `offset_`.
     - `datetime`:casted to ISO Week `_date_format` using `.strftime()` method after applying `offset_`.
 
     Additionally, it implements `._cast()` class method that automatically casts to ISOWeek-like type from the by
     calling the appropriate method for parsing.
     """
 
     @classmethod
     def from_string(cls: Type[Self], _str: str) -> Self:
         """Parse a string object in `_pattern` format."""
         if not isinstance(_str, str):
-            raise TypeError(f"Expected `str` type, found {type(_str)}.")
+            msg = f"Expected `str` type, found {type(_str)}"
+            raise TypeError(msg)
         return cls(_str)
 
     @classmethod
     def from_compact(cls: Type[Self], _str: str) -> Self:
-        """Parse a string object in `_compact_format` format. Since values are validated in the initialization method,
-        our goal in this method is to "add" the dashes in the appropriate places.
+        """Parse a string object in `_compact_format` format.
 
-        To achieve this we:
+        Since values are validated in the initialization method, our goal in this method is to "add" the dashes in the
+        appropriate places. To achieve this we:
 
         - First check that the length of the string is correct (either 7 or 8).
         - Split the string in 3 parts.
         - Remove (filter) empty values.
         - Finally join them with a dash in between.
         """
         if not isinstance(_str, str):
-            raise TypeError(f"Expected `str` type, found {type(_str)}.")
+            msg = f"Expected `str` type, found {type(_str)}"
+            raise TypeError(msg)
 
         if len(_str) != len(cls._compact_format):
             raise ValueError(format_err_msg(cls._compact_format, _str))
 
         split_idx = (0, 4, 7, None)
         value = "-".join(filter(None, (_str[i:j] for i, j in zip(split_idx[:-1], split_idx[1:]))))
         return cls(value)
 
     @classmethod
     def from_date(cls: Type[Self], _date: date) -> Self:
         """Parse a date object to `_date_format` after adjusting by `offset_`."""
         if not isinstance(_date, date):
-            raise TypeError(f"Expected `date` type, found {type(_date)}.")
+            msg = f"Expected `date` type, found {type(_date)}"
+            raise TypeError(msg)
         return cls((_date - cls.offset_).strftime(cls._date_format))
 
     @classmethod
     def from_datetime(cls: Type[Self], _datetime: datetime) -> Self:
         """Parse a datetime object to `_date_format` after adjusting by `offset_`."""
         if not isinstance(_datetime, datetime):
-            raise TypeError(f"Expected `datetime` type, found {type(_datetime)}.")
+            msg = f"Expected `datetime` type, found {type(_datetime)}"
+            raise TypeError(msg)
 
         return cls((_datetime - cls.offset_).strftime(cls._date_format))
 
     @classmethod
     def from_today(cls: Type[Self]) -> Self:  # pragma: no cover
         """Instantiates class from today's date."""
         return cls.from_date(date.today())
@@ -121,16 +129,16 @@
             cls._format.replace("YYYY", str(year).zfill(4))
             .replace("NN", str(week).zfill(2))
             .replace("D", str(weekday).zfill(1))
         )
         return cls(value)
 
     @classmethod
-    def _cast(cls: Type[Self], value: IsoWeek_T) -> Self:
-        """Automatically casts to ISOWeek-like type from the following possible types:
+    def _cast(cls: Type[Self], value: IsoWeek_T_contra) -> Self:
+        """Tries to cast from different types.
 
         - `str`: string matching `_pattern`.
         - `date`: casted to ISO Week by calling `.from_date()` method.
         - `datetime`: casted to ISO Week by calling `.from_datetime()` method.
         - `ISOWeek`-like: value will be returned as is.
 
         Arguments:
@@ -155,65 +163,67 @@
         elif isinstance(value, datetime):
             return cls.from_datetime(value)
         elif isinstance(value, date):
             return cls.from_date(value)
         elif isinstance(value, cls):
             return value
         else:
-            raise NotImplementedError(f"Cannot cast type {type(value)} into {cls.__name__}")
+            msg = f"Cannot cast type {type(value)} into {cls.__name__}"
+            raise NotImplementedError(msg)
 
 
 class ConverterMixin(IsoWeekProtocol):
-    """Mixin that implements `to_*` instance methods to convert to the following types:
+    """Mixin that handles conversion to types.
+
+    `ConverterMixin` implements `to_*` methods to convert to the following types:
 
     - `str`
     - `date`
     - `datetime`
     """
 
     def to_string(self: Self) -> str:
         """Returns as a string in the classical format."""
         return self.value_
 
     def to_compact(self: Self) -> str:
         """Returns as a string in the compact format."""
         return self.value_.replace("-", "")
 
-    def to_datetime(self: Self, value: str) -> datetime:
+    def _to_datetime(self: Self, value: str) -> datetime:
         """Converts `value` to `datetime` object and adds the `offset_`.
 
         !!! warning
             `value` must be in "%G-W%V-%u" format.
 
             In general this is not always the case and we need to manipulate `value_` attribute before passing it to
             `datetime.strptime` method.
         """
         return datetime.strptime(value, "%G-W%V-%u") + self.offset_
 
-    def to_date(self: Self, value: str) -> date:  # pragma: no cover
-        """
-        Converts `value` to `date` object and adds the `offset_`.
+    def _to_date(self: Self, value: str) -> date:  # pragma: no cover
+        """Converts `value` to `date` object and adds the `offset_`.
 
         !!! warning
             `value` must be in "%G-W%V-%u" format.
 
             In general this is not always the case and we need to manipulate `value_` attribute before passing it to
             `datetime.strptime` method.
         """
-        return self.to_datetime(value).date()  # type: ignore
+        return self._to_datetime(value).date()
 
     def to_values(self: Self) -> Tuple[int, ...]:
         """Converts `value_` to a tuple of integers (year, week, [weekday])."""
         return tuple(int(v.replace("W", "")) for v in self.value_.split("-"))
 
 
 class ComparatorMixin(IsoWeekProtocol):
     """Mixin that implements comparison operators ("==", "!=", "<", "<=", ">", ">=") between two ISO Week objects."""
 
-    def __eq__(self: Self, other: Any) -> bool:
+    def __eq__(self: Self, other: object) -> bool:
         """Equality operator.
 
         Two ISO Week objects are considered equal if and only if they have the same `offset_` and the same `value_`.
 
         Arguments:
             other: Object to compare with.
 
@@ -235,15 +245,15 @@
         ```
         """
         if isinstance(other, self.__class__):
             return (self.offset_ == other.offset_) and (self.value_ == other.value_)
         else:
             return False
 
-    def __ne__(self: Self, other: Any) -> bool:
+    def __ne__(self: Self, other: object) -> bool:
         """Inequality operator.
 
         Two ISO Week objects are considered equal if and only if they have the same `offset_` and the same `value_`.
 
         Arguments:
             other: Object to compare with.
 
@@ -297,20 +307,22 @@
         IsoWeek("2023-W01") < "2023-W01"  # TypeError
         ```
         """
         if isinstance(other, self.__class__):
             if self.offset_ == other.offset_:
                 return self.value_ < other.value_
             else:
-                raise TypeError(f"Cannot compare `{self.name}`'s with different offsets")
+                msg = f"Cannot compare `{self.name}`'s with different offsets"
+                raise TypeError(msg)
         else:
-            raise TypeError(
-                f"Cannot compare `{self.name}` with type `{type(other)}`, "
-                f"comparison is supported only with other `{self.name}` objects"
+            msg = (
+                f"Cannot compare `{self.name}` with type `{type(other)}`, comparison is supported only with other "
+                f"`{self.name}` objects"
             )
+            raise TypeError(msg)
 
     def __le__(self: Self, other: Self) -> bool:
         """Less than or equal operator.
 
         Comparing two ISO Week objects is only possible if they have the same `offset_`.
 
         If that's the case than it's enough to compare their values (as `str`) due to its lexicographical order.
```

### Comparing `iso_week_date-1.2.0/iso_week_date/pandas_utils.py` & `iso_week_date-1.3.0/iso_week_date/pandas_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,47 @@
+from __future__ import annotations
+
 import sys
 from typing import Union
 
 from iso_week_date._patterns import (
     ISOWEEK__DATE_FORMAT,
     ISOWEEK__FORMAT,
     ISOWEEK_PATTERN,
     ISOWEEKDATE__DATE_FORMAT,
     ISOWEEKDATE__FORMAT,
     ISOWEEKDATE_PATTERN,
 )
+from iso_week_date._utils import parse_version
 
-if sys.version_info >= (3, 11):
-    from typing import Self  # pragma: no cover
-else:
-    from typing_extensions import Self  # pragma: no cover
+if sys.version_info >= (3, 10):  # pragma: no cover
+    from typing import TypeAlias
+else:  # pragma: no cover
+    from typing_extensions import TypeAlias
+
+if sys.version_info >= (3, 11):  # pragma: no cover
+    from typing import Self
+else:  # pragma: no cover
+    from typing_extensions import Self
 
-try:
-    import pandas as pd
-    from pandas.api.types import is_datetime64_any_dtype as is_datetime
-except ImportError:  # pragma: no cover
+if parse_version("pandas") < (1, 0, 0):  # pragma: no cover
     raise ImportError(
-        "pandas is required for this module, install it with `python -m pip install pandas`"
-        " or `python -m pip install iso-week-date[pandas]`"
+        "pandas>=1.0.0 is required for this module, install it with `python -m pip install pandas>=1.0.0`"
+        " or `python -m pip install iso-week-date[pandas]`",
     )
+else:  # pragma: no cover
+    import pandas as pd
+    from pandas.api.types import is_datetime64_any_dtype as is_datetime
+
+OffsetType: TypeAlias = Union[int, pd.Timedelta]
 
 
 def _datetime_to_format(
     series: pd.Series,
-    offset: Union[pd.Timedelta, int],
+    offset: OffsetType,
     _format: str,
 ) -> pd.Series:
     """Converts series of `date` or `datetime` values to series of `str` values in `_format` format.
 
     Arguments:
         series: series of `date` or `datetime` values
         offset: offset in days or `pd.Timedelta`. It represents how many days to add to the date before converting to
@@ -44,29 +54,31 @@
     Raises:
         TypeError: If any of the following condition is met:
 
             - `series` is not of type `pd.Series`
             - series values are not `datetime`
             - `offset` is not of type `pd.Timedelta` or `int`
     """
-
     if not isinstance(series, pd.Series):
-        raise TypeError(f"`series` must be of type `pd.Series`, found {type(series)}")
+        msg = f"`series` must be of type `pd.Series`, found {type(series)}"
+        raise TypeError(msg)
 
     if not is_datetime(series):
-        raise TypeError(f"`series` values must be of type `datetime`, found {series.dtype}")
+        msg = f"`series` values must be of type `datetime`, found {series.dtype}"
+        raise TypeError(msg)
 
     if not isinstance(offset, (pd.Timedelta, int)):
-        raise TypeError(f"`offset` must be of type `pd.Timedelta` or `int`, found {type(offset)}")
+        msg = f"`offset` must be of type `pd.Timedelta` or `int`, found {type(offset)}"
+        raise TypeError(msg)
 
     _offset = pd.Timedelta(days=offset) if isinstance(offset, int) else offset
     return (series - _offset).dt.strftime(_format)
 
 
-def datetime_to_isoweek(series: pd.Series, offset: Union[pd.Timedelta, int] = pd.Timedelta(days=0)) -> pd.Series:
+def datetime_to_isoweek(series: pd.Series, offset: OffsetType = 0) -> pd.Series:
     """Converts series of `date` or `datetime` values to `str` values representing ISO Week format YYYY-WNN.
 
     Arguments:
         series: series of `date` or `datetime` values
         offset: offset in days or `pd.Timedelta`. It represents how many days to add to the date before converting to
             ISO Week, it can be negative
 
@@ -87,19 +99,18 @@
     from iso_week_date.pandas_utils import datetime_to_isoweek
 
     s = pd.Series(pd.date_range(date(2023, 1, 1), date(2023, 1, 10), freq="1d"))
     datetime_to_isoweek(series=s, offset=pd.Timedelta(days=1)).to_list()
     # ['2022-W52', '2022-W52', '2023-W01',..., '2023-W01', '2023-W02']
     ```
     """
-
     return _datetime_to_format(series, offset, ISOWEEK__DATE_FORMAT)
 
 
-def datetime_to_isoweekdate(series: pd.Series, offset: Union[pd.Timedelta, int] = pd.Timedelta(days=0)) -> pd.Series:
+def datetime_to_isoweekdate(series: pd.Series, offset: OffsetType = 0) -> pd.Series:
     """Converts series of `date` or `datetime` values to `str` values representing ISO Week date format YYYY-WNN-D.
 
     Arguments:
         series: series of `date` or `datetime` values
         offset: offset in days or `pd.Timedelta`. It represents how many days to add to the date before converting to
             ISO Week, it can be negative
 
@@ -120,21 +131,20 @@
     from iso_week_date.pandas_utils import datetime_to_isoweekdate
 
     s = pd.Series(pd.date_range(date(2023, 1, 1), date(2023, 1, 10), freq="1d"))
     datetime_to_isoweekdate(series=s, offset=pd.Timedelta(days=1)).to_list()
     # ['2022-W52-6', '2022-W52-7', '2023-W01-1',..., '2023-W01-7', '2023-W02-1']
     ```
     """
-
     return _datetime_to_format(series, offset, ISOWEEKDATE__DATE_FORMAT)
 
 
 def isoweek_to_datetime(
     series: pd.Series,
-    offset: Union[pd.Timedelta, int] = pd.Timedelta(days=0),
+    offset: OffsetType = 0,
     weekday: int = 1,
 ) -> pd.Series:
     """Converts series of `str` values in ISO Week format to a series of `datetime` values.
 
     `offset` represents how many days to add to the date before converting to datetime and it can be negative.
 
     `weekday` represents the weekday to use for conversion in ISO Week format (1-7), where 1 is the first day of the
@@ -169,29 +179,32 @@
     1   2023-01-03
     2   2023-01-10
     dtype: datetime64[ns]
     '''
     ```
     """
     if not is_isoweek_series(series):
-        raise ValueError(f"`series` values must match ISO Week date format {ISOWEEK__FORMAT}")
+        msg = f"`series` values must match ISO Week date format {ISOWEEK__FORMAT}"
+        raise ValueError(msg)
 
     if not isinstance(offset, (pd.Timedelta, int)):
-        raise TypeError(f"`offset` must be of type `pd.Timedelta` or `int`, found {type(offset)}")
+        msg = f"`offset` must be of type `pd.Timedelta` or `int`, found {type(offset)}"
+        raise TypeError(msg)
 
     if weekday not in range(1, 8):
-        raise ValueError(f"`weekday` value must be an integer between 1 and 7, found {weekday}")
+        msg = f"`weekday` value must be an integer between 1 and 7, found {weekday}"
+        raise ValueError(msg)
 
     _offset = pd.Timedelta(days=offset) if isinstance(offset, int) else offset
     return pd.to_datetime(series + "-" + f"{weekday}", format=ISOWEEKDATE__DATE_FORMAT) + _offset
 
 
 def isoweekdate_to_datetime(
     series: pd.Series,
-    offset: Union[pd.Timedelta, int] = pd.Timedelta(days=0),
+    offset: OffsetType = 0,
 ) -> pd.Series:
     """Converts series of `str` values in ISO Week date format to a series of `datetime` values.
 
     `offset` represents how many days to add to the date before converting to datetime and it can be negative.
 
     Arguments:
         series: series of `str` in ISO Week date format
@@ -219,18 +232,20 @@
     1   2023-01-03
     2   2023-01-10
     dtype: datetime64[ns]
     '''
     ```
     """
     if not is_isoweekdate_series(series):
-        raise ValueError(f"`series` values must match ISO Week date format {ISOWEEKDATE__FORMAT}")
+        msg = f"`series` values must match ISO Week date format {ISOWEEKDATE__FORMAT}"
+        raise ValueError(msg)
 
     if not isinstance(offset, (pd.Timedelta, int)):
-        raise TypeError(f"`offset` must be of type `pd.Timedelta` or `int`, found {type(offset)}")
+        msg = f"`offset` must be of type `pd.Timedelta` or `int`, found {type(offset)}"
+        raise TypeError(msg)
 
     _offset = pd.Timedelta(days=offset) if isinstance(offset, int) else offset
     return pd.to_datetime(series, format=ISOWEEKDATE__DATE_FORMAT) + _offset
 
 
 def _match_series(series: pd.Series, pattern: str) -> bool:
     """Checks if a `series` contains only values matching `pattern`.
@@ -242,15 +257,16 @@
     Returns:
         `True` if all values match `pattern`, `False` otherwise
 
     Raises:
         TypeError: If `series` is not of type `pd.Series`
     """
     if not isinstance(series, pd.Series):
-        raise TypeError(f"`series` must be of type `pd.Series`, found {type(series)}")
+        msg = f"`series` must be of type `pd.Series`, found {type(series)}"
+        raise TypeError(msg)
 
     try:
         return series.str.match(pattern).all()
     except AttributeError:
         return False
 
 
@@ -326,18 +342,18 @@
     Parameters:
         series: The pandas Series object the extension is attached to.
 
     Attributes:
         _series: The pandas Series object the extension is attached to.
     """
 
-    def __init__(self: Self, series: pd.Series):
+    def __init__(self: Self, series: pd.Series) -> None:
         self._series: pd.Series = series
 
-    def datetime_to_isoweek(self: Self, offset: Union[pd.Timedelta, int] = pd.Timedelta(0)) -> pd.Series:
+    def datetime_to_isoweek(self: Self, offset: OffsetType = 0) -> pd.Series:
         """Converts series of `date` or `datetime` values to `str` values representing ISO Week format YYYY-WNN.
 
         Arguments:
             offset: offset in days or `pd.Timedelta`. It represents how many days to add to the date before converting
                 to ISO Week, it can be negative
 
         Returns:
@@ -355,15 +371,15 @@
         s = pd.Series(pd.date_range(date(2023, 1, 1), date(2023, 1, 10), freq="1d"))
         s.iwd.datetime_to_isoweek(offset=pd.Timedelta(days=1)).to_list()
         # ['2022-W52', '2022-W52', '2023-W01',..., '2023-W01', '2023-W02']
         ```
         """
         return datetime_to_isoweek(self._series, offset=offset)
 
-    def datetime_to_isoweekdate(self: Self, offset: Union[pd.Timedelta, int] = pd.Timedelta(0)) -> pd.Series:
+    def datetime_to_isoweekdate(self: Self, offset: OffsetType = 0) -> pd.Series:
         """Converts series of `date` or `datetime` values to `str` values representing ISO Week date format YYYY-WNN-D.
 
         Arguments:
             offset: offset in days or `pd.Timedelta`. It represents how many days to add to the date before converting
                 to ISO Week, it can be negative
 
         Returns:
@@ -382,15 +398,17 @@
         s.iwd.datetime_to_isoweekdate(offset=pd.Timedelta(days=1)).to_list()
         # ['2022-W52-6', '2022-W52-7', '2023-W01-1',..., '2023-W01-7', '2023-W02-1']
         ```
         """
         return datetime_to_isoweekdate(self._series, offset=offset)
 
     def isoweek_to_datetime(
-        self: Self, offset: Union[pd.Timedelta, int] = pd.Timedelta(0), weekday: int = 1
+        self: Self,
+        offset: OffsetType = 0,
+        weekday: int = 1,
     ) -> pd.Series:
         """Converts series of `str` values in ISO Week format to a series of `datetime` values.
 
         `offset` represents how many days to add to the date before converting to datetime and it can be negative.
 
         `weekday` represents the weekday to use for conversion in ISO Week format (1-7), where 1 is the first day of the
         week, 7 is the last one.
@@ -420,15 +438,15 @@
         2   2023-01-10
         dtype: datetime64[ns]
         '''
         ```
         """
         return isoweek_to_datetime(self._series, offset=offset, weekday=weekday)
 
-    def isoweekdate_to_datetime(self: Self, offset: Union[pd.Timedelta, int] = pd.Timedelta(0)) -> pd.Series:
+    def isoweekdate_to_datetime(self: Self, offset: OffsetType = 0) -> pd.Series:
         """Converts series of `str` values in ISO Week date format to a series of `datetime` values.
 
         `offset` represents how many days to add to the date before converting to datetime and it can be negative.
 
         Arguments:
             offset: offset in days or pd.Timedelta. It represents how many days to add to the date before converting to
                 IsoWeek, it can be negative
```

### Comparing `iso_week_date-1.2.0/iso_week_date/polars_utils.py` & `iso_week_date-1.3.0/iso_week_date/polars_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,48 @@
+from __future__ import annotations
+
 import sys
 from datetime import timedelta
 from typing import Generic, TypeVar, Union
 
 from iso_week_date._patterns import (
     ISOWEEK__DATE_FORMAT,
     ISOWEEK__FORMAT,
     ISOWEEK_PATTERN,
     ISOWEEKDATE__DATE_FORMAT,
     ISOWEEKDATE__FORMAT,
     ISOWEEKDATE_PATTERN,
 )
+from iso_week_date._utils import parse_version
 
-if sys.version_info >= (3, 11):
-    from typing import Self  # pragma: no cover
-else:
-    from typing_extensions import Self  # pragma: no cover
+if sys.version_info >= (3, 10):  # pragma: no cover
+    from typing import TypeAlias
+else:  # pragma: no cover
+    from typing_extensions import TypeAlias
+
+if sys.version_info >= (3, 11):  # pragma: no cover
+    from typing import Self
+else:  # pragma: no cover
+    from typing_extensions import Self
 
-try:
-    import polars as pl
-except ImportError:  # pragma: no cover
+if parse_version("polars") < (0, 18, 0):  # pragma: no cover
     raise ImportError(
         "polars>=0.18.0 is required for this module, install it with `python -m pip install polars>=0.18.0` "
-        "or `python -m pip install iso-week-date[polars]`"
+        "or `python -m pip install iso-week-date[polars]`",
     )
+else:  # pragma: no cover
+    import polars as pl
 
 T = TypeVar("T", pl.Series, pl.Expr)
+OffsetType: TypeAlias = Union[int, timedelta]
 
 
 def _datetime_to_format(
     series: T,
-    offset: Union[timedelta, int],
+    offset: OffsetType,
     _format: str,
 ) -> T:
     """Converts series or expr of `date` or `datetime` values to series or expr of `str` values in `_format` format.
 
     Arguments:
         series: series or expr of `date` or `datetime` values
         offset: offset in days or `timedelta`. It represents how many days to add to the date before converting to ISO
@@ -46,26 +55,27 @@
     Raises:
         TypeError: If any of the following condition is met:
 
             - `series` is not of type `pl.Series` or `pl.Expr`
             - `offset` is not of type `timedelta` or `int`
     """
     if not isinstance(series, (pl.Series, pl.Expr)):
-        raise TypeError(f"`series` must be of type `pl.Series` or `pl.Expr`, found {type(series)}")
+        msg = f"`series` must be of type `pl.Series` or `pl.Expr`, found {type(series)}"
+        raise TypeError(msg)
 
     if not isinstance(offset, (timedelta, int)):
-        raise TypeError(f"`offset` must be of type `timedelta` or `int`, found {type(offset)}")
+        msg = f"`offset` must be of type `timedelta` or `int`, found {type(offset)}"
+        raise TypeError(msg)
 
     _offset = timedelta(days=offset) if isinstance(offset, int) else offset
     return (series - _offset).dt.strftime(_format)
 
 
-def datetime_to_isoweek(series: T, offset: Union[timedelta, int] = timedelta(days=0)) -> T:
-    """Converts `series` or `expr` of with `date` or `datetime` values to `str` values representing ISO Week format
-    YYYY-WNN.
+def datetime_to_isoweek(series: T, offset: OffsetType = timedelta(days=0)) -> T:
+    """Converts `date(time)` `series/expr` to `str` values representing ISO Week format YYYY-WNN.
 
     Arguments:
         series: series or expr of `date` or `datetime` values
         offset: offset in days or `timedelta`. It represents how many days to add to the date before converting to ISO
             Week, it can be negative
 
     Returns:
@@ -87,21 +97,19 @@
     s = pl.date_range(date(2023, 1, 1), date(2023, 1, 10), interval="1d")
     datetime_to_isoweek(s, offset=timedelta(days=1))
 
     df = pl.DataFrame({"date": s})
     df.select(datetime_to_isoweek(pl.col("date"), offset=1))
     ```
     """
-
     return _datetime_to_format(series, offset, ISOWEEK__DATE_FORMAT)
 
 
-def datetime_to_isoweekdate(series: T, offset: Union[timedelta, int] = timedelta(days=0)) -> T:
-    """Converts `series` or `expr` of with `date` or `datetime` values to `str` values representing ISO Week date
-    format YYYY-WNN-D.
+def datetime_to_isoweekdate(series: T, offset: OffsetType = timedelta(days=0)) -> T:
+    """Converts `date(time)` `series/expr`  to `str` values representing ISO Week date format YYYY-WNN-D.
 
     Arguments:
         series: series or expr of `date` or `datetime` values
         offset: offset in days or `timedelta`. It represents how many days to add to the date before converting to ISO
             Week, it can be negative
 
     Returns:
@@ -123,21 +131,20 @@
     s = pl.date_range(date(2023, 1, 1), date(2023, 1, 10), interval="1d")
     datetime_to_isoweekdate(s, offset=timedelta(days=1))
 
     df = pl.DataFrame({"date": s})
     df.select(datetime_to_isoweekdate(pl.col("date"), offset=1))
     ```
     """
-
     return _datetime_to_format(series, offset, ISOWEEKDATE__DATE_FORMAT)
 
 
 def isoweek_to_datetime(
     series: T,
-    offset: Union[timedelta, int] = timedelta(days=0),
+    offset: OffsetType = timedelta(days=0),
     weekday: int = 1,
 ) -> T:
     """Converts series or expr of `str` values in ISO Week format YYYY-WNN to a series or expr of `pl.Date` values.
 
     `offset` represents how many days to add to the date before converting to `pl.Date`, and it can be negative.
 
     `weekday` represents the weekday to use for conversion in ISO Week format (1-7), where 1 is the first day of the
@@ -173,32 +180,35 @@
     2022-12-27
     2023-01-03
     2023-01-10
     '''
     ```
     """
     if not is_isoweek_series(series):
-        raise ValueError(f"`series` values must match ISO Week format {ISOWEEK__FORMAT}")
+        msg = f"`series` values must match ISO Week format {ISOWEEK__FORMAT}"
+        raise ValueError(msg)
 
     if not isinstance(offset, (timedelta, int)):
-        raise TypeError(f"`offset` must be of type `timedelta` or `int`, found {type(offset)}")
+        msg = f"`offset` must be of type `timedelta` or `int`, found {type(offset)}"
+        raise TypeError(msg)
 
     if weekday not in range(1, 8):
-        raise ValueError(f"`weekday` value must be an integer between 1 and 7, found {weekday}")
+        msg = f"`weekday` value must be an integer between 1 and 7, found {weekday}"
+        raise ValueError(msg)
 
     _offset = timedelta(days=offset) if isinstance(offset, int) else offset
 
     return (series + f"-{weekday}").str.strptime(pl.Date, ISOWEEKDATE__DATE_FORMAT) + _offset
 
 
 def isoweekdate_to_datetime(
     series: T,
-    offset: Union[timedelta, int] = timedelta(days=0),
+    offset: OffsetType = timedelta(days=0),
 ) -> T:
-    """Converts series or expr of `str` values in ISO Week date format YYYY-WNN-D to a series or expr of `pl.Date` values.
+    """Converts `series/expr` of values in ISO Week date format YYYY-WNN-D to a series or expr of `pl.Date` values.
 
     `offset` represents how many days to add to the date before converting to `pl.Date`, and it can be negative.
 
     Arguments:
         series: series or expr of `str` values in ISO Week date format
         offset: offset in days or `timedelta`. It represents how many days to add to the date before converting to
             IsoWeek, it can be negative
@@ -225,20 +235,21 @@
     date
     2022-01-02
     2023-01-03
     2023-01-10
     '''
     ```
     """
-
     if not is_isoweekdate_series(series):
-        raise ValueError(f"`series` values must match ISO Week date format {ISOWEEKDATE__FORMAT}")
+        msg = f"`series` values must match ISO Week date format {ISOWEEKDATE__FORMAT}"
+        raise ValueError(msg)
 
     if not isinstance(offset, (timedelta, int)):
-        raise TypeError(f"`offset` must be of type `timedelta` or `int`, found {type(offset)}")
+        msg = f"`offset` must be of type `timedelta` or `int`, found {type(offset)}"
+        raise TypeError(msg)
 
     _offset = timedelta(days=offset) if isinstance(offset, int) else offset
 
     return series.str.strptime(pl.Date, ISOWEEKDATE__DATE_FORMAT) + _offset
 
 
 def _match_series(series: T, pattern: str) -> bool:
@@ -250,21 +261,21 @@
 
     Returns:
         `True` if all values match `pattern`, `False` otherwise
 
     Raises:
         TypeError: If `series` is not of type `pl.Series` or `pl.Expr`
     """
-
     if not isinstance(series, (pl.Series, pl.Expr)):
-        raise TypeError(f"`series` must be of type `pl.Series` or `pl.Expr`, found {type(series)}")
+        msg = f"`series` must be of type `pl.Series` or `pl.Expr`, found {type(series)}"
+        raise TypeError(msg)
 
     try:
-        return series.str.extract(pattern).is_not_null().all()  # type: ignore
-    except Exception:
+        return series.str.extract(pattern).is_not_null().all()  # type: ignore[return-value]
+    except Exception:  # noqa: BLE001
         return False
 
 
 def is_isoweek_series(series: T) -> bool:
     """Checks if a series or expr contains only values in ISO Week format.
 
     Arguments:
@@ -337,20 +348,19 @@
     Parameters:
         series: The pandas Series object the extension is attached to.
 
     Attributes:
         _series: The pandas Series object the extension is attached to.
     """
 
-    def __init__(self: Self, series: T):
+    def __init__(self: Self, series: T) -> None:
         self._series: T = series
 
-    def datetime_to_isoweek(self: Self, offset: Union[timedelta, int] = timedelta(0)) -> T:
-        """Converts `series` or `expr` of with `date` or `datetime` values to `str` values representing ISO Week format
-        YYYY-WNN.
+    def datetime_to_isoweek(self: Self, offset: OffsetType = timedelta(0)) -> T:
+        """Converts `date(time)` `series/expr` to `str` values representing ISO Week format YYYY-WNN.
 
         Arguments:
             offset: offset in days or `timedelta`. It represents how many days to add to the date before converting to
                 ISO Week, it can be negative
 
         Returns:
             Series or Expr with converted ISO Week values (in format YYYY-WNN)
@@ -370,17 +380,16 @@
 
         df = pl.DataFrame({"date": s})
         df.select(pl.col("date").iwd.datetime_to_isoweek(offset=1))
         ```
         """
         return datetime_to_isoweek(self._series, offset=offset)
 
-    def datetime_to_isoweekdate(self: Self, offset: Union[timedelta, int] = timedelta(0)) -> T:
-        """Converts `series` or `expr` of with `date` or `datetime` values to `str` values representing ISO Week date
-        format YYYY-WNN-D.
+    def datetime_to_isoweekdate(self: Self, offset: OffsetType = timedelta(0)) -> T:
+        """Converts `date(time)` `series/expr` to `str` values representing ISO Week date format YYYY-WNN-D.
 
         Arguments:
             offset: offset in days or `timedelta`. It represents how many days to add to the date before converting to
                 ISO Week, it can be negative
 
         Returns:
             Series or Expr with converted ISO Week values (in format YYYY-WNN-D)
@@ -400,15 +409,15 @@
 
         df = pl.DataFrame({"date": s})
         df.select(pl.col("date").iwd.datetime_to_isoweekdate(offset=1))
         ```
         """
         return datetime_to_isoweekdate(self._series, offset=offset)
 
-    def isoweek_to_datetime(self: Self, offset: Union[timedelta, int] = timedelta(0), weekday: int = 1) -> T:
+    def isoweek_to_datetime(self: Self, offset: OffsetType = timedelta(0), weekday: int = 1) -> T:
         """Converts series or expr of `str` values in ISO Week format YYYY-WNN to a series or expr of `pl.Date` values.
 
         `offset` represents how many days to add to the date before converting to `pl.Date`, and it can be negative.
 
         `weekday` represents the weekday to use for conversion in ISO Week format (1-7), where 1 is the first day of the
         week, 7 is the last one.
 
@@ -439,17 +448,16 @@
         2023-01-03
         2023-01-10
         '''
         ```
         """
         return isoweek_to_datetime(self._series, offset=offset, weekday=weekday)
 
-    def isoweekdate_to_datetime(self: Self, offset: Union[timedelta, int] = timedelta(0)) -> T:
-        """Converts series or expr of `str` values in ISO Week date format YYYY-WNN-D to a series or expr of `pl.Date`
-        values.
+    def isoweekdate_to_datetime(self: Self, offset: OffsetType = timedelta(0)) -> T:
+        """Converts `str` series or expr of ISO Week date format YYYY-WNN-D to a series or expr of `pl.Date` values.
 
         `offset` represents how many days to add to the date before converting to `pl.Date`, and it can be negative.
 
         Arguments:
             offset: offset in days or `timedelta`. It represents how many days to add to the date before converting to
                 IsoWeek, it can be negative
```

### Comparing `iso_week_date-1.2.0/iso_week_date/pydantic.py` & `iso_week_date-1.3.0/iso_week_date/pydantic.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 from __future__ import annotations
 
 import re
-from typing import Any
+import sys
+from typing import TYPE_CHECKING, Any, Type
 
 from iso_week_date._patterns import ISOWEEK_PATTERN, ISOWEEKDATE_PATTERN
-from iso_week_date._utils import weeks_of_year
+from iso_week_date._utils import parse_version, weeks_of_year
 
-try:
-    from pydantic import GetCoreSchemaHandler
-    from pydantic_core import PydanticCustomError, core_schema
-except ImportError:  # pragma: no cover
+if sys.version_info >= (3, 11):  # pragma: no cover
+    from typing import Self
+else:  # pragma: no cover
+    from typing_extensions import Self
+
+if parse_version("pydantic") < (2, 4, 0):  # pragma: no cover
     raise ImportError(
         "pydantic>=2.4.0 is required for this module, install it with `python -m pip install pydantic>=2.4.0`"
-        " or `python -m pip install iso-week-date[pydantic]`"
+        " or `python -m pip install iso-week-date[pydantic]`",
     )
+else:  # pragma: no cover
+    from pydantic_core import PydanticCustomError, core_schema
 
+    if TYPE_CHECKING:
+        from pydantic import GetCoreSchemaHandler
 
-class T_ISOWeek(str):
+
+class T_ISOWeek(str):  # noqa: N801
     """T_ISOWeek parses iso week in the [ISO 8601](https://en.wikipedia.org/wiki/ISO_week_date) format.
 
     !!! info "New in version 1.2.0"
 
     Examples:
     ```py
     from pydantic import BaseModel
@@ -39,55 +47,58 @@
     #   Invalid week number. Year 2024 has only 52 weeks. [type=T_ISOWeek, input_value='2024-W53', input_type=str]
 
     _ = Model(isoweek="abc")
     # ValidationError: 1 validation error for Model
     # isoweek
     #   Invalid iso week pattern [type=T_ISOWeek, input_value='abc', input_type=str]
     ```
-
     """
 
+    __slots__ = ()
+
     @classmethod
     def __get_pydantic_core_schema__(
-        cls: type[T_ISOWeek], source: type[Any], handler: GetCoreSchemaHandler
+        cls: Type[Self],
+        source: Type[Any],
+        handler: GetCoreSchemaHandler,
     ) -> core_schema.CoreSchema:
-        """
-        Return a Pydantic CoreSchema with the IsoWeek pattern validation.
+        """Return a Pydantic CoreSchema with the IsoWeek pattern validation.
 
         Arguments:
             source: The source type to be converted.
             handler: The handler to get the CoreSchema.
 
         Returns:
             A Pydantic CoreSchema with the IsoWeek pattern validation.
         """
         return core_schema.with_info_before_validator_function(
             cls._validate,
             core_schema.str_schema(),
         )
 
     @classmethod
-    def _validate(cls, __input_value: str, _: core_schema.ValidationInfo) -> T_ISOWeek:
+    def _validate(cls: Type[Self], __input_value: str, _: core_schema.ValidationInfo) -> Self:
         """Validates iso week string format against ISOWEEK_PATTERN."""
         _match = re.match(ISOWEEK_PATTERN, __input_value)
 
         if not _match:
             raise PydanticCustomError("T_ISOWeek", "Invalid iso week pattern")
 
         year, week = int(_match.group(1)), int(_match.group(2)[1:])
 
         if weeks_of_year(year) < week:
             raise PydanticCustomError(
-                "T_ISOWeek", f"Invalid week number. Year {year} has only {weeks_of_year(year)} weeks."
+                "T_ISOWeek",
+                f"Invalid week number. Year {year} has only {weeks_of_year(year)} weeks.",
             )
 
         return cls(__input_value)
 
 
-class T_ISOWeekDate(str):
+class T_ISOWeekDate(str):  # noqa: N801
     """T_ISOWeekDate parses iso week date in the [ISO 8601](https://en.wikipedia.org/wiki/ISO_week_date) format.
 
     !!! info "New in version 1.2.0"
 
     Examples:
     ```py
     from pydantic import BaseModel
@@ -99,29 +110,33 @@
     model = Model(isoweekdate="2024-W01-1")
     print(model)
     # isoweekdate='2024-W01-1'
 
     _ = Model(isoweekdate="2024-W53-1")
     # ValidationError: 1 validation error for Model
     # isoweekdate
-    #   Invalid week number. Year 2024 has only 52 weeks. [type=type=T_ISOWeekDate, input_value='2024-W53-1', input_type=str]
+    #   Invalid week number. Year 2024 has only 52 weeks.
+    #   [type=type=T_ISOWeekDate, input_value='2024-W53-1', input_type=str]
 
     _ = Model(isoweekdate="abc")
     # ValidationError: 1 validation error for Model
     # isoweekdate
     #   Invalid iso week pattern [type=type=T_ISOWeekDate, input_value='abc', input_type=str]
     ```
     """
 
+    __slots__ = ()
+
     @classmethod
     def __get_pydantic_core_schema__(
-        cls: type[T_ISOWeekDate], source: type[Any], handler: GetCoreSchemaHandler
+        cls: Type[Self],
+        source: Type[Any],
+        handler: GetCoreSchemaHandler,
     ) -> core_schema.CoreSchema:
-        """
-        Return a Pydantic CoreSchema with the IsoWeekDate pattern validation.
+        """Return a Pydantic CoreSchema with the IsoWeekDate pattern validation.
 
         Arguments:
             source: The source type to be converted.
             handler: The handler to get the CoreSchema.
 
         Returns:
             A Pydantic CoreSchema with the IsoWeekDate pattern validation.
@@ -129,25 +144,23 @@
         """
         return core_schema.with_info_before_validator_function(
             cls._validate,
             core_schema.str_schema(),
         )
 
     @classmethod
-    def _validate(cls, __input_value: str, _: core_schema.ValidationInfo) -> T_ISOWeekDate:
+    def _validate(cls: Type[Self], __input_value: str, _: core_schema.ValidationInfo) -> Self:
         """Validates iso week date string format against ISOWEEKDATE_PATTERN."""
         _match = re.match(ISOWEEKDATE_PATTERN, __input_value)
 
         if not _match:
             raise PydanticCustomError("T_ISOWeekDate", "Invalid iso week date pattern")
 
-        year, week, day = int(_match.group(1)), int(_match.group(2)[1:]), int(_match.group(3))
+        year, week = int(_match.group(1)), int(_match.group(2)[1:])
 
         if weeks_of_year(year) < week:
             raise PydanticCustomError(
-                "T_ISOWeekDate", f"Invalid week number. Year {year} has only {weeks_of_year(year)} weeks."
+                "T_ISOWeekDate",
+                f"Invalid week number. Year {year} has only {weeks_of_year(year)} weeks.",
             )
 
-        if day not in range(1, 8):
-            raise PydanticCustomError("T_ISOWeekDate", "Invalid day number. Day should be between 1 and 7 (inclusive)")
-
         return cls(__input_value)
```

### Comparing `iso_week_date-1.2.0/.gitignore` & `iso_week_date-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `iso_week_date-1.2.0/LICENSE` & `iso_week_date-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iso_week_date-1.2.0/README.md` & `iso_week_date-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `iso_week_date-1.2.0/pyproject.toml` & `iso_week_date-1.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "iso-week-date"
-version = "1.2.0"
+version = "1.3.0"
 description = "Toolkit to work with str representing ISO Week date format"
 
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [{name = "Francesco Bruzzesi"}]
 
 dependencies = [
-    "typing-extensions>=4.4.0; python_version < '3.12'",
+    "typing-extensions>=4.4.0; python_version < '3.11'",
 ]
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
@@ -31,15 +31,15 @@
 [project.urls]
 repository = "https://github.com/fbruzzesi/iso-week-date"
 issue-tracker = "https://github.com/fbruzzesi/iso-week-date/issues"
 documentation = "https://fbruzzesi.github.io/iso-week-date/"
 
 [project.optional-dependencies]
 pandas = [
-    "pandas",
+    "pandas>=1.0.0",
 ]
 
 polars = [
     "polars>=0.18.0",
 ]
 
 pydantic = [
@@ -76,31 +76,50 @@
 only-include = ["iso_week_date"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["iso_week_date"]
 
 [tool.ruff]
 line-length = 120
+target-version = "py38"
 
 [tool.ruff.lint]
-extend-select = ["I"]
+select = ["ALL"]
 ignore = [
-    "E731",  # do not assign a `lambda` expression, use a `def`
+    "D100",  # Checks for undocumented public module definitions.
+    "D104",  # Checks for undocumented public package definitions.
+    "D107",  # Checks for public __init__ method definitions that are missing docstrings.
+    "E731",  # Checks for lambda expressions which are assigned to a variable.
+    "EM101",  # Checks for the use of string literals in exception constructors.
+    "ISC001",  # Checks for implicitly concatenated strings on a single line.
+    "RET505",  # Checks for else statements with a return statement in the preceding if block.
+    "TRY003",  # Checks for long exception messages that are not defined in the exception class itself.
+    "DTZ"
     ]
 
+[tool.ruff.lint.per-file-ignores]
+"tests/*" = ["ANN", "D", "S101", "PT006", "PT007"]
+
 [tool.ruff.lint.pydocstyle]
 convention = "google"
 
+[tool.ruff.lint.pylint]
+max-args = 6
+
+[tool.ruff.lint.pyupgrade]
+keep-runtime-typing = true
+
 [tool.interrogate]
 ignore-nested-functions = true
 ignore-module = true
 ignore-init-method = true
 ignore-private = true
 ignore-magic = true
 ignore-property-decorators = true
+ignore-overloaded-functions = true
 fail-under = 95
 verbose = 2 # 0 (minimal output), 1 (-v), 2 (-vv)
 
 [tool.mypy]
 ignore_missing_imports = true
 
 [tool.coverage.run]
```

### Comparing `iso_week_date-1.2.0/PKG-INFO` & `iso_week_date-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: iso-week-date
-Version: 1.2.0
+Version: 1.3.0
 Summary: Toolkit to work with str representing ISO Week date format
 Project-URL: repository, https://github.com/fbruzzesi/iso-week-date
 Project-URL: issue-tracker, https://github.com/fbruzzesi/iso-week-date/issues
 Project-URL: documentation, https://fbruzzesi.github.io/iso-week-date/
 Author: Francesco Bruzzesi
 License: MIT License
         
@@ -34,28 +34,28 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: typing-extensions>=4.4.0; python_version < '3.12'
+Requires-Dist: typing-extensions>=4.4.0; python_version < '3.11'
 Provides-Extra: all
-Requires-Dist: pandas; extra == 'all'
+Requires-Dist: pandas>=1.0.0; extra == 'all'
 Requires-Dist: polars>=0.18.0; extra == 'all'
 Requires-Dist: pydantic>=2.4.0; extra == 'all'
 Provides-Extra: all-dev
 Requires-Dist: coverage==7.2.1; extra == 'all-dev'
 Requires-Dist: hatch; extra == 'all-dev'
 Requires-Dist: interrogate>=1.5.0; extra == 'all-dev'
 Requires-Dist: mkdocs-autorefs; extra == 'all-dev'
 Requires-Dist: mkdocs-material>=9.2.0; extra == 'all-dev'
 Requires-Dist: mkdocs>=1.4.2; extra == 'all-dev'
 Requires-Dist: mkdocstrings[python]>=0.20.0; extra == 'all-dev'
-Requires-Dist: pandas; extra == 'all-dev'
+Requires-Dist: pandas>=1.0.0; extra == 'all-dev'
 Requires-Dist: polars>=0.18.0; extra == 'all-dev'
 Requires-Dist: pre-commit==2.21.0; extra == 'all-dev'
 Requires-Dist: pydantic>=2.4.0; extra == 'all-dev'
 Requires-Dist: pytest-xdist==3.2.1; extra == 'all-dev'
 Requires-Dist: pytest==7.2.0; extra == 'all-dev'
 Requires-Dist: ruff>=0.4.0; extra == 'all-dev'
 Provides-Extra: dev
@@ -65,15 +65,15 @@
 Requires-Dist: mkdocs-autorefs; extra == 'docs'
 Requires-Dist: mkdocs-material>=9.2.0; extra == 'docs'
 Requires-Dist: mkdocs>=1.4.2; extra == 'docs'
 Requires-Dist: mkdocstrings[python]>=0.20.0; extra == 'docs'
 Provides-Extra: lint
 Requires-Dist: ruff>=0.4.0; extra == 'lint'
 Provides-Extra: pandas
-Requires-Dist: pandas; extra == 'pandas'
+Requires-Dist: pandas>=1.0.0; extra == 'pandas'
 Provides-Extra: polars
 Requires-Dist: polars>=0.18.0; extra == 'polars'
 Provides-Extra: pydantic
 Requires-Dist: pydantic>=2.4.0; extra == 'pydantic'
 Provides-Extra: test
 Requires-Dist: coverage==7.2.1; extra == 'test'
 Requires-Dist: interrogate>=1.5.0; extra == 'test'
```

