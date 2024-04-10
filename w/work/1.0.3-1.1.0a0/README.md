# Comparing `tmp/work-1.0.3.tar.gz` & `tmp/work-1.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "work-1.0.3.tar", max compression
+gzip compressed data, was "work-1.1.0a0.tar", max compression
```

## Comparing `work-1.0.3.tar` & `work-1.1.0a0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1033 2022-08-29 19:21:01.200221 work-1.0.3/README.md
--rw-r--r--   0        0        0      592 2023-08-23 17:05:43.504336 work-1.0.3/pyproject.toml
--rw-r--r--   0        0        0    89248 2023-08-23 17:05:34.580251 work-1.0.3/src/work.py
--rw-r--r--   0        0        0        0 2021-02-24 12:12:04.352563 work-1.0.3/src/work_components/__init__.py
--rw-r--r--   0        0        0    24173 2023-07-20 13:19:00.050197 work-1.0.3/src/work_components/arguments.py
--rw-r--r--   0        0        0     2045 2023-08-23 17:05:49.404393 work-1.0.3/src/work_components/consts.py
--rw-r--r--   0        0        0    22034 2023-08-23 17:05:29.308200 work-1.0.3/src/work_components/container.py
--rw-r--r--   0        0        0        0 2022-08-23 18:01:16.135701 work-1.0.3/src/work_components/dao/__init__.py
--rw-r--r--   0        0        0    15926 2023-07-05 14:46:26.049963 work-1.0.3/src/work_components/dao/core.py
--rw-r--r--   0        0        0     1523 2023-08-23 17:05:29.308200 work-1.0.3/src/work_components/dao/flags.py
--rw-r--r--   0        0        0    11530 2023-07-05 13:33:23.043915 work-1.0.3/src/work_components/dao/rc.py
--rw-r--r--   0        0        0    11011 2023-07-19 09:32:06.070610 work-1.0.3/src/work_components/dao/recess.py
--rw-r--r--   0        0        0     6209 2023-07-05 17:58:05.483335 work-1.0.3/src/work_components/dt_parse.py
--rw-r--r--   0        0        0     4470 2023-07-25 18:11:55.340963 work-1.0.3/src/work_components/migrate.py
--rw-r--r--   0        0        0      344 2023-07-05 13:32:05.419111 work-1.0.3/src/work_components/protocols.py
--rw-r--r--   0        0        0      471 2023-06-20 12:46:12.229256 work-1.0.3/src/work_components/timestamps.py
--rw-r--r--   0        0        0     8067 2023-07-11 18:36:01.409614 work-1.0.3/src/work_components/util.py
--rw-r--r--   0        0        0     1561 1970-01-01 00:00:00.000000 work-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1033 2022-08-29 19:21:01.200221 work-1.1.0a0/README.md
+-rw-r--r--   0        0        0      594 2024-04-09 13:51:26.037597 work-1.1.0a0/pyproject.toml
+-rw-r--r--   0        0        0    89902 2024-04-09 13:51:26.045597 work-1.1.0a0/src/work.py
+-rw-r--r--   0        0        0        0 2021-02-24 12:12:04.352563 work-1.1.0a0/src/work_components/__init__.py
+-rw-r--r--   0        0        0    24359 2024-04-08 19:32:29.849389 work-1.1.0a0/src/work_components/arguments.py
+-rw-r--r--   0        0        0     2214 2024-04-09 13:51:26.037597 work-1.1.0a0/src/work_components/consts.py
+-rw-r--r--   0        0        0    21865 2024-04-09 13:47:01.527495 work-1.1.0a0/src/work_components/container.py
+-rw-r--r--   0        0        0        0 2022-08-23 18:01:16.135701 work-1.1.0a0/src/work_components/dao/__init__.py
+-rw-r--r--   0        0        0    16847 2024-04-09 13:51:26.029596 work-1.1.0a0/src/work_components/dao/core.py
+-rw-r--r--   0        0        0      270 2024-04-08 19:32:29.853389 work-1.1.0a0/src/work_components/dao/env.py
+-rw-r--r--   0        0        0     1643 2024-04-08 19:32:29.853389 work-1.1.0a0/src/work_components/dao/flags.py
+-rw-r--r--   0        0        0    11503 2024-04-08 19:32:29.853389 work-1.1.0a0/src/work_components/dao/rc.py
+-rw-r--r--   0        0        0    11011 2024-04-08 18:05:30.527145 work-1.1.0a0/src/work_components/dao/recess.py
+-rw-r--r--   0        0        0     6212 2024-04-08 20:41:54.408996 work-1.1.0a0/src/work_components/dt_parse.py
+-rw-r--r--   0        0        0     4470 2024-04-08 18:05:30.527145 work-1.1.0a0/src/work_components/migrate.py
+-rw-r--r--   0        0        0      344 2024-04-08 18:05:30.527145 work-1.1.0a0/src/work_components/protocols.py
+-rw-r--r--   0        0        0     1664 2024-04-09 13:47:01.531495 work-1.1.0a0/src/work_components/timestamps.py
+-rw-r--r--   0        0        0     8067 2024-04-08 18:05:30.527145 work-1.1.0a0/src/work_components/util.py
+-rw-r--r--   0        0        0     1563 1970-01-01 00:00:00.000000 work-1.1.0a0/PKG-INFO
```

### Comparing `work-1.0.3/README.md` & `work-1.1.0a0/README.md`

 * *Files identical despite different names*

### Comparing `work-1.0.3/pyproject.toml` & `work-1.1.0a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "work"
-version = "1.0.3"
+version = "1.1.0a0"
 description = "Manual time tracking via a CLI that works similarly to git."
 authors = ["vauhochzett <vauhoch@zett.cc>"]
 readme = "README.md"
 homepage = "https://vauhoch.zett.cc/work/"
 packages = [
     { include = "work.py", from = "src" },
     { include = "work_components", from = "src" },
```

### Comparing `work-1.0.3/src/work.py` & `work-1.1.0a0/src/work.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,24 +32,26 @@
     Arguments,
 )
 from work_components.consts import (
     DIRECTORY,
     DIRECTORY_DEBUG,
     FLAG_FILE,
     FLAG_FILE_DEBUG,
+    MAX_RUN_HOURS,
     RC_FILE,
 )
 from work_components.container import (
     OverlapError,
     ProtocolDay,
     ProtocolMeta,
     Record,
     ShadowProtocolDay,
     sort_and_merge,
 )
