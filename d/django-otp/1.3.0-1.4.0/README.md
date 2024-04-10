# Comparing `tmp/django_otp-1.3.0.tar.gz` & `tmp/django_otp-1.4.0.tar.gz`

## Comparing `django_otp-1.3.0.tar` & `django_otp-1.4.0.tar`

### file list

```diff
@@ -1,103 +1,107 @@
--rw-r--r--   0        0        0    17689 2020-02-02 00:00:00.000000 django_otp-1.3.0/CHANGES.rst
--rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 django_otp-1.3.0/CONTRIBUTING.rst
--rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 django_otp-1.3.0/docs/Makefile
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 django_otp-1.3.0/docs/ext/otpdocs.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 django_otp-1.3.0/docs/source/.spell.utf-8.add
--rw-r--r--   0        0        0     8628 2020-02-02 00:00:00.000000 django_otp-1.3.0/docs/source/auth.rst
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_otp-1.3.0/docs/source/changes.rst
--rw-r--r--   0        0        0     8817 2020-02-02 00:00:00.000000 django_otp-1.3.0/docs/source/conf.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 django_otp-1.3.0/docs/source/contributing.rst
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 django_otp-1.3.0/docs/source/extend.rst
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 django_otp-1.3.0/docs/source/index.rst
--rw-r--r--   0        0        0    19957 2020-02-02 00:00:00.000000 django_otp-1.3.0/docs/source/overview.rst
--rw-r--r--   0        0        0     5368 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/__init__.py
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/admin.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/conf.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/decorators.py
--rw-r--r--   0        0        0    13503 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/forms.py
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/middleware.py
--rw-r--r--   0        0        0    17340 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/models.py
--rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/oath.py
--rw-r--r--   0        0        0    20302 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/tests.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/util.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/views.py
--rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3362 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/locale/pt_BR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/locale/pt_PT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/locale/pt_PT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/__init__.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_email/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_email/admin.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_email/apps.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_email/conf.py
--rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_email/models.py
--rw-r--r--   0        0        0     8981 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_email/tests.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_email/migrations/0001_initial.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_email/migrations/0002_sidechanneldevice_email.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_email/migrations/0003_emaildevice_email.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_email/migrations/0004_throttling.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_email/migrations/0005_emaildevice_last_generated_timestamp.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_email/migrations/__init__.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_email/templates/otp/email/token.txt
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_hotp/__init__.py
--rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_hotp/admin.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_hotp/apps.py
--rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_hotp/models.py
--rw-r--r--   0        0        0    13359 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_hotp/tests.py
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_hotp/migrations/0001_initial.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_hotp/migrations/0002_auto_20190420_0723.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_hotp/migrations/__init__.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_hotp/templates/otp_hotp/admin/config.html
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_static/__init__.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_static/admin.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_static/apps.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_static/lib.py
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_static/models.py
--rw-r--r--   0        0        0     8047 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_static/tests.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_static/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_static/management/commands/__init__.py
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_static/management/commands/addstatictoken.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_static/migrations/0001_initial.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_static/migrations/0002_throttling.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_static/migrations/__init__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_totp/__init__.py
--rw-r--r--   0        0        0     4759 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_totp/admin.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_totp/apps.py
--rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_totp/models.py
--rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_totp/tests.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_totp/migrations/0001_initial.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_totp/migrations/0002_auto_20190420_0723.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_totp/migrations/__init__.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/plugins/otp_totp/templates/otp_totp/admin/config.html
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 django_otp-1.3.0/src/django_otp/templates/otp/admin111/login.html
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 django_otp-1.3.0/test/config/github.toml
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 django_otp-1.3.0/test/config/sample.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.3.0/test/test_project/__init__.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 django_otp-1.3.0/test/test_project/backends.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 django_otp-1.3.0/test/test_project/config.py
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 django_otp-1.3.0/test/test_project/settings.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 django_otp-1.3.0/test/test_project/urls.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 django_otp-1.3.0/test/test_project/views.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 django_otp-1.3.0/test/test_project/templates/about.html
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 django_otp-1.3.0/test/test_project/templates/home.html
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 django_otp-1.3.0/test/test_project/templates/navbar.html
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 django_otp-1.3.0/test/test_project/templates/root.html
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 django_otp-1.3.0/test/test_project/templates/bs5/input.html
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 django_otp-1.3.0/test/test_project/templates/bs5/select.html
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 django_otp-1.3.0/test/test_project/templates/otp/email/custom.txt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 django_otp-1.3.0/test/test_project/templates/otp/email/custom_html.html
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 django_otp-1.3.0/test/test_project/templates/otp/email/token.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.3.0/test/test_project/templates/registration/logged_out.html
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 django_otp-1.3.0/test/test_project/templates/registration/login.html
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 django_otp-1.3.0/.gitignore
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 django_otp-1.3.0/.hgignore
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 django_otp-1.3.0/LICENSE
--rw-r--r--   0        0        0     6532 2020-02-02 00:00:00.000000 django_otp-1.3.0/README.rst
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 django_otp-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     7486 2020-02-02 00:00:00.000000 django_otp-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    18115 2020-02-02 00:00:00.000000 django_otp-1.4.0/CHANGES.rst
+-rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 django_otp-1.4.0/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 django_otp-1.4.0/docs/Makefile
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 django_otp-1.4.0/docs/ext/otpdocs.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 django_otp-1.4.0/docs/source/.spell.utf-8.add
+-rw-r--r--   0        0        0     8628 2020-02-02 00:00:00.000000 django_otp-1.4.0/docs/source/auth.rst
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_otp-1.4.0/docs/source/changes.rst
+-rw-r--r--   0        0        0     8817 2020-02-02 00:00:00.000000 django_otp-1.4.0/docs/source/conf.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 django_otp-1.4.0/docs/source/contributing.rst
+-rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 django_otp-1.4.0/docs/source/extend.rst
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 django_otp-1.4.0/docs/source/index.rst
+-rw-r--r--   0        0        0    19957 2020-02-02 00:00:00.000000 django_otp-1.4.0/docs/source/overview.rst
+-rw-r--r--   0        0        0     5368 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/__init__.py
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/admin.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/conf.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/decorators.py
+-rw-r--r--   0        0        0    13503 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/forms.py
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/middleware.py
+-rw-r--r--   0        0        0    19417 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/models.py
+-rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/oath.py
+-rw-r--r--   0        0        0    24238 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/tests.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/util.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/views.py
+-rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3362 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/locale/pt_PT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/locale/pt_PT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/__init__.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_email/__init__.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_email/admin.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_email/apps.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_email/conf.py
+-rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_email/models.py
+-rw-r--r--   0        0        0     9285 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_email/tests.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_email/migrations/0001_initial.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_email/migrations/0002_sidechanneldevice_email.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_email/migrations/0003_emaildevice_email.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_email/migrations/0004_throttling.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_email/migrations/0005_emaildevice_last_generated_timestamp.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_email/migrations/0006_add_timestamps.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_email/migrations/__init__.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_email/templates/otp/email/token.txt
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_hotp/__init__.py
+-rw-r--r--   0        0        0     5013 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_hotp/admin.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_hotp/apps.py
+-rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_hotp/models.py
+-rw-r--r--   0        0        0    13619 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_hotp/tests.py
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_hotp/migrations/0001_initial.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_hotp/migrations/0002_auto_20190420_0723.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_hotp/migrations/0003_add_timestamps.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_hotp/migrations/__init__.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_hotp/templates/otp_hotp/admin/config.html
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_static/__init__.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_static/admin.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_static/apps.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_static/lib.py
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_static/models.py
+-rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_static/tests.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_static/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_static/management/commands/__init__.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_static/management/commands/addstatictoken.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_static/migrations/0001_initial.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_static/migrations/0002_throttling.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_static/migrations/0003_add_timestamps.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_static/migrations/__init__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_totp/__init__.py
+-rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_totp/admin.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_totp/apps.py
+-rw-r--r--   0        0        0     5848 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_totp/models.py
+-rw-r--r--   0        0        0    12086 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_totp/tests.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_totp/migrations/0001_initial.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_totp/migrations/0002_auto_20190420_0723.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_totp/migrations/0003_add_timestamps.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_totp/migrations/__init__.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/plugins/otp_totp/templates/otp_totp/admin/config.html
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 django_otp-1.4.0/src/django_otp/templates/otp/admin111/login.html
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 django_otp-1.4.0/test/config/github.toml
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 django_otp-1.4.0/test/config/sample.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.4.0/test/test_project/__init__.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 django_otp-1.4.0/test/test_project/backends.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 django_otp-1.4.0/test/test_project/config.py
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 django_otp-1.4.0/test/test_project/settings.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 django_otp-1.4.0/test/test_project/urls.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 django_otp-1.4.0/test/test_project/views.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 django_otp-1.4.0/test/test_project/templates/about.html
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 django_otp-1.4.0/test/test_project/templates/home.html
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 django_otp-1.4.0/test/test_project/templates/navbar.html
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 django_otp-1.4.0/test/test_project/templates/root.html
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 django_otp-1.4.0/test/test_project/templates/bs5/input.html
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 django_otp-1.4.0/test/test_project/templates/bs5/select.html
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 django_otp-1.4.0/test/test_project/templates/otp/email/custom.txt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 django_otp-1.4.0/test/test_project/templates/otp/email/custom_html.html
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 django_otp-1.4.0/test/test_project/templates/otp/email/token.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_otp-1.4.0/test/test_project/templates/registration/logged_out.html
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 django_otp-1.4.0/test/test_project/templates/registration/login.html
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 django_otp-1.4.0/.gitignore
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 django_otp-1.4.0/.hgignore
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 django_otp-1.4.0/LICENSE
+-rw-r--r--   0        0        0     6532 2020-02-02 00:00:00.000000 django_otp-1.4.0/README.rst
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 django_otp-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     7486 2020-02-02 00:00:00.000000 django_otp-1.4.0/PKG-INFO
```

