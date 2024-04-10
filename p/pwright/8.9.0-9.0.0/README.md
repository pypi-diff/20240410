# Comparing `tmp/pwright-8.9.0.tar.gz` & `tmp/pwright-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwright-8.9.0.tar", last modified: Mon Apr  8 19:31:10 2024, max compression
+gzip compressed data, was "pwright-9.0.0.tar", last modified: Wed Apr 10 14:54:56 2024, max compression
```

## Comparing `pwright-8.9.0.tar` & `pwright-9.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1100 2024-04-08 19:31:10.609918 pwright-8.9.0/pyproject.toml
--rw-r--r--   0        0        0      104 2024-04-08 19:30:54.025931 pwright-8.9.0/src/pwright/__init__.py
--rw-r--r--   0        0        0       18 2024-04-08 19:30:54.025931 pwright-8.9.0/src/pwright/__version__.py
--rw-r--r--   0        0        0      260 2024-04-08 19:30:54.025931 pwright-8.9.0/src/pwright/_constants.py
--rw-r--r--   0        0        0      575 2024-04-08 19:30:54.025931 pwright-8.9.0/src/pwright/_utils.py
--rw-r--r--   0        0        0     1092 2024-04-08 19:30:54.025931 pwright-8.9.0/src/pwright/async_api/__init__.py
--rw-r--r--   0        0        0      619 2024-04-08 19:30:54.025931 pwright-8.9.0/src/pwright/async_api/_apis.py
--rw-r--r--   0        0        0     2029 2024-04-08 19:30:54.025931 pwright-8.9.0/src/pwright/async_api/_briefs.py
--rw-r--r--   0        0        0     4700 2024-04-08 19:30:54.025931 pwright-8.9.0/src/pwright/async_api/_cms.py
--rw-r--r--   0        0        0      608 2024-04-08 19:30:54.025931 pwright-8.9.0/src/pwright/async_api/_compatibilities.py
--rw-r--r--   0        0        0      879 2024-04-08 19:30:54.025931 pwright-8.9.0/src/pwright/async_api/utils.py
--rw-r--r--   0        0        0      933 2024-04-08 19:30:54.025931 pwright-8.9.0/src/pwright/sync_api/__init__.py
--rw-r--r--   0        0        0      608 2024-04-08 19:30:54.025931 pwright-8.9.0/src/pwright/sync_api/_apis.py
--rw-r--r--   0        0        0     1975 2024-04-08 19:30:54.025931 pwright-8.9.0/src/pwright/sync_api/_briefs.py
--rw-r--r--   0        0        0     4590 2024-04-08 19:30:54.025931 pwright-8.9.0/src/pwright/sync_api/_cms.py
--rw-r--r--   0        0        0      830 2024-04-08 19:30:54.025931 pwright-8.9.0/src/pwright/sync_api/utils.py
--rw-r--r--   0        0        0      394 2024-04-08 19:30:54.025931 pwright-8.9.0/src/pwright/typealiases.py
--rw-r--r--   0        0        0        0 2024-04-08 19:30:54.025931 pwright-8.9.0/tests/__init__.py
--rw-r--r--   0        0        0     1202 2024-04-08 19:30:54.025931 pwright-8.9.0/tests/test_apw.py
--rw-r--r--   0        0        0      970 2024-04-08 19:30:54.025931 pwright-8.9.0/tests/test_pw.py
--rw-r--r--   0        0        0      149 1970-01-01 00:00:00.000000 pwright-8.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-10 14:54:56.627755 pwright-9.0.0/pyproject.toml
+-rw-r--r--   0        0        0      104 2024-04-10 14:54:39.791647 pwright-9.0.0/src/pwright/__init__.py
+-rw-r--r--   0        0        0       18 2024-04-10 14:54:39.791647 pwright-9.0.0/src/pwright/__version__.py
+-rw-r--r--   0        0        0      260 2024-04-10 14:54:39.791647 pwright-9.0.0/src/pwright/_constants.py
+-rw-r--r--   0        0        0      575 2024-04-10 14:54:39.795647 pwright-9.0.0/src/pwright/_utils.py
+-rw-r--r--   0        0        0     1380 2024-04-10 14:54:39.795647 pwright-9.0.0/src/pwright/async_api/__init__.py
+-rw-r--r--   0        0        0      619 2024-04-10 14:54:39.795647 pwright-9.0.0/src/pwright/async_api/_apis.py
+-rw-r--r--   0        0        0     2029 2024-04-10 14:54:39.795647 pwright-9.0.0/src/pwright/async_api/_briefs.py
+-rw-r--r--   0        0        0     4700 2024-04-10 14:54:39.795647 pwright-9.0.0/src/pwright/async_api/_cms.py
+-rw-r--r--   0        0        0      608 2024-04-10 14:54:39.795647 pwright-9.0.0/src/pwright/async_api/_compatibilities.py
+-rw-r--r--   0        0        0      908 2024-04-10 14:54:39.795647 pwright-9.0.0/src/pwright/async_api/utils.py
+-rw-r--r--   0        0        0     1075 2024-04-10 14:54:39.795647 pwright-9.0.0/src/pwright/sync_api/__init__.py
+-rw-r--r--   0        0        0      608 2024-04-10 14:54:39.795647 pwright-9.0.0/src/pwright/sync_api/_apis.py
+-rw-r--r--   0        0        0     1975 2024-04-10 14:54:39.795647 pwright-9.0.0/src/pwright/sync_api/_briefs.py
+-rw-r--r--   0        0        0     4590 2024-04-10 14:54:39.795647 pwright-9.0.0/src/pwright/sync_api/_cms.py
+-rw-r--r--   0        0        0      860 2024-04-10 14:54:39.795647 pwright-9.0.0/src/pwright/sync_api/utils.py
+-rw-r--r--   0        0        0      484 2024-04-10 14:54:39.795647 pwright-9.0.0/src/pwright/typealiases.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:54:39.795647 pwright-9.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     1444 2024-04-10 14:54:39.795647 pwright-9.0.0/tests/test_apw.py
+-rw-r--r--   0        0        0     1196 2024-04-10 14:54:39.795647 pwright-9.0.0/tests/test_pw.py
+-rw-r--r--   0        0        0      108 1970-01-01 00:00:00.000000 pwright-9.0.0/PKG-INFO
```

### Comparing `pwright-8.9.0/pyproject.toml` & `pwright-9.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 [project]
 name = "pwright"
