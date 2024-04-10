# Comparing `tmp/pih-mio-0.25.tar.gz` & `tmp/pih-mio-0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-mio-0.25.tar", last modified: Fri Mar 29 06:40:33 2024, max compression
+gzip compressed data, was "pih-mio-0.26.tar", last modified: Wed Apr 10 01:48:51 2024, max compression
```

## Comparing `pih-mio-0.25.tar` & `pih-mio-0.26.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 06:40:33.365226 pih-mio-0.25/
-drwxrwxrwx   0        0        0        0 2024-03-29 06:40:32.957927 pih-mio-0.25/MobileHelperService/
--rw-rw-rw-   0        0        0        0 2024-01-09 05:16:13.000000 pih-mio-0.25/MobileHelperService/__init__.py
--rw-rw-rw-   0        0        0      208 2024-02-09 05:31:09.000000 pih-mio-0.25/MobileHelperService/__main__.py
--rw-rw-rw-   0        0        0   356775 2024-03-28 11:44:43.000000 pih-mio-0.25/MobileHelperService/api.py
--rw-rw-rw-   0        0        0     5980 2024-03-12 09:02:04.000000 pih-mio-0.25/MobileHelperService/client.py
--rw-rw-rw-   0        0        0      100 2024-02-20 01:16:51.000000 pih-mio-0.25/MobileHelperService/collection.py
--rw-rw-rw-   0        0        0     4373 2024-03-29 06:39:55.000000 pih-mio-0.25/MobileHelperService/const.py
--rw-rw-rw-   0        0        0      635 2024-02-14 02:40:54.000000 pih-mio-0.25/MobileHelperService/service.py
--rw-rw-rw-   0        0        0    16596 2024-03-21 06:21:36.000000 pih-mio-0.25/MobileHelperService/service_api.py
--rw-rw-rw-   0        0        0      329 2024-03-29 06:40:33.333996 pih-mio-0.25/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-29 06:40:33.287105 pih-mio-0.25/pih_mio.egg-info/
--rw-rw-rw-   0        0        0      329 2024-03-29 06:40:31.000000 pih-mio-0.25/pih_mio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      437 2024-03-29 06:40:32.000000 pih-mio-0.25/pih_mio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 06:40:31.000000 pih-mio-0.25/pih_mio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-03-29 06:40:31.000000 pih-mio-0.25/pih_mio.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2024-03-29 06:40:31.000000 pih-mio-0.25/pih_mio.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-03-29 06:40:31.000000 pih-mio-0.25/pih_mio.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-29 06:40:33.365226 pih-mio-0.25/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 01:48:51.476647 pih-mio-0.26/
+drwxrwxrwx   0        0        0        0 2024-04-10 01:48:49.845473 pih-mio-0.26/MobileHelperService/
+-rw-rw-rw-   0        0        0        0 2024-01-09 05:16:13.000000 pih-mio-0.26/MobileHelperService/__init__.py
+-rw-rw-rw-   0        0        0      208 2024-02-09 05:31:09.000000 pih-mio-0.26/MobileHelperService/__main__.py
+-rw-rw-rw-   0        0        0   361212 2024-04-09 23:32:25.000000 pih-mio-0.26/MobileHelperService/api.py
+-rw-rw-rw-   0        0        0     5980 2024-03-12 09:02:04.000000 pih-mio-0.26/MobileHelperService/client.py
+-rw-rw-rw-   0        0        0      100 2024-02-20 01:16:51.000000 pih-mio-0.26/MobileHelperService/collection.py
+-rw-rw-rw-   0        0        0     4461 2024-04-10 00:33:44.000000 pih-mio-0.26/MobileHelperService/const.py
+-rw-rw-rw-   0        0        0      635 2024-02-14 02:40:54.000000 pih-mio-0.26/MobileHelperService/service.py
+-rw-rw-rw-   0        0        0    16596 2024-03-21 06:21:36.000000 pih-mio-0.26/MobileHelperService/service_api.py
+-rw-rw-rw-   0        0        0      329 2024-04-10 01:48:51.460008 pih-mio-0.26/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-10 01:48:51.428757 pih-mio-0.26/pih_mio.egg-info/
+-rw-rw-rw-   0        0        0      329 2024-04-10 01:48:49.000000 pih-mio-0.26/pih_mio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      437 2024-04-10 01:48:49.000000 pih-mio-0.26/pih_mio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 01:48:49.000000 pih-mio-0.26/pih_mio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-04-10 01:48:49.000000 pih-mio-0.26/pih_mio.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2024-04-10 01:48:49.000000 pih-mio-0.26/pih_mio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-10 01:48:49.000000 pih-mio-0.26/pih_mio.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 01:48:51.476647 pih-mio-0.26/setup.cfg
```

### Comparing `pih-mio-0.25/MobileHelperService/api.py` & `pih-mio-0.26/MobileHelperService/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from io import BytesIO
 from time import sleep
 from enum import Enum
 from re import Match
 import traceback
 import requests
 import calendar