### Comparing `django_otp-1.3.0/CHANGES.rst` & `django_otp-1.4.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+v1.4.0 - April 09, 2024 - Add TimestampMixin
+--------------------------------------------------------------------------------
+
+- `#137`_: Add TimestampMixin
+
+  Add a new TimestampMixin with ``created_at`` and ``last_used_at`` fields for
+  device models.
+
+  All builtin plugins now have these timestamp fields and require migrating.
+
+- Some documentation cleanup.
+
+.. _#137: https://github.com/django-otp/django-otp/pull/137
+
+
 v1.3.0 - November 08, 2023 - Support cooldowns for token generation
 --------------------------------------------------------------------------------
 
 - `#122`_: Added throttling to token generation.
 
   Devices that generate random tokens can take advantage of the new
   :class:`~django_otp.models.CooldownMixin` to enforce limits on how frequently
```

### Comparing `django_otp-1.3.0/CONTRIBUTING.rst` & `django_otp-1.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/docs/Makefile` & `django_otp-1.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/docs/source/.spell.utf-8.add` & `django_otp-1.4.0/docs/source/.spell.utf-8.add`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/docs/source/auth.rst` & `django_otp-1.4.0/docs/source/auth.rst`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/docs/source/conf.py` & `django_otp-1.4.0/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 #  copyright = ''
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The full version, including alpha/beta/rc tags.
-release = '1.3.0'
+release = '1.4.0'
 
 # The short X.Y version.
 version = '.'.join(release.split('.')[:2])
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
```

### Comparing `django_otp-1.3.0/docs/source/extend.rst` & `django_otp-1.4.0/docs/source/extend.rst`

 * *Files 6% similar despite different names*

```diff
@@ -75,14 +75,17 @@
 
 .. autoclass:: django_otp.models.CooldownMixin
    :members: get_cooldown_duration, generate_is_allowed, cooldown_reset, cooldown_set
 
 .. autoclass:: django_otp.models.ThrottlingMixin
    :members: get_throttle_factor, verify_is_allowed, throttle_reset, throttle_increment
 
+.. autoclass:: django_otp.models.TimestampMixin
+   :members: set_last_used_timestamp
+
 
 .. _utilities:
 
 Utilities
 ---------
 
 django_otp provides several low-level utilities as a convenience to plugin
