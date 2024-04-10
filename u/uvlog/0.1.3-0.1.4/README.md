# Comparing `tmp/uvlog-0.1.3-py3-none-any.whl.zip` & `tmp/uvlog-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 16302 bytes, number of entries: 9
--rw-r--r--  2.0 unx     1119 b- defN 24-Apr-04 17:05 uvlog/__init__.py
--rw-r--r--  2.0 unx     5448 b- defN 24-Apr-04 17:05 uvlog/formatters.py
--rw-r--r--  2.0 unx     9844 b- defN 24-Apr-04 17:05 uvlog/handlers.py
--rw-r--r--  2.0 unx    20197 b- defN 24-Apr-04 17:05 uvlog/uvlog.py
--rw-r--r--  2.0 unx     1069 b- defN 24-Apr-04 17:05 uvlog-0.1.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     9820 b- defN 24-Apr-04 17:05 uvlog-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 17:05 uvlog-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 24-Apr-04 17:05 uvlog-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      671 b- defN 24-Apr-04 17:05 uvlog-0.1.3.dist-info/RECORD
-9 files, 48266 bytes uncompressed, 15164 bytes compressed:  68.6%
+Zip file size: 15647 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     1119 b- defN 24-Apr-10 15:43 uvlog/__init__.py
+-rw-r--r--  2.0 unx     5340 b- defN 24-Apr-10 15:43 uvlog/formatters.py
+-rw-r--r--  2.0 unx     8939 b- defN 24-Apr-10 15:43 uvlog/handlers.py
+-rw-r--r--  2.0 unx    20079 b- defN 24-Apr-10 15:43 uvlog/uvlog.py
+-rw-r--r--  2.0 unx     1069 b- defN 24-Apr-10 15:43 uvlog-0.1.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8020 b- defN 24-Apr-10 15:43 uvlog-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-10 15:43 uvlog-0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 24-Apr-10 15:43 uvlog-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      671 b- defN 24-Apr-10 15:43 uvlog-0.1.4.dist-info/RECORD
+9 files, 45335 bytes uncompressed, 14509 bytes compressed:  68.0%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: uvlog/handlers.py
 Comment: 
 
 Filename: uvlog/uvlog.py
 Comment: 
 
-Filename: uvlog-0.1.3.dist-info/LICENSE
+Filename: uvlog-0.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: uvlog-0.1.3.dist-info/METADATA
+Filename: uvlog-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: uvlog-0.1.3.dist-info/WHEEL
+Filename: uvlog-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: uvlog-0.1.3.dist-info/top_level.txt
+Filename: uvlog-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: uvlog-0.1.3.dist-info/RECORD
+Filename: uvlog-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## uvlog/__init__.py

```diff
@@ -7,15 +7,15 @@
 from uvlog.formatters import *
 from uvlog.handlers import *
 from uvlog.uvlog import *
 
 __python_version__ = "3.8"
 __author__ = "violetblackdev@gmail.com"
 __license__ = "MIT"
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 
 add_formatter_type(TextFormatter)
 add_formatter_type(JSONFormatter)
 add_handler_type(StreamHandler)
 add_handler_type(QueueStreamHandler)
 
 configure(BASIC_CONFIG)
```

## uvlog/formatters.py

```diff
@@ -1,16 +1,16 @@
 """Standard log formatters."""
 
 import io
 import traceback
 from datetime import datetime
 from json import dumps
-from typing import Any, Collection, cast
+from typing import Any, Collection, cast, ClassVar
 
-from uvlog.uvlog import Formatter, LogRecord
+from uvlog.uvlog import LogRecord, Formatter
 
 __all__ = [
     "JSONFormatter",
     "TextFormatter",
 ]
 
 DEFAULT_TIMESPEC = "seconds"
@@ -30,20 +30,20 @@
 
 
 class TextFormatter(Formatter):
     """Text log formatter.
 
     Creates human-readable log output.
 
-    Formatter settings can be set directly.
+    Formatter settings must be set directly or using the :py:func:`uvlog.config` method.
 
     .. code-block:: python
 
         _formatter = TextFormatter()
-        _formatter.timestamp_separator = ' '
+        _formatter.timespec = 'seconds'
 
     """
 
     timespec: str
     """Precision for ISO timestamps,
     see `datetime.isoformat() <https://docs.python.org/3/library/datetime.html#datetime.datetime.isoformat>`_"""
 
@@ -91,55 +91,53 @@
         traceback.print_exception(error_cls, exc, stack, None, sio)
         s = sio.getvalue()
         sio.close()
         if s[-1:] == "\n":
             s = s[:-1]
         return s
 
-    def __str__(self):
-        return f"<{self.__class__.__name__}>"
-
 
 class JSONFormatter(Formatter):
     """JSON log formatter.
 
-    To change the default `dumps` function assign it to the class attribute:
+    To change the default `dumps` function assign it to the class attribute.
 
     .. code-block:: python
 
         import orjson
 
         JSONFormatter.serializer = orjson.dumps
 
-    Formatter settings can be set directly.
+    Formatter settings must be set directly or using the :py:func:`uvlog.config` method.
 
     .. code-block:: python
 
         _formatter = JSONFormatter()
         _formatter.exc_pass_locals = True
 
     """
 
