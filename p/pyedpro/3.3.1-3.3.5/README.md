# Comparing `tmp/pyedpro-3.3.1.tar.gz` & `tmp/pyedpro-3.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyedpro-3.3.1.tar", last modified: Thu Feb 15 18:59:27 2024, max compression
+gzip compressed data, was "pyedpro-3.3.5.tar", last modified: Wed Apr 10 06:50:43 2024, max compression
```

## Comparing `pyedpro-3.3.1.tar` & `pyedpro-3.3.5.tar`

### file list

```diff
@@ -1,123 +1,177 @@
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-02-15 18:59:27.725711 pyedpro-3.3.1/
--rw-r--r--   0 peterglen  (1000) users      (100)    35153 2023-09-14 20:07:28.000000 pyedpro-3.3.1/LICENSE
--rw-r--r--   0 peterglen  (1000) users      (100)    10876 2024-02-15 18:59:27.725711 pyedpro-3.3.1/PKG-INFO
--rw-rw-r--   0 peterglen  (1000) users      (100)    10409 2022-09-23 16:51:47.000000 pyedpro-3.3.1/README.md
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-02-15 18:59:27.697710 pyedpro-3.3.1/panglib/
--rw-r--r--   0 peterglen  (1000) users      (100)      305 2023-09-14 20:07:28.000000 pyedpro-3.3.1/panglib/__init__.py
--rw-r--r--   0 peterglen  (1000) users      (100)     1564 2023-09-14 20:07:28.000000 pyedpro-3.3.1/panglib/lexer.py
--rw-r--r--   0 peterglen  (1000) users      (100)    14285 2023-09-14 20:07:28.000000 pyedpro-3.3.1/panglib/pangdisp.py
--rw-r--r--   0 peterglen  (1000) users      (100)    25354 2023-09-14 20:07:28.000000 pyedpro-3.3.1/panglib/pangfunc.py
--rw-r--r--   0 peterglen  (1000) users      (100)     4668 2023-09-14 20:07:28.000000 pyedpro-3.3.1/panglib/parser.py
--rw-r--r--   0 peterglen  (1000) users      (100)     1692 2023-09-14 20:07:28.000000 pyedpro-3.3.1/panglib/stack.py
--rw-r--r--   0 peterglen  (1000) users      (100)     5656 2023-09-14 20:07:28.000000 pyedpro-3.3.1/panglib/utils.py
--rwxr-xr-x   0 peterglen  (1000) users      (100)    37015 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pangview.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-02-15 18:59:27.709710 pyedpro-3.3.1/pedlib/
--rw-r--r--   0 peterglen  (1000) users      (100)      161 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/__init__.py
--rw-r--r--   0 peterglen  (1000) users      (100)    80657 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/acthand.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-02-15 18:59:27.717711 pyedpro-3.3.1/pedlib/data/
--rw-r--r--   0 peterglen  (1000) users      (100)    10919 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/data/KEYS
--rw-r--r--   0 peterglen  (1000) users      (100)    13260 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/data/KEYS.TXT
--rw-r--r--   0 peterglen  (1000) users      (100)    11219 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/data/KEYS.old
--rw-r--r--   0 peterglen  (1000) users      (100)    16254 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/data/PyGObject.txt
--rw-r--r--   0 peterglen  (1000) users      (100)     3143 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/data/QHELP
--rw-r--r--   0 peterglen  (1000) users      (100)        0 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/data/__init__.py
--rw-r--r--   0 peterglen  (1000) users      (100)  2283311 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/data/spell.txt
--rw-r--r--   0 peterglen  (1000) users      (100)      792 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/data/test.Makefile
--rw-r--r--   0 peterglen  (1000) users      (100)     4176 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/data/test.S
--rw-r--r--   0 peterglen  (1000) users      (100)    16003 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/data/test.c
--rw-r--r--   0 peterglen  (1000) users      (100)     1961 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/data/test.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-02-15 18:59:27.717711 pyedpro-3.3.1/pedlib/images/
--rw-r--r--   0 peterglen  (1000) users      (100)     6427 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/images/gtk-logo-rgb.gif
--rw-r--r--   0 peterglen  (1000) users      (100)      653 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/images/pedicon.png
--rw-r--r--   0 peterglen  (1000) users      (100)     4598 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/images/pedicon.svg
--rw-r--r--   0 peterglen  (1000) users      (100)     4210 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/images/pyedpro.png
--rw-r--r--   0 peterglen  (1000) users      (100)     3677 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/images/pyedpro.svg
--rw-r--r--   0 peterglen  (1000) users      (100)     6587 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/images/pyedpro_sub.png
--rw-r--r--   0 peterglen  (1000) users      (100)      645 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/images/rect3713-3.png
--rw-r--r--   0 peterglen  (1000) users      (100)      597 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/images/rect3713.png
--rw-r--r--   0 peterglen  (1000) users      (100)      295 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/importer.py
--rw-r--r--   0 peterglen  (1000) users      (100)    32296 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/keyhand.py
--rw-r--r--   0 peterglen  (1000) users      (100)     3516 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/keywords.py
--rw-r--r--   0 peterglen  (1000) users      (100)     2558 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/leven.py
--rw-r--r--   0 peterglen  (1000) users      (100)     1771 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/lexer.py
--rw-r--r--   0 peterglen  (1000) users      (100)    12478 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/notesql.py
--rw-r--r--   0 peterglen  (1000) users      (100)     7334 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/parser.py
--rw-r--r--   0 peterglen  (1000) users      (100)     8872 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/pedbuffs.py
--rw-r--r--   0 peterglen  (1000) users      (100)    15642 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/pedcal.py
--rw-r--r--   0 peterglen  (1000) users      (100)    32041 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/pedcanv.py
--rw-r--r--   0 peterglen  (1000) users      (100)    11451 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/pedcolor.py
--rw-r--r--   0 peterglen  (1000) users      (100)     3842 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/pedconfig.py
--rw-r--r--   0 peterglen  (1000) users      (100)     5268 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/peddlg.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    99906 2024-01-02 04:25:57.000000 pyedpro-3.3.1/pedlib/peddoc.py
--rw-r--r--   0 peterglen  (1000) users      (100)    73207 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/peddoc_diff.py
--rw-r--r--   0 peterglen  (1000) users      (100)    18279 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/peddraw.py
--rw-r--r--   0 peterglen  (1000) users      (100)    36498 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/pedfind.py
--rw-r--r--   0 peterglen  (1000) users      (100)     9408 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/pedfont.py
--rw-r--r--   0 peterglen  (1000) users      (100)     5123 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/pedgoto.py
--rw-r--r--   0 peterglen  (1000) users      (100)     2211 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/pedlcmd.py
--rw-r--r--   0 peterglen  (1000) users      (100)     5704 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/pedlog.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    14262 2024-02-15 18:28:08.000000 pyedpro-3.3.1/pedlib/pedmenu.py
--rw-r--r--   0 peterglen  (1000) users      (100)     2159 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/pedmisc.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    23830 2024-02-15 18:14:05.000000 pyedpro-3.3.1/pedlib/pednotes.py
--rw-r--r--   0 peterglen  (1000) users      (100)    16514 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/pedobjs.py
--rw-r--r--   0 peterglen  (1000) users      (100)    13360 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/pedofd.py
--rw-r--r--   0 peterglen  (1000) users      (100)    15573 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/pedoline.py
--rw-r--r--   0 peterglen  (1000) users      (100)     4242 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/pedplug.py
--rw-r--r--   0 peterglen  (1000) users      (100)    11954 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/pedspell.py
--rw-r--r--   0 peterglen  (1000) users      (100)     5139 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/pedsql.py
--rw-r--r--   0 peterglen  (1000) users      (100)     1277 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/pedstruct.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     9244 2023-09-26 04:44:17.000000 pyedpro-3.3.1/pedlib/pedtask.py
--rw-r--r--   0 peterglen  (1000) users      (100)     1986 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/pedtdlg.py
--rw-r--r--   0 peterglen  (1000) users      (100)     2824 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/pedthread.py
--rw-r--r--   0 peterglen  (1000) users      (100)     7225 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/pedtts.py
--rw-r--r--   0 peterglen  (1000) users      (100)     3748 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/pedui.py
--rw-r--r--   0 peterglen  (1000) users      (100)     7099 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/pedundo.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    38749 2024-02-15 18:58:31.000000 pyedpro-3.3.1/pedlib/pedutil.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    21288 2024-02-15 18:16:49.000000 pyedpro-3.3.1/pedlib/pedweb.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    88849 2024-02-15 18:25:31.000000 pyedpro-3.3.1/pedlib/pedwin.py
--rw-r--r--   0 peterglen  (1000) users      (100)      655 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/pedxtnd.py
--rw-r--r--   0 peterglen  (1000) users      (100)     5673 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/pedync.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-02-15 18:59:27.717711 pyedpro-3.3.1/pedlib/plugins/
--rw-r--r--   0 peterglen  (1000) users      (100)      178 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/plugins/__init__.py
--rw-r--r--   0 peterglen  (1000) users      (100)     1603 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/plugins/lower_right.py
--rw-r--r--   0 peterglen  (1000) users      (100)     1836 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/stack.py
--rw-r--r--   0 peterglen  (1000) users      (100)     8371 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/test.py
--rw-r--r--   0 peterglen  (1000) users      (100)     7649 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pedlib/testdiff.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     3126 2023-09-26 04:15:19.000000 pyedpro-3.3.1/pedlib/webwin.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-02-15 18:59:27.725711 pyedpro-3.3.1/pycommon/
--rw-r--r--   0 peterglen  (1000) users      (100)        0 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pycommon/__init__.py
--rw-r--r--   0 peterglen  (1000) users      (100)     7530 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pycommon/browsewin.py
--rw-r--r--   0 peterglen  (1000) users      (100)    10064 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pycommon/htmledit.py
--rw-r--r--   0 peterglen  (1000) users      (100)     8947 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pycommon/icons.py
--rw-r--r--   0 peterglen  (1000) users      (100)    21912 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pycommon/pgbox.py
--rw-r--r--   0 peterglen  (1000) users      (100)     6700 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pycommon/pgbutt.py
--rw-r--r--   0 peterglen  (1000) users      (100)     4932 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pycommon/pgentry.py
--rw-r--r--   0 peterglen  (1000) users      (100)    40484 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pycommon/pggui.py
--rw-r--r--   0 peterglen  (1000) users      (100)    15446 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pycommon/pgsimp.py
--rw-r--r--   0 peterglen  (1000) users      (100)    29354 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pycommon/pgtextview.py
--rw-r--r--   0 peterglen  (1000) users      (100)    31741 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pycommon/pgutils.py
--rw-r--r--   0 peterglen  (1000) users      (100)    25820 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pycommon/pgwkit.py
--rw-r--r--   0 peterglen  (1000) users      (100)     1017 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pycommon/plug.py
--rw-r--r--   0 peterglen  (1000) users      (100)    16446 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pycommon/pypacker.py
--rw-r--r--   0 peterglen  (1000) users      (100)     9158 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pycommon/sutil.py
--rwxr-xr-x   0 peterglen  (1000) users      (100)     2800 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pycommon/testbutt.py
--rwxr-xr-x   0 peterglen  (1000) users      (100)     3222 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pycommon/testnums.py
--rwxr-xr-x   0 peterglen  (1000) users      (100)     2530 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pycommon/testpacker.py
--rwxr-xr-x   0 peterglen  (1000) users      (100)     1202 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pycommon/testpacker2.py
--rwxr-xr-x   0 peterglen  (1000) users      (100)     1102 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pycommon/testpacker3.py
--rwxr-xr-x   0 peterglen  (1000) users      (100)      606 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pycommon/testpacker4.py
--rwxr-xr-x   0 peterglen  (1000) users      (100)     4058 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pycommon/testroot.py
--rwxr-xr-x   0 peterglen  (1000) users      (100)     2401 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pycommon/testsimple.py
--rwxr-xr-x   0 peterglen  (1000) users      (100)     7193 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pycommon/testtextv.py
--rw-r--r--   0 peterglen  (1000) users      (100)     1301 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pyedpro.desktop
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-02-15 18:59:27.725711 pyedpro-3.3.1/pyedpro.egg-info/
--rw-r--r--   0 peterglen  (1000) users      (100)    10876 2024-02-15 18:59:27.000000 pyedpro-3.3.1/pyedpro.egg-info/PKG-INFO
--rw-rw-r--   0 peterglen  (1000) users      (100)     2516 2024-02-15 18:59:27.000000 pyedpro-3.3.1/pyedpro.egg-info/SOURCES.txt
--rw-rw-r--   0 peterglen  (1000) users      (100)        1 2024-02-15 18:59:27.000000 pyedpro-3.3.1/pyedpro.egg-info/dependency_links.txt
--rw-r--r--   0 peterglen  (1000) users      (100)       74 2024-02-15 18:59:27.000000 pyedpro-3.3.1/pyedpro.egg-info/entry_points.txt
--rw-r--r--   0 peterglen  (1000) users      (100)       18 2024-02-15 18:59:27.000000 pyedpro-3.3.1/pyedpro.egg-info/requires.txt
--rw-rw-r--   0 peterglen  (1000) users      (100)       24 2024-02-15 18:59:27.000000 pyedpro-3.3.1/pyedpro.egg-info/top_level.txt
--rwxrwxr-x   0 peterglen  (1000) users      (100)    14929 2024-02-15 18:18:50.000000 pyedpro-3.3.1/pyedpro.py
--rw-r--r--   0 peterglen  (1000) users      (100)      106 2023-09-14 20:07:28.000000 pyedpro-3.3.1/pyproject.toml
--rw-r--r--   0 peterglen  (1000) users      (100)       38 2024-02-15 18:59:27.725711 pyedpro-3.3.1/setup.cfg
--rw-rw-r--   0 peterglen  (1000) users      (100)     3517 2024-02-15 18:19:01.000000 pyedpro-3.3.1/setup.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-10 06:50:43.553899 pyedpro-3.3.5/
+-rw-r--r--   0 peterglen  (1000) users      (100)    35153 2023-09-14 20:07:28.000000 pyedpro-3.3.5/LICENSE
+-rw-r--r--   0 peterglen  (1000) users      (100)    11519 2024-04-10 06:50:43.553899 pyedpro-3.3.5/PKG-INFO
+-rw-r--r--   0 peterglen  (1000) users      (100)    11053 2024-04-10 06:50:39.000000 pyedpro-3.3.5/README.md
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-10 06:50:43.513898 pyedpro-3.3.5/panglib/
+-rw-r--r--   0 peterglen  (1000) users      (100)      305 2023-09-14 20:07:28.000000 pyedpro-3.3.5/panglib/__init__.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     1564 2023-09-14 20:07:28.000000 pyedpro-3.3.5/panglib/lexer.py
+-rw-r--r--   0 peterglen  (1000) users      (100)    14285 2023-09-14 20:07:28.000000 pyedpro-3.3.5/panglib/pangdisp.py
+-rw-r--r--   0 peterglen  (1000) users      (100)    25354 2023-09-14 20:07:28.000000 pyedpro-3.3.5/panglib/pangfunc.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     4668 2023-09-14 20:07:28.000000 pyedpro-3.3.5/panglib/parser.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     1692 2023-09-14 20:07:28.000000 pyedpro-3.3.5/panglib/stack.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     5656 2023-09-14 20:07:28.000000 pyedpro-3.3.5/panglib/utils.py
+-rwxr-xr-x   0 peterglen  (1000) users      (100)    37015 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pangview.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-10 06:50:43.521899 pyedpro-3.3.5/pedlib/
+-rw-r--r--   0 peterglen  (1000) users      (100)      161 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/__init__.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    81624 2024-03-05 14:45:28.000000 pyedpro-3.3.5/pedlib/acthand.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-10 06:50:43.529899 pyedpro-3.3.5/pedlib/data/
+-rw-r--r--   0 peterglen  (1000) users      (100)    10919 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/data/KEYS
+-rw-rw-r--   0 peterglen  (1000) users      (100)    13313 2024-03-05 14:40:41.000000 pyedpro-3.3.5/pedlib/data/KEYS.TXT
+-rw-r--r--   0 peterglen  (1000) users      (100)    11219 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/data/KEYS.old
+-rw-r--r--   0 peterglen  (1000) users      (100)    16254 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/data/PyGObject.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)     3143 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/data/QHELP
+-rw-r--r--   0 peterglen  (1000) users      (100)        0 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/data/__init__.py
+-rw-r--r--   0 peterglen  (1000) users      (100)  2283311 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/data/spell.txt
+-rw-rw-r--   0 peterglen  (1000) users      (100)      793 2024-04-09 14:18:16.000000 pyedpro-3.3.5/pedlib/data/test.Makefile
+-rw-r--r--   0 peterglen  (1000) users      (100)     4176 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/data/test.S
+-rw-r--r--   0 peterglen  (1000) users      (100)    16003 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/data/test.c
+-rw-r--r--   0 peterglen  (1000) users      (100)     1961 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/data/test.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-10 06:50:43.541899 pyedpro-3.3.5/pedlib/docs/
+-rw-r--r--   0 peterglen  (1000) users      (100)   292331 2024-04-10 03:46:39.000000 pyedpro-3.3.5/pedlib/docs/acthand.html
+-rw-r--r--   0 peterglen  (1000) users      (100)     6420 2024-04-10 03:46:39.000000 pyedpro-3.3.5/pedlib/docs/importer.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    89054 2024-04-10 03:46:40.000000 pyedpro-3.3.5/pedlib/docs/keyhand.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    10600 2024-04-10 03:46:41.000000 pyedpro-3.3.5/pedlib/docs/keywords.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    12165 2024-04-10 03:46:41.000000 pyedpro-3.3.5/pedlib/docs/leven.html
+-rw-r--r--   0 peterglen  (1000) users      (100)     9447 2024-04-10 03:46:36.000000 pyedpro-3.3.5/pedlib/docs/lexer.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    47580 2024-04-10 03:46:34.000000 pyedpro-3.3.5/pedlib/docs/notesql.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    24369 2024-04-10 03:46:33.000000 pyedpro-3.3.5/pedlib/docs/parser.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    27295 2024-04-10 03:46:34.000000 pyedpro-3.3.5/pedlib/docs/pedbuffs.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    57335 2024-04-10 03:46:42.000000 pyedpro-3.3.5/pedlib/docs/pedcal.html
+-rw-r--r--   0 peterglen  (1000) users      (100)   112725 2024-04-10 03:46:42.000000 pyedpro-3.3.5/pedlib/docs/pedcanv.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    39587 2024-04-10 03:46:43.000000 pyedpro-3.3.5/pedlib/docs/pedcolor.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    16563 2024-04-10 03:46:43.000000 pyedpro-3.3.5/pedlib/docs/pedconfig.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    16774 2024-04-10 03:46:44.000000 pyedpro-3.3.5/pedlib/docs/peddlg.html
+-rw-r--r--   0 peterglen  (1000) users      (100)   339943 2024-04-10 03:46:35.000000 pyedpro-3.3.5/pedlib/docs/peddoc.html
+-rw-r--r--   0 peterglen  (1000) users      (100)   260486 2024-04-10 03:46:37.000000 pyedpro-3.3.5/pedlib/docs/peddoc_diff.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    60681 2024-04-10 03:46:45.000000 pyedpro-3.3.5/pedlib/docs/peddraw.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    90762 2024-04-10 03:46:45.000000 pyedpro-3.3.5/pedlib/docs/pedfind.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    28138 2024-04-10 03:46:46.000000 pyedpro-3.3.5/pedlib/docs/pedfont.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    17483 2024-04-10 03:46:46.000000 pyedpro-3.3.5/pedlib/docs/pedgoto.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    11050 2024-04-10 03:46:47.000000 pyedpro-3.3.5/pedlib/docs/pedlcmd.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    24284 2024-04-10 03:46:47.000000 pyedpro-3.3.5/pedlib/docs/pedlog.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    38162 2024-04-10 03:46:48.000000 pyedpro-3.3.5/pedlib/docs/pedmenu.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    10849 2024-04-10 03:46:48.000000 pyedpro-3.3.5/pedlib/docs/pedmisc.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    83915 2024-04-10 03:46:49.000000 pyedpro-3.3.5/pedlib/docs/pednotes.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    64936 2024-04-10 03:46:50.000000 pyedpro-3.3.5/pedlib/docs/pedobjs.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    39047 2024-04-10 03:46:51.000000 pyedpro-3.3.5/pedlib/docs/pedofd.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    61244 2024-04-10 03:46:51.000000 pyedpro-3.3.5/pedlib/docs/pedoline.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    17038 2024-04-10 03:46:52.000000 pyedpro-3.3.5/pedlib/docs/pedplug.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    32250 2024-04-10 03:46:53.000000 pyedpro-3.3.5/pedlib/docs/pedspell.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    22015 2024-04-10 03:46:53.000000 pyedpro-3.3.5/pedlib/docs/pedsql.html
+-rw-r--r--   0 peterglen  (1000) users      (100)     8894 2024-04-10 03:46:54.000000 pyedpro-3.3.5/pedlib/docs/pedstruct.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    37220 2024-04-10 03:46:36.000000 pyedpro-3.3.5/pedlib/docs/pedtask.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    10674 2024-04-10 03:46:54.000000 pyedpro-3.3.5/pedlib/docs/pedtdlg.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    14476 2024-04-10 03:46:33.000000 pyedpro-3.3.5/pedlib/docs/pedthread.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    28317 2024-04-10 03:46:55.000000 pyedpro-3.3.5/pedlib/docs/pedtts.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    12432 2024-04-10 03:46:55.000000 pyedpro-3.3.5/pedlib/docs/pedui.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    19906 2024-04-10 03:46:56.000000 pyedpro-3.3.5/pedlib/docs/pedundo.html
+-rw-r--r--   0 peterglen  (1000) users      (100)   108350 2024-04-10 03:46:56.000000 pyedpro-3.3.5/pedlib/docs/pedutil.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    72124 2024-04-10 03:46:32.000000 pyedpro-3.3.5/pedlib/docs/pedweb.html
+-rw-r--r--   0 peterglen  (1000) users      (100)   292122 2024-04-10 03:46:57.000000 pyedpro-3.3.5/pedlib/docs/pedwin.html
+-rw-r--r--   0 peterglen  (1000) users      (100)     7430 2024-04-10 03:46:58.000000 pyedpro-3.3.5/pedlib/docs/pedxtnd.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    19404 2024-04-10 03:46:58.000000 pyedpro-3.3.5/pedlib/docs/pedync.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    15523 2024-04-10 03:46:59.000000 pyedpro-3.3.5/pedlib/docs/stack.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    13477 2024-04-10 03:46:59.000000 pyedpro-3.3.5/pedlib/docs/webwin.html
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-10 06:50:43.541899 pyedpro-3.3.5/pedlib/images/
+-rw-r--r--   0 peterglen  (1000) users      (100)     6427 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/images/gtk-logo-rgb.gif
+-rw-r--r--   0 peterglen  (1000) users      (100)      653 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/images/pedicon.png
+-rw-r--r--   0 peterglen  (1000) users      (100)     4598 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/images/pedicon.svg
+-rw-r--r--   0 peterglen  (1000) users      (100)     4210 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/images/pyedpro.png
+-rw-r--r--   0 peterglen  (1000) users      (100)     3677 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/images/pyedpro.svg
+-rw-r--r--   0 peterglen  (1000) users      (100)     6587 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/images/pyedpro_sub.png
+-rw-r--r--   0 peterglen  (1000) users      (100)      645 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/images/rect3713-3.png
+-rw-r--r--   0 peterglen  (1000) users      (100)      597 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/images/rect3713.png
+-rw-r--r--   0 peterglen  (1000) users      (100)      295 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/importer.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    32297 2024-03-19 01:10:23.000000 pyedpro-3.3.5/pedlib/keyhand.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     3516 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/keywords.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     2558 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/leven.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     1771 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/lexer.py
+-rw-r--r--   0 peterglen  (1000) users      (100)    12478 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/notesql.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     6536 2024-04-10 03:40:22.000000 pyedpro-3.3.5/pedlib/parser.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     8877 2024-04-10 03:38:43.000000 pyedpro-3.3.5/pedlib/pedbuffs.py
+-rw-r--r--   0 peterglen  (1000) users      (100)    15642 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/pedcal.py
+-rw-r--r--   0 peterglen  (1000) users      (100)    32041 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/pedcanv.py
+-rw-r--r--   0 peterglen  (1000) users      (100)    11451 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/pedcolor.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     3842 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/pedconfig.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     5268 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/peddlg.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    99906 2024-04-10 03:45:01.000000 pyedpro-3.3.5/pedlib/peddoc.py
+-rw-r--r--   0 peterglen  (1000) users      (100)    73207 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/peddoc_diff.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    18704 2024-04-10 03:45:38.000000 pyedpro-3.3.5/pedlib/peddraw.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    36605 2024-04-09 12:58:38.000000 pyedpro-3.3.5/pedlib/pedfind.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     9408 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/pedfont.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     5123 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/pedgoto.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     2211 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/pedlcmd.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     5704 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/pedlog.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    14262 2024-02-15 18:28:08.000000 pyedpro-3.3.5/pedlib/pedmenu.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     2159 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/pedmisc.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    26045 2024-04-10 04:20:26.000000 pyedpro-3.3.5/pedlib/pednotes.py
+-rw-r--r--   0 peterglen  (1000) users      (100)    16514 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/pedobjs.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    13376 2024-04-10 03:51:37.000000 pyedpro-3.3.5/pedlib/pedofd.py
+-rw-r--r--   0 peterglen  (1000) users      (100)    15573 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/pedoline.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     4344 2024-04-10 03:46:13.000000 pyedpro-3.3.5/pedlib/pedplug.py
+-rw-r--r--   0 peterglen  (1000) users      (100)    11954 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/pedspell.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     5139 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/pedsql.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     1277 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/pedstruct.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     9309 2024-04-10 02:56:20.000000 pyedpro-3.3.5/pedlib/pedtask.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     1986 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/pedtdlg.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     2824 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/pedthread.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     7225 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/pedtts.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     3748 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/pedui.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     7099 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/pedundo.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    38749 2024-02-15 18:58:31.000000 pyedpro-3.3.5/pedlib/pedutil.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    22065 2024-04-10 03:42:04.000000 pyedpro-3.3.5/pedlib/pedweb.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    88905 2024-04-10 03:42:58.000000 pyedpro-3.3.5/pedlib/pedwin.py
+-rw-r--r--   0 peterglen  (1000) users      (100)      655 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/pedxtnd.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     5673 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/pedync.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-10 06:50:43.541899 pyedpro-3.3.5/pedlib/plugins/
+-rw-r--r--   0 peterglen  (1000) users      (100)      178 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/plugins/__init__.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     1603 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/plugins/lower_right.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     1836 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/stack.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     8371 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/test.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     7649 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pedlib/testdiff.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     3126 2023-09-26 04:15:19.000000 pyedpro-3.3.5/pedlib/webwin.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-10 06:50:43.549899 pyedpro-3.3.5/pycommon/
+-rw-r--r--   0 peterglen  (1000) users      (100)        0 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pycommon/__init__.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     7562 2024-03-19 05:08:14.000000 pyedpro-3.3.5/pycommon/browsewin.py
+-rw-r--r--   0 peterglen  (1000) users      (100)    10064 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pycommon/htmledit.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     8979 2024-03-19 05:08:15.000000 pyedpro-3.3.5/pycommon/icons.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    22092 2024-03-19 07:03:04.000000 pyedpro-3.3.5/pycommon/pgbox.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     6859 2024-03-19 05:05:47.000000 pyedpro-3.3.5/pycommon/pgbutt.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     4932 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pycommon/pgentry.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    40543 2024-03-19 07:03:02.000000 pyedpro-3.3.5/pycommon/pggui.py
+-rw-r--r--   0 peterglen  (1000) users      (100)    15446 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pycommon/pgsimp.py
+-rw-r--r--   0 peterglen  (1000) users      (100)    29354 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pycommon/pgtextview.py
+-rw-r--r--   0 peterglen  (1000) users      (100)    31741 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pycommon/pgutils.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    25822 2024-03-19 00:51:37.000000 pyedpro-3.3.5/pycommon/pgwkit.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     1017 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pycommon/plug.py
+-rw-r--r--   0 peterglen  (1000) users      (100)    16446 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pycommon/pypacker.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     9158 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pycommon/sutil.py
+-rwxr-xr-x   0 peterglen  (1000) users      (100)     2800 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pycommon/testbutt.py
+-rwxr-xr-x   0 peterglen  (1000) users      (100)     3222 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pycommon/testnums.py
+-rwxr-xr-x   0 peterglen  (1000) users      (100)     2530 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pycommon/testpacker.py
+-rwxr-xr-x   0 peterglen  (1000) users      (100)     1202 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pycommon/testpacker2.py
+-rwxr-xr-x   0 peterglen  (1000) users      (100)     1102 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pycommon/testpacker3.py
+-rwxr-xr-x   0 peterglen  (1000) users      (100)      606 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pycommon/testpacker4.py
+-rwxr-xr-x   0 peterglen  (1000) users      (100)     4058 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pycommon/testroot.py
+-rwxr-xr-x   0 peterglen  (1000) users      (100)     2401 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pycommon/testsimple.py
+-rwxr-xr-x   0 peterglen  (1000) users      (100)     7193 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pycommon/testtextv.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1297 2024-03-31 04:58:18.000000 pyedpro-3.3.5/pyedpro.desktop
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-10 06:50:43.553899 pyedpro-3.3.5/pyedpro.egg-info/
+-rw-r--r--   0 peterglen  (1000) users      (100)    11519 2024-04-10 06:50:43.000000 pyedpro-3.3.5/pyedpro.egg-info/PKG-INFO
+-rw-rw-r--   0 peterglen  (1000) users      (100)     3510 2024-04-10 06:50:43.000000 pyedpro-3.3.5/pyedpro.egg-info/SOURCES.txt
+-rw-rw-r--   0 peterglen  (1000) users      (100)        1 2024-04-10 06:50:43.000000 pyedpro-3.3.5/pyedpro.egg-info/dependency_links.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)       74 2024-04-10 06:50:43.000000 pyedpro-3.3.5/pyedpro.egg-info/entry_points.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)       18 2024-04-10 06:50:43.000000 pyedpro-3.3.5/pyedpro.egg-info/requires.txt
+-rw-rw-r--   0 peterglen  (1000) users      (100)       24 2024-04-10 06:50:43.000000 pyedpro-3.3.5/pyedpro.egg-info/top_level.txt
+-rwxrwxr-x   0 peterglen  (1000) users      (100)    14664 2024-04-10 06:01:05.000000 pyedpro-3.3.5/pyedpro.py
+-rw-r--r--   0 peterglen  (1000) users      (100)      106 2023-09-14 20:07:28.000000 pyedpro-3.3.5/pyproject.toml
+-rw-r--r--   0 peterglen  (1000) users      (100)       38 2024-04-10 06:50:43.553899 pyedpro-3.3.5/setup.cfg
+-rw-rw-r--   0 peterglen  (1000) users      (100)     3386 2024-04-10 06:50:35.000000 pyedpro-3.3.5/setup.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-10 06:50:43.553899 pyedpro-3.3.5/tests/
+-rwxr-xr-x   0 peterglen  (1000) users      (100)     5668 2023-09-14 20:07:28.000000 pyedpro-3.3.5/tests/testapp.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     1588 2024-03-30 17:43:54.000000 pyedpro-3.3.5/tests/testbutt.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)      310 2024-03-30 17:42:27.000000 pyedpro-3.3.5/tests/testgi.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)      199 2024-03-30 17:31:48.000000 pyedpro-3.3.5/tests/testimport.py
+-rwxr-xr-x   0 peterglen  (1000) users      (100)      515 2023-09-14 20:07:28.000000 pyedpro-3.3.5/tests/testkeys.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     5394 2024-03-30 17:41:49.000000 pyedpro-3.3.5/tests/testmenu.py
+-rwxr-xr-x   0 peterglen  (1000) users      (100)     3434 2023-09-14 20:07:28.000000 pyedpro-3.3.5/tests/testnb.py
```

### Comparing `pyedpro-3.3.1/LICENSE` & `pyedpro-3.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/PKG-INFO` & `pyedpro-3.3.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyedpro
-Version: 3.3.1
+Version: 3.3.5
 Summary: High power editor in python.
 Home-page: https://github.com/pglen/pyedpro
 Author: Peter Glen
 Author-email: peterglen99@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,80 +19,99 @@
 ## Python editor.
 
    Welcome to PyEdPro. This is modern multi-platform editor. Simple, powerful,
 configurable, extendable. Goodies like macro recording / playback, spell check,
 column select, multiple clipboards, unlimited undo ... makes it an editor
 that I use every day.
 