```

### Comparing `django_otp-1.3.0/docs/source/overview.rst` & `django_otp-1.4.0/docs/source/overview.rst`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/src/django_otp/__init__.py` & `django_otp-1.4.0/src/django_otp/__init__.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/src/django_otp/admin.py` & `django_otp-1.4.0/src/django_otp/admin.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/src/django_otp/conf.py` & `django_otp-1.4.0/src/django_otp/conf.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/src/django_otp/decorators.py` & `django_otp-1.4.0/src/django_otp/decorators.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/src/django_otp/forms.py` & `django_otp-1.4.0/src/django_otp/forms.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/src/django_otp/middleware.py` & `django_otp-1.4.0/src/django_otp/middleware.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/src/django_otp/models.py` & `django_otp-1.4.0/src/django_otp/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
         :param user: The user.
         :type user: :class:`~django.contrib.auth.models.User`
 
         :param confirmed: If ``None``, all matching devices are returned.
             Otherwise, this can be any true or false value to limit the query
             to confirmed or unconfirmed devices, respectively.
+
         """
         devices = self.model.objects.filter(user=user)
         if confirmed is not None:
             devices = devices.filter(confirmed=bool(confirmed))
 
         return devices
 
@@ -68,14 +69,15 @@
         individual deployments can force it to ``False`` if they wish to create
         a device and then ask the user for confirmation. As a rule, built-in
         APIs that enumerate devices will only include those that are confirmed.
 
     .. attribute:: objects
 
         A :class:`~django_otp.models.DeviceManager`.
+
     """
 
     user = models.ForeignKey(
         getattr(settings, 'AUTH_USER_MODEL', 'auth.User'),
         help_text="The user that this device belongs to.",
         on_delete=models.CASCADE,
     )
@@ -146,61 +148,68 @@
         except (ValueError, LookupError):
             pass
 
         return device
 
     def is_interactive(self):
         """
-        Returns ``True`` if this is an interactive device. The default
-        implementation returns ``True`` if
+        Returns ``True`` if this is an interactive device.
+
+        The default implementation returns ``True`` if
         :meth:`~django_otp.models.Device.generate_challenge` has been
         overridden, but subclasses are welcome to provide smarter
         implementations.
 
         :rtype: bool
+
         """
         return not hasattr(self.generate_challenge, 'stub')
 
     def generate_is_allowed(self):
         """
-        Checks whether it is permissible to call :meth:`generate_challenge`. If
-        it is allowed, returns ``(True, None)``. Otherwise returns ``(False,
+        Checks whether it is permissible to call :meth:`generate_challenge`.
+
+        If it is allowed, returns ``(True, None)``. Otherwise returns ``(False,
         data_dict)``, where ``data_dict`` contains extra information, defined
         by the implementation.
 
         This method can be used to implement throttling of token generation for
-        interactive devices. Client code should check this method before calling
-        :meth:`generate_challenge` and report problems to the user.
+        interactive devices. Client code should check this method before
+        calling :meth:`generate_challenge` and report problems to the user.
+
         """
         return (True, None)
 
     def generate_challenge(self):
         """
         Generates a challenge value that the user will need to produce a token.
+
         This method is permitted to have side effects, such as transmitting
         information to the user through some other channel (email or SMS,
-        perhaps). And, of course, some devices may need to commit the
-        challenge to the database.
+        perhaps). And, of course, some devices may need to commit the challenge
+        to the database.
 
         :returns: A message to the user. This should be a string that fits
             comfortably in the template ``'OTP Challenge: {0}'``. This may
             return ``None`` if this device is not interactive.
         :rtype: string or ``None``
 
         :raises: Any :exc:`~exceptions.Exception` is permitted. Callers should
             trap ``Exception`` and report it to the user.
+
         """
         return None
 
     generate_challenge.stub = True
 
     def verify_is_allowed(self):
         """
-        Checks whether it is permissible to call :meth:`verify_token`. If it is
-        allowed, returns ``(True, None)``. Otherwise returns ``(False,
+        Checks whether it is permissible to call :meth:`verify_token`.
+
+        If it is allowed, returns ``(True, None)``. Otherwise returns ``(False,
         data_dict)``, where ``data_dict`` contains extra information, defined
         by the implementation.
 
         This method can be used to implement throttling or locking, for
         example. Client code should check this method before calling
         :meth:`verify_token` and report problems to the user.
 
@@ -215,30 +224,41 @@
         :rtype: (bool, dict or ``None``)
 
         """
         return (True, None)
 
     def verify_token(self, token):
         """
-        Verifies a token. As a rule, the token should no longer be valid if
-        this returns ``True``.
+        Verifies a token.
+
+        As a rule, the token should no longer be valid if this returns
+        ``True``.
 
         :param str token: The OTP token provided by the user.
         :rtype: bool
+
         """
         return False
 
 
 class SideChannelDevice(Device):
     """
     Abstract base model for a side-channel :term:`device` attached to a user.
 
     This model implements token generation, verification and expiration, so the
     concrete devices only have to implement delivery.
 
+    .. attribute:: token
+
+        The token most recently generated for the user.
+
+    .. attribute:: valid_until
+
+        The datetime at which the stored token will expire.
+
     """
 
     token = models.CharField(max_length=16, blank=True, null=True)
 
     valid_until = models.DateTimeField(
         default=timezone.now,
         help_text="The timestamp of the moment of expiry of the saved token.",
@@ -248,19 +268,18 @@
         abstract = True
 
     def generate_token(self, length=6, valid_secs=300, commit=True):
         """
         Generates a token of the specified length, then sets it on the model
         and sets the expiration of the token on the model.
 
-        Pass 'commit=False' to avoid calling self.save().
-
         :param int length: Number of decimal digits in the generated token.
         :param int valid_secs: Amount of seconds the token should be valid.
-        :param bool commit: Whether to autosave the generated token.
+        :param bool commit: Pass False if you intend to save the instance
+            yourself.
 
         """
         self.token = random_number_token(length)
         self.valid_until = timezone.now() + timedelta(seconds=valid_secs)
         if commit:
             self.save()
 
@@ -290,15 +309,15 @@
             return False
 
 
 class GenerateNotAllowed(enum.Enum):
     """
     Constants that may be returned in the ``reason`` member of the extra
     information dictionary returned by
-    :meth:`~django_otp.models.Device.generate_is_allowed`
+    :meth:`~django_otp.models.Device.generate_is_allowed`.
 
     .. data:: COOLDOWN_DURATION_PENDING
 
        Indicates that a token was generated recently and we're waiting for the
        cooldown period to expire.
 
     """
@@ -314,14 +333,18 @@
     Subclass must implement :meth:`get_cooldown_duration`, and must use the
     :meth:`generate_is_allowed` method from within their generate_challenge()
     method. Further it must use :meth:`cooldown_set` when a token is generated.
 
     See the implementation of
     :class:`~django_otp.plugins.otp_email.models.EmailDevice` for an example.
 
+    .. attribute:: last_generated_timestamp
+
+        The last time a token was generated for this device.
+
     """
 
     last_generated_timestamp = models.DateTimeField(
         null=True,
         blank=True,
         help_text="The last time a token was generated for this device.",
     )
@@ -360,27 +383,29 @@
             }
 
     def cooldown_reset(self, commit=True):
         """
         Call this method to reset cooldown (normally after a successful
         verification).
 
-        Pass 'commit=False' to avoid calling self.save().
+        :param bool commit: Pass False if you intend to save the instance
+            yourself.
 
         """
         self.last_generated_timestamp = None
         if commit:
             self.save()
 
     def cooldown_set(self, commit=True):
         """
         Call this method to set the cooldown timestamp to now (normally when
         a token is generated).
 
-        Pass 'commit=False' to avoid calling self.save().
+        :param bool commit: Pass False if you intend to save the instance
+            yourself.
 
         """
         self.last_generated_timestamp = timezone.now()
         if commit:
             self.save()
 
     def verify_token(self, token):
@@ -435,14 +460,22 @@
     implement :meth:`get_throttle_factor`, and must use the
     :meth:`verify_is_allowed`, :meth:`throttle_reset` and
     :meth:`throttle_increment` methods from within their verify_token() method.
 
     See the implementation of
     :class:`~django_otp.plugins.otp_email.models.EmailDevice` for an example.
 
+    .. attribute:: throttling_failure_timestamp
+
+        The datetime of the last failed verification attempt.
+
+    .. attribute:: throttling_failure_count
+
+        The number of consecutive failed verification attempts.
+
     """
 
     throttling_failure_timestamp = models.DateTimeField(
         null=True,
         blank=True,
         default=None,
         help_text=(
@@ -499,28 +532,30 @@
         return super().verify_is_allowed()
 
     def throttle_reset(self, commit=True):
         """
         Call this method to reset throttling (normally when a verify attempt
         succeeded).
 
-        Pass 'commit=False' to avoid calling self.save().
+        :param bool commit: Pass False if you intend to save the instance
+            yourself.
 
         """
         self.throttling_failure_timestamp = None
         self.throttling_failure_count = 0
         if commit:
             self.save()
 
     def throttle_increment(self, commit=True):
         """
         Call this method to increase throttling (normally when a verify attempt
         failed).
 
-        Pass 'commit=False' to avoid calling self.save().
+        :param bool commit: Pass False if you intend to save the instance
+            yourself.
 
         """
         self.throttling_failure_timestamp = timezone.now()
         self.throttling_failure_count += 1
         if commit:
             self.save()
 
@@ -538,7 +573,59 @@
         etc. seconds. A factor of 0 disables the throttling.
 
         Normally this is just a wrapper for a plugin-specific setting like
         :setting:`OTP_EMAIL_THROTTLE_FACTOR`.
 
         """
         raise NotImplementedError()
+
+
+class TimestampMixin(models.Model):
+    """
+    Mixin class that adds timestamps to devices.
+
+    This mixin adds fields to record when a device was initially created in the
+    system and when it was last used. It enhances the ability to audit device
+    usage and lifecycle.
+
+    Subclasses can use :meth:`set_last_used_timestamp` to update the
+    `last_used_at` timestamp whenever the device is used for verification.
+
+    .. attribute:: created_at
+
+        The datetime at which this device was created.
+
+    .. attribute:: last_used_at
+
+        The datetime at which this device was last successfully used for
+        verification.
+
+    """
+
+    created_at = models.DateTimeField(
+        null=True,
+        blank=True,
+        auto_now_add=True,
+        help_text="The date and time when this device was initially created in the system.",
+    )
+
+    last_used_at = models.DateTimeField(
+        null=True,
+        blank=True,
+        help_text="The most recent date and time this device was used.",
+    )
+
+    class Meta:
+        abstract = True
+
+    def set_last_used_timestamp(self, commit=True):
+        """
+        Updates the `last_used_at` field to the current datetime to indicate
+        that the device has been used.
+
+        :param bool commit: Pass False if you intend to save the instance
+            yourself.
+
+        """
+        self.last_used_at = timezone.now()
+        if commit:
+            self.save()
```

