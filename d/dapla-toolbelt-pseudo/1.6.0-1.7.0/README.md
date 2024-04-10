# Comparing `tmp/dapla_toolbelt_pseudo-1.6.0.tar.gz` & `tmp/dapla_toolbelt_pseudo-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dapla_toolbelt_pseudo-1.6.0.tar", max compression
+gzip compressed data, was "dapla_toolbelt_pseudo-1.7.0.tar", max compression
```

## Comparing `dapla_toolbelt_pseudo-1.6.0.tar` & `dapla_toolbelt_pseudo-1.7.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1073 2024-04-04 07:31:18.250551 dapla_toolbelt_pseudo-1.6.0/LICENSE
--rw-r--r--   0        0        0    16351 2024-04-04 07:31:18.250551 dapla_toolbelt_pseudo-1.6.0/README.md
--rw-r--r--   0        0        0     4433 2024-04-04 07:31:29.954581 dapla_toolbelt_pseudo-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     1443 2024-04-04 07:31:18.250551 dapla_toolbelt_pseudo-1.6.0/src/dapla_pseudo/__init__.py
--rw-r--r--   0        0        0     1430 2024-04-04 07:31:18.250551 dapla_toolbelt_pseudo-1.6.0/src/dapla_pseudo/constants.py
--rw-r--r--   0        0        0      994 2024-04-04 07:31:18.250551 dapla_toolbelt_pseudo-1.6.0/src/dapla_pseudo/exceptions.py
--rw-r--r--   0        0        0      847 2024-04-04 07:31:18.250551 dapla_toolbelt_pseudo-1.6.0/src/dapla_pseudo/models.py
--rw-r--r--   0        0        0        0 2024-04-04 07:31:18.250551 dapla_toolbelt_pseudo-1.6.0/src/dapla_pseudo/py.typed
--rw-r--r--   0        0        0      781 2024-04-04 07:31:18.250551 dapla_toolbelt_pseudo-1.6.0/src/dapla_pseudo/types.py
--rw-r--r--   0        0        0     2125 2024-04-04 07:31:18.250551 dapla_toolbelt_pseudo-1.6.0/src/dapla_pseudo/utils.py
--rw-r--r--   0        0        0      543 2024-04-04 07:31:18.250551 dapla_toolbelt_pseudo-1.6.0/src/dapla_pseudo/v1/__init__.py
--rw-r--r--   0        0        0     9856 2024-04-04 07:31:18.250551 dapla_toolbelt_pseudo-1.6.0/src/dapla_pseudo/v1/api_models.py
--rw-r--r--   0        0        0     2747 2024-04-04 07:31:18.250551 dapla_toolbelt_pseudo-1.6.0/src/dapla_pseudo/v1/baseclass.py
--rw-r--r--   0        0        0     6125 2024-04-04 07:31:18.250551 dapla_toolbelt_pseudo-1.6.0/src/dapla_pseudo/v1/client.py
--rw-r--r--   0        0        0    14770 2024-04-04 07:31:18.250551 dapla_toolbelt_pseudo-1.6.0/src/dapla_pseudo/v1/depseudo.py
--rw-r--r--   0        0        0    14444 2024-04-04 07:31:18.250551 dapla_toolbelt_pseudo-1.6.0/src/dapla_pseudo/v1/pseudo.py
--rw-r--r--   0        0        0     8468 2024-04-04 07:31:18.250551 dapla_toolbelt_pseudo-1.6.0/src/dapla_pseudo/v1/pseudo_commons.py
--rw-r--r--   0        0        0    19398 2024-04-04 07:31:18.250551 dapla_toolbelt_pseudo-1.6.0/src/dapla_pseudo/v1/repseudo.py
--rw-r--r--   0        0        0     8396 2024-04-04 07:31:18.250551 dapla_toolbelt_pseudo-1.6.0/src/dapla_pseudo/v1/result.py
--rw-r--r--   0        0        0     4188 2024-04-04 07:31:18.250551 dapla_toolbelt_pseudo-1.6.0/src/dapla_pseudo/v1/supported_file_format.py
--rw-r--r--   0        0        0     5634 2024-04-04 07:31:18.250551 dapla_toolbelt_pseudo-1.6.0/src/dapla_pseudo/v1/validation.py
--rw-r--r--   0        0        0    17801 1970-01-01 00:00:00.000000 dapla_toolbelt_pseudo-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-09 16:03:11.809585 dapla_toolbelt_pseudo-1.7.0/LICENSE
+-rw-r--r--   0        0        0    17119 2024-04-09 16:03:11.809585 dapla_toolbelt_pseudo-1.7.0/README.md
+-rw-r--r--   0        0        0     4728 2024-04-09 16:03:28.369570 dapla_toolbelt_pseudo-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1443 2024-04-09 16:03:11.813585 dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/__init__.py
+-rw-r--r--   0        0        0     1763 2024-04-09 16:03:11.813585 dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/constants.py
+-rw-r--r--   0        0        0      994 2024-04-09 16:03:11.813585 dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/exceptions.py
+-rw-r--r--   0        0        0      847 2024-04-09 16:03:11.813585 dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/models.py
+-rw-r--r--   0        0        0        0 2024-04-09 16:03:11.813585 dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/py.typed
+-rw-r--r--   0        0        0      828 2024-04-09 16:03:11.813585 dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/types.py
+-rw-r--r--   0        0        0     2115 2024-04-09 16:03:11.813585 dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/utils.py
+-rw-r--r--   0        0        0      543 2024-04-09 16:03:11.813585 dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/__init__.py
+-rw-r--r--   0        0        0     9774 2024-04-09 16:03:11.813585 dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/api_models.py
+-rw-r--r--   0        0        0     2974 2024-04-09 16:03:11.813585 dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/baseclass.py
+-rw-r--r--   0        0        0     6118 2024-04-09 16:03:11.813585 dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/client.py
+-rw-r--r--   0        0        0    15039 2024-04-09 16:03:11.813585 dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/depseudo.py
+-rw-r--r--   0        0        0    15314 2024-04-09 16:03:11.813585 dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/pseudo.py
+-rw-r--r--   0        0        0     9346 2024-04-09 16:03:11.813585 dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/pseudo_commons.py
+-rw-r--r--   0        0        0    19278 2024-04-09 16:03:11.813585 dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/repseudo.py
+-rw-r--r--   0        0        0     8330 2024-04-09 16:03:11.813585 dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/result.py
+-rw-r--r--   0        0        0     4188 2024-04-09 16:03:11.813585 dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/supported_file_format.py
+-rw-r--r--   0        0        0     5611 2024-04-09 16:03:11.813585 dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/validation.py
+-rw-r--r--   0        0        0    18569 1970-01-01 00:00:00.000000 dapla_toolbelt_pseudo-1.7.0/PKG-INFO
```

### Comparing `dapla_toolbelt_pseudo-1.6.0/LICENSE` & `dapla_toolbelt_pseudo-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.6.0/README.md` & `dapla_toolbelt_pseudo-1.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,37 @@
 ```
 
 The default encryption algorithm is DAEAD (Deterministic Authenticated Encryption with Associated Data). However, if the
 field is a valid Norwegian personal identification number (fnr, dnr), the recommended way to pseudonymize is to use
 the function `with_stable_id()` to convert the identification number to a stable ID (SID) prior to pseudonymization.
 In that case, the pseudonymization algorithm is FPE (Format Preserving Encryption).
 
+> [!IMPORTANT]
+> FPE requires minimum two bytes/characters to perform encryption and minimum four bytes in case of Unicode.
+
+If a field cannot be converted using the function `with_stable_id()` the default behaviour is to use the original value
+as input to the FPE encryption function. However, this behaviour can be changed by supplying a `failure_strategy` like
+this:
+
+```python
+from dapla_pseudo import Pseudonymize
+from dapla_pseudo.constants import MapFailureStrategy
+
+# Example: Single field sid mapping and pseudonymization (FPE), unmatching SIDs will return Null
+result_df = (
+    Pseudonymize.from_polars(df)
+    .on_fields("fnr")
+    .with_stable_id(failure_strategy=MapFailureStrategy.RETURN_NULL)
+    .run()
+    .to_polars()
+)
+```
+
+
+### Reading dataframes
 
 Note that you may also use a Pandas DataFrame as an input or output, by exchanging `from_polars` with `from_pandas`
 and `to_polars` with `to_pandas`. However, Pandas is much less performant, so take special care especially if your
 dataset is large.
 
 Example:
```

