# Comparing `tmp/apache_airflow_providers_slack-8.6.1rc1.tar.gz` & `tmp/apache_airflow_providers_slack-8.6.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_slack-8.6.1rc1.tar", last modified: Sun Feb 11 07:28:40 2024, max compression
+gzip compressed data, was "apache_airflow_providers_slack-8.6.2rc1.tar", last modified: Tue Apr  9 12:41:24 2024, max compression
```

## Comparing `apache_airflow_providers_slack-8.6.1rc1.tar` & `apache_airflow_providers_slack-8.6.2rc1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     4396 2024-02-11 07:28:40.000000 apache_airflow_providers_slack-8.6.1rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-02-11 07:28:40.000000 apache_airflow_providers_slack-8.6.1rc1/airflow/providers/slack/LICENSE
--rw-r--r--   0        0        0     1580 2024-02-11 07:28:40.000000 apache_airflow_providers_slack-8.6.1rc1/airflow/providers/slack/__init__.py
--rw-r--r--   0        0        0     5340 2024-02-11 07:28:40.000000 apache_airflow_providers_slack-8.6.1rc1/airflow/providers/slack/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-02-11 07:28:40.000000 apache_airflow_providers_slack-8.6.1rc1/airflow/providers/slack/hooks/__init__.py
--rw-r--r--   0        0        0    17643 2024-02-11 07:28:40.000000 apache_airflow_providers_slack-8.6.1rc1/airflow/providers/slack/hooks/slack.py
--rw-r--r--   0        0        0    12938 2024-02-11 07:28:40.000000 apache_airflow_providers_slack-8.6.1rc1/airflow/providers/slack/hooks/slack_webhook.py
--rw-r--r--   0        0        0      785 2024-02-11 07:28:40.000000 apache_airflow_providers_slack-8.6.1rc1/airflow/providers/slack/notifications/__init__.py
--rw-r--r--   0        0        0     3891 2024-02-11 07:28:40.000000 apache_airflow_providers_slack-8.6.1rc1/airflow/providers/slack/notifications/slack.py
--rw-r--r--   0        0        0     1243 2024-02-11 07:28:40.000000 apache_airflow_providers_slack-8.6.1rc1/airflow/providers/slack/notifications/slack_notifier.py
--rw-r--r--   0        0        0     3844 2024-02-11 07:28:40.000000 apache_airflow_providers_slack-8.6.1rc1/airflow/providers/slack/notifications/slack_webhook.py
--rw-r--r--   0        0        0      787 2024-02-11 07:28:40.000000 apache_airflow_providers_slack-8.6.1rc1/airflow/providers/slack/operators/__init__.py
--rw-r--r--   0        0        0     9657 2024-02-11 07:28:40.000000 apache_airflow_providers_slack-8.6.1rc1/airflow/providers/slack/operators/slack.py
--rw-r--r--   0        0        0     5012 2024-02-11 07:28:40.000000 apache_airflow_providers_slack-8.6.1rc1/airflow/providers/slack/operators/slack_webhook.py
--rw-r--r--   0        0        0      785 2024-02-11 07:28:40.000000 apache_airflow_providers_slack-8.6.1rc1/airflow/providers/slack/transfers/__init__.py
--rw-r--r--   0        0        0     3308 2024-02-11 07:28:40.000000 apache_airflow_providers_slack-8.6.1rc1/airflow/providers/slack/transfers/base_sql_to_slack.py
--rw-r--r--   0        0        0     7501 2024-02-11 07:28:40.000000 apache_airflow_providers_slack-8.6.1rc1/airflow/providers/slack/transfers/sql_to_slack.py
--rw-r--r--   0        0        0     8052 2024-02-11 07:28:40.000000 apache_airflow_providers_slack-8.6.1rc1/airflow/providers/slack/transfers/sql_to_slack_webhook.py
--rw-r--r--   0        0        0     5200 2024-02-11 07:28:40.000000 apache_airflow_providers_slack-8.6.1rc1/airflow/providers/slack/utils/__init__.py
--rw-r--r--   0        0        0     3064 2024-02-11 07:28:40.000000 apache_airflow_providers_slack-8.6.1rc1/pyproject.toml
--rw-r--r--   0        0        0     6200 1970-01-01 00:00:00.000000 apache_airflow_providers_slack-8.6.1rc1/PKG-INFO
+-rw-r--r--   0        0        0     4401 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/LICENSE
+-rw-r--r--   0        0        0     1580 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/__init__.py
+-rw-r--r--   0        0        0     5361 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/hooks/__init__.py
+-rw-r--r--   0        0        0    17643 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/hooks/slack.py
+-rw-r--r--   0        0        0    12938 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/hooks/slack_webhook.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/notifications/__init__.py
+-rw-r--r--   0        0        0     3891 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/notifications/slack.py
+-rw-r--r--   0        0        0     1250 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/notifications/slack_notifier.py
+-rw-r--r--   0        0        0     3844 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/notifications/slack_webhook.py
+-rw-r--r--   0        0        0      787 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/operators/__init__.py
+-rw-r--r--   0        0        0     9784 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/operators/slack.py
+-rw-r--r--   0        0        0     5012 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/operators/slack_webhook.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/transfers/__init__.py
+-rw-r--r--   0        0        0     3308 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/transfers/base_sql_to_slack.py
+-rw-r--r--   0        0        0     8623 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/transfers/sql_to_slack.py
+-rw-r--r--   0        0        0     8156 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/transfers/sql_to_slack_webhook.py
+-rw-r--r--   0        0        0     5200 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/utils/__init__.py
+-rw-r--r--   0        0        0     3106 2024-04-09 12:41:24.000000 apache_airflow_providers_slack-8.6.2rc1/pyproject.toml
+-rw-r--r--   0        0        0     6252 1970-01-01 00:00:00.000000 apache_airflow_providers_slack-8.6.2rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_slack-8.6.1rc1/README.rst` & `apache_airflow_providers_slack-8.6.2rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-slack``
 
