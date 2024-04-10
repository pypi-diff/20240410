# Comparing `tmp/pih-mail-0.14.tar.gz` & `tmp/pih-mail-0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-mail-0.14.tar", last modified: Fri Mar 29 06:22:03 2024, max compression
+gzip compressed data, was "pih-mail-0.15.tar", last modified: Wed Apr 10 01:44:33 2024, max compression
```

## Comparing `pih-mail-0.14.tar` & `pih-mail-0.15.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 06:22:03.894349 pih-mail-0.14/
-drwxrwxrwx   0        0        0        0 2024-03-29 06:22:03.449463 pih-mail-0.14/MailService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-mail-0.14/MailService/__init__.py
--rw-rw-rw-   0        0        0      146 2024-02-15 01:08:42.000000 pih-mail-0.14/MailService/__main__.py
--rw-rw-rw-   0        0        0        2 2023-07-09 01:12:40.000000 pih-mail-0.14/MailService/api.py
--rw-rw-rw-   0        0        0     1203 2024-03-29 05:33:30.000000 pih-mail-0.14/MailService/const.py
--rw-rw-rw-   0        0        0    10183 2024-03-29 05:33:12.000000 pih-mail-0.14/MailService/service.py
--rw-rw-rw-   0        0        0      318 2024-03-29 06:22:03.843316 pih-mail-0.14/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-29 06:22:03.811498 pih-mail-0.14/pih_mail.egg-info/
--rw-rw-rw-   0        0        0      318 2024-03-29 06:22:02.000000 pih-mail-0.14/pih_mail.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2024-03-29 06:22:03.000000 pih-mail-0.14/pih_mail.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 06:22:03.000000 pih-mail-0.14/pih_mail.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-03-29 06:22:03.000000 pih-mail-0.14/pih_mail.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2024-03-29 06:22:03.000000 pih-mail-0.14/pih_mail.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-29 06:22:03.000000 pih-mail-0.14/pih_mail.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-29 06:22:03.909336 pih-mail-0.14/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 01:44:33.927933 pih-mail-0.15/
+drwxrwxrwx   0        0        0        0 2024-04-10 01:44:33.521534 pih-mail-0.15/MailService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-mail-0.15/MailService/__init__.py
+-rw-rw-rw-   0        0        0      146 2024-02-15 01:08:42.000000 pih-mail-0.15/MailService/__main__.py
+-rw-rw-rw-   0        0        0        2 2023-07-09 01:12:40.000000 pih-mail-0.15/MailService/api.py
+-rw-rw-rw-   0        0        0     1203 2024-04-10 00:27:27.000000 pih-mail-0.15/MailService/const.py
+-rw-rw-rw-   0        0        0    10167 2024-04-09 23:26:12.000000 pih-mail-0.15/MailService/service.py
+-rw-rw-rw-   0        0        0      318 2024-04-10 01:44:33.865411 pih-mail-0.15/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-10 01:44:33.844767 pih-mail-0.15/pih_mail.egg-info/
+-rw-rw-rw-   0        0        0      318 2024-04-10 01:44:32.000000 pih-mail-0.15/pih_mail.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2024-04-10 01:44:33.000000 pih-mail-0.15/pih_mail.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 01:44:33.000000 pih-mail-0.15/pih_mail.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-04-10 01:44:33.000000 pih-mail-0.15/pih_mail.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2024-04-10 01:44:33.000000 pih-mail-0.15/pih_mail.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-10 01:44:33.000000 pih-mail-0.15/pih_mail.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 01:44:33.927933 pih-mail-0.15/setup.cfg
```

### Comparing `pih-mail-0.14/MailService/const.py` & `pih-mail-0.15/MailService/const.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 NAME: str = "Mail"
 SECTION: str = "MailboxInfo"
 
 HOST = Hosts.WS255
 
 # 0.1 - Persistance caching for email address deliverability checking status and  recall for email deliverability checking if status == UNKNOWN
 # 0.12 - using new method for checking mail deliverity
-VERSION: str = "0.14"
+VERSION: str = "0.15"
 
 TIMEOUT: int = 10
 TRY_AGAIN_COUNT: int = 5
 TRY_AGAIN_SLEEP_TIME: int = 1
 PACKAGES: tuple[str, ...] = (
     "imap_tools",
     "dnspython",
```

### Comparing `pih-mail-0.14/MailService/service.py` & `pih-mail-0.15/MailService/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import ipih
 
 from pih import A
 from MailService.const import *
 from pih.collections import MailboxInfo, NewMailMessage
 from pih.tools import ne, j, n, e, nn, lw, one, nnd, nns, nna
-from pih.consts import EmailVerificationMethods, EMAIL_SPLITTER, CHARSETS
+from pih.consts import EmailVerificationMethods, CHARSETS
 
 import smtplib
 import dns.resolver
 from time import sleep
 from typing import Any
 
 SC = A.CT_SC
@@ -118,15 +118,15 @@
                 method: str = pl.next()
                 cached: bool = pl.next()
                 result: bool | None = (
                     one(A.R_DS.value(email_address, None, SECTION_DELIVERITY)) if cached else None
                 )
                 if nn(result):
                     return result
-                domain: str = email_address.split(EMAIL_SPLITTER)[1]
+                domain: str = email_address.split(A.CT.EMAIL_SPLITTER)[1]
                 if check_email_accessibility and method == A.D.get(
                     EmailVerificationMethods.NORMAL
                 ):
                     server = smtplib.SMTP()
                     server.set_debuglevel(0)
                     server.connect(str(dns.resolver.resolve(domain, "MX")[0].exchange))
                     server.helo(server.local_hostname)
@@ -149,15 +149,15 @@
                                     "&email=",
                                     email_address,
                                 )
                             ),
                             timeout=TIMEOUT,
                         )
                         if response.status_code == 200:
-                            content = A.D.rpc_unrepresent(
+                            content = A.D.rpc_decode(
                                 response.content.decode(CHARSETS.UTF8)
                             )
                             email_deliverability_status = nnd(content)[
                                 EMAIL_STATUS_FIELD
                             ]
                         else:
                             sleep(TRY_AGAIN_SLEEP_TIME)
```