+import shlex
 import json
 import re
 
 from MobileHelperContent.content import MEDIA_CONTENT  # type: ignore
 
 from pih.collections import (
     User,
@@ -58,41 +59,43 @@
     lw,
     js,
     nn,
     ne,
     nns,
     one,
     esc,
-    escs,
     jnl,
+    nnb,
+    nnl,
+    escs,
     if_else,
     while_not_do,
 )
 from pih.consts import (
     CheckableSections,
     Actions,
     JournalType,
     Tags,
-    SPLITTER,
+    A.CT.SPLITTER,
     EmailVerificationMethods,
 )
 from MobileHelperService.collection import MobileHelperUserSettings
 from pih.consts.polibase import PolibaseDocumentTypes
 from pih.consts.ssh_hosts import SSHHosts
 from MobileHelperService.const import *
 
 from pih.consts.errors import BarcodeNotFound, NotFound, Error
 from pih import (
     A,
     PIH,
-    PIHThread,
     Input,
     Stdin,
     Output,
     Session,
+    PIHThread,
     MarkInput,
     UserInput,
     UserOutput,
     MarkOutput,
     SessionBase,
     OutputStub,
 )
@@ -573,15 +576,15 @@
             )
         )
 
     def input(self, value: str) -> None:
         self.separated_line()
         with self.make_personalized(True):
             with self.make_indent(2, True):
-                self.write_line(j((value, SPLITTER)))
+                self.write_line(j((value, A.CT.SPLITTER)))
                 if self.show_exit_message:
                     with self.make_indent(2):
                         with self.make_personalized(False):
                             self.write_line(self.exit_line or self.create_exit_line())
 
     def value(self, caption: str, value: Any, text_before: str | None = None) -> None:
         self.separated_line()
@@ -3222,24 +3225,26 @@
             },
             CommandNode([""], [""]): all_passwords_node,
             CommandNode(
                 ["set"],
                 ["Установить значение переменной"],
                 self.get_or_set_variable_handler,
             ): None,