+from work_components.dao import env
 from work_components.dao.core import WorkDao
 from work_components.dao.flags import Flags
 from work_components.dao.rc import RC
 from work_components.dao.recess import RecessDao
 from work_components.util import Color, PrinTable
 
 __version__: str = consts.VERSION
@@ -61,24 +63,28 @@
 DATE_FORMAT = "%d.%m.%Y"
 DATE_FORMAT_FULL = "%A, " + DATE_FORMAT
 
 
 class Work:
     """Main class"""
 
+    # Allow external access to debug flag
     debug: bool = False
 
     def __init__(self):
         """Initialize instance variables and load the RC."""
         self.base_dir: pathlib.Path
         self.dao: WorkDao
         self.recess_dao: RecessDao
         self.configuration: RC
         self.flags: Flags
 
+        # Load environment variables
+        Work.debug = env.get_bool(consts.ENV_DEBUG)
+
         # Load and check configuration (may raise)
         self.configuration = RC.load_rc()
 
     def _connect(self, base_dir: pathlib.Path) -> None:
         """Connect the DAOs."""
         self.dao = WorkDao(base_dir)
         self.recess_dao = RecessDao(base_dir)
@@ -102,23 +108,24 @@
         if args.mode is None:
             parser.print_help()
             sys.exit(2)
 
         if args.dry_run:
             print(">>> Dry run: Only output <<<")
 
-        # Allow external access to debug flag
-        Work.debug = args.debug
+        # Debug flag can be set in environment or via arguments
+        Work.debug = Work.debug or args.debug
 
         # Load flags (no checks)
-        flag_file: pathlib.Path = FLAG_FILE if not args.debug else FLAG_FILE_DEBUG
-        self.flags = Flags(flag_file)
+        flag_file: pathlib.Path = FLAG_FILE if not Work.debug else FLAG_FILE_DEBUG
+        no_set_flags: bool = env.get_bool(consts.ENV_NO_SET_FLAGS)
+        self.flags = Flags(flag_file, no_set_flags)
 
         # Connect DAO with normal or debug dir and load RC file
-        self.base_dir = DIRECTORY if not args.debug else DIRECTORY_DEBUG
+        self.base_dir = DIRECTORY if not Work.debug else DIRECTORY_DEBUG
         self._connect(base_dir=self.base_dir)
 
         # Migrate RC file
         self.configuration.migrate(self.flags)
 
         # Only verify the protocol and state for non-maintenance modes
         if args.mode not in MAINTENANCE_NAMES:
@@ -147,32 +154,34 @@
         self.dao.ensure_protocol_integrity()
         # Restore the state if erroneous.
         self.fix_state()
 
     def fix_state(self) -> None:
         """
         Fix a possibly invalid state. Exits if an invalid state is detected.
-        Currently only checks for an active run on a different date than today.
+        Currently only checks for an active run longer than the maximum length.
         """
 
         active_start: Optional[dt.datetime] = self.dao.get_start_time()
-        if active_start is None or active_start.date() == dt.date.today():
+        if active_start is None or (length := self._minutes_active_run()) <= (
+            MAX_RUN_HOURS * 60
+        ):
             return
 