-Release: ``8.6.1.rc1``
+Release: ``8.6.2.rc1``
 
 
 `Slack <https://slack.com/>`__ services integration including:
 
   - `Slack API <https://api.slack.com/>`__
   - `Slack Incoming Webhook <https://api.slack.com/messaging/webhooks>`__
 
@@ -54,24 +54,24 @@
 Provider package
 ----------------
 
 This is a provider package for ``slack`` provider. All classes for this provider package
 are in ``airflow.providers.slack`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-slack/8.6.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-slack/8.6.2/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-slack``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -96,8 +96,8 @@
 ============================================================================================================  ==============
 Dependent package                                                                                             Extra
 ============================================================================================================  ==============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
 ============================================================================================================  ==============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-slack/8.6.1/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-slack/8.6.2/changelog.html>`_.
```

### Comparing `apache_airflow_providers_slack-8.6.1rc1/airflow/providers/slack/LICENSE` & `apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_slack-8.6.1rc1/airflow/providers/slack/__init__.py` & `apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "8.6.1"
+__version__ = "8.6.2"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
```

### Comparing `apache_airflow_providers_slack-8.6.1rc1/airflow/providers/slack/get_provider_info.py` & `apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,16 +24,17 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-slack",
         "name": "Slack",
         "description": "`Slack <https://slack.com/>`__ services integration including:\n\n  - `Slack API <https://api.slack.com/>`__\n  - `Slack Incoming Webhook <https://api.slack.com/messaging/webhooks>`__\n",
         "state": "ready",
