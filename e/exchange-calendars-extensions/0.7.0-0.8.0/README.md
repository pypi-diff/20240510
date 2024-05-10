# Comparing `tmp/exchange_calendars_extensions-0.7.0.tar.gz` & `tmp/exchange_calendars_extensions-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exchange_calendars_extensions-0.7.0.tar", max compression
+gzip compressed data, was "exchange_calendars_extensions-0.8.0.tar", max compression
```

## Comparing `exchange_calendars_extensions-0.7.0.tar` & `exchange_calendars_extensions-0.8.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2024-01-31 15:01:37.300482 exchange_calendars_extensions-0.7.0/LICENSE
--rw-r--r--   0        0        0    25890 2024-01-31 15:01:37.300482 exchange_calendars_extensions-0.7.0/README.md
--rw-r--r--   0        0        0    19725 2024-01-31 15:01:37.300482 exchange_calendars_extensions-0.7.0/exchange_calendars_extensions/core/__init__.py
--rw-r--r--   0        0        0     6785 2024-01-31 15:01:37.300482 exchange_calendars_extensions-0.7.0/exchange_calendars_extensions/core/holiday.py
--rw-r--r--   0        0        0    41212 2024-01-31 15:01:37.300482 exchange_calendars_extensions-0.7.0/exchange_calendars_extensions/core/holiday_calendar.py
--rw-r--r--   0        0        0     5678 2024-01-31 15:01:37.300482 exchange_calendars_extensions-0.7.0/exchange_calendars_extensions/core/offset.py
--rw-r--r--   0        0        0     2595 2024-01-31 15:01:37.300482 exchange_calendars_extensions-0.7.0/exchange_calendars_extensions/core/util.py
--rw-r--r--   0        0        0       18 2024-01-31 15:01:48.896487 exchange_calendars_extensions-0.7.0/exchange_calendars_extensions/core/version.py
--rw-r--r--   0        0        0     2978 2024-01-31 15:01:48.840487 exchange_calendars_extensions-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    27442 1970-01-01 00:00:00.000000 exchange_calendars_extensions-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-10 06:32:21.327228 exchange_calendars_extensions-0.8.0/LICENSE
+-rw-r--r--   0        0        0    25890 2024-05-10 06:32:21.327228 exchange_calendars_extensions-0.8.0/README.md
+-rw-r--r--   0        0        0    25332 2024-05-10 06:32:21.331228 exchange_calendars_extensions-0.8.0/exchange_calendars_extensions/core/__init__.py
+-rw-r--r--   0        0        0     6872 2024-05-10 06:32:21.331228 exchange_calendars_extensions-0.8.0/exchange_calendars_extensions/core/holiday.py
+-rw-r--r--   0        0        0    45563 2024-05-10 06:32:21.331228 exchange_calendars_extensions-0.8.0/exchange_calendars_extensions/core/holiday_calendar.py
+-rw-r--r--   0        0        0     5787 2024-05-10 06:32:21.331228 exchange_calendars_extensions-0.8.0/exchange_calendars_extensions/core/offset.py
+-rw-r--r--   0        0        0     2764 2024-05-10 06:32:21.331228 exchange_calendars_extensions-0.8.0/exchange_calendars_extensions/core/util.py
+-rw-r--r--   0        0        0       18 2024-05-10 06:32:32.371310 exchange_calendars_extensions-0.8.0/exchange_calendars_extensions/core/version.py
+-rw-r--r--   0        0        0     2911 2024-05-10 06:32:32.303310 exchange_calendars_extensions-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0    27388 1970-01-01 00:00:00.000000 exchange_calendars_extensions-0.8.0/PKG-INFO
```

### Comparing `exchange_calendars_extensions-0.7.0/LICENSE` & `exchange_calendars_extensions-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exchange_calendars_extensions-0.7.0/README.md` & `exchange_calendars_extensions-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `exchange_calendars_extensions-0.7.0/exchange_calendars_extensions/core/__init__.py` & `exchange_calendars_extensions-0.8.0/exchange_calendars_extensions/core/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import functools
-import datetime as dt
-from typing import Optional, Callable, Type, Union, Any, Dict
+from typing import Callable, Union
 
-from exchange_calendars import calendar_utils, register_calendar_type, ExchangeCalendar, get_calendar_names
+from exchange_calendars import (
+    calendar_utils,
+    register_calendar_type,
+    ExchangeCalendar,
+    get_calendar_names,
+)
 from exchange_calendars.calendar_utils import _default_calendar_factories
 from exchange_calendars.exchange_calendar_asex import ASEXExchangeCalendar
 from exchange_calendars.exchange_calendar_xams import XAMSExchangeCalendar
 from exchange_calendars.exchange_calendar_xbru import XBRUExchangeCalendar
 from exchange_calendars.exchange_calendar_xbud import XBUDExchangeCalendar
 from exchange_calendars.exchange_calendar_xcse import XCSEExchangeCalendar
 from exchange_calendars.exchange_calendar_xdub import XDUBExchangeCalendar
@@ -24,98 +28,154 @@
 from exchange_calendars.exchange_calendar_xpra import XPRAExchangeCalendar
 from exchange_calendars.exchange_calendar_xsto import XSTOExchangeCalendar
 from exchange_calendars.exchange_calendar_xswx import XSWXExchangeCalendar
 from exchange_calendars.exchange_calendar_xtae import XTAEExchangeCalendar
 from exchange_calendars.exchange_calendar_xtse import XTSEExchangeCalendar
 from exchange_calendars.exchange_calendar_xwar import XWARExchangeCalendar
 from exchange_calendars.exchange_calendar_xwbo import XWBOExchangeCalendar
-from pydantic import validate_call
+from pydantic import validate_call, BaseModel, conint
 from typing_extensions import ParamSpec, Concatenate
 
-from exchange_calendars_extensions.api.changes import ChangeSet, ChangeSetDict, DayType, DaySpec, DaySpecWithTime, TimestampLike
-from exchange_calendars_extensions.core.holiday_calendar import extend_class, ExtendedExchangeCalendar, ExchangeCalendarExtensions
+from exchange_calendars_extensions.api.changes import (
+    ChangeSet,
+    ChangeSetDict,
+    DayType,
+    DateLike,
+    DayPropsLike,
+    Tags,
+    TimeLike,
+    DayMeta,
+)
+from exchange_calendars_extensions.core.holiday_calendar import (
+    extend_class,
+    ExtendedExchangeCalendar,
+    ExchangeCalendarExtensions,
+)
 
 # Dictionary that maps from exchange key to ExchangeCalendarChangeSet. Contains all changesets to apply when creating a
-# new calendar instance.
-_changesets: Dict[str, ChangeSet] = dict()
-
-# Dictionary that maps from exchange key to ExtendedExchangeCalendar. Contains all extended calendars classes that
-# replace the vanilla classes in exchange_calendars when calling apply_extensions().
-#
-# Note: The values in this dictionary use extend_class() to create the extended classes, respectively for each exchange,
-#     based on the respective vanilla class in exchange_calendars. Also, the changeset_provider is set to a lambda
-#     function that returns the changeset for the respective exchange in _changesets, or None, if no changeset exists.
-_extensions = {
-    "ASEX": (ASEXExchangeCalendar, 4),
-    "XAMS": (XAMSExchangeCalendar, 4),
-    "XBRU": (XBRUExchangeCalendar, 4),
-    "XBUD": (XBUDExchangeCalendar, 4),
-    "XCSE": (XCSEExchangeCalendar, 4),
-    "XDUB": (XDUBExchangeCalendar, 4),
-    "XETR": (XETRExchangeCalendar, 4),
-    "XHEL": (XHELExchangeCalendar, 4),
-    "XIST": (XISTExchangeCalendar, 4),
-    "XJSE": (XJSEExchangeCalendar, 3),
-    "XLIS": (XLISExchangeCalendar, 4),
-    "XLON": (XLONExchangeCalendar, 4),
-    "XMAD": (XMADExchangeCalendar, 4),
-    "XMIL": (XMILExchangeCalendar, 4),
-    "XNYS": (XNYSExchangeCalendar, 4),
-    "XOSL": (XOSLExchangeCalendar, 4),
-    "XPAR": (XPARExchangeCalendar, 4),
-    "XPRA": (XPRAExchangeCalendar, 4),
-    "XSTO": (XSTOExchangeCalendar, 4),
-    "XSWX": (XSWXExchangeCalendar, 4),
-    "XTAE": (XTAEExchangeCalendar, 4),
-    "XTSE": (XTSEExchangeCalendar, 4),
-    "XWAR": (XWARExchangeCalendar, 4),
-    "XWBO": (XWBOExchangeCalendar, 4),
+# new calendar instance. This dictionary should only ever contain non-empty changesets. If a changeset becomes empty,
+# the corresponding entry should just be removed.
+_changesets: dict[str, ChangeSet] = dict()
+
+
+class ExtensionSpec(BaseModel, arbitrary_types_allowed=True):
+    """Specifies how to derive an extended calendar class from a vanilla calendar class."""
+
+    # The base class to extend.
+    base: type[ExchangeCalendar]
+
+    # The day of the week on which options expire. If None, expiry days are not supported.
+    day_of_week_expiry: Union[conint(ge=0, le=6), None] = None
+
+
+# Internal dictionary that specifies how to derive extended calendars for specific exchanges.
+_extensions: dict[str, ExtensionSpec] = {
+    "ASEX": ExtensionSpec(base=ASEXExchangeCalendar, day_of_week_expiry=4),
+    "XAMS": ExtensionSpec(base=XAMSExchangeCalendar, day_of_week_expiry=4),
+    "XBRU": ExtensionSpec(base=XBRUExchangeCalendar, day_of_week_expiry=4),
+    "XBUD": ExtensionSpec(base=XBUDExchangeCalendar, day_of_week_expiry=4),
+    "XCSE": ExtensionSpec(base=XCSEExchangeCalendar, day_of_week_expiry=4),
+    "XDUB": ExtensionSpec(base=XDUBExchangeCalendar, day_of_week_expiry=4),
+    "XETR": ExtensionSpec(base=XETRExchangeCalendar, day_of_week_expiry=4),
+    "XHEL": ExtensionSpec(base=XHELExchangeCalendar, day_of_week_expiry=4),
+    "XIST": ExtensionSpec(base=XISTExchangeCalendar, day_of_week_expiry=4),
+    "XJSE": ExtensionSpec(base=XJSEExchangeCalendar, day_of_week_expiry=3),
+    "XLIS": ExtensionSpec(base=XLISExchangeCalendar, day_of_week_expiry=4),
+    "XLON": ExtensionSpec(base=XLONExchangeCalendar, day_of_week_expiry=4),
+    "XMAD": ExtensionSpec(base=XMADExchangeCalendar, day_of_week_expiry=4),
+    "XMIL": ExtensionSpec(base=XMILExchangeCalendar, day_of_week_expiry=4),
+    "XNYS": ExtensionSpec(base=XNYSExchangeCalendar, day_of_week_expiry=4),
+    "XOSL": ExtensionSpec(base=XOSLExchangeCalendar, day_of_week_expiry=4),
+    "XPAR": ExtensionSpec(base=XPARExchangeCalendar, day_of_week_expiry=4),
+    "XPRA": ExtensionSpec(base=XPRAExchangeCalendar, day_of_week_expiry=4),
+    "XSTO": ExtensionSpec(base=XSTOExchangeCalendar, day_of_week_expiry=4),
+    "XSWX": ExtensionSpec(base=XSWXExchangeCalendar, day_of_week_expiry=4),
+    "XTAE": ExtensionSpec(base=XTAEExchangeCalendar, day_of_week_expiry=4),
+    "XTSE": ExtensionSpec(base=XTSEExchangeCalendar, day_of_week_expiry=4),
+    "XWAR": ExtensionSpec(base=XWARExchangeCalendar, day_of_week_expiry=4),
+    "XWBO": ExtensionSpec(base=XWBOExchangeCalendar, day_of_week_expiry=4),
 }
 
 
+# Internal dictionary containing the original calendar classes.
 _original_classes = dict()
 
 
 def apply_extensions() -> None:
     """
     Apply extensions to exchange_calendars.
 
-    This registers all extended calendars in exchange_calendars, overwriting the respective vanilla calendars.
+    This registers all extended calendars in exchange_calendars, replacing the respective vanilla calendars.
+
+    This function is idempotent. If extensions have already been applied, this function does nothing.
     """
     if len(_original_classes) > 0:
         # Extensions have already been applied.
         return
 
+    # Get all calendar names, including aliases.
     calendar_names = set(get_calendar_names())
 
     def get_changeset_fn(name: str) -> Callable[[], ChangeSet]:
+        """Returns a function that returns the changeset for the given exchange key.
+
+        Parameters
+        ----------
+        name : str
+            The exchange key for which to return the changeset.
+
+        Returns
+        -------
+        Callable[[], ChangeSet]
+            The function that returns the changeset.
+        """
+
         def fn() -> ChangeSet:
             return _changesets.get(name)
+
         return fn
 
+    # Create and register extended calendar classes for all calendars for which no explicit rules have been defined.
     for k in calendar_names - set(_extensions.keys()):
+        # Get the original class.
         cls = _default_calendar_factories.get(k)
+
         if cls is not None:
             # Store the original class for later use.
             _original_classes[k] = cls
-            # Create extended class.
-            cls = extend_class(cls, day_of_week_expiry=None, changeset_provider=get_changeset_fn(k))
+
+            # Create extended class without support for expiry days.
+            cls = extend_class(
+                cls, day_of_week_expiry=None, changeset_provider=get_changeset_fn(k)
+            )
+
             # Register extended class.
             register_calendar_type(k, cls, force=True)
+
             # Remove original class from factory cache.
             _remove_calendar_from_factory_cache(k)
 
+    # Create and register extended calendar classes for all calendars for which explicit rules have been defined.
     for k, v in _extensions.items():
-        cls, day_of_week_expiry = v
+        # Get the original class and the day of the week for expiry days.
+        cls, day_of_week_expiry = v.base, v.day_of_week_expiry
+
         # Store the original class for later use.
         _original_classes[k] = cls
-        # Create extended class.
-        cls = extend_class(cls, day_of_week_expiry=day_of_week_expiry, changeset_provider=get_changeset_fn(k))
+
+        # Create extended class with support for expiry days.
+        cls = extend_class(
+            cls,
+            day_of_week_expiry=day_of_week_expiry,
+            changeset_provider=get_changeset_fn(k),
+        )
+
         # Register extended class.
         register_calendar_type(k, cls, force=True)
+
         # Remove original class from factory cache.
         _remove_calendar_from_factory_cache(k)
 
 
 def remove_extensions() -> None:
     """
     Remove extensions from exchange_calendars.
@@ -125,21 +185,25 @@
     if len(_original_classes) == 0:
         # Extensions have not been applied.
         return
 
     for k, v in _original_classes.items():
         # Register original class.
         register_calendar_type(k, v, force=True)
+
         # Remove extended class from factory cache.
         _remove_calendar_from_factory_cache(k)
 
+    # Clear original classes.
     _original_classes.clear()
 
 
-def register_extension(name: str, cls: Type[ExchangeCalendar], day_of_week_expiry: Optional[int] = None) -> None:
+def register_extension(
+    name: str, cls: type[ExchangeCalendar], day_of_week_expiry: Union[int, None] = None
+) -> None:
     """
     Register an extended calendar class for a given exchange key and a given base class.
 
     This creates and then registers an extended calendar class based on the given class, with support for all
     additional properties of ExtendedExchangeCalendar. Expiry days are on the third instance of the given day of the
     week in each month. The extended class also supports programmatic modifications; see e.g. add_holiday().
 
@@ -152,31 +216,33 @@
     day_of_week_expiry : Optional[int]
         The day of the week on which options expire. If None, expiry days are not supported.
 
     Returns
     -------
     None
     """
-    _extensions[name] = (cls, day_of_week_expiry)
+    _extensions[name] = ExtensionSpec(base=cls, day_of_week_expiry=day_of_week_expiry)
 
 
 def _remove_calendar_from_factory_cache(name: str):
     """
     Remove a cached calendar instance for the given exchange key from the factory cache.
 
     Caveat: This function accesses the private attribute _factory_output_cache of the global calendar dispatcher.
     """
     # noinspection PyProtectedMember
     calendar_utils.global_calendar_dispatcher._factory_output_cache.pop(name, None)
 
 
-P = ParamSpec('P')
+P = ParamSpec("P")
 
 
-def _with_changeset(f: Callable[Concatenate[ChangeSet, P], ChangeSet]) -> Callable[Concatenate[str, P], None]:
+def _with_changeset(
+    f: Callable[Concatenate[ChangeSet, P], ChangeSet],
+) -> Callable[Concatenate[str, P], None]:
     """
     An annotation that obtains the changeset from _changesets that corresponds to the exchange key passed as the first
     positional argument to the wrapped function. Instead of passing the key, passes the retrieved changeset, or a newly
     created empty one, if no entry for the key exists yet, to the wrapped function.
 
     After the wrapped function has finished, saves the changeset back to _changesets under the key. Note that this only
     has an effect if the changeset was newly created upon retrieval, before the wrapped call. Otherwise, the changeset
@@ -192,14 +258,15 @@
         The function to wrap.
 
     Returns
     -------
     Callable
         The wrapped function.
     """
+
     @functools.wraps(f)
     def wrapper(exchange: str, *args: P.args, **kwargs: P.kwargs) -> None:
         # Retrieve changeset for key, create new empty one, if required.
         cs: ChangeSet = _changesets.get(exchange, ChangeSet())
 
         # Call wrapped function with changeset as first positional argument.
         cs = f(cs, *args, **kwargs)
@@ -217,149 +284,278 @@
         # Return result of wrapped function.
         return None
 
     return wrapper
 
 
 @_with_changeset
-def _add_day(cs: ChangeSet, spec: Union[DaySpec, DaySpecWithTime, dict]) -> ChangeSet:
+def _add_day(cs: ChangeSet, date: DateLike, props: DayPropsLike) -> ChangeSet:
     """
     Add a day of a given type to the changeset for a given exchange calendar.
 
     Parameters
     ----------
     cs : ChangeSet
         The changeset to which to add the day.
-    spec : Union[DaySpec, DaySpecWithTime, dict]
-        The properties to add for the day. Must match the properties required by the given day type.
+    date : TimestampLike
+        The date to add. Must be convertible to pandas.Timestamp.
+    props : DayPropsLike
+        The properties of the day to add.
 
     Returns
     -------
     ChangeSet
         The changeset with the added day.
 
     Raises
     ------
     ValueError
         If the changeset would be inconsistent after adding the day.
     """
-    return cs.add_day(spec)
+    return cs.add_day(date, props)
 
 
-@validate_call
-def add_day(exchange: str, spec: Union[DaySpec, DaySpecWithTime, dict]) -> None:
+@validate_call(config={"arbitrary_types_allowed": True})
+def add_day(exchange: str, date: DateLike, props: DayPropsLike) -> None:
     """
     Add a day of a given type to the given exchange calendar.
 
     Parameters
     ----------
     exchange : str
         The exchange key for which to add the day.
-    spec : Union[DaySpec, DaySpecWithTime, dict]
+    date : TimestampLike
+        The date to add. Must be convertible to pandas.Timestamp.
+    props : Union[DaySpec, DaySpecWithTime, dict]
         The properties to add for the day. Must match the properties required by the given day type.
 
     Returns
     -------
     None
 
     Raises
     ------
     ValidationError
         If strict is True and the changeset for the exchange would be inconsistent after adding the day.
     """
-    _add_day(exchange, spec)
+    _add_day(exchange, date, props)
 
 
 @_with_changeset
-def _remove_day(cs: ChangeSet, date: TimestampLike) -> ChangeSet:
+def _remove_day(cs: ChangeSet, date: DateLike) -> ChangeSet:
     """
     Remove a day of a given type from the changeset for a given exchange calendar.
 
     Parameters
     ----------
     cs : ChangeSet
         The changeset from which to remove the day.
     date : TimestampLike
         The date to remove. Must be convertible to pandas.Timestamp.
 
     Returns
     -------
     ChangeSet
         The changeset with the removed day.
-
-    Raises
-    ------
-    ValidationError
-        If strict is True and the changeset for the exchange would be inconsistent after removing the day.
     """
     return cs.remove_day(date)
 
 
-def remove_day(exchange: str, date: TimestampLike) -> None:
+@validate_call(config={"arbitrary_types_allowed": True})
+def remove_day(exchange: str, date: DateLike) -> None:
     """
     Remove a day of a given type from the given exchange calendar.
 
     Parameters
     ----------
     exchange : str
         The exchange key for which to remove the day.
     date : TimestampLike
         The date to remove. Must be convertible to pandas.Timestamp.
 
     Returns
     -------
     None
-
-    Raises
-    ------
-    ValidationError
-        If strict is True and the changeset for the exchange would be inconsistent after removing the day.
     """
     _remove_day(exchange, date)
 
 
 @_with_changeset
-def _reset_day(cs: ChangeSet, date: TimestampLike) -> ChangeSet:
+def _set_tags(cs: ChangeSet, date: DateLike, tags: Tags) -> ChangeSet:
+    """
+    Set tags for a given day in the given exchange calendar.
+
+    Parameters
+    ----------
+    cs : ChangeSet
+        The changeset where to set the tags.
+    date : TimestampLike
+        The date for which to set the tags.
+    tags : Tags
+        The tags to set.
+
+    Returns
+    -------
+    ChangeSet
+        The changeset with the given tags set for the given day.
+    """
+    return cs.set_tags(date, tags)
+
+
+@validate_call(config={"arbitrary_types_allowed": True})
+def set_tags(exchange: str, date: DateLike, tags: Tags) -> None:
+    """
+    Set tags for a given day in the given exchange calendar.
+
+    Parameters
+    ----------
+    exchange : str
+        The exchange for which to set the tags.
+    date : TimestampLike
+        The date for which to set the tags.
+    tags : Tags
+        The tags to set.
+
+    Returns
+    -------
+    None
+    """
+    _set_tags(exchange, date, tags)
+
+
+@_with_changeset
+def _set_comment(cs: ChangeSet, date: DateLike, comment: Union[str, None]) -> ChangeSet:
+    """
+    Set comment for a given day in the given exchange calendar.
+
+    Parameters
+    ----------
+    cs : ChangeSet
+        The changeset where to set the tags.
+    date : TimestampLike
+        The date for which to set the tags.
+    comment : str
+        The comment to set.
+
+    Returns
+    -------
+    ChangeSet
+        The changeset with the given comment set for the given day.
+    """
+    return cs.set_comment(date, comment)
+
+
+@validate_call(config={"arbitrary_types_allowed": True})
+def set_comment(exchange: str, date: DateLike, comment: Union[str, None]) -> None:
+    """
+    Set tags for a given day in the given exchange calendar.
+
+    Parameters
+    ----------
+    exchange : str
+        The exchange for which to set the tags.
+    date : TimestampLike
+        The date for which to set the tags.
+    comment : str
+        The comment to set.
+
+    Returns
+    -------
+    None
+    """
+    _set_comment(exchange, date, comment)
+
+
+@_with_changeset
+def _set_meta(cs: ChangeSet, date: DateLike, meta: Union[DayMeta, None]) -> ChangeSet:
+    """
+    Set metadata for a given day in the given exchange calendar.
+
+    Parameters
+    ----------
+    cs : ChangeSet
+        The changeset where to set the tags.
+    date : TimestampLike
+        The date for which to set the tags.
+    meta : DayMeta
+        The metadata to set.
+
+    Returns
+    -------
+    ChangeSet
+        The changeset with the given metadata set for the given day.
+    """
+    return cs.set_meta(date, meta)
+
+
+@validate_call(config={"arbitrary_types_allowed": True})
+def set_meta(exchange: str, date: DateLike, meta: Union[DayMeta, None]) -> None:
+    """
+    Set metadata for a given day in the given exchange calendar.
+
+    Parameters
+    ----------
+    exchange : str
+        The exchange for which to set the tags.
+    date : TimestampLike
+        The date for which to set the tags.
+    meta : DayMeta
+        The metadata to set.
+
+    Returns
+    -------
+    None
+    """
+    _set_meta(exchange, date, meta)
+
+
+@_with_changeset
+def _reset_day(cs: ChangeSet, date: DateLike, include_tags: bool) -> ChangeSet:
     """
     Clear a day of a given type from the changeset for a given exchange calendar.
 
     Parameters
     ----------
     cs : ChangeSet
         The changeset from which to clear the day.
     date : TimestampLike
         The date to clear. Must be convertible to pandas.Timestamp.
+    include_tags : bool
+        Whether to also clear the tags for the day.
 
     Returns
     -------
     ChangeSet
         The changeset with the cleared day.
     """
-    return cs.clear_day(date)
+    return cs.clear_day(date, include_meta=include_tags)
 
 
-def reset_day(exchange: str, date: TimestampLike) -> None:
+@validate_call(config={"arbitrary_types_allowed": True})
+def reset_day(exchange: str, date: DateLike, include_tags: bool = False) -> None:
     """
     Clear a day of a given type from the given exchange calendar.
 
     Parameters
     ----------
     exchange : str
         The exchange key for which to clear the day.
     date : TimestampLike
         The date to clear. Must be convertible to pandas.Timestamp.
+    include_tags : bool
+        Whether to also clear the tags for the day. Defaults to False.
 
     Returns
     -------
     None
     """
-    _reset_day(exchange, date)
+    _reset_day(exchange, date, include_tags=include_tags)
 
 
-def add_holiday(exchange: str, date: TimestampLike, name: str = "Holiday") -> None:
+def add_holiday(exchange: str, date: DateLike, name: str = "Holiday") -> None:
     """
     Add a holiday to an exchange calendar.
 
     Parameters
     ----------
     exchange : str
         The exchange key for which to add the day.
@@ -373,72 +569,80 @@
     None
 
     Raises
     ------
     ValidationError
         If strict is True and the changeset for the exchange would be inconsistent after adding the day.
     """
-    _add_day(exchange, {'date': date, 'type': DayType.HOLIDAY, 'name': name})
+    _add_day(exchange, date, {"type": DayType.HOLIDAY, "name": name})
 
 
-def add_special_open(exchange: str, date: TimestampLike, time: Union[dt.time, str], name: str = "Special Open") -> None:
+def add_special_open(
+    exchange: str, date: DateLike, time: TimeLike, name: str = "Special Open"
+) -> None:
     """
     Add a special open to an exchange calendar.
 
     Parameters
     ----------
     exchange : str
         The exchange key for which to add the day.
     date : TimestampLike
         The date to add. Must be convertible to pandas.Timestamp.
-    time : Union[time, str]
+    time : TimeLike
         The time of the special open. If a string, must be in the format 'HH:MM' or 'HH:MM:SS'.
     name : str
         The name of the special open.
 
     Returns
     -------
     None
 
     Raises
     ------
     ValidationError
         If strict is True and the changeset for the exchange would be inconsistent after adding the day.
     """
-    _add_day(exchange, {'date': date, 'type': DayType.SPECIAL_OPEN, 'name': name, 'time': time})
+    _add_day(exchange, date, {"type": DayType.SPECIAL_OPEN, "name": name, "time": time})
 
 
-def add_special_close(exchange: str, date: TimestampLike, time: Union[dt.time, str], name: str = "Special Close") -> None:
+def add_special_close(
+    exchange: str, date: DateLike, time: TimeLike, name: str = "Special Close"
+) -> None:
     """
     Add a special close to an exchange calendar.
 
     Parameters
     ----------
     exchange : str
         The exchange key for which to add the day.
     date : TimestampLike
         The date to add. Must be convertible to pandas.Timestamp.
-    time : Union[time, str]
+    time : TimeLike
         The time of the special close. If a string, must be in the format 'HH:MM' or 'HH:MM:SS'.
     name : str
         The name of the special close.
 
     Returns
     -------
     None
 
     Raises
     ------
     ValidationError
         If strict is True and the changeset for the exchange would be inconsistent after adding the day.
     """
-    _add_day(exchange, {'date': date, 'type': DayType.SPECIAL_CLOSE, 'name': name, 'time': time})
+    _add_day(
+        exchange, date, {"type": DayType.SPECIAL_CLOSE, "name": name, "time": time}
+    )
 
 
-def add_quarterly_expiry(exchange: str, date: TimestampLike, name: str = "Quarterly Expiry") -> None:
+def add_quarterly_expiry(
+    exchange: str, date: DateLike, name: str = "Quarterly Expiry"
+) -> None:
     """
     Add a quarterly expiry to an exchange calendar.
 
     Parameters
     ----------
     exchange : str
         The exchange key for which to add the day.
@@ -452,18 +656,20 @@
     None
 
     Raises
     ------
     ValidationError
         If strict is True and the changeset for the exchange would be inconsistent after adding the day.
     """
-    _add_day(exchange, {'date': date, 'type': DayType.QUARTERLY_EXPIRY, 'name': name})
+    _add_day(exchange, date, {"type": DayType.QUARTERLY_EXPIRY, "name": name})
 
 
-def add_monthly_expiry(exchange: str, date: Any, name: str = "Monthly Expiry") -> None:
+def add_monthly_expiry(
+    exchange: str, date: DateLike, name: str = "Monthly Expiry"
+) -> None:
     """
     Add a monthly expiry to an exchange calendar.
 
     Parameters
     ----------
     exchange : str
         The exchange key for which to add the day.
@@ -477,33 +683,33 @@
     None
 
     Raises
     ------
     ValidationError
         If strict is True and the changeset for the exchange would be inconsistent after adding the day.
     """
-    _add_day(exchange, {'date': date, 'type': DayType.MONTHLY_EXPIRY, 'name': name})
+    _add_day(exchange, date, {"type": DayType.MONTHLY_EXPIRY, "name": name})
 
 
 @_with_changeset
-def _reset_calendar(cs: ChangeSet) -> ChangeSet:
+def _reset_calendar(cs: ChangeSet, include_tags: bool) -> ChangeSet:
     """
     Reset an exchange calendar to its original state.
 
     Parameters
     ----------
     cs : ChangeSet
         The changeset to reset.
 
     Returns
     -------
     ChangeSet
         The reset changeset.
     """
-    return cs.clear()
+    return cs.clear(include_meta=include_tags)
 
 
 def reset_calendar(exchange: str) -> None:
     """
     Reset an exchange calendar to its original state.
 
     Parameters
@@ -511,15 +717,15 @@
     exchange : str
         The exchange key for which to reset the calendar.
 
     Returns
     -------
     None
     """
-    _reset_calendar(exchange)
+    _reset_calendar(exchange, include_tags=True)
 
 
 def reset_all_calendars() -> None:
     """
     Reset all exchange calendars to their original states.
 
     Returns
@@ -540,39 +746,39 @@
     """
     Apply changes to an exchange calendar.
 
     Parameters
     ----------
     exchange : str
         The exchange key for which to apply the changes.
-    changes : dict
+    changes : ChangeSet
         The changes to apply.
 
     Returns
     -------
     None
     """
     _update_calendar(exchange, changes)
 
 
-def get_changes_for_calendar(exchange: str) -> ChangeSet:
+def get_changes_for_calendar(exchange: str) -> Union[ChangeSet, None]:
     """
     Get the changes for an exchange calendar.
 
     Parameters
     ----------
     exchange : str
         The exchange key for which to get the changes.
 
     Returns
     -------
     ChangeSet
-        The changes for the exchange.
+        The changeset for the given exchange, or None, if no changes have been registered.
     """
-    cs: Optional[ChangeSet] = _changesets.get(exchange, None)
+    cs: Union[ChangeSet, None] = _changesets.get(exchange, None)
 
     if cs is not None:
         cs = cs.model_copy(deep=True)
 
     return cs
 
 
@@ -585,24 +791,45 @@
     dict
         The changes for all exchange calendars.
     """
     return ChangeSetDict({k: v.model_copy(deep=True) for k, v in _changesets.items()})
 
 
 # Declare public names.
-__all__ = ["apply_extensions", "remove_extensions", "register_extension", "extend_class", "DayType", "add_day",
-           "remove_day", "reset_day", "DaySpec", "DaySpecWithTime", "add_holiday", "add_special_close",
-           "add_special_open", "add_quarterly_expiry", "add_monthly_expiry", "reset_calendar", "reset_all_calendars",
-           "update_calendar", "get_changes_for_calendar", "get_changes_for_all_calendars", "ChangeSet",
-           "ExtendedExchangeCalendar", "ExchangeCalendarExtensions"]
+__all__ = [
+    "apply_extensions",
+    "remove_extensions",
+    "register_extension",
+    "extend_class",
+    "DayType",
+    "add_day",
+    "remove_day",
+    "reset_day",
+    "DayPropsLike",
+    "add_holiday",
+    "add_special_close",
+    "add_special_open",
+    "add_quarterly_expiry",
+    "add_monthly_expiry",
+    "set_meta",
+    "reset_calendar",
+    "reset_all_calendars",
+    "update_calendar",
+    "get_changes_for_calendar",
+    "get_changes_for_all_calendars",
+    "ChangeSet",
+    "ExtendedExchangeCalendar",
+    "ExchangeCalendarExtensions",
+]
 
 __version__ = None
 
 try:
     from importlib.metadata import version
+
     # get version from installed package
     __version__ = version("exchange_calendars_extensions")
     del version
 except ImportError:
     pass
 
 if __version__ is None:
```