-        # Forgot to stop a run: Run is active, but start date is not today
+        # Probably forgot to stop a run – prevent surprises when trying to switch or add
         print(
-            "Invalid state detected! A run started at "
-            f"{self._readable_dt(active_start)} is still active.\n"
+            f"Invalid state detected! A run of > {MAX_RUN_HOURS} hours is "
+            f"still active (started {self._readable_dt(active_start)}).\n"
         )
 
         # Read input, strip and lower
         user_says: str = (
             input(
-                "To add to log, enter an end time (%H:%M). "
-                'Cancel the run with "cancel":\n'
+                "To end the run and add it to log, enter its end time (%H:%M). "
+                'To cancel the run, write "cancel":\n'
             )
             .strip()
             .lower()
         )
 
         if user_says == "cancel":
             self.dao.cancel_run()
@@ -313,14 +322,16 @@
     ### Modes ###
 
     # start #
 
     def start(self, args) -> None:
         """Start the protocol based on the given arguments."""
 
+        raise NotImplementedError("END TIME 0")
+
         start_time: dt.datetime = self.get_single_time(args)
         self._start(start_time=start_time, force=args.force, dry_run=args.dry_run)
         print(f"Started work at {self._readable_dt(start_time)}")
 
     def ensure_valid_start_time(
         self,
         start_time: dt.datetime,
@@ -369,23 +380,29 @@
     def stop(self, args) -> None:
         """Stop the protocol based on the given arguments."""
         end_time: dt.datetime = self.get_single_time(args)
         run_length: float = self._stop(
             end_time=end_time,
             category=args.category,
             message=args.message,
+            force=args.force,
             dry_run=args.dry_run,
         )
         print(
             f"Stopped work at {self._readable_dt(end_time)} "
             f"({self._timedelta_str(run_length)} recorded)"
         )
 
     def _stop(
-        self, end_time: dt.datetime, category: str, message: str, dry_run: bool = False
+        self,
+        end_time: dt.datetime,
+        category: str,
+        message: str,
+        force: bool = False,
+        dry_run: bool = False,
     ) -> float:
         """Stop the protocol with the given end time.
         Returns the recorded run length in minutes."""
 
         start_time: Optional[dt.datetime] = self.dao.get_start_time()
 
         if start_time is None:
@@ -396,27 +413,35 @@
         if end_time == start_time:
             self.dao.cancel_run()
             raise InvalidOperationWarning(
                 "End time is identical to start time – run cancelled."
             )
 
         self._can_i_add_this(
-            start_time=start_time, end_time=end_time, operation="stop work"
+            start_time=start_time,
+            end_time=end_time,
+            operation="stop work",
+            force=force,
         )
 
         # Preconditions met: Run can be stopped.
         if not dry_run:
-            self.dao.stop_run(end_time=end_time, category=category, message=message)
+            self.dao.stop_run(
+                end_time=end_time, category=category, message=message, force=force
+            )
         return util.minutes_difference(start=start_time, end=end_time)
 
     # add #
 
     def add(self, args) -> None:
         """Add a protocol entry consisting of start time, end time and optional date flag."""
 
+        # raise NotImplementedError("END TIME 0")
+        print(" TODO TO DOJFS KFDJLK JSDL JFSD END TIME 0:00!!!!")
+
         start_time: dt.datetime
         end_time: dt.datetime
         baseline_date: dt.date = self.get_selected_date(args)
         start_time, end_time = self.get_time_from_and_to(args, baseline_date)
 
         self._can_i_add_this(
             start_time=start_time,
@@ -451,27 +476,30 @@
         force: bool = False,
     ) -> None:
         """
         Shared checks for valid start and end time of a run.
         Raises InvalidOperationWarning if not.
         """
 
-        if end_time.date() != start_time.date():
+        if end_time <= start_time:
             raise InvalidOperationWarning.cant(
                 operation,
-                "dates of start and end time differ\n"
-                + "Start date:          {}\n".format(start_time.strftime("%d.%m.%Y"))
-                + "Requested stop date: {}".format(end_time.strftime("%d.%m.%Y")),
+                "end time ({}) must be after start time ({})".format(
+                    self._readable_dt(end_time), self._readable_dt(start_time)
+                ),
             )
 
-        if end_time <= start_time:
+        if (length := util.minutes_difference(start_time, end_time)) > (
+            MAX_RUN_HOURS * 60
+        ):
             raise InvalidOperationWarning.cant(
                 operation,
-                "end time ({}) must be after start time ({})".format(
-                    self._readable_dt(end_time), self._readable_dt(start_time)
+                (
+                    f"runs may not be longer than {MAX_RUN_HOURS} hours"
+                    f"(is: {self._timedelta_str(length)})"
                 ),
             )
 
         if not force and self.dao.has_entry(start_time=start_time, end_time=end_time):
             raise InvalidOperationWarning.cant(
                 operation,
                 "an existing record overlaps with the specified time (add --force to override)",
@@ -784,14 +812,16 @@
             prospective_start=prospective_start,
             run_active=start_time is not None,
             start_argument=start_argument,
             worked_towork_split=worked_towork_split,
             extra_pause_minutes=extra_pause_minutes,
         )
 
+        # For multi-day runs, the output time counts the complete active run, even
+        # though that run will only partially be logged on the current day.
         if args.h_until:
             target: dt.datetime = dt_parse.resolve_time_argument(
                 argument=args.h_until,
                 baseline_date=today,
                 rounding_mode=dt_parse.RoundingMode.UP,
             )
 
@@ -803,23 +833,42 @@
                 )
 
             optional_output += new_section()
             optional_output += self._get_hours_worked_until_msg(
                 target_time=target, hours_data=hours_data
             )
 
-        # Only continue if args.h_target is set and not 0
+        # Calculate the end time to achieve the given target hours today.
         if args.h_target:
             target_hours, target_minutes = dt_parse.parse_time_period_str(args.h_target)
 
+            target_hours_data = hours_data
+
+            # For multi-day runs, we only count the minutes worked *today*
+            if start_time is not None and start_time.date() < dt.date.today():
+                pretend_start_time = dt.datetime.combine(dt.date.today(), dt.time())
+                pretend_minutes_active_run = util.minutes_difference(
+                    start=pretend_start_time, end=self._dt_now_stripped()
+                )
+                target_hours_data = Work.HoursData(
+                    minutes_logged=hours_data.minutes_logged,
+                    minutes_active_run=pretend_minutes_active_run,
+                    minutes_to_work_today=hours_data.minutes_to_work_today,
+                    prospective_start=hours_data.prospective_start,
+                    run_active=hours_data.run_active,
+                    start_argument=hours_data.start_argument,
+                    worked_towork_split=hours_data.worked_towork_split,
+                    extra_pause_minutes=hours_data.extra_pause_minutes,
+                )
+
             optional_output += new_section()
             optional_output += self._get_target_end_time_msg(
                 target_hours=target_hours,
                 target_minutes=target_minutes,
-                hours_data=hours_data,
+                hours_data=target_hours_data,
             )
 
         # Calculate the remaining hours for a full workday (respecting the week balance)
         if args.h_balance_target:
             # Parse balance target and classify into over-/undertime
             balance_target: str = args.h_balance_target
             target_is_overtime: bool = False
@@ -973,16 +1022,15 @@
             delta_minutes += hours_data.extra_pause_minutes
 
         # If a run was started in the past, worked_minutes includes the minutes up to now,
         # so we have to calculate the end from _dt_now_stripped().
         prospective_end: dt.datetime = hours_data.worked_towork_split
         prospective_end += dt.timedelta(minutes=delta_minutes)
 
-        # The end time might lie on the next day. We don't support multi-day runs, so
-        # we catch this here.
+        # The end time might lie on the next day. Then, the target is unachievable.
         if prospective_end.date() != dt.date.today():
             return "Given target hours can't be completed anymore today!"
 
         # End time has already been reached
         if prospective_end <= self._dt_now_stripped():
             return completed_msg
 
@@ -1055,15 +1103,15 @@
         # Simple warning for overlaps – if any run lies in the future, warn.
         warning_str: str = ""
         if self.dao.has_entry(
             start_time=hours_data.prospective_start,
             end_time=dt.datetime.combine(dt.date.today(), dt.time(23, 59)),
         ):
             warning_str = (
-                "Warning: An upcoming run has been recorded for today, which could "
+                "Warning: A logged run overlaps the current period, which could "
                 "make the calculation invalid. Please check for overlaps manually."
             )
 
         return assumption_str, warning_str
 
     # list #
 
@@ -1218,17 +1266,19 @@
 
         result: List[str] = []
         result.append(
             "{: <3}, {}: {} records{}{}".format(
                 day.strftime("%a"),
                 day.strftime(date_fmt),
                 record_count,
-                f" (merged to {len(records)})"
-                if only_time and len(records) != record_count
-                else "",
+                (
+                    f" (merged to {len(records)})"
+                    if only_time and len(records) != record_count
+                    else ""
+                ),
                 " (+ active run)" if active_start_to_include is not None else "",
             )
         )
 
         active_run_to_include: Optional[Record] = None
         if active_start_to_include is not None:
             # For a future run, we have to select an end time, so we just choose the
@@ -2148,63 +2198,28 @@
 
         minutes_active_run: float = util.minutes_difference(
             start=active_start, end=self._dt_now_stripped()
         )
         # Fixes bug for future start in which case a negative number is returned.
         return max(minutes_active_run, 0)
 
-    def _total_minutes_worked(
-        self, requested_date: dt.date = dt.date.today()
-    ) -> Tuple[float, float]:
+    def _total_minutes_worked(self) -> Tuple[float, float]:
         """
-        Return the total minutes worked on the given day (today if None is given).
+        Return the total minutes worked today.
         Includes all recorded protocol entries, as well as the current run (if active).
         """
 
-        minutes_protocol = self._minutes_logged_on(requested_date=requested_date)
+        minutes_protocol = self._minutes_logged_on(requested_date=dt.date.today())
         minutes_active_run: float = 0.0
-        # FIXME: To prepare for multi-day runs, we should only count minutes that
-        # occurred during the requested date. Currently, if the run was started
-        # yesterday, it would be discarded completely.
         active_start: Optional[dt.datetime] = self.dao.get_start_time()
-        if active_start is not None and active_start.date() == requested_date:
+        if active_start is not None:
             minutes_active_run = self._minutes_active_run()
 
         return minutes_protocol, minutes_active_run
 
-    def _total_pauses_today(self) -> float:
-        """
-        Return the pauses today, in minutes.
-        Sums up all gaps between protocol entries, also taking into account the active run.
-        """
-
-        records: List[Record] = self.dao.get_entries(date=dt.date.today())
-
-        # If a run is active, it is added as a theoretical entry
-        active_start: Optional[dt.datetime] = self.dao.get_start_time()
-        if active_start is not None:
-            records.append(Record.one_minute_record(start=active_start))
-
-        return self._total_pauses(records=records)
-
-    @staticmethod
-    def _total_pauses(records: List[Record]) -> float:
-        """Return the sum of all gaps between protocol entries."""
-
-        if len(records) <= 1:
-            return 0.0
-
-        pauses: float = 0.0
-        last_end: dt.datetime = records[0].end
-        for rec in records[1:]:
-            pauses += util.minutes_difference(start=last_end, end=rec.start)
-            last_end = rec.end
-
-        return pauses
-
     @staticmethod
     def _timedelta_str(minutes: float) -> str:
         """
         Return a string representing the minutes (e.g. 150.0) as HH:MM (e.g. 2 h 30 m).
          minutes : Positive-valued number of minutes to translate.
         """
```

### Comparing `work-1.0.3/src/work_components/arguments.py` & `work-1.1.0a0/src/work_components/arguments.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,15 +179,15 @@
         parser = argparse.ArgumentParser(
             prog=NAME,
             description="Time tracking with an interaction model inspired by git.",
             epilog="To find out more, check the help page of individual modes.",
         )
         # fmt: off
         parser.add_argument("-H", "--help-verbose", action="store_true",
-            help="show a longer help output, similar to a man page")
+            help="show a longer help output, similar to a man page, and exit")
         parser.add_argument("-V", "--version", action="version", version=f"%(prog)s {consts.VERSION}")
         parser.add_argument("-d", "--debug", action="store_true", help=argparse.SUPPRESS)
         parser.add_argument("-y", "--dry-run", action="store_true", help="only print output")
         # fmt: on
 
         modes = parser.add_subparsers(
             title="modes", dest="mode", metavar="{start, stop, add, status, list, ...}"
@@ -306,14 +306,19 @@
             "--force",
             action="store_true",
             help="Start anew even if a run is already active.",
         )
 
         stop_mode = MODES[STOP_NAME].add_as_parser(modes)
         stop_mode.set_defaults(func=program.stop)