-    serializer = _dumps_bytes
+    serializer: ClassVar = _dumps_bytes
     """Serializer function - a class attribute"""
 
     keys: Collection[str]
-    """List of serialized log record keys,
-    the available keys can be seen in :py:class:`~uvlog.LogRecord` type"""
+    """List of serialized log record keys.
+
+    The available keys can be seen in :py:class:`~uvlog.LogRecord` type"""
 
     exc_pass_locals: bool
-    """Pass locals dict in exception traceback (don't use it unless you're sure your logs are secure)"""
+    """Pass locals dict in exception traceback (don't use it unless your logs are secure)"""
 
-    exc_pass_globals: bool
-    """Pass globals dict in exception traceback (don't use it unless you're sure your logs are secure)"""
+    exc_pass_filenames: bool
+    """Pass globals dict in exception traceback (don't use it unless your logs are secure)"""
 
     def __init__(self):
         """Initialize."""
         self.exc_pass_locals = False
-        self.exc_pass_globals = False
+        self.exc_pass_filenames = False
         self.keys = (
             "name",
             "level",
             "levelno",
             "asctime",
             "message",
             "exc_info",
@@ -156,30 +154,25 @@
         for key in self.keys:
             value = getattr(record, key, None)
             if value is not None:
                 data[key] = value
         exc_info = cast(Exception, data.pop("exc_info", None))
         if exc_info:
             error_cls, exc, _ = type(exc_info), exc_info, exc_info.__traceback__
-            if hasattr(exc, "serialize"):
-                data["exc_info"] = exc.serialize()
-            else:
-                data["exc_info"] = {
-                    "message": str(exc),
-                    "type": error_cls.__name__,
-                    "data": exc.__dict__,
+            data["exc_info"] = {
+                "message": str(exc),
+                "type": error_cls.__name__,
+                "data": exc.json_repr() if hasattr(exc, "json_repr") else {},
+            }
+            tb = exc.__traceback__
+            if tb and tb.tb_next:
+                frame = tb.tb_next
+                data["exc_info"]["traceback"] = tb_dict = {
+                    "lineno": frame.tb_lineno,
+                    "func": frame.tb_frame.f_code.co_name,
                 }
-                if exc.__traceback__:
-                    frame = exc.__traceback__.tb_frame
-                    data["exc_info"]["traceback"] = tb = {
-                        "lineno": frame.f_lineno,
-                        "func": frame.f_code.co_name,
-                    }
-                    if self.exc_pass_locals:
-                        tb["locals"] = frame.f_locals
-                    if self.exc_pass_globals:
-                        tb["globals"] = frame.f_globals
+                if self.exc_pass_filenames:
+                    tb_dict["filename"] = (frame.tb_frame.f_code.co_filename,)
+                if self.exc_pass_locals:
+                    tb_dict["locals"] = frame.tb_frame.f_locals
 
         return self.__class__.serializer(data)
-
-    def __str__(self):
-        return f"<{self.__class__.__name__}>"
```

## uvlog/handlers.py

```diff
@@ -3,19 +3,18 @@
 import queue
 import sys
 import traceback
 from abc import ABC, abstractmethod
 from pathlib import Path
 from threading import Thread
 from time import sleep
-from typing import BinaryIO, List, Optional, cast, no_type_check
+from typing import BinaryIO, List, Optional, cast, no_type_check, ClassVar
 from urllib.parse import urlparse
 
-from uvlog.formatters import TextFormatter
-from uvlog.uvlog import Formatter, Handler, LevelName, LogRecord, name_to_level
+from uvlog.uvlog import Formatter, Handler, LevelName, LogRecord
 
 __all__ = ["StreamHandler", "QueueHandler", "QueueStreamHandler", "handle_error"]
 
 
 @no_type_check
 def handle_error(message: bytes, /) -> None:
     """Handle an error which occurs during an emit() call.
@@ -30,110 +29,94 @@
         frame = exc.__traceback__.tb_frame
         while frame:
             frame = frame.f_back
         if frame:
             traceback.print_stack(frame, file=sys.stderr)
         try:
             sys.stderr.write(f"Message: {message}\n")
-        except RecursionError:
+        except Exception:
             raise
-        except Exception:  # noqa: acceptable
-            sys.stderr.write(
-                "Unable to print the message and arguments"
-                " - possible formatting error.\nUse the"
-                " traceback above to help find the error.\n"
-            )
     except OSError:
         pass
     finally:
         del exc
 
 
 class StreamHandler(Handler):
     """Logging handler.
 
     A simple stream handler which immediately writes a log record to the write buffer. It provides the best performance.
     However, in server applications you may want to use `uvlog.QueueStreamLogger`
     to ensure your code is not blocking due to intensive logging.
     """
 
-    terminator = b"\n"
+    terminator: ClassVar = b"\n"
+    route_prefix: ClassVar = "file"
 
-    _level: LevelName
-    _levelno: int
-    _formatter: Formatter
-    _dest: str
     _stream: Optional[BinaryIO]
 
-    def __init__(self):
+    def __init__(self, route: str, formatter: Formatter, level: LevelName) -> None:
         """Initialize."""
-        self._level = "DEBUG"
-        self._levelno = name_to_level["DEBUG"]
-        self._formatter = TextFormatter()
-        self._dest = "stderr"
+        super().__init__(route, formatter, level)
         self._stream = None
+        if self.route not in ("stderr", "stdout"):
+            _path = Path(urlparse(route).path).absolute()
+            _path.parent.mkdir(parents=True, exist_ok=True)
+            _path.touch(exist_ok=True)
 
     def handle(self, record: LogRecord, /) -> None:
         """Immediately write a log record to the write buffer."""
-        if record.levelno < self._levelno:
+        if record.levelno < self.levelno:
             return
         if self._stream is None:
             self.open_stream()
-        record_bytes = self._formatter.format_record(record)
+        record_bytes = self.formatter.format_record(record)
         try:
             cast(BinaryIO, self._stream).write(record_bytes + self.terminator)
         except Exception:  # noqa: acceptable
             handle_error(record_bytes)
 
-    def set_level(self, level: LevelName, /) -> None:
-        self._level = level
-        self._levelno = name_to_level[level]
-
-    def set_formatter(self, formatter: Formatter, /) -> None:
-        self._formatter = formatter
-
-    def set_destination(self, dest: str, /) -> None:
-        """Set log destination (file stream).
-
-        Pre-configured destinations are: 'stdout' and 'stderr'.
+    @classmethod
+    def accepts_destination(cls, route: str, /) -> bool:
+        return any(
+            (
+                route in ("stderr", "stdout"),
+                route.startswith(cls.route_prefix + ":"),
+                route.startswith("./"),
+                route.startswith("../"),
+                route.startswith("/"),
+            )
+        )
 
-        Both plain and URL file formats are acceptable and normalized into a path string:
-
-        - logs.txt - relative path
-        - /logs.txt - absolute path
-        - file:///logs.txt - absolute path in file URL format
-        """
-        self._dest = dest
-        if dest not in ("stderr", "stdout"):
-            _path = Path(urlparse(dest).path).absolute()
-            _path.parent.mkdir(parents=True, exist_ok=True)
-            _path.touch(exist_ok=True)
+    @classmethod
+    def resolve_destination(cls, route: str, /) -> str:
+        if route in ("stderr", "stdout"):
+            return route
+        _path = Path(urlparse(route).path).resolve()
+        return str(_path)
 
     def close(self) -> None:
         """Close the handler including all connections to its destination.
 
         This method is called automatically at exit for each added handler by the :py:func:`~uvlog.clear` function.
         """
         if self._stream and not self._stream.closed:
             self._stream.flush()
             if self._stream not in (sys.stderr.buffer, sys.stdout.buffer):
                 self._stream.close()
         self._stream = None
 
     def open_stream(self) -> None:
         """Open a file stream."""
-        if self._dest == "stderr":
+        if self.route == "stderr":
             self._stream = sys.stderr.buffer
-        elif self._dest == "stdout":
+        elif self.route == "stdout":
             self._stream = sys.stdout.buffer
         else:
-            self._stream = open(self._dest, "ab")
-
-    def __str__(self) -> str:
-        return f"<{self.__class__.__name__}: {self._dest} / {self._formatter}>"
+            self._stream = open(self.route, "ab")
 
 
 class QueueHandler(Handler, ABC):
     """Logging handler with an internal queue.
 
     The handler uses a separate thread to write logs to the buffer via the :py:meth:`~uvlog.QueueHandler.write`
     method. Note that this handler doesn't use any internal locks,
@@ -145,29 +128,24 @@
     queue_size: int
     """Log queue size, infinite by default"""
 
     batch_size: int
     """Maximum number of log records to concatenate and write at once,
     consider setting it so an average batch would be ~ tens of KBs"""
 
-    _level: LevelName
-    _levelno: int
     _write_queue: queue.Queue
     _thread: Optional[Thread]
-    _formatter: Formatter
 
-    def __init__(self):
+    def __init__(self, route: str, formatter: Formatter, level: LevelName) -> None:
         """Initialize."""
+        super().__init__(route, formatter, level)
         self.queue_size = -1
         self.batch_size = 50
-        self._level = "DEBUG"
-        self._levelno = name_to_level["DEBUG"]
         self._write_queue = queue.Queue()
         self._thread = None
-        self._formatter = TextFormatter()
 
     @abstractmethod
     def open_stream(self) -> None:
         """Open a stream and prepare for sending logs there."""
         # self._stream = ...
 
     @abstractmethod
@@ -175,42 +153,31 @@
         """Close the stream if opened."""
         # self._stream = None
         # ...
 
     @abstractmethod
     def write_records(self, formatted_records: List[bytes], /) -> None: ...
 
-    def __post_init__(self):
-        self._levelno = name_to_level[self._level]
-        self._write_queue.maxsize = self.queue_size
-
-    def set_level(self, level: LevelName, /) -> None:
-        self._level = level
-        self._levelno = name_to_level[level]
-
-    def set_formatter(self, formatter: Formatter, /) -> None:
-        self._formatter = formatter
-
     def handle(self, record: LogRecord, /) -> None:
         """Put a log record to the write queue."""
-        if record.levelno < self._levelno:
+        if record.levelno < self.levelno:
             return
         if self._thread is None:
             self._thread = self._open_thread()
         self._write_queue.put(record)
 
     def write(self) -> None:
         """Write logs from the queue to the stream.
 
         This method is executed in a separate thread.
         """
         _queue = self._write_queue
         _queue.maxsize = self.queue_size
         _sentinel = self._sentinel
-        _formatter = self._formatter
+        _formatter = self.formatter
         _batch_size = self.batch_size
         _formatted_records: List[bytes] = []
         _exit = False
         self.open_stream()
 
         while not _exit:
             if _queue.qsize():
@@ -269,18 +236,18 @@
     queue_size: int
     """Log queue size, infinite by default"""
 
     batch_size: int
     """Maximum number of log records to concatenate and write at once,
     consider setting it so an average batch would be ~ tens of KBs"""
 
-    def __init__(self):
+    def __init__(self, route: str, formatter: Formatter, level: LevelName) -> None:
         """Initialize."""
-        QueueHandler.__init__(self)
-        StreamHandler.__init__(self)
+        QueueHandler.__init__(self, route, formatter, level)
+        StreamHandler.__init__(self, route, formatter, level)
 
     def open_stream(self) -> None:
         StreamHandler.open_stream(self)
 
     def close_stream(self) -> None:
         StreamHandler.close(self)
```

## uvlog/uvlog.py

```diff
@@ -1,45 +1,44 @@
 """Python logging utilities."""
 
 import logging
 import os
 import sys
-from abc import abstractmethod
+from abc import abstractmethod, ABC
 from collections import ChainMap
 from contextvars import ContextVar  # noqa: pycharm bug?
+from copy import deepcopy
 from dataclasses import dataclass, field
 from datetime import datetime
 from random import random
 from typing import (
     Any,
     Dict,
     List,
     Literal,
     Mapping,
     Optional,
     Protocol,
     Type,
     TypedDict,
     cast,
+    ClassVar,
 )
 from weakref import WeakValueDictionary
 
 __all__ = [
     "LOG_CONTEXT",
     "BASIC_CONFIG",
     "LogRecord",
     "Logger",
     "Handler",
     "Formatter",
     "add_formatter_type",
     "add_handler_type",
     "set_logger_type",
-    "add_handler",
-    "add_formatter",
-    "remove_handler",
     "get_logger",
     "configure",
     "clear",
     "LevelName",
     "name_to_level",
 ]
 
@@ -125,18 +124,17 @@
     message: str
     """Log message"""
 
     exc_info: Optional[Exception]
     """Exception (if any)"""
 
     args: Optional[tuple]
-    """Log extra information provided as positional arguments.
-    
-    This attribute is left only for compatibility reasons. It's better to use keyword arguments and `extra`
-    attribute instead.
+    """Log call positional arguments.
+
+    This attribute is left only for compatibility reasons. It's not used in formatting log messages.
     """
 
     extra: Optional[Mapping[str, Any]]
     """Log extra information provided in kwargs"""
 
     ctx: Optional[Mapping[str, Any]]
     """Log contextual information"""
@@ -146,97 +144,78 @@
 
     func: Optional[str]
     """Function name of the caller"""
 
     lineno: Optional[int]
     """Source code line number of the caller"""
 
-    def __getitem__(self, item: str, /):
-        return getattr(self, item)
-
 
 class Formatter(Protocol):
     """Log formatter interface.
 
     It's a protocol class, i.e. one doesn't need to inherit from it to create a valid formatter.
     """
 
     @abstractmethod
     def format_record(self, record: LogRecord, /) -> bytes: ...
 
+    def __str__(self) -> str:
+        return f"<{self.__class__.__name__}>"
 
-class Handler(Protocol):
+
+class Handler(ABC):
     """Log handler interface.
 
     It's a protocol class, i.e. one doesn't need to inherit from it to create a valid handler.
     """
 
-    @abstractmethod
-    def handle(self, record: LogRecord, /) -> None: ...
+    route_prefix: ClassVar[str]
 
-    @abstractmethod
-    def set_level(self, level: LevelName, /) -> None: ...
+    def __init__(self, route: str, formatter: Formatter, level: LevelName) -> None:
+        """Initialize."""
+        self.route = route
+        self.formatter = formatter
+        self.level = level
+        self.levelno = name_to_level[level]
 
-    @abstractmethod
-    def set_formatter(self, fmt: Formatter, /) -> None: ...
+    @classmethod
+    def accepts_destination(cls, route: str, /) -> bool:
+        return route.startswith(cls.route_prefix + ":")
 
+    @classmethod
     @abstractmethod
-    def set_destination(self, dest: str, /) -> None:
-        """Set a handler destination.
+    def resolve_destination(cls, route: str, /) -> str:
+        """Resolve destination route and normalize it."""
 
-        Since only one destination allowed for a single handler, this method must call :py:func:`~uvlog.add_handler`
-        to ensure that a handler for this destination doesn't exist. It also should call
-        :py:func:`~uvlog.remove_handler` for its previous destination before adding a new one.
-
-        Example:
-
-        .. code-block:: python
-
-            def set_destination(self, dest: str, /) -> None:
-                remove_handler(self._dest)
-                self._dest = dest
-                ...
-                add_handler(dest)
+    @abstractmethod
+    def handle(self, record: LogRecord, /) -> None: ...
 
-        """
-        # remove_handler(self.dest)
-        # add_handler(dest, self)
+    def set_level(self, level: LevelName, /) -> None:
+        self.level = level
+        self.levelno = name_to_level[level]
 
     @abstractmethod
     def close(self) -> None:
         """Close the handler including all connections to its destination.
 
         This method is called automatically at exit for each added handler by the :py:func:`~uvlog.clear` function.
         """
 
+    def __str__(self) -> str:
+        return f"<{self.__class__.__name__}: {self.route} / {self.formatter}>"
+
 
 def add_formatter_type(typ: Type[Formatter], /) -> None:
     _formatter_types[typ.__name__] = typ
 
 
 def add_handler_type(typ: Type[Handler], /) -> None:
     _handler_types[typ.__name__] = typ
 
 
-def add_formatter(name: str, formatter: Formatter, /) -> None:
-    _formatters[name] = formatter
-
-
-def add_handler(destination: str, handler: Handler, /) -> None:
-    if destination in _handlers:
-        remove_handler(destination)
-    _handlers[destination] = handler
-
-
-def remove_handler(destination: str, /) -> None:
-    handler = _handlers.pop(destination, None)
-    if handler is not None:
-        handler.close()
-
-
 @dataclass
 class Logger:
     """Logger object.
 
     It can be used almost like a standard Python logger, except that it allows passing keyword arguments
     directly to `extra`:
 
@@ -257,15 +236,15 @@
     """Logging level"""
 
     handlers: List[Handler] = field(default_factory=list)
     """List of attached log handlers"""
 
     sample_rate: float = 1.0
     """Log records sample rate which determines a probability at which a record should be sampled.
-    
+
     Sample rate is not considered for levels above 'INFO'. Values >= 1 disable the sampling mechanism.
     """
 
     sample_propagate: bool = True
     """By default the sampling mechanism is contextual meaning that if there's a non-empty log context,
     the log chain is marked 'sampled' as it sampled by the first logger in a chain. Once a record is 'sampled' the
     log chain cannot be *unsampled*, i.e. all subsequent loggers will be forced to sample it as well.
@@ -335,15 +314,15 @@
         *args,
         exc_info: Optional[Exception] = None,
         stack_info=None,
         stacklevel=1,
         **kws,
     ) -> None:
         ctx = self.context.get()
-        if ctx:
+        if ctx and self.sample_rate < 1.0:
             ctx["_sample"] = True
         self._log(
             "NEVER",
             name_to_level["NEVER"],
             msg,
             exc_info,
             stack_info,
@@ -363,15 +342,15 @@
         stacklevel=1,
         **kws,
     ) -> None:
         levelno = name_to_level["CRITICAL"]
         if self._levelno > levelno:
             return
         ctx = self.context.get()
-        if ctx:
+        if ctx and self.sample_rate < 1.0:
             ctx["_sample"] = True
         self._log(
             "CRITICAL", levelno, msg, exc_info, stack_info, stacklevel, ctx, args, kws
         )
 
     def error(
         self,
@@ -383,15 +362,15 @@
         stacklevel=1,
         **kws,
     ) -> None:
         levelno = name_to_level["ERROR"]
         if self._levelno > levelno:
             return
         ctx = self.context.get()
-        if ctx:
+        if ctx and self.sample_rate < 1.0:
             ctx["_sample"] = True
         self._log(
             "ERROR", levelno, msg, exc_info, stack_info, stacklevel, ctx, args, kws
         )
 
     def warning(
         self,
@@ -403,15 +382,15 @@
         stacklevel=1,
         **kws,
     ) -> None:
         levelno = name_to_level["WARNING"]
         if self._levelno > levelno:
             return
         ctx = self.context.get()
-        if ctx:
+        if ctx and self.sample_rate < 1.0:
             ctx["_sample"] = True
         self._log(
             "WARNING", levelno, msg, exc_info, stack_info, stacklevel, ctx, args, kws
         )
 
     def info(
         self,
@@ -557,47 +536,54 @@
         if key in _new_dict and isinstance(value, dict):
             _new_dict[key] = _merge_dicts(_new_dict[key], value)
         else:
             _new_dict[key] = value
     return _new_dict
 
 
-def _configure_formatter(name: str, params: dict, /) -> None:
+def _create_formatter(params: dict, /) -> Formatter:
     cls = _formatter_types[params.pop("class", "TextFormatter")]
-    _formatter = cls()
+    formatter = cls()
     for key, value in params.items():
         if not key.startswith("_"):
-            setattr(_formatter, key, value)
-    _formatters[name] = _formatter
+            setattr(formatter, key, value)
+    return formatter
 
 
-def _configure_handler(dest: str, params: dict, /) -> None:
+def _create_handler(route: str, params: dict, /) -> Handler:
     cls_name = params.pop("class", "StreamHandler")
-    _handler = _handler_types[cls_name]()
-    _handler.set_destination(dest)
+    _handler_type = _handler_types[cls_name]
+    if not _handler_type.accepts_destination(route):
+        raise ValueError(
+            f'Handler of type "{cls_name}" doesn\'t accept destination "{route}"'
+        )
+
+    route = _handler_type.resolve_destination(route)
+    if route in _handlers:
+        raise ValueError(f'Handler already exists for route "{route}"')
+
     formatter_name = params.pop("formatter", "text")
-    _handler.set_formatter(_formatters[formatter_name])
     level: LevelName = cast(LevelName, params.pop("level", "DEBUG"))
-    _handler.set_level(level)
+    handler = _handler_type(route, _formatters[formatter_name], level)
     for key, value in params.items():
         if not key.startswith("_"):
-            setattr(_handler, key, value)
-    _handlers[dest] = _handler
+            setattr(handler, key, value)
+    return handler
 
 
-def _configure_logger(name: str, params: dict, context_var: ContextVar, /) -> None:
-    _logger = get_logger(name, persistent=True)
+def _create_logger(name: str, params: dict, /) -> Logger:
+    logger = get_logger(name, persistent=True)
     handler_names = params.pop("handlers", ["stderr"])
-    _logger.handlers = [_handlers[handler_name] for handler_name in handler_names]
+    logger.handlers = [_handlers[handler_name] for handler_name in handler_names]
     level: LevelName = cast(LevelName, params.pop("level", "INFO"))
-    _logger.set_level(level)
-    _logger.context = context_var
+    logger.set_level(level)
     for key, value in params.items():
         if not key.startswith("_"):
-            setattr(_logger, key, value)
+            setattr(logger, key, value)
+    return logger
 
 
 def configure(
     config_dict: _DictConfig, /, context_var: ContextVar = LOG_CONTEXT
 ) -> Logger:
     """Configure loggers for a configuration dict.
 
@@ -647,31 +633,37 @@
         by passing a config. If you want to configure logging from zero you should call `clear()` method beforehand.
         Please note that you need to provide all the handlers, formatters, loggers in the config after doing that,
         including the root logger (empty string).
 
     """
     clear()
     config_dict = cast(
-        _DictConfig, _merge_dicts(cast(dict, BASIC_CONFIG), cast(dict, config_dict))
+        _DictConfig,
+        _merge_dicts(cast(dict, deepcopy(BASIC_CONFIG)), cast(dict, config_dict)),
     )
     for name, params in config_dict["formatters"].items():
-        _configure_formatter(name, params)
-    for dest, params in config_dict["handlers"].items():
-        _configure_handler(dest, params)
+        _formatter = _create_formatter(params)
+        _formatters[name] = _formatter
+    for route, params in config_dict["handlers"].items():
+        _handler = _create_handler(route, params)
+        _handlers[route] = _handler
     # sorting loggers to init parents before children
     loggers_params = list(config_dict["loggers"].items())
     loggers_params.sort(key=lambda x: x[0])
     for name, params in loggers_params:
-        _configure_logger(name, params, context_var)
+        _logger = _create_logger(name, params)
+        _logger.context = context_var
+        _loggers[name] = _logger
     return _loggers[_root_logger_name]
 
 
 def clear() -> None:
     """Clear all existing loggers, handlers and formatters.
 
     This function also closes all existing handlers.
     """
     _loggers_temp.clear()
     _loggers_persistent.clear()
-    for handler in tuple(_handlers):
-        remove_handler(handler)
+    for handler in _handlers.values():
+        handler.close()
+    _handlers.clear()
     _formatters.clear()
```

## Comparing `uvlog-0.1.3.dist-info/LICENSE` & `uvlog-0.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `uvlog-0.1.3.dist-info/METADATA` & `uvlog-0.1.4.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uvlog
-Version: 0.1.3
+Version: 0.1.4
 Summary: Pythonic logger with better performance and contextvars + JSON support out of the box
 Home-page: https://github.com/violet-black/uvlog
 Author: violetblackdev@gmail.com
 License: MIT
 Keywords: logging,logs
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -27,111 +27,83 @@
 Provides-Extra: dev
 Requires-Dist: pip-tools ; extra == 'dev'
 Requires-Dist: tox ; extra == 'dev'
 Requires-Dist: coverage ; extra == 'dev'
 Requires-Dist: mypy ; extra == 'dev'
 Requires-Dist: isort ; extra == 'dev'
 Requires-Dist: black ; extra == 'dev'
-Requires-Dist: bump2version ; extra == 'dev'
-Requires-Dist: bandit ; extra == 'dev'
-Requires-Dist: xenon ; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: sphinx ; extra == 'docs'
 Requires-Dist: python-docs-theme ; extra == 'docs'
+Requires-Dist: m2r2 ; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: pytest ==8.1.1 ; extra == 'test'
-Requires-Dist: orjson ==3.9.15 ; extra == 'test'
 
-[![PyPi Version](https://img.shields.io/pypi/v/uvlog.svg)](https://pypi.python.org/pypi/uvlog/)
-[![Docs](https://readthedocs.org/projects/uvlog/badge/?version=latest&style=flat)](https://uvlog.readthedocs.io)
+[![pypi](https://img.shields.io/pypi/v/uvlog.svg)](https://pypi.python.org/pypi/uvlog/)
+[![docs](https://readthedocs.org/projects/uvlog/badge/?version=latest&style=flat)](https://uvlog.readthedocs.io)
+[![codecov](https://codecov.io/gh/violet-black/uvlog/graph/badge.svg?token=FEUUMQELFX)](https://codecov.io/gh/violet-black/uvlog)
+[![tests](https://github.com/violet-black/uvlog/actions/workflows/tests.yaml/badge.svg)](https://github.com/violet-black/uvlog/actions/workflows/tests.yaml)
 [![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-[![3.8](https://github.com/violet-black/uvlog/actions/workflows/py38.yaml/badge.svg)](https://github.com/violet-black/uvlog/actions/workflows/py38.yaml)
-[![3.9](https://github.com/violet-black/uvlog/actions/workflows/py39.yaml/badge.svg)](https://github.com/violet-black/uvlog/actions/workflows/py39.yaml)
-[![3.10](https://github.com/violet-black/uvlog/actions/workflows/py310.yaml/badge.svg)](https://github.com/violet-black/uvlog/actions/workflows/py310.yaml)
-[![3.11](https://github.com/violet-black/uvlog/actions/workflows/py311.yaml/badge.svg)](https://github.com/violet-black/uvlog/actions/workflows/py311.yaml)
-[![3.12](https://github.com/violet-black/uvlog/actions/workflows/py312.yaml/badge.svg)](https://github.com/violet-black/uvlog/actions/workflows/py312.yaml)
+**uvlog** is yet another Python logging library built with an idea of a simple logger what 'just works' without
+need for extension and customization.
 
-**uvlog** is yet another logging library built with an idea of a simple logger what 'just works' without
-need for extension and customization. 
-
-- Single package, no other dependencies
+- Single package, no dependencies
 - JSON and [contextvars](https://docs.python.org/3/library/contextvars.html) out of the box
 - Less abstraction, better [performance](#Performance)
 - Pythonic method names and classes
 
+# Installation
+
+With pip and python 3.8+:
+
+```bash
+pip3 install uvlog
+```
+
 # Use
 
 Our main scenario is logging our containerized server applications, i.e. writing all the logs to the stderr
 of the container, where they are gathered and sent to the log storage by another service. However, you
-can use this library for any application as long as it does not require very complicated things like
-complex filters, adapters etc.
-
-The easiest way to access a logger is similar to the standard module. Note that you can pass
-extra variables as keyword arguments while logging.
+can use this library for any application as long as it doesn't require complicated things like filters, adapters etc.
 
 ```python
 from uvlog import get_logger
 
 logger = get_logger('app')
-logger.set_level('DEBUG')
 
 logger.info('Hello, {name} {surname}!', name='John', surname='Dowe')
 ```
 
-To write an exception use `exc_info` param.
+Note that you can use extras directly as variable keys in log calls (variable positional args are stored in a log
+record but not supported by the formatter).
+
+To write an exception use `exc_info` as in the standard logger.
 
 ```python
 try:
     ...
 except ValueError as exc:
     logger.error('Something bad happened', exc_info=exc)
 ```
 
-Configuration is possible in a way similar to `dictConfig`. The configuration dict itself is JSON compatible.
-The `configure()` function returns the root logger instance. Note that one destination can be assigned to
-only one handler, but each logger can have any number of handlers.
-
-Here's an extensive example of such config.
+Log configuration is similar to *dictConfig*. It updates the default configuration.
 
 ```python
 from uvlog import configure
 
 logger = configure({
     'loggers': {
-        '': {  # the root logger
-            'level': 'DEBUG',
-            'handlers': ['stderr', '/etc/log.txt']
-        }
+        '': {'level': 'DEBUG', 'handlers': ['./log.txt']}
     },
     'handlers': {
-        'stderr': {  # 'stderr' and 'stdout' are reserved for these special destinations
-            'class': 'StreamHandler',
-            'formatter': 'json'
-        },
-        '/etc/log.txt': {
-            'class': 'QueueStreamHandler',
-            'formatter': 'text'
-        }
-    },
-    'formatters': {
-        'text': {
-            'class': 'TextFormatter',
-            'format': '{asctime} : {name} : {message}',  # see `LogRecord` for the list of fields
-            'timestamp_separator': ' '                   # by default it's 'T'
-        },
-        'json': {
-            'class': 'JSONFormatter',
-            'keys': ['asctime', 'name', 'message']       # see `LogRecord` for the list of fields
-        }
+        './log.txt': {'formatter': 'json'}
     }
 })
-
-app_logger = logger.get_child('app', persistent=True)
 ```
 
 You can use context variables to maintain log context between log records. This can be useful for log aggregation.
 See the [documentation on contextvars](https://uvlog.readthedocs.io/guide.html#context-variables) for more info.
 
 ```python
 from uvlog import LOG_CONTEXT, get_logger
@@ -204,22 +176,20 @@
 ... or via a config dict
 
 ```python
 from uvlog import configure
 
 configure({
     'loggers': {
-        '': {
-            'sample_rate': 0.25
-        }
+        '': {'sample_rate': 0.25}
     }
 })
 ```
 
-See the [documentation on sampling](https://uvlog.readthedocs.io/guide.html#sampling>) for more info.
+See the [documentation on sampling](https://uvlog.readthedocs.io/guide.html#sampling) for more info.
 
 # Customization
 
 You can create custom formatters and handlers with ease. Note that inheritance is not required.
 Just be sure to implement `Handler` / `Formatter` protocol.
 
 See the extension guide for more info. There's an example of
@@ -242,15 +212,7 @@
 # Compatibility
 
 There's a certain compatibility between this logger and the standard logger. However, it's impossible to preserve
 full compatibility because of certain design decisions.
 
 See the [compatibility guide](https://uvlog.readthedocs.io/compatibility.html) if you want to migrate from the standard
 python logger to this one.
-
-# Ideas / goals
-
-- Rotating file handlers
-- Asynchronous queue logging to HTTP / TCP / UDP
-- Better customization for `Logger` / `LogRecord` objects
-- Better coverage
-- Cython?
```

## Comparing `uvlog-0.1.3.dist-info/RECORD` & `uvlog-0.1.4.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-uvlog/__init__.py,sha256=6hkBDN-uPHf37E8uggmN7EqpXbxqM9rQOItTzY0FZ2Y,1119
-uvlog/formatters.py,sha256=Jgcncafov667V0nk3wiWcE4ltTeJiDLwKajpYw0atwY,5448
-uvlog/handlers.py,sha256=qCthEKp3t8JQGBuvCHSwIB_V221MYohHTiKvyne4Csc,9844
-uvlog/uvlog.py,sha256=F2w-wHLKZUMR4ropzvS_K8b2rdDQfuciZanr6BAjxYM,20197
-uvlog-0.1.3.dist-info/LICENSE,sha256=VikX3YBzWiCgZEgI93vz50l4NdJDPjkmxFbYK9IogJ8,1069
-uvlog-0.1.3.dist-info/METADATA,sha256=pU49zKsMEeYMOwrrFoGgAtFXO7OwdPts7i53jin3vQc,9820
-uvlog-0.1.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-uvlog-0.1.3.dist-info/top_level.txt,sha256=7N0XBLVOTPNRRkh7r8aWji2mHqajODsmoUXOY8wXHBY,6
-uvlog-0.1.3.dist-info/RECORD,,
+uvlog/__init__.py,sha256=YCJBMudjjNp-m_DkorTfo2xfvKdO42DX8pbgJumnQR4,1119
+uvlog/formatters.py,sha256=Um6OMHBquQmMFSqLJgCmhPDaz6RsH-1-s0YZKezogCg,5340
+uvlog/handlers.py,sha256=Alm05ZHxBuA3l7pKci86EN9yRpLsmnIA8pKdCa5EdAQ,8939
+uvlog/uvlog.py,sha256=kARehu8QDnuYKLXY47EoUJZ30m_bkbXSMpL2yAjw6Io,20079
+uvlog-0.1.4.dist-info/LICENSE,sha256=VikX3YBzWiCgZEgI93vz50l4NdJDPjkmxFbYK9IogJ8,1069
+uvlog-0.1.4.dist-info/METADATA,sha256=-Rkh5TsJ3BsCvLCvUmK6dT282mRNThvRZLmgfU9bELQ,8020
+uvlog-0.1.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+uvlog-0.1.4.dist-info/top_level.txt,sha256=7N0XBLVOTPNRRkh7r8aWji2mHqajODsmoUXOY8wXHBY,6
+uvlog-0.1.4.dist-info/RECORD,,
```