### Comparing `exchange_calendars_extensions-0.7.0/exchange_calendars_extensions/core/holiday.py` & `exchange_calendars_extensions-0.8.0/exchange_calendars_extensions/core/holiday.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from datetime import timedelta, tzinfo
 from typing import Optional, Callable, Union
 
 import pandas as pd
 from exchange_calendars.pandas_extensions.holiday import Holiday
 from pandas import Series, DatetimeIndex
 
-from exchange_calendars_extensions.core.offset import LastDayOfMonthOffsetClasses, \
-    ThirdDayOfWeekInMonthOffsetClasses
+from exchange_calendars_extensions.core.offset import (
+    LastDayOfMonthOffsetClasses,
+    ThirdDayOfWeekInMonthOffsetClasses,
+)
 
 
 def get_monthly_expiry_holiday(
-        name: str,
-        day_of_week: int,
-        month: int,
-        observance: Optional[Callable[[pd.Timestamp], pd.Timestamp]] = None,
-        start_date: Optional[pd.Timestamp] = None,
-        end_date: Optional[pd.Timestamp] = None,
-        tz: Optional[tzinfo] = None) -> Holiday:
+    name: str,
+    day_of_week: int,
+    month: int,
+    observance: Union[Callable[[pd.Timestamp], pd.Timestamp], None] = None,
+    start_date: Union[pd.Timestamp, None] = None,
+    end_date: Union[pd.Timestamp, None] = None,
+    tz: Union[tzinfo, None] = None,
+) -> Holiday:
     """
     Return a holiday that occurs yearly on the third given day of the week in the given month of the year.
 
     For example, when day_of_week=2 and month=1, this returns a holiday that occurs yearly on the third Wednesday in
     January.
 
     Parameters
@@ -41,26 +44,34 @@
         The timezone in which to interpret the holiday, by default None.
 
     Returns
     -------
     Holiday
         A new Holiday object as specified.
     """
