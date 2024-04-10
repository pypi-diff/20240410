# Comparing `tmp/modelw_project_maker-2023.7.1.tar.gz` & `tmp/modelw_project_maker-2024.4.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelw_project_maker-2023.7.1.tar", max compression
+gzip compressed data, was "modelw_project_maker-2024.4.0b1.tar", max compression
```

## Comparing `modelw_project_maker-2023.7.1.tar` & `modelw_project_maker-2024.4.0b1.tar`

### file list

```diff
@@ -1,85 +1,109 @@
--rw-r--r--   0        0        0     5377 2023-07-13 09:24:13.206219 modelw_project_maker-2023.7.1/README.md
--rw-r--r--   0        0        0     1355 2023-07-13 09:24:13.206219 modelw_project_maker-2023.7.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-13 09:24:13.206219 modelw_project_maker-2023.7.1/src/model_w/project_maker/__init__.py
--rw-r--r--   0        0        0     8748 2023-07-13 09:24:13.206219 modelw_project_maker-2023.7.1/src/model_w/project_maker/__main__.py
--rw-r--r--   0        0        0       45 2023-07-13 09:24:13.206219 modelw_project_maker-2023.7.1/src/model_w/project_maker/errors.py
--rw-r--r--   0        0        0      143 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/maker/__init__.py
--rw-r--r--   0        0        0     4470 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/maker/_api.py
--rw-r--r--   0        0        0     6518 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/maker/_base.py
--rw-r--r--   0        0        0      703 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/maker/_common.py
--rw-r--r--   0        0        0     3836 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/maker/_front.py
--rw-r--r--   0        0        0     3446 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/namer.py
--rw-r--r--   0        0        0        0 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/py.typed
--rw-r--r--   0        0        0      178 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/.editorconfig
--rw-r--r--   0        0        0       27 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/.formatignore
--rw-r--r--   0        0        0     3042 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/.gitignore
--rw-r--r--   0        0        0       77 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/.prettierrc
--rw-r--r--   0        0        0     1488 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/README.md
--rw-r--r--   0        0        0     3034 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/.dockerignore
--rw-r--r--   0        0        0      381 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/.env-template
--rw-r--r--   0        0        0      181 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/Dockerfile
--rw-r--r--   0        0        0      236 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/Makefile
--rw-r--r--   0        0        0     1140 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/README.md
--rw-r--r--   0        0        0        0 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/__init__.py
--rw-r--r--   0        0        0       93 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/README.md
--rw-r--r--   0        0        0        0 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/__init__.py
--rw-r--r--   0        0        0     8589 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0001_initial.py
--rw-r--r--   0        0        0     2818 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0002_homepage.py
--rw-r--r--   0        0        0        0 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/__init__.py
--rw-r--r--   0        0        0     2036 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/models.py
--rw-r--r--   0        0        0      655 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/base.html
--rw-r--r--   0        0        0      233 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/cms/home_page.html
--rwxr-xr-x   0        0        0      755 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/cross.svg
--rwxr-xr-x   0        0        0      240 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/edit.svg
--rwxr-xr-x   0        0        0      471 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder-inverse.svg
--rwxr-xr-x   0        0        0      844 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder-open-inverse.svg
--rwxr-xr-x   0        0        0      903 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder.svg
--rwxr-xr-x   0        0        0     1092 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/plus-inverse.svg
--rwxr-xr-x   0        0        0      658 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/plus.svg
--rwxr-xr-x   0        0        0      718 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/tick-inverse.svg
--rwxr-xr-x   0        0        0      485 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/tick.svg
--rwxr-xr-x   0        0        0     2749 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/wagtail-inverse.svg
--rwxr-xr-x   0        0        0     2067 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/wagtail.svg
--rw-r--r--   0        0        0     1883 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/templates/base.html
--rw-r--r--   0        0        0      159 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/README.md
--rw-r--r--   0        0        0        0 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/__init__.py
--rw-r--r--   0        0        0     3921 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/migrations/__init__.py
--rw-r--r--   0        0        0     3150 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/models.py
--rw-r--r--   0        0        0     1343 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/serializers.py
--rw-r--r--   0        0        0     2486 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/views.py
--rw-r--r--   0        0        0      194 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/README.md
--rw-r--r--   0        0        0        0 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/__init__.py
--rw-r--r--   0        0        0      386 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/consumers.py
--rw-r--r--   0        0        0        0 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/migrations/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/models.py
--rw-r--r--   0        0        0       70 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/django/__init__.py
--rw-r--r--   0        0        0      851 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/django/asgi.py
--rw-r--r--   0        0        0      273 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/django/celery.py
--rw-r--r--   0        0        0      219 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/django/routing.py
--rw-r--r--   0        0        0     2076 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/django/settings.py
--rw-r--r--   0        0        0     1681 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/django/urls.py
--rw-r--r--   0        0        0      443 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/django/wsgi.py
--rwxr-xr-x   0        0        0      666 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/manage.py
--rwxr-xr-x   0        0        0      151 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/pmanage
--rw-r--r--   0        0        0      861 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/pyproject.toml
--rw-r--r--   0        0        0     3034 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/.dockerignore
--rw-r--r--   0        0        0      182 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/.env-template
--rw-r--r--   0        0        0      332 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/.eslintrc.js
--rw-r--r--   0        0        0        8 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/.gitignore
--rw-r--r--   0        0        0       13 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/.nvmrc
--rw-r--r--   0        0        0      185 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/Dockerfile
--rw-r--r--   0        0        0     1601 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/README.md
--rw-r--r--   0        0        0      112 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/components/blocks/title-1.vue
--rw-r--r--   0        0        0    11513 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/components/server-templated-component.vue
--rw-r--r--   0        0        0     2941 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/error.vue
--rw-r--r--   0        0        0      558 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/nuxt.config.js
--rw-r--r--   0        0        0      789 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/package.json
--rw-r--r--   0        0        0     5048 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/pages/[...wagtail].vue
--rw-r--r--   0        0        0       80 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/pages/no-wagtail-index.vue
--rw-r--r--   0        0        0      483 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/plugins/dom.client.ts
--rw-r--r--   0        0        0      505 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/plugins/dom.server.ts
--rw-r--r--   0        0        0       98 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/tsconfig.json
--rw-r--r--   0        0        0     7602 2023-07-13 09:24:13.210219 modelw_project_maker-2023.7.1/src/model_w/project_maker/template.py
--rw-r--r--   0        0        0     6592 1970-01-01 00:00:00.000000 modelw_project_maker-2023.7.1/PKG-INFO
+-rw-r--r--   0        0        0     5377 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/README.md
+-rw-r--r--   0        0        0     1357 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/__init__.py
+-rw-r--r--   0        0        0     8748 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/__main__.py
+-rw-r--r--   0        0        0       45 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/errors.py
+-rw-r--r--   0        0        0      143 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/maker/__init__.py
+-rw-r--r--   0        0        0     4470 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/maker/_api.py
+-rw-r--r--   0        0        0     6518 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/maker/_base.py
+-rw-r--r--   0        0        0      703 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/maker/_common.py
+-rw-r--r--   0        0        0     3836 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/maker/_front.py
+-rw-r--r--   0        0        0     3446 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/namer.py
+-rw-r--r--   0        0        0        0 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/py.typed
+-rw-r--r--   0        0        0      178 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/.editorconfig
+-rw-r--r--   0        0        0       27 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/.formatignore
+-rw-r--r--   0        0        0     3042 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/.gitignore
+-rw-r--r--   0        0        0       77 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/.prettierrc
+-rw-r--r--   0        0        0     1488 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/README.md
+-rw-r--r--   0        0        0     3034 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/.dockerignore
+-rw-r--r--   0        0        0      373 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/.env-template
+-rw-r--r--   0        0        0      181 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/Dockerfile
+-rw-r--r--   0        0        0      236 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/Makefile
+-rw-r--r--   0        0        0     1140 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/README.md
+-rw-r--r--   0        0        0        0 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/__init__.py
+-rw-r--r--   0        0        0       93 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/README.md
+-rw-r--r--   0        0        0        0 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/__init__.py
+-rw-r--r--   0        0        0     8633 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2818 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0002_homepage.py
+-rw-r--r--   0        0        0        0 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/__init__.py
+-rw-r--r--   0        0        0     2031 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/models.py
+-rw-r--r--   0        0        0      655 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/base.html
+-rw-r--r--   0        0        0      233 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/cms/home_page.html
+-rwxr-xr-x   0        0        0      755 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/cross.svg
+-rwxr-xr-x   0        0        0      240 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/edit.svg
+-rwxr-xr-x   0        0        0      471 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder-inverse.svg
+-rwxr-xr-x   0        0        0      844 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder-open-inverse.svg
+-rwxr-xr-x   0        0        0      903 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder.svg
+-rwxr-xr-x   0        0        0     1092 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/plus-inverse.svg
+-rwxr-xr-x   0        0        0      658 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/plus.svg
+-rwxr-xr-x   0        0        0      718 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/tick-inverse.svg
+-rwxr-xr-x   0        0        0      485 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/tick.svg
+-rwxr-xr-x   0        0        0     2749 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/wagtail-inverse.svg
+-rwxr-xr-x   0        0        0     2067 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/wagtail.svg
+-rw-r--r--   0        0        0     1883 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/templates/base.html
+-rw-r--r--   0        0        0      159 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/README.md
+-rw-r--r--   0        0        0        0 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/__init__.py
+-rw-r--r--   0        0        0     3921 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/migrations/__init__.py
+-rw-r--r--   0        0        0     3150 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/models.py
+-rw-r--r--   0        0        0     1343 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/serializers.py
+-rw-r--r--   0        0        0     2486 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/views.py
+-rw-r--r--   0        0        0      194 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/README.md
+-rw-r--r--   0        0        0        0 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/__init__.py
+-rw-r--r--   0        0        0      386 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/consumers.py
+-rw-r--r--   0        0        0        0 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/models.py
+-rw-r--r--   0        0        0       70 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/__init__.py
+-rw-r--r--   0        0        0      851 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/asgi.py
+-rw-r--r--   0        0        0      273 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/celery.py
+-rw-r--r--   0        0        0      220 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/routing.py
+-rw-r--r--   0        0        0     2076 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/settings.py
+-rw-r--r--   0        0        0     1682 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/urls.py
+-rw-r--r--   0        0        0      443 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/wsgi.py
+-rw-r--r--   0        0        0       89 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/.gitignore
+-rw-r--r--   0        0        0     7233 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/README.md
+-rw-r--r--   0        0        0        0 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/__init__.py
+-rw-r--r--   0        0        0      400 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/conftest.py
+-rw-r--r--   0        0        0      451 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/features/README.md
+-rw-r--r--   0        0        0     3001 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/features/smoke-test.feature
+-rw-r--r--   0        0        0      224 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/fixtures/README.md
+-rw-r--r--   0        0        0      126 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/fixtures/__init__.py
+-rw-r--r--   0        0        0      748 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/fixtures/data.py
+-rw-r--r--   0        0        0     5289 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/fixtures/front.py
+-rw-r--r--   0        0        0     1033 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/fixtures/reporting.py
+-rw-r--r--   0        0        0     1885 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/fixtures/utils.py
+-rw-r--r--   0        0        0     5334 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/hooks.py
+-rw-r--r--   0        0        0    16126 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/report/reporter.py
+-rw-r--r--   0        0        0     2242 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/report/utils.py
+-rw-r--r--   0        0        0      142 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/step_definitions/__init__.py
+-rw-r--r--   0        0        0     3458 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/step_definitions/common_given.py
+-rw-r--r--   0        0        0     4797 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/step_definitions/common_then.py
+-rw-r--r--   0        0        0     3484 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/step_definitions/common_when.py
+-rw-r--r--   0        0        0     3537 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/step_definitions/utils.py
+-rw-r--r--   0        0        0      680 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/test_features.py
+-rw-r--r--   0        0        0    11758 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/test_utils.py
+-rwxr-xr-x   0        0        0      666 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/manage.py
+-rwxr-xr-x   0        0        0      151 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/pmanage
+-rw-r--r--   0        0        0     1473 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/pyproject.toml
+-rw-r--r--   0        0        0     3034 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/.dockerignore
+-rw-r--r--   0        0        0      174 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/.env-template
+-rw-r--r--   0        0        0      332 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/.eslintrc.js
+-rw-r--r--   0        0        0        8 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/.gitignore
+-rw-r--r--   0        0        0       13 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/.nvmrc
+-rw-r--r--   0        0        0      185 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/Dockerfile
+-rw-r--r--   0        0        0     1601 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/README.md
+-rw-r--r--   0        0        0      112 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/components/blocks/title-1.vue
+-rw-r--r--   0        0        0    11513 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/components/server-templated-component.vue
+-rw-r--r--   0        0        0     2941 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/error.vue
+-rw-r--r--   0        0        0     6320 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/middleware/wagtail.ts
+-rw-r--r--   0        0        0      738 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/nuxt.config.js
+-rw-r--r--   0        0        0      869 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/package.json
+-rw-r--r--   0        0        0      655 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/pages/[...wagtail].vue
+-rw-r--r--   0        0        0       80 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/pages/no-wagtail-index.vue
+-rw-r--r--   0        0        0      483 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/plugins/dom.client.ts
+-rw-r--r--   0        0        0      505 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/plugins/dom.server.ts
+-rw-r--r--   0        0        0      439 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/stores/layout.js
+-rw-r--r--   0        0        0       98 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/tsconfig.json
+-rw-r--r--   0        0        0     7602 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template.py
+-rw-r--r--   0        0        0     6645 1970-01-01 00:00:00.000000 modelw_project_maker-2024.4.0b1/PKG-INFO
```

### Comparing `modelw_project_maker-2023.7.1/README.md` & `modelw_project_maker-2024.4.0b1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 This will ask you a few questions and create the project's directory for you.
 
 ## Prerequisites
 
 In order to execute the script, you need:
 