-  This project's source is at - https://github.com/pglen/pyedpro
-
   Working and tested platforms currently are:
 
         Win 7 .. Win 10 ...
         Centos 6 .. 7 Ubuntu 14 ... 16 ...  20.x (should run on any linux )
         Windows (Native) plus MSYS2, Mingw,
         Raspberry PI 3, Raspberry PI 4, ...
         Mac ** Some functions are disabled - in particular async processing
 
-Pyedpro functions near identical on Linux / Windows / Mac / Raspberry PI
+Pyedpro functions in a near identical manner
+    on Linux / Windows / Mac / Raspberry PI
 
  Pyedpro has:
 
-            o  macro recording/play,
-            o  search/replace,
-            o  functional navigation,
-            o  comment/string spell check,
-            o  full spell check, spell suggestion dialog
-            o  auto backup,
-            o  persistent undo/redo,  (undo beyond last save)
-            o  auto complete, auto correct,
+            o  Macro recording/play,
+            o  Search/replace,
+            o  Functional navigation,
+            o  Fomment/string spell check,
+            o  Full spell check, spell suggestion dialog
+            o  Auto backup,
+            o  Persistent undo/redo,  (undo beyond last save)
+            o  Auto complete, auto correct
             o
             o  ... and a lot more.
 
  It is fast, it is extendable. The editor has a table driven key mapping.
  One can easily edit the key map in keyhand.py, and the key actions
  in acthand.py The default key map resembles gedit / wed / etp / brief
 
