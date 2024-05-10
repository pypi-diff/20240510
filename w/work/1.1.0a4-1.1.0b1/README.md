# Comparing `tmp/work-1.1.0a4.tar.gz` & `tmp/work-1.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "work-1.1.0a4.tar", max compression
+gzip compressed data, was "work-1.1.0b1.tar", max compression
```

## Comparing `work-1.1.0a4.tar` & `work-1.1.0b1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     1033 2022-08-29 19:21:01.200221 work-1.1.0a4/README.md
--rw-r--r--   0        0        0      594 2024-05-08 18:57:26.331745 work-1.1.0a4/pyproject.toml
--rw-r--r--   0        0        0    92536 2024-05-08 18:57:26.327746 work-1.1.0a4/src/work.py
--rw-r--r--   0        0        0        0 2021-02-24 12:12:04.352563 work-1.1.0a4/src/work_components/__init__.py
--rw-r--r--   0        0        0    24509 2024-05-08 18:57:26.323745 work-1.1.0a4/src/work_components/arguments.py
--rw-r--r--   0        0        0     2188 2024-05-08 18:57:26.331745 work-1.1.0a4/src/work_components/consts.py
--rw-r--r--   0        0        0    22107 2024-05-08 18:57:26.327746 work-1.1.0a4/src/work_components/container.py
--rw-r--r--   0        0        0        0 2022-08-23 18:01:16.135701 work-1.1.0a4/src/work_components/dao/__init__.py
--rw-r--r--   0        0        0    17276 2024-05-08 18:57:26.323745 work-1.1.0a4/src/work_components/dao/core.py
--rw-r--r--   0        0        0      268 2024-05-08 18:57:26.323745 work-1.1.0a4/src/work_components/dao/env.py
--rw-r--r--   0        0        0     1641 2024-05-08 18:57:26.323745 work-1.1.0a4/src/work_components/dao/flags.py
--rw-r--r--   0        0        0    11501 2024-05-08 18:57:26.323745 work-1.1.0a4/src/work_components/dao/rc.py
--rw-r--r--   0        0        0    10484 2024-05-08 18:57:26.323745 work-1.1.0a4/src/work_components/dao/recess.py
--rw-r--r--   0        0        0     6236 2024-05-08 18:57:26.323745 work-1.1.0a4/src/work_components/dt_parse.py
--rw-r--r--   0        0        0     4470 2024-04-08 18:05:30.527145 work-1.1.0a4/src/work_components/migrate.py
--rw-r--r--   0        0        0      320 2024-04-10 12:10:12.266685 work-1.1.0a4/src/work_components/protocols.py
--rw-r--r--   0        0        0     2648 2024-05-08 18:57:26.323745 work-1.1.0a4/src/work_components/timestamps.py
--rw-r--r--   0        0        0     8065 2024-05-08 18:57:26.323745 work-1.1.0a4/src/work_components/util.py
--rw-r--r--   0        0        0     1614 1970-01-01 00:00:00.000000 work-1.1.0a4/PKG-INFO
+-rw-r--r--   0        0        0     1033 2022-08-29 19:21:01.200221 work-1.1.0b1/README.md
+-rw-r--r--   0        0        0      594 2024-05-10 14:25:40.109274 work-1.1.0b1/pyproject.toml
+-rw-r--r--   0        0        0    91750 2024-05-10 14:24:35.320649 work-1.1.0b1/src/work.py
+-rw-r--r--   0        0        0        0 2021-02-24 12:12:04.352563 work-1.1.0b1/src/work_components/__init__.py
+-rw-r--r--   0        0        0    24509 2024-05-10 10:13:29.676889 work-1.1.0b1/src/work_components/arguments.py
+-rw-r--r--   0        0        0     2188 2024-05-10 14:25:32.289198 work-1.1.0b1/src/work_components/consts.py
+-rw-r--r--   0        0        0    22908 2024-05-10 14:13:32.158045 work-1.1.0b1/src/work_components/container.py
+-rw-r--r--   0        0        0        0 2022-08-23 18:01:16.135701 work-1.1.0b1/src/work_components/dao/__init__.py
+-rw-r--r--   0        0        0    16504 2024-05-10 14:24:35.320649 work-1.1.0b1/src/work_components/dao/core.py
+-rw-r--r--   0        0        0      268 2024-05-09 22:17:55.296856 work-1.1.0b1/src/work_components/dao/env.py
+-rw-r--r--   0        0        0     1641 2024-05-09 22:17:55.296856 work-1.1.0b1/src/work_components/dao/flags.py
+-rw-r--r--   0        0        0     8513 2024-05-09 22:17:55.296856 work-1.1.0b1/src/work_components/dao/rc.py
+-rw-r--r--   0        0        0    10484 2024-05-09 22:17:55.296856 work-1.1.0b1/src/work_components/dao/recess.py
+-rw-r--r--   0        0        0     1734 2024-05-09 22:17:55.296856 work-1.1.0b1/src/work_components/dt_format.py
+-rw-r--r--   0        0        0     6236 2024-05-09 22:17:55.296856 work-1.1.0b1/src/work_components/dt_parse.py
+-rw-r--r--   0        0        0     3982 2024-05-10 14:24:35.320649 work-1.1.0b1/src/work_components/migrate.py
+-rw-r--r--   0        0        0      525 2024-05-10 14:24:35.320649 work-1.1.0b1/src/work_components/protocols.py
+-rw-r--r--   0        0        0     2660 2024-05-10 14:24:35.320649 work-1.1.0b1/src/work_components/timestamps.py
+-rw-r--r--   0        0        0     8065 2024-05-09 22:17:55.300856 work-1.1.0b1/src/work_components/util.py
+-rw-r--r--   0        0        0     1614 1970-01-01 00:00:00.000000 work-1.1.0b1/PKG-INFO
```

### Comparing `work-1.1.0a4/README.md` & `work-1.1.0b1/README.md`

 * *Files identical despite different names*

### Comparing `work-1.1.0a4/pyproject.toml` & `work-1.1.0b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "work"
-version = "1.1.0a4"
+version = "1.1.0b1"
 description = "Manual time tracking via a CLI that works similarly to git."
 authors = ["vauhochzett <vauhoch@zett.cc>"]
 readme = "README.md"
 homepage = "https://vauhoch.zett.cc/work/"
 packages = [
     { include = "work.py", from = "src" },
     { include = "work_components", from = "src" },
```

### Comparing `work-1.1.0a4/src/work.py` & `work-1.1.0b1/src/work.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     List,
     Optional,
     Set,
     Tuple,
     cast,
 )
 