+        stop_mode.add_argument(
+            "--force",
+            action="store_true",
+            help="Stop even if the new entry would overlap an existing one.",
+        )
 
         # start / stop have a single time argument
         for single_time_mode in [start_mode, stop_mode]:
             single_time_mode.add_argument("time", metavar="TIME", help=time_help_text)
 
         # DOUBLE TIME modes
```

### Comparing `work-1.0.3/src/work_components/consts.py` & `work-1.1.0a0/src/work_components/consts.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """ Shared constants """
 
 import os
 import pathlib
 from typing import List, Tuple
 
-VERSION: str = "1.0.3"
+VERSION: str = "1.1.0a0"
 RECORDS_VERSION: int = 3
 
 # Directories
 PARENT_DIR: pathlib.Path = pathlib.Path("~", ".local", "share").expanduser()
 DIRECTORY: pathlib.Path = PARENT_DIR.joinpath("work")
 DIRECTORY_DEBUG: pathlib.Path = PARENT_DIR.joinpath("debug", "work")
 
@@ -36,14 +36,19 @@
 # Flags – XDG_STATE_HOME
 _STATE_HOME: str = _resolve_xdg_path(
     "XDG_STATE_HOME", os.path.join("~", ".local", "state")
 )
 FLAG_FILE: pathlib.Path = pathlib.Path(_STATE_HOME, "work", "flags.wstate")
 FLAG_FILE_DEBUG: pathlib.Path = pathlib.Path(_STATE_HOME, "work", "flags-debug.wstate")
 
