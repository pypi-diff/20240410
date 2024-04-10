# Comparing `tmp/pih-plb_ntf-0.13.tar.gz` & `tmp/pih-plb_ntf-0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-plb_ntf-0.13.tar", last modified: Wed Mar 13 14:38:51 2024, max compression
+gzip compressed data, was "pih-plb_ntf-0.14.tar", last modified: Wed Apr 10 02:16:36 2024, max compression
```

## Comparing `pih-plb_ntf-0.13.tar` & `pih-plb_ntf-0.14.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-13 14:38:51.717752 pih-plb_ntf-0.13/
--rw-rw-rw-   0        0        0      292 2024-03-13 14:38:51.686473 pih-plb_ntf-0.13/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-13 14:38:51.327115 pih-plb_ntf-0.13/PolibasePersonNotificationService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-plb_ntf-0.13/PolibasePersonNotificationService/__init__.py
--rw-rw-rw-   0        0        0      168 2024-02-15 00:16:15.000000 pih-plb_ntf-0.13/PolibasePersonNotificationService/__main__.py
--rw-rw-rw-   0        0        0     1646 2024-02-16 04:43:00.000000 pih-plb_ntf-0.13/PolibasePersonNotificationService/api.py
--rw-rw-rw-   0        0        0      535 2024-03-13 12:18:39.000000 pih-plb_ntf-0.13/PolibasePersonNotificationService/const.py
--rw-rw-rw-   0        0        0    23594 2024-03-13 12:22:09.000000 pih-plb_ntf-0.13/PolibasePersonNotificationService/service.py
-drwxrwxrwx   0        0        0        0 2024-03-13 14:38:51.639592 pih-plb_ntf-0.13/pih_plb_ntf.egg-info/
--rw-rw-rw-   0        0        0      292 2024-03-13 14:38:50.000000 pih-plb_ntf-0.13/pih_plb_ntf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      432 2024-03-13 14:38:51.000000 pih-plb_ntf-0.13/pih_plb_ntf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-13 14:38:50.000000 pih-plb_ntf-0.13/pih_plb_ntf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2024-03-13 14:38:50.000000 pih-plb_ntf-0.13/pih_plb_ntf.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-03-13 14:38:50.000000 pih-plb_ntf-0.13/pih_plb_ntf.egg-info/requires.txt
--rw-rw-rw-   0        0        0       34 2024-03-13 14:38:50.000000 pih-plb_ntf-0.13/pih_plb_ntf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-13 14:38:51.733341 pih-plb_ntf-0.13/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 02:16:36.373781 pih-plb_ntf-0.14/
+-rw-rw-rw-   0        0        0      292 2024-04-10 02:16:36.342532 pih-plb_ntf-0.14/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-10 02:16:35.981029 pih-plb_ntf-0.14/PolibasePersonNotificationService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-plb_ntf-0.14/PolibasePersonNotificationService/__init__.py
+-rw-rw-rw-   0        0        0      168 2024-02-15 00:16:15.000000 pih-plb_ntf-0.14/PolibasePersonNotificationService/__main__.py
+-rw-rw-rw-   0        0        0     1629 2024-04-09 22:48:15.000000 pih-plb_ntf-0.14/PolibasePersonNotificationService/api.py
+-rw-rw-rw-   0        0        0      431 2024-04-09 22:44:24.000000 pih-plb_ntf-0.14/PolibasePersonNotificationService/const.py
+-rw-rw-rw-   0        0        0    19929 2024-04-09 22:37:16.000000 pih-plb_ntf-0.14/PolibasePersonNotificationService/service.py
+drwxrwxrwx   0        0        0        0 2024-04-10 02:16:36.311285 pih-plb_ntf-0.14/pih_plb_ntf.egg-info/
+-rw-rw-rw-   0        0        0      292 2024-04-10 02:16:35.000000 pih-plb_ntf-0.14/pih_plb_ntf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      432 2024-04-10 02:16:35.000000 pih-plb_ntf-0.14/pih_plb_ntf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 02:16:35.000000 pih-plb_ntf-0.14/pih_plb_ntf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2024-04-10 02:16:35.000000 pih-plb_ntf-0.14/pih_plb_ntf.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-04-10 02:16:35.000000 pih-plb_ntf-0.14/pih_plb_ntf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       34 2024-04-10 02:16:35.000000 pih-plb_ntf-0.14/pih_plb_ntf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 02:16:36.389407 pih-plb_ntf-0.14/setup.cfg
```

### Comparing `pih-plb_ntf-0.13/PolibasePersonNotificationService/api.py` & `pih-plb_ntf-0.14/PolibasePersonNotificationService/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import ipih
 
 from pih import A
 from pih.tools import ne
 