-    return Holiday(name, month=1, day=1,
-                   offset=ThirdDayOfWeekInMonthOffsetClasses[day_of_week][month](),
-                   observance=observance, start_date=start_date, end_date=end_date, tz=tz)
+    return Holiday(
+        name,
+        month=1,
+        day=1,
+        offset=ThirdDayOfWeekInMonthOffsetClasses[day_of_week][month](),
+        observance=observance,
+        start_date=start_date,
+        end_date=end_date,
+        tz=tz,
+    )
 
 
 def get_last_day_of_month_holiday(
-        name: str,
-        month: int,
-        observance: Optional[Callable[[pd.Timestamp], pd.Timestamp]] = None,
-        start_date: Optional[pd.Timestamp] = None,
-        end_date: Optional[pd.Timestamp] = None,
-        tz: Optional[tzinfo] = None) -> Holiday:
+    name: str,
+    month: int,
+    observance: Union[Callable[[pd.Timestamp], pd.Timestamp], None] = None,
+    start_date: Union[pd.Timestamp, None] = None,
+    end_date: Union[pd.Timestamp, None] = None,
+    tz: Union[tzinfo, None] = None,
+) -> Holiday:
     """
     Return a holiday that occurs yearly on the last day of the given month of the year.
 
     For example, when month=1, this returns a holiday that occurs yearly on the last day of January.
 
     Parameters
     ----------
@@ -78,31 +89,38 @@
         The timezone in which to interpret the holiday, by default None.
 
     Returns
     -------
     Holiday
         A new Holiday object as specified.
     """
-    return Holiday(name, month=1, day=1,
-                   offset=LastDayOfMonthOffsetClasses[month](),
-                   observance=observance, start_date=start_date, end_date=end_date, tz=tz)
+    return Holiday(
+        name,
+        month=1,
+        day=1,
+        offset=LastDayOfMonthOffsetClasses[month](),
+        observance=observance,
+        start_date=start_date,
+        end_date=end_date,
+        tz=tz,
+    )
 
 
 class DayOfWeekPeriodicHoliday(Holiday):
     """
     A holiday that occurs on a specific day of the week and repeats weekly.
     """
 
     def __init__(
         self,
         name: str,
         day_of_week: int,
         start_date: Optional[pd.Timestamp] = None,
         end_date: Optional[pd.Timestamp] = None,
-        tz: Optional[tzinfo] = None
+        tz: Optional[tzinfo] = None,
     ) -> None:
         """
         Constructor.
 
         Parameters
         ----------
         name : str
@@ -127,15 +145,15 @@
             month=None,
             day=None,
             offset=None,
             observance=None,
             start_date=start_date,
             end_date=end_date,
             days_of_week=None,
-            tz=tz
+            tz=tz,
         )
 
         # Store day of week.
         self.day_of_week = day_of_week
 
     def _dates(self, start_date, end_date) -> pd.DatetimeIndex:
         """