+# Environment variables
+env_prefix: str = "WORK_"
+ENV_DEBUG: str = f"{env_prefix}DEBUG"
+ENV_NO_SET_FLAGS: str = f"{env_prefix}DONT_SET_FLAGS"
+
 # Formats
 DATE_FORMAT = "%Y-%m-%d"
 TIME_FORMAT = "%H:%M"
 DATETIME_FORMAT = "%Y-%m-%d %H:%M"
 
 # Patterns
 INFO_FILE_CONTENT = "work-time-protocol/protocol-v{}/last-edit:{}/checksum:{}\n"
@@ -64,7 +69,8 @@
     "Wednesday",
     "Thursday",
     "Friday",
     "Saturday",
     "Sunday",
 ]
 ALLOWED_WORK_HOURS: Tuple[float, float] = (0.0, 24.0)
+MAX_RUN_HOURS: int = 24
```

### Comparing `work-1.0.3/src/work_components/container.py` & `work-1.1.0a0/src/work_components/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     DATETIME_FORMAT,
     DAY_FILE_PATTERN,
     MONTH_DIR_PATTERN,
     PROTOCOL_FILE_EXTENSION,
     TIME_FORMAT,
     YEAR_DIR_PATTERN,
 )
-from work_components.timestamps import date_equals
+import work_components.timestamps as ts
 
 ### Record container classes ###
 
 
 class Record:
     """A protocol record. Invariant: start <= end"""
 
