# Comparing `tmp/django-ckeditors-0.0.4.tar.gz` & `tmp/django-ckeditors-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ckeditors-0.0.4.tar", last modified: Wed Apr 10 21:16:53 2024, max compression
+gzip compressed data, was "django-ckeditors-0.0.5.tar", last modified: Wed Apr 10 21:49:44 2024, max compression
```

## Comparing `django-ckeditors-0.0.4.tar` & `django-ckeditors-0.0.5.tar`

### file list

```diff
@@ -1,182 +1,181 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-10 21:16:53.828584 django-ckeditors-0.0.4/
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-10 21:16:53.776580 django-ckeditors-0.0.4/.github/
--rw-rw-r--   0 mark      (1000) mark      (1000)      821 2024-04-08 05:11:52.000000 django-ckeditors-0.0.4/.github/FUNDING.yml
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-10 21:16:53.776580 django-ckeditors-0.0.4/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 mark      (1000) mark      (1000)      841 2024-04-09 02:00:32.000000 django-ckeditors-0.0.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 mark      (1000) mark      (1000)      111 2024-04-09 02:00:32.000000 django-ckeditors-0.0.4/.github/ISSUE_TEMPLATE/chore.md
--rw-rw-r--   0 mark      (1000) mark      (1000)      395 2024-04-09 02:00:32.000000 django-ckeditors-0.0.4/.github/ISSUE_TEMPLATE/documentation.md
--rw-rw-r--   0 mark      (1000) mark      (1000)      611 2024-04-09 02:00:32.000000 django-ckeditors-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-10 21:16:53.776580 django-ckeditors-0.0.4/.github/archive/
--rw-rw-r--   0 mark      (1000) mark      (1000)      858 2024-04-10 21:05:50.000000 django-ckeditors-0.0.4/.github/archive/release.yml
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-10 21:16:53.776580 django-ckeditors-0.0.4/.github/workflows/
--rw-rw-r--   0 mark      (1000) mark      (1000)     1271 2024-04-09 01:16:47.000000 django-ckeditors-0.0.4/.github/workflows/lint_python.yml
--rw-rw-r--   0 mark      (1000) mark      (1000)      891 2024-04-09 21:51:07.000000 django-ckeditors-0.0.4/.github/workflows/testpypi.yml
--rw-rw-r--   0 mark      (1000) mark      (1000)      638 2024-04-09 07:24:03.000000 django-ckeditors-0.0.4/.gitignore
--rw-rw-r--   0 mark      (1000) mark      (1000)      260 2024-04-09 03:51:27.000000 django-ckeditors-0.0.4/.readthedocs.yaml
--rw-rw-r--   0 mark      (1000) mark      (1000)     1601 2024-04-08 22:59:05.000000 django-ckeditors-0.0.4/LICENSE
--rw-rw-r--   0 mark      (1000) mark      (1000)      218 2024-04-08 08:42:00.000000 django-ckeditors-0.0.4/MANIFEST.in
--rw-r--r--   0 mark      (1000) mark      (1000)     5123 2024-04-10 21:16:53.824583 django-ckeditors-0.0.4/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)     3068 2024-04-09 08:27:23.000000 django-ckeditors-0.0.4/README.rst
--rw-rw-r--   0 mark      (1000) mark      (1000)    20263 2024-04-09 01:17:04.000000 django-ckeditors-0.0.4/commit_history_prior_to_vendoring.txt
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-10 21:16:53.780580 django-ckeditors-0.0.4/django_ckeditors/
--rw-rw-r--   0 mark      (1000) mark      (1000)       36 2024-04-08 05:11:52.000000 django-ckeditors-0.0.4/django_ckeditors/.jshintrc
--rw-rw-r--   0 mark      (1000) mark      (1000)       62 2024-04-08 06:07:51.000000 django-ckeditors-0.0.4/django_ckeditors/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      589 2024-04-08 06:18:14.000000 django-ckeditors-0.0.4/django_ckeditors/fields.py
--rw-rw-r--   0 mark      (1000) mark      (1000)       92 2024-04-08 08:47:06.000000 django-ckeditors-0.0.4/django_ckeditors/forms.py
--rw-rw-r--   0 mark      (1000) mark      (1000)   228033 2024-04-08 07:56:49.000000 django-ckeditors-0.0.4/django_ckeditors/package-lock.json
--rw-rw-r--   0 mark      (1000) mark      (1000)     2317 2024-04-08 07:56:49.000000 django-ckeditors-0.0.4/django_ckeditors/package.json
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-10 21:16:53.772580 django-ckeditors-0.0.4/django_ckeditors/static/
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-10 21:16:53.780580 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/
--rw-rw-r--   0 mark      (1000) mark      (1000)     4767 2024-04-08 06:07:32.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/app.js
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-10 21:16:53.796581 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/
--rw-rw-r--   0 mark      (1000) mark      (1000)  1057374 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/bundle.js
--rw-rw-r--   0 mark      (1000) mark      (1000)      643 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/bundle.js.LICENSE.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)  6303895 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/bundle.js.map
--rw-rw-r--   0 mark      (1000) mark      (1000)   147780 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/styles.css
--rw-rw-r--   0 mark      (1000) mark      (1000)   272908 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/styles.css.map
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-10 21:16:53.816583 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/
--rw-rw-r--   0 mark      (1000) mark      (1000)      891 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/af.js
--rw-rw-r--   0 mark      (1000) mark      (1000)    12237 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/ar.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     2661 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/ast.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     7049 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/az.js
--rw-rw-r--   0 mark      (1000) mark      (1000)    14250 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/bg.js
--rw-rw-r--   0 mark      (1000) mark      (1000)    16177 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/bn.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     2571 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/bs.js
--rw-rw-r--   0 mark      (1000) mark      (1000)    10293 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/ca.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     9901 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/cs.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     9415 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/da.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     7873 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/de-ch.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     9919 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/de.js
--rw-rw-r--   0 mark      (1000) mark      (1000)    14983 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/el.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     8627 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/en-au.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     6085 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/en-gb.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     2914 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/eo.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     1044 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/es-co.js
--rw-rw-r--   0 mark      (1000) mark      (1000)    10073 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/es.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     9437 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/et.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     3088 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/eu.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     8590 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/fa.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     9630 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/fi.js
--rw-rw-r--   0 mark      (1000) mark      (1000)    10373 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/fr.js
--rw-rw-r--   0 mark      (1000) mark      (1000)    10061 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/gl.js
--rw-rw-r--   0 mark      (1000) mark      (1000)      630 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/gu.js
--rw-rw-r--   0 mark      (1000) mark      (1000)    11489 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/he.js
--rw-rw-r--   0 mark      (1000) mark      (1000)    10448 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/hi.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     9131 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/hr.js
--rw-rw-r--   0 mark      (1000) mark      (1000)    10164 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/hu.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     2261 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/hy.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     9132 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/id.js
--rw-rw-r--   0 mark      (1000) mark      (1000)    10495 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/it.js
--rw-rw-r--   0 mark      (1000) mark      (1000)    10999 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/ja.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     3199 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/jv.js
--rw-rw-r--   0 mark      (1000) mark      (1000)      466 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/kk.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     4116 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/km.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     3534 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/kn.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     9800 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/ko.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     8457 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/ku.js
--rw-rw-r--   0 mark      (1000) mark      (1000)    10500 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/lt.js
--rw-rw-r--   0 mark      (1000) mark      (1000)    10026 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/lv.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     9281 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/ms.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     5383 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/nb.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     9566 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/ne.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     9699 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/nl.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     9317 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/no.js
--rw-rw-r--   0 mark      (1000) mark      (1000)      427 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/oc.js
--rw-rw-r--   0 mark      (1000) mark      (1000)    10275 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/pl.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     9867 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/pt-br.js
--rw-rw-r--   0 mark      (1000) mark      (1000)    10083 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/pt.js
--rw-rw-r--   0 mark      (1000) mark      (1000)    10012 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/ro.js
--rw-rw-r--   0 mark      (1000) mark      (1000)    14547 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/ru.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     2179 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/si.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     9918 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/sk.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     3737 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/sl.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     7367 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/sq.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     9671 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/sr-latn.js
--rw-rw-r--   0 mark      (1000) mark      (1000)    12923 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/sr.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     9260 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/sv.js
--rw-rw-r--   0 mark      (1000) mark      (1000)    16031 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/th.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     7970 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/tk.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     9811 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/tr.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     4028 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/tt.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     8318 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/ug.js
--rw-rw-r--   0 mark      (1000) mark      (1000)    14073 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/uk.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     8544 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/ur.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     8553 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/uz.js
--rw-rw-r--   0 mark      (1000) mark      (1000)    10741 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/vi.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     8988 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/zh-cn.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     8590 2024-04-08 07:56:16.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/zh.js
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-10 21:16:53.816583 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/src/
--rw-rw-r--   0 mark      (1000) mark      (1000)     4098 2024-04-08 05:11:52.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/src/ckeditor.js
--rw-rw-r--   0 mark      (1000) mark      (1000)      632 2024-04-08 05:11:52.000000 django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/src/override-django.css
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-10 21:16:53.772580 django-ckeditors-0.0.4/django_ckeditors/templates/
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-10 21:16:53.816583 django-ckeditors-0.0.4/django_ckeditors/templates/django_ckeditors/
--rw-rw-r--   0 mark      (1000) mark      (1000)      507 2024-04-08 06:07:32.000000 django-ckeditors-0.0.4/django_ckeditors/templates/django_ckeditors/widget.html
--rw-rw-r--   0 mark      (1000) mark      (1000)      146 2024-04-08 06:12:04.000000 django-ckeditors-0.0.4/django_ckeditors/urls.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     2358 2024-04-08 06:13:13.000000 django-ckeditors-0.0.4/django_ckeditors/views.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     2060 2024-04-08 06:07:32.000000 django-ckeditors-0.0.4/django_ckeditors/webpack.config.js
--rw-rw-r--   0 mark      (1000) mark      (1000)     3313 2024-04-08 06:15:07.000000 django-ckeditors-0.0.4/django_ckeditors/widgets.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-10 21:16:53.824583 django-ckeditors-0.0.4/django_ckeditors.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     5123 2024-04-10 21:16:53.000000 django-ckeditors-0.0.4/django_ckeditors.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)     7309 2024-04-10 21:16:53.000000 django-ckeditors-0.0.4/django_ckeditors.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-10 21:16:53.000000 django-ckeditors-0.0.4/django_ckeditors.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)      268 2024-04-10 21:16:53.000000 django-ckeditors-0.0.4/django_ckeditors.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       17 2024-04-10 21:16:53.000000 django-ckeditors-0.0.4/django_ckeditors.egg-info/top_level.txt
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-10 21:16:53.816583 django-ckeditors-0.0.4/docs/
--rw-rw-r--   0 mark      (1000) mark      (1000)      638 2024-04-09 03:51:27.000000 django-ckeditors-0.0.4/docs/Makefile
--rw-rw-r--   0 mark      (1000) mark      (1000)      769 2024-04-09 03:51:27.000000 django-ckeditors-0.0.4/docs/make.bat
--rw-rw-r--   0 mark      (1000) mark      (1000)      132 2024-02-21 00:56:21.000000 django-ckeditors-0.0.4/docs/requirements.txt
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-10 21:16:53.816583 django-ckeditors-0.0.4/docs/source/
--rw-rw-r--   0 mark      (1000) mark      (1000)        0 2024-04-09 03:51:27.000000 django-ckeditors-0.0.4/docs/source/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     2195 2024-04-09 21:53:55.000000 django-ckeditors-0.0.4/docs/source/conf.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      615 2023-11-14 00:51:59.000000 django-ckeditors-0.0.4/docs/source/extras.rst.txt
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-10 21:16:53.816583 django-ckeditors-0.0.4/docs/source/how-to/
--rw-rw-r--   0 mark      (1000) mark      (1000)      183 2024-04-09 04:38:26.000000 django-ckeditors-0.0.4/docs/source/how-to/index-how-to.rst
--rw-rw-r--   0 mark      (1000) mark      (1000)     5670 2024-04-09 07:05:37.000000 django-ckeditors-0.0.4/docs/source/how-to/quickstart.rst
--rw-rw-r--   0 mark      (1000) mark      (1000)      418 2024-04-09 04:52:22.000000 django-ckeditors-0.0.4/docs/source/index.rst
--rw-rw-r--   0 mark      (1000) mark      (1000)      132 2024-04-09 03:51:27.000000 django-ckeditors-0.0.4/docs/source/requirements.txt
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-10 21:16:53.816583 django-ckeditors-0.0.4/example/
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-10 21:16:53.816583 django-ckeditors-0.0.4/example/blog/
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-10 21:16:53.820583 django-ckeditors-0.0.4/example/blog/articles/
--rw-rw-r--   0 mark      (1000) mark      (1000)        0 2024-04-08 05:11:52.000000 django-ckeditors-0.0.4/example/blog/articles/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      343 2024-04-08 05:11:52.000000 django-ckeditors-0.0.4/example/blog/articles/admin.py
--rw-rw-r--   0 mark      (1000) mark      (1000)       91 2024-04-08 05:11:52.000000 django-ckeditors-0.0.4/example/blog/articles/apps.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1150 2024-04-08 06:09:10.000000 django-ckeditors-0.0.4/example/blog/articles/forms.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-10 21:16:53.820583 django-ckeditors-0.0.4/example/blog/articles/migrations/
--rw-rw-r--   0 mark      (1000) mark      (1000)     2230 2024-04-08 23:46:02.000000 django-ckeditors-0.0.4/example/blog/articles/migrations/0001_initial.py
--rw-rw-r--   0 mark      (1000) mark      (1000)        0 2024-04-08 05:11:52.000000 django-ckeditors-0.0.4/example/blog/articles/migrations/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      894 2024-04-08 06:18:14.000000 django-ckeditors-0.0.4/example/blog/articles/models.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      363 2024-04-08 06:07:32.000000 django-ckeditors-0.0.4/example/blog/articles/storage.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-10 21:16:53.820583 django-ckeditors-0.0.4/example/blog/articles/templates/
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-10 21:16:53.820583 django-ckeditors-0.0.4/example/blog/articles/templates/articles/
--rw-rw-r--   0 mark      (1000) mark      (1000)      255 2024-04-08 05:11:52.000000 django-ckeditors-0.0.4/example/blog/articles/templates/articles/article_create.html
--rw-rw-r--   0 mark      (1000) mark      (1000)      843 2024-04-08 05:11:52.000000 django-ckeditors-0.0.4/example/blog/articles/templates/articles/article_detail.html
--rw-rw-r--   0 mark      (1000) mark      (1000)     1155 2024-04-08 05:11:52.000000 django-ckeditors-0.0.4/example/blog/articles/templates/articles/article_list.html
--rw-rw-r--   0 mark      (1000) mark      (1000)      556 2024-04-08 05:11:52.000000 django-ckeditors-0.0.4/example/blog/articles/templates/articles/dynamic_editor.html
--rw-rw-r--   0 mark      (1000) mark      (1000)      287 2024-04-08 05:11:52.000000 django-ckeditors-0.0.4/example/blog/articles/templates/base.html
--rw-rw-r--   0 mark      (1000) mark      (1000)      423 2024-04-08 05:11:52.000000 django-ckeditors-0.0.4/example/blog/articles/urls.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1580 2024-04-08 05:11:52.000000 django-ckeditors-0.0.4/example/blog/articles/views.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-10 21:16:53.820583 django-ckeditors-0.0.4/example/blog/blog/
--rw-rw-r--   0 mark      (1000) mark      (1000)       23 2024-04-08 21:51:50.000000 django-ckeditors-0.0.4/example/blog/blog/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      402 2024-04-08 21:52:13.000000 django-ckeditors-0.0.4/example/blog/blog/asgi.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     8932 2024-04-08 09:29:10.000000 django-ckeditors-0.0.4/example/blog/blog/settings.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1109 2024-04-08 06:18:14.000000 django-ckeditors-0.0.4/example/blog/blog/urls.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      402 2024-04-08 21:52:29.000000 django-ckeditors-0.0.4/example/blog/blog/wsgi.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      424 2024-04-08 06:21:01.000000 django-ckeditors-0.0.4/example/blog/conftest.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-10 21:16:53.772580 django-ckeditors-0.0.4/example/blog/fixtures/
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-10 21:16:53.824583 django-ckeditors-0.0.4/example/blog/fixtures/files/
--rw-rw-r--   0 mark      (1000) mark      (1000)    45044 2024-04-08 22:15:17.000000 django-ckeditors-0.0.4/example/blog/fixtures/files/test.png
--rwxrwxr-x   0 mark      (1000) mark      (1000)      673 2024-04-08 22:16:13.000000 django-ckeditors-0.0.4/example/blog/manage.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-10 21:16:53.824583 django-ckeditors-0.0.4/example/blog/static_files/
--rw-rw-r--   0 mark      (1000) mark      (1000)     5319 2024-04-08 06:21:01.000000 django-ckeditors-0.0.4/example/blog/static_files/custom.css
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-10 21:16:53.824583 django-ckeditors-0.0.4/example/blog/tests/
--rw-rw-r--   0 mark      (1000) mark      (1000)      392 2024-04-08 06:21:01.000000 django-ckeditors-0.0.4/example/blog/tests/test_fields.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      646 2024-04-08 06:07:32.000000 django-ckeditors-0.0.4/example/blog/tests/test_forms.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1251 2024-04-08 09:16:46.000000 django-ckeditors-0.0.4/example/blog/tests/test_storage.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      765 2024-04-08 09:21:04.000000 django-ckeditors-0.0.4/example/blog/tests/test_upload_file.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1287 2024-04-08 09:20:47.000000 django-ckeditors-0.0.4/example/pyproject.toml
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-10 21:16:53.824583 django-ckeditors-0.0.4/node_modules/
--rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-08 06:50:18.000000 django-ckeditors-0.0.4/node_modules/.yarn-integrity
--rw-rw-r--   0 mark      (1000) mark      (1000)     5118 2024-04-09 21:52:26.000000 django-ckeditors-0.0.4/pyproject.toml
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-10 21:16:53.828584 django-ckeditors-0.0.4/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      200 2024-04-08 22:17:49.000000 django-ckeditors-0.0.4/setup.py
--rw-rw-r--   0 mark      (1000) mark      (1000)       86 2024-04-08 06:50:18.000000 django-ckeditors-0.0.4/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:49:44.216526 django-ckeditors-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:49:44.180526 django-ckeditors-0.0.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:49:44.180526 django-ckeditors-0.0.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/.github/ISSUE_TEMPLATE/chore.md
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/.github/ISSUE_TEMPLATE/documentation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:49:44.180526 django-ckeditors-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/.github/workflows/lint_python.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/.github/workflows/testpypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-04-10 21:49:44.216526 django-ckeditors-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    20263 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/commit_history_prior_to_vendoring.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:49:44.180526 django-ckeditors-0.0.5/django_ckeditors/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/django_ckeditors/.jshintrc
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/django_ckeditors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/django_ckeditors/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/django_ckeditors/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)   228033 2024-04-10 21:49:18.000000 django-ckeditors-0.0.5/django_ckeditors/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/django_ckeditors/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:49:44.172526 django-ckeditors-0.0.5/django_ckeditors/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:49:44.184526 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/
+-rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/app.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:49:44.192525 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/
+-rw-r--r--   0 runner    (1001) docker     (127)  1057374 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/bundle.js
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/bundle.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  6303895 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/bundle.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)   147780 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/styles.css
+-rw-r--r--   0 runner    (1001) docker     (127)   272908 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/styles.css.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:49:44.204526 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/af.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12237 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/ar.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/ast.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/az.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14250 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/bg.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16177 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/bn.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/bs.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10293 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/ca.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/cs.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9415 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/da.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/de-ch.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9919 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/de.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14983 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/el.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8627 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/en-au.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6085 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/en-gb.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/eo.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/es-co.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10073 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/es.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9437 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/et.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/eu.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8590 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/fa.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9630 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/fi.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10373 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/fr.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10061 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/gl.js
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/gu.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11489 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/he.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10448 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/hi.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9131 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/hr.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10164 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/hu.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/hy.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9132 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/id.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10495 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/it.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/ja.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/jv.js
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/kk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/km.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/kn.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9800 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/ko.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8457 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/ku.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10500 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/lt.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10026 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/lv.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/ms.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/nb.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9566 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/ne.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9699 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/nl.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9317 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/no.js
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/oc.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10275 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/pl.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9867 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/pt-br.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10083 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/pt.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10012 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/ro.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14547 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/ru.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/si.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9918 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/sk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/sl.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7367 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/sq.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9671 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/sr-latn.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12923 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/sr.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9260 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/sv.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16031 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/th.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7970 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/tk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9811 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/tr.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/tt.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/ug.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14073 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/uk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8544 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/ur.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/uz.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10741 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/vi.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8988 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/zh-cn.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8590 2024-04-10 21:49:37.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/zh.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:49:44.208526 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/src/ckeditor.js
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/src/override-django.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:49:44.176525 django-ckeditors-0.0.5/django_ckeditors/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:49:44.208526 django-ckeditors-0.0.5/django_ckeditors/templates/django_ckeditors/
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/django_ckeditors/templates/django_ckeditors/widget.html
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/django_ckeditors/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/django_ckeditors/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/django_ckeditors/webpack.config.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/django_ckeditors/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:49:44.212526 django-ckeditors-0.0.5/django_ckeditors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-04-10 21:49:44.000000 django-ckeditors-0.0.5/django_ckeditors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-04-10 21:49:44.000000 django-ckeditors-0.0.5/django_ckeditors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 21:49:44.000000 django-ckeditors-0.0.5/django_ckeditors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-10 21:49:44.000000 django-ckeditors-0.0.5/django_ckeditors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 21:49:44.000000 django-ckeditors-0.0.5/django_ckeditors.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:49:44.208526 django-ckeditors-0.0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:49:44.208526 django-ckeditors-0.0.5/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/docs/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/docs/source/extras.rst.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:49:44.208526 django-ckeditors-0.0.5/docs/source/how-to/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/docs/source/how-to/index-how-to.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/docs/source/how-to/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/docs/source/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:49:44.208526 django-ckeditors-0.0.5/example/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:49:44.208526 django-ckeditors-0.0.5/example/blog/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:49:44.208526 django-ckeditors-0.0.5/example/blog/articles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/example/blog/articles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/example/blog/articles/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/example/blog/articles/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/example/blog/articles/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:49:44.212526 django-ckeditors-0.0.5/example/blog/articles/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/example/blog/articles/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/example/blog/articles/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/example/blog/articles/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/example/blog/articles/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:49:44.212526 django-ckeditors-0.0.5/example/blog/articles/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:49:44.212526 django-ckeditors-0.0.5/example/blog/articles/templates/articles/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/example/blog/articles/templates/articles/article_create.html
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/example/blog/articles/templates/articles/article_detail.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/example/blog/articles/templates/articles/article_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/example/blog/articles/templates/articles/dynamic_editor.html
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/example/blog/articles/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/example/blog/articles/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/example/blog/articles/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:49:44.212526 django-ckeditors-0.0.5/example/blog/blog/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/example/blog/blog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/example/blog/blog/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/example/blog/blog/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/example/blog/blog/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/example/blog/blog/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/example/blog/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:49:44.176525 django-ckeditors-0.0.5/example/blog/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:49:44.212526 django-ckeditors-0.0.5/example/blog/fixtures/files/
+-rw-r--r--   0 runner    (1001) docker     (127)    45044 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/example/blog/fixtures/files/test.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      673 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/example/blog/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:49:44.212526 django-ckeditors-0.0.5/example/blog/static_files/
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/example/blog/static_files/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:49:44.212526 django-ckeditors-0.0.5/example/blog/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/example/blog/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/example/blog/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/example/blog/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/example/blog/tests/test_upload_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/example/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:49:44.212526 django-ckeditors-0.0.5/node_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/node_modules/.yarn-integrity
+-rw-r--r--   0 runner    (1001) docker     (127)     5118 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 21:49:44.216526 django-ckeditors-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-10 21:49:12.000000 django-ckeditors-0.0.5/yarn.lock
```

### Comparing `django-ckeditors-0.0.4/.github/FUNDING.yml` & `django-ckeditors-0.0.5/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/.github/ISSUE_TEMPLATE/bug_report.md` & `django-ckeditors-0.0.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md` & `django-ckeditors-0.0.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/.github/archive/release.yml` & `django-ckeditors-0.0.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/.github/workflows/lint_python.yml` & `django-ckeditors-0.0.5/.github/workflows/lint_python.yml`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/.github/workflows/testpypi.yml` & `django-ckeditors-0.0.5/.github/workflows/testpypi.yml`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/.gitignore` & `django-ckeditors-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/LICENSE` & `django-ckeditors-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/PKG-INFO` & `django-ckeditors-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ckeditors
-Version: 0.0.4
+Version: 0.0.5
 Summary: CKEditors for Django.
 Author-email: Vladislav Khoboko <vladislah@gmail.com>, Mark Sevelj <mark.sevelj@dunwright.com.au>
 License: BSD-3-Clause
 Project-URL: homepage, https://pypi.org/project/django-ckeditors/
 Project-URL: repository, https://github.com/imAsparky/django-ckeditors.git
 Keywords: CKEditor,CKEditors,Django
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `django-ckeditors-0.0.4/README.rst` & `django-ckeditors-0.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/commit_history_prior_to_vendoring.txt` & `django-ckeditors-0.0.5/commit_history_prior_to_vendoring.txt`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/fields.py` & `django-ckeditors-0.0.5/django_ckeditors/fields.py`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/package-lock.json` & `django-ckeditors-0.0.5/django_ckeditors/package-lock.json`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/package.json` & `django-ckeditors-0.0.5/django_ckeditors/package.json`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/app.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/app.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/bundle.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/bundle.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/bundle.js.LICENSE.txt` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/bundle.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/bundle.js.map` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/bundle.js.map`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/styles.css` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/styles.css`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/styles.css.map` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/styles.css.map`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/af.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/af.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/ar.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/ar.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/ast.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/ast.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/az.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/az.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/bg.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/bg.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/bn.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/bn.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/bs.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/bs.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/ca.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/ca.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/cs.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/cs.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/da.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/da.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/de-ch.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/de-ch.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/de.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/de.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/el.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/el.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/en-au.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/en-au.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/en-gb.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/en-gb.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/eo.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/eo.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/es-co.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/es-co.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/es.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/es.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/et.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/et.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/eu.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/eu.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/fa.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/fa.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/fi.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/fi.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/fr.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/fr.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/gl.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/gl.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/gu.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/gu.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/he.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/he.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/hi.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/hi.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/hr.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/hr.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/hu.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/hu.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/hy.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/hy.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/id.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/id.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/it.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/it.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/ja.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/ja.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/jv.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/jv.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/km.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/km.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/kn.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/kn.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/ko.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/ko.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/ku.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/ku.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/lt.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/lt.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/lv.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/lv.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/ms.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/ms.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/nb.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/nb.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/ne.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/ne.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/nl.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/nl.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/no.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/no.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/pl.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/pl.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/pt-br.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/pt-br.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/pt.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/pt.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/ro.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/ro.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/ru.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/ru.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/si.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/si.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/sk.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/sk.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/sl.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/sl.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/sq.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/sq.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/sr-latn.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/sr-latn.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/sr.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/sr.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/sv.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/sv.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/th.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/th.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/tk.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/tk.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/tr.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/tr.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/tt.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/tt.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/ug.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/ug.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/uk.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/uk.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/ur.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/ur.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/uz.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/uz.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/vi.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/vi.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/zh-cn.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/zh-cn.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/dist/translations/zh.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/dist/translations/zh.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/src/ckeditor.js` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/src/ckeditor.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/static/django_ckeditors/src/override-django.css` & `django-ckeditors-0.0.5/django_ckeditors/static/django_ckeditors/src/override-django.css`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/views.py` & `django-ckeditors-0.0.5/django_ckeditors/views.py`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/webpack.config.js` & `django-ckeditors-0.0.5/django_ckeditors/webpack.config.js`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors/widgets.py` & `django-ckeditors-0.0.5/django_ckeditors/widgets.py`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/django_ckeditors.egg-info/PKG-INFO` & `django-ckeditors-0.0.5/django_ckeditors.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ckeditors
-Version: 0.0.4
+Version: 0.0.5
 Summary: CKEditors for Django.
 Author-email: Vladislav Khoboko <vladislah@gmail.com>, Mark Sevelj <mark.sevelj@dunwright.com.au>
 License: BSD-3-Clause
 Project-URL: homepage, https://pypi.org/project/django-ckeditors/
 Project-URL: repository, https://github.com/imAsparky/django-ckeditors.git
 Keywords: CKEditor,CKEditors,Django
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `django-ckeditors-0.0.4/django_ckeditors.egg-info/SOURCES.txt` & `django-ckeditors-0.0.5/django_ckeditors.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 setup.py
 yarn.lock
 .github/FUNDING.yml
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/chore.md
 .github/ISSUE_TEMPLATE/documentation.md
 .github/ISSUE_TEMPLATE/feature_request.md
