# Comparing `tmp/flask_attachments-0.2.0.tar.gz` & `tmp/flask_attachments-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_attachments-0.2.0.tar", last modified: Tue Jan 23 05:15:02 2024, max compression
+gzip compressed data, last modified: Tue Apr  9 22:33:47 2024, max compression
```

## Comparing `flask_attachments-0.2.0.tar` & `flask_attachments-0.2.1.tar`

### file list

```diff
@@ -1,42 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 05:15:02.636304 flask_attachments-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-01-23 05:14:44.000000 flask_attachments-0.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-01-23 05:14:44.000000 flask_attachments-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-01-23 05:14:44.000000 flask_attachments-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-01-23 05:15:02.636304 flask_attachments-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-01-23 05:14:44.000000 flask_attachments-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 05:15:02.632304 flask_attachments-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-01-23 05:14:44.000000 flask_attachments-0.2.0/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (127)     4962 2024-01-23 05:14:44.000000 flask_attachments-0.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-01-23 05:14:44.000000 flask_attachments-0.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-01-23 05:14:44.000000 flask_attachments-0.2.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-01-23 05:14:44.000000 flask_attachments-0.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-01-23 05:14:44.000000 flask_attachments-0.2.0/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-23 05:14:44.000000 flask_attachments-0.2.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-01-23 05:14:44.000000 flask_attachments-0.2.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-01-23 05:14:44.000000 flask_attachments-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-01-23 05:15:02.636304 flask_attachments-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-01-23 05:14:44.000000 flask_attachments-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 05:15:02.628304 flask_attachments-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 05:15:02.632304 flask_attachments-0.2.0/src/flask_attachments/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-01-23 05:14:44.000000 flask_attachments-0.2.0/src/flask_attachments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6566 2024-01-23 05:14:44.000000 flask_attachments-0.2.0/src/flask_attachments/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-01-23 05:14:44.000000 flask_attachments-0.2.0/src/flask_attachments/compression.py
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-01-23 05:14:44.000000 flask_attachments-0.2.0/src/flask_attachments/extension.py
--rw-r--r--   0 runner    (1001) docker     (127)    11114 2024-01-23 05:14:44.000000 flask_attachments-0.2.0/src/flask_attachments/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 05:14:44.000000 flask_attachments-0.2.0/src/flask_attachments/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-01-23 05:14:44.000000 flask_attachments-0.2.0/src/flask_attachments/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-01-23 05:14:44.000000 flask_attachments-0.2.0/src/flask_attachments/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 05:15:02.636304 flask_attachments-0.2.0/src/flask_attachments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-01-23 05:15:02.000000 flask_attachments-0.2.0/src/flask_attachments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-01-23 05:15:02.000000 flask_attachments-0.2.0/src/flask_attachments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 05:15:02.000000 flask_attachments-0.2.0/src/flask_attachments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-23 05:15:02.000000 flask_attachments-0.2.0/src/flask_attachments.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 05:15:02.636304 flask_attachments-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-23 05:14:44.000000 flask_attachments-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-01-23 05:14:44.000000 flask_attachments-0.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-01-23 05:14:44.000000 flask_attachments-0.2.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-01-23 05:14:44.000000 flask_attachments-0.2.0/tests/test_compression.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-01-23 05:14:44.000000 flask_attachments-0.2.0/tests/test_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-01-23 05:14:44.000000 flask_attachments-0.2.0/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-01-23 05:14:44.000000 flask_attachments-0.2.0/tests/test_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-01-23 05:14:44.000000 flask_attachments-0.2.0/tests/test_views.py
+-rw-r--r--   0        0        0      247 2024-04-09 22:33:47.000000 flask_attachments-0.2.1/src/flask_attachments/__about__.py
+-rw-r--r--   0        0        0      372 2024-04-09 22:33:47.000000 flask_attachments-0.2.1/src/flask_attachments/__init__.py
+-rw-r--r--   0        0        0      411 2024-04-09 22:33:47.000000 flask_attachments-0.2.1/src/flask_attachments/_version.py
+-rw-r--r--   0        0        0     6566 2024-04-09 22:33:47.000000 flask_attachments-0.2.1/src/flask_attachments/cli.py
+-rw-r--r--   0        0        0     3850 2024-04-09 22:33:47.000000 flask_attachments-0.2.1/src/flask_attachments/compression.py
+-rw-r--r--   0        0        0     7419 2024-04-09 22:33:47.000000 flask_attachments-0.2.1/src/flask_attachments/extension.py
+-rw-r--r--   0        0        0    12035 2024-04-09 22:33:47.000000 flask_attachments-0.2.1/src/flask_attachments/models.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:33:47.000000 flask_attachments-0.2.1/src/flask_attachments/py.typed
+-rw-r--r--   0        0        0     2989 2024-04-09 22:33:47.000000 flask_attachments-0.2.1/src/flask_attachments/services.py
+-rw-r--r--   0        0        0     1153 2024-04-09 22:33:47.000000 flask_attachments-0.2.1/src/flask_attachments/views.py
+-rw-r--r--   0        0        0     1223 2024-04-09 22:33:47.000000 flask_attachments-0.2.1/.gitignore
+-rw-r--r--   0        0        0       98 2024-04-09 22:33:47.000000 flask_attachments-0.2.1/AUTHORS.rst
+-rw-r--r--   0        0        0     1502 2024-04-09 22:33:47.000000 flask_attachments-0.2.1/LICENSE
+-rw-r--r--   0        0        0      814 2024-04-09 22:33:47.000000 flask_attachments-0.2.1/README.md
+-rw-r--r--   0        0        0     2384 2024-04-09 22:33:47.000000 flask_attachments-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1791 2024-04-09 22:33:47.000000 flask_attachments-0.2.1/PKG-INFO
```

### Comparing `flask_attachments-0.2.0/LICENSE` & `flask_attachments-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_attachments-0.2.0/README.md` & `flask_attachments-0.2.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # Flask Attachments
 
 
 [![PyPI](https://img.shields.io/pypi/v/flask_attachments.svg)](https://pypi.python.org/pypi/flask_attachments)
-
 [![Tests](https://github.com/alexrudy/flask-attachments/workflows/Tests/badge.svg)](https://github.com/alexrudy/flask-attachments/workflows/Tests/)
+[![Documentation Status](https://readthedocs.org/projects/flask-attachments/badge/?version=latest)](https://flask-attachments.readthedocs.io/en/latest/?badge=latest)
+![BSD licensed][license-image]
 
 Flask Attachments provides a way to integrate arbitrary media with SQLAlchemy in a Flask website.
 
 Useful if you can't have all of your media statically defined, and need to allow users or administrators
 to upload binary blobs of data.
 
 
 * Free software: BSD license
+
+[license-image]: https://img.shields.io/badge/license-BSD-blue.svg
```

### Comparing `flask_attachments-0.2.0/src/flask_attachments/cli.py` & `flask_attachments-0.2.1/src/flask_attachments/cli.py`

 * *Files identical despite different names*

### Comparing `flask_attachments-0.2.0/src/flask_attachments/compression.py` & `flask_attachments-0.2.1/src/flask_attachments/compression.py`

 * *Files identical despite different names*

### Comparing `flask_attachments-0.2.0/src/flask_attachments/extension.py` & `flask_attachments-0.2.1/src/flask_attachments/extension.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,17 +8,19 @@
 from typing import cast
 from typing import TYPE_CHECKING
 
 import structlog
 from flask import current_app
 from flask import Flask
 from sqlalchemy import event
+from sqlalchemy import MetaData
 from sqlalchemy.engine import create_engine
 from sqlalchemy.engine import Engine
 from sqlalchemy.engine import make_url
+from sqlalchemy.orm import registry as Registry
 from werkzeug.local import LocalProxy
 
 from .compression import CompressionAlgorithm
 
 if TYPE_CHECKING:
     from .services import AttachmentCache
 
@@ -27,14 +29,16 @@
 
 EXTENSION_NAME = "flask-attachments"
 EXTENSION_CONFIG_NAMESPACE = "ATTACHMENTS_"
 
 
 logger = structlog.get_logger(__name__)
 
+__all__ = ["Attachments", "AttachmentSettings", "settings", "AttachmentsConfigurationError"]
+
 
 @dc.dataclass
 class AttachmentSettings:
     engine: Engine
 
     @property
     def config(self) -> dict[str, Any]:
@@ -76,29 +80,52 @@
 def get_settings() -> AttachmentSettings:
     try:
         return current_app.extensions[EXTENSION_NAME]
     except KeyError as exc:
         raise RuntimeError("No attachments extension registered on this app, call init_app first") from exc
 
 
+#: Flask proxy to the current attachment settings
 settings = cast(AttachmentSettings, LocalProxy(get_settings))
 
 
 class AttachmentsConfigurationError(ValueError):
+    """Configuration error for the Attachments extension"""
+
     pass
 
 
 class Attachments:
-    def __init__(self, app: Flask | None = None) -> None:
+    def __init__(self, app: Flask | None = None, registry: Registry | None = None) -> None:
+        from .models import Attachment
+
+        if registry is None:
+            registry = Registry()
+
+        if not hasattr(Attachment, "__mapper__"):
+            registry.map_declaratively(Attachment)
+        elif Attachment.__table__ not in registry.metadata:  # type: ignore
+            raise AttachmentsConfigurationError(
+                "The Attachment model has already been mapped to a different metadata"
+                "\nConsider providing a custom registry to the Attachments extension"
+                "\nor only intializing the extension once"
+            )
+
+        self.registry = registry
+
         if app is not None:
             self.init_app(app)
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__} at {id(self)!s}>"
 
+    @property
+    def metadata(self) -> MetaData:
+        return self.registry.metadata
+
     def init_app(self, app: Flask) -> None:
         """Initialize the app here"""
 
         from .cli import group as command_group
 
         if f"{EXTENSION_CONFIG_NAMESPACE}DATABASE_URI" not in app.config:
             raise AttachmentsConfigurationError(
```

### Comparing `flask_attachments-0.2.0/src/flask_attachments/models.py` & `flask_attachments-0.2.1/src/flask_attachments/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 import os
 import shutil
 import tempfile
 import uuid
 from pathlib import Path
 from typing import Any
 from typing import IO
+from typing import TYPE_CHECKING
 from zlib import crc32
 
 import structlog
 from flask import send_file
 from flask import url_for
 from sqlalchemy import DateTime
 from sqlalchemy import Enum
 from sqlalchemy import event
 from sqlalchemy import func
 from sqlalchemy import Integer
 from sqlalchemy import LargeBinary
 from sqlalchemy import String
 from sqlalchemy import Uuid
-from sqlalchemy.orm import DeclarativeBase
 from sqlalchemy.orm import deferred
 from sqlalchemy.orm import Mapped
 from sqlalchemy.orm import mapped_column
 from sqlalchemy.orm import validates
 from werkzeug import Response
 from werkzeug.datastructures import FileStorage
 from werkzeug.http import parse_options_header
@@ -35,42 +35,71 @@
 
 from .compression import CompressionAlgorithm
 from .extension import settings
 
 logger = structlog.get_logger(__name__)
 mtdb = mimetypes.MimeTypes()
 
+__all__ = ["Attachment"]
 
-class Base(DeclarativeBase):
-    """Provides a base class for all models in flask-attachments"""
 
-
-class Attachment(Base):
-    """Represents a file on the filesystem / or stored in the attachment database"""
+class Attachment:
+    """Represents a file on the filesystem or stored in the attachment database"""
 
     __tablename__ = "attachment"
 
+    #: Primary key (a UUID)
     id: Mapped[uuid.UUID] = mapped_column(Uuid, primary_key=True, default=uuid.uuid4)
+
+    #: When this attachment was created (in the database)
     created: Mapped[dt.datetime] = mapped_column(DateTime, nullable=False, server_default=func.now())
+
+    #: When this attachment record   was last updated
     updated: Mapped[dt.datetime] = mapped_column(
         DateTime, nullable=False, onupdate=func.now(), server_default=func.now()
     )
 
+    #: The name used for display and download of the attachment
     filename: Mapped[str] = mapped_column(String(), nullable=True, doc="for display and serving purposes")
+
+    #: The MIME type of the file
     content_type: Mapped[str] = mapped_column(String(), nullable=True, doc="for serving the correct file content_type")
+
+    #: The length of the file in bytes, uncompressed
     content_length: Mapped[int] = mapped_column(Integer(), nullable=True, doc="uncompressed content length (bytes)")
+
+    #: The compressed file contents
     contents: Mapped[bytes] = deferred(mapped_column(LargeBinary(), doc="compressed file contents"))
+
+    #: The compression algorithm used
     compression: Mapped[CompressionAlgorithm] = mapped_column(
         Enum(CompressionAlgorithm), nullable=False, doc="which compression alogirthm was used"
     )
+
+    #: The hash digest of the file
     digest: Mapped[str] = mapped_column(String(), nullable=False, doc="hash digest for file")
+
+    #: The hash digest algorithm used
     digest_algorithm: Mapped[str] = mapped_column(String(), nullable=False, doc="algorithm for digest")
 
     __table_args__ = ({"schema": "attachments"},)
 
+    if TYPE_CHECKING:
+
+        def __init__(
+            self,
+            *,
+            filename: str | None = None,
+            content_type: str | None = None,
+            content_length: int | None = None,
+            compression: CompressionAlgorithm | None = None,
+            digest_algorithm: str | None = None,
+        ) -> None:
+            ...
+
     def __repr__(self) -> str:
         return f"<Attachment id={self.id} filename={self.filename} mimetype={self.mimetype}>"
 
     def _empty_cache(self, property: str) -> None:
         try:
             delattr(self, property)
         except (AttributeError, KeyError):
@@ -78,15 +107,15 @@
 
     @cached_property
     def _parsed_content_type(self) -> tuple[str, dict[str, str]]:
         return parse_options_header(self.content_type)
 
     @cached_property
     def mimetype(self) -> None | str:
-        """Get the mimetype for this file"""
+        """The MIME type for this file, possibly inferred"""
         if self.content_type is None:
             if self.filename is not None:
                 return mtdb.guess_type(self.filename)[0]
             return None
         return self._parsed_content_type[0]
 
     @validates("content_type")
@@ -105,15 +134,15 @@
     def _validate_filename(self, key: str, value: Any) -> Any:
         self._empty_cache("extension")
         self._empty_cache("etag")
         return value
 
     @cached_property
     def extension(self) -> None | str:
-        """Get the presumed extension for this file"""
+        """The presumed extension for this file"""
         if self.filename is not None:
             suffix = Path(self.filename).suffix
             if suffix:
                 return suffix
         if self.mimetype is not None:
             return mtdb.guess_extension(self.mimetype, strict=False)
         return None
@@ -143,29 +172,31 @@
     def etag(self) -> str:
         """The entity tag which will uniquely correspond to this file"""
         source = f"{self.digest_algorithm}-{self.digest}-{self.filename}-{self.content_type}"
         return f"{self.id.hex}-{crc32(source.encode('utf-8')):x}"
 
     @cached_property
     def link(self) -> str:
+        """Url for serving the file"""
         return url_for("attachments.id", id=self.id)
 
     @cached_property
     def download_link(self) -> str:
+        """Url for downloading the file"""
         return url_for("attachments.download", id=self.id)
 
     @classmethod
     def from_file(
         cls,
         file: os.PathLike[str],
         content_type: str | None = None,
         compression: CompressionAlgorithm | str | None = None,
         digest_algorithm: str | None = None,
     ) -> "Attachment":
-        """Import a file from the filesystem"""
+        """Create a new attachment by reading a file from disk"""
 
         if content_type is None:
             content_type = mtdb.guess_type(str(file))[0]
 
         attachment = cls(
             filename=Path(file).name,
             content_type=content_type,
@@ -174,15 +205,15 @@
         with open(file, "rb") as stream:
             attachment.streamed(stream, compression=compression, digest_algorithm=digest_algorithm)
         return attachment
 
     def data(
         self, data: bytes, compression: CompressionAlgorithm | str | None = None, digest_algorithm: str | None = None
     ) -> None:
-        """Import a file from bytes"""
+        """Load a file from bytes into this attachment"""
         compression = parse_compression(compression)
         digest_algorithm = parse_digest(digest_algorithm)
 
         # Save file contents
         self.content_length = len(data)
         self.contents = compressed = compression.compress(data)
         self.compression = compression
@@ -199,15 +230,15 @@
     def streamed(
         self,
         stream: IO[bytes],
         compression: CompressionAlgorithm | str | None = None,
         digest_algorithm: str | None = None,
         chunk_size: int = 16384,
     ) -> None:
-        """Import a file from bytes"""
+        """Stream a file from bytes into this attachment"""
         compression = parse_compression(compression)
         digest_algorithm = parse_digest(digest_algorithm)
 
         # Save file contents
         contents = compression.stream(digest=digest_algorithm)
         with contextlib.closing(contents) as contents:
             shutil.copyfileobj(stream, contents, length=chunk_size)
@@ -229,14 +260,15 @@
         if self.content_type is None:
             self.content_type = file.content_type
 
         self.streamed(file.stream)
 
     @cached_property
     def cached_filepath(self) -> Path:
+        """The path to the file in the cache (on disk)"""
         filename = settings.cache_directory() / f"{self.digest_algorithm}-{self.digest}"
         if self.extension is not None:
             return filename.with_suffix(self.extension)
         return filename
 
     def warm(self) -> None:
         """Ensure that the file exists in the cache."""
```

### Comparing `flask_attachments-0.2.0/src/flask_attachments/services.py` & `flask_attachments-0.2.1/src/flask_attachments/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import datetime as dt
 from collections.abc import Iterator
 from pathlib import Path
 
 from .extension import AttachmentSettings
 from .extension import get_settings
 
+__all__ = ["AttachmentCache"]
+
 
 class AttachmentCache(collections.abc.Mapping[str, Path]):
     """On-disk cache for attachment files
 
     On-disk static files allows for more efficient serving.
     """
```

### Comparing `flask_attachments-0.2.0/src/flask_attachments/views.py` & `flask_attachments-0.2.1/src/flask_attachments/views.py`

 * *Files identical despite different names*