### Comparing `dapla_toolbelt_pseudo-1.6.0/pyproject.toml` & `dapla_toolbelt_pseudo-1.7.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dapla-toolbelt-pseudo"
-version = "1.6.0"
+version = "1.7.0"
 description = "Pseudonymization extensions for Dapla"
 authors = ["Dapla Developers <dapla-platform-developers@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/statisticsnorway/dapla-toolbelt-pseudo"
 repository = "https://github.com/statisticsnorway/dapla-toolbelt-pseudo"
 documentation = "https://statisticsnorway.github.io/dapla-toolbelt-pseudo"
@@ -40,15 +40,15 @@
 black = { extras = ["jupyter"], version = ">=23.1.0" }
 coverage = { extras = ["toml"], version = ">=6.2" }
 darglint = ">=1.8.1"
 furo = ">=2021.11.12"
 mypy = ">=0.930"
 pre-commit = ">=2.16.0"
 pre-commit-hooks = ">=4.1.0"
-ruff = ">=0.0.284"
+ruff = ">=0.3.1"
 pytest = ">=6.2.5"
 sphinx = ">=6.2.1"
 sphinx-autobuild = ">=2021.3.14"
 sphinx-autodoc-typehints = ">=1.24.0"
 sphinx-click = ">=3.0.2"
 typeguard = ">=2.13.3"
 xdoctest = { extras = ["colors"], version = ">=0.15.10" }
@@ -68,14 +68,15 @@
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 tests = ["tests", "*/tests"]
 
 [tool.coverage.run]
 branch = true
 source = ["dapla_pseudo", "tests"]
+relative_files = true
 
 [tool.coverage.report]
 show_missing = true
 fail_under = 50
 
 [tool.mypy]
 strict = true
@@ -100,64 +101,71 @@
 ]
 ignore_missing_imports = true
 
 [tool.ruff]
 force-exclude = true  # Apply excludes to pre-commit
 show-fixes = true
 src = ["src", "tests"]
-target-version = "py39"  # Minimum Python version supported
+target-version = "py310"  # Minimum Python version supported
+include = ["*.py", "*.pyi", "**/pyproject.toml", "*.ipynb"]
+extend-exclude = [
+    "__pycache__",
+    "old",
+    ".ipynb_checkpoints",
+    "noxfile.py",
+    "docs/conf.py",
+]
 
 # Ruff rules may be customized as desired: https://docs.astral.sh/ruff/rules/
+[tool.ruff.lint]
 select = [
     "A",    # prevent using keywords that clobber python builtins
+    "ANN",  # check type annotations
     "B",    # bugbear: security warnings
     "D",    # documentation
     "E",    # pycodestyle
     "F",    # pyflakes
     "ISC",  # implicit string concatenation
     "I",    # sort imports
     "UP",   # alert you when better syntax is available in your python version
     "RUF",  # the ruff developer's own rules
 ]
 ignore = [
     "ANN101", # Supress missing-type-self.
+    "ANN102", # Supress missing-type-cls.
+    "ANN202", # Don't require return type annotation for private functions.
+    "ANN401", # Allow type annotation with type Any.
     "D100",   # Supress undocumented-public-module. Only doc of public api required.
     "E402",   # Supress module-import-not-at-top-of-file, needed in jupyter notebooks.
     "E501",   # Supress line-too-long warnings: trust black's judgement on this one.
 ]
-include = ["*.py", "*.pyi", "**/pyproject.toml", "*.ipynb"]
-extend-exclude = [
-    "__pycache__",
-    "old",
-    ".ipynb_checkpoints",
-    "noxfile.py",
-    "docs/conf.py",
-]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 force-single-line = true
 
-[tool.ruff.mccabe]
+[tool.ruff.lint.mccabe]
 max-complexity = 15
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "google"  # You can also use "numpy".
 
-[tool.ruff.pep8-naming]
+[tool.ruff.lint.pep8-naming]
 classmethod-decorators = ["classmethod", "validator", "root_validator", "pydantic.validator"]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "*/__init__.py" = ["F401"]
 "**/tests/*" = [
     # asserts are encouraged in pytest
     "S101",
     # return annotations don't add value for test functions
     "ANN201",
     # docstrings are overkill for test functions
-    "D103",
     "D100",
+    "D101",
+    "D102",
+    "D103",
 ]
 "tests/integration/*" = ["F401", "F811"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dapla_toolbelt_pseudo-1.6.0/src/dapla_pseudo/__init__.py` & `dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/__init__.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.6.0/src/dapla_pseudo/constants.py` & `dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/constants.py`

 * *Files 15% similar despite different names*

```diff
@@ -48,7 +48,18 @@
     SKIP = "skip"
     DELETE = "delete"
     REDACT = "redact"
 
     def __str__(self) -> str:
         """Use value for string representation."""
         return str(self.value)
+
+
+class MapFailureStrategy(str, Enum):
+    """UnknownCharacterStrategy defines how encryption/decryption should handle non-alphabet characters."""
+
+    RETURN_NULL = "RETURN_NULL"
+    RETURN_ORIGINAL = "RETURN_ORIGINAL"
+
+    def __str__(self) -> str:
+        """Use value for string representation."""
+        return str(self.value)
```

### Comparing `dapla_toolbelt_pseudo-1.6.0/src/dapla_pseudo/exceptions.py` & `dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/exceptions.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.6.0/src/dapla_pseudo/models.py` & `dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/models.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.6.0/src/dapla_pseudo/utils.py` & `dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             item[1] for item in multipart_files_tuple if item[0] == obj_name
         )
         return matching_item[1]
     except StopIteration:
         return None
 
 
-def convert_to_date(sid_snapshot_date: t.Optional[date | str]) -> t.Optional[date]:
+def convert_to_date(sid_snapshot_date: date | str | None) -> date | None:
     """Converts the SID version date to the 'date' type, if it is a string.
 
     If None, simply passes the None through the function.
     """
     if isinstance(sid_snapshot_date, str):
         try:
             return date.fromisoformat(sid_snapshot_date)
```

### Comparing `dapla_toolbelt_pseudo-1.6.0/src/dapla_pseudo/v1/__init__.py` & `dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.6.0/src/dapla_pseudo/v1/api_models.py` & `dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/api_models.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from pydantic import BaseModel
 from pydantic import ConfigDict
 from pydantic import FieldSerializationInfo
 from pydantic import ValidationError
 from pydantic import field_serializer
 from pydantic import model_serializer
 
+from dapla_pseudo.constants import MapFailureStrategy
 from dapla_pseudo.constants import PredefinedKeys
 from dapla_pseudo.constants import PseudoFunctionTypes
 from dapla_pseudo.constants import UnknownCharacterStrategy
 from dapla_pseudo.models import APIModel
 
 
 class Mimetypes(str, Enum):