-        "source-date-epoch": 1707636520,
+        "source-date-epoch": 1712666484,
         "versions": [
+            "8.6.2",
             "8.6.1",
             "8.6.0",
             "8.5.1",
             "8.5.0",
             "8.4.0",
             "8.3.0",
             "8.2.0",
```

### Comparing `apache_airflow_providers_slack-8.6.1rc1/airflow/providers/slack/hooks/__init__.py` & `apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_slack-8.6.1rc1/airflow/providers/slack/hooks/slack.py` & `apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/hooks/slack.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_slack-8.6.1rc1/airflow/providers/slack/hooks/slack_webhook.py` & `apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/hooks/slack_webhook.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_slack-8.6.1rc1/airflow/providers/slack/notifications/__init__.py` & `apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_slack-8.6.1rc1/airflow/providers/slack/notifications/slack.py` & `apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/notifications/slack.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_slack-8.6.1rc1/airflow/providers/slack/notifications/slack_notifier.py` & `apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/notifications/slack_notifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,20 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """This module is deprecated. Please use :mod:`airflow.providers.slack.notifications.slack`."""
+
 from __future__ import annotations
 
 import warnings
 
 from airflow.exceptions import AirflowProviderDeprecationWarning
-from airflow.providers.slack.notifications.slack import SlackNotifier  # noqa
+from airflow.providers.slack.notifications.slack import SlackNotifier  # noqa: F401
 
 warnings.warn(
     "This module is deprecated. Please use `airflow.providers.slack.notifications.slack`",
     AirflowProviderDeprecationWarning,
     stacklevel=2,
 )
```

### Comparing `apache_airflow_providers_slack-8.6.1rc1/airflow/providers/slack/notifications/slack_webhook.py` & `apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/notifications/slack_webhook.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_slack-8.6.1rc1/airflow/providers/slack/operators/__init__.py` & `apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_slack-8.6.1rc1/airflow/providers/slack/operators/slack.py` & `apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/operators/slack.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from typing import TYPE_CHECKING, Any, Sequence
 
 from typing_extensions import Literal
 
 from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.models import BaseOperator
 from airflow.providers.slack.hooks.slack import SlackHook
+from airflow.utils.types import NOTSET, ArgNotSet
 
 if TYPE_CHECKING:
     from slack_sdk.http_retry import RetryHandler
 
     from airflow.utils.context import Context
 
 
@@ -222,26 +223,27 @@
         channels: str | Sequence[str] | None = None,
         initial_comment: str | None = None,
         filename: str | None = None,
         filetype: str | None = None,
         content: str | None = None,
         title: str | None = None,
         method_version: Literal["v1", "v2"] = "v1",
+        channel: str | Sequence[str] | None | ArgNotSet = NOTSET,
         **kwargs,
     ) -> None:
-        if channel := kwargs.pop("channel", None):
+        if channel is not NOTSET:
             warnings.warn(
                 "Argument `channel` is deprecated and will removed in a future releases. "
                 "Please use `channels` instead.",
                 AirflowProviderDeprecationWarning,
                 stacklevel=2,
             )
             if channels:
                 raise ValueError(f"Cannot set both arguments: channel={channel!r} and channels={channels!r}.")
-            channels = channel
+            channels = channel  # type: ignore[assignment]
 
         super().__init__(method="files.upload", **kwargs)
         self.channels = channels
         self.initial_comment = initial_comment
         self.filename = filename
         self.filetype = filetype
         self.content = content
```

### Comparing `apache_airflow_providers_slack-8.6.1rc1/airflow/providers/slack/operators/slack_webhook.py` & `apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/operators/slack_webhook.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_slack-8.6.1rc1/airflow/providers/slack/transfers/__init__.py` & `apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_slack-8.6.1rc1/airflow/providers/slack/transfers/base_sql_to_slack.py` & `apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/transfers/base_sql_to_slack.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_slack-8.6.1rc1/airflow/providers/slack/transfers/sql_to_slack.py` & `apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/transfers/sql_to_slack.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from functools import cached_property
 from tempfile import NamedTemporaryFile
 from typing import TYPE_CHECKING, Any, Mapping, Sequence
 
 from deprecated import deprecated
 from typing_extensions import Literal
 
-from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
+from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning, AirflowSkipException
 from airflow.providers.slack.hooks.slack import SlackHook
 from airflow.providers.slack.transfers.base_sql_to_slack import BaseSqlToSlackOperator
 from airflow.providers.slack.transfers.sql_to_slack_webhook import SqlToSlackWebhookOperator
 from airflow.providers.slack.utils import parse_filename
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
@@ -54,14 +54,19 @@
     :param slack_channels: Comma-separated list of channel names or IDs where the file will be shared.
          If omitting this parameter, then file will send to workspace.
     :param slack_initial_comment: The message text introducing the file in specified ``slack_channels``.
     :param slack_title: Title of file.
     :param slack_base_url: A string representing the Slack API base URL. Optional
     :param slack_method_version: The version of the Slack SDK Client method to be used, either "v1" or "v2".
     :param df_kwargs: Keyword arguments forwarded to ``pandas.DataFrame.to_{format}()`` method.