### Comparing `django_otp-1.3.0/src/django_otp/oath.py` & `django_otp-1.4.0/src/django_otp/oath.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/src/django_otp/tests.py` & `django_otp-1.4.0/src/django_otp/tests.py`

 * *Files 12% similar despite different names*

```diff
@@ -78,14 +78,123 @@
     pass
 
 
 class TransactionTestCase(OTPTestCaseMixin, DjangoTransactionTestCase):
     pass
 
 
+class TimestampTestMixin:
+    """
+    Generic tests for :class:`~django_otp.models.TimestampMixin`.
+
+    Implementing tests must initialize `self.device` with the model instance to
+    test and provide `valid_token` and `invalid_token` methods for verifying
+    token behavior.
+
+    Includes tests to:
+
+    - Check automatic setting of `created_at` upon object creation.
+    - Validate that `last_used_at` is initially None and updated only after
+      successful token verification.
+    - Ensure `set_last_used_timestamp` behaves correctly, respecting the
+      `commit` parameter.
+
+    """
+
+    def setUp(self):
+        self.device = None
+
+    def valid_token(self):
+        """Returns a valid token to pass to our device under test."""
+        raise NotImplementedError()
+
+    def invalid_token(self):
+        """Returns an invalid token to pass to our device under test."""
+        raise NotImplementedError()
+
+    #
+    # Tests
+    #
+
+    def test_created_at_set_on_creation(self):
+        """Verify that the `created_at` field is automatically set upon creation."""
+        self.assertIsNotNone(
+            self.device.created_at, "created_at should be automatically set."
+        )
+
+    def test_last_used_at_initially_none(self):
+        """Ensure `last_used_at` is None upon initial creation."""
+        self.assertIsNone(
+            self.device.last_used_at, "last_used_at should be None initially."
+        )
+
+    def test_set_last_used_timestamp_updates_field(self):
+        """Check if `set_last_used_timestamp` correctly updates the `last_used_at` field."""
+        self.device.set_last_used_timestamp(commit=True)
+        self.device.refresh_from_db()  # Assuming it's a persisted model
+
+        self.assertIsNotNone(
+            self.device.last_used_at, "last_used_at should be updated."
+        )
+
+    def test_set_last_used_timestamp_without_commit(self):
+        """
+        Ensure `set_last_used_timestamp` updates `last_used_at` without persisting
+        when commit=False.
+        """
+        original_last_used_at = self.device.last_used_at
+        self.device.set_last_used_timestamp(commit=False)
+        # Check in-memory update without saving
+        self.assertNotEqual(
+            self.device.last_used_at,
+            original_last_used_at,
+            "last_used_at should be updated in memory without commit.",
+        )
+
+        # Refresh from db to confirm it wasn't committed
+        self.device.refresh_from_db()
+        self.assertEqual(
+            self.device.last_used_at,
+            original_last_used_at,
+            "last_used_at should not be updated in db without commit.",
+        )
+
+    def test_verify_token_successful_updates_last_used_at(self):
+        """
+        Verifying with a valid token updates 'last_used_at'.
+        """
+        valid_token = self.valid_token()  # Method to generate a valid token
+        initial_last_used_at = self.device.last_used_at
+        verified = self.device.verify_token(valid_token)
+
+        self.assertTrue(verified, "Token should be verified successfully.")
+        self.device.refresh_from_db()
+        self.assertNotEqual(
+            self.device.last_used_at,
+            initial_last_used_at,
+            "'last_used_at' should be updated on successful verification.",
+        )
+
+    def test_verify_token_failed_does_not_update_last_used_at(self):
+        """
+        Verifying with an invalid token does not update 'last_used_at'.
+        """
+        invalid_token = self.invalid_token()  # Method to generate an invalid token
+        initial_last_used_at = self.device.last_used_at
+        verified = self.device.verify_token(invalid_token)
+
+        self.assertFalse(verified, "Token should not be verified.")
+        self.device.refresh_from_db()
+        self.assertEqual(
+            self.device.last_used_at,
+            initial_last_used_at,
+            "'last_used_at' should not be updated on failed verification.",
+        )
+
+
 class ThrottlingTestMixin:
     """
     Generic tests for throttled devices.
 
     Any concrete device implementation that uses throttling should define a
     TestCase subclass that includes this as a base class. This will help verify
     a correct integration of ThrottlingMixin.
```