@@ -35,15 +36,15 @@
     Parameters:
         pattern: field name or expression (e.g. a glob)
         mapping: If defined, denotes a mapping transformation that should be applied before the operation in question,
             e.g. "sid", meaning the field should be transformed to Stabil ID before being pseudonymized.
     """
 
     pattern: str
-    mapping: t.Optional[str] = None
+    mapping: str | None = None
 
 
 class PseudoKeyset(APIModel):
     """PseudoKeyset represents a wrapped data encryption key (WDEK).
 
     Example structure, represented as JSON:
     {"encrypted_keyset": "CiQAp91NBhLdknX3j9jF6vwhdyURaqcT9/M/iczV7fLn...8XYFKwxiwMtCzDT6QGzCCCM=",
@@ -77,17 +78,17 @@
     password: str
 
 
 class KeyWrapper(BaseModel):
     """Hold information about a key, such as ID and keyset information."""
 
     key_id: str = ""
-    keyset: t.Optional[PseudoKeyset] = None
+    keyset: PseudoKeyset | None = None
 
-    def __init__(self, key: t.Optional[str | PseudoKeyset] = None, **kwargs: t.Any):
+    def __init__(self, key: str | PseudoKeyset | None = None, **kwargs: t.Any) -> None:
         """Determine if a key is either a key reference (aka "common key") or a keyset.
 
         If it is a key reference, treat this as the key's ID, else retrieve the key's ID from the keyset data structure.
 
         :param key: either a key reference (as string) or a PseudoKeyset
         """
         super().__init__(**kwargs)
@@ -107,15 +108,15 @@
             else:
                 raise ValueError(f"Key '{key}' is not a valid key reference or keyset")
         # Or we have an already parsed PseudoKeyset
         elif isinstance(key, PseudoKeyset):
             self.key_id = key.get_key_id()
             self.keyset = key
 
-    def keyset_list(self) -> t.Optional[list[PseudoKeyset]]:
+    def keyset_list(self) -> list[PseudoKeyset] | None:
         """Wrap the keyset in a list if it is defined - or return None if it is not."""
         return None if self.keyset is None else [self.keyset]
 
 
 class PseudoFunctionArgs(BaseModel):
     """Representation of the possible keyword arguments."""
 
@@ -135,59 +136,55 @@
 
     Parameters:
         key_id: The key to be used for pseudonomization.
         snapshot_date (date): The timestamp for the version of the SID catalogue.
             If not specified, will choose the latest version.
             The format is: YYYY-MM-DD, e.g. 2021-05-21
         strategy: defines how encryption/decryption should handle non-alphabet characters
+        failure_strategy: defines how to handle mapping failures
     """
 
     key_id: PredefinedKeys | str = PredefinedKeys.PAPIS_COMMON_KEY_1
-    snapshot_date: t.Optional[date] = None
-    strategy: t.Optional[UnknownCharacterStrategy] = UnknownCharacterStrategy.SKIP
+    snapshot_date: date | None = None
+    strategy: UnknownCharacterStrategy | None = UnknownCharacterStrategy.SKIP
+    failure_strategy: MapFailureStrategy | None = None
 
 
 class DaeadKeywordArgs(PseudoFunctionArgs):
     """Representation of kwargs for the 'daead' function."""
 
     key_id: PredefinedKeys | str = PredefinedKeys.SSB_COMMON_KEY_1
 
 
 class FF31KeywordArgs(PseudoFunctionArgs):
     """Representation of kwargs for the 'FF31' function."""
 
     key_id: PredefinedKeys | str = PredefinedKeys.PAPIS_COMMON_KEY_1
-    strategy: t.Optional[UnknownCharacterStrategy] = UnknownCharacterStrategy.SKIP
+    strategy: UnknownCharacterStrategy | None = UnknownCharacterStrategy.SKIP
 
 
-class RedactArgs(PseudoFunctionArgs):
+class RedactKeywordArgs(PseudoFunctionArgs):
     """Representation of kwargs for the 'redact' function."""
 
-    replacement_string: str
-
-    def __str__(self) -> str:
-        """Overload the parent class. The redact function is expected as an arg, not kwarg.
-
-        I.e. 'redact(<replacement_string>)'
-        """
-        return self.replacement_string
+    placeholder: str | None = None
+    regex: str | None = None
 
 
 class PseudoFunction(BaseModel):
     """Formal representation of a pseudo function.
 
     Use to build up the string representation expected by pseudo service.
 
     Syntax: "<function_type>(<kwarg_1>=x, <kwarg_2>=y)"
 
     where <kwarg_1>, <kwarg_2>, etc. represents the keywords defined in PseudoFunctionArgs
     """
 
     function_type: PseudoFunctionTypes
-    kwargs: DaeadKeywordArgs | FF31KeywordArgs | MapSidKeywordArgs | RedactArgs
+    kwargs: DaeadKeywordArgs | FF31KeywordArgs | MapSidKeywordArgs | RedactKeywordArgs
 
     def __str__(self) -> str:
         """Create the function representation as expected by pseudo service."""
         return f"{self.function_type}({self.kwargs})"
 
     @model_serializer()
     def serialize_model(self) -> str:
@@ -206,15 +203,15 @@
 
     Parameters:
         name: A friendly name of the rule. This is optional, but can be handy for debugging
         pattern: Glob expression, such as: ``/**/{field1, field2, *navn}``
         func: A transformation function, such as ``tink-daead(<keyname>), redact(<replacementstring>) or fpe-anychar(<keyname>)``
     """
 
-    name: t.Optional[str] = None
+    name: str | None = None
     pattern: str
     func: PseudoFunction
 
     @field_serializer("func")
     def serialize_func(
         self, func: PseudoFunction, _info: FieldSerializationInfo
     ) -> str:
@@ -224,63 +221,63 @@
 
 class PseudoFieldRequest(APIModel):
     """Model of the pseudo field request sent to the service."""
 
     pseudo_func: PseudoFunction
     name: str
     values: list[str]
-    keyset: t.Optional[PseudoKeyset] = None
+    keyset: PseudoKeyset | None = None
 
 
 class DepseudoFieldRequest(APIModel):
     """Model of the depseudo field request sent to the service."""
 
     pseudo_func: PseudoFunction
     name: str
     values: list[str]
-    keyset: t.Optional[PseudoKeyset] = None
+    keyset: PseudoKeyset | None = None
 
 
 class RepseudoFieldRequest(APIModel):
     """Model of the repseudo field request sent to the service."""
 
     source_pseudo_func: PseudoFunction
     target_pseudo_func: PseudoFunction
     name: str
     values: list[str]
-    source_keyset: t.Optional[PseudoKeyset] = None
-    target_keyset: t.Optional[PseudoKeyset] = None
+    source_keyset: PseudoKeyset | None = None
+    target_keyset: PseudoKeyset | None = None
 
 
 class PseudoConfig(APIModel):
     """PseudoConfig is a container for rules and keysets."""
 
     rules: list[PseudoRule]
-    keysets: t.Optional[list[PseudoKeyset]] = None
+    keysets: list[PseudoKeyset] | None = None
 
 
 class PseudonymizeFileRequest(APIModel):
     """PseudonymizeFileRequest represents a request towards pseudonymize file API endpoints."""
 
     pseudo_config: PseudoConfig
-    target_uri: t.Optional[str] = None
+    target_uri: str | None = None
     target_content_type: Mimetypes
-    compression: t.Optional[TargetCompression] = None
+    compression: TargetCompression | None = None
 
 
 class DepseudonymizeFileRequest(APIModel):
     """DepseudonymizeFileRequest represents a request towards depseudonymize file API endpoints."""
 
     pseudo_config: PseudoConfig
-    target_uri: t.Optional[str] = None
+    target_uri: str | None = None
     target_content_type: Mimetypes
-    compression: t.Optional[TargetCompression] = None
+    compression: TargetCompression | None = None
 
 
 class RepseudonymizeFileRequest(APIModel):
     """RepseudonymizeFileRequest represents a request towards repseudonymize file API endpoints."""
 
     source_pseudo_config: PseudoConfig
     target_pseudo_config: PseudoConfig
-    target_uri: t.Optional[str] = None
+    target_uri: str | None = None
     target_content_type: Mimetypes
-    compression: t.Optional[TargetCompression] = None
+    compression: TargetCompression | None = None
```

### Comparing `dapla_toolbelt_pseudo-1.6.0/src/dapla_pseudo/v1/baseclass.py` & `dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/baseclass.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import typing as t
 from datetime import date
 
+from dapla_pseudo.constants import MapFailureStrategy
 from dapla_pseudo.constants import PredefinedKeys
 from dapla_pseudo.constants import PseudoFunctionTypes
 from dapla_pseudo.utils import convert_to_date
 from dapla_pseudo.v1.api_models import DaeadKeywordArgs
 from dapla_pseudo.v1.api_models import FF31KeywordArgs
 from dapla_pseudo.v1.api_models import MapSidKeywordArgs
 from dapla_pseudo.v1.api_models import PseudoFunction
@@ -18,43 +19,48 @@
         self, fields: list[str], dataset_type: t.Literal["file", "dataframe"]
     ) -> None:
         self._fields = fields
         self.dataset_type = dataset_type
 
     def _map_to_stable_id_and_pseudonymize(
         self,
-        sid_snapshot_date: t.Optional[str | date] = None,
-        custom_key: t.Optional[PredefinedKeys | str] = None,
+        sid_snapshot_date: str | date | None = None,
+        custom_key: PredefinedKeys | str | None = None,
+        failure_strategy: MapFailureStrategy | None = None,
     ) -> list[PseudoRule]:
         kwargs = (
             MapSidKeywordArgs(
                 key_id=custom_key,
                 snapshot_date=convert_to_date(sid_snapshot_date),
+                failure_strategy=failure_strategy,
             )
             if custom_key
-            else MapSidKeywordArgs(snapshot_date=convert_to_date(sid_snapshot_date))
+            else MapSidKeywordArgs(
+                snapshot_date=convert_to_date(sid_snapshot_date),
+                failure_strategy=failure_strategy,
+            )
         )
         pseudo_func = PseudoFunction(
             function_type=PseudoFunctionTypes.MAP_SID, kwargs=kwargs
         )
         return self._rule_constructor(pseudo_func)
 
     def _with_daead_encryption(
-        self, custom_key: t.Optional[PredefinedKeys | str] = None
+        self, custom_key: PredefinedKeys | str | None = None
     ) -> list[PseudoRule]:
         kwargs = (
             DaeadKeywordArgs(key_id=custom_key) if custom_key else DaeadKeywordArgs()
         )
         pseudo_func = PseudoFunction(
             function_type=PseudoFunctionTypes.DAEAD, kwargs=kwargs
         )
         return self._rule_constructor(pseudo_func)
 
     def _with_ff31_encryption(
-        self, custom_key: t.Optional[PredefinedKeys | str] = None
+        self, custom_key: PredefinedKeys | str | None = None
     ) -> list[PseudoRule]:
         kwargs = FF31KeywordArgs(key_id=custom_key) if custom_key else FF31KeywordArgs()
         pseudo_func = PseudoFunction(
             function_type=PseudoFunctionTypes.FF31, kwargs=kwargs
         )
         return self._rule_constructor(pseudo_func)