@@ -160,28 +178,32 @@
             end_date = min(end_date, self.end_date.tz_localize(end_date.tz))
 
         if start_date > end_date:
             # Empty result.
             return pd.DatetimeIndex([])
 
         # Get the first date larger or equal to start_date where the day of the week is the same as day_of_week.
-        first = start_date + pd.Timedelta(days=(self.day_of_week - start_date.dayofweek) % 7)
+        first = start_date + pd.Timedelta(
+            days=(self.day_of_week - start_date.dayofweek) % 7
+        )
 
         if first > end_date:
             # Empty result.
             return pd.DatetimeIndex([])
 
         # Get the last date smaller or equal to end_date where the day of the week is the same as day_of_week.
         last = end_date - pd.Timedelta(days=(end_date.dayofweek - self.day_of_week) % 7)
 
         # Create a pandas DateTimeIndex with the dates of the holidays.
         dates = pd.date_range(start=first, end=last, freq=timedelta(days=7))
 
         # Return the dates.
         return dates
 
-    def dates(self, start_date, end_date, return_name=False) -> Union[DatetimeIndex, Series]:
+    def dates(
+        self, start_date, end_date, return_name=False
+    ) -> Union[DatetimeIndex, Series]:
         # Get DateTimeIndex with the dates of the holidays.
         dates = self._dates(start_date, end_date)
 
         # Return the dates, either as a series (return_name=True) or as a DateTimeIndex (return_name=False).
         return pd.Series(self.name, index=dates) if return_name else dates
```

### Comparing `exchange_calendars_extensions-0.7.0/exchange_calendars_extensions/core/holiday_calendar.py` & `exchange_calendars_extensions-0.8.0/exchange_calendars_extensions/core/holiday_calendar.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,48 @@
 import datetime
 from abc import ABC
+from collections import OrderedDict
+from collections.abc import Iterable
 from copy import copy
 from dataclasses import field, dataclass
 from functools import reduce
-from typing import Iterable, Optional, Callable, Union, Type, Protocol, List, Tuple, runtime_checkable
+from typing import (
+    Optional,
+    Callable,
+    Union,
+    Protocol,
+    runtime_checkable,
+)
 
 import pandas as pd
 from exchange_calendars import ExchangeCalendar
-from exchange_calendars.exchange_calendar import HolidayCalendar as ExchangeCalendarsHolidayCalendar
+from exchange_calendars.exchange_calendar import (
+    HolidayCalendar as ExchangeCalendarsHolidayCalendar,
+)
 from exchange_calendars.pandas_extensions.holiday import Holiday
-from exchange_calendars.pandas_extensions.holiday import Holiday as ExchangeCalendarsHoliday
+from exchange_calendars.pandas_extensions.holiday import (
+    Holiday as ExchangeCalendarsHoliday,
+)
 from pandas.tseries.holiday import Holiday as PandasHoliday
+from pydantic import validate_call
 
-from exchange_calendars_extensions.api.changes import ChangeSet, DayType
-from exchange_calendars_extensions.core.holiday import get_monthly_expiry_holiday, DayOfWeekPeriodicHoliday, \
-    get_last_day_of_month_holiday
+from exchange_calendars_extensions.api.changes import (
+    ChangeSet,
+    DayType,
+    DayMeta,
+    TimestampLike,
+)
+from exchange_calendars_extensions.core.holiday import (
+    get_monthly_expiry_holiday,
+    DayOfWeekPeriodicHoliday,
+    get_last_day_of_month_holiday,
+)
+
+# Timdelta that represents a day minus the smallest increment of time.
+ONE_DAY_MINUS_EPS = pd.Timedelta(1, "d") - pd.Timedelta(1, "ns")
 
 
 class HolidayCalendar(ExchangeCalendarsHolidayCalendar):
     """
     A subclass of exchange_calendars.exchange_calendar.HolidayCalendar that supports overlapping rules, i.e. rules that
     apply to the same date.
 
@@ -41,15 +65,19 @@
         # Drop duplicates, keeping the first occurrence.
         if return_name:
             return holidays[~holidays.index.duplicated()]
         else:
             return holidays.drop_duplicates()
 
 
-def get_conflicts(holidays_dates: List[Union[pd.Timestamp, None]], other_holidays: pd.DatetimeIndex, weekend_days: Iterable[int]) -> List[int]:
+def get_conflicts(
+    holidays_dates: list[Union[pd.Timestamp, None]],
+    other_holidays: pd.DatetimeIndex,
+    weekend_days: Iterable[int],
+) -> list[int]:
     """
     Get the indices of holidays that coincide with holidays from the other calendar or the given weekend days.
 
     Parameters
     ----------
     holidays_dates : List[Union[pd.Timestamp, None]]
         The dates of the holidays. A date may be None and is then ignored.
@@ -61,15 +89,24 @@
     Returns
     -------
     List[int]
         The indices of holidays that coincide with holidays from the other calendar or the given weekend days.
     """
 
     # Determine the indices of holidays that coincide with holidays from the other calendar.
-    return [i for i in range(len(holidays_dates)) if holidays_dates[i] is not None and (holidays_dates[i] in other_holidays or holidays_dates[i].weekday() in weekend_days or holidays_dates[i] in holidays_dates[i+1:])]
+    return [
+        i
+        for i in range(len(holidays_dates))
+        if holidays_dates[i] is not None
+        and (
+            holidays_dates[i] in other_holidays
+            or holidays_dates[i].weekday() in weekend_days
+            or holidays_dates[i] in holidays_dates[i + 1 :]
+        )
+    ]
 
 
 # A function that takes a date and returns a date or None.
 RollFn = Callable[[pd.Timestamp], Union[pd.Timestamp, None]]
 
 
 def roll_one_day_same_month(d: pd.Timestamp) -> Union[pd.Timestamp, None]:
@@ -101,20 +138,24 @@
         return None
 
     # Return the rolled back date.
     return d
 
 
 class AdjustedHolidayCalendar(ExchangeCalendarsHolidayCalendar):
-
-    def __init__(self, rules, other: ExchangeCalendarsHolidayCalendar, weekmask: str,
-                 roll_fn: RollFn = lambda d: d - pd.Timedelta(days=1)) -> None:
+    def __init__(
+        self,
+        rules,
+        other: ExchangeCalendarsHolidayCalendar,
+        weekmask: str,
+        roll_fn: RollFn = lambda d: d - pd.Timedelta(days=1),
+    ) -> None:
         super().__init__(rules=rules)
         self._other = other
-        self._weekend_days = {d for d in range(7) if weekmask[d] == '0'}
+        self._weekend_days = {d for d in range(7) if weekmask[d] == "0"}
         self._roll_fn = roll_fn
 
     def holidays(self, start=None, end=None, return_name=False):
         # Get the holidays from the parent class.
         holidays = super().holidays(start=start, end=end, return_name=return_name)
 
         # Get the holidays from the other calendar.
@@ -128,29 +169,48 @@
             return holidays
 
         while True:
             # For each index of a conflicting holiday, adjust the date by using the roll function.
             for i in conflicts:
                 holidays_dates[i] = self._roll_fn(holidays_dates[i])
 
-            conflicts = get_conflicts(holidays_dates, other_holidays, self._weekend_days)
+            conflicts = get_conflicts(
+                holidays_dates, other_holidays, self._weekend_days
+            )
 
             if len(conflicts) == 0:
                 break
 
         if return_name:
             # Return a series, filter out dates that are None.
-            return pd.Series({d: n for d, n in zip(holidays_dates, holidays.values) if d is not None and (start is None or d >= start) and (end is None or d <= end)})
+            return pd.Series(
+                {
+                    d: n
+                    for d, n in zip(holidays_dates, holidays.values)
+                    if d is not None
+                    and (start is None or d >= start)
+                    and (end is None or d <= end)
+                }
+            )
         else:
             # Return index, filter out dates that are None.
-            return pd.DatetimeIndex([d for d in holidays_dates if d is not None and (start is None or d >= start) and (end is None or d <= end)])
+            return pd.DatetimeIndex(
+                [
+                    d
+                    for d in holidays_dates
+                    if d is not None
+                    and (start is None or d >= start)
+                    and (end is None or d <= end)
+                ]
+            )
 
 
-def get_holiday_calendar_from_timestamps(timestamps: Iterable[pd.Timestamp],
-                                         name: Optional[str] = None) -> ExchangeCalendarsHolidayCalendar:
+def get_holiday_calendar_from_timestamps(
+    timestamps: Iterable[pd.Timestamp], name: Optional[str] = None
+) -> ExchangeCalendarsHolidayCalendar:
     """
     Return a holiday calendar with holidays given by a collection of timestamps.
 
     If name is specified, each holiday will use that given name.
 
     Parameters
     ----------
@@ -161,22 +221,28 @@
 
     Returns
     -------
     ExchangeCalendarsHolidayCalendar
         A new HolidayCalendar object as specified.
     """
     # Generate list of rules, one for each timestamp.
-    rules = [Holiday(name, year=ts.year, month=ts.month, day=ts.day, start_date=ts, end_date=ts) for ts in
-             set(dict.fromkeys(timestamps))]  # As of Python 3.7, dict preserves insertion order.
+    rules = [
+        Holiday(
+            name, year=ts.year, month=ts.month, day=ts.day, start_date=ts, end_date=ts
+        )
+        for ts in set(dict.fromkeys(timestamps))
+    ]  # As of Python 3.7, dict preserves insertion order.
 
     # Return a new HolidayCalendar with the given rules.
     return ExchangeCalendarsHolidayCalendar(rules=rules)
 
 
-def get_holiday_calendar_from_day_of_week(day_of_week: int, name: Optional[str] = None) -> HolidayCalendar:
+def get_holiday_calendar_from_day_of_week(
+    day_of_week: int, name: Optional[str] = None
+) -> HolidayCalendar:
     """
     Return a holiday calendar with a periodic holiday occurring on each instance of the given day of the week.
 
     Parameters
     ----------
     day_of_week : int
         The day of the week to use, where 0 is Monday and 6 is Sunday.
@@ -186,49 +252,62 @@
     # Generate list of rules. Actually contains only one rule for the given day of the week.
     rules = [DayOfWeekPeriodicHoliday(name, day_of_week)]
 
     # Return a new HolidayCalendar with the given rules.
     return ExchangeCalendarsHolidayCalendar(rules=rules)
 
 
-def merge_calendars(calendars: Iterable[ExchangeCalendarsHolidayCalendar]) -> ExchangeCalendarsHolidayCalendar:
+def merge_calendars(
+    calendars: Iterable[ExchangeCalendarsHolidayCalendar],
+) -> ExchangeCalendarsHolidayCalendar:
     """
     Return a holiday calendar with all holidays from the given calendars merged into a single HolidayCalendar.
 
     The rules of the returned calendar will be the concatenation of the rules of the given calendars. Note that rules
     that occur earlier take precedence in case of conflicts, i.e. rules that apply to the same date.
     """
-    x = reduce(lambda x, y: HolidayCalendar(rules=[r for r in x.rules] + [r for r in y.rules]), calendars,
-               ExchangeCalendarsHolidayCalendar(rules=[]))
+    x = reduce(
+        lambda x, y: HolidayCalendar(rules=[r for r in x.rules] + [r for r in y.rules]),
+        calendars,
+        ExchangeCalendarsHolidayCalendar(rules=[]),
+    )
     return x
 
 
-def get_holidays_calendar(exchange_calendar: ExchangeCalendar) -> ExchangeCalendarsHolidayCalendar:
+def get_holidays_calendar(
+    exchange_calendar: ExchangeCalendar,
+) -> ExchangeCalendarsHolidayCalendar:
     """
     Return a holiday calendar with all holidays, regular and ad-hoc, from the given exchange calendar merged into a
     single calendar.
 
     Parameters
     ----------
     exchange_calendar : ExchangeCalendar
         The exchange calendar to use.
 
     Returns
     -------
     ExchangeCalendarsHolidayCalendar
         A new HolidayCalendar with all holidays from the given EchangeCalendar.
     """
-    holiday_calendars = [get_holiday_calendar_from_timestamps(exchange_calendar.adhoc_holidays, name='ad-hoc holiday'),
-                         exchange_calendar.regular_holidays]
+    holiday_calendars = [
+        get_holiday_calendar_from_timestamps(
+            exchange_calendar.adhoc_holidays, name="ad-hoc holiday"
+        ),
+        exchange_calendar.regular_holidays,
+    ]
 
     # Merge all calendars by reducing the list of calendars into one, calling the merge method on each pair.
     return merge_calendars(holiday_calendars)
 
 