--   Python 3.10 (you can use pyenv to load it in your current shell)
+-   Python 3.11 (you can use pyenv to load it in your current shell)
 -   Poetry (follow the instructions on
     [their website](https://python-poetry.org/docs/#installation))
 -   Git (you know where to get it)
 -   Git Flow (`apt install git-flow` or `brew install git-flow` depending on
     your OS)
 -   Node and NPM (get it your favorite way)
 -   PostgreSQL and Redis (if you enable the API side)
```

### Comparing `modelw_project_maker-2023.7.1/pyproject.toml` & `modelw_project_maker-2024.4.0b1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "modelw-project-maker"
-version = "2023.7.1"
+version = "2024.4.0b1"
 packages = [
     {  include = "model_w/project_maker", from = "src" }
 ]
 
 description = "A tool to create Model-W-compliant projects"
 authors = ["Rémy Sanchez <remy.sanchez@hyperthese.net>"]
 license = "WTFPL"
```

### Comparing `modelw_project_maker-2023.7.1/src/model_w/project_maker/__main__.py` & `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/__main__.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.1/src/model_w/project_maker/maker/_api.py` & `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/maker/_api.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.1/src/model_w/project_maker/maker/_base.py` & `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/maker/_base.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.1/src/model_w/project_maker/maker/_common.py` & `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/maker/_common.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.1/src/model_w/project_maker/maker/_front.py` & `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/maker/_front.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.1/src/model_w/project_maker/namer.py` & `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/namer.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/.gitignore` & `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/.gitignore`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/README.md` & `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/README.md`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/.dockerignore` & `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/.dockerignore`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/README.md` & `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/README.md`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0001_initial.py` & `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0001_initial.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
                         serialize=False,
                         verbose_name="ID",
                     ),
                 ),
                 ("title", models.CharField(max_length=255, verbose_name="title")),
                 (
                     "file",
-                    models.ImageField(
+                    wagtail.images.models.WagtailImageField(
                         height_field="height",
                         upload_to=wagtail.images.models.get_upload_to,
                         verbose_name="file",
                         width_field="width",
                     ),
                 ),
                 ("width", models.IntegerField(editable=False, verbose_name="width")),
@@ -194,15 +194,15 @@
                         serialize=False,
                         verbose_name="ID",
                     ),
                 ),
                 ("filter_spec", models.CharField(db_index=True, max_length=255)),
                 (
                     "file",
-                    models.ImageField(
+                    wagtail.images.models.WagtailImageField(
                         height_field="height",
                         upload_to=wagtail.images.models.get_rendition_upload_to,
                         width_field="width",
                     ),
                 ),
                 ("width", models.IntegerField(editable=False)),
                 ("height", models.IntegerField(editable=False)),
```

### Comparing `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0002_homepage.py` & `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0002_homepage.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/models.py` & `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from django.db import models
 from django.utils.translation import gettext_lazy as _
-from wagtail.core.models import Page
 from wagtail.documents.models import AbstractDocument
 from wagtail.images.models import AbstractImage, AbstractRendition
 from wagtail.images.models import Image as DefaultImage
+from wagtail.models import Page
 
 
 class CustomImage(AbstractImage):
     """
     Extends the default Wagtail image object to add an "alt" field which is
     often required for SEO purposes.
     """
```

### Comparing `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/base.html` & `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/base.html`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/cross.svg` & `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/cross.svg`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder-open-inverse.svg` & `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder-open-inverse.svg`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder.svg` & `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder.svg`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/plus-inverse.svg` & `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/plus-inverse.svg`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/plus.svg` & `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/plus.svg`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/tick-inverse.svg` & `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/tick-inverse.svg`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/wagtail-inverse.svg` & `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/wagtail-inverse.svg`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/wagtail.svg` & `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/wagtail.svg`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/templates/base.html` & `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/templates/base.html`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/migrations/0001_initial.py` & `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/models.py` & `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/models.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/serializers.py` & `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/serializers.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/views.py` & `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/views.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/django/asgi.py` & `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/asgi.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/django/settings.py` & `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/settings.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/___project_name__snake___/django/urls.py` & `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/urls.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-from ___project_name__snake___.apps.people.views import MeViewSet
 from django.conf import settings
 from django.contrib import admin
 from django.urls import include, path
 from django.utils.translation import gettext_lazy as _
 from rest_framework.routers import DefaultRouter, SimpleRouter
 
 # :: IF api__wagtail
 from wagtail import urls as wagtail_urls
 from wagtail.admin import urls as wagtailadmin_urls
 from wagtail.documents import urls as wagtaildocs_urls
 
 # :: ENDIF
 
+from ___project_name__snake___.apps.people.views import MeViewSet
+
 
 admin.site.site_title = _("___project_name__natural_double_quoted___")
 admin.site.site_header = _("___project_name__natural_double_quoted___")
 
 
 if settings.DEBUG:
     router = DefaultRouter()
```

### Comparing `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/api/manage.py` & `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/manage.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/.dockerignore` & `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/.dockerignore`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/README.md` & `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/README.md`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/components/server-templated-component.vue` & `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/components/server-templated-component.vue`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/error.vue` & `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/error.vue`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.1/src/model_w/project_maker/template/front/nuxt.config.js` & `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/nuxt.config.js`

 * *Files 21% similar despite different names*

#### js-beautify {}

```diff
@@ -1,22 +1,31 @@
 import {
     envManager,
     defineModelWConfig
 } from "@model-w/preset-nuxt3";
+import {
+    defu
+} from "defu";
 
 export default envManager((env) => {
-    return defineModelWConfig(env, {
+    const modelWConfig = defineModelWConfig(env, {
         siteName: "___project_name__snake___",
         head: {
             meta: [{
                 charset: "utf-8"
             }, {
                 name: "viewport",
                 content: "width=device-width, initial-scale=1",
             }, {
                 name: "format-detection",
                 content: "telephone=no"
             }, ],
         },
         cmsAlias: "___cms_prefix___",
     });
+
+    const viteNuxtConfig = defineNuxtConfig({
+        modules: ["@pinia/nuxt"],
+    });
+
+    return defu(modelWConfig, viteNuxtConfig);
 });
```

### Comparing `modelw_project_maker-2023.7.1/src/model_w/project_maker/template.py` & `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.7.1/PKG-INFO` & `modelw_project_maker-2024.4.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: modelw-project-maker
-Version: 2023.7.1
+Version: 2024.4.0b1
 Summary: A tool to create Model-W-compliant projects
 Home-page: https://github.com/ModelW/project-maker
 License: WTFPL
 Keywords: model-w,django,nuxt,boilerplate,template
 Author: Rémy Sanchez
 Author-email: remy.sanchez@hyperthese.net
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Utilities
 Requires-Dist: Unidecode (>=1.3.4,<2.0.0)
 Requires-Dist: black (>=22,<23)
 Requires-Dist: isort (>=5.10.1,<6.0.0)
 Requires-Dist: monoformat (>=0.1.0b3,<0.2.0)
 Requires-Dist: node-edge (>=0.1.0b2,<0.2.0)
@@ -42,15 +43,15 @@
 
 This will ask you a few questions and create the project's directory for you.
 
 ## Prerequisites
 
 In order to execute the script, you need:
 
--   Python 3.10 (you can use pyenv to load it in your current shell)
+-   Python 3.11 (you can use pyenv to load it in your current shell)
 -   Poetry (follow the instructions on
     [their website](https://python-poetry.org/docs/#installation))
 -   Git (you know where to get it)
 -   Git Flow (`apt install git-flow` or `brew install git-flow` depending on
     your OS)
 -   Node and NPM (get it your favorite way)
 -   PostgreSQL and Redis (if you enable the API side)
```

