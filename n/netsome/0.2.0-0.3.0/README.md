# Comparing `tmp/netsome-0.2.0.tar.gz` & `tmp/netsome-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netsome-0.2.0.tar", max compression
+gzip compressed data, was "netsome-0.3.0.tar", max compression
```

## Comparing `netsome-0.2.0.tar` & `netsome-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,22 @@
--rw-r--r--   0        0        0     1076 2024-03-27 09:32:36.724182 netsome-0.2.0/LICENSE
--rw-r--r--   0        0        0      216 2024-04-05 20:13:03.123602 netsome-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-03-27 19:13:03.131810 netsome-0.2.0/netsome/__init__.py
--rw-r--r--   0        0        0      254 2024-04-05 20:12:51.694562 netsome-0.2.0/netsome/constants.py
--rw-r--r--   0        0        0        0 2024-03-29 07:02:52.497218 netsome-0.2.0/netsome/types/__init__.py
--rw-r--r--   0        0        0     1606 2024-04-05 20:12:51.695230 netsome-0.2.0/netsome/types/bgp.py
--rw-r--r--   0        0        0     4041 2024-04-05 20:12:51.695776 netsome-0.2.0/netsome/types/ipv4.py
--rw-r--r--   0        0        0      429 2024-04-05 20:12:51.696340 netsome-0.2.0/netsome/types/vlans.py
--rw-r--r--   0        0        0        0 2024-03-29 07:03:11.197676 netsome-0.2.0/netsome/validators/__init__.py
--rw-r--r--   0        0        0      961 2024-04-05 20:12:51.697184 netsome-0.2.0/netsome/validators/bgp.py
--rw-r--r--   0        0        0     1838 2024-04-05 20:12:51.697727 netsome-0.2.0/netsome/validators/ipv4.py
--rw-r--r--   0        0        0      288 2024-03-29 07:09:10.484949 netsome-0.2.0/netsome/validators/vlans.py
--rw-r--r--   0        0        0     1017 2024-04-05 20:12:58.589978 netsome-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 netsome-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1286 2024-04-10 20:01:10.836837 netsome-0.3.0/LICENSE
+-rw-r--r--   0        0        0      288 2024-04-10 19:59:40.508871 netsome-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-03-27 19:13:03.131810 netsome-0.3.0/netsome/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 10:11:00.036571 netsome-0.3.0/netsome/_converters/__init__.py
+-rw-r--r--   0        0        0      940 2024-04-10 19:05:11.709525 netsome-0.3.0/netsome/_converters/bgp.py
+-rw-r--r--   0        0        0      321 2024-04-06 10:16:50.104431 netsome-0.3.0/netsome/_converters/ipv4.py
+-rw-r--r--   0        0        0      284 2024-04-10 19:05:11.712169 netsome-0.3.0/netsome/constants.py
+-rw-r--r--   0        0        0        0 2024-04-06 10:10:11.717546 netsome-0.3.0/netsome/pools/__init__.py
+-rw-r--r--   0        0        0      125 2024-04-10 19:12:45.783585 netsome-0.3.0/netsome/pools/bgp.py
+-rw-r--r--   0        0        0     1027 2024-04-10 19:12:45.779619 netsome-0.3.0/netsome/pools/ipv4.py
+-rw-r--r--   0        0        0     1409 2024-04-10 19:13:23.340144 netsome-0.3.0/netsome/pools/number.py
+-rw-r--r--   0        0        0      130 2024-04-10 19:13:24.877011 netsome-0.3.0/netsome/pools/vlans.py
+-rw-r--r--   0        0        0        0 2024-04-08 18:56:12.740789 netsome-0.3.0/netsome/types/__init__.py
+-rw-r--r--   0        0        0     2191 2024-04-10 19:16:53.282722 netsome-0.3.0/netsome/types/bgp.py
+-rw-r--r--   0        0        0     4014 2024-04-08 19:07:29.121545 netsome-0.3.0/netsome/types/ipv4.py
+-rw-r--r--   0        0        0      848 2024-04-10 19:16:35.671355 netsome-0.3.0/netsome/types/vlans.py
+-rw-r--r--   0        0        0        0 2024-04-06 10:10:11.723380 netsome-0.3.0/netsome/validators/__init__.py
+-rw-r--r--   0        0        0     1654 2024-04-10 19:05:11.715896 netsome-0.3.0/netsome/validators/bgp.py
+-rw-r--r--   0        0        0     2024 2024-04-06 10:20:26.966511 netsome-0.3.0/netsome/validators/ipv4.py
+-rw-r--r--   0        0        0      289 2024-04-06 10:14:06.090402 netsome-0.3.0/netsome/validators/vlans.py
+-rw-r--r--   0        0        0     1246 2024-04-10 20:01:34.998323 netsome-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1115 1970-01-01 00:00:00.000000 netsome-0.3.0/PKG-INFO
```

### Comparing `netsome-0.2.0/LICENSE` & `netsome-0.3.0/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-MIT License
-
 Copyright (c) 2024 Dmitriy Kudryavtsev
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
@@ -15,7 +13,11 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
+
+Except as contained in this notice, the name(s) of the above copyright holders
+shall not be used in advertising or otherwise to promote the sale, use or other
+dealings in this Software without prior written authorization.
```

### Comparing `netsome-0.2.0/netsome/types/ipv4.py` & `netsome-0.3.0/netsome/types/ipv4.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,76 +1,70 @@
 import functools
 import typing as t
 
 from netsome import constants as c