+ The editor can be run from pip; from single packed executable; from git
+directory, and from packaged appimage.
+
+ The images are available from the git largefile subsystem.
+
 [See Doxygen generated Documentation on GitHub Pages](https://pglen.github.io/pyedpro/html/)
 
 ### Platforms
 
   I mainly run it on Ubuntu, and in Win32 / MSYS2, some Fedora, Windows 10,
-and the Raspberry-Pi. It behaves consistently on all these platforms,
+(x64) and the Raspberry-Pi. It behaves consistently on all these platforms,
 it is an absolute joy to edit in a different platform without the learning
-curve of new keystrokes.  If you want an editor  that works the same way in
+curve of new keystrokes.  If you want an editor that works the same way in
 all your workspaces, PyEdPro is the one.
 
- PyEdPro now is working good on the Mac. I installed homebrew, and got it to fire up. It
-was not a trivial exercise, as the Mac PygGOject did not do half of the stuff as the
-Linux version did. No asynchronous  anything, segmentation faults everywhere. (which python
+ PyEdPro now is working OK on the Mac M1. I installed homebrew, and got
+it to fire up. It was not a trivial exercise, as the Mac PygGOject did not do
+half of the stuff as the Linux version did.
+No asynchronous  anything, segmentation faults everywhere. (which python
 is not suppose to have)
+
   The font rendering was messed up, but I got fixed by replacing Pango's
 get_pixel_size() with get_size() / PANGO_UNIT. [Suspect int vs float accuracy issues]
   Some async functions like the function updater is disabled, but it can be done
 manually. (right click on doc -> rescan) All in all the Mac's PyGobject is not a great
 subsystem, hopefully time will be kind here.
 
 ** tried the M1 ... Sun 03.Apr.2022 most of it worked; no async processing
-as Glib the timer functions bombed. Great hardware - bad PyGobject support. However
-if an editor with familiar key op is needed -- most of it works with no destructive errors.
+as in Glib the timer functions bombed. Great hardware - bad PyGobject support. However
+if an editor with familiar key op is needed -- most of it works. And no
+destructive errors.
 
-### New:
+### History:
 
     (this is extracted, use git log for up-to-date information)
 
+    Sat 11.Feb.2023 -- Pyedpro Notes export / import and the new pydbase data base
+    Thu 27.Oct.2022 -- Restored system menu processing (Alt-f [File Menu] and such)
     Sat 10.Sep.2022 -- the system shortcuts (ctrl-s ctrl-o) are re-done by hand
-    Sat 03.Sep.2022 -- pubilshed on pip
+    Sat 03.Sep.2022 -- published on pip
     Thu 21.Apr.2022 -- release issued
     Wed 16.Mar.2022 -- dialog for read only file, export notes ... lots of other stuff
     Wed 01.Dec.2021 -- on search, descending one dir level with Ext. Search
     Sun 05.Sep.2021 -- made it function on the Mac M1 laptop  - !@#$$%
+        ....        -- lot of changes, see github log
+
+
+### New:
+
+    3.3.1   Fri 15.Mar.2024 -- corrected for changes in the public pydbase interface
+    3.3.5   Wed 10.Apr.2024 -- Relocated search window for better screen allocation
 
 Partial list, some highlights;
 
+Added separate interpretation for right control keys, so exotic items
+like 'insert html comment' can be tied to a shortcut key;
+
 Added drag / drop source / target. New keystroke combo for keyboards
  without home / pgup etc ... Implemented html preview. Just right click on
 the file body, an select the corresponding menu item.
 
 Implemented markdown preview. Right click ... menu
 Implemented M4 preview. The files are pulled in from the current directory (of the macro),
 and expanded with the m4 macro processor. The results than are previewed
@@ -150,17 +169,17 @@
  Any (fixed) font can be configured. No arrangements in the program for variable pitch fonts.
 
   See KEYS file for the list of keyboard shortcuts or press F1 in the
 editor or look at the file in pyedlib/KEYS. This file is also called up when the main menu
  Help -> 'KeyHelp In Doc' is called up.
 
   If you highlight a word, and press F2, Zeal will open with the item searched and
-highlighted. Shift F2 will do the same with Devhelp. This is what I use to see the API of PyGobj.
-F1 will call up the PyEdPro's help screen. Shift-F1 will open DevDocs. Naturally,
-Devdocs/Devhelp/Zeal need to be installed for these to function.
+highlighted. Shift F2 will do the same with Devhelp. This is what I use to see the
+ API of PyGobj. F1 will call up the PyEdPro's help screen. Shift-F1 will open
+DevDocs. Naturally, Devdocs/Devhelp/Zeal need to be installed for these to function.
 
   On initial start, PyEdPro shows a left pane and a top pane. The left pane
 is for function summary and the top pane is for double view of the same file.
 (to see the caller and the called [function] at once) These panes can be hidden with
 the mouse by dragging on their handle, or by the key combination Alt-Q (Shift-Alt-Q for
 the left pane) The first file window's settings are saved for the next startup.
 
@@ -213,32 +232,33 @@
 
 Screen from Mac:
 
 ![Screen Shot](screen_shot_mac.png)
 
 ## Project stats:
 
-        Project name
-            PyEdPro
-        Generated
-            2022-04-21 13:40:49 (in 3 seconds)
-        Generator
-            GitStats (version 55c5c28), git version 2.32.0, gnuplot 5.4 patchlevel 1
-        Report Period
-            2018-09-16 00:29:10 to 2022-04-15 10:31:49
-        Age
-            1308 days, 166 active days (12.69%)
-        Total Files
-            220
-        Total Lines of Code
-            476774 (1454450 added, 977676 removed)
-        Total Commits
-            347 (average 2.1 commits per active day, 0.3 per all days)
-        Authors
-            7 (average 49.6 commits per author)
-
+    Project name
+        pgpygtk
+    Generated
+        2024-04-10 02:22:26 (in 61 seconds)
+    Generator
+        GitStats (version 55c5c28), git version 2.34.1, gnuplot 5.4 patchlevel 2
+    Report Period
+        2018-09-16 00:29:10 to 2024-04-10 02:10:24
+    Age
+        2034 days, 224 active days (11.01%)
+    Total Files
+        13122
+    Total Lines of Code
+        2412587 (7146598 added, 4734011 removed)
+    Total Commits
+        756 (average 3.4 commits per active day, 0.4 per all days)
+    Authors
+        7 (average 108.0 commits per author)
 
 ![Stats](commits_by_year_month.png)
 
-License:    Open Source, FreeWare
+## License:
+
+    Open Source, FreeWare, Unlicence, MIT at your convenience
 
 // EOF
```

### Comparing `pyedpro-3.3.1/README.md` & `pyedpro-3.3.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,80 +3,99 @@
 ## Python editor.
 
    Welcome to PyEdPro. This is modern multi-platform editor. Simple, powerful,
 configurable, extendable. Goodies like macro recording / playback, spell check,
 column select, multiple clipboards, unlimited undo ... makes it an editor
 that I use every day.
 
-  This project's source is at - https://github.com/pglen/pyedpro
-
   Working and tested platforms currently are:
 
         Win 7 .. Win 10 ...
         Centos 6 .. 7 Ubuntu 14 ... 16 ...  20.x (should run on any linux )
         Windows (Native) plus MSYS2, Mingw,
         Raspberry PI 3, Raspberry PI 4, ...
         Mac ** Some functions are disabled - in particular async processing
 
-Pyedpro functions near identical on Linux / Windows / Mac / Raspberry PI
+Pyedpro functions in a near identical manner
+    on Linux / Windows / Mac / Raspberry PI
 
  Pyedpro has:
 
-            o  macro recording/play,
-            o  search/replace,
-            o  functional navigation,
-            o  comment/string spell check,
-            o  full spell check, spell suggestion dialog
-            o  auto backup,
-            o  persistent undo/redo,  (undo beyond last save)
-            o  auto complete, auto correct,
+            o  Macro recording/play,
+            o  Search/replace,
+            o  Functional navigation,
+            o  Fomment/string spell check,
+            o  Full spell check, spell suggestion dialog
+            o  Auto backup,
+            o  Persistent undo/redo,  (undo beyond last save)
+            o  Auto complete, auto correct
             o
             o  ... and a lot more.
 
  It is fast, it is extendable. The editor has a table driven key mapping.
  One can easily edit the key map in keyhand.py, and the key actions
  in acthand.py The default key map resembles gedit / wed / etp / brief
 
+ The editor can be run from pip; from single packed executable; from git
+directory, and from packaged appimage.
+
+ The images are available from the git largefile subsystem.
+
 [See Doxygen generated Documentation on GitHub Pages](https://pglen.github.io/pyedpro/html/)
 
 ### Platforms
 
   I mainly run it on Ubuntu, and in Win32 / MSYS2, some Fedora, Windows 10,
-and the Raspberry-Pi. It behaves consistently on all these platforms,
+(x64) and the Raspberry-Pi. It behaves consistently on all these platforms,
 it is an absolute joy to edit in a different platform without the learning
-curve of new keystrokes.  If you want an editor  that works the same way in
+curve of new keystrokes.  If you want an editor that works the same way in
 all your workspaces, PyEdPro is the one.
 
- PyEdPro now is working good on the Mac. I installed homebrew, and got it to fire up. It
-was not a trivial exercise, as the Mac PygGOject did not do half of the stuff as the
-Linux version did. No asynchronous  anything, segmentation faults everywhere. (which python
+ PyEdPro now is working OK on the Mac M1. I installed homebrew, and got
+it to fire up. It was not a trivial exercise, as the Mac PygGOject did not do
+half of the stuff as the Linux version did.
+No asynchronous  anything, segmentation faults everywhere. (which python
 is not suppose to have)
+
   The font rendering was messed up, but I got fixed by replacing Pango's
 get_pixel_size() with get_size() / PANGO_UNIT. [Suspect int vs float accuracy issues]
   Some async functions like the function updater is disabled, but it can be done
 manually. (right click on doc -> rescan) All in all the Mac's PyGobject is not a great
 subsystem, hopefully time will be kind here.
 
 ** tried the M1 ... Sun 03.Apr.2022 most of it worked; no async processing
-as Glib the timer functions bombed. Great hardware - bad PyGobject support. However
-if an editor with familiar key op is needed -- most of it works with no destructive errors.
+as in Glib the timer functions bombed. Great hardware - bad PyGobject support. However
+if an editor with familiar key op is needed -- most of it works. And no
+destructive errors.
 
-### New:
+### History:
 
     (this is extracted, use git log for up-to-date information)
 
+    Sat 11.Feb.2023 -- Pyedpro Notes export / import and the new pydbase data base
+    Thu 27.Oct.2022 -- Restored system menu processing (Alt-f [File Menu] and such)
     Sat 10.Sep.2022 -- the system shortcuts (ctrl-s ctrl-o) are re-done by hand
-    Sat 03.Sep.2022 -- pubilshed on pip
+    Sat 03.Sep.2022 -- published on pip
     Thu 21.Apr.2022 -- release issued
     Wed 16.Mar.2022 -- dialog for read only file, export notes ... lots of other stuff
     Wed 01.Dec.2021 -- on search, descending one dir level with Ext. Search
     Sun 05.Sep.2021 -- made it function on the Mac M1 laptop  - !@#$$%
+        ....        -- lot of changes, see github log
+
+
+### New:
+
+    3.3.1   Fri 15.Mar.2024 -- corrected for changes in the public pydbase interface
+    3.3.5   Wed 10.Apr.2024 -- Relocated search window for better screen allocation
 
 Partial list, some highlights;
 
+Added separate interpretation for right control keys, so exotic items
+like 'insert html comment' can be tied to a shortcut key;
+
 Added drag / drop source / target. New keystroke combo for keyboards
  without home / pgup etc ... Implemented html preview. Just right click on
 the file body, an select the corresponding menu item.
 
 Implemented markdown preview. Right click ... menu
 Implemented M4 preview. The files are pulled in from the current directory (of the macro),
 and expanded with the m4 macro processor. The results than are previewed
@@ -134,17 +153,17 @@
  Any (fixed) font can be configured. No arrangements in the program for variable pitch fonts.
 
   See KEYS file for the list of keyboard shortcuts or press F1 in the
 editor or look at the file in pyedlib/KEYS. This file is also called up when the main menu
  Help -> 'KeyHelp In Doc' is called up.
 
   If you highlight a word, and press F2, Zeal will open with the item searched and
-highlighted. Shift F2 will do the same with Devhelp. This is what I use to see the API of PyGobj.
-F1 will call up the PyEdPro's help screen. Shift-F1 will open DevDocs. Naturally,
-Devdocs/Devhelp/Zeal need to be installed for these to function.
+highlighted. Shift F2 will do the same with Devhelp. This is what I use to see the
+ API of PyGobj. F1 will call up the PyEdPro's help screen. Shift-F1 will open
+DevDocs. Naturally, Devdocs/Devhelp/Zeal need to be installed for these to function.
 
   On initial start, PyEdPro shows a left pane and a top pane. The left pane
 is for function summary and the top pane is for double view of the same file.
 (to see the caller and the called [function] at once) These panes can be hidden with
 the mouse by dragging on their handle, or by the key combination Alt-Q (Shift-Alt-Q for
 the left pane) The first file window's settings are saved for the next startup.
 
@@ -197,32 +216,33 @@
 
 Screen from Mac:
 
 ![Screen Shot](screen_shot_mac.png)
 
 ## Project stats:
 
-        Project name
-            PyEdPro
-        Generated
-            2022-04-21 13:40:49 (in 3 seconds)
-        Generator
-            GitStats (version 55c5c28), git version 2.32.0, gnuplot 5.4 patchlevel 1
-        Report Period
-            2018-09-16 00:29:10 to 2022-04-15 10:31:49
-        Age
-            1308 days, 166 active days (12.69%)
-        Total Files
-            220
-        Total Lines of Code
-            476774 (1454450 added, 977676 removed)
-        Total Commits
-            347 (average 2.1 commits per active day, 0.3 per all days)
-        Authors
-            7 (average 49.6 commits per author)
-
+    Project name
+        pgpygtk
+    Generated
+        2024-04-10 02:22:26 (in 61 seconds)
+    Generator
+        GitStats (version 55c5c28), git version 2.34.1, gnuplot 5.4 patchlevel 2
+    Report Period
+        2018-09-16 00:29:10 to 2024-04-10 02:10:24
+    Age
+        2034 days, 224 active days (11.01%)
+    Total Files
+        13122
+    Total Lines of Code
+        2412587 (7146598 added, 4734011 removed)
+    Total Commits
+        756 (average 3.4 commits per active day, 0.4 per all days)
+    Authors
+        7 (average 108.0 commits per author)
 
 ![Stats](commits_by_year_month.png)
 
-License:    Open Source, FreeWare
+## License:
+
+    Open Source, FreeWare, Unlicence, MIT at your convenience
 
-// EOF
+// EOF
```

### Comparing `pyedpro-3.3.1/panglib/lexer.py` & `pyedpro-3.3.5/panglib/lexer.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/panglib/pangdisp.py` & `pyedpro-3.3.5/panglib/pangdisp.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/panglib/pangfunc.py` & `pyedpro-3.3.5/panglib/pangfunc.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/panglib/parser.py` & `pyedpro-3.3.5/panglib/parser.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/panglib/stack.py` & `pyedpro-3.3.5/panglib/stack.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/panglib/utils.py` & `pyedpro-3.3.5/panglib/utils.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pangview.py` & `pyedpro-3.3.5/pangview.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/acthand.py` & `pyedpro-3.3.5/pedlib/acthand.py`

 * *Files 1% similar despite different names*

```diff
@@ -678,16 +678,44 @@
             self2.invalidate()
         pass
 
     def ctrl_alt_b(self, self2):
         if pedconfig.conf.pgdebug > 9:
             print ("CTRL - ALT - B")
 
-        #pedbuffs.buffers(self, self2)
-        self2.mained.update_statusbar("C-A-B key pressed.")
+        #line = ""; xidx = 0; yidx = 0
+        # No selection, assume word
+        if self2.xsel == -1 or self2.ysel == -1:
+            xidx = self2.caret[0] + self2.xpos
+            yidx = self2.caret[1] + self2.ypos
+            line = self2.text[yidx]
+            #cntb, cnte = selword(line, xidx)
+            cntb, cnte = selasci2(line, xidx, "_-")
+        else:
+            # Normalize
+            xssel = min(self2.xsel, self2.xsel2)
+            xesel = max(self2.xsel, self2.xsel2)
+            yssel = min(self2.ysel, self2.ysel2)
+            yesel = max(self2.ysel, self2.ysel2)
+
+            xidx = xssel; yidx = yssel;
+            line = self2.text[yidx]
+            cntb = xssel; cnte = xesel
+
+        if cnte == cntb:
+            self2.mained.update_statusbar("Please nav to a word first.")
+            return
+
+        self2.undoarr.append((xidx, yidx, pedundo.MODIFIED, line))
+        #print ("word / selection", line[cntb:cnte])
+
+        wlow = line[cntb].upper()
+
+        self2.text[yidx] = line[:cntb] + wlow + line[cntb+1:]
+        self2.inval_line()
 
     #// Comment out code: TODO
     def ctrl_alt_c(self, self2):
         if pedconfig.conf.pgdebug > 9:
             print ("CTRL - ALT - C")
 
         extx = os.path.splitext(self2.fname)[1]
```

### Comparing `pyedpro-3.3.1/pedlib/data/KEYS` & `pyedpro-3.3.5/pedlib/data/KEYS`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/data/KEYS.TXT` & `pyedpro-3.3.5/pedlib/data/KEYS.TXT`

 * *Files 1% similar despite different names*

```diff
@@ -154,14 +154,15 @@
     Alt D                       -- Delete current line
     Alt E                       -- Show edit Menu
     Alt F                       -- Show File Menu
     Alt G                       -- Goto line dialog
     Alt H                       -- Help Menu
     Alt I                       -- Ignore (convert) tabs to spaces
     Alt J                       -- Jump to next long line (80+)
+    Alt H                       -- Show Help menu
     Alt K                       -- Delete (kill) till end of line
     Alt L                       -- Select current line
     Alt M                       -- Macros menu
     Alt N                       -- Next search result
     Alt O                       -- Open file (Simplified Dialog)
     Alt P                       -- Previous search result
     Alt Q                       -- Hide top Pane
@@ -183,15 +184,15 @@
     Alt 4                       -- Switch to buffer 4
     Alt 5                       -- Switch to buffer 5
     Alt 6                       -- Switch to buffer 6
     Alt 7                       -- Switch to buffer 7
     Alt 8                       -- Switch to buffer 8
     Alt 9                       -- Switch to buffer 9
 
-    Alt F1                      -- Gnome (system) - Menu
+    Alt F1                      -- Gnome - Menu (system menu)
     Alt F2                      -- Gnome - Run App
     Alt F4                      -- Gnome - Exit program (Use Alt X)
     Alt F7                      -- Gnome - Move window
     Alt F8                      -- Gnome - Re-size window
     Alt F9                      -- Gnome - Minimize window
     Alt F10                     -- Gnome - Full Screen window
 
@@ -202,22 +203,20 @@
     Ctrl Alt C                  -- Comment out line, and jump down below
     Ctrl Alt D                  -- Display terminal here
     Ctrl Alt E                  -- Execute last command
     Ctrl Alt Shift E            -- Execute last command, force prompt
     Ctrl Alt F                  -- Fill to column
     Ctrl Alt Shift F            -- Prompt for fill column
     Ctrl Alt G                  -- Go execute cycle.sh (shortcut for header cycle)
-
-    Ctrl Alt T                  -- Execute terminal here (most likely global)
-        ...
-
     Ctrl Alt H                  -- Find (alias)
     Ctrl Alt J                  -- Coloring
     Ctrl Alt K                  -- Hex view
+        ...
     Ctrl Alt R                  -- Read file (text to speech)
+    Ctrl Alt T                  -- Execute terminal here (most likely global)
 
     # More coming ... under construction
 
     #Ctrl Alt H                  -- Left Arrow
     Ctrl Alt V                   -- Save all buffers
 
     Super - A                    -- Save all buffers
```

### Comparing `pyedpro-3.3.1/pedlib/data/KEYS.old` & `pyedpro-3.3.5/pedlib/data/KEYS.old`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/data/PyGObject.txt` & `pyedpro-3.3.5/pedlib/data/PyGObject.txt`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/data/QHELP` & `pyedpro-3.3.5/pedlib/data/QHELP`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/data/spell.txt` & `pyedpro-3.3.5/pedlib/data/spell.txt`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/data/test.Makefile` & `pyedpro-3.3.5/pedlib/data/test.Makefile`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 #  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-#  FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+#  FOR A PARTICULAR PURPOSE AND NON INFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 #  COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 #  IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
 #  WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 all:
 	@echo "Type 'make help' for a list of targets"
```

### Comparing `pyedpro-3.3.1/pedlib/data/test.S` & `pyedpro-3.3.5/pedlib/data/test.S`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/data/test.c` & `pyedpro-3.3.5/pedlib/data/test.c`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/data/test.py` & `pyedpro-3.3.5/pedlib/data/test.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/images/gtk-logo-rgb.gif` & `pyedpro-3.3.5/pedlib/images/gtk-logo-rgb.gif`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/images/pedicon.png` & `pyedpro-3.3.5/pedlib/images/pedicon.png`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/images/pedicon.svg` & `pyedpro-3.3.5/pedlib/images/pedicon.svg`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/images/pyedpro.png` & `pyedpro-3.3.5/pedlib/images/pyedpro.png`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/images/pyedpro.svg` & `pyedpro-3.3.5/pedlib/images/pyedpro.svg`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/images/pyedpro_sub.png` & `pyedpro-3.3.5/pedlib/images/pyedpro_sub.png`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/images/rect3713-3.png` & `pyedpro-3.3.5/pedlib/images/rect3713-3.png`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/images/rect3713.png` & `pyedpro-3.3.5/pedlib/images/rect3713.png`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/keyhand.py` & `pyedpro-3.3.5/pedlib/keyhand.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 # Key Handler for the editor. Extracted to a separate module
 # for easy update. The key handler is table driven, so new key
 # assignments can be made with ease
 
-from __future__ import absolute_import
+#from __future__ import absolute_import
 
 import sys
 
 import gi
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk
 from gi.repository import Gdk
```

### Comparing `pyedpro-3.3.1/pedlib/keywords.py` & `pyedpro-3.3.5/pedlib/keywords.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/leven.py` & `pyedpro-3.3.5/pedlib/leven.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/lexer.py` & `pyedpro-3.3.5/pedlib/lexer.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/notesql.py` & `pyedpro-3.3.5/pedlib/notesql.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/parser.py` & `pyedpro-3.3.5/pedlib/parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,208 +1,208 @@
-#!/usr/bin/env python
-
-from __future__ import absolute_import
-from __future__ import print_function
-import sys, os, re
-
-# Our modules
-from . import stack, lexer
-
-''' 
-The parser needs several variables to operate. 
-  Quick summary of variables:
-     Token definitions, Lexer tokens, Parser functions,
-      Parser states, Parse state table.
-See pangparser.py for documentation and examples.
-'''
-
-# Quick into: The lexer creates a stack of tokens. The parser scans
-# the tokens, and walks the state machine for matches. If match 
-# is encountered, the parser calls the function in the state table, 
-# and / or changes state. Reduce is called after the state has been 
-# successfully digested. For more info see lex / yacc literature.
-
-_gl_cnt = 0
-def unique():             # create a unique temporary number
-    global _gl_cnt; _gl_cnt+= 10
-    return _gl_cnt
-
-# This variable controls the display of the default action.
-# The default action is executed when there is no rule for the 
-# expression. Mostly useful for debugging the grammar.
-
-_show_default_action = False
-
-# May be redefined, included here for required initial states:
-
-ANYSTATE    = [-2, "anystate"]
-REDUCE      = [-1, "reduce"]
-IGNORE      = [unique(), "ignore"]
-INIT        = [unique(), "init"]
-
-# ------------------------------------------------------------------------
-# This parser creates no error conditions. Bad for languages, good
-# for text parsing. Warnings can be generated by enabling the 
-# 'show_default' action. 
-# The parser is not fully recursive, so states need to be nested by 
-# hand. The flat parser is an advantage for text processing.
-
-class Parse():
-
-    def __init__(self, data, xstack, pvg = None):
-
-        self.fstack = stack.Stack()
-        self.fsm = INIT; self.contflag = 0
-        self.pvg = pvg
-        self.pardict = {}
-        
-        # Create parse dictionary:
-        for pt in parsetable:
-            if pt[0] != None:        
-                if pt[0][1] not in self.pardict:                    
-                    self.pardict[pt[0][1]] = dict()     # Add if new
-                dd = self.pardict[pt[0][1]]
-                if pt[2]:
-                    #print "pt2", pt[2]
-                    dd[ pt[2]] = pt[:]
-                else:
-                    self.add_class(dd, pt)                                                        
-            else:
-                for aa in pt[1]:
-                    if aa[1] not in self.pardict:                    
-                        self.pardict[aa[1]] = dict()  # Add if new            
-                    dd  = self.pardict[aa[1]]
-                    if pt[2]:
-                        #print "pt2", pt[2]
-                        dd[ pt[2] ] = pt[:]
-                    else:
-                        self.add_class(dd, pt)                                                        
-                                                                    
-        '''for sss in self.pardict.iterkeys():
-            print "Key:", sss
-            for cc in self.pardict[sss].iterkeys():
-                print "   Subkey:", cc
-                print self.pardict[sss][cc][2:]'''
-                
-        while True:
-            tt = xstack.get2()  # Gen Next token
-            if not tt: 
-                break
-            self.parse_item2(data, tt)
-        
-    def add_class(self, dd, pt):
-        for aa in pt[3]:
-            dd[ aa ] = pt[:]
-
-    # This is the new routine, dictionary driven
-    # About ten times as fast
-    
-    def parse_item2(self, data, tt): 
-    
-        #print "parse_item", data, tt[0], tt[1].start(), tt[1].end()
-        mmm = tt[1];
-        self.strx = data[mmm.start():mmm.end()]
-        #print "parser:", tt[0], "=", "'" + self.strx + "'"        
-        if self.pvg.show_state:
-            print("state:", self.fsm, "str:", "'" + self.strx + "' token:", tt[0])    
-        try:
-            curr = self.pardict[self.fsm[1]]
-        except:
-            print("no state on", tt[0], self.strx)        
-        try:
-            item = curr[tt[0][0]]
-        except:
-            if self.pvg.show_parse:
-                # show context
-                bbb = mmm.start() - 5;  eee = mmm.end()+ 5
-                cont = data[bbb:mmm.start()] + "'" +  self.strx + "'" + \
-                        data[mmm.end():eee]
-                
-                print("no key on", tt[0], cont)
-            return 
-            
-        #print "item:", item
-                
-        if item[4] != None:
-            item[4](self, tt, item) 
-      
-        if item[5] == REDUCE:     
-            # This is an actionless reduce ... rare
-            self.reduce(tt)
-
-        elif item[5] == IGNORE:
-            pass   
-        else: 
-            #print " Setting new state", pt[3], self.strx
-            self.fstack.push([self.fsm, self.contflag, tt, self.strx])                    
-            self.fsm = item[5]
-            self.contflag = item[6]            
-                
-    # This is the old routine
-    def parse_item(self, data, tt): 
-    
-        #print data, tt[0], tt[1].start(), tt[1].end()
-        mmm = tt[1];
-        self.strx = data[mmm.start():mmm.end()]
-       
-        #print "Scanning in state:", self.fsm,
-        #print  "for", tt[0][1] + "=\"" + self.strx + "\""
-        match = False
-
-        
-        # Scan parse table:            
-        for pt in parsetable:
-            statematch = 0; classmatch = False
-            
-            if pt[0] == None:
-                if self.fsm in pt[1]:
-                    statematch = 1                                 
-            elif pt[0][0] == self.fsm[0]:
-                   statematch = 1
-
-            if not statematch:
-                #print "Not in state: ", pt[0][0]
-                continue
-
-            # See if we have a class match
-            if pt[3] != None:                
-                if tt[0][0] in pt[3]:
-                    classmatch = True
-            
-            #print "tt[0][0]=", tt[0][0], "tt[0][1]=", tt[0][1], "pt[2]", pt[2]
-            if classmatch or tt[0][0] == pt[2]:
-                #print " matching table entry ", pt[0], pt[1]
-                match = True
-                if pt[4] != None:
-                    pt[4](self, tt, pt) 
-                
-                if pt[5] == REDUCE:     
-                    # This is an actionless reduce ... rare
-                    self.reduce(tt)
-
-                elif pt[5] == IGNORE:
-                    pass   
-                else: 
-                    #print " Setting new state", pt[3], self.strx
-                    self.fstack.push([self.fsm, self.contflag, tt, self.strx])                    
-                    self.fsm = pt[5]
-                    self.contflag = pt[6]            
-                # Done working, next token
-                break;
-
-        if not match:
-            if _show_default_action:
-                print(" default action on",  tt[0], "'" + self.strx + "'", \
-                "Pos:", mmm.start())
-
-    def popstate(self):
-        self.fsm, self.contflag, self.ttt, self.stry = self.fstack.pop()
-
-if __name__ == "__main__":
-    print("This module was not meant to operate as main.")
-
-# EOF
-
-
-
-
-
+#!/usr/bin/env python
+
+from __future__ import absolute_import
+from __future__ import print_function
+import sys, os, re
+
+# Our modules
+import stack, lexer
+
+'''
+The parser needs several variables to operate.
+  Quick summary of variables:
+     Token definitions, Lexer tokens, Parser functions,
+      Parser states, Parse state table.
+See pangparser.py for documentation and examples.
+'''
+
+# Quick into: The lexer creates a stack of tokens. The parser scans
+# the tokens, and walks the state machine for matches. If match
+# is encountered, the parser calls the function in the state table,
+# and / or changes state. Reduce is called after the state has been
+# successfully digested. For more info see lex / yacc literature.
+
+_gl_cnt = 0
+def unique():             # create a unique temporary number
+    global _gl_cnt; _gl_cnt+= 10
+    return _gl_cnt
+
+# This variable controls the display of the default action.
+# The default action is executed when there is no rule for the
+# expression. Mostly useful for debugging the grammar.
+
+_show_default_action = False
+
+# May be redefined, included here for required initial states:
+
+ANYSTATE    = [-2, "anystate"]
+REDUCE      = [-1, "reduce"]
+IGNORE      = [unique(), "ignore"]
+INIT        = [unique(), "init"]
+
+# ------------------------------------------------------------------------
+# This parser creates no error conditions. Bad for languages, good
+# for text parsing. Warnings can be generated by enabling the
+# 'show_default' action.
+# The parser is not fully recursive, so states need to be nested by
+# hand. The flat parser is an advantage for text processing.
+
+class Parse():
+
+    def __init__(self, data, xstack, pvg = None):
+
+        self.fstack = stack.Stack()
+        self.fsm = INIT; self.contflag = 0
+        self.pvg = pvg
+        self.pardict = {}
+
+        # Create parse dictionary:
+        for pt in parsetable:
+            if pt[0] != None:
+                if pt[0][1] not in self.pardict:
+                    self.pardict[pt[0][1]] = dict()     # Add if new
+                dd = self.pardict[pt[0][1]]
+                if pt[2]:
+                    #print "pt2", pt[2]
+                    dd[ pt[2]] = pt[:]
+                else:
+                    self.add_class(dd, pt)
+            else:
+                for aa in pt[1]:
+                    if aa[1] not in self.pardict:
+                        self.pardict[aa[1]] = dict()  # Add if new
+                    dd  = self.pardict[aa[1]]
+                    if pt[2]:
+                        #print "pt2", pt[2]
+                        dd[ pt[2] ] = pt[:]
+                    else:
+                        self.add_class(dd, pt)
+
+        '''for sss in self.pardict.iterkeys():
+            print "Key:", sss
+            for cc in self.pardict[sss].iterkeys():
+                print "   Subkey:", cc
+                print self.pardict[sss][cc][2:]'''
+
+        while True:
+            tt = xstack.get2()  # Gen Next token
+            if not tt:
+                break
+            self.parse_item2(data, tt)
+
+    def add_class(self, dd, pt):
+        for aa in pt[3]:
+            dd[ aa ] = pt[:]
+
+    # This is the new routine, dictionary driven
+    # About ten times as fast
+
+    def parse_item2(self, data, tt):
+
+        #print "parse_item", data, tt[0], tt[1].start(), tt[1].end()
+        mmm = tt[1];
+        self.strx = data[mmm.start():mmm.end()]
+        #print "parser:", tt[0], "=", "'" + self.strx + "'"
+        if self.pvg.show_state:
+            print("state:", self.fsm, "str:", "'" + self.strx + "' token:", tt[0])
+        try:
+            curr = self.pardict[self.fsm[1]]
+        except:
+            print("no state on", tt[0], self.strx)
+        try:
+            item = curr[tt[0][0]]
+        except:
+            if self.pvg.show_parse:
+                # show context
+                bbb = mmm.start() - 5;  eee = mmm.end()+ 5
+                cont = data[bbb:mmm.start()] + "'" +  self.strx + "'" + \
+                        data[mmm.end():eee]
+
+                print("no key on", tt[0], cont)
+            return
+
+        #print "item:", item
+
+        if item[4] != None:
+            item[4](self, tt, item)
+
+        if item[5] == REDUCE:
+            # This is an actionless reduce ... rare
+            self.reduce(tt)
+
+        elif item[5] == IGNORE:
+            pass
+        else:
+            #print " Setting new state", pt[3], self.strx
+            self.fstack.push([self.fsm, self.contflag, tt, self.strx])
+            self.fsm = item[5]
+            self.contflag = item[6]
+
+    # This is the old routine
+    def parse_item(self, data, tt):
+
+        #print data, tt[0], tt[1].start(), tt[1].end()
+        mmm = tt[1];
+        self.strx = data[mmm.start():mmm.end()]
+
+        #print "Scanning in state:", self.fsm,
+        #print  "for", tt[0][1] + "=\"" + self.strx + "\""
+        match = False
+
+
+        # Scan parse table:
+        for pt in parsetable:
+            statematch = 0; classmatch = False
+
+            if pt[0] == None:
+                if self.fsm in pt[1]:
+                    statematch = 1
+            elif pt[0][0] == self.fsm[0]:
+                   statematch = 1
+
+            if not statematch:
+                #print "Not in state: ", pt[0][0]
+                continue
+
+            # See if we have a class match
+            if pt[3] != None:
+                if tt[0][0] in pt[3]:
+                    classmatch = True
+
+            #print "tt[0][0]=", tt[0][0], "tt[0][1]=", tt[0][1], "pt[2]", pt[2]
+            if classmatch or tt[0][0] == pt[2]:
+                #print " matching table entry ", pt[0], pt[1]
+                match = True
+                if pt[4] != None:
+                    pt[4](self, tt, pt)
+
+                if pt[5] == REDUCE:
+                    # This is an actionless reduce ... rare
+                    self.reduce(tt)
+
+                elif pt[5] == IGNORE:
+                    pass
+                else:
+                    #print " Setting new state", pt[3], self.strx
+                    self.fstack.push([self.fsm, self.contflag, tt, self.strx])
+                    self.fsm = pt[5]
+                    self.contflag = pt[6]
+                # Done working, next token
+                break;
+
+        if not match:
+            if _show_default_action:
+                print(" default action on",  tt[0], "'" + self.strx + "'", \
+                "Pos:", mmm.start())
+
+    def popstate(self):
+        self.fsm, self.contflag, self.ttt, self.stry = self.fstack.pop()
+
+if __name__ == "__main__":
+    print("This module was not meant to operate as main.")
+
+# EOF
+
+
+
+
+
```

### Comparing `pyedpro-3.3.1/pedlib/pedbuffs.py` & `pyedpro-3.3.5/pedlib/pedbuffs.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 # Action Handler for buffers
 
 from __future__ import absolute_import
 from __future__ import print_function
 
 import re, string, sys
 
-import gi
+#import gi
 #from six.moves import range
-gi.require_version("Gtk", "3.0")
-from gi.repository import Gdk
-from gi.repository import Gtk
-from gi.repository import GObject
+#gi.require_version("Gtk", "3.0")
+#from gi.repository import Gdk
+#from gi.repository import Gtk
+#from gi.repository import GObject
 
 from pedlib import pedconfig
 from pedlib.pedutil import *
 
 def fill_list(dialog):
 
     blist = []; was = -1
```

### Comparing `pyedpro-3.3.1/pedlib/pedcal.py` & `pyedpro-3.3.5/pedlib/pedcal.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/pedcanv.py` & `pyedpro-3.3.5/pedlib/pedcanv.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/pedcolor.py` & `pyedpro-3.3.5/pedlib/pedcolor.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/pedconfig.py` & `pyedpro-3.3.5/pedlib/pedconfig.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/peddlg.py` & `pyedpro-3.3.5/pedlib/peddlg.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/peddoc.py` & `pyedpro-3.3.5/pedlib/peddoc.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/peddoc_diff.py` & `pyedpro-3.3.5/pedlib/peddoc_diff.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/peddraw.py` & `pyedpro-3.3.5/pedlib/peddraw.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,37 +275,42 @@
             else: bgcol = self.rbgcolor
 
             while cnt <  self.xlen:
                 if cnt >= yssel and cnt <= yesel:
 
                     #line2 = self.text[cnt][self.xpos:]
                     line2 = self.text[cnt]
-                    line  = untab_str(line2)
 
                     xssel2 = calc_tabs(line2, xssel, self.tabstop)
                     xesel2 = calc_tabs(line2, xesel, self.tabstop)
+                    line  = untab_str(line2)
 
                     # adjust selection to tabs
                     if self.colsel:
                         frag = line[xssel2:xesel2]
                         draw_start = xssel2
                     else :   # Startsel - endsel
                         if cnt == yssel and cnt == yesel:   # sel on the same line
                             frag = line[xssel2:xesel2]
+                            draw_start = xssel2
                         elif cnt == yssel:                  # start line
+                            draw_start = xssel2
                             frag = line[xssel2:]
                         elif cnt == yesel:                  # end line
                             draw_start = 0
                             frag = line[:xesel2]
                         else:
                             draw_start = 0                  # intermediate line
                             frag = line[:]
 
-                    #dss = draw_start #-= self.xpos
-                    dss = calc_tabs(line2, draw_start, self.tabstop) - self.xpos
+                    dss = draw_start - self.xpos
+                    #dss2 = calc_tabs(line2, draw_start, self.tabstop)
+                                #(self.xpos % self.tabstop)
+                    #print(dss, dss2)
+
                     if dss < 0:
                           frag = frag[-dss:]
                           dss = 0
                     self._draw_text(gc, dss * self.cxx, yy, \
                                       frag, self.fgcolor, bgcol)
                 cnt = cnt + 1
                 yy += self.cyy
@@ -486,19 +491,25 @@
 
     def draw_spellerr(self, cr):
         cr.set_source_rgba(255, 0, 0)
         yyy = self.ypos + self.get_height() / self.cyy
         for xaa, ybb, lcc in self.ularr:
             # Draw within visible range
             if ybb >= self.ypos and ybb < yyy:
+                # Correct for tab
+                line = self.text[ybb]
+                #print("line:", line)
+                xaa -= self.xpos;
                 ybb -= self.ypos;
-                xaa -= self.xpos; lcc -= self.xpos;
+                lcc -= self.xpos
+                xaa2 = calc_tabs(line, xaa, self.tabstop)
+                lcc += xaa2 - xaa
+                xaa = xaa2
                 if xaa < 0:
                     xaa = 0
-
                 self.draw_wiggle(cr,
                      xaa * self.cxx, ybb * self.cyy + self.cyy,
                             lcc * self.cxx, ybb * self.cyy + self.cyy)
 
     # --------------------------------------------------------------------
     # Paint main text
```

### Comparing `pyedpro-3.3.1/pedlib/pedfind.py` & `pyedpro-3.3.5/pedlib/pedfind.py`

 * *Files 0% similar despite different names*

```diff
@@ -348,16 +348,18 @@
 
     if True or oldww == 0 or oldhh == 0 or oldxx  == 0 or oldyy == 0:
         # Position it out of the way
         sxx, syy = self2.mained.mywin.get_position()
         wxx, wyy = self2.mained.mywin.get_size()
         myww = 3 * wxx / 8; myhh = 3 * wyy / 8
         win2.set_default_size(myww, myhh)
-        win2.move(sxx + wxx - (myww  + self.xnum), \
-                            syy + wyy - (myhh + self.xnum))
+        #win2.move(sxx + wxx - (myww  + self.xnum), \
+        #                    syy + wyy - (myhh + self.xnum))
+        win2.move(sxx + wxx - (myww + 8 + self.xnum), \
+                            syy + 8 + self.xnum)
     else:
         # Restore old size / location
         win2.set_default_size(oldww, oldhh)
         #win2.move(oldxx + self.xnum, oldyy + self.xnum)
         win2.move(oldxx, oldyy)
 
     vbox = Gtk.VBox()
```

### Comparing `pyedpro-3.3.1/pedlib/pedfont.py` & `pyedpro-3.3.5/pedlib/pedfont.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/pedgoto.py` & `pyedpro-3.3.5/pedlib/pedgoto.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/pedlcmd.py` & `pyedpro-3.3.5/pedlib/pedlcmd.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/pedlog.py` & `pyedpro-3.3.5/pedlib/pedlog.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/pedmenu.py` & `pyedpro-3.3.5/pedlib/pedmenu.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/pedmisc.py` & `pyedpro-3.3.5/pedlib/pedmisc.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/pednotes.py` & `pyedpro-3.3.5/pedlib/pednotes.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,55 +1,89 @@
 #!/usr/bin/env python
 
 import signal, os, time, sys, subprocess, platform
 import ctypes, datetime, sqlite3, warnings, uuid, copy
 
-#from six.moves import range
-
 import gi; gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk, Gdk
 from gi.repository import GObject
 from gi.repository import GLib
 from gi.repository import Pango
 
+#print(sys.path)
+
+realinc = os.path.realpath(os.path.dirname(__file__) + os.sep + "../pycommon")
+if realinc not in sys.path:
+    sys.path.append(realinc)
+
+#print("import", __file__)
+
 from pedlib import pedconfig
 
 # Into our name space
-from    pedlib.pedmenu import *
-from    pedlib.pedui import *
-from    pedlib.pedutil import *
-from    pedlib.pedync import *
-from    pedlib.pedofd import *
-
-from pycommon.pggui import *
-from pycommon.pgsimp import *
-from pycommon.pgtextview import *
-from pycommon.pgbutt import *
+from pedlib.pedmenu import *
+from pedlib.pedui import *
+from pedlib.pedutil import *
+from pedlib.pedync import *
+from pedlib.pedofd import *
+
+#print(sys.path)
+
+from pycommon import pgsimp
+from pycommon import pggui
+from pycommon import pgbutt
+from pycommon import pgtextview
 
 try:
-    # This is a copy of the pydbase -- refresh when needed
-    #np = os.path.split(__file__)[0] + os.sep + '..' + os.sep + "pydbase"
-    #print(np)
-    #sys.path.append(np)
-    #from pydbase
-    import twinbase
-    #from pydbase
-    import twincore
+    #from pydbase import dbutils
+    #from pydbase import twinbase
+    from pydbase import twincore
+
+    #print("pednotes", sys.path)
+    #print(os.getcwd())
 except:
-    print("Cannot import twincore / twinbase", sys.exc_info())
+    try:
+        print("local")
+        # This will change once the pydbase is out of dev stage
+        np = os.path.split(__file__)[0] + os.sep + '..' + os.sep + ".." + os.sep + ".."
+        #print(np)
+        #np =  '..' + os.sep + "pydbase"
+        sys.path.append(np)
+        np += os.sep + "pydbase"
+        sys.path.append(np)
+
+        np =  os.path.split(__file__)[0] + os.sep + '..' + os.sep + "pydbase"
+        sys.path.append(np)
+
+        #print(sys.path[-3:])
+
+        from pydbase import dbutils
+        from pydbase import twinbase
+        from pydbase import twincore
+    except:
+        np = os.path.split(__file__)[0]
+        sys.path.append(np)
+        sys.path.append(np + os.sep + "..")
+        print("files2", os.listdir(np))
+        print("special2", sys.path)
+
+        import dbutils
+        import twinbase
+        import twincore
 
 # ------------------------------------------------------------------------
 
 class pgnotes(Gtk.VBox):
 
     def __init__(self):
 
         Gtk.VBox.__init__(self)
 
         self.wasin = False
+        self.old_iter = None
 
         #self.modify_bg(Gtk.StateType.NORMAL, Gdk.color_parse("#444444"))
         #self.prevsel = None;  self.prevkey = None;
 
         self.lastsel = None;  self.lastkey = None
         self.cnt = 0
         self.popwin = None
@@ -63,14 +97,16 @@
 
         if pedconfig.conf.verbose:
             print("Using notesdir:", self.notes_dir)
 
         try:
             self.core = twincore.TwinCore(self.notes_dir + os.sep + "peddata.pydb")
             #print("core", self.core, self.core.fname)
+            #self.core.pgdebug = 10
+
         except:
             print("Cannot make notes py database")
 
         #message("Cannot make notes database")
 
         #hbox = Gtk.HBox()
         #self.pack_start(Gtk.Label("s"), 0, 0, 0)
@@ -109,15 +145,15 @@
         frame3 = Gtk.Frame();
         frame3.add(scroll2)
         self.vpaned.add(frame3)
 
         self.vpaned.set_position(200)
 
         #self.edview = pgsimp.TextViewWin()
-        self.edview =  pgTextView()
+        self.edview =  pgtextview.pgTextView()
         #self.edview.callb = self.savetext
         self.edview.findcall = self.findx, self
 
         self.edview.textview.set_margin_left(2)
         self.edview.textview.set_margin_right(2)
         self.edview.textview.set_margin_top(2)
         self.edview.textview.set_margin_bottom(2)
@@ -136,69 +172,69 @@
         frame4.set_border_width(3)
         frame4.add(self.edview)
 
         self.vpaned.add(frame4)
         self.pack_start(self.vpaned, 1, 1, 0)
 
         hbox13 = Gtk.HBox()
-        hbox13.pack_start(zSpacer(), 1, 1, 0)
+        hbox13.pack_start(pgsimp.zSpacer(), 1, 1, 0)
 
-        hbox13.pack_start(zSpacer(), 0, 0, 0)
-        butt3 = smallbutt(" _New Item ", self.newitem, "Create new record")
+        hbox13.pack_start(pgsimp.zSpacer(), 0, 0, 0)
+        butt3 = pgbutt.smallbutt(" _New Item ", self.newitem, "Create new record")
         hbox13.pack_start(butt3, 0, 0, 0)
-        hbox13.pack_start(zSpacer(), 0, 0, 0)
+        hbox13.pack_start(pgsimp.zSpacer(), 0, 0, 0)
 
-        butt3x = smallbutt(" Find in Text ", self.findx, "Find in text")
+        butt3x = pgbutt.smallbutt(" Find in Text ", self.findx, "Find in text")
         hbox13.pack_start(butt3x, 0, 0, 0)
-        hbox13.pack_start(zSpacer(), 0, 0, 0)
+        hbox13.pack_start(pgsimp.zSpacer(), 0, 0, 0)
 
-        butt3a = smallbutt(" Search All ", self.searchall, "Search ALL data")
+        butt3a = pgbutt.smallbutt(" Search All ", self.searchall, "Search ALL data")
 
         hbox13.pack_start(butt3a, 0, 0, 0)
 
-        hbox13.pack_start(zSpacer(), 0, 0, 0)
-        hbox13.pack_start(zSpacer(), 1, 1, 0)
+        hbox13.pack_start(pgsimp.zSpacer(), 0, 0, 0)
+        hbox13.pack_start(pgsimp.zSpacer(), 1, 1, 0)
 
         hbox13a = Gtk.HBox()
-        hbox13a.pack_start(zSpacer(), 1, 1, 0)
+        hbox13a.pack_start(pgsimp.zSpacer(), 1, 1, 0)
 
-        hbox13a.pack_start(zSpacer(), 0, 0, 0)
-        butt11 = smallbutt(" Del Item ", self.delitem, "Delete item")
+        hbox13a.pack_start(pgsimp.zSpacer(), 0, 0, 0)
+        butt11 = pgbutt.smallbutt(" Del Item ", self.delitem, "Delete item")
         hbox13a.pack_start(butt11, 0, 0, 0)
-        hbox13a.pack_start(zSpacer(), 0, 0, 0)
+        hbox13a.pack_start(pgsimp.zSpacer(), 0, 0, 0)
 
-        butt12 = smallbutt(" Export ", self.export, "Export items")
+        butt12 = pgbutt.smallbutt(" Export ", self.export, "Export items")
         hbox13a.pack_start(butt12, 0, 0, 0)
 
-        hbox13a.pack_start(zSpacer(), 0, 0, 0)
+        hbox13a.pack_start(pgsimp.zSpacer(), 0, 0, 0)
 
-        butt12a = smallbutt(" Import ", self.importx, "Import items")
+        butt12a = pgbutt.smallbutt(" Import ", self.importx, "Import items")
         hbox13a.pack_start(butt12a, 0, 0, 0)
-        hbox13a.pack_start(zSpacer(), 0, 0, 0)
+        hbox13a.pack_start(pgsimp.zSpacer(), 0, 0, 0)
 
-        butt12b = smallbutt(" Popout ", self.popx, "Pop out window")
+        butt12b = pgbutt.smallbutt(" Popout ", self.popx, "Pop out window")
         hbox13a.pack_start(butt12b, 0, 0, 0)
-        hbox13a.pack_start(zSpacer(), 0, 0, 0)
+        hbox13a.pack_start(pgsimp.zSpacer(), 0, 0, 0)
 
-        hbox13a.pack_start(zSpacer(), 1, 1, 0)
+        hbox13a.pack_start(pgsimp.zSpacer(), 1, 1, 0)
 
         self.pack_start(hbox13, 0, 0, 0)
         self.pack_start(hbox13a, 0, 0, 0)
         pedconfig.conf.pedwin.mywin.connect("configure-event", self.resize)
         self.load()
 
     def resize(self, widg, newconf):
         #print("resize", newconf.width, newconf.height)
         self.vpaned.set_position(newconf.height / 6)
 
     def __del__(self):
         # Did not happen automatically
         #print("pednotes __del__")
         self.savetext()
-        self.core.__del__()
+        #del self.core
 
     def switched(self, pageto):
         #print("SW page signal web", pageto)
         if pageto == self:
             #print("Notes in")
             self.wasin = True
         else:
@@ -229,28 +265,45 @@
         ret = dlg.run()
         if ret != Gtk.ResponseType.OK:
             dlg.destroy()
             return
         txt = dlg.entry.get_text()
         dlg.destroy()
         self.treeview2.clear()
+        self.edview.set_text("")
         cnt = 0
         txt2 = txt.lower()
+        arrx = []
         try:
-            datax = self._getall()
-            for aa in datax:
-                ddd = self.core.retrieve(aa)
+            #datax = self._getall()
+            #for aa in datax:
+            dbsize = self.core.getdbsize()
+            for aa in range(dbsize-1, 0, -1):
+                #ddd = self.core.retrieve(aa)
+                #ddd = self.core.findrecpos(aa, 1)
+                ddd = self.core.get_rec(aa)
+                if not ddd:
+                    continue
                 #print(ddd)
-                for cc in ddd:
-                    for ee in cc:
-                        #print("ee", ee.lower())
-                        if txt2 in str(ee).lower():
-                            #print("    ", aa)
-                            self.treeview2.append((aa, "", ""))
-                            cnt += 1
+                if type(ddd[0]) != type(""):
+                    ddd[0] = ddd[0].decode()
+                if type(ddd[1]) != type(""):
+                    try:
+                        ddd[1] = ddd[1].decode()
+                    except:
+                        ddd[1] = ddd[1].decode("cp437")
+
+                sss = ddd[1].lower()
+                #print("sss", sss)
+                if txt2 in sss:
+                    print("found:", txt2, "in", ddd[0])
+                    if ddd[0] not in arrx:
+                        arrx.append(ddd[0])
+                        self.treeview2.append((ddd[0], "", ""))
+                    cnt += 1
             if not cnt:
                 self.treeview2.append(("No records found", "", ""))
 
             pass
         except:
             #print("exc in search ", sys.exc_info())
             put_exception("search all")
@@ -264,20 +317,27 @@
             dlg.destroy()
             return
         txt = dlg.entry.get_text()
         dlg.destroy()
         #print("Searching for:", txt)
 
         textbuffer  =  self.edview.textview.get_buffer()
-        start_iter  =  textbuffer.get_start_iter()
-        found       =  start_iter.forward_search(txt, Gtk.TextSearchFlags.CASE_INSENSITIVE, None)
+        if self.old_iter:
+            start_iter  =  self.old_iter
+        else:
+            start_iter  =  textbuffer.get_start_iter()
+        found  = start_iter.forward_search(txt, Gtk.TextSearchFlags.CASE_INSENSITIVE, None)
         if found:
-           match_start,match_end = found #add this line to get match_start and match_end#try:
-           textbuffer.select_range(match_start,match_end)#    datax = self.sql.getall()
+           match_start, match_end = found
+           self.old_iter = match_end
+           textbuffer.select_range(match_start, match_end)
            self.edview.textview.scroll_to_iter(match_start, 0, False, 0, 0)
+        else:
+            self.old_iter = None
+            message("\n'%s' not found or EOF reached. \n" % (txt))
 
     def newitem(self, arg):
         self.savetext()
         rrr = HeadDialog("New Item %d" % self.cnt, None)
         ret = rrr.run()
         if ret != Gtk.ResponseType.OK:
             rrr.destroy()
@@ -583,40 +643,54 @@
             self.savetext()
 
         self.lastsel = args
         self._readrec(args)
 
     def _readrec(self, args):
 
-        ddd = self.core.retrieve(args[0])
+        #print("readargs", args)
+        ddd = None
+        #ddd = self.core.retrieve(args[0])
+        for aa in range(self.core.getdbsize()-1, -1, -1):
+            rec = self.core.get_rec(aa)
+            if not rec:
+                continue
+            #print("rec", rec[0])
+            if rec[0].decode() == args[0]:
+                #print("found")
+                ddd = rec
+                break
+
+        #print("readrec", ddd)
+
         #for aa in ddd:
         #    print(aa)
         #print("ddd", type(ddd), ddd)
         #print(b"'" + ddd[0][1][:3]) + b"'"
 
         # See what kind it is
         try:
-            if ddd[0][1][:13] == b"GTKTEXTBUFFER":
+            if ddd[1][:13] == b"GTKTEXTBUFFER":
                 self.edview.set_text("")
                 #print("deser", ddd[0][1])
-                self.edview.deser_buff(ddd[0][1])
+                self.edview.deser_buff(ddd[1])
             else:
                 #print("load", ddd[0][1])
-                self.edview.set_text(ddd[0][1].decode())
+                self.edview.set_text(ddd[1].decode())
         except:
             print("treesel", sys.exc_info())
             pass
 
         self.edview.set_modified(0)
 
     def _getall(self):
         datax = []
         try:
             dbsize = self.core.getdbsize()
-            for aa in range(dbsize-1, 0, -1):
+            for aa in range(dbsize-1, -1, -1):
                 ddd = self.core.get_rec(aa)
                 if len(ddd) < 2:
                     continue        # Deleted record
                 #print("ddd", ddd)
                 #print("Item:", ddd[0], "Data:", ddd[1][:16] + b" ..." )
                 try:
                     ppp = ddd[0].split(b",")
@@ -672,16 +746,14 @@
                     if ccc > self.cnt:
                         self.cnt = ccc
                 except:
                     pass
         self.cnt += 1
         #print("self.cnt", self.cnt)
 
-
-
 class   PopWin(Gtk.Window):
 
     def __init__(self):
 
         Gtk.Window.__init__(self)
 
         #self.win2 = Gtk.Window()
@@ -698,15 +770,15 @@
         self.set_events(Gdk.EventMask.ALL_EVENTS_MASK )
 
         self.connect("key-press-event", self._area_key, self)
         self.connect("key-release-event", self._area_key, self)
         self.connect("destroy", self._area_destroy)
 
         #self.connect("focus-out-event", self._focus)
-        self.view = pgTextView(True)
+        self.view = pgtextview.pgTextView(True)
         #self.view.textview.set_editable(False)
 
         self.scroll = Gtk.ScrolledWindow();
         self.scroll.add(self.view)
         frame = Gtk.Frame(); frame.add(self.scroll)
         self.add(frame)
         self.show_all()
```

### Comparing `pyedpro-3.3.1/pedlib/pedobjs.py` & `pyedpro-3.3.5/pedlib/pedobjs.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/pedofd.py` & `pyedpro-3.3.5/pedlib/pedofd.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,14 +142,15 @@
                 res.append(xstr2)
             iter = xmodel.iter_next(iter)
             if not iter:
                 break
 
     #print ("response", response, "result", res  )
     dialog.destroy()
+    #del dialog
     return res
 
 def butt_this(butt, dialog):
     ttt = dialog.entry.get_text()
     #print("butt_this", ttt)
     if ttt:
         # Expand user var
```

### Comparing `pyedpro-3.3.1/pedlib/pedoline.py` & `pyedpro-3.3.5/pedlib/pedoline.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/pedplug.py` & `pyedpro-3.3.5/pedlib/pedplug.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import gi; gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk
 from gi.repository import Gdk
 from gi.repository import GLib
 from gi.repository import Gio
 
 from pedlib import pedconfig
-from pedlib import peddoc
+#from pedlib import peddoc
 from pedlib import pedync
 from pedlib import pedlog
 from pedlib import pedcal
 from pedlib import pednotes
 from pedlib import pedoline
 from pedlib import pedfont
 from pedlib import pedcolor
@@ -42,15 +42,19 @@
 from    pedlib.pedui import *
 from    pedlib.pedutil import *
 
 plugin_list = []
 
 def     load_plugins():
 
+    if not os.path.isdir(pedconfig.conf.plugins_dir):
+        os.mkdir(pedconfig.conf.plugins_dir)
+
     sys.path.append(pedconfig.conf.plugins_dir)
+
     for aa in os.listdir(pedconfig.conf.plugins_dir):
         if aa[-3:] == ".py":
             modname =  aa[:-3]
             if pedconfig.conf.verbose:
                 print("Loading user plugin:", modname);
             try:
                 ppp = importlib.import_module(modname)
```

### Comparing `pyedpro-3.3.1/pedlib/pedspell.py` & `pyedpro-3.3.5/pedlib/pedspell.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/pedsql.py` & `pyedpro-3.3.5/pedlib/pedsql.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/pedstruct.py` & `pyedpro-3.3.5/pedlib/pedstruct.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/pedtask.py` & `pyedpro-3.3.5/pedlib/pedtask.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,26 +153,28 @@
             return
         try:
             outs, errs = ret.communicate()
         except:
             print("Cannot communicate with MD filter %s" % str(comline), sys.exc_info())
             return
 
-        newfname = os.path.splitext(self.fname)[0] + ".html"
-        print("processed:", self.fname, newfname)
+        newfname = os.path.splitext(self.fname)[0] + ".preview.html"
+        #print("processed:", self.fname, newfname)
         with open(newfname,'wb') as fd:
             fd.write(outs)
 
         if not os.path.isfile(newfname):
             print("No conversion on %s" % self.fname)
             pedync.message("\n   Cannot convert '%s' \n"
                 "   to MD / HTML file\n\n"  % self.fname )
             return
 
         self.start_htmlwin(newfname)
+        pedconfig.conf.pedwin.cleanit.append(newfname)
+
 
     def start_browser(self, newfname):
         comline2 = ["firefox", newfname,]
         try:
             ret = subprocess.Popen(comline2)
         except:
             print("Cannot start browser %s" % str(comline2), sys.exc_info())
```

### Comparing `pyedpro-3.3.1/pedlib/pedtdlg.py` & `pyedpro-3.3.5/pedlib/pedtdlg.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/pedthread.py` & `pyedpro-3.3.5/pedlib/pedthread.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/pedtts.py` & `pyedpro-3.3.5/pedlib/pedtts.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/pedui.py` & `pyedpro-3.3.5/pedlib/pedui.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/pedundo.py` & `pyedpro-3.3.5/pedlib/pedundo.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/pedutil.py` & `pyedpro-3.3.5/pedlib/pedutil.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/pedweb.py` & `pyedpro-3.3.5/pedlib/pedweb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 #!/usr/bin/env python3
 
 from __future__ import absolute_import, print_function
 import signal, os, time, sys, subprocess, platform
 import ctypes, datetime, sqlite3, warnings
 
-import gi;
+#import gi;
+#from gi.repository import Gtk
+#from gi.repository import Gdk
+#from gi.repository import GObject
+#from gi.repository import GLib
 
-from gi.repository import Gtk
-from gi.repository import Gdk
-from gi.repository import GObject
-from gi.repository import GLib
-
-#    gi.require_version('WebKit2', '4.0')
+#gi.require_version('WebKit2', '4.0')
 
 from pedlib import pedconfig
 
 # Into our name space
 from    pedlib.pedmenu import *
 from    pedlib.pedui import *
 from    pedlib.pedutil import *
@@ -25,24 +24,29 @@
 from pycommon.pgbutt import *
 from pycommon.browsewin import *
 
 try:
     # This will change once the pydbase is out of dev stage
     np = os.path.split(__file__)[0] + os.sep + '..' + os.sep + ".." + os.sep + ".."
     #print(np)
-
     #np =  '..' + os.sep + "pydbase"
-
     sys.path.append(np)
+    np += os.sep + "pydbase"
+    sys.path.append(np)
+
     #print(sys.path)
     #print(os.getcwd())
-    #from pydbase
-    import twincore
+    from pydbase import twincore
 except:
-    put_exception("Cannot Load twincore")
+    np =  os.path.split(__file__)[0] + os.sep + '..' + os.sep + "pydbase"
+    sys.path.append(np)
+    print(sys.path[-3:])
+
+    from pydbase import twincore
+    #put_exception("Cannot Load twincore")
 
 # ------------------------------------------------------------------------
 
 class pgweb(Gtk.VBox):
 
     def __init__(self):
 
@@ -78,15 +82,15 @@
         #self.pack_start(pggui.xSpacer(), 0, 0, 0)
         self.lsel = pgsimp.LetterNumberSel(self.letterfilter, font="Mono 12")
         self.lsel.set_tooltip_text("Filter entries by letter / number")
         self.pack_start(self.lsel, 0, 0, 2)
 
         #self.modify_bg(Gtk.StateType.NORMAL, Gdk.color_parse("#dd8822"))
 
-        hbox3 = Gtk.HBox()
+        #hbox3 = Gtk.HBox()
         #hbox3.pack_start(Gtk.Label(""), 0, 0, 0)
         #hbox3.pack_start(pggui.xSpacer(4), 0, 0, 0)
         #hbox3.pack_start(Gtk.Label(""), 0, 0, 0)
         #self.edit = Gtk.Entry()
         #hbox3.pack_start(Gtk.Label(" Find: "), 0, 0, 0)
         #hbox3.pack_start(self.edit, 1, 1, 0)
         #butt2 = Gtk.Button.new_with_mnemonic("Find")
@@ -168,55 +172,55 @@
         butt5 = Gtk.Button("~")
         butt5.connect("pressed", self.anchor)
         butt5.set_tooltip_text("Goto local anchor page")
         hbox4.pack_start(Gtk.Label(" "), 0, 0, 0)
         hbox4.pack_start(butt5, 0, 0, 0)
 
         #hbox3.pack_start(Gtk.Label(" "), 0, 0, 0)
-
         #self.pack_start(hbox4, 0, 0, 2)
 
         self.treeview3 = SimpleTree(("Hour", "Subject", "Alarm", "Notes"))
         self.treeview3.setcallb(self.treesel)
 
-        scroll2 = Gtk.ScrolledWindow()
-        scroll2.add(self.treeview3)
-        frame3 = Gtk.Frame(); frame3.add(scroll2)
+        scroll2a = Gtk.ScrolledWindow()
+        scroll2a.add(self.treeview3)
+        frame3 = Gtk.Frame(); frame3.add(scroll2a)
         #self.pack_start(frame3, 1, 1, 2)
 
         #self.edview = SimpleEdit()
         #self.edview.setsavecb(self.savetext)
         #scroll3 = Gtk.ScrolledWindow()
         #scroll3.add(self.edview)
         #frame4 = Gtk.Frame(); frame4.add(scroll3)
 
         scrolled_window = Gtk.ScrolledWindow()
         try:
             #self.brow_win = WebKit2.WebView()
             #self.brow_win = pgwkit.pgwebw(self)
             self.brow_win = brow_win()
+            #self.brow_win = Gtk.Label("No WebView Available.")
             #print("dir", dir(self.brow_win))
             #self.brow_win.load_uri("file://" + self.fname)
+            pass
         except:
             #self.brow_win = Gtk.Label("No WebView Available.")
             put_exception("WebView load")
 
         vbox5 = Gtk.VBox()
         frame4 = Gtk.Frame();
         frame4.add(scrolled_window)
-        vbox5.pack_start(frame4, 1,1,0)
+        vbox5.pack_start(frame4, 1, 1, 0)
         vpaned.add(vbox5)
 
         #self.brow_win.override_background_color(
         #                Gtk.StateFlags.NORMAL, Gdk.RGBA(1, .5, .5) )
 
         #webview.load_uri("https://google.com")
         scrolled_window.add(self.brow_win)
-        self.pack_start(scrolled_window, 1, 1, 2)
-
+        #self.pack_start(scrolled_window, 1, 1, 2)
         #self.status = Gtk.Label(" Status: ")
         #self.pack_start(self.status, 0, 0, 2)
 
         hbox13 = Gtk.HBox()
         hbox13.pack_start(Gtk.Label(label=""), 1, 1, 0)
 
         #hbox13.pack_start(Gtk.Label(" | "), 0, 0, 0)
@@ -577,17 +581,30 @@
 
         #print("treesel", args[0])
 
         self.savetext()
         self.lastsel = args
 
         hhh = ""
+
         try:
-            ddd = self.core.retrieve(args[0])[0]
-            hhh = ddd[1].decode()
+            #ddd = self.core.retrieve(args[0])[0]
+            dbsize = self.core.getdbsize()
+            for aa in range(dbsize-1, 0, -1):
+                #ddd = self.core.retrieve(aa)
+                #ddd = self.core.findrecpos(aa, 1)
+                ddd = self.core.get_rec(aa)
+                if not ddd:
+                    continue
+                #print(ddd)
+                if ddd[0].decode() == args[0]:
+                    #print("found", ddd[0])
+                    #print(ddd[0], args[0])
+                    hhh = ddd[1].decode()
+                    break
         except:
             if pedconfig.conf.verbose:
                 put_exception("treesel")
             pass
 
         #print("Content", hhh)
```

### Comparing `pyedpro-3.3.1/pedlib/pedwin.py` & `pyedpro-3.3.5/pedlib/pedwin.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 from pedlib import pedcolor
 from pedlib import pedfind
 from pedlib import pedweb
 from pedlib import peddlg
 from pedlib import pedthread
 from pedlib import pedspell
 from pedlib import pedofd
+#from pedlib import pedplug
 #from pedlib import pedutil
 
 #sys.path.append('..' + os.sep + "pycommon")
 
 from pycommon.pggui import *
 from pycommon.pgsimp import *
 from pycommon.pgbutt import *
@@ -402,14 +403,15 @@
         #self.mywin.connect("event", self.area_event)
         #self.mywin.connect("enter-notify-event", self.area_enter)
         #self.mywin.connect("leave-notify-event", self.area_leave)
         #self.mywin.connect("event", self.unmap)
 
         self.tbar = self.merge.get_widget("/ToolBar")
         #self.tbar.set_tooltips(True)
+        self.tbar.set_icon_size(Gtk.IconSize.LARGE_TOOLBAR)
         self.tbar.show()
 
         self.hpaned = Gtk.HPaned(); self.hpaned.set_border_width(2)
 
         #warnings.simplefilter("ignore")
         scroll = Gtk.ScrolledWindow()
         #warnings.simplefilter("default")
@@ -1652,18 +1654,16 @@
 
     # Traditional open file
     def open(self):
 
         #warnings.simplefilter("ignore")
         but =   "Cancel", Gtk.ButtonsType.CANCEL,\
          "Open File", Gtk.ButtonsType.OK
-        fc = Gtk.FileChooserDialog("Open file", self.mywin, \
-             Gtk.FileChooserAction.OPEN  \
-            #Gtk.FILE_CHOOSER_ACTION_SELECT_FOLDER
-            , but)
+        fc = Gtk.FileChooserDialog(title="Open file", transient_for=self.mywin, \
+             action=Gtk.FileChooserAction.OPEN, buttons=but)
         #warnings.simplefilter("default")
 
         filters = []
         filters.append(self.makefilter("*.*", "All files (*.*)"))
         filters.append(self.makefilter("*.py", "Python files (*.py)"))
         filters.append(self.makefilter("*.c", "'C' source files (*.c)"))
         filters.append(self.makefilter("*.h", "'H' source files (*.h)"))
```

### Comparing `pyedpro-3.3.1/pedlib/pedxtnd.py` & `pyedpro-3.3.5/pedlib/pedxtnd.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/pedync.py` & `pyedpro-3.3.5/pedlib/pedync.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/plugins/lower_right.py` & `pyedpro-3.3.5/pedlib/plugins/lower_right.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/stack.py` & `pyedpro-3.3.5/pedlib/stack.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/test.py` & `pyedpro-3.3.5/pedlib/test.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/testdiff.py` & `pyedpro-3.3.5/pedlib/testdiff.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pedlib/webwin.py` & `pyedpro-3.3.5/pedlib/webwin.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pycommon/browsewin.py` & `pyedpro-3.3.5/pycommon/browsewin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/env python
 
 ''' This encapsulates the browser window wit the webkia an toolbars '''
 
 import os, sys, getopt, signal, random, time, warnings
 
 realinc = os.path.realpath(os.path.dirname(__file__) + os.sep + "../pycommon")
-sys.path.append(realinc)
+if realinc not in sys.path:
+    sys.path.append(realinc)
 
 from pgutils import  *
 from pggui import  *
 from pgsimp import  *
 
 import gi
 gi.require_version("Gtk", "3.0")
```

### Comparing `pyedpro-3.3.1/pycommon/htmledit.py` & `pyedpro-3.3.5/pycommon/htmledit.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pycommon/icons.py` & `pyedpro-3.3.5/pycommon/icons.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 
 import os, sys, getopt, signal, random, time, warnings
 
 realinc = os.path.realpath(os.path.dirname(__file__) + os.sep + "../pycommon")
-sys.path.append(realinc)
+if realinc not in sys.path:
+    sys.path.append(realinc)
 
 from pgutils import  *
 from pggui import  *
 from pgsimp import  *
 
 import gi
 gi.require_version("Gtk", "3.0")
```

### Comparing `pyedpro-3.3.1/pycommon/pgbox.py` & `pyedpro-3.3.5/pycommon/pgbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,24 @@
 from gi.repository import Gtk
 from gi.repository import Gdk
 from gi.repository import GLib
 from gi.repository import GObject
 from gi.repository import Pango
 from gi.repository import PangoCairo
 
-import sutil
+realinc = os.path.realpath(os.path.dirname(__file__) + os.sep + "../pycommon")
+if realinc not in sys.path:
+    sys.path.append(realinc)
 
-sys.path.append('..')
-import pycommon.pgutils
+#print("import", __file__)
 
+import sutil
+#sys.path.append('..')
+#import pycommon.pgutils
+import pgutils
 
 box_testmode = False
 
 def str2rgb(col):
 
     #print("in", col)
     aa = int(col[1:3], base=16)
```

### Comparing `pyedpro-3.3.1/pycommon/pgbutt.py` & `pyedpro-3.3.5/pycommon/pgbutt.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,16 +14,22 @@
 from gi.repository import GObject
 from gi.repository import Pango
 from gi.repository import GObject
 
 gi.require_version('PangoCairo', '1.0')
 from gi.repository import PangoCairo
 
+realinc = os.path.realpath(os.path.dirname(__file__) + os.sep + "../pycommon")
+if realinc not in sys.path:
+    sys.path.append(realinc)
+
 import cairo
-from sutil import *
+import pgutils
+import pgsimp
+import sutil
 
 class smallbutt(Gtk.EventBox):
 
     __gsignals__ = {
     #"activate": (GObject.SIGNAL_RUN_FIRST, GObject.TYPE_NONE, () ),
     "pressed": (GObject.SIGNAL_RUN_FIRST, GObject.TYPE_NONE, () ),
     }
```

### Comparing `pyedpro-3.3.1/pycommon/pgentry.py` & `pyedpro-3.3.5/pycommon/pgentry.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pycommon/pggui.py` & `pyedpro-3.3.5/pycommon/pggui.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,16 +13,18 @@
 from gi.repository import GObject
 from gi.repository import Pango
 
 gi.require_version('PangoCairo', '1.0')
 from gi.repository import PangoCairo
 
 realinc = os.path.realpath(os.path.dirname(__file__) + os.sep + "../pycommon")
-sys.path.append(realinc)
+if realinc not in sys.path:
+    sys.path.append(realinc)
 
+#print("import", __file__)
 import pgutils
 import pgsimp
 
 IDXERR = "Index is larger than the available number of controls."
 
 gui_testmode = 0
```

### Comparing `pyedpro-3.3.1/pycommon/pgsimp.py` & `pyedpro-3.3.5/pycommon/pgsimp.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pycommon/pgtextview.py` & `pyedpro-3.3.5/pycommon/pgtextview.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pycommon/pgutils.py` & `pyedpro-3.3.5/pycommon/pgutils.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pycommon/pgwkit.py` & `pyedpro-3.3.5/pycommon/pgwkit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python
 
 ''' This encapsulates the webkit '''
 
 import os, sys, getopt, signal, random, time, warnings
 import inspect
 
-realinc = os.path.realpath(os.path.dirname(__file__) + os.sep + "../pycommon")
-sys.path.append(realinc)
+#realinc = os.path.realpath(os.path.dirname(__file__) + os.sep + "../pycommon")
+#sys.path.append(realinc)
 
 from pgutils import  *
 from pggui import  *
 from pgsimp import  *
 from pgtextview import  *
 
 import gi
```

### Comparing `pyedpro-3.3.1/pycommon/plug.py` & `pyedpro-3.3.5/pycommon/plug.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pycommon/pypacker.py` & `pyedpro-3.3.5/pycommon/pypacker.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pycommon/sutil.py` & `pyedpro-3.3.5/pycommon/sutil.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pycommon/testbutt.py` & `pyedpro-3.3.5/pycommon/testbutt.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pycommon/testnums.py` & `pyedpro-3.3.5/pycommon/testnums.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pycommon/testpacker.py` & `pyedpro-3.3.5/pycommon/testpacker.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pycommon/testpacker2.py` & `pyedpro-3.3.5/pycommon/testpacker2.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pycommon/testpacker3.py` & `pyedpro-3.3.5/pycommon/testpacker3.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pycommon/testpacker4.py` & `pyedpro-3.3.5/pycommon/testpacker4.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pycommon/testroot.py` & `pyedpro-3.3.5/pycommon/testroot.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pycommon/testsimple.py` & `pyedpro-3.3.5/pycommon/testsimple.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pycommon/testtextv.py` & `pyedpro-3.3.5/pycommon/testtextv.py`

 * *Files identical despite different names*

### Comparing `pyedpro-3.3.1/pyedpro.desktop` & `pyedpro-3.3.5/pyedpro.desktop`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 Type=Application
 
 # Enter the name of the icon you want to use for the application, you can
 #enter a path for the icon as well like /usr/share/pixmaps/icon.png but make
 #sure to include the icon.png file in your project folder first and in the
 #setup.py file as well. Here we'll use the "system" icon for now.
 
-Icon=/usr/share/icons/hicolor/96x96/apps/pyedpro.png
+Icon=/usr/share/icons/hicolor/96x96/apps/pyedpro
 
 # The category of the file, you can view the available categories from the
 # freedesktop website.
 Categories=GNOME;GTK;Utility;
 StartupNotify=false
 
 # EOF
```

### Comparing `pyedpro-3.3.1/pyedpro.egg-info/PKG-INFO` & `pyedpro-3.3.5/pyedpro.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyedpro
-Version: 3.3.1
+Version: 3.3.5
 Summary: High power editor in python.
 Home-page: https://github.com/pglen/pyedpro
 Author: Peter Glen
 Author-email: peterglen99@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,80 +19,99 @@
 ## Python editor.
 
    Welcome to PyEdPro. This is modern multi-platform editor. Simple, powerful,
 configurable, extendable. Goodies like macro recording / playback, spell check,
 column select, multiple clipboards, unlimited undo ... makes it an editor
 that I use every day.
 
-  This project's source is at - https://github.com/pglen/pyedpro
-
   Working and tested platforms currently are:
 
         Win 7 .. Win 10 ...
         Centos 6 .. 7 Ubuntu 14 ... 16 ...  20.x (should run on any linux )
         Windows (Native) plus MSYS2, Mingw,
         Raspberry PI 3, Raspberry PI 4, ...
         Mac ** Some functions are disabled - in particular async processing
 
-Pyedpro functions near identical on Linux / Windows / Mac / Raspberry PI
+Pyedpro functions in a near identical manner
+    on Linux / Windows / Mac / Raspberry PI
 
  Pyedpro has:
 
-            o  macro recording/play,
-            o  search/replace,
-            o  functional navigation,
-            o  comment/string spell check,
-            o  full spell check, spell suggestion dialog
-            o  auto backup,
-            o  persistent undo/redo,  (undo beyond last save)
-            o  auto complete, auto correct,
+            o  Macro recording/play,
+            o  Search/replace,
+            o  Functional navigation,
+            o  Fomment/string spell check,
+            o  Full spell check, spell suggestion dialog
+            o  Auto backup,
+            o  Persistent undo/redo,  (undo beyond last save)
+            o  Auto complete, auto correct
             o
             o  ... and a lot more.
 
  It is fast, it is extendable. The editor has a table driven key mapping.
  One can easily edit the key map in keyhand.py, and the key actions
  in acthand.py The default key map resembles gedit / wed / etp / brief
 
+ The editor can be run from pip; from single packed executable; from git
+directory, and from packaged appimage.
+
+ The images are available from the git largefile subsystem.
+
 [See Doxygen generated Documentation on GitHub Pages](https://pglen.github.io/pyedpro/html/)
 
 ### Platforms
 
   I mainly run it on Ubuntu, and in Win32 / MSYS2, some Fedora, Windows 10,
-and the Raspberry-Pi. It behaves consistently on all these platforms,
+(x64) and the Raspberry-Pi. It behaves consistently on all these platforms,
 it is an absolute joy to edit in a different platform without the learning
-curve of new keystrokes.  If you want an editor  that works the same way in
+curve of new keystrokes.  If you want an editor that works the same way in
 all your workspaces, PyEdPro is the one.
 
- PyEdPro now is working good on the Mac. I installed homebrew, and got it to fire up. It
-was not a trivial exercise, as the Mac PygGOject did not do half of the stuff as the
-Linux version did. No asynchronous  anything, segmentation faults everywhere. (which python
+ PyEdPro now is working OK on the Mac M1. I installed homebrew, and got
+it to fire up. It was not a trivial exercise, as the Mac PygGOject did not do
+half of the stuff as the Linux version did.
+No asynchronous  anything, segmentation faults everywhere. (which python
 is not suppose to have)
+
   The font rendering was messed up, but I got fixed by replacing Pango's
 get_pixel_size() with get_size() / PANGO_UNIT. [Suspect int vs float accuracy issues]
   Some async functions like the function updater is disabled, but it can be done
 manually. (right click on doc -> rescan) All in all the Mac's PyGobject is not a great
 subsystem, hopefully time will be kind here.
 
 ** tried the M1 ... Sun 03.Apr.2022 most of it worked; no async processing
-as Glib the timer functions bombed. Great hardware - bad PyGobject support. However
-if an editor with familiar key op is needed -- most of it works with no destructive errors.
+as in Glib the timer functions bombed. Great hardware - bad PyGobject support. However
+if an editor with familiar key op is needed -- most of it works. And no
+destructive errors.
 
-### New:
+### History:
 
     (this is extracted, use git log for up-to-date information)
 
+    Sat 11.Feb.2023 -- Pyedpro Notes export / import and the new pydbase data base
+    Thu 27.Oct.2022 -- Restored system menu processing (Alt-f [File Menu] and such)
     Sat 10.Sep.2022 -- the system shortcuts (ctrl-s ctrl-o) are re-done by hand
-    Sat 03.Sep.2022 -- pubilshed on pip
+    Sat 03.Sep.2022 -- published on pip
     Thu 21.Apr.2022 -- release issued
     Wed 16.Mar.2022 -- dialog for read only file, export notes ... lots of other stuff
     Wed 01.Dec.2021 -- on search, descending one dir level with Ext. Search
     Sun 05.Sep.2021 -- made it function on the Mac M1 laptop  - !@#$$%
+        ....        -- lot of changes, see github log
+
+
+### New:
+
+    3.3.1   Fri 15.Mar.2024 -- corrected for changes in the public pydbase interface
+    3.3.5   Wed 10.Apr.2024 -- Relocated search window for better screen allocation
 
 Partial list, some highlights;
 
+Added separate interpretation for right control keys, so exotic items
+like 'insert html comment' can be tied to a shortcut key;
+
 Added drag / drop source / target. New keystroke combo for keyboards
  without home / pgup etc ... Implemented html preview. Just right click on
 the file body, an select the corresponding menu item.
 
 Implemented markdown preview. Right click ... menu
 Implemented M4 preview. The files are pulled in from the current directory (of the macro),
 and expanded with the m4 macro processor. The results than are previewed
@@ -150,17 +169,17 @@
  Any (fixed) font can be configured. No arrangements in the program for variable pitch fonts.
 
   See KEYS file for the list of keyboard shortcuts or press F1 in the
 editor or look at the file in pyedlib/KEYS. This file is also called up when the main menu
  Help -> 'KeyHelp In Doc' is called up.
 
   If you highlight a word, and press F2, Zeal will open with the item searched and
-highlighted. Shift F2 will do the same with Devhelp. This is what I use to see the API of PyGobj.
-F1 will call up the PyEdPro's help screen. Shift-F1 will open DevDocs. Naturally,
-Devdocs/Devhelp/Zeal need to be installed for these to function.
+highlighted. Shift F2 will do the same with Devhelp. This is what I use to see the
+ API of PyGobj. F1 will call up the PyEdPro's help screen. Shift-F1 will open
+DevDocs. Naturally, Devdocs/Devhelp/Zeal need to be installed for these to function.
 
   On initial start, PyEdPro shows a left pane and a top pane. The left pane
 is for function summary and the top pane is for double view of the same file.
 (to see the caller and the called [function] at once) These panes can be hidden with
 the mouse by dragging on their handle, or by the key combination Alt-Q (Shift-Alt-Q for
 the left pane) The first file window's settings are saved for the next startup.
 
@@ -213,32 +232,33 @@
 
 Screen from Mac:
 
 ![Screen Shot](screen_shot_mac.png)
 
 ## Project stats:
 
-        Project name
-            PyEdPro
-        Generated
-            2022-04-21 13:40:49 (in 3 seconds)
-        Generator
-            GitStats (version 55c5c28), git version 2.32.0, gnuplot 5.4 patchlevel 1
-        Report Period
-            2018-09-16 00:29:10 to 2022-04-15 10:31:49
-        Age
-            1308 days, 166 active days (12.69%)
-        Total Files
-            220
-        Total Lines of Code
-            476774 (1454450 added, 977676 removed)
-        Total Commits
-            347 (average 2.1 commits per active day, 0.3 per all days)
-        Authors
-            7 (average 49.6 commits per author)
-
+    Project name
+        pgpygtk
+    Generated
+        2024-04-10 02:22:26 (in 61 seconds)
+    Generator
+        GitStats (version 55c5c28), git version 2.34.1, gnuplot 5.4 patchlevel 2
+    Report Period
+        2018-09-16 00:29:10 to 2024-04-10 02:10:24
+    Age
+        2034 days, 224 active days (11.01%)
+    Total Files
+        13122
+    Total Lines of Code
+        2412587 (7146598 added, 4734011 removed)
+    Total Commits
+        756 (average 3.4 commits per active day, 0.4 per all days)
+    Authors
+        7 (average 108.0 commits per author)
 
 ![Stats](commits_by_year_month.png)
 
-License:    Open Source, FreeWare
+## License:
+
+    Open Source, FreeWare, Unlicence, MIT at your convenience
 
 // EOF
```

### Comparing `pyedpro-3.3.1/pyedpro.py` & `pyedpro-3.3.5/pyedpro.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python3
 
+__doc__ = \
 '''! \mainpage
 
 ## Welcome to PyEdPro.
 
 This is modern multi-platform editor. Simple, powerful,
 configurable, extendable. Goodies like macro recording / playback, spell check,
 column select, multiple clipboards, unlimited undo ... makes it an editor
@@ -50,95 +51,70 @@
             o
             o  ... and a lot more.
 
   PyeEdPro is fast, it is extendable. The editor has a table driven key mapping.
  One can easily edit the key map in keyhand.py, and the key actions
  in acthand.py The default key map resembles gedit / wed / etp / brief / Notepad
 
-ASCII text editor, requires pyGtk. (PyGObject)
-
- See pygtk-dependencies for easy install of dependencies.
- See also the INSTALL file.
-
-'''
-
-#from __future__ import absolute_import
-#from __future__ import print_function
-
-import os
-import sys
-import getopt
-import signal
-import time
-import platform
-
-'''!
- \mainpage
  ------------------------------------------------------------------------
- This project is a successor of pyedit.py
+ ## This project is a successor of pyedit.py
 
  Pyedpro functions near identical on Linux / Windows / Mac / Raspberry PI
 
  It is fast, it is extendable. The editor has a table driven key mapping.
  One can easily edit the key map in keyhand.py, and the key actions
  in acthand.py The default key map resembles gedit / wed / etp / brief
 
- History:  (incomplete list)
+History:  (incomplete list, see git log for a more complete list)
 
- Thu 27.Oct.2022   Restored menu keymaps for the system to handle it.
- Sun 05.Sep.2021   ported to Mac M1 ... what a pain .. half the things did not work
- jul/19/2018       Coloring for spell check, Trigger by scroll, more dominant color
- Jul/xx/2018       Update README, KEYS.TXT
- Jun/xx/2018       Log Files for time accounting.
- Jun/08/2020       Menu control / Headerbar / Version update
- Mon 28.Sep.2020   Reshuffled imports pylint
- Fri 25.Dec.2020   Added web view, m4 filter md2html filterRelese ready
- Fri 07.May.2021   Many fixed, installs, new features
- Tue 06.Sep.2022   Installation, anchor for search ...
+    jul/19/2018       Coloring for spell check, Trigger by scroll, more dominant color
+    Jul/xx/2018       Update README, KEYS.TXT
+    Jun/xx/2018       Log Files for time accounting.
+    Jun/08/2020       Menu control / Headerbar / Version update
+    Mon 28.Sep.2020   Reshuffled imports pylint
+    Fri 25.Dec.2020   Added web view, m4 filter md2html filterRelese ready
+    Fri 07.May.2021   Many fixed, installs, new features
+    Sun 05.Sep.2021   ported to Mac M1 ... what a pain .. half the things did not work
+    Tue 06.Sep.2022   Installation, anchor for search ...
+    Thu 27.Oct.2022   Restored menu keymaps for the system to handle it.
 
  ASCII text editor, requires pyGtk. (pygobject)
  See pygtk-dependencies for easy install of dependencies.
  See also the INSTALL file.
+
 '''
 
+import os, sys, getopt, signal, time, platform, atexit
+
 import gettext
 gettext.bindtextdomain('pyedpro', './locale/')
 gettext.textdomain('pyedpro')
 _ = gettext.gettext
 #locale.setlocale(locale.LC_ALL, '')
+#print("domain", gettext.textdomain)
+
+import gi; gi.require_version("Gtk", "3.0")
+from gi.repository import Gtk
+from gi.repository import Gdk
+from gi.repository import GLib
+from gi.repository import Gio
+from gi.repository import GObject
 
 orgbase = os.getcwd()
 #print("cwd", orgbase)
-
-#base    = os.path.realpath(__file__)
-#basedir = os.path.dirname(base)
-#print("file", os.path.dirname(base))
 #os.chdir(basedir)
 
-#modbase = ""
-#for aa in sys.path:
-#    if "pyedpro-" in aa:
-#        #print("aa", aa)
-#        modbase = aa
-
-#sys.path.append(basedir + os.sep + "panglib")
-#sys.path.append(basedir + os.sep + "pedlib")
-#sys.path.append(basedir + os.sep + "pycommon")
-
-# Also add pyedpro's EGG module dependencies
-
-#sys.path.append(modbase + os.sep + "panglib")
-#sys.path.append(modbase + os.sep + "pedlib")
-#sys.path.append(modbase + os.sep + "pycommon")
-
-#sys.path.append("panglib")
-#sys.path.append("pedlib")
-#sys.path.append("pycommon")
+basedir = os.path.dirname(os.path.realpath(__file__))
+#print("file dir", basedir)
+sys.path.append(basedir + os.sep)
+sys.path.append(basedir + os.sep + "pycommon")
+sys.path.append(basedir + os.sep + "pedlib")
+#sys.path.append(basedir + os.sep + ".." + os.sep + "pycommon")
 
-#print(sys.path)
+#print("pyedpro path", sys.path)
 
 from pedlib import pedconfig
 from pedlib import pedync
 
 # Commit global crap here
 pedconfig.conf = pedconfig.Conf()
 
@@ -146,47 +122,35 @@
 from pedlib import acthand
 from pedlib import pedsql
 
 pedconfig.conf.acth = acthand.ActHand()
 pedconfig.conf.keyh = keyhand.KeyHand(pedconfig.conf.acth)
 pedconfig.conf.orig_path = orgbase
 
-#sys.path.append('.' + os.sep + "pycommon")
-
 from pedlib import pedwin
 from pedlib import pedlog
 from pedlib import pedutil
 from pedlib import pedplug
 
-import gi; gi.require_version("Gtk", "3.0")
-from gi.repository import Gtk
-from gi.repository import Gtk
-from gi.repository import Gdk
-from gi.repository import GLib
-from gi.repository import Gio
-from gi.repository import GObject
-
 import faulthandler
 faulthandler.enable()
 
 def tracer(frame, event, arg):
     if event != "line" and event != "return":
         print(event, frame.f_code.co_filename, frame.f_lineno)
     return tracer
 
-#print("domain", gettext.textdomain)
-
 #try:
 #    from pkg_resources import resource_filename
 #    print (os.path.abspath(resource_filename(__name__.data, 'pedicon.png')) )
 #except:
 #    print(sys.exc_info())
 
-VERSION     = "3.3.1"
-BUILDDATE   = "Thu 15.Feb.2024"
+VERSION     = "3.3.5"
+BUILDDATE   = "Wed 10.Apr.2024"
 PROGNAME    = "PyEdPro"
 
 # ------------------------------------------------------------------------
 
 class MainPyed(Gtk.Application):
 
     def __init__(self, projname, strarr):
@@ -215,27 +179,37 @@
         mainwin = pedwin.EdMainWindow(None, None, self.strarr, orgbase)
         self.add_window(mainwin.mywin)
         pedconfig.conf.pedwin = mainwin
 
         if self.projname:
             mainwin.opensess(self.projname)
 
+def cleanup(mw):
+    #print("Cleanup", mw.cleanit)
+    for aa in mw.cleanit:
+        bb = os.path.join(pedconfig.conf.temp_dir, os.path.basename(aa))
+        if os.path.isfile(bb):
+            os.remove(bb)
+        #print("Cleaning", aa, bb)
+        os.rename(aa, bb)
 
 def run_main(projname, strarr):
 
     if pedconfig.conf.verbose:
         print(PROGNAME, "running on", "'" + os.name + "'", \
             "GTK", Gtk._version, "PyGtk", \
                "%d.%d.%d" % (Gtk.get_major_version(), \
                     Gtk.get_minor_version(), \
                         Gtk.get_micro_version()))
 
     signal.signal(signal.SIGTERM, terminate)
     mainwin = pedwin.EdMainWindow(None, None, strarr, orgbase)
     pedconfig.conf.pedwin = mainwin
+    mainwin.cleanit = []
+    atexit.register(cleanup, mainwin)
 
     if projname:
         mainwin.opensess(projname)
     Gtk.main()
 
 def xversion():
     ''' Offer version number '''
@@ -461,8 +435,8 @@
     mainstart("", [], "")
 
 # Setup needed it for scripts
 
 if __name__ == '__main__':
     mainfunc()
 
-# EOF
+# EOF
```

### Comparing `pyedpro-3.3.1/setup.py` & `pyedpro-3.3.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os, sys, shutil
 import setuptools
 
 descx = '''PyEdPro is modern multi-platform editor. Simple, powerful,
 configurable, extendable. Goodies like macro recording / playback, spell check,
 column select, multiple clipboards, unlimited undo ...
    PyEdPro.py has macro recording/play, search/replace, one click function navigation,
 auto backup, undo/redo, auto complete, auto correct, syntax check, spell suggestion
@@ -10,83 +11,85 @@
  after the editor is closed.
     The spell checker can check code comments. The parsing of the code is
 rudimentary, comments and strings are spell checked. (Press F9 or Shit-F9) The code is filtered
 out for Python and  'C'. The spell checker is executed on live text. (while typing)
 '''
 
 classx = [
-          'Development Status :: Mature',
-          'Environment :: GUI',
-          'Intended Audience :: End Users/Desktop',
-          'Intended Audience :: Developers',
-          'Intended Audience :: System Administrators',
-          'License :: OSI Approved :: Python Software Foundation License',
-          'Operating System :: Microsoft :: Windows',
-          'Operating System :: POSIX',
-          'Programming Language :: Python',
-          'Topic :: Editors',
-          'Topic :: Software Development :: Editor',
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
         ]
 
 includex = ["*", "pedlib/", "panglib", "pedlib/images",
             "image.png", "pyedpro_ubuntu.png"]
 
+#shutil.copy("../README.md", "README.copy.md")
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
+#os.remove("README.copy.md")
+
+# Get version number  from the server support file:
+fp = open("pyedpro.py", "rt")
+vvv = fp.read(); fp.close()
+loc_vers =  '1.0.0'     # Default
+for aa in vvv.split("\n"):
+    idx = aa.find("VERSION ")
+    if idx == 0:        # At the beginning of line
+        try:
+            loc_vers = aa.split()[2].replace('"', "")
+            break
+        except:
+            pass
+#print("loc_vers:", loc_vers)
+#sys.exit()
 
 setuptools.setup(
     name="pyedpro",
-    version="3.3.1",
+    version=loc_vers,
     author="Peter Glen",
     author_email="peterglen99@gmail.com",
     description="High power editor in python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pglen/pyedpro",
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
+    classifiers=classx,
     include_package_data=True,
+    package_data={ "pedlib": ["docs/*"], },
     packages=setuptools.find_packages(include=includex),
-    #packages=setuptools.find_packages('pedlib, pedlib/data, panglib, pycommon'),
-
-    #str(['pedlib', 'panglib', 'pycommon'])),
     scripts = ['pyedpro.py', 'pangview.py'],
 
     package_dir = {
                     'pedlib': 'pedlib',
-                    'pydbase': 'pydbase',
                     'pedlib/images': 'pedlib/images',
                     'pedlib/plugins': 'pedlib/plugins',
                     'pedlib/data' : 'pedlib/data',
                     'pycommon': 'pycommon',
                     'panglib': 'panglib',
                    },
 
-    package_py = {
-                    '':
-                        ['pedlib/images/pyedpro.png',
-                         'pedlib/images/pyedpro_sub.png',
-                         'pedlib/images/pedicon.png', 'image.png',
-                         'pyedpro_ubuntu.png'
-                        ]
-                    },
+    #package_py = {
+    #                '':
+    #                    ['pedlib/images/pyedpro.png',
+    #                     'pedlib/images/pyedpro_sub.png',
+    #                     'pedlib/images/pedicon.png', 'image.png',
+    #                     'pyedpro_ubuntu.png'
+    #                    ]
+    #                },
 
     data_files =  [('/usr/share/icons/hicolor/96x96/apps/',
                         ['pedlib/images/pyedpro.png',
                             'pedlib/images/pedicon.png',
                             'pedlib/images/pyedpro_sub.png' ]),
                             ('/usr/share/applications', ['pyedpro.desktop']),
                    ],
 
     python_requires='>=3',
-    install_requires=['pyvpacker', 'pydbase', ],
+    install_requires=["pyvpacker", "pydbase" ],
     entry_points={
         'console_scripts': [ "pyedpro=pyedpro:mainfunc",
             "pangview=pangview:mainfunc",
             ],
     },
 )
 
-# EOF
+# EOF
```