-def get_special_opens_calendar(exchange_calendar: ExchangeCalendar) -> ExchangeCalendarsHolidayCalendar:
+def get_special_opens_calendar(
+    exchange_calendar: ExchangeCalendar,
+) -> ExchangeCalendarsHolidayCalendar:
     """
     Return a holiday calendar with all special opens, regular and ad-hoc, from the given exchange calendar merged into a
     single calendar.
 
     Parameters
     ----------
     exchange_calendar : ExchangeCalendar
@@ -240,29 +319,35 @@
         A new HolidayCalendar with all special opens from the given EchangeCalendar.
     """
     holiday_calendars = []
 
     # Add ad-hoc special opens.
     for item in exchange_calendar.special_opens_adhoc:
         _, definition = item
-        holiday_calendars.append(get_holiday_calendar_from_timestamps(definition, name='ad-hoc special open'))
+        holiday_calendars.append(
+            get_holiday_calendar_from_timestamps(definition, name="ad-hoc special open")
+        )
 
     # Add regular special open days.
     for item in exchange_calendar.special_opens:
         _, definition = item
         if isinstance(definition, ExchangeCalendarsHolidayCalendar):
             holiday_calendars.append(definition)
         elif isinstance(definition, int):
-            holiday_calendars.append(get_holiday_calendar_from_day_of_week(definition, name='special open'))
+            holiday_calendars.append(
+                get_holiday_calendar_from_day_of_week(definition, name="special open")
+            )
 
     # Merge all calendars by reducing the list of calendars into one, calling the merge method on each pair.
     return merge_calendars(holiday_calendars)
 
 
-def get_special_closes_calendar(exchange_calendar: ExchangeCalendar) -> ExchangeCalendarsHolidayCalendar:
+def get_special_closes_calendar(
+    exchange_calendar: ExchangeCalendar,
+) -> ExchangeCalendarsHolidayCalendar:
     """
     Return a holiday calendar with all special closes, regular and ad-hoc, from the given exchange calendar merged into
     a single calendar.
 
     Parameters
     ----------
     exchange_calendar : ExchangeCalendar
@@ -274,49 +359,62 @@
         A new HolidayCalendar with all special closes from the given EchangeCalendar.
     """
     holiday_calendars = []
 
     # Add ad-hoc special closes.
     for item in exchange_calendar.special_closes_adhoc:
         _, definition = item
-        holiday_calendars.append(get_holiday_calendar_from_timestamps(definition, name='ad-hoc special close'))
+        holiday_calendars.append(
+            get_holiday_calendar_from_timestamps(
+                definition, name="ad-hoc special close"
+            )
+        )
 
     # Add regular special close days.
     for item in exchange_calendar.special_closes:
         _, definition = item
         if isinstance(definition, ExchangeCalendarsHolidayCalendar):
             holiday_calendars.append(definition)
         elif isinstance(definition, int):
-            holiday_calendars.append(get_holiday_calendar_from_day_of_week(definition, name='special close'))
+            holiday_calendars.append(
+                get_holiday_calendar_from_day_of_week(definition, name="special close")
+            )
 
     # Merge all calendars by reducing the list of calendars into one, calling the merge method on each pair.
     return merge_calendars(holiday_calendars)
 
 
-def get_weekend_days_calendar(exchange_calendar: ExchangeCalendar) -> ExchangeCalendarsHolidayCalendar:
+def get_weekend_days_calendar(
+    exchange_calendar: ExchangeCalendar,
+) -> ExchangeCalendarsHolidayCalendar:
     """
     Return a holiday calendar with all weekend days from the given exchange calendar as holidays.
 
     Parameters
     ----------
     exchange_calendar : ExchangeCalendar
         The exchange calendar to use.
 
     Returns
     -------
     ExchangeCalendarsHolidayCalendar
         A new HolidayCalendar with all weekend days from the given EchangeCalendar.
     """
-    rules = [DayOfWeekPeriodicHoliday('weekend day', day_of_week) for day_of_week, v in
-             enumerate(exchange_calendar.weekmask) if v == '0']
+    rules = [
+        DayOfWeekPeriodicHoliday("weekend day", day_of_week)
+        for day_of_week, v in enumerate(exchange_calendar.weekmask)
+        if v == "0"
+    ]
     return ExchangeCalendarsHolidayCalendar(rules=rules)
 
 
-def get_monthly_expiry_rules(day_of_week: int,
-                             observance: Optional[Callable[[pd.Timestamp], pd.Timestamp]] = None) -> List[Holiday]:
+def get_monthly_expiry_rules(
+    day_of_week: int,
+    observance: Optional[Callable[[pd.Timestamp], pd.Timestamp]] = None,
+) -> list[Holiday]:
     """
     Return a list of rules for a calendar with a holiday for each month's expiry, but excluding quarterly expiry days.
 
     Parameters
     ----------
     day_of_week : int
         The day of the week to use, where 0 is Monday and 6 is Sunday.
@@ -324,20 +422,24 @@
         The observance function to use, by default None.
 
     Returns
     -------
     List[Holiday]
         A list of rules for a calendar with a holiday for each month's expiry, but excluding quarterly expiry days.
     """
-    return [get_monthly_expiry_holiday('monthly expiry', day_of_week, month, observance) for month in
-             [1, 2, 4, 5, 7, 8, 10, 11]]
+    return [
+        get_monthly_expiry_holiday("monthly expiry", day_of_week, month, observance)
+        for month in [1, 2, 4, 5, 7, 8, 10, 11]
+    ]
 
 
-def get_quadruple_witching_rules(day_of_week: int,
-                                 observance: Optional[Callable[[pd.Timestamp], pd.Timestamp]] = None) -> List[Holiday]:
+def get_quadruple_witching_rules(
+    day_of_week: int,
+    observance: Optional[Callable[[pd.Timestamp], pd.Timestamp]] = None,
+) -> list[Holiday]:
     """
     Return a list of rules for a calendar with a holiday for each quarterly expiry aka quadruple witching.
 
     Parameters
     ----------
     day_of_week : int
         The day of the week to use, where 0 is Monday and 6 is Sunday.
@@ -345,19 +447,24 @@
         The observance function to use, by default None.
 
     Returns
     -------
     List[Holiday]
         A list of rules for a calendar with a holiday for each quarterly expiry aka quadruple witching.
     """
-    return [get_monthly_expiry_holiday('quarterly expiry', day_of_week, month, observance) for month in [3, 6, 9, 12]]
+    return [
+        get_monthly_expiry_holiday("quarterly expiry", day_of_week, month, observance)
+        for month in [3, 6, 9, 12]
+    ]
 
 
-def get_last_day_of_month_rules(name: Optional[str] = 'last trading day of month', observance: Optional[
-    Callable[[pd.Timestamp], pd.Timestamp]] = None) -> List[Holiday]:
+def get_last_day_of_month_rules(
+    name: Optional[str] = "last trading day of month",
+    observance: Optional[Callable[[pd.Timestamp], pd.Timestamp]] = None,
+) -> list[Holiday]:
     """
     Return a list of rules for a calendar with a holiday for each last trading day of the month.
 
     Parameters
     ----------
     name : Optional[str], optional
         The name to use for the holidays, by default 'last trading day of month'.
@@ -365,15 +472,18 @@
         The observance function to use, by default None.
 
     Returns
     -------
     List[Holiday]
         A list of rules for a calendar with a holiday for each last trading day of the month.
     """
-    return [get_last_day_of_month_holiday(name, i, observance=observance) for i in range(1, 13)]
+    return [
+        get_last_day_of_month_holiday(name, i, observance=observance)
+        for i in range(1, 13)
+    ]
 
 
 @runtime_checkable
 class ExchangeCalendarExtensions(Protocol):
     """
     A protocol for extensions to the exchange_calendars.ExchangeCalendar class.
     """
@@ -447,94 +557,108 @@
         -------
         ExchangeCalendarsHolidayCalendar
             A new HolidayCalendar with a holiday for each quarterly expiry.
         """
         ...  # pragma: no cover
 
     @property
-    def last_trading_days_of_months(self) -> Union[ExchangeCalendarsHolidayCalendar, None]:
+    def last_trading_days_of_months(
+        self,
+    ) -> Union[ExchangeCalendarsHolidayCalendar, None]:
         """
         Return a holiday calendar with a holiday for each last trading day of the month.
 
         Returns
         -------
         ExchangeCalendarsHolidayCalendar
             A new HolidayCalendar with a holiday for each last trading day of the month.
         """
         ...  # pragma: no cover
 
     @property
-    def last_regular_trading_days_of_months(self) -> Union[ExchangeCalendarsHolidayCalendar, None]:
+    def last_regular_trading_days_of_months(
+        self,
+    ) -> Union[ExchangeCalendarsHolidayCalendar, None]:
         """
         Return a holiday calendar with a holiday for each last regular trading day of the month.
 
         Returns
         -------
         ExchangeCalendarsHolidayCalendar
             A new HolidayCalendar with a holiday for each last regular trading day of the month.
         """
         ...
 
+    def meta(
+        self,
+        start: Union[TimestampLike, None] = None,
+        end: Union[TimestampLike, None] = None,
+    ) -> dict[pd.Timestamp, DayMeta]: ...
+
 
 @dataclass
 class AdjustedProperties:
     """
     A dataclass for storing adjusted properties of an exchange calendar.
     """
 
     # The regular holidays of the exchange calendar.
-    regular_holidays: List[Holiday]
+    regular_holidays: list[Holiday]
 
     # The ad-hoc holidays of the exchange calendar.
-    adhoc_holidays: List[pd.Timestamp]
+    adhoc_holidays: list[pd.Timestamp]
 
     # The special closes of the exchange calendar.
-    special_closes: List[Tuple[datetime.time, Union[List[Holiday], int]]]
+    special_closes: list[tuple[datetime.time, Union[list[Holiday], int]]]
 
     # The ad-hoc special closes of the exchange calendar.
-    adhoc_special_closes: List[Tuple[datetime.time, pd.DatetimeIndex]]
+    adhoc_special_closes: list[tuple[datetime.time, pd.DatetimeIndex]]
 
     # The special opens of the exchange calendar.
-    special_opens: List[Tuple[datetime.time, Union[List[Holiday], int]]]
+    special_opens: list[tuple[datetime.time, Union[list[Holiday], int]]]
 
     # The ad-hoc special opens of the exchange calendar.
-    adhoc_special_opens: List[Tuple[datetime.time, pd.DatetimeIndex]]
+    adhoc_special_opens: list[tuple[datetime.time, pd.DatetimeIndex]]
 
     # The quarterly expiry days of the exchange calendar.
-    quarterly_expiries: List[Holiday] = field(default_factory=list)
+    quarterly_expiries: list[Holiday] = field(default_factory=list)
 
     # The monthly expiry days of the exchange calendar.
-    monthly_expiries: List[Holiday] = field(default_factory=list)
+    monthly_expiries: list[Holiday] = field(default_factory=list)
 
     # The last trading days of the month of the exchange calendar.
-    last_trading_days_of_months: List[Holiday] = field(default_factory=list)
+    last_trading_days_of_months: list[Holiday] = field(default_factory=list)
 
     # The last regular trading days of the month of the exchange calendar.
-    last_regular_trading_days_of_months: List[Holiday] = field(default_factory=list)
+    last_regular_trading_days_of_months: list[Holiday] = field(default_factory=list)
 
 
 class ExtendedExchangeCalendar(ExchangeCalendar, ExchangeCalendarExtensions, ABC):
     """
     Abstract base class for exchange calendars with extended functionality.
     """
+
     ...
 
 
-def extend_class(cls: Type[ExchangeCalendar], day_of_week_expiry: Optional[int] = None,
-                 changeset_provider: Callable[[], ChangeSet] = None) -> type:
+def extend_class(
+    cls: type[ExchangeCalendar],
+    day_of_week_expiry: Union[int, None] = None,
+    changeset_provider: Union[Callable[[], ChangeSet], None] = None,
+) -> type:
     """
     Extend the given ExchangeCalendar class with additional properties.
 
     Parameters
     ----------
     cls : Type[ExchangeCalendar]
         The input class to extend.
-    day_of_week_expiry : int, optional
+    day_of_week_expiry : Union[int, None]
         The day of the week when expiry days are observed, where 0 is Monday and 6 is Sunday. Defaults to 4 (Friday).
-    changeset_provider : Callable[[], ExchangeCalendarChangeSet], optional
+    changeset_provider : Union[Callable[[], ChangeSet], None]
         The optional function that returns a changeset to apply to the calendar.
 
     Returns
     -------
     type
         The extended class.
 