+from netsome._converters import ipv4 as converters
 from netsome.validators import ipv4 as validators
 
 
-def _address_to_int(string: str) -> int:
-    octets = map(int, string.split(c.DOT, maxsplit=3))
-    return int.from_bytes(octets, byteorder="big")
-
-
-def _int_to_address(number: int) -> str:
-    octets = map(str, number.to_bytes(length=4, byteorder="big"))
-    return c.DOT.join(octets)
-
-
 class IPv4Address:
     def __init__(self, address: str) -> None:
         validators.validate_address_str(address)
-        self._addr = _address_to_int(address)
+        self._addr = converters.address_to_int(address)
 
     @classmethod
     def from_int(cls, number: int) -> "IPv4Address":
         validators.validate_address_int(number)
-        return cls(_int_to_address(number))
+        return cls(converters.int_to_address(number))
 
     @functools.cached_property
     def address(self) -> str:
-        return _int_to_address(self._addr)
+        return converters.int_to_address(self._addr)
 
     def __int__(self) -> int:
         return self._addr
 
     def __repr__(self) -> str:
         return f'{self.__class__.__name__}("{self.address}")'
 
+    def __hash__(self) -> int:
+        return hash(self._addr)
 
-def _validate_network_int(address: int, prefixlen: int):
-    netmask = c.IPV4_MAX ^ (c.IPV4_MAX >> prefixlen)
-    if address & netmask != address:
-        raise ValueError("host bits set")
+    def __lt__(self, other: t.Any) -> bool:
+        return isinstance(other, self.__class__) and self._addr < other._addr
+
+    def __eq__(self, other: t.Any) -> bool:
+        return isinstance(other, self.__class__) and self._addr == other._addr
 
 
 class IPv4Network:
     def __init__(self, network: str) -> None:
         address, prefixlen = network.split(c.SLASH, maxsplit=1)
         validators.validate_address_str(address)
         validators.validate_prefixlen_str(prefixlen)
-
-        _validate_network_int(_address_to_int(address), int(prefixlen))
+        validators.validate_network_int(
+            converters.address_to_int(address), int(prefixlen)
+        )
 
         self._prefixlen = int(prefixlen)
         self._netaddr = IPv4Address(address)
         self._netmask = IPv4Address.from_int(
             c.IPV4_MAX ^ (c.IPV4_MAX >> self._prefixlen)
         )
 
     def __repr__(self) -> str:
         return f'{self.__class__.__name__}("{self.address}")'
 
     @classmethod
     def from_int(cls, int_address: int, prefixlen: int) -> "IPv4Network":
         validators.validate_address_int(int_address)
         validators.validate_prefixlen_int(prefixlen)
+        validators.validate_network_int(int_address, prefixlen)
 
-        _validate_network_int(int_address, prefixlen)
-
-        address = f"{_int_to_address(int_address)}{c.SLASH}{prefixlen}"
+        address = f"{converters.int_to_address(int_address)}{c.SLASH}{prefixlen}"
         return cls(address)
 
     @property
     def prefixlen(self) -> int:
         return self._prefixlen
 
     @property
```

### Comparing `netsome-0.2.0/netsome/validators/bgp.py` & `netsome-0.3.0/netsome/validators/bgp.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,53 @@
 from netsome import constants as c
-from netsome.converters import bgp as converters
+from netsome._converters import bgp as converters
 
 
 def validate_asplain(number: int) -> None:
     if not isinstance(number, int):
         raise TypeError("Invalid asplain type, must be int")
 
-    if number < c.ZERO or number > c.ASN_MAX:
+    if not (c.ZERO <= number <= c.ASN_MAX):
         raise ValueError(
             f"Invalid asplain number. Must be in range {c.ZERO}-{c.ASN_MAX}"
         )
 
 
 def validate_asdotplus(string: str) -> None:
     if not isinstance(string, str):
         raise TypeError("Invalid asdot+ type, must be str")
 
     if c.DOT not in string:
         raise ValueError("Invalid asdot+ format, must be HIGH_ORDER.LOW_ORDER")
 
