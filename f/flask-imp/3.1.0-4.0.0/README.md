# Comparing `tmp/flask_imp-3.1.0.tar.gz` & `tmp/flask_imp-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_imp-3.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "flask_imp-4.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `flask_imp-3.1.0.tar` & `flask_imp-4.0.0.tar`

### file list

```diff
@@ -1,95 +1,91 @@
--rw-r--r--   0        0        0    25308 2024-03-11 17:31:21.979301 flask_imp-3.1.0/LICENSE
--rw-r--r--   0        0        0     2915 2024-03-11 17:31:21.979391 flask_imp-3.1.0/README.md
--rw-r--r--   0        0        0     2616 2024-03-11 17:31:21.990751 flask_imp-3.1.0/docs_md/Blueprint-Introduction.md
--rw-r--r--   0        0        0     3130 2024-03-11 17:31:21.990845 flask_imp-3.1.0/docs_md/Blueprint-config-toml.md
--rw-r--r--   0        0        0      375 2024-03-11 17:31:21.990920 flask_imp-3.1.0/docs_md/Blueprint-init.md
--rw-r--r--   0        0        0     1432 2024-03-11 17:31:21.990986 flask_imp-3.1.0/docs_md/Blueprint_x-import_models.md
--rw-r--r--   0        0        0     1414 2024-03-11 17:31:21.991095 flask_imp-3.1.0/docs_md/Blueprint_x-import_nested_blueprint.md
--rw-r--r--   0        0        0     1383 2024-03-11 17:31:21.991151 flask_imp-3.1.0/docs_md/Blueprint_x-import_nested_blueprints.md
--rw-r--r--   0        0        0     1080 2024-03-11 17:31:21.991224 flask_imp-3.1.0/docs_md/Blueprint_x-import_resources.md
--rw-r--r--   0        0        0      341 2024-03-11 17:31:21.991285 flask_imp-3.1.0/docs_md/Blueprint_x-init_session.md
--rw-r--r--   0        0        0      904 2024-03-11 17:31:21.991350 flask_imp-3.1.0/docs_md/Blueprint_x-tmpl.md
--rw-r--r--   0        0        0     2694 2024-03-11 17:31:21.991411 flask_imp-3.1.0/docs_md/CLI Commands-flask-imp blueprint.md
--rw-r--r--   0        0        0     5441 2024-03-11 17:31:21.991514 flask_imp-3.1.0/docs_md/CLI Commands-flask-imp init.md
--rw-r--r--   0        0        0     2770 2024-03-11 17:31:21.991569 flask_imp-3.1.0/docs_md/Imp-Introduction.md
--rw-r--r--   0        0        0      531 2024-03-11 17:31:21.991624 flask_imp-3.1.0/docs_md/Imp-load-env-vars.md
--rw-r--r--   0        0        0     3846 2024-03-11 17:31:21.991690 flask_imp-3.1.0/docs_md/Imp-x-config-toml.md
--rw-r--r--   0        0        0     2429 2024-03-11 17:31:21.991756 flask_imp-3.1.0/docs_md/Imp_x-import_app_resources.md
--rw-r--r--   0        0        0     2104 2024-03-11 17:31:21.991824 flask_imp-3.1.0/docs_md/Imp_x-import_blueprint.md
--rw-r--r--   0        0        0      971 2024-03-11 17:31:21.991888 flask_imp-3.1.0/docs_md/Imp_x-import_blueprints.md
--rw-r--r--   0        0        0     1401 2024-03-11 17:31:21.991949 flask_imp-3.1.0/docs_md/Imp_x-import_models.md
--rw-r--r--   0        0        0      904 2024-03-11 17:31:21.992012 flask_imp-3.1.0/docs_md/Imp_x-init_app-init.md
--rw-r--r--   0        0        0      742 2024-03-11 17:31:21.992079 flask_imp-3.1.0/docs_md/Imp_x-init_session.md
--rw-r--r--   0        0        0      965 2024-03-11 17:31:21.992158 flask_imp-3.1.0/docs_md/Imp_x-model.md
--rw-r--r--   0        0        0     1867 2024-03-11 17:31:21.992228 flask_imp-3.1.0/docs_md/__index__.md
--rw-r--r--   0        0        0      968 2024-03-11 17:31:21.992287 flask_imp-3.1.0/docs_md/__menu__.md
--rw-r--r--   0        0        0     1630 2024-03-11 17:31:21.992361 flask_imp-3.1.0/docs_md/flask_imp_auth-authenticate_password.md
--rw-r--r--   0        0        0     1566 2024-03-11 17:31:21.992429 flask_imp-3.1.0/docs_md/flask_imp_auth-encrypt_password.md
--rw-r--r--   0        0        0      440 2024-03-11 17:31:21.992490 flask_imp-3.1.0/docs_md/flask_imp_auth-generate_alphanumeric_validator.md
--rw-r--r--   0        0        0      502 2024-03-11 17:31:21.992550 flask_imp-3.1.0/docs_md/flask_imp_auth-generate_csrf_token.md
--rw-r--r--   0        0        0      588 2024-03-11 17:31:21.992597 flask_imp-3.1.0/docs_md/flask_imp_auth-generate_email_validator.md
--rw-r--r--   0        0        0      507 2024-03-11 17:31:21.992684 flask_imp-3.1.0/docs_md/flask_imp_auth-generate_numeric_validator.md
--rw-r--r--   0        0        0      474 2024-03-11 17:31:21.992776 flask_imp-3.1.0/docs_md/flask_imp_auth-generate_password.md
--rw-r--r--   0        0        0      904 2024-03-11 17:31:21.992914 flask_imp-3.1.0/docs_md/flask_imp_auth-generate_private_key.md
--rw-r--r--   0        0        0      856 2024-03-11 17:31:21.992979 flask_imp-3.1.0/docs_md/flask_imp_auth-generate_salt.md
--rw-r--r--   0        0        0      865 2024-03-11 17:31:21.993047 flask_imp-3.1.0/docs_md/flask_imp_auth-is_email_address_valid.md
--rw-r--r--   0        0        0     1037 2024-03-11 17:31:21.993124 flask_imp-3.1.0/docs_md/flask_imp_auth-is_username_valid.md
--rw-r--r--   0        0        0     1018 2024-03-11 17:31:21.993190 flask_imp-3.1.0/docs_md/flask_imp_security-api_login_check.md
--rw-r--r--   0        0        0     1104 2024-03-11 17:31:21.993250 flask_imp-3.1.0/docs_md/flask_imp_security-include_csrf.md
--rw-r--r--   0        0        0     1641 2024-03-11 17:31:21.993327 flask_imp-3.1.0/docs_md/flask_imp_security-login_check.md
--rw-r--r--   0        0        0      169 2024-03-11 17:31:21.993393 flask_imp-3.1.0/docs_md/flask_imp_security-pass_function_check.md
--rw-r--r--   0        0        0     1403 2024-03-11 17:31:21.993454 flask_imp-3.1.0/docs_md/flask_imp_security-permission_check.md
--rw-r--r--   0        0        0      252 2024-03-13 10:48:12.803901 flask_imp-3.1.0/flask_imp/__init__.py
--rw-r--r--   0        0        0     1989 2024-03-11 17:31:21.993655 flask_imp-3.1.0/flask_imp/_cli/__init__.py
--rw-r--r--   0        0        0     4733 2024-03-11 17:31:21.993770 flask_imp-3.1.0/flask_imp/_cli/blueprint.py
--rw-r--r--   0        0        0      299 2024-03-11 17:31:21.993886 flask_imp-3.1.0/flask_imp/_cli/filelib/__init__.py
--rw-r--r--   0        0        0     6517 2024-03-11 17:31:21.994015 flask_imp-3.1.0/flask_imp/_cli/filelib/all_files.py
--rw-r--r--   0        0        0     9126 2024-03-11 17:31:21.994100 flask_imp-3.1.0/flask_imp/_cli/filelib/app.py
--rw-r--r--   0        0        0     3726 2024-03-11 17:31:21.994192 flask_imp-3.1.0/flask_imp/_cli/filelib/blueprint.py
--rw-r--r--   0        0        0    33707 2024-03-11 17:31:21.994306 flask_imp-3.1.0/flask_imp/_cli/filelib/favicon.py
--rw-r--r--   0        0        0    17864 2024-03-11 17:31:21.994420 flask_imp-3.1.0/flask_imp/_cli/filelib/flask_imp_logo.py
--rw-r--r--   0        0        0      823 2024-03-11 17:31:21.994511 flask_imp-3.1.0/flask_imp/_cli/filelib/head_tag_generator.py
--rw-r--r--   0        0        0       88 2024-03-11 17:31:21.994564 flask_imp-3.1.0/flask_imp/_cli/filelib/main_js.py
--rw-r--r--   0        0        0    17166 2024-03-11 17:31:21.994646 flask_imp-3.1.0/flask_imp/_cli/filelib/water_css.py
--rw-r--r--   0        0        0      587 2024-03-11 17:31:21.994731 flask_imp-3.1.0/flask_imp/_cli/helpers.py
--rw-r--r--   0        0        0     9303 2024-03-11 17:31:21.994809 flask_imp-3.1.0/flask_imp/_cli/init.py
--rw-r--r--   0        0        0     1057 2024-03-11 17:31:21.994913 flask_imp-3.1.0/flask_imp/auth/__init__.py
--rw-r--r--   0        0        0     6432 2024-03-11 17:31:21.995112 flask_imp-3.1.0/flask_imp/auth/__legacy__.py
--rw-r--r--   0        0        0      850 2024-03-11 17:31:21.995175 flask_imp-3.1.0/flask_imp/auth/__private_funcs__.py
--rw-r--r--   0        0        0     2748 2024-03-11 17:31:21.995246 flask_imp-3.1.0/flask_imp/auth/authenticate_password.py
--rw-r--r--   0        0        0    14294 2024-03-11 17:31:21.995365 flask_imp-3.1.0/flask_imp/auth/dataclasses.py
--rw-r--r--   0        0        0     1844 2024-03-11 17:31:21.995427 flask_imp-3.1.0/flask_imp/auth/encrypt_password.py
--rw-r--r--   0        0        0      535 2024-03-11 17:31:21.995484 flask_imp-3.1.0/flask_imp/auth/generate_alphanumeric_validator.py
--rw-r--r--   0        0        0      385 2024-03-11 17:31:21.995544 flask_imp-3.1.0/flask_imp/auth/generate_csrf_token.py
--rw-r--r--   0        0        0      524 2024-03-11 17:31:21.995600 flask_imp-3.1.0/flask_imp/auth/generate_email_validator.py
--rw-r--r--   0        0        0      607 2024-03-11 17:31:21.995686 flask_imp-3.1.0/flask_imp/auth/generate_numeric_validator.py
--rw-r--r--   0        0        0     1545 2024-03-11 17:31:21.995743 flask_imp-3.1.0/flask_imp/auth/generate_password.py
--rw-r--r--   0        0        0      697 2024-03-11 17:31:21.995815 flask_imp-3.1.0/flask_imp/auth/generate_private_key.py
--rw-r--r--   0        0        0      426 2024-03-11 17:31:21.995879 flask_imp-3.1.0/flask_imp/auth/generate_salt.py
--rw-r--r--   0        0        0     1139 2024-03-11 17:31:21.995940 flask_imp-3.1.0/flask_imp/auth/is_email_address_valid.py
--rw-r--r--   0        0        0     1872 2024-03-11 17:31:21.995999 flask_imp-3.1.0/flask_imp/auth/is_username_valid.py
--rw-r--r--   0        0        0    14426 2024-03-11 17:31:21.996116 flask_imp-3.1.0/flask_imp/blueprint.py
--rw-r--r--   0        0        0     7277 2024-03-11 17:31:21.996235 flask_imp-3.1.0/flask_imp/helpers.py
--rw-r--r--   0        0        0    21802 2024-03-13 10:44:27.466837 flask_imp-3.1.0/flask_imp/imp.py
--rw-r--r--   0        0        0      756 2024-03-11 17:31:21.996422 flask_imp-3.1.0/flask_imp/protocols.py
--rw-r--r--   0        0        0      917 2024-03-11 17:31:21.996484 flask_imp-3.1.0/flask_imp/registeries.py
--rw-r--r--   0        0        0      349 2024-03-11 17:31:21.996580 flask_imp-3.1.0/flask_imp/security/__init__.py
--rw-r--r--   0        0        0      708 2024-03-11 17:31:21.996651 flask_imp-3.1.0/flask_imp/security/__private_funcs__.py
--rw-r--r--   0        0        0     1802 2024-03-11 17:31:21.996745 flask_imp-3.1.0/flask_imp/security/api_login_check.py
--rw-r--r--   0        0        0     2222 2024-03-11 17:31:21.996828 flask_imp-3.1.0/flask_imp/security/include_csrf.py
--rw-r--r--   0        0        0     3880 2024-03-11 17:31:21.996900 flask_imp-3.1.0/flask_imp/security/login_check.py
--rw-r--r--   0        0        0     7117 2024-03-11 17:31:21.997016 flask_imp-3.1.0/flask_imp/security/pass_function_check.py
--rw-r--r--   0        0        0     2688 2024-03-11 17:31:21.997074 flask_imp-3.1.0/flask_imp/security/permission_check.py
--rw-r--r--   0        0        0     4664 2024-03-11 17:31:21.997182 flask_imp-3.1.0/flask_imp/utilities.py
--rw-r--r--   0        0        0     1732 2024-03-11 17:31:21.997298 flask_imp-3.1.0/gdocs/__init__.py
--rw-r--r--   0        0        0       55 2024-03-11 17:31:21.997394 flask_imp-3.1.0/gdocs/ssg/__init__.py
--rw-r--r--   0        0        0     4180 2024-03-11 17:31:21.997503 flask_imp-3.1.0/gdocs/ssg/compiler.py
--rw-r--r--   0        0        0      746 2024-03-11 17:31:21.997572 flask_imp-3.1.0/gdocs/ssg/exceptions.py
--rw-r--r--   0        0        0     1260 2024-03-11 17:31:21.997641 flask_imp-3.1.0/gdocs/ssg/helpers.py
--rw-r--r--   0        0        0      659 2024-03-11 17:31:21.997719 flask_imp-3.1.0/gdocs/ssg/render_engines.py
--rw-r--r--   0        0        0      903 2024-03-11 17:31:21.997836 flask_imp-3.1.0/gdocs/templates/__main__.html
--rw-r--r--   0        0        0     1423 2024-03-11 17:31:21.997908 flask_imp-3.1.0/gdocs/templates/__menu__.html
--rw-r--r--   0        0        0      819 2024-03-11 17:31:21.997984 flask_imp-3.1.0/gdocs/templates/index.html
--rw-r--r--   0        0        0     1666 2024-03-11 17:31:21.998057 flask_imp-3.1.0/pyproject.toml
--rw-r--r--   0        0        0       29 2024-03-11 17:31:21.998120 flask_imp-3.1.0/requirements.txt
--rw-r--r--   0        0        0     4158 1970-01-01 00:00:00.000000 flask_imp-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-10 12:24:23.959533 flask_imp-4.0.0/LICENSE
+-rw-r--r--   0        0        0     2805 2024-04-10 11:19:08.688270 flask_imp-4.0.0/README.md
+-rw-r--r--   0        0        0     2771 2024-04-10 11:19:08.711168 flask_imp-4.0.0/docs_md/Blueprint-Introduction.md
+-rw-r--r--   0        0        0     4015 2024-04-10 11:19:08.711269 flask_imp-4.0.0/docs_md/Blueprint-config-x.md
+-rw-r--r--   0        0        0      375 2024-03-11 17:31:21.990920 flask_imp-4.0.0/docs_md/Blueprint-init.md
+-rw-r--r--   0        0        0     1432 2024-03-11 17:31:21.990986 flask_imp-4.0.0/docs_md/Blueprint_x-import_models.md
+-rw-r--r--   0        0        0     1414 2024-03-11 17:31:21.991095 flask_imp-4.0.0/docs_md/Blueprint_x-import_nested_blueprint.md
+-rw-r--r--   0        0        0     1383 2024-03-11 17:31:21.991151 flask_imp-4.0.0/docs_md/Blueprint_x-import_nested_blueprints.md
+-rw-r--r--   0        0        0     1080 2024-03-11 17:31:21.991224 flask_imp-4.0.0/docs_md/Blueprint_x-import_resources.md
+-rw-r--r--   0        0        0      341 2024-03-11 17:31:21.991285 flask_imp-4.0.0/docs_md/Blueprint_x-init_session.md
+-rw-r--r--   0        0        0      904 2024-03-11 17:31:21.991350 flask_imp-4.0.0/docs_md/Blueprint_x-tmpl.md
+-rw-r--r--   0        0        0     2876 2024-04-10 11:19:08.711483 flask_imp-4.0.0/docs_md/CLI Commands-flask-imp blueprint.md
+-rw-r--r--   0        0        0     6032 2024-04-10 11:19:08.711690 flask_imp-4.0.0/docs_md/CLI Commands-flask-imp init.md
+-rw-r--r--   0        0        0     2674 2024-04-10 11:19:08.711991 flask_imp-4.0.0/docs_md/Imp-Introduction.md
+-rw-r--r--   0        0        0     7475 2024-04-10 11:19:08.712087 flask_imp-4.0.0/docs_md/Imp-config-x.md
+-rw-r--r--   0        0        0     2429 2024-03-11 17:31:21.991756 flask_imp-4.0.0/docs_md/Imp_x-import_app_resources.md
+-rw-r--r--   0        0        0     2104 2024-03-11 17:31:21.991824 flask_imp-4.0.0/docs_md/Imp_x-import_blueprint.md
+-rw-r--r--   0        0        0      971 2024-03-11 17:31:21.991888 flask_imp-4.0.0/docs_md/Imp_x-import_blueprints.md
+-rw-r--r--   0        0        0     1401 2024-03-11 17:31:21.991949 flask_imp-4.0.0/docs_md/Imp_x-import_models.md
+-rw-r--r--   0        0        0     1236 2024-04-10 11:19:08.712300 flask_imp-4.0.0/docs_md/Imp_x-init_app-init.md
+-rw-r--r--   0        0        0      734 2024-04-10 11:19:08.712558 flask_imp-4.0.0/docs_md/Imp_x-init_session.md
+-rw-r--r--   0        0        0      965 2024-03-11 17:31:21.992158 flask_imp-4.0.0/docs_md/Imp_x-model.md
+-rw-r--r--   0        0        0     4354 2024-04-10 11:19:08.712814 flask_imp-4.0.0/docs_md/__index__.md
+-rw-r--r--   0        0        0      935 2024-04-10 11:19:08.713090 flask_imp-4.0.0/docs_md/__menu__.md
+-rw-r--r--   0        0        0     1630 2024-03-11 17:31:21.992361 flask_imp-4.0.0/docs_md/flask_imp_auth-authenticate_password.md
+-rw-r--r--   0        0        0     1566 2024-03-11 17:31:21.992429 flask_imp-4.0.0/docs_md/flask_imp_auth-encrypt_password.md
+-rw-r--r--   0        0        0      440 2024-03-11 17:31:21.992490 flask_imp-4.0.0/docs_md/flask_imp_auth-generate_alphanumeric_validator.md
+-rw-r--r--   0        0        0      502 2024-03-11 17:31:21.992550 flask_imp-4.0.0/docs_md/flask_imp_auth-generate_csrf_token.md
+-rw-r--r--   0        0        0      588 2024-03-11 17:31:21.992597 flask_imp-4.0.0/docs_md/flask_imp_auth-generate_email_validator.md
+-rw-r--r--   0        0        0      507 2024-03-11 17:31:21.992684 flask_imp-4.0.0/docs_md/flask_imp_auth-generate_numeric_validator.md
+-rw-r--r--   0        0        0      474 2024-03-11 17:31:21.992776 flask_imp-4.0.0/docs_md/flask_imp_auth-generate_password.md
+-rw-r--r--   0        0        0      904 2024-03-11 17:31:21.992914 flask_imp-4.0.0/docs_md/flask_imp_auth-generate_private_key.md
+-rw-r--r--   0        0        0      856 2024-03-11 17:31:21.992979 flask_imp-4.0.0/docs_md/flask_imp_auth-generate_salt.md
+-rw-r--r--   0        0        0      865 2024-03-11 17:31:21.993047 flask_imp-4.0.0/docs_md/flask_imp_auth-is_email_address_valid.md
+-rw-r--r--   0        0        0     1037 2024-03-11 17:31:21.993124 flask_imp-4.0.0/docs_md/flask_imp_auth-is_username_valid.md
+-rw-r--r--   0        0        0     1018 2024-03-11 17:31:21.993190 flask_imp-4.0.0/docs_md/flask_imp_security-api_login_check.md
+-rw-r--r--   0        0        0     1104 2024-03-11 17:31:21.993250 flask_imp-4.0.0/docs_md/flask_imp_security-include_csrf.md
+-rw-r--r--   0        0        0     1641 2024-03-11 17:31:21.993327 flask_imp-4.0.0/docs_md/flask_imp_security-login_check.md
+-rw-r--r--   0        0        0      169 2024-03-11 17:31:21.993393 flask_imp-4.0.0/docs_md/flask_imp_security-pass_function_check.md
+-rw-r--r--   0        0        0     1403 2024-03-11 17:31:21.993454 flask_imp-4.0.0/docs_md/flask_imp_security-permission_check.md
+-rw-r--r--   0        0        0      673 2024-04-10 11:19:08.713363 flask_imp-4.0.0/flask_imp/__init__.py
+-rw-r--r--   0        0        0     3144 2024-04-10 11:19:08.713710 flask_imp-4.0.0/flask_imp/_cli/__init__.py
+-rw-r--r--   0        0        0     4990 2024-04-10 11:19:08.714051 flask_imp-4.0.0/flask_imp/_cli/blueprint.py
+-rw-r--r--   0        0        0      299 2024-03-11 17:31:21.993886 flask_imp-4.0.0/flask_imp/_cli/filelib/__init__.py
+-rw-r--r--   0        0        0     6517 2024-03-11 17:31:21.994015 flask_imp-4.0.0/flask_imp/_cli/filelib/all_files.py
+-rw-r--r--   0        0        0    14125 2024-04-10 11:19:08.714430 flask_imp-4.0.0/flask_imp/_cli/filelib/app.py
+-rw-r--r--   0        0        0     4527 2024-04-10 11:54:53.832600 flask_imp-4.0.0/flask_imp/_cli/filelib/blueprint.py
+-rw-r--r--   0        0        0    33707 2024-03-11 17:31:21.994306 flask_imp-4.0.0/flask_imp/_cli/filelib/favicon.py
+-rw-r--r--   0        0        0    17864 2024-03-11 17:31:21.994420 flask_imp-4.0.0/flask_imp/_cli/filelib/flask_imp_logo.py
+-rw-r--r--   0        0        0      823 2024-03-11 17:31:21.994511 flask_imp-4.0.0/flask_imp/_cli/filelib/head_tag_generator.py
+-rw-r--r--   0        0        0       88 2024-03-11 17:31:21.994564 flask_imp-4.0.0/flask_imp/_cli/filelib/main_js.py
+-rw-r--r--   0        0        0    17166 2024-03-11 17:31:21.994646 flask_imp-4.0.0/flask_imp/_cli/filelib/water_css.py
+-rw-r--r--   0        0        0      587 2024-03-11 17:31:21.994731 flask_imp-4.0.0/flask_imp/_cli/helpers.py
+-rw-r--r--   0        0        0     9739 2024-04-10 11:19:08.715059 flask_imp-4.0.0/flask_imp/_cli/init.py
+-rw-r--r--   0        0        0     1057 2024-03-11 17:31:21.994913 flask_imp-4.0.0/flask_imp/auth/__init__.py
+-rw-r--r--   0        0        0     6432 2024-03-11 17:31:21.995112 flask_imp-4.0.0/flask_imp/auth/__legacy__.py
+-rw-r--r--   0        0        0      850 2024-03-11 17:31:21.995175 flask_imp-4.0.0/flask_imp/auth/__private_funcs__.py
+-rw-r--r--   0        0        0     2748 2024-03-11 17:31:21.995246 flask_imp-4.0.0/flask_imp/auth/authenticate_password.py
+-rw-r--r--   0        0        0    14294 2024-03-11 17:31:21.995365 flask_imp-4.0.0/flask_imp/auth/dataclasses.py
+-rw-r--r--   0        0        0     1844 2024-03-11 17:31:21.995427 flask_imp-4.0.0/flask_imp/auth/encrypt_password.py
+-rw-r--r--   0        0        0      535 2024-03-11 17:31:21.995484 flask_imp-4.0.0/flask_imp/auth/generate_alphanumeric_validator.py
+-rw-r--r--   0        0        0      385 2024-03-11 17:31:21.995544 flask_imp-4.0.0/flask_imp/auth/generate_csrf_token.py
+-rw-r--r--   0        0        0      524 2024-03-11 17:31:21.995600 flask_imp-4.0.0/flask_imp/auth/generate_email_validator.py
+-rw-r--r--   0        0        0      607 2024-03-11 17:31:21.995686 flask_imp-4.0.0/flask_imp/auth/generate_numeric_validator.py
+-rw-r--r--   0        0        0     1545 2024-03-11 17:31:21.995743 flask_imp-4.0.0/flask_imp/auth/generate_password.py
+-rw-r--r--   0        0        0      697 2024-03-11 17:31:21.995815 flask_imp-4.0.0/flask_imp/auth/generate_private_key.py
+-rw-r--r--   0        0        0      426 2024-03-11 17:31:21.995879 flask_imp-4.0.0/flask_imp/auth/generate_salt.py
+-rw-r--r--   0        0        0     1139 2024-03-11 17:31:21.995940 flask_imp-4.0.0/flask_imp/auth/is_email_address_valid.py
+-rw-r--r--   0        0        0     1872 2024-03-11 17:31:21.995999 flask_imp-4.0.0/flask_imp/auth/is_username_valid.py
+-rw-r--r--   0        0        0     1558 2024-04-10 11:19:08.715176 flask_imp-4.0.0/flask_imp/config_database_template.py
+-rw-r--r--   0        0        0     8880 2024-04-10 11:19:08.715330 flask_imp-4.0.0/flask_imp/config_flask_template.py
+-rw-r--r--   0        0        0     2528 2024-04-10 11:19:08.715438 flask_imp-4.0.0/flask_imp/config_imp_blueprint_template.py
+-rw-r--r--   0        0        0     2067 2024-04-10 11:19:08.715555 flask_imp-4.0.0/flask_imp/config_imp_template.py
+-rw-r--r--   0        0        0      932 2024-04-10 11:19:08.715674 flask_imp-4.0.0/flask_imp/config_object_parser.py
+-rw-r--r--   0        0        0     6370 2024-04-10 11:19:08.715800 flask_imp-4.0.0/flask_imp/config_toml_parser.py
+-rw-r--r--   0        0        0       87 2024-04-10 11:19:08.715907 flask_imp-4.0.0/flask_imp/exceptions.py
+-rw-r--r--   0        0        0    24112 2024-04-10 11:19:08.716353 flask_imp-4.0.0/flask_imp/imp.py
+-rw-r--r--   0        0        0    14397 2024-04-10 11:55:17.235524 flask_imp-4.0.0/flask_imp/imp_blueprint.py
+-rw-r--r--   0        0        0     4840 2024-04-10 11:43:13.630660 flask_imp-4.0.0/flask_imp/protocols.py
+-rw-r--r--   0        0        0      917 2024-03-11 17:31:21.996484 flask_imp-4.0.0/flask_imp/registeries.py
+-rw-r--r--   0        0        0      349 2024-03-11 17:31:21.996580 flask_imp-4.0.0/flask_imp/security/__init__.py
+-rw-r--r--   0        0        0      708 2024-03-11 17:31:21.996651 flask_imp-4.0.0/flask_imp/security/__private_funcs__.py
+-rw-r--r--   0        0        0     1802 2024-03-11 17:31:21.996745 flask_imp-4.0.0/flask_imp/security/api_login_check.py
+-rw-r--r--   0        0        0     2222 2024-03-11 17:31:21.996828 flask_imp-4.0.0/flask_imp/security/include_csrf.py
+-rw-r--r--   0        0        0     3880 2024-03-11 17:31:21.996900 flask_imp-4.0.0/flask_imp/security/login_check.py
+-rw-r--r--   0        0        0     7117 2024-03-11 17:31:21.997016 flask_imp-4.0.0/flask_imp/security/pass_function_check.py
+-rw-r--r--   0        0        0     2688 2024-03-11 17:31:21.997074 flask_imp-4.0.0/flask_imp/security/permission_check.py
+-rw-r--r--   0        0        0     5476 2024-04-10 11:19:08.717102 flask_imp-4.0.0/flask_imp/utilities.py
+-rw-r--r--   0        0        0     1883 2024-04-10 12:54:20.642886 flask_imp-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0       27 2024-04-10 11:19:08.717892 flask_imp-4.0.0/requirements.txt
+-rw-r--r--   0        0        0     4012 1970-01-01 00:00:00.000000 flask_imp-4.0.0/PKG-INFO
```