+import work_components.dt_format as dt_format
 import work_components.timestamps as ts
 from work_components import consts, dt_parse, migrate, util
 from work_components.arguments import (
     ADD_NAME,
     MAINTENANCE_NAMES,
     START_NAME,
     STOP_NAME,
@@ -48,25 +49,21 @@
     sort_and_merge,
 )
 from work_components.dao import env
 from work_components.dao.core import WorkDao
 from work_components.dao.flags import Flags
 from work_components.dao.rc import RC
 from work_components.dao.recess import Holiday, RecessDao, ReducedHourDay, Vacation
+from work_components.dt_format import DATE_FORMAT, DATE_FORMAT_FULL, TIME_FORMAT
 from work_components.util import Color, PrinTable
 
 __version__: str = consts.VERSION
 
 assert sys.version_info >= (3, 8)
 
-# Formats
-TIME_FORMAT = "%H:%M"
-DATE_FORMAT = "%d.%m.%Y"
-DATE_FORMAT_FULL = "%A, " + DATE_FORMAT
-
 
 class Work:
     """Main class"""
 
     # Allow external access to debug flag
     debug: bool = False
 
@@ -120,27 +117,24 @@
         no_set_flags: bool = env.get_bool(consts.ENV_NO_SET_FLAGS)
         self.flags = Flags(flag_file, no_set_flags)
 
         # Connect DAO with normal or debug dir and load RC file
         self.base_dir = DIRECTORY if not Work.debug else DIRECTORY_DEBUG
         self._connect(base_dir=self.base_dir)
 