@@ -50,17 +50,17 @@
     @property
     def end(self) -> dt.datetime:
         return self._end
 
     @property
     def date(self) -> dt.date:
         """This record's date. Raises if start date != end date."""
-        if self.start.date() != self.end.date():
+        if not ts.date_equals(self.start, self.end):
             raise ValueError("Record end date differs from start date!")
-        return self.start.date()
+        return ts.single_shared_date(self.start, self.end)
 
     @property
     def category(self) -> str:
         return self._category
 
     @property
     def message(self) -> str:
@@ -287,42 +287,40 @@
         if 0 == len(entries):
             raise IOError(f"Empty protocol file on disk: {self.path}")
 
         return entries
 
     def _raise_if_invalid_for_me(self, record: Record):
         """Check if the record matches this ProtocolDay and raise if not."""
-        if not date_equals(record.start, self.date):
+        if not ts.date_equals(record.start, self.date):
             raise Record.CorruptedProtocolRowError("date does not match file path")
-        if not date_equals(record.start, record.end):
+        if not ts.date_equals(record.start, record.end):
             raise Record.CorruptedProtocolRowError("start and end date differ")
 
     def add(self, record: Record, force: bool = False) -> None:
         """
         Store a new entry on disk. Rewrites the file.
 
         force: Overwrite existing entries if necessary.
         """
 
-        if record.start.date() != self.date or record.end.date() != self.date:
+        if not (
+            ts.date_equals(record.start, self.date)
+            and ts.date_equals(record.end, self.date)
+        ):
             raise IOError("Given start or end time lie on a different day!")
 
         entries: List[Record] = self.entries
         if force:
             entries = self._cut(entries=entries, space_for=record)
         entries.append(record)
         try:
             entries_processed: List[Record] = sort_and_merge(entries)
         except OverlapError as ovl_err:
-            ovl_err.message = (
-                "Overlapping entries detected – please fix manually. Offending records:\n"
-                f"  {ovl_err.left.strf(TIME_FORMAT)}\n"
-                f"  {ovl_err.right.strf(TIME_FORMAT)}\n"
-                f"In file: {self.path}"
-            )
+            ovl_err.message = ovl_err.message + f"\nIn file: {self.path}"
             raise ovl_err
 
         self._write_out(records=entries_processed)
 
     def _cut(self, entries: List[Record], space_for: Record) -> List[Record]:
         """Remove any overlaps with `space_for` in the given list of entries."""
         processed_entries: List[Record] = []
@@ -580,24 +578,23 @@
 class OverlapError(ValueError):
     """Entries overlap when they shouldn't."""
 
     def __init__(self, left: Record, right: Record) -> None:
         super().__init__()
         self.left = left
         self.right = right
-        self.message = f"Overlapping entries: {left} / {right}"
+        self.message = (
+            "Overlapping entries detected – please fix manually. Offending records:\n"
+            f"  {left.strf(TIME_FORMAT)}\n"
+            f"  {right.strf(TIME_FORMAT)}"
+        )
 
     def __str__(self) -> str:
         return self.message
 
-        # (
-        #         "Overlapping entries detected – please fix manually. "
-        #         f"Offending records:\n  {last_record}\n  {next_record}"
-        #     )
-
 
 def sort_and_merge(entries: List[Record], output: bool = True) -> List[Record]:
     """Sort the given entries based on their start time and merge touching and
     mergeable entries."""
 
     # Before entries are added, the DAO checks and prevents overlaps. Therefore, we can
     # assume that entries should be either apart or "touch" and raise otherwise.