-# version 0.1
-
 from pih.collections import (
     WhatsAppMessage,
     PolibasePersonNotificationConfirmation as PPNC,
 )
 
 
 class PolibasePersonNotificationApi:
```

### Comparing `pih-plb_ntf-0.13/PolibasePersonNotificationService/service.py` & `pih-plb_ntf-0.14/PolibasePersonNotificationService/service.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import ipih
 
 from pih import A, PIHThread, serve, subscribe_on
 from PolibasePersonNotificationService.const import SD
 
-# version 0.2
 SC = A.CT_SC
 
 ISOLATED: bool = False
 
 
 def start(as_standalone: bool = False) -> None:
 
@@ -22,40 +21,36 @@
     )
     from pih.consts.polibase import (
         PolibasePersonVisitStatus,
         PolibasePersonVisitNotificationType as PPVNType,
     )
     from pih.collections import (
         Result,
-        Message,
-        PolibasePerson,
-        WhatsAppMessage,
         DelayedMessageDS,
-        BonusInformation,
         MessageSearchCritery,
         DelayedMessage as DM,
         PolibasePersonVisitDS as PPVDS,
         PolibasePersonVisitNotification as PPVN,
-        PolibasePersonVisitNotificationDS as PPVNVO,
-        PolibasePersonNotificationConfirmation as PPNC,
+        PolibasePersonVisitNotificationDS as PPVNDS,
     )
     from pih.tools import (
-        ParameterList,
-        FullNameTool,
-        while_not_do,
+        j,
         e,
-        ne,
         n,
+        b,
+        ne,
         nn,
-        j,
         js,
-        b,
         nl,
-        one,
-        esc,
+        nns,
+        nni,
+        nndt,
+        FullNameTool,
+        while_not_do,
+        ParameterList,
     )
     from PolibasePersonNotificationService.api import (
         PolibasePersonNotificationApi as Api,
     )
 
     SENDER: str = A.D.get(A.CT_ME_WH_W.Profiles.CALL_CENTRE)
 
@@ -80,19 +75,19 @@
             MessageStatuses.REGISTERED, datetime
         )
         DH.message_stack += A.R_ME_D.get(search_critery, True).data or []
         search_critery.date = ""
         DH.message_stack += A.R_ME_D.get(search_critery, True).data or []
 
     def send_delayed_message(message: DelayedMessageDS) -> bool:
-        sender: str = message.sender
+        sender: str = nns(message.sender)
         has_notification_confirmation: bool = A.C_P_N_С.exists(
-            message.recipient, sender, True
+            nns(message.recipient), sender, True
         )
-        message_id: int = message.id
+        message_id: int = nni(message.id)
         if nn(message_id):
             person_visit_notification: PPVN | None = A.R_P_N.by_message_id(
                 message_id
             ).data
             if nn(person_visit_notification):
                 person_visit: PPVDS = A.R_P_V.by_id(
                     person_visit_notification.visitID
@@ -172,15 +167,15 @@
                             )
                         else:
                             message_text = A.S.get(
                                 A.CT_S.POLIBASE_PERSON_VISIT_GREETING_NOTIFICATION_TEXT_WITHOUT_DATE_FOR_CONFIRMED_NOTIFICATION
                                 if has_notification_confirmation
                                 else A.CT_S.POLIBASE_PERSON_VISIT_GREETING_NOTIFICATION_TEXT_WITHOUT_DATE
                             )