-        # Migrate RC file
-        self.configuration.migrate(self.flags)
-
         # Only verify the protocol and state for non-maintenance modes
         if args.mode not in MAINTENANCE_NAMES:
             self.run_checks()
 
-        # Migrate records files to UTF-8 and \n-newlines
-        self.dao.migrate_records_encoding(self.flags)
-
         # Print "what's new" message once for each release
         migrate.print_whats_new_in(__version__, self.flags)
 
+        # Offer to migrate entries
+        migrate.offer_midnight_migration_if_not_denied(self.flags, self.dao)
+
         # Check for use of deprecated flags
         for deprecated_flag in ["--date", "-D"]:
             if deprecated_flag in sys.argv:
                 print(
                     f"{Color.color('Warning', Color.ORANGE)}: The flag {deprecated_flag} "
                     "has been deprecated and will be removed in the future."
                 )
@@ -169,15 +163,15 @@
             or self._minutes_active_run() <= (8 * 60)
         ):
             return
 
         # Probably forgot to stop a run – prevent surprises when trying to switch or add
         print(
             "Invalid state detected!\n  A run started at "
-            f"{self._readable_dt(active_start)} is still active.\n"
+            f"{dt_format.readable_dt(active_start)} is still active.\n"
         )
 
         # Read input, strip and lower
         user_says: str = (
             input(
                 "Press [Enter] to end the run and add it to log, or\n"
                 'Enter "cancel" to cancel it.\n\n> '
@@ -215,15 +209,15 @@
 
         category: str = input("Category? (leave empty for none): ")
         message: str = input("Message?  (leave empty for none): ")
         run_length: float = self._stop(
             end_time=end_time, category=category, message=message
         )
         print(
-            f"Stopped work at {self._readable_dt(end_time)} "
+            f"Stopped work at {dt_format.readable_dt(end_time)} "
             f"({self._timedelta_str(run_length)} recorded)"
         )
 
     ### Argument parsing / Step two ###
 
     def get_single_time(self, args) -> dt.datetime:
         """Resolve the single time argument (start, stop, switch)."""
@@ -344,15 +338,15 @@
     # start #
 
     def start(self, args) -> None:
         """Start the protocol based on the given arguments."""
 
         start_time: dt.datetime = self.get_single_time(args)
         self._start(start_time=start_time, force=args.force, dry_run=args.dry_run)
-        print(f"Started work at {self._readable_dt(start_time)}")
+        print(f"Started work at {dt_format.readable_dt(start_time)}")
 
     def ensure_valid_start_time(
         self,
         start_time: dt.datetime,
         action: str = "start work",
         time_desc: str = "starting time",
     ) -> None:
@@ -402,15 +396,15 @@
             end_time=end_time,
             category=args.category,
             message=args.message,
             force=args.force,
             dry_run=args.dry_run,
         )
         print(
-            f"Stopped work at {self._readable_dt(end_time)} "
+            f"Stopped work at {dt_format.readable_dt(end_time)} "
             f"({self._timedelta_str(run_length)} recorded)"
         )
 
     def _stop(
         self,
         end_time: dt.datetime,
         category: str,
@@ -471,20 +465,21 @@
                 end_time=end_time,
                 category=args.category,
                 message=args.message,
                 force=args.force,
             )
 
         formatted_start: str = start_time.strftime(TIME_FORMAT)
-        if not ts.date_equals(start_time, end_time):
-            formatted_start = self._readable_dt(start_time)
+        # We specifically do not use ts.date_equals, as this also applies to midnight.
+        if start_time.date() != end_time.date():
+            formatted_start = dt_format.readable_dt(start_time)
         print(
             "Added a record from {} to {}".format(
                 formatted_start,
-                self._readable_dt(end_time),
+                dt_format.readable_dt(end_time),
             )
         )
 
     def _can_i_add_this(
         self,
         start_time: dt.datetime,
         end_time: dt.datetime,
@@ -538,23 +533,23 @@
             message=args.message,
             force=args.force,
             dry_run=args.dry_run,
         )
 
         if not args.start:
             print(
-                f"Switched work at {self._readable_dt(switch_time)} "
+                f"Switched work at {dt_format.readable_dt(switch_time)} "
                 f"({self._timedelta_str(run_length)} recorded)"
             )
         else:
             print(
                 "Stopped work at {} ({} recorded) and restarted at {}".format(
                     switch_time.strftime(TIME_FORMAT),
                     self._timedelta_str(run_length),
-                    self._readable_dt(restart_time),
+                    dt_format.readable_dt(restart_time),
                 )
             )
 
     def _switch(
         self,
         switch_time: dt.datetime,
         restart_time: dt.datetime,
@@ -656,19 +651,20 @@
         output: str
 
         if active_start is None:
             output = "Inactive"
         elif active_start > dt.datetime.now():
             output = (
                 Color.color("Scheduled", Color.BLUE)
-                + f" to start work at {self._readable_dt(active_start)}"
+                + f" to start work at {dt_format.readable_dt(active_start)}"
             )
         else:
             output = Color.color("Active", Color.BLUE) + " since {} ({})".format(
-                self._readable_dt(active_start), self._timedelta_str(minutes_active_run)
+                dt_format.readable_dt(active_start),
+                self._timedelta_str(minutes_active_run),
             )
 
         if args.oneline:
             print(output)
             return
 
         total_minutes_worked = minutes_protocol + minutes_active_run
@@ -828,15 +824,15 @@
                 rounding_mode=dt_parse.RoundingMode.UP,
             )
 
             # Verify input correctness
             if target.date() < today or target < prospective_start:
                 raise InvalidOperationWarning(
                     "The target time supplied to --until needs to be after the "
-                    f"(prospective) start time {self._readable_dt(prospective_start)}."
+                    f"(prospective) start time {dt_format.readable_dt(prospective_start)}."
                 )
 
             optional_output += new_section()
             optional_output += self._get_hours_worked_until_msg(
                 target_time=target, hours_data=hours_data
             )
 
@@ -1274,15 +1270,15 @@
         :param active_start_to_include: If given, the "active run" will be added to the output.
         """
 
         if active_run_to_include is not None and active_run_to_include.date != day:
             raise ValueError("Invalid day for active_start_to_include passed.")
 
         # Add the year to the printout if it's not the current year
-        date_fmt: str = self._date_fmt(day)
+        date_fmt: str = dt_format.date_fmt(day)
 
         # Merge entries for only_time
         record_count: int = len(records)
         if only_time:
             for i in range(len(records)):  # pylint: disable=consider-using-enumerate
                 records[i] = Record(start=records[i].start, end=records[i].end)
             records = sort_and_merge(entries=records, output=False)
@@ -1766,29 +1762,21 @@
 
         edited: int = 0
         modification_buffer: List[Tuple[Record, Record]] = []
 
         for record in selected_records:
             print(f"\n > Selected record: {record.strf(TIME_FORMAT)}\n")
 
-            new_start: dt.datetime = self._new_time_or_not(
-                time_name="start", old_val=record.start
-            )
+            new_start: dt.datetime = self._new_time_or_not("start", record.start)
             new_end: dt.datetime = self._new_time_or_not(
-                time_name="end", old_val=record.end
-            )
-            new_category: str = self._new_text_field_or_not(
-                field_name="category", old_val=record.category
-            )
-            new_message: str = self._new_text_field_or_not(
-                field_name="message", old_val=record.message
-            )
-            new_record: Record = Record(
-                start=new_start, end=new_end, category=new_category, message=new_message
+                "end", record.end, base=record.start
             )
+            new_category: str = self._new_text_field_or_not("category", record.category)
+            new_message: str = self._new_text_field_or_not("message", record.message)
+            new_record: Record = Record(new_start, new_end, new_category, new_message)
 
             if new_record == record:
                 print("Unchanged")
                 continue
 
             # Check if the edited entry would overlap the currently active run
             active_start: Optional[dt.datetime] = self.dao.get_start_time()
@@ -1831,29 +1819,39 @@
             raise InvalidOperationWarning(
                 "Edits would lead to overlap of the following entries:\n"
                 f"  {ovl_err.left.strf(TIME_FORMAT)}\n"
                 f"  {ovl_err.right.strf(TIME_FORMAT)}\n"
                 "Aborting."
             ) from ovl_err
 
+        # We implement the dry run indirectly, by reverting the changes again.
+        if args.dry_run:
+            shadow.overwrite(protocol)
+
         self._end_manipulation_mode(num_edited=edited, verb="edited")
 
-    def _new_time_or_not(self, time_name: str, old_val: dt.datetime) -> dt.datetime:
+    def _new_time_or_not(
+        self, time_name: str, old_val: dt.datetime, base: Optional[dt.datetime] = None
+    ) -> dt.datetime:
         """User interaction: Ask for a new time (or no change)."""
 
-        user_choice = input(f"New {time_name} time? ({old_val.strftime(TIME_FORMAT)}) ")
+        message = f"New {time_name} time? ({dt_format.readable_t(old_val, base)}) "
+        user_choice = input(message)
         if user_choice == "":
             return old_val
 
         try:
-            return dt_parse.resolve_time_argument(
+            new_val = dt_parse.resolve_time_argument(
                 argument=user_choice,
                 baseline_date=old_val.date(),
                 rounding_mode=dt_parse.RoundingMode.NONE,
             )
+            if not ts.date_equals(old_val, new_val):
+                raise ValueError("New time must lie on the same date (<= 24:00).")
+            return new_val
         except ValueError as val_err:
             print(f"{Color.color('Parse error', Color.RED)}: {str(val_err)}")
             return self._new_time_or_not(time_name, old_val)
 
     def _new_text_field_or_not(self, field_name: str, old_val: str) -> str:
         """User interaction: Ask for a new text field, field removal, or no change."""
 
@@ -2069,15 +2067,15 @@
                 + "\nShould non-working days be removed from the vacation before it "
                 + "is added?\n[Y/n] "
             )
             if user_says.lower().strip() != "n":
                 days_to_remove.extend(non_working_in_period)
 
         if holidays_in_period:
-            user_says: str = input(
+            user_says = input(
                 "The vacation overlaps with configured holiday(s): "
                 + ", ".join(
                     [hdip.strftime("%d.%m.%Y (%A)") for hdip in holidays_in_period]
                 )
                 + "\nHolidays must be removed from the vacation before it can be "
                 + "added. Remove?\n[Y/n] "
             )
@@ -2197,42 +2195,14 @@
                 print(f"{macro:<} = {expansion}")
         # When adding a new option, make sure to update the "choices" of the ArgumentParser!
         else:
             raise NotImplementedError(f"Target {s_target} unknown")
 
     ### Shared functionality ###
 
-    def _readable_dt(self, date_and_time: dt.datetime) -> str:
-        """
-        Convert the given datetime.datetime to a human readable string with the time
-        and day.
-        """
-        result: str = date_and_time.strftime(TIME_FORMAT)
-        result += " " + self._readable_d(date_and_time.date())
-        return result
-
-    @staticmethod
-    def _readable_d(date: dt.date) -> str:
-        """Convert the given datetime.date to a human readable string with the day."""
-        if date == dt.date.today():
-            return "today"
-        elif date == (dt.date.today() + dt.timedelta(days=1)):
-            return "tomorrow"
-        elif date == (dt.date.today() - dt.timedelta(days=1)):
-            return "yesterday"
-        else:
-            return "on " + date.strftime(DATE_FORMAT_FULL)
-
-    @staticmethod
-    def _date_fmt(date_to_format: dt.date) -> str:
-        """Return date format that only includes the year if it's not the current one."""
-        if date_to_format.year == dt.date.today().year:
-            return "%d.%m."
-        return "%d.%m.%Y"
-
     def _minutes_logged_on(self, requested_date: dt.date) -> float:
         """Return the minutes logged on the requested date."""
         the_days_records: List[Record] = self.dao.get_entries(date=requested_date)
         return self._minutes_worked(the_days_records)
 
     @staticmethod
     def _minutes_worked(records: List[Record]) -> float:
```

### Comparing `work-1.1.0a4/src/work_components/arguments.py` & `work-1.1.0b1/src/work_components/arguments.py`

 * *Files identical despite different names*

### Comparing `work-1.1.0a4/src/work_components/consts.py` & `work-1.1.0b1/src/work_components/consts.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """Shared constants"""
 
 import os
 import pathlib
 from typing import List, Tuple
 
-VERSION: str = "1.1.0a4"
+VERSION: str = "1.1.0b1"
 RECORDS_VERSION: int = 3
 
 # Directories
 PARENT_DIR: pathlib.Path = pathlib.Path("~", ".local", "share").expanduser()
 DIRECTORY: pathlib.Path = PARENT_DIR.joinpath("work")
 DIRECTORY_DEBUG: pathlib.Path = PARENT_DIR.joinpath("debug", "work")
```

### Comparing `work-1.1.0a4/src/work_components/container.py` & `work-1.1.0b1/src/work_components/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import pathlib
 import re
 import shutil
 import tempfile
 from typing import Iterable, List, Optional
 
 import work_components.timestamps as ts
-from work_components import migrate, util
+from work_components import util
 from work_components.consts import (
     DATETIME_FORMAT,
     DAY_FILE_PATTERN,
     MONTH_DIR_PATTERN,
     PROTOCOL_FILE_EXTENSION,
     TIME_FORMAT,
     YEAR_DIR_PATTERN,
@@ -154,15 +154,14 @@
     @staticmethod
     def from_protocol_row(row):
         # type: (List[str]) -> Record
         """
         Parse one row of a protocol file in the form of
         ["start", "end", "category", "message"].
         """
-        migrate.raise_old_protocol_version(row)
 
         if len(row) != 4:
             raise Record.CorruptedProtocolRowError(
                 f"expected 4 elements, got {len(row)}"
             )
 
         start: str
@@ -179,14 +178,33 @@
         )
 
     @staticmethod
     def one_minute_record(start: dt.datetime):
         """Create a `Record` with the given `start` and a length of one minute."""
         return Record(start, start + dt.timedelta(minutes=1))
 
+    @staticmethod
+    def split_by_date(start, end, category=None, message=None):
+        # type: (dt.datetime, dt.datetime, Optional[str], Optional[str]) -> List[Record]
+        """Create valid Record instances even if the given `start` and `end` lie on
+        different dates by splitting the timeframe up by date."""
+        if ts.date_equals(start, end):
+            return [Record(start, end, category, message)]
+
+        if end.date() < start.date():
+            raise ValueError("End date may not lie before start date!")
+
+        records: List[Record] = []
+        while start.date() < end.date():
+            split = start.replace(day=start.day + 1, hour=0, minute=0)
+            records.append(Record(start, split, category, message))
+            start = split
+        records.append(Record(start, end, category, message))
+        return records
+
     class UnmergeableError(Exception):
         def __init__(self, msg: str) -> None:
             super().__init__(f"Unmergeable records: {msg}")
 
     class CorruptedProtocolRowError(Exception):
         def __init__(self, msg: str) -> None:
             super().__init__(
```

### Comparing `work-1.1.0a4/src/work_components/dao/core.py` & `work-1.1.0b1/src/work_components/dao/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import datetime as dt
 import json
 import pathlib
 import zlib
 from types import SimpleNamespace
 from typing import Dict, List, Optional, Tuple
 
-import work_components.timestamps as ts
+import work_components.dt_format as dt_format
 from work_components import migrate
 from work_components.consts import (
     DATETIME_FORMAT,
     INFO_FILE_NAME,
     PROTOCOL_DIRECTORY_NAME,
     RECORDS_VERSION,
     RUN_FILE_NAME,
@@ -22,14 +22,15 @@
 from work_components.container import (
     Protocol,
     ProtocolDay,
     ProtocolMeta,
     ProtocolRange,
     Record,
 )
+from work_components.timestamps import Timestamp
 
 
 class WorkDao:
     """DAO for the work directory and its children."""
 
     # work_directory        self.work_directory
     # |- info.winf          self.info_file
@@ -53,44 +54,53 @@
         self.records_directory: pathlib.Path = self.work_directory.joinpath(
             PROTOCOL_DIRECTORY_NAME
         )
 
         # We assume existence of the root directory in many operations.
         self._ensure_work_dir_exists()
 
-    ### <MIGRATE-encoding> To be removed in v0.104 ###
+    ### <MIGRATE-midnight> To be removed in v1.3 ###
 
-    def migrate_records_encoding(self, flags):
-        """Unify records files to UTF-8 and \\n line terminator."""
-        migrate.noop_records_encoding()
+    def migrate_records_touching_midnight(self, end_lower_bound: Timestamp):
+        """Extend records touching midnight to end at 24:00."""
+        migrate.noop_records_midnight()
 
-        records_migrated_flag = "dao:records_converted_to_utf8"
-        if flags.is_set(records_migrated_flag):
-            return
-        flags.set(records_migrated_flag)
-
-        print("Converting records files to UTF-8 encoding and \\n newline character...")
+        print("Extending records...")
 
         # Iterate complete protocol
         protocol = self._load_protocol()
-        current_year: int = 0
         pday: ProtocolDay
-        print("  Converting:", end="")
         for pday in protocol.days:
-            if pday.date.year != current_year:
-                check = "✔"
-                if current_year == 0:
-                    check = ""
-                current_year = pday.date.year
-                print(f"{check} {current_year} ", end="", flush=True)
-            if entries := pday.entries:
-                # pylint: disable-msg=protected-access
-                pday._write_out(entries)
+            relative_bound: dt.datetime = end_lower_bound.combined(pday.date)
+            assert relative_bound.date() == pday.date
 
-        print("✔\n  Conversion done.")
+            if not pday.entries:
+                continue
+            last = pday.entries[-1]
+            midnight = (last.start + dt.timedelta(days=1)).replace(hour=0, minute=0)
+            if last.end < relative_bound or last.end >= midnight:
+                continue
+
+            last = pday.entries[-1]
+            edited = Record(
+                last.start,
+                midnight,
+                category=last.category,
+                message=last.message,
+            )
+            pday.replace(last, edited)
+            print(
+                f"✔ Edited {pday.date.strftime(dt_format.DATE_FORMAT)}: "
+                f"Last entry extended from {dt_format.readable_t(last.end)} "
+                f"to {dt_format.readable_t(edited.end, edited.start)}"
+            )
+
+        # Update the edit time and checksum
+        self.update_info_file()
+        print("\nConversion done.")
 
     ### Interface ###
 
     def start_run(self, start_time: dt.datetime, force: bool = False) -> None:
         """Start a run at the given time. Raises on invalid operation."""
 
         if not force and self.run_file.exists():
@@ -138,37 +148,20 @@
 
         if self.invalid_start_and_end_error(start_time, end_time) is not None:
             raise ValueError("Invalid combination of start and end time!")
 
         if not force and self.has_entry(start_time=start_time, end_time=end_time):
             raise RuntimeError("Given time(s) overlap with existing protocol entry!")
 
-        # If start end end lie on different dates, we split the entry up into two
-        entries = [(start_time, end_time)]
-        if not ts.date_equals(end_time, start_time):
-            assert end_time.date() == (start_time.date() + dt.timedelta(days=1))
-            split_time = end_time.replace(hour=0, minute=0)
-            entries = [(start_time, split_time), (split_time, end_time)]
-
-        for single_start, single_end in entries:
-            # Entries may lie on different dates technically, so we use our helper function
-            # to get shared (overlapping) date.
-            their_date: dt.date = ts.single_shared_date(single_start, single_end)
-
-            protocol_day: ProtocolDay = self._load_protocol_date(their_date)
-
-            protocol_day.add(
-                Record(
-                    start=single_start,
-                    end=single_end,
-                    category=category,
-                    message=message,
-                ),
-                force=force,
-            )
+        # If start end end lie on different dates, the factory splits them up.
+        records = Record.split_by_date(start_time, end_time, category, message)
+
+        for record in records:
+            protocol_day: ProtocolDay = self._load_protocol_date(record.date)
+            protocol_day.add(record=record, force=force)
 
         # Update the edit time and checksum
         self.update_info_file()
 
     def cancel_run(self) -> None:
         """Cancel any currently active run."""
         self.run_file.unlink()
@@ -380,25 +373,16 @@
 
             if self.file.exists():
                 self.load()
 
         def load(self) -> None:
             """Load and store info file contents."""
 
-            migrate.check_and_convert_textfile(self.file)
-
             with self.file.open(mode="r", encoding="utf-8") as info_file:
-                try:
-                    info_file_content = json.load(info_file)
-                except json.JSONDecodeError as json_err:
-                    if migrate.upgrade_info_file(info_file, self.update):
-                        return self.load()
-                    raise IOError(
-                        f"Invalid info file at {self.file.resolve()}"
-                    ) from json_err
+                info_file_content = json.load(info_file)
 
             self.program_version = info_file_content["program version"]
             self.records_version = info_file_content["records format version"]
             self.checksum = info_file_content["checksum"]
 
         def write(self) -> None:
             """Write info file content to disk. Only changes 'last update' field."""
@@ -451,16 +435,14 @@
             Wrapper for file.open(), handler.read(), and strptime(content).
 
             Utilizes cached file content if available.
             """
             if self.cache is not None:
                 return self.cache
 
-            migrate.check_and_convert_textfile(self.file)
-
             with self.file.open(mode="r", encoding="utf-8") as run_file_h:
                 content: str = run_file_h.read()
 
             try:
                 return dt.datetime.strptime(content, DATETIME_FORMAT)
             except ValueError as val_error:
                 raise IOError(
```

### Comparing `work-1.1.0a4/src/work_components/dao/flags.py` & `work-1.1.0b1/src/work_components/dao/flags.py`

 * *Files identical despite different names*

### Comparing `work-1.1.0a4/src/work_components/dao/recess.py` & `work-1.1.0b1/src/work_components/dao/recess.py`

 * *Files identical despite different names*

### Comparing `work-1.1.0a4/src/work_components/dt_parse.py` & `work-1.1.0b1/src/work_components/dt_parse.py`

 * *Files identical despite different names*

### Comparing `work-1.1.0a4/src/work_components/timestamps.py` & `work-1.1.0b1/src/work_components/timestamps.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """API wrapper and extension for datetime"""
 
-from dataclasses import dataclass
 import datetime as dt
+from dataclasses import dataclass
 from typing import Set
 
 
 def date_equals(left: dt.date, right: dt.date) -> bool:
     """Compare date equality of arbitrary date or datetime instances.
     Handles comparison of datetime to date."""
     # Intersection is not empty => (at least) one associated date overlaps
@@ -47,15 +47,15 @@
         assert isinstance(given, dt.date)
         return {given}
     if given.time() != dt.time(0, 0):
         return {given.date()}
     return {given.date() - dt.timedelta(days=1), given.date()}
 
 
-@dataclass(init=False)
+@dataclass(init=False, order=True)
 class Timestamp:
     hour: int
     minute: int
 
     def __init__(self, hour: int, minute: int):
         if hour not in range(0, 30):
             raise ValueError("hour must be in 0..29")
```

### Comparing `work-1.1.0a4/src/work_components/util.py` & `work-1.1.0b1/src/work_components/util.py`

 * *Files identical despite different names*

### Comparing `work-1.1.0a4/PKG-INFO` & `work-1.1.0b1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: work
-Version: 1.1.0a4
+Version: 1.1.0b1
 Summary: Manual time tracking via a CLI that works similarly to git.
 Home-page: https://vauhoch.zett.cc/work/
 Author: vauhochzett
 Author-email: vauhoch@zett.cc
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