### Comparing `django_otp-1.3.0/src/django_otp/util.py` & `django_otp-1.4.0/src/django_otp/util.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/src/django_otp/views.py` & `django_otp-1.4.0/src/django_otp/views.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/src/django_otp/locale/de/LC_MESSAGES/django.mo` & `django_otp-1.4.0/src/django_otp/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/src/django_otp/locale/de/LC_MESSAGES/django.po` & `django_otp-1.4.0/src/django_otp/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/src/django_otp/locale/es/LC_MESSAGES/django.mo` & `django_otp-1.4.0/src/django_otp/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/src/django_otp/locale/es/LC_MESSAGES/django.po` & `django_otp-1.4.0/src/django_otp/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/src/django_otp/locale/fr/LC_MESSAGES/django.mo` & `django_otp-1.4.0/src/django_otp/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/src/django_otp/locale/fr/LC_MESSAGES/django.po` & `django_otp-1.4.0/src/django_otp/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/src/django_otp/locale/pt_BR/LC_MESSAGES/django.mo` & `django_otp-1.4.0/src/django_otp/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/src/django_otp/locale/pt_BR/LC_MESSAGES/django.po` & `django_otp-1.4.0/src/django_otp/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/src/django_otp/locale/pt_PT/LC_MESSAGES/django.mo` & `django_otp-1.4.0/src/django_otp/locale/pt_PT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/src/django_otp/locale/pt_PT/LC_MESSAGES/django.po` & `django_otp-1.4.0/src/django_otp/locale/pt_PT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/src/django_otp/plugins/otp_email/conf.py` & `django_otp-1.4.0/src/django_otp/plugins/otp_email/conf.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/src/django_otp/plugins/otp_email/models.py` & `django_otp-1.4.0/src/django_otp/plugins/otp_email/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from django.template.loader import get_template
 
 from django_otp.models import (
     CooldownMixin,
     GenerateNotAllowed,
     SideChannelDevice,
     ThrottlingMixin,
+    TimestampMixin,
 )
 from django_otp.util import hex_validator, random_hex
 
 from .conf import settings
 
 
 def default_key():  # pragma: no cover
@@ -21,15 +22,15 @@
 
 
 def key_validator(value):  # pragma: no cover
     """Obsolete code here for migrations."""
     return hex_validator()(value)
 
 
-class EmailDevice(CooldownMixin, ThrottlingMixin, SideChannelDevice):
+class EmailDevice(TimestampMixin, CooldownMixin, ThrottlingMixin, SideChannelDevice):
     """
     A :class:`~django_otp.models.SideChannelDevice` that delivers a token to
     the email address saved in this object or alternatively to the user's
     registered email address (``user.email``).
 
     The tokens are valid for :setting:`OTP_EMAIL_TOKEN_VALIDITY` seconds. Once
     a token has been accepted, it is no longer valid.
@@ -113,15 +114,17 @@
     def verify_token(self, token):
         """"""
         verify_allowed, _ = self.verify_is_allowed()
         if verify_allowed:
             verified = super().verify_token(token)
 
             if verified:
-                self.throttle_reset()
+                self.throttle_reset(commit=False)
+                self.set_last_used_timestamp(commit=False)
+                self.save()
             else:
                 self.throttle_increment()
         else:
             verified = False
 
         return verified
```

### Comparing `django_otp-1.3.0/src/django_otp/plugins/otp_email/tests.py` & `django_otp-1.4.0/src/django_otp/plugins/otp_email/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,20 @@
 from freezegun import freeze_time
 
 from django.core import mail
 from django.db import IntegrityError
 from django.test.utils import override_settings
 
 from django_otp.forms import OTPAuthenticationForm
-from django_otp.tests import CooldownTestMixin, TestCase, ThrottlingTestMixin
+from django_otp.tests import (
+    CooldownTestMixin,
+    TestCase,
+    ThrottlingTestMixin,
+    TimestampTestMixin,
+)
 
 from .models import EmailDevice
 
 
 class EmailDeviceMixin:
     def setUp(self):
         try:
@@ -30,15 +35,15 @@
 
 class AuthFormTest(EmailDeviceMixin, TestCase):
     @override_settings(OTP_EMAIL_SENDER='test@example.com')
     def test_email_interaction(self):
         data = {
             'username': 'alice',
             'password': 'password',
-            'otp_device': 'otp_email.emaildevice/1',
+            'otp_device': self.device.persistent_id,
             'otp_token': '',
             'otp_challenge': '1',
         }
         form = OTPAuthenticationForm(None, data)
 
         self.assertFalse(form.is_valid())
         alice = form.get_user()
@@ -264,7 +269,18 @@
     def test_cooldown_imposed_expiration_message(self):
         with freeze_time() as frozen_time:
             self.device.generate_challenge()
             frozen_time.tick(delta=timedelta(seconds=5))
             self.device.refresh_from_db()
             message = self.device.generate_challenge()
             self.assertIn("Next generation allowed 5\xa0seconds from now.", message)
+
+
+class TimestampTestCase(EmailDeviceMixin, TimestampTestMixin, TestCase):
+    def valid_token(self):
+        if self.device.token is None:
+            self.device.generate_token()
+
+        return self.device.token
+
+    def invalid_token(self):
+        return -1
```

### Comparing `django_otp-1.3.0/src/django_otp/plugins/otp_email/migrations/0001_initial.py` & `django_otp-1.4.0/src/django_otp/plugins/otp_email/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/src/django_otp/plugins/otp_email/migrations/0002_sidechanneldevice_email.py` & `django_otp-1.4.0/src/django_otp/plugins/otp_email/migrations/0002_sidechanneldevice_email.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/src/django_otp/plugins/otp_email/migrations/0004_throttling.py` & `django_otp-1.4.0/src/django_otp/plugins/otp_email/migrations/0004_throttling.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/src/django_otp/plugins/otp_hotp/admin.py` & `django_otp-1.4.0/src/django_otp/plugins/otp_hotp/admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 
 class HOTPDeviceAdmin(admin.ModelAdmin):
     """
     :class:`~django.contrib.admin.ModelAdmin` for
     :class:`~django_otp.plugins.otp_hotp.models.HOTPDevice`.
     """
 
-    list_display = ['user', 'name', 'confirmed']
+    list_display = ['user', 'name', 'created_at', 'last_used_at', 'confirmed']
+    list_filter = ['created_at', 'last_used_at', 'confirmed']
 
     raw_id_fields = ['user']
-    readonly_fields = ['qrcode_link']
+    readonly_fields = ['created_at', 'last_used_at', 'qrcode_link']
     radio_fields = {'digits': admin.HORIZONTAL}
 
     def get_list_display(self, request):
         list_display = super().get_list_display(request)
         if not settings.OTP_ADMIN_HIDE_SENSITIVE_DATA:
             list_display = [*list_display, 'qrcode_link']
         return list_display
@@ -40,14 +41,20 @@
             (
                 'Identity',
                 {
                     'fields': ['user', 'name', 'confirmed'],
                 },
             ),
             (
+                'Timestamps',
+                {
+                    'fields': ['created_at', 'last_used_at'],
+                },
+            ),
+            (
                 'Configuration',
                 {
                     'fields': configuration_fields,
                 },
             ),
             (
                 'State',
```

### Comparing `django_otp-1.3.0/src/django_otp/plugins/otp_hotp/models.py` & `django_otp-1.4.0/src/django_otp/plugins/otp_hotp/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from base64 import b32encode
 from binascii import unhexlify
 from urllib.parse import quote, urlencode
 
 from django.conf import settings
 from django.db import models
 
-from django_otp.models import Device, ThrottlingMixin
+from django_otp.models import Device, ThrottlingMixin, TimestampMixin
 from django_otp.oath import hotp
 from django_otp.util import hex_validator, random_hex
 
 
 def default_key():
     return random_hex(20)
 
 
 def key_validator(value):
     return hex_validator()(value)
 
 
-class HOTPDevice(ThrottlingMixin, Device):
+class HOTPDevice(TimestampMixin, ThrottlingMixin, Device):
     """
     A generic HOTP :class:`~django_otp.models.Device`. The model fields mostly
     correspond to the arguments to :func:`django_otp.oath.hotp`. They all have
     sensible defaults, including the key, which is randomly generated.
 
     .. attribute:: key
 