-.github/archive/release.yml
 .github/workflows/lint_python.yml
+.github/workflows/release.yml
 .github/workflows/testpypi.yml
 django_ckeditors/.jshintrc
 django_ckeditors/__init__.py
 django_ckeditors/fields.py
 django_ckeditors/forms.py
 django_ckeditors/package-lock.json
 django_ckeditors/package.json
```

### Comparing `django-ckeditors-0.0.4/docs/Makefile` & `django-ckeditors-0.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/docs/make.bat` & `django-ckeditors-0.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/docs/source/conf.py` & `django-ckeditors-0.0.5/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 import os
 import sys
 
 sys.path.insert(0, os.path.abspath(".."))
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 
 project = "Django CKEditors"
 project_copyright = "2024, Mark Sevelj"
 author = "Mark Sevelj"
 release = __version__
 
 # -- General configuration ---------------------------------------------------
```

### Comparing `django-ckeditors-0.0.4/docs/source/extras.rst.txt` & `django-ckeditors-0.0.5/docs/source/extras.rst.txt`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/docs/source/how-to/quickstart.rst` & `django-ckeditors-0.0.5/docs/source/how-to/quickstart.rst`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/example/blog/articles/forms.py` & `django-ckeditors-0.0.5/example/blog/articles/forms.py`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/example/blog/articles/migrations/0001_initial.py` & `django-ckeditors-0.0.5/example/blog/articles/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/example/blog/articles/models.py` & `django-ckeditors-0.0.5/example/blog/articles/models.py`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/example/blog/articles/templates/articles/article_detail.html` & `django-ckeditors-0.0.5/example/blog/articles/templates/articles/article_detail.html`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/example/blog/articles/templates/articles/article_list.html` & `django-ckeditors-0.0.5/example/blog/articles/templates/articles/article_list.html`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/example/blog/articles/templates/articles/dynamic_editor.html` & `django-ckeditors-0.0.5/example/blog/articles/templates/articles/dynamic_editor.html`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/example/blog/articles/views.py` & `django-ckeditors-0.0.5/example/blog/articles/views.py`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/example/blog/blog/settings.py` & `django-ckeditors-0.0.5/example/blog/blog/settings.py`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/example/blog/blog/urls.py` & `django-ckeditors-0.0.5/example/blog/blog/urls.py`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/example/blog/fixtures/files/test.png` & `django-ckeditors-0.0.5/example/blog/fixtures/files/test.png`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/example/blog/manage.py` & `django-ckeditors-0.0.5/example/blog/manage.py`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/example/blog/static_files/custom.css` & `django-ckeditors-0.0.5/example/blog/static_files/custom.css`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/example/blog/tests/test_forms.py` & `django-ckeditors-0.0.5/example/blog/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/example/blog/tests/test_storage.py` & `django-ckeditors-0.0.5/example/blog/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/example/blog/tests/test_upload_file.py` & `django-ckeditors-0.0.5/example/blog/tests/test_upload_file.py`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/example/pyproject.toml` & `django-ckeditors-0.0.5/example/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-ckeditors-0.0.4/pyproject.toml` & `django-ckeditors-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "django-ckeditors"
 description = "CKEditors for Django."
 keywords = ["CKEditor", "CKEditors", "Django"]
 license = {text = "BSD-3-Clause"}
 readme = "README.rst"
 requires-python = ">=3.7"
-version = "0.0.4"
+version = "0.0.5"
 
 authors = [
     {"name" = "Vladislav Khoboko", "email" = "vladislah@gmail.com"},
     {"name" = "Mark Sevelj", "email" = "mark.sevelj@dunwright.com.au"},
 ]
 
 classifiers = [
```