-    # FIXME
     validate_asplain(converters.asdotplus_to_asplain(string))
 
 
 def validate_asdot(string: str) -> None:
     if not isinstance(string, str):
         raise TypeError("Invalid asdot type, must be str")
 
     if c.DOT in string:
         validate_asdotplus(string)
         return
 
     validate_asplain(int(string))
+
+
+def validate_community(string: str) -> None:
+    if not isinstance(string, str):
+        raise TypeError("Invalid Community type, must be str")
+
+    if string.count(c.COLON) != 1:
+        raise ValueError(
+            "Invalid Community format, delimiter must be colon – ASN:VALUE"
+        )
+
+    asn, value = map(int, string.split(c.COLON, maxsplit=1))
+    if not (c.ZERO <= asn <= c.ASN_ORDER_MAX):
+        raise ValueError(
+            f"Invalid ASN in Community. Must be in range {c.ZERO}-{c.ASN_ORDER_MAX}"
+        )
+    if not (c.ZERO <= value <= c.ASN_ORDER_MAX):
+        raise ValueError(
+            f"Invalid VALUE number in Community. Must be in range {c.ZERO}-{c.ASN_ORDER_MAX }"
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `netsome-0.2.0/netsome/validators/ipv4.py` & `netsome-0.3.0/netsome/validators/ipv4.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         validate_octet_str(octet)
 
 
 def validate_address_int(number: int) -> None:
     if not isinstance(number, int):
         raise TypeError("Invalid type")
 
-    if number < c.ZERO or number > c.IPV4_MAX:
+    if not (c.ZERO <= number <= c.IPV4_MAX):
         raise ValueError("Invalid value")
 
 
 def validate_octet_str(string: str) -> None:
     if not isinstance(string, str):
         raise TypeError("Invalid type")
 
@@ -34,15 +34,15 @@
     validate_octet_int(int(string))
 
 
 def validate_octet_int(number: int) -> None:
     if not isinstance(number, int):
         raise TypeError("Invalid type")
 
-    if number < c.ZERO or number > c.IPV4_OCTET_MAX:
+    if not (c.ZERO <= number <= c.IPV4_OCTET_MAX):
         raise ValueError("Invalid value")
 
 
 def validate_prefixlen_str(string: str) -> None:
     if not isinstance(string, str):
         raise TypeError()
 
@@ -60,7 +60,13 @@
     max_len: int = c.IPV4_PREFIXLEN_MAX,
 ) -> None:
     if not isinstance(number, int):
         raise TypeError()
 
     if not (min_len <= number <= max_len):
         raise ValueError()
+
+
+def validate_network_int(address: int, prefixlen: int):
+    netmask = c.IPV4_MAX ^ (c.IPV4_MAX >> prefixlen)
+    if address & netmask != address:
+        raise ValueError("host bits set")
```

### Comparing `netsome-0.2.0/pyproject.toml` & `netsome-0.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -11,31 +11,37 @@
   "poetry run autoflake --in-place --verbose --recursive $DIRS",
   "poetry run black $DIRS",
   "poetry run isort $DIRS",
   "poetry run toml-sort --in-place --all pyproject.toml"
 ]
 
 [tool.poe.tasks.tests]
-cmd = "poetry run pytest -vvv"
+cmd = "poetry run pytest -vvv --cov=. --cov-report html"
 
 [tool.poetry]
 authors = ["kuderr <dakudryavcev@gmail.com>"]
 classifiers = [
   "Development Status :: 1 - Planning",
   "Topic :: Software Development :: Libraries",
   "Topic :: System :: Networking"
 ]
-description = "The one and only library to make your network business code handsome"
+description = "The one and only library to make your network code handsome"
 keywords = ["library", "network"]
-license = "MIT License"
+license = "X11 License Distribution Modification Variant"
 name = "netsome"
 readme = "README.md"
 repository = "https://github.com/kuderr/netsome"
-version = "0.2.0"
+version = "0.3.0"
 
 [tool.poetry.dependencies]
 python = "^3.12"
+sortedcontainers = "^2.4.0"
 
 [tool.poetry.group.dev.dependencies]
 poethepoet = "^0.25.0"
 pytest = "^8.1.1"
+pytest-cov = "^5.0.0"
 toml-sort = "^0.23.1"
+
+[tool.poetry.urls]
+"Bug Tracker" = "https://github.com/kuderr/netsome/issues"
+"Homepage" = "https://github.com/kuderr/netsome"
```