### Comparing `flask_imp-3.1.0/README.md` & `flask_imp-4.0.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -12,18 +12,14 @@
 Flask-Imp's main purpose is to help simplify the importing of blueprints, resources, and models.
 It has a few extra features built in to help with securing pages and password authentication.
 
 ## Documentation
 
 [https://cheesecake87.github.io/flask-imp/](https://cheesecake87.github.io/flask-imp/)
 
-### Notable Breaking Changes
-
-[2.x.x to 3.0.0](https://github.com/CheeseCake87/flask-imp/releases/tag/3.0.0)
-
 ## Getting Started
 
 ### Setup.
 
 Create a new project folder and navigate to it.
 
 ```text
```

### Comparing `flask_imp-3.1.0/docs_md/Blueprint-Introduction.md` & `flask_imp-4.0.0/docs_md/Blueprint-Introduction.md`

 * *Files 7% similar despite different names*

```diff
@@ -11,154 +11,164 @@
 000000a0: 6164 6469 7469 6f6e 616c 206d 6574 686f  additional metho
 000000b0: 6473 2074 6f20 616c 6c6f 7720 666f 7220  ds to allow for 
 000000c0: 6175 746f 0a69 6d70 6f72 7469 6e67 206f  auto.importing o
 000000d0: 6620 6d6f 6465 6c73 2c20 7265 736f 7572  f models, resour
 000000e0: 6365 7320 616e 6420 6f74 6865 7220 6e65  ces and other ne
 000000f0: 7374 6564 2062 6c75 6570 7269 6e74 732e  sted blueprints.
 00000100: 0a0a 5468 6520 466c 6173 6b2d 496d 7020  ..The Flask-Imp 
-00000110: 426c 7565 7072 696e 7420 7265 6164 7320  Blueprint reads 
-00000120: 636f 6e66 6967 7572 6174 696f 6e20 6672  configuration fr
-00000130: 6f6d 2061 2063 6f6e 6669 672e 746f 6d6c  om a config.toml
-00000140: 2066 696c 652c 2077 6869 6368 2069 7320   file, which is 
-00000150: 6c6f 6361 7465 6420 696e 2074 6865 2073  located in the s
-00000160: 616d 6520 6469 7265 6374 6f72 7920 6173  ame directory as
-00000170: 2074 6865 0a60 5f5f 696e 6974 5f5f 2e70   the.`__init__.p
-00000180: 7960 2066 696c 652e 0a0a 4865 7265 2773  y` file...Here's
-00000190: 2061 6e20 6578 616d 706c 6520 6f66 2061   an example of a
-000001a0: 2046 6c61 736b 2d49 6d70 2042 6c75 6570   Flask-Imp Bluep
-000001b0: 7269 6e74 2073 7472 7563 7475 7265 3a0a  rint structure:.
-000001c0: 0a60 6060 7465 7874 0a77 7777 2f0a e294  .```text.www/...
-000001d0: 9ce2 9480 e294 8020 6e65 7374 6564 5f62  ....... nested_b
-000001e0: 6c75 6570 7269 6e74 732f 0ae2 9482 2020  lueprints/....  
-000001f0: 20e2 949c e294 80e2 9480 2062 6c75 6570   ......... bluep
-00000200: 7269 6e74 5f6f 6e65 2f0a e294 8220 2020  rint_one/....   
-00000210: e294 8220 2020 e294 9ce2 9480 e294 8020  ...   ......... 
-00000220: 2e2e 2e0a e294 8220 2020 e294 8220 2020  .......   ...   
-00000230: e294 9ce2 9480 e294 8020 5f5f 696e 6974  ......... __init
-00000240: 5f5f 2e70 790a e294 8220 2020 e294 8220  __.py....   ... 
-00000250: 2020 e294 94e2 9480 e294 8020 636f 6e66    ......... conf
-00000260: 6967 2e74 6f6d 6c0a e294 8220 2020 e294  ig.toml....   ..
-00000270: 94e2 9480 e294 8020 626c 7565 7072 696e  ....... blueprin
-00000280: 745f 7477 6f2f 0ae2 9482 2020 2020 2020  t_two/....      
-00000290: 20e2 949c e294 80e2 9480 202e 2e2e 0ae2   ......... .....
-000002a0: 9482 2020 2020 2020 20e2 949c e294 80e2  ..       .......
-000002b0: 9480 205f 5f69 6e69 745f 5f2e 7079 0ae2  .. __init__.py..
-000002c0: 9482 2020 2020 2020 20e2 9494 e294 80e2  ..       .......
-000002d0: 9480 2063 6f6e 6669 672e 746f 6d6c 0ae2  .. config.toml..
-000002e0: 949c e294 80e2 9480 2073 7461 6e64 616c  ........ standal
-000002f0: 6f6e 655f 6e65 7374 6564 5f62 6c75 6570  one_nested_bluep
-00000300: 7269 6e74 2f0a e294 8220 2020 e294 9ce2  rint/....   ....
-00000310: 9480 e294 8020 2e2e 2e0a e294 8220 2020  ..... .......   
-00000320: e294 9ce2 9480 e294 8020 5f5f 696e 6974  ......... __init
-00000330: 5f5f 2e70 790a e294 8220 2020 e294 94e2  __.py....   ....
-00000340: 9480 e294 8020 636f 6e66 6967 2e74 6f6d  ..... config.tom
-00000350: 6c0a e294 9ce2 9480 e294 8020 6d6f 6465  l.......... mode
-00000360: 6c73 2f0a e294 8220 2020 e294 94e2 9480  ls/....   ......
-00000370: e294 8020 2e2e 2e0a e294 9ce2 9480 e294  ... ............
-00000380: 8020 726f 7574 6573 2f0a e294 8220 2020  . routes/....   
-00000390: e294 94e2 9480 e294 8020 696e 6465 782e  ......... index.
-000003a0: 7079 0ae2 949c e294 80e2 9480 2073 7461  py.......... sta
-000003b0: 7469 632f 0ae2 9482 2020 20e2 9494 e294  tic/....   .....
-000003c0: 80e2 9480 202e 2e2e 0ae2 949c e294 80e2  .... ...........
-000003d0: 9480 2074 656d 706c 6174 6573 2f0a e294  .. templates/...
-000003e0: 8220 2020 e294 94e2 9480 e294 8020 7777  .   ......... ww
-000003f0: 772f 0ae2 9482 2020 2020 2020 20e2 9494  w/....       ...
-00000400: e294 80e2 9480 2069 6e64 6578 2e68 746d  ...... index.htm
-00000410: 6c0a e294 9ce2 9480 e294 8020 5f5f 696e  l.......... __in
-00000420: 6974 5f5f 2e70 790a e294 94e2 9480 e294  it__.py.........
-00000430: 8020 636f 6e66 6967 2e74 6f6d 6c0a 6060  . config.toml.``
-00000440: 600a 0a46 696c 653a 2060 5f5f 696e 6974  `..File: `__init
-00000450: 5f5f 2e70 7960 0a0a 6060 6070 7974 686f  __.py`..```pytho
-00000460: 6e0a 6672 6f6d 2066 6c61 736b 5f69 6d70  n.from flask_imp
-00000470: 2069 6d70 6f72 7420 426c 7565 7072 696e   import Blueprin
-00000480: 740a 0a62 7020 3d20 426c 7565 7072 696e  t..bp = Blueprin
-00000490: 7428 5f5f 6e61 6d65 5f5f 290a 0a62 702e  t(__name__)..bp.
-000004a0: 696d 706f 7274 5f72 6573 6f75 7263 6573  import_resources
-000004b0: 2822 726f 7574 6573 2229 0a62 702e 696d  ("routes").bp.im
-000004c0: 706f 7274 5f6d 6f64 656c 7328 226d 6f64  port_models("mod
-000004d0: 656c 7322 290a 6270 2e69 6d70 6f72 745f  els").bp.import_
-000004e0: 6e65 7374 6564 5f62 6c75 6570 7269 6e74  nested_blueprint
-000004f0: 7328 226e 6573 7465 645f 626c 7565 7072  s("nested_bluepr
-00000500: 696e 7473 2229 0a62 702e 696d 706f 7274  ints").bp.import
-00000510: 5f6e 6573 7465 645f 626c 7565 7072 696e  _nested_blueprin
-00000520: 7428 2273 7461 6e64 616c 6f6e 655f 6e65  t("standalone_ne
-00000530: 7374 6564 5f62 6c75 6570 7269 6e74 2229  sted_blueprint")
-00000540: 0a0a 0a40 6270 2e62 6566 6f72 655f 6170  ...@bp.before_ap
-00000550: 705f 7265 7175 6573 740a 6465 6620 6265  p_request.def be
-00000560: 666f 7265 5f61 7070 5f72 6571 7565 7374  fore_app_request
-00000570: 2829 3a0a 2020 2020 6270 2e69 6e69 745f  ():.    bp.init_
-00000580: 7365 7373 696f 6e28 290a 6060 600a 0a54  session().```..T
-00000590: 6861 7420 6063 6f6e 6669 672e 746f 6d6c  hat `config.toml
-000005a0: 6020 6669 6c65 2069 7320 6c6f 6164 6564  ` file is loaded
-000005b0: 2064 7572 696e 6720 7468 6520 605f 5f69   during the `__i
-000005c0: 6e69 745f 5f60 206d 6574 686f 6420 6f66  nit__` method of
-000005d0: 2074 6865 2042 6c75 6570 7269 6e74 2063   the Blueprint c
-000005e0: 6c61 7373 2e0a 546f 2073 6565 206d 6f72  lass..To see mor
-000005f0: 6520 6162 6f75 7420 7468 6520 636f 6e66  e about the conf
-00000600: 6967 2066 696c 6520 7365 653a 205b 426c  ig file see: [Bl
-00000610: 7565 7072 696e 7420 2f20 636f 6e66 6967  ueprint / config
-00000620: 2e74 6f6d 6c5d 2862 6c75 6570 7269 6e74  .toml](blueprint
-00000630: 2d63 6f6e 6669 672d 746f 6d6c 2e68 746d  -config-toml.htm
-00000640: 6c29 0a0a 6069 6d70 6f72 745f 7265 736f  l)..`import_reso
-00000650: 7572 6365 7360 206d 6574 686f 6420 7769  urces` method wi
-00000660: 6c6c 2077 616c 6b20 6f6e 6520 6c65 7665  ll walk one leve
-00000670: 6c20 6465 6570 2069 6e74 6f20 7468 6520  l deep into the 
-00000680: 6072 6f75 7465 7360 2066 6f6c 6465 722c  `routes` folder,
-00000690: 2061 6e64 2069 6d70 6f72 7420 616c 6c20   and import all 
-000006a0: 602e 7079 6020 6669 6c65 7320 6173 206d  `.py` files as m
-000006b0: 6f64 756c 6573 2e0a 466f 7220 6d6f 7265  odules..For more
-000006c0: 2069 6e66 6f72 6d61 7469 6f6e 2073 6565   information see
-000006d0: 3a20 5b42 6c75 6570 7269 6e74 2e78 202f  : [Blueprint.x /
-000006e0: 2069 6d70 6f72 745f 7265 736f 7572 6365   import_resource
-000006f0: 735d 2862 6c75 6570 7269 6e74 5f78 2d69  s](blueprint_x-i
-00000700: 6d70 6f72 745f 7265 736f 7572 6365 732e  mport_resources.
-00000710: 6874 6d6c 290a 0a60 696d 706f 7274 5f6d  html)..`import_m
-00000720: 6f64 656c 7360 2077 6f72 6b73 2074 6865  odels` works the
-00000730: 2073 616d 6520 6173 2060 696d 702e 696d   same as `imp.im
-00000740: 706f 7274 5f6d 6f64 656c 7360 2c20 6974  port_models`, it
-00000750: 2077 696c 6c20 6c6f 6f6b 2066 6f72 2069   will look for i
-00000760: 6e73 7461 6e63 6573 206f 6620 6064 622e  nstances of `db.
-00000770: 4d6f 6465 6c60 2061 6e64 2069 6d70 6f72  Model` and impor
-00000780: 7420 7468 656d 2e20 5468 6573 650a 7769  t them. These.wi
-00000790: 6c6c 2061 6c73 6f20 6265 2061 7661 696c  ll also be avail
-000007a0: 6162 6c65 2069 6e20 7468 6520 6d6f 6465  able in the mode
-000007b0: 6c20 6c6f 6f6b 7570 206d 6574 686f 6420  l lookup method 
-000007c0: 6069 6d70 2e6d 6f64 656c 602e 0a46 6f72  `imp.model`..For
-000007d0: 206d 6f72 6520 696e 666f 726d 6174 696f   more informatio
-000007e0: 6e20 7365 653a 205b 496d 702e 7820 2f20  n see: [Imp.x / 
-000007f0: 696d 706f 7274 5f6d 6f64 656c 735d 2869  import_models](i
-00000800: 6d70 5f78 2d69 6d70 6f72 745f 6d6f 6465  mp_x-import_mode
-00000810: 6c73 2e68 746d 6c29 0a0a 6069 6d70 6f72  ls.html)..`impor
-00000820: 745f 6e65 7374 6564 5f62 6c75 6570 7269  t_nested_bluepri
-00000830: 6e74 7360 2077 696c 6c20 646f 2074 6865  nts` will do the
-00000840: 2073 616d 6520 6173 2060 696d 702e 696d   same as `imp.im
-00000850: 706f 7274 5f62 6c75 6570 7269 6e74 7360  port_blueprints`
-00000860: 2c20 6275 7420 7769 6c6c 2072 6567 6973  , but will regis
-00000870: 7465 7220 7468 6520 626c 7565 7072 696e  ter the blueprin
-00000880: 7473 2066 6f75 6e64 2061 730a 6e65 7374  ts found as.nest
-00000890: 6564 2074 6f20 7468 6520 6375 7272 656e  ed to the curren
-000008a0: 7420 626c 7565 7072 696e 742e 2046 6f72  t blueprint. For
-000008b0: 2065 7861 6d70 6c65 2060 7777 772e 626c   example `www.bl
-000008c0: 7565 7072 696e 745f 6f6e 652e 696e 6465  ueprint_one.inde
-000008d0: 7860 0a0a 6069 6d70 6f72 745f 6e65 7374  x`..`import_nest
-000008e0: 6564 5f62 6c75 6570 7269 6e74 6020 6265  ed_blueprint` be
-000008f0: 6861 7665 7320 7468 6520 7361 6d65 2061  haves the same a
-00000900: 7320 6069 6d70 6f72 745f 6e65 7374 6564  s `import_nested
-00000910: 5f62 6c75 6570 7269 6e74 7360 2c20 6275  _blueprints`, bu
-00000920: 7420 7769 6c6c 206f 6e6c 7920 696d 706f  t will only impo
-00000930: 7274 2061 2073 696e 676c 6520 626c 7565  rt a single blue
-00000940: 7072 696e 742e 0a0a 6062 702e 696e 6974  print...`bp.init
-00000950: 5f73 6573 7369 6f6e 6020 7769 6c6c 206c  _session` will l
-00000960: 6f61 6420 7468 6520 7365 7373 696f 6e20  oad the session 
-00000970: 7661 7269 6162 6c65 7320 6672 6f6d 2074  variables from t
-00000980: 6865 2063 6f6e 6669 6720 6669 6c65 2069  he config file i
-00000990: 6e74 6f20 7468 6520 7365 7373 696f 6e20  nto the session 
-000009a0: 6f62 6a65 6374 2e20 466f 7220 6d6f 7265  object. For more
-000009b0: 2069 6e66 6f72 6d61 7469 6f6e 0a73 6565   information.see
-000009c0: 3a20 5b42 6c75 6570 7269 6e74 2e78 202f  : [Blueprint.x /
-000009d0: 2069 6e69 745f 7365 7373 696f 6e5d 2862   init_session](b
-000009e0: 6c75 6570 7269 6e74 5f78 2d69 6e69 745f  lueprint_x-init_
-000009f0: 7365 7373 696f 6e2e 6874 6d6c 2920 616e  session.html) an
-00000a00: 640a 5b42 6c75 6570 7269 6e74 202f 2063  d.[Blueprint / c
-00000a10: 6f6e 6669 672e 746f 6d6c 5d28 626c 7565  onfig.toml](blue
-00000a20: 7072 696e 742d 636f 6e66 6967 2d74 6f6d  print-config-tom
-00000a30: 6c2e 6874 6d6c 290a                      l.html).
+00000110: 426c 7565 7072 696e 7420 6279 2064 6566  Blueprint by def
+00000120: 6175 6c74 2c20 7265 6164 7320 636f 6e66  ault, reads conf
+00000130: 6967 7572 6174 696f 6e20 6672 6f6d 2061  iguration from a
+00000140: 2063 6f6e 6669 672e 746f 6d6c 2066 696c   config.toml fil
+00000150: 6520 6f72 2066 726f 6d20 6120 636f 6e66  e or from a conf
+00000160: 6967 2063 6c61 7373 2c20 0a77 6869 6368  ig class, .which
+00000170: 2069 7320 6c6f 6361 7465 6420 696e 2074   is located in t
+00000180: 6865 2073 616d 6520 6469 7265 6374 6f72  he same director
+00000190: 7920 6173 2074 6865 0a60 5f5f 696e 6974  y as the.`__init
+000001a0: 5f5f 2e70 7960 2066 696c 652e 0a0a 4865  __.py` file...He
+000001b0: 7265 2773 2061 6e20 6578 616d 706c 6520  re's an example 
+000001c0: 6f66 2061 2046 6c61 736b 2d49 6d70 2042  of a Flask-Imp B
+000001d0: 6c75 6570 7269 6e74 2073 7472 7563 7475  lueprint structu
+000001e0: 7265 3a0a 0a60 6060 7465 7874 0a77 7777  re:..```text.www
+000001f0: 2f0a e294 9ce2 9480 e294 8020 6e65 7374  /.......... nest
+00000200: 6564 5f62 6c75 6570 7269 6e74 732f 0ae2  ed_blueprints/..
+00000210: 9482 2020 20e2 949c e294 80e2 9480 2062  ..   ......... b
+00000220: 6c75 6570 7269 6e74 5f6f 6e65 2f0a e294  lueprint_one/...
+00000230: 8220 2020 e294 8220 2020 e294 9ce2 9480  .   ...   ......
+00000240: e294 8020 2e2e 2e0a e294 8220 2020 e294  ... .......   ..
+00000250: 8220 2020 e294 9ce2 9480 e294 8020 5f5f  .   ......... __
+00000260: 696e 6974 5f5f 2e70 790a e294 8220 2020  init__.py....   
+00000270: e294 8220 2020 e294 94e2 9480 e294 8020  ...   ......... 
+00000280: 636f 6e66 6967 2e70 790a e294 8220 2020  config.py....   
+00000290: e294 94e2 9480 e294 8020 626c 7565 7072  ......... bluepr
+000002a0: 696e 745f 7477 6f2f 0ae2 9482 2020 2020  int_two/....    
+000002b0: 2020 20e2 949c e294 80e2 9480 202e 2e2e     ......... ...
+000002c0: 0ae2 9482 2020 2020 2020 20e2 949c e294  ....       .....
+000002d0: 80e2 9480 205f 5f69 6e69 745f 5f2e 7079  .... __init__.py
+000002e0: 0ae2 9482 2020 2020 2020 20e2 9494 e294  ....       .....
+000002f0: 80e2 9480 2063 6f6e 6669 672e 7079 0ae2  .... config.py..
+00000300: 949c e294 80e2 9480 2073 7461 6e64 616c  ........ standal
+00000310: 6f6e 655f 6e65 7374 6564 5f62 6c75 6570  one_nested_bluep
+00000320: 7269 6e74 2f0a e294 8220 2020 e294 9ce2  rint/....   ....
+00000330: 9480 e294 8020 2e2e 2e0a e294 8220 2020  ..... .......   
+00000340: e294 9ce2 9480 e294 8020 5f5f 696e 6974  ......... __init
+00000350: 5f5f 2e70 790a e294 8220 2020 e294 94e2  __.py....   ....
+00000360: 9480 e294 8020 636f 6e66 6967 2e70 790a  ..... config.py.
+00000370: e294 9ce2 9480 e294 8020 6d6f 6465 6c73  ......... models
+00000380: 2f0a e294 8220 2020 e294 94e2 9480 e294  /....   ........
+00000390: 8020 2e2e 2e0a e294 9ce2 9480 e294 8020  . ............. 
+000003a0: 726f 7574 6573 2f0a e294 8220 2020 e294  routes/....   ..
+000003b0: 94e2 9480 e294 8020 696e 6465 782e 7079  ....... index.py
+000003c0: 0ae2 949c e294 80e2 9480 2073 7461 7469  .......... stati
+000003d0: 632f 0ae2 9482 2020 20e2 9494 e294 80e2  c/....   .......
+000003e0: 9480 202e 2e2e 0ae2 949c e294 80e2 9480  .. .............
+000003f0: 2074 656d 706c 6174 6573 2f0a e294 8220   templates/.... 
+00000400: 2020 e294 94e2 9480 e294 8020 7777 772f    ......... www/
+00000410: 0ae2 9482 2020 2020 2020 20e2 9494 e294  ....       .....
+00000420: 80e2 9480 2069 6e64 6578 2e68 746d 6c0a  .... index.html.
+00000430: e294 9ce2 9480 e294 8020 5f5f 696e 6974  ......... __init
+00000440: 5f5f 2e70 790a e294 94e2 9480 e294 8020  __.py.......... 
+00000450: 636f 6e66 6967 2e70 790a 6060 600a 0a46  config.py.```..F
+00000460: 696c 653a 2060 5f5f 696e 6974 5f5f 2e70  ile: `__init__.p
+00000470: 7960 0a0a 6060 6070 7974 686f 6e0a 6672  y`..```python.fr
+00000480: 6f6d 2066 6c61 736b 5f69 6d70 2069 6d70  om flask_imp imp
+00000490: 6f72 7420 426c 7565 7072 696e 740a 0a62  ort Blueprint..b
+000004a0: 7020 3d20 426c 7565 7072 696e 7428 5f5f  p = Blueprint(__
+000004b0: 6e61 6d65 5f5f 290a 0a62 702e 696d 706f  name__)..bp.impo
+000004c0: 7274 5f72 6573 6f75 7263 6573 2822 726f  rt_resources("ro
+000004d0: 7574 6573 2229 0a62 702e 696d 706f 7274  utes").bp.import
+000004e0: 5f6d 6f64 656c 7328 226d 6f64 656c 7322  _models("models"
+000004f0: 290a 6270 2e69 6d70 6f72 745f 6e65 7374  ).bp.import_nest
+00000500: 6564 5f62 6c75 6570 7269 6e74 7328 226e  ed_blueprints("n
+00000510: 6573 7465 645f 626c 7565 7072 696e 7473  ested_blueprints
+00000520: 2229 0a62 702e 696d 706f 7274 5f6e 6573  ").bp.import_nes
+00000530: 7465 645f 626c 7565 7072 696e 7428 2273  ted_blueprint("s
+00000540: 7461 6e64 616c 6f6e 655f 6e65 7374 6564  tandalone_nested
+00000550: 5f62 6c75 6570 7269 6e74 2229 0a0a 0a40  _blueprint")...@
+00000560: 6270 2e62 6566 6f72 655f 6170 705f 7265  bp.before_app_re
+00000570: 7175 6573 740a 6465 6620 6265 666f 7265  quest.def before
+00000580: 5f61 7070 5f72 6571 7565 7374 2829 3a0a  _app_request():.
+00000590: 2020 2020 6270 2e69 6e69 745f 7365 7373      bp.init_sess
+000005a0: 696f 6e28 290a 6060 600a 0a44 7572 696e  ion().```..Durin
+000005b0: 6720 7468 6520 605f 5f69 6e69 745f 5f60  g the `__init__`
+000005c0: 206d 6574 686f 6420 6f66 2074 6865 2042   method of the B
+000005d0: 6c75 6570 7269 6e74 2063 6c61 7373 2c20  lueprint class, 
+000005e0: 6966 2074 6865 2063 6f6e 6669 6720 6172  if the config ar
+000005f0: 6775 6d65 6e74 2069 7320 6e6f 7420 7365  gument is not se
+00000600: 7420 746f 2060 4e6f 6e65 602c 2074 6865  t to `None`, the
+00000610: 2042 6c75 6570 7269 6e74 2077 696c 6c0a   Blueprint will.
+00000620: 6174 7465 6d70 7420 746f 206c 6f61 6420  attempt to load 
+00000630: 7468 6520 636f 6e66 6967 7572 6174 696f  the configuratio
+00000640: 6e20 6672 6f6d 2065 6974 6865 7220 6063  n from either `c
+00000650: 6f6e 6669 672e 746f 6d6c 6020 6669 6c65  onfig.toml` file
+00000660: 206f 7220 6120 6043 6f6e 6669 6760 2063   or a `Config` c
+00000670: 6c61 7373 2066 726f 6d20 6120 6063 6f6e  lass from a `con
+00000680: 6669 672e 7079 6020 6669 6c65 2e0a 0a54  fig.py` file...T
+00000690: 6f20 7365 6520 6d6f 7265 2061 626f 7574  o see more about
+000006a0: 2063 6f6e 6669 6775 7261 7469 6f6e 2073   configuration s
+000006b0: 6565 3a20 5b42 6c75 6570 7269 6e74 202f  ee: [Blueprint /
+000006c0: 2063 6f6e 6669 672e 785d 2862 6c75 6570   config.x](bluep
+000006d0: 7269 6e74 2d63 6f6e 6669 672d 782e 6874  rint-config-x.ht
+000006e0: 6d6c 290a 0a60 696d 706f 7274 5f72 6573  ml)..`import_res
+000006f0: 6f75 7263 6573 6020 6d65 7468 6f64 2077  ources` method w
+00000700: 696c 6c20 7761 6c6b 206f 6e65 206c 6576  ill walk one lev
+00000710: 656c 2064 6565 7020 696e 746f 2074 6865  el deep into the
+00000720: 2060 726f 7574 6573 6020 666f 6c64 6572   `routes` folder
+00000730: 2c20 616e 6420 696d 706f 7274 2061 6c6c  , and import all
+00000740: 2060 2e70 7960 2066 696c 6573 2061 7320   `.py` files as 
+00000750: 6d6f 6475 6c65 732e 0a46 6f72 206d 6f72  modules..For mor
+00000760: 6520 696e 666f 726d 6174 696f 6e20 7365  e information se
+00000770: 653a 205b 426c 7565 7072 696e 742e 7820  e: [Blueprint.x 
+00000780: 2f20 696d 706f 7274 5f72 6573 6f75 7263  / import_resourc
+00000790: 6573 5d28 626c 7565 7072 696e 745f 782d  es](blueprint_x-
+000007a0: 696d 706f 7274 5f72 6573 6f75 7263 6573  import_resources
+000007b0: 2e68 746d 6c29 0a0a 6069 6d70 6f72 745f  .html)..`import_
+000007c0: 6d6f 6465 6c73 6020 776f 726b 7320 7468  models` works th
+000007d0: 6520 7361 6d65 2061 7320 6069 6d70 2e69  e same as `imp.i
+000007e0: 6d70 6f72 745f 6d6f 6465 6c73 602c 2069  mport_models`, i
+000007f0: 7420 7769 6c6c 206c 6f6f 6b20 666f 7220  t will look for 
+00000800: 696e 7374 616e 6365 7320 6f66 2060 6462  instances of `db
+00000810: 2e4d 6f64 656c 6020 616e 6420 696d 706f  .Model` and impo
+00000820: 7274 2074 6865 6d2e 2054 6865 7365 0a77  rt them. These.w
+00000830: 696c 6c20 616c 736f 2062 6520 6176 6169  ill also be avai
+00000840: 6c61 626c 6520 696e 2074 6865 206d 6f64  lable in the mod
+00000850: 656c 206c 6f6f 6b75 7020 6d65 7468 6f64  el lookup method
+00000860: 2060 696d 702e 6d6f 6465 6c60 2e0a 466f   `imp.model`..Fo
+00000870: 7220 6d6f 7265 2069 6e66 6f72 6d61 7469  r more informati
+00000880: 6f6e 2073 6565 3a20 5b49 6d70 2e78 202f  on see: [Imp.x /
+00000890: 2069 6d70 6f72 745f 6d6f 6465 6c73 5d28   import_models](
+000008a0: 696d 705f 782d 696d 706f 7274 5f6d 6f64  imp_x-import_mod
+000008b0: 656c 732e 6874 6d6c 290a 0a60 696d 706f  els.html)..`impo
+000008c0: 7274 5f6e 6573 7465 645f 626c 7565 7072  rt_nested_bluepr
+000008d0: 696e 7473 6020 7769 6c6c 2064 6f20 7468  ints` will do th
+000008e0: 6520 7361 6d65 2061 7320 6069 6d70 2e69  e same as `imp.i
+000008f0: 6d70 6f72 745f 626c 7565 7072 696e 7473  mport_blueprints
+00000900: 602c 2062 7574 2077 696c 6c20 7265 6769  `, but will regi
+00000910: 7374 6572 2074 6865 2062 6c75 6570 7269  ster the bluepri
+00000920: 6e74 7320 666f 756e 6420 6173 0a6e 6573  nts found as.nes
+00000930: 7465 6420 746f 2074 6865 2063 7572 7265  ted to the curre
+00000940: 6e74 2062 6c75 6570 7269 6e74 2e20 466f  nt blueprint. Fo
+00000950: 7220 6578 616d 706c 6520 6077 7777 2e62  r example `www.b
+00000960: 6c75 6570 7269 6e74 5f6f 6e65 2e69 6e64  lueprint_one.ind
+00000970: 6578 600a 0a60 696d 706f 7274 5f6e 6573  ex`..`import_nes
+00000980: 7465 645f 626c 7565 7072 696e 7460 2062  ted_blueprint` b
+00000990: 6568 6176 6573 2074 6865 2073 616d 6520  ehaves the same 
+000009a0: 6173 2060 696d 706f 7274 5f6e 6573 7465  as `import_neste
+000009b0: 645f 626c 7565 7072 696e 7473 602c 2062  d_blueprints`, b
+000009c0: 7574 2077 696c 6c20 6f6e 6c79 2069 6d70  ut will only imp
+000009d0: 6f72 7420 6120 7369 6e67 6c65 2062 6c75  ort a single blu
+000009e0: 6570 7269 6e74 2e0a 0a60 6270 2e69 6e69  eprint...`bp.ini
+000009f0: 745f 7365 7373 696f 6e60 2077 696c 6c20  t_session` will 
+00000a00: 6c6f 6164 2074 6865 2073 6573 7369 6f6e  load the session
+00000a10: 2076 6172 6961 626c 6573 2066 726f 6d20   variables from 
+00000a20: 7468 6520 636f 6e66 6967 2066 696c 6520  the config file 
+00000a30: 696e 746f 2074 6865 2073 6573 7369 6f6e  into the session
+00000a40: 206f 626a 6563 742e 2046 6f72 206d 6f72   object. For mor
+00000a50: 6520 696e 666f 726d 6174 696f 6e0a 7365  e information.se
+00000a60: 653a 205b 426c 7565 7072 696e 742e 7820  e: [Blueprint.x 
+00000a70: 2f20 696e 6974 5f73 6573 7369 6f6e 5d28  / init_session](
+00000a80: 626c 7565 7072 696e 745f 782d 696e 6974  blueprint_x-init
+00000a90: 5f73 6573 7369 6f6e 2e68 746d 6c29 2061  _session.html) a
+00000aa0: 6e64 0a5b 426c 7565 7072 696e 7420 2f20  nd.[Blueprint / 
+00000ab0: 636f 6e66 6967 2e78 5d28 626c 7565 7072  config.x](bluepr
+00000ac0: 696e 742d 636f 6e66 6967 2d78 2e68 746d  int-config-x.htm
+00000ad0: 6c29 0a                                  l).
```

### Comparing `flask_imp-3.1.0/docs_md/Blueprint_x-import_models.md` & `flask_imp-4.0.0/docs_md/Blueprint_x-import_models.md`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/docs_md/Blueprint_x-import_nested_blueprint.md` & `flask_imp-4.0.0/docs_md/Blueprint_x-import_nested_blueprint.md`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/docs_md/Blueprint_x-import_nested_blueprints.md` & `flask_imp-4.0.0/docs_md/Blueprint_x-import_nested_blueprints.md`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/docs_md/Blueprint_x-import_resources.md` & `flask_imp-4.0.0/docs_md/Blueprint_x-import_resources.md`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/docs_md/Blueprint_x-tmpl.md` & `flask_imp-4.0.0/docs_md/Blueprint_x-tmpl.md`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/docs_md/CLI Commands-flask-imp blueprint.md` & `flask_imp-4.0.0/docs_md/CLI Commands-flask-imp blueprint.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ```
 Menu = CLI Commands/flask-imp blueprint
 Title = Generate a Flask-Imp Blueprint
 ```
 
 Flask-Imp has its own type of blueprint. It can read some configuration from a toml file and has some extra methods for
-auto importing. 
+auto importing.
 
 ```bash
 flask-imp blueprint --help
 ```
 
 To generate a Flask-Imp blueprint, run the following command:
 
@@ -24,34 +24,45 @@
 Folder to create blueprint in [Current Working Directory]: 
 ```
 
 As detailed in the prompt, the creation of the blueprint is relative to the current working directory. So to create a
 blueprint in the folder `app/blueprints`, you would enter `app/blueprints` in the prompt.
 
 ```text
+~ $ flask-imp blueprint
 (Creation is relative to the current working directory)
 Folder to create blueprint in [Current Working Directory]: app/blueprints
 ```
 
 You will then be prompted to enter a name for your blueprint:
 
 ```text
-(Creation is relative to the current working directory)
-Folder to create blueprint in [Current Working Directory]: app/blueprints 
+~ $ flask-imp blueprint
+...
 Name of the blueprint to create [my_new_blueprint]: 
 ```
 
 The default name is 'my_new_blueprint', we will change this to 'admin'
 
 ```text
-(Creation is relative to the current working directory)
-Folder to create blueprint in [Current Working Directory]: app/blueprints 
+~ $ flask-imp blueprint
+...
 Name of the blueprint to create [my_new_blueprint]: admin
 ```
 
+Finally, you will be asked what type of configuration file you would like to use:
+
+```text
+~ $ flask-imp blueprint
+...
+What type of config file would you like to use? (py, toml) [py]:
+```
+
+`py` is recommended, as it is more flexible.
+
 After creating your blueprint, the folder structure will look like this:
 
 ```text
 app/
 ├── blueprints
 │   └── admin
 │       ├── routes
@@ -71,20 +82,26 @@
 │       │       │   └── main.html
 │       │       ├── includes
 │       │       │   ├── footer.html
 │       │       │   └── header.html
 │       │       └── index.html
 │       │
 │       ├── __init__.py
-│       └─── config.toml
+│       └─── config.py
 │
 ...
 ```
 
 This is a self-contained blueprint, so it has its own static, templates and routes folders. You can now navigate '
 /admin'
 
-You can streamline this process by specifying the name of the blueprint and the folder to create it in, like so:
+You can streamline this process by specifying the name of the blueprint, the folder to 
+create it in and the configuration to use, like so:
 
 ```bash
-flask-imp blueprint -n admin -f app/blueprints
-```
+flask-imp blueprint -n admin -f app/blueprints --pyconfig
+```
+or
+```bash
+flask-imp blueprint -n admin -f app/blueprints --tomlconfig
+```
+for a toml config.
```

### Comparing `flask_imp-3.1.0/docs_md/CLI Commands-flask-imp init.md` & `flask_imp-4.0.0/docs_md/CLI Commands-flask-imp init.md`

 * *Files 18% similar despite different names*

```diff
@@ -9,62 +9,82 @@
 
 ```bash
 flask-imp init --help
 ```
 
 ## Create a new project
 
-Make sure you are in the virtual environment, and at the root of your project folder, then run the following command:
+Make sure you are in the virtual environment, and at the root of your 
+project folder, then run the following command:
 
 ```bash
 flask-imp init
 ```
 
-After running this command, you will be prompted to choose what type of app you want to deploy:
+After running this command, you will be prompted to choose what type of 
+app you want to deploy:
 
 ```text
 ~ $ flask-imp init
 What type of app would you like to create? (full, slim, minimal) [full]:
 ```
 
 See below for the differences between the app types.
 
 After this, you will be prompted to enter a name for your app:
 
 ```text
 ~ $ flask-imp init
+...
 What would you like to call your app? [app]: 
 ```
 
-'app' is the default name, so if you just press enter, your app will be called 'app'. You will then see this output:
+'app' is the default name, so if you just press enter, your app will be 
+called 'app'. You will then see this output:
+
+Next you will be asked what configuration file you would like to use:
+
+```text
+~ $ flask-imp init
+...
+What type of config file would you like to use? (py, toml) [py]:
+```
+
+`py` is recommended, as it is more flexible.
+
 
 ```text
+~ FILES CREATED WILL LOOP OUT HERE ~
+
 ===================
 Flask app deployed!
 ===================
  
 Your app has the default name of 'app'
 Flask will automatically look for this!
 Run: flask run --debug
 
 ```
 
 If you called your app something other than 'app', like 'new' for example, you will see:
 
 ```text
+~ FILES CREATED WILL LOOP OUT HERE ~
+
 ===================
 Flask app deployed!
 ===================
 
 Your app has the name of 'new'
 Run: flask --app new run --debug
 
 ```
 
-As you can see from the output, it gives you instructions on how to start your app, depending on the name you gave it.
+As you can see from the output, it gives you instructions on how to start your app, 
+depending on the name you gave it.
 
 You should see a new folder that has been given the name you specified in
 the `flask-imp init` command.
 
 ### Additional options
 
 You can also specify a name for your app in the command itself, like so:
@@ -83,25 +103,41 @@
 
 You can also deploy a minimal app, that will have no blueprints, models, or extensions, like so:
 
 ```bash
 flask-imp init -n my_app --minimal
 ```
 
+This also works for what configuration file you would like to use:
+
+```bash
+flask-imp init -n my_app --pyconfig
+```
+or
+```bash
+flask-imp init -n my_app --tomlconfig
+```
+
+This will create a new minimal app called 'my_app' with a python configuration file.
+
+```bash
+flask-imp init -n my_app --minimal --pyconfig
+```
+
 ## init Folder structures
 
 ### Full app
 
-`flask-imp init`:
+`flask-imp init --full`:
 
 ```text
 app/
 ├── blueprints
 │   └── www
-│       ├── config.toml
+│       ├── config.py
 │       ├── __init__.py
 │       ├── routes
 │       │   └── index.py
 │       ├── static
 │       │   ├── css
 │       │   │   └── water.css
 │       │   ├── img
@@ -144,15 +180,15 @@
 │       └── index.html
 │
 ├── models
 │   ├── example_user_table.py
 │   └── __init__.py
 │
 ├── __init__.py
-└── default.config.toml
+└── config.py
 ```
 
 ### Slim app
 
 `flask-imp init --slim`:
 
 ```text
@@ -173,15 +209,15 @@
 │           ├── 401.html
 │           ├── 403.html
 │           ├── 404.html
 │           ├── 405.html
 │           └── 500.html
 │
 ├── www
-│   ├── config.toml
+│   ├── config.py
 │   ├── __init__.py
 │   ├── routes
 │   │   └── index.py
 │   ├── static
 │   │   ├── css
 │   │   │   └── water.css
 │   │   ├── img
@@ -194,15 +230,15 @@
 │           │   └── main.html
 │           ├── includes
 │           │   ├── footer.html
 │           │   └── header.html
 │           └── index.html
 │
 ├── __init__.py
-└── default.config.toml
+└── config.py
 ```
 
 ### Minimal app
 
 `flask-imp init --minimal`:
 
 ```text
@@ -218,9 +254,9 @@
 │   │   │   └── flask-imp-logo.png
 │   │   └── favicon.ico
 │   ├── templates
 │   │   └── index.html
 │   └── routes.py
 │
 ├── __init__.py
-└── default.config.toml
+└── config.py
 ```
```

### Comparing `flask_imp-3.1.0/docs_md/Imp-Introduction.md` & `flask_imp-4.0.0/docs_md/Imp-Introduction.md`

 * *Files 17% similar despite different names*

```diff
@@ -44,131 +44,125 @@
 000002b0: 9482 2020 20e2 949c e294 80e2 9480 2063  ..   ......... c
 000002c0: 6f6e 7465 7874 5f70 726f 6365 7373 6f72  ontext_processor
 000002d0: 732f 2e2e 2e0a e294 8220 2020 e294 9ce2  s/.......   ....
 000002e0: 9480 e294 8020 7374 6174 6963 2f2e 2e2e  ..... static/...
 000002f0: 0ae2 9482 2020 20e2 9494 e294 80e2 9480  ....   .........
 00000300: 2074 656d 706c 6174 6573 2f2e 2e2e 0ae2   templates/.....
 00000310: 949c e294 80e2 9480 206d 6f64 656c 732f  ........ models/
-00000320: 2e2e 2e0a e294 9ce2 9480 e294 8020 6465  ............. de
-00000330: 6661 756c 742e 636f 6e66 6967 2e74 6f6d  fault.config.tom
-00000340: 6c0a e294 94e2 9480 e294 8020 5f5f 696e  l.......... __in
-00000350: 6974 5f5f 2e70 790a 6060 600a 0a48 6572  it__.py.```..Her
-00000360: 6527 7320 616e 2065 7861 6d70 6c65 206f  e's an example o
-00000370: 6620 7468 6520 6061 7070 2f5f 5f69 6e69  f the `app/__ini
-00000380: 745f 5f2e 7079 6020 6669 6c65 3a0a 0a60  t__.py` file:..`
-00000390: 6060 7079 7468 6f6e 0a66 726f 6d20 666c  ``python.from fl
-000003a0: 6173 6b20 696d 706f 7274 2046 6c61 736b  ask import Flask
-000003b0: 0a66 726f 6d20 666c 6173 6b5f 7371 6c61  .from flask_sqla
-000003c0: 6c63 6865 6d79 2069 6d70 6f72 7420 5351  lchemy import SQ
-000003d0: 4c41 6c63 6865 6d79 0a66 726f 6d20 666c  LAlchemy.from fl
-000003e0: 6173 6b5f 696d 7020 696d 706f 7274 2049  ask_imp import I
-000003f0: 6d70 0a0a 6462 203d 2053 514c 416c 6368  mp..db = SQLAlch
-00000400: 656d 7928 290a 696d 7020 3d20 496d 7028  emy().imp = Imp(
-00000410: 290a 0a0a 6465 6620 6372 6561 7465 5f61  )...def create_a
-00000420: 7070 2829 3a0a 2020 2020 6170 7020 3d20  pp():.    app = 
-00000430: 466c 6173 6b28 5f5f 6e61 6d65 5f5f 290a  Flask(__name__).
-00000440: 2020 2020 696d 702e 696e 6974 5f61 7070      imp.init_app
-00000450: 2861 7070 290a 2020 2020 6462 2e69 6e69  (app).    db.ini
-00000460: 745f 6170 7028 6170 7029 0a0a 2020 2020  t_app(app)..    
-00000470: 696d 702e 696d 706f 7274 5f61 7070 5f72  imp.import_app_r
-00000480: 6573 6f75 7263 6573 2822 7265 736f 7572  esources("resour
-00000490: 6365 7322 290a 2020 2020 696d 702e 696d  ces").    imp.im
-000004a0: 706f 7274 5f6d 6f64 656c 7328 226d 6f64  port_models("mod
-000004b0: 656c 7322 290a 2020 2020 696d 702e 696d  els").    imp.im
-000004c0: 706f 7274 5f62 6c75 6570 7269 6e74 7328  port_blueprints(
-000004d0: 2262 6c75 6570 7269 6e74 7322 290a 0a20  "blueprints").. 
-000004e0: 2020 2072 6574 7572 6e20 6170 700a 6060     return app.``
-000004f0: 600a 0a44 7572 696e 6720 6069 6d70 2e69  `..During `imp.i
-00000500: 6e69 745f 6170 7060 2074 6865 2060 6465  nit_app` the `de
-00000510: 6661 756c 742e 636f 6e66 6967 2e74 6f6d  fault.config.tom
-00000520: 6c60 2066 696c 6520 7769 6c6c 206c 6f61  l` file will loa
-00000530: 6420 7661 7269 6162 6c65 7320 756e 6465  d variables unde
-00000540: 7220 605b 464c 4153 4b5d 6020 696e 746f  r `[FLASK]` into
-00000550: 2074 6865 2046 6c61 736b 2061 7070 2063   the Flask app c
-00000560: 6f6e 6669 672e 0a49 7420 7769 6c6c 2061  onfig..It will a
-00000570: 6c73 6f20 6c6f 6164 2076 6172 6961 626c  lso load variabl
-00000580: 6573 2075 6e64 6572 2060 5b44 4154 4142  es under `[DATAB
-00000590: 4153 455d 6020 696e 746f 2074 6865 2046  ASE]` into the F
-000005a0: 6c61 736b 2061 7070 2063 6f6e 6669 6720  lask app config 
-000005b0: 6173 2060 5351 4c41 4c43 4845 4d59 5f44  as `SQLALCHEMY_D
-000005c0: 4154 4142 4153 455f 5552 4960 2e0a 0a56  ATABASE_URI`...V
-000005d0: 616c 7565 7320 756e 6465 7220 605b 5345  alues under `[SE
-000005e0: 5353 494f 4e5d 6020 6361 6e20 6265 206c  SSION]` can be l
-000005f0: 6f61 6465 6420 7769 7468 3a0a 0a60 6060  oaded with:..```
-00000600: 7079 7468 6f6e 0a40 6170 702e 6265 666f  python.@app.befo
-00000610: 7265 5f72 6571 7565 7374 0a64 6566 2062  re_request.def b
-00000620: 6566 6f72 655f 7265 7175 6573 7428 293a  efore_request():
-00000630: 0a20 2020 2069 6d70 2e69 6e69 745f 7365  .    imp.init_se
-00000640: 7373 696f 6e28 290a 6060 600a 0a53 6565  ssion().```..See
-00000650: 206d 6f72 6520 6162 6f75 7420 7468 6520   more about the 
-00000660: 636f 6e66 6967 2066 696c 6520 6865 7265  config file here
-00000670: 3a20 5b49 6d70 202f 2078 2e63 6f6e 6669  : [Imp / x.confi
-00000680: 672e 746f 6d6c 5d28 696d 702d 782d 636f  g.toml](imp-x-co
-00000690: 6e66 6967 2d74 6f6d 6c2e 6874 6d6c 290a  nfig-toml.html).
-000006a0: 0a60 696d 706f 7274 5f61 7070 5f72 6573  .`import_app_res
-000006b0: 6f75 7263 6573 6020 7769 6c6c 2077 616c  ources` will wal
-000006c0: 6b20 6f6e 6520 6c65 7665 6c20 6465 6570  k one level deep
-000006d0: 2069 6e74 6f20 7468 6520 6072 6573 6f75   into the `resou
-000006e0: 7263 6573 6020 666f 6c64 6572 2c20 616e  rces` folder, an
-000006f0: 6420 696d 706f 7274 2061 6c6c 2060 2e70  d import all `.p
-00000700: 7960 2066 696c 6573 2061 7320 6d6f 6475  y` files as modu
-00000710: 6c65 732e 2049 7420 7769 6c6c 0a61 6c73  les. It will.als
-00000720: 6f20 6368 6563 6b20 666f 7220 7468 6520  o check for the 
-00000730: 6578 6973 7465 6e63 6520 6f66 2061 2060  existence of a `
-00000740: 7374 6174 6963 6020 616e 6420 6074 656d  static` and `tem
-00000750: 706c 6174 6573 6020 666f 6c64 6572 2c20  plates` folder, 
-00000760: 616e 6420 7265 6769 7374 6572 2074 6865  and register the
-00000770: 6d20 7769 7468 2074 6865 2046 6c61 736b  m with the Flask
-00000780: 2061 7070 2e0a 0a54 6865 7265 2069 7320   app...There is 
-00000790: 6120 636f 7570 6c65 206f 6620 6f70 7469  a couple of opti
-000007a0: 6f6e 7320 666f 7220 6069 6d70 6f72 745f  ons for `import_
-000007b0: 6170 705f 7265 736f 7572 6365 7360 2074  app_resources` t
-000007c0: 6f20 636f 6e74 726f 6c20 7768 6174 0a69  o control what.i
-000007d0: 7320 696d 706f 7274 6564 2c20 7365 653a  s imported, see:
-000007e0: 205b 496d 702e 7820 2f20 696d 706f 7274   [Imp.x / import
-000007f0: 5f61 7070 5f72 6573 6f75 7263 6573 5d28  _app_resources](
-00000800: 696d 705f 782d 696d 706f 7274 5f61 7070  imp_x-import_app
-00000810: 5f72 6573 6f75 7263 6573 2e68 746d 6c29  _resources.html)
-00000820: 0a0a 6069 6d70 6f72 745f 6d6f 6465 6c73  ..`import_models
-00000830: 6020 7769 6c6c 2069 6d70 6f72 7420 616c  ` will import al
-00000840: 6c20 4d6f 6465 6c20 636c 6173 7365 7320  l Model classes 
-00000850: 6672 6f6d 2074 6865 2073 7065 6369 6669  from the specifi
-00000860: 6564 2066 696c 6520 6f72 2066 6f6c 6465  ed file or folde
-00000870: 722e 2049 7420 7769 6c6c 2061 6c73 6f20  r. It will also 
-00000880: 706c 6163 6520 6561 6368 206d 6f64 656c  place each model
-00000890: 2066 6f75 6e64 0a69 6e74 6f20 6120 6c6f   found.into a lo
-000008a0: 6f6b 7570 2074 6162 6c65 2074 6861 7420  okup table that 
-000008b0: 796f 7520 6361 6e20 6163 6365 7373 2076  you can access v
-000008c0: 6961 2060 696d 702e 6d6f 6465 6c60 0a0a  ia `imp.model`..
-000008d0: 5365 6520 6d6f 7265 2061 626f 7574 2068  See more about h
-000008e0: 6f77 2069 6d70 6f72 745f 6d6f 6465 6c73  ow import_models
-000008f0: 2061 6e64 2074 6865 206c 6f6f 6b75 700a   and the lookup.
-00000900: 6865 7265 3a20 5b49 6d70 2e78 202f 2069  here: [Imp.x / i
-00000910: 6d70 6f72 745f 6d6f 6465 6c73 5d28 696d  mport_models](im
-00000920: 705f 782d 696d 706f 7274 5f6d 6f64 656c  p_x-import_model
-00000930: 732e 6874 6d6c 2920 616e 6420 5b49 6d70  s.html) and [Imp
-00000940: 2e78 202f 206d 6f64 656c 5d28 696d 705f  .x / model](imp_
-00000950: 782d 6d6f 6465 6c2e 6874 6d6c 290a 0a60  x-model.html)..`
-00000960: 696d 706f 7274 5f62 6c75 6570 7269 6e74  import_blueprint
-00000970: 7360 2065 7870 6563 7473 2061 2066 6f6c  s` expects a fol
-00000980: 6465 7220 7468 6174 2063 6f6e 7461 696e  der that contain
-00000990: 7320 6d61 6e79 2042 6c75 6570 7269 6e74  s many Blueprint
-000009a0: 2061 7320 5079 7468 6f6e 2070 6163 6b61   as Python packa
-000009b0: 6765 732e 0a49 7420 7769 6c6c 2063 6865  ges..It will che
-000009c0: 636b 2065 6163 6820 626c 7565 7072 696e  ck each blueprin
-000009d0: 7420 666f 6c64 6572 2773 2060 5f5f 696e  t folder's `__in
-000009e0: 6974 5f5f 2e70 7960 2066 696c 6520 666f  it__.py` file fo
-000009f0: 7220 616e 2069 6e73 7461 6e63 6520 6f66  r an instance of
-00000a00: 2061 2046 6c61 736b 2042 6c75 6570 7269   a Flask Bluepri
-00000a10: 6e74 206f 7220 610a 466c 6173 6b2d 496d  nt or a.Flask-Im
-00000a20: 7020 426c 7565 7072 696e 742e 2054 6861  p Blueprint. Tha
-00000a30: 7420 696e 7374 616e 7420 7769 6c6c 2074  t instant will t
-00000a40: 6865 6e20 6265 2072 6567 6973 7465 7265  hen be registere
-00000a50: 6420 7769 7468 2074 6865 2046 6c61 736b  d with the Flask
-00000a60: 2061 7070 2e0a 0a53 6565 206d 6f72 6520   app...See more 
-00000a70: 6162 6f75 7420 686f 7720 696d 706f 7274  about how import
-00000a80: 696e 6720 626c 7565 7072 696e 7473 2077  ing blueprints w
-00000a90: 6f72 6b20 6865 7265 3a20 5b42 6c75 6570  ork here: [Bluep
-00000aa0: 7269 6e74 202f 2049 6e74 726f 6475 6374  rint / Introduct
-00000ab0: 696f 6e5d 2862 6c75 6570 7269 6e74 2d69  ion](blueprint-i
-00000ac0: 6e74 726f 6475 6374 696f 6e2e 6874 6d6c  ntroduction.html
-00000ad0: 290a                                     ).
+00000320: 2e2e 2e0a e294 9ce2 9480 e294 8020 636f  ............. co
+00000330: 6e66 6967 2e70 790a e294 94e2 9480 e294  nfig.py.........
+00000340: 8020 5f5f 696e 6974 5f5f 2e70 790a 6060  . __init__.py.``
+00000350: 600a 0a48 6572 6527 7320 616e 2065 7861  `..Here's an exa
+00000360: 6d70 6c65 206f 6620 7468 6520 6061 7070  mple of the `app
+00000370: 2f5f 5f69 6e69 745f 5f2e 7079 6020 6669  /__init__.py` fi
+00000380: 6c65 3a0a 0a60 6060 7079 7468 6f6e 0a66  le:..```python.f
+00000390: 726f 6d20 666c 6173 6b20 696d 706f 7274  rom flask import
+000003a0: 2046 6c61 736b 0a66 726f 6d20 666c 6173   Flask.from flas
+000003b0: 6b5f 7371 6c61 6c63 6865 6d79 2069 6d70  k_sqlalchemy imp
+000003c0: 6f72 7420 5351 4c41 6c63 6865 6d79 0a66  ort SQLAlchemy.f
+000003d0: 726f 6d20 666c 6173 6b5f 696d 7020 696d  rom flask_imp im
+000003e0: 706f 7274 2049 6d70 0a0a 6462 203d 2053  port Imp..db = S
+000003f0: 514c 416c 6368 656d 7928 290a 696d 7020  QLAlchemy().imp 
+00000400: 3d20 496d 7028 290a 0a0a 6465 6620 6372  = Imp()...def cr
+00000410: 6561 7465 5f61 7070 2829 3a0a 2020 2020  eate_app():.    
+00000420: 6170 7020 3d20 466c 6173 6b28 5f5f 6e61  app = Flask(__na
+00000430: 6d65 5f5f 290a 2020 2020 696d 702e 696e  me__).    imp.in
+00000440: 6974 5f61 7070 2861 7070 290a 2020 2020  it_app(app).    
+00000450: 6462 2e69 6e69 745f 6170 7028 6170 7029  db.init_app(app)
+00000460: 0a0a 2020 2020 696d 702e 696d 706f 7274  ..    imp.import
+00000470: 5f61 7070 5f72 6573 6f75 7263 6573 2822  _app_resources("
+00000480: 7265 736f 7572 6365 7322 290a 2020 2020  resources").    
+00000490: 696d 702e 696d 706f 7274 5f6d 6f64 656c  imp.import_model
+000004a0: 7328 226d 6f64 656c 7322 290a 2020 2020  s("models").    
+000004b0: 696d 702e 696d 706f 7274 5f62 6c75 6570  imp.import_bluep
+000004c0: 7269 6e74 7328 2262 6c75 6570 7269 6e74  rints("blueprint
+000004d0: 7322 290a 0a20 2020 2072 6574 7572 6e20  s")..    return 
+000004e0: 6170 700a 6060 600a 0a54 6865 2060 696e  app.```..The `in
+000004f0: 6974 5f61 7070 6020 6d65 7468 6f64 206f  it_app` method o
+00000500: 6620 7468 6520 496d 7020 636c 6173 7320  f the Imp class 
+00000510: 7769 6c6c 2061 7574 6f6d 6174 6963 616c  will automatical
+00000520: 6c79 206c 6f61 6420 636f 6e66 6967 7572  ly load configur
+00000530: 6174 696f 6e0a 6966 2074 6865 2063 6f6e  ation.if the con
+00000540: 6669 6720 6172 6775 6d65 6e74 2069 7320  fig argument is 
+00000550: 6e6f 7420 7365 7420 746f 2060 4e6f 6e65  not set to `None
+00000560: 602e 0a0a 416e 2061 7474 656d 7074 2074  `...An attempt t
+00000570: 6f20 6c6f 6164 2074 6865 2063 6f6e 6669  o load the confi
+00000580: 6775 7261 7469 6f6e 2066 726f 6d20 6569  guration from ei
+00000590: 7468 6572 2060 636f 6e66 6967 2e74 6f6d  ther `config.tom
+000005a0: 6c60 2066 696c 6520 6f72 2061 2060 436f  l` file or a `Co
+000005b0: 6e66 6967 600a 636c 6173 7320 6672 6f6d  nfig`.class from
+000005c0: 2061 2060 636f 6e66 6967 2e70 7960 2066   a `config.py` f
+000005d0: 696c 6520 7769 6c6c 2062 6520 6d61 6465  ile will be made
+000005e0: 2e0a 0a46 6f72 206d 6f72 6520 696e 666f  ...For more info
+000005f0: 726d 6174 696f 6e20 6162 6f75 7420 7468  rmation about th
+00000600: 6520 6063 6f6e 6669 6760 2070 6172 616d  e `config` param
+00000610: 6574 6572 2073 6565 3a20 5b49 6d70 202f  eter see: [Imp /
+00000620: 2063 6f6e 6669 672e 785d 2869 6d70 2d63   config.x](imp-c
+00000630: 6f6e 6669 672d 782e 6874 6d6c 290a 0a60  onfig-x.html)..`
+00000640: 696d 706f 7274 5f61 7070 5f72 6573 6f75  import_app_resou
+00000650: 7263 6573 6020 7769 6c6c 2077 616c 6b20  rces` will walk 
+00000660: 6f6e 6520 6c65 7665 6c20 6465 6570 2069  one level deep i
+00000670: 6e74 6f20 7468 6520 6072 6573 6f75 7263  nto the `resourc
+00000680: 6573 6020 666f 6c64 6572 2c20 616e 6420  es` folder, and 
+00000690: 696d 706f 7274 200a 616c 6c20 602e 7079  import .all `.py
+000006a0: 6020 6669 6c65 7320 6173 206d 6f64 756c  ` files as modul
+000006b0: 6573 2e20 0a49 7420 7769 6c6c 2061 6c73  es. .It will als
+000006c0: 6f20 6368 6563 6b20 666f 7220 7468 6520  o check for the 
+000006d0: 6578 6973 7465 6e63 6520 6f66 2061 2060  existence of a `
+000006e0: 7374 6174 6963 6020 616e 6420 6074 656d  static` and `tem
+000006f0: 706c 6174 6573 6020 666f 6c64 6572 2c20  plates` folder, 
+00000700: 616e 6420 7265 6769 7374 6572 2074 6865  and register the
+00000710: 6d20 7769 7468 2074 6865 2046 6c61 736b  m with the Flask
+00000720: 2061 7070 2e0a 0a54 6865 7265 2069 7320   app...There is 
+00000730: 6120 636f 7570 6c65 206f 6620 6f70 7469  a couple of opti
+00000740: 6f6e 7320 666f 7220 6069 6d70 6f72 745f  ons for `import_
+00000750: 6170 705f 7265 736f 7572 6365 7360 2074  app_resources` t
+00000760: 6f20 636f 6e74 726f 6c20 7768 6174 0a69  o control what.i
+00000770: 7320 696d 706f 7274 6564 2c20 7365 653a  s imported, see:
+00000780: 205b 496d 702e 7820 2f20 696d 706f 7274   [Imp.x / import
+00000790: 5f61 7070 5f72 6573 6f75 7263 6573 5d28  _app_resources](
+000007a0: 696d 705f 782d 696d 706f 7274 5f61 7070  imp_x-import_app
+000007b0: 5f72 6573 6f75 7263 6573 2e68 746d 6c29  _resources.html)
+000007c0: 0a0a 6069 6d70 6f72 745f 6d6f 6465 6c73  ..`import_models
+000007d0: 6020 7769 6c6c 2069 6d70 6f72 7420 616c  ` will import al
+000007e0: 6c20 4d6f 6465 6c20 636c 6173 7365 7320  l Model classes 
+000007f0: 6672 6f6d 2074 6865 2073 7065 6369 6669  from the specifi
+00000800: 6564 2066 696c 6520 6f72 2066 6f6c 6465  ed file or folde
+00000810: 722e 2049 7420 7769 6c6c 2061 6c73 6f20  r. It will also 
+00000820: 706c 6163 6520 6561 6368 206d 6f64 656c  place each model
+00000830: 2066 6f75 6e64 0a69 6e74 6f20 6120 6c6f   found.into a lo
+00000840: 6f6b 7570 2074 6162 6c65 2074 6861 7420  okup table that 
+00000850: 796f 7520 6361 6e20 6163 6365 7373 2076  you can access v
+00000860: 6961 2060 696d 702e 6d6f 6465 6c60 0a0a  ia `imp.model`..
+00000870: 5365 6520 6d6f 7265 2061 626f 7574 2068  See more about h
+00000880: 6f77 2069 6d70 6f72 745f 6d6f 6465 6c73  ow import_models
+00000890: 2061 6e64 2074 6865 206c 6f6f 6b75 700a   and the lookup.
+000008a0: 6865 7265 3a20 5b49 6d70 2e78 202f 2069  here: [Imp.x / i
+000008b0: 6d70 6f72 745f 6d6f 6465 6c73 5d28 696d  mport_models](im
+000008c0: 705f 782d 696d 706f 7274 5f6d 6f64 656c  p_x-import_model
+000008d0: 732e 6874 6d6c 2920 616e 6420 5b49 6d70  s.html) and [Imp
+000008e0: 2e78 202f 206d 6f64 656c 5d28 696d 705f  .x / model](imp_
+000008f0: 782d 6d6f 6465 6c2e 6874 6d6c 290a 0a60  x-model.html)..`
+00000900: 696d 706f 7274 5f62 6c75 6570 7269 6e74  import_blueprint
+00000910: 7360 2065 7870 6563 7473 2061 2066 6f6c  s` expects a fol
+00000920: 6465 7220 7468 6174 2063 6f6e 7461 696e  der that contain
+00000930: 7320 6d61 6e79 2042 6c75 6570 7269 6e74  s many Blueprint
+00000940: 2061 7320 5079 7468 6f6e 2070 6163 6b61   as Python packa
+00000950: 6765 732e 0a49 7420 7769 6c6c 2063 6865  ges..It will che
+00000960: 636b 2065 6163 6820 626c 7565 7072 696e  ck each blueprin
+00000970: 7420 666f 6c64 6572 2773 2060 5f5f 696e  t folder's `__in
+00000980: 6974 5f5f 2e70 7960 2066 696c 6520 666f  it__.py` file fo
+00000990: 7220 616e 2069 6e73 7461 6e63 6520 6f66  r an instance of
+000009a0: 2061 2046 6c61 736b 2042 6c75 6570 7269   a Flask Bluepri
+000009b0: 6e74 206f 7220 610a 466c 6173 6b2d 496d  nt or a.Flask-Im
+000009c0: 7020 426c 7565 7072 696e 742e 2054 6861  p Blueprint. Tha
+000009d0: 7420 696e 7374 616e 7420 7769 6c6c 2074  t instant will t
+000009e0: 6865 6e20 6265 2072 6567 6973 7465 7265  hen be registere
+000009f0: 6420 7769 7468 2074 6865 2046 6c61 736b  d with the Flask
+00000a00: 2061 7070 2e0a 0a53 6565 206d 6f72 6520   app...See more 
+00000a10: 6162 6f75 7420 686f 7720 696d 706f 7274  about how import
+00000a20: 696e 6720 626c 7565 7072 696e 7473 2077  ing blueprints w
+00000a30: 6f72 6b20 6865 7265 3a20 5b42 6c75 6570  ork here: [Bluep
+00000a40: 7269 6e74 202f 2049 6e74 726f 6475 6374  rint / Introduct
+00000a50: 696f 6e5d 2862 6c75 6570 7269 6e74 2d69  ion](blueprint-i
+00000a60: 6e74 726f 6475 6374 696f 6e2e 6874 6d6c  ntroduction.html
+00000a70: 290a                                     ).
```

### Comparing `flask_imp-3.1.0/docs_md/Imp_x-import_app_resources.md` & `flask_imp-4.0.0/docs_md/Imp_x-import_app_resources.md`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/docs_md/Imp_x-import_blueprint.md` & `flask_imp-4.0.0/docs_md/Imp_x-import_blueprint.md`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/docs_md/Imp_x-import_blueprints.md` & `flask_imp-4.0.0/docs_md/Imp_x-import_blueprints.md`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/docs_md/Imp_x-import_models.md` & `flask_imp-4.0.0/docs_md/Imp_x-import_models.md`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/docs_md/Imp_x-init_app-init.md` & `flask_imp-4.0.0/docs_md/Imp_x-init_app-init.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 ```
 Menu = Imp.x/init_app, __init__
 Title = Imp.init_app, __init__
 ```
 
 ```python
-init_app(
+def init_app(
     app: Flask,
-    app_config_file: Optional[str] = None,
-    ignore_missing_env_variables: bool = False
-) -> None
+    config: t.Union[str, ImpConfig] = os.environ.get("IMP_CONFIG")
+) -> None:
 # -or- 
 Imp(
-    app: Optional[Flask] = None,
-    app_config_file: Optional[str] = None,
-    ignore_missing_env_variables: bool = False
+    app: Flask,
+    config: t.Union[str, ImpConfig] = os.environ.get("IMP_CONFIG")
 ) -> None
 ```
 
 ---
 
 Initializes the flask app to work with flask-imp.
 
-If no `app_config_file` specified, an attempt to read `IMP_CONFIG` from the environment will be made.
+If no `config` specified, an attempt to read `IMP_CONFIG` from the environment will be made.
+
+The config value can be a toml file `my_config.toml`, for example; or an import string. An example
+of an import string would be `config.Config` where `config` is the module and `Config` is the class.
+
+If `IMP_CONFIG` is not in the environment variables, an attempt to load `config.toml` will be made. 
 
-If `IMP_CONFIG` is not in the environment variables, an attempt to load `default.config.toml` will be made.
+If `config.toml` is not found, an attempt to load a class called `Config` from `config.py` will be made. 
+The Config class must be an instance of `ImpConfig` `from flask_imp import ImpConfig`.
 
-`default.config.toml` will be created, and used if not found.
+An exception will be raised if none of the above methods are successful.
 
 If `ignore_missing_env_variables` is `True`, then missing environment variables will be ignored.
 
 If `ignore_missing_env_variables` is `False` (default), then missing environment variables will raise a ValueError
```

### Comparing `flask_imp-3.1.0/docs_md/Imp_x-init_session.md` & `flask_imp-4.0.0/docs_md/Imp_x-init_session.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,37 +11,36 @@
 000000a0: 6d6f 6e6c 7920 7573 6564 2069 6e20 6061  monly used in `a
 000000b0: 7070 2e62 6566 6f72 655f 7265 7175 6573  pp.before_reques
 000000c0: 7460 2e0a 0a60 6060 7079 7468 6f6e 0a40  t`...```python.@
 000000d0: 6170 702e 6265 666f 7265 5f72 6571 7565  app.before_reque
 000000e0: 7374 0a64 6566 2062 6566 6f72 655f 7265  st.def before_re
 000000f0: 7175 6573 7428 293a 0a20 2020 2069 6d70  quest():.    imp
 00000100: 2e69 6e69 745f 7365 7373 696f 6e28 290a  .init_session().
-00000110: 6060 600a 0a46 696c 653a 2060 6465 6661  ```..File: `defa
-00000120: 756c 742e 636f 6e66 6967 2e74 6f6d 6c60  ult.config.toml`
-00000130: 0a0a 6060 6074 6f6d 6c0a 2e2e 2e0a 5b53  ..```toml.....[S
-00000140: 4553 5349 4f4e 5d0a 6c6f 6767 6564 5f69  ESSION].logged_i
-00000150: 6e20 3d20 6661 6c73 650a 2e2e 2e0a 6060  n = false.....``
-00000160: 600a 0a60 6c6f 6767 6564 5f69 6e60 2069  `..`logged_in` i
-00000170: 7320 6e6f 7720 6176 6169 6c61 626c 6520  s now available 
-00000180: 696e 2074 6865 2073 6573 7369 6f6e 2e0a  in the session..
-00000190: 0a60 6060 7079 7468 6f6e 0a40 6170 702e  .```python.@app.
-000001a0: 726f 7574 6528 272f 6765 742d 7365 7373  route('/get-sess
-000001b0: 696f 6e2d 7661 6c75 6527 290a 6465 6620  ion-value').def 
-000001c0: 6c6f 6769 6e28 293a 0a20 2020 2070 7269  login():.    pri
-000001d0: 6e74 2873 6573 7369 6f6e 5b27 6c6f 6767  nt(session['logg
-000001e0: 6564 5f69 6e27 5d29 0a20 2020 2072 6574  ed_in']).    ret
-000001f0: 7572 6e20 2243 6865 636b 2054 6572 6d69  urn "Check Termi
-00000200: 6e61 6c22 0a60 6060 0a0a 604f 7574 7075  nal".```..`Outpu
-00000210: 743a 2046 616c 7365 600a 0a43 616e 2061  t: False`..Can a
-00000220: 6c73 6f20 6265 2075 7365 6420 746f 2072  lso be used to r
-00000230: 6573 6574 2074 6865 2076 616c 7565 7320  eset the values 
-00000240: 696e 2074 6865 2073 6573 7369 6f6e 2e20  in the session. 
-00000250: 4865 7265 2773 2061 6e20 6578 616d 706c  Here's an exampl
-00000260: 653a 0a0a 6060 6070 7974 686f 6e0a 4061  e:..```python.@a
-00000270: 7070 2e72 6f75 7465 2827 2f6c 6f67 6f75  pp.route('/logou
-00000280: 7427 290a 6465 6620 6c6f 676f 7574 2829  t').def logout()
-00000290: 3a0a 2020 2020 7365 7373 696f 6e2e 636c  :.    session.cl
-000002a0: 6561 7228 290a 2020 2020 696d 702e 696e  ear().    imp.in
-000002b0: 6974 5f73 6573 7369 6f6e 2829 0a20 2020  it_session().   
-000002c0: 2072 6574 7572 6e20 7265 6469 7265 6374   return redirect
-000002d0: 2875 726c 5f66 6f72 2827 696e 6465 7827  (url_for('index'
-000002e0: 2929 0a60 6060                           )).```
+00000110: 6060 600a 0a46 696c 653a 2060 636f 6e66  ```..File: `conf
+00000120: 6967 2e74 6f6d 6c60 0a0a 6060 6074 6f6d  ig.toml`..```tom
+00000130: 6c0a 2e2e 2e0a 5b53 4553 5349 4f4e 5d0a  l.....[SESSION].
+00000140: 6c6f 6767 6564 5f69 6e20 3d20 6661 6c73  logged_in = fals
+00000150: 650a 2e2e 2e0a 6060 600a 0a60 6c6f 6767  e.....```..`logg
+00000160: 6564 5f69 6e60 2069 7320 6e6f 7720 6176  ed_in` is now av
+00000170: 6169 6c61 626c 6520 696e 2074 6865 2073  ailable in the s
+00000180: 6573 7369 6f6e 2e0a 0a60 6060 7079 7468  ession...```pyth
+00000190: 6f6e 0a40 6170 702e 726f 7574 6528 272f  on.@app.route('/
+000001a0: 6765 742d 7365 7373 696f 6e2d 7661 6c75  get-session-valu
+000001b0: 6527 290a 6465 6620 6c6f 6769 6e28 293a  e').def login():
+000001c0: 0a20 2020 2070 7269 6e74 2873 6573 7369  .    print(sessi
+000001d0: 6f6e 5b27 6c6f 6767 6564 5f69 6e27 5d29  on['logged_in'])
+000001e0: 0a20 2020 2072 6574 7572 6e20 2243 6865  .    return "Che
+000001f0: 636b 2054 6572 6d69 6e61 6c22 0a60 6060  ck Terminal".```
+00000200: 0a0a 604f 7574 7075 743a 2046 616c 7365  ..`Output: False
+00000210: 600a 0a43 616e 2061 6c73 6f20 6265 2075  `..Can also be u
+00000220: 7365 6420 746f 2072 6573 6574 2074 6865  sed to reset the
+00000230: 2076 616c 7565 7320 696e 2074 6865 2073   values in the s
+00000240: 6573 7369 6f6e 2e20 4865 7265 2773 2061  ession. Here's a
+00000250: 6e20 6578 616d 706c 653a 0a0a 6060 6070  n example:..```p
+00000260: 7974 686f 6e0a 4061 7070 2e72 6f75 7465  ython.@app.route
+00000270: 2827 2f6c 6f67 6f75 7427 290a 6465 6620  ('/logout').def 
+00000280: 6c6f 676f 7574 2829 3a0a 2020 2020 7365  logout():.    se
+00000290: 7373 696f 6e2e 636c 6561 7228 290a 2020  ssion.clear().  
+000002a0: 2020 696d 702e 696e 6974 5f73 6573 7369    imp.init_sessi
+000002b0: 6f6e 2829 0a20 2020 2072 6574 7572 6e20  on().    return 
+000002c0: 7265 6469 7265 6374 2875 726c 5f66 6f72  redirect(url_for
+000002d0: 2827 696e 6465 7827 2929 0a60 6060       ('index')).```
```

### Comparing `flask_imp-3.1.0/docs_md/Imp_x-model.md` & `flask_imp-4.0.0/docs_md/Imp_x-model.md`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/docs_md/__menu__.md` & `flask_imp-4.0.0/docs_md/__menu__.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 - CLI Commands
     - flask-imp init
     - flask-imp blueprint
 - Imp
     - Introduction
-    - x.config.toml
-    - Load Env Variables
+    - config.x
 - Blueprint
     - Introduction
-    - config.toml
+    - config.x
 - Imp.x
     - init_app, __init__
     - init_session
     - import_app_resources
     - import_blueprint
     - import_blueprints
     - import_models
```

### Comparing `flask_imp-3.1.0/docs_md/flask_imp_auth-authenticate_password.md` & `flask_imp-4.0.0/docs_md/flask_imp_auth-authenticate_password.md`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/docs_md/flask_imp_auth-encrypt_password.md` & `flask_imp-4.0.0/docs_md/flask_imp_auth-encrypt_password.md`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/docs_md/flask_imp_auth-generate_email_validator.md` & `flask_imp-4.0.0/docs_md/flask_imp_auth-generate_email_validator.md`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/docs_md/flask_imp_auth-generate_private_key.md` & `flask_imp-4.0.0/docs_md/flask_imp_auth-generate_private_key.md`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/docs_md/flask_imp_auth-generate_salt.md` & `flask_imp-4.0.0/docs_md/flask_imp_auth-generate_salt.md`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/docs_md/flask_imp_auth-is_email_address_valid.md` & `flask_imp-4.0.0/docs_md/flask_imp_auth-is_email_address_valid.md`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/docs_md/flask_imp_auth-is_username_valid.md` & `flask_imp-4.0.0/docs_md/flask_imp_auth-is_username_valid.md`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/docs_md/flask_imp_security-api_login_check.md` & `flask_imp-4.0.0/docs_md/flask_imp_security-api_login_check.md`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/docs_md/flask_imp_security-include_csrf.md` & `flask_imp-4.0.0/docs_md/flask_imp_security-include_csrf.md`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/docs_md/flask_imp_security-login_check.md` & `flask_imp-4.0.0/docs_md/flask_imp_security-login_check.md`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/docs_md/flask_imp_security-permission_check.md` & `flask_imp-4.0.0/docs_md/flask_imp_security-permission_check.md`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/flask_imp/_cli/__init__.py` & `flask_imp-4.0.0/flask_imp/_cli/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,16 +26,34 @@
     "-n",
     "--name",
     nargs=1,
     default="my_new_blueprint",
     prompt="Name of the blueprint to create",
     help="The name of the blueprint to create",
 )
-def add_blueprint(folder, name):
-    _add_blueprint(folder, name)
+@click.option(
+    "-pyc", "--pyconfig", is_flag=True, default=False, help="Use python config files"
+)
+@click.option(
+    "-tc", "--tomlconfig", is_flag=True, default=False, help="Use python config files"
+)
+def add_blueprint(folder, name, pyconfig, tomlconfig):
+    if not pyconfig and not tomlconfig:
+        choice = click.prompt(
+            "What type of config file would you like to use?",
+            default="py",
+            type=click.Choice(["py", "toml"]),
+        )
+
+        if choice == "py":
+            pyconfig = True
+        elif choice == "toml":
+            pyconfig = False
+
+    _add_blueprint(folder, name, pyconfig=pyconfig)
 
 
 @cli.command("init", help="Create a new flask-imp app")
 @click.option(
     "-n",
     "--name",
     nargs=1,
@@ -43,15 +61,21 @@
     help="The name of the app folder that will be created",
 )
 @click.option("-f", "--full", is_flag=True, default=False, help="Create a full app")
 @click.option("-s", "--slim", is_flag=True, default=False, help="Create a slim app")
 @click.option(
     "-m", "--minimal", is_flag=True, default=False, help="Create a minimal app"
 )
-def init_new_app(name, full, slim, minimal):
+@click.option(
+    "-pyc", "--pyconfig", is_flag=True, default=False, help="Use python config files"
+)
+@click.option(
+    "-tc", "--tomlconfig", is_flag=True, default=False, help="Use python config files"
+)
+def init_new_app(name, full, slim, minimal, pyconfig, tomlconfig):
     if not full and not slim and not minimal:
         choice = click.prompt(
             "What type of app would you like to create?",
             default="full",
             type=click.Choice(["full", "slim", "minimal"]),
         )
 
@@ -67,8 +91,20 @@
 
     else:
         set_name = name
 
     if minimal:
         slim = True
 
-    _init_app(set_name, full, slim, minimal)
+    if not pyconfig and not tomlconfig:
+        choice = click.prompt(
+            "What type of config file would you like to use?",
+            default="py",
+            type=click.Choice(["py", "toml"]),
+        )
+
+        if choice == "py":
+            pyconfig = True
+        elif choice == "toml":
+            pyconfig = False
+
+    _init_app(set_name, full, slim, minimal, pyconfig)
```

### Comparing `flask_imp-3.1.0/flask_imp/_cli/blueprint.py` & `flask_imp-4.0.0/flask_imp/_cli/blueprint.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,21 @@
 from .filelib.head_tag_generator import head_tag_generator
 from .filelib.main_js import main_js
 from .filelib.water_css import water_css
 from .helpers import Sprinkles as Sp
 from .helpers import to_snake_case
 
 
-def add_blueprint(folder, name, _init_app: bool = False, _cwd: Optional[Path] = None):
+def add_blueprint(
+    folder,
+    name,
+    _init_app: bool = False,
+    _cwd: Optional[Path] = None,
+    pyconfig: bool = False,
+):
     click.echo(f"{Sp.OKGREEN}Creating Blueprint: {name}")
 
     if _cwd:
         cwd = _cwd
 
     else:
         if folder != "Current Working Directory":
@@ -41,18 +47,14 @@
         "templates/extends": cwd / name / "templates" / name / "extends",
         "templates/includes": cwd / name / "templates" / name / "includes",
     }
 
     # Files
     files = {
         "root/__init__.py": (folders["root"] / "__init__.py", BpFlib.init_py),
-        "root/config.toml": (
-            folders["root"] / "config.toml",
-            BpFlib.config_toml.format(name=name, url_prefix="" if _init_app else name),
-        ),
         "routes/index.py": (
             folders["routes"] / "index.py",
             BpFlib.routes_index_py.format(name=name),
         ),
         "static/img/flask-imp-logo.png": (
             folders["static/img"] / "flask-imp-logo.png",
             flask_imp_logo,
@@ -97,14 +99,25 @@
             BpFlib.templates_includes_footer_html.format(
                 footer_html=folders["templates/includes"] / "footer.html",
                 main_html=folders["templates/extends"] / "main.html",
             ),
         ),
     }
 
+    if pyconfig:
+        files["root/config.py"] = (
+            folders["root"] / "config.py",
+            BpFlib.config_py.format(name=name, url_prefix="" if _init_app else name),
+        )
+    else:
+        files["root/config.toml"] = (
+            folders["root"] / "config.toml",
+            BpFlib.config_toml.format(name=name, url_prefix="" if _init_app else name),
+        )
+
     # Loop create folders
     for folder, path in folders.items():
         if not path.exists():
             path.mkdir(parents=True)
             click.echo(f"{Sp.OKGREEN}Blueprint folder: {folder}, created{Sp.END}")
         else:
             click.echo(
```

### Comparing `flask_imp-3.1.0/flask_imp/_cli/filelib/all_files.py` & `flask_imp-4.0.0/flask_imp/_cli/filelib/all_files.py`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/flask_imp/_cli/filelib/blueprint.py` & `flask_imp-4.0.0/flask_imp/_cli/filelib/blueprint.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,29 +27,64 @@
 #URL_DEFAULTS = {{}}
 STATIC_FOLDER = "static"
 TEMPLATE_FOLDER = "templates"
 STATIC_URL_PATH = "/static"
 #ROOT_PATH = ""
 #CLI_GROUP = ""
 
-[SESSION]
+[INIT_SESSION]
 #{name}_session = "yes"
 
 # Set ENABLED to true to allow the blueprint
 # to create a database bind, change settings accordingly.
 [DATABASE_BIND]
 ENABLED = false
 DIALECT = "sqlite"
-DATABASE_NAME = "{name}"
+NAME = "{name}"
+BIND_KEY = "{name}"
 LOCATION = ""
 PORT = ""
 USERNAME = ""
 PASSWORD = ""
 """
 
+    # Format to: name, url_prefix
+    config_py = """\
+from flask_imp import ImpBlueprintConfig, DatabaseConfig
+
+
+class Config(ImpBlueprintConfig):
+    ENABLED: bool = True
+    URL_PREFIX: str = "/{url_prefix}"
+    # SUBDOMAIN: str = ""
+    # URL_DEFAULTS: dict = {{}}
+    STATIC_FOLDER: str = "static"
+    TEMPLATE_FOLDER: str = "templates"
+    STATIC_URL_PATH: str = "/static"
+    # ROOT_PATH: str = ""
+    # CLI_GROUP: str = ""
+
+    INIT_SESSION: dict = {{
+        "{name}_session": "yes"
+    }}
+
+    DATABASE_BINDS: = {{
+        DatabaseConfig(
+            ENABLED=False,
+            DIALECT="sqlite",
+            NAME="{name}",
+            BIND_KEY="{name}",
+            LOCATION="",
+            PORT=0,
+            USERNAME="",
+            PASSWORD="",
+        )
+    }}
+    """
+
     # Format to: Name
     routes_index_py = """\
 from flask import render_template
 
 from .. import bp
```

### Comparing `flask_imp-3.1.0/flask_imp/_cli/filelib/favicon.py` & `flask_imp-4.0.0/flask_imp/_cli/filelib/favicon.py`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/flask_imp/_cli/filelib/flask_imp_logo.py` & `flask_imp-4.0.0/flask_imp/_cli/filelib/flask_imp_logo.py`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/flask_imp/_cli/filelib/head_tag_generator.py` & `flask_imp-4.0.0/flask_imp/_cli/filelib/head_tag_generator.py`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/flask_imp/_cli/filelib/water_css.py` & `flask_imp-4.0.0/flask_imp/_cli/filelib/water_css.py`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/flask_imp/_cli/helpers.py` & `flask_imp-4.0.0/flask_imp/_cli/helpers.py`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/flask_imp/_cli/init.py` & `flask_imp-4.0.0/flask_imp/_cli/init.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,21 @@
 from .filelib.favicon import favicon
 from .filelib.flask_imp_logo import flask_imp_logo
 from .filelib.head_tag_generator import head_tag_generator
 from .filelib.water_css import water_css
 from .helpers import Sprinkles as Sp
 
 
-def init_app(name, _full: bool = False, _slim: bool = False, _minimal: bool = False):
+def init_app(
+    name,
+    _full: bool = False,
+    _slim: bool = False,
+    _minimal: bool = False,
+    pyconfig: bool = False,
+):
     click.echo(f"{Sp.OKGREEN}Creating App: {name}")
 
     cwd = Path.cwd()
 
     app_folder = cwd / name
 
     if app_folder.exists():
@@ -64,20 +70,14 @@
                 "resources/filters": app_folder / "resources" / "filters",
                 "resources/routes": app_folder / "resources" / "routes",
             }
         )
 
     # Files
     files = {
-        "root/default.config.toml": (
-            folders["root"] / "default.config.toml",
-            AppFileLib.default_init_config_toml.format(secret_key=os.urandom(24).hex())
-            if not _slim
-            else AppFileLib.default_config_toml.format(secret_key=os.urandom(24).hex()),
-        ),
         "root/__init__.py": (
             folders["root"] / "__init__.py",
             AppFileLib.init_py.format(app_name=name)
             if not _slim
             else AppFileLib.slim_init_py.format(app_name=name)
             if not _minimal
             else AppFileLib.minimal_init_py.format(app_name=name),
@@ -90,14 +90,33 @@
             folders["extensions"] / "__init__.py",
             AppFileLib.extensions_init_py
             if not _slim
             else AppFileLib.slim_extensions_init_py,
         ),
     }
 
+    if pyconfig:
+        files["root/config.py"] = (
+            folders["root"] / "config.py",
+            AppFileLib.default_config_py.format(secret_key=os.urandom(24).hex())
+            if _full
+            else AppFileLib.default_slim_config_py.format(
+                secret_key=os.urandom(24).hex()
+            ),
+        )
+    else:
+        files["root/config.toml"] = (
+            folders["root"] / "config.toml",
+            AppFileLib.default_config_toml.format(secret_key=os.urandom(24).hex())
+            if _full
+            else AppFileLib.default_slim_config_toml.format(
+                secret_key=os.urandom(24).hex()
+            ),
+        )
+
     if _minimal:
         files.update(
             {
                 "resources/templates/index.html": (
                     folders["resources/templates"] / "index.html",
                     GlobalFileLib.minimal_templates_index_html.format(
                         head_tag=head_tag_generator(
@@ -222,14 +241,15 @@
 
     if not _minimal:
         add_blueprint(
             f"{name}/blueprints",
             "www",
             _init_app=True,
             _cwd=folders["blueprints"] if not _slim else folders["root"],
+            pyconfig=pyconfig,
         )
 
     click.echo(" ")
     click.echo(f"{Sp.OKBLUE}==================={Sp.END}")
     click.echo(f"{Sp.OKBLUE}Flask app deployed!{Sp.END}")
     click.echo(f"{Sp.OKBLUE}==================={Sp.END}")
     click.echo(" ")
```

### Comparing `flask_imp-3.1.0/flask_imp/auth/__init__.py` & `flask_imp-4.0.0/flask_imp/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/flask_imp/auth/__legacy__.py` & `flask_imp-4.0.0/flask_imp/auth/__legacy__.py`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/flask_imp/auth/__private_funcs__.py` & `flask_imp-4.0.0/flask_imp/auth/__private_funcs__.py`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/flask_imp/auth/authenticate_password.py` & `flask_imp-4.0.0/flask_imp/auth/authenticate_password.py`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/flask_imp/auth/dataclasses.py` & `flask_imp-4.0.0/flask_imp/auth/dataclasses.py`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/flask_imp/auth/encrypt_password.py` & `flask_imp-4.0.0/flask_imp/auth/encrypt_password.py`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/flask_imp/auth/generate_alphanumeric_validator.py` & `flask_imp-4.0.0/flask_imp/auth/generate_alphanumeric_validator.py`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/flask_imp/auth/generate_email_validator.py` & `flask_imp-4.0.0/flask_imp/auth/generate_email_validator.py`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/flask_imp/auth/generate_numeric_validator.py` & `flask_imp-4.0.0/flask_imp/auth/generate_numeric_validator.py`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/flask_imp/auth/generate_password.py` & `flask_imp-4.0.0/flask_imp/auth/generate_password.py`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/flask_imp/auth/generate_private_key.py` & `flask_imp-4.0.0/flask_imp/auth/generate_private_key.py`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/flask_imp/auth/is_email_address_valid.py` & `flask_imp-4.0.0/flask_imp/auth/is_email_address_valid.py`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/flask_imp/auth/is_username_valid.py` & `flask_imp-4.0.0/flask_imp/auth/is_username_valid.py`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/flask_imp/blueprint.py` & `flask_imp-4.0.0/flask_imp/imp_blueprint.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,59 @@
-import logging
+import typing as t
 from functools import partial
 from importlib import import_module
 from importlib.util import find_spec
 from inspect import getmembers
 from pathlib import Path
 
 from flask import Blueprint
 from flask import session
 
-from .helpers import _init_bp_config, _build_database_uri
-from .utilities import cast_to_import_str
+from .config_imp_blueprint_template import ImpBlueprintConfigTemplate
+from .config_object_parser import load_object
+from .config_toml_parser import load_app_blueprint_toml
+from .exceptions import NoConfigProvided
+from .protocols import Flask
+from .utilities import (
+    _toml_suffix,
+    cast_to_import_str,
+    slug,
+    _partial_models_import,
+    build_database_binds,
+)
+
+
+def _prevent_if_disabled(func) -> t.Callable:
+    def decorator(self, *args, **kwargs):
+        if not self.config.ENABLED:
+            return
+        return func(self, *args, **kwargs)
+
+    return decorator
 
 
 class ImpBlueprint(Blueprint):
     """
     A Class that extends the capabilities of the Flask Blueprint class.
     """
 
-    enabled: bool = False
+    config: ImpBlueprintConfigTemplate
+
     location: Path
     bp_name: str
     package: str
 
-    session: dict
-    settings: dict
-    database_bind: dict
-
-    __model_imports__: list
-    __nested_blueprint_imports__: list
+    _models: t.Set = None
+    _nested_blueprints: t.Union[t.Set, t.Set[t.Union["ImpBlueprint", Blueprint]]] = None
 
-    def __init__(self, dunder_name: str, config_file: str = "config.toml") -> None:
+    def __init__(
+        self,
+        dunder_name: str,
+        config: t.Union[str, ImpBlueprintConfigTemplate] = None,
+    ) -> None:
         """
         Creates a new ImpBlueprint instance.
 
         :raw-html:`<br />`
 
         `config.toml` must be in the same directory as the `__init__.py` file.
 
@@ -69,65 +89,89 @@
         :raw-html:`<br />`
 
         -----
 
         :param dunder_name: __name__
         :param config_file: Must be in the same directory as the blueprint, defaults to "config.toml"
         """
-        self.package = dunder_name
-        self.__model_imports__ = []
-        self.__nested_blueprint_imports__ = []
 
+        if not hasattr(self, "_models") or self._models is None:
+            self._models = set()
+
+        if not hasattr(self, "_nested_blueprints") or self._nested_blueprints is None:
+            self._nested_blueprints = set()
+
+        self.package = dunder_name
         spec = find_spec(self.package)
 
         if spec is None:
             raise ImportError(f"Cannot find origin of {self.package}")
 
         self.location = Path(f"{spec.origin}").parent
         self.bp_name = self.location.name
 
-        (
-            self.enabled,
-            self.session,
-            self.settings,
-            self.database_bind,
-        ) = _init_bp_config(
-            self.bp_name,
-            self.location / config_file,
-        )
+        if config is None:
+            if Path(self.location / "config.py").exists():
+                config = "config.Config"
+
+            elif Path(self.location / "config.toml").exists():
+                config = "config.toml"
+
+            else:
+                raise NoConfigProvided(
+                    f"No config was provided, and no default config was found in {self.location}"
+                )
+
+        self.load_config(config, self.location)
+
+        if not self.config.URL_PREFIX:
+            self.config.URL_PREFIX = f"/{slug(self.bp_name)}"
+
+        super().__init__(self.bp_name, self.package, **self.config.super_settings())
+
+    def set_app_config(self, flask_app: Flask, app_path: Path) -> None:
+        build_database_binds(flask_app, app_path, self.config.DATABASE_BINDS)
 
-        if self.enabled:
-            super().__init__(self.bp_name, self.package, **self.settings)
+    def load_config(
+        self,
+        config: t.Union[str, ImpBlueprintConfigTemplate],
+        location: t.Optional[Path],
+    ) -> None:
+        if isinstance(config, ImpBlueprintConfigTemplate):
+            self.config = config
 
+        if isinstance(config, str):
+            toml_file = Path(location / config)
+            if toml_file.exists() and toml_file.suffix in _toml_suffix:
+                self.config = load_app_blueprint_toml(config, location)
+            else:
+                self.config = load_object(f"{self.package}.{config}")
+
+    @_prevent_if_disabled
     def import_resources(self, folder: str = "routes") -> None:
         """
         Will import all the resources (cli, routes, filters, context_processors...) from the given folder.
         Given folder must be relative to the blueprint (in the same folder as the __init__.py file).
 
-        :raw-html:`<br />`
-
         **Example use:**
 
-        :raw-html:`<br />`
-
         --- Folder structure ---
 
         .. code-block::
 
             my_blueprint
             ├── user_routes
             │   ├── user_dashboard.py
             │   └── user_settings.py
             ├── car_routes
             │   ├── car_dashboard.py
             │   └── car_settings.py
             ├── __init__.py
             └── config.toml
 
-
         :raw-html:`<br />`
 
         --- __init__.py ---
 
         .. code-block::
 
             from flask_imp import Blueprint
@@ -158,30 +202,29 @@
 
         :raw-html:`<br />`
 
         -----
 
         :param folder: Folder to look for resources in. Defaults to "routes". Must be relative.
         """
-        if not self.enabled:
-            return
 
         resource_path = self.location / folder
         if not resource_path.exists():
             raise NotADirectoryError(f"{resource_path} is not a directory")
 
         resources = resource_path.glob("*.py")
         for resource in resources:
             try:
                 import_module(f"{self.package}.{folder}.{resource.stem}")
             except ImportError as e:
                 raise ImportError(
                     f"Error when importing {self.package}.{resource}: {e}"
                 )
 
+    @_prevent_if_disabled
     def import_nested_blueprint(self, blueprint: str) -> None:
         """
         Imports the specified Flask-Imp Blueprint or a standard Flask Blueprint as a nested blueprint,
         under the current blueprint.
 
         :raw-html:`<br />`
 
@@ -229,21 +272,30 @@
         :raw-html:`<br />`
 
         -----
 
         :param blueprint: The blueprint (folder name) to import. Must be relative.
         :return: None
         """
-        if not self.enabled:
-            return
+        if Path(blueprint).is_absolute():
+            potential_bp = Path(blueprint)
+        else:
+            potential_bp = Path(self.location / blueprint)
 
-        self.__nested_blueprint_imports__.append(
-            partial(self._partial_nested_blueprint_import, blueprint=blueprint)
-        )
+        if potential_bp.exists() and potential_bp.is_dir():
+            module = import_module(
+                cast_to_import_str(self.package.split(".")[0], potential_bp)
+            )
+            for name, potential in getmembers(module):
+                if isinstance(potential, Blueprint) or isinstance(
+                    potential, ImpBlueprint
+                ):
+                    self._nested_blueprints.add(potential)
 
+    @_prevent_if_disabled
     def import_nested_blueprints(self, folder: str) -> None:
         """
         Imports all blueprints in the given folder.
 
         .. Note::
             Folder has no requirement to be a Python package.
 
@@ -300,22 +352,24 @@
         :raw-html:`<br />`
 
         -----
 
         :param folder: Folder to look for nested blueprints in.
         Must be relative.
         """
-        if not self.enabled:
-            return
 
         folder_path = Path(self.location / folder)
 
+        if not folder_path.exists() or not folder_path.is_dir():
+            raise NotADirectoryError(f"{folder_path} is not a directory")
+
         for potential_bp in folder_path.iterdir():
-            self.import_nested_blueprint(potential_bp.as_posix())
+            self.import_nested_blueprint(f"{potential_bp}")
 
+    @_prevent_if_disabled
     def init_session(self) -> None:
         """
         Similar to the `Imp.init_session()` method,
         but scoped to the current blueprint's config.toml session values.
 
         :raw-html:`<br />`
 
@@ -332,22 +386,20 @@
         :raw-html:`<br />`
 
         -----
 
         :return: None
 
         """
-        if not self.enabled:
-            return
-
-        for key in self.session:
+        for key in self.config.INIT_SESSION or {}:
             if key not in session:
-                session.update(self.session)
+                session.update(self.config.INIT_SESSION)
                 break
 
+    @_prevent_if_disabled
     def import_models(self, file_or_folder: str) -> None:
         """
         Same actions as `Imp.import_models()`, but scoped to the current blueprint's package.
 
         :raw-html:`<br />`
 
         **Each model found will be added to the model registry.**
@@ -425,19 +477,23 @@
         :raw-html:`<br />`
 
         -----
 
         :param file_or_folder: The file or folder to import from. Must be relative.
         :return: None
         """
-        if not self.enabled:
+        if not self.config.ENABLED:
             return
 
-        self.__model_imports__.append(
-            partial(self._partial_models_import, file_or_folder=file_or_folder)
+        self._models.add(
+            partial(
+                _partial_models_import,
+                location=self.location,
+                file_or_folder=file_or_folder,
+            )
         )
 
     def tmpl(self, template: str) -> str:
         """
         Pushes the blueprint name to the template name.
         This saves time in having to type out the blueprint name when rendering a
         template file from the blueprint's template folder.
@@ -481,63 +537,7 @@
 
         -----
 
         :param template: The template name to push the blueprint name to.
         :return: str - The template name with the blueprint name pushed to it.
         """
         return f"{self.name}/{template}"
-
-    def _setup_imp_blueprint(self, imp_instance) -> None:
-        """
-        Sets up the ImpBlueprint instance. This is a private method and should not be called directly.
-        """
-        bind_enabled = self.database_bind.get("ENABLED", False)
-
-        app_instance = imp_instance.app
-
-        if bind_enabled:
-            database_uri = _build_database_uri(self.database_bind, app_instance)
-
-            if database_uri:
-                if self.name in app_instance.config.get("SQLALCHEMY_BINDS", {}):
-                    raise ValueError(
-                        f"Blueprint {self.name} already has a database bind set"
-                    )
-
-                app_instance.config["SQLALCHEMY_BINDS"].update(
-                    {self.name: database_uri}
-                )
-
-        for partial_models_import in self.__model_imports__:
-            partial_models_import(imp_instance=imp_instance)
-
-        for partial_nested_blueprint_import in self.__nested_blueprint_imports__:
-            partial_nested_blueprint_import(imp_instance=imp_instance)
-
-    def _partial_models_import(
-        self,
-        file_or_folder: str,
-        imp_instance,
-    ) -> None:
-        file_or_folder_path = Path(self.location / file_or_folder)
-        imp_instance.import_models(file_or_folder_path.as_posix())
-
-    def _partial_nested_blueprint_import(self, blueprint: str, imp_instance) -> None:
-        if Path(blueprint).is_absolute():
-            potential_bp = Path(blueprint)
-        else:
-            potential_bp = Path(self.location / blueprint)
-
-        if potential_bp.exists() and potential_bp.is_dir():
-            module = import_module(
-                cast_to_import_str(self.package.split(".")[0], potential_bp)
-            )
-            for name, value in getmembers(module):
-                if isinstance(value, Blueprint) or isinstance(value, ImpBlueprint):
-                    if hasattr(value, "_setup_imp_blueprint"):
-                        if getattr(value, "enabled", False):
-                            value._setup_imp_blueprint(imp_instance)
-                            self.register_blueprint(value)
-                        else:
-                            logging.debug(f"Blueprint {name} is disabled")
-                    else:
-                        self.register_blueprint(value)
```

### Comparing `flask_imp-3.1.0/flask_imp/imp.py` & `flask_imp-4.0.0/flask_imp/imp.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,50 +1,54 @@
-import logging
 import os
+import typing as t
 from importlib import import_module
 from inspect import getmembers
 from inspect import isclass
 from pathlib import Path
-from typing import Dict, Union, Optional, List
 
 from flask import Blueprint, session
 from flask_sqlalchemy.model import DefaultMeta
 
-from .helpers import _init_app_config
+from .config_imp_template import ImpConfigTemplate as ImpConfig
+from .config_object_parser import load_object
+from .config_toml_parser import load_app_toml
+from .exceptions import NoConfigProvided
 from .protocols import Flask, ImpBlueprint
 from .registeries import ModelRegistry
-from .utilities import cast_to_import_str
+from .utilities import (
+    cast_to_import_str,
+    _toml_suffix,
+    build_database_main,
+    build_database_binds,
+)
 
 
 class Imp:
     app: Flask
     app_name: str
     app_path: Path
     app_folder: Path
     app_resources_imported: bool = False
 
-    __model_registry__: ModelRegistry
+    model_registry: ModelRegistry
 
-    config_path: Path
-    config: Dict
+    config: ImpConfig
 
     def __init__(
         self,
-        app: Optional[Flask] = None,
-        app_config_file: Optional[str] = None,
-        ignore_missing_env_variables: bool = False,
+        app: Flask = None,
+        config: t.Union[str, ImpConfig] = None,
     ) -> None:
         if app is not None:
-            self.init_app(app, app_config_file, ignore_missing_env_variables)
+            self.init_app(app, config)
 
     def init_app(
         self,
         app: Flask,
-        app_config_file: Optional[str] = os.environ.get("IMP_CONFIG"),
-        ignore_missing_env_variables: bool = False,
+        config: t.Union[str, ImpConfig] = os.environ.get("IMP_CONFIG"),
     ) -> None:
         """
         Initializes the flask app to work with flask-imp.
 
         :raw-html:`<br />`
 
         If no `app_config_file` specified, an attempt to read `IMP_CONFIG` from the environment will be made.
@@ -58,54 +62,88 @@
         `default.config.toml` will be created, and used if not found.
 
         :raw-html:`<br />`
 
         -----
 
         :param app: The flask app to initialize.
-        :param app_config_file: The config file to use.
-        :param ignore_missing_env_variables: Will ignore missing environment variables in the config if set to True.
+        :param config: The config to use
         :return: None
         """
 
         if app is None:
             raise ImportError(
                 "No app was passed in, do ba = Imp(flaskapp) or app.initapp(flaskapp)"
             )
         if not isinstance(app, Flask):
             raise TypeError("The app that was passed in is not an instance of Flask")
 
-        if app_config_file is None:
-            app_config_file = "default.config.toml"
-
-        self.app = app
-
-        if "imp" in self.app.extensions:
+        if "imp" in app.extensions:
             raise ImportError("The app has already been initialized with flask-imp.")
 
+        self.app = app
         self.app_name = app.name
         self.app_path = Path(self.app.root_path)
         self.app_folder = self.app_path.parent
-        self.config_path = self.app_path / app_config_file
+        self.app.extensions["imp"] = self
 
-        self.config = _init_app_config(
-            self.config_path, ignore_missing_env_variables, self.app
+        self.model_registry = ModelRegistry()
+
+        if config is None:
+            if Path(self.app_path / "config.py").exists():
+                config = f"{self.app_path.name}.config.Config"
+
+            elif Path(self.app_path / "config.toml").exists():
+                config = "config.toml"
+
+            else:
+                raise NoConfigProvided(
+                    f"No config was provided, and no default config was found in {self.app_path}"
+                )
+
+        if isinstance(config, ImpConfig):
+            self.config = config
+
+        if isinstance(config, str):
+            toml_file = Path(self.app_path / config)
+            if toml_file.suffix.lower() in _toml_suffix and toml_file.exists():
+                self.config = load_app_toml(config, self.app_path)
+            else:
+                self.config = load_object(config)
+
+        self.set_app_config(flask_app=app)
+
+    def set_app_config(self, flask_app: Flask) -> None:
+        flask_app.config.update(
+            **{attr[0]: attr[1] for attr in self.config.FLASK.attrs()}
         )
+        _allowed_types = (str, bool, int, float, dict, list, set)
 
-        self.__model_registry__ = ModelRegistry()
-        self.app.extensions["imp"] = self
+        for attr in self.config.__dir__():
+            if attr not in self.config._attrs and attr not in self.config._known_funcs:
+                _ = getattr(self.config, attr)
+                if (
+                    not attr.startswith("_")
+                    and _ is not None
+                    and type(attr) in _allowed_types
+                    and attr not in flask_app.config
+                ):
+                    flask_app.config[attr] = getattr(self.config, attr)
+
+        build_database_main(flask_app, self.app_path, self.config.DATABASE_MAIN)
+        build_database_binds(flask_app, self.app_path, self.config.DATABASE_BINDS)
 
     def import_app_resources(
         self,
         folder: str = "resources",
-        factories: Optional[List] = None,
+        factories: t.Optional[t.List] = None,
         static_folder: str = "static",
         templates_folder: str = "templates",
-        files_to_import: Optional[List] = None,
-        folders_to_import: Optional[List] = None,
+        files_to_import: t.Optional[t.List] = None,
+        folders_to_import: t.Optional[t.List] = None,
     ) -> None:
         """
         Import standard app resources from the specified folder.
 
         :raw-html:`<br />`
 
         This will import any resources that have been set to the Flask app. Routes, context processors, cli, etc.
@@ -253,28 +291,14 @@
             folders_to_import = ["*"]
 
         if self.app_resources_imported:
             raise ImportError("The app resources can only be imported once.")
 
         self.app_resources_imported = True
 
-        def process_module(import_location: str) -> tuple:
-            def gm(mf):
-                with self.app.app_context():
-                    return getmembers(mf)
-
-            module_file = import_module(import_location)
-            flask_instance = (
-                True
-                if [name for name, value in gm(module_file) if isinstance(value, Flask)]
-                else False
-            )
-
-            return module_file, flask_instance
-
         resources_folder = self.app_path / folder
         app_static_folder = resources_folder / static_folder
         app_templates_folder = resources_folder / templates_folder
 
         if not resources_folder.exists():
             raise ImportError(
                 f"Cannot find resources collection folder at {resources_folder}"
@@ -295,15 +319,15 @@
 
         skip_folders = (
             "static",
             "templates",
         )
 
         for item in resources_folder.iterdir():
-            if "__" in item.name:
+            if item.name.startswith("__"):
                 continue
 
             # iter over files and folders in the resources folder
             if item.is_file() and item.suffix == ".py":
                 # only pull in python files
                 if not import_all_files:
                     # if import_all_files is False, only import the files in the list
@@ -353,18 +377,18 @@
 
         :raw-html:`<br />`
 
         -----
 
         :return: None
         """
-        if self.config.get("SESSION"):
-            for key, value in self.config.get("SESSION", {}).items():
-                if key not in session:
-                    session[key] = value
+        if self.config.INIT_SESSION:
+            session.update(
+                {k: v for k, v in self.config.INIT_SESSION.items() if k not in session}
+            )
 
     def import_blueprint(self, blueprint: str) -> None:
         """
         Import a specified Flask-Imp or standard Flask Blueprint.
 
         :raw-html:`<br />`
 
@@ -470,35 +494,70 @@
         :raw-html:`<br />`
 
         -----
 
         :param blueprint: The blueprint (folder name) to import. Must be relative.
         :return: None
         """
+
+        def process_nested_blueprint_registration(
+            parent: t.Union[Blueprint, ImpBlueprint],
+            child: t.Union[Blueprint, ImpBlueprint],
+        ):
+            if hasattr(child, "config"):
+                if child.config.ENABLED:
+                    parent.register_blueprint(child)
+
+                    if hasattr(child, "_models"):
+                        for partial_model in child._models:
+                            partial_model(imp_instance=self)
+
+                    if hasattr(child, "set_app_config"):
+                        child.set_app_config(self.app, self.app_path)
+
+                else:
+                    print(f"Blueprint {child.name} is disabled")
+
+        def process_blueprint_registration(pbp: t.Union[Blueprint, ImpBlueprint]):
+            if hasattr(pbp, "config"):
+                if pbp.config.ENABLED:
+                    if hasattr(pbp, "_nested_blueprints"):
+                        for nested_bp in pbp._nested_blueprints:
+                            process_nested_blueprint_registration(pbp, nested_bp)
+
+                    if hasattr(pbp, "_models"):
+                        for partial_model in pbp._models:
+                            partial_model(imp_instance=self)
+
+                    if hasattr(pbp, "set_app_config"):
+                        pbp.set_app_config(self.app, self.app_path)
+
+                    self.app.register_blueprint(pbp)
+
+                else:
+                    print(f"Blueprint {potential_bp.name} is disabled")
+            else:
+                self.app.register_blueprint(pbp)
+
         if Path(blueprint).is_absolute():
             potential_bp = Path(blueprint)
         else:
             potential_bp = Path(self.app_path / blueprint)
 
         if potential_bp.exists() and potential_bp.is_dir():
-            try:
-                module = import_module(cast_to_import_str(self.app_name, potential_bp))
-                for name, value in getmembers(module):
-                    if isinstance(value, Blueprint) or isinstance(value, ImpBlueprint):
-                        if hasattr(value, "_setup_imp_blueprint"):
-                            if getattr(value, "enabled", False):
-                                value._setup_imp_blueprint(self)
-                                self.app.register_blueprint(value)
-                            else:
-                                logging.debug(f"Blueprint {name} is disabled")
-                        else:
-                            self.app.register_blueprint(value)
+            # try:
+            module = import_module(cast_to_import_str(self.app_name, potential_bp))
+            for name, potential in getmembers(module):
+                if isinstance(potential, Blueprint) or isinstance(
+                    potential, ImpBlueprint
+                ):
+                    process_blueprint_registration(potential)
 
-            except Exception as e:
-                raise ImportError(f"Error when importing {potential_bp.name}: {e}")
+            # except Exception as e:
+            #     raise ImportError(f"Error when importing {potential_bp.name}: {e}")
 
     def import_blueprints(self, folder: str) -> None:
         """
         Imports all the blueprints in the given folder.
 
         :raw-html:`<br />`
 
@@ -528,16 +587,22 @@
         -----
 
         :param folder: The folder to import from. Must be relative.
         """
 
         folder_path = Path(self.app_path / folder)
 
+        if not folder_path.exists():
+            raise ImportError(f"Cannot find blueprints folder at {folder_path}")
+
+        if not folder_path.is_dir():
+            raise ImportError(f"Blueprints must be a folder {folder_path}")
+
         for potential_bp in folder_path.iterdir():
-            self.import_blueprint(potential_bp.as_posix())
+            self.import_blueprint(f"{potential_bp}")
 
     def import_models(self, file_or_folder: str) -> None:
         """
         Imports all the models from the given file or folder.
 
 
         :raw-html:`<br />`
@@ -623,15 +688,15 @@
             Picks apart the model from_file and builds a registry of the models found.
             """
             import_string = cast_to_import_str(self.app_name, path)
             try:
                 model_module = import_module(import_string)
                 for name, value in getmembers(model_module, isclass):
                     if hasattr(value, "__tablename__"):
-                        self.__model_registry__.add(name, value)
+                        self.model_registry.add(name, value)
 
             except ImportError as e:
                 raise ImportError(f"Error when importing {import_string}: {e}")
 
         if Path(file_or_folder).is_absolute():
             file_or_folder_path = Path(file_or_folder)
         else:
@@ -689,17 +754,17 @@
 
         :raw-html:`<br />`
 
         -----
         :param class_: The class name of the model to return.
         :return: The model class [DefaultMeta].
         """
-        return self.__model_registry__.class_(class_)
+        return self.model_registry.class_(class_)
 
-    def model_meta(self, class_: Union[str, DefaultMeta]) -> dict:
+    def model_meta(self, class_: t.Union[str, DefaultMeta]) -> dict:
         """
         Returns meta information for the given ORM class name
 
         :raw-html:`<br />`
 
         **Example:**
 
@@ -755,15 +820,15 @@
         """
 
         def check_for_table_name(model_):
             if not hasattr(model_, "__tablename__"):
                 raise AttributeError(f"{model_} is not a valid model")
 
         if isinstance(class_, str):
-            model = self.__model_registry__.class_(class_)
+            model = self.model_registry.class_(class_)
             check_for_table_name(model)
             return {
                 "location": model.__module__,
                 "table_name": model.__tablename__,
             }
 
         return {
```

### Comparing `flask_imp-3.1.0/flask_imp/registeries.py` & `flask_imp-4.0.0/flask_imp/registeries.py`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/flask_imp/security/__private_funcs__.py` & `flask_imp-4.0.0/flask_imp/security/__private_funcs__.py`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/flask_imp/security/api_login_check.py` & `flask_imp-4.0.0/flask_imp/security/api_login_check.py`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/flask_imp/security/include_csrf.py` & `flask_imp-4.0.0/flask_imp/security/include_csrf.py`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/flask_imp/security/login_check.py` & `flask_imp-4.0.0/flask_imp/security/login_check.py`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/flask_imp/security/pass_function_check.py` & `flask_imp-4.0.0/flask_imp/security/pass_function_check.py`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/flask_imp/security/permission_check.py` & `flask_imp-4.0.0/flask_imp/security/permission_check.py`

 * *Files identical despite different names*

### Comparing `flask_imp-3.1.0/flask_imp/utilities.py` & `flask_imp-4.0.0/flask_imp/utilities.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,96 +1,93 @@
 import functools
 import logging
-import os
 import re
 import sys
 import typing as t
 from pathlib import Path
 
+from flask_imp.protocols import Flask, DatabaseConfigTemplate, Imp
+
 
 class Sprinkles:
     HEADER = "\033[95m"
     OKBLUE = "\033[94m"
     OKCYAN = "\033[96m"
     OKGREEN = "\033[92m"
     WARNING = "\033[93m"
     FAIL = "\033[91m"
     BOLD = "\033[1m"
     UNDERLINE = "\033[4m"
     END = "\033[0m"
 
 
+_toml_suffix = (".toml", ".tml")
+
+
 def deprecated(message: str):
     def func_wrapper(func):
         @functools.wraps(func)
         def proc_function(*args, **kwargs):
-            logging.critical(
+            logging.warning(
                 f"{Sprinkles.FAIL}Function deprecated: {message}{Sprinkles.END}"
             )
             return func(*args, **kwargs)
 
         return proc_function
 
     return func_wrapper
 
 
-def if_env_replace(
-    env_value: t.Optional[t.Any], ignore_missing_env_variables: bool = False
-) -> t.Any:
-    """
-    Looks for the replacement pattern to swap out values in the config file with environment variables.
-    """
-    pattern = re.compile(r"<(.*?)>")
-
-    if isinstance(env_value, str):
-        if re.match(pattern, env_value):
-            env_var = re.findall(pattern, env_value)[0]
-
-            if env_var:
-                if os.environ.get(env_var):
-                    return parse_config_env_var(os.environ.get(env_var))
-
-                if ignore_missing_env_variables:
-                    return None
-
-                raise ValueError(f"Environment variable {env_value} not found")
-
-    return env_value
-
-
-def process_dict(
-    this_dict: t.Optional[dict],
-    key_case_switch: str = "upper",
-    ignore_missing_env_variables: bool = False,
-    crawl: bool = False,
-) -> dict:
-    """
-    Used to process the config from_file dictionary and replace environment variables. Turns all keys to upper case.
-    """
+def _partial_models_import(
+    location: Path,
+    file_or_folder: str,
+    imp_instance: Imp,
+) -> None:
+    file_or_folder_path = Path(location / file_or_folder)
+    imp_instance.import_models(f"{file_or_folder_path}")
+
+
+def build_database_main(
+    flask_app: Flask, app_path: Path, database_main: DatabaseConfigTemplate
+):
+    if database_main:
+        if database_main.enabled:
+            flask_app.config["SQLALCHEMY_DATABASE_URI"] = build_database_uri(
+                flask_app, app_path, database_main
+            )
 
-    if this_dict is None:
-        return {}
 
-    return_dict = {}
-    for key, value in this_dict.items():
-        if key_case_switch == "ignore":
-            cs_key = key
-        else:
-            cs_key = key.upper() if key_case_switch == "upper" else key.lower()
+def build_database_binds(
+    flask_app: Flask, app_path: Path, database_binds: t.Set[DatabaseConfigTemplate]
+):
+    if database_binds:
+        for db in database_binds:
+            if db.enabled:
+                if "SQLALCHEMY_BINDS" not in flask_app.config:
+                    flask_app.config["SQLALCHEMY_BINDS"] = {}
 
-        if crawl:
-            if isinstance(value, dict):
-                return_dict[cs_key] = process_dict(
-                    value, key_case_switch, ignore_missing_env_variables, crawl
+                flask_app.config["SQLALCHEMY_BINDS"][db.bind_key] = build_database_uri(
+                    flask_app, app_path, db
                 )
-                continue
 
-        return_dict[cs_key] = if_env_replace(value, ignore_missing_env_variables)
 
-    return return_dict
+def build_database_uri(flask_app: Flask, app_path: Path, db: DatabaseConfigTemplate):
+    if db.dialect == "sqlite":
+        filepath = (
+            app_path
+            / "instance"
+            / (db.name + flask_app.config.get("SQLITE_DB_EXTENSION", ".sqlite"))
+        )
+        return f"{db.dialect}:///{filepath}"
+
+    return (
+        f"{db.dialect}://{db.username}:"
+        f"{db.password}@{db.location}:"
+        f"{db.port}/{db.name}"
+    )
 
 
 def cast_to_import_str(app_name: str, folder_path: Path) -> str:
     """
     Takes the folder path and converts it to a string that can be imported
     """
     folder_parts = folder_path.parts
@@ -106,14 +103,23 @@
     """
     Switches name of the class CamelCase to snake_case
     """
     s1 = re.sub("(.)([A-Z][a-z]+)", r"\1_\2", value)
     return re.sub("([a-z0-9])([A-Z])", r"\1_\2", s1).lower()
 
 
+def slug(value: str) -> str:
+    """
+    Switches name of the class CamelCase to slug-case
+    """
+    value = value.replace("_", "-")
+    s1 = re.sub("(.)([A-Z][a-z]+)", r"\1-\2", value)
+    return re.sub("([a-z0-9])([A-Z])", r"\1-\2", s1).lower()
+
+
 def class_field(class_: str, field: str) -> str:
     """
     Switches name of the class CamelCase to snake_case and tacks on the field name
 
     Used for SQLAlchemy foreign key assignments
 
     INFO ::: This function may not produce the correct information if you are using __tablename__ in your class
@@ -139,29 +145,67 @@
             return False
         else:
             raise TypeError(f"Cannot cast {value} to bool")
     else:
         raise TypeError(f"Cannot cast {value} to bool")
 
 
-def parse_config_env_var(value: t.Optional[str]) -> t.Optional[t.Union[bool, str, int]]:
+def cast_to_int(value: t.Union[str, int, float, bool, None]) -> int:
     """
-    Casts value to a boolean, string, or int if possible. If not, returns none.
+    Casts string, float, and bool to int
     """
-    if value == "None":
-        return None
+
+    if value is None:
+        return 0
+
+    if isinstance(value, int):
+        return value
 
     if isinstance(value, str):
-        true_str = ("true", "yes", "y", "1")
-        false_str = ("false", "no", "n", "0")
+        if value == "":
+            return 0
 
-        if value.lower() in true_str:
-            return True
-        elif value.lower() in false_str:
-            return False
-        else:
-            try:
-                return int(value)
-            except ValueError:
-                return value
+        try:
+            return int(value)
+        except ValueError:
+            raise TypeError(f"Cannot cast {value} to int")
+
+    if isinstance(value, float):
+        return int(value)
+
+    if isinstance(value, bool):
+        if value:
+            return 1
+        return 0
+
+    raise TypeError(f"Cannot cast {value} to int")
+
+
+def cast_to_float(value: t.Union[str, int, float, bool, None]) -> float:
+    """
+    Casts string, int, and bool to float
+    """
+
+    if value is None:
+        return 0.0
+
+    if isinstance(value, float):
+        return value
+
+    if isinstance(value, str):
+        if value == "":
+            return 0.0
+
+        try:
+            return float(value)
+        except ValueError:
+            raise TypeError(f"Cannot cast {value} to float")
+
+    if isinstance(value, int):
+        return float(value)
+
+    if isinstance(value, bool):
+        if value:
+            return 1.0
+        return 0.0
 
-    return None
+    raise TypeError(f"Cannot cast {value} to float")
```

### Comparing `flask_imp-3.1.0/pyproject.toml` & `flask_imp-4.0.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 description = 'A Flask auto importer that allows your Flask apps to grow big.'
 authors = [{ name = "David Carmichael", email = "david@uilix.com" }]
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Environment :: Web Environment', 'Intended Audience :: Developers',
-    'License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)',
+    'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent', 'Programming Language :: Python',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Programming Language :: Python :: 3.12',
     'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
@@ -37,24 +37,33 @@
 
 [project.urls]
 Documentation = "https://cheesecake87.github.io/flask-imp/"
 Source = "https://github.com/CheeseCake87/flask-imp"
 
 [tool.flit.sdist]
 exclude = [
+    "venv/",
+    ".venv/",
     ".github/",
     "_assets/",
     "app/",
     "dist/",
     "docs/",
-    "docs_gen/",
+    "gdocs/",
     "test_app/",
     "test_docker/",
     "tests/",
     ".env",
     ".gitignore",
     "docker-compose.yaml",
     "Dockerfile",
     "requirements_build.txt",
     "requirements_dev.txt",
     "requirements_docs.txt",
-]
+]
+
+[tool.pyqwe]
+install = "*:flit install --symlink"
+build = "*:flit build"
+publish = "*shell:export=FLIT_USERNAME=__token__ && flit publish"
+docs = "*:flask --app gdocs compile"
+docs-watch = "*:flask --app gdocs compile --watch"
```

### Comparing `flask_imp-3.1.0/PKG-INFO` & `flask_imp-4.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: flask-imp
-Version: 3.1.0
+Version: 4.0.0
 Summary: A Flask auto importer that allows your Flask apps to grow big.
 Author-email: David Carmichael <david@uilix.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -41,18 +41,14 @@
 Flask-Imp's main purpose is to help simplify the importing of blueprints, resources, and models.
 It has a few extra features built in to help with securing pages and password authentication.
 
 ## Documentation
 
 [https://cheesecake87.github.io/flask-imp/](https://cheesecake87.github.io/flask-imp/)
 
-### Notable Breaking Changes
-
-[2.x.x to 3.0.0](https://github.com/CheeseCake87/flask-imp/releases/tag/3.0.0)
-
 ## Getting Started
 
 ### Setup.
 
 Create a new project folder and navigate to it.
 
 ```text
```