```

### Comparing `dapla_toolbelt_pseudo-1.6.0/src/dapla_pseudo/v1/client.py` & `dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,17 +29,17 @@
         PseudonymizeFileRequest: "pseudonymize/file",
         DepseudonymizeFileRequest: "depseudonymize/file",
         RepseudonymizeFileRequest: "repseudonymize/file",
     }
 
     def __init__(
         self,
-        pseudo_service_url: t.Optional[str] = None,
-        auth_token: t.Optional[str] = None,
-    ):
+        pseudo_service_url: str | None = None,
+        auth_token: str | None = None,
+    ) -> None:
         """Use a default url for dapla-pseudo-service if not explicitly set."""
         self.pseudo_service_url = (
             "http://dapla-pseudo-service.dapla.svc.cluster.local"
             if pseudo_service_url is None
             else pseudo_service_url
         )
         self.static_auth_token = auth_token
@@ -127,15 +127,15 @@
         PseudoClient._handle_response_error(response)
         return response
 
     def _post_to_sid_endpoint(
         self,
         path: str,
         values: list[str],
-        sid_snapshot_date: t.Optional[date] = None,
+        sid_snapshot_date: date | None = None,
         stream: bool = False,
     ) -> requests.Response:
         request: dict[str, t.Collection[str]] = {"fnrList": values}
         response = requests.post(
             url=f"{self.pseudo_service_url}/{path}",
             params={"snapshot": str(sid_snapshot_date)} if sid_snapshot_date else None,
             # Do not set content-type, as this will cause the json to serialize incorrectly
```

### Comparing `dapla_toolbelt_pseudo-1.6.0/src/dapla_pseudo/v1/depseudo.py` & `dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/depseudo.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Builder for submitting a pseudonymization request."""
 
 import os
 import typing as t
 from concurrent.futures import ThreadPoolExecutor
 from concurrent.futures import as_completed
 from datetime import date
-from typing import Optional
 
 import pandas as pd
 import polars as pl
 
 from dapla_pseudo.constants import TIMEOUT_DEFAULT
 from dapla_pseudo.constants import Env
+from dapla_pseudo.constants import MapFailureStrategy
 from dapla_pseudo.constants import PredefinedKeys
 from dapla_pseudo.constants import PseudoFunctionTypes
 from dapla_pseudo.types import FileLikeDatasetDecl
 from dapla_pseudo.utils import convert_to_date
 from dapla_pseudo.v1.api_models import DaeadKeywordArgs
 from dapla_pseudo.v1.api_models import DepseudoFieldRequest
 from dapla_pseudo.v1.api_models import DepseudonymizeFileRequest
@@ -29,15 +29,15 @@
 from dapla_pseudo.v1.api_models import PseudoRule
 from dapla_pseudo.v1.client import PseudoClient
 from dapla_pseudo.v1.pseudo_commons import File
 from dapla_pseudo.v1.pseudo_commons import PseudoFieldResponse
 from dapla_pseudo.v1.pseudo_commons import PseudoFileResponse
 from dapla_pseudo.v1.pseudo_commons import RawPseudoMetadata
 from dapla_pseudo.v1.pseudo_commons import get_file_data_from_dataset
-from dapla_pseudo.v1.pseudo_commons import pseudo_operation_file
+from dapla_pseudo.v1.pseudo_commons import pseudo_operation_dataset
 from dapla_pseudo.v1.pseudo_commons import pseudonymize_operation_field
 from dapla_pseudo.v1.result import Result
 
 
 class Depseudonymize:
     """Starting point for depseudonymization of datasets.
 
@@ -85,31 +85,31 @@
         file_handle, content_type = get_file_data_from_dataset(dataset)
         Depseudonymize.dataset = File(file_handle, content_type)
         return Depseudonymize._Depseudonymizer()
 
     class _Depseudonymizer:
         """Select one or multiple fields to be pseudonymized."""
 
-        def __init__(self, rules: Optional[list[PseudoRule]] = None) -> None:
+        def __init__(self, rules: list[PseudoRule] | None = None) -> None:
             """Initialize the class."""
             self._rules: list[PseudoRule] = [] if rules is None else rules
-            self._pseudo_keyset: Optional[PseudoKeyset | str] = None
+            self._pseudo_keyset: PseudoKeyset | str | None = None
             self._timeout: int = TIMEOUT_DEFAULT
             self._pseudo_client: PseudoClient = PseudoClient(
                 pseudo_service_url=os.getenv(Env.PSEUDO_SERVICE_URL),
                 auth_token=os.getenv(Env.PSEUDO_SERVICE_AUTH_TOKEN),
             )
 
         def on_fields(self, *fields: str) -> "Depseudonymize._DepseudoFuncSelector":
             """Specify one or multiple fields to be depseudonymized."""
             return Depseudonymize._DepseudoFuncSelector(list(fields), self._rules)
 
         def run(
             self,
-            custom_keyset: Optional[PseudoKeyset | str] = None,
+            custom_keyset: PseudoKeyset | str | None = None,
             timeout: int = TIMEOUT_DEFAULT,
         ) -> Result:
             """Depseudonymize the dataset.
 
             Args:
                 custom_keyset (PseudoKeyset | str, optional): The depseudonymization keyset to use.
                     This can either be a PseudoKeyset, a JSON-string matching the fields of PseudoKeyset,
@@ -155,18 +155,17 @@
                     keysets=KeyWrapper(self._pseudo_keyset).keyset_list(),
                 ),
                 target_content_type=Mimetypes.JSON,
                 target_uri=None,
                 compression=None,
             )
 
-            pseudo_response: PseudoFileResponse = pseudo_operation_file(
-                file_handle=file.file_handle,
+            pseudo_response: PseudoFileResponse = pseudo_operation_dataset(
+                dataset_ref=file,
                 pseudo_operation_request=depseudonymize_request,
-                input_content_type=file.content_type,
             )
             return Result(pseudo_response=pseudo_response)
 
         def _depseudonymize_field(self) -> Result:
             """Depseudonymizes the specified fields in the DataFrame using the provided pseudonymization function.
 
             The depseudonymization is performed in parallel. After the parallel processing is finished,
@@ -229,53 +228,59 @@
                 pseudo_response=PseudoFieldResponse(
                     data=dataframe, raw_metadata=raw_metadata_fields
                 )
             )
 
     class _DepseudoFuncSelector:
         def __init__(
-            self, fields: list[str], rules: Optional[list[PseudoRule]] = None
+            self, fields: list[str], rules: list[PseudoRule] | None = None
         ) -> None:
             self._fields = fields
             self._existing_rules = [] if rules is None else rules
 
         def with_stable_id(
             self,
-            sid_snapshot_date: Optional[str | date] = None,
-            custom_key: Optional[str] = None,
+            sid_snapshot_date: str | date | None = None,
+            custom_key: str | None = None,
+            failure_strategy: MapFailureStrategy | None = None,
         ) -> "Depseudonymize._Depseudonymizer":
             """Depseudonymize the selected fields with the default encryption algorithm (DAEAD).
 
             1) Decrypt stable-id
             2) Then map decrypted stable-id to fnr and return original fnr.
 
             Args:
                 sid_snapshot_date (Optional[str | date], optional): Date representing SID-catalogue version to use.
                     Latest if unspecified. Format: YYYY-MM-DD
                 custom_key (Optional[PredefinedKeys | str], optional): Override the key to use for pseudonymization.
                     Must be one of the keys defined in PredefinedKeys. If not defined, uses the default key for this function (papis-common-key-1)
+                failure_strategy (Optional[MapFailureStrategy], optional): defines how to handle mapping failures
 
             Returns:
                 Self: The object configured to be mapped to fnr
             """
             kwargs = (
                 MapSidKeywordArgs(
                     key_id=custom_key,
                     snapshot_date=convert_to_date(sid_snapshot_date),
+                    failure_strategy=failure_strategy,
                 )
                 if custom_key
-                else MapSidKeywordArgs(snapshot_date=convert_to_date(sid_snapshot_date))
+                else MapSidKeywordArgs(
+                    snapshot_date=convert_to_date(sid_snapshot_date),
+                    failure_strategy=failure_strategy,
+                )
             )
             function = PseudoFunction(
                 function_type=PseudoFunctionTypes.MAP_SID, kwargs=kwargs
             )
             return self._rule_constructor(function)
 
         def with_default_encryption(
-            self, custom_key: Optional[PredefinedKeys | str] = None
+            self, custom_key: PredefinedKeys | str | None = None
         ) -> "Depseudonymize._Depseudonymizer":
             """Depseudonymize the selected fields with the default encryption algorithm (DAEAD).
 
             Args:
                 custom_key (Optional[PredefinedKeys | str], optional): Override the key to use for pseudonymization.
                     Must be one of the keys defined in PredefinedKeys. If not defined, uses the default key for this function (ssb-common-key-1)
 
@@ -289,15 +294,15 @@
             )
             function = PseudoFunction(
                 function_type=PseudoFunctionTypes.DAEAD, kwargs=kwargs
             )
             return self._rule_constructor(function)
 
         def with_papis_compatible_encryption(
-            self, custom_key: Optional[PredefinedKeys | str] = None
+            self, custom_key: PredefinedKeys | str | None = None
         ) -> "Depseudonymize._Depseudonymizer":
             """Depseudonymize the selected fields with a PAPIS-compatible encryption algorithm (FF31).
 
             Args:
                 custom_key (Optional[PredefinedKeys | str], optional): Override the key to use for pseudonymization.
                     Must be one of the keys defined in PredefinedKeys. If not defined, uses the default key for this function (papis-common-key-1)
