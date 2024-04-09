# Comparing `tmp/pyventus-0.4.1.tar.gz` & `tmp/pyventus-0.5.0.tar.gz`

## Comparing `pyventus-0.4.1.tar` & `pyventus-0.5.0.tar`

### file list

```diff
@@ -1,55 +1,51 @@
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 pyventus-0.4.1/CITATION.cff
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 pyventus-0.4.1/src/pyventus/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyventus-0.4.1/src/pyventus/core/__init__.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pyventus-0.4.1/src/pyventus/core/constants/__init__.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 pyventus-0.4.1/src/pyventus/core/constants/stdout_colors.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pyventus-0.4.1/src/pyventus/core/exceptions/__init__.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 pyventus-0.4.1/src/pyventus/core/exceptions/pyventus_exception.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 pyventus-0.4.1/src/pyventus/core/loggers/__init__.py
--rw-r--r--   0        0        0     2674 2020-02-02 00:00:00.000000 pyventus-0.4.1/src/pyventus/core/loggers/logger.py
--rw-r--r--   0        0        0     6528 2020-02-02 00:00:00.000000 pyventus-0.4.1/src/pyventus/core/loggers/stdout_logger.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 pyventus-0.4.1/src/pyventus/emitters/__init__.py
--rw-r--r--   0        0        0    12295 2020-02-02 00:00:00.000000 pyventus-0.4.1/src/pyventus/emitters/event_emitter.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 pyventus-0.4.1/src/pyventus/emitters/asyncio/__init__.py
--rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 pyventus-0.4.1/src/pyventus/emitters/asyncio/asyncio_event_emitter.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pyventus-0.4.1/src/pyventus/emitters/celery/__init__.py
--rw-r--r--   0        0        0    11399 2020-02-02 00:00:00.000000 pyventus-0.4.1/src/pyventus/emitters/celery/celery_event_emitter.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 pyventus-0.4.1/src/pyventus/emitters/executor/__init__.py
--rw-r--r--   0        0        0     4577 2020-02-02 00:00:00.000000 pyventus-0.4.1/src/pyventus/emitters/executor/executor_event_emitter.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 pyventus-0.4.1/src/pyventus/emitters/fastapi/__init__.py
--rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 pyventus-0.4.1/src/pyventus/emitters/fastapi/fastapi_event_emitter.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 pyventus-0.4.1/src/pyventus/emitters/rq/__init__.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 pyventus-0.4.1/src/pyventus/emitters/rq/rq_event_emitter.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pyventus-0.4.1/src/pyventus/events/__init__.py
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 pyventus-0.4.1/src/pyventus/events/event.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pyventus-0.4.1/src/pyventus/handlers/__init__.py
--rw-r--r--   0        0        0     8957 2020-02-02 00:00:00.000000 pyventus-0.4.1/src/pyventus/handlers/event_handler.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pyventus-0.4.1/src/pyventus/linkers/__init__.py
--rw-r--r--   0        0        0    28111 2020-02-02 00:00:00.000000 pyventus-0.4.1/src/pyventus/linkers/event_linker.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 pyventus-0.4.1/tests/__init__.py
--rw-r--r--   0        0        0     6341 2020-02-02 00:00:00.000000 pyventus-0.4.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyventus-0.4.1/tests/core/__init__.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 pyventus-0.4.1/tests/core/test_logger.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyventus-0.4.1/tests/emitters/__init__.py
--rw-r--r--   0        0        0    12955 2020-02-02 00:00:00.000000 pyventus-0.4.1/tests/emitters/event_emitter_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyventus-0.4.1/tests/emitters/asyncio/__init__.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 pyventus-0.4.1/tests/emitters/asyncio/test_asyncio_event_emitter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyventus-0.4.1/tests/emitters/celery/__init__.py
--rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 pyventus-0.4.1/tests/emitters/celery/test_celery_event_emitter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyventus-0.4.1/tests/emitters/executor/__init__.py
--rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 pyventus-0.4.1/tests/emitters/executor/test_executor_event_emitter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyventus-0.4.1/tests/emitters/fastapi/__init__.py
--rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 pyventus-0.4.1/tests/emitters/fastapi/test_fastapi_event_emitter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyventus-0.4.1/tests/emitters/rq/__init__.py
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 pyventus-0.4.1/tests/emitters/rq/test_rq_event_emitter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyventus-0.4.1/tests/events/__init__.py
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 pyventus-0.4.1/tests/events/test_event.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyventus-0.4.1/tests/handlers/__init__.py
--rw-r--r--   0        0        0    10015 2020-02-02 00:00:00.000000 pyventus-0.4.1/tests/handlers/test_event_handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyventus-0.4.1/tests/linkers/__init__.py
--rw-r--r--   0        0        0    29025 2020-02-02 00:00:00.000000 pyventus-0.4.1/tests/linkers/test_event_linker.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 pyventus-0.4.1/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 pyventus-0.4.1/LICENSE
--rw-r--r--   0        0        0    17821 2020-02-02 00:00:00.000000 pyventus-0.4.1/README.md
--rw-r--r--   0        0        0     5801 2020-02-02 00:00:00.000000 pyventus-0.4.1/pyproject.toml
--rw-r--r--   0        0        0    20434 2020-02-02 00:00:00.000000 pyventus-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 pyventus-0.5.0/CITATION.cff
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 pyventus-0.5.0/src/pyventus/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyventus-0.5.0/src/pyventus/core/__init__.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pyventus-0.5.0/src/pyventus/core/constants/__init__.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 pyventus-0.5.0/src/pyventus/core/constants/stdout_colors.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pyventus-0.5.0/src/pyventus/core/exceptions/__init__.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 pyventus-0.5.0/src/pyventus/core/exceptions/pyventus_exception.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 pyventus-0.5.0/src/pyventus/core/loggers/__init__.py
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 pyventus-0.5.0/src/pyventus/core/loggers/logger.py
+-rw-r--r--   0        0        0     6394 2020-02-02 00:00:00.000000 pyventus-0.5.0/src/pyventus/core/loggers/stdout_logger.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 pyventus-0.5.0/src/pyventus/emitters/__init__.py
+-rw-r--r--   0        0        0    11154 2020-02-02 00:00:00.000000 pyventus-0.5.0/src/pyventus/emitters/event_emitter.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 pyventus-0.5.0/src/pyventus/emitters/asyncio/__init__.py
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 pyventus-0.5.0/src/pyventus/emitters/asyncio/asyncio_event_emitter.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pyventus-0.5.0/src/pyventus/emitters/celery/__init__.py
+-rw-r--r--   0        0        0    11064 2020-02-02 00:00:00.000000 pyventus-0.5.0/src/pyventus/emitters/celery/celery_event_emitter.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 pyventus-0.5.0/src/pyventus/emitters/executor/__init__.py
+-rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 pyventus-0.5.0/src/pyventus/emitters/executor/executor_event_emitter.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 pyventus-0.5.0/src/pyventus/emitters/fastapi/__init__.py
+-rw-r--r--   0        0        0     3913 2020-02-02 00:00:00.000000 pyventus-0.5.0/src/pyventus/emitters/fastapi/fastapi_event_emitter.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 pyventus-0.5.0/src/pyventus/emitters/rq/__init__.py
+-rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 pyventus-0.5.0/src/pyventus/emitters/rq/rq_event_emitter.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pyventus-0.5.0/src/pyventus/handlers/__init__.py
+-rw-r--r--   0        0        0    11615 2020-02-02 00:00:00.000000 pyventus-0.5.0/src/pyventus/handlers/event_handler.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pyventus-0.5.0/src/pyventus/linkers/__init__.py
+-rw-r--r--   0        0        0    31357 2020-02-02 00:00:00.000000 pyventus-0.5.0/src/pyventus/linkers/event_linker.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pyventus-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     8362 2020-02-02 00:00:00.000000 pyventus-0.5.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyventus-0.5.0/tests/core/__init__.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 pyventus-0.5.0/tests/core/test_logger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyventus-0.5.0/tests/emitters/__init__.py
+-rw-r--r--   0        0        0    13551 2020-02-02 00:00:00.000000 pyventus-0.5.0/tests/emitters/event_emitter_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyventus-0.5.0/tests/emitters/asyncio/__init__.py
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 pyventus-0.5.0/tests/emitters/asyncio/test_asyncio_event_emitter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyventus-0.5.0/tests/emitters/celery/__init__.py
+-rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 pyventus-0.5.0/tests/emitters/celery/test_celery_event_emitter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyventus-0.5.0/tests/emitters/executor/__init__.py
+-rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 pyventus-0.5.0/tests/emitters/executor/test_executor_event_emitter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyventus-0.5.0/tests/emitters/fastapi/__init__.py
+-rw-r--r--   0        0        0     3974 2020-02-02 00:00:00.000000 pyventus-0.5.0/tests/emitters/fastapi/test_fastapi_event_emitter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyventus-0.5.0/tests/emitters/rq/__init__.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pyventus-0.5.0/tests/emitters/rq/test_rq_event_emitter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyventus-0.5.0/tests/handlers/__init__.py
+-rw-r--r--   0        0        0    15647 2020-02-02 00:00:00.000000 pyventus-0.5.0/tests/handlers/test_event_handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyventus-0.5.0/tests/linkers/__init__.py
+-rw-r--r--   0        0        0    34169 2020-02-02 00:00:00.000000 pyventus-0.5.0/tests/linkers/test_event_linker.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 pyventus-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 pyventus-0.5.0/LICENSE
+-rw-r--r--   0        0        0    25045 2020-02-02 00:00:00.000000 pyventus-0.5.0/README.md
+-rw-r--r--   0        0        0     5773 2020-02-02 00:00:00.000000 pyventus-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    27655 2020-02-02 00:00:00.000000 pyventus-0.5.0/PKG-INFO
```

### Comparing `pyventus-0.4.1/CITATION.cff` & `pyventus-0.5.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `pyventus-0.4.1/src/pyventus/__init__.py` & `pyventus-0.5.0/src/pyventus/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,24 @@
-"""
-A modern and robust Python package for event-driven programming. Define, emit, and orchestrate events with ease using
-customizable event emitters and flexible responses.
-"""
+"""A powerful Python package for event-driven programming; define, emit, and orchestrate events with ease."""
 
-__version__ = "0.4.1"
+__version__ = "0.5.0"
 
 from .core.exceptions import PyventusException
 from .emitters import EventEmitter, EmittableEventType
 from .emitters.asyncio import AsyncIOEventEmitter
 from .emitters.executor import ExecutorEventEmitter
-from .events import Event
 from .handlers import EventHandler, EventCallbackType, SuccessCallbackType, FailureCallbackType
 from .linkers import EventLinker, SubscribableEventType
 
 __all__ = [
     "PyventusException",
     "EventEmitter",
     "EmittableEventType",
     "AsyncIOEventEmitter",
     "ExecutorEventEmitter",
-    "Event",
     "EventHandler",
     "EventCallbackType",
     "SuccessCallbackType",
     "FailureCallbackType",
     "EventLinker",
     "SubscribableEventType",
 ]
```

### Comparing `pyventus-0.4.1/src/pyventus/core/exceptions/pyventus_exception.py` & `pyventus-0.5.0/src/pyventus/core/exceptions/pyventus_exception.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from typing import List
 
 
 class PyventusException(Exception):
     """
-    Custom exception class for the Pyventus package.
+    A custom exception class for the Pyventus package that provides a robust mechanism for
+    handling and identifying potential exceptions within the package.
 
-    This class inherits from the base Exception class in Python, allowing it to be raised as an exception
-    when needed. It serves as a specific exception type for the Pyventus package, providing a way to handle
-    and identify exceptions that occur within the package.
+    **Notes:**
+
+    -   This class inherits from the base `Exception` class in Python, allowing it to be
+        raised as needed.
     """
 
     def __init__(self, errors: str | List[str] | None = None):
         """
-        Initializes a new `PyventusException` instance.
-        :param errors: The error messages associated with the exception. Defaults to None.
+        Initialize an instance of `PyventusException`.
+        :param errors: The error messages associated with the exception. Defaults to `None`.
         """
         self.errors: str | List[str] = errors if errors else self.__class__.__name__
         super().__init__(errors)
```

### Comparing `pyventus-0.4.1/src/pyventus/core/loggers/logger.py` & `pyventus-0.5.0/src/pyventus/core/loggers/logger.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,35 @@
 from .stdout_logger import StdOutLogger
 
 
 class Logger:
-    """
-    Logger is a custom logger class that wraps the logging module and provides additional functionality.
-
-    This class extends the functionality of the `StdOutLogger` class and adds additional attributes and methods for
-    logging and controlling log behavior. It allows for easy logging of messages, events, and errors, and provides
-    options to enable or disable debug mode and specify a custom name to be displayed with log messages.
-    """
+    """A custom logger class that wraps the `StdOutLogger` and provides additional functionality."""
 
     # Strict class attributes
     __slots__ = ("_name", "_debug")
 
     @property
     def debug_enabled(self) -> bool:
         """
         Returns a boolean value indicating whether debug mode is enabled.
         :return: `True` if debug mode is enabled, `False` otherwise.
         """
         return self._debug
 
     def __init__(self, name: str | None = None, debug: bool = False):
         """
-        Initializes a new logger instance.
+        Initializes an instance of `Logger`.
         :param name: The name of the logger instance.
         :param debug: A flag indicating whether debug mode is enabled.
         """
         self._name: str | None = name
-        """ The name of the logger. """
+        """The name of the logger."""
 
         self._debug = debug
-        """ A flag indicating whether or not debug mode is enabled. """
+        """A flag indicating whether or not debug mode is enabled."""
 
     def error(self, msg: str, action: str | None = None) -> None:
         """
         Logs an ERROR level message.
         :param msg: The message to be logged.
         :param action: The action or method associated with the log. Defaults to None.
         :return: None
```

### Comparing `pyventus-0.4.1/src/pyventus/core/loggers/stdout_logger.py` & `pyventus-0.5.0/src/pyventus/core/loggers/stdout_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,15 @@
 from logging import StreamHandler, INFO, DEBUG, WARNING, ERROR, Formatter, getLogger
 from sys import stdout
 
 from ...core.constants import StdOutColors
 
 
 class StdOutLogger(ABC):
-    """
-    StdOutLogger is a simple logging interface for logging operations to the standard output.
-
-    This class provides a straightforward logging interface for writing log messages to the standard output.
-    """
+    """A simple logging interface for writing log messages to the standard output."""
 
     class Handler:
         """Inner class representing a logger handler."""
 
         @classmethod
         def get_color_by_level(cls, level: int) -> str:
             """
```

### Comparing `pyventus-0.4.1/src/pyventus/emitters/event_emitter.py` & `pyventus-0.5.0/src/pyventus/emitters/event_emitter.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,57 +4,57 @@
 from sys import gettrace
 from typing import List, Type, TypeAlias, Any, Tuple, Dict, final
 from uuid import uuid4
 
 from ..core.constants import StdOutColors
 from ..core.exceptions import PyventusException
 from ..core.loggers import Logger, StdOutLogger
-from ..events import Event
 from ..handlers import EventHandler
 from ..linkers import EventLinker
 
-EmittableEventType: TypeAlias = Event | Exception | str
-""" A type alias representing the supported types of events that can be emitted. """
+EmittableEventType: TypeAlias = str | Exception | object
+"""A type alias representing the supported types of events that can be emitted."""
 
 
 class EventEmitter(ABC):
     """
     An abstract base class for event emitters.
 
-    This abstract base class defines a common interface for emitting events. It serves as
-    a foundation for  implementing custom event emitters with specific dispatch strategies.
-    It is designed to handle `string-named` events with variable-length argument list and
-    arbitrary keyword arguments, as well as instances of `Event` objects and `Exceptions`.
-
-    The main goal of this class is to decouple the dispatching of event handler callbacks
-    from the underlying implementation. This loose coupling promotes flexibility and
-    adaptability through separation of concerns, allowing custom event emitters to
-    be implemented without affecting existing consumers.
+    **Notes:**
 
-    For more information and code examples, please refer to the `EventEmitter` tutorials
-    at: [https://mdapena.github.io/pyventus/tutorials/emitters/](https://mdapena.github.io/pyventus/tutorials/emitters/).
+    -   This class defines a common interface for emitting events. It serves as a foundation for
+        implementing custom event emitters with specific dispatch strategies. It is designed to
+        handle `string-named` events with positional and keyword arguments, as well as instances
+        of `dataclass` objects and `Exceptions` objects.
+
+    -   The main goal of this class is to decouple the event emission process from the underlying
+        implementation. This loose coupling promotes flexibility, adaptability, and adheres to the
+        Open-Closed principle, allowing custom event emitters to be implemented without affecting
+        existing consumers.
+
+    ---
+    Read more in the
+    [Pyventus docs for Event Emitter](https://mdapena.github.io/pyventus/tutorials/emitters/).
     """
 
     @final
     class EventEmission:
         """
         Represents an event emission that has been triggered but whose propagation is not
         yet complete. It provides a self-contained context for executing the event emission,
         encapsulating both the event data and the associated event handlers.
 
         This class acts as an isolated unit of work to asynchronously propagate the emission
-        of an event.
-
-        This class is managed by the `EventEmitter` class, which creates an instance when an
-        event is emitted. This instance is then processed by the EventEmitter's `_process()`
-        method.
+        of an event. When an event occurs, the `EventEmitter` class creates an `EventEmission`
+        instance, which is then processed by the `_process()` method to handle the event
+        propagation.
         """
 
         # Event emission attributes
-        __slots__ = ("_id", "_timestamp", "_debug", "_event", "_event_handlers", "_args", "_kwargs")
+        __slots__ = ("_id", "_timestamp", "_debug", "_event", "_event_handlers", "_event_args", "_event_kwargs")
 
         @property
         def id(self) -> str:
             """
             Gets the unique identifier of the event emission.
             :return: The unique identifier of the event emission.
             """
@@ -72,202 +72,184 @@
         def event(self) -> str:
             """
             Gets the name of the event being emitted.
             :return: The name of the event.
             """
             return self._event
 
-        def __init__(self, debug: bool, event: str, event_handlers: List[EventHandler], /, *args: Any, **kwargs: Any):
+        def __init__(
+            self,
+            event: str,
+            event_handlers: List[EventHandler],
+            event_args: Tuple[Any, ...],
+            event_kwargs: Dict[str, Any],
+            debug: bool,
+        ) -> None:
             """
-            Initialize the `EventEmission` object.
-            :param debug: Indicates if debug mode is enabled.
+            Initialize an instance of `EventEmission`.
             :param event: The name of the event being emitted.
             :param event_handlers: List of event handlers associated with the event.
-            :param args: Positional arguments to be passed to the event handlers.
-            :param kwargs: Keyword arguments to be passed to the event handlers.
+            :param event_args: Positional arguments to be passed to the event handlers.
+            :param event_kwargs: Keyword arguments to be passed to the event handlers.
+            :param debug: Indicates if debug mode is enabled.
             :raises PyventusException: If `event_handlers` or `event` is empty.
             """
             if not event_handlers:  # pragma: no cover
                 raise PyventusException("The 'event_handlers' argument cannot be empty.")
 
             if not event:  # pragma: no cover
                 raise PyventusException("The 'event' argument cannot be empty.")
 
+            # Set the event emission metadata
             self._id: str = str(uuid4())
-            """The unique identifier for the event emission."""
-
             self._timestamp: datetime = datetime.now()
-            """The timestamp when the event emission was created."""
-
             self._debug: bool = debug
-            """A flag indicating whether or not debug mode is enabled."""
 
+            # Set the event emission properties
             self._event: str = event
-            """The name of the event being emitted."""
-
             self._event_handlers: Tuple[EventHandler, ...] = tuple(event_handlers)
-            """Tuple of event handlers associated with the event."""
-
-            self._args: Tuple[Any, ...] = args
-            """Positional arguments to be passed to the event handlers."""
-
-            self._kwargs: Dict[str, Any] = kwargs
-            """Keyword arguments to be passed to the event handlers."""
+            self._event_args: Tuple[Any, ...] = event_args
+            self._event_kwargs: Dict[str, Any] = event_kwargs
 
         async def __call__(self) -> None:
             """
             Execute the event handlers concurrently.
             :return: None
             """
             # Log the event execution if debug is enabled
             if self._debug:  # pragma: no cover
                 StdOutLogger.debug(name=self.__class__.__name__, action="Running:", msg=str(self))
 
             # Execute the event handlers concurrently
             await gather(
-                *[event_handler(*self._args, **self._kwargs) for event_handler in self._event_handlers],
+                *[event_handler(*self._event_args, **self._event_kwargs) for event_handler in self._event_handlers],
                 return_exceptions=True,
             )
 
         def __str__(self) -> str:
             """
-            Gets a string representation of the EventEmission object.
-            :return: String representation of the object.
+            Returns a formatted string representation of the event emission.
+            :return: The formatted string representation of the event emission.
             """
             return (
                 f"ID: {self.id} | Timestamp: {self.timestamp.strftime('%Y-%m-%d %I:%M:%S %p')} | "
                 f"Event: {self.event} | Handlers: {len(self._event_handlers)}"
             )
 
-    def __init__(self, event_linker: Type[EventLinker] = EventLinker, debug: bool | None = None):
+    def __init__(self, event_linker: Type[EventLinker] = EventLinker, debug: bool | None = None) -> None:
         """
-        Initializes an instance of the `EventEmitter`.
-        :param event_linker: Specifies the type of event linker to use for associating
-            events with their respective event handlers. Defaults to `EventLinker`.
+        Initialize an instance of `EventEmitter`.
+        :param event_linker: Specifies the type of event linker used to manage and access
+            events along with their corresponding event handlers. Defaults to `EventLinker`.
         :param debug: Specifies the debug mode for the subclass logger. If `None`,
             it is determined based on the execution environment.
         :raises PyventusException: If the `event_linker` argument is None.
         """
         # Validate the event linker argument
         if event_linker is None:
             raise PyventusException("The 'event_linker' argument cannot be None.")
+        if not issubclass(event_linker, EventLinker):
+            raise PyventusException("The 'event_linker' argument must be a subtype of the EventLinker class.")
 
         # Set the event_linker value
         self._event_linker: Type[EventLinker] = event_linker
         """
-        The `EventLinker` attribute specifies the type of event linker to 
-        use for associating events with their respective event handlers.
+        Specifies the type of event linker to use for associating events with their 
+        respective event handlers.
         """
 
         self._logger: Logger = Logger(
             name=self.__class__.__name__,
             debug=debug if debug is not None else bool(gettrace() is not None),
         )
         """
-        An instance of the logger used for logging events and debugging information. The 
-        debug mode of the logger can be explicitly set by providing a boolean value for the 
-        `debug` argument in the constructor. If `debug` is set to `None`, the debug will be
-        automatically determined based on the execution environment and the value returned
-        by the `gettrace()` function.
+        An instance of the logger used for logging events and debugging information.
         """
 
     def emit(self, /, event: EmittableEventType, *args: Any, **kwargs: Any) -> None:
         """
-        Emits an event and triggers any associated event handlers. When emitting `Event` or
-        `Exception` objects, they are automatically passed to the event handler as the
-        first positional argument, even if you pass `*args` or `**kwargs`.
-
-        **Note:** If there are event handlers subscribed to the emission of any `Event` or
-        `Exception`, they will also be executed.
-
-        :param event: The event to emit. It can be an instance of `Event`, `Exception`,
-            or a simple `str`.
-        :param args: Additional positional arguments to pass to the event handlers.
-        :param kwargs: Additional keyword arguments to pass to the event handlers.
+        Emits an event and triggers its associated event handlers.
+
+        **Notes:**
+
+        -   When emitting `dataclass` objects or `Exception` objects, they are automatically passed
+            to the event handler as the first positional argument, even if you pass additional `*args`
+            or `**kwargs`.
+        -   If there are event handlers subscribed to the global event `...`, also known as `Ellipsis`,
+            they will also be triggered each time an event or exception is emitted.
+
+        :param event: The event to be emitted. It can be `str`, a `dataclass`
+            object, or an `Exception` object.
+        :param args: Positional arguments to be passed to the event handlers.
+        :param kwargs: Keyword arguments to be passed to the event handlers.
         :return: None
         """
-        # Raises an exception if the event is None
+        # Raise an exception if the event is None
         if event is None:
             raise PyventusException("The 'event' argument cannot be None.")
 
-        # Raises an exception if the event is a type object
-        if event.__class__ is type:  # type: ignore[comparison-overlap]
+        # Raise an exception if the event is a type
+        if isinstance(event, type):
             raise PyventusException("The 'event' argument cannot be a type.")
 
-        # Determines if the event is a string instance
-        is_string: bool = isinstance(event, str)
+        # Determine the event name
+        event_name: str = self._event_linker.get_event_name(event=event if isinstance(event, str) else type(event))
 
-        # Raises an exception if the event is a string and it is empty
-        if is_string and len(event) == 0:  # type: ignore[arg-type]
-            raise PyventusException("The 'event' argument cannot be an empty string.")
-
-        # Constructs the arguments tuple based on whether the event is a string or an object
-        event_args: Tuple[Any, ...] = args if is_string else (event, *args)
-
-        # Retrieves the event handlers associated with the event sorted by their timestamp
-        event_handlers: List[EventHandler] = sorted(
-            self._event_linker.get_handlers_by_events(
-                event if is_string else event.__class__,  # type: ignore[arg-type]
-                Event if not issubclass(event.__class__, Exception) else Exception,
-            ),
-            key=lambda handler: handler.timestamp,
-        )
+        # Retrieve the event handlers associated with the event
+        event_handlers: List[EventHandler] = self._event_linker.get_event_handlers_by_events(event_name, Ellipsis)
 
-        # Initializes the list of event handlers to be executed
+        # Sort the event handlers by timestamp
+        event_handlers.sort(key=lambda handler: handler.timestamp)
+
+        # Initialize the list of event handlers to be executed
         pending_event_handlers: List[EventHandler] = []
 
-        # Iterates through each event handler and triggers the associated callbacks
+        # Iterate through each event handler
         for event_handler in event_handlers:
-            # Checks if the event handler is a one-time handler before executing the event handler
+            # Check if the event handler is a one-time subscription
             if event_handler.once:
-                # If the event handler is a one-time handler, we try to remove it. If it is successfully
-                # removed, it means it hasn't been executed before, so we execute the callback
+                # If the event handler is a one-time subscription, we attempt to remove it.
                 if self._event_linker.remove_event_handler(event_handler=event_handler):  # pragma: no cover (Race-Cond)
-                    # Adds the current event handler to the execution list
+                    # If the removal is successful, it indicates that the handler has not
+                    # been processed before, so we add it to the pending list.
                     pending_event_handlers.append(event_handler)
             else:
-                # Adds the current event handler to the execution list
                 pending_event_handlers.append(event_handler)
 
-        # Determine the event name
-        event_name: str = str(event if is_string else event.__class__.__name__)
-
-        # Checks if the pending_event_handlers is not empty
+        # Check if the pending list of event handlers is not empty
         if len(pending_event_handlers) > 0:
-            # Creates a new EventEmission instance
+            # Create a new EventEmission instance
             event_emission: EventEmitter.EventEmission = EventEmitter.EventEmission(
-                self._logger.debug_enabled,
-                event_name,
-                pending_event_handlers,
-                *event_args,
-                **kwargs,
+                event=event_name,
+                event_handlers=pending_event_handlers,
+                event_args=args if isinstance(event, str) else (event, *args),
+                event_kwargs=kwargs,
+                debug=self._logger.debug_enabled,
             )
 
-            # Logs the event emission when debug is enabled
+            # Log the event emission when debug is enabled
             if self._logger.debug_enabled:  # pragma: no cover
                 self._logger.debug(
                     action="Emitting Event:",
                     msg=f"{event_emission.event}{StdOutColors.PURPLE} ID:{StdOutColors.DEFAULT} {event_emission.id}",
                 )
 
-            # Delegates the processing of the event emission to subclasses
+            # Delegate the event emission processing to subclasses
             self._process(event_emission)
 
-        # Logs a debug message if no event handlers are subscribed to the event
+        # Log a debug message if there are no event handlers subscribed to the event
         elif self._logger.debug_enabled:  # pragma: no cover
             self._logger.debug(
                 action="Emitting Event:",
                 msg=f"{event_name}{StdOutColors.PURPLE} Message:{StdOutColors.DEFAULT} No event handlers subscribed",
             )
 
     @abstractmethod
     def _process(self, event_emission: EventEmission) -> None:
         """
-        Processes the execution of the event emission.
-
-        **Note:** Subclasses must implement this method to define the specific
-        processing logic for the event emission.
+        Process the event emission execution. Subclasses must implement
+        this method to define the specific processing logic.
 
         :param event_emission: The event emission to be processed.
         :return: None
         """
         pass
```

### Comparing `pyventus-0.4.1/src/pyventus/emitters/asyncio/asyncio_event_emitter.py` & `pyventus-0.5.0/src/pyventus/emitters/asyncio/asyncio_event_emitter.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,66 +4,62 @@
 
 from ..event_emitter import EventEmitter
 from ...linkers import EventLinker
 
 
 class AsyncIOEventEmitter(EventEmitter):
     """
-    A class that inherits from `EventEmitter` and uses the `AsyncIO` framework to handle
-    the execution of the event handlers.
+    An event emitter subclass that utilizes the AsyncIO framework to handle
+    the execution of event emissions.
 
-    **Asynchronous Execution**: In an asynchronous context where an event loop is already
-    running, the event emission is scheduled and processed on that existing loop. If the
-    event loop is closed before all callbacks complete, any remaining scheduled callback
-    will be canceled.
-
-    **Synchronous Execution**: In a synchronous context where no event loop is active, a new event
-    loop is started and subsequently closed by the `asyncio.run()` method. Within this loop, it
-    executes the event emission. The loop then waits for all scheduled tasks to finish before
-    closing. This preserves synchronous execution while still gaining the benefits of the
-    concurrent execution.
+    **Notes:**
 
-    For more information and code examples, please refer to the `AsyncIOEventEmitter`
-    tutorials at: [https://mdapena.github.io/pyventus/tutorials/emitters/asyncio/](https://mdapena.github.io/pyventus/tutorials/emitters/asyncio/).
+    -   When used in an asynchronous context where an event loop is already running,
+        the event emission is scheduled and processed on that existing loop. If the
+        event loop is closed before all callbacks complete, any remaining scheduled
+        callbacks will be canceled.
+
+    -   When used in a synchronous context where no event loop is active, a new event
+        loop is started and subsequently closed by the `asyncio.run()` method. Within
+        this loop, the event emission is executed. The loop then waits for all
+        scheduled tasks to finish before closing.
+
+    ---
+    Read more in the
+    [Pyventus docs for AsyncIO Event Emitter](https://mdapena.github.io/pyventus/tutorials/emitters/asyncio/).
     """
 
     @property
     def __is_loop_running(self) -> bool:
         """
-        Check if an asyncio event loop is currently running.
-
-        This method checks if there is a current asyncio event loop running by calling
-        `asyncio.get_running_loop()`.If no exception is raised, it means there is a
-        running loop and `True` is returned. If a `RuntimeError` is  raised, it
-        means there is no running loop and `False` is returned.
-
-        :return: `True` if there is a current running event loop, `False` otherwise
+        Check if there is currently an active AsyncIO event loop.
+        :return: `True` if an event loop is running, `False` otherwise.
         """
         try:
             asyncio.get_running_loop()
             return True
         except RuntimeError:
             return False
 
-    def __init__(self, event_linker: Type[EventLinker] = EventLinker, debug: bool | None = None):
+    def __init__(self, event_linker: Type[EventLinker] = EventLinker, debug: bool | None = None) -> None:
         """
-        Initializes an instance of the `AsyncIOEventEmitter` class.
-        :param event_linker: Specifies the type of event linker to use for associating
-            events with their respective event handlers. Defaults to `EventLinker`.
+        Initialize an instance of `AsyncIOEventEmitter`.
+        :param event_linker: Specifies the type of event linker used to manage and access
+            events along with their corresponding event handlers. Defaults to `EventLinker`.
         :param debug: Specifies the debug mode for the logger. If `None`, it is
             determined based on the execution environment.
         """
-        # Call the parent class' __init__ method to set up the event linker
+        # Call the parent class' __init__ method
         super().__init__(event_linker=event_linker, debug=debug)
 
         # Initialize the set of background futures
         self._background_futures: Set[Future] = set()  # type: ignore[type-arg]
 
     def _process(self, event_emission: EventEmitter.EventEmission) -> None:
-        # Check if AsyncIO event loop is running
+        # Check if there is an active event loop
         is_loop_running: bool = self.__is_loop_running
 
         # Log the execution context, if debug mode is enabled
         if self._logger.debug_enabled:  # pragma: no cover
             self._logger.debug(action=f"Context:", msg=f"{'Async' if is_loop_running else 'Sync'}")
 
         if is_loop_running:
@@ -72,9 +68,9 @@
 
             # Remove the Future from the set of background futures after completion
             future.add_done_callback(self._background_futures.remove)
 
             # Add the Future to the set of background futures
             self._background_futures.add(future)
         else:
-            # Run the event emission in a synchronous manner
+            # Run the event emission in a blocking manner
             asyncio.run(event_emission())
```

### Comparing `pyventus-0.4.1/src/pyventus/emitters/celery/celery_event_emitter.py` & `pyventus-0.5.0/src/pyventus/emitters/celery/celery_event_emitter.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,38 +16,38 @@
         "Optional dependency 'celery' not found."
         "\nPlease install it using 'pip install pyventus[celery]' to use this event emitter."
     )
 
 
 class CeleryEventEmitter(EventEmitter):
     """
-    A class that enables event handling using the powerful Celery distributed task queue system.
+    An event emitter subclass that utilizes the Celery distributed system
+    to handle the execution of event emissions.
 
-    This class extends the base `EventEmitter` class and provides the functionality to enqueue and
-    event handlers using `Celery`. Once enqueued, these event handlers are processed asynchronously
-    by `Celery` workers. The `CeleryEventEmitter` is particularly useful when dealing with events
-    that require resource-intensive tasks.
+    **Notes:**
 
-    The `CeleryEventEmitter` works by utilizing the provided `Queue` instance to enqueue the event
-    emissions for asynchronous processing.
-
-    For more information and code examples, please refer to the `CeleryEventEmitter` tutorials at:
-    [https://mdapena.github.io/pyventus/tutorials/emitters/celery/](https://mdapena.github.io/pyventus/tutorials/emitters/celery/).
+    -   This class uses a Celery Queue instance to enqueue event emissions, which are
+        subsequently executed by Celery workers. This approach provides a scalable
+        and distributed method for handling the execution of event emissions.
+
+    ---
+    Read more in the
+    [Pyventus docs for Celery Event Emitter](https://mdapena.github.io/pyventus/tutorials/emitters/celery/).
     """
 
     class Queue:
-        """A class representing the Celery task queue used for enqueuing event emissions."""
+        """A Celery event emitter queue used for enqueuing event emissions."""
 
         class Serializer:
-            """`EventEmission` Serializer for Celery Tasks"""
+            """An event emitter object serializer for Celery queues."""
 
             @staticmethod
             def dumps(obj: EventEmitter.EventEmission) -> Any:
                 """
-                Serializes the event emission object
+                Serializes the event emission object.
                 :param obj: The event emission object to be serialized.
                 :return: The serialized representation of the event emission object.
                 """
                 return dumps(obj)  # pragma: no cover
 
             @staticmethod
             def loads(serialized_obj: Any) -> EventEmitter.EventEmission:
@@ -55,112 +55,106 @@
                 Deserializes the task payload back to the event emission object.
                 :param serialized_obj: The serialized object to be loaded.
                 :return: The deserialized event emission object.
                 """
                 return cast(EventEmitter.EventEmission, loads(serialized_obj))  # pragma: no cover
 
         class _Payload(NamedTuple):
-            """Represents the payload data sent to Celery."""
+            """The Celery event emitter queue payload."""
 
             serialized_obj: bytes
-            """The serialized event emission object."""
+            """Serialized event emission object."""
 
             obj_hash: bytes | None
-            """The hash of the serialized event emission object."""
-
-            def to_json(self) -> Dict[str, Any]:
-                """
-                Converts the payload to a JSON-compatible dictionary.
-                :return: JSON-compatible dictionary representing the payload.
-                """
-                return self._asdict()
+            """Hash of the serialized event emission object."""
 
             @classmethod
             def from_json(cls, **kwargs: Any) -> "CeleryEventEmitter.Queue._Payload":
                 """
                 Creates a Payload instance from a JSON-compatible dictionary.
                 :param kwargs: JSON-compatible dictionary representing the payload.
                 :return: Payload instance.
                 :raises ValueError: If the JSON data is missing fields or contains extra keys.
                 """
                 # Get the field names of the named tuple
                 tuple_fields: tuple[str, ...] = CeleryEventEmitter.Queue._Payload._fields
 
-                # Check if all the fields are present in the JSON data
+                # Check if all expected fields are present
                 if not set(tuple_fields).issubset(kwargs.keys()):
                     raise PyventusException("Missing fields in JSON data.")
 
                 # Check for extra keys in the JSON data
                 extra_keys = set(kwargs.keys()) - set(tuple_fields)
                 if extra_keys:
                     raise PyventusException("Extra keys in JSON data: {}".format(extra_keys))
 
                 # Create the named tuple using the JSON data
                 return cls(**kwargs)
 
+            def to_json(self) -> Dict[str, Any]:
+                """
+                Converts the payload to a JSON-compatible dictionary.
+                :return: JSON-compatible dictionary representing the payload.
+                """
+                return self._asdict()
+
         def __init__(
             self,
             celery: Celery,
             name: str | None = None,
             secret: str | None = None,
             serializer: Type[Serializer] = Serializer,
-        ):
+        ) -> None:
             """
-            Initialize the Celery event emitter `Queue`.
-            :param celery: The Celery instance used to enqueue and process event emissions.
+            Initialize an instance of `CeleryEventEmitter.Queue`.
+            :param celery: The Celery object used to enqueue and process event emissions.
             :param name: The name of the queue where the event emission will be enqueued.
                 Default is None (task_default_queue).
             :param secret: The secret key used for message authentication and integrity validation.
                 This key is used for hashing the event emission object and verifying its integrity.
             :param serializer: The serializer class used for serializing and deserializing event
                 emission objects.
-            :raises PyventusException: If the Celery instance is None, or the secret key is not None
+            :raises PyventusException: If the Celery object is None, or the secret key is not None
                 and empty, or if the content type 'application/x-python-serialize' is not accepted.
             """
             if celery is None:
                 raise PyventusException("The 'celery' argument cannot be None.")
+            if not isinstance(celery, Celery):
+                raise PyventusException("The 'celery' argument must be an instance of the Celery class.")
 
             if secret is not None and len(secret) == 0:
                 raise PyventusException("The 'secret' argument cannot be empty.")
 
             if "application/x-python-serialize" not in celery.conf.accept_content:
                 raise PyventusException(
                     "Unsupported content type. "
                     "'application/x-python-serialize' is not in the list of accepted content types."
                 )
 
+            # Set the Celery queue properties
             self._celery: Celery = celery
-            """The Celery instance."""
-
             self._name: str = self._celery.conf.task_default_queue if name is None else name
-            """The name of the queue where the event emission will be enqueued."""
-
             self._secret: bytes | None = secret.encode("utf-8") if secret else None
-            """The secret key used for message authentication and integrity validation, encoded as bytes."""
-
-            self._digestmod: str | Callable[[], Any] | ModuleType = sha256
-            """The digest algorithm used for hashing."""
-
+            self._digestmod: str | Callable[[], Any] | ModuleType = sha256  # The digest algorithm used for hashing
             self._serializer: Type[CeleryEventEmitter.Queue.Serializer] = serializer
-            """The serializer class used for serializing and deserializing event emission objects."""
 
-            # Registers the event processor method as a Celery task.
-            self._celery.task(self._executor, name=self._executor.__name__, queue=self._name)
+            # Register the event processor method as a Celery task
+            self._celery.task(self._executor, name=f"pyventus{self._executor.__name__}", queue=self._name)
 
         def enqueue(self, event_emission: EventEmitter.EventEmission) -> None:
             """
             Enqueues an event emission object for asynchronous processing in Celery.
 
             This method takes an `EventEmission` object and enqueues it for asynchronous
             execution by Celery workers. If a secret key is provided during initialization,
             the event emission object is first serialized, and its hash is calculated using
             the secret key. This hash is used to verify the integrity of the event emission
-            object during processing.
+            object during execution.
 
-            :param event_emission: The event emission object to be queued for processing.
+            :param event_emission: The event emission object to be enqueued for asynchronous execution.
             :return: None
             """
             # Serialize the event emission object
             serialized_obj: Any = self._serializer.dumps(event_emission)
 
             # Calculate the hash of the serialized object if a secret key was provided
             obj_hash: Any | None = None
@@ -169,32 +163,32 @@
 
             # Create a payload with the serialized event emission instance and its hash
             payload = CeleryEventEmitter.Queue._Payload(
                 serialized_obj=serialized_obj,
                 obj_hash=obj_hash,
             )
 
-            # Send the event emission to Celery for execution
+            # Send the event emission object to Celery for asynchronous execution
             self._celery.send_task(
-                self._executor.__name__,
+                f"pyventus{self._executor.__name__}",
                 kwargs=payload.to_json(),
                 queue=self._name,
             )
 
         def _executor(self, **kwargs: Any) -> None:
             """
-            Processes the enqueued event emission object.
+            Process the enqueued event emission object.
 
-            This method is the actual Celery task that processes the enqueued event emission.
-            It deserializes the event emission object and verifies its integrity.
+            This method serves as the Celery task responsible
+            for processing the enqueued event emission.
 
             :param kwargs: The JSON-compatible dictionary representing the payload.
             :return: None
             """
-            # Create a Payload instance from the payload JSON data
+            # Create a Payload instance from the JSON data
             payload = CeleryEventEmitter.Queue._Payload.from_json(**kwargs)
 
             # Check payload
             if self._secret:  # pragma: no cover
                 if not payload.obj_hash:
                     raise PyventusException("Invalid payload structure.")
 
@@ -215,30 +209,31 @@
             # Check if the deserialized event emission object is valid
             if event_emission is None:  # pragma: no cover
                 raise PyventusException("Failed to deserialize the event emission object.")
 
             # Run the event emission
             asyncio.run(event_emission())
 
-    def __init__(self, queue: Queue, event_linker: Type[EventLinker] = EventLinker, debug: bool | None = None):
+    def __init__(self, queue: Queue, event_linker: Type[EventLinker] = EventLinker, debug: bool | None = None) -> None:
         """
-        Initializes an instance of the `CeleryEventEmitter` class.
-        :param queue: The celery event task executor used to process the event task.
-        :param event_linker: Specifies the type of event linker to use for associating
-            events with their respective event handlers. Defaults to `EventLinker`.
+        Initialize an instance of `CeleryEventEmitter`.
+        :param queue: The queue used for enqueuing event emissions in the Celery event emitter.
+        :param event_linker: Specifies the type of event linker used to manage and access
+            events along with their corresponding event handlers. Defaults to `EventLinker`.
         :param debug: Specifies the debug mode for the logger. If `None`, it is
             determined based on the execution environment.
         """
-        # Call the parent class' __init__ method to set up the event linker
+        # Call the parent class' __init__ method
         super().__init__(event_linker=event_linker, debug=debug)
 
-        # Validate the executor argument
+        # Validate the queue argument
         if queue is None:
             raise PyventusException("The 'queue' argument cannot be None")
+        if not isinstance(queue, CeleryEventEmitter.Queue):
+            raise PyventusException("The 'queue' argument must be an instance of the CeleryEventEmitter.Queue class.")
 
-        # Store the queue instance
+        # Store the queue object
         self._queue: CeleryEventEmitter.Queue = queue
-        """The Queue instance used to process the event emission."""
 
     def _process(self, event_emission: EventEmitter.EventEmission) -> None:
-        # Add the event emission to the Celery Queue
+        # Add the event emission object to the Celery queue for asynchronous execution
         self._queue.enqueue(event_emission=event_emission)
```

### Comparing `pyventus-0.4.1/src/pyventus/emitters/executor/executor_event_emitter.py` & `pyventus-0.5.0/src/pyventus/emitters/executor/executor_event_emitter.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,96 +6,93 @@
 from ..event_emitter import EventEmitter
 from ...core.exceptions import PyventusException
 from ...linkers import EventLinker
 
 
 class ExecutorEventEmitter(EventEmitter):
     """
-    An event emitter that executes event handlers using an `Executor`.
-
-    This class utilizes the `concurrent.futures` Executor base class to handle asynchronous
-    execution of event emissions. It can work with either `ThreadPoolExecutor` for thread-based
-    execution or `ProcessPoolExecutor` for process-based execution.
-
-    By inheriting from `EventEmitter` and utilizing the `Executor` interface, this class
-    provides a consistent way to emit events and execute handlers asynchronously in either
-    threads or processes. This allows choosing the optimal execution approach based on
-    application needs.
-
-    **Note:** It is important to properly manage the underlying `Executor` when using
-    this event emitter. Once finished emitting events, call the `shutdown()` method to
-    signal the executor to free any resources for pending futures.
-
-    - You can avoid having to call this method explicitly if you use the `with` statement,
-      which will shut down the `Executor` (waiting as if `Executor.shutdown()` were called
-      with `wait` set to `True`).
-
-    For more information and code examples, please refer to the `ExecutorEventEmitter`
-    tutorials at: [https://mdapena.github.io/pyventus/tutorials/emitters/executor/](https://mdapena.github.io/pyventus/tutorials/emitters/executor/).
+    An event emitter subclass that utilizes the `concurrent.futures` Executor base class to
+    handle the execution of event emissions. It can work with either `ThreadPoolExecutor`
+    for thread-based execution or `ProcessPoolExecutor` for process-based execution.
+
+    **Notes:**
+
+    -   When using this event emitter, it is important to properly manage the underlying `Executor`.
+        Once you have finished emitting events, call the `shutdown()` method to signal the executor to
+        free any resources for pending futures. You can avoid the need to call this method explicitly
+        by using the `with` statement, which will automatically shut down the `Executor` (waiting as
+        if `Executor.shutdown()` were called with `wait` set to `True`).
+
+    ---
+    Read more in the
+    [Pyventus docs for Executor Event Emitter](https://mdapena.github.io/pyventus/tutorials/emitters/executor/).
     """
 
+    @staticmethod
+    def _callback(event_emission: EventEmitter.EventEmission) -> None:
+        """
+        This method is used as the callback function for the executor
+        to process the event emission.
+        :param event_emission: The event emission to be executed.
+        :return: None
+        """
+        asyncio.run(event_emission())
+
     def __init__(
         self,
         executor: Executor = ThreadPoolExecutor(),
         event_linker: Type[EventLinker] = EventLinker,
         debug: bool | None = None,
-    ):
+    ) -> None:
         """
-        Initializes an instance of the `ExecutorEventEmitter` class.
-        :param executor: The executor object used for executing event handlers. Defaults
-            to `ThreadPoolExecutor()`.
-        :param event_linker: Specifies the type of event linker to use for associating
-            events with their respective event handlers. Defaults to `EventLinker`.
+        Initialize an instance of `ExecutorEventEmitter`.
+        :param executor: The executor object used to handle the execution of event
+            emissions. Defaults to `ThreadPoolExecutor()`.
+        :param event_linker: Specifies the type of event linker used to manage and access
+            events along with their corresponding event handlers. Defaults to `EventLinker`.
         :param debug: Specifies the debug mode for the logger. If `None`, it is
             determined based on the execution environment.
         """
-        # Call the parent class' __init__ method to set up the event linker
+        # Call the parent class' __init__ method
         super().__init__(event_linker=event_linker, debug=debug)
 
         # Validate the executor argument
-        if executor is None or not issubclass(executor.__class__, Executor):
-            raise PyventusException("The 'executor' argument must be a valid executor.")
+        if executor is None:
+            raise PyventusException("The 'executor' argument cannot be None.")
+        if not isinstance(executor, Executor):
+            raise PyventusException("The 'executor' argument must be an instance of the Executor class.")
 
         # Set the executor object reference
         self._executor: Executor = executor
 
     def __enter__(self) -> "ExecutorEventEmitter":
         """
-        Returns the instance of `ExecutorEventEmitter` for context management.
-        :return: The instance of `ExecutorEventEmitter`.
+        Returns the current instance of `ExecutorEventEmitter` for context management.
+        :return: The current instance of `ExecutorEventEmitter`.
         """
         return self
 
     def __exit__(
         self, exc_type: Type[BaseException] | None, exc_val: BaseException | None, exc_tb: TracebackType | None
     ) -> None:
         """
         Cleans up the executor resources when exiting the context.
         :param exc_type: The exception type, if any.
         :param exc_val: The exception value, if any.
         :param exc_tb: The traceback information, if any.
-        :return: A boolean indicating whether to propagate any exception or not.
+        :return: None
         """
         self.shutdown(wait=True)
 
     def shutdown(self, wait: bool = True, cancel_futures: bool = False) -> None:
         """
         Shuts down the executor and frees any resources it is using.
         :param wait: A boolean indicating whether to wait for the currently pending futures
             to complete before shutting down.
         :param cancel_futures: A boolean indicating whether to cancel any pending futures.
         :return: None
         """
         self._executor.shutdown(wait=wait, cancel_futures=cancel_futures)
 
     def _process(self, event_emission: EventEmitter.EventEmission) -> None:
-        # Submit the event emission to the execution callback
-        self._executor.submit(ExecutorEventEmitter._execution_callback, event_emission)
-
-    @staticmethod
-    def _execution_callback(event_emission: EventEmitter.EventEmission) -> None:
-        """
-        This method serves as a callback to be passed to the executor.
-        :param event_emission: The event emission to be executed.
-        :return: None
-        """
-        asyncio.run(event_emission())
+        # Submit the event emission to the executor
+        self._executor.submit(ExecutorEventEmitter._callback, event_emission)
```

### Comparing `pyventus-0.4.1/src/pyventus/emitters/fastapi/fastapi_event_emitter.py` & `pyventus-0.5.0/src/pyventus/emitters/fastapi/fastapi_event_emitter.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,73 +11,79 @@
         "Optional dependency 'fastapi' not found."
         "\nPlease install it using 'pip install pyventus[fastapi]' to use this event emitter."
     )
 
 
 class FastAPIEventEmitter(EventEmitter):
     """
-    A class that enables event handling in [FastAPI](https://fastapi.tiangolo.com/) using its powerful
-    [BackgroundTasks](https://fastapi.tiangolo.com/reference/background/) system.
+    An event emitter subclass that utilizes FastAPI's BackgroundTasks system
+    to handle the execution of event emissions.
 
-    This class extends the base `EventEmitter` class and leverages the FastAPI's BackgroundTasks feature to
-    process event emissions asynchronously. It provides a convenient way to incorporate event-driven
-    functionality into FastAPI applications.
-
-    This class provides a powerful mechanism for implementing asynchronous and decoupled operations,
-    such as asynchronously sending emails in an event-driven manner. It opens up possibilities for
-    building scalable and responsive FastAPI applications.
+    **Notes:**
 
-    For more information and code examples, please refer to the `FastAPIEventEmitter` tutorials at:
-    [https://mdapena.github.io/pyventus/tutorials/emitters/fastapi/](https://mdapena.github.io/pyventus/tutorials/emitters/fastapi/).
+    -   It provides a convenient way to incorporate event-driven functionality
+        into FastAPI apps.
+    -   This class offers a powerful mechanism for implementing asynchronous
+        and decoupled operations in FastAPI, such as asynchronously sending
+        emails in an event-driven manner.
+
+    ---
+    Read more in the
+    [Pyventus docs for FastAPI Event Emitter](https://mdapena.github.io/pyventus/tutorials/emitters/fastapi/).
     """
 
     @classmethod
     def options(
         cls, event_linker: Type[EventLinker] = EventLinker, debug: bool | None = None
     ) -> Callable[[BackgroundTasks], "FastAPIEventEmitter"]:
         """
-        Returns a decorator that allows configuring the `FastAPIEventEmitter` class when
-        using the `Depends` method of `FastAPI`.
-        :param event_linker: Specifies the type of event linker to use for associating
-            events with their respective event handlers. Defaults to `EventLinker`.
+        Returns a decorator that allows you to configure the `FastAPIEventEmitter` class
+        when using FastAPI's `Depends` method.
+        :param event_linker: Specifies the type of event linker used to manage and access
+            events along with their corresponding event handlers. Defaults to `EventLinker`.
         :param debug: Specifies the debug mode for the logger. If `None`, it is
             determined based on the execution environment.
         :return: A decorator that can be used with the `Depends` method.
         """
 
         def wrapper(background_tasks: BackgroundTasks) -> "FastAPIEventEmitter":
             """
-            Decorator wrapper function that configures the `FastAPIEventEmitter` class with the provided options.
-            :param background_tasks: The FastAPI `BackgroundTasks` object used to process event emissions.
+            A decorator wrapper function that configures the `FastAPIEventEmitter` class with
+            the provided options.
+            :param background_tasks: The FastAPI `BackgroundTasks` object used to handle
+                the execution of event emissions.
             :return: An instance of `FastAPIEventEmitter` configured with the specified options.
             """
             return cls(background_tasks=background_tasks, event_linker=event_linker, debug=debug)
 
         return wrapper
 
     def __init__(
         self,
         background_tasks: BackgroundTasks,
         event_linker: Type[EventLinker] = EventLinker,
         debug: bool | None = None,
-    ):
+    ) -> None:
         """
-        Initializes the `FastAPIEventEmitter`.
-        :param background_tasks: The FastAPI `BackgroundTasks` object used to process event emissions.
+        Initialize an instance of `FastAPIEventEmitter`.
+        :param background_tasks: The FastAPI `BackgroundTasks` object used to handle
+            the execution of event emissions.
         :param event_linker: Specifies the type of event linker to use for associating
             events with their respective event handlers. Defaults to `EventLinker`.
         :param debug: Specifies the debug mode for the logger. If `None`, it is
             determined based on the execution environment.
         """
-        # Call the parent class' __init__ method to set up the event linker
+        # Call the parent class' __init__ method
         super().__init__(event_linker=event_linker, debug=debug)
 
         # Check if the provided background_tasks object is valid
-        if background_tasks is None or not isinstance(background_tasks, BackgroundTasks):
-            raise PyventusException("The 'background_tasks' argument must be a valid FastAPI BackgroundTask instance.")
+        if background_tasks is None:
+            raise PyventusException("The 'background_tasks' argument cannot be None.")
+        if not isinstance(background_tasks, BackgroundTasks):
+            raise PyventusException("The 'background_tasks' argument must be an instance of the BackgroundTasks class.")
 
         # Set the background tasks
         self._background_tasks: BackgroundTasks = background_tasks
 
     def _process(self, event_emission: EventEmitter.EventEmission) -> None:
         # Submit the event emission to the background tasks
         self._background_tasks.add_task(event_emission)
```

### Comparing `pyventus-0.4.1/src/pyventus/emitters/rq/rq_event_emitter.py` & `pyventus-0.5.0/src/pyventus/emitters/rq/rq_event_emitter.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,54 +11,54 @@
         "Optional dependency 'rq' not found."
         "\nPlease install it using 'pip install pyventus[rq]' to use this event emitter."
     )
 
 
 class RQEventEmitter(EventEmitter):
     """
-    A class that enables event handling using the powerful Redis Queue (RQ) pub/sub and
-    worker system.
+    An event emitter subclass that utilizes the Redis Queue system to handle the
+    execution of event emissions.
 
-    This class extends the base `EventEmitter` class and provides the functionality to enqueue
-    event emissions using the [RQ package](https://python-rq.org/). Once enqueued, these event
-    emissions are processed by RQ workers. This event emitter is particularly useful when
-    dealing with events that require resource-intensive tasks like model optimization
-    or video processing.
+    **Notes:**
 
-    For more information and code examples, please refer to the `RQEventEmitter` tutorials
-    at: [https://mdapena.github.io/pyventus/tutorials/emitters/rq/](https://mdapena.github.io/pyventus/tutorials/emitters/rq/).
+    -   This class uses a Redis Queue instance to enqueue event emissions, which are
+        subsequently executed by Redis Queue workers. This approach provides a scalable
+        and distributed method for handling the execution of event emissions.
+
+    ---
+    Read more in the
+    [Pyventus docs for RQ Event Emitter](https://mdapena.github.io/pyventus/tutorials/emitters/rq/).
     """
 
     def __init__(
         self,
         queue: Queue,
         options: Dict[str, Any] | None = None,
         event_linker: Type[EventLinker] = EventLinker,
         debug: bool | None = None,
-    ):
+    ) -> None:
         """
-        Initializes an instance of the `RQEventEmitter` class.
+        Initialize an instance of `RQEventEmitter`.
         :param queue: The Redis queue for enqueuing event handlers.
         :param options: Additional options for the RQ package enqueueing method.
             Defaults to an empty dictionary.
-        :param event_linker: Specifies the type of event linker to use for associating
-            events with their respective event handlers. Defaults to `EventLinker`.
+        :param event_linker: Specifies the type of event linker used to manage and access
+            events along with their corresponding event handlers. Defaults to `EventLinker`.
         :param debug: Specifies the debug mode for the logger. If `None`, it is
             determined based on the execution environment.
         """
-        # Call the parent class' __init__ method to set up the event linker
+        # Call the parent class' __init__ method
         super().__init__(event_linker=event_linker, debug=debug)
 
         # Validate the queue argument
-        if queue is None or not isinstance(queue, Queue):
-            raise PyventusException("The 'queue' argument must be a valid (RQ) queue.")
+        if queue is None:
+            raise PyventusException("The 'queue' argument cannot be None.")
+        if not isinstance(queue, Queue):
+            raise PyventusException("The 'queue' argument must be an instance of the Queue class.")
 
-        # Store the RQ queue and options
+        # Store the Redis queue and RQ options
         self._queue: Queue = queue
-        """ The Redis queue for enqueuing event handlers. """
-
         self._options: Dict[str, Any] = options if options is not None else {}
-        """ Additional options for the RQ package enqueueing method. """
 
     def _process(self, event_emission: EventEmitter.EventEmission) -> None:
         # Add the event emission to the Redis Queue
         self._queue.enqueue(event_emission, **self._options)
```

### Comparing `pyventus-0.4.1/src/pyventus/handlers/event_handler.py` & `pyventus-0.5.0/src/pyventus/handlers/event_handler.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,207 +3,274 @@
 from inspect import isfunction, isclass, isbuiltin, ismethod
 from typing import Callable, Any, final, ParamSpec, TypeAlias
 
 from ..core.exceptions import PyventusException
 from ..core.loggers import StdOutLogger
 
 P = ParamSpec("P")
-""" A generic type to represent the parameter names and types of the callbacks. """
+"""A generic type representing the names and types of the event callback parameters."""
 
 EventCallbackType: TypeAlias = Callable[P, Any]
-""" Type alias for the main callback invoked when an associated event occurs. """
+"""Type alias for the event callback invoked when the associated event occurs."""
 
 SuccessCallbackType: TypeAlias = Callable[..., Any]
-""" Type alias for a callback invoked upon successful completion of an event. """
+"""Type alias for the callback invoked upon successful completion of the event."""
 
 FailureCallbackType: TypeAlias = Callable[[Exception], Any]
-""" Type alias for a callback invoked when event processing fails. """
+"""Type alias for the callback invoked when the event processing fails."""
 
 
 @final
 class EventHandler:
     """
-    A class that encapsulates event callbacks.
+    A class that encapsulates event callbacks and provides a mechanism for executing them
+    when the event occurs. This class manages both asynchronous and synchronous execution
+    and handles event completion in both success and error scenarios.
 
-    The `EventHandler` class provides a mechanism for managing and executing callbacks
-    when an event occurs.
+    **Notes:**
 
-    **Important**: The `__call__` method of the `EventHandler` class is always an async
-    method and returns a `Coroutine`. It should never be treated as a sync function.
+    -   The `__call__` method of the `EventHandler` class is an asynchronous method
+        that returns a `Coroutine`. It should never be treated as a synchronous function.
 
-    **Note:** The event handler can be invoked by calling the instance as a function
-    and passing the necessary arguments. If the event handler has the `once` property
-    set to `True`, it will only be invoked once when the event occurs. If `once` is set
-    to `False` (default), the event handler will be invoked every time the event occurs
-    until explicitly unsubscribed. Also, this class is not intended to be subclassed or
-    created manually. It is used internally to encapsulate the callbacks associated
-    with an event.
-    """
-
-    # Event handler attributes
-    __slots__ = (
-        "_once",
-        "_timestamp",
-        "_event_callback",
-        "_success_callback",
-        "_failure_callback",
-        "_is_event_callback_async",
-        "_is_success_callback_async",
-        "_is_failure_callback_async",
-    )
+    -   This class is not intended to be subclassed or manually created. It is used
+        internally to encapsulate the callbacks associated with an event and manage
+        their execution.
 
-    @property
-    def once(self) -> bool:
-        """
-        Determines if the handler is a one-time handler.
-        :return: `True` if the event handler is a one-time handler; otherwise, `False`.
-        """
-        return self._once
+    -   The event handler can be invoked by calling the instance as a function and
+        passing the required arguments.
 
-    @property
-    def timestamp(self) -> datetime:
-        """
-        Gets the timestamp of when the event handler was registered.
-        :return: The timestamp of when this handler was registered.
-        """
-        return self._timestamp
+    ---
+    Read more in the
+    [Pyventus docs for Event Handler](https://mdapena.github.io/pyventus/tutorials/event-linker/#event-handlers).
+    """
 
     @staticmethod
     def get_callback_name(
         callback: EventCallbackType | SuccessCallbackType | FailureCallbackType | None,  # type: ignore[type-arg]
     ) -> str:
+        """
+        Retrieves the name of the provided callback.
+        :param callback: The callback object.
+        :return: The name of the callback as a string.
+        """
         if callback is not None and hasattr(callback, "__name__"):
             return callback.__name__
         elif callback is not None and hasattr(callback, "__class__"):
-            return callback.__class__.__name__
+            return type(callback).__name__
         else:
             return "None"
 
     @staticmethod
     def validate_callback(
         callback: EventCallbackType | SuccessCallbackType | FailureCallbackType,  # type: ignore[type-arg]
     ) -> None:
         """
-        Validates that the provided callback is a compatible callable.
-        :param callback: The callback to validate.
+        Validates whether the provided callback is a valid callable object.
+        :param callback: The callback to be validated.
         :return: None
         :raises PyventusException: If the callback is not a callable object.
         """
         if not callable(callback):
             raise PyventusException(
                 f"'{callback.__name__ if hasattr(callback, '__name__') else callback}' is not a callable object."
             )
 
     @staticmethod
     def is_async(
         callback: EventCallbackType | SuccessCallbackType | FailureCallbackType,  # type: ignore[type-arg]
     ) -> bool:
         """
-        Checks if a callback is an asynchronous function or method.
-        :param callback: The callback to check.
-        :return: `True` if the callback is an asynchronous function or method,
-            `False` otherwise.
+        Checks whether the provided callback is an asynchronous function or method.
+        :param callback: The callback to be checked.
+        :return: `True` if the callback is an asynchronous function or method, `False` otherwise.
+        :raises PyventusException: If the callback is not a callable or a string.
         """
         if ismethod(callback) or isfunction(callback) or isbuiltin(callback):
             return iscoroutinefunction(callback)
-        elif not isclass(callback) and hasattr(callback, "__call__"):  # a callable class instance
+        elif not isclass(callback) and hasattr(callback, "__call__"):  # A callable class instance
             return iscoroutinefunction(callback.__call__)
         else:
             raise PyventusException("Expected a callable or a string, but got: {0}".format(callback))
 
+    # Event handler attributes
+    __slots__ = (
+        "_once",
+        "_force_async",
+        "_event_callback",
+        "_success_callback",
+        "_failure_callback",
+        "_is_event_callback_async",
+        "_is_success_callback_async",
+        "_is_failure_callback_async",
+        "_timestamp",
+    )
+
+    @property
+    def once(self) -> bool:
+        """
+        Determines if the event handler is a one-time subscription.
+        :return: A boolean value indicating if the event handler is
+            a one-time subscription.
+        """
+        return self._once
+
+    @property
+    def force_async(self) -> bool:
+        """
+        Determines whether all callbacks are forced to run asynchronously.
+        :return: A boolean value indicating if all callbacks are forced to run
+            asynchronously. If `True`, synchronous callbacks will be converted to
+            run asynchronously in a thread pool, using the `asyncio.to_thread`
+            function. If `False`, callbacks will run synchronously or
+            asynchronously as defined.
+        """
+        return self._force_async
+
+    @property
+    def timestamp(self) -> datetime:
+        """
+        Retrieves the timestamp when the event handler was created.
+        :return: The timestamp when the event handler was created.
+        """
+        return self._timestamp
+
     def __init__(
         self,
+        once: bool,
+        force_async: bool,
         event_callback: EventCallbackType,  # type: ignore[type-arg]
         success_callback: SuccessCallbackType | None = None,
         failure_callback: FailureCallbackType | None = None,
-        once: bool = False,
     ) -> None:
         """
-        Initializes an instance of the `EventHandler` class.
+        Initialize an instance of `EventHandler`.
+        :param once: Specifies if the event handler is a one-time subscription.
+        :param force_async: Determines whether to force all callbacks to run asynchronously.
+            If `True`, synchronous callbacks will be converted to run asynchronously in a
+            thread pool, using the `asyncio.to_thread` function. If `False`, callbacks
+            will run synchronously or asynchronously as defined.
         :param event_callback: The callback to be executed when the event occurs.
         :param success_callback: The callback to be executed when the event execution
-            completes successfully.
-        :param failure_callback: The callback to be executed when the event execution fails.
-        :param once: Specifies if the event handler is a one-time handler. If set to `True`,
-            the handler will be invoked once when the event occurs and then automatically
-            unsubscribed. If set to `False` (default), the handler can be invoked multiple
-            times until explicitly unsubscribed.
-        :raises PyventusException: If callbacks are invalid.
+            completes successfully. Default is `None`.
+        :param failure_callback: The callback to be executed when the event execution
+            fails. Default is `None`.
+        :raises PyventusException: If the provided callbacks are invalid.
         """
         # Validate callbacks
         EventHandler.validate_callback(callback=event_callback)
 
         if success_callback is not None:
             EventHandler.validate_callback(callback=success_callback)
 
         if failure_callback is not None:
             EventHandler.validate_callback(callback=failure_callback)
 
-        # Initialize attributes
+        # Validate flags
+        if not isinstance(once, bool):
+            raise PyventusException("The 'once' argument must be a boolean value.")
+        if not isinstance(force_async, bool):
+            raise PyventusException("The 'force_async' argument must be a boolean value.")
+
+        # Set the event handler flags
         self._once: bool = once
-        self._timestamp: datetime = datetime.now()
+        self._force_async: bool = force_async
 
-        # Store callbacks
+        # Set the event handler callbacks
         self._event_callback: EventCallbackType = event_callback  # type: ignore[type-arg]
         self._success_callback: SuccessCallbackType | None = success_callback
         self._failure_callback: FailureCallbackType | None = failure_callback
 
-        # Flags
+        # Set the event handler callbacks flags
         self._is_event_callback_async: bool = EventHandler.is_async(event_callback)
         self._is_success_callback_async: bool | None = (
             EventHandler.is_async(success_callback) if success_callback else None
         )
         self._is_failure_callback_async: bool | None = (
             EventHandler.is_async(failure_callback) if failure_callback else None
         )
 
+        # Set the event handler timestamp
+        self._timestamp: datetime = datetime.now()
+
     async def __call__(self, *args: P.args, **kwargs: P.kwargs) -> None:
         """
-        Executes the event handler by invoking the associated callbacks.
-        :param args: Variable-length argument list.
-        :param kwargs: Arbitrary keyword arguments.
+        Executes the event flow by invoking the associated callbacks.
+        :param args: Positional arguments to be passed to the event callback.
+        :param kwargs: Keyword arguments to be passed to the event callback.
         :return: Coroutine
         """
-        # Callback results
-        results: Any
+        # Event callback results
+        results: Any | None = None
 
         try:
-            # Invokes the event callback, checking if async.
+            # Invoke the event callback.
             if self._is_event_callback_async:
                 results = await self._event_callback(*args, **kwargs)
-            else:
+            elif self._force_async:
                 results = await to_thread(self._event_callback, *args, **kwargs)
+            else:
+                results = self._event_callback(*args, **kwargs)
         except Exception as exception:
             # Log the exception with error level
             StdOutLogger.error(name=f"{self.__class__.__name__}", action="Exception:", msg=f"{exception}")
 
-            # Invokes failure callback, checking if async.
+            # Invoke the failure callback and pass the exception.
             if self._failure_callback:
                 if self._is_failure_callback_async:
                     await self._failure_callback(exception)
-                else:
+                elif self._force_async:
                     await to_thread(self._failure_callback, exception)
+                else:
+                    self._failure_callback(exception)
         else:
-            # Invokes success callback, checking if async.
+            # Invoke the success callback and pass the results, if any.
             if self._success_callback:
                 if self._is_success_callback_async:
-                    if results:
+                    if results is None:
+                        await self._success_callback()
+                    else:
                         await self._success_callback(results)
+                elif self._force_async:
+                    if results is None:
+                        await to_thread(self._success_callback)
                     else:
-                        await self._success_callback()
-                else:
-                    if results:
                         await to_thread(self._success_callback, results)
+                else:
+                    if results is None:
+                        self._success_callback()
                     else:
-                        await to_thread(self._success_callback)
+                        self._success_callback(results)
 
     def __str__(self) -> str:
-        return (
-            f"Event Callback: '{EventHandler.get_callback_name(callback=self._event_callback)}'"
-            f"{' (Async)' if self._is_event_callback_async else ' (Sync)'} | "
-            f"Success Callback: '{EventHandler.get_callback_name(callback=self._success_callback)}'"
-            f"{' (Async)' if self._is_success_callback_async else ' (Sync)' if self._success_callback else ''} | "
-            f"Failure Callback: '{EventHandler.get_callback_name(callback=self._failure_callback)}'"
-            f"{' (Async)' if self._is_failure_callback_async else ' (Sync)' if self._failure_callback else ''} | "
-            f"Timestamp: {self.timestamp.strftime('%Y-%m-%d %I:%M:%S %p')} | "
-            f"Once: {self.once}"
+        """
+        Returns a formatted string representation of the event handler.
+        :return: A string representation of the event handler.
+        """
+        return "".join(
+            [
+                f"Event Callback: `{EventHandler.get_callback_name(callback=self._event_callback)}",
+                "` (Async) | " if self._is_event_callback_async else "` (Sync) | ",
+                (
+                    "Success Callback: `".join(
+                        [
+                            EventHandler.get_callback_name(callback=self._success_callback),
+                            "` (Async) | " if self._is_success_callback_async else "` (Sync) | ",
+                        ]
+                    )
+                    if self._success_callback
+                    else ""
+                ),
+                (
+                    "Failure Callback: `".join(
+                        [
+                            EventHandler.get_callback_name(callback=self._failure_callback),
+                            "` (Async) | " if self._is_failure_callback_async else "` (Sync) | ",
+                        ]
+                    )
+                    if self._failure_callback
+                    else ""
+                ),
+                f"Once: {self.once} | ",
+                f"Force Async: {self.force_async} | ",
+                f"Timestamp: {self.timestamp.strftime('%Y-%m-%d %I:%M:%S %p')}",
+            ]
         )
```

### Comparing `pyventus-0.4.1/src/pyventus/linkers/event_linker.py` & `pyventus-0.5.0/src/pyventus/linkers/event_linker.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,615 +1,680 @@
-from abc import ABC
-from itertools import chain
+from dataclasses import is_dataclass
 from sys import gettrace
 from threading import Lock
-from types import TracebackType
+from types import TracebackType, EllipsisType
 from typing import TypeAlias, Callable, Mapping, Tuple, Dict, List, Type, Set, Any, final
 
 from ..core.constants import StdOutColors
 from ..core.exceptions import PyventusException
 from ..core.loggers import Logger
-from ..events import Event
 from ..handlers import EventHandler, EventCallbackType, SuccessCallbackType, FailureCallbackType
 
-SubscribableEventType: TypeAlias = Type[Event] | Type[Exception] | str
-""" A type alias representing the supported event types for subscription. """
+SubscribableEventType: TypeAlias = str | Type[Exception] | Type[object] | EllipsisType
+"""A type alias representing the supported event types for subscription."""
 
 
-class EventLinker(ABC):
+class EventLinker:
     """
-    A base class that acts as a global registry for linking events with their associated event
-    handlers.
-
-    The `EventLinker` class provides a centralized mechanism for managing event subscriptions,
-    unsubscriptions, and retrieval of events and their associated event handlers. It acts as a
-    global registry, ensuring that events and their handlers are organized and easily accessible.
-
-    The `EventLinker` class can be subclassed to create specific namespaces or contexts for
-    managing events and event handlers separately. By subclassing the `EventLinker`, users can
-    organize event subscriptions and handlers within different scopes, providing modularity and
-    flexibility in event management. Subclassing also allows users to configure settings of the
-    `EventLinker` to suit their specific use cases.
-
-    **Thread-Safe:** The `EventLinker` has been implemented with thread safety in mind. All of its
-    methods synchronize access to prevent race conditions when managing events and event handlers
-    across multiple threads. This ensures that concurrent operations on the `EventLinker` are
-    properly synchronized, avoiding data inconsistencies and race conditions.
-
-    For more information and code examples, please refer to the `EventLinker` tutorials at:
-    [https://mdapena.github.io/pyventus/tutorials/event-linker/](https://mdapena.github.io/pyventus/tutorials/event-linker/).
+    A base class that acts as a global registry for events and callbacks linkage. It provides
+    a centralized mechanism for managing event subscriptions, unsubscriptions, and retrieval
+    of events and their associated event handlers.
+
+    **Notes:**
+
+    -   The `EventLinker` class can be subclassed to create specific namespaces or contexts
+        for managing events and event handlers separately. By subclassing the `EventLinker`,
+        users can organize event subscriptions and handlers within different scopes, providing
+        modularity and flexibility in event management. Subclassing also allows users to
+        configure settings of the `EventLinker` to suit their specific use cases.
+
+    -   The `EventLinker` has been implemented with *thread safety* in mind. All of its methods
+        synchronize access to prevent race conditions when managing events and event handlers
+        across multiple threads. This ensures that concurrent operations on the `EventLinker`
+        are properly synchronized, avoiding data inconsistencies and race conditions.
+
+    ---
+    Read more in the
+    [Pyventus docs for Event Linker](https://mdapena.github.io/pyventus/tutorials/event-linker/).
     """
 
     @final
     class EventLinkageWrapper:
         """
         A class that serves as a wrapper for event linking operations, providing a simplified
-        interface for subscribing events and associating callbacks.
+        interface for subscribing events with their corresponding callbacks.
 
-        This class can be used as either a decorator or context manager. As a decorator, it
-        automatically subscribes the decorated callback to the specified events.
+        **Notes:**
 
-        When used as a context manager via the `with` statement, it allows multiple callbacks
-        to be associated with events within the context block.
-
-        Also, this class is not intended to be subclassed or created manually. It is used
-        internally to serves as a wrapper for event linking operation.
-        """
+        -   This class can be used as either a decorator or a context manager. When used as a
+            decorator, it automatically subscribes the decorated callback to the provided events.
+            When used as a context manager with the `with` statement, it allows multiple callbacks
+            to be associated with the provided events within the context block.
+
+        -   This class is not intended to be subclassed or manually created.
+            The `EventLinkageWrapper` is used internally as a wrapper for event
+            linking operations.
+        """
+
+        # Event linkage wrapper attributes
+        __slots__ = (
+            "_event_linker",
+            "_events",
+            "_once",
+            "_force_async",
+            "_event_callback",
+            "_success_callback",
+            "_failure_callback",
+        )
 
         @property
         def on_event(self) -> Callable[[EventCallbackType], EventCallbackType]:  # type: ignore[type-arg]
             """
-            Decorator that sets the main callback for the event. This callback will be invoked
-            when the associated event occurs.
+            Decorator that sets the main callback for the event. This callback
+            will be invoked when the associated event occurs.
             :return: The decorated callback.
             """
 
             def _wrapper(callback: EventCallbackType) -> EventCallbackType:  # type: ignore[type-arg]
                 self._event_callback = callback
                 return callback
 
             return _wrapper
 
         @property
         def on_success(self) -> Callable[[SuccessCallbackType], SuccessCallbackType]:
             """
-            Decorator that sets the success callback. This callback will be invoked when the
-            event execution completes successfully.
+            Decorator that sets the success callback. This callback will be
+            invoked when the event execution completes successfully.
             :return: The decorated callback.
             """
 
             def _wrapper(callback: SuccessCallbackType) -> SuccessCallbackType:
                 self._success_callback = callback
                 return callback
 
             return _wrapper
 
         @property
         def on_failure(self) -> Callable[[FailureCallbackType], FailureCallbackType]:
             """
-            Decorator that sets the failure callback. This callback will be invoked when the
-            event execution fails.
+            Decorator that sets the failure callback. This callback
+            will be invoked when the event execution fails.
             :return: The decorated callback.
             """
 
             def _wrapper(callback: FailureCallbackType) -> FailureCallbackType:
                 self._failure_callback = callback
                 return callback
 
             return _wrapper
 
-        def __init__(self, *events: SubscribableEventType, event_linker: Type["EventLinker"], once: bool):
+        def __init__(
+            self,
+            *events: SubscribableEventType,
+            event_linker: Type["EventLinker"],
+            force_async: bool,
+            once: bool,
+        ) -> None:
             """
-            Initializes the wrapper instance.
-            :param events: The events to link/subscribe to.
-            :param event_linker: The event linker type for associating events with callbacks.
-            :param once: Whether the callback is a one-time subscription.
+            Initialize an instance of `EventLinkageWrapper`.
+            :param events: The events to subscribe/link to.
+            :param event_linker: The event linker instance used for subscription.
+            :param force_async: Determines whether to force all callbacks to run asynchronously.
+            :param once: Specifies if the callback is a one-time subscription.
             """
-            self._events: Tuple[SubscribableEventType, ...] = events
             self._event_linker: Type[EventLinker] = event_linker
-            self._once: bool = once
+            self._events: Tuple[SubscribableEventType, ...] = events
 
+            self._once: bool = once
+            self._force_async: bool = force_async
             self._event_callback: EventCallbackType | None = None  # type: ignore[type-arg, no-redef, assignment]
             self._success_callback: SuccessCallbackType | None = None  # type: ignore[no-redef, assignment]
             self._failure_callback: FailureCallbackType | None = None  # type: ignore[no-redef, assignment]
 
         def __call__(self, callback: EventCallbackType) -> EventCallbackType:  # type: ignore[type-arg]
             """
-            Decorates a callback to subscribe it to the specified events.
-            :param callback: The callback to associate.
+            Subscribes the provided events to the decorated callback.
+            :param callback: The callback to associate with the events.
             :return: The decorated callback.
             """
             self._event_callback = callback
             self._event_linker.subscribe(
                 *self._events,
                 event_callback=self._event_callback,
                 success_callback=None,
                 failure_callback=None,
+                force_async=self._force_async,
                 once=self._once,
             )
             del self
             return callback
 
         def __enter__(self) -> "EventLinker.EventLinkageWrapper":
             """
-            Enters the linkage context block, allowing multiple callbacks to be associated
-            with events within the block.
+            Enters the linkage context block, allowing multiple
+            callbacks to be associated with the events.
             :return: The context manager object
             """
             return self
 
         def __exit__(
             self, exc_type: Type[BaseException] | None, exc_val: BaseException | None, exc_tb: TracebackType | None
         ) -> None:
             """
-            Exits the linkage context manager, subscribing any callbacks associated within the
-            block to the specified events. Also performs any cleanup.
+            Exits the linkage context block, subscribing the provided callbacks within
+            the context to the specified events. Performs any necessary cleanup.
             :param exc_type: The type of the exception raised, if any.
             :param exc_val: The exception object raised, if any.
             :param exc_tb: The traceback information, if any.
             :return: None
             """
             self._event_linker.subscribe(
                 *self._events,
                 event_callback=self._event_callback,
                 success_callback=self._success_callback,
                 failure_callback=self._failure_callback,
+                force_async=self._force_async,
                 once=self._once,
             )
             del self
 
-    __event_registry: Dict[str, List[EventHandler]] = {}
+    __registry: Dict[str, List[EventHandler]] = {}
     """ 
-    A dictionary that serves as a container for storing events and their respective event handlers.
-    The keys represent event names, and the values are lists of `EventHandler` objects. 
+    A dictionary that serves as a container for storing events and their associated event 
+    handlers. The keys represent registered event names, and the values are lists of event
+    handler objects associated with each event.
     """
 
     __max_event_handlers: int | None = None
-    """ The maximum number of `EventHandlers` allowed per event, or None if no limit. """
+    """The maximum number of `EventHandlers` allowed per event, or `None` if there is no limit."""
 
     __default_success_callback: SuccessCallbackType | None = None
     """ 
-    Represents the default success callback function that will be assigned to event handlers in the
-    absence of a specific success callback. This callback will be executed upon successful completion
-    of the event execution in each event handler.
+    Represents the default success callback function that will be assigned to event handlers in 
+    the absence of a specific success callback. This callback will be executed upon successful 
+    completion of the event execution in each event handler.
     """
 
     __default_failure_callback: FailureCallbackType | None = None
     """
-    Represents the default failure callback function that will be assigned to event handlers in the 
-    absence of a specific failure callback. This callback will be executed when the event execution
-    fails in each event handler.
+    Represents the default failure callback function that will be assigned to event handlers in 
+    the absence of a specific failure callback. This callback will be executed when the event 
+    execution fails in each event handler.
     """
 
     __thread_lock: Lock = Lock()
     """
-    A `threading.Lock` object used for thread synchronization when accessing and modifying the event
-    registry to ensure thread safety. It prevents multiple threads from accessing or modifying the 
-    registry simultaneously.
+    A `threading.Lock` object used for thread synchronization when accessing and modifying the 
+    event registry to ensure thread safety. It prevents multiple threads from accessing and 
+    modifying the registry simultaneously.
     """
 
     __logger: Logger = Logger(name="EventLinker", debug=bool(gettrace() is not None))
     """
-    An instance of the logger used for logging events and debugging information. The debug mode
+    The logger used to debug and log information within the `EventLinker` class. The debug mode
     of the logger depends on the execution environment and the value returned by the `gettrace()`
     function. The debug mode can also be influenced by subclassing and overridden in subclasses.
     """
 
     def __init_subclass__(
         cls,
         max_event_handlers: int | None = None,
         default_success_callback: SuccessCallbackType | None = None,
         default_failure_callback: FailureCallbackType | None = None,
         debug: bool | None = None,
         **kwargs: Any,
     ) -> None:
         """
-        Custom `__init_subclass__` method called when a subclass is created.
+        Initialize a subclass of `EventLinker`.
 
-        This method initializes the subclass by setting up the event registry and thread
-        lock. It also allows specifying the maximum number of event handlers per event.
+        By default, this method sets up the main registry and thread lock object, but
+        it can also be used to configure specific settings of the `EventLinker` subclass.
 
         :param max_event_handlers: The maximum number of event handlers allowed per event,
-            or `None` if no limit.
-        :param default_success_callback: The default callback to be assigned as the success
+            or `None` if there is no limit.
+        :param default_success_callback: The default callback to assign as the success
             callback in the event handlers when no specific success callback is provided.
-        :param default_failure_callback: The default callback to be assigned as the failure
+        :param default_failure_callback: The default callback to assign as the failure
             callback in the event handlers when no specific failure callback is provided.
         :param debug: Specifies the debug mode for the subclass logger. If `None`,
             it is determined based on the execution environment.
         :param kwargs: The keyword arguments to pass to the superclass
             `__init_subclass__` method.
-        :raises PyventusException: If `max_event_handlers` is less than 1.
-        :return: Any
+        :raises PyventusException: If `max_event_handlers` is less than 1 or
+            if the provided callbacks are invalid.
+        :return: None
         """
         # Call the parent class' __init_subclass__ method
         super().__init_subclass__(**kwargs)
 
-        # Initialize the event registry dictionary
-        cls.__event_registry = {}
+        # Initialize the main registry
+        cls.__registry = {}
 
         # Create a lock object for thread synchronization
         cls.__thread_lock = Lock()
 
         # Validate the max_event_handlers argument
         if max_event_handlers is not None and max_event_handlers < 1:
             raise PyventusException("The 'max_event_handlers' argument must be greater than or equal to 1.")
 
         # Set the maximum number of event handlers per event
         cls.__max_event_handlers = max_event_handlers
 
         # Validate the default success callback, if any
-        if default_success_callback:
+        if default_success_callback is not None:
             EventHandler.validate_callback(callback=default_success_callback)
 
         # Set the default success callback
         cls.__default_success_callback = default_success_callback
 
         # Validate the default failure callback, if any
-        if default_failure_callback:
+        if default_failure_callback is not None:
             EventHandler.validate_callback(callback=default_failure_callback)
 
         # Set the default failure callback
         cls.__default_failure_callback = default_failure_callback
 
-        # Set up the logger for the subclass
+        # Validate the debug argument
+        if debug is not None and not isinstance(debug, bool):
+            raise PyventusException("The 'debug' argument must be a boolean value.")
+
+        # Set up the logger
         cls.__logger = Logger(
             name=cls.__name__,
             debug=debug if debug is not None else bool(gettrace() is not None),
         )
 
     @classmethod
-    def get_event_registry(cls) -> Mapping[str, List[EventHandler]]:
+    def _get_logger(cls) -> Logger:
         """
-        Retrieves the event registry mapping.
-        :return: A mapping of event names to event handlers.
+        Retrieve the class-level logger instance.
+        :return: The class-level logger instance used to debug and log
+            information within the `EventLinker` class.
         """
-        with cls.__thread_lock:
-            return {event: list(event_handlers) for event, event_handlers in cls.__event_registry.items()}
+        return cls.__logger
 
     @classmethod
-    def get_events(cls) -> List[str]:
+    def get_event_name(cls, event: SubscribableEventType) -> str:
         """
-        Returns a list of all the registered event names.
-        :return: A list of event names.
+        Determines the name of the event.
+        :param event: The event to obtain the name for.
+        :return: A string that represents the event name.
+        :raises PyventusException: If the `event` argument is invalid
+            or if the event is not supported.
         """
-        with cls.__thread_lock:
-            return list(cls.__event_registry.keys())
+        # Validate the event argument
+        if event is None:
+            raise PyventusException("The 'event' argument cannot be None.")
 
-    @classmethod
-    def get_event_handlers(cls) -> List[EventHandler]:
-        """
-        Retrieves a list of non-duplicated event handlers
-        who have been registered across all events.
-        :return: A list of event handlers.
-        """
-        with cls.__thread_lock:
-            return list(set(chain(*cls.__event_registry.values())))
+        if event is Ellipsis:
+            # If the event is Ellipsis, return its type name
+            return type(event).__name__
+        elif isinstance(event, str):
+            if not event:
+                raise PyventusException("String events cannot be empty.")
+            # If the event is a non-empty string, return it as the event name
+            return event
+        elif isinstance(event, type):
+            if not is_dataclass(event) and not issubclass(event, Exception):
+                raise PyventusException("Type events must be either a dataclass or an exception.")
+            # If the event is either a dataclass type or an exception type, return its type name
+            return event.__name__
+        else:
+            # If the event is not supported, raise an exception
+            raise PyventusException("Unsupported event")
 
     @classmethod
-    def get_max_event_handlers(cls) -> None | int:
+    def get_max_event_handlers(cls) -> int | None:
         """
-        Retrieves the maximum number of handlers allowed per event.
-        :return: The maximum number of handlers or None if there is no limit.
+        Retrieve the maximum number of event handlers allowed per event.
+        :return: The maximum number of event handlers or `None` if there is no limit.
         """
         return cls.__max_event_handlers
 
     @classmethod
     def get_default_success_callback(cls) -> SuccessCallbackType | None:
         """
-        Retrieves the default callback to be assigned as the success callback in
-            the event handlers when no specific success callback is provided.
-        :return: The default callback to be assigned as the success callback in
-            the event handlers when no specific success callback is provided.
+        Retrieve the default callback to be assigned as the success callback
+        in the event handlers when no specific success callback is provided.
+        :return: The default success callback or `None` if not set.
         """
         return cls.__default_success_callback
 
     @classmethod
     def get_default_failure_callback(cls) -> FailureCallbackType | None:
         """
-        Retrieves the default callback to be assigned as the failure callback
-            in the event handlers when no specific failure callback is provided.
-        :return: The default callback to be assigned as the failure callback
-            in the event handlers when no specific failure callback is provided.
+        Retrieve the default callback to be assigned as the failure callback
+        in the event handlers when no specific failure callback is provided.
+        :return: The default failure callback or `None` if not set.
         """
         return cls.__default_failure_callback
 
     @classmethod
-    def _get_logger(cls) -> Logger:
+    def get_registry(cls) -> Mapping[str, List[EventHandler]]:
         """
-        Returns the class-level logger instance.
-        :return: The class-level logger instance used for logging events and
-            debugging information.
+        Retrieve the main registry mapping.
+        :return: A mapping of event names to event handlers.
         """
-        return cls.__logger
+        with cls.__thread_lock:
+            return {event_name: list(event_handlers) for event_name, event_handlers in cls.__registry.items()}
 
     @classmethod
-    def _get_event_key(cls, event: SubscribableEventType) -> str:
+    def get_events(cls) -> List[str]:
         """
-        Determines the event string key based on the given event.
-        :param event: The event to obtain the key for.
-        :return: The event string key.
-        :raises PyventusException: If the `event` argument is None or if
-            the event type is not supported.
+        Retrieve a list of all the registered events.
+        :return: A list of event names.
         """
-        # Validate the event argument
-        if event is None:
-            raise PyventusException("The 'event' argument cannot be None.")
+        with cls.__thread_lock:
+            return list(cls.__registry.keys())
 
-        if isinstance(event, str):
-            # If the event is already a string, return it as the key
-            return event
-        elif issubclass(event, (Event, Exception)):
-            # If the event is a subclass of Event or Exception, return its name as the key
-            return event.__name__
-        else:
-            # If the event type is not supported, raise an exception
-            raise PyventusException("Unsupported event type")
+    @classmethod
+    def get_event_handlers(cls) -> List[EventHandler]:
+        """
+        Retrieve a list of non-duplicated event handlers
+        that have been registered across all events.
+        :return: A list of event handlers.
+        """
+        with cls.__thread_lock:
+            return list(
+                {event_handler for event_handlers in cls.__registry.values() for event_handler in event_handlers}
+            )
 
     @classmethod
-    def get_events_by_handler(cls, event_handler: EventHandler) -> List[str]:
+    def get_events_by_event_handler(cls, event_handler: EventHandler) -> List[str]:
         """
-        Retrieves a list of event names associated with the specified event handler.
+        Retrieve a list of event names associated with the provided event handler.
         :param event_handler: The handler to retrieve the associated events for.
         :return: A list of event names.
-        :raise PyventusException: If the `event_handler` argument is None.
+        :raise PyventusException: If the `event_handler` argument is `None` or invalid.
         """
         # Validate the event_handler argument
         if event_handler is None:
             raise PyventusException("The 'event_handler' argument cannot be None.")
+        if not isinstance(event_handler, EventHandler):
+            raise PyventusException("The 'event_handler' argument must be an instance of the EventHandler class.")
 
         with cls.__thread_lock:
             return [
-                event_key
-                for event_key, event_handlers in cls.__event_registry.items()
-                if event_handler in event_handlers
+                event_name for event_name, event_handlers in cls.__registry.items() if event_handler in event_handlers
             ]
 
     @classmethod
-    def get_handlers_by_events(cls, *events: SubscribableEventType) -> List[EventHandler]:
+    def get_event_handlers_by_events(cls, *events: SubscribableEventType) -> List[EventHandler]:
         """
-        Retrieves a list of non-duplicated event handlers associated with the specified events.
-        :param events: Events to retrieve the handlers for.
+        Retrieve a list of non-duplicated event handlers associated with the provided events.
+        :param events: Events to retrieve the event handlers for.
         :return: A list of event handlers.
-        :raise PyventusException: If the `events` argument is None, empty or unsupported.
+        :raise PyventusException: If the `events` argument is `None`, empty or unsupported.
         """
         # Validate the events argument
         if events is None or len(events) <= 0:
             raise PyventusException("The 'events' argument cannot be None or empty.")
 
-        # Retrieve all unique event keys
-        event_keys: Set[str] = set([cls._get_event_key(event=event) for event in events])
+        # Retrieve all unique event names
+        event_names: Set[str] = {cls.get_event_name(event=event) for event in events}
 
         with cls.__thread_lock:
             return list(
-                {event_handler for event_key in event_keys for event_handler in cls.__event_registry.get(event_key, [])}
+                {event_handler for event_name in event_names for event_handler in cls.__registry.get(event_name, [])}
             )
 
     @classmethod
-    def once(cls, *events: SubscribableEventType) -> EventLinkageWrapper:
+    def once(cls, *events: SubscribableEventType, force_async: bool = False) -> EventLinkageWrapper:
         """
-        Decorator that subscribes a callback to the specified events to be invoked only once.
-        This decorator is used to conveniently subscribe a callback as a one-time handler.
+        Decorator that allows you to conveniently subscribe callbacks to the provided events
+        for a single invocation.
+
+        This method can be used as either a decorator or a context manager. When used as a
+        decorator, it automatically subscribes the decorated callback to the provided events.
+        When used as a context manager with the `with` statement, it allows multiple callbacks
+        to be associated with the provided events within the context block.
+
         :param events: The events to subscribe to.
+        :param force_async: Determines whether to force all callbacks to run asynchronously.
+            If `True`, synchronous callbacks will be converted to run asynchronously in a
+            thread pool, using the `asyncio.to_thread` function. If `False`, callbacks
+            will run synchronously or asynchronously as defined.
         :return: The decorator that wraps the callback.
         """
-        return EventLinker.EventLinkageWrapper(*events, event_linker=cls, once=True)
+        return EventLinker.EventLinkageWrapper(*events, event_linker=cls, force_async=force_async, once=True)
 
     @classmethod
-    def on(cls, *events: SubscribableEventType) -> EventLinkageWrapper:
+    def on(cls, *events: SubscribableEventType, force_async: bool = False) -> EventLinkageWrapper:
         """
-        Decorator that subscribes a callback to the specified events.
+        Decorator that allows you to conveniently subscribe callbacks to the provided events.
+
+        This method can be used as either a decorator or a context manager. When used as a
+        decorator, it automatically subscribes the decorated callback to the provided events.
+        When used as a context manager with the `with` statement, it allows multiple callbacks
+        to be associated with the provided events within the context block.
+
         :param events: The events to subscribe to.
+        :param force_async: Determines whether to force all callbacks to run asynchronously.
+            If `True`, synchronous callbacks will be converted to run asynchronously in a
+            thread pool, using the `asyncio.to_thread` function. If `False`, callbacks
+            will run synchronously or asynchronously as defined.
         :return: The decorator that wraps the callback.
         """
-        return EventLinker.EventLinkageWrapper(*events, event_linker=cls, once=False)
+        return EventLinker.EventLinkageWrapper(*events, event_linker=cls, force_async=force_async, once=False)
 
     @classmethod
     def subscribe(
         cls,
         *events: SubscribableEventType,
         event_callback: EventCallbackType,  # type: ignore[type-arg]
         success_callback: SuccessCallbackType | None = None,
         failure_callback: FailureCallbackType | None = None,
+        force_async: bool = False,
         once: bool = False,
     ) -> EventHandler:
         """
-        Subscribes callbacks to the specified events.
+        Subscribes callbacks to the provided events.
         :param events: The events to subscribe to.
         :param event_callback: The callback to be executed when the event occurs.
         :param success_callback: The callback to be executed when the event execution completes
             successfully.
         :param failure_callback: The callback to be executed when the event execution fails.
-        :param once: Specifies if the callback is a one-time subscription. If set to `True`,
-            the handler will be invoked once when the event occurs and then automatically unsubscribed.
-            If set to `False` (default), the handler can be invoked multiple times until explicitly
-            unsubscribed.
-        :return: The event handler object associated with the events.
-        :raises PyventusException: If the maximum number of handlers for an event has been exceeded
-            or if the `events` argument is None, empty or unsupported.
+        :param force_async: Determines whether to force all callbacks to run asynchronously.
+            If `True`, synchronous callbacks will be converted to run asynchronously in a
+            thread pool, using the `asyncio.to_thread` function. If `False`, callbacks
+            will run synchronously or asynchronously as defined.
+        :param once: Specifies if the event handler is a one-time subscription.
+        :return: The event handler object associated with the given events.
         """
         # Validate the events argument
         if events is None or len(events) <= 0:
             raise PyventusException("The 'events' argument cannot be None or empty.")
 
-        # Retrieve all unique event keys
-        event_keys: Set[str] = set([cls._get_event_key(event=event) for event in events])
+        # Retrieve all unique event names
+        event_names: Set[str] = {cls.get_event_name(event=event) for event in events}
 
-        # Acquire the lock to ensure exclusive access to the event registry
+        # Acquire the lock to ensure exclusive access to the main registry
         with cls.__thread_lock:
             # Check if the maximum number of handlers property is set
             if cls.__max_event_handlers is not None:
-                # For each event key, check if the maximum number of handlers for the event has been exceeded
-                for event_key in event_keys:
-                    if len(cls.__event_registry.get(event_key, [])) >= cls.__max_event_handlers:
+                # For each event name, check if the maximum number of handlers for the event has been exceeded
+                for event_name in event_names:
+                    if len(cls.__registry.get(event_name, [])) >= cls.__max_event_handlers:
                         raise PyventusException(
-                            f"The event '{event_key}' has exceeded the maximum number of handlers allowed. The "
-                            f"'{event_callback.__name__ if hasattr(event_callback, '__name__') else event_callback}'"
-                            f" callback cannot be added."
+                            f"The event '{event_name}' has exceeded the maximum number of handlers allowed. The "
+                            f"'{EventHandler.get_callback_name(callback=event_callback)}'"
+                            f" callback cannot be subscribed."
                         )
 
             # Create a new event handler
             event_handler: EventHandler = EventHandler(
                 event_callback=event_callback,
                 success_callback=success_callback if success_callback else cls.__default_success_callback,
                 failure_callback=failure_callback if failure_callback else cls.__default_failure_callback,
+                force_async=force_async,
                 once=once,
             )
 
-            # For each event key, register the event handler
-            for event_key in event_keys:
-                # If the event key is not present in the event registry, create a new empty list for it
-                if event_key not in cls.__event_registry:
-                    cls.__event_registry[event_key] = []
+            # For each event name, register the event handler
+            for event_name in event_names:
+                # If the event name is not present in the main registry, create a new empty list for it
+                if event_name not in cls.__registry:
+                    cls.__registry[event_name] = []
 
                 # Append the event handler to the list of handlers for the event
-                cls.__event_registry[event_key].append(event_handler)
+                cls.__registry[event_name].append(event_handler)
 
                 # Log the subscription if debug is enabled
                 if cls.__logger.debug_enabled:  # pragma: no cover
                     cls.__logger.debug(
                         action="Subscribed:",
-                        msg=f"{event_handler} {StdOutColors.PURPLE}Event:{StdOutColors.DEFAULT} {event_key}",
+                        msg=f"{event_handler} {StdOutColors.PURPLE}Event:{StdOutColors.DEFAULT} {event_name}",
                     )
 
         # Return the new event handler
         return event_handler
 
     @classmethod
     def unsubscribe(cls, *events: SubscribableEventType, event_handler: EventHandler) -> bool:
         """
-        Unsubscribes an event handler from the specified events. The method removes the event
-        handler from the event registry and, if there are no more handlers for a particular
-        event, removes that event from the registry as well.
+        Unsubscribes an event handler from the provided events. If there are no more
+        handlers for a particular event, that event is also removed from the registry.
         :param events: The events to unsubscribe from.
         :param event_handler: The event handler to unsubscribe.
-        :return: `True` if the event handler associated with the events was found and removed,
-            `False` otherwise.
-        :raises PyventusException: If the `events` argument is None, empty, unsupported or if
-            the `event_handler` argument is None.
+        :return: `True` if the event handler associated with the events was found and
+            removed, `False` otherwise.
+        :raises PyventusException: If the `events` argument is `None`, empty, unsupported,
+            or if the `event_handler` argument is `None`, invalid.
         """
         # Validate the events argument
         if events is None or len(events) <= 0:
             raise PyventusException("The 'events' argument cannot be None or empty.")
 
         # Validate the event_handler argument
         if event_handler is None:
             raise PyventusException("The 'event_handler' argument cannot be None.")
+        if not isinstance(event_handler, EventHandler):
+            raise PyventusException("The 'event_handler' argument must be an instance of the EventHandler class.")
 
-        # Retrieve all unique event keys
-        event_keys: Set[str] = set([cls._get_event_key(event=event) for event in events])
+        # Retrieve all unique event names
+        event_names: Set[str] = {cls.get_event_name(event=event) for event in events}
 
-        # Flag indicating whether the event handler was successfully removed
+        # A flag indicating whether the event handler was successfully removed
         deleted: bool = False
 
-        # Obtain the lock to ensure exclusive access to the event registry
+        # Obtain the lock to ensure exclusive access to the main registry
         with cls.__thread_lock:
-            # For each event key, check and remove the event handler if found
-            for event_key in event_keys:
-                # Get the list of event handlers for the event key, or an empty list if it doesn't exist
-                event_handlers = cls.__event_registry.get(event_key, [])
+            # For each event name, check and remove the event handler if found
+            for event_name in event_names:
+                # Get the list of event handlers for the event name, or an empty list if it doesn't exist
+                event_handlers = cls.__registry.get(event_name, [])
 
                 # Check if the event handler is present in the list of handlers for the event
                 if event_handler in event_handlers:
                     # Remove the event handler from the list of handlers
                     event_handlers.remove(event_handler)
                     deleted = True
 
-                    # If there are no more handlers for the event, remove the event key from the registry
+                    # If there are no more handlers for the event, remove the event name from the registry
                     if not event_handlers:
-                        cls.__event_registry.pop(event_key)
+                        cls.__registry.pop(event_name)
 
                     # Log the unsubscription if debug is enabled
                     if cls.__logger.debug_enabled:  # pragma: no cover
                         cls.__logger.debug(
-                            action="Unsubscribed",
-                            msg=f"{event_handler} {StdOutColors.PURPLE}Event:{StdOutColors.DEFAULT} {event_key}",
+                            action="Unsubscribed:",
+                            msg=f"{event_handler} {StdOutColors.PURPLE}Event:{StdOutColors.DEFAULT} {event_name}",
                         )
 
         # Return the flag indicating whether the event handler was deleted
         return deleted
 
     @classmethod
     def remove_event_handler(cls, event_handler: EventHandler) -> bool:
         """
         Removes an event handler from all subscribed events. If there are no more
-        handlers for a particular event, that event is removed from the registry.
+        handlers for a particular event, that event is also removed from the registry.
         :param event_handler: The event handler to remove.
         :return: `True` if the event handler was found and removed, `False` otherwise.
-        :raises PyventusException: If the `event_handler` argument is None.
+        :raises PyventusException: If the `event_handler` argument is `None` or invalid.
         """
         # Validate the event_handler argument
         if event_handler is None:
             raise PyventusException("The 'event_handler' argument cannot be None.")
+        if not isinstance(event_handler, EventHandler):
+            raise PyventusException("The 'event_handler' argument must be an instance of the EventHandler class.")
 
         # A flag indicating if the event handler gets removed
         deleted: bool = False
 
-        # Acquire the lock to ensure exclusive access to the event registry
+        # Acquire the lock to ensure exclusive access to the main registry
         with cls.__thread_lock:
-            # Iterate through each event and its associated handlers in the event registry
-            for event_key in list(cls.__event_registry.keys()):
-                # Get the list of event handlers for the event key, or an empty list if it doesn't exist
-                event_handlers = cls.__event_registry.get(event_key, [])
+            # Iterate through each event and its associated handlers in the main registry
+            for event_name in list(cls.__registry.keys()):
+                # Get the list of event handlers for the event name, or an empty list if it doesn't exist
+                event_handlers = cls.__registry.get(event_name, [])
 
                 # Check if the event handler is present in the list of handlers for the event
                 if event_handler in event_handlers:
                     # Remove the event handler from the list of handlers
                     event_handlers.remove(event_handler)
                     deleted = True
 
                     # If there are no more handlers for the event, remove the event from the registry
                     if not event_handlers:
-                        cls.__event_registry.pop(event_key)
+                        cls.__registry.pop(event_name)
 
                     # Log the removal of the event handler if debug is enabled
                     if cls.__logger.debug_enabled:  # pragma: no cover
                         cls.__logger.debug(
                             action="Handler Removed:",
-                            msg=f"{event_handler} {StdOutColors.PURPLE}Event:{StdOutColors.DEFAULT} {event_key}",
+                            msg=f"{event_handler} {StdOutColors.PURPLE}Event:{StdOutColors.DEFAULT} {event_name}",
                         )
 
         # Return the flag indicating if the event handler was found and deleted
         return deleted
 
     @classmethod
     def remove_event(cls, event: SubscribableEventType) -> bool:
         """
-        Removes an event and all associated event handlers.
+        Removes an event from the registry, including all its event handler subscriptions.
         :param event: The event to remove.
         :return: `True` if the event was found and removed, `False` otherwise.
         """
-        # Get the event key
-        event_key: str = cls._get_event_key(event=event)
+        # Get the event name
+        event_name: str = cls.get_event_name(event=event)
 
-        # Acquire the lock to ensure exclusive access to the event registry
+        # Acquire the lock to ensure exclusive access to the main registry
         with cls.__thread_lock:
-            # Check if the event key is present in the event registry
-            if event_key in cls.__event_registry:
+            # Check if the event name is present in the main registry
+            if event_name in cls.__registry:
                 # Remove the event from the registry
-                cls.__event_registry.pop(event_key)
+                cls.__registry.pop(event_name)
 
                 # Log the removal of the event if debug is enabled
                 if cls.__logger.debug_enabled:  # pragma: no cover
-                    cls.__logger.debug(action="Event Removed:", msg=f"{event_key}")
+                    cls.__logger.debug(action="Event Removed:", msg=f"{event_name}")
 
                 # Return True to indicate successful removal
                 return True
 
         return False
 
     @classmethod
     def remove_all(cls) -> bool:
         """
-        Removes all events and event handlers.
+        Removes all events and their associated event handlers from the registry.
         :return: `True` if the events were found and removed, `False` otherwise.
         """
-        # Acquire the lock to ensure exclusive access to the event registry
+        # Acquire the lock to ensure exclusive access to the main registry
         with cls.__thread_lock:
-            # Clear the event registry by assigning an empty dictionary
-            cls.__event_registry = {}
+            if cls.__registry:
+                # Clear the main registry
+                cls.__registry.clear()
 
-        # Log a debug message if debug is enabled
-        if cls.__logger.debug_enabled:  # pragma: no cover
-            cls.__logger.debug(msg="All events and handlers were successfully removed")
+                # Log a debug message if debug is enabled
+                if cls.__logger.debug_enabled:  # pragma: no cover
+                    cls.__logger.debug(msg="All events and handlers were successfully removed.")
+
+                return True
+            else:
+                # Log a debug message if debug is enabled
+                if cls.__logger.debug_enabled:  # pragma: no cover
+                    cls.__logger.debug(msg="The event registry is already empty.")
 
-        return True
+                return False
```

### Comparing `pyventus-0.4.1/tests/emitters/event_emitter_test.py` & `pyventus-0.5.0/tests/emitters/event_emitter_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from abc import ABC, abstractmethod
 from contextlib import contextmanager
 from typing import Type, Generator, List, Dict
 
 from _pytest.python_api import raises
 
-from pyventus import EventEmitter, EventLinker, Event, PyventusException
+from pyventus import EventEmitter, EventLinker, PyventusException
 from .. import CallbackFixtures, EventFixtures
 
 
 class EventEmitterTest(ABC):
-    """
-    A set of pre-configured tests for subclasses of EventEmitter.
-    """
+    """A set of pre-configured tests for subclasses of EventEmitter."""
 
     @staticmethod
     @contextmanager
     def run_emission_test(event_emitter: EventEmitter, event_linker: Type[EventLinker] = EventLinker) -> Generator:
         """
         Context manager for performing tests to check if the event emission is working
         properly using both synchronous and asynchronous callbacks.
@@ -43,160 +41,166 @@
         :return: A generator object for the test.
         """
 
         # Clear event linker
         event_linker.remove_all()
 
         # Test emission when empty
-        event_emitter.emit(Event())
-
-        # Set Sync and Async callback class
-        sync_callback_cls: Type[CallbackFixtures.Base] = CallbackFixtures.Sync
-        async_callback_cls: Type[CallbackFixtures.Base] = CallbackFixtures.Async
+        event_emitter.emit(EventFixtures.EmptyEvent())
 
         # Create a dummy event linker for testing purposes
         class __DummyEventLinker(EventLinker, max_event_handlers=1):
             pass  # pragma: no cover
 
-        # --------------------
+        # ----------------------------------------------
         # Arrange
         # ----------
 
         int_param: int = 2
         str_param: str = "param1"
-        event_param: Event = Event()
+        event_param: object = EventFixtures.EmptyEvent()
         list_param: List[int] = [1, 2, 3, 4, 5, 6, 7, 8, 9]
         dict_param: Dict[str, str] = {"key1": "value1"}
-        custom_event1 = EventFixtures.CustomEvent1(attr1="attr1")
-        custom_event2 = EventFixtures.CustomEvent2(attr1={"attr1": "attr"}, attr2="attr2")
-        custom_event_with_validation = EventFixtures.CustomEventWithValidation(attr1="att", attr2=7.65)
+        custom_event1 = EventFixtures.DtcEvent1(attr1="attr1")
+        custom_event2 = EventFixtures.DtcEvent2(attr1="attr1", attr2={"attr2": "attr"})
+        custom_event_with_validation = EventFixtures.DtcWithValidation(attr1="att", attr2=7.65)
         custom_exception1 = EventFixtures.CustomException1("Custom Exception 1 raised!")
         custom_exception2 = EventFixtures.CustomException2("Custom Exception 2 raised!")
-        return_value: Event = Event()
+        return_value: object = EventFixtures.EmptyEvent()
 
         # Callbacks
-        cb_without_params: CallbackFixtures.Base = sync_callback_cls()
-        cb_with_two_params: CallbackFixtures.Base = async_callback_cls()
-        cb_with_args: CallbackFixtures.Base = sync_callback_cls()
-        cb_with_kwargs: CallbackFixtures.Base = async_callback_cls()
-        cb_with_custom_event1: CallbackFixtures.Base = sync_callback_cls()
-        cb_with_custom_event2_and_extras: CallbackFixtures.Base = async_callback_cls()
-        cb_with_custom_event_validated: CallbackFixtures.Base = sync_callback_cls()
-        cb_with_event: CallbackFixtures.Base = async_callback_cls()
-        cb_with_custom_exception1: CallbackFixtures.Base = sync_callback_cls()
-        cb_with_custom_exception2_and_extras: CallbackFixtures.Base = async_callback_cls()
-        cb_with_exception: CallbackFixtures.Base = sync_callback_cls()
-        cb_with_args_and_kwargs: CallbackFixtures.Base = async_callback_cls()
+        cb_without_params: CallbackFixtures.Base = CallbackFixtures.Sync()
+        cb_with_two_params: CallbackFixtures.Base = CallbackFixtures.Async()
+        cb_with_args: CallbackFixtures.Base = CallbackFixtures.Sync()
+        cb_with_kwargs: CallbackFixtures.Base = CallbackFixtures.Async()
+        cb_with_custom_event1: CallbackFixtures.Base = CallbackFixtures.Sync()
+        cb_with_custom_event2_and_extras: CallbackFixtures.Base = CallbackFixtures.Async()
+        cb_with_custom_event_validated: CallbackFixtures.Base = CallbackFixtures.Sync()
+        cb_with_event: CallbackFixtures.Base = CallbackFixtures.Async()
+        cb_with_custom_exception1: CallbackFixtures.Base = CallbackFixtures.Sync()
+        cb_with_custom_exception2_and_extras: CallbackFixtures.Base = CallbackFixtures.Async()
+        cb_with_exception: CallbackFixtures.Base = CallbackFixtures.Sync()
+        cb_with_args_and_kwargs: CallbackFixtures.Base = CallbackFixtures.Async()
 
-        cb_with_return_value: CallbackFixtures.Base = sync_callback_cls(return_value=return_value)
-        cb_with_raise_exception: CallbackFixtures.Base = async_callback_cls(raise_exception=custom_exception1)
+        cb_with_return_value: CallbackFixtures.Base = CallbackFixtures.Sync(return_value=return_value)
+        cb_with_raise_exception: CallbackFixtures.Base = CallbackFixtures.Async(raise_exception=custom_exception1)
 
         # Success and failure callbacks
         default_success_callback = event_linker.get_default_success_callback()
         success_callback: CallbackFixtures.Base = (
-            default_success_callback if default_success_callback else async_callback_cls()  # type: ignore
+            default_success_callback if default_success_callback else CallbackFixtures.Async()
         )
         default_failure_callback = event_linker.get_default_failure_callback()
         failure_callback: CallbackFixtures.Base = (
-            default_failure_callback if default_failure_callback else sync_callback_cls()  # type: ignore
+            default_failure_callback if default_failure_callback else CallbackFixtures.Sync()
         )
 
         # String Events
-        event_linker.subscribe("StringEventWithoutParams", event_callback=cb_without_params.__call__)
+        event_linker.subscribe("StringEventWithoutParams", event_callback=cb_without_params.__call__, force_async=True)
         event_linker.subscribe("StringEventWithoutParams", "AnotherStringEvent", event_callback=cb_without_params)
-        event_linker.subscribe("StringEventWithTwoParams", event_callback=cb_with_two_params)
+        event_linker.subscribe("StringEventWithTwoParams", event_callback=cb_with_two_params, force_async=True)
         event_linker.subscribe("StringEventWithArgs", event_callback=cb_with_args)
         event_linker.subscribe("StringEventWithKwargs", event_callback=cb_with_kwargs, once=True)
 
         # Events
-        event_linker.subscribe(EventFixtures.CustomEvent1, event_callback=cb_with_custom_event1)
-        event_linker.subscribe(EventFixtures.CustomEvent2, event_callback=cb_with_custom_event2_and_extras)
-        event_linker.subscribe(EventFixtures.CustomEventWithValidation, event_callback=cb_with_custom_event_validated)
+        event_linker.subscribe(EventFixtures.DtcEvent1, event_callback=cb_with_custom_event1)
+        event_linker.subscribe(EventFixtures.DtcEvent2, event_callback=cb_with_custom_event2_and_extras)
+        event_linker.subscribe(EventFixtures.DtcWithValidation, event_callback=cb_with_custom_event_validated)
         event_linker.subscribe(
-            EventFixtures.CustomEvent1, EventFixtures.CustomEvent2, event_callback=cb_with_event, once=True
+            EventFixtures.DtcEvent1, EventFixtures.DtcEvent2, event_callback=cb_with_event, once=True
         )
 
         # Exception Events
         event_linker.subscribe(EventFixtures.CustomException1, event_callback=cb_with_custom_exception1)
         event_linker.subscribe(EventFixtures.CustomException2, event_callback=cb_with_custom_exception2_and_extras)
-        event_linker.subscribe(TypeError, ValueError, event_callback=cb_with_exception)
-        event_linker.subscribe(Exception, event_callback=cb_with_exception, once=True)
+        event_linker.subscribe(TypeError, EventFixtures.CustomException1, event_callback=cb_with_exception, once=True)
 
-        # With success callback
+        # Test success callback execution
         with event_linker.once("StringEventWithSuccessCallback") as linker:
             linker.on_event(cb_with_return_value)
             linker.on_success(success_callback)
             linker.on_failure(failure_callback)
 
-        # With success callback
-        with event_linker.on("StringEventWithFailureCallback") as linker:
+        # Test failure callback execution
+        with event_linker.on("StringEventWithFailureCallback", force_async=True) as linker:
             linker.on_event(cb_with_raise_exception)
             linker.on_success(success_callback)
             linker.on_failure(failure_callback)
 
-        # Any Event and Exception
-        event_linker.subscribe(Event, Exception, event_callback=cb_with_args_and_kwargs)
+        # Test Error Handling
+        with event_linker.on("ErrorHandling") as linker:
+            linker.on_event(CallbackFixtures.Sync())
+            linker.on_success(CallbackFixtures.Async(raise_exception=ValueError("Something went wrong!")))
+            linker.on_failure(failure_callback)
+
+        with event_linker.on("ErrorHandling") as linker:
+            linker.on_event(CallbackFixtures.Sync(raise_exception=ValueError("Something went wrong!")))
+            linker.on_success(success_callback)
+            linker.on_failure(CallbackFixtures.Async(raise_exception=ValueError("Something went wrong!")))
+
+        # Any Event
+        event_linker.subscribe(..., event_callback=cb_with_args_and_kwargs)
 
         # Different namespace
-        __DummyEventLinker.subscribe(Event, Exception, event_callback=cb_with_args_and_kwargs)
+        __DummyEventLinker.subscribe(..., event_callback=cb_with_args_and_kwargs)
 
-        # --------------------
+        # ----------------------------------------------
         # Act
         # ----------
 
         # String events
-        with raises(PyventusException):
-            event_emitter.emit("")
-        with raises(PyventusException):
-            event_emitter.emit(None)  # type: ignore
-
         event_emitter.emit("AnotherStringEvent")
         event_emitter.emit("StringEventWithoutParams")
         event_emitter.emit("StringEventWithTwoParams", dict_param, param2=event_param)
         event_emitter.emit("StringEventWithTwoParams", dict_param, param2=event_param)
         event_emitter.emit("StringEventWithArgs", int_param, str_param, dict_param)
         event_emitter.emit("StringEventWithKwargs", param1=int_param, param2=str_param, param3=list_param)
         event_emitter.emit("StringEventWithKwargs", str_param, param2=int_param, param3=dict_param)
         event_emitter.emit("UnsubscribedEvent", int_param, param2=dict_param)
 
-        # Events
         with raises(PyventusException):
-            event_emitter.emit(Event)  # type: ignore
-        with raises(ValueError):
-            event_emitter.emit(EventFixtures.CustomEventWithValidation(attr1="at", attr2=2.3))
+            event_emitter.emit("")
 
+        # Events
         event_emitter.emit(custom_event1)
         event_emitter.emit(custom_event2, int_param, str_param, param3=event_param, param4=list_param)
         event_emitter.emit(custom_event_with_validation)
-        event_emitter.emit(Event())
+        event_emitter.emit(EventFixtures.EmptyEvent())
 
-        # Exception events
         with raises(PyventusException):
-            event_emitter.emit(Exception)  # type: ignore
+            event_emitter.emit(None)
+        with raises(PyventusException):
+            event_emitter.emit(EventFixtures.EmptyEvent)
+        with raises(PyventusException):
+            event_emitter.emit(EventFixtures.DtcWithValidation(attr1="at", attr2=2.3))
 
+        # Exception events
         event_emitter.emit(custom_exception1)
         event_emitter.emit(custom_exception2, int_param, str_param, param2=event_param, param3=list_param)
-
         event_emitter.emit(Exception())
 
         try:
-            EventFixtures.CustomEventWithValidation(attr1="at", attr2=7)
-        except ValueError as e:
+            EventFixtures.DtcWithValidation(attr1="at", attr2=7)
+        except PyventusException as e:
             event_emitter.emit(e)
 
+        with raises(PyventusException):
+            event_emitter.emit(Exception)
+
         # Events with success and failure callbacks
         event_emitter.emit("StringEventWithSuccessCallback")
         event_emitter.emit("StringEventWithSuccessCallback")
         event_emitter.emit("StringEventWithFailureCallback")
+        event_emitter.emit("ErrorHandling")
 
         # Wait for all events to propagate
         yield
 
-        # --------------------
-        # Asserts
+        # ----------------------------------------------
+        # Assert
         # ----------
 
         assert cb_without_params.call_count == 3
 
         assert cb_with_two_params.call_count == 2
         assert cb_with_two_params.args == (dict_param,)
         assert cb_with_two_params.kwargs == {"param2": event_param}
@@ -229,15 +233,16 @@
         assert cb_with_custom_exception1.args == (custom_exception1,)
         assert not cb_with_custom_exception1.kwargs
 
         assert cb_with_custom_exception2_and_extras.call_count == 1
         assert cb_with_custom_exception2_and_extras.args == (custom_exception2, int_param, str_param)
         assert cb_with_custom_exception2_and_extras.kwargs == {"param2": event_param, "param3": list_param}
 
-        assert cb_with_exception.call_count == 2
+        assert cb_with_exception.call_count == 1
+        assert cb_with_exception.args == (custom_exception1,)
         assert not cb_with_exception.kwargs
 
         assert cb_with_return_value.call_count == 1
         assert not cb_with_return_value.args
         assert not cb_with_return_value.kwargs
         assert cb_with_return_value.return_value == return_value
 
@@ -249,15 +254,15 @@
         assert not cb_with_raise_exception.args
         assert not cb_with_raise_exception.kwargs
 
         assert failure_callback.call_count == 1
         assert failure_callback.args == (custom_exception1,)
         assert not failure_callback.kwargs
 
-        assert cb_with_args_and_kwargs.call_count == 19
+        assert cb_with_args_and_kwargs.call_count == 20
 
     @abstractmethod
     def test_emission_in_sync_context(self, *args, **kwargs) -> None:
         """
         Performs tests to check if the event emission is working properly within a (SYNC) context.
         """
         pass
```

### Comparing `pyventus-0.4.1/tests/emitters/asyncio/test_asyncio_event_emitter.py` & `pyventus-0.5.0/tests/emitters/asyncio/test_asyncio_event_emitter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,55 +1,45 @@
 import asyncio
 
 import pytest
 from _pytest.python_api import raises
 
-from ..event_emitter_test import EventEmitterTest
 from pyventus import EventLinker, AsyncIOEventEmitter, PyventusException
+from ..event_emitter_test import EventEmitterTest
 
 
 class TestAsyncIOEventEmitter(EventEmitterTest):
     @staticmethod
-    async def __run_until_complete():
+    async def __run_until_complete() -> None:
         """Waits for all AsyncIO pending task to complete"""
         await asyncio.gather(*asyncio.all_tasks().difference({asyncio.current_task()}), return_exceptions=True)
 
-    # --------------------
-    # Creation
-    # ----------
-
-    def test_creation(self, clean_event_linker: bool) -> None:
+    def test_creation(self) -> None:
         event_emitter = AsyncIOEventEmitter()
         assert event_emitter is not None
 
-    def test_creation_with_invalid_params(self, clean_event_linker: bool) -> None:
+    def test_creation_with_invalid_params(self) -> None:
         with raises(PyventusException):
-            AsyncIOEventEmitter(event_linker=None)  # type: ignore
-
-    # --------------------
-    # Sync Context
-    # ----------
+            AsyncIOEventEmitter(event_linker=None)
+        with raises(PyventusException):
+            AsyncIOEventEmitter(event_linker=Exception)
 
     def test_emission_in_sync_context(self) -> None:
         event_emitter = AsyncIOEventEmitter()
         with TestAsyncIOEventEmitter.run_emission_test(event_emitter=event_emitter):
             pass
 
     def test_emission_in_sync_context_with_custom_event_linker(self) -> None:
         class CustomEventLinker(EventLinker):
             pass
 
         event_emitter = AsyncIOEventEmitter(event_linker=CustomEventLinker)
         with TestAsyncIOEventEmitter.run_emission_test(event_emitter=event_emitter, event_linker=CustomEventLinker):
             pass
 
-    # --------------------
-    # Async Context
-    # ----------
-
     @pytest.mark.asyncio
     async def test_emission_in_async_context(self) -> None:
         event_emitter = AsyncIOEventEmitter()
         with TestAsyncIOEventEmitter.run_emission_test(event_emitter=event_emitter):
             await TestAsyncIOEventEmitter.__run_until_complete()
 
     @pytest.mark.asyncio
```

### Comparing `pyventus-0.4.1/tests/emitters/celery/test_celery_event_emitter.py` & `pyventus-0.5.0/tests/emitters/celery/test_celery_event_emitter.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,86 +5,67 @@
 from pyventus import PyventusException, EventLinker
 from pyventus.emitters.celery import CeleryEventEmitter
 from ..event_emitter_test import EventEmitterTest
 from ... import CeleryMock
 
 
 class TestCeleryEventEmitter(EventEmitterTest):
-    # --------------------
-    # Creation
-    # ----------
-
-    def test_creation(
-        self,
-        clean_event_linker: bool,
-        celery_queue: CeleryEventEmitter.Queue,
-    ) -> None:
+
+    def test_payload(self):
+        # Arrange | Act | Assert
+        payload = CeleryEventEmitter.Queue._Payload.from_json(serialized_obj=b"object", obj_hash=b"hash")
+        assert payload is not None
+
+        # Arrange | Act | Assert
+        with raises(PyventusException):
+            CeleryEventEmitter.Queue._Payload.from_json(serialized_obj=b"object")
+
+        # Arrange | Act | Assert
+        with raises(PyventusException):
+            CeleryEventEmitter.Queue._Payload.from_json(serialized_obj=b"object", obj_hash=b"hash", extra="extra")
+
+    def test_creation(self, celery_queue: CeleryEventEmitter.Queue) -> None:
         event_emitter = CeleryEventEmitter(queue=celery_queue)
         assert event_emitter is not None
 
-    def test_creation_with_invalid_params(
-        self,
-        clean_event_linker: bool,
-    ) -> None:
+    def test_creation_with_invalid_params(self) -> None:
+        with raises(PyventusException):
+            CeleryEventEmitter(queue=None)
         with raises(PyventusException):
-            CeleryEventEmitter(queue=None)  # type: ignore
+            CeleryEventEmitter(queue=True)
 
         with raises(PyventusException):
-            CeleryEventEmitter.Queue(celery=None)  # type: ignore
+            CeleryEventEmitter.Queue(celery=None)
+        with raises(PyventusException):
+            CeleryEventEmitter.Queue(celery=True)
 
         with raises(PyventusException):
             CeleryEventEmitter.Queue(celery=Celery())
-
         with raises(PyventusException):
             celery_app = CeleryMock()
             celery_app.conf.accept_content = ["application/json", "application/x-python-serialize"]
             CeleryEventEmitter.Queue(celery=celery_app, secret="")
 
-    # --------------------
-    # Sync Context
-    # ----------
-
     def test_emission_in_sync_context(self, celery_queue: CeleryEventEmitter.Queue) -> None:
         event_emitter = CeleryEventEmitter(queue=celery_queue)
         with TestCeleryEventEmitter.run_emission_test(event_emitter=event_emitter):
             pass
 
     def test_emission_in_sync_context_with_custom_event_linker(self, celery_queue: CeleryEventEmitter.Queue) -> None:
         class CustomEventLinker(EventLinker):
             pass
 
         event_emitter = CeleryEventEmitter(queue=celery_queue, event_linker=CustomEventLinker)
         with TestCeleryEventEmitter.run_emission_test(event_emitter=event_emitter, event_linker=CustomEventLinker):
             pass
 
-    # --------------------
-    # Async Context
-    # ----------
-
     @pytest.mark.asyncio
     async def test_emission_in_async_context(self) -> None:
         pytest.skip(
             "Celery package doesn't support async tests yet, but works fine in async contexts outside of testing."
         )
 
     @pytest.mark.asyncio
     async def test_emission_in_async_context_with_custom_event_linker(self) -> None:
         pytest.skip(
             "Celery package doesn't support async tests yet, but works fine in async contexts outside of testing."
         )
-
-    # --------------------
-    # Extras
-    # ----------
-
-    def test_queue_payload(self):
-        # Arrange | Act | Assert
-        payload = CeleryEventEmitter.Queue._Payload.from_json(serialized_obj=b"object", obj_hash=b"hash")
-        assert payload is not None
-
-        # Arrange | Act | Assert
-        with raises(PyventusException):
-            CeleryEventEmitter.Queue._Payload.from_json(serialized_obj=b"object")
-
-        # Arrange | Act | Assert
-        with raises(PyventusException):
-            CeleryEventEmitter.Queue._Payload.from_json(serialized_obj=b"object", obj_hash=b"hash", extra="extra")
```

### Comparing `pyventus-0.4.1/tests/emitters/executor/test_executor_event_emitter.py` & `pyventus-0.5.0/tests/emitters/executor/test_executor_event_emitter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,34 @@
 from concurrent.futures import ThreadPoolExecutor, ProcessPoolExecutor
 
 import pytest
+from _pytest.python_api import raises
 
-from ..event_emitter_test import EventEmitterTest
 from pyventus import ExecutorEventEmitter, EventLinker, PyventusException
+from ..event_emitter_test import EventEmitterTest
 
 
 class TestExecutorEventEmitter(EventEmitterTest):
-    # --------------------
-    # Creation
-    # ----------
 
-    def test_creation(self, clean_event_linker: bool) -> None:
+    def test_creation(self) -> None:
         # Thread event emitter
-        thread_emitter = ExecutorEventEmitter()
+        thread_emitter = ExecutorEventEmitter(executor=ThreadPoolExecutor())
         assert thread_emitter is not None
         thread_emitter.shutdown()
 
         # Process event emitter
         process_emitter = ExecutorEventEmitter(executor=ProcessPoolExecutor())
         assert process_emitter is not None
         process_emitter.shutdown()
 
-    def test_creation_with_invalid_params(self, clean_event_linker: bool) -> None:
-        with pytest.raises(PyventusException):
-            ExecutorEventEmitter(event_linker=None)  # type: ignore
-        with pytest.raises(PyventusException):
-            ExecutorEventEmitter(executor=None)  # type: ignore
-
-    # --------------------
-    # SyncContext
-    # ----------
+    def test_creation_with_invalid_params(self) -> None:
+        with raises(PyventusException):
+            ExecutorEventEmitter(executor=None)
+        with raises(PyventusException):
+            ExecutorEventEmitter(executor=True)
 
     def test_emission_in_sync_context(self) -> None:
         # Thread emission
         thread_emitter = ExecutorEventEmitter(executor=ThreadPoolExecutor())
         with TestExecutorEventEmitter.run_emission_test(event_emitter=thread_emitter), thread_emitter:
             pass  # pragma: no cover
 
@@ -42,18 +36,14 @@
         class CustomEventLinker(EventLinker):
             pass
 
         thread_emitter = ExecutorEventEmitter(executor=ThreadPoolExecutor(), event_linker=CustomEventLinker)
         with TestExecutorEventEmitter.run_emission_test(event_emitter=thread_emitter, event_linker=CustomEventLinker):
             thread_emitter.shutdown(wait=True)
 
-    # --------------------
-    # Async Context
-    # ----------
-
     @pytest.mark.asyncio
     async def test_emission_in_async_context(self) -> None:
         # Thread emission
         thread_emitter = ExecutorEventEmitter(executor=ThreadPoolExecutor())
         with TestExecutorEventEmitter.run_emission_test(event_emitter=thread_emitter):
             thread_emitter.shutdown(wait=True)
```

### Comparing `pyventus-0.4.1/tests/emitters/fastapi/test_fastapi_event_emitter.py` & `pyventus-0.5.0/tests/emitters/fastapi/test_fastapi_event_emitter.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,126 +8,81 @@
 from pyventus import EventLinker, PyventusException
 from pyventus.emitters.fastapi import FastAPIEventEmitter
 from ..event_emitter_test import EventEmitterTest
 from ... import FastAPITestContext
 
 
 class TestFastAPIEventEmitter(EventEmitterTest):
-    # --------------------
-    # Creation
-    # ----------
-
-    def test_creation(
-        self,
-        clean_event_linker: bool,
-        fastapi_test_context: FastAPITestContext,
-    ) -> None:
-        # Arrange
+
+    def test_creation(self, fastapi_test_context: FastAPITestContext) -> None:
         @fastapi_test_context.client.app.get("/")
         def callback(
             background_tasks: BackgroundTasks,
             event_emitter1: FastAPIEventEmitter = Depends(FastAPIEventEmitter),
             event_emitter2: FastAPIEventEmitter = Depends(FastAPIEventEmitter.options(debug=True)),
         ) -> None:
             event_emitter0 = FastAPIEventEmitter(background_tasks=background_tasks, debug=False)
             assert event_emitter0 and isinstance(event_emitter0, FastAPIEventEmitter)
             assert event_emitter1 and isinstance(event_emitter1, FastAPIEventEmitter)
             assert event_emitter2 and isinstance(event_emitter2, FastAPIEventEmitter)
 
-        # Act
         res = fastapi_test_context.client.get("/")
 
-        # Assert
         assert res.status_code == status.HTTP_200_OK
 
-    def test_creation_with_invalid_params(
-        self,
-        clean_event_linker: bool,
-        fastapi_test_context: FastAPITestContext,
-    ) -> None:
-        # Arrange | Act | Assert
+    def test_creation_with_invalid_params(self, fastapi_test_context: FastAPITestContext) -> None:
+        with raises(PyventusException):
+            FastAPIEventEmitter(background_tasks=None)
         with raises(PyventusException):
-            FastAPIEventEmitter(background_tasks=None)  # type: ignore
+            FastAPIEventEmitter(background_tasks=True)
 
-    # --------------------
-    # Sync Context
-    # ----------
-
-    def test_emission_in_sync_context(
-        self,
-        fastapi_test_context: FastAPITestContext,
-    ) -> None:
-        # Arrange
+    def test_emission_in_sync_context(self, fastapi_test_context: FastAPITestContext) -> None:
         @fastapi_test_context.client.app.get("/")
         def callback(event_emitter: FastAPIEventEmitter = Depends(FastAPIEventEmitter)) -> None:
             with TestFastAPIEventEmitter.run_emission_test(event_emitter=event_emitter):
                 pass
 
-        # Act
         res = fastapi_test_context.client.get("/")
 
-        # Assert
         assert res.status_code == status.HTTP_200_OK
 
-    def test_emission_in_sync_context_with_custom_event_linker(
-        self,
-        fastapi_test_context: FastAPITestContext,
-    ) -> None:
-        # Arrange
+    def test_emission_in_sync_context_with_custom_event_linker(self, fastapi_test_context: FastAPITestContext) -> None:
         class CustomEventLinker(EventLinker):
             pass
 
         @fastapi_test_context.client.app.get("/")
         def callback(
             event_emitter: FastAPIEventEmitter = Depends(FastAPIEventEmitter.options(event_linker=CustomEventLinker)),
         ) -> None:
             with TestFastAPIEventEmitter.run_emission_test(event_emitter=event_emitter, event_linker=CustomEventLinker):
                 pass
 
-        # Act
         res = fastapi_test_context.client.get("/")
 
-        # Assert
         assert res.status_code == status.HTTP_200_OK
 
-    # --------------------
-    # Async Context
-    # ----------
-
     @pytest.mark.asyncio
-    async def test_emission_in_async_context(
-        self,
-        fastapi_test_context: FastAPITestContext,
-    ) -> None:
-        # Arrange
+    async def test_emission_in_async_context(self, fastapi_test_context: FastAPITestContext) -> None:
         @fastapi_test_context.client.app.get("/")
         async def callback(event_emitter: FastAPIEventEmitter = Depends(FastAPIEventEmitter)) -> None:
             with TestFastAPIEventEmitter.run_emission_test(event_emitter=event_emitter):
                 await asyncio.gather(*fastapi_test_context.background_futures, return_exceptions=True)
 
-        # Act
         res = fastapi_test_context.client.get("/")
 
-        # Assert
         assert res.status_code == status.HTTP_200_OK
 
     @pytest.mark.asyncio
-    async def test_emission_in_async_context_with_custom_event_linker(
-        self,
-        fastapi_test_context: FastAPITestContext,
-    ) -> None:
-        # Arrange
+    async def test_emission_in_async_context_with_custom_event_linker(self, fastapi_test_context: FastAPITestContext):
         class CustomEventLinker(EventLinker):
             pass
 
         @fastapi_test_context.client.app.get("/")
         async def callback(
             event_emitter: FastAPIEventEmitter = Depends(FastAPIEventEmitter.options(event_linker=CustomEventLinker)),
         ) -> None:
             with TestFastAPIEventEmitter.run_emission_test(event_emitter=event_emitter, event_linker=CustomEventLinker):
                 await asyncio.gather(*fastapi_test_context.background_futures, return_exceptions=True)
 
-        # Act
         res = fastapi_test_context.client.get("/")
 
-        # Assert
         assert res.status_code == status.HTTP_200_OK
```

### Comparing `pyventus-0.4.1/tests/emitters/rq/test_rq_event_emitter.py` & `pyventus-0.5.0/tests/emitters/rq/test_rq_event_emitter.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,49 +4,38 @@
 
 from pyventus import EventLinker, PyventusException
 from pyventus.emitters.rq import RQEventEmitter
 from ..event_emitter_test import EventEmitterTest
 
 
 class TestRQEventEmitter(EventEmitterTest):
-    # --------------------
-    # Creation
-    # ----------
 
-    def test_creation(self, clean_event_linker: bool, rq_queue: Queue):
-        # Arrange, Act and Assert
+    def test_creation(self, rq_queue: Queue):
         event_emitter = RQEventEmitter(queue=rq_queue)
         assert event_emitter is not None
 
-    def test_creation_with_invalid_params(self, clean_event_linker: bool):
-        # Arrange, Act and Assert
+    def test_creation_with_invalid_params(self):
         with raises(PyventusException):
-            RQEventEmitter(queue=None)  # type: ignore
-
-    # --------------------
-    # Sync Context
-    # ----------
+            RQEventEmitter(queue=None)
+        with raises(PyventusException):
+            RQEventEmitter(queue=True)
 
     def test_emission_in_sync_context(self, rq_queue: Queue):
         event_emitter = RQEventEmitter(queue=rq_queue)
         with TestRQEventEmitter.run_emission_test(event_emitter=event_emitter):
             pass
 
     def test_emission_in_sync_context_with_custom_event_linker(self, rq_queue: Queue):
         class CustomEventLinker(EventLinker):
             pass
 
         event_emitter = RQEventEmitter(queue=rq_queue, event_linker=CustomEventLinker)
         with TestRQEventEmitter.run_emission_test(event_emitter=event_emitter, event_linker=CustomEventLinker):
             pass
 
-    # --------------------
-    # Async Context
-    # ----------
-
     @pytest.mark.asyncio
     async def test_emission_in_async_context(self):
         pytest.skip("RQ package doesn't support async tests yet, but works fine in async contexts outside of testing.")
 
     @pytest.mark.asyncio
     async def test_emission_in_async_context_with_custom_event_linker(self):
         pytest.skip("RQ package doesn't support async tests yet, but works fine in async contexts outside of testing.")
```

### Comparing `pyventus-0.4.1/.gitignore` & `pyventus-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyventus-0.4.1/LICENSE` & `pyventus-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyventus-0.4.1/README.md` & `pyventus-0.5.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 <br>
 
 <p align="center">
    <img src="https://mdapena.github.io/pyventus/images/logo/pyventus-logo-name-slogan.svg" alt="Pyventus" width="750px">
 </p>
 
 <br>
@@ -17,444 +18,569 @@
 </a>
 
 <a href='https://coveralls.io/github/mdapena/pyventus?branch=master'>
 	<img src='https://coveralls.io/repos/github/mdapena/pyventus/badge.svg?branch=master' alt='Coverage Status'/>
 </a>
 
 <a href="https://pypi.org/project/pyventus" target="_blank">
-    <img src="https://img.shields.io/pypi/v/pyventus?color=blue" alt="Package version">
+    <img src="https://img.shields.io/pypi/v/pyventus?color=0097a8" alt="Package version">
 </a>
 
 <a href="https://pypi.org/project/pyventus" target="_blank">
-    <img src="https://img.shields.io/pypi/pyversions/pyventus?color=blue" alt="Supported Python versions">
+    <img src="https://img.shields.io/pypi/pyversions/pyventus?color=0097a8" alt="Supported Python versions">
 </a>
 
 <a href="https://github.com/psf/black">
 	<img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style: black">
 </a>
 
 </p>
 
 <br>
 
-
 ---
 
 **Documentation**: <a href="https://mdapena.github.io/pyventus" target="_blank">https://mdapena.github.io/pyventus</a>
 
 **Source Code**: <a href="https://github.com/mdapena/pyventus" target="_blank">https://github.com/mdapena/pyventus</a>
 
 ---
 
-<p style='text-align: justify;'>
-    &emsp;&emsp;Pyventus is a modern and robust Python package for event-driven programming. It offers a comprehensive
-	suite of tools to easily define, emit, and orchestrate events using customizable event emitters and flexible
-	responses. With Pyventus, you can easily build scalable, extensible, and loosely-coupled event-driven applications.
+<p style='text-align: justify;' markdown>
+    &emsp;&emsp;Pyventus is a powerful Python package for event-driven programming. It offers a comprehensive suite
+	of tools to easily define, emit, and orchestrate events. With Pyventus, you can build scalable, extensible, and
+	loosely-coupled event-driven applications.
 </p>
 
-## More than just Events
+[//]: # (--------------------------------------------------------------------------------------------------------------)
 
-<p style='text-align: justify;'>
-	Pyventus offers several key features that make it a powerful event-driven programming package for your 
-	Python projects:
-</p> 
+## Key Features
 
-<ul style='text-align: justify;'>
+<p style='text-align: justify;' markdown>
+    Pyventus offers several key features, such as:
+</p>
 
-<li><b>An Intuitive API</b> ─ 
-Pyventus provides a user-friendly API for defining events, emitters, and handlers. Its design simplifies the process
-of working with events, enabling you to organize your code around discrete events and their associated actions.
-</li>
+<ul style='text-align: justify;'>
 
 <li><b>Sync and Async Support</b> ─ 
 Whether your code is synchronous or asynchronous, Pyventus allows you to define event handlers as either sync or async
 callbacks and emit events from both scopes. 
 </li>
 
-<li><b>Runtime Flexibility</b> ─ 
-Pyventus' runtime flexibility allows you to switch seamlessly between different official or custom event emitter
-implementations on the fly.
-</li>
-
 <li><b>Customization</b> ─ 
 Whether you choose official emitters or custom ones, Pyventus allows you to customize the behavior and capabilities of
 the event emitters to perfectly align with your unique requirements.
 </li>
 
+<li><b>An Intuitive API</b> ─ 
+Pyventus provides a user-friendly API for defining events, emitters, and handlers. Its design simplifies the process
+of working with events, enabling you to organize your code around discrete events and their associated actions.
+</li>
+
+<li><b>Runtime Flexibility</b> ─ 
+Pyventus' runtime flexibility allows you to switch seamlessly between different built-in or custom event emitter
+implementations on the fly, providing a dynamic and adaptable environment for event-driven programming.
+</li>
+
 <li><b>Reliable Event Handling</b> ─ 
 Pyventus allows you to define handlers to customize how events are processed upon completion. Attach success and
 failure logic to take targeted actions based on the outcome of each event execution. 
 </li>
 
 <li><b>Scalability and Maintainability</b> ─ 
 By adopting an event-driven approach with Pyventus, you can create scalable and maintainable code thanks to the loose
 coupling between its components that enables extensibility and modularity.
 </li>
 
 <li><b>Comprehensive Documentation</b> ─ 
-Pyventus provides a comprehensive documentation suite that includes API references, usage examples, best practices
-guides, and tutorials to effectively leverage all the features and capabilities of the package.
+Pyventus provides a comprehensive documentation suite that includes API references, usage examples, and tutorials to
+effectively leverage all the features and capabilities of the package.
 </li>
 
 </ul>
 
-## Requirements
-
-<p style='text-align: justify;'>
-	&emsp;&emsp;Pyevents <b>only requires Python 3.10+</b> by default, which includes the 
-	<a href="https://mdapena.github.io/pyventus/tutorials/emitters/asyncio" target="_blank"><code>AsyncIOEventEmitter</code></a>
-	and the <a href="https://mdapena.github.io/pyventus/tutorials/emitters/executor" target="_blank"><code>ExecutorEventEmitter</code></a> 
-	with no additional dependencies. However, your requirements may expand if you opt to use  
-	<a href="https://mdapena.github.io/pyventus/getting-started/#optional-dependencies" target="_blank">alternative built-in event emitter implementations</a>.
-</p>
+[//]: # (--------------------------------------------------------------------------------------------------------------)
 
-## Installation
+## Quick Start
 
 <p style='text-align: justify;'>
-	&emsp;&emsp;Pyventus is available as a Python package and can be easily installed using <code>pip</code>. Open your terminal
-	and execute the following command to install it:
+	&emsp;&emsp;Pyventus is published as a <a href="https://pypi.org/project/pyventus/" target="_blank">Python package</a> 
+	and can be installed using <code>pip</code>, ideally in a <a href="https://realpython.com/python-virtual-environments-a-primer/" target="_blank">virtual environment</a>
+	for proper dependency isolation. To get started, open up a terminal and install Pyventus with the following command:
 </p>
 
 ```console
 pip install pyventus
 ```
 
-## <code>Hello, World!</code> Example
+<p style='text-align: justify;'>
+	&emsp;&emsp;Pyventus by default relies on the Python standard library and <b>requires Python 3.10 or higher</b> with no 
+	additional dependencies. However, this package also includes alternative integrations to access additional features 
+	such as Redis Queue, Celery, and FastAPI. For more information on this matter, please refer to the 
+	<a href="https://mdapena.github.io/pyventus/getting-started/#optional-dependencies" target="_blank">Optional Dependencies</a>
+	section.
+</p>
+
+[//]: # (--------------------------------------------------------------------------------------------------------------)
+
+## A Simple Example
 
 <p style='text-align: justify;'>
-    &emsp;&emsp;Experience the power of Pyventus through a simple <code>Hello, World!</code> example that illustrates 
-	the core concepts and basic usage of the package. This example will walk you through the essential steps of 
-	creating an event handler and triggering events within your application.
+    &emsp;&emsp;Experience the power of Pyventus through a simple <code>Hello, World!</code> example that illustrates
+	the core concepts and basic usage of the package. By following this example, you’ll learn how to subscribe to events
+	and emit them within your application.
 </p>
 
-```Python title="Hello, World! example with Pyventus" linenums="1"
+```Python title="Hello, World! Example" linenums="1"
 from pyventus import EventLinker, EventEmitter, AsyncIOEventEmitter
 
 
-@EventLinker.on("MyEvent")
-def event_callback():
+@EventLinker.on("GreetEvent")
+def handle_greet_event():
     print("Hello, World!")
 
 
 event_emitter: EventEmitter = AsyncIOEventEmitter()
-event_emitter.emit("MyEvent")
+event_emitter.emit("GreetEvent")
 ```
 
 <details markdown="1" class="info">
 <summary>You can also work with <code>async</code> functions and contexts...</summary>
 
-```Python title="Hello, World! example with Pyventus (Async version)" linenums="1" hl_lines="5 14"
+```Python title="Hello, World! Example (Async version)" linenums="1" hl_lines="5"
 from pyventus import EventLinker, EventEmitter, AsyncIOEventEmitter
 
 
-@EventLinker.on("MyEvent")
-async def event_callback():
+@EventLinker.on("GreetEvent")
+async def handle_greet_event():
     print("Hello, World!")
 
 
 event_emitter: EventEmitter = AsyncIOEventEmitter()
-event_emitter.emit("MyEvent")
+event_emitter.emit("GreetEvent")
 ```
 
 </details>
 
 <p style='text-align: justify;'>
     &emsp;&emsp;As we can see from the <code>Hello, World!</code> example, Pyventus follows a simple and intuitive 
-	workflow for event-driven programming. Let's recap the essential steps involved:
+	workflow for defining and emitting events. Let's recap the essential steps involved:
 </p>
 
 <ol style='text-align: justify;'>
 
 <li>
-<b>Defining the event handler callback:</b> We defined the function <code>event_callback()</code> and used the 
-<code>@EventLinker.on()</code> decorator to associate it with the string event <code>MyEvent</code>. This decorator
-indicates that the function should be triggered when <code>MyEvent</code> occurs.
+<b>Importing Necessary Modules:</b> 
+We first imported the required modules from Pyventus,  which encompassed the <code>EventLinker</code>
+class, the <code>EventEmitter</code> interface, and the <code>AsyncIOEventEmitter</code> implementation.
+</li>
+
+<li>
+<b>Linking Events to Callbacks:</b> 
+Next, we used the <code>@EventLinker.on()</code> decorator to define and link the string event <code>GreetEvent</code> 
+to the function <code>handle_greet_event()</code>, which will print <i>'Hello, World!'</i> to the console whenever the
+<code>GreetEvent</code> is emitted.
 </li>
 
 <li>
-<b>Creating the event emitter instance:</b> We instantiated the <code>AsyncIOEventEmitter</code> class, which acts as 
-the event emitter responsible for dispatching events and invoking the associated event handler callbacks. It's important 
-to note that the event emitter used can be changed by any of the built-in or custom event emitter implementations.
+<b>Instantiating an Event Emitter:</b> 
+After that, and in order to trigger our event, we needed to create an instance of the event emitter class. While 
+<code>AsyncIOEventEmitter</code> was utilized, any <a href="https://mdapena.github.io/pyventus/getting-started/#optional-dependencies"><i>built-in</i></a>
+or custom implementation could be employed.
 </li>
 
 <li>
-<b>Emitting the event:</b> By utilizing the <code>emit()</code> method of the event emitter, we emitted the string 
-event <code>MyEvent</code>. This action subsequently execute the registered event handler callbacks, which in this case
-is the <code>event_callback()</code>.
+<b>Triggering the Event:</b>
+Finally, by using the <code>emit()</code> method of the event emitter instance, we were able to trigger the 
+<code>GreetEvent</code>, which resulted in the execution of the <code>handle_greet_event()</code> callback.
 </li>
 
 </ol>
 
 <p style='text-align: justify;'>
     &emsp;&emsp;Having gained a clear understanding of the workflow showcased in the <code>Hello, World!</code> example,
 	you are now well-equipped to explore more intricate event-driven scenarios and fully harness the capabilities of 
-	Pyventus in your own projects.
+	Pyventus in your own projects. For a deep dive into the package's functionalities, you can refer to the 
+	Pyventus <a href="https://mdapena.github.io/pyventus/tutorials" target="_blank">Tutorials</a> or 
+	<a href="https://mdapena.github.io/pyventus/api" target="_blank">API</a>.
+</p>
+
+[//]: # (--------------------------------------------------------------------------------------------------------------)
+
+## A Practical Example
+
+<p style='text-align: justify;'>
+    &emsp;&emsp;To showcase Pyventus' event-driven capabilities in a real-world scenario, we will explore a practical 
+	example of implementing a voltage sensor using an event-driven architecture (crucial for such scenarios). The 
+	purpose of this example is to create an efficient voltage sensor that can seamlessly handle real-time data 
+	and respond appropriately to specific voltage conditions.
+</p>
+
+
+<details markdown="1" class="quote" open>
+<summary>Example ─ Monitoring Voltage Levels Across Devices (Context)</summary>
+
+<a style="text-align: center" href="https://unsplash.com/photos/macro-photography-of-black-circuit-board-FO7JIlwjOtU?utm_content=creditShareLink&utm_medium=referral&utm_source=unsplash" target="_blank">
+	<img src="https://mdapena.github.io/pyventus/images/examples/practical-example-index.jpg" alt="Macro photography of black circuit board">
+</a>
+
+<p style='text-align: justify;'>
+	<i>&emsp;&emsp;A common aspect found in many systems is the need to monitor and respond to changes in sensor data.
+	Whether it's pressure sensors, temperature sensors, or other types, capturing and reacting to sensor data is crucial
+	for effective system operation. In our practical example, we will focus on a specific scenario: building a sensor 
+	system that monitors voltage levels across devices. The goal of our voltage sensor is to detect potential issues,
+	such as low or high voltage conditions, and respond appropriately in real-time.</i>
+</p>
+
+</details>
+
+
+<p style='text-align: justify;'>
+    &emsp;&emsp;To accomplish our goal, we will define a <code>VoltageSensor</code> class to read voltage levels and emit 
+	events based on predefined thresholds. We will create event handlers to respond to these events, performing actions 
+	such as activating eco-mode for low voltage or implementing high-voltage protection. Additionally, a shared event 
+	handler will provide general notifications for out-of-range voltage situations. The code example below illustrates 
+	the implementation of this system.
+</p>
+
+```Python title="Voltage Sensor System with Pyventus (Practical Example)" linenums="1" hl_lines="9 14 27-30 35-36 41-42 47-48 55"
+import asyncio
+import random
+
+from pyventus import EventEmitter, EventLinker, AsyncIOEventEmitter
+
+
+class VoltageSensor:
+
+    def __init__(self, name: str, low: float, high: float, event_emitter: EventEmitter) -> None:
+        # Initialize the VoltageSensor object with the provided parameters
+        self._name: str = name
+        self._low: float = low
+        self._high: float = high
+        self._event_emitter: EventEmitter = event_emitter
+
+    async def __call__(self) -> None:
+        # Start voltage readings for the sensor
+        print(f"Starting voltage readings for: {self._name}")
+        print(f"Low: {self._low:.3g}v | High: {self._high:.3g}v\n-----------\n")
+
+        while True:
+            # Simulate sensor readings
+            voltage: float = random.uniform(0, 5)
+            print("\tSensor Reading:", "\033[32m", f"{voltage:.3g}v", "\033[0m")
+
+            # Emit events based on voltage readings
+            if voltage < self._low:
+                self._event_emitter.emit("LowVoltageEvent", sensor=self._name, voltage=voltage)
+            elif voltage > self._high:
+                self._event_emitter.emit("HighVoltageEvent", sensor=self._name, voltage=voltage)
+
+            await asyncio.sleep(1)
+
+
+@EventLinker.on("LowVoltageEvent")
+def handle_low_voltage_event(sensor: str, voltage: float):
+    print(f"🪫 Turning on eco-mode for '{sensor}'. ({voltage:.3g}v)\n")
+    # Perform action for low voltage...
+
+
+@EventLinker.on("HighVoltageEvent")
+async def handle_high_voltage_event(sensor: str, voltage: float):
+    print(f"⚡ Starting high-voltage protection for '{sensor}'. ({voltage:.3g}v)\n")
+    # Perform action for high voltage...
+
+
+@EventLinker.on("LowVoltageEvent", "HighVoltageEvent")
+def handle_voltage_event(sensor: str, voltage: float):
+    print(f"\033[31m\nSensor '{sensor}' out of range.\033[0m (Voltage: {voltage:.3g})")
+    # Perform notification for out of range voltage...
+
+
+async def main():
+    # Initialize the sensor and run the sensor readings
+    sensor = VoltageSensor(name="PressureSensor", low=0.5, high=3.9, event_emitter=AsyncIOEventEmitter())
+    await asyncio.gather(sensor(), )  # Add new sensors inside the 'gather' for multi-device monitoring
+
+
+asyncio.run(main())
+```
+
+<p style='text-align: justify;'>
+    &emsp;&emsp;As we can see from this practical example, Pyventus enables us to easily build an event-driven system 
+	for voltage sensors that is flexible, efficient, and highly responsive. With its intuitive API and support for both
+	synchronous and asynchronous operations, we were able to effectively monitor voltage levels, detect anomalies, and 
+	trigger appropriate actions in real-time.
 </p>
 
-## Support for Synchronous and Asynchronous code
+[//]: # (--------------------------------------------------------------------------------------------------------------)
+
+## Support for Synchronous and Asynchronous Code
 
 <p style='text-align: justify;'>
     &emsp;&emsp;Pyventus is designed from the ground up to seamlessly support both synchronous and asynchronous
-	programming models. Its unified sync/async API allows you to define event handler callbacks and emit events
-	across <code>sync</code> and <code>async</code> contexts. Let's take a look at some use cases that illustrate 
-	how the API handles event registration and dispatch transparently.
+	programming models. Its unified sync/async API allows you to define event callbacks and emit events across 
+	<code>sync</code> and <code>async</code> contexts.
 </p>
 
-### Registering Event Handlers as <code>Sync</code> and <code>Async</code> Callbacks
+### Subscribing Event Handlers with <code>Sync</code> and <code>Async</code> Callbacks
 
-```Python 
+```Python linenums="1" hl_lines="2 7"
 @EventLinker.on("MyEvent")
 def sync_event_callback():
-    # Synchronous event handling
-    print("Event received!")
+    pass  # Synchronous event handling
 
 
 @EventLinker.on("MyEvent")
 async def async_event_callback():
-    # Asynchronous event handling
-    print("Event received!")  
+	pass  # Asynchronous event handling
+```
+
+<details markdown="1" class="info">
+<summary>You can optimize the execution of your callbacks based on their workload...</summary>
+
+<p style='text-align: justify;'>
+    &emsp;&emsp;By default, event handlers in Pyventus are executed concurrently during an event emission, running their
+	<code>sync</code> and <code>async</code> callbacks as defined. However, if you have a <code>sync</code> callback
+	that involves I/O or non-CPU bound operations, you can enable the <code>force_async</code> parameter to offload it
+	to a thread pool, ensuring optimal performance and responsiveness. The <code>force_async</code> parameter utilizes 
+	the <a href="https://docs.python.org/3/library/asyncio-task.html#running-in-threads" target="_blank"><code>asyncio.to_thread()</code></a>
+	function to execute <code>sync</code> callbacks asynchronously.
+</p>
+
+```Python linenums="1" hl_lines="1"
+@EventLinker.on("BlockingIO", force_async=True)
+def blocking_io():
+    print(f"start blocking_io at {time.strftime('%X')}")
+    # Note that time.sleep() can be replaced with any blocking
+    # IO-bound operation, such as file operations.
+    time.sleep(1)
+    print(f"blocking_io complete at {time.strftime('%X')}")
 ```
 
+</details>
+
 ### Emitting Events from <code>Sync</code> and <code>Async</code> Contexts
 
-```Python 
+```Python linenums="1" hl_lines="3 8"
 # Emitting an event within a sync function
 def sync_function(event_emitter: EventEmitter):
     event_emitter.emit("MyEvent")
 
 
 # Emitting an event within an async function
 async def async_function(event_emitter: EventEmitter):
     event_emitter.emit("MyEvent")
 ```
 
-<details markdown="1" class="info" open>
-<summary>Event Propagation Within Different Contexts</summary>
+<details markdown="1" class="info">
+<summary>Event propagation within different contexts...</summary>
 
 <p style='text-align: justify;'>
     &emsp;&emsp;While Pyventus provides a base <code>EventEmitter</code> class with a unified sync/async API, the 
 	specific propagation behavior when emitting events may vary depending on the concrete <code>EventEmitter</code>
 	used. For example, the <code>AsyncIOEventEmitter</code> implementation leverages the <code>AsyncIO</code> event
 	loop to schedule callbacks added from asynchronous contexts without blocking. But alternative emitters could 
 	structure propagation differently to suit their needs.
 </p>
 
 </details>
 
+[//]: # (--------------------------------------------------------------------------------------------------------------)
+
 ## Runtime Flexibility and Customization
 
 <p style='text-align: justify;'>
     &emsp;&emsp;At its core, Pyventus utilizes a modular event emitter design that allows you to switch seamlessly
-	between different built-in or custom event emitter implementations on the fly. Whether you opt for official
-	emitters or decide to create your custom ones, Pyventus allows you to tailor the behavior and capabilities
-	of the event emitters to perfectly align with your unique requirements.
-</p>
-
-<p style='text-align: justify;'>
-    &emsp;&emsp;By leveraging the principles of dependency inversion and open-close, Pyventus decouples the event
-	emission process from the underlying implementation that handles the event emission and enables you, in conjunction
-	with the <code>EventLinker</code>, to change the event emitter at runtime without the need to reconfigure all 
-	connections or employ complex logic.
+	between different <a href="https://mdapena.github.io/pyventus/getting-started/#optional-dependencies"><i>built-in</i></a>
+	or custom event emitter implementations on the fly. Whether you opt for official emitters or decide to create your 
+	custom ones, Pyventus allows you to tailor the behavior and capabilities of the event emitters to perfectly align 
+	with your unique requirements.
 </p>
 
-### Seeing it in Action
+### Swapping Event Emitter Implementations at Runtime
 
 <p style='text-align: justify;'>
-    &emsp;&emsp;Now let's put Pyventus' flexibility to the test with a practical example. First, we'll build a
-	custom <a href="https://fastapi.tiangolo.com/" target="_blank">FastAPI</a> EventEmitter to properly handle
-	the event emission using the framework's <a href="https://fastapi.tiangolo.com/reference/background/" target="_blank">BackgroundTasks</a>
-	workflow. Then, we'll illustrate Pyventus' dynamic capabilities by swapping this custom emitter out for a built-in
-	alternative on the fly.
+    &emsp;&emsp;By leveraging the principle of dependency inversion and using the base <code>EventEmitter</code> as a
+	dependency, you can change the concrete implementation on the fly. Let's demonstrate this using the AsyncIO 
+	Event Emitter and the Executor Event Emitter: 
 </p>
 
-<p style='text-align: justify;'>
-    &emsp;&emsp;To follow along, please ensure that you have the FastAPI framework <a href="https://fastapi.tiangolo.com/?h=#installation" target="_blank">installed</a>. 
-	Once that is complete, let's dive into the step-by-step implementation:
-</p>
-
-<ol style='text-align: justify;'>
-
-<li>
-Create a <code>main.py</code> file with:
-
-```Python title="main.py" linenums="1"  hl_lines="9 16-17 37 40"
-from asyncio import sleep
-from random import randint
-
-from fastapi import BackgroundTasks, FastAPI
+```Python title="Event Emitter Runtime Flexibility Example" linenums="1" hl_lines="10-11 14 16"
+from pyventus import EventLinker, EventEmitter, AsyncIOEventEmitter, ExecutorEventEmitter
 
-from pyventus import EventEmitter, EventLinker, AsyncIOEventEmitter
 
+@EventLinker.on("GreetEvent")
+def handle_greet_event(name: str = "World"):
+    print(f"Hello, {name}!")
 
-class FastAPIEventEmitter(EventEmitter):
-    """Custom event emitter class that leverages the FastAPI's asynchronous workflow."""
 
-    def __init__(self, background_tasks: BackgroundTasks):
-        super().__init__()
-        self._background_tasks = background_tasks  # Store the FastAPI background tasks object
-
-    def _process(self, event_emission: EventEmitter.EventEmission) -> None:
-        self._background_tasks.add_task(event_emission)  # Execute the event emission as background tasks
+if __name__ == "__main__":
+    def main(event_emitter: EventEmitter) -> None:
+        event_emitter.emit("GreetEvent", name=type(event_emitter).__name__)
 
 
-@EventLinker.on("console_print")
-async def console_print(message: str):
-    await sleep(randint(0, 3))  # Simulate a random delay
-    print(message)
+    main(event_emitter=AsyncIOEventEmitter())
+    with ExecutorEventEmitter() as executor_event_emitter:
+        main(event_emitter=executor_event_emitter)
+```
 
+### Defining Custom Event Emitters
 
-app = FastAPI()
+<p style='text-align: justify;'>
+    &emsp;&emsp;To illustrate Pyventus' customization capabilities, we will define and implement a custom event emitter
+	class for the FastAPI framework. This class will efficiently handle the execution of event emissions through its 
+	<a href="https://fastapi.tiangolo.com/reference/background/" target="_blank">background tasks</a> workflow.
+</p>
 
+```Python title="Custom Event Emitter Example" linenums="1" hl_lines="6 10-11 13-14"
+from fastapi import BackgroundTasks
 
-@app.get("/print")
-async def console_print_endpoint(background_tasks: BackgroundTasks):
-    """FastAPI endpoint that triggers the console_print event."""
+from pyventus import EventEmitter, EventLinker
 
-    def console_print_app_service(event_emitter: EventEmitter) -> None:
-        event_emitter.emit("console_print", message=f"\nHello, {event_emitter.__class__.__name__}!")
 
-    # Emit the console_print event using FastAPIEventEmitter
-    console_print_app_service(event_emitter=FastAPIEventEmitter(background_tasks))
+class FastAPIEventEmitter(EventEmitter):
+    """A custom event emitter that uses the FastAPI background tasks."""
 
-    # Emit the console_print event using AsyncIOEventEmitter
-    console_print_app_service(event_emitter=AsyncIOEventEmitter())
+    def __init__(self, background_tasks: BackgroundTasks):
+        super().__init__(event_linker=EventLinker, debug=False)
+        self._background_tasks = background_tasks
 
-    return {"message": "Console print triggered!"}
+    def _process(self, event_emission: EventEmitter.EventEmission) -> None:
+        self._background_tasks.add_task(event_emission)  # Process the event emission as a background task
 ```
 
-</li> 
-
+<details markdown="1" class="tip">
+<summary>Official <code>FastAPIEventEmitter</code> Integration.</summary>
 
+<p style='text-align: justify;'>
+    In case you're interested in integrating Pyventus with FastAPI, you can refer to the official Pyventus 
+	<a href="https://mdapena.github.io/pyventus/tutorials/emitters/fastapi/"><i>FastAPI Event Emitter</i></a> 
+	implementation.
+</p>
 
-<li>
-<a href="https://fastapi.tiangolo.com/#run-it" target="_blank">Run the server</a> with:
+</details>
 
-```console
-uvicorn main:app --reload
-```
+[//]: # (--------------------------------------------------------------------------------------------------------------)
 
-</li>
+## Event Objects and Global Events
 
-<li>
-Open your browser at <a href="http://127.0.0.1:8000/print" target="_blank">http://127.0.0.1:8000/print</a>. You will 
-see the JSON response as:
+<p style='text-align: justify;'>
+    &emsp;&emsp;In addition to string events, Pyventus also supports Event Objects, which provide a structured way to 
+	define events and encapsulate relevant data payloads.
+</p>
 
-```JSON
-{ "message": "Console print triggered!" }
-```
+```Python title="Event Object Example" linenums="1" hl_lines="1-2 7-8 16-19"
+@dataclass  # Define a Python dataclass representing the event and its payload.
+class OrderCreatedEvent:
+    order_id: int
+    payload: dict[str, any]
 
-You'll also be able to see the outputs of the event emitters in the console logs as:
 
-```console
-INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
-INFO:     Started reloader process [28720]
-INFO:     Started server process [28722]
-INFO:     Waiting for application startup.
-INFO:     Application startup complete.
-INFO:     127.0.0.1:52391 - "GET /print HTTP/1.1" 200 OK
+@EventLinker.on(OrderCreatedEvent)  # Subscribe event handlers to the event.
+def handle_order_created_event(event: OrderCreatedEvent):
+    # Pyventus will automatically pass the Event Object 
+    # as the first positional argument.
+    print(f"Event Object: {event}")
 
-Hello, FastAPIEventEmitter!
 
-Hello, AsyncIOEventEmitter!
+event_emitter: EventEmitter = AsyncIOEventEmitter()
+event_emitter.emit(
+    event=OrderCreatedEvent(  # Emit an instance of the event!
+        order_id=6452879,
+        payload={},
+    ),
+)
 ```
 
-</li>
-
-</ol> 
-
 <p style='text-align: justify;'>
-    &emsp;&emsp;As we can see from this practical example, we were able to easily adapt the event emitter to the
-	context of the FastAPI framework. We defined and implemented a custom emitter tailored for FastAPI's workflow,
-	using background tasks to handle the event emission accordingly.
+    &emsp;&emsp;Furthermore, Pyventus provides support for Global Events, which are particularly useful for 
+	implementing cross-cutting concerns such as logging, monitoring, or analytics. By subscribing event handlers to
+	<code>...</code> or <code>Ellipsis</code>, you can capture all events that may occur within that 
+	<code>EventLinker</code> context.
 </p>
 
-<p style='text-align: justify;'>
-    &emsp;&emsp;We also saw Pyventus' dynamic flexibility firsthand - swapping emitters in real-time required no
-	intricate reconfiguration or re-establishing of handlers. Simply changing the concrete emitter allowed for
-	a seamless transition between implementations.
-</p>
+```Python title="Global Event Example" linenums="1" hl_lines="1"
+@EventLinker.on(...)
+def handle_any_event(*args, **kwargs):
+    print(f"Perform logging...\nArgs: {args}\tKwargs: {kwargs}")
 
-<details markdown="1" class="tip" open>
-<summary>Official <code>FastAPIEventEmitter</code> integration</summary>
-<p style='text-align: justify;'>
-No need for manual implementation! Pyventus now offers an official <b><a href="https://mdapena.github.io/pyventus/tutorials/emitters/fastapi">FastAPIEventEmitter</a></b>
-integration.
-</p>
-</details>
 
-## Defining Event Response Logic
+event_emitter: EventEmitter = AsyncIOEventEmitter()
+event_emitter.emit("GreetEvent", name="Pyventus")
+```
 
-<p style='text-align: justify;'>
-    &emsp;&emsp;As we mentioned earlier, Pyventus allows you to customize how events are processed upon completion in
-	success or error scenarios by attaching custom handlers. To utilize this functionality, Pyventus provides a simple
-	yet powerful Pythonic syntax through its <code>event linkage context</code>.
-</p>
+[//]: # (--------------------------------------------------------------------------------------------------------------)
+
+## Success and Error Handling
 
 <p style='text-align: justify;'>
-    &emsp;&emsp;The <code>event linkage context</code> enables defining the event workflow and completion handlers in an
-	organized manner. This is done by using the <code>EventLinker.on</code> method within a <code>with</code> statement
-	block. Let's examine examples demonstrating how success and failure handlers can be attached using the event linkage
-	context:
+    &emsp;&emsp;With Pyventus, you can customize how events are handled upon completion, whether they succeed or 
+	encounter errors. This customization is achieved by using either the EventLinker's <code>on()</code> or 
+	<code>once()</code> decorator within a <code>with</code> statement block. Inside this block, you can 
+	define not only the event callbacks but also the overall workflow of the event. Now, let’s explore 
+	this simple yet powerful Pythonic syntax of Pyventus through an example.
 </p>
 
-### Success and Error Handling Example
-
-```Python linenums="1"  hl_lines="7 10-12"
+```Python title="Success and Error Handling Example" linenums="1" hl_lines="4 6-7 10-11 14-15"
 from pyventus import EventLinker, EventEmitter, AsyncIOEventEmitter
 
-
-with EventLinker.on("StringEvent") as linker:
-	
+# Create an event linker for the "DivisionEvent"
+with EventLinker.on("DivisionEvent") as linker:
     @linker.on_event
-    def event_callback() -> str:
-        print("Event received!")
-        return "Event succeeded!"
+    def divide(a: float, b: float) -> float:
+        return a / b
 
     @linker.on_success
-    def success_callback(msg: str) -> None:
-        print(msg)
+    def handle_success(result: float) -> None:
+        print(f"Division result: {result:.3g}")
 
     @linker.on_failure
-    def failure_callback(exc: Exception) -> None:
-        print(exc)
+    def handle_failure(e: Exception) -> None:
+        print(f"Oops, something went wrong: {e}")
 
-	    
-event_emitter: EventEmitter = AsyncIOEventEmitter()
-event_emitter.emit("StringEvent")
+event_emitter: EventEmitter = AsyncIOEventEmitter()  # Create an event emitter
+event_emitter.emit("DivisionEvent", a=1, b=0)  # Example: Division by zero
+event_emitter.emit("DivisionEvent", a=1, b=2)  # Example: Valid division
 ```
 
 <p style='text-align: justify;'>
-    &emsp;&emsp;As we have seen from the examples, Pyventus' event linkage context provides a reliable and Pythonic way
-	to manage the event workflow and response to different completion outcomes through the use of custom handlers.
+    &emsp;&emsp;As we have seen from the example, Pyventus offers a reliable and Pythonic solution for customizing 
+	event handling. By utilizing the EventLinker and its decorators within a <code>with</code> statement block, we
+	were able to define the <code>DivisionEvent</code> and specify the callbacks for division, success, and failure
+	cases.
 </p>
 
+[//]: # (--------------------------------------------------------------------------------------------------------------)
+
 ## Continuous Evolution
 
 <p style='text-align: justify;'>
 	&emsp;&emsp;Pyventus continuously adapts to support developers across technological and programming domains. Its
 	aim is to remain at the forefront of event-driven design. Future development may introduce new official event 
 	emitters, expanding compatibility with different technologies through seamless integration.
+</p>
 
 <p style='text-align: justify;'>
 	&emsp;&emsp;Current default emitters provide reliable out-of-the-box capabilities for common use cases. They
 	efficiently handle core event operations and lay the foundation for building event-driven applications.
 </p>
 
 <details markdown="1" class="info">
 <summary>Driving Innovation Through Collaboration</summary>
 
 <p style='text-align: justify;'>
     &emsp;&emsp;Pyventus is an open source project that welcomes community involvement. If you wish to contribute
-	additional event emitters, improvements, or bug fixes, please check the <a href="https://mdapena.github.io/pyventus/contributing/">Contributing</a> section
-	for guidelines on collaborating. Together, we can further the possibilities of event-driven development.
+	additional event emitters, improvements, or bug fixes, please check the <a href="https://mdapena.github.io/pyventus/contributing/" target="_blank">Contributing</a> 
+	section for guidelines on collaborating. Together, we can further the possibilities of event-driven development.
 </p>
 
 </details>
 
+[//]: # (--------------------------------------------------------------------------------------------------------------)
+
 ## License
 
 <p style='text-align: justify;' markdown>
     &emsp;&emsp;Pyventus is distributed as open source software and is released under the <a href="https://choosealicense.com/licenses/mit/" target="_blank">MIT License</a>. 
     You can view the full text of the license in the <a href="https://github.com/mdapena/pyventus/blob/master/LICENSE" target="_blank"><code>LICENSE</code></a> 
 	file located in the Pyventus repository.
 </p>
-
```

### Comparing `pyventus-0.4.1/pyproject.toml` & `pyventus-0.5.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # ------------------------------------------------------------------
 # | Project                                                        |
 # ------------------------------------------------------------------
 
 [project]
 name = "pyventus"
 dynamic = ["version"]
-description = "A modern and robust Python package for event-driven programming. Define, emit, and orchestrate events with ease using customizable event emitters and flexible responses."
+description = "A powerful Python package for event-driven programming; define, emit, and orchestrate events with ease."
 requires-python = ">=3.10"
 readme = "README.md"
 license = "MIT"
 authors = [
     { name = "Manuel Da Pena", email = "dapensoft@gmail.com" },
 ]
 keywords = ["events", "event-emitters", "event-dispatchers", "event-handlers", "event-linkers", "event-driven", "python"]
@@ -59,18 +59,19 @@
 ]
 
 # --------------------
 # | Docs dependencies
 # ----------
 
 docs = [
-    "mkdocs-material>=9.4.0",
+    "mkdocs-material>=9.5.17",
     "mkdocstrings[python]>=0.24.0",
     "mkdocs-git-revision-date-localized-plugin>=1.2.1",
-    "mkdocs-git-authors-plugin>=0.7.2",
+    "mkdocs-git-committers-plugin-2>=2.3.0",
+    "mkdocs-material[imaging]",
 ]
 
 # --------------------
 # | Tests dependencies
 # ----------
 
 tests = [
```

### Comparing `pyventus-0.4.1/PKG-INFO` & `pyventus-0.5.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,1278 +1,1729 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 7079 7665  : 2.1.Name: pyve
+00000010: 3a20 322e 330a 4e61 6d65 3a20 7079 7665  : 2.3.Name: pyve
 00000020: 6e74 7573 0a56 6572 7369 6f6e 3a20 302e  ntus.Version: 0.
-00000030: 342e 310a 5375 6d6d 6172 793a 2041 206d  4.1.Summary: A m
-00000040: 6f64 6572 6e20 616e 6420 726f 6275 7374  odern and robust
-00000050: 2050 7974 686f 6e20 7061 636b 6167 6520   Python package 
-00000060: 666f 7220 6576 656e 742d 6472 6976 656e  for event-driven
-00000070: 2070 726f 6772 616d 6d69 6e67 2e20 4465   programming. De
-00000080: 6669 6e65 2c20 656d 6974 2c20 616e 6420  fine, emit, and 
-00000090: 6f72 6368 6573 7472 6174 6520 6576 656e  orchestrate even
-000000a0: 7473 2077 6974 6820 6561 7365 2075 7369  ts with ease usi
-000000b0: 6e67 2063 7573 746f 6d69 7a61 626c 6520  ng customizable 
-000000c0: 6576 656e 7420 656d 6974 7465 7273 2061  event emitters a
-000000d0: 6e64 2066 6c65 7869 626c 6520 7265 7370  nd flexible resp
-000000e0: 6f6e 7365 732e 0a50 726f 6a65 6374 2d55  onses..Project-U
-000000f0: 524c 3a20 486f 6d65 7061 6765 2c20 6874  RL: Homepage, ht
-00000100: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000110: 2f6d 6461 7065 6e61 2f70 7976 656e 7475  /mdapena/pyventu
-00000120: 730a 5072 6f6a 6563 742d 5552 4c3a 2044  s.Project-URL: D
-00000130: 6f63 756d 656e 7461 7469 6f6e 2c20 6874  ocumentation, ht
-00000140: 7470 733a 2f2f 6d64 6170 656e 612e 6769  tps://mdapena.gi
-00000150: 7468 7562 2e69 6f2f 7079 7665 6e74 7573  thub.io/pyventus
-00000160: 0a50 726f 6a65 6374 2d55 524c 3a20 5265  .Project-URL: Re
-00000170: 706f 7369 746f 7279 2c20 6874 7470 733a  pository, https:
-00000180: 2f2f 6769 7468 7562 2e63 6f6d 2f6d 6461  //github.com/mda
-00000190: 7065 6e61 2f70 7976 656e 7475 730a 5072  pena/pyventus.Pr
-000001a0: 6f6a 6563 742d 5552 4c3a 2043 6861 6e67  oject-URL: Chang
-000001b0: 656c 6f67 2c20 6874 7470 733a 2f2f 6d64  elog, https://md
-000001c0: 6170 656e 612e 6769 7468 7562 2e69 6f2f  apena.github.io/
-000001d0: 7079 7665 6e74 7573 2f72 656c 6561 7365  pyventus/release
-000001e0: 2d6e 6f74 6573 0a41 7574 686f 722d 656d  -notes.Author-em
-000001f0: 6169 6c3a 204d 616e 7565 6c20 4461 2050  ail: Manuel Da P
-00000200: 656e 6120 3c64 6170 656e 736f 6674 4067  ena <dapensoft@g
-00000210: 6d61 696c 2e63 6f6d 3e0a 4c69 6365 6e73  mail.com>.Licens
-00000220: 652d 4578 7072 6573 7369 6f6e 3a20 4d49  e-Expression: MI
-00000230: 540a 4c69 6365 6e73 652d 4669 6c65 3a20  T.License-File: 
-00000240: 4c49 4345 4e53 450a 4b65 7977 6f72 6473  LICENSE.Keywords
-00000250: 3a20 6576 656e 742d 6469 7370 6174 6368  : event-dispatch
-00000260: 6572 732c 6576 656e 742d 6472 6976 656e  ers,event-driven
-00000270: 2c65 7665 6e74 2d65 6d69 7474 6572 732c  ,event-emitters,
-00000280: 6576 656e 742d 6861 6e64 6c65 7273 2c65  event-handlers,e
-00000290: 7665 6e74 2d6c 696e 6b65 7273 2c65 7665  vent-linkers,eve
-000002a0: 6e74 732c 7079 7468 6f6e 0a43 6c61 7373  nts,python.Class
-000002b0: 6966 6965 723a 2049 6e74 656e 6465 6420  ifier: Intended 
-000002c0: 4175 6469 656e 6365 203a 3a20 4465 7665  Audience :: Deve
-000002d0: 6c6f 7065 7273 0a43 6c61 7373 6966 6965  lopers.Classifie
-000002e0: 723a 204c 6963 656e 7365 203a 3a20 4f53  r: License :: OS
-000002f0: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
-00000300: 5420 4c69 6365 6e73 650a 436c 6173 7369  T License.Classi
-00000310: 6669 6572 3a20 4f70 6572 6174 696e 6720  fier: Operating 
-00000320: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
-00000330: 6570 656e 6465 6e74 0a43 6c61 7373 6966  ependent.Classif
-00000340: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00000350: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000360: 686f 6e0a 436c 6173 7369 6669 6572 3a20  hon.Classifier: 
-00000370: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000380: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000390: 3a20 330a 436c 6173 7369 6669 6572 3a20  : 3.Classifier: 
-000003a0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000003b0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000003c0: 3a20 3320 3a3a 204f 6e6c 790a 436c 6173  : 3 :: Only.Clas
-000003d0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-000003e0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000003f0: 5079 7468 6f6e 203a 3a20 332e 3130 0a43  Python :: 3.10.C
-00000400: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-00000410: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000420: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
-00000430: 310a 436c 6173 7369 6669 6572 3a20 5072  1.Classifier: Pr
-00000440: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000450: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000460: 332e 3132 0a43 6c61 7373 6966 6965 723a  3.12.Classifier:
-00000470: 2054 6f70 6963 203a 3a20 536f 6674 7761   Topic :: Softwa
-00000480: 7265 2044 6576 656c 6f70 6d65 6e74 0a43  re Development.C
-00000490: 6c61 7373 6966 6965 723a 2054 6f70 6963  lassifier: Topic
-000004a0: 203a 3a20 536f 6674 7761 7265 2044 6576   :: Software Dev
-000004b0: 656c 6f70 6d65 6e74 203a 3a20 4c69 6272  elopment :: Libr
-000004c0: 6172 6965 730a 436c 6173 7369 6669 6572  aries.Classifier
-000004d0: 3a20 546f 7069 6320 3a3a 2053 6f66 7477  : Topic :: Softw
-000004e0: 6172 6520 4465 7665 6c6f 706d 656e 7420  are Development 
-000004f0: 3a3a 204c 6962 7261 7269 6573 203a 3a20  :: Libraries :: 
-00000500: 5079 7468 6f6e 204d 6f64 756c 6573 0a43  Python Modules.C
-00000510: 6c61 7373 6966 6965 723a 2054 7970 696e  lassifier: Typin
-00000520: 6720 3a3a 2054 7970 6564 0a52 6571 7569  g :: Typed.Requi
-00000530: 7265 732d 5079 7468 6f6e 3a20 3e3d 332e  res-Python: >=3.
-00000540: 3130 0a50 726f 7669 6465 732d 4578 7472  10.Provides-Extr
-00000550: 613a 2061 6c6c 0a52 6571 7569 7265 732d  a: all.Requires-
-00000560: 4469 7374 3a20 7079 7665 6e74 7573 5b63  Dist: pyventus[c
-00000570: 656c 6572 795d 3b20 6578 7472 6120 3d3d  elery]; extra ==
-00000580: 2027 616c 6c27 0a52 6571 7569 7265 732d   'all'.Requires-
-00000590: 4469 7374 3a20 7079 7665 6e74 7573 5b66  Dist: pyventus[f
-000005a0: 6173 7461 7069 5d3b 2065 7874 7261 203d  astapi]; extra =
-000005b0: 3d20 2761 6c6c 270a 5265 7175 6972 6573  = 'all'.Requires
-000005c0: 2d44 6973 743a 2070 7976 656e 7475 735b  -Dist: pyventus[
-000005d0: 7271 5d3b 2065 7874 7261 203d 3d20 2761  rq]; extra == 'a
-000005e0: 6c6c 270a 5072 6f76 6964 6573 2d45 7874  ll'.Provides-Ext
-000005f0: 7261 3a20 6365 6c65 7279 0a52 6571 7569  ra: celery.Requi
-00000600: 7265 732d 4469 7374 3a20 6365 6c65 7279  res-Dist: celery
-00000610: 3e3d 352e 332e 353b 2065 7874 7261 203d  >=5.3.5; extra =
-00000620: 3d20 2763 656c 6572 7927 0a50 726f 7669  = 'celery'.Provi
-00000630: 6465 732d 4578 7472 613a 2064 6576 0a52  des-Extra: dev.R
-00000640: 6571 7569 7265 732d 4469 7374 3a20 6861  equires-Dist: ha
-00000650: 7463 683e 3d31 2e38 2e31 3b20 6578 7472  tch>=1.8.1; extr
-00000660: 6120 3d3d 2027 6465 7627 0a52 6571 7569  a == 'dev'.Requi
-00000670: 7265 732d 4469 7374 3a20 7079 7665 6e74  res-Dist: pyvent
-00000680: 7573 5b64 6f63 735d 3b20 6578 7472 6120  us[docs]; extra 
-00000690: 3d3d 2027 6465 7627 0a52 6571 7569 7265  == 'dev'.Require
-000006a0: 732d 4469 7374 3a20 7079 7665 6e74 7573  s-Dist: pyventus
-000006b0: 5b74 6573 7473 5d3b 2065 7874 7261 203d  [tests]; extra =
-000006c0: 3d20 2764 6576 270a 5072 6f76 6964 6573  = 'dev'.Provides
-000006d0: 2d45 7874 7261 3a20 646f 6373 0a52 6571  -Extra: docs.Req
-000006e0: 7569 7265 732d 4469 7374 3a20 6d6b 646f  uires-Dist: mkdo
-000006f0: 6373 2d67 6974 2d61 7574 686f 7273 2d70  cs-git-authors-p
-00000700: 6c75 6769 6e3e 3d30 2e37 2e32 3b20 6578  lugin>=0.7.2; ex
-00000710: 7472 6120 3d3d 2027 646f 6373 270a 5265  tra == 'docs'.Re
-00000720: 7175 6972 6573 2d44 6973 743a 206d 6b64  quires-Dist: mkd
-00000730: 6f63 732d 6769 742d 7265 7669 7369 6f6e  ocs-git-revision
-00000740: 2d64 6174 652d 6c6f 6361 6c69 7a65 642d  -date-localized-
-00000750: 706c 7567 696e 3e3d 312e 322e 313b 2065  plugin>=1.2.1; e
-00000760: 7874 7261 203d 3d20 2764 6f63 7327 0a52  xtra == 'docs'.R
-00000770: 6571 7569 7265 732d 4469 7374 3a20 6d6b  equires-Dist: mk
-00000780: 646f 6373 2d6d 6174 6572 6961 6c3e 3d39  docs-material>=9
-00000790: 2e34 2e30 3b20 6578 7472 6120 3d3d 2027  .4.0; extra == '
-000007a0: 646f 6373 270a 5265 7175 6972 6573 2d44  docs'.Requires-D
-000007b0: 6973 743a 206d 6b64 6f63 7374 7269 6e67  ist: mkdocstring
-000007c0: 735b 7079 7468 6f6e 5d3e 3d30 2e32 342e  s[python]>=0.24.
-000007d0: 303b 2065 7874 7261 203d 3d20 2764 6f63  0; extra == 'doc
-000007e0: 7327 0a50 726f 7669 6465 732d 4578 7472  s'.Provides-Extr
-000007f0: 613a 2066 6173 7461 7069 0a52 6571 7569  a: fastapi.Requi
-00000800: 7265 732d 4469 7374 3a20 6661 7374 6170  res-Dist: fastap
-00000810: 693e 3d30 2e39 352e 323b 2065 7874 7261  i>=0.95.2; extra
-00000820: 203d 3d20 2766 6173 7461 7069 270a 5072   == 'fastapi'.Pr
-00000830: 6f76 6964 6573 2d45 7874 7261 3a20 7271  ovides-Extra: rq
-00000840: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000850: 7271 3e3d 312e 3135 2e30 3b20 6578 7472  rq>=1.15.0; extr
-00000860: 6120 3d3d 2027 7271 270a 5072 6f76 6964  a == 'rq'.Provid
-00000870: 6573 2d45 7874 7261 3a20 7465 7374 730a  es-Extra: tests.
-00000880: 5265 7175 6972 6573 2d44 6973 743a 2062  Requires-Dist: b
-00000890: 6c61 636b 3e3d 3233 2e31 322e 303b 2065  lack>=23.12.0; e
-000008a0: 7874 7261 203d 3d20 2774 6573 7473 270a  xtra == 'tests'.
-000008b0: 5265 7175 6972 6573 2d44 6973 743a 2063  Requires-Dist: c
-000008c0: 6f76 6572 6167 655b 746f 6d6c 5d3e 3d37  overage[toml]>=7
-000008d0: 2e33 2e33 3b20 6578 7472 6120 3d3d 2027  .3.3; extra == '
-000008e0: 7465 7374 7327 0a52 6571 7569 7265 732d  tests'.Requires-
-000008f0: 4469 7374 3a20 6661 6b65 7265 6469 733e  Dist: fakeredis>
-00000900: 3d32 2e32 302e 303b 2065 7874 7261 203d  =2.20.0; extra =
-00000910: 3d20 2774 6573 7473 270a 5265 7175 6972  = 'tests'.Requir
-00000920: 6573 2d44 6973 743a 2068 7474 7078 3e3d  es-Dist: httpx>=
-00000930: 302e 3233 2e30 3b20 6578 7472 6120 3d3d  0.23.0; extra ==
-00000940: 2027 7465 7374 7327 0a52 6571 7569 7265   'tests'.Require
-00000950: 732d 4469 7374 3a20 6d79 7079 3e3d 312e  s-Dist: mypy>=1.
-00000960: 372e 313b 2065 7874 7261 203d 3d20 2774  7.1; extra == 't
-00000970: 6573 7473 270a 5265 7175 6972 6573 2d44  ests'.Requires-D
-00000980: 6973 743a 2070 7974 6573 742d 6173 796e  ist: pytest-asyn
-00000990: 6369 6f3e 3d30 2e32 312e 303b 2065 7874  cio>=0.21.0; ext
-000009a0: 7261 203d 3d20 2774 6573 7473 270a 5265  ra == 'tests'.Re
-000009b0: 7175 6972 6573 2d44 6973 743a 2070 7974  quires-Dist: pyt
-000009c0: 6573 743e 3d37 2e34 2e30 3b20 6578 7472  est>=7.4.0; extr
-000009d0: 6120 3d3d 2027 7465 7374 7327 0a52 6571  a == 'tests'.Req
-000009e0: 7569 7265 732d 4469 7374 3a20 7079 7665  uires-Dist: pyve
-000009f0: 6e74 7573 5b61 6c6c 5d3b 2065 7874 7261  ntus[all]; extra
-00000a00: 203d 3d20 2774 6573 7473 270a 4465 7363   == 'tests'.Desc
-00000a10: 7269 7074 696f 6e2d 436f 6e74 656e 742d  ription-Content-
-00000a20: 5479 7065 3a20 7465 7874 2f6d 6172 6b64  Type: text/markd
-00000a30: 6f77 6e0a 0a3c 6272 3e0a 0a3c 7020 616c  own..<br>..<p al
-00000a40: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
-00000a50: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
-00000a60: 3a2f 2f6d 6461 7065 6e61 2e67 6974 6875  ://mdapena.githu
-00000a70: 622e 696f 2f70 7976 656e 7475 732f 696d  b.io/pyventus/im
-00000a80: 6167 6573 2f6c 6f67 6f2f 7079 7665 6e74  ages/logo/pyvent
-00000a90: 7573 2d6c 6f67 6f2d 6e61 6d65 2d73 6c6f  us-logo-name-slo
-00000aa0: 6761 6e2e 7376 6722 2061 6c74 3d22 5079  gan.svg" alt="Py
-00000ab0: 7665 6e74 7573 2220 7769 6474 683d 2237  ventus" width="7
-00000ac0: 3530 7078 223e 0a3c 2f70 3e0a 0a3c 6272  50px">.</p>..<br
-00000ad0: 3e0a 0a3c 7020 616c 6967 6e3d 2263 656e  >..<p align="cen
-00000ae0: 7465 7222 3e0a 0a3c 6120 6872 6566 3d22  ter">..<a href="
-00000af0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000b00: 6f6d 2f6d 6461 7065 6e61 2f70 7976 656e  om/mdapena/pyven
-00000b10: 7475 732f 6163 7469 6f6e 733f 7175 6572  tus/actions?quer
-00000b20: 793d 776f 726b 666c 6f77 2533 4154 6573  y=workflow%3ATes
-00000b30: 7473 2b65 7665 6e74 2533 4170 7573 682b  ts+event%3Apush+
-00000b40: 6272 616e 6368 2533 416d 6173 7465 7222  branch%3Amaster"
-00000b50: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
-00000b60: 3e0a 2020 2020 3c69 6d67 2073 7263 3d22  >.    <img src="
-00000b70: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000b80: 6f6d 2f6d 6461 7065 6e61 2f70 7976 656e  om/mdapena/pyven
-00000b90: 7475 732f 6163 7469 6f6e 732f 776f 726b  tus/actions/work
-00000ba0: 666c 6f77 732f 7275 6e2d 7465 7374 732e  flows/run-tests.
-00000bb0: 796d 6c2f 6261 6467 652e 7376 673f 6272  yml/badge.svg?br
-00000bc0: 616e 6368 3d6d 6173 7465 7222 2061 6c74  anch=master" alt
-00000bd0: 3d22 5465 7374 7322 3e0a 3c2f 613e 0a0a  ="Tests">.</a>..
-00000be0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00000bf0: 2f67 6974 6875 622e 636f 6d2f 6d64 6170  /github.com/mdap
-00000c00: 656e 612f 7079 7665 6e74 7573 2f61 6374  ena/pyventus/act
-00000c10: 696f 6e73 3f71 7565 7279 3d77 6f72 6b66  ions?query=workf
-00000c20: 6c6f 7725 3341 446f 6373 2b65 7665 6e74  low%3ADocs+event
-00000c30: 2533 4170 7573 682b 6272 616e 6368 2533  %3Apush+branch%3
-00000c40: 416d 6173 7465 7222 2074 6172 6765 743d  Amaster" target=
-00000c50: 225f 626c 616e 6b22 3e0a 2020 2020 3c69  "_blank">.    <i
-00000c60: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00000c70: 6769 7468 7562 2e63 6f6d 2f6d 6461 7065  github.com/mdape
-00000c80: 6e61 2f70 7976 656e 7475 732f 6163 7469  na/pyventus/acti
-00000c90: 6f6e 732f 776f 726b 666c 6f77 732f 6465  ons/workflows/de
-00000ca0: 706c 6f79 2d64 6f63 732e 796d 6c2f 6261  ploy-docs.yml/ba
-00000cb0: 6467 652e 7376 673f 6272 616e 6368 3d6d  dge.svg?branch=m
-00000cc0: 6173 7465 7222 2061 6c74 3d22 446f 6373  aster" alt="Docs
-00000cd0: 223e 0a3c 2f61 3e0a 0a3c 6120 6872 6566  ">.</a>..<a href
-00000ce0: 3d27 6874 7470 733a 2f2f 636f 7665 7261  ='https://covera
-00000cf0: 6c6c 732e 696f 2f67 6974 6875 622f 6d64  lls.io/github/md
-00000d00: 6170 656e 612f 7079 7665 6e74 7573 3f62  apena/pyventus?b
-00000d10: 7261 6e63 683d 6d61 7374 6572 273e 0a09  ranch=master'>..
-00000d20: 3c69 6d67 2073 7263 3d27 6874 7470 733a  <img src='https:
-00000d30: 2f2f 636f 7665 7261 6c6c 732e 696f 2f72  //coveralls.io/r
-00000d40: 6570 6f73 2f67 6974 6875 622f 6d64 6170  epos/github/mdap
-00000d50: 656e 612f 7079 7665 6e74 7573 2f62 6164  ena/pyventus/bad
-00000d60: 6765 2e73 7667 3f62 7261 6e63 683d 6d61  ge.svg?branch=ma
-00000d70: 7374 6572 2720 616c 743d 2743 6f76 6572  ster' alt='Cover
-00000d80: 6167 6520 5374 6174 7573 272f 3e0a 3c2f  age Status'/>.</
-00000d90: 613e 0a0a 3c61 2068 7265 663d 2268 7474  a>..<a href="htt
-00000da0: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
-00000db0: 6f6a 6563 742f 7079 7665 6e74 7573 2220  oject/pyventus" 
-00000dc0: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
-00000dd0: 0a20 2020 203c 696d 6720 7372 633d 2268  .    <img src="h
-00000de0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000df0: 6473 2e69 6f2f 7079 7069 2f76 2f70 7976  ds.io/pypi/v/pyv
-00000e00: 656e 7475 733f 636f 6c6f 723d 626c 7565  entus?color=blue
+00000030: 352e 300a 5375 6d6d 6172 793a 2041 2070  5.0.Summary: A p
+00000040: 6f77 6572 6675 6c20 5079 7468 6f6e 2070  owerful Python p
+00000050: 6163 6b61 6765 2066 6f72 2065 7665 6e74  ackage for event
+00000060: 2d64 7269 7665 6e20 7072 6f67 7261 6d6d  -driven programm
+00000070: 696e 673b 2064 6566 696e 652c 2065 6d69  ing; define, emi
+00000080: 742c 2061 6e64 206f 7263 6865 7374 7261  t, and orchestra
+00000090: 7465 2065 7665 6e74 7320 7769 7468 2065  te events with e
+000000a0: 6173 652e 0a50 726f 6a65 6374 2d55 524c  ase..Project-URL
+000000b0: 3a20 486f 6d65 7061 6765 2c20 6874 7470  : Homepage, http
+000000c0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6d  s://github.com/m
+000000d0: 6461 7065 6e61 2f70 7976 656e 7475 730a  dapena/pyventus.
+000000e0: 5072 6f6a 6563 742d 5552 4c3a 2044 6f63  Project-URL: Doc
+000000f0: 756d 656e 7461 7469 6f6e 2c20 6874 7470  umentation, http
+00000100: 733a 2f2f 6d64 6170 656e 612e 6769 7468  s://mdapena.gith
+00000110: 7562 2e69 6f2f 7079 7665 6e74 7573 0a50  ub.io/pyventus.P
+00000120: 726f 6a65 6374 2d55 524c 3a20 5265 706f  roject-URL: Repo
+00000130: 7369 746f 7279 2c20 6874 7470 733a 2f2f  sitory, https://
+00000140: 6769 7468 7562 2e63 6f6d 2f6d 6461 7065  github.com/mdape
+00000150: 6e61 2f70 7976 656e 7475 730a 5072 6f6a  na/pyventus.Proj
+00000160: 6563 742d 5552 4c3a 2043 6861 6e67 656c  ect-URL: Changel
+00000170: 6f67 2c20 6874 7470 733a 2f2f 6d64 6170  og, https://mdap
+00000180: 656e 612e 6769 7468 7562 2e69 6f2f 7079  ena.github.io/py
+00000190: 7665 6e74 7573 2f72 656c 6561 7365 2d6e  ventus/release-n
+000001a0: 6f74 6573 0a41 7574 686f 722d 656d 6169  otes.Author-emai
+000001b0: 6c3a 204d 616e 7565 6c20 4461 2050 656e  l: Manuel Da Pen
+000001c0: 6120 3c64 6170 656e 736f 6674 4067 6d61  a <dapensoft@gma
+000001d0: 696c 2e63 6f6d 3e0a 4c69 6365 6e73 652d  il.com>.License-
+000001e0: 4578 7072 6573 7369 6f6e 3a20 4d49 540a  Expression: MIT.
+000001f0: 4c69 6365 6e73 652d 4669 6c65 3a20 4c49  License-File: LI
+00000200: 4345 4e53 450a 4b65 7977 6f72 6473 3a20  CENSE.Keywords: 
+00000210: 6576 656e 742d 6469 7370 6174 6368 6572  event-dispatcher
+00000220: 732c 6576 656e 742d 6472 6976 656e 2c65  s,event-driven,e
+00000230: 7665 6e74 2d65 6d69 7474 6572 732c 6576  vent-emitters,ev
+00000240: 656e 742d 6861 6e64 6c65 7273 2c65 7665  ent-handlers,eve
+00000250: 6e74 2d6c 696e 6b65 7273 2c65 7665 6e74  nt-linkers,event
+00000260: 732c 7079 7468 6f6e 0a43 6c61 7373 6966  s,python.Classif
+00000270: 6965 723a 2049 6e74 656e 6465 6420 4175  ier: Intended Au
+00000280: 6469 656e 6365 203a 3a20 4465 7665 6c6f  dience :: Develo
+00000290: 7065 7273 0a43 6c61 7373 6966 6965 723a  pers.Classifier:
+000002a0: 204c 6963 656e 7365 203a 3a20 4f53 4920   License :: OSI 
+000002b0: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
+000002c0: 4c69 6365 6e73 650a 436c 6173 7369 6669  License.Classifi
+000002d0: 6572 3a20 4f70 6572 6174 696e 6720 5379  er: Operating Sy
+000002e0: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
+000002f0: 656e 6465 6e74 0a43 6c61 7373 6966 6965  endent.Classifie
+00000300: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+00000310: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000320: 6e0a 436c 6173 7369 6669 6572 3a20 5072  n.Classifier: Pr
+00000330: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000340: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000350: 330a 436c 6173 7369 6669 6572 3a20 5072  3.Classifier: Pr
+00000360: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000370: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000380: 3320 3a3a 204f 6e6c 790a 436c 6173 7369  3 :: Only.Classi
+00000390: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+000003a0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000003b0: 7468 6f6e 203a 3a20 332e 3130 0a43 6c61  thon :: 3.10.Cla
+000003c0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+000003d0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000003e0: 2050 7974 686f 6e20 3a3a 2033 2e31 310a   Python :: 3.11.
+000003f0: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+00000400: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000410: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000420: 3132 0a43 6c61 7373 6966 6965 723a 2054  12.Classifier: T
+00000430: 6f70 6963 203a 3a20 536f 6674 7761 7265  opic :: Software
+00000440: 2044 6576 656c 6f70 6d65 6e74 0a43 6c61   Development.Cla
+00000450: 7373 6966 6965 723a 2054 6f70 6963 203a  ssifier: Topic :
+00000460: 3a20 536f 6674 7761 7265 2044 6576 656c  : Software Devel
+00000470: 6f70 6d65 6e74 203a 3a20 4c69 6272 6172  opment :: Librar
+00000480: 6965 730a 436c 6173 7369 6669 6572 3a20  ies.Classifier: 
+00000490: 546f 7069 6320 3a3a 2053 6f66 7477 6172  Topic :: Softwar
+000004a0: 6520 4465 7665 6c6f 706d 656e 7420 3a3a  e Development ::
+000004b0: 204c 6962 7261 7269 6573 203a 3a20 5079   Libraries :: Py
+000004c0: 7468 6f6e 204d 6f64 756c 6573 0a43 6c61  thon Modules.Cla
+000004d0: 7373 6966 6965 723a 2054 7970 696e 6720  ssifier: Typing 
+000004e0: 3a3a 2054 7970 6564 0a52 6571 7569 7265  :: Typed.Require
+000004f0: 732d 5079 7468 6f6e 3a20 3e3d 332e 3130  s-Python: >=3.10
+00000500: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
+00000510: 2061 6c6c 0a52 6571 7569 7265 732d 4469   all.Requires-Di
+00000520: 7374 3a20 7079 7665 6e74 7573 5b63 656c  st: pyventus[cel
+00000530: 6572 795d 3b20 6578 7472 6120 3d3d 2027  ery]; extra == '
+00000540: 616c 6c27 0a52 6571 7569 7265 732d 4469  all'.Requires-Di
+00000550: 7374 3a20 7079 7665 6e74 7573 5b66 6173  st: pyventus[fas
+00000560: 7461 7069 5d3b 2065 7874 7261 203d 3d20  tapi]; extra == 
+00000570: 2761 6c6c 270a 5265 7175 6972 6573 2d44  'all'.Requires-D
+00000580: 6973 743a 2070 7976 656e 7475 735b 7271  ist: pyventus[rq
+00000590: 5d3b 2065 7874 7261 203d 3d20 2761 6c6c  ]; extra == 'all
+000005a0: 270a 5072 6f76 6964 6573 2d45 7874 7261  '.Provides-Extra
+000005b0: 3a20 6365 6c65 7279 0a52 6571 7569 7265  : celery.Require
+000005c0: 732d 4469 7374 3a20 6365 6c65 7279 3e3d  s-Dist: celery>=
+000005d0: 352e 332e 353b 2065 7874 7261 203d 3d20  5.3.5; extra == 
+000005e0: 2763 656c 6572 7927 0a50 726f 7669 6465  'celery'.Provide
+000005f0: 732d 4578 7472 613a 2064 6576 0a52 6571  s-Extra: dev.Req
+00000600: 7569 7265 732d 4469 7374 3a20 6861 7463  uires-Dist: hatc
+00000610: 683e 3d31 2e38 2e31 3b20 6578 7472 6120  h>=1.8.1; extra 
+00000620: 3d3d 2027 6465 7627 0a52 6571 7569 7265  == 'dev'.Require
+00000630: 732d 4469 7374 3a20 7079 7665 6e74 7573  s-Dist: pyventus
+00000640: 5b64 6f63 735d 3b20 6578 7472 6120 3d3d  [docs]; extra ==
+00000650: 2027 6465 7627 0a52 6571 7569 7265 732d   'dev'.Requires-
+00000660: 4469 7374 3a20 7079 7665 6e74 7573 5b74  Dist: pyventus[t
+00000670: 6573 7473 5d3b 2065 7874 7261 203d 3d20  ests]; extra == 
+00000680: 2764 6576 270a 5072 6f76 6964 6573 2d45  'dev'.Provides-E
+00000690: 7874 7261 3a20 646f 6373 0a52 6571 7569  xtra: docs.Requi
+000006a0: 7265 732d 4469 7374 3a20 6d6b 646f 6373  res-Dist: mkdocs
+000006b0: 2d67 6974 2d63 6f6d 6d69 7474 6572 732d  -git-committers-
+000006c0: 706c 7567 696e 2d32 3e3d 322e 332e 303b  plugin-2>=2.3.0;
+000006d0: 2065 7874 7261 203d 3d20 2764 6f63 7327   extra == 'docs'
+000006e0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+000006f0: 6d6b 646f 6373 2d67 6974 2d72 6576 6973  mkdocs-git-revis
+00000700: 696f 6e2d 6461 7465 2d6c 6f63 616c 697a  ion-date-localiz
+00000710: 6564 2d70 6c75 6769 6e3e 3d31 2e32 2e31  ed-plugin>=1.2.1
+00000720: 3b20 6578 7472 6120 3d3d 2027 646f 6373  ; extra == 'docs
+00000730: 270a 5265 7175 6972 6573 2d44 6973 743a  '.Requires-Dist:
+00000740: 206d 6b64 6f63 732d 6d61 7465 7269 616c   mkdocs-material
+00000750: 3e3d 392e 352e 3137 3b20 6578 7472 6120  >=9.5.17; extra 
+00000760: 3d3d 2027 646f 6373 270a 5265 7175 6972  == 'docs'.Requir
+00000770: 6573 2d44 6973 743a 206d 6b64 6f63 732d  es-Dist: mkdocs-
+00000780: 6d61 7465 7269 616c 5b69 6d61 6769 6e67  material[imaging
+00000790: 5d3b 2065 7874 7261 203d 3d20 2764 6f63  ]; extra == 'doc
+000007a0: 7327 0a52 6571 7569 7265 732d 4469 7374  s'.Requires-Dist
+000007b0: 3a20 6d6b 646f 6373 7472 696e 6773 5b70  : mkdocstrings[p
+000007c0: 7974 686f 6e5d 3e3d 302e 3234 2e30 3b20  ython]>=0.24.0; 
+000007d0: 6578 7472 6120 3d3d 2027 646f 6373 270a  extra == 'docs'.
+000007e0: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
+000007f0: 6661 7374 6170 690a 5265 7175 6972 6573  fastapi.Requires
+00000800: 2d44 6973 743a 2066 6173 7461 7069 3e3d  -Dist: fastapi>=
+00000810: 302e 3935 2e32 3b20 6578 7472 6120 3d3d  0.95.2; extra ==
+00000820: 2027 6661 7374 6170 6927 0a50 726f 7669   'fastapi'.Provi
+00000830: 6465 732d 4578 7472 613a 2072 710a 5265  des-Extra: rq.Re
+00000840: 7175 6972 6573 2d44 6973 743a 2072 713e  quires-Dist: rq>
+00000850: 3d31 2e31 352e 303b 2065 7874 7261 203d  =1.15.0; extra =
+00000860: 3d20 2772 7127 0a50 726f 7669 6465 732d  = 'rq'.Provides-
+00000870: 4578 7472 613a 2074 6573 7473 0a52 6571  Extra: tests.Req
+00000880: 7569 7265 732d 4469 7374 3a20 626c 6163  uires-Dist: blac
+00000890: 6b3e 3d32 332e 3132 2e30 3b20 6578 7472  k>=23.12.0; extr
+000008a0: 6120 3d3d 2027 7465 7374 7327 0a52 6571  a == 'tests'.Req
+000008b0: 7569 7265 732d 4469 7374 3a20 636f 7665  uires-Dist: cove
+000008c0: 7261 6765 5b74 6f6d 6c5d 3e3d 372e 332e  rage[toml]>=7.3.
+000008d0: 333b 2065 7874 7261 203d 3d20 2774 6573  3; extra == 'tes
+000008e0: 7473 270a 5265 7175 6972 6573 2d44 6973  ts'.Requires-Dis
+000008f0: 743a 2066 616b 6572 6564 6973 3e3d 322e  t: fakeredis>=2.
+00000900: 3230 2e30 3b20 6578 7472 6120 3d3d 2027  20.0; extra == '
+00000910: 7465 7374 7327 0a52 6571 7569 7265 732d  tests'.Requires-
+00000920: 4469 7374 3a20 6874 7470 783e 3d30 2e32  Dist: httpx>=0.2
+00000930: 332e 303b 2065 7874 7261 203d 3d20 2774  3.0; extra == 't
+00000940: 6573 7473 270a 5265 7175 6972 6573 2d44  ests'.Requires-D
+00000950: 6973 743a 206d 7970 793e 3d31 2e37 2e31  ist: mypy>=1.7.1
+00000960: 3b20 6578 7472 6120 3d3d 2027 7465 7374  ; extra == 'test
+00000970: 7327 0a52 6571 7569 7265 732d 4469 7374  s'.Requires-Dist
+00000980: 3a20 7079 7465 7374 2d61 7379 6e63 696f  : pytest-asyncio
+00000990: 3e3d 302e 3231 2e30 3b20 6578 7472 6120  >=0.21.0; extra 
+000009a0: 3d3d 2027 7465 7374 7327 0a52 6571 7569  == 'tests'.Requi
+000009b0: 7265 732d 4469 7374 3a20 7079 7465 7374  res-Dist: pytest
+000009c0: 3e3d 372e 342e 303b 2065 7874 7261 203d  >=7.4.0; extra =
+000009d0: 3d20 2774 6573 7473 270a 5265 7175 6972  = 'tests'.Requir
+000009e0: 6573 2d44 6973 743a 2070 7976 656e 7475  es-Dist: pyventu
+000009f0: 735b 616c 6c5d 3b20 6578 7472 6120 3d3d  s[all]; extra ==
+00000a00: 2027 7465 7374 7327 0a44 6573 6372 6970   'tests'.Descrip
+00000a10: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
+00000a20: 653a 2074 6578 742f 6d61 726b 646f 776e  e: text/markdown
+00000a30: 0a0a 0a3c 6272 3e0a 0a3c 7020 616c 6967  ...<br>..<p alig
+00000a40: 6e3d 2263 656e 7465 7222 3e0a 2020 203c  n="center">.   <
+00000a50: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00000a60: 2f6d 6461 7065 6e61 2e67 6974 6875 622e  /mdapena.github.
+00000a70: 696f 2f70 7976 656e 7475 732f 696d 6167  io/pyventus/imag
+00000a80: 6573 2f6c 6f67 6f2f 7079 7665 6e74 7573  es/logo/pyventus
+00000a90: 2d6c 6f67 6f2d 6e61 6d65 2d73 6c6f 6761  -logo-name-sloga
+00000aa0: 6e2e 7376 6722 2061 6c74 3d22 5079 7665  n.svg" alt="Pyve
+00000ab0: 6e74 7573 2220 7769 6474 683d 2237 3530  ntus" width="750
+00000ac0: 7078 223e 0a3c 2f70 3e0a 0a3c 6272 3e0a  px">.</p>..<br>.
+00000ad0: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+00000ae0: 7222 3e0a 0a3c 6120 6872 6566 3d22 6874  r">..<a href="ht
+00000af0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000b00: 2f6d 6461 7065 6e61 2f70 7976 656e 7475  /mdapena/pyventu
+00000b10: 732f 6163 7469 6f6e 733f 7175 6572 793d  s/actions?query=
+00000b20: 776f 726b 666c 6f77 2533 4154 6573 7473  workflow%3ATests
+00000b30: 2b65 7665 6e74 2533 4170 7573 682b 6272  +event%3Apush+br
+00000b40: 616e 6368 2533 416d 6173 7465 7222 2074  anch%3Amaster" t
+00000b50: 6172 6765 743d 225f 626c 616e 6b22 3e0a  arget="_blank">.
+00000b60: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
+00000b70: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000b80: 2f6d 6461 7065 6e61 2f70 7976 656e 7475  /mdapena/pyventu
+00000b90: 732f 6163 7469 6f6e 732f 776f 726b 666c  s/actions/workfl
+00000ba0: 6f77 732f 7275 6e2d 7465 7374 732e 796d  ows/run-tests.ym
+00000bb0: 6c2f 6261 6467 652e 7376 673f 6272 616e  l/badge.svg?bran
+00000bc0: 6368 3d6d 6173 7465 7222 2061 6c74 3d22  ch=master" alt="
+00000bd0: 5465 7374 7322 3e0a 3c2f 613e 0a0a 3c61  Tests">.</a>..<a
+00000be0: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+00000bf0: 6974 6875 622e 636f 6d2f 6d64 6170 656e  ithub.com/mdapen
+00000c00: 612f 7079 7665 6e74 7573 2f61 6374 696f  a/pyventus/actio
+00000c10: 6e73 3f71 7565 7279 3d77 6f72 6b66 6c6f  ns?query=workflo
+00000c20: 7725 3341 446f 6373 2b65 7665 6e74 2533  w%3ADocs+event%3
+00000c30: 4170 7573 682b 6272 616e 6368 2533 416d  Apush+branch%3Am
+00000c40: 6173 7465 7222 2074 6172 6765 743d 225f  aster" target="_
+00000c50: 626c 616e 6b22 3e0a 2020 2020 3c69 6d67  blank">.    <img
+00000c60: 2073 7263 3d22 6874 7470 733a 2f2f 6769   src="https://gi
+00000c70: 7468 7562 2e63 6f6d 2f6d 6461 7065 6e61  thub.com/mdapena
+00000c80: 2f70 7976 656e 7475 732f 6163 7469 6f6e  /pyventus/action
+00000c90: 732f 776f 726b 666c 6f77 732f 6465 706c  s/workflows/depl
+00000ca0: 6f79 2d64 6f63 732e 796d 6c2f 6261 6467  oy-docs.yml/badg
+00000cb0: 652e 7376 673f 6272 616e 6368 3d6d 6173  e.svg?branch=mas
+00000cc0: 7465 7222 2061 6c74 3d22 446f 6373 223e  ter" alt="Docs">
+00000cd0: 0a3c 2f61 3e0a 0a3c 6120 6872 6566 3d27  .</a>..<a href='
+00000ce0: 6874 7470 733a 2f2f 636f 7665 7261 6c6c  https://coverall
+00000cf0: 732e 696f 2f67 6974 6875 622f 6d64 6170  s.io/github/mdap
+00000d00: 656e 612f 7079 7665 6e74 7573 3f62 7261  ena/pyventus?bra
+00000d10: 6e63 683d 6d61 7374 6572 273e 0a09 3c69  nch=master'>..<i
+00000d20: 6d67 2073 7263 3d27 6874 7470 733a 2f2f  mg src='https://
+00000d30: 636f 7665 7261 6c6c 732e 696f 2f72 6570  coveralls.io/rep
+00000d40: 6f73 2f67 6974 6875 622f 6d64 6170 656e  os/github/mdapen
+00000d50: 612f 7079 7665 6e74 7573 2f62 6164 6765  a/pyventus/badge
+00000d60: 2e73 7667 3f62 7261 6e63 683d 6d61 7374  .svg?branch=mast
+00000d70: 6572 2720 616c 743d 2743 6f76 6572 6167  er' alt='Coverag
+00000d80: 6520 5374 6174 7573 272f 3e0a 3c2f 613e  e Status'/>.</a>
+00000d90: 0a0a 3c61 2068 7265 663d 2268 7474 7073  ..<a href="https
+00000da0: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+00000db0: 6563 742f 7079 7665 6e74 7573 2220 7461  ect/pyventus" ta
+00000dc0: 7267 6574 3d22 5f62 6c61 6e6b 223e 0a20  rget="_blank">. 
+00000dd0: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
+00000de0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000df0: 2e69 6f2f 7079 7069 2f76 2f70 7976 656e  .io/pypi/v/pyven
+00000e00: 7475 733f 636f 6c6f 723d 3030 3937 6138  tus?color=0097a8
 00000e10: 2220 616c 743d 2250 6163 6b61 6765 2076  " alt="Package v
 00000e20: 6572 7369 6f6e 223e 0a3c 2f61 3e0a 0a3c  ersion">.</a>..<
 00000e30: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
 00000e40: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
 00000e50: 2f70 7976 656e 7475 7322 2074 6172 6765  /pyventus" targe
 00000e60: 743d 225f 626c 616e 6b22 3e0a 2020 2020  t="_blank">.    
 00000e70: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
 00000e80: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
 00000e90: 2f70 7970 692f 7079 7665 7273 696f 6e73  /pypi/pyversions
 00000ea0: 2f70 7976 656e 7475 733f 636f 6c6f 723d  /pyventus?color=
-00000eb0: 626c 7565 2220 616c 743d 2253 7570 706f  blue" alt="Suppo
-00000ec0: 7274 6564 2050 7974 686f 6e20 7665 7273  rted Python vers
-00000ed0: 696f 6e73 223e 0a3c 2f61 3e0a 0a3c 6120  ions">.</a>..<a 
-00000ee0: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
-00000ef0: 7468 7562 2e63 6f6d 2f70 7366 2f62 6c61  thub.com/psf/bla
-00000f00: 636b 223e 0a09 3c69 6d67 2073 7263 3d22  ck">..<img src="
-00000f10: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000f20: 6c64 732e 696f 2f62 6164 6765 2f63 6f64  lds.io/badge/cod
-00000f30: 6525 3230 7374 796c 652d 626c 6163 6b2d  e%20style-black-
-00000f40: 3030 3030 3030 2e73 7667 2220 616c 743d  000000.svg" alt=
-00000f50: 2243 6f64 6520 7374 796c 653a 2062 6c61  "Code style: bla
-00000f60: 636b 223e 0a3c 2f61 3e0a 0a3c 2f70 3e0a  ck">.</a>..</p>.
-00000f70: 0a3c 6272 3e0a 0a0a 2d2d 2d0a 0a2a 2a44  .<br>...---..**D
-00000f80: 6f63 756d 656e 7461 7469 6f6e 2a2a 3a20  ocumentation**: 
-00000f90: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00000fa0: 2f6d 6461 7065 6e61 2e67 6974 6875 622e  /mdapena.github.
-00000fb0: 696f 2f70 7976 656e 7475 7322 2074 6172  io/pyventus" tar
-00000fc0: 6765 743d 225f 626c 616e 6b22 3e68 7474  get="_blank">htt
-00000fd0: 7073 3a2f 2f6d 6461 7065 6e61 2e67 6974  ps://mdapena.git
-00000fe0: 6875 622e 696f 2f70 7976 656e 7475 733c  hub.io/pyventus<
-00000ff0: 2f61 3e0a 0a2a 2a53 6f75 7263 6520 436f  /a>..**Source Co
-00001000: 6465 2a2a 3a20 3c61 2068 7265 663d 2268  de**: <a href="h
-00001010: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001020: 6d2f 6d64 6170 656e 612f 7079 7665 6e74  m/mdapena/pyvent
-00001030: 7573 2220 7461 7267 6574 3d22 5f62 6c61  us" target="_bla
-00001040: 6e6b 223e 6874 7470 733a 2f2f 6769 7468  nk">https://gith
-00001050: 7562 2e63 6f6d 2f6d 6461 7065 6e61 2f70  ub.com/mdapena/p
-00001060: 7976 656e 7475 733c 2f61 3e0a 0a2d 2d2d  yventus</a>..---
-00001070: 0a0a 3c70 2073 7479 6c65 3d27 7465 7874  ..<p style='text
-00001080: 2d61 6c69 676e 3a20 6a75 7374 6966 793b  -align: justify;
-00001090: 273e 0a20 2020 2026 656d 7370 3b26 656d  '>.    &emsp;&em
-000010a0: 7370 3b50 7976 656e 7475 7320 6973 2061  sp;Pyventus is a
-000010b0: 206d 6f64 6572 6e20 616e 6420 726f 6275   modern and robu
-000010c0: 7374 2050 7974 686f 6e20 7061 636b 6167  st Python packag
-000010d0: 6520 666f 7220 6576 656e 742d 6472 6976  e for event-driv
-000010e0: 656e 2070 726f 6772 616d 6d69 6e67 2e20  en programming. 
-000010f0: 4974 206f 6666 6572 7320 6120 636f 6d70  It offers a comp
-00001100: 7265 6865 6e73 6976 650a 0973 7569 7465  rehensive..suite
-00001110: 206f 6620 746f 6f6c 7320 746f 2065 6173   of tools to eas
-00001120: 696c 7920 6465 6669 6e65 2c20 656d 6974  ily define, emit
-00001130: 2c20 616e 6420 6f72 6368 6573 7472 6174  , and orchestrat
-00001140: 6520 6576 656e 7473 2075 7369 6e67 2063  e events using c
-00001150: 7573 746f 6d69 7a61 626c 6520 6576 656e  ustomizable even
-00001160: 7420 656d 6974 7465 7273 2061 6e64 2066  t emitters and f
-00001170: 6c65 7869 626c 650a 0972 6573 706f 6e73  lexible..respons
-00001180: 6573 2e20 5769 7468 2050 7976 656e 7475  es. With Pyventu
-00001190: 732c 2079 6f75 2063 616e 2065 6173 696c  s, you can easil
-000011a0: 7920 6275 696c 6420 7363 616c 6162 6c65  y build scalable
-000011b0: 2c20 6578 7465 6e73 6962 6c65 2c20 616e  , extensible, an
-000011c0: 6420 6c6f 6f73 656c 792d 636f 7570 6c65  d loosely-couple
-000011d0: 6420 6576 656e 742d 6472 6976 656e 2061  d event-driven a
-000011e0: 7070 6c69 6361 7469 6f6e 732e 0a3c 2f70  pplications..</p
-000011f0: 3e0a 0a23 2320 4d6f 7265 2074 6861 6e20  >..## More than 
-00001200: 6a75 7374 2045 7665 6e74 730a 0a3c 7020  just Events..<p 
-00001210: 7374 796c 653d 2774 6578 742d 616c 6967  style='text-alig
-00001220: 6e3a 206a 7573 7469 6679 3b27 3e0a 0950  n: justify;'>..P
-00001230: 7976 656e 7475 7320 6f66 6665 7273 2073  yventus offers s
-00001240: 6576 6572 616c 206b 6579 2066 6561 7475  everal key featu
-00001250: 7265 7320 7468 6174 206d 616b 6520 6974  res that make it
-00001260: 2061 2070 6f77 6572 6675 6c20 6576 656e   a powerful even
-00001270: 742d 6472 6976 656e 2070 726f 6772 616d  t-driven program
-00001280: 6d69 6e67 2070 6163 6b61 6765 2066 6f72  ming package for
-00001290: 2079 6f75 7220 0a09 5079 7468 6f6e 2070   your ..Python p
-000012a0: 726f 6a65 6374 733a 0a3c 2f70 3e20 0a0a  rojects:.</p> ..
-000012b0: 3c75 6c20 7374 796c 653d 2774 6578 742d  <ul style='text-
-000012c0: 616c 6967 6e3a 206a 7573 7469 6679 3b27  align: justify;'
-000012d0: 3e0a 0a3c 6c69 3e3c 623e 416e 2049 6e74  >..<li><b>An Int
-000012e0: 7569 7469 7665 2041 5049 3c2f 623e 20e2  uitive API</b> .
-000012f0: 9480 200a 5079 7665 6e74 7573 2070 726f  .. .Pyventus pro
-00001300: 7669 6465 7320 6120 7573 6572 2d66 7269  vides a user-fri
-00001310: 656e 646c 7920 4150 4920 666f 7220 6465  endly API for de
-00001320: 6669 6e69 6e67 2065 7665 6e74 732c 2065  fining events, e
-00001330: 6d69 7474 6572 732c 2061 6e64 2068 616e  mitters, and han
-00001340: 646c 6572 732e 2049 7473 2064 6573 6967  dlers. Its desig
-00001350: 6e20 7369 6d70 6c69 6669 6573 2074 6865  n simplifies the
-00001360: 2070 726f 6365 7373 0a6f 6620 776f 726b   process.of work
-00001370: 696e 6720 7769 7468 2065 7665 6e74 732c  ing with events,
-00001380: 2065 6e61 626c 696e 6720 796f 7520 746f   enabling you to
-00001390: 206f 7267 616e 697a 6520 796f 7572 2063   organize your c
-000013a0: 6f64 6520 6172 6f75 6e64 2064 6973 6372  ode around discr
-000013b0: 6574 6520 6576 656e 7473 2061 6e64 2074  ete events and t
-000013c0: 6865 6972 2061 7373 6f63 6961 7465 6420  heir associated 
-000013d0: 6163 7469 6f6e 732e 0a3c 2f6c 693e 0a0a  actions..</li>..
-000013e0: 3c6c 693e 3c62 3e53 796e 6320 616e 6420  <li><b>Sync and 
-000013f0: 4173 796e 6320 5375 7070 6f72 743c 2f62  Async Support</b
-00001400: 3e20 e294 8020 0a57 6865 7468 6572 2079  > ... .Whether y
-00001410: 6f75 7220 636f 6465 2069 7320 7379 6e63  our code is sync
-00001420: 6872 6f6e 6f75 7320 6f72 2061 7379 6e63  hronous or async
-00001430: 6872 6f6e 6f75 732c 2050 7976 656e 7475  hronous, Pyventu
-00001440: 7320 616c 6c6f 7773 2079 6f75 2074 6f20  s allows you to 
-00001450: 6465 6669 6e65 2065 7665 6e74 2068 616e  define event han
-00001460: 646c 6572 7320 6173 2065 6974 6865 7220  dlers as either 
-00001470: 7379 6e63 206f 7220 6173 796e 630a 6361  sync or async.ca
-00001480: 6c6c 6261 636b 7320 616e 6420 656d 6974  llbacks and emit
-00001490: 2065 7665 6e74 7320 6672 6f6d 2062 6f74   events from bot
-000014a0: 6820 7363 6f70 6573 2e20 0a3c 2f6c 693e  h scopes. .</li>
-000014b0: 0a0a 3c6c 693e 3c62 3e52 756e 7469 6d65  ..<li><b>Runtime
-000014c0: 2046 6c65 7869 6269 6c69 7479 3c2f 623e   Flexibility</b>
-000014d0: 20e2 9480 200a 5079 7665 6e74 7573 2720   ... .Pyventus' 
-000014e0: 7275 6e74 696d 6520 666c 6578 6962 696c  runtime flexibil
-000014f0: 6974 7920 616c 6c6f 7773 2079 6f75 2074  ity allows you t
-00001500: 6f20 7377 6974 6368 2073 6561 6d6c 6573  o switch seamles
-00001510: 736c 7920 6265 7477 6565 6e20 6469 6666  sly between diff
-00001520: 6572 656e 7420 6f66 6669 6369 616c 206f  erent official o
-00001530: 7220 6375 7374 6f6d 2065 7665 6e74 2065  r custom event e
-00001540: 6d69 7474 6572 0a69 6d70 6c65 6d65 6e74  mitter.implement
-00001550: 6174 696f 6e73 206f 6e20 7468 6520 666c  ations on the fl
-00001560: 792e 0a3c 2f6c 693e 0a0a 3c6c 693e 3c62  y..</li>..<li><b
-00001570: 3e43 7573 746f 6d69 7a61 7469 6f6e 3c2f  >Customization</
-00001580: 623e 20e2 9480 200a 5768 6574 6865 7220  b> ... .Whether 
-00001590: 796f 7520 6368 6f6f 7365 206f 6666 6963  you choose offic
-000015a0: 6961 6c20 656d 6974 7465 7273 206f 7220  ial emitters or 
-000015b0: 6375 7374 6f6d 206f 6e65 732c 2050 7976  custom ones, Pyv
-000015c0: 656e 7475 7320 616c 6c6f 7773 2079 6f75  entus allows you
-000015d0: 2074 6f20 6375 7374 6f6d 697a 6520 7468   to customize th
-000015e0: 6520 6265 6861 7669 6f72 2061 6e64 2063  e behavior and c
-000015f0: 6170 6162 696c 6974 6965 7320 6f66 0a74  apabilities of.t
-00001600: 6865 2065 7665 6e74 2065 6d69 7474 6572  he event emitter
-00001610: 7320 746f 2070 6572 6665 6374 6c79 2061  s to perfectly a
-00001620: 6c69 676e 2077 6974 6820 796f 7572 2075  lign with your u
-00001630: 6e69 7175 6520 7265 7175 6972 656d 656e  nique requiremen
-00001640: 7473 2e0a 3c2f 6c69 3e0a 0a3c 6c69 3e3c  ts..</li>..<li><
-00001650: 623e 5265 6c69 6162 6c65 2045 7665 6e74  b>Reliable Event
-00001660: 2048 616e 646c 696e 673c 2f62 3e20 e294   Handling</b> ..
-00001670: 8020 0a50 7976 656e 7475 7320 616c 6c6f  . .Pyventus allo
-00001680: 7773 2079 6f75 2074 6f20 6465 6669 6e65  ws you to define
-00001690: 2068 616e 646c 6572 7320 746f 2063 7573   handlers to cus
-000016a0: 746f 6d69 7a65 2068 6f77 2065 7665 6e74  tomize how event
-000016b0: 7320 6172 6520 7072 6f63 6573 7365 6420  s are processed 
-000016c0: 7570 6f6e 2063 6f6d 706c 6574 696f 6e2e  upon completion.
-000016d0: 2041 7474 6163 6820 7375 6363 6573 7320   Attach success 
-000016e0: 616e 640a 6661 696c 7572 6520 6c6f 6769  and.failure logi
-000016f0: 6320 746f 2074 616b 6520 7461 7267 6574  c to take target
-00001700: 6564 2061 6374 696f 6e73 2062 6173 6564  ed actions based
-00001710: 206f 6e20 7468 6520 6f75 7463 6f6d 6520   on the outcome 
-00001720: 6f66 2065 6163 6820 6576 656e 7420 6578  of each event ex
-00001730: 6563 7574 696f 6e2e 200a 3c2f 6c69 3e0a  ecution. .</li>.
-00001740: 0a3c 6c69 3e3c 623e 5363 616c 6162 696c  .<li><b>Scalabil
-00001750: 6974 7920 616e 6420 4d61 696e 7461 696e  ity and Maintain
-00001760: 6162 696c 6974 793c 2f62 3e20 e294 8020  ability</b> ... 
-00001770: 0a42 7920 6164 6f70 7469 6e67 2061 6e20  .By adopting an 
-00001780: 6576 656e 742d 6472 6976 656e 2061 7070  event-driven app
-00001790: 726f 6163 6820 7769 7468 2050 7976 656e  roach with Pyven
-000017a0: 7475 732c 2079 6f75 2063 616e 2063 7265  tus, you can cre
-000017b0: 6174 6520 7363 616c 6162 6c65 2061 6e64  ate scalable and
-000017c0: 206d 6169 6e74 6169 6e61 626c 6520 636f   maintainable co
-000017d0: 6465 2074 6861 6e6b 7320 746f 2074 6865  de thanks to the
-000017e0: 206c 6f6f 7365 0a63 6f75 706c 696e 6720   loose.coupling 
-000017f0: 6265 7477 6565 6e20 6974 7320 636f 6d70  between its comp
-00001800: 6f6e 656e 7473 2074 6861 7420 656e 6162  onents that enab
-00001810: 6c65 7320 6578 7465 6e73 6962 696c 6974  les extensibilit
-00001820: 7920 616e 6420 6d6f 6475 6c61 7269 7479  y and modularity
-00001830: 2e0a 3c2f 6c69 3e0a 0a3c 6c69 3e3c 623e  ..</li>..<li><b>
-00001840: 436f 6d70 7265 6865 6e73 6976 6520 446f  Comprehensive Do
-00001850: 6375 6d65 6e74 6174 696f 6e3c 2f62 3e20  cumentation</b> 
-00001860: e294 8020 0a50 7976 656e 7475 7320 7072  ... .Pyventus pr
-00001870: 6f76 6964 6573 2061 2063 6f6d 7072 6568  ovides a compreh
-00001880: 656e 7369 7665 2064 6f63 756d 656e 7461  ensive documenta
-00001890: 7469 6f6e 2073 7569 7465 2074 6861 7420  tion suite that 
-000018a0: 696e 636c 7564 6573 2041 5049 2072 6566  includes API ref
-000018b0: 6572 656e 6365 732c 2075 7361 6765 2065  erences, usage e
-000018c0: 7861 6d70 6c65 732c 2062 6573 7420 7072  xamples, best pr
-000018d0: 6163 7469 6365 730a 6775 6964 6573 2c20  actices.guides, 
-000018e0: 616e 6420 7475 746f 7269 616c 7320 746f  and tutorials to
-000018f0: 2065 6666 6563 7469 7665 6c79 206c 6576   effectively lev
-00001900: 6572 6167 6520 616c 6c20 7468 6520 6665  erage all the fe
-00001910: 6174 7572 6573 2061 6e64 2063 6170 6162  atures and capab
-00001920: 696c 6974 6965 7320 6f66 2074 6865 2070  ilities of the p
-00001930: 6163 6b61 6765 2e0a 3c2f 6c69 3e0a 0a3c  ackage..</li>..<
-00001940: 2f75 6c3e 0a0a 2323 2052 6571 7569 7265  /ul>..## Require
-00001950: 6d65 6e74 730a 0a3c 7020 7374 796c 653d  ments..<p style=
-00001960: 2774 6578 742d 616c 6967 6e3a 206a 7573  'text-align: jus
-00001970: 7469 6679 3b27 3e0a 0926 656d 7370 3b26  tify;'>..&emsp;&
-00001980: 656d 7370 3b50 7965 7665 6e74 7320 3c62  emsp;Pyevents <b
-00001990: 3e6f 6e6c 7920 7265 7175 6972 6573 2050  >only requires P
-000019a0: 7974 686f 6e20 332e 3130 2b3c 2f62 3e20  ython 3.10+</b> 
-000019b0: 6279 2064 6566 6175 6c74 2c20 7768 6963  by default, whic
-000019c0: 6820 696e 636c 7564 6573 2074 6865 200a  h includes the .
-000019d0: 093c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
-000019e0: 2f2f 6d64 6170 656e 612e 6769 7468 7562  //mdapena.github
-000019f0: 2e69 6f2f 7079 7665 6e74 7573 2f74 7574  .io/pyventus/tut
-00001a00: 6f72 6961 6c73 2f65 6d69 7474 6572 732f  orials/emitters/
-00001a10: 6173 796e 6369 6f22 2074 6172 6765 743d  asyncio" target=
-00001a20: 225f 626c 616e 6b22 3e3c 636f 6465 3e41  "_blank"><code>A
-00001a30: 7379 6e63 494f 4576 656e 7445 6d69 7474  syncIOEventEmitt
-00001a40: 6572 3c2f 636f 6465 3e3c 2f61 3e0a 0961  er</code></a>..a
-00001a50: 6e64 2074 6865 203c 6120 6872 6566 3d22  nd the <a href="
-00001a60: 6874 7470 733a 2f2f 6d64 6170 656e 612e  https://mdapena.
-00001a70: 6769 7468 7562 2e69 6f2f 7079 7665 6e74  github.io/pyvent
-00001a80: 7573 2f74 7574 6f72 6961 6c73 2f65 6d69  us/tutorials/emi
-00001a90: 7474 6572 732f 6578 6563 7574 6f72 2220  tters/executor" 
-00001aa0: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
-00001ab0: 3c63 6f64 653e 4578 6563 7574 6f72 4576  <code>ExecutorEv
-00001ac0: 656e 7445 6d69 7474 6572 3c2f 636f 6465  entEmitter</code
-00001ad0: 3e3c 2f61 3e20 0a09 7769 7468 206e 6f20  ></a> ..with no 
-00001ae0: 6164 6469 7469 6f6e 616c 2064 6570 656e  additional depen
-00001af0: 6465 6e63 6965 732e 2048 6f77 6576 6572  dencies. However
-00001b00: 2c20 796f 7572 2072 6571 7569 7265 6d65  , your requireme
-00001b10: 6e74 7320 6d61 7920 6578 7061 6e64 2069  nts may expand i
-00001b20: 6620 796f 7520 6f70 7420 746f 2075 7365  f you opt to use
-00001b30: 2020 0a09 3c61 2068 7265 663d 2268 7474    ..<a href="htt
-00001b40: 7073 3a2f 2f6d 6461 7065 6e61 2e67 6974  ps://mdapena.git
-00001b50: 6875 622e 696f 2f70 7976 656e 7475 732f  hub.io/pyventus/
-00001b60: 6765 7474 696e 672d 7374 6172 7465 642f  getting-started/
-00001b70: 236f 7074 696f 6e61 6c2d 6465 7065 6e64  #optional-depend
-00001b80: 656e 6369 6573 2220 7461 7267 6574 3d22  encies" target="
-00001b90: 5f62 6c61 6e6b 223e 616c 7465 726e 6174  _blank">alternat
-00001ba0: 6976 6520 6275 696c 742d 696e 2065 7665  ive built-in eve
-00001bb0: 6e74 2065 6d69 7474 6572 2069 6d70 6c65  nt emitter imple
-00001bc0: 6d65 6e74 6174 696f 6e73 3c2f 613e 2e0a  mentations</a>..
-00001bd0: 3c2f 703e 0a0a 2323 2049 6e73 7461 6c6c  </p>..## Install
-00001be0: 6174 696f 6e0a 0a3c 7020 7374 796c 653d  ation..<p style=
-00001bf0: 2774 6578 742d 616c 6967 6e3a 206a 7573  'text-align: jus
-00001c00: 7469 6679 3b27 3e0a 0926 656d 7370 3b26  tify;'>..&emsp;&
-00001c10: 656d 7370 3b50 7976 656e 7475 7320 6973  emsp;Pyventus is
-00001c20: 2061 7661 696c 6162 6c65 2061 7320 6120   available as a 
-00001c30: 5079 7468 6f6e 2070 6163 6b61 6765 2061  Python package a
-00001c40: 6e64 2063 616e 2062 6520 6561 7369 6c79  nd can be easily
-00001c50: 2069 6e73 7461 6c6c 6564 2075 7369 6e67   installed using
-00001c60: 203c 636f 6465 3e70 6970 3c2f 636f 6465   <code>pip</code
-00001c70: 3e2e 204f 7065 6e20 796f 7572 2074 6572  >. Open your ter
-00001c80: 6d69 6e61 6c0a 0961 6e64 2065 7865 6375  minal..and execu
-00001c90: 7465 2074 6865 2066 6f6c 6c6f 7769 6e67  te the following
-00001ca0: 2063 6f6d 6d61 6e64 2074 6f20 696e 7374   command to inst
-00001cb0: 616c 6c20 6974 3a0a 3c2f 703e 0a0a 6060  all it:.</p>..``
-00001cc0: 6063 6f6e 736f 6c65 0a70 6970 2069 6e73  `console.pip ins
-00001cd0: 7461 6c6c 2070 7976 656e 7475 730a 6060  tall pyventus.``
-00001ce0: 600a 0a23 2320 3c63 6f64 653e 4865 6c6c  `..## <code>Hell
-00001cf0: 6f2c 2057 6f72 6c64 213c 2f63 6f64 653e  o, World!</code>
-00001d00: 2045 7861 6d70 6c65 0a0a 3c70 2073 7479   Example..<p sty
-00001d10: 6c65 3d27 7465 7874 2d61 6c69 676e 3a20  le='text-align: 
-00001d20: 6a75 7374 6966 793b 273e 0a20 2020 2026  justify;'>.    &
-00001d30: 656d 7370 3b26 656d 7370 3b45 7870 6572  emsp;&emsp;Exper
-00001d40: 6965 6e63 6520 7468 6520 706f 7765 7220  ience the power 
-00001d50: 6f66 2050 7976 656e 7475 7320 7468 726f  of Pyventus thro
-00001d60: 7567 6820 6120 7369 6d70 6c65 203c 636f  ugh a simple <co
-00001d70: 6465 3e48 656c 6c6f 2c20 576f 726c 6421  de>Hello, World!
-00001d80: 3c2f 636f 6465 3e20 6578 616d 706c 6520  </code> example 
-00001d90: 7468 6174 2069 6c6c 7573 7472 6174 6573  that illustrates
-00001da0: 200a 0974 6865 2063 6f72 6520 636f 6e63   ..the core conc
-00001db0: 6570 7473 2061 6e64 2062 6173 6963 2075  epts and basic u
-00001dc0: 7361 6765 206f 6620 7468 6520 7061 636b  sage of the pack
-00001dd0: 6167 652e 2054 6869 7320 6578 616d 706c  age. This exampl
-00001de0: 6520 7769 6c6c 2077 616c 6b20 796f 7520  e will walk you 
-00001df0: 7468 726f 7567 6820 7468 6520 6573 7365  through the esse
-00001e00: 6e74 6961 6c20 7374 6570 7320 6f66 200a  ntial steps of .
-00001e10: 0963 7265 6174 696e 6720 616e 2065 7665  .creating an eve
-00001e20: 6e74 2068 616e 646c 6572 2061 6e64 2074  nt handler and t
-00001e30: 7269 6767 6572 696e 6720 6576 656e 7473  riggering events
-00001e40: 2077 6974 6869 6e20 796f 7572 2061 7070   within your app
-00001e50: 6c69 6361 7469 6f6e 2e0a 3c2f 703e 0a0a  lication..</p>..
-00001e60: 6060 6050 7974 686f 6e20 7469 746c 653d  ```Python title=
-00001e70: 2248 656c 6c6f 2c20 576f 726c 6421 2065  "Hello, World! e
-00001e80: 7861 6d70 6c65 2077 6974 6820 5079 7665  xample with Pyve
-00001e90: 6e74 7573 2220 6c69 6e65 6e75 6d73 3d22  ntus" linenums="
-00001ea0: 3122 0a66 726f 6d20 7079 7665 6e74 7573  1".from pyventus
-00001eb0: 2069 6d70 6f72 7420 4576 656e 744c 696e   import EventLin
-00001ec0: 6b65 722c 2045 7665 6e74 456d 6974 7465  ker, EventEmitte
-00001ed0: 722c 2041 7379 6e63 494f 4576 656e 7445  r, AsyncIOEventE
-00001ee0: 6d69 7474 6572 0a0a 0a40 4576 656e 744c  mitter...@EventL
-00001ef0: 696e 6b65 722e 6f6e 2822 4d79 4576 656e  inker.on("MyEven
-00001f00: 7422 290a 6465 6620 6576 656e 745f 6361  t").def event_ca
-00001f10: 6c6c 6261 636b 2829 3a0a 2020 2020 7072  llback():.    pr
-00001f20: 696e 7428 2248 656c 6c6f 2c20 576f 726c  int("Hello, Worl
-00001f30: 6421 2229 0a0a 0a65 7665 6e74 5f65 6d69  d!")...event_emi
-00001f40: 7474 6572 3a20 4576 656e 7445 6d69 7474  tter: EventEmitt
-00001f50: 6572 203d 2041 7379 6e63 494f 4576 656e  er = AsyncIOEven
-00001f60: 7445 6d69 7474 6572 2829 0a65 7665 6e74  tEmitter().event
-00001f70: 5f65 6d69 7474 6572 2e65 6d69 7428 224d  _emitter.emit("M
-00001f80: 7945 7665 6e74 2229 0a60 6060 0a0a 3c64  yEvent").```..<d
-00001f90: 6574 6169 6c73 206d 6172 6b64 6f77 6e3d  etails markdown=
-00001fa0: 2231 2220 636c 6173 733d 2269 6e66 6f22  "1" class="info"
-00001fb0: 3e0a 3c73 756d 6d61 7279 3e59 6f75 2063  >.<summary>You c
-00001fc0: 616e 2061 6c73 6f20 776f 726b 2077 6974  an also work wit
-00001fd0: 6820 3c63 6f64 653e 6173 796e 633c 2f63  h <code>async</c
-00001fe0: 6f64 653e 2066 756e 6374 696f 6e73 2061  ode> functions a
-00001ff0: 6e64 2063 6f6e 7465 7874 732e 2e2e 3c2f  nd contexts...</
-00002000: 7375 6d6d 6172 793e 0a0a 6060 6050 7974  summary>..```Pyt
-00002010: 686f 6e20 7469 746c 653d 2248 656c 6c6f  hon title="Hello
-00002020: 2c20 576f 726c 6421 2065 7861 6d70 6c65  , World! example
-00002030: 2077 6974 6820 5079 7665 6e74 7573 2028   with Pyventus (
-00002040: 4173 796e 6320 7665 7273 696f 6e29 2220  Async version)" 
-00002050: 6c69 6e65 6e75 6d73 3d22 3122 2068 6c5f  linenums="1" hl_
-00002060: 6c69 6e65 733d 2235 2031 3422 0a66 726f  lines="5 14".fro
-00002070: 6d20 7079 7665 6e74 7573 2069 6d70 6f72  m pyventus impor
-00002080: 7420 4576 656e 744c 696e 6b65 722c 2045  t EventLinker, E
-00002090: 7665 6e74 456d 6974 7465 722c 2041 7379  ventEmitter, Asy
-000020a0: 6e63 494f 4576 656e 7445 6d69 7474 6572  ncIOEventEmitter
-000020b0: 0a0a 0a40 4576 656e 744c 696e 6b65 722e  ...@EventLinker.
-000020c0: 6f6e 2822 4d79 4576 656e 7422 290a 6173  on("MyEvent").as
-000020d0: 796e 6320 6465 6620 6576 656e 745f 6361  ync def event_ca
-000020e0: 6c6c 6261 636b 2829 3a0a 2020 2020 7072  llback():.    pr
-000020f0: 696e 7428 2248 656c 6c6f 2c20 576f 726c  int("Hello, Worl
-00002100: 6421 2229 0a0a 0a65 7665 6e74 5f65 6d69  d!")...event_emi
-00002110: 7474 6572 3a20 4576 656e 7445 6d69 7474  tter: EventEmitt
-00002120: 6572 203d 2041 7379 6e63 494f 4576 656e  er = AsyncIOEven
-00002130: 7445 6d69 7474 6572 2829 0a65 7665 6e74  tEmitter().event
-00002140: 5f65 6d69 7474 6572 2e65 6d69 7428 224d  _emitter.emit("M
-00002150: 7945 7665 6e74 2229 0a60 6060 0a0a 3c2f  yEvent").```..</
-00002160: 6465 7461 696c 733e 0a0a 3c70 2073 7479  details>..<p sty
-00002170: 6c65 3d27 7465 7874 2d61 6c69 676e 3a20  le='text-align: 
-00002180: 6a75 7374 6966 793b 273e 0a20 2020 2026  justify;'>.    &
-00002190: 656d 7370 3b26 656d 7370 3b41 7320 7765  emsp;&emsp;As we
-000021a0: 2063 616e 2073 6565 2066 726f 6d20 7468   can see from th
-000021b0: 6520 3c63 6f64 653e 4865 6c6c 6f2c 2057  e <code>Hello, W
-000021c0: 6f72 6c64 213c 2f63 6f64 653e 2065 7861  orld!</code> exa
-000021d0: 6d70 6c65 2c20 5079 7665 6e74 7573 2066  mple, Pyventus f
-000021e0: 6f6c 6c6f 7773 2061 2073 696d 706c 6520  ollows a simple 
-000021f0: 616e 6420 696e 7475 6974 6976 6520 0a09  and intuitive ..
-00002200: 776f 726b 666c 6f77 2066 6f72 2065 7665  workflow for eve
-00002210: 6e74 2d64 7269 7665 6e20 7072 6f67 7261  nt-driven progra
-00002220: 6d6d 696e 672e 204c 6574 2773 2072 6563  mming. Let's rec
-00002230: 6170 2074 6865 2065 7373 656e 7469 616c  ap the essential
-00002240: 2073 7465 7073 2069 6e76 6f6c 7665 643a   steps involved:
-00002250: 0a3c 2f70 3e0a 0a3c 6f6c 2073 7479 6c65  .</p>..<ol style
-00002260: 3d27 7465 7874 2d61 6c69 676e 3a20 6a75  ='text-align: ju
-00002270: 7374 6966 793b 273e 0a0a 3c6c 693e 0a3c  stify;'>..<li>.<
-00002280: 623e 4465 6669 6e69 6e67 2074 6865 2065  b>Defining the e
-00002290: 7665 6e74 2068 616e 646c 6572 2063 616c  vent handler cal
-000022a0: 6c62 6163 6b3a 3c2f 623e 2057 6520 6465  lback:</b> We de
-000022b0: 6669 6e65 6420 7468 6520 6675 6e63 7469  fined the functi
-000022c0: 6f6e 203c 636f 6465 3e65 7665 6e74 5f63  on <code>event_c
-000022d0: 616c 6c62 6163 6b28 293c 2f63 6f64 653e  allback()</code>
-000022e0: 2061 6e64 2075 7365 6420 7468 6520 0a3c   and used the .<
-000022f0: 636f 6465 3e40 4576 656e 744c 696e 6b65  code>@EventLinke
-00002300: 722e 6f6e 2829 3c2f 636f 6465 3e20 6465  r.on()</code> de
-00002310: 636f 7261 746f 7220 746f 2061 7373 6f63  corator to assoc
-00002320: 6961 7465 2069 7420 7769 7468 2074 6865  iate it with the
-00002330: 2073 7472 696e 6720 6576 656e 7420 3c63   string event <c
-00002340: 6f64 653e 4d79 4576 656e 743c 2f63 6f64  ode>MyEvent</cod
-00002350: 653e 2e20 5468 6973 2064 6563 6f72 6174  e>. This decorat
-00002360: 6f72 0a69 6e64 6963 6174 6573 2074 6861  or.indicates tha
-00002370: 7420 7468 6520 6675 6e63 7469 6f6e 2073  t the function s
-00002380: 686f 756c 6420 6265 2074 7269 6767 6572  hould be trigger
-00002390: 6564 2077 6865 6e20 3c63 6f64 653e 4d79  ed when <code>My
-000023a0: 4576 656e 743c 2f63 6f64 653e 206f 6363  Event</code> occ
-000023b0: 7572 732e 0a3c 2f6c 693e 0a0a 3c6c 693e  urs..</li>..<li>
-000023c0: 0a3c 623e 4372 6561 7469 6e67 2074 6865  .<b>Creating the
-000023d0: 2065 7665 6e74 2065 6d69 7474 6572 2069   event emitter i
-000023e0: 6e73 7461 6e63 653a 3c2f 623e 2057 6520  nstance:</b> We 
-000023f0: 696e 7374 616e 7469 6174 6564 2074 6865  instantiated the
-00002400: 203c 636f 6465 3e41 7379 6e63 494f 4576   <code>AsyncIOEv
-00002410: 656e 7445 6d69 7474 6572 3c2f 636f 6465  entEmitter</code
-00002420: 3e20 636c 6173 732c 2077 6869 6368 2061  > class, which a
-00002430: 6374 7320 6173 200a 7468 6520 6576 656e  cts as .the even
-00002440: 7420 656d 6974 7465 7220 7265 7370 6f6e  t emitter respon
-00002450: 7369 626c 6520 666f 7220 6469 7370 6174  sible for dispat
-00002460: 6368 696e 6720 6576 656e 7473 2061 6e64  ching events and
-00002470: 2069 6e76 6f6b 696e 6720 7468 6520 6173   invoking the as
-00002480: 736f 6369 6174 6564 2065 7665 6e74 2068  sociated event h
-00002490: 616e 646c 6572 2063 616c 6c62 6163 6b73  andler callbacks
-000024a0: 2e20 4974 2773 2069 6d70 6f72 7461 6e74  . It's important
-000024b0: 200a 746f 206e 6f74 6520 7468 6174 2074   .to note that t
-000024c0: 6865 2065 7665 6e74 2065 6d69 7474 6572  he event emitter
-000024d0: 2075 7365 6420 6361 6e20 6265 2063 6861   used can be cha
-000024e0: 6e67 6564 2062 7920 616e 7920 6f66 2074  nged by any of t
-000024f0: 6865 2062 7569 6c74 2d69 6e20 6f72 2063  he built-in or c
-00002500: 7573 746f 6d20 6576 656e 7420 656d 6974  ustom event emit
-00002510: 7465 7220 696d 706c 656d 656e 7461 7469  ter implementati
-00002520: 6f6e 732e 0a3c 2f6c 693e 0a0a 3c6c 693e  ons..</li>..<li>
-00002530: 0a3c 623e 456d 6974 7469 6e67 2074 6865  .<b>Emitting the
-00002540: 2065 7665 6e74 3a3c 2f62 3e20 4279 2075   event:</b> By u
-00002550: 7469 6c69 7a69 6e67 2074 6865 203c 636f  tilizing the <co
-00002560: 6465 3e65 6d69 7428 293c 2f63 6f64 653e  de>emit()</code>
-00002570: 206d 6574 686f 6420 6f66 2074 6865 2065   method of the e
-00002580: 7665 6e74 2065 6d69 7474 6572 2c20 7765  vent emitter, we
-00002590: 2065 6d69 7474 6564 2074 6865 2073 7472   emitted the str
-000025a0: 696e 6720 0a65 7665 6e74 203c 636f 6465  ing .event <code
-000025b0: 3e4d 7945 7665 6e74 3c2f 636f 6465 3e2e  >MyEvent</code>.
-000025c0: 2054 6869 7320 6163 7469 6f6e 2073 7562   This action sub
-000025d0: 7365 7175 656e 746c 7920 6578 6563 7574  sequently execut
-000025e0: 6520 7468 6520 7265 6769 7374 6572 6564  e the registered
-000025f0: 2065 7665 6e74 2068 616e 646c 6572 2063   event handler c
-00002600: 616c 6c62 6163 6b73 2c20 7768 6963 6820  allbacks, which 
-00002610: 696e 2074 6869 7320 6361 7365 0a69 7320  in this case.is 
-00002620: 7468 6520 3c63 6f64 653e 6576 656e 745f  the <code>event_
-00002630: 6361 6c6c 6261 636b 2829 3c2f 636f 6465  callback()</code
-00002640: 3e2e 0a3c 2f6c 693e 0a0a 3c2f 6f6c 3e0a  >..</li>..</ol>.
-00002650: 0a3c 7020 7374 796c 653d 2774 6578 742d  .<p style='text-
-00002660: 616c 6967 6e3a 206a 7573 7469 6679 3b27  align: justify;'
-00002670: 3e0a 2020 2020 2665 6d73 703b 2665 6d73  >.    &emsp;&ems
-00002680: 703b 4861 7669 6e67 2067 6169 6e65 6420  p;Having gained 
-00002690: 6120 636c 6561 7220 756e 6465 7273 7461  a clear understa
-000026a0: 6e64 696e 6720 6f66 2074 6865 2077 6f72  nding of the wor
-000026b0: 6b66 6c6f 7720 7368 6f77 6361 7365 6420  kflow showcased 
-000026c0: 696e 2074 6865 203c 636f 6465 3e48 656c  in the <code>Hel
-000026d0: 6c6f 2c20 576f 726c 6421 3c2f 636f 6465  lo, World!</code
-000026e0: 3e20 6578 616d 706c 652c 0a09 796f 7520  > example,..you 
-000026f0: 6172 6520 6e6f 7720 7765 6c6c 2d65 7175  are now well-equ
-00002700: 6970 7065 6420 746f 2065 7870 6c6f 7265  ipped to explore
-00002710: 206d 6f72 6520 696e 7472 6963 6174 6520   more intricate 
-00002720: 6576 656e 742d 6472 6976 656e 2073 6365  event-driven sce
-00002730: 6e61 7269 6f73 2061 6e64 2066 756c 6c79  narios and fully
-00002740: 2068 6172 6e65 7373 2074 6865 2063 6170   harness the cap
-00002750: 6162 696c 6974 6965 7320 6f66 200a 0950  abilities of ..P
-00002760: 7976 656e 7475 7320 696e 2079 6f75 7220  yventus in your 
-00002770: 6f77 6e20 7072 6f6a 6563 7473 2e0a 3c2f  own projects..</
-00002780: 703e 0a0a 2323 2053 7570 706f 7274 2066  p>..## Support f
-00002790: 6f72 2053 796e 6368 726f 6e6f 7573 2061  or Synchronous a
-000027a0: 6e64 2041 7379 6e63 6872 6f6e 6f75 7320  nd Asynchronous 
-000027b0: 636f 6465 0a0a 3c70 2073 7479 6c65 3d27  code..<p style='
-000027c0: 7465 7874 2d61 6c69 676e 3a20 6a75 7374  text-align: just
-000027d0: 6966 793b 273e 0a20 2020 2026 656d 7370  ify;'>.    &emsp
-000027e0: 3b26 656d 7370 3b50 7976 656e 7475 7320  ;&emsp;Pyventus 
-000027f0: 6973 2064 6573 6967 6e65 6420 6672 6f6d  is designed from
-00002800: 2074 6865 2067 726f 756e 6420 7570 2074   the ground up t
-00002810: 6f20 7365 616d 6c65 7373 6c79 2073 7570  o seamlessly sup
-00002820: 706f 7274 2062 6f74 6820 7379 6e63 6872  port both synchr
-00002830: 6f6e 6f75 7320 616e 6420 6173 796e 6368  onous and asynch
-00002840: 726f 6e6f 7573 0a09 7072 6f67 7261 6d6d  ronous..programm
-00002850: 696e 6720 6d6f 6465 6c73 2e20 4974 7320  ing models. Its 
-00002860: 756e 6966 6965 6420 7379 6e63 2f61 7379  unified sync/asy
-00002870: 6e63 2041 5049 2061 6c6c 6f77 7320 796f  nc API allows yo
-00002880: 7520 746f 2064 6566 696e 6520 6576 656e  u to define even
-00002890: 7420 6861 6e64 6c65 7220 6361 6c6c 6261  t handler callba
-000028a0: 636b 7320 616e 6420 656d 6974 2065 7665  cks and emit eve
-000028b0: 6e74 730a 0961 6372 6f73 7320 3c63 6f64  nts..across <cod
-000028c0: 653e 7379 6e63 3c2f 636f 6465 3e20 616e  e>sync</code> an
-000028d0: 6420 3c63 6f64 653e 6173 796e 633c 2f63  d <code>async</c
-000028e0: 6f64 653e 2063 6f6e 7465 7874 732e 204c  ode> contexts. L
-000028f0: 6574 2773 2074 616b 6520 6120 6c6f 6f6b  et's take a look
-00002900: 2061 7420 736f 6d65 2075 7365 2063 6173   at some use cas
-00002910: 6573 2074 6861 7420 696c 6c75 7374 7261  es that illustra
-00002920: 7465 200a 0968 6f77 2074 6865 2041 5049  te ..how the API
-00002930: 2068 616e 646c 6573 2065 7665 6e74 2072   handles event r
-00002940: 6567 6973 7472 6174 696f 6e20 616e 6420  egistration and 
-00002950: 6469 7370 6174 6368 2074 7261 6e73 7061  dispatch transpa
-00002960: 7265 6e74 6c79 2e0a 3c2f 703e 0a0a 2323  rently..</p>..##
-00002970: 2320 5265 6769 7374 6572 696e 6720 4576  # Registering Ev
-00002980: 656e 7420 4861 6e64 6c65 7273 2061 7320  ent Handlers as 
-00002990: 3c63 6f64 653e 5379 6e63 3c2f 636f 6465  <code>Sync</code
-000029a0: 3e20 616e 6420 3c63 6f64 653e 4173 796e  > and <code>Asyn
-000029b0: 633c 2f63 6f64 653e 2043 616c 6c62 6163  c</code> Callbac
-000029c0: 6b73 0a0a 6060 6050 7974 686f 6e20 0a40  ks..```Python .@
-000029d0: 4576 656e 744c 696e 6b65 722e 6f6e 2822  EventLinker.on("
-000029e0: 4d79 4576 656e 7422 290a 6465 6620 7379  MyEvent").def sy
-000029f0: 6e63 5f65 7665 6e74 5f63 616c 6c62 6163  nc_event_callbac
-00002a00: 6b28 293a 0a20 2020 2023 2053 796e 6368  k():.    # Synch
-00002a10: 726f 6e6f 7573 2065 7665 6e74 2068 616e  ronous event han
-00002a20: 646c 696e 670a 2020 2020 7072 696e 7428  dling.    print(
-00002a30: 2245 7665 6e74 2072 6563 6569 7665 6421  "Event received!
-00002a40: 2229 0a0a 0a40 4576 656e 744c 696e 6b65  ")...@EventLinke
-00002a50: 722e 6f6e 2822 4d79 4576 656e 7422 290a  r.on("MyEvent").
-00002a60: 6173 796e 6320 6465 6620 6173 796e 635f  async def async_
-00002a70: 6576 656e 745f 6361 6c6c 6261 636b 2829  event_callback()
-00002a80: 3a0a 2020 2020 2320 4173 796e 6368 726f  :.    # Asynchro
-00002a90: 6e6f 7573 2065 7665 6e74 2068 616e 646c  nous event handl
-00002aa0: 696e 670a 2020 2020 7072 696e 7428 2245  ing.    print("E
-00002ab0: 7665 6e74 2072 6563 6569 7665 6421 2229  vent received!")
-00002ac0: 2020 0a60 6060 0a0a 2323 2320 456d 6974    .```..### Emit
-00002ad0: 7469 6e67 2045 7665 6e74 7320 6672 6f6d  ting Events from
-00002ae0: 203c 636f 6465 3e53 796e 633c 2f63 6f64   <code>Sync</cod
-00002af0: 653e 2061 6e64 203c 636f 6465 3e41 7379  e> and <code>Asy
-00002b00: 6e63 3c2f 636f 6465 3e20 436f 6e74 6578  nc</code> Contex
-00002b10: 7473 0a0a 6060 6050 7974 686f 6e20 0a23  ts..```Python .#
-00002b20: 2045 6d69 7474 696e 6720 616e 2065 7665   Emitting an eve
-00002b30: 6e74 2077 6974 6869 6e20 6120 7379 6e63  nt within a sync
-00002b40: 2066 756e 6374 696f 6e0a 6465 6620 7379   function.def sy
-00002b50: 6e63 5f66 756e 6374 696f 6e28 6576 656e  nc_function(even
-00002b60: 745f 656d 6974 7465 723a 2045 7665 6e74  t_emitter: Event
-00002b70: 456d 6974 7465 7229 3a0a 2020 2020 6576  Emitter):.    ev
-00002b80: 656e 745f 656d 6974 7465 722e 656d 6974  ent_emitter.emit
-00002b90: 2822 4d79 4576 656e 7422 290a 0a0a 2320  ("MyEvent")...# 
-00002ba0: 456d 6974 7469 6e67 2061 6e20 6576 656e  Emitting an even
-00002bb0: 7420 7769 7468 696e 2061 6e20 6173 796e  t within an asyn
-00002bc0: 6320 6675 6e63 7469 6f6e 0a61 7379 6e63  c function.async
-00002bd0: 2064 6566 2061 7379 6e63 5f66 756e 6374   def async_funct
-00002be0: 696f 6e28 6576 656e 745f 656d 6974 7465  ion(event_emitte
-00002bf0: 723a 2045 7665 6e74 456d 6974 7465 7229  r: EventEmitter)
-00002c00: 3a0a 2020 2020 6576 656e 745f 656d 6974  :.    event_emit
-00002c10: 7465 722e 656d 6974 2822 4d79 4576 656e  ter.emit("MyEven
-00002c20: 7422 290a 6060 600a 0a3c 6465 7461 696c  t").```..<detail
-00002c30: 7320 6d61 726b 646f 776e 3d22 3122 2063  s markdown="1" c
-00002c40: 6c61 7373 3d22 696e 666f 2220 6f70 656e  lass="info" open
-00002c50: 3e0a 3c73 756d 6d61 7279 3e45 7665 6e74  >.<summary>Event
-00002c60: 2050 726f 7061 6761 7469 6f6e 2057 6974   Propagation Wit
-00002c70: 6869 6e20 4469 6666 6572 656e 7420 436f  hin Different Co
-00002c80: 6e74 6578 7473 3c2f 7375 6d6d 6172 793e  ntexts</summary>
-00002c90: 0a0a 3c70 2073 7479 6c65 3d27 7465 7874  ..<p style='text
-00002ca0: 2d61 6c69 676e 3a20 6a75 7374 6966 793b  -align: justify;
-00002cb0: 273e 0a20 2020 2026 656d 7370 3b26 656d  '>.    &emsp;&em
-00002cc0: 7370 3b57 6869 6c65 2050 7976 656e 7475  sp;While Pyventu
-00002cd0: 7320 7072 6f76 6964 6573 2061 2062 6173  s provides a bas
-00002ce0: 6520 3c63 6f64 653e 4576 656e 7445 6d69  e <code>EventEmi
-00002cf0: 7474 6572 3c2f 636f 6465 3e20 636c 6173  tter</code> clas
-00002d00: 7320 7769 7468 2061 2075 6e69 6669 6564  s with a unified
-00002d10: 2073 796e 632f 6173 796e 6320 4150 492c   sync/async API,
-00002d20: 2074 6865 200a 0973 7065 6369 6669 6320   the ..specific 
-00002d30: 7072 6f70 6167 6174 696f 6e20 6265 6861  propagation beha
-00002d40: 7669 6f72 2077 6865 6e20 656d 6974 7469  vior when emitti
-00002d50: 6e67 2065 7665 6e74 7320 6d61 7920 7661  ng events may va
-00002d60: 7279 2064 6570 656e 6469 6e67 206f 6e20  ry depending on 
-00002d70: 7468 6520 636f 6e63 7265 7465 203c 636f  the concrete <co
-00002d80: 6465 3e45 7665 6e74 456d 6974 7465 723c  de>EventEmitter<
-00002d90: 2f63 6f64 653e 0a09 7573 6564 2e20 466f  /code>..used. Fo
-00002da0: 7220 6578 616d 706c 652c 2074 6865 203c  r example, the <
-00002db0: 636f 6465 3e41 7379 6e63 494f 4576 656e  code>AsyncIOEven
-00002dc0: 7445 6d69 7474 6572 3c2f 636f 6465 3e20  tEmitter</code> 
-00002dd0: 696d 706c 656d 656e 7461 7469 6f6e 206c  implementation l
-00002de0: 6576 6572 6167 6573 2074 6865 203c 636f  everages the <co
-00002df0: 6465 3e41 7379 6e63 494f 3c2f 636f 6465  de>AsyncIO</code
-00002e00: 3e20 6576 656e 740a 096c 6f6f 7020 746f  > event..loop to
-00002e10: 2073 6368 6564 756c 6520 6361 6c6c 6261   schedule callba
-00002e20: 636b 7320 6164 6465 6420 6672 6f6d 2061  cks added from a
-00002e30: 7379 6e63 6872 6f6e 6f75 7320 636f 6e74  synchronous cont
-00002e40: 6578 7473 2077 6974 686f 7574 2062 6c6f  exts without blo
-00002e50: 636b 696e 672e 2042 7574 2061 6c74 6572  cking. But alter
-00002e60: 6e61 7469 7665 2065 6d69 7474 6572 7320  native emitters 
-00002e70: 636f 756c 6420 0a09 7374 7275 6374 7572  could ..structur
-00002e80: 6520 7072 6f70 6167 6174 696f 6e20 6469  e propagation di
-00002e90: 6666 6572 656e 746c 7920 746f 2073 7569  fferently to sui
-00002ea0: 7420 7468 6569 7220 6e65 6564 732e 0a3c  t their needs..<
-00002eb0: 2f70 3e0a 0a3c 2f64 6574 6169 6c73 3e0a  /p>..</details>.
-00002ec0: 0a23 2320 5275 6e74 696d 6520 466c 6578  .## Runtime Flex
-00002ed0: 6962 696c 6974 7920 616e 6420 4375 7374  ibility and Cust
-00002ee0: 6f6d 697a 6174 696f 6e0a 0a3c 7020 7374  omization..<p st
-00002ef0: 796c 653d 2774 6578 742d 616c 6967 6e3a  yle='text-align:
-00002f00: 206a 7573 7469 6679 3b27 3e0a 2020 2020   justify;'>.    
-00002f10: 2665 6d73 703b 2665 6d73 703b 4174 2069  &emsp;&emsp;At i
-00002f20: 7473 2063 6f72 652c 2050 7976 656e 7475  ts core, Pyventu
-00002f30: 7320 7574 696c 697a 6573 2061 206d 6f64  s utilizes a mod
-00002f40: 756c 6172 2065 7665 6e74 2065 6d69 7474  ular event emitt
-00002f50: 6572 2064 6573 6967 6e20 7468 6174 2061  er design that a
-00002f60: 6c6c 6f77 7320 796f 7520 746f 2073 7769  llows you to swi
-00002f70: 7463 6820 7365 616d 6c65 7373 6c79 0a09  tch seamlessly..
-00002f80: 6265 7477 6565 6e20 6469 6666 6572 656e  between differen
-00002f90: 7420 6275 696c 742d 696e 206f 7220 6375  t built-in or cu
-00002fa0: 7374 6f6d 2065 7665 6e74 2065 6d69 7474  stom event emitt
-00002fb0: 6572 2069 6d70 6c65 6d65 6e74 6174 696f  er implementatio
-00002fc0: 6e73 206f 6e20 7468 6520 666c 792e 2057  ns on the fly. W
-00002fd0: 6865 7468 6572 2079 6f75 206f 7074 2066  hether you opt f
-00002fe0: 6f72 206f 6666 6963 6961 6c0a 0965 6d69  or official..emi
-00002ff0: 7474 6572 7320 6f72 2064 6563 6964 6520  tters or decide 
-00003000: 746f 2063 7265 6174 6520 796f 7572 2063  to create your c
-00003010: 7573 746f 6d20 6f6e 6573 2c20 5079 7665  ustom ones, Pyve
-00003020: 6e74 7573 2061 6c6c 6f77 7320 796f 7520  ntus allows you 
-00003030: 746f 2074 6169 6c6f 7220 7468 6520 6265  to tailor the be
-00003040: 6861 7669 6f72 2061 6e64 2063 6170 6162  havior and capab
-00003050: 696c 6974 6965 730a 096f 6620 7468 6520  ilities..of the 
-00003060: 6576 656e 7420 656d 6974 7465 7273 2074  event emitters t
-00003070: 6f20 7065 7266 6563 746c 7920 616c 6967  o perfectly alig
-00003080: 6e20 7769 7468 2079 6f75 7220 756e 6971  n with your uniq
-00003090: 7565 2072 6571 7569 7265 6d65 6e74 732e  ue requirements.
-000030a0: 0a3c 2f70 3e0a 0a3c 7020 7374 796c 653d  .</p>..<p style=
-000030b0: 2774 6578 742d 616c 6967 6e3a 206a 7573  'text-align: jus
-000030c0: 7469 6679 3b27 3e0a 2020 2020 2665 6d73  tify;'>.    &ems
-000030d0: 703b 2665 6d73 703b 4279 206c 6576 6572  p;&emsp;By lever
-000030e0: 6167 696e 6720 7468 6520 7072 696e 6369  aging the princi
-000030f0: 706c 6573 206f 6620 6465 7065 6e64 656e  ples of dependen
-00003100: 6379 2069 6e76 6572 7369 6f6e 2061 6e64  cy inversion and
-00003110: 206f 7065 6e2d 636c 6f73 652c 2050 7976   open-close, Pyv
-00003120: 656e 7475 7320 6465 636f 7570 6c65 7320  entus decouples 
-00003130: 7468 6520 6576 656e 740a 0965 6d69 7373  the event..emiss
-00003140: 696f 6e20 7072 6f63 6573 7320 6672 6f6d  ion process from
-00003150: 2074 6865 2075 6e64 6572 6c79 696e 6720   the underlying 
-00003160: 696d 706c 656d 656e 7461 7469 6f6e 2074  implementation t
-00003170: 6861 7420 6861 6e64 6c65 7320 7468 6520  hat handles the 
-00003180: 6576 656e 7420 656d 6973 7369 6f6e 2061  event emission a
-00003190: 6e64 2065 6e61 626c 6573 2079 6f75 2c20  nd enables you, 
-000031a0: 696e 2063 6f6e 6a75 6e63 7469 6f6e 0a09  in conjunction..
-000031b0: 7769 7468 2074 6865 203c 636f 6465 3e45  with the <code>E
-000031c0: 7665 6e74 4c69 6e6b 6572 3c2f 636f 6465  ventLinker</code
-000031d0: 3e2c 2074 6f20 6368 616e 6765 2074 6865  >, to change the
-000031e0: 2065 7665 6e74 2065 6d69 7474 6572 2061   event emitter a
-000031f0: 7420 7275 6e74 696d 6520 7769 7468 6f75  t runtime withou
-00003200: 7420 7468 6520 6e65 6564 2074 6f20 7265  t the need to re
-00003210: 636f 6e66 6967 7572 6520 616c 6c20 0a09  configure all ..
-00003220: 636f 6e6e 6563 7469 6f6e 7320 6f72 2065  connections or e
-00003230: 6d70 6c6f 7920 636f 6d70 6c65 7820 6c6f  mploy complex lo
-00003240: 6769 632e 0a3c 2f70 3e0a 0a23 2323 2053  gic..</p>..### S
-00003250: 6565 696e 6720 6974 2069 6e20 4163 7469  eeing it in Acti
-00003260: 6f6e 0a0a 3c70 2073 7479 6c65 3d27 7465  on..<p style='te
-00003270: 7874 2d61 6c69 676e 3a20 6a75 7374 6966  xt-align: justif
-00003280: 793b 273e 0a20 2020 2026 656d 7370 3b26  y;'>.    &emsp;&
-00003290: 656d 7370 3b4e 6f77 206c 6574 2773 2070  emsp;Now let's p
-000032a0: 7574 2050 7976 656e 7475 7327 2066 6c65  ut Pyventus' fle
-000032b0: 7869 6269 6c69 7479 2074 6f20 7468 6520  xibility to the 
-000032c0: 7465 7374 2077 6974 6820 6120 7072 6163  test with a prac
-000032d0: 7469 6361 6c20 6578 616d 706c 652e 2046  tical example. F
-000032e0: 6972 7374 2c20 7765 276c 6c20 6275 696c  irst, we'll buil
-000032f0: 6420 610a 0963 7573 746f 6d20 3c61 2068  d a..custom <a h
-00003300: 7265 663d 2268 7474 7073 3a2f 2f66 6173  ref="https://fas
-00003310: 7461 7069 2e74 6961 6e67 6f6c 6f2e 636f  tapi.tiangolo.co
-00003320: 6d2f 2220 7461 7267 6574 3d22 5f62 6c61  m/" target="_bla
-00003330: 6e6b 223e 4661 7374 4150 493c 2f61 3e20  nk">FastAPI</a> 
-00003340: 4576 656e 7445 6d69 7474 6572 2074 6f20  EventEmitter to 
-00003350: 7072 6f70 6572 6c79 2068 616e 646c 650a  properly handle.
-00003360: 0974 6865 2065 7665 6e74 2065 6d69 7373  .the event emiss
-00003370: 696f 6e20 7573 696e 6720 7468 6520 6672  ion using the fr
-00003380: 616d 6577 6f72 6b27 7320 3c61 2068 7265  amework's <a hre
-00003390: 663d 2268 7474 7073 3a2f 2f66 6173 7461  f="https://fasta
-000033a0: 7069 2e74 6961 6e67 6f6c 6f2e 636f 6d2f  pi.tiangolo.com/
-000033b0: 7265 6665 7265 6e63 652f 6261 636b 6772  reference/backgr
-000033c0: 6f75 6e64 2f22 2074 6172 6765 743d 225f  ound/" target="_
-000033d0: 626c 616e 6b22 3e42 6163 6b67 726f 756e  blank">Backgroun
-000033e0: 6454 6173 6b73 3c2f 613e 0a09 776f 726b  dTasks</a>..work
-000033f0: 666c 6f77 2e20 5468 656e 2c20 7765 276c  flow. Then, we'l
-00003400: 6c20 696c 6c75 7374 7261 7465 2050 7976  l illustrate Pyv
-00003410: 656e 7475 7327 2064 796e 616d 6963 2063  entus' dynamic c
-00003420: 6170 6162 696c 6974 6965 7320 6279 2073  apabilities by s
-00003430: 7761 7070 696e 6720 7468 6973 2063 7573  wapping this cus
-00003440: 746f 6d20 656d 6974 7465 7220 6f75 7420  tom emitter out 
-00003450: 666f 7220 6120 6275 696c 742d 696e 0a09  for a built-in..
-00003460: 616c 7465 726e 6174 6976 6520 6f6e 2074  alternative on t
-00003470: 6865 2066 6c79 2e0a 3c2f 703e 0a0a 3c70  he fly..</p>..<p
-00003480: 2073 7479 6c65 3d27 7465 7874 2d61 6c69   style='text-ali
-00003490: 676e 3a20 6a75 7374 6966 793b 273e 0a20  gn: justify;'>. 
-000034a0: 2020 2026 656d 7370 3b26 656d 7370 3b54     &emsp;&emsp;T
-000034b0: 6f20 666f 6c6c 6f77 2061 6c6f 6e67 2c20  o follow along, 
-000034c0: 706c 6561 7365 2065 6e73 7572 6520 7468  please ensure th
-000034d0: 6174 2079 6f75 2068 6176 6520 7468 6520  at you have the 
-000034e0: 4661 7374 4150 4920 6672 616d 6577 6f72  FastAPI framewor
-000034f0: 6b20 3c61 2068 7265 663d 2268 7474 7073  k <a href="https
-00003500: 3a2f 2f66 6173 7461 7069 2e74 6961 6e67  ://fastapi.tiang
-00003510: 6f6c 6f2e 636f 6d2f 3f68 3d23 696e 7374  olo.com/?h=#inst
-00003520: 616c 6c61 7469 6f6e 2220 7461 7267 6574  allation" target
-00003530: 3d22 5f62 6c61 6e6b 223e 696e 7374 616c  ="_blank">instal
-00003540: 6c65 643c 2f61 3e2e 200a 094f 6e63 6520  led</a>. ..Once 
-00003550: 7468 6174 2069 7320 636f 6d70 6c65 7465  that is complete
-00003560: 2c20 6c65 7427 7320 6469 7665 2069 6e74  , let's dive int
-00003570: 6f20 7468 6520 7374 6570 2d62 792d 7374  o the step-by-st
-00003580: 6570 2069 6d70 6c65 6d65 6e74 6174 696f  ep implementatio
-00003590: 6e3a 0a3c 2f70 3e0a 0a3c 6f6c 2073 7479  n:.</p>..<ol sty
-000035a0: 6c65 3d27 7465 7874 2d61 6c69 676e 3a20  le='text-align: 
-000035b0: 6a75 7374 6966 793b 273e 0a0a 3c6c 693e  justify;'>..<li>
-000035c0: 0a43 7265 6174 6520 6120 3c63 6f64 653e  .Create a <code>
-000035d0: 6d61 696e 2e70 793c 2f63 6f64 653e 2066  main.py</code> f
-000035e0: 696c 6520 7769 7468 3a0a 0a60 6060 5079  ile with:..```Py
-000035f0: 7468 6f6e 2074 6974 6c65 3d22 6d61 696e  thon title="main
-00003600: 2e70 7922 206c 696e 656e 756d 733d 2231  .py" linenums="1
-00003610: 2220 2068 6c5f 6c69 6e65 733d 2239 2031  "  hl_lines="9 1
-00003620: 362d 3137 2033 3720 3430 220a 6672 6f6d  6-17 37 40".from
-00003630: 2061 7379 6e63 696f 2069 6d70 6f72 7420   asyncio import 
-00003640: 736c 6565 700a 6672 6f6d 2072 616e 646f  sleep.from rando
-00003650: 6d20 696d 706f 7274 2072 616e 6469 6e74  m import randint
-00003660: 0a0a 6672 6f6d 2066 6173 7461 7069 2069  ..from fastapi i
-00003670: 6d70 6f72 7420 4261 636b 6772 6f75 6e64  mport Background
-00003680: 5461 736b 732c 2046 6173 7441 5049 0a0a  Tasks, FastAPI..
-00003690: 6672 6f6d 2070 7976 656e 7475 7320 696d  from pyventus im
-000036a0: 706f 7274 2045 7665 6e74 456d 6974 7465  port EventEmitte
-000036b0: 722c 2045 7665 6e74 4c69 6e6b 6572 2c20  r, EventLinker, 
-000036c0: 4173 796e 6349 4f45 7665 6e74 456d 6974  AsyncIOEventEmit
-000036d0: 7465 720a 0a0a 636c 6173 7320 4661 7374  ter...class Fast
-000036e0: 4150 4945 7665 6e74 456d 6974 7465 7228  APIEventEmitter(
-000036f0: 4576 656e 7445 6d69 7474 6572 293a 0a20  EventEmitter):. 
-00003700: 2020 2022 2222 4375 7374 6f6d 2065 7665     """Custom eve
-00003710: 6e74 2065 6d69 7474 6572 2063 6c61 7373  nt emitter class
-00003720: 2074 6861 7420 6c65 7665 7261 6765 7320   that leverages 
-00003730: 7468 6520 4661 7374 4150 4927 7320 6173  the FastAPI's as
-00003740: 796e 6368 726f 6e6f 7573 2077 6f72 6b66  ynchronous workf
-00003750: 6c6f 772e 2222 220a 0a20 2020 2064 6566  low."""..    def
-00003760: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-00003770: 6261 636b 6772 6f75 6e64 5f74 6173 6b73  background_tasks
-00003780: 3a20 4261 636b 6772 6f75 6e64 5461 736b  : BackgroundTask
-00003790: 7329 3a0a 2020 2020 2020 2020 7375 7065  s):.        supe
-000037a0: 7228 292e 5f5f 696e 6974 5f5f 2829 0a20  r().__init__(). 
-000037b0: 2020 2020 2020 2073 656c 662e 5f62 6163         self._bac
-000037c0: 6b67 726f 756e 645f 7461 736b 7320 3d20  kground_tasks = 
-000037d0: 6261 636b 6772 6f75 6e64 5f74 6173 6b73  background_tasks
-000037e0: 2020 2320 5374 6f72 6520 7468 6520 4661    # Store the Fa
-000037f0: 7374 4150 4920 6261 636b 6772 6f75 6e64  stAPI background
-00003800: 2074 6173 6b73 206f 626a 6563 740a 0a20   tasks object.. 
-00003810: 2020 2064 6566 205f 7072 6f63 6573 7328     def _process(
-00003820: 7365 6c66 2c20 6576 656e 745f 656d 6973  self, event_emis
-00003830: 7369 6f6e 3a20 4576 656e 7445 6d69 7474  sion: EventEmitt
-00003840: 6572 2e45 7665 6e74 456d 6973 7369 6f6e  er.EventEmission
-00003850: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00003860: 2020 2073 656c 662e 5f62 6163 6b67 726f     self._backgro
-00003870: 756e 645f 7461 736b 732e 6164 645f 7461  und_tasks.add_ta
-00003880: 736b 2865 7665 6e74 5f65 6d69 7373 696f  sk(event_emissio
-00003890: 6e29 2020 2320 4578 6563 7574 6520 7468  n)  # Execute th
-000038a0: 6520 6576 656e 7420 656d 6973 7369 6f6e  e event emission
-000038b0: 2061 7320 6261 636b 6772 6f75 6e64 2074   as background t
-000038c0: 6173 6b73 0a0a 0a40 4576 656e 744c 696e  asks...@EventLin
-000038d0: 6b65 722e 6f6e 2822 636f 6e73 6f6c 655f  ker.on("console_
-000038e0: 7072 696e 7422 290a 6173 796e 6320 6465  print").async de
-000038f0: 6620 636f 6e73 6f6c 655f 7072 696e 7428  f console_print(
-00003900: 6d65 7373 6167 653a 2073 7472 293a 0a20  message: str):. 
-00003910: 2020 2061 7761 6974 2073 6c65 6570 2872     await sleep(r
-00003920: 616e 6469 6e74 2830 2c20 3329 2920 2023  andint(0, 3))  #
-00003930: 2053 696d 756c 6174 6520 6120 7261 6e64   Simulate a rand
-00003940: 6f6d 2064 656c 6179 0a20 2020 2070 7269  om delay.    pri
-00003950: 6e74 286d 6573 7361 6765 290a 0a0a 6170  nt(message)...ap
-00003960: 7020 3d20 4661 7374 4150 4928 290a 0a0a  p = FastAPI()...
-00003970: 4061 7070 2e67 6574 2822 2f70 7269 6e74  @app.get("/print
-00003980: 2229 0a61 7379 6e63 2064 6566 2063 6f6e  ").async def con
-00003990: 736f 6c65 5f70 7269 6e74 5f65 6e64 706f  sole_print_endpo
-000039a0: 696e 7428 6261 636b 6772 6f75 6e64 5f74  int(background_t
-000039b0: 6173 6b73 3a20 4261 636b 6772 6f75 6e64  asks: Background
-000039c0: 5461 736b 7329 3a0a 2020 2020 2222 2246  Tasks):.    """F
-000039d0: 6173 7441 5049 2065 6e64 706f 696e 7420  astAPI endpoint 
-000039e0: 7468 6174 2074 7269 6767 6572 7320 7468  that triggers th
-000039f0: 6520 636f 6e73 6f6c 655f 7072 696e 7420  e console_print 
-00003a00: 6576 656e 742e 2222 220a 0a20 2020 2064  event."""..    d
-00003a10: 6566 2063 6f6e 736f 6c65 5f70 7269 6e74  ef console_print
-00003a20: 5f61 7070 5f73 6572 7669 6365 2865 7665  _app_service(eve
-00003a30: 6e74 5f65 6d69 7474 6572 3a20 4576 656e  nt_emitter: Even
-00003a40: 7445 6d69 7474 6572 2920 2d3e 204e 6f6e  tEmitter) -> Non
-00003a50: 653a 0a20 2020 2020 2020 2065 7665 6e74  e:.        event
-00003a60: 5f65 6d69 7474 6572 2e65 6d69 7428 2263  _emitter.emit("c
-00003a70: 6f6e 736f 6c65 5f70 7269 6e74 222c 206d  onsole_print", m
-00003a80: 6573 7361 6765 3d66 225c 6e48 656c 6c6f  essage=f"\nHello
-00003a90: 2c20 7b65 7665 6e74 5f65 6d69 7474 6572  , {event_emitter
-00003aa0: 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e 616d  .__class__.__nam
-00003ab0: 655f 5f7d 2122 290a 0a20 2020 2023 2045  e__}!")..    # E
-00003ac0: 6d69 7420 7468 6520 636f 6e73 6f6c 655f  mit the console_
-00003ad0: 7072 696e 7420 6576 656e 7420 7573 696e  print event usin
-00003ae0: 6720 4661 7374 4150 4945 7665 6e74 456d  g FastAPIEventEm
-00003af0: 6974 7465 720a 2020 2020 636f 6e73 6f6c  itter.    consol
-00003b00: 655f 7072 696e 745f 6170 705f 7365 7276  e_print_app_serv
-00003b10: 6963 6528 6576 656e 745f 656d 6974 7465  ice(event_emitte
-00003b20: 723d 4661 7374 4150 4945 7665 6e74 456d  r=FastAPIEventEm
-00003b30: 6974 7465 7228 6261 636b 6772 6f75 6e64  itter(background
-00003b40: 5f74 6173 6b73 2929 0a0a 2020 2020 2320  _tasks))..    # 
-00003b50: 456d 6974 2074 6865 2063 6f6e 736f 6c65  Emit the console
-00003b60: 5f70 7269 6e74 2065 7665 6e74 2075 7369  _print event usi
-00003b70: 6e67 2041 7379 6e63 494f 4576 656e 7445  ng AsyncIOEventE
-00003b80: 6d69 7474 6572 0a20 2020 2063 6f6e 736f  mitter.    conso
-00003b90: 6c65 5f70 7269 6e74 5f61 7070 5f73 6572  le_print_app_ser
-00003ba0: 7669 6365 2865 7665 6e74 5f65 6d69 7474  vice(event_emitt
-00003bb0: 6572 3d41 7379 6e63 494f 4576 656e 7445  er=AsyncIOEventE
-00003bc0: 6d69 7474 6572 2829 290a 0a20 2020 2072  mitter())..    r
-00003bd0: 6574 7572 6e20 7b22 6d65 7373 6167 6522  eturn {"message"
-00003be0: 3a20 2243 6f6e 736f 6c65 2070 7269 6e74  : "Console print
-00003bf0: 2074 7269 6767 6572 6564 2122 7d0a 6060   triggered!"}.``
-00003c00: 600a 0a3c 2f6c 693e 200a 0a0a 0a3c 6c69  `..</li> ....<li
-00003c10: 3e0a 3c61 2068 7265 663d 2268 7474 7073  >.<a href="https
-00003c20: 3a2f 2f66 6173 7461 7069 2e74 6961 6e67  ://fastapi.tiang
-00003c30: 6f6c 6f2e 636f 6d2f 2372 756e 2d69 7422  olo.com/#run-it"
-00003c40: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
-00003c50: 3e52 756e 2074 6865 2073 6572 7665 723c  >Run the server<
-00003c60: 2f61 3e20 7769 7468 3a0a 0a60 6060 636f  /a> with:..```co
-00003c70: 6e73 6f6c 650a 7576 6963 6f72 6e20 6d61  nsole.uvicorn ma
-00003c80: 696e 3a61 7070 202d 2d72 656c 6f61 640a  in:app --reload.
-00003c90: 6060 600a 0a3c 2f6c 693e 0a0a 3c6c 693e  ```..</li>..<li>
-00003ca0: 0a4f 7065 6e20 796f 7572 2062 726f 7773  .Open your brows
-00003cb0: 6572 2061 7420 3c61 2068 7265 663d 2268  er at <a href="h
-00003cc0: 7474 703a 2f2f 3132 372e 302e 302e 313a  ttp://127.0.0.1:
-00003cd0: 3830 3030 2f70 7269 6e74 2220 7461 7267  8000/print" targ
-00003ce0: 6574 3d22 5f62 6c61 6e6b 223e 6874 7470  et="_blank">http
-00003cf0: 3a2f 2f31 3237 2e30 2e30 2e31 3a38 3030  ://127.0.0.1:800
-00003d00: 302f 7072 696e 743c 2f61 3e2e 2059 6f75  0/print</a>. You
-00003d10: 2077 696c 6c20 0a73 6565 2074 6865 204a   will .see the J
-00003d20: 534f 4e20 7265 7370 6f6e 7365 2061 733a  SON response as:
-00003d30: 0a0a 6060 604a 534f 4e0a 7b20 226d 6573  ..```JSON.{ "mes
-00003d40: 7361 6765 223a 2022 436f 6e73 6f6c 6520  sage": "Console 
-00003d50: 7072 696e 7420 7472 6967 6765 7265 6421  print triggered!
-00003d60: 2220 7d0a 6060 600a 0a59 6f75 276c 6c20  " }.```..You'll 
-00003d70: 616c 736f 2062 6520 6162 6c65 2074 6f20  also be able to 
-00003d80: 7365 6520 7468 6520 6f75 7470 7574 7320  see the outputs 
-00003d90: 6f66 2074 6865 2065 7665 6e74 2065 6d69  of the event emi
-00003da0: 7474 6572 7320 696e 2074 6865 2063 6f6e  tters in the con
-00003db0: 736f 6c65 206c 6f67 7320 6173 3a0a 0a60  sole logs as:..`
-00003dc0: 6060 636f 6e73 6f6c 650a 494e 464f 3a20  ``console.INFO: 
-00003dd0: 2020 2020 5576 6963 6f72 6e20 7275 6e6e      Uvicorn runn
-00003de0: 696e 6720 6f6e 2068 7474 703a 2f2f 3132  ing on http://12
-00003df0: 372e 302e 302e 313a 3830 3030 2028 5072  7.0.0.1:8000 (Pr
-00003e00: 6573 7320 4354 524c 2b43 2074 6f20 7175  ess CTRL+C to qu
-00003e10: 6974 290a 494e 464f 3a20 2020 2020 5374  it).INFO:     St
-00003e20: 6172 7465 6420 7265 6c6f 6164 6572 2070  arted reloader p
-00003e30: 726f 6365 7373 205b 3238 3732 305d 0a49  rocess [28720].I
-00003e40: 4e46 4f3a 2020 2020 2053 7461 7274 6564  NFO:     Started
-00003e50: 2073 6572 7665 7220 7072 6f63 6573 7320   server process 
-00003e60: 5b32 3837 3232 5d0a 494e 464f 3a20 2020  [28722].INFO:   
-00003e70: 2020 5761 6974 696e 6720 666f 7220 6170    Waiting for ap
-00003e80: 706c 6963 6174 696f 6e20 7374 6172 7475  plication startu
-00003e90: 702e 0a49 4e46 4f3a 2020 2020 2041 7070  p..INFO:     App
-00003ea0: 6c69 6361 7469 6f6e 2073 7461 7274 7570  lication startup
-00003eb0: 2063 6f6d 706c 6574 652e 0a49 4e46 4f3a   complete..INFO:
-00003ec0: 2020 2020 2031 3237 2e30 2e30 2e31 3a35       127.0.0.1:5
-00003ed0: 3233 3931 202d 2022 4745 5420 2f70 7269  2391 - "GET /pri
-00003ee0: 6e74 2048 5454 502f 312e 3122 2032 3030  nt HTTP/1.1" 200
-00003ef0: 204f 4b0a 0a48 656c 6c6f 2c20 4661 7374   OK..Hello, Fast
-00003f00: 4150 4945 7665 6e74 456d 6974 7465 7221  APIEventEmitter!
-00003f10: 0a0a 4865 6c6c 6f2c 2041 7379 6e63 494f  ..Hello, AsyncIO
-00003f20: 4576 656e 7445 6d69 7474 6572 210a 6060  EventEmitter!.``
-00003f30: 600a 0a3c 2f6c 693e 0a0a 3c2f 6f6c 3e20  `..</li>..</ol> 
-00003f40: 0a0a 3c70 2073 7479 6c65 3d27 7465 7874  ..<p style='text
-00003f50: 2d61 6c69 676e 3a20 6a75 7374 6966 793b  -align: justify;
-00003f60: 273e 0a20 2020 2026 656d 7370 3b26 656d  '>.    &emsp;&em
-00003f70: 7370 3b41 7320 7765 2063 616e 2073 6565  sp;As we can see
-00003f80: 2066 726f 6d20 7468 6973 2070 7261 6374   from this pract
-00003f90: 6963 616c 2065 7861 6d70 6c65 2c20 7765  ical example, we
-00003fa0: 2077 6572 6520 6162 6c65 2074 6f20 6561   were able to ea
-00003fb0: 7369 6c79 2061 6461 7074 2074 6865 2065  sily adapt the e
-00003fc0: 7665 6e74 2065 6d69 7474 6572 2074 6f20  vent emitter to 
-00003fd0: 7468 650a 0963 6f6e 7465 7874 206f 6620  the..context of 
-00003fe0: 7468 6520 4661 7374 4150 4920 6672 616d  the FastAPI fram
-00003ff0: 6577 6f72 6b2e 2057 6520 6465 6669 6e65  ework. We define
-00004000: 6420 616e 6420 696d 706c 656d 656e 7465  d and implemente
-00004010: 6420 6120 6375 7374 6f6d 2065 6d69 7474  d a custom emitt
-00004020: 6572 2074 6169 6c6f 7265 6420 666f 7220  er tailored for 
-00004030: 4661 7374 4150 4927 7320 776f 726b 666c  FastAPI's workfl
-00004040: 6f77 2c0a 0975 7369 6e67 2062 6163 6b67  ow,..using backg
-00004050: 726f 756e 6420 7461 736b 7320 746f 2068  round tasks to h
-00004060: 616e 646c 6520 7468 6520 6576 656e 7420  andle the event 
-00004070: 656d 6973 7369 6f6e 2061 6363 6f72 6469  emission accordi
-00004080: 6e67 6c79 2e0a 3c2f 703e 0a0a 3c70 2073  ngly..</p>..<p s
-00004090: 7479 6c65 3d27 7465 7874 2d61 6c69 676e  tyle='text-align
-000040a0: 3a20 6a75 7374 6966 793b 273e 0a20 2020  : justify;'>.   
-000040b0: 2026 656d 7370 3b26 656d 7370 3b57 6520   &emsp;&emsp;We 
-000040c0: 616c 736f 2073 6177 2050 7976 656e 7475  also saw Pyventu
-000040d0: 7327 2064 796e 616d 6963 2066 6c65 7869  s' dynamic flexi
-000040e0: 6269 6c69 7479 2066 6972 7374 6861 6e64  bility firsthand
-000040f0: 202d 2073 7761 7070 696e 6720 656d 6974   - swapping emit
-00004100: 7465 7273 2069 6e20 7265 616c 2d74 696d  ters in real-tim
-00004110: 6520 7265 7175 6972 6564 206e 6f0a 0969  e required no..i
-00004120: 6e74 7269 6361 7465 2072 6563 6f6e 6669  ntricate reconfi
-00004130: 6775 7261 7469 6f6e 206f 7220 7265 2d65  guration or re-e
-00004140: 7374 6162 6c69 7368 696e 6720 6f66 2068  stablishing of h
-00004150: 616e 646c 6572 732e 2053 696d 706c 7920  andlers. Simply 
-00004160: 6368 616e 6769 6e67 2074 6865 2063 6f6e  changing the con
-00004170: 6372 6574 6520 656d 6974 7465 7220 616c  crete emitter al
-00004180: 6c6f 7765 6420 666f 720a 0961 2073 6561  lowed for..a sea
-00004190: 6d6c 6573 7320 7472 616e 7369 7469 6f6e  mless transition
-000041a0: 2062 6574 7765 656e 2069 6d70 6c65 6d65   between impleme
-000041b0: 6e74 6174 696f 6e73 2e0a 3c2f 703e 0a0a  ntations..</p>..
-000041c0: 3c64 6574 6169 6c73 206d 6172 6b64 6f77  <details markdow
-000041d0: 6e3d 2231 2220 636c 6173 733d 2274 6970  n="1" class="tip
-000041e0: 2220 6f70 656e 3e0a 3c73 756d 6d61 7279  " open>.<summary
-000041f0: 3e4f 6666 6963 6961 6c20 3c63 6f64 653e  >Official <code>
-00004200: 4661 7374 4150 4945 7665 6e74 456d 6974  FastAPIEventEmit
-00004210: 7465 723c 2f63 6f64 653e 2069 6e74 6567  ter</code> integ
-00004220: 7261 7469 6f6e 3c2f 7375 6d6d 6172 793e  ration</summary>
-00004230: 0a3c 7020 7374 796c 653d 2774 6578 742d  .<p style='text-
-00004240: 616c 6967 6e3a 206a 7573 7469 6679 3b27  align: justify;'
-00004250: 3e0a 4e6f 206e 6565 6420 666f 7220 6d61  >.No need for ma
-00004260: 6e75 616c 2069 6d70 6c65 6d65 6e74 6174  nual implementat
-00004270: 696f 6e21 2050 7976 656e 7475 7320 6e6f  ion! Pyventus no
-00004280: 7720 6f66 6665 7273 2061 6e20 6f66 6669  w offers an offi
-00004290: 6369 616c 203c 623e 3c61 2068 7265 663d  cial <b><a href=
-000042a0: 2268 7474 7073 3a2f 2f6d 6461 7065 6e61  "https://mdapena
-000042b0: 2e67 6974 6875 622e 696f 2f70 7976 656e  .github.io/pyven
-000042c0: 7475 732f 7475 746f 7269 616c 732f 656d  tus/tutorials/em
-000042d0: 6974 7465 7273 2f66 6173 7461 7069 223e  itters/fastapi">
-000042e0: 4661 7374 4150 4945 7665 6e74 456d 6974  FastAPIEventEmit
-000042f0: 7465 723c 2f61 3e3c 2f62 3e0a 696e 7465  ter</a></b>.inte
-00004300: 6772 6174 696f 6e2e 0a3c 2f70 3e0a 3c2f  gration..</p>.</
-00004310: 6465 7461 696c 733e 0a0a 2323 2044 6566  details>..## Def
-00004320: 696e 696e 6720 4576 656e 7420 5265 7370  ining Event Resp
-00004330: 6f6e 7365 204c 6f67 6963 0a0a 3c70 2073  onse Logic..<p s
-00004340: 7479 6c65 3d27 7465 7874 2d61 6c69 676e  tyle='text-align
-00004350: 3a20 6a75 7374 6966 793b 273e 0a20 2020  : justify;'>.   
-00004360: 2026 656d 7370 3b26 656d 7370 3b41 7320   &emsp;&emsp;As 
-00004370: 7765 206d 656e 7469 6f6e 6564 2065 6172  we mentioned ear
-00004380: 6c69 6572 2c20 5079 7665 6e74 7573 2061  lier, Pyventus a
-00004390: 6c6c 6f77 7320 796f 7520 746f 2063 7573  llows you to cus
-000043a0: 746f 6d69 7a65 2068 6f77 2065 7665 6e74  tomize how event
-000043b0: 7320 6172 6520 7072 6f63 6573 7365 6420  s are processed 
-000043c0: 7570 6f6e 2063 6f6d 706c 6574 696f 6e20  upon completion 
-000043d0: 696e 0a09 7375 6363 6573 7320 6f72 2065  in..success or e
-000043e0: 7272 6f72 2073 6365 6e61 7269 6f73 2062  rror scenarios b
-000043f0: 7920 6174 7461 6368 696e 6720 6375 7374  y attaching cust
-00004400: 6f6d 2068 616e 646c 6572 732e 2054 6f20  om handlers. To 
-00004410: 7574 696c 697a 6520 7468 6973 2066 756e  utilize this fun
-00004420: 6374 696f 6e61 6c69 7479 2c20 5079 7665  ctionality, Pyve
-00004430: 6e74 7573 2070 726f 7669 6465 7320 6120  ntus provides a 
-00004440: 7369 6d70 6c65 0a09 7965 7420 706f 7765  simple..yet powe
-00004450: 7266 756c 2050 7974 686f 6e69 6320 7379  rful Pythonic sy
-00004460: 6e74 6178 2074 6872 6f75 6768 2069 7473  ntax through its
-00004470: 203c 636f 6465 3e65 7665 6e74 206c 696e   <code>event lin
-00004480: 6b61 6765 2063 6f6e 7465 7874 3c2f 636f  kage context</co
-00004490: 6465 3e2e 0a3c 2f70 3e0a 0a3c 7020 7374  de>..</p>..<p st
-000044a0: 796c 653d 2774 6578 742d 616c 6967 6e3a  yle='text-align:
-000044b0: 206a 7573 7469 6679 3b27 3e0a 2020 2020   justify;'>.    
-000044c0: 2665 6d73 703b 2665 6d73 703b 5468 6520  &emsp;&emsp;The 
-000044d0: 3c63 6f64 653e 6576 656e 7420 6c69 6e6b  <code>event link
-000044e0: 6167 6520 636f 6e74 6578 743c 2f63 6f64  age context</cod
-000044f0: 653e 2065 6e61 626c 6573 2064 6566 696e  e> enables defin
-00004500: 696e 6720 7468 6520 6576 656e 7420 776f  ing the event wo
-00004510: 726b 666c 6f77 2061 6e64 2063 6f6d 706c  rkflow and compl
-00004520: 6574 696f 6e20 6861 6e64 6c65 7273 2069  etion handlers i
-00004530: 6e20 616e 0a09 6f72 6761 6e69 7a65 6420  n an..organized 
-00004540: 6d61 6e6e 6572 2e20 5468 6973 2069 7320  manner. This is 
-00004550: 646f 6e65 2062 7920 7573 696e 6720 7468  done by using th
-00004560: 6520 3c63 6f64 653e 4576 656e 744c 696e  e <code>EventLin
-00004570: 6b65 722e 6f6e 3c2f 636f 6465 3e20 6d65  ker.on</code> me
-00004580: 7468 6f64 2077 6974 6869 6e20 6120 3c63  thod within a <c
-00004590: 6f64 653e 7769 7468 3c2f 636f 6465 3e20  ode>with</code> 
-000045a0: 7374 6174 656d 656e 740a 0962 6c6f 636b  statement..block
-000045b0: 2e20 4c65 7427 7320 6578 616d 696e 6520  . Let's examine 
-000045c0: 6578 616d 706c 6573 2064 656d 6f6e 7374  examples demonst
-000045d0: 7261 7469 6e67 2068 6f77 2073 7563 6365  rating how succe
-000045e0: 7373 2061 6e64 2066 6169 6c75 7265 2068  ss and failure h
-000045f0: 616e 646c 6572 7320 6361 6e20 6265 2061  andlers can be a
-00004600: 7474 6163 6865 6420 7573 696e 6720 7468  ttached using th
-00004610: 6520 6576 656e 7420 6c69 6e6b 6167 650a  e event linkage.
-00004620: 0963 6f6e 7465 7874 3a0a 3c2f 703e 0a0a  .context:.</p>..
-00004630: 2323 2320 5375 6363 6573 7320 616e 6420  ### Success and 
-00004640: 4572 726f 7220 4861 6e64 6c69 6e67 2045  Error Handling E
-00004650: 7861 6d70 6c65 0a0a 6060 6050 7974 686f  xample..```Pytho
-00004660: 6e20 6c69 6e65 6e75 6d73 3d22 3122 2020  n linenums="1"  
-00004670: 686c 5f6c 696e 6573 3d22 3720 3130 2d31  hl_lines="7 10-1
-00004680: 3222 0a66 726f 6d20 7079 7665 6e74 7573  2".from pyventus
-00004690: 2069 6d70 6f72 7420 4576 656e 744c 696e   import EventLin
-000046a0: 6b65 722c 2045 7665 6e74 456d 6974 7465  ker, EventEmitte
-000046b0: 722c 2041 7379 6e63 494f 4576 656e 7445  r, AsyncIOEventE
-000046c0: 6d69 7474 6572 0a0a 0a77 6974 6820 4576  mitter...with Ev
-000046d0: 656e 744c 696e 6b65 722e 6f6e 2822 5374  entLinker.on("St
-000046e0: 7269 6e67 4576 656e 7422 2920 6173 206c  ringEvent") as l
-000046f0: 696e 6b65 723a 0a09 0a20 2020 2040 6c69  inker:...    @li
-00004700: 6e6b 6572 2e6f 6e5f 6576 656e 740a 2020  nker.on_event.  
-00004710: 2020 6465 6620 6576 656e 745f 6361 6c6c    def event_call
-00004720: 6261 636b 2829 202d 3e20 7374 723a 0a20  back() -> str:. 
-00004730: 2020 2020 2020 2070 7269 6e74 2822 4576         print("Ev
-00004740: 656e 7420 7265 6365 6976 6564 2122 290a  ent received!").
-00004750: 2020 2020 2020 2020 7265 7475 726e 2022          return "
-00004760: 4576 656e 7420 7375 6363 6565 6465 6421  Event succeeded!
-00004770: 220a 0a20 2020 2040 6c69 6e6b 6572 2e6f  "..    @linker.o
-00004780: 6e5f 7375 6363 6573 730a 2020 2020 6465  n_success.    de
-00004790: 6620 7375 6363 6573 735f 6361 6c6c 6261  f success_callba
-000047a0: 636b 286d 7367 3a20 7374 7229 202d 3e20  ck(msg: str) -> 
-000047b0: 4e6f 6e65 3a0a 2020 2020 2020 2020 7072  None:.        pr
-000047c0: 696e 7428 6d73 6729 0a0a 2020 2020 406c  int(msg)..    @l
-000047d0: 696e 6b65 722e 6f6e 5f66 6169 6c75 7265  inker.on_failure
-000047e0: 0a20 2020 2064 6566 2066 6169 6c75 7265  .    def failure
-000047f0: 5f63 616c 6c62 6163 6b28 6578 633a 2045  _callback(exc: E
-00004800: 7863 6570 7469 6f6e 2920 2d3e 204e 6f6e  xception) -> Non
-00004810: 653a 0a20 2020 2020 2020 2070 7269 6e74  e:.        print
-00004820: 2865 7863 290a 0a09 2020 2020 0a65 7665  (exc)...    .eve
-00004830: 6e74 5f65 6d69 7474 6572 3a20 4576 656e  nt_emitter: Even
-00004840: 7445 6d69 7474 6572 203d 2041 7379 6e63  tEmitter = Async
-00004850: 494f 4576 656e 7445 6d69 7474 6572 2829  IOEventEmitter()
-00004860: 0a65 7665 6e74 5f65 6d69 7474 6572 2e65  .event_emitter.e
-00004870: 6d69 7428 2253 7472 696e 6745 7665 6e74  mit("StringEvent
-00004880: 2229 0a60 6060 0a0a 3c70 2073 7479 6c65  ").```..<p style
-00004890: 3d27 7465 7874 2d61 6c69 676e 3a20 6a75  ='text-align: ju
-000048a0: 7374 6966 793b 273e 0a20 2020 2026 656d  stify;'>.    &em
-000048b0: 7370 3b26 656d 7370 3b41 7320 7765 2068  sp;&emsp;As we h
-000048c0: 6176 6520 7365 656e 2066 726f 6d20 7468  ave seen from th
-000048d0: 6520 6578 616d 706c 6573 2c20 5079 7665  e examples, Pyve
-000048e0: 6e74 7573 2720 6576 656e 7420 6c69 6e6b  ntus' event link
-000048f0: 6167 6520 636f 6e74 6578 7420 7072 6f76  age context prov
-00004900: 6964 6573 2061 2072 656c 6961 626c 6520  ides a reliable 
-00004910: 616e 6420 5079 7468 6f6e 6963 2077 6179  and Pythonic way
-00004920: 0a09 746f 206d 616e 6167 6520 7468 6520  ..to manage the 
-00004930: 6576 656e 7420 776f 726b 666c 6f77 2061  event workflow a
-00004940: 6e64 2072 6573 706f 6e73 6520 746f 2064  nd response to d
-00004950: 6966 6665 7265 6e74 2063 6f6d 706c 6574  ifferent complet
-00004960: 696f 6e20 6f75 7463 6f6d 6573 2074 6872  ion outcomes thr
-00004970: 6f75 6768 2074 6865 2075 7365 206f 6620  ough the use of 
-00004980: 6375 7374 6f6d 2068 616e 646c 6572 732e  custom handlers.
-00004990: 0a3c 2f70 3e0a 0a23 2320 436f 6e74 696e  .</p>..## Contin
-000049a0: 756f 7573 2045 766f 6c75 7469 6f6e 0a0a  uous Evolution..
-000049b0: 3c70 2073 7479 6c65 3d27 7465 7874 2d61  <p style='text-a
-000049c0: 6c69 676e 3a20 6a75 7374 6966 793b 273e  lign: justify;'>
-000049d0: 0a09 2665 6d73 703b 2665 6d73 703b 5079  ..&emsp;&emsp;Py
-000049e0: 7665 6e74 7573 2063 6f6e 7469 6e75 6f75  ventus continuou
-000049f0: 736c 7920 6164 6170 7473 2074 6f20 7375  sly adapts to su
-00004a00: 7070 6f72 7420 6465 7665 6c6f 7065 7273  pport developers
-00004a10: 2061 6372 6f73 7320 7465 6368 6e6f 6c6f   across technolo
-00004a20: 6769 6361 6c20 616e 6420 7072 6f67 7261  gical and progra
-00004a30: 6d6d 696e 6720 646f 6d61 696e 732e 2049  mming domains. I
-00004a40: 7473 0a09 6169 6d20 6973 2074 6f20 7265  ts..aim is to re
-00004a50: 6d61 696e 2061 7420 7468 6520 666f 7265  main at the fore
-00004a60: 6672 6f6e 7420 6f66 2065 7665 6e74 2d64  front of event-d
-00004a70: 7269 7665 6e20 6465 7369 676e 2e20 4675  riven design. Fu
-00004a80: 7475 7265 2064 6576 656c 6f70 6d65 6e74  ture development
-00004a90: 206d 6179 2069 6e74 726f 6475 6365 206e   may introduce n
-00004aa0: 6577 206f 6666 6963 6961 6c20 6576 656e  ew official even
-00004ab0: 7420 0a09 656d 6974 7465 7273 2c20 6578  t ..emitters, ex
-00004ac0: 7061 6e64 696e 6720 636f 6d70 6174 6962  panding compatib
-00004ad0: 696c 6974 7920 7769 7468 2064 6966 6665  ility with diffe
-00004ae0: 7265 6e74 2074 6563 686e 6f6c 6f67 6965  rent technologie
-00004af0: 7320 7468 726f 7567 6820 7365 616d 6c65  s through seamle
-00004b00: 7373 2069 6e74 6567 7261 7469 6f6e 2e0a  ss integration..
-00004b10: 0a3c 7020 7374 796c 653d 2774 6578 742d  .<p style='text-
-00004b20: 616c 6967 6e3a 206a 7573 7469 6679 3b27  align: justify;'
-00004b30: 3e0a 0926 656d 7370 3b26 656d 7370 3b43  >..&emsp;&emsp;C
-00004b40: 7572 7265 6e74 2064 6566 6175 6c74 2065  urrent default e
-00004b50: 6d69 7474 6572 7320 7072 6f76 6964 6520  mitters provide 
-00004b60: 7265 6c69 6162 6c65 206f 7574 2d6f 662d  reliable out-of-
-00004b70: 7468 652d 626f 7820 6361 7061 6269 6c69  the-box capabili
-00004b80: 7469 6573 2066 6f72 2063 6f6d 6d6f 6e20  ties for common 
-00004b90: 7573 6520 6361 7365 732e 2054 6865 790a  use cases. They.
-00004ba0: 0965 6666 6963 6965 6e74 6c79 2068 616e  .efficiently han
-00004bb0: 646c 6520 636f 7265 2065 7665 6e74 206f  dle core event o
-00004bc0: 7065 7261 7469 6f6e 7320 616e 6420 6c61  perations and la
-00004bd0: 7920 7468 6520 666f 756e 6461 7469 6f6e  y the foundation
-00004be0: 2066 6f72 2062 7569 6c64 696e 6720 6576   for building ev
-00004bf0: 656e 742d 6472 6976 656e 2061 7070 6c69  ent-driven appli
-00004c00: 6361 7469 6f6e 732e 0a3c 2f70 3e0a 0a3c  cations..</p>..<
-00004c10: 6465 7461 696c 7320 6d61 726b 646f 776e  details markdown
-00004c20: 3d22 3122 2063 6c61 7373 3d22 696e 666f  ="1" class="info
-00004c30: 223e 0a3c 7375 6d6d 6172 793e 4472 6976  ">.<summary>Driv
-00004c40: 696e 6720 496e 6e6f 7661 7469 6f6e 2054  ing Innovation T
-00004c50: 6872 6f75 6768 2043 6f6c 6c61 626f 7261  hrough Collabora
-00004c60: 7469 6f6e 3c2f 7375 6d6d 6172 793e 0a0a  tion</summary>..
-00004c70: 3c70 2073 7479 6c65 3d27 7465 7874 2d61  <p style='text-a
-00004c80: 6c69 676e 3a20 6a75 7374 6966 793b 273e  lign: justify;'>
-00004c90: 0a20 2020 2026 656d 7370 3b26 656d 7370  .    &emsp;&emsp
-00004ca0: 3b50 7976 656e 7475 7320 6973 2061 6e20  ;Pyventus is an 
-00004cb0: 6f70 656e 2073 6f75 7263 6520 7072 6f6a  open source proj
-00004cc0: 6563 7420 7468 6174 2077 656c 636f 6d65  ect that welcome
-00004cd0: 7320 636f 6d6d 756e 6974 7920 696e 766f  s community invo
-00004ce0: 6c76 656d 656e 742e 2049 6620 796f 7520  lvement. If you 
-00004cf0: 7769 7368 2074 6f20 636f 6e74 7269 6275  wish to contribu
-00004d00: 7465 0a09 6164 6469 7469 6f6e 616c 2065  te..additional e
-00004d10: 7665 6e74 2065 6d69 7474 6572 732c 2069  vent emitters, i
-00004d20: 6d70 726f 7665 6d65 6e74 732c 206f 7220  mprovements, or 
-00004d30: 6275 6720 6669 7865 732c 2070 6c65 6173  bug fixes, pleas
-00004d40: 6520 6368 6563 6b20 7468 6520 3c61 2068  e check the <a h
-00004d50: 7265 663d 2268 7474 7073 3a2f 2f6d 6461  ref="https://mda
-00004d60: 7065 6e61 2e67 6974 6875 622e 696f 2f70  pena.github.io/p
-00004d70: 7976 656e 7475 732f 636f 6e74 7269 6275  yventus/contribu
-00004d80: 7469 6e67 2f22 3e43 6f6e 7472 6962 7574  ting/">Contribut
-00004d90: 696e 673c 2f61 3e20 7365 6374 696f 6e0a  ing</a> section.
-00004da0: 0966 6f72 2067 7569 6465 6c69 6e65 7320  .for guidelines 
-00004db0: 6f6e 2063 6f6c 6c61 626f 7261 7469 6e67  on collaborating
-00004dc0: 2e20 546f 6765 7468 6572 2c20 7765 2063  . Together, we c
-00004dd0: 616e 2066 7572 7468 6572 2074 6865 2070  an further the p
-00004de0: 6f73 7369 6269 6c69 7469 6573 206f 6620  ossibilities of 
-00004df0: 6576 656e 742d 6472 6976 656e 2064 6576  event-driven dev
-00004e00: 656c 6f70 6d65 6e74 2e0a 3c2f 703e 0a0a  elopment..</p>..
-00004e10: 3c2f 6465 7461 696c 733e 0a0a 2323 204c  </details>..## L
-00004e20: 6963 656e 7365 0a0a 3c70 2073 7479 6c65  icense..<p style
-00004e30: 3d27 7465 7874 2d61 6c69 676e 3a20 6a75  ='text-align: ju
-00004e40: 7374 6966 793b 2720 6d61 726b 646f 776e  stify;' markdown
-00004e50: 3e0a 2020 2020 2665 6d73 703b 2665 6d73  >.    &emsp;&ems
-00004e60: 703b 5079 7665 6e74 7573 2069 7320 6469  p;Pyventus is di
-00004e70: 7374 7269 6275 7465 6420 6173 206f 7065  stributed as ope
-00004e80: 6e20 736f 7572 6365 2073 6f66 7477 6172  n source softwar
-00004e90: 6520 616e 6420 6973 2072 656c 6561 7365  e and is release
-00004ea0: 6420 756e 6465 7220 7468 6520 3c61 2068  d under the <a h
-00004eb0: 7265 663d 2268 7474 7073 3a2f 2f63 686f  ref="https://cho
-00004ec0: 6f73 6561 6c69 6365 6e73 652e 636f 6d2f  osealicense.com/
-00004ed0: 6c69 6365 6e73 6573 2f6d 6974 2f22 2074  licenses/mit/" t
-00004ee0: 6172 6765 743d 225f 626c 616e 6b22 3e4d  arget="_blank">M
-00004ef0: 4954 204c 6963 656e 7365 3c2f 613e 2e20  IT License</a>. 
-00004f00: 0a20 2020 2059 6f75 2063 616e 2076 6965  .    You can vie
-00004f10: 7720 7468 6520 6675 6c6c 2074 6578 7420  w the full text 
-00004f20: 6f66 2074 6865 206c 6963 656e 7365 2069  of the license i
-00004f30: 6e20 7468 6520 3c61 2068 7265 663d 2268  n the <a href="h
-00004f40: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004f50: 6d2f 6d64 6170 656e 612f 7079 7665 6e74  m/mdapena/pyvent
-00004f60: 7573 2f62 6c6f 622f 6d61 7374 6572 2f4c  us/blob/master/L
-00004f70: 4943 454e 5345 2220 7461 7267 6574 3d22  ICENSE" target="
-00004f80: 5f62 6c61 6e6b 223e 3c63 6f64 653e 4c49  _blank"><code>LI
-00004f90: 4345 4e53 453c 2f63 6f64 653e 3c2f 613e  CENSE</code></a>
-00004fa0: 200a 0966 696c 6520 6c6f 6361 7465 6420   ..file located 
-00004fb0: 696e 2074 6865 2050 7976 656e 7475 7320  in the Pyventus 
-00004fc0: 7265 706f 7369 746f 7279 2e0a 3c2f 703e  repository..</p>
-00004fd0: 0a0a                                     ..
+00000eb0: 3030 3937 6138 2220 616c 743d 2253 7570  0097a8" alt="Sup
+00000ec0: 706f 7274 6564 2050 7974 686f 6e20 7665  ported Python ve
+00000ed0: 7273 696f 6e73 223e 0a3c 2f61 3e0a 0a3c  rsions">.</a>..<
+00000ee0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000ef0: 6769 7468 7562 2e63 6f6d 2f70 7366 2f62  github.com/psf/b
+00000f00: 6c61 636b 223e 0a09 3c69 6d67 2073 7263  lack">..<img src
+00000f10: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+00000f20: 6965 6c64 732e 696f 2f62 6164 6765 2f63  ields.io/badge/c
+00000f30: 6f64 6525 3230 7374 796c 652d 626c 6163  ode%20style-blac
+00000f40: 6b2d 3030 3030 3030 2e73 7667 2220 616c  k-000000.svg" al
+00000f50: 743d 2243 6f64 6520 7374 796c 653a 2062  t="Code style: b
+00000f60: 6c61 636b 223e 0a3c 2f61 3e0a 0a3c 2f70  lack">.</a>..</p
+00000f70: 3e0a 0a3c 6272 3e0a 0a2d 2d2d 0a0a 2a2a  >..<br>..---..**
+00000f80: 446f 6375 6d65 6e74 6174 696f 6e2a 2a3a  Documentation**:
+00000f90: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+00000fa0: 2f2f 6d64 6170 656e 612e 6769 7468 7562  //mdapena.github
+00000fb0: 2e69 6f2f 7079 7665 6e74 7573 2220 7461  .io/pyventus" ta
+00000fc0: 7267 6574 3d22 5f62 6c61 6e6b 223e 6874  rget="_blank">ht
+00000fd0: 7470 733a 2f2f 6d64 6170 656e 612e 6769  tps://mdapena.gi
+00000fe0: 7468 7562 2e69 6f2f 7079 7665 6e74 7573  thub.io/pyventus
+00000ff0: 3c2f 613e 0a0a 2a2a 536f 7572 6365 2043  </a>..**Source C
+00001000: 6f64 652a 2a3a 203c 6120 6872 6566 3d22  ode**: <a href="
+00001010: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001020: 6f6d 2f6d 6461 7065 6e61 2f70 7976 656e  om/mdapena/pyven
+00001030: 7475 7322 2074 6172 6765 743d 225f 626c  tus" target="_bl
+00001040: 616e 6b22 3e68 7474 7073 3a2f 2f67 6974  ank">https://git
+00001050: 6875 622e 636f 6d2f 6d64 6170 656e 612f  hub.com/mdapena/
+00001060: 7079 7665 6e74 7573 3c2f 613e 0a0a 2d2d  pyventus</a>..--
+00001070: 2d0a 0a3c 7020 7374 796c 653d 2774 6578  -..<p style='tex
+00001080: 742d 616c 6967 6e3a 206a 7573 7469 6679  t-align: justify
+00001090: 3b27 206d 6172 6b64 6f77 6e3e 0a20 2020  ;' markdown>.   
+000010a0: 2026 656d 7370 3b26 656d 7370 3b50 7976   &emsp;&emsp;Pyv
+000010b0: 656e 7475 7320 6973 2061 2070 6f77 6572  entus is a power
+000010c0: 6675 6c20 5079 7468 6f6e 2070 6163 6b61  ful Python packa
+000010d0: 6765 2066 6f72 2065 7665 6e74 2d64 7269  ge for event-dri
+000010e0: 7665 6e20 7072 6f67 7261 6d6d 696e 672e  ven programming.
+000010f0: 2049 7420 6f66 6665 7273 2061 2063 6f6d   It offers a com
+00001100: 7072 6568 656e 7369 7665 2073 7569 7465  prehensive suite
+00001110: 0a09 6f66 2074 6f6f 6c73 2074 6f20 6561  ..of tools to ea
+00001120: 7369 6c79 2064 6566 696e 652c 2065 6d69  sily define, emi
+00001130: 742c 2061 6e64 206f 7263 6865 7374 7261  t, and orchestra
+00001140: 7465 2065 7665 6e74 732e 2057 6974 6820  te events. With 
+00001150: 5079 7665 6e74 7573 2c20 796f 7520 6361  Pyventus, you ca
+00001160: 6e20 6275 696c 6420 7363 616c 6162 6c65  n build scalable
+00001170: 2c20 6578 7465 6e73 6962 6c65 2c20 616e  , extensible, an
+00001180: 640a 096c 6f6f 7365 6c79 2d63 6f75 706c  d..loosely-coupl
+00001190: 6564 2065 7665 6e74 2d64 7269 7665 6e20  ed event-driven 
+000011a0: 6170 706c 6963 6174 696f 6e73 2e0a 3c2f  applications..</
+000011b0: 703e 0a0a 5b2f 2f5d 3a20 2320 282d 2d2d  p>..[//]: # (---
+000011c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000011d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000011e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000011f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001200: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001210: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001220: 2d2d 2d2d 2d2d 2d2d 2d2d 2d29 0a0a 2323  -----------)..##
+00001230: 204b 6579 2046 6561 7475 7265 730a 0a3c   Key Features..<
+00001240: 7020 7374 796c 653d 2774 6578 742d 616c  p style='text-al
+00001250: 6967 6e3a 206a 7573 7469 6679 3b27 206d  ign: justify;' m
+00001260: 6172 6b64 6f77 6e3e 0a20 2020 2050 7976  arkdown>.    Pyv
+00001270: 656e 7475 7320 6f66 6665 7273 2073 6576  entus offers sev
+00001280: 6572 616c 206b 6579 2066 6561 7475 7265  eral key feature
+00001290: 732c 2073 7563 6820 6173 3a0a 3c2f 703e  s, such as:.</p>
+000012a0: 0a0a 3c75 6c20 7374 796c 653d 2774 6578  ..<ul style='tex
+000012b0: 742d 616c 6967 6e3a 206a 7573 7469 6679  t-align: justify
+000012c0: 3b27 3e0a 0a3c 6c69 3e3c 623e 5379 6e63  ;'>..<li><b>Sync
+000012d0: 2061 6e64 2041 7379 6e63 2053 7570 706f   and Async Suppo
+000012e0: 7274 3c2f 623e 20e2 9480 200a 5768 6574  rt</b> ... .Whet
+000012f0: 6865 7220 796f 7572 2063 6f64 6520 6973  her your code is
+00001300: 2073 796e 6368 726f 6e6f 7573 206f 7220   synchronous or 
+00001310: 6173 796e 6368 726f 6e6f 7573 2c20 5079  asynchronous, Py
+00001320: 7665 6e74 7573 2061 6c6c 6f77 7320 796f  ventus allows yo
+00001330: 7520 746f 2064 6566 696e 6520 6576 656e  u to define even
+00001340: 7420 6861 6e64 6c65 7273 2061 7320 6569  t handlers as ei
+00001350: 7468 6572 2073 796e 6320 6f72 2061 7379  ther sync or asy
+00001360: 6e63 0a63 616c 6c62 6163 6b73 2061 6e64  nc.callbacks and
+00001370: 2065 6d69 7420 6576 656e 7473 2066 726f   emit events fro
+00001380: 6d20 626f 7468 2073 636f 7065 732e 200a  m both scopes. .
+00001390: 3c2f 6c69 3e0a 0a3c 6c69 3e3c 623e 4375  </li>..<li><b>Cu
+000013a0: 7374 6f6d 697a 6174 696f 6e3c 2f62 3e20  stomization</b> 
+000013b0: e294 8020 0a57 6865 7468 6572 2079 6f75  ... .Whether you
+000013c0: 2063 686f 6f73 6520 6f66 6669 6369 616c   choose official
+000013d0: 2065 6d69 7474 6572 7320 6f72 2063 7573   emitters or cus
+000013e0: 746f 6d20 6f6e 6573 2c20 5079 7665 6e74  tom ones, Pyvent
+000013f0: 7573 2061 6c6c 6f77 7320 796f 7520 746f  us allows you to
+00001400: 2063 7573 746f 6d69 7a65 2074 6865 2062   customize the b
+00001410: 6568 6176 696f 7220 616e 6420 6361 7061  ehavior and capa
+00001420: 6269 6c69 7469 6573 206f 660a 7468 6520  bilities of.the 
+00001430: 6576 656e 7420 656d 6974 7465 7273 2074  event emitters t
+00001440: 6f20 7065 7266 6563 746c 7920 616c 6967  o perfectly alig
+00001450: 6e20 7769 7468 2079 6f75 7220 756e 6971  n with your uniq
+00001460: 7565 2072 6571 7569 7265 6d65 6e74 732e  ue requirements.
+00001470: 0a3c 2f6c 693e 0a0a 3c6c 693e 3c62 3e41  .</li>..<li><b>A
+00001480: 6e20 496e 7475 6974 6976 6520 4150 493c  n Intuitive API<
+00001490: 2f62 3e20 e294 8020 0a50 7976 656e 7475  /b> ... .Pyventu
+000014a0: 7320 7072 6f76 6964 6573 2061 2075 7365  s provides a use
+000014b0: 722d 6672 6965 6e64 6c79 2041 5049 2066  r-friendly API f
+000014c0: 6f72 2064 6566 696e 696e 6720 6576 656e  or defining even
+000014d0: 7473 2c20 656d 6974 7465 7273 2c20 616e  ts, emitters, an
+000014e0: 6420 6861 6e64 6c65 7273 2e20 4974 7320  d handlers. Its 
+000014f0: 6465 7369 676e 2073 696d 706c 6966 6965  design simplifie
+00001500: 7320 7468 6520 7072 6f63 6573 730a 6f66  s the process.of
+00001510: 2077 6f72 6b69 6e67 2077 6974 6820 6576   working with ev
+00001520: 656e 7473 2c20 656e 6162 6c69 6e67 2079  ents, enabling y
+00001530: 6f75 2074 6f20 6f72 6761 6e69 7a65 2079  ou to organize y
+00001540: 6f75 7220 636f 6465 2061 726f 756e 6420  our code around 
+00001550: 6469 7363 7265 7465 2065 7665 6e74 7320  discrete events 
+00001560: 616e 6420 7468 6569 7220 6173 736f 6369  and their associ
+00001570: 6174 6564 2061 6374 696f 6e73 2e0a 3c2f  ated actions..</
+00001580: 6c69 3e0a 0a3c 6c69 3e3c 623e 5275 6e74  li>..<li><b>Runt
+00001590: 696d 6520 466c 6578 6962 696c 6974 793c  ime Flexibility<
+000015a0: 2f62 3e20 e294 8020 0a50 7976 656e 7475  /b> ... .Pyventu
+000015b0: 7327 2072 756e 7469 6d65 2066 6c65 7869  s' runtime flexi
+000015c0: 6269 6c69 7479 2061 6c6c 6f77 7320 796f  bility allows yo
+000015d0: 7520 746f 2073 7769 7463 6820 7365 616d  u to switch seam
+000015e0: 6c65 7373 6c79 2062 6574 7765 656e 2064  lessly between d
+000015f0: 6966 6665 7265 6e74 2062 7569 6c74 2d69  ifferent built-i
+00001600: 6e20 6f72 2063 7573 746f 6d20 6576 656e  n or custom even
+00001610: 7420 656d 6974 7465 720a 696d 706c 656d  t emitter.implem
+00001620: 656e 7461 7469 6f6e 7320 6f6e 2074 6865  entations on the
+00001630: 2066 6c79 2c20 7072 6f76 6964 696e 6720   fly, providing 
+00001640: 6120 6479 6e61 6d69 6320 616e 6420 6164  a dynamic and ad
+00001650: 6170 7461 626c 6520 656e 7669 726f 6e6d  aptable environm
+00001660: 656e 7420 666f 7220 6576 656e 742d 6472  ent for event-dr
+00001670: 6976 656e 2070 726f 6772 616d 6d69 6e67  iven programming
+00001680: 2e0a 3c2f 6c69 3e0a 0a3c 6c69 3e3c 623e  ..</li>..<li><b>
+00001690: 5265 6c69 6162 6c65 2045 7665 6e74 2048  Reliable Event H
+000016a0: 616e 646c 696e 673c 2f62 3e20 e294 8020  andling</b> ... 
+000016b0: 0a50 7976 656e 7475 7320 616c 6c6f 7773  .Pyventus allows
+000016c0: 2079 6f75 2074 6f20 6465 6669 6e65 2068   you to define h
+000016d0: 616e 646c 6572 7320 746f 2063 7573 746f  andlers to custo
+000016e0: 6d69 7a65 2068 6f77 2065 7665 6e74 7320  mize how events 
+000016f0: 6172 6520 7072 6f63 6573 7365 6420 7570  are processed up
+00001700: 6f6e 2063 6f6d 706c 6574 696f 6e2e 2041  on completion. A
+00001710: 7474 6163 6820 7375 6363 6573 7320 616e  ttach success an
+00001720: 640a 6661 696c 7572 6520 6c6f 6769 6320  d.failure logic 
+00001730: 746f 2074 616b 6520 7461 7267 6574 6564  to take targeted
+00001740: 2061 6374 696f 6e73 2062 6173 6564 206f   actions based o
+00001750: 6e20 7468 6520 6f75 7463 6f6d 6520 6f66  n the outcome of
+00001760: 2065 6163 6820 6576 656e 7420 6578 6563   each event exec
+00001770: 7574 696f 6e2e 200a 3c2f 6c69 3e0a 0a3c  ution. .</li>..<
+00001780: 6c69 3e3c 623e 5363 616c 6162 696c 6974  li><b>Scalabilit
+00001790: 7920 616e 6420 4d61 696e 7461 696e 6162  y and Maintainab
+000017a0: 696c 6974 793c 2f62 3e20 e294 8020 0a42  ility</b> ... .B
+000017b0: 7920 6164 6f70 7469 6e67 2061 6e20 6576  y adopting an ev
+000017c0: 656e 742d 6472 6976 656e 2061 7070 726f  ent-driven appro
+000017d0: 6163 6820 7769 7468 2050 7976 656e 7475  ach with Pyventu
+000017e0: 732c 2079 6f75 2063 616e 2063 7265 6174  s, you can creat
+000017f0: 6520 7363 616c 6162 6c65 2061 6e64 206d  e scalable and m
+00001800: 6169 6e74 6169 6e61 626c 6520 636f 6465  aintainable code
+00001810: 2074 6861 6e6b 7320 746f 2074 6865 206c   thanks to the l
+00001820: 6f6f 7365 0a63 6f75 706c 696e 6720 6265  oose.coupling be
+00001830: 7477 6565 6e20 6974 7320 636f 6d70 6f6e  tween its compon
+00001840: 656e 7473 2074 6861 7420 656e 6162 6c65  ents that enable
+00001850: 7320 6578 7465 6e73 6962 696c 6974 7920  s extensibility 
+00001860: 616e 6420 6d6f 6475 6c61 7269 7479 2e0a  and modularity..
+00001870: 3c2f 6c69 3e0a 0a3c 6c69 3e3c 623e 436f  </li>..<li><b>Co
+00001880: 6d70 7265 6865 6e73 6976 6520 446f 6375  mprehensive Docu
+00001890: 6d65 6e74 6174 696f 6e3c 2f62 3e20 e294  mentation</b> ..
+000018a0: 8020 0a50 7976 656e 7475 7320 7072 6f76  . .Pyventus prov
+000018b0: 6964 6573 2061 2063 6f6d 7072 6568 656e  ides a comprehen
+000018c0: 7369 7665 2064 6f63 756d 656e 7461 7469  sive documentati
+000018d0: 6f6e 2073 7569 7465 2074 6861 7420 696e  on suite that in
+000018e0: 636c 7564 6573 2041 5049 2072 6566 6572  cludes API refer
+000018f0: 656e 6365 732c 2075 7361 6765 2065 7861  ences, usage exa
+00001900: 6d70 6c65 732c 2061 6e64 2074 7574 6f72  mples, and tutor
+00001910: 6961 6c73 2074 6f0a 6566 6665 6374 6976  ials to.effectiv
+00001920: 656c 7920 6c65 7665 7261 6765 2061 6c6c  ely leverage all
+00001930: 2074 6865 2066 6561 7475 7265 7320 616e   the features an
+00001940: 6420 6361 7061 6269 6c69 7469 6573 206f  d capabilities o
+00001950: 6620 7468 6520 7061 636b 6167 652e 0a3c  f the package..<
+00001960: 2f6c 693e 0a0a 3c2f 756c 3e0a 0a5b 2f2f  /li>..</ul>..[//
+00001970: 5d3a 2023 2028 2d2d 2d2d 2d2d 2d2d 2d2d  ]: # (----------
+00001980: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001990: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000019a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000019b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000019c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000019d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000019e0: 2d2d 2d2d 290a 0a23 2320 5175 6963 6b20  ----)..## Quick 
+000019f0: 5374 6172 740a 0a3c 7020 7374 796c 653d  Start..<p style=
+00001a00: 2774 6578 742d 616c 6967 6e3a 206a 7573  'text-align: jus
+00001a10: 7469 6679 3b27 3e0a 0926 656d 7370 3b26  tify;'>..&emsp;&
+00001a20: 656d 7370 3b50 7976 656e 7475 7320 6973  emsp;Pyventus is
+00001a30: 2070 7562 6c69 7368 6564 2061 7320 6120   published as a 
+00001a40: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00001a50: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
+00001a60: 742f 7079 7665 6e74 7573 2f22 2074 6172  t/pyventus/" tar
+00001a70: 6765 743d 225f 626c 616e 6b22 3e50 7974  get="_blank">Pyt
+00001a80: 686f 6e20 7061 636b 6167 653c 2f61 3e20  hon package</a> 
+00001a90: 0a09 616e 6420 6361 6e20 6265 2069 6e73  ..and can be ins
+00001aa0: 7461 6c6c 6564 2075 7369 6e67 203c 636f  talled using <co
+00001ab0: 6465 3e70 6970 3c2f 636f 6465 3e2c 2069  de>pip</code>, i
+00001ac0: 6465 616c 6c79 2069 6e20 6120 3c61 2068  deally in a <a h
+00001ad0: 7265 663d 2268 7474 7073 3a2f 2f72 6561  ref="https://rea
+00001ae0: 6c70 7974 686f 6e2e 636f 6d2f 7079 7468  lpython.com/pyth
+00001af0: 6f6e 2d76 6972 7475 616c 2d65 6e76 6972  on-virtual-envir
+00001b00: 6f6e 6d65 6e74 732d 612d 7072 696d 6572  onments-a-primer
+00001b10: 2f22 2074 6172 6765 743d 225f 626c 616e  /" target="_blan
+00001b20: 6b22 3e76 6972 7475 616c 2065 6e76 6972  k">virtual envir
+00001b30: 6f6e 6d65 6e74 3c2f 613e 0a09 666f 7220  onment</a>..for 
+00001b40: 7072 6f70 6572 2064 6570 656e 6465 6e63  proper dependenc
+00001b50: 7920 6973 6f6c 6174 696f 6e2e 2054 6f20  y isolation. To 
+00001b60: 6765 7420 7374 6172 7465 642c 206f 7065  get started, ope
+00001b70: 6e20 7570 2061 2074 6572 6d69 6e61 6c20  n up a terminal 
+00001b80: 616e 6420 696e 7374 616c 6c20 5079 7665  and install Pyve
+00001b90: 6e74 7573 2077 6974 6820 7468 6520 666f  ntus with the fo
+00001ba0: 6c6c 6f77 696e 6720 636f 6d6d 616e 643a  llowing command:
+00001bb0: 0a3c 2f70 3e0a 0a60 6060 636f 6e73 6f6c  .</p>..```consol
+00001bc0: 650a 7069 7020 696e 7374 616c 6c20 7079  e.pip install py
+00001bd0: 7665 6e74 7573 0a60 6060 0a0a 3c70 2073  ventus.```..<p s
+00001be0: 7479 6c65 3d27 7465 7874 2d61 6c69 676e  tyle='text-align
+00001bf0: 3a20 6a75 7374 6966 793b 273e 0a09 2665  : justify;'>..&e
+00001c00: 6d73 703b 2665 6d73 703b 5079 7665 6e74  msp;&emsp;Pyvent
+00001c10: 7573 2062 7920 6465 6661 756c 7420 7265  us by default re
+00001c20: 6c69 6573 206f 6e20 7468 6520 5079 7468  lies on the Pyth
+00001c30: 6f6e 2073 7461 6e64 6172 6420 6c69 6272  on standard libr
+00001c40: 6172 7920 616e 6420 3c62 3e72 6571 7569  ary and <b>requi
+00001c50: 7265 7320 5079 7468 6f6e 2033 2e31 3020  res Python 3.10 
+00001c60: 6f72 2068 6967 6865 723c 2f62 3e20 7769  or higher</b> wi
+00001c70: 7468 206e 6f20 0a09 6164 6469 7469 6f6e  th no ..addition
+00001c80: 616c 2064 6570 656e 6465 6e63 6965 732e  al dependencies.
+00001c90: 2048 6f77 6576 6572 2c20 7468 6973 2070   However, this p
+00001ca0: 6163 6b61 6765 2061 6c73 6f20 696e 636c  ackage also incl
+00001cb0: 7564 6573 2061 6c74 6572 6e61 7469 7665  udes alternative
+00001cc0: 2069 6e74 6567 7261 7469 6f6e 7320 746f   integrations to
+00001cd0: 2061 6363 6573 7320 6164 6469 7469 6f6e   access addition
+00001ce0: 616c 2066 6561 7475 7265 7320 0a09 7375  al features ..su
+00001cf0: 6368 2061 7320 5265 6469 7320 5175 6575  ch as Redis Queu
+00001d00: 652c 2043 656c 6572 792c 2061 6e64 2046  e, Celery, and F
+00001d10: 6173 7441 5049 2e20 466f 7220 6d6f 7265  astAPI. For more
+00001d20: 2069 6e66 6f72 6d61 7469 6f6e 206f 6e20   information on 
+00001d30: 7468 6973 206d 6174 7465 722c 2070 6c65  this matter, ple
+00001d40: 6173 6520 7265 6665 7220 746f 2074 6865  ase refer to the
+00001d50: 200a 093c 6120 6872 6566 3d22 6874 7470   ..<a href="http
+00001d60: 733a 2f2f 6d64 6170 656e 612e 6769 7468  s://mdapena.gith
+00001d70: 7562 2e69 6f2f 7079 7665 6e74 7573 2f67  ub.io/pyventus/g
+00001d80: 6574 7469 6e67 2d73 7461 7274 6564 2f23  etting-started/#
+00001d90: 6f70 7469 6f6e 616c 2d64 6570 656e 6465  optional-depende
+00001da0: 6e63 6965 7322 2074 6172 6765 743d 225f  ncies" target="_
+00001db0: 626c 616e 6b22 3e4f 7074 696f 6e61 6c20  blank">Optional 
+00001dc0: 4465 7065 6e64 656e 6369 6573 3c2f 613e  Dependencies</a>
+00001dd0: 0a09 7365 6374 696f 6e2e 0a3c 2f70 3e0a  ..section..</p>.
+00001de0: 0a5b 2f2f 5d3a 2023 2028 2d2d 2d2d 2d2d  .[//]: # (------
+00001df0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001e00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001e10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001e20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001e30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001e40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001e50: 2d2d 2d2d 2d2d 2d2d 290a 0a23 2320 4120  --------)..## A 
+00001e60: 5369 6d70 6c65 2045 7861 6d70 6c65 0a0a  Simple Example..
+00001e70: 3c70 2073 7479 6c65 3d27 7465 7874 2d61  <p style='text-a
+00001e80: 6c69 676e 3a20 6a75 7374 6966 793b 273e  lign: justify;'>
+00001e90: 0a20 2020 2026 656d 7370 3b26 656d 7370  .    &emsp;&emsp
+00001ea0: 3b45 7870 6572 6965 6e63 6520 7468 6520  ;Experience the 
+00001eb0: 706f 7765 7220 6f66 2050 7976 656e 7475  power of Pyventu
+00001ec0: 7320 7468 726f 7567 6820 6120 7369 6d70  s through a simp
+00001ed0: 6c65 203c 636f 6465 3e48 656c 6c6f 2c20  le <code>Hello, 
+00001ee0: 576f 726c 6421 3c2f 636f 6465 3e20 6578  World!</code> ex
+00001ef0: 616d 706c 6520 7468 6174 2069 6c6c 7573  ample that illus
+00001f00: 7472 6174 6573 0a09 7468 6520 636f 7265  trates..the core
+00001f10: 2063 6f6e 6365 7074 7320 616e 6420 6261   concepts and ba
+00001f20: 7369 6320 7573 6167 6520 6f66 2074 6865  sic usage of the
+00001f30: 2070 6163 6b61 6765 2e20 4279 2066 6f6c   package. By fol
+00001f40: 6c6f 7769 6e67 2074 6869 7320 6578 616d  lowing this exam
+00001f50: 706c 652c 2079 6f75 e280 996c 6c20 6c65  ple, you...ll le
+00001f60: 6172 6e20 686f 7720 746f 2073 7562 7363  arn how to subsc
+00001f70: 7269 6265 2074 6f20 6576 656e 7473 0a09  ribe to events..
+00001f80: 616e 6420 656d 6974 2074 6865 6d20 7769  and emit them wi
+00001f90: 7468 696e 2079 6f75 7220 6170 706c 6963  thin your applic
+00001fa0: 6174 696f 6e2e 0a3c 2f70 3e0a 0a60 6060  ation..</p>..```
+00001fb0: 5079 7468 6f6e 2074 6974 6c65 3d22 4865  Python title="He
+00001fc0: 6c6c 6f2c 2057 6f72 6c64 2120 4578 616d  llo, World! Exam
+00001fd0: 706c 6522 206c 696e 656e 756d 733d 2231  ple" linenums="1
+00001fe0: 220a 6672 6f6d 2070 7976 656e 7475 7320  ".from pyventus 
+00001ff0: 696d 706f 7274 2045 7665 6e74 4c69 6e6b  import EventLink
+00002000: 6572 2c20 4576 656e 7445 6d69 7474 6572  er, EventEmitter
+00002010: 2c20 4173 796e 6349 4f45 7665 6e74 456d  , AsyncIOEventEm
+00002020: 6974 7465 720a 0a0a 4045 7665 6e74 4c69  itter...@EventLi
+00002030: 6e6b 6572 2e6f 6e28 2247 7265 6574 4576  nker.on("GreetEv
+00002040: 656e 7422 290a 6465 6620 6861 6e64 6c65  ent").def handle
+00002050: 5f67 7265 6574 5f65 7665 6e74 2829 3a0a  _greet_event():.
+00002060: 2020 2020 7072 696e 7428 2248 656c 6c6f      print("Hello
+00002070: 2c20 576f 726c 6421 2229 0a0a 0a65 7665  , World!")...eve
+00002080: 6e74 5f65 6d69 7474 6572 3a20 4576 656e  nt_emitter: Even
+00002090: 7445 6d69 7474 6572 203d 2041 7379 6e63  tEmitter = Async
+000020a0: 494f 4576 656e 7445 6d69 7474 6572 2829  IOEventEmitter()
+000020b0: 0a65 7665 6e74 5f65 6d69 7474 6572 2e65  .event_emitter.e
+000020c0: 6d69 7428 2247 7265 6574 4576 656e 7422  mit("GreetEvent"
+000020d0: 290a 6060 600a 0a3c 6465 7461 696c 7320  ).```..<details 
+000020e0: 6d61 726b 646f 776e 3d22 3122 2063 6c61  markdown="1" cla
+000020f0: 7373 3d22 696e 666f 223e 0a3c 7375 6d6d  ss="info">.<summ
+00002100: 6172 793e 596f 7520 6361 6e20 616c 736f  ary>You can also
+00002110: 2077 6f72 6b20 7769 7468 203c 636f 6465   work with <code
+00002120: 3e61 7379 6e63 3c2f 636f 6465 3e20 6675  >async</code> fu
+00002130: 6e63 7469 6f6e 7320 616e 6420 636f 6e74  nctions and cont
+00002140: 6578 7473 2e2e 2e3c 2f73 756d 6d61 7279  exts...</summary
+00002150: 3e0a 0a60 6060 5079 7468 6f6e 2074 6974  >..```Python tit
+00002160: 6c65 3d22 4865 6c6c 6f2c 2057 6f72 6c64  le="Hello, World
+00002170: 2120 4578 616d 706c 6520 2841 7379 6e63  ! Example (Async
+00002180: 2076 6572 7369 6f6e 2922 206c 696e 656e   version)" linen
+00002190: 756d 733d 2231 2220 686c 5f6c 696e 6573  ums="1" hl_lines
+000021a0: 3d22 3522 0a66 726f 6d20 7079 7665 6e74  ="5".from pyvent
+000021b0: 7573 2069 6d70 6f72 7420 4576 656e 744c  us import EventL
+000021c0: 696e 6b65 722c 2045 7665 6e74 456d 6974  inker, EventEmit
+000021d0: 7465 722c 2041 7379 6e63 494f 4576 656e  ter, AsyncIOEven
+000021e0: 7445 6d69 7474 6572 0a0a 0a40 4576 656e  tEmitter...@Even
+000021f0: 744c 696e 6b65 722e 6f6e 2822 4772 6565  tLinker.on("Gree
+00002200: 7445 7665 6e74 2229 0a61 7379 6e63 2064  tEvent").async d
+00002210: 6566 2068 616e 646c 655f 6772 6565 745f  ef handle_greet_
+00002220: 6576 656e 7428 293a 0a20 2020 2070 7269  event():.    pri
+00002230: 6e74 2822 4865 6c6c 6f2c 2057 6f72 6c64  nt("Hello, World
+00002240: 2122 290a 0a0a 6576 656e 745f 656d 6974  !")...event_emit
+00002250: 7465 723a 2045 7665 6e74 456d 6974 7465  ter: EventEmitte
+00002260: 7220 3d20 4173 796e 6349 4f45 7665 6e74  r = AsyncIOEvent
+00002270: 456d 6974 7465 7228 290a 6576 656e 745f  Emitter().event_
+00002280: 656d 6974 7465 722e 656d 6974 2822 4772  emitter.emit("Gr
+00002290: 6565 7445 7665 6e74 2229 0a60 6060 0a0a  eetEvent").```..
+000022a0: 3c2f 6465 7461 696c 733e 0a0a 3c70 2073  </details>..<p s
+000022b0: 7479 6c65 3d27 7465 7874 2d61 6c69 676e  tyle='text-align
+000022c0: 3a20 6a75 7374 6966 793b 273e 0a20 2020  : justify;'>.   
+000022d0: 2026 656d 7370 3b26 656d 7370 3b41 7320   &emsp;&emsp;As 
+000022e0: 7765 2063 616e 2073 6565 2066 726f 6d20  we can see from 
+000022f0: 7468 6520 3c63 6f64 653e 4865 6c6c 6f2c  the <code>Hello,
+00002300: 2057 6f72 6c64 213c 2f63 6f64 653e 2065   World!</code> e
+00002310: 7861 6d70 6c65 2c20 5079 7665 6e74 7573  xample, Pyventus
+00002320: 2066 6f6c 6c6f 7773 2061 2073 696d 706c   follows a simpl
+00002330: 6520 616e 6420 696e 7475 6974 6976 6520  e and intuitive 
+00002340: 0a09 776f 726b 666c 6f77 2066 6f72 2064  ..workflow for d
+00002350: 6566 696e 696e 6720 616e 6420 656d 6974  efining and emit
+00002360: 7469 6e67 2065 7665 6e74 732e 204c 6574  ting events. Let
+00002370: 2773 2072 6563 6170 2074 6865 2065 7373  's recap the ess
+00002380: 656e 7469 616c 2073 7465 7073 2069 6e76  ential steps inv
+00002390: 6f6c 7665 643a 0a3c 2f70 3e0a 0a3c 6f6c  olved:.</p>..<ol
+000023a0: 2073 7479 6c65 3d27 7465 7874 2d61 6c69   style='text-ali
+000023b0: 676e 3a20 6a75 7374 6966 793b 273e 0a0a  gn: justify;'>..
+000023c0: 3c6c 693e 0a3c 623e 496d 706f 7274 696e  <li>.<b>Importin
+000023d0: 6720 4e65 6365 7373 6172 7920 4d6f 6475  g Necessary Modu
+000023e0: 6c65 733a 3c2f 623e 200a 5765 2066 6972  les:</b> .We fir
+000023f0: 7374 2069 6d70 6f72 7465 6420 7468 6520  st imported the 
+00002400: 7265 7175 6972 6564 206d 6f64 756c 6573  required modules
+00002410: 2066 726f 6d20 5079 7665 6e74 7573 2c20   from Pyventus, 
+00002420: 2077 6869 6368 2065 6e63 6f6d 7061 7373   which encompass
+00002430: 6564 2074 6865 203c 636f 6465 3e45 7665  ed the <code>Eve
+00002440: 6e74 4c69 6e6b 6572 3c2f 636f 6465 3e0a  ntLinker</code>.
+00002450: 636c 6173 732c 2074 6865 203c 636f 6465  class, the <code
+00002460: 3e45 7665 6e74 456d 6974 7465 723c 2f63  >EventEmitter</c
+00002470: 6f64 653e 2069 6e74 6572 6661 6365 2c20  ode> interface, 
+00002480: 616e 6420 7468 6520 3c63 6f64 653e 4173  and the <code>As
+00002490: 796e 6349 4f45 7665 6e74 456d 6974 7465  yncIOEventEmitte
+000024a0: 723c 2f63 6f64 653e 2069 6d70 6c65 6d65  r</code> impleme
+000024b0: 6e74 6174 696f 6e2e 0a3c 2f6c 693e 0a0a  ntation..</li>..
+000024c0: 3c6c 693e 0a3c 623e 4c69 6e6b 696e 6720  <li>.<b>Linking 
+000024d0: 4576 656e 7473 2074 6f20 4361 6c6c 6261  Events to Callba
+000024e0: 636b 733a 3c2f 623e 200a 4e65 7874 2c20  cks:</b> .Next, 
+000024f0: 7765 2075 7365 6420 7468 6520 3c63 6f64  we used the <cod
+00002500: 653e 4045 7665 6e74 4c69 6e6b 6572 2e6f  e>@EventLinker.o
+00002510: 6e28 293c 2f63 6f64 653e 2064 6563 6f72  n()</code> decor
+00002520: 6174 6f72 2074 6f20 6465 6669 6e65 2061  ator to define a
+00002530: 6e64 206c 696e 6b20 7468 6520 7374 7269  nd link the stri
+00002540: 6e67 2065 7665 6e74 203c 636f 6465 3e47  ng event <code>G
+00002550: 7265 6574 4576 656e 743c 2f63 6f64 653e  reetEvent</code>
+00002560: 200a 746f 2074 6865 2066 756e 6374 696f   .to the functio
+00002570: 6e20 3c63 6f64 653e 6861 6e64 6c65 5f67  n <code>handle_g
+00002580: 7265 6574 5f65 7665 6e74 2829 3c2f 636f  reet_event()</co
+00002590: 6465 3e2c 2077 6869 6368 2077 696c 6c20  de>, which will 
+000025a0: 7072 696e 7420 3c69 3e27 4865 6c6c 6f2c  print <i>'Hello,
+000025b0: 2057 6f72 6c64 2127 3c2f 693e 2074 6f20   World!'</i> to 
+000025c0: 7468 6520 636f 6e73 6f6c 6520 7768 656e  the console when
+000025d0: 6576 6572 2074 6865 0a3c 636f 6465 3e47  ever the.<code>G
+000025e0: 7265 6574 4576 656e 743c 2f63 6f64 653e  reetEvent</code>
+000025f0: 2069 7320 656d 6974 7465 642e 0a3c 2f6c   is emitted..</l
+00002600: 693e 0a0a 3c6c 693e 0a3c 623e 496e 7374  i>..<li>.<b>Inst
+00002610: 616e 7469 6174 696e 6720 616e 2045 7665  antiating an Eve
+00002620: 6e74 2045 6d69 7474 6572 3a3c 2f62 3e20  nt Emitter:</b> 
+00002630: 0a41 6674 6572 2074 6861 742c 2061 6e64  .After that, and
+00002640: 2069 6e20 6f72 6465 7220 746f 2074 7269   in order to tri
+00002650: 6767 6572 206f 7572 2065 7665 6e74 2c20  gger our event, 
+00002660: 7765 206e 6565 6465 6420 746f 2063 7265  we needed to cre
+00002670: 6174 6520 616e 2069 6e73 7461 6e63 6520  ate an instance 
+00002680: 6f66 2074 6865 2065 7665 6e74 2065 6d69  of the event emi
+00002690: 7474 6572 2063 6c61 7373 2e20 5768 696c  tter class. Whil
+000026a0: 6520 0a3c 636f 6465 3e41 7379 6e63 494f  e .<code>AsyncIO
+000026b0: 4576 656e 7445 6d69 7474 6572 3c2f 636f  EventEmitter</co
+000026c0: 6465 3e20 7761 7320 7574 696c 697a 6564  de> was utilized
+000026d0: 2c20 616e 7920 3c61 2068 7265 663d 2268  , any <a href="h
+000026e0: 7474 7073 3a2f 2f6d 6461 7065 6e61 2e67  ttps://mdapena.g
+000026f0: 6974 6875 622e 696f 2f70 7976 656e 7475  ithub.io/pyventu
+00002700: 732f 6765 7474 696e 672d 7374 6172 7465  s/getting-starte
+00002710: 642f 236f 7074 696f 6e61 6c2d 6465 7065  d/#optional-depe
+00002720: 6e64 656e 6369 6573 223e 3c69 3e62 7569  ndencies"><i>bui
+00002730: 6c74 2d69 6e3c 2f69 3e3c 2f61 3e0a 6f72  lt-in</i></a>.or
+00002740: 2063 7573 746f 6d20 696d 706c 656d 656e   custom implemen
+00002750: 7461 7469 6f6e 2063 6f75 6c64 2062 6520  tation could be 
+00002760: 656d 706c 6f79 6564 2e0a 3c2f 6c69 3e0a  employed..</li>.
+00002770: 0a3c 6c69 3e0a 3c62 3e54 7269 6767 6572  .<li>.<b>Trigger
+00002780: 696e 6720 7468 6520 4576 656e 743a 3c2f  ing the Event:</
+00002790: 623e 0a46 696e 616c 6c79 2c20 6279 2075  b>.Finally, by u
+000027a0: 7369 6e67 2074 6865 203c 636f 6465 3e65  sing the <code>e
+000027b0: 6d69 7428 293c 2f63 6f64 653e 206d 6574  mit()</code> met
+000027c0: 686f 6420 6f66 2074 6865 2065 7665 6e74  hod of the event
+000027d0: 2065 6d69 7474 6572 2069 6e73 7461 6e63   emitter instanc
+000027e0: 652c 2077 6520 7765 7265 2061 626c 6520  e, we were able 
+000027f0: 746f 2074 7269 6767 6572 2074 6865 200a  to trigger the .
+00002800: 3c63 6f64 653e 4772 6565 7445 7665 6e74  <code>GreetEvent
+00002810: 3c2f 636f 6465 3e2c 2077 6869 6368 2072  </code>, which r
+00002820: 6573 756c 7465 6420 696e 2074 6865 2065  esulted in the e
+00002830: 7865 6375 7469 6f6e 206f 6620 7468 6520  xecution of the 
+00002840: 3c63 6f64 653e 6861 6e64 6c65 5f67 7265  <code>handle_gre
+00002850: 6574 5f65 7665 6e74 2829 3c2f 636f 6465  et_event()</code
+00002860: 3e20 6361 6c6c 6261 636b 2e0a 3c2f 6c69  > callback..</li
+00002870: 3e0a 0a3c 2f6f 6c3e 0a0a 3c70 2073 7479  >..</ol>..<p sty
+00002880: 6c65 3d27 7465 7874 2d61 6c69 676e 3a20  le='text-align: 
+00002890: 6a75 7374 6966 793b 273e 0a20 2020 2026  justify;'>.    &
+000028a0: 656d 7370 3b26 656d 7370 3b48 6176 696e  emsp;&emsp;Havin
+000028b0: 6720 6761 696e 6564 2061 2063 6c65 6172  g gained a clear
+000028c0: 2075 6e64 6572 7374 616e 6469 6e67 206f   understanding o
+000028d0: 6620 7468 6520 776f 726b 666c 6f77 2073  f the workflow s
+000028e0: 686f 7763 6173 6564 2069 6e20 7468 6520  howcased in the 
+000028f0: 3c63 6f64 653e 4865 6c6c 6f2c 2057 6f72  <code>Hello, Wor
+00002900: 6c64 213c 2f63 6f64 653e 2065 7861 6d70  ld!</code> examp
+00002910: 6c65 2c0a 0979 6f75 2061 7265 206e 6f77  le,..you are now
+00002920: 2077 656c 6c2d 6571 7569 7070 6564 2074   well-equipped t
+00002930: 6f20 6578 706c 6f72 6520 6d6f 7265 2069  o explore more i
+00002940: 6e74 7269 6361 7465 2065 7665 6e74 2d64  ntricate event-d
+00002950: 7269 7665 6e20 7363 656e 6172 696f 7320  riven scenarios 
+00002960: 616e 6420 6675 6c6c 7920 6861 726e 6573  and fully harnes
+00002970: 7320 7468 6520 6361 7061 6269 6c69 7469  s the capabiliti
+00002980: 6573 206f 6620 0a09 5079 7665 6e74 7573  es of ..Pyventus
+00002990: 2069 6e20 796f 7572 206f 776e 2070 726f   in your own pro
+000029a0: 6a65 6374 732e 2046 6f72 2061 2064 6565  jects. For a dee
+000029b0: 7020 6469 7665 2069 6e74 6f20 7468 6520  p dive into the 
+000029c0: 7061 636b 6167 6527 7320 6675 6e63 7469  package's functi
+000029d0: 6f6e 616c 6974 6965 732c 2079 6f75 2063  onalities, you c
+000029e0: 616e 2072 6566 6572 2074 6f20 7468 6520  an refer to the 
+000029f0: 0a09 5079 7665 6e74 7573 203c 6120 6872  ..Pyventus <a hr
+00002a00: 6566 3d22 6874 7470 733a 2f2f 6d64 6170  ef="https://mdap
+00002a10: 656e 612e 6769 7468 7562 2e69 6f2f 7079  ena.github.io/py
+00002a20: 7665 6e74 7573 2f74 7574 6f72 6961 6c73  ventus/tutorials
+00002a30: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+00002a40: 223e 5475 746f 7269 616c 733c 2f61 3e20  ">Tutorials</a> 
+00002a50: 6f72 200a 093c 6120 6872 6566 3d22 6874  or ..<a href="ht
+00002a60: 7470 733a 2f2f 6d64 6170 656e 612e 6769  tps://mdapena.gi
+00002a70: 7468 7562 2e69 6f2f 7079 7665 6e74 7573  thub.io/pyventus
+00002a80: 2f61 7069 2220 7461 7267 6574 3d22 5f62  /api" target="_b
+00002a90: 6c61 6e6b 223e 4150 493c 2f61 3e2e 0a3c  lank">API</a>..<
+00002aa0: 2f70 3e0a 0a5b 2f2f 5d3a 2023 2028 2d2d  /p>..[//]: # (--
+00002ab0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002ac0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002ad0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002ae0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002af0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002b00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002b10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 290a 0a23  ------------)..#
+00002b20: 2320 4120 5072 6163 7469 6361 6c20 4578  # A Practical Ex
+00002b30: 616d 706c 650a 0a3c 7020 7374 796c 653d  ample..<p style=
+00002b40: 2774 6578 742d 616c 6967 6e3a 206a 7573  'text-align: jus
+00002b50: 7469 6679 3b27 3e0a 2020 2020 2665 6d73  tify;'>.    &ems
+00002b60: 703b 2665 6d73 703b 546f 2073 686f 7763  p;&emsp;To showc
+00002b70: 6173 6520 5079 7665 6e74 7573 2720 6576  ase Pyventus' ev
+00002b80: 656e 742d 6472 6976 656e 2063 6170 6162  ent-driven capab
+00002b90: 696c 6974 6965 7320 696e 2061 2072 6561  ilities in a rea
+00002ba0: 6c2d 776f 726c 6420 7363 656e 6172 696f  l-world scenario
+00002bb0: 2c20 7765 2077 696c 6c20 6578 706c 6f72  , we will explor
+00002bc0: 6520 6120 7072 6163 7469 6361 6c20 0a09  e a practical ..
+00002bd0: 6578 616d 706c 6520 6f66 2069 6d70 6c65  example of imple
+00002be0: 6d65 6e74 696e 6720 6120 766f 6c74 6167  menting a voltag
+00002bf0: 6520 7365 6e73 6f72 2075 7369 6e67 2061  e sensor using a
+00002c00: 6e20 6576 656e 742d 6472 6976 656e 2061  n event-driven a
+00002c10: 7263 6869 7465 6374 7572 6520 2863 7275  rchitecture (cru
+00002c20: 6369 616c 2066 6f72 2073 7563 6820 7363  cial for such sc
+00002c30: 656e 6172 696f 7329 2e20 5468 6520 0a09  enarios). The ..
+00002c40: 7075 7270 6f73 6520 6f66 2074 6869 7320  purpose of this 
+00002c50: 6578 616d 706c 6520 6973 2074 6f20 6372  example is to cr
+00002c60: 6561 7465 2061 6e20 6566 6669 6369 656e  eate an efficien
+00002c70: 7420 766f 6c74 6167 6520 7365 6e73 6f72  t voltage sensor
+00002c80: 2074 6861 7420 6361 6e20 7365 616d 6c65   that can seamle
+00002c90: 7373 6c79 2068 616e 646c 6520 7265 616c  ssly handle real
+00002ca0: 2d74 696d 6520 6461 7461 200a 0961 6e64  -time data ..and
+00002cb0: 2072 6573 706f 6e64 2061 7070 726f 7072   respond appropr
+00002cc0: 6961 7465 6c79 2074 6f20 7370 6563 6966  iately to specif
+00002cd0: 6963 2076 6f6c 7461 6765 2063 6f6e 6469  ic voltage condi
+00002ce0: 7469 6f6e 732e 0a3c 2f70 3e0a 0a0a 3c64  tions..</p>...<d
+00002cf0: 6574 6169 6c73 206d 6172 6b64 6f77 6e3d  etails markdown=
+00002d00: 2231 2220 636c 6173 733d 2271 756f 7465  "1" class="quote
+00002d10: 2220 6f70 656e 3e0a 3c73 756d 6d61 7279  " open>.<summary
+00002d20: 3e45 7861 6d70 6c65 20e2 9480 204d 6f6e  >Example ... Mon
+00002d30: 6974 6f72 696e 6720 566f 6c74 6167 6520  itoring Voltage 
+00002d40: 4c65 7665 6c73 2041 6372 6f73 7320 4465  Levels Across De
+00002d50: 7669 6365 7320 2843 6f6e 7465 7874 293c  vices (Context)<
+00002d60: 2f73 756d 6d61 7279 3e0a 0a3c 6120 7374  /summary>..<a st
+00002d70: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
+00002d80: 2063 656e 7465 7222 2068 7265 663d 2268   center" href="h
+00002d90: 7474 7073 3a2f 2f75 6e73 706c 6173 682e  ttps://unsplash.
+00002da0: 636f 6d2f 7068 6f74 6f73 2f6d 6163 726f  com/photos/macro
+00002db0: 2d70 686f 746f 6772 6170 6879 2d6f 662d  -photography-of-
+00002dc0: 626c 6163 6b2d 6369 7263 7569 742d 626f  black-circuit-bo
+00002dd0: 6172 642d 464f 374a 496c 776a 4f74 553f  ard-FO7JIlwjOtU?
+00002de0: 7574 6d5f 636f 6e74 656e 743d 6372 6564  utm_content=cred
+00002df0: 6974 5368 6172 654c 696e 6b26 7574 6d5f  itShareLink&utm_
+00002e00: 6d65 6469 756d 3d72 6566 6572 7261 6c26  medium=referral&
+00002e10: 7574 6d5f 736f 7572 6365 3d75 6e73 706c  utm_source=unspl
+00002e20: 6173 6822 2074 6172 6765 743d 225f 626c  ash" target="_bl
+00002e30: 616e 6b22 3e0a 093c 696d 6720 7372 633d  ank">..<img src=
+00002e40: 2268 7474 7073 3a2f 2f6d 6461 7065 6e61  "https://mdapena
+00002e50: 2e67 6974 6875 622e 696f 2f70 7976 656e  .github.io/pyven
+00002e60: 7475 732f 696d 6167 6573 2f65 7861 6d70  tus/images/examp
+00002e70: 6c65 732f 7072 6163 7469 6361 6c2d 6578  les/practical-ex
+00002e80: 616d 706c 652d 696e 6465 782e 6a70 6722  ample-index.jpg"
+00002e90: 2061 6c74 3d22 4d61 6372 6f20 7068 6f74   alt="Macro phot
+00002ea0: 6f67 7261 7068 7920 6f66 2062 6c61 636b  ography of black
+00002eb0: 2063 6972 6375 6974 2062 6f61 7264 223e   circuit board">
+00002ec0: 0a3c 2f61 3e0a 0a3c 7020 7374 796c 653d  .</a>..<p style=
+00002ed0: 2774 6578 742d 616c 6967 6e3a 206a 7573  'text-align: jus
+00002ee0: 7469 6679 3b27 3e0a 093c 693e 2665 6d73  tify;'>..<i>&ems
+00002ef0: 703b 2665 6d73 703b 4120 636f 6d6d 6f6e  p;&emsp;A common
+00002f00: 2061 7370 6563 7420 666f 756e 6420 696e   aspect found in
+00002f10: 206d 616e 7920 7379 7374 656d 7320 6973   many systems is
+00002f20: 2074 6865 206e 6565 6420 746f 206d 6f6e   the need to mon
+00002f30: 6974 6f72 2061 6e64 2072 6573 706f 6e64  itor and respond
+00002f40: 2074 6f20 6368 616e 6765 7320 696e 2073   to changes in s
+00002f50: 656e 736f 7220 6461 7461 2e0a 0957 6865  ensor data...Whe
+00002f60: 7468 6572 2069 7427 7320 7072 6573 7375  ther it's pressu
+00002f70: 7265 2073 656e 736f 7273 2c20 7465 6d70  re sensors, temp
+00002f80: 6572 6174 7572 6520 7365 6e73 6f72 732c  erature sensors,
+00002f90: 206f 7220 6f74 6865 7220 7479 7065 732c   or other types,
+00002fa0: 2063 6170 7475 7269 6e67 2061 6e64 2072   capturing and r
+00002fb0: 6561 6374 696e 6720 746f 2073 656e 736f  eacting to senso
+00002fc0: 7220 6461 7461 2069 7320 6372 7563 6961  r data is crucia
+00002fd0: 6c0a 0966 6f72 2065 6666 6563 7469 7665  l..for effective
+00002fe0: 2073 7973 7465 6d20 6f70 6572 6174 696f   system operatio
+00002ff0: 6e2e 2049 6e20 6f75 7220 7072 6163 7469  n. In our practi
+00003000: 6361 6c20 6578 616d 706c 652c 2077 6520  cal example, we 
+00003010: 7769 6c6c 2066 6f63 7573 206f 6e20 6120  will focus on a 
+00003020: 7370 6563 6966 6963 2073 6365 6e61 7269  specific scenari
+00003030: 6f3a 2062 7569 6c64 696e 6720 6120 7365  o: building a se
+00003040: 6e73 6f72 200a 0973 7973 7465 6d20 7468  nsor ..system th
+00003050: 6174 206d 6f6e 6974 6f72 7320 766f 6c74  at monitors volt
+00003060: 6167 6520 6c65 7665 6c73 2061 6372 6f73  age levels acros
+00003070: 7320 6465 7669 6365 732e 2054 6865 2067  s devices. The g
+00003080: 6f61 6c20 6f66 206f 7572 2076 6f6c 7461  oal of our volta
+00003090: 6765 2073 656e 736f 7220 6973 2074 6f20  ge sensor is to 
+000030a0: 6465 7465 6374 2070 6f74 656e 7469 616c  detect potential
+000030b0: 2069 7373 7565 732c 0a09 7375 6368 2061   issues,..such a
+000030c0: 7320 6c6f 7720 6f72 2068 6967 6820 766f  s low or high vo
+000030d0: 6c74 6167 6520 636f 6e64 6974 696f 6e73  ltage conditions
+000030e0: 2c20 616e 6420 7265 7370 6f6e 6420 6170  , and respond ap
+000030f0: 7072 6f70 7269 6174 656c 7920 696e 2072  propriately in r
+00003100: 6561 6c2d 7469 6d65 2e3c 2f69 3e0a 3c2f  eal-time.</i>.</
+00003110: 703e 0a0a 3c2f 6465 7461 696c 733e 0a0a  p>..</details>..
+00003120: 0a3c 7020 7374 796c 653d 2774 6578 742d  .<p style='text-
+00003130: 616c 6967 6e3a 206a 7573 7469 6679 3b27  align: justify;'
+00003140: 3e0a 2020 2020 2665 6d73 703b 2665 6d73  >.    &emsp;&ems
+00003150: 703b 546f 2061 6363 6f6d 706c 6973 6820  p;To accomplish 
+00003160: 6f75 7220 676f 616c 2c20 7765 2077 696c  our goal, we wil
+00003170: 6c20 6465 6669 6e65 2061 203c 636f 6465  l define a <code
+00003180: 3e56 6f6c 7461 6765 5365 6e73 6f72 3c2f  >VoltageSensor</
+00003190: 636f 6465 3e20 636c 6173 7320 746f 2072  code> class to r
+000031a0: 6561 6420 766f 6c74 6167 6520 6c65 7665  ead voltage leve
+000031b0: 6c73 2061 6e64 2065 6d69 7420 0a09 6576  ls and emit ..ev
+000031c0: 656e 7473 2062 6173 6564 206f 6e20 7072  ents based on pr
+000031d0: 6564 6566 696e 6564 2074 6872 6573 686f  edefined thresho
+000031e0: 6c64 732e 2057 6520 7769 6c6c 2063 7265  lds. We will cre
+000031f0: 6174 6520 6576 656e 7420 6861 6e64 6c65  ate event handle
+00003200: 7273 2074 6f20 7265 7370 6f6e 6420 746f  rs to respond to
+00003210: 2074 6865 7365 2065 7665 6e74 732c 2070   these events, p
+00003220: 6572 666f 726d 696e 6720 6163 7469 6f6e  erforming action
+00003230: 7320 0a09 7375 6368 2061 7320 6163 7469  s ..such as acti
+00003240: 7661 7469 6e67 2065 636f 2d6d 6f64 6520  vating eco-mode 
+00003250: 666f 7220 6c6f 7720 766f 6c74 6167 6520  for low voltage 
+00003260: 6f72 2069 6d70 6c65 6d65 6e74 696e 6720  or implementing 
+00003270: 6869 6768 2d76 6f6c 7461 6765 2070 726f  high-voltage pro
+00003280: 7465 6374 696f 6e2e 2041 6464 6974 696f  tection. Additio
+00003290: 6e61 6c6c 792c 2061 2073 6861 7265 6420  nally, a shared 
+000032a0: 6576 656e 7420 0a09 6861 6e64 6c65 7220  event ..handler 
+000032b0: 7769 6c6c 2070 726f 7669 6465 2067 656e  will provide gen
+000032c0: 6572 616c 206e 6f74 6966 6963 6174 696f  eral notificatio
+000032d0: 6e73 2066 6f72 206f 7574 2d6f 662d 7261  ns for out-of-ra
+000032e0: 6e67 6520 766f 6c74 6167 6520 7369 7475  nge voltage situ
+000032f0: 6174 696f 6e73 2e20 5468 6520 636f 6465  ations. The code
+00003300: 2065 7861 6d70 6c65 2062 656c 6f77 2069   example below i
+00003310: 6c6c 7573 7472 6174 6573 200a 0974 6865  llustrates ..the
+00003320: 2069 6d70 6c65 6d65 6e74 6174 696f 6e20   implementation 
+00003330: 6f66 2074 6869 7320 7379 7374 656d 2e0a  of this system..
+00003340: 3c2f 703e 0a0a 6060 6050 7974 686f 6e20  </p>..```Python 
+00003350: 7469 746c 653d 2256 6f6c 7461 6765 2053  title="Voltage S
+00003360: 656e 736f 7220 5379 7374 656d 2077 6974  ensor System wit
+00003370: 6820 5079 7665 6e74 7573 2028 5072 6163  h Pyventus (Prac
+00003380: 7469 6361 6c20 4578 616d 706c 6529 2220  tical Example)" 
+00003390: 6c69 6e65 6e75 6d73 3d22 3122 2068 6c5f  linenums="1" hl_
+000033a0: 6c69 6e65 733d 2239 2031 3420 3237 2d33  lines="9 14 27-3
+000033b0: 3020 3335 2d33 3620 3431 2d34 3220 3437  0 35-36 41-42 47
+000033c0: 2d34 3820 3535 220a 696d 706f 7274 2061  -48 55".import a
+000033d0: 7379 6e63 696f 0a69 6d70 6f72 7420 7261  syncio.import ra
+000033e0: 6e64 6f6d 0a0a 6672 6f6d 2070 7976 656e  ndom..from pyven
+000033f0: 7475 7320 696d 706f 7274 2045 7665 6e74  tus import Event
+00003400: 456d 6974 7465 722c 2045 7665 6e74 4c69  Emitter, EventLi
+00003410: 6e6b 6572 2c20 4173 796e 6349 4f45 7665  nker, AsyncIOEve
+00003420: 6e74 456d 6974 7465 720a 0a0a 636c 6173  ntEmitter...clas
+00003430: 7320 566f 6c74 6167 6553 656e 736f 723a  s VoltageSensor:
+00003440: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
+00003450: 5f5f 2873 656c 662c 206e 616d 653a 2073  __(self, name: s
+00003460: 7472 2c20 6c6f 773a 2066 6c6f 6174 2c20  tr, low: float, 
+00003470: 6869 6768 3a20 666c 6f61 742c 2065 7665  high: float, eve
+00003480: 6e74 5f65 6d69 7474 6572 3a20 4576 656e  nt_emitter: Even
+00003490: 7445 6d69 7474 6572 2920 2d3e 204e 6f6e  tEmitter) -> Non
+000034a0: 653a 0a20 2020 2020 2020 2023 2049 6e69  e:.        # Ini
+000034b0: 7469 616c 697a 6520 7468 6520 566f 6c74  tialize the Volt
+000034c0: 6167 6553 656e 736f 7220 6f62 6a65 6374  ageSensor object
+000034d0: 2077 6974 6820 7468 6520 7072 6f76 6964   with the provid
+000034e0: 6564 2070 6172 616d 6574 6572 730a 2020  ed parameters.  
+000034f0: 2020 2020 2020 7365 6c66 2e5f 6e61 6d65        self._name
+00003500: 3a20 7374 7220 3d20 6e61 6d65 0a20 2020  : str = name.   
+00003510: 2020 2020 2073 656c 662e 5f6c 6f77 3a20       self._low: 
+00003520: 666c 6f61 7420 3d20 6c6f 770a 2020 2020  float = low.    
+00003530: 2020 2020 7365 6c66 2e5f 6869 6768 3a20      self._high: 
+00003540: 666c 6f61 7420 3d20 6869 6768 0a20 2020  float = high.   
+00003550: 2020 2020 2073 656c 662e 5f65 7665 6e74       self._event
+00003560: 5f65 6d69 7474 6572 3a20 4576 656e 7445  _emitter: EventE
+00003570: 6d69 7474 6572 203d 2065 7665 6e74 5f65  mitter = event_e
+00003580: 6d69 7474 6572 0a0a 2020 2020 6173 796e  mitter..    asyn
+00003590: 6320 6465 6620 5f5f 6361 6c6c 5f5f 2873  c def __call__(s
+000035a0: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
+000035b0: 2020 2020 2020 2320 5374 6172 7420 766f        # Start vo
+000035c0: 6c74 6167 6520 7265 6164 696e 6773 2066  ltage readings f
+000035d0: 6f72 2074 6865 2073 656e 736f 720a 2020  or the sensor.  
+000035e0: 2020 2020 2020 7072 696e 7428 6622 5374        print(f"St
+000035f0: 6172 7469 6e67 2076 6f6c 7461 6765 2072  arting voltage r
+00003600: 6561 6469 6e67 7320 666f 723a 207b 7365  eadings for: {se
+00003610: 6c66 2e5f 6e61 6d65 7d22 290a 2020 2020  lf._name}").    
+00003620: 2020 2020 7072 696e 7428 6622 4c6f 773a      print(f"Low:
+00003630: 207b 7365 6c66 2e5f 6c6f 773a 2e33 677d   {self._low:.3g}
+00003640: 7620 7c20 4869 6768 3a20 7b73 656c 662e  v | High: {self.
+00003650: 5f68 6967 683a 2e33 677d 765c 6e2d 2d2d  _high:.3g}v\n---
+00003660: 2d2d 2d2d 2d2d 2d2d 5c6e 2229 0a0a 2020  --------\n")..  
+00003670: 2020 2020 2020 7768 696c 6520 5472 7565        while True
+00003680: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+00003690: 5369 6d75 6c61 7465 2073 656e 736f 7220  Simulate sensor 
+000036a0: 7265 6164 696e 6773 0a20 2020 2020 2020  readings.       
+000036b0: 2020 2020 2076 6f6c 7461 6765 3a20 666c       voltage: fl
+000036c0: 6f61 7420 3d20 7261 6e64 6f6d 2e75 6e69  oat = random.uni
+000036d0: 666f 726d 2830 2c20 3529 0a20 2020 2020  form(0, 5).     
+000036e0: 2020 2020 2020 2070 7269 6e74 2822 5c74         print("\t
+000036f0: 5365 6e73 6f72 2052 6561 6469 6e67 3a22  Sensor Reading:"
+00003700: 2c20 225c 3033 335b 3332 6d22 2c20 6622  , "\033[32m", f"
+00003710: 7b76 6f6c 7461 6765 3a2e 3367 7d76 222c  {voltage:.3g}v",
+00003720: 2022 5c30 3333 5b30 6d22 290a 0a20 2020   "\033[0m")..   
+00003730: 2020 2020 2020 2020 2023 2045 6d69 7420           # Emit 
+00003740: 6576 656e 7473 2062 6173 6564 206f 6e20  events based on 
+00003750: 766f 6c74 6167 6520 7265 6164 696e 6773  voltage readings
+00003760: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00003770: 766f 6c74 6167 6520 3c20 7365 6c66 2e5f  voltage < self._
+00003780: 6c6f 773a 0a20 2020 2020 2020 2020 2020  low:.           
+00003790: 2020 2020 2073 656c 662e 5f65 7665 6e74       self._event
+000037a0: 5f65 6d69 7474 6572 2e65 6d69 7428 224c  _emitter.emit("L
+000037b0: 6f77 566f 6c74 6167 6545 7665 6e74 222c  owVoltageEvent",
+000037c0: 2073 656e 736f 723d 7365 6c66 2e5f 6e61   sensor=self._na
+000037d0: 6d65 2c20 766f 6c74 6167 653d 766f 6c74  me, voltage=volt
+000037e0: 6167 6529 0a20 2020 2020 2020 2020 2020  age).           
+000037f0: 2065 6c69 6620 766f 6c74 6167 6520 3e20   elif voltage > 
+00003800: 7365 6c66 2e5f 6869 6768 3a0a 2020 2020  self._high:.    
+00003810: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003820: 2e5f 6576 656e 745f 656d 6974 7465 722e  ._event_emitter.
+00003830: 656d 6974 2822 4869 6768 566f 6c74 6167  emit("HighVoltag
+00003840: 6545 7665 6e74 222c 2073 656e 736f 723d  eEvent", sensor=
+00003850: 7365 6c66 2e5f 6e61 6d65 2c20 766f 6c74  self._name, volt
+00003860: 6167 653d 766f 6c74 6167 6529 0a0a 2020  age=voltage)..  
+00003870: 2020 2020 2020 2020 2020 6177 6169 7420            await 
+00003880: 6173 796e 6369 6f2e 736c 6565 7028 3129  asyncio.sleep(1)
+00003890: 0a0a 0a40 4576 656e 744c 696e 6b65 722e  ...@EventLinker.
+000038a0: 6f6e 2822 4c6f 7756 6f6c 7461 6765 4576  on("LowVoltageEv
+000038b0: 656e 7422 290a 6465 6620 6861 6e64 6c65  ent").def handle
+000038c0: 5f6c 6f77 5f76 6f6c 7461 6765 5f65 7665  _low_voltage_eve
+000038d0: 6e74 2873 656e 736f 723a 2073 7472 2c20  nt(sensor: str, 
+000038e0: 766f 6c74 6167 653a 2066 6c6f 6174 293a  voltage: float):
+000038f0: 0a20 2020 2070 7269 6e74 2866 22f0 9faa  .    print(f"...
+00003900: ab20 5475 726e 696e 6720 6f6e 2065 636f  . Turning on eco
+00003910: 2d6d 6f64 6520 666f 7220 277b 7365 6e73  -mode for '{sens
+00003920: 6f72 7d27 2e20 287b 766f 6c74 6167 653a  or}'. ({voltage:
+00003930: 2e33 677d 7629 5c6e 2229 0a20 2020 2023  .3g}v)\n").    #
+00003940: 2050 6572 666f 726d 2061 6374 696f 6e20   Perform action 
+00003950: 666f 7220 6c6f 7720 766f 6c74 6167 652e  for low voltage.
+00003960: 2e2e 0a0a 0a40 4576 656e 744c 696e 6b65  .....@EventLinke
+00003970: 722e 6f6e 2822 4869 6768 566f 6c74 6167  r.on("HighVoltag
+00003980: 6545 7665 6e74 2229 0a61 7379 6e63 2064  eEvent").async d
+00003990: 6566 2068 616e 646c 655f 6869 6768 5f76  ef handle_high_v
+000039a0: 6f6c 7461 6765 5f65 7665 6e74 2873 656e  oltage_event(sen
+000039b0: 736f 723a 2073 7472 2c20 766f 6c74 6167  sor: str, voltag
+000039c0: 653a 2066 6c6f 6174 293a 0a20 2020 2070  e: float):.    p
+000039d0: 7269 6e74 2866 22e2 9aa1 2053 7461 7274  rint(f"... Start
+000039e0: 696e 6720 6869 6768 2d76 6f6c 7461 6765  ing high-voltage
+000039f0: 2070 726f 7465 6374 696f 6e20 666f 7220   protection for 
+00003a00: 277b 7365 6e73 6f72 7d27 2e20 287b 766f  '{sensor}'. ({vo
+00003a10: 6c74 6167 653a 2e33 677d 7629 5c6e 2229  ltage:.3g}v)\n")
+00003a20: 0a20 2020 2023 2050 6572 666f 726d 2061  .    # Perform a
+00003a30: 6374 696f 6e20 666f 7220 6869 6768 2076  ction for high v
+00003a40: 6f6c 7461 6765 2e2e 2e0a 0a0a 4045 7665  oltage......@Eve
+00003a50: 6e74 4c69 6e6b 6572 2e6f 6e28 224c 6f77  ntLinker.on("Low
+00003a60: 566f 6c74 6167 6545 7665 6e74 222c 2022  VoltageEvent", "
+00003a70: 4869 6768 566f 6c74 6167 6545 7665 6e74  HighVoltageEvent
+00003a80: 2229 0a64 6566 2068 616e 646c 655f 766f  ").def handle_vo
+00003a90: 6c74 6167 655f 6576 656e 7428 7365 6e73  ltage_event(sens
+00003aa0: 6f72 3a20 7374 722c 2076 6f6c 7461 6765  or: str, voltage
+00003ab0: 3a20 666c 6f61 7429 3a0a 2020 2020 7072  : float):.    pr
+00003ac0: 696e 7428 6622 5c30 3333 5b33 316d 5c6e  int(f"\033[31m\n
+00003ad0: 5365 6e73 6f72 2027 7b73 656e 736f 727d  Sensor '{sensor}
+00003ae0: 2720 6f75 7420 6f66 2072 616e 6765 2e5c  ' out of range.\
+00003af0: 3033 335b 306d 2028 566f 6c74 6167 653a  033[0m (Voltage:
+00003b00: 207b 766f 6c74 6167 653a 2e33 677d 2922   {voltage:.3g})"
+00003b10: 290a 2020 2020 2320 5065 7266 6f72 6d20  ).    # Perform 
+00003b20: 6e6f 7469 6669 6361 7469 6f6e 2066 6f72  notification for
+00003b30: 206f 7574 206f 6620 7261 6e67 6520 766f   out of range vo
+00003b40: 6c74 6167 652e 2e2e 0a0a 0a61 7379 6e63  ltage......async
+00003b50: 2064 6566 206d 6169 6e28 293a 0a20 2020   def main():.   
+00003b60: 2023 2049 6e69 7469 616c 697a 6520 7468   # Initialize th
+00003b70: 6520 7365 6e73 6f72 2061 6e64 2072 756e  e sensor and run
+00003b80: 2074 6865 2073 656e 736f 7220 7265 6164   the sensor read
+00003b90: 696e 6773 0a20 2020 2073 656e 736f 7220  ings.    sensor 
+00003ba0: 3d20 566f 6c74 6167 6553 656e 736f 7228  = VoltageSensor(
+00003bb0: 6e61 6d65 3d22 5072 6573 7375 7265 5365  name="PressureSe
+00003bc0: 6e73 6f72 222c 206c 6f77 3d30 2e35 2c20  nsor", low=0.5, 
+00003bd0: 6869 6768 3d33 2e39 2c20 6576 656e 745f  high=3.9, event_
+00003be0: 656d 6974 7465 723d 4173 796e 6349 4f45  emitter=AsyncIOE
+00003bf0: 7665 6e74 456d 6974 7465 7228 2929 0a20  ventEmitter()). 
+00003c00: 2020 2061 7761 6974 2061 7379 6e63 696f     await asyncio
+00003c10: 2e67 6174 6865 7228 7365 6e73 6f72 2829  .gather(sensor()
+00003c20: 2c20 2920 2023 2041 6464 206e 6577 2073  , )  # Add new s
+00003c30: 656e 736f 7273 2069 6e73 6964 6520 7468  ensors inside th
+00003c40: 6520 2767 6174 6865 7227 2066 6f72 206d  e 'gather' for m
+00003c50: 756c 7469 2d64 6576 6963 6520 6d6f 6e69  ulti-device moni
+00003c60: 746f 7269 6e67 0a0a 0a61 7379 6e63 696f  toring...asyncio
+00003c70: 2e72 756e 286d 6169 6e28 2929 0a60 6060  .run(main()).```
+00003c80: 0a0a 3c70 2073 7479 6c65 3d27 7465 7874  ..<p style='text
+00003c90: 2d61 6c69 676e 3a20 6a75 7374 6966 793b  -align: justify;
+00003ca0: 273e 0a20 2020 2026 656d 7370 3b26 656d  '>.    &emsp;&em
+00003cb0: 7370 3b41 7320 7765 2063 616e 2073 6565  sp;As we can see
+00003cc0: 2066 726f 6d20 7468 6973 2070 7261 6374   from this pract
+00003cd0: 6963 616c 2065 7861 6d70 6c65 2c20 5079  ical example, Py
+00003ce0: 7665 6e74 7573 2065 6e61 626c 6573 2075  ventus enables u
+00003cf0: 7320 746f 2065 6173 696c 7920 6275 696c  s to easily buil
+00003d00: 6420 616e 2065 7665 6e74 2d64 7269 7665  d an event-drive
+00003d10: 6e20 7379 7374 656d 200a 0966 6f72 2076  n system ..for v
+00003d20: 6f6c 7461 6765 2073 656e 736f 7273 2074  oltage sensors t
+00003d30: 6861 7420 6973 2066 6c65 7869 626c 652c  hat is flexible,
+00003d40: 2065 6666 6963 6965 6e74 2c20 616e 6420   efficient, and 
+00003d50: 6869 6768 6c79 2072 6573 706f 6e73 6976  highly responsiv
+00003d60: 652e 2057 6974 6820 6974 7320 696e 7475  e. With its intu
+00003d70: 6974 6976 6520 4150 4920 616e 6420 7375  itive API and su
+00003d80: 7070 6f72 7420 666f 7220 626f 7468 0a09  pport for both..
+00003d90: 7379 6e63 6872 6f6e 6f75 7320 616e 6420  synchronous and 
+00003da0: 6173 796e 6368 726f 6e6f 7573 206f 7065  asynchronous ope
+00003db0: 7261 7469 6f6e 732c 2077 6520 7765 7265  rations, we were
+00003dc0: 2061 626c 6520 746f 2065 6666 6563 7469   able to effecti
+00003dd0: 7665 6c79 206d 6f6e 6974 6f72 2076 6f6c  vely monitor vol
+00003de0: 7461 6765 206c 6576 656c 732c 2064 6574  tage levels, det
+00003df0: 6563 7420 616e 6f6d 616c 6965 732c 2061  ect anomalies, a
+00003e00: 6e64 200a 0974 7269 6767 6572 2061 7070  nd ..trigger app
+00003e10: 726f 7072 6961 7465 2061 6374 696f 6e73  ropriate actions
+00003e20: 2069 6e20 7265 616c 2d74 696d 652e 0a3c   in real-time..<
+00003e30: 2f70 3e0a 0a5b 2f2f 5d3a 2023 2028 2d2d  /p>..[//]: # (--
+00003e40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003e50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003e60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003e70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003e80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003e90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003ea0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 290a 0a23  ------------)..#
+00003eb0: 2320 5375 7070 6f72 7420 666f 7220 5379  # Support for Sy
+00003ec0: 6e63 6872 6f6e 6f75 7320 616e 6420 4173  nchronous and As
+00003ed0: 796e 6368 726f 6e6f 7573 2043 6f64 650a  ynchronous Code.
+00003ee0: 0a3c 7020 7374 796c 653d 2774 6578 742d  .<p style='text-
+00003ef0: 616c 6967 6e3a 206a 7573 7469 6679 3b27  align: justify;'
+00003f00: 3e0a 2020 2020 2665 6d73 703b 2665 6d73  >.    &emsp;&ems
+00003f10: 703b 5079 7665 6e74 7573 2069 7320 6465  p;Pyventus is de
+00003f20: 7369 676e 6564 2066 726f 6d20 7468 6520  signed from the 
+00003f30: 6772 6f75 6e64 2075 7020 746f 2073 6561  ground up to sea
+00003f40: 6d6c 6573 736c 7920 7375 7070 6f72 7420  mlessly support 
+00003f50: 626f 7468 2073 796e 6368 726f 6e6f 7573  both synchronous
+00003f60: 2061 6e64 2061 7379 6e63 6872 6f6e 6f75   and asynchronou
+00003f70: 730a 0970 726f 6772 616d 6d69 6e67 206d  s..programming m
+00003f80: 6f64 656c 732e 2049 7473 2075 6e69 6669  odels. Its unifi
+00003f90: 6564 2073 796e 632f 6173 796e 6320 4150  ed sync/async AP
+00003fa0: 4920 616c 6c6f 7773 2079 6f75 2074 6f20  I allows you to 
+00003fb0: 6465 6669 6e65 2065 7665 6e74 2063 616c  define event cal
+00003fc0: 6c62 6163 6b73 2061 6e64 2065 6d69 7420  lbacks and emit 
+00003fd0: 6576 656e 7473 2061 6372 6f73 7320 0a09  events across ..
+00003fe0: 3c63 6f64 653e 7379 6e63 3c2f 636f 6465  <code>sync</code
+00003ff0: 3e20 616e 6420 3c63 6f64 653e 6173 796e  > and <code>asyn
+00004000: 633c 2f63 6f64 653e 2063 6f6e 7465 7874  c</code> context
+00004010: 732e 0a3c 2f70 3e0a 0a23 2323 2053 7562  s..</p>..### Sub
+00004020: 7363 7269 6269 6e67 2045 7665 6e74 2048  scribing Event H
+00004030: 616e 646c 6572 7320 7769 7468 203c 636f  andlers with <co
+00004040: 6465 3e53 796e 633c 2f63 6f64 653e 2061  de>Sync</code> a
+00004050: 6e64 203c 636f 6465 3e41 7379 6e63 3c2f  nd <code>Async</
+00004060: 636f 6465 3e20 4361 6c6c 6261 636b 730a  code> Callbacks.
+00004070: 0a60 6060 5079 7468 6f6e 206c 696e 656e  .```Python linen
+00004080: 756d 733d 2231 2220 686c 5f6c 696e 6573  ums="1" hl_lines
+00004090: 3d22 3220 3722 0a40 4576 656e 744c 696e  ="2 7".@EventLin
+000040a0: 6b65 722e 6f6e 2822 4d79 4576 656e 7422  ker.on("MyEvent"
+000040b0: 290a 6465 6620 7379 6e63 5f65 7665 6e74  ).def sync_event
+000040c0: 5f63 616c 6c62 6163 6b28 293a 0a20 2020  _callback():.   
+000040d0: 2070 6173 7320 2023 2053 796e 6368 726f   pass  # Synchro
+000040e0: 6e6f 7573 2065 7665 6e74 2068 616e 646c  nous event handl
+000040f0: 696e 670a 0a0a 4045 7665 6e74 4c69 6e6b  ing...@EventLink
+00004100: 6572 2e6f 6e28 224d 7945 7665 6e74 2229  er.on("MyEvent")
+00004110: 0a61 7379 6e63 2064 6566 2061 7379 6e63  .async def async
+00004120: 5f65 7665 6e74 5f63 616c 6c62 6163 6b28  _event_callback(
+00004130: 293a 0a09 7061 7373 2020 2320 4173 796e  ):..pass  # Asyn
+00004140: 6368 726f 6e6f 7573 2065 7665 6e74 2068  chronous event h
+00004150: 616e 646c 696e 670a 6060 600a 0a3c 6465  andling.```..<de
+00004160: 7461 696c 7320 6d61 726b 646f 776e 3d22  tails markdown="
+00004170: 3122 2063 6c61 7373 3d22 696e 666f 223e  1" class="info">
+00004180: 0a3c 7375 6d6d 6172 793e 596f 7520 6361  .<summary>You ca
+00004190: 6e20 6f70 7469 6d69 7a65 2074 6865 2065  n optimize the e
+000041a0: 7865 6375 7469 6f6e 206f 6620 796f 7572  xecution of your
+000041b0: 2063 616c 6c62 6163 6b73 2062 6173 6564   callbacks based
+000041c0: 206f 6e20 7468 6569 7220 776f 726b 6c6f   on their worklo
+000041d0: 6164 2e2e 2e3c 2f73 756d 6d61 7279 3e0a  ad...</summary>.
+000041e0: 0a3c 7020 7374 796c 653d 2774 6578 742d  .<p style='text-
+000041f0: 616c 6967 6e3a 206a 7573 7469 6679 3b27  align: justify;'
+00004200: 3e0a 2020 2020 2665 6d73 703b 2665 6d73  >.    &emsp;&ems
+00004210: 703b 4279 2064 6566 6175 6c74 2c20 6576  p;By default, ev
+00004220: 656e 7420 6861 6e64 6c65 7273 2069 6e20  ent handlers in 
+00004230: 5079 7665 6e74 7573 2061 7265 2065 7865  Pyventus are exe
+00004240: 6375 7465 6420 636f 6e63 7572 7265 6e74  cuted concurrent
+00004250: 6c79 2064 7572 696e 6720 616e 2065 7665  ly during an eve
+00004260: 6e74 2065 6d69 7373 696f 6e2c 2072 756e  nt emission, run
+00004270: 6e69 6e67 2074 6865 6972 0a09 3c63 6f64  ning their..<cod
+00004280: 653e 7379 6e63 3c2f 636f 6465 3e20 616e  e>sync</code> an
+00004290: 6420 3c63 6f64 653e 6173 796e 633c 2f63  d <code>async</c
+000042a0: 6f64 653e 2063 616c 6c62 6163 6b73 2061  ode> callbacks a
+000042b0: 7320 6465 6669 6e65 642e 2048 6f77 6576  s defined. Howev
+000042c0: 6572 2c20 6966 2079 6f75 2068 6176 6520  er, if you have 
+000042d0: 6120 3c63 6f64 653e 7379 6e63 3c2f 636f  a <code>sync</co
+000042e0: 6465 3e20 6361 6c6c 6261 636b 0a09 7468  de> callback..th
+000042f0: 6174 2069 6e76 6f6c 7665 7320 492f 4f20  at involves I/O 
+00004300: 6f72 206e 6f6e 2d43 5055 2062 6f75 6e64  or non-CPU bound
+00004310: 206f 7065 7261 7469 6f6e 732c 2079 6f75   operations, you
+00004320: 2063 616e 2065 6e61 626c 6520 7468 6520   can enable the 
+00004330: 3c63 6f64 653e 666f 7263 655f 6173 796e  <code>force_asyn
+00004340: 633c 2f63 6f64 653e 2070 6172 616d 6574  c</code> paramet
+00004350: 6572 2074 6f20 6f66 666c 6f61 6420 6974  er to offload it
+00004360: 0a09 746f 2061 2074 6872 6561 6420 706f  ..to a thread po
+00004370: 6f6c 2c20 656e 7375 7269 6e67 206f 7074  ol, ensuring opt
+00004380: 696d 616c 2070 6572 666f 726d 616e 6365  imal performance
+00004390: 2061 6e64 2072 6573 706f 6e73 6976 656e   and responsiven
+000043a0: 6573 732e 2054 6865 203c 636f 6465 3e66  ess. The <code>f
+000043b0: 6f72 6365 5f61 7379 6e63 3c2f 636f 6465  orce_async</code
+000043c0: 3e20 7061 7261 6d65 7465 7220 7574 696c  > parameter util
+000043d0: 697a 6573 200a 0974 6865 203c 6120 6872  izes ..the <a hr
+000043e0: 6566 3d22 6874 7470 733a 2f2f 646f 6373  ef="https://docs
+000043f0: 2e70 7974 686f 6e2e 6f72 672f 332f 6c69  .python.org/3/li
+00004400: 6272 6172 792f 6173 796e 6369 6f2d 7461  brary/asyncio-ta
+00004410: 736b 2e68 746d 6c23 7275 6e6e 696e 672d  sk.html#running-
+00004420: 696e 2d74 6872 6561 6473 2220 7461 7267  in-threads" targ
+00004430: 6574 3d22 5f62 6c61 6e6b 223e 3c63 6f64  et="_blank"><cod
+00004440: 653e 6173 796e 6369 6f2e 746f 5f74 6872  e>asyncio.to_thr
+00004450: 6561 6428 293c 2f63 6f64 653e 3c2f 613e  ead()</code></a>
+00004460: 0a09 6675 6e63 7469 6f6e 2074 6f20 6578  ..function to ex
+00004470: 6563 7574 6520 3c63 6f64 653e 7379 6e63  ecute <code>sync
+00004480: 3c2f 636f 6465 3e20 6361 6c6c 6261 636b  </code> callback
+00004490: 7320 6173 796e 6368 726f 6e6f 7573 6c79  s asynchronously
+000044a0: 2e0a 3c2f 703e 0a0a 6060 6050 7974 686f  ..</p>..```Pytho
+000044b0: 6e20 6c69 6e65 6e75 6d73 3d22 3122 2068  n linenums="1" h
+000044c0: 6c5f 6c69 6e65 733d 2231 220a 4045 7665  l_lines="1".@Eve
+000044d0: 6e74 4c69 6e6b 6572 2e6f 6e28 2242 6c6f  ntLinker.on("Blo
+000044e0: 636b 696e 6749 4f22 2c20 666f 7263 655f  ckingIO", force_
+000044f0: 6173 796e 633d 5472 7565 290a 6465 6620  async=True).def 
+00004500: 626c 6f63 6b69 6e67 5f69 6f28 293a 0a20  blocking_io():. 
+00004510: 2020 2070 7269 6e74 2866 2273 7461 7274     print(f"start
+00004520: 2062 6c6f 636b 696e 675f 696f 2061 7420   blocking_io at 
+00004530: 7b74 696d 652e 7374 7266 7469 6d65 2827  {time.strftime('
+00004540: 2558 2729 7d22 290a 2020 2020 2320 4e6f  %X')}").    # No
+00004550: 7465 2074 6861 7420 7469 6d65 2e73 6c65  te that time.sle
+00004560: 6570 2829 2063 616e 2062 6520 7265 706c  ep() can be repl
+00004570: 6163 6564 2077 6974 6820 616e 7920 626c  aced with any bl
+00004580: 6f63 6b69 6e67 0a20 2020 2023 2049 4f2d  ocking.    # IO-
+00004590: 626f 756e 6420 6f70 6572 6174 696f 6e2c  bound operation,
+000045a0: 2073 7563 6820 6173 2066 696c 6520 6f70   such as file op
+000045b0: 6572 6174 696f 6e73 2e0a 2020 2020 7469  erations..    ti
+000045c0: 6d65 2e73 6c65 6570 2831 290a 2020 2020  me.sleep(1).    
+000045d0: 7072 696e 7428 6622 626c 6f63 6b69 6e67  print(f"blocking
+000045e0: 5f69 6f20 636f 6d70 6c65 7465 2061 7420  _io complete at 
+000045f0: 7b74 696d 652e 7374 7266 7469 6d65 2827  {time.strftime('
+00004600: 2558 2729 7d22 290a 6060 600a 0a3c 2f64  %X')}").```..</d
+00004610: 6574 6169 6c73 3e0a 0a23 2323 2045 6d69  etails>..### Emi
+00004620: 7474 696e 6720 4576 656e 7473 2066 726f  tting Events fro
+00004630: 6d20 3c63 6f64 653e 5379 6e63 3c2f 636f  m <code>Sync</co
+00004640: 6465 3e20 616e 6420 3c63 6f64 653e 4173  de> and <code>As
+00004650: 796e 633c 2f63 6f64 653e 2043 6f6e 7465  ync</code> Conte
+00004660: 7874 730a 0a60 6060 5079 7468 6f6e 206c  xts..```Python l
+00004670: 696e 656e 756d 733d 2231 2220 686c 5f6c  inenums="1" hl_l
+00004680: 696e 6573 3d22 3320 3822 0a23 2045 6d69  ines="3 8".# Emi
+00004690: 7474 696e 6720 616e 2065 7665 6e74 2077  tting an event w
+000046a0: 6974 6869 6e20 6120 7379 6e63 2066 756e  ithin a sync fun
+000046b0: 6374 696f 6e0a 6465 6620 7379 6e63 5f66  ction.def sync_f
+000046c0: 756e 6374 696f 6e28 6576 656e 745f 656d  unction(event_em
+000046d0: 6974 7465 723a 2045 7665 6e74 456d 6974  itter: EventEmit
+000046e0: 7465 7229 3a0a 2020 2020 6576 656e 745f  ter):.    event_
+000046f0: 656d 6974 7465 722e 656d 6974 2822 4d79  emitter.emit("My
+00004700: 4576 656e 7422 290a 0a0a 2320 456d 6974  Event")...# Emit
+00004710: 7469 6e67 2061 6e20 6576 656e 7420 7769  ting an event wi
+00004720: 7468 696e 2061 6e20 6173 796e 6320 6675  thin an async fu
+00004730: 6e63 7469 6f6e 0a61 7379 6e63 2064 6566  nction.async def
+00004740: 2061 7379 6e63 5f66 756e 6374 696f 6e28   async_function(
+00004750: 6576 656e 745f 656d 6974 7465 723a 2045  event_emitter: E
+00004760: 7665 6e74 456d 6974 7465 7229 3a0a 2020  ventEmitter):.  
+00004770: 2020 6576 656e 745f 656d 6974 7465 722e    event_emitter.
+00004780: 656d 6974 2822 4d79 4576 656e 7422 290a  emit("MyEvent").
+00004790: 6060 600a 0a3c 6465 7461 696c 7320 6d61  ```..<details ma
+000047a0: 726b 646f 776e 3d22 3122 2063 6c61 7373  rkdown="1" class
+000047b0: 3d22 696e 666f 223e 0a3c 7375 6d6d 6172  ="info">.<summar
+000047c0: 793e 4576 656e 7420 7072 6f70 6167 6174  y>Event propagat
+000047d0: 696f 6e20 7769 7468 696e 2064 6966 6665  ion within diffe
+000047e0: 7265 6e74 2063 6f6e 7465 7874 732e 2e2e  rent contexts...
+000047f0: 3c2f 7375 6d6d 6172 793e 0a0a 3c70 2073  </summary>..<p s
+00004800: 7479 6c65 3d27 7465 7874 2d61 6c69 676e  tyle='text-align
+00004810: 3a20 6a75 7374 6966 793b 273e 0a20 2020  : justify;'>.   
+00004820: 2026 656d 7370 3b26 656d 7370 3b57 6869   &emsp;&emsp;Whi
+00004830: 6c65 2050 7976 656e 7475 7320 7072 6f76  le Pyventus prov
+00004840: 6964 6573 2061 2062 6173 6520 3c63 6f64  ides a base <cod
+00004850: 653e 4576 656e 7445 6d69 7474 6572 3c2f  e>EventEmitter</
+00004860: 636f 6465 3e20 636c 6173 7320 7769 7468  code> class with
+00004870: 2061 2075 6e69 6669 6564 2073 796e 632f   a unified sync/
+00004880: 6173 796e 6320 4150 492c 2074 6865 200a  async API, the .
+00004890: 0973 7065 6369 6669 6320 7072 6f70 6167  .specific propag
+000048a0: 6174 696f 6e20 6265 6861 7669 6f72 2077  ation behavior w
+000048b0: 6865 6e20 656d 6974 7469 6e67 2065 7665  hen emitting eve
+000048c0: 6e74 7320 6d61 7920 7661 7279 2064 6570  nts may vary dep
+000048d0: 656e 6469 6e67 206f 6e20 7468 6520 636f  ending on the co
+000048e0: 6e63 7265 7465 203c 636f 6465 3e45 7665  ncrete <code>Eve
+000048f0: 6e74 456d 6974 7465 723c 2f63 6f64 653e  ntEmitter</code>
+00004900: 0a09 7573 6564 2e20 466f 7220 6578 616d  ..used. For exam
+00004910: 706c 652c 2074 6865 203c 636f 6465 3e41  ple, the <code>A
+00004920: 7379 6e63 494f 4576 656e 7445 6d69 7474  syncIOEventEmitt
+00004930: 6572 3c2f 636f 6465 3e20 696d 706c 656d  er</code> implem
+00004940: 656e 7461 7469 6f6e 206c 6576 6572 6167  entation leverag
+00004950: 6573 2074 6865 203c 636f 6465 3e41 7379  es the <code>Asy
+00004960: 6e63 494f 3c2f 636f 6465 3e20 6576 656e  ncIO</code> even
+00004970: 740a 096c 6f6f 7020 746f 2073 6368 6564  t..loop to sched
+00004980: 756c 6520 6361 6c6c 6261 636b 7320 6164  ule callbacks ad
+00004990: 6465 6420 6672 6f6d 2061 7379 6e63 6872  ded from asynchr
+000049a0: 6f6e 6f75 7320 636f 6e74 6578 7473 2077  onous contexts w
+000049b0: 6974 686f 7574 2062 6c6f 636b 696e 672e  ithout blocking.
+000049c0: 2042 7574 2061 6c74 6572 6e61 7469 7665   But alternative
+000049d0: 2065 6d69 7474 6572 7320 636f 756c 6420   emitters could 
+000049e0: 0a09 7374 7275 6374 7572 6520 7072 6f70  ..structure prop
+000049f0: 6167 6174 696f 6e20 6469 6666 6572 656e  agation differen
+00004a00: 746c 7920 746f 2073 7569 7420 7468 6569  tly to suit thei
+00004a10: 7220 6e65 6564 732e 0a3c 2f70 3e0a 0a3c  r needs..</p>..<
+00004a20: 2f64 6574 6169 6c73 3e0a 0a5b 2f2f 5d3a  /details>..[//]:
+00004a30: 2023 2028 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   # (------------
+00004a40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004a50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004a60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004a70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004a80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004a90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004aa0: 2d2d 290a 0a23 2320 5275 6e74 696d 6520  --)..## Runtime 
+00004ab0: 466c 6578 6962 696c 6974 7920 616e 6420  Flexibility and 
+00004ac0: 4375 7374 6f6d 697a 6174 696f 6e0a 0a3c  Customization..<
+00004ad0: 7020 7374 796c 653d 2774 6578 742d 616c  p style='text-al
+00004ae0: 6967 6e3a 206a 7573 7469 6679 3b27 3e0a  ign: justify;'>.
+00004af0: 2020 2020 2665 6d73 703b 2665 6d73 703b      &emsp;&emsp;
+00004b00: 4174 2069 7473 2063 6f72 652c 2050 7976  At its core, Pyv
+00004b10: 656e 7475 7320 7574 696c 697a 6573 2061  entus utilizes a
+00004b20: 206d 6f64 756c 6172 2065 7665 6e74 2065   modular event e
+00004b30: 6d69 7474 6572 2064 6573 6967 6e20 7468  mitter design th
+00004b40: 6174 2061 6c6c 6f77 7320 796f 7520 746f  at allows you to
+00004b50: 2073 7769 7463 6820 7365 616d 6c65 7373   switch seamless
+00004b60: 6c79 0a09 6265 7477 6565 6e20 6469 6666  ly..between diff
+00004b70: 6572 656e 7420 3c61 2068 7265 663d 2268  erent <a href="h
+00004b80: 7474 7073 3a2f 2f6d 6461 7065 6e61 2e67  ttps://mdapena.g
+00004b90: 6974 6875 622e 696f 2f70 7976 656e 7475  ithub.io/pyventu
+00004ba0: 732f 6765 7474 696e 672d 7374 6172 7465  s/getting-starte
+00004bb0: 642f 236f 7074 696f 6e61 6c2d 6465 7065  d/#optional-depe
+00004bc0: 6e64 656e 6369 6573 223e 3c69 3e62 7569  ndencies"><i>bui
+00004bd0: 6c74 2d69 6e3c 2f69 3e3c 2f61 3e0a 096f  lt-in</i></a>..o
+00004be0: 7220 6375 7374 6f6d 2065 7665 6e74 2065  r custom event e
+00004bf0: 6d69 7474 6572 2069 6d70 6c65 6d65 6e74  mitter implement
+00004c00: 6174 696f 6e73 206f 6e20 7468 6520 666c  ations on the fl
+00004c10: 792e 2057 6865 7468 6572 2079 6f75 206f  y. Whether you o
+00004c20: 7074 2066 6f72 206f 6666 6963 6961 6c20  pt for official 
+00004c30: 656d 6974 7465 7273 206f 7220 6465 6369  emitters or deci
+00004c40: 6465 2074 6f20 6372 6561 7465 2079 6f75  de to create you
+00004c50: 7220 0a09 6375 7374 6f6d 206f 6e65 732c  r ..custom ones,
+00004c60: 2050 7976 656e 7475 7320 616c 6c6f 7773   Pyventus allows
+00004c70: 2079 6f75 2074 6f20 7461 696c 6f72 2074   you to tailor t
+00004c80: 6865 2062 6568 6176 696f 7220 616e 6420  he behavior and 
+00004c90: 6361 7061 6269 6c69 7469 6573 206f 6620  capabilities of 
+00004ca0: 7468 6520 6576 656e 7420 656d 6974 7465  the event emitte
+00004cb0: 7273 2074 6f20 7065 7266 6563 746c 7920  rs to perfectly 
+00004cc0: 616c 6967 6e20 0a09 7769 7468 2079 6f75  align ..with you
+00004cd0: 7220 756e 6971 7565 2072 6571 7569 7265  r unique require
+00004ce0: 6d65 6e74 732e 0a3c 2f70 3e0a 0a23 2323  ments..</p>..###
+00004cf0: 2053 7761 7070 696e 6720 4576 656e 7420   Swapping Event 
+00004d00: 456d 6974 7465 7220 496d 706c 656d 656e  Emitter Implemen
+00004d10: 7461 7469 6f6e 7320 6174 2052 756e 7469  tations at Runti
+00004d20: 6d65 0a0a 3c70 2073 7479 6c65 3d27 7465  me..<p style='te
+00004d30: 7874 2d61 6c69 676e 3a20 6a75 7374 6966  xt-align: justif
+00004d40: 793b 273e 0a20 2020 2026 656d 7370 3b26  y;'>.    &emsp;&
+00004d50: 656d 7370 3b42 7920 6c65 7665 7261 6769  emsp;By leveragi
+00004d60: 6e67 2074 6865 2070 7269 6e63 6970 6c65  ng the principle
+00004d70: 206f 6620 6465 7065 6e64 656e 6379 2069   of dependency i
+00004d80: 6e76 6572 7369 6f6e 2061 6e64 2075 7369  nversion and usi
+00004d90: 6e67 2074 6865 2062 6173 6520 3c63 6f64  ng the base <cod
+00004da0: 653e 4576 656e 7445 6d69 7474 6572 3c2f  e>EventEmitter</
+00004db0: 636f 6465 3e20 6173 2061 0a09 6465 7065  code> as a..depe
+00004dc0: 6e64 656e 6379 2c20 796f 7520 6361 6e20  ndency, you can 
+00004dd0: 6368 616e 6765 2074 6865 2063 6f6e 6372  change the concr
+00004de0: 6574 6520 696d 706c 656d 656e 7461 7469  ete implementati
+00004df0: 6f6e 206f 6e20 7468 6520 666c 792e 204c  on on the fly. L
+00004e00: 6574 2773 2064 656d 6f6e 7374 7261 7465  et's demonstrate
+00004e10: 2074 6869 7320 7573 696e 6720 7468 6520   this using the 
+00004e20: 4173 796e 6349 4f20 0a09 4576 656e 7420  AsyncIO ..Event 
+00004e30: 456d 6974 7465 7220 616e 6420 7468 6520  Emitter and the 
+00004e40: 4578 6563 7574 6f72 2045 7665 6e74 2045  Executor Event E
+00004e50: 6d69 7474 6572 3a20 0a3c 2f70 3e0a 0a60  mitter: .</p>..`
+00004e60: 6060 5079 7468 6f6e 2074 6974 6c65 3d22  ``Python title="
+00004e70: 4576 656e 7420 456d 6974 7465 7220 5275  Event Emitter Ru
+00004e80: 6e74 696d 6520 466c 6578 6962 696c 6974  ntime Flexibilit
+00004e90: 7920 4578 616d 706c 6522 206c 696e 656e  y Example" linen
+00004ea0: 756d 733d 2231 2220 686c 5f6c 696e 6573  ums="1" hl_lines
+00004eb0: 3d22 3130 2d31 3120 3134 2031 3622 0a66  ="10-11 14 16".f
+00004ec0: 726f 6d20 7079 7665 6e74 7573 2069 6d70  rom pyventus imp
+00004ed0: 6f72 7420 4576 656e 744c 696e 6b65 722c  ort EventLinker,
+00004ee0: 2045 7665 6e74 456d 6974 7465 722c 2041   EventEmitter, A
+00004ef0: 7379 6e63 494f 4576 656e 7445 6d69 7474  syncIOEventEmitt
+00004f00: 6572 2c20 4578 6563 7574 6f72 4576 656e  er, ExecutorEven
+00004f10: 7445 6d69 7474 6572 0a0a 0a40 4576 656e  tEmitter...@Even
+00004f20: 744c 696e 6b65 722e 6f6e 2822 4772 6565  tLinker.on("Gree
+00004f30: 7445 7665 6e74 2229 0a64 6566 2068 616e  tEvent").def han
+00004f40: 646c 655f 6772 6565 745f 6576 656e 7428  dle_greet_event(
+00004f50: 6e61 6d65 3a20 7374 7220 3d20 2257 6f72  name: str = "Wor
+00004f60: 6c64 2229 3a0a 2020 2020 7072 696e 7428  ld"):.    print(
+00004f70: 6622 4865 6c6c 6f2c 207b 6e61 6d65 7d21  f"Hello, {name}!
+00004f80: 2229 0a0a 0a69 6620 5f5f 6e61 6d65 5f5f  ")...if __name__
+00004f90: 203d 3d20 225f 5f6d 6169 6e5f 5f22 3a0a   == "__main__":.
+00004fa0: 2020 2020 6465 6620 6d61 696e 2865 7665      def main(eve
+00004fb0: 6e74 5f65 6d69 7474 6572 3a20 4576 656e  nt_emitter: Even
+00004fc0: 7445 6d69 7474 6572 2920 2d3e 204e 6f6e  tEmitter) -> Non
+00004fd0: 653a 0a20 2020 2020 2020 2065 7665 6e74  e:.        event
+00004fe0: 5f65 6d69 7474 6572 2e65 6d69 7428 2247  _emitter.emit("G
+00004ff0: 7265 6574 4576 656e 7422 2c20 6e61 6d65  reetEvent", name
+00005000: 3d74 7970 6528 6576 656e 745f 656d 6974  =type(event_emit
+00005010: 7465 7229 2e5f 5f6e 616d 655f 5f29 0a0a  ter).__name__)..
+00005020: 0a20 2020 206d 6169 6e28 6576 656e 745f  .    main(event_
+00005030: 656d 6974 7465 723d 4173 796e 6349 4f45  emitter=AsyncIOE
+00005040: 7665 6e74 456d 6974 7465 7228 2929 0a20  ventEmitter()). 
+00005050: 2020 2077 6974 6820 4578 6563 7574 6f72     with Executor
+00005060: 4576 656e 7445 6d69 7474 6572 2829 2061  EventEmitter() a
+00005070: 7320 6578 6563 7574 6f72 5f65 7665 6e74  s executor_event
+00005080: 5f65 6d69 7474 6572 3a0a 2020 2020 2020  _emitter:.      
+00005090: 2020 6d61 696e 2865 7665 6e74 5f65 6d69    main(event_emi
+000050a0: 7474 6572 3d65 7865 6375 746f 725f 6576  tter=executor_ev
+000050b0: 656e 745f 656d 6974 7465 7229 0a60 6060  ent_emitter).```
+000050c0: 0a0a 2323 2320 4465 6669 6e69 6e67 2043  ..### Defining C
+000050d0: 7573 746f 6d20 4576 656e 7420 456d 6974  ustom Event Emit
+000050e0: 7465 7273 0a0a 3c70 2073 7479 6c65 3d27  ters..<p style='
+000050f0: 7465 7874 2d61 6c69 676e 3a20 6a75 7374  text-align: just
+00005100: 6966 793b 273e 0a20 2020 2026 656d 7370  ify;'>.    &emsp
+00005110: 3b26 656d 7370 3b54 6f20 696c 6c75 7374  ;&emsp;To illust
+00005120: 7261 7465 2050 7976 656e 7475 7327 2063  rate Pyventus' c
+00005130: 7573 746f 6d69 7a61 7469 6f6e 2063 6170  ustomization cap
+00005140: 6162 696c 6974 6965 732c 2077 6520 7769  abilities, we wi
+00005150: 6c6c 2064 6566 696e 6520 616e 6420 696d  ll define and im
+00005160: 706c 656d 656e 7420 6120 6375 7374 6f6d  plement a custom
+00005170: 2065 7665 6e74 2065 6d69 7474 6572 0a09   event emitter..
+00005180: 636c 6173 7320 666f 7220 7468 6520 4661  class for the Fa
+00005190: 7374 4150 4920 6672 616d 6577 6f72 6b2e  stAPI framework.
+000051a0: 2054 6869 7320 636c 6173 7320 7769 6c6c   This class will
+000051b0: 2065 6666 6963 6965 6e74 6c79 2068 616e   efficiently han
+000051c0: 646c 6520 7468 6520 6578 6563 7574 696f  dle the executio
+000051d0: 6e20 6f66 2065 7665 6e74 2065 6d69 7373  n of event emiss
+000051e0: 696f 6e73 2074 6872 6f75 6768 2069 7473  ions through its
+000051f0: 200a 093c 6120 6872 6566 3d22 6874 7470   ..<a href="http
+00005200: 733a 2f2f 6661 7374 6170 692e 7469 616e  s://fastapi.tian
+00005210: 676f 6c6f 2e63 6f6d 2f72 6566 6572 656e  golo.com/referen
+00005220: 6365 2f62 6163 6b67 726f 756e 642f 2220  ce/background/" 
+00005230: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
+00005240: 6261 636b 6772 6f75 6e64 2074 6173 6b73  background tasks
+00005250: 3c2f 613e 2077 6f72 6b66 6c6f 772e 0a3c  </a> workflow..<
+00005260: 2f70 3e0a 0a60 6060 5079 7468 6f6e 2074  /p>..```Python t
+00005270: 6974 6c65 3d22 4375 7374 6f6d 2045 7665  itle="Custom Eve
+00005280: 6e74 2045 6d69 7474 6572 2045 7861 6d70  nt Emitter Examp
+00005290: 6c65 2220 6c69 6e65 6e75 6d73 3d22 3122  le" linenums="1"
+000052a0: 2068 6c5f 6c69 6e65 733d 2236 2031 302d   hl_lines="6 10-
+000052b0: 3131 2031 332d 3134 220a 6672 6f6d 2066  11 13-14".from f
+000052c0: 6173 7461 7069 2069 6d70 6f72 7420 4261  astapi import Ba
+000052d0: 636b 6772 6f75 6e64 5461 736b 730a 0a66  ckgroundTasks..f
+000052e0: 726f 6d20 7079 7665 6e74 7573 2069 6d70  rom pyventus imp
+000052f0: 6f72 7420 4576 656e 7445 6d69 7474 6572  ort EventEmitter
+00005300: 2c20 4576 656e 744c 696e 6b65 720a 0a0a  , EventLinker...
+00005310: 636c 6173 7320 4661 7374 4150 4945 7665  class FastAPIEve
+00005320: 6e74 456d 6974 7465 7228 4576 656e 7445  ntEmitter(EventE
+00005330: 6d69 7474 6572 293a 0a20 2020 2022 2222  mitter):.    """
+00005340: 4120 6375 7374 6f6d 2065 7665 6e74 2065  A custom event e
+00005350: 6d69 7474 6572 2074 6861 7420 7573 6573  mitter that uses
+00005360: 2074 6865 2046 6173 7441 5049 2062 6163   the FastAPI bac
+00005370: 6b67 726f 756e 6420 7461 736b 732e 2222  kground tasks.""
+00005380: 220a 0a20 2020 2064 6566 205f 5f69 6e69  "..    def __ini
+00005390: 745f 5f28 7365 6c66 2c20 6261 636b 6772  t__(self, backgr
+000053a0: 6f75 6e64 5f74 6173 6b73 3a20 4261 636b  ound_tasks: Back
+000053b0: 6772 6f75 6e64 5461 736b 7329 3a0a 2020  groundTasks):.  
+000053c0: 2020 2020 2020 7375 7065 7228 292e 5f5f        super().__
+000053d0: 696e 6974 5f5f 2865 7665 6e74 5f6c 696e  init__(event_lin
+000053e0: 6b65 723d 4576 656e 744c 696e 6b65 722c  ker=EventLinker,
+000053f0: 2064 6562 7567 3d46 616c 7365 290a 2020   debug=False).  
+00005400: 2020 2020 2020 7365 6c66 2e5f 6261 636b        self._back
+00005410: 6772 6f75 6e64 5f74 6173 6b73 203d 2062  ground_tasks = b
+00005420: 6163 6b67 726f 756e 645f 7461 736b 730a  ackground_tasks.
+00005430: 0a20 2020 2064 6566 205f 7072 6f63 6573  .    def _proces
+00005440: 7328 7365 6c66 2c20 6576 656e 745f 656d  s(self, event_em
+00005450: 6973 7369 6f6e 3a20 4576 656e 7445 6d69  ission: EventEmi
+00005460: 7474 6572 2e45 7665 6e74 456d 6973 7369  tter.EventEmissi
+00005470: 6f6e 2920 2d3e 204e 6f6e 653a 0a20 2020  on) -> None:.   
+00005480: 2020 2020 2073 656c 662e 5f62 6163 6b67       self._backg
+00005490: 726f 756e 645f 7461 736b 732e 6164 645f  round_tasks.add_
+000054a0: 7461 736b 2865 7665 6e74 5f65 6d69 7373  task(event_emiss
+000054b0: 696f 6e29 2020 2320 5072 6f63 6573 7320  ion)  # Process 
+000054c0: 7468 6520 6576 656e 7420 656d 6973 7369  the event emissi
+000054d0: 6f6e 2061 7320 6120 6261 636b 6772 6f75  on as a backgrou
+000054e0: 6e64 2074 6173 6b0a 6060 600a 0a3c 6465  nd task.```..<de
+000054f0: 7461 696c 7320 6d61 726b 646f 776e 3d22  tails markdown="
+00005500: 3122 2063 6c61 7373 3d22 7469 7022 3e0a  1" class="tip">.
+00005510: 3c73 756d 6d61 7279 3e4f 6666 6963 6961  <summary>Officia
+00005520: 6c20 3c63 6f64 653e 4661 7374 4150 4945  l <code>FastAPIE
+00005530: 7665 6e74 456d 6974 7465 723c 2f63 6f64  ventEmitter</cod
+00005540: 653e 2049 6e74 6567 7261 7469 6f6e 2e3c  e> Integration.<
+00005550: 2f73 756d 6d61 7279 3e0a 0a3c 7020 7374  /summary>..<p st
+00005560: 796c 653d 2774 6578 742d 616c 6967 6e3a  yle='text-align:
+00005570: 206a 7573 7469 6679 3b27 3e0a 2020 2020   justify;'>.    
+00005580: 496e 2063 6173 6520 796f 7527 7265 2069  In case you're i
+00005590: 6e74 6572 6573 7465 6420 696e 2069 6e74  nterested in int
+000055a0: 6567 7261 7469 6e67 2050 7976 656e 7475  egrating Pyventu
+000055b0: 7320 7769 7468 2046 6173 7441 5049 2c20  s with FastAPI, 
+000055c0: 796f 7520 6361 6e20 7265 6665 7220 746f  you can refer to
+000055d0: 2074 6865 206f 6666 6963 6961 6c20 5079   the official Py
+000055e0: 7665 6e74 7573 200a 093c 6120 6872 6566  ventus ..<a href
+000055f0: 3d22 6874 7470 733a 2f2f 6d64 6170 656e  ="https://mdapen
+00005600: 612e 6769 7468 7562 2e69 6f2f 7079 7665  a.github.io/pyve
+00005610: 6e74 7573 2f74 7574 6f72 6961 6c73 2f65  ntus/tutorials/e
+00005620: 6d69 7474 6572 732f 6661 7374 6170 692f  mitters/fastapi/
+00005630: 223e 3c69 3e46 6173 7441 5049 2045 7665  "><i>FastAPI Eve
+00005640: 6e74 2045 6d69 7474 6572 3c2f 693e 3c2f  nt Emitter</i></
+00005650: 613e 200a 0969 6d70 6c65 6d65 6e74 6174  a> ..implementat
+00005660: 696f 6e2e 0a3c 2f70 3e0a 0a3c 2f64 6574  ion..</p>..</det
+00005670: 6169 6c73 3e0a 0a5b 2f2f 5d3a 2023 2028  ails>..[//]: # (
+00005680: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005690: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000056a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000056b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000056c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000056d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000056e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 290a  --------------).
+000056f0: 0a23 2320 4576 656e 7420 4f62 6a65 6374  .## Event Object
+00005700: 7320 616e 6420 476c 6f62 616c 2045 7665  s and Global Eve
+00005710: 6e74 730a 0a3c 7020 7374 796c 653d 2774  nts..<p style='t
+00005720: 6578 742d 616c 6967 6e3a 206a 7573 7469  ext-align: justi
+00005730: 6679 3b27 3e0a 2020 2020 2665 6d73 703b  fy;'>.    &emsp;
+00005740: 2665 6d73 703b 496e 2061 6464 6974 696f  &emsp;In additio
+00005750: 6e20 746f 2073 7472 696e 6720 6576 656e  n to string even
+00005760: 7473 2c20 5079 7665 6e74 7573 2061 6c73  ts, Pyventus als
+00005770: 6f20 7375 7070 6f72 7473 2045 7665 6e74  o supports Event
+00005780: 204f 626a 6563 7473 2c20 7768 6963 6820   Objects, which 
+00005790: 7072 6f76 6964 6520 6120 7374 7275 6374  provide a struct
+000057a0: 7572 6564 2077 6179 2074 6f20 0a09 6465  ured way to ..de
+000057b0: 6669 6e65 2065 7665 6e74 7320 616e 6420  fine events and 
+000057c0: 656e 6361 7073 756c 6174 6520 7265 6c65  encapsulate rele
+000057d0: 7661 6e74 2064 6174 6120 7061 796c 6f61  vant data payloa
+000057e0: 6473 2e0a 3c2f 703e 0a0a 6060 6050 7974  ds..</p>..```Pyt
+000057f0: 686f 6e20 7469 746c 653d 2245 7665 6e74  hon title="Event
+00005800: 204f 626a 6563 7420 4578 616d 706c 6522   Object Example"
+00005810: 206c 696e 656e 756d 733d 2231 2220 686c   linenums="1" hl
+00005820: 5f6c 696e 6573 3d22 312d 3220 372d 3820  _lines="1-2 7-8 
+00005830: 3136 2d31 3922 0a40 6461 7461 636c 6173  16-19".@dataclas
+00005840: 7320 2023 2044 6566 696e 6520 6120 5079  s  # Define a Py
+00005850: 7468 6f6e 2064 6174 6163 6c61 7373 2072  thon dataclass r
+00005860: 6570 7265 7365 6e74 696e 6720 7468 6520  epresenting the 
+00005870: 6576 656e 7420 616e 6420 6974 7320 7061  event and its pa
+00005880: 796c 6f61 642e 0a63 6c61 7373 204f 7264  yload..class Ord
+00005890: 6572 4372 6561 7465 6445 7665 6e74 3a0a  erCreatedEvent:.
+000058a0: 2020 2020 6f72 6465 725f 6964 3a20 696e      order_id: in
+000058b0: 740a 2020 2020 7061 796c 6f61 643a 2064  t.    payload: d
+000058c0: 6963 745b 7374 722c 2061 6e79 5d0a 0a0a  ict[str, any]...
+000058d0: 4045 7665 6e74 4c69 6e6b 6572 2e6f 6e28  @EventLinker.on(
+000058e0: 4f72 6465 7243 7265 6174 6564 4576 656e  OrderCreatedEven
+000058f0: 7429 2020 2320 5375 6273 6372 6962 6520  t)  # Subscribe 
+00005900: 6576 656e 7420 6861 6e64 6c65 7273 2074  event handlers t
+00005910: 6f20 7468 6520 6576 656e 742e 0a64 6566  o the event..def
+00005920: 2068 616e 646c 655f 6f72 6465 725f 6372   handle_order_cr
+00005930: 6561 7465 645f 6576 656e 7428 6576 656e  eated_event(even
+00005940: 743a 204f 7264 6572 4372 6561 7465 6445  t: OrderCreatedE
+00005950: 7665 6e74 293a 0a20 2020 2023 2050 7976  vent):.    # Pyv
+00005960: 656e 7475 7320 7769 6c6c 2061 7574 6f6d  entus will autom
+00005970: 6174 6963 616c 6c79 2070 6173 7320 7468  atically pass th
+00005980: 6520 4576 656e 7420 4f62 6a65 6374 200a  e Event Object .
+00005990: 2020 2020 2320 6173 2074 6865 2066 6972      # as the fir
+000059a0: 7374 2070 6f73 6974 696f 6e61 6c20 6172  st positional ar
+000059b0: 6775 6d65 6e74 2e0a 2020 2020 7072 696e  gument..    prin
+000059c0: 7428 6622 4576 656e 7420 4f62 6a65 6374  t(f"Event Object
+000059d0: 3a20 7b65 7665 6e74 7d22 290a 0a0a 6576  : {event}")...ev
+000059e0: 656e 745f 656d 6974 7465 723a 2045 7665  ent_emitter: Eve
+000059f0: 6e74 456d 6974 7465 7220 3d20 4173 796e  ntEmitter = Asyn
+00005a00: 6349 4f45 7665 6e74 456d 6974 7465 7228  cIOEventEmitter(
+00005a10: 290a 6576 656e 745f 656d 6974 7465 722e  ).event_emitter.
+00005a20: 656d 6974 280a 2020 2020 6576 656e 743d  emit(.    event=
+00005a30: 4f72 6465 7243 7265 6174 6564 4576 656e  OrderCreatedEven
+00005a40: 7428 2020 2320 456d 6974 2061 6e20 696e  t(  # Emit an in
+00005a50: 7374 616e 6365 206f 6620 7468 6520 6576  stance of the ev
+00005a60: 656e 7421 0a20 2020 2020 2020 206f 7264  ent!.        ord
+00005a70: 6572 5f69 643d 3634 3532 3837 392c 0a20  er_id=6452879,. 
+00005a80: 2020 2020 2020 2070 6179 6c6f 6164 3d7b         payload={
+00005a90: 7d2c 0a20 2020 2029 2c0a 290a 6060 600a  },.    ),.).```.
+00005aa0: 0a3c 7020 7374 796c 653d 2774 6578 742d  .<p style='text-
+00005ab0: 616c 6967 6e3a 206a 7573 7469 6679 3b27  align: justify;'
+00005ac0: 3e0a 2020 2020 2665 6d73 703b 2665 6d73  >.    &emsp;&ems
+00005ad0: 703b 4675 7274 6865 726d 6f72 652c 2050  p;Furthermore, P
+00005ae0: 7976 656e 7475 7320 7072 6f76 6964 6573  yventus provides
+00005af0: 2073 7570 706f 7274 2066 6f72 2047 6c6f   support for Glo
+00005b00: 6261 6c20 4576 656e 7473 2c20 7768 6963  bal Events, whic
+00005b10: 6820 6172 6520 7061 7274 6963 756c 6172  h are particular
+00005b20: 6c79 2075 7365 6675 6c20 666f 7220 0a09  ly useful for ..
+00005b30: 696d 706c 656d 656e 7469 6e67 2063 726f  implementing cro
+00005b40: 7373 2d63 7574 7469 6e67 2063 6f6e 6365  ss-cutting conce
+00005b50: 726e 7320 7375 6368 2061 7320 6c6f 6767  rns such as logg
+00005b60: 696e 672c 206d 6f6e 6974 6f72 696e 672c  ing, monitoring,
+00005b70: 206f 7220 616e 616c 7974 6963 732e 2042   or analytics. B
+00005b80: 7920 7375 6273 6372 6962 696e 6720 6576  y subscribing ev
+00005b90: 656e 7420 6861 6e64 6c65 7273 2074 6f0a  ent handlers to.
+00005ba0: 093c 636f 6465 3e2e 2e2e 3c2f 636f 6465  .<code>...</code
+00005bb0: 3e20 6f72 203c 636f 6465 3e45 6c6c 6970  > or <code>Ellip
+00005bc0: 7369 733c 2f63 6f64 653e 2c20 796f 7520  sis</code>, you 
+00005bd0: 6361 6e20 6361 7074 7572 6520 616c 6c20  can capture all 
+00005be0: 6576 656e 7473 2074 6861 7420 6d61 7920  events that may 
+00005bf0: 6f63 6375 7220 7769 7468 696e 2074 6861  occur within tha
+00005c00: 7420 0a09 3c63 6f64 653e 4576 656e 744c  t ..<code>EventL
+00005c10: 696e 6b65 723c 2f63 6f64 653e 2063 6f6e  inker</code> con
+00005c20: 7465 7874 2e0a 3c2f 703e 0a0a 6060 6050  text..</p>..```P
+00005c30: 7974 686f 6e20 7469 746c 653d 2247 6c6f  ython title="Glo
+00005c40: 6261 6c20 4576 656e 7420 4578 616d 706c  bal Event Exampl
+00005c50: 6522 206c 696e 656e 756d 733d 2231 2220  e" linenums="1" 
+00005c60: 686c 5f6c 696e 6573 3d22 3122 0a40 4576  hl_lines="1".@Ev
+00005c70: 656e 744c 696e 6b65 722e 6f6e 282e 2e2e  entLinker.on(...
+00005c80: 290a 6465 6620 6861 6e64 6c65 5f61 6e79  ).def handle_any
+00005c90: 5f65 7665 6e74 282a 6172 6773 2c20 2a2a  _event(*args, **
+00005ca0: 6b77 6172 6773 293a 0a20 2020 2070 7269  kwargs):.    pri
+00005cb0: 6e74 2866 2250 6572 666f 726d 206c 6f67  nt(f"Perform log
+00005cc0: 6769 6e67 2e2e 2e5c 6e41 7267 733a 207b  ging...\nArgs: {
+00005cd0: 6172 6773 7d5c 744b 7761 7267 733a 207b  args}\tKwargs: {
+00005ce0: 6b77 6172 6773 7d22 290a 0a0a 6576 656e  kwargs}")...even
+00005cf0: 745f 656d 6974 7465 723a 2045 7665 6e74  t_emitter: Event
+00005d00: 456d 6974 7465 7220 3d20 4173 796e 6349  Emitter = AsyncI
+00005d10: 4f45 7665 6e74 456d 6974 7465 7228 290a  OEventEmitter().
+00005d20: 6576 656e 745f 656d 6974 7465 722e 656d  event_emitter.em
+00005d30: 6974 2822 4772 6565 7445 7665 6e74 222c  it("GreetEvent",
+00005d40: 206e 616d 653d 2250 7976 656e 7475 7322   name="Pyventus"
+00005d50: 290a 6060 600a 0a5b 2f2f 5d3a 2023 2028  ).```..[//]: # (
+00005d60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005d70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005d80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005d90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005da0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005db0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005dc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 290a  --------------).
+00005dd0: 0a23 2320 5375 6363 6573 7320 616e 6420  .## Success and 
+00005de0: 4572 726f 7220 4861 6e64 6c69 6e67 0a0a  Error Handling..
+00005df0: 3c70 2073 7479 6c65 3d27 7465 7874 2d61  <p style='text-a
+00005e00: 6c69 676e 3a20 6a75 7374 6966 793b 273e  lign: justify;'>
+00005e10: 0a20 2020 2026 656d 7370 3b26 656d 7370  .    &emsp;&emsp
+00005e20: 3b57 6974 6820 5079 7665 6e74 7573 2c20  ;With Pyventus, 
+00005e30: 796f 7520 6361 6e20 6375 7374 6f6d 697a  you can customiz
+00005e40: 6520 686f 7720 6576 656e 7473 2061 7265  e how events are
+00005e50: 2068 616e 646c 6564 2075 706f 6e20 636f   handled upon co
+00005e60: 6d70 6c65 7469 6f6e 2c20 7768 6574 6865  mpletion, whethe
+00005e70: 7220 7468 6579 2073 7563 6365 6564 206f  r they succeed o
+00005e80: 7220 0a09 656e 636f 756e 7465 7220 6572  r ..encounter er
+00005e90: 726f 7273 2e20 5468 6973 2063 7573 746f  rors. This custo
+00005ea0: 6d69 7a61 7469 6f6e 2069 7320 6163 6869  mization is achi
+00005eb0: 6576 6564 2062 7920 7573 696e 6720 6569  eved by using ei
+00005ec0: 7468 6572 2074 6865 2045 7665 6e74 4c69  ther the EventLi
+00005ed0: 6e6b 6572 2773 203c 636f 6465 3e6f 6e28  nker's <code>on(
+00005ee0: 293c 2f63 6f64 653e 206f 7220 0a09 3c63  )</code> or ..<c
+00005ef0: 6f64 653e 6f6e 6365 2829 3c2f 636f 6465  ode>once()</code
+00005f00: 3e20 6465 636f 7261 746f 7220 7769 7468  > decorator with
+00005f10: 696e 2061 203c 636f 6465 3e77 6974 683c  in a <code>with<
+00005f20: 2f63 6f64 653e 2073 7461 7465 6d65 6e74  /code> statement
+00005f30: 2062 6c6f 636b 2e20 496e 7369 6465 2074   block. Inside t
+00005f40: 6869 7320 626c 6f63 6b2c 2079 6f75 2063  his block, you c
+00005f50: 616e 200a 0964 6566 696e 6520 6e6f 7420  an ..define not 
+00005f60: 6f6e 6c79 2074 6865 2065 7665 6e74 2063  only the event c
+00005f70: 616c 6c62 6163 6b73 2062 7574 2061 6c73  allbacks but als
+00005f80: 6f20 7468 6520 6f76 6572 616c 6c20 776f  o the overall wo
+00005f90: 726b 666c 6f77 206f 6620 7468 6520 6576  rkflow of the ev
+00005fa0: 656e 742e 204e 6f77 2c20 6c65 74e2 8099  ent. Now, let...
+00005fb0: 7320 6578 706c 6f72 6520 0a09 7468 6973  s explore ..this
+00005fc0: 2073 696d 706c 6520 7965 7420 706f 7765   simple yet powe
+00005fd0: 7266 756c 2050 7974 686f 6e69 6320 7379  rful Pythonic sy
+00005fe0: 6e74 6178 206f 6620 5079 7665 6e74 7573  ntax of Pyventus
+00005ff0: 2074 6872 6f75 6768 2061 6e20 6578 616d   through an exam
+00006000: 706c 652e 0a3c 2f70 3e0a 0a60 6060 5079  ple..</p>..```Py
+00006010: 7468 6f6e 2074 6974 6c65 3d22 5375 6363  thon title="Succ
+00006020: 6573 7320 616e 6420 4572 726f 7220 4861  ess and Error Ha
+00006030: 6e64 6c69 6e67 2045 7861 6d70 6c65 2220  ndling Example" 
+00006040: 6c69 6e65 6e75 6d73 3d22 3122 2068 6c5f  linenums="1" hl_
+00006050: 6c69 6e65 733d 2234 2036 2d37 2031 302d  lines="4 6-7 10-
+00006060: 3131 2031 342d 3135 220a 6672 6f6d 2070  11 14-15".from p
+00006070: 7976 656e 7475 7320 696d 706f 7274 2045  yventus import E
+00006080: 7665 6e74 4c69 6e6b 6572 2c20 4576 656e  ventLinker, Even
+00006090: 7445 6d69 7474 6572 2c20 4173 796e 6349  tEmitter, AsyncI
+000060a0: 4f45 7665 6e74 456d 6974 7465 720a 0a23  OEventEmitter..#
+000060b0: 2043 7265 6174 6520 616e 2065 7665 6e74   Create an event
+000060c0: 206c 696e 6b65 7220 666f 7220 7468 6520   linker for the 
+000060d0: 2244 6976 6973 696f 6e45 7665 6e74 220a  "DivisionEvent".
+000060e0: 7769 7468 2045 7665 6e74 4c69 6e6b 6572  with EventLinker
+000060f0: 2e6f 6e28 2244 6976 6973 696f 6e45 7665  .on("DivisionEve
+00006100: 6e74 2229 2061 7320 6c69 6e6b 6572 3a0a  nt") as linker:.
+00006110: 2020 2020 406c 696e 6b65 722e 6f6e 5f65      @linker.on_e
+00006120: 7665 6e74 0a20 2020 2064 6566 2064 6976  vent.    def div
+00006130: 6964 6528 613a 2066 6c6f 6174 2c20 623a  ide(a: float, b:
+00006140: 2066 6c6f 6174 2920 2d3e 2066 6c6f 6174   float) -> float
+00006150: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00006160: 2061 202f 2062 0a0a 2020 2020 406c 696e   a / b..    @lin
+00006170: 6b65 722e 6f6e 5f73 7563 6365 7373 0a20  ker.on_success. 
+00006180: 2020 2064 6566 2068 616e 646c 655f 7375     def handle_su
+00006190: 6363 6573 7328 7265 7375 6c74 3a20 666c  ccess(result: fl
+000061a0: 6f61 7429 202d 3e20 4e6f 6e65 3a0a 2020  oat) -> None:.  
+000061b0: 2020 2020 2020 7072 696e 7428 6622 4469        print(f"Di
+000061c0: 7669 7369 6f6e 2072 6573 756c 743a 207b  vision result: {
+000061d0: 7265 7375 6c74 3a2e 3367 7d22 290a 0a20  result:.3g}").. 
+000061e0: 2020 2040 6c69 6e6b 6572 2e6f 6e5f 6661     @linker.on_fa
+000061f0: 696c 7572 650a 2020 2020 6465 6620 6861  ilure.    def ha
+00006200: 6e64 6c65 5f66 6169 6c75 7265 2865 3a20  ndle_failure(e: 
+00006210: 4578 6365 7074 696f 6e29 202d 3e20 4e6f  Exception) -> No
+00006220: 6e65 3a0a 2020 2020 2020 2020 7072 696e  ne:.        prin
+00006230: 7428 6622 4f6f 7073 2c20 736f 6d65 7468  t(f"Oops, someth
+00006240: 696e 6720 7765 6e74 2077 726f 6e67 3a20  ing went wrong: 
+00006250: 7b65 7d22 290a 0a65 7665 6e74 5f65 6d69  {e}")..event_emi
+00006260: 7474 6572 3a20 4576 656e 7445 6d69 7474  tter: EventEmitt
+00006270: 6572 203d 2041 7379 6e63 494f 4576 656e  er = AsyncIOEven
+00006280: 7445 6d69 7474 6572 2829 2020 2320 4372  tEmitter()  # Cr
+00006290: 6561 7465 2061 6e20 6576 656e 7420 656d  eate an event em
+000062a0: 6974 7465 720a 6576 656e 745f 656d 6974  itter.event_emit
+000062b0: 7465 722e 656d 6974 2822 4469 7669 7369  ter.emit("Divisi
+000062c0: 6f6e 4576 656e 7422 2c20 613d 312c 2062  onEvent", a=1, b
+000062d0: 3d30 2920 2023 2045 7861 6d70 6c65 3a20  =0)  # Example: 
+000062e0: 4469 7669 7369 6f6e 2062 7920 7a65 726f  Division by zero
+000062f0: 0a65 7665 6e74 5f65 6d69 7474 6572 2e65  .event_emitter.e
+00006300: 6d69 7428 2244 6976 6973 696f 6e45 7665  mit("DivisionEve
+00006310: 6e74 222c 2061 3d31 2c20 623d 3229 2020  nt", a=1, b=2)  
+00006320: 2320 4578 616d 706c 653a 2056 616c 6964  # Example: Valid
+00006330: 2064 6976 6973 696f 6e0a 6060 600a 0a3c   division.```..<
+00006340: 7020 7374 796c 653d 2774 6578 742d 616c  p style='text-al
+00006350: 6967 6e3a 206a 7573 7469 6679 3b27 3e0a  ign: justify;'>.
+00006360: 2020 2020 2665 6d73 703b 2665 6d73 703b      &emsp;&emsp;
+00006370: 4173 2077 6520 6861 7665 2073 6565 6e20  As we have seen 
+00006380: 6672 6f6d 2074 6865 2065 7861 6d70 6c65  from the example
+00006390: 2c20 5079 7665 6e74 7573 206f 6666 6572  , Pyventus offer
+000063a0: 7320 6120 7265 6c69 6162 6c65 2061 6e64  s a reliable and
+000063b0: 2050 7974 686f 6e69 6320 736f 6c75 7469   Pythonic soluti
+000063c0: 6f6e 2066 6f72 2063 7573 746f 6d69 7a69  on for customizi
+000063d0: 6e67 200a 0965 7665 6e74 2068 616e 646c  ng ..event handl
+000063e0: 696e 672e 2042 7920 7574 696c 697a 696e  ing. By utilizin
+000063f0: 6720 7468 6520 4576 656e 744c 696e 6b65  g the EventLinke
+00006400: 7220 616e 6420 6974 7320 6465 636f 7261  r and its decora
+00006410: 746f 7273 2077 6974 6869 6e20 6120 3c63  tors within a <c
+00006420: 6f64 653e 7769 7468 3c2f 636f 6465 3e20  ode>with</code> 
+00006430: 7374 6174 656d 656e 7420 626c 6f63 6b2c  statement block,
+00006440: 2077 650a 0977 6572 6520 6162 6c65 2074   we..were able t
+00006450: 6f20 6465 6669 6e65 2074 6865 203c 636f  o define the <co
+00006460: 6465 3e44 6976 6973 696f 6e45 7665 6e74  de>DivisionEvent
+00006470: 3c2f 636f 6465 3e20 616e 6420 7370 6563  </code> and spec
+00006480: 6966 7920 7468 6520 6361 6c6c 6261 636b  ify the callback
+00006490: 7320 666f 7220 6469 7669 7369 6f6e 2c20  s for division, 
+000064a0: 7375 6363 6573 732c 2061 6e64 2066 6169  success, and fai
+000064b0: 6c75 7265 0a09 6361 7365 732e 0a3c 2f70  lure..cases..</p
+000064c0: 3e0a 0a5b 2f2f 5d3a 2023 2028 2d2d 2d2d  >..[//]: # (----
+000064d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000064e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000064f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006500: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006510: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006520: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006530: 2d2d 2d2d 2d2d 2d2d 2d2d 290a 0a23 2320  ----------)..## 
+00006540: 436f 6e74 696e 756f 7573 2045 766f 6c75  Continuous Evolu
+00006550: 7469 6f6e 0a0a 3c70 2073 7479 6c65 3d27  tion..<p style='
+00006560: 7465 7874 2d61 6c69 676e 3a20 6a75 7374  text-align: just
+00006570: 6966 793b 273e 0a09 2665 6d73 703b 2665  ify;'>..&emsp;&e
+00006580: 6d73 703b 5079 7665 6e74 7573 2063 6f6e  msp;Pyventus con
+00006590: 7469 6e75 6f75 736c 7920 6164 6170 7473  tinuously adapts
+000065a0: 2074 6f20 7375 7070 6f72 7420 6465 7665   to support deve
+000065b0: 6c6f 7065 7273 2061 6372 6f73 7320 7465  lopers across te
+000065c0: 6368 6e6f 6c6f 6769 6361 6c20 616e 6420  chnological and 
+000065d0: 7072 6f67 7261 6d6d 696e 6720 646f 6d61  programming doma
+000065e0: 696e 732e 2049 7473 0a09 6169 6d20 6973  ins. Its..aim is
+000065f0: 2074 6f20 7265 6d61 696e 2061 7420 7468   to remain at th
+00006600: 6520 666f 7265 6672 6f6e 7420 6f66 2065  e forefront of e
+00006610: 7665 6e74 2d64 7269 7665 6e20 6465 7369  vent-driven desi
+00006620: 676e 2e20 4675 7475 7265 2064 6576 656c  gn. Future devel
+00006630: 6f70 6d65 6e74 206d 6179 2069 6e74 726f  opment may intro
+00006640: 6475 6365 206e 6577 206f 6666 6963 6961  duce new officia
+00006650: 6c20 6576 656e 7420 0a09 656d 6974 7465  l event ..emitte
+00006660: 7273 2c20 6578 7061 6e64 696e 6720 636f  rs, expanding co
+00006670: 6d70 6174 6962 696c 6974 7920 7769 7468  mpatibility with
+00006680: 2064 6966 6665 7265 6e74 2074 6563 686e   different techn
+00006690: 6f6c 6f67 6965 7320 7468 726f 7567 6820  ologies through 
+000066a0: 7365 616d 6c65 7373 2069 6e74 6567 7261  seamless integra
+000066b0: 7469 6f6e 2e0a 3c2f 703e 0a0a 3c70 2073  tion..</p>..<p s
+000066c0: 7479 6c65 3d27 7465 7874 2d61 6c69 676e  tyle='text-align
+000066d0: 3a20 6a75 7374 6966 793b 273e 0a09 2665  : justify;'>..&e
+000066e0: 6d73 703b 2665 6d73 703b 4375 7272 656e  msp;&emsp;Curren
+000066f0: 7420 6465 6661 756c 7420 656d 6974 7465  t default emitte
+00006700: 7273 2070 726f 7669 6465 2072 656c 6961  rs provide relia
+00006710: 626c 6520 6f75 742d 6f66 2d74 6865 2d62  ble out-of-the-b
+00006720: 6f78 2063 6170 6162 696c 6974 6965 7320  ox capabilities 
+00006730: 666f 7220 636f 6d6d 6f6e 2075 7365 2063  for common use c
+00006740: 6173 6573 2e20 5468 6579 0a09 6566 6669  ases. They..effi
+00006750: 6369 656e 746c 7920 6861 6e64 6c65 2063  ciently handle c
+00006760: 6f72 6520 6576 656e 7420 6f70 6572 6174  ore event operat
+00006770: 696f 6e73 2061 6e64 206c 6179 2074 6865  ions and lay the
+00006780: 2066 6f75 6e64 6174 696f 6e20 666f 7220   foundation for 
+00006790: 6275 696c 6469 6e67 2065 7665 6e74 2d64  building event-d
+000067a0: 7269 7665 6e20 6170 706c 6963 6174 696f  riven applicatio
+000067b0: 6e73 2e0a 3c2f 703e 0a0a 3c64 6574 6169  ns..</p>..<detai
+000067c0: 6c73 206d 6172 6b64 6f77 6e3d 2231 2220  ls markdown="1" 
+000067d0: 636c 6173 733d 2269 6e66 6f22 3e0a 3c73  class="info">.<s
+000067e0: 756d 6d61 7279 3e44 7269 7669 6e67 2049  ummary>Driving I
+000067f0: 6e6e 6f76 6174 696f 6e20 5468 726f 7567  nnovation Throug
+00006800: 6820 436f 6c6c 6162 6f72 6174 696f 6e3c  h Collaboration<
+00006810: 2f73 756d 6d61 7279 3e0a 0a3c 7020 7374  /summary>..<p st
+00006820: 796c 653d 2774 6578 742d 616c 6967 6e3a  yle='text-align:
+00006830: 206a 7573 7469 6679 3b27 3e0a 2020 2020   justify;'>.    
+00006840: 2665 6d73 703b 2665 6d73 703b 5079 7665  &emsp;&emsp;Pyve
+00006850: 6e74 7573 2069 7320 616e 206f 7065 6e20  ntus is an open 
+00006860: 736f 7572 6365 2070 726f 6a65 6374 2074  source project t
+00006870: 6861 7420 7765 6c63 6f6d 6573 2063 6f6d  hat welcomes com
+00006880: 6d75 6e69 7479 2069 6e76 6f6c 7665 6d65  munity involveme
+00006890: 6e74 2e20 4966 2079 6f75 2077 6973 6820  nt. If you wish 
+000068a0: 746f 2063 6f6e 7472 6962 7574 650a 0961  to contribute..a
+000068b0: 6464 6974 696f 6e61 6c20 6576 656e 7420  dditional event 
+000068c0: 656d 6974 7465 7273 2c20 696d 7072 6f76  emitters, improv
+000068d0: 656d 656e 7473 2c20 6f72 2062 7567 2066  ements, or bug f
+000068e0: 6978 6573 2c20 706c 6561 7365 2063 6865  ixes, please che
+000068f0: 636b 2074 6865 203c 6120 6872 6566 3d22  ck the <a href="
+00006900: 6874 7470 733a 2f2f 6d64 6170 656e 612e  https://mdapena.
+00006910: 6769 7468 7562 2e69 6f2f 7079 7665 6e74  github.io/pyvent
+00006920: 7573 2f63 6f6e 7472 6962 7574 696e 672f  us/contributing/
+00006930: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+00006940: 223e 436f 6e74 7269 6275 7469 6e67 3c2f  ">Contributing</
+00006950: 613e 200a 0973 6563 7469 6f6e 2066 6f72  a> ..section for
+00006960: 2067 7569 6465 6c69 6e65 7320 6f6e 2063   guidelines on c
+00006970: 6f6c 6c61 626f 7261 7469 6e67 2e20 546f  ollaborating. To
+00006980: 6765 7468 6572 2c20 7765 2063 616e 2066  gether, we can f
+00006990: 7572 7468 6572 2074 6865 2070 6f73 7369  urther the possi
+000069a0: 6269 6c69 7469 6573 206f 6620 6576 656e  bilities of even
+000069b0: 742d 6472 6976 656e 2064 6576 656c 6f70  t-driven develop
+000069c0: 6d65 6e74 2e0a 3c2f 703e 0a0a 3c2f 6465  ment..</p>..</de
+000069d0: 7461 696c 733e 0a0a 5b2f 2f5d 3a20 2320  tails>..[//]: # 
+000069e0: 282d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  (---------------
+000069f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006a00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006a10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006a20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006a30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006a40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d29  ---------------)
+00006a50: 0a0a 2323 204c 6963 656e 7365 0a0a 3c70  ..## License..<p
+00006a60: 2073 7479 6c65 3d27 7465 7874 2d61 6c69   style='text-ali
+00006a70: 676e 3a20 6a75 7374 6966 793b 2720 6d61  gn: justify;' ma
+00006a80: 726b 646f 776e 3e0a 2020 2020 2665 6d73  rkdown>.    &ems
+00006a90: 703b 2665 6d73 703b 5079 7665 6e74 7573  p;&emsp;Pyventus
+00006aa0: 2069 7320 6469 7374 7269 6275 7465 6420   is distributed 
+00006ab0: 6173 206f 7065 6e20 736f 7572 6365 2073  as open source s
+00006ac0: 6f66 7477 6172 6520 616e 6420 6973 2072  oftware and is r
+00006ad0: 656c 6561 7365 6420 756e 6465 7220 7468  eleased under th
+00006ae0: 6520 3c61 2068 7265 663d 2268 7474 7073  e <a href="https
+00006af0: 3a2f 2f63 686f 6f73 6561 6c69 6365 6e73  ://choosealicens
+00006b00: 652e 636f 6d2f 6c69 6365 6e73 6573 2f6d  e.com/licenses/m
+00006b10: 6974 2f22 2074 6172 6765 743d 225f 626c  it/" target="_bl
+00006b20: 616e 6b22 3e4d 4954 204c 6963 656e 7365  ank">MIT License
+00006b30: 3c2f 613e 2e20 0a20 2020 2059 6f75 2063  </a>. .    You c
+00006b40: 616e 2076 6965 7720 7468 6520 6675 6c6c  an view the full
+00006b50: 2074 6578 7420 6f66 2074 6865 206c 6963   text of the lic
+00006b60: 656e 7365 2069 6e20 7468 6520 3c61 2068  ense in the <a h
+00006b70: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+00006b80: 6875 622e 636f 6d2f 6d64 6170 656e 612f  hub.com/mdapena/
+00006b90: 7079 7665 6e74 7573 2f62 6c6f 622f 6d61  pyventus/blob/ma
+00006ba0: 7374 6572 2f4c 4943 454e 5345 2220 7461  ster/LICENSE" ta
+00006bb0: 7267 6574 3d22 5f62 6c61 6e6b 223e 3c63  rget="_blank"><c
+00006bc0: 6f64 653e 4c49 4345 4e53 453c 2f63 6f64  ode>LICENSE</cod
+00006bd0: 653e 3c2f 613e 200a 0966 696c 6520 6c6f  e></a> ..file lo
+00006be0: 6361 7465 6420 696e 2074 6865 2050 7976  cated in the Pyv
+00006bf0: 656e 7475 7320 7265 706f 7369 746f 7279  entus repository
+00006c00: 2e0a 3c2f 703e 0a                        ..</p>.
```