-            CommandNode(
-                ["open"],
-                ["Открытие дверей холодного прохода"],
-                lambda: self.door_open_handler("cold_pass"),
-            ): None,
-            CommandNode(
-                ["close"],
-                ["Закрытие дверей холодного прохода"],
-                lambda: self.door_close_handler("cold_pass"),
-            ): None,
+            CommandNode(["door", "дверь"], [""]): {
+                CommandNode(
+                    ["open"],
+                    ["Открытие дверей холодного прохода"],
+                    lambda: self.door_open_handler("cold_pass"),
+                ),
+                CommandNode(
+                    ["close"],
+                    ["Закрытие дверей холодного прохода"],
+                    lambda: self.door_close_handler("cold_pass"),
+                )
+            },
             CommandNode(
                 ["get"],
                 ["Показать значение переменной"],
                 lambda: self.get_or_set_variable_handler(True),
             ): None,
             CommandNode(["qr"], [""]): {
                 CommandNode(["code", "код"], ["Создание QR-кода", "Создать QR-код"]): {
@@ -3369,23 +3374,23 @@
         search_request_source: str | None = search_request
         file_pattern_index: int | None = get_file_pattern_index(search_request)
         if ne(search_request):
             search_request = search_request[
                 len(FILE_PATTERN_LIST[file_pattern_index]) :
             ]
             if n(command_type):
-                splitter_index: int = search_request.find(SPLITTER)
+                splitter_index: int = search_request.find(A.CT.SPLITTER)
                 command_type = A.D_Ex.command_type(
                     search_request
                     if splitter_index == -1
                     else search_request[0:splitter_index]
                 )
 
         def label_function(file: File, _) -> str:
-            title_list: list[str] = file.title.split(SPLITTER)
+            title_list: list[str] = file.title.split(A.CT.SPLITTER)
             if len(title_list) == 3:
                 return j(
                     ([b(title_list[0].upper()), ": "] if n(filter_function) else [])
                     + [
                         b(title_list[-1]),
                         " (",
                         title_list[-2],
@@ -3415,15 +3420,15 @@
                 exclude_private_files=True,
             ).data  # type: ignore
         file: File = self.input.item_by_index(
             "Выберите файл",
             A.D.filter(filter_function or (lambda _: True), file_list),
             label_function,
         )
-        title_list: list[str] = file.title.split(SPLITTER)  # type: ignore
+        title_list: list[str] = file.title.split(A.CT.SPLITTER)  # type: ignore
         self.output.separated_line()
         if nn(search_request_source) and search_request_source in self.arg_list:
             self.arg_list.remove(search_request_source)
         command_type = command_type or A.D_Ex.command_type(file)
         if not (self.is_silence or self.is_only_result):
             self.output.head1(
                 js(
@@ -3646,15 +3651,15 @@
                     or self.input.input(
                         f"Введите:\n  {A.CT_V.BULLET} Адресс электронной почты\nили\n  {A.CT_V.BULLET} Поисковый запрос для поиска пациента"
                     )
                 )
             polibase_person_string: str = ""
             if ne(polibase_person):
                 polibase_person_string = j(
-                    ("клиента ", b(polibase_person.FullName), SPLITTER)  # type: ignore
+                    ("клиента ", b(polibase_person.FullName), A.CT.SPLITTER)  # type: ignore
                 )
             if not only_for_polibase_person:
                 if ne(value):
                     if A.C.email(nns(value)):
                         result = A.C_EML.accessability(value, not self.is_forced, EmailVerificationMethods.NORMAL if self.is_test else None)  # type: ignore
                         self.output.separated_line()
                         text: str = js(
@@ -3772,15 +3777,15 @@
                             self.user_given_name,
                             ", ожидайте уведовление об процессе создания бекапа база данных Polibase в telegram-группе: ",
                             b("Backup Console"),
                         )
                     )
                 )
             )
-        A.A_P.DB.backup(self.input.answer if answer else name, test)
+        A.A_P.DB.backup(self.input.answer if answer else name, test, self.is_forced)
 
     def show_polibase_password_handler(self) -> None:
         LOGIN: str = "login"
         PASSWORD: str = "password"
         result: dict[str, Any] | None = None
 
         def execute_query_for_password(condition: str) -> dict[str, Any] | None:
@@ -3840,18 +3845,45 @@
                 )
             )
 
     def robocopy_job_run_handler(self) -> None:
         forced: bool = self.is_forced
         source_job_name: str | None = self.arg()
         if ne(source_job_name):
-            source_job_name = source_job_name.lower()
+            source_job_name = lw(source_job_name)
         job_name_set: set = set()
         job_status_map_by_name: dict[str, list[RobocopyJobStatus]] = defaultdict(list)
         job_status_list: list[RobocopyJobStatus] = A.R_B.robocopy_job_status_list().data