@@ -597,17 +721,21 @@
         Returns
         -------
         bool
             True if the timestamp is a holiday, False otherwise.
         """
         return any([d == ts for d in holiday.dates(start_date=ts, end_date=ts)])
 
-    def clone_holiday(holiday: Union[PandasHoliday, ExchangeCalendarsHoliday, DayOfWeekPeriodicHoliday],
-                      start_date: Optional[pd.Timestamp] = None, end_date: Optional[pd.Timestamp] = None) -> Union[
-        PandasHoliday, ExchangeCalendarsHoliday, DayOfWeekPeriodicHoliday]:
+    def clone_holiday(
+        holiday: Union[
+            PandasHoliday, ExchangeCalendarsHoliday, DayOfWeekPeriodicHoliday
+        ],
+        start_date: Optional[pd.Timestamp] = None,
+        end_date: Optional[pd.Timestamp] = None,
+    ) -> Union[PandasHoliday, ExchangeCalendarsHoliday, DayOfWeekPeriodicHoliday]:
         """
         Return a copy of the given holiday.
 
         Parameters
         ----------
         holiday : Union[PandasHoliday, ExchangeCalendarsHoliday, DayOfWeekPeriodicHoliday]
             The holiday to copy.
@@ -618,33 +746,56 @@
 
         Returns
         -------
         Union[PandasHoliday, ExchangeCalendarsHoliday, DayOfWeekPeriodicHoliday]
             The copy of the given holiday.
         """
         # Determine the effective start and end dates.
-        start_date_effective = start_date if start_date is not None else holiday.start_date
+        start_date_effective = (
+            start_date if start_date is not None else holiday.start_date
+        )
         end_date_effective = end_date if end_date is not None else holiday.end_date
 
         if isinstance(holiday, DayOfWeekPeriodicHoliday):
-            return DayOfWeekPeriodicHoliday(name=holiday.name, day_of_week=holiday.day_of_week,
-                                            start_date=start_date_effective, end_date=end_date_effective, tz=holiday.tz)
+            return DayOfWeekPeriodicHoliday(
+                name=holiday.name,
+                day_of_week=holiday.day_of_week,
+                start_date=start_date_effective,
+                end_date=end_date_effective,
+                tz=holiday.tz,
+            )
         elif isinstance(holiday, ExchangeCalendarsHoliday):
-            return ExchangeCalendarsHoliday(name=holiday.name, year=holiday.year, month=holiday.month, day=holiday.day,
-                                            offset=holiday.offset, observance=holiday.observance,
-                                            start_date=start_date_effective, end_date=end_date_effective,
-                                            days_of_week=holiday.days_of_week, tz=holiday.tz)
+            return ExchangeCalendarsHoliday(
+                name=holiday.name,
+                year=holiday.year,
+                month=holiday.month,
+                day=holiday.day,
+                offset=holiday.offset,
+                observance=holiday.observance,
+                start_date=start_date_effective,
+                end_date=end_date_effective,
+                days_of_week=holiday.days_of_week,
+                tz=holiday.tz,
+            )
         elif isinstance(holiday, PandasHoliday):
-            return PandasHoliday(name=holiday.name, year=holiday.year, month=holiday.month, day=holiday.day,
-                                 offset=holiday.offset, observance=holiday.observance, start_date=start_date_effective,
-                                 end_date=end_date_effective, days_of_week=holiday.days_of_week)
+            return PandasHoliday(
+                name=holiday.name,
+                year=holiday.year,
+                month=holiday.month,
+                day=holiday.day,
+                offset=holiday.offset,
+                observance=holiday.observance,
+                start_date=start_date_effective,
+                end_date=end_date_effective,
+                days_of_week=holiday.days_of_week,
+            )
         else:
             raise NotImplementedError(f"Unsupported holiday type: {type(holiday)}")
 
-    def remove_day_from_rules(ts: pd.Timestamp, rules: List[Holiday]) -> List[Holiday]:
+    def remove_day_from_rules(ts: pd.Timestamp, rules: list[Holiday]) -> list[Holiday]:
         """
         Parameters
         ----------
         ts : pd.Timestamp
             The timestamp to exclude.
         rules : List[Holiday]
             The list of rules to modify.
@@ -657,28 +808,32 @@
         """
         # Determine any rules that coincide with ts.
         remove = [rule for rule in rules if is_holiday(rule, ts)]
 
         # Modify rules to exclude ts.
         for rule in remove:
             # Create copies of rule with end date set to ts - 1 day and ts + 1 day, respectively.
-            rule_before_ts = clone_holiday(rule, end_date=ts - pd.Timedelta(days=1))
+            rule_before_ts = clone_holiday(rule, end_date=ts + pd.Timedelta(days=-1))
             rule_after_ts = clone_holiday(rule, start_date=ts + pd.Timedelta(days=1))
             # Determine index of rule in list.
             rule_index = rules.index(rule)
             # Remove original rule.
             rules.pop(rule_index)
             # Add the new rules.
             rules.insert(rule_index, rule_before_ts)
             rules.insert(rule_index + 1, rule_after_ts)
 
         return rules
 
-    def add_special_session(name: str, ts: pd.Timestamp, t: datetime.time, special_sessions: List[Tuple[
-        datetime.time, List[Holiday]]]) -> List[Tuple[datetime.time, List[Holiday]]]:
+    def add_special_session(
+        name: str,
+        ts: pd.Timestamp,
+        t: datetime.time,
+        special_sessions: list[tuple[datetime.time, list[Holiday]]],
+    ) -> list[tuple[datetime.time, list[Holiday]]]:
         """
         Add a special session to the given list of special sessions.
 
         Parameters
         ----------
         name : str
             The name of the special session to add.
@@ -713,16 +868,19 @@
 
         # If the holiday was not added, add a new entry.
         if not added:
             special_sessions.append((t, [h]))
 
         return special_sessions
 
-    def remove_holiday(ts: pd.Timestamp, regular_holidays_rules: List[Holiday],
-                       adhoc_holidays: List[pd.Timestamp] = []) -> Tuple[List[Holiday], List[pd.Timestamp]]:
+    def remove_holiday(
+        ts: pd.Timestamp,
+        regular_holidays_rules: list[Holiday],
+        adhoc_holidays: list[pd.Timestamp] = [],
+    ) -> tuple[list[Holiday], list[pd.Timestamp]]:
         """
         Remove any holidays that coincide with ts.
 
         Parameters
         ----------
         ts : pd.Timestamp
             The timestamp to remove.
@@ -737,17 +895,22 @@
             The modified lists of regular and ad-hoc holidays.
         """
         regular_holidays_rules = remove_day_from_rules(ts, regular_holidays_rules)
         # Remove any ad-hoc holidays that coincide with ts, maybe.
         adhoc_holidays = [adhoc_ts for adhoc_ts in adhoc_holidays if adhoc_ts != ts]
         return regular_holidays_rules, adhoc_holidays
 
-    def remove_special_session(ts: pd.Timestamp, regular_special_sessions: List[Tuple[datetime.time, List[Holiday]]],
-                               adhoc_special_sessions: List[Tuple[datetime.time, pd.DatetimeIndex]]) -> Tuple[
-        List[Tuple[datetime.time, List[Holiday]]], List[Tuple[datetime.time, pd.DatetimeIndex]]]:
+    def remove_special_session(
+        ts: pd.Timestamp,
+        regular_special_sessions: list[tuple[datetime.time, list[Holiday]]],
+        adhoc_special_sessions: list[tuple[datetime.time, pd.DatetimeIndex]],
+    ) -> tuple[
+        list[tuple[datetime.time, list[Holiday]]],
+        list[tuple[datetime.time, pd.DatetimeIndex]],
+    ]:
         """
         Remove any special sessions that coincide with ts.
 
         Parameters
         ----------
         ts : pd.Timestamp
             The timestamp to remove.
@@ -763,131 +926,190 @@
         """
         # Loop over all times in regular_special_sessions.
         for _, rules in regular_special_sessions:
             if isinstance(rules, int):
                 # Check if the day of week corresponding to ts is the same as rules.
                 if ts.dayofweek == rules:
                     raise NotImplementedError(
-                        "Removing a special session date that corresponds to a day of week rule is not supported.")
+                        "Removing a special session date that corresponds to a day of week rule is not supported."
+                    )
             else:
                 # List of rules.
                 _ = remove_day_from_rules(ts, rules)
 
         # Remove any ad-hoc special sessions that coincide with ts.
-        adhoc_special_sessions = [(t, adhoc_ts.drop(ts, errors='ignore')) for t, adhoc_ts in adhoc_special_sessions]
+        adhoc_special_sessions = [
+            (t, adhoc_ts.drop(ts, errors="ignore"))
+            for t, adhoc_ts in adhoc_special_sessions
+        ]
 
         # Remove empty DateTime indices.
-        adhoc_special_sessions = [(t, adhoc_ts) for t, adhoc_ts in adhoc_special_sessions if not adhoc_ts.empty]
+        adhoc_special_sessions = [
+            (t, adhoc_ts)
+            for t, adhoc_ts in adhoc_special_sessions
+            if not adhoc_ts.empty
+        ]
 
         return regular_special_sessions, adhoc_special_sessions
 
     def __init__(self, *args, **kwargs):
         # Save adjusted properties. Initialize with copies of the original properties.
-        a = AdjustedProperties(regular_holidays=list(copy(regular_holidays_orig(self).rules)),
-                               adhoc_holidays=list(copy(adhoc_holidays_orig(self))),
-                               special_closes=[(t, d if isinstance(d, int) else list(copy(d.rules))) for t, d in
-                                               copy(special_closes_orig(self))],
-                               adhoc_special_closes=list(copy(adhoc_special_closes_orig(self))),
-                               special_opens=[(t, d if isinstance(d, int) else list(copy(d.rules))) for t, d in
-                                              copy(special_opens_orig(self))],
-                               adhoc_special_opens=list(copy(adhoc_special_opens_orig(self))))
+        a = AdjustedProperties(
+            regular_holidays=list(copy(regular_holidays_orig(self).rules)),
+            adhoc_holidays=list(copy(adhoc_holidays_orig(self))),
+            special_closes=[
+                (t, d if isinstance(d, int) else list(copy(d.rules)))
+                for t, d in copy(special_closes_orig(self))
+            ],
+            adhoc_special_closes=list(copy(adhoc_special_closes_orig(self))),
+            special_opens=[
+                (t, d if isinstance(d, int) else list(copy(d.rules)))
+                for t, d in copy(special_opens_orig(self))
+            ],
+            adhoc_special_opens=list(copy(adhoc_special_opens_orig(self))),
+        )
 
         # Get changeset from provider, maybe.
-        changeset: ChangeSet = changeset_provider() if changeset_provider is not None else None
+        changeset: Union[ChangeSet, None] = (
+            changeset_provider() if changeset_provider is not None else None
+        )
 
         # Set changeset to None if it is empty.
         if changeset is not None and len(changeset) <= 0:
             changeset = None
 
         if changeset is not None:
             # Remove all changed days from holidays, special opens, and special closes.
-            for ts in changeset.all_days:
-                a.regular_holidays, a.adhoc_holidays = remove_holiday(ts, a.regular_holidays, a.adhoc_holidays)
-                a.special_opens, a.adhoc_special_opens = remove_special_session(ts, a.special_opens,
-                                                                                a.adhoc_special_opens)
-                a.special_closes, a.adhoc_special_closes = remove_special_session(ts, a.special_closes,
-                                                                                  a.adhoc_special_closes)
+            for ts in changeset.all_days(include_meta=False):
+                a.regular_holidays, a.adhoc_holidays = remove_holiday(
+                    ts, a.regular_holidays, a.adhoc_holidays
+                )
+                a.special_opens, a.adhoc_special_opens = remove_special_session(
+                    ts, a.special_opens, a.adhoc_special_opens
+                )
+                a.special_closes, a.adhoc_special_closes = remove_special_session(
+                    ts, a.special_closes, a.adhoc_special_closes
+                )
 
             # Add holiday, special opens, and special closes.
-            for spec in changeset.add:
-                if spec.type == DayType.HOLIDAY:
+            for date, props in changeset.add.items():
+                if props.type == DayType.HOLIDAY:
                     # Add the holiday.
-                    a.regular_holidays.append(Holiday(spec.name, year=spec.date.year, month=spec.date.month,
-                                                      day=spec.date.day))
-                elif spec.type == DayType.SPECIAL_OPEN:
+                    a.regular_holidays.append(
+                        Holiday(
+                            props.name, year=date.year, month=date.month, day=date.day
+                        )
+                    )
+                elif props.type == DayType.SPECIAL_OPEN:
                     # Add the special open.
