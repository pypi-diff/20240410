# Comparing `tmp/pytest_databases-0.2.3.tar.gz` & `tmp/pytest_databases-0.2.4.tar.gz`

## Comparing `pytest_databases-0.2.3.tar` & `pytest_databases-0.2.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/.sourcery.yaml
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/CODEOWNERS
--rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/CONTRIBUTING.rst
--rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/Makefile
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/sonar-project.properties
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/.vscode/settings.json
--rw-r--r--   0        0        0     8877 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/requirements/requirements-dev.txt
--rw-r--r--   0        0        0     6540 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/requirements/requirements-docs.txt
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/requirements/requirements.txt
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/scripts/__init__.py
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/scripts/build_docs.py
--rwxr-xr-x   0        0        0      186 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/scripts/convert_docs.sh
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/src/pytest_databases/__init__.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/src/pytest_databases/__metadata__.py
--rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/src/pytest_databases/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/src/pytest_databases/py.typed
--rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/src/pytest_databases/docker/__init__.py
--rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/src/pytest_databases/docker/cockroachdb.py
--rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/src/pytest_databases/docker/docker-compose.yml
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/src/pytest_databases/docker/dragonfly.py
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/src/pytest_databases/docker/keydb.py
--rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/src/pytest_databases/docker/mariadb.py
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/src/pytest_databases/docker/mssql.py
--rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/src/pytest_databases/docker/mysql.py
--rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/src/pytest_databases/docker/oracle.py
--rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/src/pytest_databases/docker/postgres.py
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/src/pytest_databases/docker/redis.py
--rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/src/pytest_databases/docker/spanner.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/tests/__init__.py
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/tests/conftest.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/tests/docker/__init__.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/tests/docker/test_cockroachdb.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/tests/docker/test_dragonfly.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/tests/docker/test_keydb.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/tests/docker/test_mariadb.py
--rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/tests/docker/test_mssql.py
--rw-r--r--   0        0        0     4193 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/tests/docker/test_mysql.py
--rw-r--r--   0        0        0     3471 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/tests/docker/test_oracle.py
--rw-r--r--   0        0        0     6003 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/tests/docker/test_postgres.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/tests/docker/test_redis.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/tests/docker/test_spanner.py
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/LICENSE
--rw-r--r--   0        0        0    12148 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/README.md
--rw-r--r--   0        0        0    16950 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/pyproject.toml
--rw-r--r--   0        0        0    13954 2020-02-02 00:00:00.000000 pytest_databases-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/.sourcery.yaml
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/CODEOWNERS
+-rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/Makefile
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/sonar-project.properties
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/.vscode/settings.json
+-rw-r--r--   0        0        0     8877 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/requirements/requirements-dev.txt
+-rw-r--r--   0        0        0     6540 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/requirements/requirements-docs.txt
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/requirements/requirements.txt
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/scripts/__init__.py
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/scripts/build_docs.py
+-rwxr-xr-x   0        0        0      186 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/scripts/convert_docs.sh
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/src/pytest_databases/__init__.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/src/pytest_databases/__metadata__.py
+-rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/src/pytest_databases/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/src/pytest_databases/py.typed
+-rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/src/pytest_databases/docker/__init__.py
+-rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/src/pytest_databases/docker/cockroachdb.py
+-rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/src/pytest_databases/docker/docker-compose.yml
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/src/pytest_databases/docker/dragonfly.py
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/src/pytest_databases/docker/keydb.py
+-rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/src/pytest_databases/docker/mariadb.py
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/src/pytest_databases/docker/mssql.py
+-rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/src/pytest_databases/docker/mysql.py
+-rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/src/pytest_databases/docker/oracle.py
+-rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/src/pytest_databases/docker/postgres.py
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/src/pytest_databases/docker/redis.py
+-rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/src/pytest_databases/docker/spanner.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/tests/__init__.py
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/tests/conftest.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/tests/docker/__init__.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/tests/docker/test_cockroachdb.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/tests/docker/test_dragonfly.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/tests/docker/test_keydb.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/tests/docker/test_mariadb.py
+-rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/tests/docker/test_mssql.py
+-rw-r--r--   0        0        0     4193 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/tests/docker/test_mysql.py
+-rw-r--r--   0        0        0     3471 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/tests/docker/test_oracle.py
+-rw-r--r--   0        0        0     6003 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/tests/docker/test_postgres.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/tests/docker/test_redis.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/tests/docker/test_spanner.py
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/LICENSE
+-rw-r--r--   0        0        0    12148 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/README.md
+-rw-r--r--   0        0        0    16950 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0    13954 2020-02-02 00:00:00.000000 pytest_databases-0.2.4/PKG-INFO
```

### Comparing `pytest_databases-0.2.3/.pre-commit-config.yaml` & `pytest_databases-0.2.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.3/.sourcery.yaml` & `pytest_databases-0.2.4/.sourcery.yaml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.3/CONTRIBUTING.rst` & `pytest_databases-0.2.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.3/Makefile` & `pytest_databases-0.2.4/Makefile`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.3/.vscode/settings.json` & `pytest_databases-0.2.4/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.3/requirements/requirements-dev.txt` & `pytest_databases-0.2.4/requirements/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.3/requirements/requirements-docs.txt` & `pytest_databases-0.2.4/requirements/requirements-docs.txt`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.3/scripts/__init__.py` & `pytest_databases-0.2.4/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.3/scripts/build_docs.py` & `pytest_databases-0.2.4/scripts/build_docs.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.3/src/pytest_databases/__init__.py` & `pytest_databases-0.2.4/src/pytest_databases/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.3/src/pytest_databases/__metadata__.py` & `pytest_databases-0.2.4/src/pytest_databases/__metadata__.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.3/src/pytest_databases/helpers.py` & `pytest_databases-0.2.4/src/pytest_databases/helpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 
 from __future__ import annotations
 