```

### Comparing `dapla_toolbelt_pseudo-1.6.0/src/dapla_pseudo/v1/pseudo.py` & `dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/pseudo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """Builder for submitting a pseudonymization request."""
 
 import os
-import typing as t
 from concurrent.futures import ThreadPoolExecutor
 from concurrent.futures import as_completed
 from datetime import date
-from typing import Optional
 
 import pandas as pd
 import polars as pl
 
 from dapla_pseudo.constants import TIMEOUT_DEFAULT
 from dapla_pseudo.constants import Env
+from dapla_pseudo.constants import MapFailureStrategy
 from dapla_pseudo.constants import PredefinedKeys
 from dapla_pseudo.constants import PseudoFunctionTypes
 from dapla_pseudo.types import FileLikeDatasetDecl
 from dapla_pseudo.utils import convert_to_date
 from dapla_pseudo.v1.api_models import DaeadKeywordArgs
 from dapla_pseudo.v1.api_models import FF31KeywordArgs
 from dapla_pseudo.v1.api_models import KeyWrapper
@@ -25,42 +24,49 @@
 from dapla_pseudo.v1.api_models import PseudoFieldRequest
 from dapla_pseudo.v1.api_models import PseudoFunction
 from dapla_pseudo.v1.api_models import PseudoKeyset
 from dapla_pseudo.v1.api_models import PseudonymizeFileRequest
 from dapla_pseudo.v1.api_models import PseudoRule
 from dapla_pseudo.v1.client import PseudoClient
 from dapla_pseudo.v1.pseudo_commons import File
+from dapla_pseudo.v1.pseudo_commons import HierarchicalDataFrame
 from dapla_pseudo.v1.pseudo_commons import PseudoFieldResponse
 from dapla_pseudo.v1.pseudo_commons import PseudoFileResponse
 from dapla_pseudo.v1.pseudo_commons import RawPseudoMetadata
 from dapla_pseudo.v1.pseudo_commons import get_file_data_from_dataset
-from dapla_pseudo.v1.pseudo_commons import pseudo_operation_file
+from dapla_pseudo.v1.pseudo_commons import pseudo_operation_dataset
 from dapla_pseudo.v1.pseudo_commons import pseudonymize_operation_field
 from dapla_pseudo.v1.result import Result
 
 
 class Pseudonymize:
     """Starting point for pseudonymization of datasets.
 
     This class should not be instantiated, only the static methods should be used.
     """
 
-    dataset: File | pl.DataFrame
+    dataset: File | pl.DataFrame | HierarchicalDataFrame
 
     @staticmethod
     def from_pandas(dataframe: pd.DataFrame) -> "Pseudonymize._Pseudonymizer":
         """Initialize a pseudonymization request from a pandas DataFrame."""
         dataset: pl.DataFrame = pl.from_pandas(dataframe)
-        Pseudonymize.dataset = dataset
+        if pl.Struct in dataset.dtypes:
+            Pseudonymize.dataset = HierarchicalDataFrame(dataset)
+        else:
+            Pseudonymize.dataset = dataset
         return Pseudonymize._Pseudonymizer()
 
     @staticmethod
     def from_polars(dataframe: pl.DataFrame) -> "Pseudonymize._Pseudonymizer":
         """Initialize a pseudonymization request from a polars DataFrame."""
-        Pseudonymize.dataset = dataframe
+        if pl.Struct in dataframe.dtypes:
+            Pseudonymize.dataset = HierarchicalDataFrame(dataframe)
+        else:
+            Pseudonymize.dataset = dataframe
         return Pseudonymize._Pseudonymizer()
 
     @staticmethod
     def from_file(dataset: FileLikeDatasetDecl) -> "Pseudonymize._Pseudonymizer":
         """Initialize a pseudonymization request from a pandas dataframe read from file.
 
         Args:
@@ -85,31 +91,35 @@
         file_handle, content_type = get_file_data_from_dataset(dataset)
         Pseudonymize.dataset = File(file_handle, content_type)
         return Pseudonymize._Pseudonymizer()
 
     class _Pseudonymizer:
         """Select one or multiple fields to be pseudonymized."""
 
-        def __init__(self, rules: Optional[list[PseudoRule]] = None) -> None:
+        def __init__(self, rules: list[PseudoRule] | None = None) -> None:
             """Initialize the class."""
             self._rules: list[PseudoRule] = [] if rules is None else rules
-            self._pseudo_keyset: Optional[PseudoKeyset | str] = None
+            self._pseudo_keyset: PseudoKeyset | str | None = None
             self._timeout: int = TIMEOUT_DEFAULT
             self._pseudo_client: PseudoClient = PseudoClient(
                 pseudo_service_url=os.getenv(Env.PSEUDO_SERVICE_URL),
                 auth_token=os.getenv(Env.PSEUDO_SERVICE_AUTH_TOKEN),
             )
 
         def on_fields(self, *fields: str) -> "Pseudonymize._PseudoFuncSelector":
             """Specify one or multiple fields to be pseudonymized."""
             return Pseudonymize._PseudoFuncSelector(list(fields), self._rules)
 
+        def add_rules(self, *rules: PseudoRule) -> "Pseudonymize._Pseudonymizer":
+            """Specify one or more existing pseudonymization rule."""
+            return Pseudonymize._Pseudonymizer(self._rules + list(rules))
+
         def run(
             self,
-            custom_keyset: Optional[PseudoKeyset | str] = None,
+            custom_keyset: PseudoKeyset | str | None = None,
             timeout: int = TIMEOUT_DEFAULT,
         ) -> Result:
             """Pseudonymize the dataset.
 
             Args:
                 custom_keyset (PseudoKeyset, optional): The pseudonymization keyset to use. Defaults to None.
                 timeout (int): The timeout in seconds for the API call. Defaults to TIMEOUT_DEFAULT.
@@ -121,55 +131,53 @@
                 Result: The pseudonymized dataset and the associated metadata.
             """
             if Pseudonymize.dataset is None:
                 raise ValueError("No dataset has been provided.")
 
             if self._rules == []:
                 raise ValueError(
-                    "No fields have been provided. Use the 'on_fields' method."
+                    "No fields have been provided. Use the 'on_fields' or the 'add_rules' method."
                 )
 
             if custom_keyset is not None:
                 self._pseudo_keyset = custom_keyset
 
             self._timeout = timeout
             match Pseudonymize.dataset:  # Differentiate between file and DataFrame
                 case File():
-                    return self._pseudonymize_file()
+                    return self._pseudonymize_dataframe(Pseudonymize.dataset)
                 case pl.DataFrame():
-                    return self._pseudonymize_field()
+                    return self._pseudonymize_field(Pseudonymize.dataset)
+                case HierarchicalDataFrame():
+                    return self._pseudonymize_dataframe(Pseudonymize.dataset.contents)
                 case _ as invalid_dataset:
                     raise ValueError(
                         f"Unsupported data type: {type(invalid_dataset)}. Should only be DataFrame or file-like type."
                     )
 
-        def _pseudonymize_file(self) -> Result:
-            """Pseudonymize the entire file."""
-            # Need to type-cast explicitly. We know that Pseudonymize.dataset is a "File" if we reach this method.
-            file = t.cast(File, Pseudonymize.dataset)
-
+        def _pseudonymize_dataframe(self, dataframe: File | pl.DataFrame) -> Result:
+            """Pseudonymize the entire dataframe."""
             pseudonymize_request = PseudonymizeFileRequest(
                 pseudo_config=PseudoConfig(
                     rules=self._rules,
                     keysets=KeyWrapper(self._pseudo_keyset).keyset_list(),
                 ),
                 target_content_type=Mimetypes.JSON,
                 target_uri=None,
                 compression=None,
             )
 
-            pseudo_response: PseudoFileResponse = pseudo_operation_file(
-                file_handle=file.file_handle,
+            pseudo_response: PseudoFileResponse = pseudo_operation_dataset(
+                dataset_ref=dataframe,
                 pseudo_operation_request=pseudonymize_request,
-                input_content_type=file.content_type,
             )
 
             return Result(pseudo_response=pseudo_response)
 
-        def _pseudonymize_field(self) -> Result:
+        def _pseudonymize_field(self, dataframe: pl.DataFrame) -> Result:
             """Pseudonymizes the specified fields in the DataFrame using the provided pseudonymization function.
 
             The pseudonymization is performed in parallel. After the parallel processing is finished,
             the pseudonymized fields replace the original fields in the DataFrame stored in `self._dataframe`.
 
             Returns:
                 Result: Containing the pseudonymized 'self._dataframe' and the associated metadata.