```

### Comparing `work-1.0.3/src/work_components/dao/core.py` & `work-1.1.0a0/src/work_components/dao/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,26 +8,28 @@
 import zlib
 from typing import Dict, List, Optional, Tuple
 
 from work_components import migrate
 from work_components.consts import (
     DATETIME_FORMAT,
     INFO_FILE_NAME,
+    MAX_RUN_HOURS,
     PROTOCOL_DIRECTORY_NAME,
     RECORDS_VERSION,
     RUN_FILE_NAME,
     VERSION,
 )
 from work_components.container import (
     Protocol,
     ProtocolDay,
     ProtocolMeta,
     ProtocolRange,
     Record,
 )
+import work_components.timestamps as ts
 
 
 class WorkDao:
     """DAO for the work directory and its children."""
 
     # work_directory        self.work_directory
     # |- info.winf          self.info_file
@@ -94,22 +96,24 @@
         if not force and self.run_file.exists():
             raise IOError(
                 f'File "{self.run_file.resolve()}" exists already! Could not create.'
             )
 
         self.run_file.write(start_time)
 
-    def stop_run(self, end_time: dt.datetime, category: str, message: str) -> None:
+    def stop_run(
+        self, end_time: dt.datetime, category: str, message: str, force: bool = False
+    ) -> None:
         """Stop a run at the given time. Raises on invalid operation."""
 
         start_time = self.get_start_time()
         if start_time is None:
             raise RuntimeError("Tried to stop, but no run is active!")
 