+import hashlib
 import inspect
 from contextlib import AbstractAsyncContextManager, AbstractContextManager
 from functools import partial
 from typing import TYPE_CHECKING, Callable, TypeVar, cast, overload
 
 import anyio
 from typing_extensions import ParamSpec
@@ -77,7 +78,25 @@
     if inspect.iscoroutinefunction(fn):
         return fn
 
     async def wrapped(*args: P.args, **kwargs: P.kwargs) -> T:
         return await anyio.to_thread.run_sync(partial(fn, *args, **kwargs))
 
     return wrapped
+
+
+def simple_string_hash(string_to_hash: str) -> str:
+    """Generates a short hash based on a string.
+
+    Args:
+      string_to_hash: The string to hash.
+
+    Returns:
+      A short hash string.
+    """
+
+    string_bytes = string_to_hash.encode("utf-8")
+    hasher = hashlib.sha256()
+    hasher.update(string_bytes)
+    digest = hasher.digest()
+    hex_string = digest.hex()
+    return hex_string[:12]
```

### Comparing `pytest_databases-0.2.3/src/pytest_databases/docker/__init__.py` & `pytest_databases-0.2.4/src/pytest_databases/docker/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 import sys
 import timeit
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Callable
 
 import pytest
 
-from pytest_databases.helpers import wrap_sync
+from pytest_databases.helpers import simple_string_hash, wrap_sync
 
 if TYPE_CHECKING:
     from collections.abc import Awaitable, Generator
 
 
 async def wait_until_responsive(
     check: Callable[..., Awaitable],
@@ -66,25 +66,26 @@
     raise RuntimeError(msg)
 
 
 SKIP_DOCKER_COMPOSE: bool = bool(os.environ.get("SKIP_DOCKER_COMPOSE", False))
 USE_LEGACY_DOCKER_COMPOSE: bool = bool(
     os.environ.get("USE_LEGACY_DOCKER_COMPOSE", os.getenv("GITHUB_ACTIONS") != "true")
 )
+COMPOSE_PROJECT_NAME: str = f"pytest-databases-{simple_string_hash(__file__)}"
 
 
 class DockerServiceRegistry:
-    def __init__(self, worker_id: str) -> None:
+    def __init__(self, worker_id: str, compose_project_name: str = COMPOSE_PROJECT_NAME) -> None:
         self._running_services: set[str] = set()
         self.docker_ip = self._get_docker_ip()
         self._base_command = ["docker-compose"] if USE_LEGACY_DOCKER_COMPOSE else ["docker", "compose"]
         self._base_command.extend(
             [
                 f"--file={Path(__file__).parent / 'docker-compose.yml'}",
-                f"--project-name=pytest-databases-{worker_id}",
+                f"--project-name={compose_project_name}-{worker_id}",
             ],
         )
 
     @staticmethod
     def _get_docker_ip() -> str:
         docker_host = os.environ.get("DOCKER_HOST", "").strip()
         if not docker_host or docker_host.startswith("unix://"):
@@ -128,19 +129,24 @@
 
     def down(self) -> None:
         if not SKIP_DOCKER_COMPOSE:
             self.run_command("down", "--remove-orphans", "--volumes", "-t", "10")
 
 
 @pytest.fixture(scope="session")
-def docker_services(worker_id: str = "main") -> Generator[DockerServiceRegistry, None, None]:
+def compose_project_name() -> str:
+    return os.environ.get("COMPOSE_PROJECT_NAME", COMPOSE_PROJECT_NAME)
+
+
+@pytest.fixture(scope="session")
+def docker_services(compose_project_name: str, worker_id: str = "main") -> Generator[DockerServiceRegistry, None, None]:
     if os.getenv("GITHUB_ACTIONS") == "true" and sys.platform != "linux":
         pytest.skip("Docker not available on this platform")
 
-    registry = DockerServiceRegistry(worker_id)
+    registry = DockerServiceRegistry(worker_id, compose_project_name=compose_project_name)
     try:
         yield registry
     finally:
         registry.down()
 
 
 @pytest.fixture(scope="session")
```

### Comparing `pytest_databases-0.2.3/src/pytest_databases/docker/cockroachdb.py` & `pytest_databases-0.2.4/src/pytest_databases/docker/cockroachdb.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.3/src/pytest_databases/docker/docker-compose.yml` & `pytest_databases-0.2.4/src/pytest_databases/docker/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.3/src/pytest_databases/docker/dragonfly.py` & `pytest_databases-0.2.4/src/pytest_databases/docker/dragonfly.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.3/src/pytest_databases/docker/keydb.py` & `pytest_databases-0.2.4/src/pytest_databases/docker/keydb.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.3/src/pytest_databases/docker/mariadb.py` & `pytest_databases-0.2.4/src/pytest_databases/docker/mariadb.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.3/src/pytest_databases/docker/mssql.py` & `pytest_databases-0.2.4/src/pytest_databases/docker/mssql.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.3/src/pytest_databases/docker/mysql.py` & `pytest_databases-0.2.4/src/pytest_databases/docker/mysql.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.3/src/pytest_databases/docker/oracle.py` & `pytest_databases-0.2.4/src/pytest_databases/docker/oracle.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.3/src/pytest_databases/docker/postgres.py` & `pytest_databases-0.2.4/src/pytest_databases/docker/postgres.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.3/src/pytest_databases/docker/redis.py` & `pytest_databases-0.2.4/src/pytest_databases/docker/redis.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.3/src/pytest_databases/docker/spanner.py` & `pytest_databases-0.2.4/src/pytest_databases/docker/spanner.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.3/tests/__init__.py` & `pytest_databases-0.2.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.3/tests/conftest.py` & `pytest_databases-0.2.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.3/tests/docker/__init__.py` & `pytest_databases-0.2.4/tests/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.3/tests/docker/test_cockroachdb.py` & `pytest_databases-0.2.4/tests/docker/test_cockroachdb.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.3/tests/docker/test_dragonfly.py` & `pytest_databases-0.2.4/tests/docker/test_dragonfly.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.3/tests/docker/test_keydb.py` & `pytest_databases-0.2.4/tests/docker/test_keydb.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.3/tests/docker/test_mariadb.py` & `pytest_databases-0.2.4/tests/docker/test_mariadb.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.3/tests/docker/test_mssql.py` & `pytest_databases-0.2.4/tests/docker/test_mssql.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.3/tests/docker/test_mysql.py` & `pytest_databases-0.2.4/tests/docker/test_mysql.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.3/tests/docker/test_oracle.py` & `pytest_databases-0.2.4/tests/docker/test_oracle.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.3/tests/docker/test_postgres.py` & `pytest_databases-0.2.4/tests/docker/test_postgres.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.3/tests/docker/test_redis.py` & `pytest_databases-0.2.4/tests/docker/test_redis.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.3/tests/docker/test_spanner.py` & `pytest_databases-0.2.4/tests/docker/test_spanner.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.3/.gitignore` & `pytest_databases-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.3/LICENSE` & `pytest_databases-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.3/README.md` & `pytest_databases-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.2.3/pyproject.toml` & `pytest_databases-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 [project]
 description = 'Reusable database fixtures for any and all databases.'
 license = "MIT"
 name = "pytest-databases"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "0.2.3"
+version = "0.2.4"
 #
 authors = [{ name = "Cody Fincher", email = "cody.fincher@gmail.com" }]
 keywords = [
   "database",
   "migration",
   "postgres",
   "mysql",
```

### Comparing `pytest_databases-0.2.3/PKG-INFO` & `pytest_databases-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-databases
-Version: 0.2.3
+Version: 0.2.4
 Summary: Reusable database fixtures for any and all databases.
 Project-URL: Documentation, https://github.com/litestar-org/pytest-databases#readme
 Project-URL: Issues, https://github.com/litestar-org/pytest-databases/issues
 Project-URL: Source, https://github.com/litestar-org/pytest-databases
 Author-email: Cody Fincher <cody.fincher@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
```