@@ -86,14 +86,15 @@
             key = self.bin_key
 
             for counter in range(self.counter, self.counter + self.tolerance + 1):
                 if hotp(key, counter, self.digits) == token:
                     verified = True
                     self.counter = counter + 1
                     self.throttle_reset(commit=False)
+                    self.set_last_used_timestamp(commit=False)
                     self.save()
                     break
             else:
                 verified = False
 
         if not verified:
             self.throttle_increment(commit=True)
```

### Comparing `django_otp-1.3.0/src/django_otp/plugins/otp_hotp/tests.py` & `django_otp-1.4.0/src/django_otp/plugins/otp_hotp/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from django.core.exceptions import PermissionDenied
 from django.db import IntegrityError
 from django.test import RequestFactory
 from django.test.utils import override_settings
 from django.urls import reverse
 
 from django_otp.forms import OTPAuthenticationForm
-from django_otp.tests import TestCase, ThrottlingTestMixin
+from django_otp.tests import TestCase, ThrottlingTestMixin, TimestampTestMixin
 
 from .admin import HOTPDeviceAdmin
 from .models import HOTPDevice
 
 
 class HOTPDeviceMixin:
     """
@@ -308,22 +308,22 @@
         self.assertIn('key', fields)
         self.assertIn('qrcode_link', fields)
 
     @override_settings(OTP_ADMIN_HIDE_SENSITIVE_DATA=True)
     def test_list_display_when_sensitive_information_hidden(self):
         self.assertEqual(
             self.device_admin.get_list_display(self.get_request),
-            ['user', 'name', 'confirmed'],
+            ['user', 'name', 'created_at', 'last_used_at', 'confirmed'],
         )
 
     @override_settings(OTP_ADMIN_HIDE_SENSITIVE_DATA=False)
     def test_list_display_when_sensitive_information_shown(self):
         self.assertEqual(
             self.device_admin.get_list_display(self.get_request),
-            ['user', 'name', 'confirmed', 'qrcode_link'],
+            ['user', 'name', 'created_at', 'last_used_at', 'confirmed', 'qrcode_link'],
         )
 
     @override_settings(OTP_ADMIN_HIDE_SENSITIVE_DATA=True)
     def test_config_view_when_sensitive_information_hidden(self):
         self._add_device_perms('change_hotpdevice')
         with self.assertRaises(PermissionDenied):
             self.device_admin.config_view(self.get_request, self.device.id)
@@ -375,7 +375,15 @@
 )
 class ThrottlingTestCase(HOTPDeviceMixin, ThrottlingTestMixin, TestCase):
     def valid_token(self):
         return self.tokens[0]
 
     def invalid_token(self):
         return -1
+
+
+class TimetstampTestCase(HOTPDeviceMixin, TimestampTestMixin, TestCase):
+    def valid_token(self):
+        return self.tokens[0]
+
+    def invalid_token(self):
+        return -1
```

### Comparing `django_otp-1.3.0/src/django_otp/plugins/otp_hotp/migrations/0001_initial.py` & `django_otp-1.4.0/src/django_otp/plugins/otp_hotp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/src/django_otp/plugins/otp_hotp/migrations/0002_auto_20190420_0723.py` & `django_otp-1.4.0/src/django_otp/plugins/otp_hotp/migrations/0002_auto_20190420_0723.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/src/django_otp/plugins/otp_hotp/templates/otp_hotp/admin/config.html` & `django_otp-1.4.0/src/django_otp/plugins/otp_hotp/templates/otp_hotp/admin/config.html`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/src/django_otp/plugins/otp_static/admin.py` & `django_otp-1.4.0/src/django_otp/plugins/otp_static/admin.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,23 +13,34 @@
 
 class StaticDeviceAdmin(admin.ModelAdmin):
     """
     :class:`~django.contrib.admin.ModelAdmin` for
     :class:`~django_otp.plugins.otp_static.models.StaticDevice`.
     """
 
+    list_display = ['user', 'name', 'created_at', 'last_used_at', 'confirmed']
+    list_filter = ['created_at', 'last_used_at', 'confirmed']
+
+    raw_id_fields = ['user']
+    readonly_fields = ['created_at', 'last_used_at']
+
     fieldsets = [
         (
             'Identity',
             {
                 'fields': ['user', 'name', 'confirmed'],
             },
         ),
+        (
+            'Timestamps',
+            {
+                'fields': ['created_at', 'last_used_at'],
+            },
+        ),
     ]
-    raw_id_fields = ['user']
 
     inlines = [
         StaticTokenInline,
     ]
 
     def get_inline_instances(self, request, obj=None):
         if settings.OTP_ADMIN_HIDE_SENSITIVE_DATA and obj:
```

### Comparing `django_otp-1.3.0/src/django_otp/plugins/otp_static/lib.py` & `django_otp-1.4.0/src/django_otp/plugins/otp_static/lib.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/src/django_otp/plugins/otp_static/models.py` & `django_otp-1.4.0/src/django_otp/plugins/otp_static/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from base64 import b32encode
 from os import urandom
 
 from django.conf import settings
 from django.db import models
 
-from django_otp.models import Device, ThrottlingMixin
+from django_otp.models import Device, ThrottlingMixin, TimestampMixin
 
 
-class StaticDevice(ThrottlingMixin, Device):
+class StaticDevice(TimestampMixin, ThrottlingMixin, Device):
     """
     A static :class:`~django_otp.models.Device` simply consists of random
     tokens shared by the database and the user.
 
     These are frequently used as emergency tokens in case a user's normal
     device is lost or unavailable. They can be consumed in any order; each
     token will be removed from the database as soon as it is used.