@@ -198,15 +206,14 @@
                     path="pseudonymize/field",
                     pseudo_field_request=request,
                     timeout=self._timeout,
                     pseudo_client=self._pseudo_client,
                 )
                 return field_name, data, metadata
 
-            dataframe = t.cast(pl.DataFrame, Pseudonymize.dataset)
             # Execute the pseudonymization API calls in parallel
             with ThreadPoolExecutor() as executor:
                 pseudonymized_field: dict[str, pl.Series] = {}
                 raw_metadata_fields: list[RawPseudoMetadata] = []
                 futures = [
                     executor.submit(
                         pseudonymize_field_runner,
@@ -219,61 +226,67 @@
                 # Wait for the futures to finish, then add each field to pseudonymized_field map
                 for future in as_completed(futures):
                     field_name, data, raw_metadata = future.result()
                     pseudonymized_field[field_name] = data
                     raw_metadata_fields.append(raw_metadata)
 
                 pseudonymized_df = pl.DataFrame(pseudonymized_field)
-                dataframe = dataframe.update(pseudonymized_df)
+                dataframe = dataframe.update(pseudonymized_df, include_nulls=True)
             return Result(
                 pseudo_response=PseudoFieldResponse(
                     data=dataframe, raw_metadata=raw_metadata_fields
                 )
             )
 
     class _PseudoFuncSelector:
         def __init__(
-            self, fields: list[str], rules: Optional[list[PseudoRule]] = None
+            self, fields: list[str], rules: list[PseudoRule] | None = None
         ) -> None:
             self._fields = fields
             self._existing_rules = [] if rules is None else rules
 
         def with_stable_id(
             self,
-            sid_snapshot_date: Optional[str | date] = None,
-            custom_key: Optional[PredefinedKeys | str] = None,
+            sid_snapshot_date: str | date | None = None,
+            custom_key: PredefinedKeys | str | None = None,
+            failure_strategy: MapFailureStrategy | None = None,
         ) -> "Pseudonymize._Pseudonymizer":
             """Map the selected fields to Stable ID, then pseudonymize with a PAPIS-compatible encryption.
 
             In other words, this is a compound operation that both: 1) maps FNR to stable ID 2) then encrypts the Stable IDs.
 
             Args:
                 sid_snapshot_date (Optional[str | date], optional): Date representing SID-catalogue version to use.
                     Latest if unspecified. Format: YYYY-MM-DD
                 custom_key (Optional[PredefinedKeys | str], optional): Override the key to use for pseudonymization.
                     Must be one of the keys defined in PredefinedKeys. If not defined, uses the default key for this function (papis-common-key-1)
+                failure_strategy (Optional[MapFailureStrategy], optional): defines how to handle mapping failures
 
             Returns:
                 Self: The object configured to be mapped to stable ID
             """
             kwargs = (
                 MapSidKeywordArgs(
                     key_id=custom_key,
                     snapshot_date=convert_to_date(sid_snapshot_date),
+                    failure_strategy=failure_strategy,
                 )
                 if custom_key
-                else MapSidKeywordArgs(snapshot_date=convert_to_date(sid_snapshot_date))
+                else MapSidKeywordArgs(
+                    snapshot_date=convert_to_date(sid_snapshot_date),
+                    failure_strategy=failure_strategy,
+                )
             )
             function = PseudoFunction(
                 function_type=PseudoFunctionTypes.MAP_SID, kwargs=kwargs
             )
             return self._rule_constructor(function)
 
         def with_default_encryption(
-            self, custom_key: Optional[PredefinedKeys | str] = None
+            self, custom_key: PredefinedKeys | str | None = None
         ) -> "Pseudonymize._Pseudonymizer":
             """Pseudonymize the selected fields with the default encryption algorithm (DAEAD).
 
             Args:
                 custom_key (Optional[PredefinedKeys | str], optional): Override the key to use for pseudonymization.
                     Must be one of the keys defined in PredefinedKeys. If not defined, uses the default key for this function (ssb-common-key-1)
 
@@ -287,15 +300,15 @@
             )
             function = PseudoFunction(
                 function_type=PseudoFunctionTypes.DAEAD, kwargs=kwargs
             )
             return self._rule_constructor(function)
 
         def with_papis_compatible_encryption(
-            self, custom_key: Optional[PredefinedKeys | str] = None
+            self, custom_key: PredefinedKeys | str | None = None
         ) -> "Pseudonymize._Pseudonymizer":
             """Pseudonymize the selected fields with a PAPIS-compatible encryption algorithm (FF31).
 
             Args:
                 custom_key (Optional[PredefinedKeys | str], optional): Override the key to use for pseudonymization.
                     Must be one of the keys defined in PredefinedKeys. If not defined, uses the default key for this function (papis-common-key-1)
```

### Comparing `dapla_toolbelt_pseudo-1.6.0/src/dapla_pseudo/v1/pseudo_commons.py` & `dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/pseudo_commons.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         DefaultCredentialsError: If the provided dataset is a GCS path and no Google credentials are found
         ValueError: If the provided dataset is not of a supported type
         FileInvalidError: If the file is empty
 
     Returns:
         tuple[BinaryFileDecl, Mimetypes]: A tuple of (file handle, content type)
     """
-    file_handle: t.Optional[BinaryFileDecl] = None
+    file_handle: BinaryFileDecl | None = None
     match dataset:
         case str() | Path():
             # File path
             if str(dataset).startswith("gs://"):
                 try:
                     file_handle = FileClient().gcs_open(str(dataset), mode="rb")
                 except OSError as err:
@@ -128,21 +128,28 @@
             f"The provided input format '{file_format}' is not supported from file."
         ) from None
 
     return content_type
 
 
 @dataclass
+class HierarchicalDataFrame:
+    """HierarchicalDataset holds a hierarchical dataframe."""
+
+    contents: pl.DataFrame
+
+
+@dataclass
 class RawPseudoMetadata:
     """RawPseudoMetadata holds the raw metadata obtained from Pseudo Service."""
 
     logs: list[str]
     metrics: list[str]
     datadoc: list[dict[str, t.Any]]
-    field_name: t.Optional[str] = None
+    field_name: str | None = None
 
 
 @dataclass
 class PseudoFieldResponse:
     """PseudoFileResponse holds the data and metadata from a Pseudo Service field response."""
 
     data: pl.DataFrame
@@ -156,55 +163,68 @@
     data: list[dict[str, t.Any]]
     raw_metadata: RawPseudoMetadata
     content_type: Mimetypes
     file_name: str
     streamed: bool = True
 
 
-def pseudo_operation_file(
-    file_handle: t.BinaryIO,
+def pseudo_operation_dataset(
+    dataset_ref: File | pl.DataFrame,
     pseudo_operation_request: (
         PseudonymizeFileRequest | DepseudonymizeFileRequest | RepseudonymizeFileRequest
     ),
-    input_content_type: Mimetypes,
 ) -> PseudoFileResponse:
-    """Makes pseudonymization API calls for a file and returns the pseudonymized data and metadata.
+    """Calls pseudonymization API for an entire dataset (file handle or dataframe) and returns the pseudonymized data and metadata.
 
     Args:
-        file_handle: A file handle repreresenting the data to be pseudonymized
+        dataset_ref: A file handle or a dataframe representing the data to be pseudonymized
         pseudo_operation_request: An object representing the data and how it should be pseudonymized
-        input_content_type: A supported Mimetype for the file.
 
     Returns:
         PseudoFileResponse: An object representing the response from the Pseudo Service.
     """
     request_spec: FileSpecDecl = (
         None,
         pseudo_operation_request.to_json(),
         str(Mimetypes.JSON),
     )
+    file_name: str
+    data_spec: FileSpecDecl
 
-    file_name = _extract_name(
-        file_handle=file_handle, input_content_type=input_content_type
-    )
-
-    data_spec: FileSpecDecl = (
-        file_name,
-        file_handle,
-        str(pseudo_operation_request.target_content_type),
-    )
-
-    response = _client()._post_to_file_endpoint(
-        path=PseudoClient.pseudo_op_to_endpoint[type(pseudo_operation_request)],
-        request_spec=request_spec,
-        data_spec=data_spec,
-        stream=True,
-    )
-
-    file_handle.close()
+    if type(dataset_ref) is pl.DataFrame:
+        file_name = "data.json"
+        data_spec = (
+            file_name,
+            json.dumps(dataset_ref.to_dicts()),
+            str(pseudo_operation_request.target_content_type),
+        )
+        response = _client()._post_to_file_endpoint(
+            path=PseudoClient.pseudo_op_to_endpoint[type(pseudo_operation_request)],
+            request_spec=request_spec,
+            data_spec=data_spec,
+            stream=False,
+        )
+    else:
+        file = t.cast(File, dataset_ref)
+        with file.file_handle as file_handle:
+            file_name = _extract_name(
+                file_handle=file_handle, input_content_type=file.content_type
+            )
+            data_spec = (
+                file_name,
+                file_handle,
+                str(pseudo_operation_request.target_content_type),
+            )
+            # Post to file endpoint must be within the 'with' block to keep the file_handle open
+            response = _client()._post_to_file_endpoint(
+                path=PseudoClient.pseudo_op_to_endpoint[type(pseudo_operation_request)],
+                request_spec=request_spec,
+                data_spec=data_spec,
+                stream=True,
+            )
 
     payload = json.loads(response.content.decode("utf-8"))
     pseudo_data = payload["data"]
     metadata = RawPseudoMetadata(
         logs=payload["logs"],
         metrics=payload["metrics"],
         datadoc=payload["datadoc_metadata"]["pseudo_variables"],
```

### Comparing `dapla_toolbelt_pseudo-1.6.0/src/dapla_pseudo/v1/repseudo.py` & `dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/repseudo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Builder for submitting a pseudonymization request."""
 
 import os
 import typing as t
 from concurrent.futures import ThreadPoolExecutor
 from concurrent.futures import as_completed
 from datetime import date
-from typing import Optional
 
 import pandas as pd
 import polars as pl
 
 from dapla_pseudo.constants import TIMEOUT_DEFAULT
 from dapla_pseudo.constants import Env
 from dapla_pseudo.constants import PredefinedKeys
@@ -25,15 +24,15 @@
 from dapla_pseudo.v1.baseclass import _RuleConstructor
 from dapla_pseudo.v1.client import PseudoClient
 from dapla_pseudo.v1.pseudo_commons import File
 from dapla_pseudo.v1.pseudo_commons import PseudoFieldResponse
 from dapla_pseudo.v1.pseudo_commons import PseudoFileResponse
 from dapla_pseudo.v1.pseudo_commons import RawPseudoMetadata
 from dapla_pseudo.v1.pseudo_commons import get_file_data_from_dataset
-from dapla_pseudo.v1.pseudo_commons import pseudo_operation_file
+from dapla_pseudo.v1.pseudo_commons import pseudo_operation_dataset
 from dapla_pseudo.v1.pseudo_commons import pseudonymize_operation_field
 from dapla_pseudo.v1.result import Result
 
 
 class Repseudonymize:
     """Starting point for pseudonymization of datasets.
 
@@ -86,16 +85,16 @@
         """Select one or multiple fields to be pseudonymized."""
 
         source_rules: t.ClassVar[list[PseudoRule]] = []
         target_rules: t.ClassVar[list[PseudoRule]] = []
 
         def __init__(
             self,
-            source_rules: t.Optional[list[PseudoRule]] = None,
-            target_rules: t.Optional[list[PseudoRule]] = None,
+            source_rules: list[PseudoRule] | None = None,
+            target_rules: list[PseudoRule] | None = None,
         ) -> None:
             """Initialize the class."""
             if source_rules is None or target_rules is None:
                 # Because the "source_rules" and "target_rules" are static class variables,
                 # we need to reset the lists when the first call to "_Repseudonymizer" is made.
                 # This is because if we were to use the base class "Repseudonymize" twice in the same file,
                 # the lists of rules would persist across runs.
@@ -103,32 +102,32 @@
                 # "_RepseudoFuncSelectorSource" and "_RepseudoFuncSelectorTarget", which would hurt readability
                 Repseudonymize._Repseudonymizer.source_rules = []
                 Repseudonymize._Repseudonymizer.target_rules = []
             else:
                 Repseudonymize._Repseudonymizer.source_rules.extend(source_rules)
                 Repseudonymize._Repseudonymizer.target_rules.extend(target_rules)
 
-            self._source_pseudo_keyset: Optional[PseudoKeyset | str] = None
-            self._target_pseudo_keyset: Optional[PseudoKeyset | str] = None
+            self._source_pseudo_keyset: PseudoKeyset | str | None = None
+            self._target_pseudo_keyset: PseudoKeyset | str | None = None
             self._timeout: int
             self._pseudo_client: PseudoClient = PseudoClient(
                 pseudo_service_url=os.getenv(Env.PSEUDO_SERVICE_URL),
                 auth_token=os.getenv(Env.PSEUDO_SERVICE_AUTH_TOKEN),
             )
 
         def on_fields(
             self, *fields: str
         ) -> "Repseudonymize._RepseudoFuncSelectorSource":
             """Specify one or multiple fields to be pseudonymized."""
             return Repseudonymize._RepseudoFuncSelectorSource(list(fields))
 
         def run(
             self,
-            custom_source_keyset: Optional[PseudoKeyset | str] = None,
-            custom_target_keyset: Optional[PseudoKeyset | str] = None,
+            custom_source_keyset: PseudoKeyset | str | None = None,
+            custom_target_keyset: PseudoKeyset | str | None = None,
             timeout: int = TIMEOUT_DEFAULT,
         ) -> Result:
             """Pseudonymize the dataset.
 
             Args:
                 custom_source_keyset (PseudoKeyset, optional): The source pseudonymization keyset to use. Defaults to None.
                 custom_target_keyset (PseudoKeyset, optional): The target pseudonymization keyset to use. Defaults to None.
@@ -183,18 +182,17 @@
                     keysets=KeyWrapper(self._target_pseudo_keyset).keyset_list(),
                 ),
                 target_content_type=Mimetypes.JSON,
                 target_uri=None,
                 compression=None,
             )
 
-            pseudo_response: PseudoFileResponse = pseudo_operation_file(
-                file_handle=file.file_handle,
+            pseudo_response: PseudoFileResponse = pseudo_operation_dataset(
+                dataset_ref=file,
                 pseudo_operation_request=pseudonymize_request,
-                input_content_type=file.content_type,
             )
 
             return Result(pseudo_response=pseudo_response)
 
         def _repseudonymize_field(self) -> Result:
             """Pseudonymizes the specified fields in the DataFrame using the provided pseudonymization function.
 
@@ -248,15 +246,15 @@
                         repseudonymize_field_runner,
                         source_rule.pattern,
                         dataframe[source_rule.pattern],
                         source_rule.func,
                         target_rule.func,
                     )
                     for (source_rule, target_rule) in zip(
-                        self.source_rules, self.target_rules
+                        self.source_rules, self.target_rules, strict=False
                     )
                 ]
                 # Wait for the futures to finish, then add each field to pseudonymized_field map
                 for future in as_completed(futures):
                     field_name, data, raw_metadata = future.result()
                     pseudonymized_field[field_name] = data
                     raw_metadata_fields.append(raw_metadata)
@@ -266,27 +264,27 @@
             return Result(
                 pseudo_response=PseudoFieldResponse(
                     data=dataframe, raw_metadata=raw_metadata_fields
                 )
             )
 
     class _RepseudoFuncSelectorSource(_RuleConstructor):
-        def __init__(self, fields: list[str]):
+        def __init__(self, fields: list[str]) -> None:
             dataset_type: t.Literal["dataframe", "file"] = (
                 "dataframe"
                 if isinstance(Repseudonymize.dataset, pl.DataFrame)
                 else "file"
             )
             self.fields = fields
             super().__init__(fields, dataset_type)
 
         def from_stable_id(
             self,
-            sid_snapshot_date: t.Optional[str | date] = None,
-            custom_key: t.Optional[PredefinedKeys | str] = None,
+            sid_snapshot_date: str | date | None = None,
+            custom_key: PredefinedKeys | str | None = None,
         ) -> "Repseudonymize._RepseudoFuncSelectorTarget":
             """Claim that the selected fields were mapped to Stable ID, then pseudonymized with PAPIS-compatible encryption.
 
             Args:
                 sid_snapshot_date (Optional[str | date], optional): Date representing SID-catalogue version that was used.
                     Latest if unspecified. Format: YYYY-MM-DD
                 custom_key (Optional[PredefinedKeys | str], optional): Override the key to use for pseudonymization.
@@ -297,30 +295,30 @@
             """
             rules = super()._map_to_stable_id_and_pseudonymize(
                 sid_snapshot_date, custom_key
             )
             return Repseudonymize._RepseudoFuncSelectorTarget(self.fields, rules)
 
         def from_default_encryption(
-            self, custom_key: t.Optional[PredefinedKeys | str] = None
+            self, custom_key: PredefinedKeys | str | None = None
         ) -> "Repseudonymize._RepseudoFuncSelectorTarget":
             """Claim that the selected fields were pseudonymized with default encryption.
 
             Args:
                 custom_key (Optional[PredefinedKeys | str], optional): Override the key to use for pseudonymization.
                     Must be one of the keys defined in PredefinedKeys. If not defined, uses the default key for this function (papis-common-key-1)
 
             Returns:
                 An object with methods to choose how the field should be pseudonymized.
             """
             rules = super()._with_daead_encryption(custom_key)
             return Repseudonymize._RepseudoFuncSelectorTarget(self.fields, rules)
 
         def from_papis_compatible_encryption(
-            self, custom_key: t.Optional[PredefinedKeys | str] = None
+            self, custom_key: PredefinedKeys | str | None = None
         ) -> "Repseudonymize._RepseudoFuncSelectorTarget":
             """Claim that the selected fields were pseudonymized with PAPIS-compatible encryption.
 
             Args:
                 custom_key (Optional[PredefinedKeys | str], optional): Override the key to use for pseudonymization.
                     Must be one of the keys defined in PredefinedKeys. If not defined, uses the default key for this function (papis-common-key-1)
 
@@ -334,28 +332,28 @@
             self, function: PseudoFunction
         ) -> "Repseudonymize._RepseudoFuncSelectorTarget":
             """Claim that the selected fields were pseudonymized with a custom, specified Pseudo Function."""
             rules = super()._with_custom_function(function)
             return Repseudonymize._RepseudoFuncSelectorTarget(self.fields, rules)
 
     class _RepseudoFuncSelectorTarget(_RuleConstructor):
-        def __init__(self, fields: list[str], source_rules: list[PseudoRule]):
+        def __init__(self, fields: list[str], source_rules: list[PseudoRule]) -> None:
             self.source_rules = source_rules
 
             dataset_type: t.Literal["dataframe", "file"] = (
                 "dataframe"
                 if isinstance(Repseudonymize.dataset, pl.DataFrame)
                 else "file"
             )
             super().__init__(fields, dataset_type)
 
         def to_stable_id(
             self,
-            sid_snapshot_date: t.Optional[str | date] = None,
-            custom_key: t.Optional[PredefinedKeys | str] = None,
+            sid_snapshot_date: str | date | None = None,
+            custom_key: PredefinedKeys | str | None = None,
         ) -> "Repseudonymize._Repseudonymizer":
             """Map the selected fields to Stable ID, then pseudonymize with a PAPIS-compatible encryption.
 
             In other words, this is a compound operation that both: 1) maps FNR to stable ID 2) then encrypts the Stable IDs.
 
             Args:
                 sid_snapshot_date (Optional[str | date], optional): Date representing SID-catalogue version to use.