-        self.add_protocol_entry(start_time, end_time, category, message)
+        self.add_protocol_entry(start_time, end_time, category, message, force)
         self.run_file.unlink()
 
     def add_protocol_entry(
         self,
         start_time: dt.datetime,
         end_time: dt.datetime,
         category: str,
@@ -120,34 +124,45 @@
         Add the given elements to the end of the protocol file.
         Checks validity of the info file and updates it after write.
         """
 
         if not start_time < end_time:
             raise ValueError("End time is not after start time!")
 
-        if start_time.date() != end_time.date():
-            raise ValueError("Start and end lie on different dates!")
+        if (end_time - start_time) >= dt.timedelta(hours=MAX_RUN_HOURS):
+            raise ValueError(
+                f"Start and end lie more than {MAX_RUN_HOURS} hours apart!"
+            )
 
         if not force and self.has_entry(start_time=start_time, end_time=end_time):
-            raise RuntimeError("Given time(s) overlap with existing protocol entry")
-
-        # Both start and end lie on the same day, so we can just use one date
-        their_date: dt.date = start_time.date()
+            raise RuntimeError("Given time(s) overlap with existing protocol entry!")
 
-        protocol_day: ProtocolDay = self._load_protocol_date(their_date)
-
-        protocol_day.add(
-            Record(
-                start=start_time,
-                end=end_time,
-                category=category,
-                message=message,
-            ),
-            force=force,
-        )
+        # If start end end lie on different dates, we split the entry up into two
+        entries = [(start_time, end_time)]
+        if end_time.date() != start_time.date():
+            assert end_time.date() == (start_time.date() + dt.timedelta(days=1))
+            split_time = end_time.replace(hour=0, minute=0)
+            entries = [(start_time, split_time), (split_time, end_time)]
+
+        for single_start, single_end in entries:
+            # Entries may lie on different dates technically, so we use our helper function
+            # to get shared (overlapping) date.
+            their_date: dt.date = ts.single_shared_date(single_start, single_end)
+
+            protocol_day: ProtocolDay = self._load_protocol_date(their_date)
+
+            protocol_day.add(
+                Record(
+                    start=single_start,
+                    end=single_end,
+                    category=category,
+                    message=message,
+                ),
+                force=force,
+            )
 
         # Update the edit time and checksum
         self.update_info_file()
 
     def cancel_run(self) -> None:
         """Cancel any currently active run."""
         self.run_file.unlink()
@@ -175,17 +190,19 @@
 
         # Minimum run length: 1 minute
         end_time = end_time or start_time + dt.timedelta(minutes=1)
 
         start_date: dt.date = start_time.date()
         end_date: dt.date = end_time.date()
 
+        # This comparison works even with our looser definition of "same date".
         if start_date > end_date:
             raise ValueError("Start date lies after end date!")
 
+        # We can "forget" the 0:00 case, as the start time only affects upcoming days.
         current_date: dt.date = start_date
         protocol_days: List[ProtocolDay] = []
         # Add all days covered by start and end time.
         while current_date <= end_date:
             protocol_days.append(self._load_protocol_date(current_date))
             current_date += dt.timedelta(days=1)
```

### Comparing `work-1.0.3/src/work_components/dao/flags.py` & `work-1.1.0a0/src/work_components/dao/flags.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 import pathlib
 from typing import List
 
 
 class Flags:
     """Read and modify flags."""
 
-    def __init__(self, flag_file: pathlib.Path) -> None:
+    def __init__(self, flag_file: pathlib.Path, no_set_flags: bool = False) -> None:
         self._file: pathlib.Path = flag_file
+        self._no_set_flags = no_set_flags
         self._flags: List[str] = []
         self._load()
 
     def _load(self) -> None:
         """Load flags into memory."""
 
         if not self._file.exists():
@@ -28,14 +29,16 @@
 
     def is_set(self, key: str) -> bool:
         """Return if given flag is set."""
         return key in self._flags
 
     def set(self, *flags: str) -> None:
         """Add given flag(s) to flag store."""
+        if self._no_set_flags:
+            return
         self._flags.extend(flags)
         self._write()
 
     def remove(self, *flags: str) -> None:
         """Remove given flag(s) from flag store. Accepts nonexistent flags."""
         for flag in filter(lambda f: f in self._flags, flags):
             self._flags.remove(flag)
```

### Comparing `work-1.0.3/src/work_components/dao/rc.py` & `work-1.1.0a0/src/work_components/dao/rc.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # pylint: disable-msg=invalid-name
 
 """ The DAO for the runtime configuration file. """
 
 import json
 from collections import ChainMap
-from typing import IO, Any, Dict, List, Mapping, MutableMapping, Optional
+from typing import IO, Any, Callable, Dict, List, Mapping, MutableMapping, Optional
 
 from work_components import consts, migrate, util
 from work_components.arguments import MODES
 from work_components.consts import RC_FILE
 from work_components.protocols import IFlags
 
 # When a new key is to be added:
@@ -226,25 +226,23 @@
                 if k not in data:
                     raise RCError(f'Missing expected key "{k}"')
 
         for k in data:
             if k not in expected_keys:
                 raise RCError(f'Unexpected key "{k}"')
 
-        # Verify expected_hours
-        if RC.expected_hours_k in data:
-            RC._verify_expected_hours(data[RC.expected_hours_k])
-
-        # Verify aliases
-        if RC.aliases_k in data:
-            RC._verify_aliases(data[RC.aliases_k])
-
-        # Verify macros
-        if RC.macros_k in data:
-            RC._verify_macros(data[RC.macros_k])
+        verifiers: Dict[str, Callable] = {
+            RC.expected_hours_k: RC._verify_expected_hours,
+            RC.aliases_k: RC._verify_aliases,
+            RC.macros_k: RC._verify_macros,
+        }
+
+        for key, verifier in verifiers.items():
+            if key in data:
+                verifier(data[key])
 
     @staticmethod
     def _verify_expected_hours(expected_hours) -> None:
         """Verify the value for expected hours. Raises RCError if invalid."""
 
         # Should be a mapping of day to hours: { "Monday": 8.0, Tuesday: 0.0, ... }
         if not isinstance(expected_hours, Mapping):
```

### Comparing `work-1.0.3/src/work_components/dao/recess.py` & `work-1.1.0a0/src/work_components/dao/recess.py`

 * *Files identical despite different names*

### Comparing `work-1.0.3/src/work_components/dt_parse.py` & `work-1.1.0a0/src/work_components/dt_parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 def resolve_time_argument(
     argument: str, baseline_date: dt.date, rounding_mode: RoundingMode
 ) -> dt.datetime:
     """Parse the input to the time argument.
 
     Important: This function only understands mode-agnostic times."""
 
-    # Custom Rounding: now-, now+, now! (now-/+ rundet immer ab/auf; now! rundet nicht)
+    # Custom Rounding: now-, now+, now! (now-/+ always runds down/up; now! does not round)
     if argument.startswith("now"):
         baseline_time = dt.datetime.now().replace(second=0, microsecond=0).time()
         baseline_datetime = dt.datetime.combine(baseline_date, baseline_time)
 
         valid_arguments = [f"now{suffix}" for suffix in ["", "+", "-", "!"]]
         if argument not in valid_arguments:
             raise ValueError(
```

### Comparing `work-1.0.3/src/work_components/migrate.py` & `work-1.1.0a0/src/work_components/migrate.py`

 * *Files identical despite different names*

### Comparing `work-1.0.3/src/work_components/util.py` & `work-1.1.0a0/src/work_components/util.py`

 * *Files identical despite different names*

### Comparing `work-1.0.3/PKG-INFO` & `work-1.1.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: work
-Version: 1.0.3
+Version: 1.1.0a0
 Summary: Manual time tracking via a CLI that works similarly to git.
 Home-page: https://vauhoch.zett.cc/work/
 Author: vauhochzett
 Author-email: vauhoch@zett.cc
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