-version = "8.9.0"
+version = "9.0.0"
 requires-python = ">=3.8"
 dependencies = [
     "playwright>=1.34.0",
-    "typing-extensions>=4.11.0",
 ]
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `pwright-8.9.0/src/pwright/_utils.py` & `pwright-9.0.0/src/pwright/_utils.py`

 * *Files identical despite different names*

### Comparing `pwright-8.9.0/src/pwright/async_api/__init__.py` & `pwright-9.0.0/src/pwright/sync_api/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import sys
-
-from ..typealiases import AsyncGeneratorContextManager as AsyncGeneratorContextManager
+from ..typealiases import Generator as Generator
+from ..typealiases import GeneratorContextManager as GeneratorContextManager
+from ..typealiases import GeneratorContextManagerGenerator as GeneratorContextManagerGenerator
 from ._apis import Browser as Browser
 from ._apis import BrowserContext as BrowserContext
 from ._apis import Dialog as Dialog
 from ._apis import ElementHandle as ElementHandle
 from ._apis import Page as Page
 from ._apis import Playwright as Playwright
 from ._apis import Route as Route
@@ -13,18 +13,13 @@
 from ._briefs import pw_browser as pw_browser
 from ._briefs import pw_context as pw_context
 from ._briefs import pw_page as pw_page
 from ._cms import playwright_browser as playwright_browser
 from ._cms import playwright_context as playwright_context
 from ._cms import playwright_page as playwright_page
 from .utils import auto_renew as auto_renew
-from .utils import renewable as renewable
+from .utils import renewing as renewing
 from .utils import screenshot as screenshot
 
 
-GeneratorContextManager = AsyncGeneratorContextManager
 Eh = ElementHandle
 playwright = playwright
-
-
-if sys.version_info < (3, 10):
-    from ._compatibilities import anext as anext
```

### Comparing `pwright-8.9.0/src/pwright/async_api/_apis.py` & `pwright-9.0.0/src/pwright/async_api/_apis.py`

 * *Files identical despite different names*

### Comparing `pwright-8.9.0/src/pwright/async_api/_briefs.py` & `pwright-9.0.0/src/pwright/async_api/_briefs.py`

 * *Files identical despite different names*

### Comparing `pwright-8.9.0/src/pwright/async_api/_cms.py` & `pwright-9.0.0/src/pwright/async_api/_cms.py`

 * *Files identical despite different names*

### Comparing `pwright-8.9.0/src/pwright/async_api/_compatibilities.py` & `pwright-9.0.0/src/pwright/async_api/_compatibilities.py`

 * *Files identical despite different names*

### Comparing `pwright-8.9.0/src/pwright/async_api/utils.py` & `pwright-9.0.0/src/pwright/async_api/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 from contextlib import asynccontextmanager
 import logging
 from pathlib import Path
 import typing as t
 
 from .._utils import relative_to_cwd
+from ..typealiases import AsyncGeneratorContextManager
 from ._apis import Page
 
 
 logger = logging.getLogger(__name__)
 
 
 T = t.TypeVar('T')
 
 
 @asynccontextmanager