+    :param action_on_empty_df: Specifying how to handle an empty sql output df. Possible values:
+
+        - ``send``: (default) send the slack with an empty file.
+        - ``skip``: skip sending the slack message. Task state set to "skipped".
+        - ``error``: raise an error to fail the task. Task state set to "failed".
     """
 
     template_fields: Sequence[str] = (
         "sql",
         "slack_channels",
         "slack_filename",
         "slack_initial_comment",
@@ -83,27 +88,31 @@
         slack_filename: str,
         slack_channels: str | Sequence[str] | None = None,
         slack_initial_comment: str | None = None,
         slack_title: str | None = None,
         slack_base_url: str | None = None,
         slack_method_version: Literal["v1", "v2"] = "v1",
         df_kwargs: dict | None = None,
+        action_on_empty_df: Literal["send", "skip", "error"] = "send",
         **kwargs,
     ):
         super().__init__(
             sql=sql, sql_conn_id=sql_conn_id, sql_hook_params=sql_hook_params, parameters=parameters, **kwargs
         )
         self.slack_conn_id = slack_conn_id
         self.slack_filename = slack_filename
         self.slack_channels = slack_channels
         self.slack_initial_comment = slack_initial_comment
         self.slack_title = slack_title
         self.slack_base_url = slack_base_url
         self.slack_method_version = slack_method_version
         self.df_kwargs = df_kwargs or {}
+        if not action_on_empty_df or action_on_empty_df not in ("send", "skip", "error"):
+            raise ValueError(f"Invalid `action_on_empty_df` value {action_on_empty_df!r}")
+        self.action_on_empty_df = action_on_empty_df
 
     @cached_property
     def slack_hook(self):
         """Slack API Hook."""
         return SlackHook(
             slack_conn_id=self.slack_conn_id,
             base_url=self.slack_base_url,
@@ -130,14 +139,21 @@
             # pandas will open file in correct mode itself depend on file type.
             # So we close file descriptor here for avoid incidentally write anything.
             fp.close()
 
             output_file_name = fp.name
             output_file_format = output_file_format.upper()
             df_result = self._get_query_results()
+            if df_result.empty:
+                if self.action_on_empty_df == "skip":
+                    raise AirflowSkipException("SQL output df is empty. Skipping.")
+                elif self.action_on_empty_df == "error":
+                    raise ValueError("SQL output df must be non-empty. Failing.")
+                elif self.action_on_empty_df != "send":
+                    raise ValueError(f"Invalid `action_on_empty_df` value {self.action_on_empty_df!r}")
             if output_file_format == "CSV":
                 df_result.to_csv(output_file_name, **self.df_kwargs)
             elif output_file_format == "JSON":
                 df_result.to_json(output_file_name, **self.df_kwargs)
             elif output_file_format == "HTML":
                 df_result.to_html(output_file_name, **self.df_kwargs)
             else:
```

### Comparing `apache_airflow_providers_slack-8.6.1rc1/airflow/providers/slack/transfers/sql_to_slack_webhook.py` & `apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/transfers/sql_to_slack_webhook.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 from deprecated import deprecated
 from tabulate import tabulate
 
 from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.providers.slack.hooks.slack_webhook import SlackWebhookHook
 from airflow.providers.slack.transfers.base_sql_to_slack import BaseSqlToSlackOperator
+from airflow.utils.types import NOTSET, ArgNotSet
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class SqlToSlackWebhookOperator(BaseSqlToSlackOperator):
     """
@@ -83,30 +84,31 @@
         sql_conn_id: str,
         slack_webhook_conn_id: str | None = None,
         sql_hook_params: dict | None = None,
         slack_channel: str | None = None,
         slack_message: str,
         results_df_name: str = "results_df",
         parameters: list | tuple | Mapping[str, Any] | None = None,
+        slack_conn_id: str | ArgNotSet = NOTSET,
         **kwargs,
     ) -> None:
-        if slack_conn_id := kwargs.pop("slack_conn_id", None):
+        if slack_conn_id is not NOTSET:
             warnings.warn(
                 "Parameter `slack_conn_id` is deprecated because this attribute initially intend to use with "
                 "Slack API however this operator provided integration with Slack Incoming Webhook. "
                 "Please use `slack_webhook_conn_id` instead.",
                 AirflowProviderDeprecationWarning,
                 stacklevel=3,
             )
             if slack_webhook_conn_id and slack_conn_id != slack_webhook_conn_id:
                 raise ValueError(
                     "Conflicting Connection ids provided, "
                     f"slack_webhook_conn_id={slack_webhook_conn_id!r}, slack_conn_id={slack_conn_id!r}."
                 )
-            slack_webhook_conn_id = slack_conn_id
+            slack_webhook_conn_id = slack_conn_id  # type: ignore[assignment]
         if not slack_webhook_conn_id:
             raise ValueError("Got an empty `slack_webhook_conn_id` value.")
         super().__init__(
             sql=sql, sql_conn_id=sql_conn_id, sql_hook_params=sql_hook_params, parameters=parameters, **kwargs
         )
 
         self.slack_webhook_conn_id = slack_webhook_conn_id
```

### Comparing `apache_airflow_providers_slack-8.6.1rc1/airflow/providers/slack/utils/__init__.py` & `apache_airflow_providers_slack-8.6.2rc1/airflow/providers/slack/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_slack-8.6.1rc1/pyproject.toml` & `apache_airflow_providers_slack-8.6.2rc1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-slack"
-version = "8.6.1.rc1"
+version = "8.6.2.rc1"
 description = "Provider package apache-airflow-providers-slack for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -47,26 +47,27 @@
     "Framework :: Apache Airflow",
     "Framework :: Apache Airflow :: Provider",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: System :: Monitoring",
 ]
 requires-python = "~=3.8"
 dependencies = [
-    "apache-airflow-providers-common-sql>=1.3.1.dev0",
-    "apache-airflow>=2.6.0.dev0",
+    "apache-airflow-providers-common-sql>=1.3.1rc0",
+    "apache-airflow>=2.6.0rc0",
     "slack_sdk>=3.19.0",
 ]
 
 [project.urls]
-"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-slack/8.6.1"
-"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-slack/8.6.1/changelog.html"
+"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-slack/8.6.2"
+"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-slack/8.6.2/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
 "Slack Chat" = "https://s.apache.org/airflow-slack"
 "Twitter" = "https://twitter.com/ApacheAirflow"
 "YouTube" = "https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/"
 
 [project.entry-points."apache_airflow_provider"]
```

### Comparing `apache_airflow_providers_slack-8.6.1rc1/PKG-INFO` & `apache_airflow_providers_slack-8.6.2rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-slack
-Version: 8.6.1rc1
+Version: 8.6.2rc1
 Summary: Provider package apache-airflow-providers-slack for Apache Airflow
 Keywords: airflow-provider,slack,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,22 +15,23 @@
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Monitoring
-Requires-Dist: apache-airflow-providers-common-sql>=1.3.1.dev0
-Requires-Dist: apache-airflow>=2.6.0.dev0
+Requires-Dist: apache-airflow-providers-common-sql>=1.3.1rc0
+Requires-Dist: apache-airflow>=2.6.0rc0
 Requires-Dist: slack_sdk>=3.19.0
 Requires-Dist: apache-airflow-providers-common-sql ; extra == "common.sql"
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-slack/8.6.1/changelog.html
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-slack/8.6.1
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-slack/8.6.2/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-slack/8.6.2
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Provides-Extra: common.sql
 
 
@@ -73,15 +74,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-slack``
 
-Release: ``8.6.1.rc1``
+Release: ``8.6.2.rc1``
 
 
 `Slack <https://slack.com/>`__ services integration including:
 
   - `Slack API <https://api.slack.com/>`__
   - `Slack Incoming Webhook <https://api.slack.com/messaging/webhooks>`__
 
@@ -89,24 +90,24 @@
 Provider package
 ----------------
 
 This is a provider package for ``slack`` provider. All classes for this provider package
 are in ``airflow.providers.slack`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-slack/8.6.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-slack/8.6.2/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-slack``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -131,8 +132,8 @@
 ============================================================================================================  ==============
 Dependent package                                                                                             Extra
 ============================================================================================================  ==============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
 ============================================================================================================  ==============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-slack/8.6.1/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-slack/8.6.2/changelog.html>`_.
```