@@ -30,15 +30,17 @@
 
     def verify_token(self, token):
         verify_allowed, _ = self.verify_is_allowed()
         if verify_allowed:
             match = self.token_set.filter(token=token).first()
             if match is not None:
                 match.delete()
-                self.throttle_reset()
+                self.throttle_reset(commit=False)
+                self.set_last_used_timestamp(commit=False)
+                self.save()
             else:
                 self.throttle_increment()
         else:
             match = None
 
         return match is not None
```

### Comparing `django_otp-1.3.0/src/django_otp/plugins/otp_static/tests.py` & `django_otp-1.4.0/src/django_otp/plugins/otp_static/tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from django.contrib.auth.models import Permission
 from django.contrib.contenttypes.models import ContentType
 from django.db import IntegrityError
 from django.test import RequestFactory
 from django.test.utils import override_settings
 
 from django_otp.forms import OTPAuthenticationForm
-from django_otp.tests import TestCase, ThrottlingTestMixin
+from django_otp.tests import TestCase, ThrottlingTestMixin, TimestampTestMixin
 
 from .admin import StaticDeviceAdmin, StaticTokenInline
 from .lib import add_static_token
 from .models import StaticDevice, StaticToken
 
 
 class DeviceTest(TestCase):
@@ -179,14 +179,33 @@
     def setUp(self):
         try:
             user = self.create_user('alice', 'password')
         except IntegrityError:
             self.skipTest("Unable to create a test user.")
         else:
             self.device = user.staticdevice_set.create()
+            self.device.token_set.create(token='valid1')
+            self.device.token_set.create(token='valid2')
+            self.device.token_set.create(token='valid3')
+
+    def valid_token(self):
+        return self.device.token_set.first().token
+
+    def invalid_token(self):
+        return 'bogus'
+
+
+class TimestampTestCase(TimestampTestMixin, TestCase):
+    def setUp(self):
+        try:
+            user = self.create_user('alice', 'password')
+        except IntegrityError:
+            self.skipTest("Unable to create a test user.")
+        else:
+            self.device = user.staticdevice_set.create()
             self.device.token_set.create(token='valid1')
             self.device.token_set.create(token='valid2')
             self.device.token_set.create(token='valid3')
 
     def valid_token(self):
         return self.device.token_set.first().token
```

### Comparing `django_otp-1.3.0/src/django_otp/plugins/otp_static/management/commands/addstatictoken.py` & `django_otp-1.4.0/src/django_otp/plugins/otp_static/management/commands/addstatictoken.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/src/django_otp/plugins/otp_static/migrations/0001_initial.py` & `django_otp-1.4.0/src/django_otp/plugins/otp_static/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/src/django_otp/plugins/otp_static/migrations/0002_throttling.py` & `django_otp-1.4.0/src/django_otp/plugins/otp_static/migrations/0002_throttling.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/src/django_otp/plugins/otp_totp/admin.py` & `django_otp-1.4.0/src/django_otp/plugins/otp_totp/admin.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 
 class TOTPDeviceAdmin(admin.ModelAdmin):
     """
     :class:`~django.contrib.admin.ModelAdmin` for
     :class:`~django_otp.plugins.otp_totp.models.TOTPDevice`.
     """
 
-    list_display = ['user', 'name', 'confirmed']
+    list_display = ['user', 'name', 'created_at', 'last_used_at', 'confirmed']
+    list_filter = ['created_at', 'last_used_at', 'confirmed']
 
     raw_id_fields = ['user']
-    readonly_fields = ['qrcode_link']
+    readonly_fields = ['created_at', 'last_used_at', 'qrcode_link']
     radio_fields = {'digits': admin.HORIZONTAL}
 
     def get_list_display(self, request):
         list_display = super().get_list_display(request)
         if not settings.OTP_ADMIN_HIDE_SENSITIVE_DATA:
             list_display = [*list_display, 'qrcode_link']
         return list_display