@@ -368,30 +366,30 @@
             """
             rules = super()._map_to_stable_id_and_pseudonymize(
                 sid_snapshot_date, custom_key
             )
             return Repseudonymize._Repseudonymizer(self.source_rules, rules)
 
         def to_default_encryption(
-            self, custom_key: t.Optional[PredefinedKeys | str] = None
+            self, custom_key: PredefinedKeys | str | None = None
         ) -> "Repseudonymize._Repseudonymizer":
             """Pseudonymize the selected fields with the default encryption algorithm (DAEAD).
 
             Args:
                 custom_key (Optional[PredefinedKeys | str], optional): Override the key to use for pseudonymization.
                     Must be one of the keys defined in PredefinedKeys. If not defined, uses the default key for this function (ssb-common-key-1)
 
             Returns:
                 Self: The object configured to be mapped to stable ID
             """
             rules = super()._with_daead_encryption(custom_key)
             return Repseudonymize._Repseudonymizer(self.source_rules, rules)
 
         def to_papis_compatible_encryption(
-            self, custom_key: t.Optional[PredefinedKeys | str] = None
+            self, custom_key: PredefinedKeys | str | None = None
         ) -> "Repseudonymize._Repseudonymizer":
             """Pseudonymize the selected fields with a PAPIS-compatible encryption algorithm (FF31).
 
             Args:
                 custom_key (Optional[PredefinedKeys | str], optional): Override the key to use for pseudonymization.
                     Must be one of the keys defined in PredefinedKeys. If not defined, uses the default key for this function (papis-common-key-1)