+        if self.is_all and n(source_job_name):
+            filtered_job_status_list: list[RobocopyJobStatus] = A.D.filter(
+                lambda item: not (item.exclude or (item.active and not self.is_forced)),
+                job_status_list,
+            )
+            length: int = len(filtered_job_status_list)
+            if length > 0 and self.yes_no(js(("Запустить все", length, "заданий"))):
+                job_status: RobocopyJobStatus
+                for job_status in filtered_job_status_list:
+                    A.A_B.start_robocopy_job(
+                        job_status.name,
+                        job_status.source,
+                        job_status.destination,
+                        forced,
+                    )
+                self.write_line(
+                    i(
+                        js(
+                            (
+                                j((self.user_given_name, ",")),
+                                "ожидайте уведовление об процессе выполнения Robocopy-задания в telegram-группе",
+                                b("Backup Console"),
+                            )
+                        )
+                    )
+                )
+                return
         job_status_map: dict[str, RobocopyJobStatus] = {}
         for job_status in job_status_list:
             job_name: str = job_status.name
             job_name_set.add(job_name)
             job_status_map_by_name[job_name].append(job_status)
             job_status_map[
                 A.D_F_B.job_full_name(
@@ -3869,18 +3901,20 @@
                 if job_status.name == job_name:
                     inacitve_count += 1
                     if job_status.active:
                         inacitve_count -= 1
             return inacitve_count == 0
 
         if ne(source_job_name) and is_active(source_job_name) and not forced:
-            self.output.error(f"Robocopy-задание '{source_job_name}' уже выполняется")
+            self.output.error(
+                js(("Robocopy-задание", escs(source_job_name), "уже выполняется"))
+            )
         else:
             if source_job_name not in job_name_list:
-                self.write_line(f"{b('Список Robocopy-заданий:')}\n")
+                self.write_line(nl(b("Список Robocopy-заданий:")))
 
             def job_status_list_label_function(name: str) -> str:
                 job_list: list[RobocopyJobStatus] = job_status_map_by_name[name]
 
                 def job_status_item_label_function(
                     job_status: RobocopyJobStatus,
                 ) -> str:
@@ -3894,49 +3928,68 @@
                     if job_status.active:
                         date = "выполняется"
                     else:
                         if job_status.last_created is not None:
                             date = A.D_F.datetime(job_status.last_created)
                         status = job_status.last_status
                     return (
-                        f"   {A.CT.VISUAL.BULLET} {source}{A.CT.VISUAL.ARROW}{destination}"
+                        j(
+                            (
+                                "   ",
+                                A.CT.VISUAL.BULLET,
+                                " ",
+                                source,
+                                A.CT.VISUAL.ARROW,
+                                destination,
+                            )
+                        )
                         + ("" if status is None else f" [ {b(status)} ]")
-                        + ("" if date is None else f"\n     {date}")
+                        + (
+                            ""
+                            if date is None
+                            else nl(j((" " * 5, date)), reversed=True)
+                        )
                     )
 
                 return nl(
                     jnl(A.D.map(job_status_item_label_function, job_list)),
                     reversed=True,
                 )
 
             def job_label_function(name: str) -> str:
-                return j((b(name), SPLITTER, job_status_list_label_function(name)))
+                return j((b(name), A.CT.SPLITTER, job_status_list_label_function(name)))
 
             job_name: str = source_job_name or self.input.item_by_index(
                 "Пожалуйста, выберите Robocopy-задание, которое необходимо запустить",
                 job_name_list,
                 lambda name, _: job_label_function(name),
             )
             job_list: list[RobocopyJobStatus] = job_status_map_by_name[job_name]
             job_list = (
                 job_list
                 if forced
                 else A.D.filter(lambda item: not item.active or item.live, job_list)
             )
             if len(job_list) > 0:
                 self.write_line(nl(j((b("Robocopy-задание"), ": ", job_name))))
-                job_item: RobocopyJobStatus = self.input.item_by_index(
-                    "Пожалуйста, выберите направление",
-                    job_list
-                    + ([] if len(job_list) < 2 else [RobocopyJobStatus("Все")]),
-                    lambda item, _: (
-                        b(item.name)
-                        if n(item.destination)
-                        else b(j((item.source, A.CT.VISUAL.ARROW, item.destination)))
-                    ),
+                all_job_item: RobocopyJobStatus = RobocopyJobStatus("Все")
+                job_item: RobocopyJobStatus = (
+                    all_job_item
+                    if self.is_all
+                    else self.input.item_by_index(
+                        "Пожалуйста, выберите направление",
+                        job_list + ([] if len(job_list) <= 1 else [all_job_item]),
+                        lambda item, _: (
+                            b(item.name)
+                            if n(item.destination)
+                            else b(
+                                j((item.source, A.CT.VISUAL.ARROW, item.destination))
+                            )
+                        ),
+                    )
                 )
                 if A.A_B.start_robocopy_job(
                     job_name, job_item.source, job_item.destination, forced
                 ):
                     self.write_line(
                         i(
                             j(
@@ -4369,15 +4422,15 @@
                 except NotFound as _:
                     pass
         if not was_found:
             self.output.error("Ничего не найдена")
 
     def run_command_handler(self, command_type: A.CT_CMDT | None = None) -> None:
         def filter_function(item: Note) -> bool:
-            title_list: list[str] = item.title.split(SPLITTER)  # type: ignore
+            title_list: list[str] = item.title.split(A.CT.SPLITTER)  # type: ignore
             if len(title_list) > 1:
                 return title_list[0].lower() in A.D.get(command_type)[1:]
             return True
 
         arg: Any | None = None
         if n(command_type):
             for i in range(max(1, self.arg_len)):
@@ -4420,52 +4473,55 @@
         command_type: A.CT_CMDT | None = None,
         text: str | None = None,
         title: str | None = None,
         test: bool | None = None,
     ) -> None:
         host: str | None = None
 
-        def extract_parameters(value: str) -> str:
+        def extract_parameters(value: str, for_cmd: bool = False) -> str:
             class DH:
                 parameters_map: dict[str, list[str | None]] = {}
 
             def get_name_and_title(value: Match[str]) -> tuple[str, str | None]:
                 name_and_title: str = value.group()[1:]
-                name_and_title_list: list[str] = name_and_title.split(SPLITTER)
+                name_and_title_list: list[str] = name_and_title.split(A.CT.SPLITTER)
                 return (
                     name_and_title_list[0],
                     name_and_title_list[1] if len(name_and_title_list) > 1 else None,
                 )
 
             def create_parameters_map(value: Match[str]) -> str:
                 name: str | None = None
                 title: str | None = None
                 name, title = get_name_and_title(value)
                 if name not in DH.parameters_map:
                     DH.parameters_map[name] = [None, title]
                 return value.group()
 
-            re.sub(PARAMETER_PATTERN, create_parameters_map, value)
+            parameter_pattern: str = [PARAMETER_PATTERN, PARAMETER_PATTERN_FOR_CMD][
+                for_cmd
+            ]
+            re.sub(parameter_pattern, create_parameters_map, value)
             fileless_arg_list: list[str] = self.arg_list_exclude_file
             for index, parameter in enumerate(DH.parameters_map):
                 DH.parameters_map[parameter][0] = A.D.if_is_in(
                     fileless_arg_list, index
                 ) or self.input.input(
                     js(
                         (
-                            "Введите параметр",
+                            "Введите значение для параметра",
                             b(DH.parameters_map[parameter][1] or parameter),
                         )
                     )
                 )
 
             def put_parameters(value: Match[str]) -> str:
                 return DH.parameters_map[get_name_and_title(value)[0]][0]
 
-            return re.sub(PARAMETER_PATTERN, put_parameters, value)
+            return re.sub(parameter_pattern, put_parameters, value)
 
         if e(text):
             search_request: str | None = self.arg()
             file_pattern_index: int | None = get_file_pattern_index(search_request)
             if nn(file_pattern_index) or self.yes_no("Выбрать файл"):
                 text = self.choose_file(
                     search_request,
@@ -4513,124 +4569,161 @@
                             )
                         )
                     )
                     if self.yes_no("Поробовать ввести команду снова"):
                         text = None
                     else:
                         break
-        if command_type == A.CT_CMDT.CMD:
+        if command_type in (A.CT_CMDT.CMD, A.CT_CMDT.POWERSHELL):
+            is_powershell: bool = command_type == A.CT_CMDT.POWERSHELL
             default_host: str = A.SYS.host()
             host = None
 
-            def get_command(value: str | None = None) -> list[str]:
-                result: tuple[list[str], list[str]] = A.D.separate_unquoted_and_quoted(
-                    value or self.pih.input.input("Введите команду")
+            def get_command(
+                value: str | None = None, for_cmd: bool = False
+            ) -> tuple[str, ...]:
+                result: tuple[list[str], list[str]] | list[str] = (
+                    shlex.split(nns(value), posix=False)
+                    if for_cmd
+                    else A.D.separate_unquoted_and_quoted(
+                        value or self.pih.input.input("Введите команду")
+                    )
+                )
+                return tuple(
+                    A.D.filter(
+                        lambda item: ne(item),
+                        result if for_cmd else result[0] + result[1],
+                    )
                 )
-                return A.D.filter(lambda item: ne(item), result[0] + result[1])
 
             use_psexec_executor: bool | None = None
             host_is_local: bool | None = None
-            if ne(text):
-                text = extract_parameters(text)
-            command_text_list: list[str] = A.D.filter(
-                lambda item: not item.startswith("::"),
-                ([None] if e(text) else text.splitlines()),
-            )
-            for text in command_text_list:
-                text = get_command(text if ne(text) else None)
-                if n(use_psexec_executor):
-                    use_psexec_executor = e(
-                        [
-                            value
-                            for value in A.D.map(lambda item: item.lower(), text)
-                            if value in A.CT.PSTOOLS.COMMAND_LIST
-                        ]
+            if n(text):
+                text = self.input.input("Введите команду")
+            for text_line in text.split("@\\n"):
+                if ne(text_line):
+                    text_line = extract_parameters(text_line, True)
+                if nn(text):
+                    command_text_list: list[str] = A.D.not_empty_items(
+                        A.D.filter(
+                            lambda item: not item.startswith("::"),
+                            ([None] if e(text_line) else text_line.splitlines()),
+                        )
+                    )
+                for command_text_line in command_text_list:
+                    command_text_line = get_command(
+                        command_text_line if ne(command_text_line) else None,
+                        for_cmd=True,
                     )
-                process_result: CompletedProcess | None = None
-                if use_psexec_executor:
-                    if e(host):
-                        if self.yes_no(
-                            j(
-                                (
-                                    "Использовать хост ",
-                                    b(default_host),
-                                    ", для выполнения команды",
-                                )
-                            ),
-                            no_label=b("Или введите название хоста"),
-                        ):
-                            host = default_host
-                        else:
-                            host = self.input.answer
-                    while True:
-                        host = host.lower()
-                        if A.C_R.accessibility_by_ping(host, count=1):
-                            self.write_line(
-                                nl(
-                                    js(
-                                        (
-                                            "Команда будет запущена на хосте",
-                                            b(host),
+                    if n(use_psexec_executor):
+                        use_psexec_executor = e(
+                            [
+                                value
+                                for value in A.D.map(
+                                    lambda item: lw(item), command_text_line
+                                )
+                                if value in A.CT.PSTOOLS.COMMAND_LIST
+                            ]
+                        )
+                    process_result: CompletedProcess | None = None
+                    if use_psexec_executor:
+                        if e(host):
+                            if self.yes_no(
+                                j(
+                                    (
+                                        "Использовать хост ",
+                                        b(default_host),
+                                        ", для выполнения команды",
+                                    )
+                                ),
+                                no_label=b("Или введите название хоста"),
+                            ):
+                                host = default_host
+                            else:
+                                host = self.input.answer
+                        while True:
+                            host = lw(host)
+                            if host == default_host or A.C_R.accessibility_by_ping(
+                                host, count=1
+                            ):
+                                self.write_line(
+                                    nl(
+                                        js(
+                                            (
+                                                "Команда будет запущена на хосте",
+                                                b(host),
+                                            )
                                         )
                                     )
                                 )
+                                break
+                            else:
+                                self.output.error(js(("Хост", b(host), "не доступен")))
+                                host = self.input.input(
+                                    "Введите имя хоста, на котором будет выполнена команда"
+                                )
+                    if n(host_is_local):
+                        host_is_local = A.SYS.host_is_local(host)
+                    self.write_line(
+                        js(
+                            (
+                                self.get_formatted_given_name(),
+                                "ожидайте окончания выполнения команды...",
                             )
-                            break
-                        else:
-                            self.output.error(js(("Хост", b(host), "не доступен")))
-                            host = self.input.input(
-                                "Введите имя хоста, на котором будет выполнена команда"
-                            )
-                if n(host_is_local):
-                    host_is_local = A.SYS.host_is_local(host)
-                self.write_line(
-                    j(
-                        (
-                            self.get_formatted_given_name(),
-                            "ожидайте окончания выполнения команды...",
                         )
                     )
-                )
-                if use_psexec_executor:
-                    with self.output.make_loading(0.5, "Выролнение команды. Ожидайте"):
-                        process_result = A.EXC.execute(
-                            (
-                                text
-                                if host_is_local
-                                else A.EXC.create_command_for_powershell(
-                                    text,
-                                    host,
-                                    interactive=None,
-                                    run_from_system_account=True,
-                                )
-                            ),
-                            True,
-                            True,
-                            False,
-                        )
-                else:
-                    with self.output.make_loading(0.5, "Выполнение команды. Ожидайте"):
-                        process_result = A.EXC.execute(
-                            A.EXC.create_command_for_executor(text[0], text[1:]),
-                            True,
-                            True,
-                            False,
-                        )
-
-                def decode(value: bytes | None) -> str | None:
-                    if e(value):
-                        return None
-                    return value.decode(A.CT_WINDOWS.CHARSETS.ALTERNATIVE)
+                    if use_psexec_executor:
+                        with self.output.make_loading(
+                            0.5, "Выролнение команды. Ожидайте"
+                        ):
+                            process_result = A.EXC.execute(
+                                (
+                                    A.EXC.create_command_for_powershell(
+                                        command_text_line
+                                    )
+                                    if is_powershell
+                                    else (
+                                        command_text_line
+                                        if host_is_local
+                                        else A.EXC.create_command_for_psexec_powershell(
+                                            command_text_line,
+                                            host,
+                                            interactive=None,
+                                            run_from_system_account=True,
+                                        )
+                                    )
+                                ),  # type: ignore
+                                True,
+                                True,
+                                False,
+                            )
+                    else:
+                        with self.output.make_loading(
+                            0.5, "Выполнение команды. Ожидайте"
+                        ):
+                            process_result = A.EXC.execute(
+                                A.EXC.create_command_for_executor(
+                                    nnl(text)[0], nnl(command_text_line)[1:]
+                                ),
+                                True,
+                                True,
+                                False,
+                            )
 
-                output: str | None = decode(process_result.stdout)
-                error: str | None = decode(process_result.stderr)
-                if ne(output):
-                    self.write_line(output)
-                if ne(error):
-                    self.output.error(error)
+                    def decode(value: bytes | None) -> str | None:
+                        if e(value):
+                            return None
+                        return nnb(value).decode(A.CT_WINDOWS.CHARSETS.ALTERNATIVE)
+
+                    output: str | None = decode(process_result.stdout)
+                    error: str | None = decode(process_result.stderr)
+                    if ne(output):
+                        self.write_line(nns(output))
+                    if ne(error):
+                        self.output.error(error)
         elif command_type == A.CT_CMDT.PYTHON:
             if self.session.is_mobile:
                 while True:
                     command_line_list: list[str] = []
                     line_count: int = 0
                     while e(text):
                         if line_count == 0 or self.yes_no(
@@ -4808,23 +4901,23 @@
                                                 ),
                                                 result,
                                             )
                                 else:
                                     result_title: str = (
                                         title
                                         or self.input.input("Введите название файла")
-                                    ).split(SPLITTER)[-1]
+                                    ).split(A.CT.SPLITTER)[-1]
                                     result_file_path: str = A.PTH.add_extension(
                                         A.PTH.join(A.PTH_MIO.FILES_FOLDER, A.D.uuid()),
                                         A.CT_F_E.EXCEL_NEW,
                                     )
                                     with self.output.make_loading(
                                         0.5, "Идёт создание файла"
                                     ):
-                                        if A.A_D.save_xlsx(
+                                        if A.A_DOC.save_xlsx(
                                             result_title, result, result_file_path
                                         ):
                                             self.output.write_document(
                                                 result_title,
                                                 result_title,
                                                 A.D_CO.file_to_base64(result_file_path),
                                             )
@@ -6452,18 +6545,18 @@
         self.output.write_result(
             A.R.sort(sort_function, A.R_M.free_list(False)),
             False,
             title="Свободные карты доступа:",
         )
 
     def door_close_handler(self, name: str) -> None:
-        A.A_M.door_operation(name, "close")
+        A.A_DR.close(name)
 
     def door_open_handler(self, name: str) -> None:
-        A.A_M.door_operation(name, "open")
+        A.A_DR.open(name)
 
     def get_or_set_variable_handler(self, get_action: bool = False) -> None:
         variable_name: str | None = (
             None
             if self.is_all and (not get_action or self.argless)
             else (
                 self.arg()
@@ -6551,15 +6644,15 @@
                             value = A.D_F.datetime(value)
                         else:
                             group_name = "Переменная"
                     if isinstance(variable_holder, A.CT_S):
                         group_name = "Настройка"
                     if isinstance(variable_holder, A.CT_MR.Types):
                         group_name = "Материальный ресурс"
-                    self.write_line(j((A.CT_V.BULLET, " ", group_name, SPLITTER)))
+                    self.write_line(j((A.CT_V.BULLET, " ", group_name, A.CT.SPLITTER)))
                     with self.output.make_indent(3, True):
                         self.write_line(f"{label_function(variable_holder)}:")
                         self.write_line(js(("Значение: ", b(value))))
 
         if self.is_all:
             with self.output.make_personalized(False):
                 for variable_value_holder in variable_value_holder_list:
@@ -6939,15 +7032,15 @@
                     (
                         b(A.CT_FC.POSITION.caption),
                         if_else(
                             display_only_card_folder_label,
                             lambda: js(("", b("папки"), b(folder))),
                             "",
                         ),
-                        SPLITTER,
+                        A.CT.SPLITTER,
                     )
                 )
             )
             card_folder_first_letter: str | None = folder[0]
             if card_folder_first_letter in A.CT_CR.PLACE_NAME:
                 result_label_list.append(
                     f" {A.CT_V.BULLET} Место: {b(A.CT_CR.PLACE_NAME[card_folder_first_letter])}"
@@ -7441,15 +7534,15 @@
                 self.language_index = index
                 return True
         return False
 
     def parse_arguments(self, line: str) -> list[str]:
         line = line[len(PIH.NAME) :]
         line_part_list: list[str] | None = None
-        line = line.replace(u"\xa0", u" ")
+        line = line.replace("\xa0", " ")
         line_part_list, self.arg_list = A.D.separate_unquoted_and_quoted(line)
         self.comandless_line_part_list = list(line_part_list)
         self.line_part_list = A.D.not_empty_items(line.split(" "))
         line_part_list = A.D.filter(
             lambda item: item.lower() not in (PIH.NAME, PIH.NAME_ALT),
             line_part_list,
         )
```

### Comparing `pih-mio-0.25/MobileHelperService/client.py` & `pih-mio-0.26/MobileHelperService/client.py`

 * *Files identical despite different names*

### Comparing `pih-mio-0.25/MobileHelperService/const.py` & `pih-mio-0.26/MobileHelperService/const.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from enum import Enum, auto
 
 import ipih
 
 from pih import A
 from pih.tools import j, js, b
 from pih.consts.hosts import Hosts
-from pih.consts import SessionFlags, SPLITTER
+from pih.consts import CONST, SessionFlags
 from pih.collections.service import ServiceDescription
 from pih.collections import StorageVariableHolder, IntStorageVariableHolder
 
 
 NAME: str = "MobileHelper"
 
 DEFAULT_COUNT = 100
 ADMIN_ALIAS: str = "admin"
 COUNT_ALIAS: str = "count"
-VERSION: str = "0.25"
+VERSION: str = "0.26"
 
 HOST = Hosts.WS255
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="Mobile helper service",
     host=HOST.NAME,
@@ -48,20 +48,20 @@
 
 class INPUT_TYPE:
     INDEX: int = 1
 
 
 FROM_FILE_REDIRECT_SYMBOL: str = "<"
 FILE_PATTERN_LIST: tuple[str, ...] = (
-    j(("file", SPLITTER)),
+    j(("file", CONST.SPLITTER)),
     FROM_FILE_REDIRECT_SYMBOL,
     "file=",
 )  # type: ignore
 PARAMETER_PATTERN: str = r"\B(\$[\w+а-яА-Я]+)(:[\w \(\)\.\,а-яА-Я]+)?"
-
+PARAMETER_PATTERN_FOR_CMD: str = r"\B(@[\w+а-яА-Я]+)(:[\w \(\)\.\,а-яА-Я]+)?"
 Groups = A.CT_AD.Groups
 
 MAX_MESSAGE_LINE_LENGTH = 12
 
 
 class MessageType(Enum):
     SEPARATE_ONCE = auto()
```

### Comparing `pih-mio-0.25/MobileHelperService/service.py` & `pih-mio-0.26/MobileHelperService/service.py`

 * *Files identical despite different names*

### Comparing `pih-mio-0.25/MobileHelperService/service_api.py` & `pih-mio-0.26/MobileHelperService/service_api.py`

 * *Files identical despite different names*