-                            message_text = message_text.format(
+                            message_text = nns(message_text).format(
                                 name=person_name,
                                 appointment_information=appointment_information,
                             )
                     elif type == PPVNType.REMINDER:
                         if person_visit.status == PolibasePersonVisitStatus.CONFIRMED:
                             visit_date_time: datetime = A.D.datetime_from_string(
                                 person_visit.beginDate, A.CT.ISO_DATETIME_FORMAT
@@ -227,84 +222,14 @@
         return False
 
     def server_call_handler(sc: SC, pl: ParameterList) -> bool | None:
         if sc == SC.heart_beat:
             fetch_delayed_messages(A.D_Ex.parameter_list(pl).get())
             heat_beat_handler()
             return True
-        if sc == SC.send_event:
-            event: A.CT_E = A.D_Ex_E.get(pl)
-            if event == A.CT_E.WHATSAPP_MESSAGE_RECEIVED:
-                message: WhatsAppMessage | None = A.D_Ex_E.whatsapp_message(pl)
-                if ne(message):
-                    sender: str = message.profile_id
-                    if sender == SENDER:
-                        telephone_number: str = A.D_F.telephone_number_international(
-                            message.sender
-                        )
-                        notification_confirmation: PPNC | None = A.R_P_N_C.by(
-                            telephone_number, sender
-                        ).data
-                        if (
-                            ne(notification_confirmation)
-                            and notification_confirmation.status == 2
-                        ):
-                            full_name: str | None = one(
-                                A.R_P_V_DS.search(
-                                    PPVDS(
-                                        telephoneNumber=A.D_F.telephone_number(
-                                            telephone_number
-                                        )
-                                    )
-                                )
-                            ).FullName
-                            if A.A_P_N_C.update(telephone_number, sender, 1):
-                                A.ME_WH_W_Q.add_message(
-                                    Message(
-                                        A.S_P_V.offer_telegram_bot_url_text(full_name),
-                                        telephone_number,
-                                        sender,
-                                    )
-                                )
-                                A.ME_WH_W_Q.add_message(
-                                    Message(
-                                        A.CT_P.TELEGRAM_BOT_URL,
-                                        telephone_number,
-                                        sender,
-                                    )
-                                )
-                                A.L.polibase(
-                                    js(
-                                        (
-                                            "Пациент:",
-                                            full_name,
-                                            j(("(", telephone_number, ")")),
-                                            "ответил:",
-                                            esc(message.message),
-                                            "на получение ссылки",
-                                        )
-                                    )
-                                )
-            elif event == A.CT_E.POLIBASE_PERSON_BONUSES_WAS_UPDATED:
-                polibase_person_pin: int = A.D_Ex_E.parameters(pl)[0]
-                bonus_information: BonusInformation = one(
-                    A.R_P.bonus_information(polibase_person_pin)
-                )
-                A.L.polibase(
-                    js(
-                        (
-                            "Для клиента:",
-                            polibase_person_pin,
-                            "обновлены бонусы:",
-                            bonus_information.last,
-                            "из",
-                            bonus_information.active,
-                        )
-                    )
-                )
         return None
 
     def complete_buffered_message_sending_action(message: DelayedMessageDS) -> bool:
         message_id: int | None = message.id
         if e(message_id):
             A.L.polibase(
                 j(
@@ -365,15 +290,14 @@
                         A.CT_L_ME_F.ERROR,
                     )
             else:
                 sleep(1)
 
     def service_starts_handler() -> None:
         subscribe_on(SC.heart_beat)
-        subscribe_on(SC.send_event)
         search_critery: MessageSearchCritery = create_message_search_critery(
             MessageStatuses.AT_WORK
         )
         DH.message_stack += A.R_ME_D.get(search_critery).data or []
         search_critery.date = ""
         search_critery.status = A.D.get(MessageStatuses.REGISTERED)
         DH.message_stack += A.R_ME_D.get(search_critery, True).data or []
@@ -385,16 +309,16 @@
             A.R_P_V_DS.last().data, lambda item: item.id
         )
         visit_list_result: Result[list[PPVDS]] | None = None
         if n(last_visit_id):
             visit_list_result = A.R_P_V.today()
         else:
             visit_list_result = A.R_P_V.after_id(last_visit_id)
-        if not A.R.is_empty(visit_list_result):
-            visit_map: dict[list] = defaultdict(list)
+        if ne(visit_list_result):
+            visit_map: dict[str | int, list] = defaultdict(list)
 
             def fill_person_visits_map(visit: PPVDS) -> None:
                 if visit.pin == A.CT_P.PRERECORDING_PIN:
                     visit_map[visit.telephoneNumber].append(visit)
                 else:
                     visit_map[visit.pin].append(visit)
 
@@ -424,54 +348,56 @@
     def new_person_visit_action(visit: PPVDS) -> None:
         def set_visit_notification_unique_property(
             visit: PPVDS, notification: PPVN
         ) -> None:
             notification.telephoneNumber = visit.telephoneNumber
 
         result_visit_ds: Result[PPVDS] = A.R_P_V_DS.search(PPVDS(id=visit.id))
-        if not A.R.is_empty(result_visit_ds):
+        if ne(result_visit_ds):
             A.L.polibase(j(("Визит-дубликат: ", visit, nl(), result_visit_ds.data)))
         if A.A_P_V_DS.update(visit):
             if visit.status == PolibasePersonVisitStatus.CANCELED:
                 return
             telephone_number: str | None = visit.telephoneNumber
             if nn(telephone_number) and A.C.telephone_number(telephone_number):
                 telephone_number = A.D_F.telephone_number_international(
                     telephone_number
                 )
                 Api.check_for_notification_confirmation(telephone_number, SENDER)
                 A.E.polibase_person_visit_was_registered(visit)
                 type_value: int | None = None
-                visit_notification: PPVN | None = None
+                visit_notification: PPVNDS
                 visit_notification_check_for_unique_per_date: PPVN | None = None
                 message: DM = DM(None, telephone_number, SENDER)
                 if A.S.get(
                     A.CT_S.POLIBASE_PERSON_VISIT_NEED_REGISTER_GREETING_NOTIFICATION
                 ):
                     type_value = A.D.get(PPVNType.GREETING)
                     visit_notification_check_for_unique_per_date = PPVN(
                         type=type_value,
                         registrationDate=A.D.to_date_string(visit.registrationDate),
                     )
                     set_visit_notification_unique_property(
                         visit, visit_notification_check_for_unique_per_date
                     )
                     if not A.C_P_N.exists(visit_notification_check_for_unique_per_date):
-                        visit_notification = PPVNVO(
+                        visit_notification = PPVNDS(
                             visit.id, A.ME_D.register(message), type_value
                         )
                         if A.A_P_N.register(visit_notification):
                             A.E.polibase_person_visit_notification_was_registered(
                                 visit, visit_notification
                             )
                     else:
-                        if A.D.now() <= A.D.datetime_from_string(
-                            visit.beginDate, A.CT.ISO_DATETIME_FORMAT
+                        if A.D.now() <= nndt(
+                            A.D.datetime_from_string(
+                                visit.beginDate, A.CT.ISO_DATETIME_FORMAT
+                            )
                         ):
-                            visit_notification = PPVNVO(
+                            visit_notification = PPVNDS(
                                 visit.id,
                                 A.ME_D.register(message),
                                 PPVNType.DEFAULT.value,
                             )
                             if A.A_P_N.register(visit_notification):
                                 A.E.polibase_person_visit_notification_was_registered(
                                     visit, visit_notification
@@ -494,15 +420,15 @@
                             visit.beginDate
                         ) - timedelta(
                             minutes=A.S.get(
                                 A.CT_S.POLIBASE_PERSON_VISIT_TIME_BEFORE_REMINDER_NOTIFICATION_IN_MINUTES
                             )
                         )
                         if A.D.now() < message.date:
-                            visit_notification = PPVNVO(
+                            visit_notification = PPVNDS(
                                 visit.id, A.ME_D.register(message), type_value
                             )
                             if A.A_P_N.register(visit_notification):
                                 A.E.polibase_person_visit_notification_was_registered(
                                     visit, visit_notification
                                 )
                         else:
```