```

### Comparing `dapla_toolbelt_pseudo-1.6.0/src/dapla_pseudo/v1/result.py` & `dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/result.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,22 +63,21 @@
                 data, file_metadata, _content_type, file_name, _streamed
             ):
                 self._pseudo_data = data
                 self._metadata[file_name] = {
                     "logs": file_metadata.logs,
                     "metrics": file_metadata.metrics,
                 }
-                pseudo_variable = self._datadoc_from_raw_metadata_fields(
-                    file_metadata.datadoc
+                pseudo_variables = list(
+                    PseudoVariable.model_validate(item)
+                    for item in file_metadata.datadoc
                 )
                 self._datadoc = MetadataContainer(
                     pseudonymization=PseudonymizationMetadata(
-                        pseudo_variables=(
-                            [pseudo_variable] if pseudo_variable is not None else []
-                        )
+                        pseudo_variables=pseudo_variables
                     )
                 )
 
     def to_polars(self, **kwargs: t.Any) -> pl.DataFrame:
         """Output pseudonymized data as a Polars DataFrame.
 
         Args:
@@ -193,13 +192,13 @@
             str: A JSON-formattted string representing the datadoc metadata.
         """
         return self._datadoc.model_dump_json()
 
     def _datadoc_from_raw_metadata_fields(
         self,
         raw_metadata: list[dict[str, Any]],
-    ) -> t.Optional[PseudoVariable]:
+    ) -> PseudoVariable | None:
         if len(raw_metadata) == 0:
             return None
         elif len(raw_metadata) > 1:
             print(f"Unexpected length of metadata: {len(raw_metadata)}")
         return PseudoVariable.model_validate(raw_metadata[0])
```

### Comparing `dapla_toolbelt_pseudo-1.6.0/src/dapla_pseudo/v1/supported_file_format.py` & `dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/supported_file_format.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.6.0/src/dapla_pseudo/v1/validation.py` & `dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/validation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Builder for submitting a validation request."""
 
 import json
 from collections.abc import Sequence
 from datetime import date
 from pathlib import Path
 from typing import Any
-from typing import Optional
 
 import pandas as pd
 import polars as pl
 import requests
 
 from dapla_pseudo.utils import convert_to_date
 from dapla_pseudo.utils import get_file_format_from_file_name
@@ -74,15 +73,15 @@
         return Validator._FieldSelector(
             read_to_polars_df(file_format, file_path, **kwargs)
         )
 
     class _FieldSelector:
         """Select a field to be validated."""
 
-        def __init__(self, dataframe: pd.DataFrame | pl.DataFrame):
+        def __init__(self, dataframe: pd.DataFrame | pl.DataFrame) -> None:
             """Initialize the class."""
             self._dataframe: pl.DataFrame
             if isinstance(dataframe, pd.DataFrame):
                 self._dataframe = pl.from_pandas(dataframe)
             else:
                 self._dataframe = dataframe
 
@@ -98,15 +97,15 @@
             dataframe: pl.DataFrame,
             field: str,
         ) -> None:
             self._dataframe: pl.DataFrame = dataframe
             self._field: str = field
 
         def validate_map_to_stable_id(
-            self, sid_snapshot_date: Optional[str | date] = None
+            self, sid_snapshot_date: str | date | None = None
         ) -> Result:
             """Checks if all the selected fields can be mapped to a stable ID.
 
             Args:
                 sid_snapshot_date (Optional[str | date], optional): Date representing SID-catalogue version to use.
                     Latest if unspecified. Format: YYYY-MM-DD
```

### Comparing `dapla_toolbelt_pseudo-1.6.0/PKG-INFO` & `dapla_toolbelt_pseudo-1.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dapla-toolbelt-pseudo
-Version: 1.6.0
+Version: 1.7.0
 Summary: Pseudonymization extensions for Dapla
 Home-page: https://github.com/statisticsnorway/dapla-toolbelt-pseudo
 License: MIT
 Author: Dapla Developers
 Author-email: dapla-platform-developers@ssb.no
 Requires-Python: >=3.10,<3.13
 Classifier: Development Status :: 4 - Beta
@@ -105,14 +105,37 @@
 ```
 
 The default encryption algorithm is DAEAD (Deterministic Authenticated Encryption with Associated Data). However, if the
 field is a valid Norwegian personal identification number (fnr, dnr), the recommended way to pseudonymize is to use
 the function `with_stable_id()` to convert the identification number to a stable ID (SID) prior to pseudonymization.
 In that case, the pseudonymization algorithm is FPE (Format Preserving Encryption).
 
+> [!IMPORTANT]
+> FPE requires minimum two bytes/characters to perform encryption and minimum four bytes in case of Unicode.
+
+If a field cannot be converted using the function `with_stable_id()` the default behaviour is to use the original value
+as input to the FPE encryption function. However, this behaviour can be changed by supplying a `failure_strategy` like
+this:
+
+```python
+from dapla_pseudo import Pseudonymize
+from dapla_pseudo.constants import MapFailureStrategy
+
+# Example: Single field sid mapping and pseudonymization (FPE), unmatching SIDs will return Null
+result_df = (
+    Pseudonymize.from_polars(df)
+    .on_fields("fnr")
+    .with_stable_id(failure_strategy=MapFailureStrategy.RETURN_NULL)
+    .run()
+    .to_polars()
+)
+```
+
+
+### Reading dataframes
 
 Note that you may also use a Pandas DataFrame as an input or output, by exchanging `from_polars` with `from_pandas`
 and `to_polars` with `to_pandas`. However, Pandas is much less performant, so take special care especially if your
 dataset is large.
 
 Example:
```