@@ -40,14 +41,20 @@
             (
                 'Identity',
                 {
                     'fields': ['user', 'name', 'confirmed'],
                 },
             ),
             (
+                'Timestamps',
+                {
+                    'fields': ['created_at', 'last_used_at'],
+                },
+            ),
+            (
                 'Configuration',
                 {
                     'fields': configuration_fields,
                 },
             ),
             (
                 'State',
```

### Comparing `django_otp-1.3.0/src/django_otp/plugins/otp_totp/models.py` & `django_otp-1.4.0/src/django_otp/plugins/otp_totp/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 from binascii import unhexlify
 import time
 from urllib.parse import quote, urlencode
 
 from django.conf import settings
 from django.db import models
 
-from django_otp.models import Device, ThrottlingMixin
+from django_otp.models import Device, ThrottlingMixin, TimestampMixin
 from django_otp.oath import TOTP
 from django_otp.util import hex_validator, random_hex
 
 
 def default_key():
     return random_hex(20)
 
 
 def key_validator(value):
     return hex_validator()(value)
 
 
-class TOTPDevice(ThrottlingMixin, Device):
+class TOTPDevice(TimestampMixin, ThrottlingMixin, Device):
     """
     A generic TOTP :class:`~django_otp.models.Device`. The model fields mostly
     correspond to the arguments to :func:`django_otp.oath.totp`. They all have
     sensible defaults, including the key, which is randomly generated.
 
     .. attribute:: key
 
@@ -125,14 +125,15 @@
 
             verified = totp.verify(token, self.tolerance, self.last_t + 1)
             if verified:
                 self.last_t = totp.t()
                 if OTP_TOTP_SYNC:
                     self.drift = totp.drift
                 self.throttle_reset(commit=False)
+                self.set_last_used_timestamp(commit=False)
                 self.save()
 
         if not verified:
             self.throttle_increment(commit=True)
 
         return verified
```

### Comparing `django_otp-1.3.0/src/django_otp/plugins/otp_totp/tests.py` & `django_otp-1.4.0/src/django_otp/plugins/otp_totp/tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from django.contrib.contenttypes.models import ContentType
 from django.core.exceptions import PermissionDenied
 from django.db import IntegrityError
 from django.test import RequestFactory
 from django.test.utils import override_settings
 from django.urls import reverse
 
-from django_otp.tests import TestCase, ThrottlingTestMixin
+from django_otp.tests import TestCase, ThrottlingTestMixin, TimestampTestMixin
 
 from .admin import TOTPDeviceAdmin
 from .models import TOTPDevice
 
 
 class TOTPDeviceMixin:
     """
@@ -264,22 +264,22 @@
         self.assertIn('key', fields)
         self.assertIn('qrcode_link', fields)
 
     @override_settings(OTP_ADMIN_HIDE_SENSITIVE_DATA=True)
     def test_list_display_when_sensitive_information_hidden(self):
         self.assertEqual(
             self.device_admin.get_list_display(self.get_request),
-            ['user', 'name', 'confirmed'],
+            ['user', 'name', 'created_at', 'last_used_at', 'confirmed'],
         )
 
     @override_settings(OTP_ADMIN_HIDE_SENSITIVE_DATA=False)
     def test_list_display_when_sensitive_information_shown(self):
         self.assertEqual(
             self.device_admin.get_list_display(self.get_request),
-            ['user', 'name', 'confirmed', 'qrcode_link'],
+            ['user', 'name', 'created_at', 'last_used_at', 'confirmed', 'qrcode_link'],
         )
 
     @override_settings(OTP_ADMIN_HIDE_SENSITIVE_DATA=True)
     def test_config_view_when_sensitive_information_hidden(self):
         self._add_device_perms('change_totpdevice')
         with self.assertRaises(PermissionDenied):
             self.device_admin.config_view(self.get_request, self.device.id)
@@ -331,7 +331,15 @@
 )
 class ThrottlingTestCase(TOTPDeviceMixin, ThrottlingTestMixin, TestCase):
     def valid_token(self):
         return self.tokens[3]
 
     def invalid_token(self):
         return -1
+
+
+class TimetstampTestCase(TOTPDeviceMixin, TimestampTestMixin, TestCase):
+    def valid_token(self):
+        return self.tokens[3]
+
+    def invalid_token(self):
+        return -1
```

### Comparing `django_otp-1.3.0/src/django_otp/plugins/otp_totp/migrations/0001_initial.py` & `django_otp-1.4.0/src/django_otp/plugins/otp_totp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/src/django_otp/plugins/otp_totp/migrations/0002_auto_20190420_0723.py` & `django_otp-1.4.0/src/django_otp/plugins/otp_totp/migrations/0002_auto_20190420_0723.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/src/django_otp/plugins/otp_totp/templates/otp_totp/admin/config.html` & `django_otp-1.4.0/src/django_otp/plugins/otp_totp/templates/otp_totp/admin/config.html`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/src/django_otp/templates/otp/admin111/login.html` & `django_otp-1.4.0/src/django_otp/templates/otp/admin111/login.html`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/test/config/sample.toml` & `django_otp-1.4.0/test/config/sample.toml`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/test/test_project/config.py` & `django_otp-1.4.0/test/test_project/config.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/test/test_project/settings.py` & `django_otp-1.4.0/test/test_project/settings.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/test/test_project/urls.py` & `django_otp-1.4.0/test/test_project/urls.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/test/test_project/views.py` & `django_otp-1.4.0/test/test_project/views.py`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/test/test_project/templates/about.html` & `django_otp-1.4.0/test/test_project/templates/about.html`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/test/test_project/templates/home.html` & `django_otp-1.4.0/test/test_project/templates/home.html`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/test/test_project/templates/navbar.html` & `django_otp-1.4.0/test/test_project/templates/navbar.html`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/test/test_project/templates/root.html` & `django_otp-1.4.0/test/test_project/templates/root.html`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/test/test_project/templates/registration/login.html` & `django_otp-1.4.0/test/test_project/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/LICENSE` & `django_otp-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/README.rst` & `django_otp-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `django_otp-1.3.0/pyproject.toml` & `django_otp-1.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "django-otp"
-version = "1.3.0"
+version = "1.4.0"
 description = "A pluggable framework for adding two-factor authentication to Django using one-time passwords."
 readme = "README.rst"
 requires-python = ">=3.7"
 license = "Unlicense"
 authors = [
     { name = "Peter Sagerson", email = "psagers@ignorare.net" },
 ]
```

### Comparing `django_otp-1.3.0/PKG-INFO` & `django_otp-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-otp
-Version: 1.3.0
+Version: 1.4.0
 Summary: A pluggable framework for adding two-factor authentication to Django using one-time passwords.
 Project-URL: Homepage, https://github.com/django-otp/django-otp
 Project-URL: Documentation, https://django-otp-official.readthedocs.io/
 Author-email: Peter Sagerson <psagers@ignorare.net>
 License-Expression: Unlicense
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_3ljg_9l1_/tmppazwebte_TarContainer/0/102", line 173, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-otp Version: 1.3.0 Summary: A pluggable
+Metadata-Version: 2.1 Name: django-otp Version: 1.4.0 Summary: A pluggable
 framework for adding two-factor authentication to Django using one-time
 passwords. Project-URL: Homepage, https://github.com/django-otp/django-otp
 Project-URL: Documentation, https://django-otp-official.readthedocs.io/ Author-
 email: Peter Sagerson
 ignorare.net> License-Expression: Unlicense License-File: LICENSE Classifier:
 Development Status :: 5 - Production/Stable Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
```