-async def auto_renew(
-    p: t.Callable[..., t.AsyncContextManager[T]], n: int
+async def renewing(
+    p: AsyncGeneratorContextManager[T], n: int
 ) -> t.AsyncGenerator[t.AsyncGenerator[T, None], None]:
-    yield renewable(p, n)
+    yield auto_renew(p, n)
 
 
-async def renewable(
-    p: t.Callable[..., t.AsyncContextManager[T]], n: int
-) -> t.AsyncGenerator[T, None]:
+async def auto_renew(p: AsyncGeneratorContextManager[T], n: int) -> t.AsyncGenerator[T, None]:
     while True:
         async with p() as y:
             for _ in range(n):
                 yield y
 
 
 async def screenshot(
```

### Comparing `pwright-8.9.0/src/pwright/sync_api/_apis.py` & `pwright-9.0.0/src/pwright/sync_api/_apis.py`

 * *Files identical despite different names*

### Comparing `pwright-8.9.0/src/pwright/sync_api/_briefs.py` & `pwright-9.0.0/src/pwright/sync_api/_briefs.py`

 * *Files identical despite different names*

### Comparing `pwright-8.9.0/src/pwright/sync_api/_cms.py` & `pwright-9.0.0/src/pwright/sync_api/_cms.py`

 * *Files identical despite different names*

### Comparing `pwright-8.9.0/src/pwright/sync_api/utils.py` & `pwright-9.0.0/src/pwright/sync_api/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from contextlib import contextmanager
 import logging
 from pathlib import Path
 import typing as t
 
 from .._utils import relative_to_cwd
+from ..typealiases import GeneratorContextManager
 from ._apis import Page
 
 
 logger = logging.getLogger(__name__)
 
 
 T = t.TypeVar('T')
 
 
 @contextmanager
-def auto_renew(
-    p: t.Callable[..., t.ContextManager[T]], n: int
+def renewing(
+    p: GeneratorContextManager[T], n: int
 ) -> t.Generator[t.Generator[T, None, None], None, None]:
-    yield renewable(p, n)
+    yield auto_renew(p, n)
 
 
-def renewable(p: t.Callable[..., t.ContextManager[T]], n: int) -> t.Generator[T, None, None]:
+def auto_renew(p: GeneratorContextManager[T], n: int) -> t.Generator[T, None, None]:
     while True:
         with p() as obj:
             for _ in range(n):
                 yield obj
 
 
 def screenshot(
```

### Comparing `pwright-8.9.0/tests/test_apw.py` & `pwright-9.0.0/tests/test_apw.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,54 @@
 import asyncio
 from contextlib import asynccontextmanager
 import sys
 import time
-import typing as t
 
-from pwright import apw
+from pwright import apw as pw
 
 
 if sys.version_info < (3, 10):
-    anext = apw.anext
+    anext = pw.anext
 
 
 def test_pw_page():
     async def get_title(*, url: str):
-        async with apw.pw_page() as page:
+        async with pw.pw_page() as page:
             await page.goto(url)
             title = await page.title()
             return title
 
     assert 'Playwright' in asyncio.run(get_title(url='https://playwright.dev/'))
 
 
 async def _test_renew(headed=True):
     @asynccontextmanager
     async def gen_page():
-        async with apw.pw_page(headed=headed) as page:
+        async with pw.pw_page(headed=headed) as page:
             yield page
 
-    async def run(gen: t.AsyncGenerator[apw.Page, None]):
+    gen_page_cm: pw.AsyncGeneratorContextManager[pw.Page] = gen_page
+
+    async def run(*, page_gen: pw.AsyncGenerator[pw.Page]):
         for _ in range(5):
-            page = await anext(gen)
+            page = await anext(page_gen)
             await page.goto('https://playwright.dev/')
             print(id(page))
             if 0:
                 time.sleep(0.2)
-        await gen.aclose()
+        await page_gen.aclose()
         if 0:
             await asyncio.sleep(30)
 
-    await run(apw.renewable(gen_page, 3))
-    async with apw.auto_renew(gen_page, 3) as agen:
-        await run(agen)
+    auto_renew_page_gen: pw.AsyncGenerator[pw.Page] = pw.auto_renew(gen_page_cm, 3)
+    await run(page_gen=auto_renew_page_gen)
+
+    renewing: pw.AsyncGeneratorContextManagerAsyncGenerator[pw.Page] = pw.renewing(gen_page_cm, 3)
+    async with renewing as agen:
+        await run(page_gen=agen)
 
 
 def test_renew():
     asyncio.run(_test_renew(headed=False))
 
 
 if __name__ == '__main__':
```