-                    a.special_opens = add_special_session(spec.name, spec.date, spec.time, a.special_opens)
-                elif spec.type == DayType.SPECIAL_CLOSE:
+                    a.special_opens = add_special_session(
+                        props.name, date, props.time, a.special_opens
+                    )
+                elif props.type == DayType.SPECIAL_CLOSE:
                     # Add the special close.
-                    a.special_closes = add_special_session(spec.name, spec.date, spec.time, a.special_closes)
+                    a.special_closes = add_special_session(
+                        props.name, date, props.time, a.special_closes
+                    )
 
         self._adjusted_properties = a
 
+        # Save meta.
+        self._meta = changeset.meta if changeset is not None else {}
+
         # Call upstream init method.
         init_orig(self, *args, **kwargs)
 
         # Set up monthly and quarterly expiries. This can only be done after holidays, special opens, and special closes
         # have been set up.
-        a.monthly_expiries = get_monthly_expiry_rules(day_of_week_expiry) if day_of_week_expiry is not None else []
-        a.quarterly_expiries = get_quadruple_witching_rules(day_of_week_expiry) if day_of_week_expiry is not None else []
+        a.monthly_expiries = (
+            get_monthly_expiry_rules(day_of_week_expiry)
+            if day_of_week_expiry is not None
+            else []
+        )
+        a.quarterly_expiries = (
+            get_quadruple_witching_rules(day_of_week_expiry)
+            if day_of_week_expiry is not None
+            else []
+        )
 
         if changeset is not None:
             # Remove all changed days from monthly and quarterly expiries.
-            for ts in changeset.all_days:
+            for ts in changeset.all_days(include_meta=False):
                 a.monthly_expiries, _ = remove_holiday(ts, a.monthly_expiries)
                 a.quarterly_expiries, _ = remove_holiday(ts, a.quarterly_expiries)
 
             # Add monthly and quarterly expiries.
-            for spec in changeset.add:
-                if spec.type == DayType.MONTHLY_EXPIRY:
+            for date, props in changeset.add.items():
+                if props.type == DayType.MONTHLY_EXPIRY:
                     # Add the monthly expiry.
-                    a.monthly_expiries.append(Holiday(spec.name, year=spec.date.year, month=spec.date.month,
-                                                      day=spec.date.day))
-                elif spec.type == DayType.QUARTERLY_EXPIRY:
+                    a.monthly_expiries.append(
+                        Holiday(
+                            props.name, year=date.year, month=date.month, day=date.day
+                        )
+                    )
+                elif props.type == DayType.QUARTERLY_EXPIRY:
                     # Add the quarterly expiry.
-                    a.quarterly_expiries.append(Holiday(spec.name, year=spec.date.year, month=spec.date.month,
-                                                        day=spec.date.day))
+                    a.quarterly_expiries.append(
+                        Holiday(
+                            props.name, year=date.year, month=date.month, day=date.day
+                        )
+                    )
 
         # Set up last trading days of the month.
-        a.last_trading_days_of_months = get_last_day_of_month_rules('last trading day of month')
+        a.last_trading_days_of_months = get_last_day_of_month_rules(
+            "last trading day of month"
+        )
 
         # Set up last regular trading days of the month. This can only be done after holidays, special opens,
         # special closes, monthly expiries, and quarterly expiries have been set up.
-        a.last_regular_trading_days_of_months = get_last_day_of_month_rules('last regular trading day of month')
+        a.last_regular_trading_days_of_months = get_last_day_of_month_rules(
+            "last regular trading day of month"
+        )
 
         # Save a calendar with all holidays and another one with all holidays and special business days for later use.
         # These calendars are needed to generate calendars for monthly expiries, quarterly expiries, last trading days
         # of the month, and last regular trading days of the month. Each of these calendars defines contains days that
         # need to be rolled back to a previous business day if they fall on a holiday and/or special business day.
         self._holidays_shared = get_holidays_calendar(self)
         self._holidays_and_special_business_days_shared = merge_calendars(
-            [get_holidays_calendar(self), get_special_opens_calendar(self), get_special_closes_calendar(self)])
+            [
+                get_holidays_calendar(self),
+                get_special_opens_calendar(self),
+                get_special_closes_calendar(self),
+            ]
+        )
 
     @property
     def regular_holidays(self) -> Union[HolidayCalendar, None]:
         return HolidayCalendar(rules=self._adjusted_properties.regular_holidays)
 
     @property
-    def adhoc_holidays(self) -> List[pd.Timestamp]:
+    def adhoc_holidays(self) -> list[pd.Timestamp]:
         return copy(self._adjusted_properties.adhoc_holidays)
 
     @property
-    def special_closes(self) -> List[Tuple[datetime.time, Union[HolidayCalendar, int]]]:
-        return [(t, rules if isinstance(rules, int) else HolidayCalendar(rules=rules)) for t, rules in self._adjusted_properties.special_closes]
+    def special_closes(self) -> list[tuple[datetime.time, Union[HolidayCalendar, int]]]:
+        return [
+            (t, rules if isinstance(rules, int) else HolidayCalendar(rules=rules))
+            for t, rules in self._adjusted_properties.special_closes
+        ]
 
     @property
-    def special_closes_adhoc(self) -> List[Tuple[datetime.time, pd.DatetimeIndex]]:
+    def special_closes_adhoc(self) -> list[tuple[datetime.time, pd.DatetimeIndex]]:
         return copy(self._adjusted_properties.adhoc_special_closes)
 
     @property
-    def special_opens(self) -> List[Tuple[datetime.time, Union[HolidayCalendar, int]]]:
-        return [(t, rules if isinstance(rules, int) else HolidayCalendar(rules=rules)) for t, rules in self._adjusted_properties.special_opens]
+    def special_opens(self) -> list[tuple[datetime.time, Union[HolidayCalendar, int]]]:
+        return [
+            (t, rules if isinstance(rules, int) else HolidayCalendar(rules=rules))
+            for t, rules in self._adjusted_properties.special_opens
+        ]
 
     @property
-    def special_opens_adhoc(self) -> List[Tuple[datetime.time, pd.DatetimeIndex]]:
+    def special_opens_adhoc(self) -> list[tuple[datetime.time, pd.DatetimeIndex]]:
         return copy(self._adjusted_properties.adhoc_special_opens)
 
     @property
     def weekend_days(self) -> Union[HolidayCalendar, None]:
         return get_weekend_days_calendar(self)
 
     @property
@@ -899,50 +1121,119 @@
         return get_special_opens_calendar(self)
 
     @property
     def special_closes_all(self) -> Union[HolidayCalendar, None]:
         return get_special_closes_calendar(self)
 
     @property
-    def monthly_expiries(self) -> Union[HolidayCalendar, None]:
-        return AdjustedHolidayCalendar(rules=self._adjusted_properties.monthly_expiries,
-                                       other=self._holidays_and_special_business_days_shared, weekmask=self.weekmask,
-                                       roll_fn=roll_one_day_same_month)
-
-    @property
-    def quarterly_expiries(self) -> Union[HolidayCalendar, None]:
-        return AdjustedHolidayCalendar(rules=self._adjusted_properties.quarterly_expiries,
-                                       other=self._holidays_and_special_business_days_shared, weekmask=self.weekmask,
-                                       roll_fn=roll_one_day_same_month)
-
-    @property
-    def last_trading_days_of_months(self) -> Union[HolidayCalendar, None]:
-        return AdjustedHolidayCalendar(rules=self._adjusted_properties.last_trading_days_of_months,
-                                       other=self._holidays_shared, weekmask=self.weekmask,
-                                       roll_fn=roll_one_day_same_month)
+    def monthly_expiries(self) -> Union[ExchangeCalendarsHolidayCalendar, None]:
+        return AdjustedHolidayCalendar(
+            rules=self._adjusted_properties.monthly_expiries,
+            other=self._holidays_and_special_business_days_shared,
+            weekmask=self.weekmask,
+            roll_fn=roll_one_day_same_month,
+        )
 
     @property
-    def last_regular_trading_days_of_months(self) -> Union[HolidayCalendar, None]:
-        return AdjustedHolidayCalendar(rules=self._adjusted_properties.last_regular_trading_days_of_months,
-                                       other=self._holidays_and_special_business_days_shared, weekmask=self.weekmask,
-                                       roll_fn=roll_one_day_same_month)
+    def quarterly_expiries(self) -> Union[ExchangeCalendarsHolidayCalendar, None]:
+        return AdjustedHolidayCalendar(
+            rules=self._adjusted_properties.quarterly_expiries,
+            other=self._holidays_and_special_business_days_shared,
+            weekmask=self.weekmask,
+            roll_fn=roll_one_day_same_month,
+        )
+
+    @property
+    def last_trading_days_of_months(
+        self,
+    ) -> Union[ExchangeCalendarsHolidayCalendar, None]:
+        return AdjustedHolidayCalendar(
+            rules=self._adjusted_properties.last_trading_days_of_months,
+            other=self._holidays_shared,
+            weekmask=self.weekmask,
+            roll_fn=roll_one_day_same_month,
+        )
+
+    @property
+    def last_regular_trading_days_of_months(
+        self,
+    ) -> Union[ExchangeCalendarsHolidayCalendar, None]:
+        return AdjustedHolidayCalendar(
+            rules=self._adjusted_properties.last_regular_trading_days_of_months,
+            other=self._holidays_and_special_business_days_shared,
+            weekmask=self.weekmask,
+            roll_fn=roll_one_day_same_month,
+        )
+
+    @validate_call(config={"arbitrary_types_allowed": True})
+    def meta(
+        self,
+        start: Union[TimestampLike, None] = None,
+        end: Union[TimestampLike, None] = None,
+    ) -> dict[pd.Timestamp, DayMeta]:
+        # Check that when start and end are both given, they are both timezone-aware or both timezone-naive.
+        if start and end:
+            if bool(start.tz) != bool(end.tz):
+                raise ValueError(
+                    "start and end must both be timezone-aware or both timezone-naive."
+                )
+
+            if start > end:
+                raise ValueError("start must be less than or equal to end.")
+
+        # Get timezone from start or end, if given.
+        tz = (start and start.tz) or (end and end.tz) or None
+
+        # Return a dictionary with all metadata for days in the given range. A day is considered to comprise the full
+        # period between midnight (inclusive) and the next midnight (exclusive). If that period overlaps with the given
+        # range, the day is included in the result.
+        #
+        # Note: The code assumes that ONE_DAY_MINUS_EPS gets applied to timezone-naive timestamps where it corresponds
+        # to (almost) a calendar day. The same may not be true for timezone-aware timestamps when the period includes
+        # e.g. a DST transition.
+        if tz:
+            return OrderedDict(
+                [
+                    (k, v)
+                    for k, v in self._meta.items()
+                    if (
+                        start is None
+                        or (k + ONE_DAY_MINUS_EPS).tz_localize(tz=self.tz) >= start
+                    )
+                    and (end is None or (k.tz_localize(tz=self.tz)) <= end)
+                ]
+            )
+        else:
+            return OrderedDict(
+                [
+                    (k, v)
+                    for k, v in self._meta.items()
+                    if (start is None or (k + ONE_DAY_MINUS_EPS) >= start)
+                    and (end is None or k <= end)
+                ]
+            )
 
     # Use type to create a new class.
-    extended = type(cls.__name__ + "Extended", (cls, ExtendedExchangeCalendar), {
-        "__init__": __init__,
-        "regular_holidays": regular_holidays,
-        "adhoc_holidays": adhoc_holidays,
-        "special_closes": special_closes,
-        "special_closes_adhoc": special_closes_adhoc,
-        "special_opens": special_opens,
-        "special_opens_adhoc": special_opens_adhoc,
-        "weekend_days": weekend_days,
-        "holidays_all": holidays_all,
-        "special_opens_all": special_opens_all,
-        "special_closes_all": special_closes_all,
-        "monthly_expiries": monthly_expiries,
-        "quarterly_expiries": quarterly_expiries,
-        "last_trading_days_of_months": last_trading_days_of_months,
-        "last_regular_trading_days_of_months": last_regular_trading_days_of_months
-    })
+    extended = type(
+        cls.__name__ + "Extended",
+        (cls, ExtendedExchangeCalendar),
+        {
+            "__init__": __init__,
+            "regular_holidays": regular_holidays,
+            "adhoc_holidays": adhoc_holidays,
+            "special_closes": special_closes,
+            "special_closes_adhoc": special_closes_adhoc,
+            "special_opens": special_opens,
+            "special_opens_adhoc": special_opens_adhoc,
+            "weekend_days": weekend_days,
+            "holidays_all": holidays_all,
+            "special_opens_all": special_opens_all,
+            "special_closes_all": special_closes_all,
+            "monthly_expiries": monthly_expiries,
+            "quarterly_expiries": quarterly_expiries,
+            "last_trading_days_of_months": last_trading_days_of_months,
+            "last_regular_trading_days_of_months": last_regular_trading_days_of_months,
+            "meta": meta,
+        },
+    )
 
     return extended
```

### Comparing `exchange_calendars_extensions-0.7.0/exchange_calendars_extensions/core/offset.py` & `exchange_calendars_extensions-0.8.0/exchange_calendars_extensions/core/offset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from abc import ABC, abstractmethod
 from datetime import datetime, date
-from typing import Type
 
 import pandas as pd
 from pandas._libs.tslibs import localize_pydatetime
 from pandas._libs.tslibs.offsets import Easter, apply_wraps
 
-from exchange_calendars_extensions.core.util import get_month_name, get_day_of_week_name, third_day_of_week_in_month, \
-    last_day_in_month
+from exchange_calendars_extensions.core.util import (
+    get_month_name,
+    get_day_of_week_name,
+    third_day_of_week_in_month,
+    last_day_in_month,
+)
 
 
 class AbstractHolidayOffset(Easter, ABC):
-
     @staticmethod
     def _is_normalized(dt):
         if dt.hour != 0 or dt.minute != 0 or dt.second != 0 or dt.microsecond != 0:
             # Regardless of whether dt is datetime vs Timestamp
             return False
         if isinstance(dt, pd.Timestamp):
             return dt.nanosecond == 0
@@ -59,19 +61,21 @@
 
     def is_on_offset(self, dt):
         if self.normalize and not AbstractHolidayOffset._is_normalized(dt):
             return False
         return date(dt.year, dt.month, dt.day) == self.holiday(dt.year).to_pydate()
 
 
-def get_third_day_of_week_in_month_offset_class(day_of_week: int, month: int) -> Type[AbstractHolidayOffset]:
+def get_third_day_of_week_in_month_offset_class(
+    day_of_week: int, month: int
+) -> type[AbstractHolidayOffset]:
     """
     Return a new class that represents an offset that, when applied to the first day of a year, results in the third
     given day of the week in the given month.
-    
+
     For example, to get the offset for the third Friday in June, call this function with day_of_week=4 and month=6. On
     many exchanges, this will be the quadruple witching day for the second quarter of the year.
 
     Parameters
     ----------
     day_of_week : int
         The day of the week, where 0 is Monday and 6 is Sunday.
@@ -93,17 +97,21 @@
     # Get name of day of week.
     day_of_week_name = get_day_of_week_name(day_of_week)
 
     # Get name of month.
     month_name = get_month_name(month)
 
     # Create the new class.
-    offset = type(f"MonthlyExpiry{month_name}{day_of_week_name}Offset", (AbstractHolidayOffset,), {
-        "holiday": holiday,
-    })
+    offset = type(
+        f"MonthlyExpiry{month_name}{day_of_week_name}Offset",
+        (AbstractHolidayOffset,),
+        {
+            "holiday": holiday,
+        },
+    )
 
     # Return the new class.
     return offset
 
 
 # A dictionary of dictionaries that maps day of week and month to corresponding offset class as returned by
 # get_third_day_of_week_in_month_offset_class. Used as an internal cache to avoid unnecessarily creating classes with
@@ -114,46 +122,59 @@
 # 1 = January). To instantiate the offset, use the following: OffsetClasses[4][6]().
 #
 # The offset classes can be used to define typical expiry days (options, futures, et cetera) on exchanges which often
 # happen on the third Friday or Thursday in a month. The quarterly expiry days in months March, June, September, and
 # December are also called quadruple witching.
 #
 # Currently, includes cases for Monday to Friday which should cover all real-world scenarios.
-ThirdDayOfWeekInMonthOffsetClasses = {day_of_week: {month: get_third_day_of_week_in_month_offset_class(day_of_week, month) for month in range(1, 13)} for day_of_week in range(5)}
+ThirdDayOfWeekInMonthOffsetClasses = {
+    day_of_week: {
+        month: get_third_day_of_week_in_month_offset_class(day_of_week, month)
+        for month in range(1, 13)
+    }
+    for day_of_week in range(5)
+}
 
 
-def get_last_day_of_month_offset_class(month: int) -> Type[AbstractHolidayOffset]:
+def get_last_day_of_month_offset_class(month: int) -> type[AbstractHolidayOffset]:
     """
     Return a new class that represents an offset that, when applied to the first day of a year, results in the last
     day of the given month.
 
     Parameters
     ----------
     month : int
         The month, where 1 is January and 12 is December.
 
     Returns
     -------
     Type[AbstractHolidayOffset]
         A new class that represents the offset.
     """
+
     def holiday(self, year) -> date:
         """
         Return a function that returns the last day of the month for a given year.
         """
         return last_day_in_month(month, year)
 
     # Get name of month.
     month_name = get_month_name(month)
 
     # Create the new class.
-    offset = type(f"LastDayOfMonth{month_name}Offset", (AbstractHolidayOffset,), {
-        "holiday": holiday,
-    })
+    offset = type(
+        f"LastDayOfMonth{month_name}Offset",
+        (AbstractHolidayOffset,),
+        {
+            "holiday": holiday,
+        },
+    )
 
     # Return the new class.
     return offset
 
 
 # A dictionary that maps month to corresponding offset class as returned by get_last_day_of_month_offset_class. Used
 # as an internal cache to avoid unnecessarily creating classes with the same parameters.
-LastDayOfMonthOffsetClasses = {month: get_last_day_of_month_offset_class(month) for month in range(1, 13)}
+LastDayOfMonthOffsetClasses = {
+    month: get_last_day_of_month_offset_class(month) for month in range(1, 13)
+}
```

### Comparing `exchange_calendars_extensions-0.7.0/exchange_calendars_extensions/core/util.py` & `exchange_calendars_extensions-0.8.0/exchange_calendars_extensions/core/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,17 +15,28 @@
     -------
     str
         Name of month.
     """
     if month < 1 or month > 12:
         raise ValueError("Month must be between 1 and 12.")
 
-    month_name = \
-    ["January", "February", "March", "April", "May", "June", "July", "August", "September", "October", "November",
-     "December"][month - 1]
+    month_name = [
+        "January",
+        "February",
+        "March",
+        "April",
+        "May",
+        "June",
+        "July",
+        "August",
+        "September",
+        "October",
+        "November",
+        "December",
+    ][month - 1]
 
     return month_name
 
 
 def get_day_of_week_name(day_of_week: int) -> str:
     """
     Convert day of week number to name.
@@ -39,15 +50,23 @@
     -------
     str
         Name of day of week.
     """
     if day_of_week < 0 or day_of_week > 6:
         raise ValueError("Day of week must be between 0 and 6.")
 
-    day_of_week_name = ["Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday", "Sunday"][day_of_week]
+    day_of_week_name = [
+        "Monday",
+        "Tuesday",
+        "Wednesday",
+        "Thursday",
+        "Friday",
+        "Saturday",
+        "Sunday",
+    ][day_of_week]
 
     return day_of_week_name
 
 
 def third_day_of_week_in_month(day_of_week: int, month: int, year: int) -> date:
     """
     Return the third given day of the week in the given month and year.
@@ -91,8 +110,10 @@
         the year, must be an integer
 
     Returns
     -------
     datetime.date
         the datetime.date representing the last day in the given month.
     """
-    return (date(year, month, 1) + timedelta(days=32)).replace(day=1) - timedelta(days=1)
+    return (date(year, month, 1) + timedelta(days=32)).replace(day=1) - timedelta(
+        days=1
+    )
```

### Comparing `exchange_calendars_extensions-0.7.0/pyproject.toml` & `exchange_calendars_extensions-0.8.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "exchange-calendars-extensions"
-version = "0.7.0"
+version = "0.8.0"
 description = "Extensions of the exchange-calendars package"
 license = "Apache-2.0"
 authors = ["Jens Keiner <jens.keiner@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/jenskeiner/exchange_calendars_extensions/"
 repository = "https://github.com/jenskeiner/exchange_calendars_extensions/"
 documentation = "https://github.com/jenskeiner/exchange_calendars_extensions/tree/main/docs/"
@@ -18,49 +18,40 @@
     "License :: OSI Approved :: Apache Software License",
     "Intended Audience :: Developers",
     "Intended Audience :: Financial and Insurance Industry",
     "Intended Audience :: Information Technology",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 packages = [{include = "exchange_calendars_extensions"}]
 
 [tool.poetry.dependencies]
-python = "~=3.8"
-exchange-calendars-extensions-api = ">=0.2.0,<1.0.0"
+python = "~=3.9"
+exchange-calendars-extensions-api = ">=0.4.0,<1"
 exchange-calendars = ">=4.0.1,<5"
 typing-extensions = ">=4.0,<5"
 pydantic = ">=2.0,<3"
 
 [tool.poetry.group.dev.dependencies]
-pytest = ">=7.3.1,<8.1.0"
-pytest-mock = ">=3.11.1,<3.13.0"
-pytest-cov = "~=4.1.0"
-pre-commit = ">=3.3.3,<3.6.0"
+pytest = ">=7.3.1,<8.3.0"
+pytest-mock = ">=3.11.1,<3.15.0"
+pytest-cov = ">=4.1,<5.1"
+pre-commit = ">=3.3.3,<3.8.0"
 
 [tool.pytest.ini_options]
 addopts = "--cov=exchange_calendars_extensions --cov-report=term-missing"
 
 [tool.ruff]
-# Enable pycodestyle (`E`) and Pyflakes (`F`) codes by default.
-select = ["E", "F"]
-ignore = ["E501"]
-
-# Allow autofix for all enabled rules (when `--fix`) is provided.
-fixable = ["A", "B", "C", "D", "E", "F", "G", "I", "N", "Q", "S", "T", "W", "ANN", "ARG", "BLE", "COM", "DJ", "DTZ", "EM", "ERA", "EXE", "FBT", "ICN", "INP", "ISC", "NPY", "PD", "PGH", "PIE", "PL", "PT", "PTH", "PYI", "RET", "RSE", "RUF", "SIM", "SLF", "TCH", "TID", "TRY", "UP", "YTT"]
-unfixable = []
-
 # Exclude a variety of commonly ignored directories.
 exclude = [
     ".bzr",
     ".direnv",
     ".eggs",
     ".git",
     ".git-rewrite",
@@ -81,16 +72,25 @@
     "node_modules",
     "venv",
 ]
 
 # Same as Black.
 line-length = 88
 
+# Assume Python 3.9.
+target-version = "py39"
+
+
+[lint]
+# Enable pycodestyle (`E`) and Pyflakes (`F`) codes by default.
+select = ["E", "F"]
+ignore = ["E501"]
+
+# Allow autofix for all enabled rules (when `--fix`) is provided.
+fixable = ["A", "B", "C", "D", "E", "F", "G", "I", "N", "Q", "S", "T", "W", "ANN", "ARG", "BLE", "COM", "DJ", "DTZ", "EM", "ERA", "EXE", "FBT", "ICN", "INP", "ISC", "NPY", "PD", "PGH", "PIE", "PL", "PT", "PTH", "PYI", "RET", "RSE", "RUF", "SIM", "SLF", "TCH", "TID", "TRY", "UP", "YTT"]
+unfixable = []
+
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
-# Assume Python 3.10.
-target-version = "py38"
-
-[tool.ruff.mccabe]
 # Unlike Flake8, default to a complexity level of 10.
-max-complexity = 10
+mccabe = 10
```

### Comparing `exchange_calendars_extensions-0.7.0/PKG-INFO` & `exchange_calendars_extensions-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: exchange-calendars-extensions
-Version: 0.7.0
+Version: 0.8.0
 Summary: Extensions of the exchange-calendars package
 Home-page: https://github.com/jenskeiner/exchange_calendars_extensions/
 License: Apache-2.0
 Keywords: exchange,calendar,trading,holidays
 Author: Jens Keiner
 Author-email: jens.keiner@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: exchange-calendars (>=4.0.1,<5)
-Requires-Dist: exchange-calendars-extensions-api (>=0.2.0,<1.0.0)
+Requires-Dist: exchange-calendars-extensions-api (>=0.4.0,<1)
 Requires-Dist: pydantic (>=2.0,<3)
 Requires-Dist: typing-extensions (>=4.0,<5)
 Project-URL: Documentation, https://github.com/jenskeiner/exchange_calendars_extensions/tree/main/docs/
 Project-URL: Repository, https://github.com/jenskeiner/exchange_calendars_extensions/
 Description-Content-Type: text/markdown
 
 # exchange-calendars-extensions
```

