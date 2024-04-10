# Comparing `tmp/not1mm-24.4.9.2.tar.gz` & `tmp/not1mm-24.4.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "not1mm-24.4.9.2.tar", last modified: Wed Apr 10 00:24:43 2024, max compression
+gzip compressed data, was "not1mm-24.4.9.3.tar", last modified: Wed Apr 10 00:37:46 2024, max compression
```

## Comparing `not1mm-24.4.9.2.tar` & `not1mm-24.4.9.3.tar`

### file list

```diff
@@ -1,159 +1,159 @@
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-10 00:24:43.979837 not1mm-24.4.9.2/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/LICENSE
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    27150 2024-04-10 00:24:43.975837 not1mm-24.4.9.2/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    26077 2024-04-09 23:24:41.000000 not1mm-24.4.9.2/README.md
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-10 00:24:43.645831 not1mm-24.4.9.2/not1mm/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   123101 2024-04-09 22:52:19.000000 not1mm-24.4.9.2/not1mm/__main__.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    34021 2024-04-09 23:22:19.000000 not1mm-24.4.9.2/not1mm/bandmap.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10168 2024-04-09 23:22:21.000000 not1mm-24.4.9.2/not1mm/checkwindow.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-10 00:24:43.745833 not1mm-24.4.9.2/not1mm/data/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/JetBrainsMono-Regular.ttf
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   366478 2024-04-02 17:57:36.000000 not1mm-24.4.9.2/not1mm/data/MASTER.SCP
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2067 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/about.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      224 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/alpha bravo charlie delta.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7125 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/bandmap.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      387 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/check.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4614 2024-04-09 18:40:45.000000 not1mm-24.4.9.2/not1mm/data/checkwindow.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51643 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/configuration.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    89307 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/contests.sql
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)  4790698 2024-04-02 16:11:52.000000 not1mm-24.4.9.2/not1mm/data/cty.json
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      451 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/cwmacros.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      116 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/donors.html
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    27404 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/editcontact.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2689 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/editmacro.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      474 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/greendot.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/k6gte-not1mm.desktop
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6076 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/k6gte.not1mm-128.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1526 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/k6gte.not1mm-32.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2925 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/k6gte.not1mm-64.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1436 2024-04-01 23:54:49.000000 not1mm-24.4.9.2/not1mm/data/logwindow.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1610 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/logwindowx.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54341 2024-04-04 21:22:08.000000 not1mm-24.4.9.2/not1mm/data/main.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    21823 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/new_contest.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    23273 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/not1mm.html
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2247 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/opon.ui
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-10 00:24:43.842835 not1mm-24.4.9.2/not1mm/data/phonetics/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42590 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/0.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30248 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/1.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29584 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/2.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32072 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/3.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43052 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/4.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51976 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/5.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58634 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/6.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49154 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/7.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32842 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/73.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35636 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/8.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39592 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/9.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46800 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/a.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44594 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/again.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40976 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/b.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46746 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/c.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    62558 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/contest.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    92498 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/cq.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52524 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/d.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    45700 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/e.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    53438 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/f.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42766 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/g.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50040 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/h.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46372 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/i.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43434 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/j.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49066 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/k.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   185562 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/k6gte.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43154 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/l.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54352 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/m.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56798 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/mynumber.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52204 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/n.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   154544 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/nil.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47440 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/o.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    38300 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/p.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    55288 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/q.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47432 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/r.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46122 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/roger.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    60698 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/s.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    70424 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/space.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58196 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/t.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56320 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/thankyou.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    94980 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/thankyouqrz.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    65922 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/u.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50142 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/v.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    37638 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/w.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    61870 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/x.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56524 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/y.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46510 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/yourcall.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51768 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/z.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1600 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/pickcontest.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1234 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/radio_green.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1258 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/radio_grey.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      957 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/radio_red.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/reddot.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40028 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/settings.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      470 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/ssbmacros.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2054 2024-04-09 22:51:54.000000 not1mm-24.4.9.2/not1mm/data/vfo.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1652 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/fsutils.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-10 00:24:43.878835 not1mm-24.4.9.2/not1mm/lib/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/lib/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      416 2024-04-02 16:43:54.000000 not1mm-24.4.9.2/not1mm/lib/about.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15127 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/lib/cat_interface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3126 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/lib/cwinterface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42480 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/lib/database.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      353 2024-04-02 16:43:38.000000 not1mm-24.4.9.2/not1mm/lib/edit_contact.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      517 2024-04-02 16:43:30.000000 not1mm-24.4.9.2/not1mm/lib/edit_macro.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      359 2024-04-02 16:43:21.000000 not1mm-24.4.9.2/not1mm/lib/edit_opon.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1965 2024-04-02 16:43:09.000000 not1mm-24.4.9.2/not1mm/lib/edit_station.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4220 2024-04-08 02:01:24.000000 not1mm-24.4.9.2/not1mm/lib/ft8_watcher.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10978 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/lib/ham_utility.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13952 2024-04-03 03:28:34.000000 not1mm-24.4.9.2/not1mm/lib/lookup.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3249 2024-04-02 17:02:22.000000 not1mm-24.4.9.2/not1mm/lib/multicast.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5712 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/lib/n1mm.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      816 2024-04-04 17:56:24.000000 not1mm-24.4.9.2/not1mm/lib/new_contest.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8605 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/lib/plugin_common.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      359 2024-04-02 16:41:42.000000 not1mm-24.4.9.2/not1mm/lib/select_contest.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8877 2024-04-02 16:41:49.000000 not1mm-24.4.9.2/not1mm/lib/settings.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2334 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/lib/super_check_partial.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       49 2024-04-09 23:23:17.000000 not1mm-24.4.9.2/not1mm/lib/version.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1286 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/lib/versiontest.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    44603 2024-04-09 23:22:17.000000 not1mm-24.4.9.2/not1mm/logwindow.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-10 00:24:43.970837 not1mm-24.4.9.2/not1mm/plugins/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10873 2024-04-04 18:50:36.000000 not1mm-24.4.9.2/not1mm/plugins/10_10_fall_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10878 2024-04-04 18:58:51.000000 not1mm-24.4.9.2/not1mm/plugins/10_10_spring_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10887 2024-04-04 18:58:54.000000 not1mm-24.4.9.2/not1mm/plugins/10_10_summer_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10890 2024-04-04 18:58:56.000000 not1mm-24.4.9.2/not1mm/plugins/10_10_winter_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/plugins/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13677 2024-04-04 19:07:30.000000 not1mm-24.4.9.2/not1mm/plugins/arrl_10m.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13722 2024-04-04 19:09:51.000000 not1mm-24.4.9.2/not1mm/plugins/arrl_dx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13725 2024-04-04 19:10:06.000000 not1mm-24.4.9.2/not1mm/plugins/arrl_dx_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10052 2024-04-04 18:11:53.000000 not1mm-24.4.9.2/not1mm/plugins/arrl_field_day.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7994 2024-04-04 19:10:45.000000 not1mm-24.4.9.2/not1mm/plugins/arrl_rtty_ru.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12989 2024-04-04 20:51:30.000000 not1mm-24.4.9.2/not1mm/plugins/arrl_ss_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12977 2024-04-04 20:53:34.000000 not1mm-24.4.9.2/not1mm/plugins/arrl_ss_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12481 2024-04-04 19:17:41.000000 not1mm-24.4.9.2/not1mm/plugins/arrl_vhf_jan.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11500 2024-04-04 19:18:17.000000 not1mm-24.4.9.2/not1mm/plugins/arrl_vhf_jun.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11500 2024-04-04 19:18:29.000000 not1mm-24.4.9.2/not1mm/plugins/arrl_vhf_sep.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11907 2024-04-04 19:23:16.000000 not1mm-24.4.9.2/not1mm/plugins/canada_day.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14059 2024-04-04 19:27:40.000000 not1mm-24.4.9.2/not1mm/plugins/cq_160_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14102 2024-04-04 19:27:52.000000 not1mm-24.4.9.2/not1mm/plugins/cq_160_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12399 2024-04-04 19:29:11.000000 not1mm-24.4.9.2/not1mm/plugins/cq_wpx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12487 2024-04-04 19:29:08.000000 not1mm-24.4.9.2/not1mm/plugins/cq_wpx_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11114 2024-04-04 19:31:31.000000 not1mm-24.4.9.2/not1mm/plugins/cq_ww_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11119 2024-04-04 19:31:27.000000 not1mm-24.4.9.2/not1mm/plugins/cq_ww_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12020 2024-04-04 19:46:16.000000 not1mm-24.4.9.2/not1mm/plugins/cwt.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3387 2024-04-04 17:53:54.000000 not1mm-24.4.9.2/not1mm/plugins/general_logging.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11461 2024-04-04 19:46:13.000000 not1mm-24.4.9.2/not1mm/plugins/iaru_hf.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11090 2024-04-04 19:47:46.000000 not1mm-24.4.9.2/not1mm/plugins/jidx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11092 2024-04-04 19:47:59.000000 not1mm-24.4.9.2/not1mm/plugins/jidx_ph.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11510 2024-04-04 19:50:33.000000 not1mm-24.4.9.2/not1mm/plugins/naqp_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11515 2024-04-04 19:50:44.000000 not1mm-24.4.9.2/not1mm/plugins/naqp_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12316 2024-04-04 19:51:26.000000 not1mm-24.4.9.2/not1mm/plugins/phone_weekly_test.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10588 2024-04-04 19:52:18.000000 not1mm-24.4.9.2/not1mm/plugins/stew_perry_topband.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10238 2024-04-04 18:05:44.000000 not1mm-24.4.9.2/not1mm/plugins/winter_field_day.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12169 2024-04-09 23:22:14.000000 not1mm-24.4.9.2/not1mm/vfo.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-10 00:24:43.973837 not1mm-24.4.9.2/not1mm.egg-info/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    27150 2024-04-10 00:24:43.000000 not1mm-24.4.9.2/not1mm.egg-info/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4105 2024-04-10 00:24:43.000000 not1mm-24.4.9.2/not1mm.egg-info/SOURCES.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2024-04-10 00:24:43.000000 not1mm-24.4.9.2/not1mm.egg-info/dependency_links.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2024-04-10 00:24:43.000000 not1mm-24.4.9.2/not1mm.egg-info/entry_points.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      131 2024-04-10 00:24:43.000000 not1mm-24.4.9.2/not1mm.egg-info/requires.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       25 2024-04-10 00:24:43.000000 not1mm-24.4.9.2/not1mm.egg-info/top_level.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1427 2024-04-09 23:23:27.000000 not1mm-24.4.9.2/pyproject.toml
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2024-04-10 00:24:43.979837 not1mm-24.4.9.2/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-10 00:37:46.472488 not1mm-24.4.9.3/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/LICENSE
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    27215 2024-04-10 00:37:46.471488 not1mm-24.4.9.3/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    26142 2024-04-10 00:36:30.000000 not1mm-24.4.9.3/README.md
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-10 00:37:46.382487 not1mm-24.4.9.3/not1mm/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   123052 2024-04-10 00:33:05.000000 not1mm-24.4.9.3/not1mm/__main__.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    34021 2024-04-09 23:22:19.000000 not1mm-24.4.9.3/not1mm/bandmap.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10168 2024-04-09 23:22:21.000000 not1mm-24.4.9.3/not1mm/checkwindow.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-10 00:37:46.405487 not1mm-24.4.9.3/not1mm/data/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/JetBrainsMono-Regular.ttf
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   366478 2024-04-02 17:57:36.000000 not1mm-24.4.9.3/not1mm/data/MASTER.SCP
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2067 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/about.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      224 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/alpha bravo charlie delta.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7125 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/bandmap.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      387 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/check.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4614 2024-04-09 18:40:45.000000 not1mm-24.4.9.3/not1mm/data/checkwindow.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51643 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/configuration.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    89307 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/contests.sql
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)  4790698 2024-04-02 16:11:52.000000 not1mm-24.4.9.3/not1mm/data/cty.json
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      451 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/cwmacros.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      116 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/donors.html
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    27404 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/editcontact.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2689 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/editmacro.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      474 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/greendot.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/k6gte-not1mm.desktop
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6076 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/k6gte.not1mm-128.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1526 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/k6gte.not1mm-32.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2925 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/k6gte.not1mm-64.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1436 2024-04-01 23:54:49.000000 not1mm-24.4.9.3/not1mm/data/logwindow.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1610 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/logwindowx.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54341 2024-04-04 21:22:08.000000 not1mm-24.4.9.3/not1mm/data/main.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    21823 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/new_contest.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    23273 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/not1mm.html
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2247 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/opon.ui
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-10 00:37:46.438488 not1mm-24.4.9.3/not1mm/data/phonetics/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42590 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/0.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30248 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/1.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29584 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/2.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32072 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/3.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43052 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/4.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51976 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/5.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58634 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/6.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49154 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/7.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32842 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/73.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35636 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/8.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39592 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/9.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46800 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/a.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44594 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/again.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40976 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/b.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46746 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/c.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    62558 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/contest.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    92498 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/cq.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52524 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/d.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    45700 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/e.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    53438 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/f.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42766 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/g.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50040 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/h.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46372 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/i.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43434 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/j.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49066 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/k.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   185562 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/k6gte.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43154 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/l.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54352 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/m.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56798 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/mynumber.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52204 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/n.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   154544 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/nil.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47440 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/o.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    38300 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/p.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    55288 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/q.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47432 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/r.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46122 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/roger.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    60698 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/s.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    70424 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/space.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58196 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/t.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56320 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/thankyou.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    94980 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/thankyouqrz.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    65922 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/u.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50142 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/v.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    37638 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/w.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    61870 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/x.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56524 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/y.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46510 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/yourcall.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51768 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/phonetics/z.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1600 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/pickcontest.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1234 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/radio_green.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1258 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/radio_grey.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      957 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/radio_red.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/reddot.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40028 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/settings.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      470 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/data/ssbmacros.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2054 2024-04-09 22:51:54.000000 not1mm-24.4.9.3/not1mm/data/vfo.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1652 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/fsutils.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-10 00:37:46.447488 not1mm-24.4.9.3/not1mm/lib/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/lib/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      416 2024-04-02 16:43:54.000000 not1mm-24.4.9.3/not1mm/lib/about.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15127 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/lib/cat_interface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3126 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/lib/cwinterface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42480 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/lib/database.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      353 2024-04-02 16:43:38.000000 not1mm-24.4.9.3/not1mm/lib/edit_contact.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      517 2024-04-02 16:43:30.000000 not1mm-24.4.9.3/not1mm/lib/edit_macro.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      359 2024-04-02 16:43:21.000000 not1mm-24.4.9.3/not1mm/lib/edit_opon.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1965 2024-04-02 16:43:09.000000 not1mm-24.4.9.3/not1mm/lib/edit_station.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4220 2024-04-08 02:01:24.000000 not1mm-24.4.9.3/not1mm/lib/ft8_watcher.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10978 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/lib/ham_utility.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13952 2024-04-03 03:28:34.000000 not1mm-24.4.9.3/not1mm/lib/lookup.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3249 2024-04-02 17:02:22.000000 not1mm-24.4.9.3/not1mm/lib/multicast.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5712 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/lib/n1mm.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      816 2024-04-04 17:56:24.000000 not1mm-24.4.9.3/not1mm/lib/new_contest.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8605 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/lib/plugin_common.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      359 2024-04-02 16:41:42.000000 not1mm-24.4.9.3/not1mm/lib/select_contest.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8877 2024-04-02 16:41:49.000000 not1mm-24.4.9.3/not1mm/lib/settings.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2334 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/lib/super_check_partial.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       49 2024-04-10 00:34:50.000000 not1mm-24.4.9.3/not1mm/lib/version.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1286 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/lib/versiontest.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    44603 2024-04-09 23:22:17.000000 not1mm-24.4.9.3/not1mm/logwindow.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-10 00:37:46.470488 not1mm-24.4.9.3/not1mm/plugins/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10873 2024-04-04 18:50:36.000000 not1mm-24.4.9.3/not1mm/plugins/10_10_fall_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10878 2024-04-04 18:58:51.000000 not1mm-24.4.9.3/not1mm/plugins/10_10_spring_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10887 2024-04-04 18:58:54.000000 not1mm-24.4.9.3/not1mm/plugins/10_10_summer_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10890 2024-04-04 18:58:56.000000 not1mm-24.4.9.3/not1mm/plugins/10_10_winter_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2024-03-31 16:17:00.000000 not1mm-24.4.9.3/not1mm/plugins/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13677 2024-04-04 19:07:30.000000 not1mm-24.4.9.3/not1mm/plugins/arrl_10m.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13722 2024-04-04 19:09:51.000000 not1mm-24.4.9.3/not1mm/plugins/arrl_dx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13725 2024-04-04 19:10:06.000000 not1mm-24.4.9.3/not1mm/plugins/arrl_dx_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10052 2024-04-04 18:11:53.000000 not1mm-24.4.9.3/not1mm/plugins/arrl_field_day.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7994 2024-04-04 19:10:45.000000 not1mm-24.4.9.3/not1mm/plugins/arrl_rtty_ru.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12989 2024-04-04 20:51:30.000000 not1mm-24.4.9.3/not1mm/plugins/arrl_ss_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12977 2024-04-04 20:53:34.000000 not1mm-24.4.9.3/not1mm/plugins/arrl_ss_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12481 2024-04-04 19:17:41.000000 not1mm-24.4.9.3/not1mm/plugins/arrl_vhf_jan.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11500 2024-04-04 19:18:17.000000 not1mm-24.4.9.3/not1mm/plugins/arrl_vhf_jun.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11500 2024-04-04 19:18:29.000000 not1mm-24.4.9.3/not1mm/plugins/arrl_vhf_sep.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11907 2024-04-04 19:23:16.000000 not1mm-24.4.9.3/not1mm/plugins/canada_day.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14059 2024-04-04 19:27:40.000000 not1mm-24.4.9.3/not1mm/plugins/cq_160_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14102 2024-04-04 19:27:52.000000 not1mm-24.4.9.3/not1mm/plugins/cq_160_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12399 2024-04-04 19:29:11.000000 not1mm-24.4.9.3/not1mm/plugins/cq_wpx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12487 2024-04-04 19:29:08.000000 not1mm-24.4.9.3/not1mm/plugins/cq_wpx_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11114 2024-04-04 19:31:31.000000 not1mm-24.4.9.3/not1mm/plugins/cq_ww_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11119 2024-04-04 19:31:27.000000 not1mm-24.4.9.3/not1mm/plugins/cq_ww_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12020 2024-04-04 19:46:16.000000 not1mm-24.4.9.3/not1mm/plugins/cwt.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3387 2024-04-04 17:53:54.000000 not1mm-24.4.9.3/not1mm/plugins/general_logging.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11461 2024-04-04 19:46:13.000000 not1mm-24.4.9.3/not1mm/plugins/iaru_hf.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11090 2024-04-04 19:47:46.000000 not1mm-24.4.9.3/not1mm/plugins/jidx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11092 2024-04-04 19:47:59.000000 not1mm-24.4.9.3/not1mm/plugins/jidx_ph.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11510 2024-04-04 19:50:33.000000 not1mm-24.4.9.3/not1mm/plugins/naqp_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11515 2024-04-04 19:50:44.000000 not1mm-24.4.9.3/not1mm/plugins/naqp_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12316 2024-04-04 19:51:26.000000 not1mm-24.4.9.3/not1mm/plugins/phone_weekly_test.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10588 2024-04-04 19:52:18.000000 not1mm-24.4.9.3/not1mm/plugins/stew_perry_topband.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10238 2024-04-04 18:05:44.000000 not1mm-24.4.9.3/not1mm/plugins/winter_field_day.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12169 2024-04-09 23:22:14.000000 not1mm-24.4.9.3/not1mm/vfo.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-10 00:37:46.470488 not1mm-24.4.9.3/not1mm.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    27215 2024-04-10 00:37:46.000000 not1mm-24.4.9.3/not1mm.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4105 2024-04-10 00:37:46.000000 not1mm-24.4.9.3/not1mm.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2024-04-10 00:37:46.000000 not1mm-24.4.9.3/not1mm.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2024-04-10 00:37:46.000000 not1mm-24.4.9.3/not1mm.egg-info/entry_points.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      131 2024-04-10 00:37:46.000000 not1mm-24.4.9.3/not1mm.egg-info/requires.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       25 2024-04-10 00:37:46.000000 not1mm-24.4.9.3/not1mm.egg-info/top_level.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1427 2024-04-10 00:35:05.000000 not1mm-24.4.9.3/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2024-04-10 00:37:46.472488 not1mm-24.4.9.3/setup.cfg
```

### Comparing `not1mm-24.4.9.2/LICENSE` & `not1mm-24.4.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/PKG-INFO` & `not1mm-24.4.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: not1mm
-Version: 24.4.9.2
+Version: 24.4.9.3
 Summary: NOT1MM Logger
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/not1mm
 Project-URL: Bug Tracker, https://github.com/mbridak/not1mm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -173,14 +173,15 @@
 - Phone Weekly Test
 - RAC Canada Day
 - Stew Perry Topband
 - Winter Field Day
 
 ## Recent Changes
 
+- [24-4-9-3] Ugh. It's not a real day unless you forget to test.
 - [24-4-9-2] Put back the floatable dock widgets, 'cause Wayland strikes again.
 - [24-4-9-1] Removed DockWidgetFloatable from the dock widgets since my wee brain can't figure out how to add a dragable window frame to them once they are floating. Added a minimum size for the VFO LCD digits. Defaulted bandmap window to the right.
 - [24-4-9] Fixed Checkwindow not showing calls from logged contacts.
 - [24-4-7] Added FT8Watcher class to prep for FT8 support.
 - [24-4-4-1] Made docking widgets open state persistent.
 - [24-4-4] Added per-contest echange hint when adding new contest.
 - [24-4-2] Migrated to PyQt6. I'm sure there are broken things.
```

### Comparing `not1mm-24.4.9.2/README.md` & `not1mm-24.4.9.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -141,14 +141,15 @@
 - Phone Weekly Test
 - RAC Canada Day
 - Stew Perry Topband
 - Winter Field Day
 
 ## Recent Changes
 
+- [24-4-9-3] Ugh. It's not a real day unless you forget to test.
 - [24-4-9-2] Put back the floatable dock widgets, 'cause Wayland strikes again.
 - [24-4-9-1] Removed DockWidgetFloatable from the dock widgets since my wee brain can't figure out how to add a dragable window frame to them once they are floating. Added a minimum size for the VFO LCD digits. Defaulted bandmap window to the right.
 - [24-4-9] Fixed Checkwindow not showing calls from logged contacts.
 - [24-4-7] Added FT8Watcher class to prep for FT8 support.
 - [24-4-4-1] Made docking widgets open state persistent.
 - [24-4-4] Added per-contest echange hint when adding new contest.
 - [24-4-2] Migrated to PyQt6. I'm sure there are broken things.
```

### Comparing `not1mm-24.4.9.2/not1mm/__main__.py` & `not1mm-24.4.9.3/not1mm/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3404,4291 +3404,4288 @@
 0000d4b0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
 0000d4c0: 6c66 2e61 6464 446f 636b 5769 6467 6574  lf.addDockWidget
 0000d4d0: 2851 742e 446f 636b 5769 6467 6574 4172  (Qt.DockWidgetAr
 0000d4e0: 6561 2e52 6967 6874 446f 636b 5769 6467  ea.RightDockWidg
 0000d4f0: 6574 4172 6561 2c20 7365 6c66 2e76 666f  etArea, self.vfo
 0000d500: 5f77 696e 646f 7729 0a20 2020 2020 2020  _window).       
 0000d510: 2020 2020 2073 656c 662e 7666 6f5f 7769       self.vfo_wi
-0000d520: 6e64 6f77 2e73 6574 5469 746c 6542 6172  ndow.setTitleBar
-0000d530: 5769 6467 6574 2831 290a 2020 2020 2020  Widget(1).      
-0000d540: 2020 2020 2020 7365 6c66 2e76 666f 5f77        self.vfo_w
-0000d550: 696e 646f 772e 7368 6f77 2829 0a0a 2020  indow.show()..  
-0000d560: 2020 6465 6620 636c 6561 725f 6261 6e64    def clear_band
-0000d570: 5f69 6e64 6963 6174 6f72 7328 7365 6c66  _indicators(self
-0000d580: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-0000d590: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
-0000d5a0: 6c65 6172 2074 6865 2069 6e64 6963 6174  lear the indicat
-0000d5b0: 6f72 732e 0a0a 2020 2020 2020 2020 5061  ors...        Pa
-0000d5c0: 7261 6d65 7465 7273 3a0a 2020 2020 2020  rameters:.      
-0000d5d0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-0000d5e0: 2020 2020 204e 6f6e 650a 0a20 2020 2020       None..     
-0000d5f0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-0000d600: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-0000d610: 2020 2020 4e6f 6e65 0a20 2020 2020 2020      None.       
-0000d620: 2022 2222 0a20 2020 2020 2020 2066 6f72   """.        for
-0000d630: 205f 2c20 696e 6469 6361 746f 7273 2069   _, indicators i
-0000d640: 6e20 7365 6c66 2e61 6c6c 5f6d 6f64 655f  n self.all_mode_
-0000d650: 696e 6469 6361 746f 7273 2e69 7465 6d73  indicators.items
-0000d660: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-0000d670: 666f 7220 5f2c 2069 6e64 6963 6174 6f72  for _, indicator
-0000d680: 2069 6e20 696e 6469 6361 746f 7273 2e69   in indicators.i
-0000d690: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
-0000d6a0: 2020 2020 2020 2020 696e 6469 6361 746f          indicato
-0000d6b0: 722e 7365 7446 7261 6d65 5368 6170 6528  r.setFrameShape(
-0000d6c0: 5174 5769 6467 6574 732e 5146 7261 6d65  QtWidgets.QFrame
-0000d6d0: 2e53 6861 7065 2e4e 6f46 7261 6d65 290a  .Shape.NoFrame).
-0000d6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6f0: 6966 2073 656c 662e 7465 7874 5f63 6f6c  if self.text_col
-0000d700: 6f72 203d 3d20 5143 6f6c 6f72 436f 6e73  or == QColorCons
-0000d710: 7461 6e74 732e 426c 6163 6b3a 0a20 2020  tants.Black:.   
+0000d520: 6e64 6f77 2e73 686f 7728 290a 0a20 2020  ndow.show()..   
+0000d530: 2064 6566 2063 6c65 6172 5f62 616e 645f   def clear_band_
+0000d540: 696e 6469 6361 746f 7273 2873 656c 6629  indicators(self)
+0000d550: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+0000d560: 2020 2222 220a 2020 2020 2020 2020 436c    """.        Cl
+0000d570: 6561 7220 7468 6520 696e 6469 6361 746f  ear the indicato
+0000d580: 7273 2e0a 0a20 2020 2020 2020 2050 6172  rs...        Par
+0000d590: 616d 6574 6572 733a 0a20 2020 2020 2020  ameters:.       
+0000d5a0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+0000d5b0: 2020 2020 4e6f 6e65 0a0a 2020 2020 2020      None..      
+0000d5c0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+0000d5d0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
+0000d5e0: 2020 204e 6f6e 650a 2020 2020 2020 2020     None.        
+0000d5f0: 2222 220a 2020 2020 2020 2020 666f 7220  """.        for 
+0000d600: 5f2c 2069 6e64 6963 6174 6f72 7320 696e  _, indicators in
+0000d610: 2073 656c 662e 616c 6c5f 6d6f 6465 5f69   self.all_mode_i
+0000d620: 6e64 6963 6174 6f72 732e 6974 656d 7328  ndicators.items(
+0000d630: 293a 0a20 2020 2020 2020 2020 2020 2066  ):.            f
+0000d640: 6f72 205f 2c20 696e 6469 6361 746f 7220  or _, indicator 
+0000d650: 696e 2069 6e64 6963 6174 6f72 732e 6974  in indicators.it
+0000d660: 656d 7328 293a 0a20 2020 2020 2020 2020  ems():.         
+0000d670: 2020 2020 2020 2069 6e64 6963 6174 6f72         indicator
+0000d680: 2e73 6574 4672 616d 6553 6861 7065 2851  .setFrameShape(Q
+0000d690: 7457 6964 6765 7473 2e51 4672 616d 652e  tWidgets.QFrame.
+0000d6a0: 5368 6170 652e 4e6f 4672 616d 6529 0a20  Shape.NoFrame). 
+0000d6b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000d6c0: 6620 7365 6c66 2e74 6578 745f 636f 6c6f  f self.text_colo
+0000d6d0: 7220 3d3d 2051 436f 6c6f 7243 6f6e 7374  r == QColorConst
+0000d6e0: 616e 7473 2e42 6c61 636b 3a0a 2020 2020  ants.Black:.    
+0000d6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d700: 696e 6469 6361 746f 722e 7365 7453 7479  indicator.setSty
+0000d710: 6c65 5368 6565 7428 0a20 2020 2020 2020  leSheet(.       
 0000d720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d730: 2069 6e64 6963 6174 6f72 2e73 6574 5374   indicator.setSt
-0000d740: 796c 6553 6865 6574 280a 2020 2020 2020  yleSheet(.      
-0000d750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d760: 2020 2266 6f6e 742d 6661 6d69 6c79 3a20    "font-family: 
-0000d770: 4a65 7442 7261 696e 7320 4d6f 6e6f 3b20  JetBrains Mono; 
-0000d780: 636f 6c6f 723a 2062 6c61 636b 3b22 0a20  color: black;". 
-0000d790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d7a0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0000d7b0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000d7c0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000d7d0: 6e64 6963 6174 6f72 2e73 6574 5374 796c  ndicator.setStyl
-0000d7e0: 6553 6865 6574 2822 666f 6e74 2d66 616d  eSheet("font-fam
-0000d7f0: 696c 793a 204a 6574 4272 6169 6e73 204d  ily: JetBrains M
-0000d800: 6f6e 6f3b 2063 6f6c 6f72 3a20 7768 6974  ono; color: whit
-0000d810: 6522 290a 0a20 2020 2064 6566 2073 6574  e")..    def set
-0000d820: 5f62 616e 645f 696e 6469 6361 746f 7228  _band_indicator(
-0000d830: 7365 6c66 2c20 6261 6e64 3a20 7374 7229  self, band: str)
-0000d840: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-0000d850: 2020 2222 220a 2020 2020 2020 2020 5365    """.        Se
-0000d860: 7420 7468 6520 6261 6e64 2069 6e64 6963  t the band indic
-0000d870: 6174 6f72 0a0a 2020 2020 2020 2020 5061  ator..        Pa
-0000d880: 7261 6d65 7465 7273 3a0a 2020 2020 2020  rameters:.      
-0000d890: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-0000d8a0: 2020 2020 2062 616e 643a 2073 7472 0a20       band: str. 
-0000d8b0: 2020 2020 2020 2062 616e 6420 746f 2073         band to s
-0000d8c0: 6574 2069 6e64 6963 6174 6f72 2066 6f72  et indicator for
-0000d8d0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-0000d8e0: 733a 0a20 2020 2020 2020 202d 2d2d 2d2d  s:.        -----
-0000d8f0: 2d2d 0a20 2020 2020 2020 204e 6f6e 650a  --.        None.
-0000d900: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
-0000d910: 2020 2020 2069 6620 6261 6e64 2061 6e64       if band and
-0000d920: 2073 656c 662e 6375 7272 656e 745f 6d6f   self.current_mo
-0000d930: 6465 3a0a 2020 2020 2020 2020 2020 2020  de:.            
-0000d940: 7365 6c66 2e63 6c65 6172 5f62 616e 645f  self.clear_band_
-0000d950: 696e 6469 6361 746f 7273 2829 0a20 2020  indicators().   
-0000d960: 2020 2020 2020 2020 2069 6e64 6963 6174           indicat
-0000d970: 6f72 203d 2073 656c 662e 616c 6c5f 6d6f  or = self.all_mo
-0000d980: 6465 5f69 6e64 6963 6174 6f72 735b 7365  de_indicators[se
-0000d990: 6c66 2e63 7572 7265 6e74 5f6d 6f64 655d  lf.current_mode]
-0000d9a0: 2e67 6574 2862 616e 642c 204e 6f6e 6529  .get(band, None)
-0000d9b0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000d9c0: 696e 6469 6361 746f 723a 0a20 2020 2020  indicator:.     
-0000d9d0: 2020 2020 2020 2020 2020 2069 6e64 6963             indic
-0000d9e0: 6174 6f72 2e73 6574 4672 616d 6553 6861  ator.setFrameSha
-0000d9f0: 7065 2851 7457 6964 6765 7473 2e51 4672  pe(QtWidgets.QFr
-0000da00: 616d 652e 5368 6170 652e 426f 7829 0a20  ame.Shape.Box). 
-0000da10: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000da20: 6e64 6963 6174 6f72 2e73 6574 5374 796c  ndicator.setStyl
-0000da30: 6553 6865 6574 2822 666f 6e74 2d66 616d  eSheet("font-fam
-0000da40: 696c 793a 204a 6574 4272 6169 6e73 204d  ily: JetBrains M
-0000da50: 6f6e 6f3b 2063 6f6c 6f72 3a20 6772 6565  ono; color: gree
-0000da60: 6e3b 2229 0a0a 2020 2020 6465 6620 636c  n;")..    def cl
-0000da70: 6f73 6545 7665 6e74 2873 656c 662c 205f  oseEvent(self, _
-0000da80: 6576 656e 7429 202d 3e20 4e6f 6e65 3a0a  event) -> None:.
-0000da90: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000daa0: 2020 2020 5772 6974 6520 7769 6e64 6f77      Write window
-0000dab0: 2073 697a 6520 616e 6420 706f 7369 7469   size and positi
-0000dac0: 6f6e 2074 6f20 636f 6e66 6967 2066 696c  on to config fil
-0000dad0: 652e 0a0a 2020 2020 2020 2020 5061 7261  e...        Para
-0000dae0: 6d65 7465 7273 3a0a 2020 2020 2020 2020  meters:.        
-0000daf0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-0000db00: 2020 205f 6576 656e 743a 2051 436c 6f73     _event: QClos
-0000db10: 6545 7665 6e74 0a0a 2020 2020 2020 2020  eEvent..        
-0000db20: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-0000db30: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
-0000db40: 204e 6f6e 650a 2020 2020 2020 2020 2222   None.        ""
-0000db50: 220a 0a20 2020 2020 2020 2063 6d64 203d  "..        cmd =
-0000db60: 207b 7d0a 2020 2020 2020 2020 636d 645b   {}.        cmd[
-0000db70: 2263 6d64 225d 203d 2022 4841 4c54 220a  "cmd"] = "HALT".
-0000db80: 2020 2020 2020 2020 636d 645b 2273 7461          cmd["sta
-0000db90: 7469 6f6e 225d 203d 2070 6c61 7466 6f72  tion"] = platfor
-0000dba0: 6d2e 6e6f 6465 2829 0a20 2020 2020 2020  m.node().       
-0000dbb0: 2073 656c 662e 6d75 6c74 6963 6173 745f   self.multicast_
-0000dbc0: 696e 7465 7266 6163 652e 7365 6e64 5f61  interface.send_a
-0000dbd0: 735f 6a73 6f6e 2863 6d64 290a 2020 2020  s_json(cmd).    
-0000dbe0: 2020 2020 7365 6c66 2e70 7265 665b 2277      self.pref["w
-0000dbf0: 696e 646f 775f 7769 6474 6822 5d20 3d20  indow_width"] = 
-0000dc00: 7365 6c66 2e73 697a 6528 292e 7769 6474  self.size().widt
-0000dc10: 6828 290a 2020 2020 2020 2020 7365 6c66  h().        self
-0000dc20: 2e70 7265 665b 2277 696e 646f 775f 6865  .pref["window_he
-0000dc30: 6967 6874 225d 203d 2073 656c 662e 7369  ight"] = self.si
-0000dc40: 7a65 2829 2e68 6569 6768 7428 290a 2020  ze().height().  
-0000dc50: 2020 2020 2020 7365 6c66 2e70 7265 665b        self.pref[
-0000dc60: 2277 696e 646f 775f 7822 5d20 3d20 7365  "window_x"] = se
-0000dc70: 6c66 2e70 6f73 2829 2e78 2829 0a20 2020  lf.pos().x().   
-0000dc80: 2020 2020 2073 656c 662e 7072 6566 5b22       self.pref["
-0000dc90: 7769 6e64 6f77 5f79 225d 203d 2073 656c  window_y"] = sel
-0000dca0: 662e 706f 7328 292e 7928 290a 2020 2020  f.pos().y().    
-0000dcb0: 2020 2020 7365 6c66 2e77 7269 7465 5f70      self.write_p
-0000dcc0: 7265 6665 7265 6e63 6528 290a 0a20 2020  reference()..   
-0000dcd0: 2064 6566 2063 7479 5f6c 6f6f 6b75 7028   def cty_lookup(
-0000dce0: 7365 6c66 2c20 6361 6c6c 7369 676e 3a20  self, callsign: 
-0000dcf0: 7374 7229 202d 3e20 6c69 7374 3a0a 2020  str) -> list:.  
-0000dd00: 2020 2020 2020 2222 224c 6f6f 6b75 7020        """Lookup 
-0000dd10: 6361 6c6c 7369 676e 2069 6e20 6374 792e  callsign in cty.
-0000dd20: 6461 7420 6669 6c65 2e0a 0a20 2020 2020  dat file...     
-0000dd30: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-0000dd40: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-0000dd50: 0a20 2020 2020 2020 2063 616c 6c73 6967  .        callsig
-0000dd60: 6e20 3a20 7374 720a 2020 2020 2020 2020  n : str.        
-0000dd70: 6361 6c6c 7369 676e 2074 6f20 6c6f 6f6b  callsign to look
-0000dd80: 7570 0a0a 2020 2020 2020 2020 5265 7475  up..        Retu
-0000dd90: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
-0000dda0: 2d2d 2d0a 2020 2020 2020 2020 7265 7475  ---.        retu
-0000ddb0: 726e 203a 206c 6973 740a 2020 2020 2020  rn : list.      
-0000ddc0: 2020 6c69 7374 206f 6620 6469 6374 7320    list of dicts 
-0000ddd0: 636f 6e74 6169 6e69 6e67 2074 6865 2063  containing the c
-0000dde0: 616c 6c73 6967 6e20 616e 6420 7468 6520  allsign and the 
-0000ddf0: 7374 6174 696f 6e2e 0a20 2020 2020 2020  station..       
-0000de00: 2022 2222 0a20 2020 2020 2020 2063 616c   """.        cal
-0000de10: 6c73 6967 6e20 3d20 6361 6c6c 7369 676e  lsign = callsign
-0000de20: 2e75 7070 6572 2829 0a20 2020 2020 2020  .upper().       
-0000de30: 2066 6f72 2063 6f75 6e74 2069 6e20 7265   for count in re
-0000de40: 7665 7273 6564 2872 616e 6765 286c 656e  versed(range(len
-0000de50: 2863 616c 6c73 6967 6e29 2929 3a0a 2020  (callsign))):.  
-0000de60: 2020 2020 2020 2020 2020 7365 6172 6368            search
-0000de70: 6974 656d 203d 2063 616c 6c73 6967 6e5b  item = callsign[
-0000de80: 3a20 636f 756e 7420 2b20 315d 0a20 2020  : count + 1].   
-0000de90: 2020 2020 2020 2020 2072 6573 756c 7420           result 
-0000dea0: 3d20 7b6b 6579 3a20 7661 6c20 666f 7220  = {key: val for 
-0000deb0: 6b65 792c 2076 616c 2069 6e20 4354 5946  key, val in CTYF
-0000dec0: 494c 452e 6974 656d 7328 2920 6966 206b  ILE.items() if k
-0000ded0: 6579 203d 3d20 7365 6172 6368 6974 656d  ey == searchitem
-0000dee0: 7d0a 2020 2020 2020 2020 2020 2020 6966  }.            if
-0000def0: 206e 6f74 2072 6573 756c 743a 0a20 2020   not result:.   
-0000df00: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-0000df10: 7469 6e75 650a 2020 2020 2020 2020 2020  tinue.          
-0000df20: 2020 6966 2072 6573 756c 742e 6765 7428    if result.get(
-0000df30: 7365 6172 6368 6974 656d 292e 6765 7428  searchitem).get(
-0000df40: 2265 7861 6374 5f6d 6174 6368 2229 3a0a  "exact_match"):.
-0000df50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df60: 6966 2073 6561 7263 6869 7465 6d20 3d3d  if searchitem ==
-0000df70: 2063 616c 6c73 6967 6e3a 0a20 2020 2020   callsign:.     
-0000df80: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000df90: 6574 7572 6e20 7265 7375 6c74 0a20 2020  eturn result.   
-0000dfa0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-0000dfb0: 7469 6e75 650a 2020 2020 2020 2020 2020  tinue.          
-0000dfc0: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-0000dfd0: 0a20 2020 2064 6566 2063 7773 7065 6564  .    def cwspeed
-0000dfe0: 5f73 7069 6e62 6f78 5f63 6861 6e67 6564  _spinbox_changed
-0000dff0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-0000e000: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000e010: 2020 2020 5472 6967 6765 7265 6420 7768      Triggered wh
-0000e020: 656e 2076 616c 7565 206f 6620 4357 2073  en value of CW s
-0000e030: 7065 6564 2069 6e20 7468 6520 7370 696e  peed in the spin
-0000e040: 626f 7820 6368 616e 6765 732e 0a0a 2020  box changes...  
-0000e050: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-0000e060: 3a0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  :.        ------
-0000e070: 2d2d 2d2d 0a20 2020 2020 2020 204e 6f6e  ----.        Non
-0000e080: 650a 0a20 2020 2020 2020 2052 6574 7572  e..        Retur
-0000e090: 6e73 3a0a 2020 2020 2020 2020 2d2d 2d2d  ns:.        ----
-0000e0a0: 2d2d 2d0a 2020 2020 2020 2020 4e6f 6e65  ---.        None
-0000e0b0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000e0c0: 2020 2020 2069 6620 7365 6c66 2e63 7720       if self.cw 
-0000e0d0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-0000e0e0: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-0000e0f0: 2020 2020 6966 2073 656c 662e 6377 2e73      if self.cw.s
-0000e100: 6572 7665 7274 7970 6520 3d3d 2031 3a0a  ervertype == 1:.
-0000e110: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000e120: 2e63 772e 7370 6565 6420 3d20 7365 6c66  .cw.speed = self
-0000e130: 2e63 775f 7370 6565 642e 7661 6c75 6528  .cw_speed.value(
-0000e140: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-0000e150: 6c66 2e63 772e 7365 6e64 6377 2866 225c  lf.cw.sendcw(f"\
-0000e160: 7831 6232 7b73 656c 662e 6377 2e73 7065  x1b2{self.cw.spe
-0000e170: 6564 7d22 290a 2020 2020 2020 2020 6966  ed}").        if
-0000e180: 2073 656c 662e 6377 2e73 6572 7665 7274   self.cw.servert
-0000e190: 7970 6520 3d3d 2032 3a0a 2020 2020 2020  ype == 2:.      
-0000e1a0: 2020 2020 2020 7365 6c66 2e63 772e 7365        self.cw.se
-0000e1b0: 745f 7769 6e6b 6579 6572 5f73 7065 6564  t_winkeyer_speed
-0000e1c0: 2873 656c 662e 6377 5f73 7065 6564 2e76  (self.cw_speed.v
-0000e1d0: 616c 7565 2829 290a 0a20 2020 2064 6566  alue())..    def
-0000e1e0: 206b 6579 5072 6573 7345 7665 6e74 2873   keyPressEvent(s
-0000e1f0: 656c 662c 2065 7665 6e74 2920 2d3e 204e  elf, event) -> N
-0000e200: 6f6e 653a 2020 2320 7079 6c69 6e74 3a20  one:  # pylint: 
-0000e210: 6469 7361 626c 653d 696e 7661 6c69 642d  disable=invalid-
-0000e220: 6e61 6d65 0a20 2020 2020 2020 2022 2222  name.        """
-0000e230: 0a20 2020 2020 2020 2054 6869 7320 6f76  .        This ov
-0000e240: 6572 7269 6465 7320 5174 206b 6579 2065  errides Qt key e
-0000e250: 7665 6e74 2e0a 0a20 2020 2020 2020 2050  vent...        P
-0000e260: 6172 616d 6574 6572 733a 0a20 2020 2020  arameters:.     
-0000e270: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-0000e280: 2020 2020 2020 6576 656e 743a 2051 4b65        event: QKe
-0000e290: 7945 7665 6e74 0a20 2020 2020 2020 2051  yEvent.        Q
-0000e2a0: 7420 6b65 7920 6576 656e 740a 0a20 2020  t key event..   
-0000e2b0: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-0000e2c0: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
-0000e2d0: 2020 2020 2020 4e6f 6e65 0a20 2020 2020        None.     
-0000e2e0: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
-0000e2f0: 6d6f 6469 6669 6572 203d 2065 7665 6e74  modifier = event
-0000e300: 2e6d 6f64 6966 6965 7273 2829 0a20 2020  .modifiers().   
-0000e310: 2020 2020 2069 6620 6576 656e 742e 6b65       if event.ke
-0000e320: 7928 2920 3d3d 2051 742e 4b65 792e 4b65  y() == Qt.Key.Ke
-0000e330: 795f 4b3a 0a20 2020 2020 2020 2020 2020  y_K:.           
-0000e340: 2073 656c 662e 746f 6767 6c65 5f63 775f   self.toggle_cw_
-0000e350: 656e 7472 7928 290a 2020 2020 2020 2020  entry().        
-0000e360: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-0000e370: 2020 2069 6620 280a 2020 2020 2020 2020     if (.        
-0000e380: 2020 2020 6576 656e 742e 6b65 7928 2920      event.key() 
-0000e390: 3d3d 2051 742e 4b65 792e 4b65 795f 530a  == Qt.Key.Key_S.
-0000e3a0: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-0000e3b0: 6d6f 6469 6669 6572 203d 3d20 5174 2e4b  modifier == Qt.K
-0000e3c0: 6579 626f 6172 644d 6f64 6966 6965 722e  eyboardModifier.
-0000e3d0: 436f 6e74 726f 6c4d 6f64 6966 6965 720a  ControlModifier.
-0000e3e0: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
-0000e3f0: 2020 2020 2020 2066 7265 7120 3d20 7365         freq = se
-0000e400: 6c66 2e72 6164 696f 5f73 7461 7465 2e67  lf.radio_state.g
-0000e410: 6574 2822 7666 6f61 2229 0a20 2020 2020  et("vfoa").     
-0000e420: 2020 2020 2020 2064 7820 3d20 7365 6c66         dx = self
-0000e430: 2e63 616c 6c73 6967 6e2e 7465 7874 2829  .callsign.text()
-0000e440: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000e450: 6672 6571 2061 6e64 2064 783a 0a20 2020  freq and dx:.   
-0000e460: 2020 2020 2020 2020 2020 2020 2063 6d64               cmd
-0000e470: 203d 207b 7d0a 2020 2020 2020 2020 2020   = {}.          
-0000e480: 2020 2020 2020 636d 645b 2263 6d64 225d        cmd["cmd"]
-0000e490: 203d 2022 5350 4f54 4458 220a 2020 2020   = "SPOTDX".    
+0000d730: 2022 666f 6e74 2d66 616d 696c 793a 204a   "font-family: J
+0000d740: 6574 4272 6169 6e73 204d 6f6e 6f3b 2063  etBrains Mono; c
+0000d750: 6f6c 6f72 3a20 626c 6163 6b3b 220a 2020  olor: black;".  
+0000d760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d770: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0000d780: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000d790: 2020 2020 2020 2020 2020 2020 2020 696e                in
+0000d7a0: 6469 6361 746f 722e 7365 7453 7479 6c65  dicator.setStyle
+0000d7b0: 5368 6565 7428 2266 6f6e 742d 6661 6d69  Sheet("font-fami
+0000d7c0: 6c79 3a20 4a65 7442 7261 696e 7320 4d6f  ly: JetBrains Mo
+0000d7d0: 6e6f 3b20 636f 6c6f 723a 2077 6869 7465  no; color: white
+0000d7e0: 2229 0a0a 2020 2020 6465 6620 7365 745f  ")..    def set_
+0000d7f0: 6261 6e64 5f69 6e64 6963 6174 6f72 2873  band_indicator(s
+0000d800: 656c 662c 2062 616e 643a 2073 7472 2920  elf, band: str) 
+0000d810: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+0000d820: 2022 2222 0a20 2020 2020 2020 2053 6574   """.        Set
+0000d830: 2074 6865 2062 616e 6420 696e 6469 6361   the band indica
+0000d840: 746f 720a 0a20 2020 2020 2020 2050 6172  tor..        Par
+0000d850: 616d 6574 6572 733a 0a20 2020 2020 2020  ameters:.       
+0000d860: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+0000d870: 2020 2020 6261 6e64 3a20 7374 720a 2020      band: str.  
+0000d880: 2020 2020 2020 6261 6e64 2074 6f20 7365        band to se
+0000d890: 7420 696e 6469 6361 746f 7220 666f 720a  t indicator for.
+0000d8a0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+0000d8b0: 3a0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  :.        ------
+0000d8c0: 2d0a 2020 2020 2020 2020 4e6f 6e65 0a20  -.        None. 
+0000d8d0: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
+0000d8e0: 2020 2020 6966 2062 616e 6420 616e 6420      if band and 
+0000d8f0: 7365 6c66 2e63 7572 7265 6e74 5f6d 6f64  self.current_mod
+0000d900: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0000d910: 656c 662e 636c 6561 725f 6261 6e64 5f69  elf.clear_band_i
+0000d920: 6e64 6963 6174 6f72 7328 290a 2020 2020  ndicators().    
+0000d930: 2020 2020 2020 2020 696e 6469 6361 746f          indicato
+0000d940: 7220 3d20 7365 6c66 2e61 6c6c 5f6d 6f64  r = self.all_mod
+0000d950: 655f 696e 6469 6361 746f 7273 5b73 656c  e_indicators[sel
+0000d960: 662e 6375 7272 656e 745f 6d6f 6465 5d2e  f.current_mode].
+0000d970: 6765 7428 6261 6e64 2c20 4e6f 6e65 290a  get(band, None).
+0000d980: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+0000d990: 6e64 6963 6174 6f72 3a0a 2020 2020 2020  ndicator:.      
+0000d9a0: 2020 2020 2020 2020 2020 696e 6469 6361            indica
+0000d9b0: 746f 722e 7365 7446 7261 6d65 5368 6170  tor.setFrameShap
+0000d9c0: 6528 5174 5769 6467 6574 732e 5146 7261  e(QtWidgets.QFra
+0000d9d0: 6d65 2e53 6861 7065 2e42 6f78 290a 2020  me.Shape.Box).  
+0000d9e0: 2020 2020 2020 2020 2020 2020 2020 696e                in
+0000d9f0: 6469 6361 746f 722e 7365 7453 7479 6c65  dicator.setStyle
+0000da00: 5368 6565 7428 2266 6f6e 742d 6661 6d69  Sheet("font-fami
+0000da10: 6c79 3a20 4a65 7442 7261 696e 7320 4d6f  ly: JetBrains Mo
+0000da20: 6e6f 3b20 636f 6c6f 723a 2067 7265 656e  no; color: green
+0000da30: 3b22 290a 0a20 2020 2064 6566 2063 6c6f  ;")..    def clo
+0000da40: 7365 4576 656e 7428 7365 6c66 2c20 5f65  seEvent(self, _e
+0000da50: 7665 6e74 2920 2d3e 204e 6f6e 653a 0a20  vent) -> None:. 
+0000da60: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000da70: 2020 2057 7269 7465 2077 696e 646f 7720     Write window 
+0000da80: 7369 7a65 2061 6e64 2070 6f73 6974 696f  size and positio
+0000da90: 6e20 746f 2063 6f6e 6669 6720 6669 6c65  n to config file
+0000daa0: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+0000dab0: 6574 6572 733a 0a20 2020 2020 2020 202d  eters:.        -
+0000dac0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+0000dad0: 2020 5f65 7665 6e74 3a20 5143 6c6f 7365    _event: QClose
+0000dae0: 4576 656e 740a 0a20 2020 2020 2020 2052  Event..        R
+0000daf0: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+0000db00: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+0000db10: 4e6f 6e65 0a20 2020 2020 2020 2022 2222  None.        """
+0000db20: 0a0a 2020 2020 2020 2020 636d 6420 3d20  ..        cmd = 
+0000db30: 7b7d 0a20 2020 2020 2020 2063 6d64 5b22  {}.        cmd["
+0000db40: 636d 6422 5d20 3d20 2248 414c 5422 0a20  cmd"] = "HALT". 
+0000db50: 2020 2020 2020 2063 6d64 5b22 7374 6174         cmd["stat
+0000db60: 696f 6e22 5d20 3d20 706c 6174 666f 726d  ion"] = platform
+0000db70: 2e6e 6f64 6528 290a 2020 2020 2020 2020  .node().        
+0000db80: 7365 6c66 2e6d 756c 7469 6361 7374 5f69  self.multicast_i
+0000db90: 6e74 6572 6661 6365 2e73 656e 645f 6173  nterface.send_as
+0000dba0: 5f6a 736f 6e28 636d 6429 0a20 2020 2020  _json(cmd).     
+0000dbb0: 2020 2073 656c 662e 7072 6566 5b22 7769     self.pref["wi
+0000dbc0: 6e64 6f77 5f77 6964 7468 225d 203d 2073  ndow_width"] = s
+0000dbd0: 656c 662e 7369 7a65 2829 2e77 6964 7468  elf.size().width
+0000dbe0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+0000dbf0: 7072 6566 5b22 7769 6e64 6f77 5f68 6569  pref["window_hei
+0000dc00: 6768 7422 5d20 3d20 7365 6c66 2e73 697a  ght"] = self.siz
+0000dc10: 6528 292e 6865 6967 6874 2829 0a20 2020  e().height().   
+0000dc20: 2020 2020 2073 656c 662e 7072 6566 5b22       self.pref["
+0000dc30: 7769 6e64 6f77 5f78 225d 203d 2073 656c  window_x"] = sel
+0000dc40: 662e 706f 7328 292e 7828 290a 2020 2020  f.pos().x().    
+0000dc50: 2020 2020 7365 6c66 2e70 7265 665b 2277      self.pref["w
+0000dc60: 696e 646f 775f 7922 5d20 3d20 7365 6c66  indow_y"] = self
+0000dc70: 2e70 6f73 2829 2e79 2829 0a20 2020 2020  .pos().y().     
+0000dc80: 2020 2073 656c 662e 7772 6974 655f 7072     self.write_pr
+0000dc90: 6566 6572 656e 6365 2829 0a0a 2020 2020  eference()..    
+0000dca0: 6465 6620 6374 795f 6c6f 6f6b 7570 2873  def cty_lookup(s
+0000dcb0: 656c 662c 2063 616c 6c73 6967 6e3a 2073  elf, callsign: s
+0000dcc0: 7472 2920 2d3e 206c 6973 743a 0a20 2020  tr) -> list:.   
+0000dcd0: 2020 2020 2022 2222 4c6f 6f6b 7570 2063       """Lookup c
+0000dce0: 616c 6c73 6967 6e20 696e 2063 7479 2e64  allsign in cty.d
+0000dcf0: 6174 2066 696c 652e 0a0a 2020 2020 2020  at file...      
+0000dd00: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+0000dd10: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
+0000dd20: 2020 2020 2020 2020 6361 6c6c 7369 676e          callsign
+0000dd30: 203a 2073 7472 0a20 2020 2020 2020 2063   : str.        c
+0000dd40: 616c 6c73 6967 6e20 746f 206c 6f6f 6b75  allsign to looku
+0000dd50: 700a 0a20 2020 2020 2020 2052 6574 7572  p..        Retur
+0000dd60: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
+0000dd70: 2d2d 0a20 2020 2020 2020 2072 6574 7572  --.        retur
+0000dd80: 6e20 3a20 6c69 7374 0a20 2020 2020 2020  n : list.       
+0000dd90: 206c 6973 7420 6f66 2064 6963 7473 2063   list of dicts c
+0000dda0: 6f6e 7461 696e 696e 6720 7468 6520 6361  ontaining the ca
+0000ddb0: 6c6c 7369 676e 2061 6e64 2074 6865 2073  llsign and the s
+0000ddc0: 7461 7469 6f6e 2e0a 2020 2020 2020 2020  tation..        
+0000ddd0: 2222 220a 2020 2020 2020 2020 6361 6c6c  """.        call
+0000dde0: 7369 676e 203d 2063 616c 6c73 6967 6e2e  sign = callsign.
+0000ddf0: 7570 7065 7228 290a 2020 2020 2020 2020  upper().        
+0000de00: 666f 7220 636f 756e 7420 696e 2072 6576  for count in rev
+0000de10: 6572 7365 6428 7261 6e67 6528 6c65 6e28  ersed(range(len(
+0000de20: 6361 6c6c 7369 676e 2929 293a 0a20 2020  callsign))):.   
+0000de30: 2020 2020 2020 2020 2073 6561 7263 6869           searchi
+0000de40: 7465 6d20 3d20 6361 6c6c 7369 676e 5b3a  tem = callsign[:
+0000de50: 2063 6f75 6e74 202b 2031 5d0a 2020 2020   count + 1].    
+0000de60: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+0000de70: 207b 6b65 793a 2076 616c 2066 6f72 206b   {key: val for k
+0000de80: 6579 2c20 7661 6c20 696e 2043 5459 4649  ey, val in CTYFI
+0000de90: 4c45 2e69 7465 6d73 2829 2069 6620 6b65  LE.items() if ke
+0000dea0: 7920 3d3d 2073 6561 7263 6869 7465 6d7d  y == searchitem}
+0000deb0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000dec0: 6e6f 7420 7265 7375 6c74 3a0a 2020 2020  not result:.    
+0000ded0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+0000dee0: 696e 7565 0a20 2020 2020 2020 2020 2020  inue.           
+0000def0: 2069 6620 7265 7375 6c74 2e67 6574 2873   if result.get(s
+0000df00: 6561 7263 6869 7465 6d29 2e67 6574 2822  earchitem).get("
+0000df10: 6578 6163 745f 6d61 7463 6822 293a 0a20  exact_match"):. 
+0000df20: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000df30: 6620 7365 6172 6368 6974 656d 203d 3d20  f searchitem == 
+0000df40: 6361 6c6c 7369 676e 3a0a 2020 2020 2020  callsign:.      
+0000df50: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0000df60: 7475 726e 2072 6573 756c 740a 2020 2020  turn result.    
+0000df70: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+0000df80: 696e 7565 0a20 2020 2020 2020 2020 2020  inue.           
+0000df90: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+0000dfa0: 2020 2020 6465 6620 6377 7370 6565 645f      def cwspeed_
+0000dfb0: 7370 696e 626f 785f 6368 616e 6765 6428  spinbox_changed(
+0000dfc0: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
+0000dfd0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000dfe0: 2020 2054 7269 6767 6572 6564 2077 6865     Triggered whe
+0000dff0: 6e20 7661 6c75 6520 6f66 2043 5720 7370  n value of CW sp
+0000e000: 6565 6420 696e 2074 6865 2073 7069 6e62  eed in the spinb
+0000e010: 6f78 2063 6861 6e67 6573 2e0a 0a20 2020  ox changes...   
+0000e020: 2020 2020 2050 6172 616d 6574 6572 733a       Parameters:
+0000e030: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+0000e040: 2d2d 2d0a 2020 2020 2020 2020 4e6f 6e65  ---.        None
+0000e050: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+0000e060: 733a 0a20 2020 2020 2020 202d 2d2d 2d2d  s:.        -----
+0000e070: 2d2d 0a20 2020 2020 2020 204e 6f6e 650a  --.        None.
+0000e080: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000e090: 2020 2020 6966 2073 656c 662e 6377 2069      if self.cw i
+0000e0a0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+0000e0b0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+0000e0c0: 2020 2069 6620 7365 6c66 2e63 772e 7365     if self.cw.se
+0000e0d0: 7276 6572 7479 7065 203d 3d20 313a 0a20  rvertype == 1:. 
+0000e0e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000e0f0: 6377 2e73 7065 6564 203d 2073 656c 662e  cw.speed = self.
+0000e100: 6377 5f73 7065 6564 2e76 616c 7565 2829  cw_speed.value()
+0000e110: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000e120: 662e 6377 2e73 656e 6463 7728 6622 5c78  f.cw.sendcw(f"\x
+0000e130: 3162 327b 7365 6c66 2e63 772e 7370 6565  1b2{self.cw.spee
+0000e140: 647d 2229 0a20 2020 2020 2020 2069 6620  d}").        if 
+0000e150: 7365 6c66 2e63 772e 7365 7276 6572 7479  self.cw.serverty
+0000e160: 7065 203d 3d20 323a 0a20 2020 2020 2020  pe == 2:.       
+0000e170: 2020 2020 2073 656c 662e 6377 2e73 6574       self.cw.set
+0000e180: 5f77 696e 6b65 7965 725f 7370 6565 6428  _winkeyer_speed(
+0000e190: 7365 6c66 2e63 775f 7370 6565 642e 7661  self.cw_speed.va
+0000e1a0: 6c75 6528 2929 0a0a 2020 2020 6465 6620  lue())..    def 
+0000e1b0: 6b65 7950 7265 7373 4576 656e 7428 7365  keyPressEvent(se
+0000e1c0: 6c66 2c20 6576 656e 7429 202d 3e20 4e6f  lf, event) -> No
+0000e1d0: 6e65 3a20 2023 2070 796c 696e 743a 2064  ne:  # pylint: d
+0000e1e0: 6973 6162 6c65 3d69 6e76 616c 6964 2d6e  isable=invalid-n
+0000e1f0: 616d 650a 2020 2020 2020 2020 2222 220a  ame.        """.
+0000e200: 2020 2020 2020 2020 5468 6973 206f 7665          This ove
+0000e210: 7272 6964 6573 2051 7420 6b65 7920 6576  rrides Qt key ev
+0000e220: 656e 742e 0a0a 2020 2020 2020 2020 5061  ent...        Pa
+0000e230: 7261 6d65 7465 7273 3a0a 2020 2020 2020  rameters:.      
+0000e240: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+0000e250: 2020 2020 2065 7665 6e74 3a20 514b 6579       event: QKey
+0000e260: 4576 656e 740a 2020 2020 2020 2020 5174  Event.        Qt
+0000e270: 206b 6579 2065 7665 6e74 0a0a 2020 2020   key event..    
+0000e280: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+0000e290: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
+0000e2a0: 2020 2020 204e 6f6e 650a 2020 2020 2020       None.      
+0000e2b0: 2020 2222 220a 0a20 2020 2020 2020 206d    """..        m
+0000e2c0: 6f64 6966 6965 7220 3d20 6576 656e 742e  odifier = event.
+0000e2d0: 6d6f 6469 6669 6572 7328 290a 2020 2020  modifiers().    
+0000e2e0: 2020 2020 6966 2065 7665 6e74 2e6b 6579      if event.key
+0000e2f0: 2829 203d 3d20 5174 2e4b 6579 2e4b 6579  () == Qt.Key.Key
+0000e300: 5f4b 3a0a 2020 2020 2020 2020 2020 2020  _K:.            
+0000e310: 7365 6c66 2e74 6f67 676c 655f 6377 5f65  self.toggle_cw_e
+0000e320: 6e74 7279 2829 0a20 2020 2020 2020 2020  ntry().         
+0000e330: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+0000e340: 2020 6966 2028 0a20 2020 2020 2020 2020    if (.         
+0000e350: 2020 2065 7665 6e74 2e6b 6579 2829 203d     event.key() =
+0000e360: 3d20 5174 2e4b 6579 2e4b 6579 5f53 0a20  = Qt.Key.Key_S. 
+0000e370: 2020 2020 2020 2020 2020 2061 6e64 206d             and m
+0000e380: 6f64 6966 6965 7220 3d3d 2051 742e 4b65  odifier == Qt.Ke
+0000e390: 7962 6f61 7264 4d6f 6469 6669 6572 2e43  yboardModifier.C
+0000e3a0: 6f6e 7472 6f6c 4d6f 6469 6669 6572 0a20  ontrolModifier. 
+0000e3b0: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
+0000e3c0: 2020 2020 2020 6672 6571 203d 2073 656c        freq = sel
+0000e3d0: 662e 7261 6469 6f5f 7374 6174 652e 6765  f.radio_state.ge
+0000e3e0: 7428 2276 666f 6122 290a 2020 2020 2020  t("vfoa").      
+0000e3f0: 2020 2020 2020 6478 203d 2073 656c 662e        dx = self.
+0000e400: 6361 6c6c 7369 676e 2e74 6578 7428 290a  callsign.text().
+0000e410: 2020 2020 2020 2020 2020 2020 6966 2066              if f
+0000e420: 7265 7120 616e 6420 6478 3a0a 2020 2020  req and dx:.    
+0000e430: 2020 2020 2020 2020 2020 2020 636d 6420              cmd 
+0000e440: 3d20 7b7d 0a20 2020 2020 2020 2020 2020  = {}.           
+0000e450: 2020 2020 2063 6d64 5b22 636d 6422 5d20       cmd["cmd"] 
+0000e460: 3d20 2253 504f 5444 5822 0a20 2020 2020  = "SPOTDX".     
+0000e470: 2020 2020 2020 2020 2020 2063 6d64 5b22             cmd["
+0000e480: 7374 6174 696f 6e22 5d20 3d20 706c 6174  station"] = plat
+0000e490: 666f 726d 2e6e 6f64 6528 290a 2020 2020  form.node().    
 0000e4a0: 2020 2020 2020 2020 2020 2020 636d 645b              cmd[
-0000e4b0: 2273 7461 7469 6f6e 225d 203d 2070 6c61  "station"] = pla
-0000e4c0: 7466 6f72 6d2e 6e6f 6465 2829 0a20 2020  tform.node().   
-0000e4d0: 2020 2020 2020 2020 2020 2020 2063 6d64               cmd
-0000e4e0: 5b22 6478 225d 203d 2064 780a 2020 2020  ["dx"] = dx.    
-0000e4f0: 2020 2020 2020 2020 2020 2020 636d 645b              cmd[
-0000e500: 2266 7265 7122 5d20 3d20 666c 6f61 7428  "freq"] = float(
-0000e510: 696e 7428 6672 6571 2920 2f20 3130 3030  int(freq) / 1000
-0000e520: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000e530: 2020 7365 6c66 2e6d 756c 7469 6361 7374    self.multicast
-0000e540: 5f69 6e74 6572 6661 6365 2e73 656e 645f  _interface.send_
-0000e550: 6173 5f6a 736f 6e28 636d 6429 0a20 2020  as_json(cmd).   
-0000e560: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-0000e570: 2020 2020 2020 2020 6966 2028 0a20 2020          if (.   
-0000e580: 2020 2020 2020 2020 2065 7665 6e74 2e6b           event.k
-0000e590: 6579 2829 203d 3d20 5174 2e4b 6579 2e4b  ey() == Qt.Key.K
-0000e5a0: 6579 5f4d 0a20 2020 2020 2020 2020 2020  ey_M.           
-0000e5b0: 2061 6e64 206d 6f64 6966 6965 7220 3d3d   and modifier ==
-0000e5c0: 2051 742e 4b65 7962 6f61 7264 4d6f 6469   Qt.KeyboardModi
-0000e5d0: 6669 6572 2e43 6f6e 7472 6f6c 4d6f 6469  fier.ControlModi
-0000e5e0: 6669 6572 0a20 2020 2020 2020 2029 3a0a  fier.        ):.
-0000e5f0: 2020 2020 2020 2020 2020 2020 6672 6571              freq
-0000e600: 203d 2073 656c 662e 7261 6469 6f5f 7374   = self.radio_st
-0000e610: 6174 652e 6765 7428 2276 666f 6122 290a  ate.get("vfoa").
-0000e620: 2020 2020 2020 2020 2020 2020 6478 203d              dx =
-0000e630: 2073 656c 662e 6361 6c6c 7369 676e 2e74   self.callsign.t
-0000e640: 6578 7428 290a 2020 2020 2020 2020 2020  ext().          
-0000e650: 2020 6966 2066 7265 7120 616e 6420 6478    if freq and dx
-0000e660: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000e670: 2020 636d 6420 3d20 7b7d 0a20 2020 2020    cmd = {}.     
-0000e680: 2020 2020 2020 2020 2020 2063 6d64 5b22             cmd["
-0000e690: 636d 6422 5d20 3d20 224d 4152 4b44 5822  cmd"] = "MARKDX"
+0000e4b0: 2264 7822 5d20 3d20 6478 0a20 2020 2020  "dx"] = dx.     
+0000e4c0: 2020 2020 2020 2020 2020 2063 6d64 5b22             cmd["
+0000e4d0: 6672 6571 225d 203d 2066 6c6f 6174 2869  freq"] = float(i
+0000e4e0: 6e74 2866 7265 7129 202f 2031 3030 3029  nt(freq) / 1000)
+0000e4f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e500: 2073 656c 662e 6d75 6c74 6963 6173 745f   self.multicast_
+0000e510: 696e 7465 7266 6163 652e 7365 6e64 5f61  interface.send_a
+0000e520: 735f 6a73 6f6e 2863 6d64 290a 2020 2020  s_json(cmd).    
+0000e530: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+0000e540: 2020 2020 2020 2069 6620 280a 2020 2020         if (.    
+0000e550: 2020 2020 2020 2020 6576 656e 742e 6b65          event.ke
+0000e560: 7928 2920 3d3d 2051 742e 4b65 792e 4b65  y() == Qt.Key.Ke
+0000e570: 795f 4d0a 2020 2020 2020 2020 2020 2020  y_M.            
+0000e580: 616e 6420 6d6f 6469 6669 6572 203d 3d20  and modifier == 
+0000e590: 5174 2e4b 6579 626f 6172 644d 6f64 6966  Qt.KeyboardModif
+0000e5a0: 6965 722e 436f 6e74 726f 6c4d 6f64 6966  ier.ControlModif
+0000e5b0: 6965 720a 2020 2020 2020 2020 293a 0a20  ier.        ):. 
+0000e5c0: 2020 2020 2020 2020 2020 2066 7265 7120             freq 
+0000e5d0: 3d20 7365 6c66 2e72 6164 696f 5f73 7461  = self.radio_sta
+0000e5e0: 7465 2e67 6574 2822 7666 6f61 2229 0a20  te.get("vfoa"). 
+0000e5f0: 2020 2020 2020 2020 2020 2064 7820 3d20             dx = 
+0000e600: 7365 6c66 2e63 616c 6c73 6967 6e2e 7465  self.callsign.te
+0000e610: 7874 2829 0a20 2020 2020 2020 2020 2020  xt().           
+0000e620: 2069 6620 6672 6571 2061 6e64 2064 783a   if freq and dx:
+0000e630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e640: 2063 6d64 203d 207b 7d0a 2020 2020 2020   cmd = {}.      
+0000e650: 2020 2020 2020 2020 2020 636d 645b 2263            cmd["c
+0000e660: 6d64 225d 203d 2022 4d41 524b 4458 220a  md"] = "MARKDX".
+0000e670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e680: 636d 645b 2273 7461 7469 6f6e 225d 203d  cmd["station"] =
+0000e690: 2070 6c61 7466 6f72 6d2e 6e6f 6465 2829   platform.node()
 0000e6a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e6b0: 2063 6d64 5b22 7374 6174 696f 6e22 5d20   cmd["station"] 
-0000e6c0: 3d20 706c 6174 666f 726d 2e6e 6f64 6528  = platform.node(
-0000e6d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000e6e0: 2020 636d 645b 2264 7822 5d20 3d20 6478    cmd["dx"] = dx
-0000e6f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e700: 2063 6d64 5b22 6672 6571 225d 203d 2066   cmd["freq"] = f
-0000e710: 6c6f 6174 2869 6e74 2866 7265 7129 202f  loat(int(freq) /
-0000e720: 2031 3030 3029 0a20 2020 2020 2020 2020   1000).         
-0000e730: 2020 2020 2020 2073 656c 662e 6d75 6c74         self.mult
-0000e740: 6963 6173 745f 696e 7465 7266 6163 652e  icast_interface.
-0000e750: 7365 6e64 5f61 735f 6a73 6f6e 2863 6d64  send_as_json(cmd
-0000e760: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-0000e770: 7475 726e 0a20 2020 2020 2020 2069 6620  turn.        if 
-0000e780: 280a 2020 2020 2020 2020 2020 2020 6576  (.            ev
-0000e790: 656e 742e 6b65 7928 2920 3d3d 2051 742e  ent.key() == Qt.
-0000e7a0: 4b65 792e 4b65 795f 470a 2020 2020 2020  Key.Key_G.      
-0000e7b0: 2020 2020 2020 616e 6420 6d6f 6469 6669        and modifi
-0000e7c0: 6572 203d 3d20 5174 2e4b 6579 626f 6172  er == Qt.Keyboar
-0000e7d0: 644d 6f64 6966 6965 722e 436f 6e74 726f  dModifier.Contro
-0000e7e0: 6c4d 6f64 6966 6965 720a 2020 2020 2020  lModifier.      
-0000e7f0: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
-0000e800: 2064 7820 3d20 7365 6c66 2e63 616c 6c73   dx = self.calls
-0000e810: 6967 6e2e 7465 7874 2829 0a20 2020 2020  ign.text().     
-0000e820: 2020 2020 2020 2069 6620 6478 3a0a 2020         if dx:.  
-0000e830: 2020 2020 2020 2020 2020 2020 2020 636d                cm
-0000e840: 6420 3d20 7b7d 0a20 2020 2020 2020 2020  d = {}.         
-0000e850: 2020 2020 2020 2063 6d64 5b22 636d 6422         cmd["cmd"
-0000e860: 5d20 3d20 2246 494e 4444 5822 0a20 2020  ] = "FINDDX".   
+0000e6b0: 2063 6d64 5b22 6478 225d 203d 2064 780a   cmd["dx"] = dx.
+0000e6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e6d0: 636d 645b 2266 7265 7122 5d20 3d20 666c  cmd["freq"] = fl
+0000e6e0: 6f61 7428 696e 7428 6672 6571 2920 2f20  oat(int(freq) / 
+0000e6f0: 3130 3030 290a 2020 2020 2020 2020 2020  1000).          
+0000e700: 2020 2020 2020 7365 6c66 2e6d 756c 7469        self.multi
+0000e710: 6361 7374 5f69 6e74 6572 6661 6365 2e73  cast_interface.s
+0000e720: 656e 645f 6173 5f6a 736f 6e28 636d 6429  end_as_json(cmd)
+0000e730: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000e740: 7572 6e0a 2020 2020 2020 2020 6966 2028  urn.        if (
+0000e750: 0a20 2020 2020 2020 2020 2020 2065 7665  .            eve
+0000e760: 6e74 2e6b 6579 2829 203d 3d20 5174 2e4b  nt.key() == Qt.K
+0000e770: 6579 2e4b 6579 5f47 0a20 2020 2020 2020  ey.Key_G.       
+0000e780: 2020 2020 2061 6e64 206d 6f64 6966 6965       and modifie
+0000e790: 7220 3d3d 2051 742e 4b65 7962 6f61 7264  r == Qt.Keyboard
+0000e7a0: 4d6f 6469 6669 6572 2e43 6f6e 7472 6f6c  Modifier.Control
+0000e7b0: 4d6f 6469 6669 6572 0a20 2020 2020 2020  Modifier.       
+0000e7c0: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
+0000e7d0: 6478 203d 2073 656c 662e 6361 6c6c 7369  dx = self.callsi
+0000e7e0: 676e 2e74 6578 7428 290a 2020 2020 2020  gn.text().      
+0000e7f0: 2020 2020 2020 6966 2064 783a 0a20 2020        if dx:.   
+0000e800: 2020 2020 2020 2020 2020 2020 2063 6d64               cmd
+0000e810: 203d 207b 7d0a 2020 2020 2020 2020 2020   = {}.          
+0000e820: 2020 2020 2020 636d 645b 2263 6d64 225d        cmd["cmd"]
+0000e830: 203d 2022 4649 4e44 4458 220a 2020 2020   = "FINDDX".    
+0000e840: 2020 2020 2020 2020 2020 2020 636d 645b              cmd[
+0000e850: 2273 7461 7469 6f6e 225d 203d 2070 6c61  "station"] = pla
+0000e860: 7466 6f72 6d2e 6e6f 6465 2829 0a20 2020  tform.node().   
 0000e870: 2020 2020 2020 2020 2020 2020 2063 6d64               cmd
-0000e880: 5b22 7374 6174 696f 6e22 5d20 3d20 706c  ["station"] = pl
-0000e890: 6174 666f 726d 2e6e 6f64 6528 290a 2020  atform.node().  
-0000e8a0: 2020 2020 2020 2020 2020 2020 2020 636d                cm
-0000e8b0: 645b 2264 7822 5d20 3d20 6478 0a20 2020  d["dx"] = dx.   
-0000e8c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000e8d0: 662e 6d75 6c74 6963 6173 745f 696e 7465  f.multicast_inte
-0000e8e0: 7266 6163 652e 7365 6e64 5f61 735f 6a73  rface.send_as_js
-0000e8f0: 6f6e 2863 6d64 290a 2020 2020 2020 2020  on(cmd).        
-0000e900: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-0000e910: 2020 2069 6620 280a 2020 2020 2020 2020     if (.        
-0000e920: 2020 2020 6576 656e 742e 6b65 7928 2920      event.key() 
-0000e930: 3d3d 2051 742e 4b65 792e 4b65 795f 4573  == Qt.Key.Key_Es
-0000e940: 6361 7065 0a20 2020 2020 2020 2020 2020  cape.           
-0000e950: 2061 6e64 206d 6f64 6966 6965 7220 213d   and modifier !=
-0000e960: 2051 742e 4b65 7962 6f61 7264 4d6f 6469   Qt.KeyboardModi
-0000e970: 6669 6572 2e43 6f6e 7472 6f6c 4d6f 6469  fier.ControlModi
-0000e980: 6669 6572 0a20 2020 2020 2020 2029 3a20  fier.        ): 
-0000e990: 2023 2070 796c 696e 743a 2064 6973 6162   # pylint: disab
-0000e9a0: 6c65 3d6e 6f2d 6d65 6d62 6572 0a20 2020  le=no-member.   
-0000e9b0: 2020 2020 2020 2020 2073 656c 662e 636c           self.cl
-0000e9c0: 6561 7269 6e70 7574 7328 290a 2020 2020  earinputs().    
-0000e9d0: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-0000e9e0: 2020 2020 2020 2069 6620 280a 2020 2020         if (.    
-0000e9f0: 2020 2020 2020 2020 6576 656e 742e 6b65          event.ke
-0000ea00: 7928 2920 3d3d 2051 742e 4b65 792e 4b65  y() == Qt.Key.Ke
-0000ea10: 795f 4573 6361 7065 0a20 2020 2020 2020  y_Escape.       
-0000ea20: 2020 2020 2061 6e64 206d 6f64 6966 6965       and modifie
-0000ea30: 7220 3d3d 2051 742e 4b65 7962 6f61 7264  r == Qt.Keyboard
-0000ea40: 4d6f 6469 6669 6572 2e43 6f6e 7472 6f6c  Modifier.Control
-0000ea50: 4d6f 6469 6669 6572 0a20 2020 2020 2020  Modifier.       
-0000ea60: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
-0000ea70: 6966 2073 656c 662e 6377 2069 7320 6e6f  if self.cw is no
-0000ea80: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0000ea90: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000eaa0: 6377 2e73 6572 7665 7274 7970 6520 3d3d  cw.servertype ==
-0000eab0: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
-0000eac0: 2020 2020 2020 2020 7365 6c66 2e63 772e          self.cw.
-0000ead0: 7365 6e64 6377 2822 5c78 3162 3422 290a  sendcw("\x1b4").
-0000eae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eaf0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-0000eb00: 2020 2069 6620 6576 656e 742e 6b65 7928     if event.key(
-0000eb10: 2920 3d3d 2051 742e 4b65 792e 4b65 795f  ) == Qt.Key.Key_
-0000eb20: 5570 3a0a 2020 2020 2020 2020 2020 2020  Up:.            
-0000eb30: 636d 6420 3d20 7b7d 0a20 2020 2020 2020  cmd = {}.       
-0000eb40: 2020 2020 2063 6d64 5b22 636d 6422 5d20       cmd["cmd"] 
-0000eb50: 3d20 2250 5245 5653 504f 5422 0a20 2020  = "PREVSPOT".   
-0000eb60: 2020 2020 2020 2020 2063 6d64 5b22 7374           cmd["st
-0000eb70: 6174 696f 6e22 5d20 3d20 706c 6174 666f  ation"] = platfo
-0000eb80: 726d 2e6e 6f64 6528 290a 2020 2020 2020  rm.node().      
-0000eb90: 2020 2020 2020 7365 6c66 2e6d 756c 7469        self.multi
-0000eba0: 6361 7374 5f69 6e74 6572 6661 6365 2e73  cast_interface.s
-0000ebb0: 656e 645f 6173 5f6a 736f 6e28 636d 6429  end_as_json(cmd)
-0000ebc0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000ebd0: 7572 6e0a 2020 2020 2020 2020 6966 2065  urn.        if e
-0000ebe0: 7665 6e74 2e6b 6579 2829 203d 3d20 5174  vent.key() == Qt
-0000ebf0: 2e4b 6579 2e4b 6579 5f44 6f77 6e3a 0a20  .Key.Key_Down:. 
-0000ec00: 2020 2020 2020 2020 2020 2063 6d64 203d             cmd =
-0000ec10: 207b 7d0a 2020 2020 2020 2020 2020 2020   {}.            
-0000ec20: 636d 645b 2263 6d64 225d 203d 2022 4e45  cmd["cmd"] = "NE
-0000ec30: 5854 5350 4f54 220a 2020 2020 2020 2020  XTSPOT".        
-0000ec40: 2020 2020 636d 645b 2273 7461 7469 6f6e      cmd["station
-0000ec50: 225d 203d 2070 6c61 7466 6f72 6d2e 6e6f  "] = platform.no
-0000ec60: 6465 2829 0a20 2020 2020 2020 2020 2020  de().           
-0000ec70: 2073 656c 662e 6d75 6c74 6963 6173 745f   self.multicast_
-0000ec80: 696e 7465 7266 6163 652e 7365 6e64 5f61  interface.send_a
-0000ec90: 735f 6a73 6f6e 2863 6d64 290a 2020 2020  s_json(cmd).    
-0000eca0: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-0000ecb0: 2020 2020 2020 2069 6620 280a 2020 2020         if (.    
-0000ecc0: 2020 2020 2020 2020 6576 656e 742e 6b65          event.ke
-0000ecd0: 7928 2920 3d3d 2051 742e 4b65 792e 4b65  y() == Qt.Key.Ke
-0000ece0: 795f 5061 6765 5570 0a20 2020 2020 2020  y_PageUp.       
-0000ecf0: 2020 2020 2061 6e64 206d 6f64 6966 6965       and modifie
-0000ed00: 7220 213d 2051 742e 4b65 7962 6f61 7264  r != Qt.Keyboard
-0000ed10: 4d6f 6469 6669 6572 2e43 6f6e 7472 6f6c  Modifier.Control
-0000ed20: 4d6f 6469 6669 6572 0a20 2020 2020 2020  Modifier.       
-0000ed30: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
-0000ed40: 6966 2073 656c 662e 6377 2069 7320 6e6f  if self.cw is no
-0000ed50: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0000ed60: 2020 2020 2020 2020 7365 6c66 2e63 772e          self.cw.
-0000ed70: 7370 6565 6420 2b3d 2031 0a20 2020 2020  speed += 1.     
-0000ed80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000ed90: 6377 5f73 7065 6564 2e73 6574 5661 6c75  cw_speed.setValu
-0000eda0: 6528 7365 6c66 2e63 772e 7370 6565 6429  e(self.cw.speed)
-0000edb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000edc0: 2069 6620 7365 6c66 2e63 772e 7365 7276   if self.cw.serv
-0000edd0: 6572 7479 7065 203d 3d20 313a 0a20 2020  ertype == 1:.   
-0000ede0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000edf0: 2073 656c 662e 6377 2e73 656e 6463 7728   self.cw.sendcw(
-0000ee00: 6622 5c78 3162 327b 7365 6c66 2e63 772e  f"\x1b2{self.cw.
-0000ee10: 7370 6565 647d 2229 0a20 2020 2020 2020  speed}").       
-0000ee20: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-0000ee30: 2e63 772e 7365 7276 6572 7479 7065 203d  .cw.servertype =
-0000ee40: 3d20 323a 0a20 2020 2020 2020 2020 2020  = 2:.           
-0000ee50: 2020 2020 2020 2020 2073 656c 662e 6377           self.cw
-0000ee60: 2e73 6574 5f77 696e 6b65 7965 725f 7370  .set_winkeyer_sp
-0000ee70: 6565 6428 7365 6c66 2e63 775f 7370 6565  eed(self.cw_spee
-0000ee80: 642e 7661 6c75 6528 2929 0a20 2020 2020  d.value()).     
-0000ee90: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-0000eea0: 2020 2020 2020 6966 2028 0a20 2020 2020        if (.     
-0000eeb0: 2020 2020 2020 2065 7665 6e74 2e6b 6579         event.key
-0000eec0: 2829 203d 3d20 5174 2e4b 6579 2e4b 6579  () == Qt.Key.Key
-0000eed0: 5f50 6167 6544 6f77 6e0a 2020 2020 2020  _PageDown.      
-0000eee0: 2020 2020 2020 616e 6420 6d6f 6469 6669        and modifi
-0000eef0: 6572 2021 3d20 5174 2e4b 6579 626f 6172  er != Qt.Keyboar
-0000ef00: 644d 6f64 6966 6965 722e 436f 6e74 726f  dModifier.Contro
-0000ef10: 6c4d 6f64 6966 6965 720a 2020 2020 2020  lModifier.      
-0000ef20: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
-0000ef30: 2069 6620 7365 6c66 2e63 7720 6973 206e   if self.cw is n
-0000ef40: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000ef50: 2020 2020 2020 2020 2073 656c 662e 6377           self.cw
-0000ef60: 2e73 7065 6564 202d 3d20 310a 2020 2020  .speed -= 1.    
-0000ef70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000ef80: 2e63 775f 7370 6565 642e 7365 7456 616c  .cw_speed.setVal
-0000ef90: 7565 2873 656c 662e 6377 2e73 7065 6564  ue(self.cw.speed
-0000efa0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000efb0: 2020 6966 2073 656c 662e 6377 2e73 6572    if self.cw.ser
-0000efc0: 7665 7274 7970 6520 3d3d 2031 3a0a 2020  vertype == 1:.  
-0000efd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000efe0: 2020 7365 6c66 2e63 772e 7365 6e64 6377    self.cw.sendcw
-0000eff0: 2866 225c 7831 6232 7b73 656c 662e 6377  (f"\x1b2{self.cw
-0000f000: 2e73 7065 6564 7d22 290a 2020 2020 2020  .speed}").      
-0000f010: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-0000f020: 662e 6377 2e73 6572 7665 7274 7970 6520  f.cw.servertype 
-0000f030: 3d3d 2032 3a0a 2020 2020 2020 2020 2020  == 2:.          
-0000f040: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0000f050: 772e 7365 745f 7769 6e6b 6579 6572 5f73  w.set_winkeyer_s
-0000f060: 7065 6564 2873 656c 662e 6377 5f73 7065  peed(self.cw_spe
-0000f070: 6564 2e76 616c 7565 2829 290a 2020 2020  ed.value()).    
-0000f080: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-0000f090: 2020 2020 2020 2069 6620 6576 656e 742e         if event.
-0000f0a0: 6b65 7928 2920 3d3d 2051 742e 4b65 792e  key() == Qt.Key.
-0000f0b0: 4b65 795f 5461 6220 6f72 2065 7665 6e74  Key_Tab or event
-0000f0c0: 2e6b 6579 2829 203d 3d20 5174 2e4b 6579  .key() == Qt.Key
-0000f0d0: 2e4b 6579 5f42 6163 6b74 6162 3a0a 2020  .Key_Backtab:.  
-0000f0e0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-0000f0f0: 662e 7365 6e74 2e68 6173 466f 6375 7328  f.sent.hasFocus(
-0000f100: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000f110: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-0000f120: 2246 726f 6d20 7365 6e74 2229 0a20 2020  "From sent").   
-0000f130: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000f140: 6d6f 6469 6669 6572 203d 3d20 5174 2e4b  modifier == Qt.K
-0000f150: 6579 626f 6172 644d 6f64 6966 6965 722e  eyboardModifier.
-0000f160: 5368 6966 744d 6f64 6966 6965 723a 0a20  ShiftModifier:. 
-0000f170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f180: 2020 2070 7265 765f 7461 6220 3d20 7365     prev_tab = se
-0000f190: 6c66 2e74 6162 5f70 7265 762e 6765 7428  lf.tab_prev.get(
-0000f1a0: 7365 6c66 2e73 656e 7429 0a20 2020 2020  self.sent).     
-0000f1b0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000f1c0: 7265 765f 7461 622e 7365 7446 6f63 7573  rev_tab.setFocus
-0000f1d0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-0000f1e0: 2020 2020 2020 2070 7265 765f 7461 622e         prev_tab.
-0000f1f0: 6465 7365 6c65 6374 2829 0a20 2020 2020  deselect().     
-0000f200: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000f210: 7265 765f 7461 622e 656e 6428 4661 6c73  rev_tab.end(Fals
-0000f220: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-0000f230: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000f240: 2020 2020 2020 2020 2020 2020 206e 6578               nex
-0000f250: 745f 7461 6220 3d20 7365 6c66 2e74 6162  t_tab = self.tab
-0000f260: 5f6e 6578 742e 6765 7428 7365 6c66 2e73  _next.get(self.s
-0000f270: 656e 7429 0a20 2020 2020 2020 2020 2020  ent).           
-0000f280: 2020 2020 2020 2020 206e 6578 745f 7461           next_ta
-0000f290: 622e 7365 7446 6f63 7573 2829 0a20 2020  b.setFocus().   
-0000f2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f2b0: 206e 6578 745f 7461 622e 6465 7365 6c65   next_tab.desele
-0000f2c0: 6374 2829 0a20 2020 2020 2020 2020 2020  ct().           
-0000f2d0: 2020 2020 2020 2020 206e 6578 745f 7461           next_ta
-0000f2e0: 622e 656e 6428 4661 6c73 6529 0a20 2020  b.end(False).   
-0000f2f0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-0000f300: 7572 6e0a 2020 2020 2020 2020 2020 2020  urn.            
-0000f310: 6966 2073 656c 662e 7265 6365 6976 652e  if self.receive.
-0000f320: 6861 7346 6f63 7573 2829 3a0a 2020 2020  hasFocus():.    
-0000f330: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-0000f340: 6572 2e64 6562 7567 2822 4672 6f6d 2072  er.debug("From r
-0000f350: 6563 6569 7665 2229 0a20 2020 2020 2020  eceive").       
-0000f360: 2020 2020 2020 2020 2069 6620 6d6f 6469           if modi
-0000f370: 6669 6572 203d 3d20 5174 2e4b 6579 626f  fier == Qt.Keybo
-0000f380: 6172 644d 6f64 6966 6965 722e 5368 6966  ardModifier.Shif
-0000f390: 744d 6f64 6966 6965 723a 0a20 2020 2020  tModifier:.     
-0000f3a0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000f3b0: 7265 765f 7461 6220 3d20 7365 6c66 2e74  rev_tab = self.t
-0000f3c0: 6162 5f70 7265 762e 6765 7428 7365 6c66  ab_prev.get(self
-0000f3d0: 2e72 6563 6569 7665 290a 2020 2020 2020  .receive).      
-0000f3e0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-0000f3f0: 6576 5f74 6162 2e73 6574 466f 6375 7328  ev_tab.setFocus(
-0000f400: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000f410: 2020 2020 2020 7072 6576 5f74 6162 2e64        prev_tab.d
-0000f420: 6573 656c 6563 7428 290a 2020 2020 2020  eselect().      
-0000f430: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-0000f440: 6576 5f74 6162 2e65 6e64 2846 616c 7365  ev_tab.end(False
-0000f450: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000f460: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000f470: 2020 2020 2020 2020 2020 2020 6e65 7874              next
-0000f480: 5f74 6162 203d 2073 656c 662e 7461 625f  _tab = self.tab_
-0000f490: 6e65 7874 2e67 6574 2873 656c 662e 7265  next.get(self.re
-0000f4a0: 6365 6976 6529 0a20 2020 2020 2020 2020  ceive).         
-0000f4b0: 2020 2020 2020 2020 2020 206e 6578 745f             next_
-0000f4c0: 7461 622e 7365 7446 6f63 7573 2829 0a20  tab.setFocus(). 
-0000f4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f4e0: 2020 206e 6578 745f 7461 622e 6465 7365     next_tab.dese
-0000f4f0: 6c65 6374 2829 0a20 2020 2020 2020 2020  lect().         
-0000f500: 2020 2020 2020 2020 2020 206e 6578 745f             next_
-0000f510: 7461 622e 656e 6428 4661 6c73 6529 0a20  tab.end(False). 
-0000f520: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000f530: 6574 7572 6e0a 2020 2020 2020 2020 2020  eturn.          
-0000f540: 2020 6966 2073 656c 662e 6f74 6865 725f    if self.other_
-0000f550: 312e 6861 7346 6f63 7573 2829 3a0a 2020  1.hasFocus():.  
-0000f560: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-0000f570: 6767 6572 2e64 6562 7567 2822 4672 6f6d  gger.debug("From
-0000f580: 206f 7468 6572 5f31 2229 0a20 2020 2020   other_1").     
-0000f590: 2020 2020 2020 2020 2020 2069 6620 6d6f             if mo
-0000f5a0: 6469 6669 6572 203d 3d20 5174 2e4b 6579  difier == Qt.Key
-0000f5b0: 626f 6172 644d 6f64 6966 6965 722e 5368  boardModifier.Sh
-0000f5c0: 6966 744d 6f64 6966 6965 723a 0a20 2020  iftModifier:.   
-0000f5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f5e0: 2070 7265 765f 7461 6220 3d20 7365 6c66   prev_tab = self
-0000f5f0: 2e74 6162 5f70 7265 762e 6765 7428 7365  .tab_prev.get(se
-0000f600: 6c66 2e6f 7468 6572 5f31 290a 2020 2020  lf.other_1).    
-0000f610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f620: 7072 6576 5f74 6162 2e73 6574 466f 6375  prev_tab.setFocu
-0000f630: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
-0000f640: 2020 2020 2020 2020 7072 6576 5f74 6162          prev_tab
-0000f650: 2e64 6573 656c 6563 7428 290a 2020 2020  .deselect().    
-0000f660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f670: 7072 6576 5f74 6162 2e65 6e64 2846 616c  prev_tab.end(Fal
-0000f680: 7365 290a 2020 2020 2020 2020 2020 2020  se).            
-0000f690: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000f6a0: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
-0000f6b0: 7874 5f74 6162 203d 2073 656c 662e 7461  xt_tab = self.ta
-0000f6c0: 625f 6e65 7874 2e67 6574 2873 656c 662e  b_next.get(self.
-0000f6d0: 6f74 6865 725f 3129 0a20 2020 2020 2020  other_1).       
-0000f6e0: 2020 2020 2020 2020 2020 2020 206e 6578               nex
-0000f6f0: 745f 7461 622e 7365 7446 6f63 7573 2829  t_tab.setFocus()
-0000f700: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f710: 2020 2020 206e 6578 745f 7461 622e 6465       next_tab.de
-0000f720: 7365 6c65 6374 2829 0a20 2020 2020 2020  select().       
-0000f730: 2020 2020 2020 2020 2020 2020 206e 6578               nex
-0000f740: 745f 7461 622e 656e 6428 4661 6c73 6529  t_tab.end(False)
-0000f750: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f760: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-0000f770: 2020 2020 6966 2073 656c 662e 6f74 6865      if self.othe
-0000f780: 725f 322e 6861 7346 6f63 7573 2829 3a0a  r_2.hasFocus():.
-0000f790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f7a0: 6c6f 6767 6572 2e64 6562 7567 2822 4672  logger.debug("Fr
-0000f7b0: 6f6d 206f 7468 6572 5f32 2229 0a20 2020  om other_2").   
-0000f7c0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000f7d0: 6d6f 6469 6669 6572 203d 3d20 5174 2e4b  modifier == Qt.K
-0000f7e0: 6579 626f 6172 644d 6f64 6966 6965 722e  eyboardModifier.
-0000f7f0: 5368 6966 744d 6f64 6966 6965 723a 0a20  ShiftModifier:. 
-0000f800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f810: 2020 2070 7265 765f 7461 6220 3d20 7365     prev_tab = se
-0000f820: 6c66 2e74 6162 5f70 7265 762e 6765 7428  lf.tab_prev.get(
-0000f830: 7365 6c66 2e6f 7468 6572 5f32 290a 2020  self.other_2).  
-0000f840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f850: 2020 7072 6576 5f74 6162 2e73 6574 466f    prev_tab.setFo
-0000f860: 6375 7328 290a 2020 2020 2020 2020 2020  cus().          
-0000f870: 2020 2020 2020 2020 2020 7072 6576 5f74            prev_t
-0000f880: 6162 2e64 6573 656c 6563 7428 290a 2020  ab.deselect().  
-0000f890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f8a0: 2020 7072 6576 5f74 6162 2e65 6e64 2846    prev_tab.end(F
-0000f8b0: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
-0000f8c0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000f8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f8e0: 6e65 7874 5f74 6162 203d 2073 656c 662e  next_tab = self.
-0000f8f0: 7461 625f 6e65 7874 2e67 6574 2873 656c  tab_next.get(sel
-0000f900: 662e 6f74 6865 725f 3229 0a20 2020 2020  f.other_2).     
-0000f910: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-0000f920: 6578 745f 7461 622e 7365 7446 6f63 7573  ext_tab.setFocus
-0000f930: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-0000f940: 2020 2020 2020 206e 6578 745f 7461 622e         next_tab.
-0000f950: 6465 7365 6c65 6374 2829 0a20 2020 2020  deselect().     
-0000f960: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-0000f970: 6578 745f 7461 622e 656e 6428 4661 6c73  ext_tab.end(Fals
-0000f980: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-0000f990: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-0000f9a0: 2020 2020 2020 6966 2073 656c 662e 6361        if self.ca
-0000f9b0: 6c6c 7369 676e 2e68 6173 466f 6375 7328  llsign.hasFocus(
-0000f9c0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000f9d0: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-0000f9e0: 2246 726f 6d20 6361 6c6c 7369 676e 2229  "From callsign")
-0000f9f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fa00: 2073 656c 662e 6368 6563 6b5f 6361 6c6c   self.check_call
-0000fa10: 7369 676e 2873 656c 662e 6361 6c6c 7369  sign(self.callsi
-0000fa20: 676e 2e74 6578 7428 2929 0a20 2020 2020  gn.text()).     
-0000fa30: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000fa40: 6c66 2e63 6865 636b 5f64 7570 6528 7365  lf.check_dupe(se
-0000fa50: 6c66 2e63 616c 6c73 6967 6e2e 7465 7874  lf.callsign.text
-0000fa60: 2829 293a 0a20 2020 2020 2020 2020 2020  ()):.           
-0000fa70: 2020 2020 2020 2020 2073 656c 662e 6475           self.du
-0000fa80: 7065 5f69 6e64 6963 6174 6f72 2e73 686f  pe_indicator.sho
-0000fa90: 7728 290a 2020 2020 2020 2020 2020 2020  w().            
-0000faa0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000fab0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000fac0: 6c66 2e64 7570 655f 696e 6469 6361 746f  lf.dupe_indicato
-0000fad0: 722e 6869 6465 2829 0a20 2020 2020 2020  r.hide().       
-0000fae0: 2020 2020 2020 2020 2069 6620 6d6f 6469           if modi
-0000faf0: 6669 6572 203d 3d20 5174 2e4b 6579 626f  fier == Qt.Keybo
-0000fb00: 6172 644d 6f64 6966 6965 722e 5368 6966  ardModifier.Shif
-0000fb10: 744d 6f64 6966 6965 723a 0a20 2020 2020  tModifier:.     
-0000fb20: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000fb30: 7265 765f 7461 6220 3d20 7365 6c66 2e74  rev_tab = self.t
-0000fb40: 6162 5f70 7265 762e 6765 7428 7365 6c66  ab_prev.get(self
-0000fb50: 2e63 616c 6c73 6967 6e29 0a20 2020 2020  .callsign).     
-0000fb60: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000fb70: 7265 765f 7461 622e 7365 7446 6f63 7573  rev_tab.setFocus
-0000fb80: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-0000fb90: 2020 2020 2020 2070 7265 765f 7461 622e         prev_tab.
-0000fba0: 6465 7365 6c65 6374 2829 0a20 2020 2020  deselect().     
-0000fbb0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000fbc0: 7265 765f 7461 622e 656e 6428 4661 6c73  rev_tab.end(Fals
-0000fbd0: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-0000fbe0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000fbf0: 2020 2020 2020 2020 2020 2020 2074 6578               tex
-0000fc00: 7420 3d20 7365 6c66 2e63 616c 6c73 6967  t = self.callsig
-0000fc10: 6e2e 7465 7874 2829 0a20 2020 2020 2020  n.text().       
-0000fc20: 2020 2020 2020 2020 2020 2020 2074 6578               tex
-0000fc30: 7420 3d20 7465 7874 2e75 7070 6572 2829  t = text.upper()
-0000fc40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fc50: 2020 2020 205f 7468 6574 6872 6561 6420       _thethread 
-0000fc60: 3d20 7468 7265 6164 696e 672e 5468 7265  = threading.Thre
-0000fc70: 6164 280a 2020 2020 2020 2020 2020 2020  ad(.            
-0000fc80: 2020 2020 2020 2020 2020 2020 7461 7267              targ
-0000fc90: 6574 3d73 656c 662e 6368 6563 6b5f 6361  et=self.check_ca
-0000fca0: 6c6c 7369 676e 322c 0a20 2020 2020 2020  llsign2,.       
-0000fcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fcc0: 2061 7267 733d 2874 6578 742c 292c 0a20   args=(text,),. 
-0000fcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fce0: 2020 2020 2020 2064 6165 6d6f 6e3d 5472         daemon=Tr
-0000fcf0: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-0000fd00: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000fd10: 2020 2020 2020 2020 2020 2020 2020 5f74                _t
-0000fd20: 6865 7468 7265 6164 2e73 7461 7274 2829  hethread.start()
-0000fd30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fd40: 2020 2020 206e 6578 745f 7461 6220 3d20       next_tab = 
-0000fd50: 7365 6c66 2e74 6162 5f6e 6578 742e 6765  self.tab_next.ge
-0000fd60: 7428 7365 6c66 2e63 616c 6c73 6967 6e29  t(self.callsign)
-0000fd70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fd80: 2020 2020 206e 6578 745f 7461 622e 7365       next_tab.se
-0000fd90: 7446 6f63 7573 2829 0a20 2020 2020 2020  tFocus().       
-0000fda0: 2020 2020 2020 2020 2020 2020 206e 6578               nex
-0000fdb0: 745f 7461 622e 6465 7365 6c65 6374 2829  t_tab.deselect()
-0000fdc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fdd0: 2020 2020 206e 6578 745f 7461 622e 656e       next_tab.en
-0000fde0: 6428 4661 6c73 6529 0a20 2020 2020 2020  d(False).       
-0000fdf0: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-0000fe00: 2020 2020 2020 2020 6966 2065 7665 6e74          if event
-0000fe10: 2e6b 6579 2829 203d 3d20 5174 2e4b 6579  .key() == Qt.Key
-0000fe20: 2e4b 6579 5f46 313a 0a20 2020 2020 2020  .Key_F1:.       
-0000fe30: 2020 2020 2073 656c 662e 7072 6f63 6573       self.proces
-0000fe40: 735f 6675 6e63 7469 6f6e 5f6b 6579 2873  s_function_key(s
-0000fe50: 656c 662e 4631 290a 2020 2020 2020 2020  elf.F1).        
-0000fe60: 6966 2065 7665 6e74 2e6b 6579 2829 203d  if event.key() =
-0000fe70: 3d20 5174 2e4b 6579 2e4b 6579 5f46 323a  = Qt.Key.Key_F2:
-0000fe80: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000fe90: 662e 7072 6f63 6573 735f 6675 6e63 7469  f.process_functi
-0000fea0: 6f6e 5f6b 6579 2873 656c 662e 4632 290a  on_key(self.F2).
-0000feb0: 2020 2020 2020 2020 6966 2065 7665 6e74          if event
-0000fec0: 2e6b 6579 2829 203d 3d20 5174 2e4b 6579  .key() == Qt.Key
-0000fed0: 2e4b 6579 5f46 333a 0a20 2020 2020 2020  .Key_F3:.       
-0000fee0: 2020 2020 2073 656c 662e 7072 6f63 6573       self.proces
-0000fef0: 735f 6675 6e63 7469 6f6e 5f6b 6579 2873  s_function_key(s
-0000ff00: 656c 662e 4633 290a 2020 2020 2020 2020  elf.F3).        
-0000ff10: 6966 2065 7665 6e74 2e6b 6579 2829 203d  if event.key() =
-0000ff20: 3d20 5174 2e4b 6579 2e4b 6579 5f46 343a  = Qt.Key.Key_F4:
-0000ff30: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000ff40: 662e 7072 6f63 6573 735f 6675 6e63 7469  f.process_functi
-0000ff50: 6f6e 5f6b 6579 2873 656c 662e 4634 290a  on_key(self.F4).
-0000ff60: 2020 2020 2020 2020 6966 2065 7665 6e74          if event
-0000ff70: 2e6b 6579 2829 203d 3d20 5174 2e4b 6579  .key() == Qt.Key
-0000ff80: 2e4b 6579 5f46 353a 0a20 2020 2020 2020  .Key_F5:.       
-0000ff90: 2020 2020 2073 656c 662e 7072 6f63 6573       self.proces
-0000ffa0: 735f 6675 6e63 7469 6f6e 5f6b 6579 2873  s_function_key(s
-0000ffb0: 656c 662e 4635 290a 2020 2020 2020 2020  elf.F5).        
-0000ffc0: 6966 2065 7665 6e74 2e6b 6579 2829 203d  if event.key() =
-0000ffd0: 3d20 5174 2e4b 6579 2e4b 6579 5f46 363a  = Qt.Key.Key_F6:
-0000ffe0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000fff0: 662e 7072 6f63 6573 735f 6675 6e63 7469  f.process_functi
-00010000: 6f6e 5f6b 6579 2873 656c 662e 4636 290a  on_key(self.F6).
-00010010: 2020 2020 2020 2020 6966 2065 7665 6e74          if event
-00010020: 2e6b 6579 2829 203d 3d20 5174 2e4b 6579  .key() == Qt.Key
-00010030: 2e4b 6579 5f46 373a 0a20 2020 2020 2020  .Key_F7:.       
-00010040: 2020 2020 2073 656c 662e 7072 6f63 6573       self.proces
-00010050: 735f 6675 6e63 7469 6f6e 5f6b 6579 2873  s_function_key(s
-00010060: 656c 662e 4637 290a 2020 2020 2020 2020  elf.F7).        
-00010070: 6966 2065 7665 6e74 2e6b 6579 2829 203d  if event.key() =
-00010080: 3d20 5174 2e4b 6579 2e4b 6579 5f46 383a  = Qt.Key.Key_F8:
-00010090: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000100a0: 662e 7072 6f63 6573 735f 6675 6e63 7469  f.process_functi
-000100b0: 6f6e 5f6b 6579 2873 656c 662e 4638 290a  on_key(self.F8).
-000100c0: 2020 2020 2020 2020 6966 2065 7665 6e74          if event
-000100d0: 2e6b 6579 2829 203d 3d20 5174 2e4b 6579  .key() == Qt.Key
-000100e0: 2e4b 6579 5f46 393a 0a20 2020 2020 2020  .Key_F9:.       
-000100f0: 2020 2020 2073 656c 662e 7072 6f63 6573       self.proces
-00010100: 735f 6675 6e63 7469 6f6e 5f6b 6579 2873  s_function_key(s
-00010110: 656c 662e 4639 290a 2020 2020 2020 2020  elf.F9).        
-00010120: 6966 2065 7665 6e74 2e6b 6579 2829 203d  if event.key() =
-00010130: 3d20 5174 2e4b 6579 2e4b 6579 5f46 3130  = Qt.Key.Key_F10
-00010140: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00010150: 6c66 2e70 726f 6365 7373 5f66 756e 6374  lf.process_funct
-00010160: 696f 6e5f 6b65 7928 7365 6c66 2e46 3130  ion_key(self.F10
-00010170: 290a 2020 2020 2020 2020 6966 2065 7665  ).        if eve
-00010180: 6e74 2e6b 6579 2829 203d 3d20 5174 2e4b  nt.key() == Qt.K
-00010190: 6579 2e4b 6579 5f46 3131 3a0a 2020 2020  ey.Key_F11:.    
-000101a0: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
-000101b0: 6365 7373 5f66 756e 6374 696f 6e5f 6b65  cess_function_ke
-000101c0: 7928 7365 6c66 2e46 3131 290a 2020 2020  y(self.F11).    
-000101d0: 2020 2020 6966 2065 7665 6e74 2e6b 6579      if event.key
-000101e0: 2829 203d 3d20 5174 2e4b 6579 2e4b 6579  () == Qt.Key.Key
-000101f0: 5f46 3132 3a0a 2020 2020 2020 2020 2020  _F12:.          
-00010200: 2020 7365 6c66 2e70 726f 6365 7373 5f66    self.process_f
-00010210: 756e 6374 696f 6e5f 6b65 7928 7365 6c66  unction_key(self
-00010220: 2e46 3132 290a 0a20 2020 2064 6566 2073  .F12)..    def s
-00010230: 6574 5f77 696e 646f 775f 7469 746c 6528  et_window_title(
-00010240: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
-00010250: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00010260: 2020 2053 6574 2077 696e 646f 7720 7469     Set window ti
-00010270: 746c 6520 6261 7365 6420 6f6e 2063 7572  tle based on cur
-00010280: 7265 6e74 2073 7461 7465 2e0a 2020 2020  rent state..    
-00010290: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
-000102a0: 2076 666f 6120 3d20 7365 6c66 2e72 6164   vfoa = self.rad
-000102b0: 696f 5f73 7461 7465 2e67 6574 2822 7666  io_state.get("vf
-000102c0: 6f61 222c 2022 2229 0a20 2020 2020 2020  oa", "").       
-000102d0: 2069 6620 7666 6f61 3a0a 2020 2020 2020   if vfoa:.      
-000102e0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-000102f0: 2020 2020 2020 2020 2020 2076 666f 6120             vfoa 
-00010300: 3d20 696e 7428 7666 6f61 2920 2f20 3130  = int(vfoa) / 10
-00010310: 3030 0a20 2020 2020 2020 2020 2020 2065  00.            e
-00010320: 7863 6570 7420 5661 6c75 6545 7272 6f72  xcept ValueError
-00010330: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00010340: 2020 7666 6f61 203d 2030 2e30 0a20 2020    vfoa = 0.0.   
-00010350: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00010360: 2020 2020 2020 2076 666f 6120 3d20 302e         vfoa = 0.
-00010370: 300a 2020 2020 2020 2020 636f 6e74 6573  0.        contes
-00010380: 745f 6e61 6d65 203d 2022 220a 2020 2020  t_name = "".    
-00010390: 2020 2020 6966 2073 656c 662e 636f 6e74      if self.cont
-000103a0: 6573 743a 0a20 2020 2020 2020 2020 2020  est:.           
-000103b0: 2063 6f6e 7465 7374 5f6e 616d 6520 3d20   contest_name = 
-000103c0: 7365 6c66 2e63 6f6e 7465 7374 2e6e 616d  self.contest.nam
-000103d0: 650a 2020 2020 2020 2020 6c69 6e65 203d  e.        line =
-000103e0: 2028 0a20 2020 2020 2020 2020 2020 2066   (.            f
-000103f0: 2276 666f 613a 7b72 6f75 6e64 2876 666f  "vfoa:{round(vfo
-00010400: 612c 3229 7d20 220a 2020 2020 2020 2020  a,2)} ".        
-00010410: 2020 2020 6622 6d6f 6465 3a7b 7365 6c66      f"mode:{self
-00010420: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
-00010430: 2827 6d6f 6465 272c 2027 2729 7d20 220a  ('mode', '')} ".
-00010440: 2020 2020 2020 2020 2020 2020 6622 4f50              f"OP
-00010450: 3a7b 7365 6c66 2e63 7572 7265 6e74 5f6f  :{self.current_o
-00010460: 707d 207b 636f 6e74 6573 745f 6e61 6d65  p} {contest_name
-00010470: 7d20 220a 2020 2020 2020 2020 2020 2020  } ".            
-00010480: 6622 2d20 4e6f 7431 4d4d 2076 7b5f 5f76  f"- Not1MM v{__v
-00010490: 6572 7369 6f6e 5f5f 7d22 0a20 2020 2020  ersion__}".     
-000104a0: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
-000104b0: 662e 7365 7457 696e 646f 7754 6974 6c65  f.setWindowTitle
-000104c0: 286c 696e 6529 0a0a 2020 2020 6465 6620  (line)..    def 
-000104d0: 7365 6e64 5f77 6f72 6b65 645f 6c69 7374  send_worked_list
-000104e0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-000104f0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00010500: 2020 2020 5365 6e64 206d 6573 7361 6765      Send message
-00010510: 2063 6f6e 7461 696e 696e 6720 776f 726b   containing work
-00010520: 6564 2063 6f6e 7461 6374 7320 616e 6420  ed contacts and 
-00010530: 6261 6e64 730a 0a20 2020 2020 2020 2050  bands..        P
-00010540: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-00010550: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-00010560: 2020 2020 204e 6f6e 650a 0a20 2020 2020       None..     
-00010570: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
-00010580: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
-00010590: 2020 204e 6f6e 650a 2020 2020 2020 2020     None.        
-000105a0: 2222 220a 0a20 2020 2020 2020 2063 6d64  """..        cmd
-000105b0: 203d 207b 7d0a 2020 2020 2020 2020 636d   = {}.        cm
-000105c0: 645b 2263 6d64 225d 203d 2022 574f 524b  d["cmd"] = "WORK
-000105d0: 4544 220a 2020 2020 2020 2020 636d 645b  ED".        cmd[
-000105e0: 2273 7461 7469 6f6e 225d 203d 2070 6c61  "station"] = pla
-000105f0: 7466 6f72 6d2e 6e6f 6465 2829 0a20 2020  tform.node().   
-00010600: 2020 2020 2063 6d64 5b22 776f 726b 6564       cmd["worked
-00010610: 225d 203d 2073 656c 662e 776f 726b 6564  "] = self.worked
-00010620: 5f6c 6973 740a 2020 2020 2020 2020 6c6f  _list.        lo
-00010630: 6767 6572 2e64 6562 7567 2822 2573 222c  gger.debug("%s",
-00010640: 2066 227b 636d 647d 2229 0a20 2020 2020   f"{cmd}").     
-00010650: 2020 2073 656c 662e 6d75 6c74 6963 6173     self.multicas
-00010660: 745f 696e 7465 7266 6163 652e 7365 6e64  t_interface.send
-00010670: 5f61 735f 6a73 6f6e 2863 6d64 290a 0a20  _as_json(cmd).. 
-00010680: 2020 2064 6566 2063 6c65 6172 696e 7075     def clearinpu
-00010690: 7473 2873 656c 6629 202d 3e20 4e6f 6e65  ts(self) -> None
-000106a0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-000106b0: 2020 2020 2020 436c 6561 7273 2074 6865        Clears the
-000106c0: 2074 6578 7420 696e 7075 7420 6669 656c   text input fiel
-000106d0: 6473 2061 6e64 2073 6574 7320 666f 6375  ds and sets focu
-000106e0: 7320 746f 2063 616c 6c73 6967 6e20 6669  s to callsign fi
-000106f0: 656c 642e 0a0a 2020 2020 2020 2020 5061  eld...        Pa
-00010700: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
-00010710: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00010720: 2020 2020 4e6f 6e65 0a0a 2020 2020 2020      None..      
-00010730: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
-00010740: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
-00010750: 2020 4e6f 6e65 0a20 2020 2020 2020 2022    None.        "
-00010760: 2222 0a0a 2020 2020 2020 2020 7365 6c66  ""..        self
-00010770: 2e64 7570 655f 696e 6469 6361 746f 722e  .dupe_indicator.
-00010780: 6869 6465 2829 0a20 2020 2020 2020 2073  hide().        s
-00010790: 656c 662e 636f 6e74 6163 7420 3d20 7365  elf.contact = se
-000107a0: 6c66 2e64 6174 6162 6173 652e 656d 7074  lf.database.empt
-000107b0: 795f 636f 6e74 6163 740a 2020 2020 2020  y_contact.      
-000107c0: 2020 7365 6c66 2e68 6561 6469 6e67 5f64    self.heading_d
-000107d0: 6973 7461 6e63 652e 7365 7454 6578 7428  istance.setText(
-000107e0: 2222 290a 2020 2020 2020 2020 7365 6c66  "").        self
-000107f0: 2e64 785f 656e 7469 7479 2e73 6574 5465  .dx_entity.setTe
-00010800: 7874 2822 2229 0a20 2020 2020 2020 2069  xt("").        i
-00010810: 6620 7365 6c66 2e63 6f6e 7465 7374 3a0a  f self.contest:.
-00010820: 2020 2020 2020 2020 2020 2020 6d75 6c74              mult
+0000e880: 5b22 6478 225d 203d 2064 780a 2020 2020  ["dx"] = dx.    
+0000e890: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000e8a0: 2e6d 756c 7469 6361 7374 5f69 6e74 6572  .multicast_inter
+0000e8b0: 6661 6365 2e73 656e 645f 6173 5f6a 736f  face.send_as_jso
+0000e8c0: 6e28 636d 6429 0a20 2020 2020 2020 2020  n(cmd).         
+0000e8d0: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+0000e8e0: 2020 6966 2028 0a20 2020 2020 2020 2020    if (.         
+0000e8f0: 2020 2065 7665 6e74 2e6b 6579 2829 203d     event.key() =
+0000e900: 3d20 5174 2e4b 6579 2e4b 6579 5f45 7363  = Qt.Key.Key_Esc
+0000e910: 6170 650a 2020 2020 2020 2020 2020 2020  ape.            
+0000e920: 616e 6420 6d6f 6469 6669 6572 2021 3d20  and modifier != 
+0000e930: 5174 2e4b 6579 626f 6172 644d 6f64 6966  Qt.KeyboardModif
+0000e940: 6965 722e 436f 6e74 726f 6c4d 6f64 6966  ier.ControlModif
+0000e950: 6965 720a 2020 2020 2020 2020 293a 2020  ier.        ):  
+0000e960: 2320 7079 6c69 6e74 3a20 6469 7361 626c  # pylint: disabl
+0000e970: 653d 6e6f 2d6d 656d 6265 720a 2020 2020  e=no-member.    
+0000e980: 2020 2020 2020 2020 7365 6c66 2e63 6c65          self.cle
+0000e990: 6172 696e 7075 7473 2829 0a20 2020 2020  arinputs().     
+0000e9a0: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+0000e9b0: 2020 2020 2020 6966 2028 0a20 2020 2020        if (.     
+0000e9c0: 2020 2020 2020 2065 7665 6e74 2e6b 6579         event.key
+0000e9d0: 2829 203d 3d20 5174 2e4b 6579 2e4b 6579  () == Qt.Key.Key
+0000e9e0: 5f45 7363 6170 650a 2020 2020 2020 2020  _Escape.        
+0000e9f0: 2020 2020 616e 6420 6d6f 6469 6669 6572      and modifier
+0000ea00: 203d 3d20 5174 2e4b 6579 626f 6172 644d   == Qt.KeyboardM
+0000ea10: 6f64 6966 6965 722e 436f 6e74 726f 6c4d  odifier.ControlM
+0000ea20: 6f64 6966 6965 720a 2020 2020 2020 2020  odifier.        
+0000ea30: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
+0000ea40: 6620 7365 6c66 2e63 7720 6973 206e 6f74  f self.cw is not
+0000ea50: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000ea60: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+0000ea70: 772e 7365 7276 6572 7479 7065 203d 3d20  w.servertype == 
+0000ea80: 313a 0a20 2020 2020 2020 2020 2020 2020  1:.             
+0000ea90: 2020 2020 2020 2073 656c 662e 6377 2e73         self.cw.s
+0000eaa0: 656e 6463 7728 225c 7831 6234 2229 0a20  endcw("\x1b4"). 
+0000eab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eac0: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+0000ead0: 2020 6966 2065 7665 6e74 2e6b 6579 2829    if event.key()
+0000eae0: 203d 3d20 5174 2e4b 6579 2e4b 6579 5f55   == Qt.Key.Key_U
+0000eaf0: 703a 0a20 2020 2020 2020 2020 2020 2063  p:.            c
+0000eb00: 6d64 203d 207b 7d0a 2020 2020 2020 2020  md = {}.        
+0000eb10: 2020 2020 636d 645b 2263 6d64 225d 203d      cmd["cmd"] =
+0000eb20: 2022 5052 4556 5350 4f54 220a 2020 2020   "PREVSPOT".    
+0000eb30: 2020 2020 2020 2020 636d 645b 2273 7461          cmd["sta
+0000eb40: 7469 6f6e 225d 203d 2070 6c61 7466 6f72  tion"] = platfor
+0000eb50: 6d2e 6e6f 6465 2829 0a20 2020 2020 2020  m.node().       
+0000eb60: 2020 2020 2073 656c 662e 6d75 6c74 6963       self.multic
+0000eb70: 6173 745f 696e 7465 7266 6163 652e 7365  ast_interface.se
+0000eb80: 6e64 5f61 735f 6a73 6f6e 2863 6d64 290a  nd_as_json(cmd).
+0000eb90: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000eba0: 726e 0a20 2020 2020 2020 2069 6620 6576  rn.        if ev
+0000ebb0: 656e 742e 6b65 7928 2920 3d3d 2051 742e  ent.key() == Qt.
+0000ebc0: 4b65 792e 4b65 795f 446f 776e 3a0a 2020  Key.Key_Down:.  
+0000ebd0: 2020 2020 2020 2020 2020 636d 6420 3d20            cmd = 
+0000ebe0: 7b7d 0a20 2020 2020 2020 2020 2020 2063  {}.            c
+0000ebf0: 6d64 5b22 636d 6422 5d20 3d20 224e 4558  md["cmd"] = "NEX
+0000ec00: 5453 504f 5422 0a20 2020 2020 2020 2020  TSPOT".         
+0000ec10: 2020 2063 6d64 5b22 7374 6174 696f 6e22     cmd["station"
+0000ec20: 5d20 3d20 706c 6174 666f 726d 2e6e 6f64  ] = platform.nod
+0000ec30: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+0000ec40: 7365 6c66 2e6d 756c 7469 6361 7374 5f69  self.multicast_i
+0000ec50: 6e74 6572 6661 6365 2e73 656e 645f 6173  nterface.send_as
+0000ec60: 5f6a 736f 6e28 636d 6429 0a20 2020 2020  _json(cmd).     
+0000ec70: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+0000ec80: 2020 2020 2020 6966 2028 0a20 2020 2020        if (.     
+0000ec90: 2020 2020 2020 2065 7665 6e74 2e6b 6579         event.key
+0000eca0: 2829 203d 3d20 5174 2e4b 6579 2e4b 6579  () == Qt.Key.Key
+0000ecb0: 5f50 6167 6555 700a 2020 2020 2020 2020  _PageUp.        
+0000ecc0: 2020 2020 616e 6420 6d6f 6469 6669 6572      and modifier
+0000ecd0: 2021 3d20 5174 2e4b 6579 626f 6172 644d   != Qt.KeyboardM
+0000ece0: 6f64 6966 6965 722e 436f 6e74 726f 6c4d  odifier.ControlM
+0000ecf0: 6f64 6966 6965 720a 2020 2020 2020 2020  odifier.        
+0000ed00: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
+0000ed10: 6620 7365 6c66 2e63 7720 6973 206e 6f74  f self.cw is not
+0000ed20: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000ed30: 2020 2020 2020 2073 656c 662e 6377 2e73         self.cw.s
+0000ed40: 7065 6564 202b 3d20 310a 2020 2020 2020  peed += 1.      
+0000ed50: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0000ed60: 775f 7370 6565 642e 7365 7456 616c 7565  w_speed.setValue
+0000ed70: 2873 656c 662e 6377 2e73 7065 6564 290a  (self.cw.speed).
+0000ed80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ed90: 6966 2073 656c 662e 6377 2e73 6572 7665  if self.cw.serve
+0000eda0: 7274 7970 6520 3d3d 2031 3a0a 2020 2020  rtype == 1:.    
+0000edb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000edc0: 7365 6c66 2e63 772e 7365 6e64 6377 2866  self.cw.sendcw(f
+0000edd0: 225c 7831 6232 7b73 656c 662e 6377 2e73  "\x1b2{self.cw.s
+0000ede0: 7065 6564 7d22 290a 2020 2020 2020 2020  peed}").        
+0000edf0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000ee00: 6377 2e73 6572 7665 7274 7970 6520 3d3d  cw.servertype ==
+0000ee10: 2032 3a0a 2020 2020 2020 2020 2020 2020   2:.            
+0000ee20: 2020 2020 2020 2020 7365 6c66 2e63 772e          self.cw.
+0000ee30: 7365 745f 7769 6e6b 6579 6572 5f73 7065  set_winkeyer_spe
+0000ee40: 6564 2873 656c 662e 6377 5f73 7065 6564  ed(self.cw_speed
+0000ee50: 2e76 616c 7565 2829 290a 2020 2020 2020  .value()).      
+0000ee60: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+0000ee70: 2020 2020 2069 6620 280a 2020 2020 2020       if (.      
+0000ee80: 2020 2020 2020 6576 656e 742e 6b65 7928        event.key(
+0000ee90: 2920 3d3d 2051 742e 4b65 792e 4b65 795f  ) == Qt.Key.Key_
+0000eea0: 5061 6765 446f 776e 0a20 2020 2020 2020  PageDown.       
+0000eeb0: 2020 2020 2061 6e64 206d 6f64 6966 6965       and modifie
+0000eec0: 7220 213d 2051 742e 4b65 7962 6f61 7264  r != Qt.Keyboard
+0000eed0: 4d6f 6469 6669 6572 2e43 6f6e 7472 6f6c  Modifier.Control
+0000eee0: 4d6f 6469 6669 6572 0a20 2020 2020 2020  Modifier.       
+0000eef0: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
+0000ef00: 6966 2073 656c 662e 6377 2069 7320 6e6f  if self.cw is no
+0000ef10: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000ef20: 2020 2020 2020 2020 7365 6c66 2e63 772e          self.cw.
+0000ef30: 7370 6565 6420 2d3d 2031 0a20 2020 2020  speed -= 1.     
+0000ef40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000ef50: 6377 5f73 7065 6564 2e73 6574 5661 6c75  cw_speed.setValu
+0000ef60: 6528 7365 6c66 2e63 772e 7370 6565 6429  e(self.cw.speed)
+0000ef70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ef80: 2069 6620 7365 6c66 2e63 772e 7365 7276   if self.cw.serv
+0000ef90: 6572 7479 7065 203d 3d20 313a 0a20 2020  ertype == 1:.   
+0000efa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000efb0: 2073 656c 662e 6377 2e73 656e 6463 7728   self.cw.sendcw(
+0000efc0: 6622 5c78 3162 327b 7365 6c66 2e63 772e  f"\x1b2{self.cw.
+0000efd0: 7370 6565 647d 2229 0a20 2020 2020 2020  speed}").       
+0000efe0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+0000eff0: 2e63 772e 7365 7276 6572 7479 7065 203d  .cw.servertype =
+0000f000: 3d20 323a 0a20 2020 2020 2020 2020 2020  = 2:.           
+0000f010: 2020 2020 2020 2020 2073 656c 662e 6377           self.cw
+0000f020: 2e73 6574 5f77 696e 6b65 7965 725f 7370  .set_winkeyer_sp
+0000f030: 6565 6428 7365 6c66 2e63 775f 7370 6565  eed(self.cw_spee
+0000f040: 642e 7661 6c75 6528 2929 0a20 2020 2020  d.value()).     
+0000f050: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+0000f060: 2020 2020 2020 6966 2065 7665 6e74 2e6b        if event.k
+0000f070: 6579 2829 203d 3d20 5174 2e4b 6579 2e4b  ey() == Qt.Key.K
+0000f080: 6579 5f54 6162 206f 7220 6576 656e 742e  ey_Tab or event.
+0000f090: 6b65 7928 2920 3d3d 2051 742e 4b65 792e  key() == Qt.Key.
+0000f0a0: 4b65 795f 4261 636b 7461 623a 0a20 2020  Key_Backtab:.   
+0000f0b0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+0000f0c0: 2e73 656e 742e 6861 7346 6f63 7573 2829  .sent.hasFocus()
+0000f0d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000f0e0: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
+0000f0f0: 4672 6f6d 2073 656e 7422 290a 2020 2020  From sent").    
+0000f100: 2020 2020 2020 2020 2020 2020 6966 206d              if m
+0000f110: 6f64 6966 6965 7220 3d3d 2051 742e 4b65  odifier == Qt.Ke
+0000f120: 7962 6f61 7264 4d6f 6469 6669 6572 2e53  yboardModifier.S
+0000f130: 6869 6674 4d6f 6469 6669 6572 3a0a 2020  hiftModifier:.  
+0000f140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f150: 2020 7072 6576 5f74 6162 203d 2073 656c    prev_tab = sel
+0000f160: 662e 7461 625f 7072 6576 2e67 6574 2873  f.tab_prev.get(s
+0000f170: 656c 662e 7365 6e74 290a 2020 2020 2020  elf.sent).      
+0000f180: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+0000f190: 6576 5f74 6162 2e73 6574 466f 6375 7328  ev_tab.setFocus(
+0000f1a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000f1b0: 2020 2020 2020 7072 6576 5f74 6162 2e64        prev_tab.d
+0000f1c0: 6573 656c 6563 7428 290a 2020 2020 2020  eselect().      
+0000f1d0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+0000f1e0: 6576 5f74 6162 2e65 6e64 2846 616c 7365  ev_tab.end(False
+0000f1f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000f200: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000f210: 2020 2020 2020 2020 2020 2020 6e65 7874              next
+0000f220: 5f74 6162 203d 2073 656c 662e 7461 625f  _tab = self.tab_
+0000f230: 6e65 7874 2e67 6574 2873 656c 662e 7365  next.get(self.se
+0000f240: 6e74 290a 2020 2020 2020 2020 2020 2020  nt).            
+0000f250: 2020 2020 2020 2020 6e65 7874 5f74 6162          next_tab
+0000f260: 2e73 6574 466f 6375 7328 290a 2020 2020  .setFocus().    
+0000f270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f280: 6e65 7874 5f74 6162 2e64 6573 656c 6563  next_tab.deselec
+0000f290: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
+0000f2a0: 2020 2020 2020 2020 6e65 7874 5f74 6162          next_tab
+0000f2b0: 2e65 6e64 2846 616c 7365 290a 2020 2020  .end(False).    
+0000f2c0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000f2d0: 726e 0a20 2020 2020 2020 2020 2020 2069  rn.            i
+0000f2e0: 6620 7365 6c66 2e72 6563 6569 7665 2e68  f self.receive.h
+0000f2f0: 6173 466f 6375 7328 293a 0a20 2020 2020  asFocus():.     
+0000f300: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+0000f310: 722e 6465 6275 6728 2246 726f 6d20 7265  r.debug("From re
+0000f320: 6365 6976 6522 290a 2020 2020 2020 2020  ceive").        
+0000f330: 2020 2020 2020 2020 6966 206d 6f64 6966          if modif
+0000f340: 6965 7220 3d3d 2051 742e 4b65 7962 6f61  ier == Qt.Keyboa
+0000f350: 7264 4d6f 6469 6669 6572 2e53 6869 6674  rdModifier.Shift
+0000f360: 4d6f 6469 6669 6572 3a0a 2020 2020 2020  Modifier:.      
+0000f370: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+0000f380: 6576 5f74 6162 203d 2073 656c 662e 7461  ev_tab = self.ta
+0000f390: 625f 7072 6576 2e67 6574 2873 656c 662e  b_prev.get(self.
+0000f3a0: 7265 6365 6976 6529 0a20 2020 2020 2020  receive).       
+0000f3b0: 2020 2020 2020 2020 2020 2020 2070 7265               pre
+0000f3c0: 765f 7461 622e 7365 7446 6f63 7573 2829  v_tab.setFocus()
+0000f3d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f3e0: 2020 2020 2070 7265 765f 7461 622e 6465       prev_tab.de
+0000f3f0: 7365 6c65 6374 2829 0a20 2020 2020 2020  select().       
+0000f400: 2020 2020 2020 2020 2020 2020 2070 7265               pre
+0000f410: 765f 7461 622e 656e 6428 4661 6c73 6529  v_tab.end(False)
+0000f420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f430: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000f440: 2020 2020 2020 2020 2020 206e 6578 745f             next_
+0000f450: 7461 6220 3d20 7365 6c66 2e74 6162 5f6e  tab = self.tab_n
+0000f460: 6578 742e 6765 7428 7365 6c66 2e72 6563  ext.get(self.rec
+0000f470: 6569 7665 290a 2020 2020 2020 2020 2020  eive).          
+0000f480: 2020 2020 2020 2020 2020 6e65 7874 5f74            next_t
+0000f490: 6162 2e73 6574 466f 6375 7328 290a 2020  ab.setFocus().  
+0000f4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f4b0: 2020 6e65 7874 5f74 6162 2e64 6573 656c    next_tab.desel
+0000f4c0: 6563 7428 290a 2020 2020 2020 2020 2020  ect().          
+0000f4d0: 2020 2020 2020 2020 2020 6e65 7874 5f74            next_t
+0000f4e0: 6162 2e65 6e64 2846 616c 7365 290a 2020  ab.end(False).  
+0000f4f0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0000f500: 7475 726e 0a20 2020 2020 2020 2020 2020  turn.           
+0000f510: 2069 6620 7365 6c66 2e6f 7468 6572 5f31   if self.other_1
+0000f520: 2e68 6173 466f 6375 7328 293a 0a20 2020  .hasFocus():.   
+0000f530: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+0000f540: 6765 722e 6465 6275 6728 2246 726f 6d20  ger.debug("From 
+0000f550: 6f74 6865 725f 3122 290a 2020 2020 2020  other_1").      
+0000f560: 2020 2020 2020 2020 2020 6966 206d 6f64            if mod
+0000f570: 6966 6965 7220 3d3d 2051 742e 4b65 7962  ifier == Qt.Keyb
+0000f580: 6f61 7264 4d6f 6469 6669 6572 2e53 6869  oardModifier.Shi
+0000f590: 6674 4d6f 6469 6669 6572 3a0a 2020 2020  ftModifier:.    
+0000f5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f5b0: 7072 6576 5f74 6162 203d 2073 656c 662e  prev_tab = self.
+0000f5c0: 7461 625f 7072 6576 2e67 6574 2873 656c  tab_prev.get(sel
+0000f5d0: 662e 6f74 6865 725f 3129 0a20 2020 2020  f.other_1).     
+0000f5e0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000f5f0: 7265 765f 7461 622e 7365 7446 6f63 7573  rev_tab.setFocus
+0000f600: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+0000f610: 2020 2020 2020 2070 7265 765f 7461 622e         prev_tab.
+0000f620: 6465 7365 6c65 6374 2829 0a20 2020 2020  deselect().     
+0000f630: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000f640: 7265 765f 7461 622e 656e 6428 4661 6c73  rev_tab.end(Fals
+0000f650: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+0000f660: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000f670: 2020 2020 2020 2020 2020 2020 206e 6578               nex
+0000f680: 745f 7461 6220 3d20 7365 6c66 2e74 6162  t_tab = self.tab
+0000f690: 5f6e 6578 742e 6765 7428 7365 6c66 2e6f  _next.get(self.o
+0000f6a0: 7468 6572 5f31 290a 2020 2020 2020 2020  ther_1).        
+0000f6b0: 2020 2020 2020 2020 2020 2020 6e65 7874              next
+0000f6c0: 5f74 6162 2e73 6574 466f 6375 7328 290a  _tab.setFocus().
+0000f6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f6e0: 2020 2020 6e65 7874 5f74 6162 2e64 6573      next_tab.des
+0000f6f0: 656c 6563 7428 290a 2020 2020 2020 2020  elect().        
+0000f700: 2020 2020 2020 2020 2020 2020 6e65 7874              next
+0000f710: 5f74 6162 2e65 6e64 2846 616c 7365 290a  _tab.end(False).
+0000f720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f730: 7265 7475 726e 0a20 2020 2020 2020 2020  return.         
+0000f740: 2020 2069 6620 7365 6c66 2e6f 7468 6572     if self.other
+0000f750: 5f32 2e68 6173 466f 6375 7328 293a 0a20  _2.hasFocus():. 
+0000f760: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0000f770: 6f67 6765 722e 6465 6275 6728 2246 726f  ogger.debug("Fro
+0000f780: 6d20 6f74 6865 725f 3222 290a 2020 2020  m other_2").    
+0000f790: 2020 2020 2020 2020 2020 2020 6966 206d              if m
+0000f7a0: 6f64 6966 6965 7220 3d3d 2051 742e 4b65  odifier == Qt.Ke
+0000f7b0: 7962 6f61 7264 4d6f 6469 6669 6572 2e53  yboardModifier.S
+0000f7c0: 6869 6674 4d6f 6469 6669 6572 3a0a 2020  hiftModifier:.  
+0000f7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f7e0: 2020 7072 6576 5f74 6162 203d 2073 656c    prev_tab = sel
+0000f7f0: 662e 7461 625f 7072 6576 2e67 6574 2873  f.tab_prev.get(s
+0000f800: 656c 662e 6f74 6865 725f 3229 0a20 2020  elf.other_2).   
+0000f810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f820: 2070 7265 765f 7461 622e 7365 7446 6f63   prev_tab.setFoc
+0000f830: 7573 2829 0a20 2020 2020 2020 2020 2020  us().           
+0000f840: 2020 2020 2020 2020 2070 7265 765f 7461           prev_ta
+0000f850: 622e 6465 7365 6c65 6374 2829 0a20 2020  b.deselect().   
+0000f860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f870: 2070 7265 765f 7461 622e 656e 6428 4661   prev_tab.end(Fa
+0000f880: 6c73 6529 0a20 2020 2020 2020 2020 2020  lse).           
+0000f890: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000f8a0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0000f8b0: 6578 745f 7461 6220 3d20 7365 6c66 2e74  ext_tab = self.t
+0000f8c0: 6162 5f6e 6578 742e 6765 7428 7365 6c66  ab_next.get(self
+0000f8d0: 2e6f 7468 6572 5f32 290a 2020 2020 2020  .other_2).      
+0000f8e0: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+0000f8f0: 7874 5f74 6162 2e73 6574 466f 6375 7328  xt_tab.setFocus(
+0000f900: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000f910: 2020 2020 2020 6e65 7874 5f74 6162 2e64        next_tab.d
+0000f920: 6573 656c 6563 7428 290a 2020 2020 2020  eselect().      
+0000f930: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+0000f940: 7874 5f74 6162 2e65 6e64 2846 616c 7365  xt_tab.end(False
+0000f950: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000f960: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+0000f970: 2020 2020 2069 6620 7365 6c66 2e63 616c       if self.cal
+0000f980: 6c73 6967 6e2e 6861 7346 6f63 7573 2829  lsign.hasFocus()
+0000f990: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000f9a0: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
+0000f9b0: 4672 6f6d 2063 616c 6c73 6967 6e22 290a  From callsign").
+0000f9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f9d0: 7365 6c66 2e63 6865 636b 5f63 616c 6c73  self.check_calls
+0000f9e0: 6967 6e28 7365 6c66 2e63 616c 6c73 6967  ign(self.callsig
+0000f9f0: 6e2e 7465 7874 2829 290a 2020 2020 2020  n.text()).      
+0000fa00: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0000fa10: 662e 6368 6563 6b5f 6475 7065 2873 656c  f.check_dupe(sel
+0000fa20: 662e 6361 6c6c 7369 676e 2e74 6578 7428  f.callsign.text(
+0000fa30: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
+0000fa40: 2020 2020 2020 2020 7365 6c66 2e64 7570          self.dup
+0000fa50: 655f 696e 6469 6361 746f 722e 7368 6f77  e_indicator.show
+0000fa60: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+0000fa70: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000fa80: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000fa90: 662e 6475 7065 5f69 6e64 6963 6174 6f72  f.dupe_indicator
+0000faa0: 2e68 6964 6528 290a 2020 2020 2020 2020  .hide().        
+0000fab0: 2020 2020 2020 2020 6966 206d 6f64 6966          if modif
+0000fac0: 6965 7220 3d3d 2051 742e 4b65 7962 6f61  ier == Qt.Keyboa
+0000fad0: 7264 4d6f 6469 6669 6572 2e53 6869 6674  rdModifier.Shift
+0000fae0: 4d6f 6469 6669 6572 3a0a 2020 2020 2020  Modifier:.      
+0000faf0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+0000fb00: 6576 5f74 6162 203d 2073 656c 662e 7461  ev_tab = self.ta
+0000fb10: 625f 7072 6576 2e67 6574 2873 656c 662e  b_prev.get(self.
+0000fb20: 6361 6c6c 7369 676e 290a 2020 2020 2020  callsign).      
+0000fb30: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+0000fb40: 6576 5f74 6162 2e73 6574 466f 6375 7328  ev_tab.setFocus(
+0000fb50: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000fb60: 2020 2020 2020 7072 6576 5f74 6162 2e64        prev_tab.d
+0000fb70: 6573 656c 6563 7428 290a 2020 2020 2020  eselect().      
+0000fb80: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+0000fb90: 6576 5f74 6162 2e65 6e64 2846 616c 7365  ev_tab.end(False
+0000fba0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000fbb0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000fbc0: 2020 2020 2020 2020 2020 2020 7465 7874              text
+0000fbd0: 203d 2073 656c 662e 6361 6c6c 7369 676e   = self.callsign
+0000fbe0: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
+0000fbf0: 2020 2020 2020 2020 2020 2020 7465 7874              text
+0000fc00: 203d 2074 6578 742e 7570 7065 7228 290a   = text.upper().
+0000fc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fc20: 2020 2020 5f74 6865 7468 7265 6164 203d      _thethread =
+0000fc30: 2074 6872 6561 6469 6e67 2e54 6872 6561   threading.Threa
+0000fc40: 6428 0a20 2020 2020 2020 2020 2020 2020  d(.             
+0000fc50: 2020 2020 2020 2020 2020 2074 6172 6765             targe
+0000fc60: 743d 7365 6c66 2e63 6865 636b 5f63 616c  t=self.check_cal
+0000fc70: 6c73 6967 6e32 2c0a 2020 2020 2020 2020  lsign2,.        
+0000fc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fc90: 6172 6773 3d28 7465 7874 2c29 2c0a 2020  args=(text,),.  
+0000fca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fcb0: 2020 2020 2020 6461 656d 6f6e 3d54 7275        daemon=Tru
+0000fcc0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0000fcd0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000fce0: 2020 2020 2020 2020 2020 2020 205f 7468               _th
+0000fcf0: 6574 6872 6561 642e 7374 6172 7428 290a  ethread.start().
+0000fd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fd10: 2020 2020 6e65 7874 5f74 6162 203d 2073      next_tab = s
+0000fd20: 656c 662e 7461 625f 6e65 7874 2e67 6574  elf.tab_next.get
+0000fd30: 2873 656c 662e 6361 6c6c 7369 676e 290a  (self.callsign).
+0000fd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fd50: 2020 2020 6e65 7874 5f74 6162 2e73 6574      next_tab.set
+0000fd60: 466f 6375 7328 290a 2020 2020 2020 2020  Focus().        
+0000fd70: 2020 2020 2020 2020 2020 2020 6e65 7874              next
+0000fd80: 5f74 6162 2e64 6573 656c 6563 7428 290a  _tab.deselect().
+0000fd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fda0: 2020 2020 6e65 7874 5f74 6162 2e65 6e64      next_tab.end
+0000fdb0: 2846 616c 7365 290a 2020 2020 2020 2020  (False).        
+0000fdc0: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+0000fdd0: 2020 2020 2020 2069 6620 6576 656e 742e         if event.
+0000fde0: 6b65 7928 2920 3d3d 2051 742e 4b65 792e  key() == Qt.Key.
+0000fdf0: 4b65 795f 4631 3a0a 2020 2020 2020 2020  Key_F1:.        
+0000fe00: 2020 2020 7365 6c66 2e70 726f 6365 7373      self.process
+0000fe10: 5f66 756e 6374 696f 6e5f 6b65 7928 7365  _function_key(se
+0000fe20: 6c66 2e46 3129 0a20 2020 2020 2020 2069  lf.F1).        i
+0000fe30: 6620 6576 656e 742e 6b65 7928 2920 3d3d  f event.key() ==
+0000fe40: 2051 742e 4b65 792e 4b65 795f 4632 3a0a   Qt.Key.Key_F2:.
+0000fe50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000fe60: 2e70 726f 6365 7373 5f66 756e 6374 696f  .process_functio
+0000fe70: 6e5f 6b65 7928 7365 6c66 2e46 3229 0a20  n_key(self.F2). 
+0000fe80: 2020 2020 2020 2069 6620 6576 656e 742e         if event.
+0000fe90: 6b65 7928 2920 3d3d 2051 742e 4b65 792e  key() == Qt.Key.
+0000fea0: 4b65 795f 4633 3a0a 2020 2020 2020 2020  Key_F3:.        
+0000feb0: 2020 2020 7365 6c66 2e70 726f 6365 7373      self.process
+0000fec0: 5f66 756e 6374 696f 6e5f 6b65 7928 7365  _function_key(se
+0000fed0: 6c66 2e46 3329 0a20 2020 2020 2020 2069  lf.F3).        i
+0000fee0: 6620 6576 656e 742e 6b65 7928 2920 3d3d  f event.key() ==
+0000fef0: 2051 742e 4b65 792e 4b65 795f 4634 3a0a   Qt.Key.Key_F4:.
+0000ff00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000ff10: 2e70 726f 6365 7373 5f66 756e 6374 696f  .process_functio
+0000ff20: 6e5f 6b65 7928 7365 6c66 2e46 3429 0a20  n_key(self.F4). 
+0000ff30: 2020 2020 2020 2069 6620 6576 656e 742e         if event.
+0000ff40: 6b65 7928 2920 3d3d 2051 742e 4b65 792e  key() == Qt.Key.
+0000ff50: 4b65 795f 4635 3a0a 2020 2020 2020 2020  Key_F5:.        
+0000ff60: 2020 2020 7365 6c66 2e70 726f 6365 7373      self.process
+0000ff70: 5f66 756e 6374 696f 6e5f 6b65 7928 7365  _function_key(se
+0000ff80: 6c66 2e46 3529 0a20 2020 2020 2020 2069  lf.F5).        i
+0000ff90: 6620 6576 656e 742e 6b65 7928 2920 3d3d  f event.key() ==
+0000ffa0: 2051 742e 4b65 792e 4b65 795f 4636 3a0a   Qt.Key.Key_F6:.
+0000ffb0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000ffc0: 2e70 726f 6365 7373 5f66 756e 6374 696f  .process_functio
+0000ffd0: 6e5f 6b65 7928 7365 6c66 2e46 3629 0a20  n_key(self.F6). 
+0000ffe0: 2020 2020 2020 2069 6620 6576 656e 742e         if event.
+0000fff0: 6b65 7928 2920 3d3d 2051 742e 4b65 792e  key() == Qt.Key.
+00010000: 4b65 795f 4637 3a0a 2020 2020 2020 2020  Key_F7:.        
+00010010: 2020 2020 7365 6c66 2e70 726f 6365 7373      self.process
+00010020: 5f66 756e 6374 696f 6e5f 6b65 7928 7365  _function_key(se
+00010030: 6c66 2e46 3729 0a20 2020 2020 2020 2069  lf.F7).        i
+00010040: 6620 6576 656e 742e 6b65 7928 2920 3d3d  f event.key() ==
+00010050: 2051 742e 4b65 792e 4b65 795f 4638 3a0a   Qt.Key.Key_F8:.
+00010060: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010070: 2e70 726f 6365 7373 5f66 756e 6374 696f  .process_functio
+00010080: 6e5f 6b65 7928 7365 6c66 2e46 3829 0a20  n_key(self.F8). 
+00010090: 2020 2020 2020 2069 6620 6576 656e 742e         if event.
+000100a0: 6b65 7928 2920 3d3d 2051 742e 4b65 792e  key() == Qt.Key.
+000100b0: 4b65 795f 4639 3a0a 2020 2020 2020 2020  Key_F9:.        
+000100c0: 2020 2020 7365 6c66 2e70 726f 6365 7373      self.process
+000100d0: 5f66 756e 6374 696f 6e5f 6b65 7928 7365  _function_key(se
+000100e0: 6c66 2e46 3929 0a20 2020 2020 2020 2069  lf.F9).        i
+000100f0: 6620 6576 656e 742e 6b65 7928 2920 3d3d  f event.key() ==
+00010100: 2051 742e 4b65 792e 4b65 795f 4631 303a   Qt.Key.Key_F10:
+00010110: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00010120: 662e 7072 6f63 6573 735f 6675 6e63 7469  f.process_functi
+00010130: 6f6e 5f6b 6579 2873 656c 662e 4631 3029  on_key(self.F10)
+00010140: 0a20 2020 2020 2020 2069 6620 6576 656e  .        if even
+00010150: 742e 6b65 7928 2920 3d3d 2051 742e 4b65  t.key() == Qt.Ke
+00010160: 792e 4b65 795f 4631 313a 0a20 2020 2020  y.Key_F11:.     
+00010170: 2020 2020 2020 2073 656c 662e 7072 6f63         self.proc
+00010180: 6573 735f 6675 6e63 7469 6f6e 5f6b 6579  ess_function_key
+00010190: 2873 656c 662e 4631 3129 0a20 2020 2020  (self.F11).     
+000101a0: 2020 2069 6620 6576 656e 742e 6b65 7928     if event.key(
+000101b0: 2920 3d3d 2051 742e 4b65 792e 4b65 795f  ) == Qt.Key.Key_
+000101c0: 4631 323a 0a20 2020 2020 2020 2020 2020  F12:.           
+000101d0: 2073 656c 662e 7072 6f63 6573 735f 6675   self.process_fu
+000101e0: 6e63 7469 6f6e 5f6b 6579 2873 656c 662e  nction_key(self.
+000101f0: 4631 3229 0a0a 2020 2020 6465 6620 7365  F12)..    def se
+00010200: 745f 7769 6e64 6f77 5f74 6974 6c65 2873  t_window_title(s
+00010210: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
+00010220: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00010230: 2020 5365 7420 7769 6e64 6f77 2074 6974    Set window tit
+00010240: 6c65 2062 6173 6564 206f 6e20 6375 7272  le based on curr
+00010250: 656e 7420 7374 6174 652e 0a20 2020 2020  ent state..     
+00010260: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
+00010270: 7666 6f61 203d 2073 656c 662e 7261 6469  vfoa = self.radi
+00010280: 6f5f 7374 6174 652e 6765 7428 2276 666f  o_state.get("vfo
+00010290: 6122 2c20 2222 290a 2020 2020 2020 2020  a", "").        
+000102a0: 6966 2076 666f 613a 0a20 2020 2020 2020  if vfoa:.       
+000102b0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+000102c0: 2020 2020 2020 2020 2020 7666 6f61 203d            vfoa =
+000102d0: 2069 6e74 2876 666f 6129 202f 2031 3030   int(vfoa) / 100
+000102e0: 300a 2020 2020 2020 2020 2020 2020 6578  0.            ex
+000102f0: 6365 7074 2056 616c 7565 4572 726f 723a  cept ValueError:
+00010300: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010310: 2076 666f 6120 3d20 302e 300a 2020 2020   vfoa = 0.0.    
+00010320: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00010330: 2020 2020 2020 7666 6f61 203d 2030 2e30        vfoa = 0.0
+00010340: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
+00010350: 5f6e 616d 6520 3d20 2222 0a20 2020 2020  _name = "".     
+00010360: 2020 2069 6620 7365 6c66 2e63 6f6e 7465     if self.conte
+00010370: 7374 3a0a 2020 2020 2020 2020 2020 2020  st:.            
+00010380: 636f 6e74 6573 745f 6e61 6d65 203d 2073  contest_name = s
+00010390: 656c 662e 636f 6e74 6573 742e 6e61 6d65  elf.contest.name
+000103a0: 0a20 2020 2020 2020 206c 696e 6520 3d20  .        line = 
+000103b0: 280a 2020 2020 2020 2020 2020 2020 6622  (.            f"
+000103c0: 7666 6f61 3a7b 726f 756e 6428 7666 6f61  vfoa:{round(vfoa
+000103d0: 2c32 297d 2022 0a20 2020 2020 2020 2020  ,2)} ".         
+000103e0: 2020 2066 226d 6f64 653a 7b73 656c 662e     f"mode:{self.
+000103f0: 7261 6469 6f5f 7374 6174 652e 6765 7428  radio_state.get(
+00010400: 276d 6f64 6527 2c20 2727 297d 2022 0a20  'mode', '')} ". 
+00010410: 2020 2020 2020 2020 2020 2066 224f 503a             f"OP:
+00010420: 7b73 656c 662e 6375 7272 656e 745f 6f70  {self.current_op
+00010430: 7d20 7b63 6f6e 7465 7374 5f6e 616d 657d  } {contest_name}
+00010440: 2022 0a20 2020 2020 2020 2020 2020 2066   ".            f
+00010450: 222d 204e 6f74 314d 4d20 767b 5f5f 7665  "- Not1MM v{__ve
+00010460: 7273 696f 6e5f 5f7d 220a 2020 2020 2020  rsion__}".      
+00010470: 2020 290a 2020 2020 2020 2020 7365 6c66    ).        self
+00010480: 2e73 6574 5769 6e64 6f77 5469 746c 6528  .setWindowTitle(
+00010490: 6c69 6e65 290a 0a20 2020 2064 6566 2073  line)..    def s
+000104a0: 656e 645f 776f 726b 6564 5f6c 6973 7428  end_worked_list(
+000104b0: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
+000104c0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000104d0: 2020 2053 656e 6420 6d65 7373 6167 6520     Send message 
+000104e0: 636f 6e74 6169 6e69 6e67 2077 6f72 6b65  containing worke
+000104f0: 6420 636f 6e74 6163 7473 2061 6e64 2062  d contacts and b
+00010500: 616e 6473 0a0a 2020 2020 2020 2020 5061  ands..        Pa
+00010510: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+00010520: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+00010530: 2020 2020 4e6f 6e65 0a0a 2020 2020 2020      None..      
+00010540: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
+00010550: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+00010560: 2020 4e6f 6e65 0a20 2020 2020 2020 2022    None.        "
+00010570: 2222 0a0a 2020 2020 2020 2020 636d 6420  ""..        cmd 
+00010580: 3d20 7b7d 0a20 2020 2020 2020 2063 6d64  = {}.        cmd
+00010590: 5b22 636d 6422 5d20 3d20 2257 4f52 4b45  ["cmd"] = "WORKE
+000105a0: 4422 0a20 2020 2020 2020 2063 6d64 5b22  D".        cmd["
+000105b0: 7374 6174 696f 6e22 5d20 3d20 706c 6174  station"] = plat
+000105c0: 666f 726d 2e6e 6f64 6528 290a 2020 2020  form.node().    
+000105d0: 2020 2020 636d 645b 2277 6f72 6b65 6422      cmd["worked"
+000105e0: 5d20 3d20 7365 6c66 2e77 6f72 6b65 645f  ] = self.worked_
+000105f0: 6c69 7374 0a20 2020 2020 2020 206c 6f67  list.        log
+00010600: 6765 722e 6465 6275 6728 2225 7322 2c20  ger.debug("%s", 
+00010610: 6622 7b63 6d64 7d22 290a 2020 2020 2020  f"{cmd}").      
+00010620: 2020 7365 6c66 2e6d 756c 7469 6361 7374    self.multicast
+00010630: 5f69 6e74 6572 6661 6365 2e73 656e 645f  _interface.send_
+00010640: 6173 5f6a 736f 6e28 636d 6429 0a0a 2020  as_json(cmd)..  
+00010650: 2020 6465 6620 636c 6561 7269 6e70 7574    def clearinput
+00010660: 7328 7365 6c66 2920 2d3e 204e 6f6e 653a  s(self) -> None:
+00010670: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00010680: 2020 2020 2043 6c65 6172 7320 7468 6520       Clears the 
+00010690: 7465 7874 2069 6e70 7574 2066 6965 6c64  text input field
+000106a0: 7320 616e 6420 7365 7473 2066 6f63 7573  s and sets focus
+000106b0: 2074 6f20 6361 6c6c 7369 676e 2066 6965   to callsign fie
+000106c0: 6c64 2e0a 0a20 2020 2020 2020 2050 6172  ld...        Par
+000106d0: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
+000106e0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+000106f0: 2020 204e 6f6e 650a 0a20 2020 2020 2020     None..       
+00010700: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
+00010710: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
+00010720: 204e 6f6e 650a 2020 2020 2020 2020 2222   None.        ""
+00010730: 220a 0a20 2020 2020 2020 2073 656c 662e  "..        self.
+00010740: 6475 7065 5f69 6e64 6963 6174 6f72 2e68  dupe_indicator.h
+00010750: 6964 6528 290a 2020 2020 2020 2020 7365  ide().        se
+00010760: 6c66 2e63 6f6e 7461 6374 203d 2073 656c  lf.contact = sel
+00010770: 662e 6461 7461 6261 7365 2e65 6d70 7479  f.database.empty
+00010780: 5f63 6f6e 7461 6374 0a20 2020 2020 2020  _contact.       
+00010790: 2073 656c 662e 6865 6164 696e 675f 6469   self.heading_di
+000107a0: 7374 616e 6365 2e73 6574 5465 7874 2822  stance.setText("
+000107b0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+000107c0: 6478 5f65 6e74 6974 792e 7365 7454 6578  dx_entity.setTex
+000107d0: 7428 2222 290a 2020 2020 2020 2020 6966  t("").        if
+000107e0: 2073 656c 662e 636f 6e74 6573 743a 0a20   self.contest:. 
+000107f0: 2020 2020 2020 2020 2020 206d 756c 7473             mults
+00010800: 203d 2073 656c 662e 636f 6e74 6573 742e   = self.contest.
+00010810: 7368 6f77 5f6d 756c 7473 2873 656c 6629  show_mults(self)
+00010820: 0a20 2020 2020 2020 2020 2020 2071 736f  .            qso
 00010830: 7320 3d20 7365 6c66 2e63 6f6e 7465 7374  s = self.contest
-00010840: 2e73 686f 775f 6d75 6c74 7328 7365 6c66  .show_mults(self
-00010850: 290a 2020 2020 2020 2020 2020 2020 7173  ).            qs
-00010860: 6f73 203d 2073 656c 662e 636f 6e74 6573  os = self.contes
-00010870: 742e 7368 6f77 5f71 736f 2873 656c 6629  t.show_qso(self)
-00010880: 0a20 2020 2020 2020 2020 2020 206d 756c  .            mul
-00010890: 7473 7472 696e 6720 3d20 6622 7b71 736f  tstring = f"{qso
-000108a0: 737d 2f7b 6d75 6c74 737d 220a 2020 2020  s}/{mults}".    
-000108b0: 2020 2020 2020 2020 7365 6c66 2e6d 756c          self.mul
-000108c0: 7473 2e73 6574 5465 7874 286d 756c 7473  ts.setText(mults
-000108d0: 7472 696e 6729 0a20 2020 2020 2020 2020  tring).         
-000108e0: 2020 2073 636f 7265 203d 2073 656c 662e     score = self.
-000108f0: 636f 6e74 6573 742e 6361 6c63 5f73 636f  contest.calc_sco
-00010900: 7265 2873 656c 6629 0a20 2020 2020 2020  re(self).       
-00010910: 2020 2020 2073 656c 662e 7363 6f72 652e       self.score.
-00010920: 7365 7454 6578 7428 7374 7228 7363 6f72  setText(str(scor
-00010930: 6529 290a 2020 2020 2020 2020 2020 2020  e)).            
-00010940: 7365 6c66 2e63 6f6e 7465 7374 2e72 6573  self.contest.res
-00010950: 6574 5f6c 6162 656c 2873 656c 6629 0a20  et_label(self). 
-00010960: 2020 2020 2020 2073 656c 662e 6361 6c6c         self.call
-00010970: 7369 676e 2e63 6c65 6172 2829 0a20 2020  sign.clear().   
-00010980: 2020 2020 2069 6620 7365 6c66 2e63 7572       if self.cur
-00010990: 7265 6e74 5f6d 6f64 6520 3d3d 2022 4357  rent_mode == "CW
-000109a0: 223a 0a20 2020 2020 2020 2020 2020 2073  ":.            s
-000109b0: 656c 662e 7365 6e74 2e73 6574 5465 7874  elf.sent.setText
-000109c0: 2822 3539 3922 290a 2020 2020 2020 2020  ("599").        
-000109d0: 2020 2020 7365 6c66 2e72 6563 6569 7665      self.receive
-000109e0: 2e73 6574 5465 7874 2822 3539 3922 290a  .setText("599").
-000109f0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00010a00: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00010a10: 656e 742e 7365 7454 6578 7428 2235 3922  ent.setText("59"
-00010a20: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00010a30: 6c66 2e72 6563 6569 7665 2e73 6574 5465  lf.receive.setTe
-00010a40: 7874 2822 3539 2229 0a20 2020 2020 2020  xt("59").       
-00010a50: 2073 656c 662e 6f74 6865 725f 312e 636c   self.other_1.cl
-00010a60: 6561 7228 290a 2020 2020 2020 2020 7365  ear().        se
-00010a70: 6c66 2e6f 7468 6572 5f32 2e63 6c65 6172  lf.other_2.clear
-00010a80: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-00010a90: 6361 6c6c 7369 676e 2e73 6574 466f 6375  callsign.setFocu
-00010aa0: 7328 290a 2020 2020 2020 2020 636d 6420  s().        cmd 
-00010ab0: 3d20 7b7d 0a20 2020 2020 2020 2063 6d64  = {}.        cmd
-00010ac0: 5b22 636d 6422 5d20 3d20 2243 414c 4c43  ["cmd"] = "CALLC
-00010ad0: 4841 4e47 4544 220a 2020 2020 2020 2020  HANGED".        
-00010ae0: 636d 645b 2273 7461 7469 6f6e 225d 203d  cmd["station"] =
-00010af0: 2070 6c61 7466 6f72 6d2e 6e6f 6465 2829   platform.node()
-00010b00: 0a20 2020 2020 2020 2063 6d64 5b22 6361  .        cmd["ca
-00010b10: 6c6c 225d 203d 2022 220a 2020 2020 2020  ll"] = "".      
-00010b20: 2020 7365 6c66 2e6d 756c 7469 6361 7374    self.multicast
-00010b30: 5f69 6e74 6572 6661 6365 2e73 656e 645f  _interface.send_
-00010b40: 6173 5f6a 736f 6e28 636d 6429 0a0a 2020  as_json(cmd)..  
-00010b50: 2020 6465 6620 7361 7665 5f63 6f6e 7461    def save_conta
-00010b60: 6374 2873 656c 6629 202d 3e20 4e6f 6e65  ct(self) -> None
-00010b70: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00010b80: 2020 2020 2020 5361 7665 2063 6f6e 7461        Save conta
-00010b90: 6374 2074 6f20 6461 7461 6261 7365 2e0a  ct to database..
-00010ba0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-00010bb0: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
-00010bc0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 204e  ------.        N
-00010bd0: 6f6e 650a 0a20 2020 2020 2020 2052 6574  one..        Ret
-00010be0: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
-00010bf0: 2d2d 2d2d 0a20 2020 2020 2020 204e 6f6e  ----.        Non
-00010c00: 650a 2020 2020 2020 2020 2222 220a 0a20  e.        """.. 
-00010c10: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-00010c20: 6275 6728 2273 6176 696e 6720 636f 6e74  bug("saving cont
-00010c30: 6163 7422 290a 2020 2020 2020 2020 6966  act").        if
-00010c40: 2073 656c 662e 636f 6e74 6573 7420 6973   self.contest is
-00010c50: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00010c60: 2020 2073 656c 662e 7368 6f77 5f6d 6573     self.show_mes
-00010c70: 7361 6765 5f62 6f78 2822 596f 7520 6861  sage_box("You ha
-00010c80: 7665 206e 6f20 636f 6e74 6573 7420 6465  ve no contest de
-00010c90: 6669 6e65 642e 2229 0a20 2020 2020 2020  fined.").       
-00010ca0: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-00010cb0: 2020 2020 6966 206c 656e 2873 656c 662e      if len(self.
-00010cc0: 6361 6c6c 7369 676e 2e74 6578 7428 2929  callsign.text())
-00010cd0: 203c 2033 3a0a 2020 2020 2020 2020 2020   < 3:.          
-00010ce0: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-00010cf0: 2069 6620 6e6f 7420 616e 7928 6368 6172   if not any(char
-00010d00: 2e69 7364 6967 6974 2829 2066 6f72 2063  .isdigit() for c
-00010d10: 6861 7220 696e 2073 656c 662e 6361 6c6c  har in self.call
-00010d20: 7369 676e 2e74 6578 7428 2929 3a0a 2020  sign.text()):.  
-00010d30: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00010d40: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00010d50: 616e 7928 6368 6172 2e69 7361 6c70 6861  any(char.isalpha
-00010d60: 2829 2066 6f72 2063 6861 7220 696e 2073  () for char in s
-00010d70: 656c 662e 6361 6c6c 7369 676e 2e74 6578  elf.callsign.tex
-00010d80: 7428 2929 3a0a 2020 2020 2020 2020 2020  t()):.          
-00010d90: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-00010da0: 2073 656c 662e 636f 6e74 6163 745b 2254   self.contact["T
-00010db0: 5322 5d20 3d20 6461 7465 7469 6d65 2e64  S"] = datetime.d
-00010dc0: 6174 6574 696d 652e 6e6f 7728 6461 7465  atetime.now(date
-00010dd0: 7469 6d65 2e74 696d 657a 6f6e 652e 7574  time.timezone.ut
-00010de0: 6329 2e69 736f 666f 726d 6174 280a 2020  c).isoformat(.  
-00010df0: 2020 2020 2020 2020 2020 2220 220a 2020            " ".  
-00010e00: 2020 2020 2020 295b 3a31 395d 0a20 2020        )[:19].   
-00010e10: 2020 2020 2073 656c 662e 636f 6e74 6163       self.contac
-00010e20: 745b 2243 616c 6c22 5d20 3d20 7365 6c66  t["Call"] = self
-00010e30: 2e63 616c 6c73 6967 6e2e 7465 7874 2829  .callsign.text()
-00010e40: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-00010e50: 6e74 6163 745b 2246 7265 7122 5d20 3d20  ntact["Freq"] = 
-00010e60: 726f 756e 6428 666c 6f61 7428 7365 6c66  round(float(self
-00010e70: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
-00010e80: 2822 7666 6f61 222c 2030 2e30 2929 202f  ("vfoa", 0.0)) /
-00010e90: 2031 3030 302c 2032 290a 2020 2020 2020   1000, 2).      
-00010ea0: 2020 7365 6c66 2e63 6f6e 7461 6374 5b22    self.contact["
-00010eb0: 5153 5846 7265 7122 5d20 3d20 726f 756e  QSXFreq"] = roun
-00010ec0: 6428 0a20 2020 2020 2020 2020 2020 2066  d(.            f
-00010ed0: 6c6f 6174 2873 656c 662e 7261 6469 6f5f  loat(self.radio_
-00010ee0: 7374 6174 652e 6765 7428 2276 666f 6122  state.get("vfoa"
-00010ef0: 2c20 302e 3029 2920 2f20 3130 3030 2c20  , 0.0)) / 1000, 
-00010f00: 320a 2020 2020 2020 2020 290a 2020 2020  2.        ).    
-00010f10: 2020 2020 7365 6c66 2e63 6f6e 7461 6374      self.contact
-00010f20: 5b22 4d6f 6465 225d 203d 2073 656c 662e  ["Mode"] = self.
-00010f30: 7261 6469 6f5f 7374 6174 652e 6765 7428  radio_state.get(
-00010f40: 226d 6f64 6522 2c20 2222 290a 2020 2020  "mode", "").    
-00010f50: 2020 2020 7365 6c66 2e63 6f6e 7461 6374      self.contact
-00010f60: 5b22 436f 6e74 6573 744e 616d 6522 5d20  ["ContestName"] 
-00010f70: 3d20 7365 6c66 2e63 6f6e 7465 7374 2e63  = self.contest.c
-00010f80: 6162 7269 6c6c 6f5f 6e61 6d65 0a20 2020  abrillo_name.   
-00010f90: 2020 2020 2073 656c 662e 636f 6e74 6163       self.contac
-00010fa0: 745b 2243 6f6e 7465 7374 4e52 225d 203d  t["ContestNR"] =
-00010fb0: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
-00010fc0: 636f 6e74 6573 7422 2c20 2230 2229 0a20  contest", "0"). 
-00010fd0: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
-00010fe0: 6163 745b 2253 7461 7469 6f6e 5072 6566  act["StationPref
-00010ff0: 6978 225d 203d 2073 656c 662e 7374 6174  ix"] = self.stat
-00011000: 696f 6e2e 6765 7428 2243 616c 6c22 2c20  ion.get("Call", 
-00011010: 2222 290a 2020 2020 2020 2020 7365 6c66  "").        self
-00011020: 2e63 6f6e 7461 6374 5b22 5750 5850 7265  .contact["WPXPre
-00011030: 6669 7822 5d20 3d20 6361 6c63 756c 6174  fix"] = calculat
-00011040: 655f 7770 785f 7072 6566 6978 2873 656c  e_wpx_prefix(sel
-00011050: 662e 6361 6c6c 7369 676e 2e74 6578 7428  f.callsign.text(
-00011060: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-00011070: 636f 6e74 6163 745b 2249 7352 756e 5153  contact["IsRunQS
-00011080: 4f22 5d20 3d20 7365 6c66 2e72 6164 696f  O"] = self.radio
-00011090: 4275 7474 6f6e 5f72 756e 2e69 7343 6865  Button_run.isChe
-000110a0: 636b 6564 2829 0a20 2020 2020 2020 2073  cked().        s
-000110b0: 656c 662e 636f 6e74 6163 745b 224f 7065  elf.contact["Ope
-000110c0: 7261 746f 7222 5d20 3d20 7365 6c66 2e63  rator"] = self.c
-000110d0: 7572 7265 6e74 5f6f 700a 2020 2020 2020  urrent_op.      
-000110e0: 2020 7365 6c66 2e63 6f6e 7461 6374 5b22    self.contact["
-000110f0: 4e65 7442 696f 734e 616d 6522 5d20 3d20  NetBiosName"] = 
-00011100: 736f 636b 6574 2e67 6574 686f 7374 6e61  socket.gethostna
-00011110: 6d65 2829 0a20 2020 2020 2020 2073 656c  me().        sel
-00011120: 662e 636f 6e74 6163 745b 2249 734f 7269  f.contact["IsOri
-00011130: 6769 6e61 6c22 5d20 3d20 310a 2020 2020  ginal"] = 1.    
-00011140: 2020 2020 7365 6c66 2e63 6f6e 7461 6374      self.contact
-00011150: 5b22 4944 225d 203d 2075 7569 642e 7575  ["ID"] = uuid.uu
-00011160: 6964 3428 292e 6865 780a 2020 2020 2020  id4().hex.      
-00011170: 2020 7365 6c66 2e63 6f6e 7465 7374 2e73    self.contest.s
-00011180: 6574 5f63 6f6e 7461 6374 5f76 6172 7328  et_contact_vars(
-00011190: 7365 6c66 290a 2020 2020 2020 2020 7365  self).        se
-000111a0: 6c66 2e63 6f6e 7461 6374 5b22 506f 696e  lf.contact["Poin
-000111b0: 7473 225d 203d 2073 656c 662e 636f 6e74  ts"] = self.cont
-000111c0: 6573 742e 706f 696e 7473 2873 656c 6629  est.points(self)
-000111d0: 0a20 2020 2020 2020 2064 6562 7567 5f6f  .        debug_o
-000111e0: 7574 7075 7420 3d20 6622 7b73 656c 662e  utput = f"{self.
-000111f0: 636f 6e74 6163 747d 220a 2020 2020 2020  contact}".      
-00011200: 2020 6c6f 6767 6572 2e64 6562 7567 2864    logger.debug(d
-00011210: 6562 7567 5f6f 7574 7075 7429 0a0a 2020  ebug_output)..  
-00011220: 2020 2020 2020 6966 2073 656c 662e 6e31        if self.n1
-00011230: 6d6d 3a0a 2020 2020 2020 2020 2020 2020  mm:.            
-00011240: 6c6f 6767 6572 2e64 6562 7567 2822 7061  logger.debug("pa
-00011250: 636b 6574 7320 2573 222c 2066 227b 7365  ckets %s", f"{se
+00010840: 2e73 686f 775f 7173 6f28 7365 6c66 290a  .show_qso(self).
+00010850: 2020 2020 2020 2020 2020 2020 6d75 6c74              mult
+00010860: 7374 7269 6e67 203d 2066 227b 7173 6f73  string = f"{qsos
+00010870: 7d2f 7b6d 756c 7473 7d22 0a20 2020 2020  }/{mults}".     
+00010880: 2020 2020 2020 2073 656c 662e 6d75 6c74         self.mult
+00010890: 732e 7365 7454 6578 7428 6d75 6c74 7374  s.setText(multst
+000108a0: 7269 6e67 290a 2020 2020 2020 2020 2020  ring).          
+000108b0: 2020 7363 6f72 6520 3d20 7365 6c66 2e63    score = self.c
+000108c0: 6f6e 7465 7374 2e63 616c 635f 7363 6f72  ontest.calc_scor
+000108d0: 6528 7365 6c66 290a 2020 2020 2020 2020  e(self).        
+000108e0: 2020 2020 7365 6c66 2e73 636f 7265 2e73      self.score.s
+000108f0: 6574 5465 7874 2873 7472 2873 636f 7265  etText(str(score
+00010900: 2929 0a20 2020 2020 2020 2020 2020 2073  )).            s
+00010910: 656c 662e 636f 6e74 6573 742e 7265 7365  elf.contest.rese
+00010920: 745f 6c61 6265 6c28 7365 6c66 290a 2020  t_label(self).  
+00010930: 2020 2020 2020 7365 6c66 2e63 616c 6c73        self.calls
+00010940: 6967 6e2e 636c 6561 7228 290a 2020 2020  ign.clear().    
+00010950: 2020 2020 6966 2073 656c 662e 6375 7272      if self.curr
+00010960: 656e 745f 6d6f 6465 203d 3d20 2243 5722  ent_mode == "CW"
+00010970: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00010980: 6c66 2e73 656e 742e 7365 7454 6578 7428  lf.sent.setText(
+00010990: 2235 3939 2229 0a20 2020 2020 2020 2020  "599").         
+000109a0: 2020 2073 656c 662e 7265 6365 6976 652e     self.receive.
+000109b0: 7365 7454 6578 7428 2235 3939 2229 0a20  setText("599"). 
+000109c0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+000109d0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+000109e0: 6e74 2e73 6574 5465 7874 2822 3539 2229  nt.setText("59")
+000109f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00010a00: 662e 7265 6365 6976 652e 7365 7454 6578  f.receive.setTex
+00010a10: 7428 2235 3922 290a 2020 2020 2020 2020  t("59").        
+00010a20: 7365 6c66 2e6f 7468 6572 5f31 2e63 6c65  self.other_1.cle
+00010a30: 6172 2829 0a20 2020 2020 2020 2073 656c  ar().        sel
+00010a40: 662e 6f74 6865 725f 322e 636c 6561 7228  f.other_2.clear(
+00010a50: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+00010a60: 616c 6c73 6967 6e2e 7365 7446 6f63 7573  allsign.setFocus
+00010a70: 2829 0a20 2020 2020 2020 2063 6d64 203d  ().        cmd =
+00010a80: 207b 7d0a 2020 2020 2020 2020 636d 645b   {}.        cmd[
+00010a90: 2263 6d64 225d 203d 2022 4341 4c4c 4348  "cmd"] = "CALLCH
+00010aa0: 414e 4745 4422 0a20 2020 2020 2020 2063  ANGED".        c
+00010ab0: 6d64 5b22 7374 6174 696f 6e22 5d20 3d20  md["station"] = 
+00010ac0: 706c 6174 666f 726d 2e6e 6f64 6528 290a  platform.node().
+00010ad0: 2020 2020 2020 2020 636d 645b 2263 616c          cmd["cal
+00010ae0: 6c22 5d20 3d20 2222 0a20 2020 2020 2020  l"] = "".       
+00010af0: 2073 656c 662e 6d75 6c74 6963 6173 745f   self.multicast_
+00010b00: 696e 7465 7266 6163 652e 7365 6e64 5f61  interface.send_a
+00010b10: 735f 6a73 6f6e 2863 6d64 290a 0a20 2020  s_json(cmd)..   
+00010b20: 2064 6566 2073 6176 655f 636f 6e74 6163   def save_contac
+00010b30: 7428 7365 6c66 2920 2d3e 204e 6f6e 653a  t(self) -> None:
+00010b40: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00010b50: 2020 2020 2053 6176 6520 636f 6e74 6163       Save contac
+00010b60: 7420 746f 2064 6174 6162 6173 652e 0a0a  t to database...
+00010b70: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+00010b80: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
+00010b90: 2d2d 2d2d 2d0a 2020 2020 2020 2020 4e6f  -----.        No
+00010ba0: 6e65 0a0a 2020 2020 2020 2020 5265 7475  ne..        Retu
+00010bb0: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
+00010bc0: 2d2d 2d0a 2020 2020 2020 2020 4e6f 6e65  ---.        None
+00010bd0: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
+00010be0: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+00010bf0: 7567 2822 7361 7669 6e67 2063 6f6e 7461  ug("saving conta
+00010c00: 6374 2229 0a20 2020 2020 2020 2069 6620  ct").        if 
+00010c10: 7365 6c66 2e63 6f6e 7465 7374 2069 7320  self.contest is 
+00010c20: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00010c30: 2020 7365 6c66 2e73 686f 775f 6d65 7373    self.show_mess
+00010c40: 6167 655f 626f 7828 2259 6f75 2068 6176  age_box("You hav
+00010c50: 6520 6e6f 2063 6f6e 7465 7374 2064 6566  e no contest def
+00010c60: 696e 6564 2e22 290a 2020 2020 2020 2020  ined.").        
+00010c70: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+00010c80: 2020 2069 6620 6c65 6e28 7365 6c66 2e63     if len(self.c
+00010c90: 616c 6c73 6967 6e2e 7465 7874 2829 2920  allsign.text()) 
+00010ca0: 3c20 333a 0a20 2020 2020 2020 2020 2020  < 3:.           
+00010cb0: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
+00010cc0: 6966 206e 6f74 2061 6e79 2863 6861 722e  if not any(char.
+00010cd0: 6973 6469 6769 7428 2920 666f 7220 6368  isdigit() for ch
+00010ce0: 6172 2069 6e20 7365 6c66 2e63 616c 6c73  ar in self.calls
+00010cf0: 6967 6e2e 7465 7874 2829 293a 0a20 2020  ign.text()):.   
+00010d00: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+00010d10: 2020 2020 2020 2020 6966 206e 6f74 2061          if not a
+00010d20: 6e79 2863 6861 722e 6973 616c 7068 6128  ny(char.isalpha(
+00010d30: 2920 666f 7220 6368 6172 2069 6e20 7365  ) for char in se
+00010d40: 6c66 2e63 616c 6c73 6967 6e2e 7465 7874  lf.callsign.text
+00010d50: 2829 293a 0a20 2020 2020 2020 2020 2020  ()):.           
+00010d60: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
+00010d70: 7365 6c66 2e63 6f6e 7461 6374 5b22 5453  self.contact["TS
+00010d80: 225d 203d 2064 6174 6574 696d 652e 6461  "] = datetime.da
+00010d90: 7465 7469 6d65 2e6e 6f77 2864 6174 6574  tetime.now(datet
+00010da0: 696d 652e 7469 6d65 7a6f 6e65 2e75 7463  ime.timezone.utc
+00010db0: 292e 6973 6f66 6f72 6d61 7428 0a20 2020  ).isoformat(.   
+00010dc0: 2020 2020 2020 2020 2022 2022 0a20 2020           " ".   
+00010dd0: 2020 2020 2029 5b3a 3139 5d0a 2020 2020       )[:19].    
+00010de0: 2020 2020 7365 6c66 2e63 6f6e 7461 6374      self.contact
+00010df0: 5b22 4361 6c6c 225d 203d 2073 656c 662e  ["Call"] = self.
+00010e00: 6361 6c6c 7369 676e 2e74 6578 7428 290a  callsign.text().
+00010e10: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+00010e20: 7461 6374 5b22 4672 6571 225d 203d 2072  tact["Freq"] = r
+00010e30: 6f75 6e64 2866 6c6f 6174 2873 656c 662e  ound(float(self.
+00010e40: 7261 6469 6f5f 7374 6174 652e 6765 7428  radio_state.get(
+00010e50: 2276 666f 6122 2c20 302e 3029 2920 2f20  "vfoa", 0.0)) / 
+00010e60: 3130 3030 2c20 3229 0a20 2020 2020 2020  1000, 2).       
+00010e70: 2073 656c 662e 636f 6e74 6163 745b 2251   self.contact["Q
+00010e80: 5358 4672 6571 225d 203d 2072 6f75 6e64  SXFreq"] = round
+00010e90: 280a 2020 2020 2020 2020 2020 2020 666c  (.            fl
+00010ea0: 6f61 7428 7365 6c66 2e72 6164 696f 5f73  oat(self.radio_s
+00010eb0: 7461 7465 2e67 6574 2822 7666 6f61 222c  tate.get("vfoa",
+00010ec0: 2030 2e30 2929 202f 2031 3030 302c 2032   0.0)) / 1000, 2
+00010ed0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+00010ee0: 2020 2073 656c 662e 636f 6e74 6163 745b     self.contact[
+00010ef0: 224d 6f64 6522 5d20 3d20 7365 6c66 2e72  "Mode"] = self.r
+00010f00: 6164 696f 5f73 7461 7465 2e67 6574 2822  adio_state.get("
+00010f10: 6d6f 6465 222c 2022 2229 0a20 2020 2020  mode", "").     
+00010f20: 2020 2073 656c 662e 636f 6e74 6163 745b     self.contact[
+00010f30: 2243 6f6e 7465 7374 4e61 6d65 225d 203d  "ContestName"] =
+00010f40: 2073 656c 662e 636f 6e74 6573 742e 6361   self.contest.ca
+00010f50: 6272 696c 6c6f 5f6e 616d 650a 2020 2020  brillo_name.    
+00010f60: 2020 2020 7365 6c66 2e63 6f6e 7461 6374      self.contact
+00010f70: 5b22 436f 6e74 6573 744e 5222 5d20 3d20  ["ContestNR"] = 
+00010f80: 7365 6c66 2e70 7265 662e 6765 7428 2263  self.pref.get("c
+00010f90: 6f6e 7465 7374 222c 2022 3022 290a 2020  ontest", "0").  
+00010fa0: 2020 2020 2020 7365 6c66 2e63 6f6e 7461        self.conta
+00010fb0: 6374 5b22 5374 6174 696f 6e50 7265 6669  ct["StationPrefi
+00010fc0: 7822 5d20 3d20 7365 6c66 2e73 7461 7469  x"] = self.stati
+00010fd0: 6f6e 2e67 6574 2822 4361 6c6c 222c 2022  on.get("Call", "
+00010fe0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+00010ff0: 636f 6e74 6163 745b 2257 5058 5072 6566  contact["WPXPref
+00011000: 6978 225d 203d 2063 616c 6375 6c61 7465  ix"] = calculate
+00011010: 5f77 7078 5f70 7265 6669 7828 7365 6c66  _wpx_prefix(self
+00011020: 2e63 616c 6c73 6967 6e2e 7465 7874 2829  .callsign.text()
+00011030: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+00011040: 6f6e 7461 6374 5b22 4973 5275 6e51 534f  ontact["IsRunQSO
+00011050: 225d 203d 2073 656c 662e 7261 6469 6f42  "] = self.radioB
+00011060: 7574 746f 6e5f 7275 6e2e 6973 4368 6563  utton_run.isChec
+00011070: 6b65 6428 290a 2020 2020 2020 2020 7365  ked().        se
+00011080: 6c66 2e63 6f6e 7461 6374 5b22 4f70 6572  lf.contact["Oper
+00011090: 6174 6f72 225d 203d 2073 656c 662e 6375  ator"] = self.cu
+000110a0: 7272 656e 745f 6f70 0a20 2020 2020 2020  rrent_op.       
+000110b0: 2073 656c 662e 636f 6e74 6163 745b 224e   self.contact["N
+000110c0: 6574 4269 6f73 4e61 6d65 225d 203d 2073  etBiosName"] = s
+000110d0: 6f63 6b65 742e 6765 7468 6f73 746e 616d  ocket.gethostnam
+000110e0: 6528 290a 2020 2020 2020 2020 7365 6c66  e().        self
+000110f0: 2e63 6f6e 7461 6374 5b22 4973 4f72 6967  .contact["IsOrig
+00011100: 696e 616c 225d 203d 2031 0a20 2020 2020  inal"] = 1.     
+00011110: 2020 2073 656c 662e 636f 6e74 6163 745b     self.contact[
+00011120: 2249 4422 5d20 3d20 7575 6964 2e75 7569  "ID"] = uuid.uui
+00011130: 6434 2829 2e68 6578 0a20 2020 2020 2020  d4().hex.       
+00011140: 2073 656c 662e 636f 6e74 6573 742e 7365   self.contest.se
+00011150: 745f 636f 6e74 6163 745f 7661 7273 2873  t_contact_vars(s
+00011160: 656c 6629 0a20 2020 2020 2020 2073 656c  elf).        sel
+00011170: 662e 636f 6e74 6163 745b 2250 6f69 6e74  f.contact["Point
+00011180: 7322 5d20 3d20 7365 6c66 2e63 6f6e 7465  s"] = self.conte
+00011190: 7374 2e70 6f69 6e74 7328 7365 6c66 290a  st.points(self).
+000111a0: 2020 2020 2020 2020 6465 6275 675f 6f75          debug_ou
+000111b0: 7470 7574 203d 2066 227b 7365 6c66 2e63  tput = f"{self.c
+000111c0: 6f6e 7461 6374 7d22 0a20 2020 2020 2020  ontact}".       
+000111d0: 206c 6f67 6765 722e 6465 6275 6728 6465   logger.debug(de
+000111e0: 6275 675f 6f75 7470 7574 290a 0a20 2020  bug_output)..   
+000111f0: 2020 2020 2069 6620 7365 6c66 2e6e 316d       if self.n1m
+00011200: 6d3a 0a20 2020 2020 2020 2020 2020 206c  m:.            l
+00011210: 6f67 6765 722e 6465 6275 6728 2270 6163  ogger.debug("pac
+00011220: 6b65 7473 2025 7322 2c20 6622 7b73 656c  kets %s", f"{sel
+00011230: 662e 6e31 6d6d 2e73 656e 645f 636f 6e74  f.n1mm.send_cont
+00011240: 6163 745f 7061 636b 6574 737d 2229 0a20  act_packets}"). 
+00011250: 2020 2020 2020 2020 2020 2069 6620 7365             if se
 00011260: 6c66 2e6e 316d 6d2e 7365 6e64 5f63 6f6e  lf.n1mm.send_con
-00011270: 7461 6374 5f70 6163 6b65 7473 7d22 290a  tact_packets}").
-00011280: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00011290: 656c 662e 6e31 6d6d 2e73 656e 645f 636f  elf.n1mm.send_co
-000112a0: 6e74 6163 745f 7061 636b 6574 733a 0a20  ntact_packets:. 
-000112b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000112c0: 656c 662e 6e31 6d6d 2e63 6f6e 7461 6374  elf.n1mm.contact
-000112d0: 5f69 6e66 6f5b 2274 696d 6573 7461 6d70  _info["timestamp
-000112e0: 225d 203d 2073 656c 662e 636f 6e74 6163  "] = self.contac
-000112f0: 745b 2254 5322 5d0a 2020 2020 2020 2020  t["TS"].        
-00011300: 2020 2020 2020 2020 7365 6c66 2e6e 316d          self.n1m
-00011310: 6d2e 636f 6e74 6163 745f 696e 666f 5b22  m.contact_info["
-00011320: 6f6c 6463 616c 6c22 5d20 3d20 7365 6c66  oldcall"] = self
-00011330: 2e6e 316d 6d2e 636f 6e74 6163 745f 696e  .n1mm.contact_in
-00011340: 666f 5b22 6361 6c6c 225d 203d 2028 0a20  fo["call"] = (. 
-00011350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011360: 2020 2073 656c 662e 636f 6e74 6163 745b     self.contact[
-00011370: 2243 616c 6c22 5d0a 2020 2020 2020 2020  "Call"].        
-00011380: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00011390: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-000113a0: 316d 6d2e 636f 6e74 6163 745f 696e 666f  1mm.contact_info
-000113b0: 5b22 7478 6672 6571 225d 203d 2073 656c  ["txfreq"] = sel
-000113c0: 662e 6e31 6d6d 2e63 6f6e 7461 6374 5f69  f.n1mm.contact_i
-000113d0: 6e66 6f5b 2272 7866 7265 7122 5d20 3d20  nfo["rxfreq"] = 
-000113e0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000113f0: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
-00011400: 7261 6469 6f5f 696e 666f 5b22 4672 6571  radio_info["Freq
-00011410: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
-00011420: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00011430: 2020 2020 2073 656c 662e 6e31 6d6d 2e63       self.n1mm.c
-00011440: 6f6e 7461 6374 5f69 6e66 6f5b 226d 6f64  ontact_info["mod
-00011450: 6522 5d20 3d20 7365 6c66 2e63 6f6e 7461  e"] = self.conta
-00011460: 6374 5b22 4d6f 6465 225d 0a20 2020 2020  ct["Mode"].     
-00011470: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00011480: 6e31 6d6d 2e63 6f6e 7461 6374 5f69 6e66  n1mm.contact_inf
-00011490: 6f5b 2263 6f6e 7465 7374 6e61 6d65 225d  o["contestname"]
-000114a0: 203d 2073 656c 662e 636f 6e74 6163 745b   = self.contact[
-000114b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000114c0: 2020 2020 2022 436f 6e74 6573 744e 616d       "ContestNam
-000114d0: 6522 0a20 2020 2020 2020 2020 2020 2020  e".             
-000114e0: 2020 205d 2e72 6570 6c61 6365 2822 2d22     ].replace("-"
-000114f0: 2c20 2222 290a 2020 2020 2020 2020 2020  , "").          
-00011500: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
-00011510: 636f 6e74 6163 745f 696e 666f 5b22 636f  contact_info["co
-00011520: 6e74 6573 746e 7222 5d20 3d20 7365 6c66  ntestnr"] = self
-00011530: 2e63 6f6e 7461 6374 5b22 436f 6e74 6573  .contact["Contes
-00011540: 744e 5222 5d0a 2020 2020 2020 2020 2020  tNR"].          
-00011550: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
-00011560: 636f 6e74 6163 745f 696e 666f 5b22 7374  contact_info["st
-00011570: 6174 696f 6e70 7265 6669 7822 5d20 3d20  ationprefix"] = 
-00011580: 7365 6c66 2e63 6f6e 7461 6374 5b22 5374  self.contact["St
-00011590: 6174 696f 6e50 7265 6669 7822 5d0a 2020  ationPrefix"].  
-000115a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000115b0: 6c66 2e6e 316d 6d2e 636f 6e74 6163 745f  lf.n1mm.contact_
-000115c0: 696e 666f 5b22 7770 7870 7265 6669 7822  info["wpxprefix"
-000115d0: 5d20 3d20 7365 6c66 2e63 6f6e 7461 6374  ] = self.contact
-000115e0: 5b22 5750 5850 7265 6669 7822 5d0a 2020  ["WPXPrefix"].  
-000115f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00011600: 6c66 2e6e 316d 6d2e 636f 6e74 6163 745f  lf.n1mm.contact_
-00011610: 696e 666f 5b22 4973 5275 6e51 534f 225d  info["IsRunQSO"]
-00011620: 203d 2073 656c 662e 636f 6e74 6163 745b   = self.contact[
-00011630: 2249 7352 756e 5153 4f22 5d0a 2020 2020  "IsRunQSO"].    
-00011640: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00011650: 2e6e 316d 6d2e 636f 6e74 6163 745f 696e  .n1mm.contact_in
-00011660: 666f 5b22 6f70 6572 6174 6f72 225d 203d  fo["operator"] =
-00011670: 2073 656c 662e 636f 6e74 6163 745b 224f   self.contact["O
-00011680: 7065 7261 746f 7222 5d0a 2020 2020 2020  perator"].      
-00011690: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-000116a0: 316d 6d2e 636f 6e74 6163 745f 696e 666f  1mm.contact_info
-000116b0: 5b22 6d79 6361 6c6c 225d 203d 2073 656c  ["mycall"] = sel
-000116c0: 662e 636f 6e74 6163 745b 224f 7065 7261  f.contact["Opera
-000116d0: 746f 7222 5d0a 2020 2020 2020 2020 2020  tor"].          
-000116e0: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
-000116f0: 636f 6e74 6163 745f 696e 666f 5b22 5374  contact_info["St
-00011700: 6174 696f 6e4e 616d 6522 5d20 3d20 7365  ationName"] = se
-00011710: 6c66 2e6e 316d 6d2e 636f 6e74 6163 745f  lf.n1mm.contact_
-00011720: 696e 666f 5b0a 2020 2020 2020 2020 2020  info[.          
-00011730: 2020 2020 2020 2020 2020 224e 6574 4269            "NetBi
-00011740: 6f73 4e61 6d65 220a 2020 2020 2020 2020  osName".        
-00011750: 2020 2020 2020 2020 5d20 3d20 7365 6c66          ] = self
-00011760: 2e63 6f6e 7461 6374 5b22 4e65 7442 696f  .contact["NetBio
-00011770: 734e 616d 6522 5d0a 2020 2020 2020 2020  sName"].        
-00011780: 2020 2020 2020 2020 7365 6c66 2e6e 316d          self.n1m
-00011790: 6d2e 636f 6e74 6163 745f 696e 666f 5b22  m.contact_info["
-000117a0: 4973 4f72 6967 696e 616c 225d 203d 2073  IsOriginal"] = s
-000117b0: 656c 662e 636f 6e74 6163 745b 2249 734f  elf.contact["IsO
-000117c0: 7269 6769 6e61 6c22 5d0a 2020 2020 2020  riginal"].      
-000117d0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-000117e0: 316d 6d2e 636f 6e74 6163 745f 696e 666f  1mm.contact_info
-000117f0: 5b22 4944 225d 203d 2073 656c 662e 636f  ["ID"] = self.co
-00011800: 6e74 6163 745b 2249 4422 5d0a 2020 2020  ntact["ID"].    
-00011810: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00011820: 2e6e 316d 6d2e 636f 6e74 6163 745f 696e  .n1mm.contact_in
-00011830: 666f 5b22 706f 696e 7473 225d 203d 2073  fo["points"] = s
-00011840: 656c 662e 636f 6e74 6163 745b 2250 6f69  elf.contact["Poi
-00011850: 6e74 7322 5d0a 2020 2020 2020 2020 2020  nts"].          
-00011860: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
-00011870: 636f 6e74 6163 745f 696e 666f 5b22 736e  contact_info["sn
-00011880: 7422 5d20 3d20 7365 6c66 2e63 6f6e 7461  t"] = self.conta
-00011890: 6374 5b22 534e 5422 5d0a 2020 2020 2020  ct["SNT"].      
-000118a0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-000118b0: 316d 6d2e 636f 6e74 6163 745f 696e 666f  1mm.contact_info
-000118c0: 5b22 7263 7622 5d20 3d20 7365 6c66 2e63  ["rcv"] = self.c
-000118d0: 6f6e 7461 6374 5b22 5243 5622 5d0a 2020  ontact["RCV"].  
-000118e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000118f0: 6c66 2e6e 316d 6d2e 636f 6e74 6163 745f  lf.n1mm.contact_
-00011900: 696e 666f 5b22 736e 746e 7222 5d20 3d20  info["sntnr"] = 
-00011910: 7365 6c66 2e63 6f6e 7461 6374 5b22 5365  self.contact["Se
-00011920: 6e74 4e72 225d 0a20 2020 2020 2020 2020  ntNr"].         
-00011930: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
-00011940: 2e63 6f6e 7461 6374 5f69 6e66 6f5b 2272  .contact_info["r
-00011950: 6376 6e72 225d 203d 2073 656c 662e 636f  cvnr"] = self.co
-00011960: 6e74 6163 745b 224e 5222 5d0a 2020 2020  ntact["NR"].    
-00011970: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00011980: 2e6e 316d 6d2e 636f 6e74 6163 745f 696e  .n1mm.contact_in
-00011990: 666f 5b22 6973 6d75 6c74 6970 6c69 6572  fo["ismultiplier
-000119a0: 3122 5d20 3d20 7365 6c66 2e63 6f6e 7461  1"] = self.conta
-000119b0: 6374 2e67 6574 280a 2020 2020 2020 2020  ct.get(.        
-000119c0: 2020 2020 2020 2020 2020 2020 2249 734d              "IsM
-000119d0: 756c 7469 706c 6965 7231 222c 2030 0a20  ultiplier1", 0. 
-000119e0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-000119f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011a00: 2073 656c 662e 6e31 6d6d 2e63 6f6e 7461   self.n1mm.conta
-00011a10: 6374 5f69 6e66 6f5b 2269 736d 756c 7469  ct_info["ismulti
-00011a20: 706c 6965 7232 225d 203d 2073 656c 662e  plier2"] = self.
-00011a30: 636f 6e74 6163 742e 6765 7428 0a20 2020  contact.get(.   
-00011a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a50: 2022 4973 4d75 6c74 6970 6c69 6572 3222   "IsMultiplier2"
-00011a60: 2c20 300a 2020 2020 2020 2020 2020 2020  , 0.            
-00011a70: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00011a80: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
-00011a90: 636f 6e74 6163 745f 696e 666f 5b22 6973  contact_info["is
-00011aa0: 6d75 6c74 6970 6c69 6572 3322 5d20 3d20  multiplier3"] = 
-00011ab0: 7365 6c66 2e63 6f6e 7461 6374 2e67 6574  self.contact.get
-00011ac0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00011ad0: 2020 2020 2020 2249 734d 756c 7469 706c        "IsMultipl
-00011ae0: 6965 7233 222c 2030 0a20 2020 2020 2020  ier3", 0.       
-00011af0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00011b00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00011b10: 6e31 6d6d 2e63 6f6e 7461 6374 5f69 6e66  n1mm.contact_inf
-00011b20: 6f5b 2273 6563 7469 6f6e 225d 203d 2073  o["section"] = s
-00011b30: 656c 662e 636f 6e74 6163 745b 2253 6563  elf.contact["Sec
-00011b40: 7422 5d0a 2020 2020 2020 2020 2020 2020  t"].            
-00011b50: 2020 2020 7365 6c66 2e6e 316d 6d2e 636f      self.n1mm.co
-00011b60: 6e74 6163 745f 696e 666f 5b22 7072 6563  ntact_info["prec
-00011b70: 225d 203d 2073 656c 662e 636f 6e74 6163  "] = self.contac
-00011b80: 745b 2250 7265 6322 5d0a 2020 2020 2020  t["Prec"].      
-00011b90: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00011ba0: 316d 6d2e 636f 6e74 6163 745f 696e 666f  1mm.contact_info
-00011bb0: 5b22 636b 225d 203d 2073 656c 662e 636f  ["ck"] = self.co
-00011bc0: 6e74 6163 745b 2243 4b22 5d0a 2020 2020  ntact["CK"].    
-00011bd0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00011be0: 2e6e 316d 6d2e 636f 6e74 6163 745f 696e  .n1mm.contact_in
-00011bf0: 666f 5b22 7a6e 225d 203d 2073 656c 662e  fo["zn"] = self.
-00011c00: 636f 6e74 6163 745b 225a 4e22 5d0a 2020  contact["ZN"].  
-00011c10: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00011c20: 6c66 2e6e 316d 6d2e 636f 6e74 6163 745f  lf.n1mm.contact_
-00011c30: 696e 666f 5b22 706f 7765 7222 5d20 3d20  info["power"] = 
-00011c40: 7365 6c66 2e63 6f6e 7461 6374 5b22 506f  self.contact["Po
-00011c50: 7765 7222 5d0a 2020 2020 2020 2020 2020  wer"].          
-00011c60: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
-00011c70: 636f 6e74 6163 745f 696e 666f 5b22 6261  contact_info["ba
-00011c80: 6e64 225d 203d 2073 656c 662e 636f 6e74  nd"] = self.cont
-00011c90: 6163 745b 2242 616e 6422 5d0a 2020 2020  act["Band"].    
-00011ca0: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-00011cb0: 6572 2e64 6562 7567 2822 2573 222c 2066  er.debug("%s", f
-00011cc0: 227b 7365 6c66 2e6e 316d 6d2e 636f 6e74  "{self.n1mm.cont
-00011cd0: 6163 745f 696e 666f 7d22 290a 2020 2020  act_info}").    
-00011ce0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00011cf0: 2e6e 316d 6d2e 7365 6e64 5f63 6f6e 7461  .n1mm.send_conta
-00011d00: 6374 5f69 6e66 6f28 290a 0a20 2020 2020  ct_info()..     
-00011d10: 2020 2073 656c 662e 6461 7461 6261 7365     self.database
-00011d20: 2e6c 6f67 5f63 6f6e 7461 6374 2873 656c  .log_contact(sel
-00011d30: 662e 636f 6e74 6163 7429 0a20 2020 2020  f.contact).     
-00011d40: 2020 2073 656c 662e 776f 726b 6564 5f6c     self.worked_l
-00011d50: 6973 7420 3d20 7365 6c66 2e64 6174 6162  ist = self.datab
-00011d60: 6173 652e 6765 745f 6361 6c6c 735f 616e  ase.get_calls_an
-00011d70: 645f 6261 6e64 7328 290a 2020 2020 2020  d_bands().      
-00011d80: 2020 7365 6c66 2e73 656e 645f 776f 726b    self.send_work
-00011d90: 6564 5f6c 6973 7428 290a 2020 2020 2020  ed_list().      
-00011da0: 2020 7365 6c66 2e63 6c65 6172 696e 7075    self.clearinpu
-00011db0: 7473 2829 0a0a 2020 2020 2020 2020 636d  ts()..        cm
-00011dc0: 6420 3d20 7b7d 0a20 2020 2020 2020 2063  d = {}.        c
-00011dd0: 6d64 5b22 636d 6422 5d20 3d20 2255 5044  md["cmd"] = "UPD
-00011de0: 4154 454c 4f47 220a 2020 2020 2020 2020  ATELOG".        
-00011df0: 636d 645b 2273 7461 7469 6f6e 225d 203d  cmd["station"] =
-00011e00: 2070 6c61 7466 6f72 6d2e 6e6f 6465 2829   platform.node()
-00011e10: 0a20 2020 2020 2020 2073 656c 662e 6d75  .        self.mu
-00011e20: 6c74 6963 6173 745f 696e 7465 7266 6163  lticast_interfac
-00011e30: 652e 7365 6e64 5f61 735f 6a73 6f6e 2863  e.send_as_json(c
-00011e40: 6d64 290a 0a20 2020 2064 6566 206e 6577  md)..    def new
-00011e50: 5f63 6f6e 7465 7374 5f64 6961 6c6f 6728  _contest_dialog(
-00011e60: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
-00011e70: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00011e80: 2020 2053 686f 7720 6e65 7720 636f 6e74     Show new cont
-00011e90: 6573 7420 6469 616c 6f67 2e0a 0a20 2020  est dialog...   
-00011ea0: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-00011eb0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00011ec0: 2d2d 0a20 2020 2020 2020 204e 6f6e 650a  --.        None.
-00011ed0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00011ee0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00011ef0: 0a20 2020 2020 2020 204e 6f6e 650a 2020  .        None.  
-00011f00: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
-00011f10: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-00011f20: 224e 6577 2063 6f6e 7465 7374 2044 6961  "New contest Dia
-00011f30: 6c6f 6722 290a 0a20 2020 2020 2020 2073  log")..        s
-00011f40: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-00011f50: 6f67 203d 204e 6577 436f 6e74 6573 7428  og = NewContest(
-00011f60: 6673 7574 696c 732e 4150 505f 4441 5441  fsutils.APP_DATA
-00011f70: 5f50 4154 4829 0a20 2020 2020 2020 2069  _PATH).        i
-00011f80: 6620 7365 6c66 2e63 7572 7265 6e74 5f70  f self.current_p
-00011f90: 616c 6574 7465 3a0a 2020 2020 2020 2020  alette:.        
-00011fa0: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
-00011fb0: 5f64 6961 6c6f 672e 7365 7450 616c 6574  _dialog.setPalet
-00011fc0: 7465 2873 656c 662e 6375 7272 656e 745f  te(self.current_
-00011fd0: 7061 6c65 7474 6529 0a20 2020 2020 2020  palette).       
-00011fe0: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
-00011ff0: 745f 6469 616c 6f67 2e65 7863 6861 6e67  t_dialog.exchang
-00012000: 652e 7365 7450 616c 6574 7465 2873 656c  e.setPalette(sel
-00012010: 662e 6375 7272 656e 745f 7061 6c65 7474  f.current_palett
-00012020: 6529 0a20 2020 2020 2020 2020 2020 2073  e).            s
-00012030: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-00012040: 6f67 2e6f 7065 7261 746f 7273 2e73 6574  og.operators.set
-00012050: 5061 6c65 7474 6528 7365 6c66 2e63 7572  Palette(self.cur
-00012060: 7265 6e74 5f70 616c 6574 7465 290a 0a20  rent_palette).. 
-00012070: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
-00012080: 6573 745f 6469 616c 6f67 2e61 6363 6570  est_dialog.accep
-00012090: 7465 642e 636f 6e6e 6563 7428 7365 6c66  ted.connect(self
-000120a0: 2e73 6176 655f 636f 6e74 6573 7429 0a20  .save_contest). 
-000120b0: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
-000120c0: 6573 745f 6469 616c 6f67 2e64 6174 6554  est_dialog.dateT
-000120d0: 696d 6545 6469 742e 7365 7444 6174 6528  imeEdit.setDate(
-000120e0: 5174 436f 7265 2e51 4461 7465 2e63 7572  QtCore.QDate.cur
-000120f0: 7265 6e74 4461 7465 2829 290a 2020 2020  rentDate()).    
-00012100: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
-00012110: 5f64 6961 6c6f 672e 6461 7465 5469 6d65  _dialog.dateTime
-00012120: 4564 6974 2e73 6574 4361 6c65 6e64 6172  Edit.setCalendar
-00012130: 506f 7075 7028 5472 7565 290a 2020 2020  Popup(True).    
-00012140: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
-00012150: 5f64 6961 6c6f 672e 6461 7465 5469 6d65  _dialog.dateTime
-00012160: 4564 6974 2e73 6574 5469 6d65 2851 7443  Edit.setTime(QtC
-00012170: 6f72 652e 5154 696d 6528 302c 2030 2929  ore.QTime(0, 0))
-00012180: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-00012190: 6e74 6573 745f 6469 616c 6f67 2e70 6f77  ntest_dialog.pow
-000121a0: 6572 2e73 6574 4375 7272 656e 7454 6578  er.setCurrentTex
-000121b0: 7428 224c 4f57 2229 0a20 2020 2020 2020  t("LOW").       
-000121c0: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
-000121d0: 616c 6f67 2e73 7461 7469 6f6e 2e73 6574  alog.station.set
-000121e0: 4375 7272 656e 7454 6578 7428 2246 4958  CurrentText("FIX
-000121f0: 4544 2229 0a20 2020 2020 2020 2073 656c  ED").        sel
-00012200: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
-00012210: 2e6f 7065 6e28 290a 0a20 2020 2064 6566  .open()..    def
-00012220: 2073 6176 655f 636f 6e74 6573 7428 7365   save_contest(se
-00012230: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
-00012240: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00012250: 2053 6176 6520 436f 6e74 6573 7420 746f   Save Contest to
-00012260: 2064 6174 6162 6173 652e 0a0a 2020 2020   database...    
-00012270: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-00012280: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-00012290: 2d0a 2020 2020 2020 2020 4e6f 6e65 0a0a  -.        None..
-000122a0: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
-000122b0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
-000122c0: 2020 2020 2020 2020 4e6f 6e65 0a20 2020          None.   
-000122d0: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
-000122e0: 2020 6e65 7874 5f6e 756d 6265 7220 3d20    next_number = 
-000122f0: 7365 6c66 2e64 6174 6162 6173 652e 6765  self.database.ge
-00012300: 745f 6e65 7874 5f63 6f6e 7465 7374 5f6e  t_next_contest_n
-00012310: 7228 290a 2020 2020 2020 2020 636f 6e74  r().        cont
-00012320: 6573 7420 3d20 7b7d 0a20 2020 2020 2020  est = {}.       
-00012330: 2063 6f6e 7465 7374 5b22 436f 6e74 6573   contest["Contes
-00012340: 744e 616d 6522 5d20 3d20 280a 2020 2020  tName"] = (.    
-00012350: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-00012360: 7465 7374 5f64 6961 6c6f 672e 636f 6e74  test_dialog.cont
-00012370: 6573 742e 6375 7272 656e 7454 6578 7428  est.currentText(
-00012380: 292e 6c6f 7765 7228 292e 7265 706c 6163  ).lower().replac
-00012390: 6528 2220 222c 2022 5f22 290a 2020 2020  e(" ", "_").    
-000123a0: 2020 2020 290a 2020 2020 2020 2020 636f      ).        co
-000123b0: 6e74 6573 745b 2253 7461 7274 4461 7465  ntest["StartDate
-000123c0: 225d 203d 2073 656c 662e 636f 6e74 6573  "] = self.contes
-000123d0: 745f 6469 616c 6f67 2e64 6174 6554 696d  t_dialog.dateTim
-000123e0: 6545 6469 742e 6461 7465 5469 6d65 2829  eEdit.dateTime()
-000123f0: 2e74 6f53 7472 696e 6728 0a20 2020 2020  .toString(.     
-00012400: 2020 2020 2020 2022 7979 7979 2d4d 4d2d         "yyyy-MM-
-00012410: 6464 2068 683a 6d6d 3a73 7322 0a20 2020  dd hh:mm:ss".   
-00012420: 2020 2020 2029 0a20 2020 2020 2020 2063       ).        c
-00012430: 6f6e 7465 7374 5b22 4f70 6572 6174 6f72  ontest["Operator
-00012440: 4361 7465 676f 7279 225d 203d 2073 656c  Category"] = sel
-00012450: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
-00012460: 2e6f 7065 7261 746f 725f 636c 6173 732e  .operator_class.
-00012470: 6375 7272 656e 7454 6578 7428 290a 2020  currentText().  
-00012480: 2020 2020 2020 636f 6e74 6573 745b 2242        contest["B
-00012490: 616e 6443 6174 6567 6f72 7922 5d20 3d20  andCategory"] = 
-000124a0: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
-000124b0: 6c6f 672e 6261 6e64 2e63 7572 7265 6e74  log.band.current
-000124c0: 5465 7874 2829 0a20 2020 2020 2020 2063  Text().        c
-000124d0: 6f6e 7465 7374 5b22 506f 7765 7243 6174  ontest["PowerCat
-000124e0: 6567 6f72 7922 5d20 3d20 7365 6c66 2e63  egory"] = self.c
-000124f0: 6f6e 7465 7374 5f64 6961 6c6f 672e 706f  ontest_dialog.po
-00012500: 7765 722e 6375 7272 656e 7454 6578 7428  wer.currentText(
-00012510: 290a 2020 2020 2020 2020 636f 6e74 6573  ).        contes
-00012520: 745b 224d 6f64 6543 6174 6567 6f72 7922  t["ModeCategory"
-00012530: 5d20 3d20 7365 6c66 2e63 6f6e 7465 7374  ] = self.contest
-00012540: 5f64 6961 6c6f 672e 6d6f 6465 2e63 7572  _dialog.mode.cur
-00012550: 7265 6e74 5465 7874 2829 0a20 2020 2020  rentText().     
-00012560: 2020 2063 6f6e 7465 7374 5b22 4f76 6572     contest["Over
-00012570: 6c61 7943 6174 6567 6f72 7922 5d20 3d20  layCategory"] = 
-00012580: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
-00012590: 6c6f 672e 6f76 6572 6c61 792e 6375 7272  log.overlay.curr
-000125a0: 656e 7454 6578 7428 290a 2020 2020 2020  entText().      
-000125b0: 2020 2320 636f 6e74 6573 745b 2743 6c61    # contest['Cla
-000125c0: 696d 6564 5363 6f72 6527 5d20 3d20 7365  imedScore'] = se
-000125d0: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-000125e0: 672e 0a20 2020 2020 2020 2063 6f6e 7465  g..        conte
-000125f0: 7374 5b22 4f70 6572 6174 6f72 7322 5d20  st["Operators"] 
-00012600: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f64  = self.contest_d
-00012610: 6961 6c6f 672e 6f70 6572 6174 6f72 732e  ialog.operators.
-00012620: 7465 7874 2829 0a20 2020 2020 2020 2063  text().        c
-00012630: 6f6e 7465 7374 5b22 536f 6170 626f 7822  ontest["Soapbox"
-00012640: 5d20 3d20 7365 6c66 2e63 6f6e 7465 7374  ] = self.contest
-00012650: 5f64 6961 6c6f 672e 736f 6170 626f 782e  _dialog.soapbox.
-00012660: 746f 506c 6169 6e54 6578 7428 290a 2020  toPlainText().  
-00012670: 2020 2020 2020 636f 6e74 6573 745b 2253        contest["S
-00012680: 656e 7445 7863 6861 6e67 6522 5d20 3d20  entExchange"] = 
-00012690: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
-000126a0: 6c6f 672e 6578 6368 616e 6765 2e74 6578  log.exchange.tex
-000126b0: 7428 290a 2020 2020 2020 2020 636f 6e74  t().        cont
-000126c0: 6573 745b 2243 6f6e 7465 7374 4e52 225d  est["ContestNR"]
-000126d0: 203d 206e 6578 745f 6e75 6d62 6572 2e67   = next_number.g
-000126e0: 6574 2822 636f 756e 7422 2c20 3129 0a20  et("count", 1). 
-000126f0: 2020 2020 2020 2073 656c 662e 7072 6566         self.pref
-00012700: 5b22 636f 6e74 6573 7422 5d20 3d20 6e65  ["contest"] = ne
-00012710: 7874 5f6e 756d 6265 722e 6765 7428 2263  xt_number.get("c
-00012720: 6f75 6e74 222c 2031 290a 2020 2020 2020  ount", 1).      
-00012730: 2020 2320 636f 6e74 6573 745b 2753 7562    # contest['Sub
-00012740: 5479 7065 275d 203d 2073 656c 662e 636f  Type'] = self.co
-00012750: 6e74 6573 745f 6469 616c 6f67 2e0a 2020  ntest_dialog..  
-00012760: 2020 2020 2020 636f 6e74 6573 745b 2253        contest["S
-00012770: 7461 7469 6f6e 4361 7465 676f 7279 225d  tationCategory"]
-00012780: 203d 2073 656c 662e 636f 6e74 6573 745f   = self.contest_
-00012790: 6469 616c 6f67 2e73 7461 7469 6f6e 2e63  dialog.station.c
-000127a0: 7572 7265 6e74 5465 7874 2829 0a20 2020  urrentText().   
-000127b0: 2020 2020 2063 6f6e 7465 7374 5b22 4173       contest["As
-000127c0: 7369 7374 6564 4361 7465 676f 7279 225d  sistedCategory"]
-000127d0: 203d 2073 656c 662e 636f 6e74 6573 745f   = self.contest_
-000127e0: 6469 616c 6f67 2e61 7373 6973 7465 642e  dialog.assisted.
-000127f0: 6375 7272 656e 7454 6578 7428 290a 2020  currentText().  
-00012800: 2020 2020 2020 636f 6e74 6573 745b 2254        contest["T
-00012810: 7261 6e73 6d69 7474 6572 4361 7465 676f  ransmitterCatego
-00012820: 7279 225d 203d 2073 656c 662e 636f 6e74  ry"] = self.cont
-00012830: 6573 745f 6469 616c 6f67 2e74 7261 6e73  est_dialog.trans
-00012840: 6d69 7474 6572 2e63 7572 7265 6e74 5465  mitter.currentTe
-00012850: 7874 2829 0a20 2020 2020 2020 2023 2063  xt().        # c
-00012860: 6f6e 7465 7374 5b27 5469 6d65 4361 7465  ontest['TimeCate
-00012870: 676f 7279 275d 203d 2073 656c 662e 636f  gory'] = self.co
-00012880: 6e74 6573 745f 6469 616c 6f67 2e0a 2020  ntest_dialog..  
-00012890: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-000128a0: 7567 2822 2573 222c 2066 227b 636f 6e74  ug("%s", f"{cont
-000128b0: 6573 747d 2229 0a20 2020 2020 2020 2073  est}").        s
-000128c0: 656c 662e 6461 7461 6261 7365 2e61 6464  elf.database.add
-000128d0: 5f63 6f6e 7465 7374 2863 6f6e 7465 7374  _contest(contest
-000128e0: 290a 2020 2020 2020 2020 7365 6c66 2e77  ).        self.w
-000128f0: 7269 7465 5f70 7265 6665 7265 6e63 6528  rite_preference(
-00012900: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
-00012910: 6f61 645f 636f 6e74 6573 7428 290a 0a20  oad_contest().. 
-00012920: 2020 2064 6566 2065 6469 745f 7374 6174     def edit_stat
-00012930: 696f 6e5f 7365 7474 696e 6773 2873 656c  ion_settings(sel
-00012940: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
-00012950: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00012960: 5368 6f77 2073 6574 7469 6e67 7320 6469  Show settings di
-00012970: 616c 6f67 2066 6f72 2073 7461 7469 6f6e  alog for station
-00012980: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-00012990: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
-000129a0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-000129b0: 204e 6f6e 650a 0a20 2020 2020 2020 2052   None..        R
-000129c0: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
-000129d0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 204e  ------.        N
-000129e0: 6f6e 650a 2020 2020 2020 2020 2222 220a  one.        """.
-000129f0: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
-00012a00: 6465 6275 6728 2253 7461 7469 6f6e 2053  debug("Station S
-00012a10: 6574 7469 6e67 7320 7365 6c65 6374 6564  ettings selected
-00012a20: 2229 0a0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00012a30: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
-00012a40: 203d 2045 6469 7453 7461 7469 6f6e 2866   = EditStation(f
-00012a50: 7375 7469 6c73 2e41 5050 5f44 4154 415f  sutils.APP_DATA_
-00012a60: 5041 5448 290a 2020 2020 2020 2020 6966  PATH).        if
-00012a70: 2073 656c 662e 6375 7272 656e 745f 7061   self.current_pa
-00012a80: 6c65 7474 653a 0a20 2020 2020 2020 2020  lette:.         
-00012a90: 2020 2073 656c 662e 7365 7474 696e 6773     self.settings
-00012aa0: 5f64 6961 6c6f 672e 7365 7450 616c 6574  _dialog.setPalet
-00012ab0: 7465 2873 656c 662e 6375 7272 656e 745f  te(self.current_
-00012ac0: 7061 6c65 7474 6529 0a0a 2020 2020 2020  palette)..      
-00012ad0: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
-00012ae0: 6469 616c 6f67 2e61 6363 6570 7465 642e  dialog.accepted.
-00012af0: 636f 6e6e 6563 7428 7365 6c66 2e73 6176  connect(self.sav
-00012b00: 655f 7365 7474 696e 6773 290a 2020 2020  e_settings).    
-00012b10: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
-00012b20: 735f 6469 616c 6f67 2e43 616c 6c2e 7365  s_dialog.Call.se
-00012b30: 7454 6578 7428 7365 6c66 2e73 7461 7469  tText(self.stati
-00012b40: 6f6e 2e67 6574 2822 4361 6c6c 222c 2022  on.get("Call", "
-00012b50: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
-00012b60: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
-00012b70: 2e4e 616d 652e 7365 7454 6578 7428 7365  .Name.setText(se
-00012b80: 6c66 2e73 7461 7469 6f6e 2e67 6574 2822  lf.station.get("
-00012b90: 4e61 6d65 222c 2022 2229 290a 2020 2020  Name", "")).    
-00012ba0: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
-00012bb0: 735f 6469 616c 6f67 2e41 6464 7265 7373  s_dialog.Address
-00012bc0: 312e 7365 7454 6578 7428 7365 6c66 2e73  1.setText(self.s
-00012bd0: 7461 7469 6f6e 2e67 6574 2822 5374 7265  tation.get("Stre
-00012be0: 6574 3122 2c20 2222 2929 0a20 2020 2020  et1", "")).     
-00012bf0: 2020 2073 656c 662e 7365 7474 696e 6773     self.settings
-00012c00: 5f64 6961 6c6f 672e 4164 6472 6573 7332  _dialog.Address2
-00012c10: 2e73 6574 5465 7874 2873 656c 662e 7374  .setText(self.st
-00012c20: 6174 696f 6e2e 6765 7428 2253 7472 6565  ation.get("Stree
-00012c30: 7432 222c 2022 2229 290a 2020 2020 2020  t2", "")).      
-00012c40: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
-00012c50: 6469 616c 6f67 2e43 6974 792e 7365 7454  dialog.City.setT
-00012c60: 6578 7428 7365 6c66 2e73 7461 7469 6f6e  ext(self.station
-00012c70: 2e67 6574 2822 4369 7479 222c 2022 2229  .get("City", "")
-00012c80: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-00012c90: 6574 7469 6e67 735f 6469 616c 6f67 2e53  ettings_dialog.S
-00012ca0: 7461 7465 2e73 6574 5465 7874 2873 656c  tate.setText(sel
-00012cb0: 662e 7374 6174 696f 6e2e 6765 7428 2253  f.station.get("S
-00012cc0: 7461 7465 222c 2022 2229 290a 2020 2020  tate", "")).    
-00012cd0: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
-00012ce0: 735f 6469 616c 6f67 2e5a 6970 2e73 6574  s_dialog.Zip.set
-00012cf0: 5465 7874 2873 656c 662e 7374 6174 696f  Text(self.statio
-00012d00: 6e2e 6765 7428 225a 6970 222c 2022 2229  n.get("Zip", "")
-00012d10: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-00012d20: 6574 7469 6e67 735f 6469 616c 6f67 2e43  ettings_dialog.C
-00012d30: 6f75 6e74 7279 2e73 6574 5465 7874 2873  ountry.setText(s
-00012d40: 656c 662e 7374 6174 696f 6e2e 6765 7428  elf.station.get(
-00012d50: 2243 6f75 6e74 7279 222c 2022 2229 290a  "Country", "")).
-00012d60: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-00012d70: 7469 6e67 735f 6469 616c 6f67 2e47 7269  tings_dialog.Gri
-00012d80: 6453 7175 6172 652e 7365 7454 6578 7428  dSquare.setText(
-00012d90: 7365 6c66 2e73 7461 7469 6f6e 2e67 6574  self.station.get
-00012da0: 2822 4772 6964 5371 7561 7265 222c 2022  ("GridSquare", "
-00012db0: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
-00012dc0: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
-00012dd0: 2e43 515a 6f6e 652e 7365 7454 6578 7428  .CQZone.setText(
-00012de0: 7374 7228 7365 6c66 2e73 7461 7469 6f6e  str(self.station
-00012df0: 2e67 6574 2822 4351 5a6f 6e65 222c 2022  .get("CQZone", "
-00012e00: 2229 2929 0a20 2020 2020 2020 2073 656c  "))).        sel
-00012e10: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
-00012e20: 672e 4954 555a 6f6e 652e 7365 7454 6578  g.ITUZone.setTex
-00012e30: 7428 7374 7228 7365 6c66 2e73 7461 7469  t(str(self.stati
-00012e40: 6f6e 2e67 6574 2822 4941 5255 5a6f 6e65  on.get("IARUZone
-00012e50: 222c 2022 2229 2929 0a20 2020 2020 2020  ", ""))).       
-00012e60: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
-00012e70: 6961 6c6f 672e 4c69 6365 6e73 652e 7365  ialog.License.se
-00012e80: 7454 6578 7428 7365 6c66 2e73 7461 7469  tText(self.stati
-00012e90: 6f6e 2e67 6574 2822 4c69 6365 6e73 6543  on.get("LicenseC
-00012ea0: 6c61 7373 222c 2022 2229 290a 2020 2020  lass", "")).    
-00012eb0: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
-00012ec0: 735f 6469 616c 6f67 2e4c 6174 6974 7564  s_dialog.Latitud
-00012ed0: 652e 7365 7454 6578 7428 7374 7228 7365  e.setText(str(se
-00012ee0: 6c66 2e73 7461 7469 6f6e 2e67 6574 2822  lf.station.get("
-00012ef0: 4c61 7469 7475 6465 222c 2022 2229 2929  Latitude", "")))
-00012f00: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-00012f10: 7474 696e 6773 5f64 6961 6c6f 672e 4c6f  ttings_dialog.Lo
-00012f20: 6e67 6974 7564 652e 7365 7454 6578 7428  ngitude.setText(
-00012f30: 7374 7228 7365 6c66 2e73 7461 7469 6f6e  str(self.station
-00012f40: 2e67 6574 2822 4c6f 6e67 6974 7564 6522  .get("Longitude"
-00012f50: 2c20 2222 2929 290a 2020 2020 2020 2020  , ""))).        
-00012f60: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
-00012f70: 616c 6f67 2e53 7461 7469 6f6e 5458 5258  alog.StationTXRX
-00012f80: 2e73 6574 5465 7874 2873 656c 662e 7374  .setText(self.st
-00012f90: 6174 696f 6e2e 6765 7428 2273 7461 7469  ation.get("stati
-00012fa0: 6f6e 7478 7278 222c 2022 2229 290a 2020  ontxrx", "")).  
-00012fb0: 2020 2020 2020 7365 6c66 2e73 6574 7469        self.setti
-00012fc0: 6e67 735f 6469 616c 6f67 2e50 6f77 6572  ngs_dialog.Power
-00012fd0: 2e73 6574 5465 7874 2873 656c 662e 7374  .setText(self.st
-00012fe0: 6174 696f 6e2e 6765 7428 2253 506f 7765  ation.get("SPowe
-00012ff0: 222c 2022 2229 290a 2020 2020 2020 2020  ", "")).        
-00013000: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
-00013010: 616c 6f67 2e41 6e74 656e 6e61 2e73 6574  alog.Antenna.set
-00013020: 5465 7874 2873 656c 662e 7374 6174 696f  Text(self.statio
-00013030: 6e2e 6765 7428 2253 416e 7465 222c 2022  n.get("SAnte", "
-00013040: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
-00013050: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
-00013060: 2e41 6e74 4865 6967 6874 2e73 6574 5465  .AntHeight.setTe
-00013070: 7874 2873 656c 662e 7374 6174 696f 6e2e  xt(self.station.
-00013080: 6765 7428 2253 416e 7448 3122 2c20 2222  get("SAntH1", ""
-00013090: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-000130a0: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
-000130b0: 4153 4c2e 7365 7454 6578 7428 7365 6c66  ASL.setText(self
-000130c0: 2e73 7461 7469 6f6e 2e67 6574 2822 5341  .station.get("SA
-000130d0: 6e74 4832 222c 2022 2229 290a 2020 2020  ntH2", "")).    
-000130e0: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
-000130f0: 735f 6469 616c 6f67 2e41 5252 4c53 6563  s_dialog.ARRLSec
-00013100: 7469 6f6e 2e73 6574 5465 7874 2873 656c  tion.setText(sel
-00013110: 662e 7374 6174 696f 6e2e 6765 7428 2241  f.station.get("A
-00013120: 5252 4c53 6563 7469 6f6e 222c 2022 2229  RRLSection", "")
-00013130: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-00013140: 6574 7469 6e67 735f 6469 616c 6f67 2e52  ettings_dialog.R
-00013150: 6f76 6572 5154 482e 7365 7454 6578 7428  overQTH.setText(
-00013160: 7365 6c66 2e73 7461 7469 6f6e 2e67 6574  self.station.get
-00013170: 2822 526f 7665 7251 5448 222c 2022 2229  ("RoverQTH", "")
-00013180: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-00013190: 6574 7469 6e67 735f 6469 616c 6f67 2e43  ettings_dialog.C
-000131a0: 6c75 622e 7365 7454 6578 7428 7365 6c66  lub.setText(self
-000131b0: 2e73 7461 7469 6f6e 2e67 6574 2822 436c  .station.get("Cl
-000131c0: 7562 222c 2022 2229 290a 2020 2020 2020  ub", "")).      
-000131d0: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
-000131e0: 6469 616c 6f67 2e45 6d61 696c 2e73 6574  dialog.Email.set
-000131f0: 5465 7874 2873 656c 662e 7374 6174 696f  Text(self.statio
-00013200: 6e2e 6765 7428 2245 6d61 696c 222c 2022  n.get("Email", "
-00013210: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
-00013220: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
-00013230: 2e6f 7065 6e28 290a 0a20 2020 2064 6566  .open()..    def
-00013240: 2073 6176 655f 7365 7474 696e 6773 2873   save_settings(s
-00013250: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
-00013260: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00013270: 2020 5361 7665 2073 6574 7469 6e67 7320    Save settings 
-00013280: 746f 2064 6174 6162 6173 652e 0a0a 2020  to database...  
-00013290: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+00011270: 7461 6374 5f70 6163 6b65 7473 3a0a 2020  tact_packets:.  
+00011280: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00011290: 6c66 2e6e 316d 6d2e 636f 6e74 6163 745f  lf.n1mm.contact_
+000112a0: 696e 666f 5b22 7469 6d65 7374 616d 7022  info["timestamp"
+000112b0: 5d20 3d20 7365 6c66 2e63 6f6e 7461 6374  ] = self.contact
+000112c0: 5b22 5453 225d 0a20 2020 2020 2020 2020  ["TS"].         
+000112d0: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
+000112e0: 2e63 6f6e 7461 6374 5f69 6e66 6f5b 226f  .contact_info["o
+000112f0: 6c64 6361 6c6c 225d 203d 2073 656c 662e  ldcall"] = self.
+00011300: 6e31 6d6d 2e63 6f6e 7461 6374 5f69 6e66  n1mm.contact_inf
+00011310: 6f5b 2263 616c 6c22 5d20 3d20 280a 2020  o["call"] = (.  
+00011320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011330: 2020 7365 6c66 2e63 6f6e 7461 6374 5b22    self.contact["
+00011340: 4361 6c6c 225d 0a20 2020 2020 2020 2020  Call"].         
+00011350: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00011360: 2020 2020 2020 2020 2073 656c 662e 6e31           self.n1
+00011370: 6d6d 2e63 6f6e 7461 6374 5f69 6e66 6f5b  mm.contact_info[
+00011380: 2274 7866 7265 7122 5d20 3d20 7365 6c66  "txfreq"] = self
+00011390: 2e6e 316d 6d2e 636f 6e74 6163 745f 696e  .n1mm.contact_in
+000113a0: 666f 5b22 7278 6672 6571 225d 203d 2028  fo["rxfreq"] = (
+000113b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000113c0: 2020 2020 2073 656c 662e 6e31 6d6d 2e72       self.n1mm.r
+000113d0: 6164 696f 5f69 6e66 6f5b 2246 7265 7122  adio_info["Freq"
+000113e0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+000113f0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00011400: 2020 2020 7365 6c66 2e6e 316d 6d2e 636f      self.n1mm.co
+00011410: 6e74 6163 745f 696e 666f 5b22 6d6f 6465  ntact_info["mode
+00011420: 225d 203d 2073 656c 662e 636f 6e74 6163  "] = self.contac
+00011430: 745b 224d 6f64 6522 5d0a 2020 2020 2020  t["Mode"].      
+00011440: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00011450: 316d 6d2e 636f 6e74 6163 745f 696e 666f  1mm.contact_info
+00011460: 5b22 636f 6e74 6573 746e 616d 6522 5d20  ["contestname"] 
+00011470: 3d20 7365 6c66 2e63 6f6e 7461 6374 5b0a  = self.contact[.
+00011480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011490: 2020 2020 2243 6f6e 7465 7374 4e61 6d65      "ContestName
+000114a0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+000114b0: 2020 5d2e 7265 706c 6163 6528 222d 222c    ].replace("-",
+000114c0: 2022 2229 0a20 2020 2020 2020 2020 2020   "").           
+000114d0: 2020 2020 2073 656c 662e 6e31 6d6d 2e63       self.n1mm.c
+000114e0: 6f6e 7461 6374 5f69 6e66 6f5b 2263 6f6e  ontact_info["con
+000114f0: 7465 7374 6e72 225d 203d 2073 656c 662e  testnr"] = self.
+00011500: 636f 6e74 6163 745b 2243 6f6e 7465 7374  contact["Contest
+00011510: 4e52 225d 0a20 2020 2020 2020 2020 2020  NR"].           
+00011520: 2020 2020 2073 656c 662e 6e31 6d6d 2e63       self.n1mm.c
+00011530: 6f6e 7461 6374 5f69 6e66 6f5b 2273 7461  ontact_info["sta
+00011540: 7469 6f6e 7072 6566 6978 225d 203d 2073  tionprefix"] = s
+00011550: 656c 662e 636f 6e74 6163 745b 2253 7461  elf.contact["Sta
+00011560: 7469 6f6e 5072 6566 6978 225d 0a20 2020  tionPrefix"].   
+00011570: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00011580: 662e 6e31 6d6d 2e63 6f6e 7461 6374 5f69  f.n1mm.contact_i
+00011590: 6e66 6f5b 2277 7078 7072 6566 6978 225d  nfo["wpxprefix"]
+000115a0: 203d 2073 656c 662e 636f 6e74 6163 745b   = self.contact[
+000115b0: 2257 5058 5072 6566 6978 225d 0a20 2020  "WPXPrefix"].   
+000115c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000115d0: 662e 6e31 6d6d 2e63 6f6e 7461 6374 5f69  f.n1mm.contact_i
+000115e0: 6e66 6f5b 2249 7352 756e 5153 4f22 5d20  nfo["IsRunQSO"] 
+000115f0: 3d20 7365 6c66 2e63 6f6e 7461 6374 5b22  = self.contact["
+00011600: 4973 5275 6e51 534f 225d 0a20 2020 2020  IsRunQSO"].     
+00011610: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00011620: 6e31 6d6d 2e63 6f6e 7461 6374 5f69 6e66  n1mm.contact_inf
+00011630: 6f5b 226f 7065 7261 746f 7222 5d20 3d20  o["operator"] = 
+00011640: 7365 6c66 2e63 6f6e 7461 6374 5b22 4f70  self.contact["Op
+00011650: 6572 6174 6f72 225d 0a20 2020 2020 2020  erator"].       
+00011660: 2020 2020 2020 2020 2073 656c 662e 6e31           self.n1
+00011670: 6d6d 2e63 6f6e 7461 6374 5f69 6e66 6f5b  mm.contact_info[
+00011680: 226d 7963 616c 6c22 5d20 3d20 7365 6c66  "mycall"] = self
+00011690: 2e63 6f6e 7461 6374 5b22 4f70 6572 6174  .contact["Operat
+000116a0: 6f72 225d 0a20 2020 2020 2020 2020 2020  or"].           
+000116b0: 2020 2020 2073 656c 662e 6e31 6d6d 2e63       self.n1mm.c
+000116c0: 6f6e 7461 6374 5f69 6e66 6f5b 2253 7461  ontact_info["Sta
+000116d0: 7469 6f6e 4e61 6d65 225d 203d 2073 656c  tionName"] = sel
+000116e0: 662e 6e31 6d6d 2e63 6f6e 7461 6374 5f69  f.n1mm.contact_i
+000116f0: 6e66 6f5b 0a20 2020 2020 2020 2020 2020  nfo[.           
+00011700: 2020 2020 2020 2020 2022 4e65 7442 696f           "NetBio
+00011710: 734e 616d 6522 0a20 2020 2020 2020 2020  sName".         
+00011720: 2020 2020 2020 205d 203d 2073 656c 662e         ] = self.
+00011730: 636f 6e74 6163 745b 224e 6574 4269 6f73  contact["NetBios
+00011740: 4e61 6d65 225d 0a20 2020 2020 2020 2020  Name"].         
+00011750: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
+00011760: 2e63 6f6e 7461 6374 5f69 6e66 6f5b 2249  .contact_info["I
+00011770: 734f 7269 6769 6e61 6c22 5d20 3d20 7365  sOriginal"] = se
+00011780: 6c66 2e63 6f6e 7461 6374 5b22 4973 4f72  lf.contact["IsOr
+00011790: 6967 696e 616c 225d 0a20 2020 2020 2020  iginal"].       
+000117a0: 2020 2020 2020 2020 2073 656c 662e 6e31           self.n1
+000117b0: 6d6d 2e63 6f6e 7461 6374 5f69 6e66 6f5b  mm.contact_info[
+000117c0: 2249 4422 5d20 3d20 7365 6c66 2e63 6f6e  "ID"] = self.con
+000117d0: 7461 6374 5b22 4944 225d 0a20 2020 2020  tact["ID"].     
+000117e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000117f0: 6e31 6d6d 2e63 6f6e 7461 6374 5f69 6e66  n1mm.contact_inf
+00011800: 6f5b 2270 6f69 6e74 7322 5d20 3d20 7365  o["points"] = se
+00011810: 6c66 2e63 6f6e 7461 6374 5b22 506f 696e  lf.contact["Poin
+00011820: 7473 225d 0a20 2020 2020 2020 2020 2020  ts"].           
+00011830: 2020 2020 2073 656c 662e 6e31 6d6d 2e63       self.n1mm.c
+00011840: 6f6e 7461 6374 5f69 6e66 6f5b 2273 6e74  ontact_info["snt
+00011850: 225d 203d 2073 656c 662e 636f 6e74 6163  "] = self.contac
+00011860: 745b 2253 4e54 225d 0a20 2020 2020 2020  t["SNT"].       
+00011870: 2020 2020 2020 2020 2073 656c 662e 6e31           self.n1
+00011880: 6d6d 2e63 6f6e 7461 6374 5f69 6e66 6f5b  mm.contact_info[
+00011890: 2272 6376 225d 203d 2073 656c 662e 636f  "rcv"] = self.co
+000118a0: 6e74 6163 745b 2252 4356 225d 0a20 2020  ntact["RCV"].   
+000118b0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000118c0: 662e 6e31 6d6d 2e63 6f6e 7461 6374 5f69  f.n1mm.contact_i
+000118d0: 6e66 6f5b 2273 6e74 6e72 225d 203d 2073  nfo["sntnr"] = s
+000118e0: 656c 662e 636f 6e74 6163 745b 2253 656e  elf.contact["Sen
+000118f0: 744e 7222 5d0a 2020 2020 2020 2020 2020  tNr"].          
+00011900: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
+00011910: 636f 6e74 6163 745f 696e 666f 5b22 7263  contact_info["rc
+00011920: 766e 7222 5d20 3d20 7365 6c66 2e63 6f6e  vnr"] = self.con
+00011930: 7461 6374 5b22 4e52 225d 0a20 2020 2020  tact["NR"].     
+00011940: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00011950: 6e31 6d6d 2e63 6f6e 7461 6374 5f69 6e66  n1mm.contact_inf
+00011960: 6f5b 2269 736d 756c 7469 706c 6965 7231  o["ismultiplier1
+00011970: 225d 203d 2073 656c 662e 636f 6e74 6163  "] = self.contac
+00011980: 742e 6765 7428 0a20 2020 2020 2020 2020  t.get(.         
+00011990: 2020 2020 2020 2020 2020 2022 4973 4d75             "IsMu
+000119a0: 6c74 6970 6c69 6572 3122 2c20 300a 2020  ltiplier1", 0.  
+000119b0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+000119c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000119d0: 7365 6c66 2e6e 316d 6d2e 636f 6e74 6163  self.n1mm.contac
+000119e0: 745f 696e 666f 5b22 6973 6d75 6c74 6970  t_info["ismultip
+000119f0: 6c69 6572 3222 5d20 3d20 7365 6c66 2e63  lier2"] = self.c
+00011a00: 6f6e 7461 6374 2e67 6574 280a 2020 2020  ontact.get(.    
+00011a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a20: 2249 734d 756c 7469 706c 6965 7232 222c  "IsMultiplier2",
+00011a30: 2030 0a20 2020 2020 2020 2020 2020 2020   0.             
+00011a40: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00011a50: 2020 2020 2073 656c 662e 6e31 6d6d 2e63       self.n1mm.c
+00011a60: 6f6e 7461 6374 5f69 6e66 6f5b 2269 736d  ontact_info["ism
+00011a70: 756c 7469 706c 6965 7233 225d 203d 2073  ultiplier3"] = s
+00011a80: 656c 662e 636f 6e74 6163 742e 6765 7428  elf.contact.get(
+00011a90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011aa0: 2020 2020 2022 4973 4d75 6c74 6970 6c69       "IsMultipli
+00011ab0: 6572 3322 2c20 300a 2020 2020 2020 2020  er3", 0.        
+00011ac0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00011ad0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00011ae0: 316d 6d2e 636f 6e74 6163 745f 696e 666f  1mm.contact_info
+00011af0: 5b22 7365 6374 696f 6e22 5d20 3d20 7365  ["section"] = se
+00011b00: 6c66 2e63 6f6e 7461 6374 5b22 5365 6374  lf.contact["Sect
+00011b10: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
+00011b20: 2020 2073 656c 662e 6e31 6d6d 2e63 6f6e     self.n1mm.con
+00011b30: 7461 6374 5f69 6e66 6f5b 2270 7265 6322  tact_info["prec"
+00011b40: 5d20 3d20 7365 6c66 2e63 6f6e 7461 6374  ] = self.contact
+00011b50: 5b22 5072 6563 225d 0a20 2020 2020 2020  ["Prec"].       
+00011b60: 2020 2020 2020 2020 2073 656c 662e 6e31           self.n1
+00011b70: 6d6d 2e63 6f6e 7461 6374 5f69 6e66 6f5b  mm.contact_info[
+00011b80: 2263 6b22 5d20 3d20 7365 6c66 2e63 6f6e  "ck"] = self.con
+00011b90: 7461 6374 5b22 434b 225d 0a20 2020 2020  tact["CK"].     
+00011ba0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00011bb0: 6e31 6d6d 2e63 6f6e 7461 6374 5f69 6e66  n1mm.contact_inf
+00011bc0: 6f5b 227a 6e22 5d20 3d20 7365 6c66 2e63  o["zn"] = self.c
+00011bd0: 6f6e 7461 6374 5b22 5a4e 225d 0a20 2020  ontact["ZN"].   
+00011be0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00011bf0: 662e 6e31 6d6d 2e63 6f6e 7461 6374 5f69  f.n1mm.contact_i
+00011c00: 6e66 6f5b 2270 6f77 6572 225d 203d 2073  nfo["power"] = s
+00011c10: 656c 662e 636f 6e74 6163 745b 2250 6f77  elf.contact["Pow
+00011c20: 6572 225d 0a20 2020 2020 2020 2020 2020  er"].           
+00011c30: 2020 2020 2073 656c 662e 6e31 6d6d 2e63       self.n1mm.c
+00011c40: 6f6e 7461 6374 5f69 6e66 6f5b 2262 616e  ontact_info["ban
+00011c50: 6422 5d20 3d20 7365 6c66 2e63 6f6e 7461  d"] = self.conta
+00011c60: 6374 5b22 4261 6e64 225d 0a20 2020 2020  ct["Band"].     
+00011c70: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+00011c80: 722e 6465 6275 6728 2225 7322 2c20 6622  r.debug("%s", f"
+00011c90: 7b73 656c 662e 6e31 6d6d 2e63 6f6e 7461  {self.n1mm.conta
+00011ca0: 6374 5f69 6e66 6f7d 2229 0a20 2020 2020  ct_info}").     
+00011cb0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00011cc0: 6e31 6d6d 2e73 656e 645f 636f 6e74 6163  n1mm.send_contac
+00011cd0: 745f 696e 666f 2829 0a0a 2020 2020 2020  t_info()..      
+00011ce0: 2020 7365 6c66 2e64 6174 6162 6173 652e    self.database.
+00011cf0: 6c6f 675f 636f 6e74 6163 7428 7365 6c66  log_contact(self
+00011d00: 2e63 6f6e 7461 6374 290a 2020 2020 2020  .contact).      
+00011d10: 2020 7365 6c66 2e77 6f72 6b65 645f 6c69    self.worked_li
+00011d20: 7374 203d 2073 656c 662e 6461 7461 6261  st = self.databa
+00011d30: 7365 2e67 6574 5f63 616c 6c73 5f61 6e64  se.get_calls_and
+00011d40: 5f62 616e 6473 2829 0a20 2020 2020 2020  _bands().       
+00011d50: 2073 656c 662e 7365 6e64 5f77 6f72 6b65   self.send_worke
+00011d60: 645f 6c69 7374 2829 0a20 2020 2020 2020  d_list().       
+00011d70: 2073 656c 662e 636c 6561 7269 6e70 7574   self.clearinput
+00011d80: 7328 290a 0a20 2020 2020 2020 2063 6d64  s()..        cmd
+00011d90: 203d 207b 7d0a 2020 2020 2020 2020 636d   = {}.        cm
+00011da0: 645b 2263 6d64 225d 203d 2022 5550 4441  d["cmd"] = "UPDA
+00011db0: 5445 4c4f 4722 0a20 2020 2020 2020 2063  TELOG".        c
+00011dc0: 6d64 5b22 7374 6174 696f 6e22 5d20 3d20  md["station"] = 
+00011dd0: 706c 6174 666f 726d 2e6e 6f64 6528 290a  platform.node().
+00011de0: 2020 2020 2020 2020 7365 6c66 2e6d 756c          self.mul
+00011df0: 7469 6361 7374 5f69 6e74 6572 6661 6365  ticast_interface
+00011e00: 2e73 656e 645f 6173 5f6a 736f 6e28 636d  .send_as_json(cm
+00011e10: 6429 0a0a 2020 2020 6465 6620 6e65 775f  d)..    def new_
+00011e20: 636f 6e74 6573 745f 6469 616c 6f67 2873  contest_dialog(s
+00011e30: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
+00011e40: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00011e50: 2020 5368 6f77 206e 6577 2063 6f6e 7465    Show new conte
+00011e60: 7374 2064 6961 6c6f 672e 0a0a 2020 2020  st dialog...    
+00011e70: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+00011e80: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+00011e90: 2d0a 2020 2020 2020 2020 4e6f 6e65 0a0a  -.        None..
+00011ea0: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
+00011eb0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
+00011ec0: 2020 2020 2020 2020 4e6f 6e65 0a20 2020          None.   
+00011ed0: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+00011ee0: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
+00011ef0: 4e65 7720 636f 6e74 6573 7420 4469 616c  New contest Dial
+00011f00: 6f67 2229 0a0a 2020 2020 2020 2020 7365  og")..        se
+00011f10: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
+00011f20: 6720 3d20 4e65 7743 6f6e 7465 7374 2866  g = NewContest(f
+00011f30: 7375 7469 6c73 2e41 5050 5f44 4154 415f  sutils.APP_DATA_
+00011f40: 5041 5448 290a 2020 2020 2020 2020 6966  PATH).        if
+00011f50: 2073 656c 662e 6375 7272 656e 745f 7061   self.current_pa
+00011f60: 6c65 7474 653a 0a20 2020 2020 2020 2020  lette:.         
+00011f70: 2020 2073 656c 662e 636f 6e74 6573 745f     self.contest_
+00011f80: 6469 616c 6f67 2e73 6574 5061 6c65 7474  dialog.setPalett
+00011f90: 6528 7365 6c66 2e63 7572 7265 6e74 5f70  e(self.current_p
+00011fa0: 616c 6574 7465 290a 2020 2020 2020 2020  alette).        
+00011fb0: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
+00011fc0: 5f64 6961 6c6f 672e 6578 6368 616e 6765  _dialog.exchange
+00011fd0: 2e73 6574 5061 6c65 7474 6528 7365 6c66  .setPalette(self
+00011fe0: 2e63 7572 7265 6e74 5f70 616c 6574 7465  .current_palette
+00011ff0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00012000: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
+00012010: 672e 6f70 6572 6174 6f72 732e 7365 7450  g.operators.setP
+00012020: 616c 6574 7465 2873 656c 662e 6375 7272  alette(self.curr
+00012030: 656e 745f 7061 6c65 7474 6529 0a0a 2020  ent_palette)..  
+00012040: 2020 2020 2020 7365 6c66 2e63 6f6e 7465        self.conte
+00012050: 7374 5f64 6961 6c6f 672e 6163 6365 7074  st_dialog.accept
+00012060: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
+00012070: 7361 7665 5f63 6f6e 7465 7374 290a 2020  save_contest).  
+00012080: 2020 2020 2020 7365 6c66 2e63 6f6e 7465        self.conte
+00012090: 7374 5f64 6961 6c6f 672e 6461 7465 5469  st_dialog.dateTi
+000120a0: 6d65 4564 6974 2e73 6574 4461 7465 2851  meEdit.setDate(Q
+000120b0: 7443 6f72 652e 5144 6174 652e 6375 7272  tCore.QDate.curr
+000120c0: 656e 7444 6174 6528 2929 0a20 2020 2020  entDate()).     
+000120d0: 2020 2073 656c 662e 636f 6e74 6573 745f     self.contest_
+000120e0: 6469 616c 6f67 2e64 6174 6554 696d 6545  dialog.dateTimeE
+000120f0: 6469 742e 7365 7443 616c 656e 6461 7250  dit.setCalendarP
+00012100: 6f70 7570 2854 7275 6529 0a20 2020 2020  opup(True).     
+00012110: 2020 2073 656c 662e 636f 6e74 6573 745f     self.contest_
+00012120: 6469 616c 6f67 2e64 6174 6554 696d 6545  dialog.dateTimeE
+00012130: 6469 742e 7365 7454 696d 6528 5174 436f  dit.setTime(QtCo
+00012140: 7265 2e51 5469 6d65 2830 2c20 3029 290a  re.QTime(0, 0)).
+00012150: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+00012160: 7465 7374 5f64 6961 6c6f 672e 706f 7765  test_dialog.powe
+00012170: 722e 7365 7443 7572 7265 6e74 5465 7874  r.setCurrentText
+00012180: 2822 4c4f 5722 290a 2020 2020 2020 2020  ("LOW").        
+00012190: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
+000121a0: 6c6f 672e 7374 6174 696f 6e2e 7365 7443  log.station.setC
+000121b0: 7572 7265 6e74 5465 7874 2822 4649 5845  urrentText("FIXE
+000121c0: 4422 290a 2020 2020 2020 2020 7365 6c66  D").        self
+000121d0: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
+000121e0: 6f70 656e 2829 0a0a 2020 2020 6465 6620  open()..    def 
+000121f0: 7361 7665 5f63 6f6e 7465 7374 2873 656c  save_contest(sel
+00012200: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+00012210: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00012220: 5361 7665 2043 6f6e 7465 7374 2074 6f20  Save Contest to 
+00012230: 6461 7461 6261 7365 2e0a 0a20 2020 2020  database...     
+00012240: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+00012250: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+00012260: 0a20 2020 2020 2020 204e 6f6e 650a 0a20  .        None.. 
+00012270: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
+00012280: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
+00012290: 2020 2020 2020 204e 6f6e 650a 2020 2020         None.    
+000122a0: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
+000122b0: 206e 6578 745f 6e75 6d62 6572 203d 2073   next_number = s
+000122c0: 656c 662e 6461 7461 6261 7365 2e67 6574  elf.database.get
+000122d0: 5f6e 6578 745f 636f 6e74 6573 745f 6e72  _next_contest_nr
+000122e0: 2829 0a20 2020 2020 2020 2063 6f6e 7465  ().        conte
+000122f0: 7374 203d 207b 7d0a 2020 2020 2020 2020  st = {}.        
+00012300: 636f 6e74 6573 745b 2243 6f6e 7465 7374  contest["Contest
+00012310: 4e61 6d65 225d 203d 2028 0a20 2020 2020  Name"] = (.     
+00012320: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
+00012330: 6573 745f 6469 616c 6f67 2e63 6f6e 7465  est_dialog.conte
+00012340: 7374 2e63 7572 7265 6e74 5465 7874 2829  st.currentText()
+00012350: 2e6c 6f77 6572 2829 2e72 6570 6c61 6365  .lower().replace
+00012360: 2822 2022 2c20 225f 2229 0a20 2020 2020  (" ", "_").     
+00012370: 2020 2029 0a20 2020 2020 2020 2063 6f6e     ).        con
+00012380: 7465 7374 5b22 5374 6172 7444 6174 6522  test["StartDate"
+00012390: 5d20 3d20 7365 6c66 2e63 6f6e 7465 7374  ] = self.contest
+000123a0: 5f64 6961 6c6f 672e 6461 7465 5469 6d65  _dialog.dateTime
+000123b0: 4564 6974 2e64 6174 6554 696d 6528 292e  Edit.dateTime().
+000123c0: 746f 5374 7269 6e67 280a 2020 2020 2020  toString(.      
+000123d0: 2020 2020 2020 2279 7979 792d 4d4d 2d64        "yyyy-MM-d
+000123e0: 6420 6868 3a6d 6d3a 7373 220a 2020 2020  d hh:mm:ss".    
+000123f0: 2020 2020 290a 2020 2020 2020 2020 636f      ).        co
+00012400: 6e74 6573 745b 224f 7065 7261 746f 7243  ntest["OperatorC
+00012410: 6174 6567 6f72 7922 5d20 3d20 7365 6c66  ategory"] = self
+00012420: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
+00012430: 6f70 6572 6174 6f72 5f63 6c61 7373 2e63  operator_class.c
+00012440: 7572 7265 6e74 5465 7874 2829 0a20 2020  urrentText().   
+00012450: 2020 2020 2063 6f6e 7465 7374 5b22 4261       contest["Ba
+00012460: 6e64 4361 7465 676f 7279 225d 203d 2073  ndCategory"] = s
+00012470: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
+00012480: 6f67 2e62 616e 642e 6375 7272 656e 7454  og.band.currentT
+00012490: 6578 7428 290a 2020 2020 2020 2020 636f  ext().        co
+000124a0: 6e74 6573 745b 2250 6f77 6572 4361 7465  ntest["PowerCate
+000124b0: 676f 7279 225d 203d 2073 656c 662e 636f  gory"] = self.co
+000124c0: 6e74 6573 745f 6469 616c 6f67 2e70 6f77  ntest_dialog.pow
+000124d0: 6572 2e63 7572 7265 6e74 5465 7874 2829  er.currentText()
+000124e0: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
+000124f0: 5b22 4d6f 6465 4361 7465 676f 7279 225d  ["ModeCategory"]
+00012500: 203d 2073 656c 662e 636f 6e74 6573 745f   = self.contest_
+00012510: 6469 616c 6f67 2e6d 6f64 652e 6375 7272  dialog.mode.curr
+00012520: 656e 7454 6578 7428 290a 2020 2020 2020  entText().      
+00012530: 2020 636f 6e74 6573 745b 224f 7665 726c    contest["Overl
+00012540: 6179 4361 7465 676f 7279 225d 203d 2073  ayCategory"] = s
+00012550: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
+00012560: 6f67 2e6f 7665 726c 6179 2e63 7572 7265  og.overlay.curre
+00012570: 6e74 5465 7874 2829 0a20 2020 2020 2020  ntText().       
+00012580: 2023 2063 6f6e 7465 7374 5b27 436c 6169   # contest['Clai
+00012590: 6d65 6453 636f 7265 275d 203d 2073 656c  medScore'] = sel
+000125a0: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+000125b0: 2e0a 2020 2020 2020 2020 636f 6e74 6573  ..        contes
+000125c0: 745b 224f 7065 7261 746f 7273 225d 203d  t["Operators"] =
+000125d0: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
+000125e0: 616c 6f67 2e6f 7065 7261 746f 7273 2e74  alog.operators.t
+000125f0: 6578 7428 290a 2020 2020 2020 2020 636f  ext().        co
+00012600: 6e74 6573 745b 2253 6f61 7062 6f78 225d  ntest["Soapbox"]
+00012610: 203d 2073 656c 662e 636f 6e74 6573 745f   = self.contest_
+00012620: 6469 616c 6f67 2e73 6f61 7062 6f78 2e74  dialog.soapbox.t
+00012630: 6f50 6c61 696e 5465 7874 2829 0a20 2020  oPlainText().   
+00012640: 2020 2020 2063 6f6e 7465 7374 5b22 5365       contest["Se
+00012650: 6e74 4578 6368 616e 6765 225d 203d 2073  ntExchange"] = s
+00012660: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
+00012670: 6f67 2e65 7863 6861 6e67 652e 7465 7874  og.exchange.text
+00012680: 2829 0a20 2020 2020 2020 2063 6f6e 7465  ().        conte
+00012690: 7374 5b22 436f 6e74 6573 744e 5222 5d20  st["ContestNR"] 
+000126a0: 3d20 6e65 7874 5f6e 756d 6265 722e 6765  = next_number.ge
+000126b0: 7428 2263 6f75 6e74 222c 2031 290a 2020  t("count", 1).  
+000126c0: 2020 2020 2020 7365 6c66 2e70 7265 665b        self.pref[
+000126d0: 2263 6f6e 7465 7374 225d 203d 206e 6578  "contest"] = nex
+000126e0: 745f 6e75 6d62 6572 2e67 6574 2822 636f  t_number.get("co
+000126f0: 756e 7422 2c20 3129 0a20 2020 2020 2020  unt", 1).       
+00012700: 2023 2063 6f6e 7465 7374 5b27 5375 6254   # contest['SubT
+00012710: 7970 6527 5d20 3d20 7365 6c66 2e63 6f6e  ype'] = self.con
+00012720: 7465 7374 5f64 6961 6c6f 672e 0a20 2020  test_dialog..   
+00012730: 2020 2020 2063 6f6e 7465 7374 5b22 5374       contest["St
+00012740: 6174 696f 6e43 6174 6567 6f72 7922 5d20  ationCategory"] 
+00012750: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f64  = self.contest_d
+00012760: 6961 6c6f 672e 7374 6174 696f 6e2e 6375  ialog.station.cu
+00012770: 7272 656e 7454 6578 7428 290a 2020 2020  rrentText().    
+00012780: 2020 2020 636f 6e74 6573 745b 2241 7373      contest["Ass
+00012790: 6973 7465 6443 6174 6567 6f72 7922 5d20  istedCategory"] 
+000127a0: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f64  = self.contest_d
+000127b0: 6961 6c6f 672e 6173 7369 7374 6564 2e63  ialog.assisted.c
+000127c0: 7572 7265 6e74 5465 7874 2829 0a20 2020  urrentText().   
+000127d0: 2020 2020 2063 6f6e 7465 7374 5b22 5472       contest["Tr
+000127e0: 616e 736d 6974 7465 7243 6174 6567 6f72  ansmitterCategor
+000127f0: 7922 5d20 3d20 7365 6c66 2e63 6f6e 7465  y"] = self.conte
+00012800: 7374 5f64 6961 6c6f 672e 7472 616e 736d  st_dialog.transm
+00012810: 6974 7465 722e 6375 7272 656e 7454 6578  itter.currentTex
+00012820: 7428 290a 2020 2020 2020 2020 2320 636f  t().        # co
+00012830: 6e74 6573 745b 2754 696d 6543 6174 6567  ntest['TimeCateg
+00012840: 6f72 7927 5d20 3d20 7365 6c66 2e63 6f6e  ory'] = self.con
+00012850: 7465 7374 5f64 6961 6c6f 672e 0a20 2020  test_dialog..   
+00012860: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+00012870: 6728 2225 7322 2c20 6622 7b63 6f6e 7465  g("%s", f"{conte
+00012880: 7374 7d22 290a 2020 2020 2020 2020 7365  st}").        se
+00012890: 6c66 2e64 6174 6162 6173 652e 6164 645f  lf.database.add_
+000128a0: 636f 6e74 6573 7428 636f 6e74 6573 7429  contest(contest)
+000128b0: 0a20 2020 2020 2020 2073 656c 662e 7772  .        self.wr
+000128c0: 6974 655f 7072 6566 6572 656e 6365 2829  ite_preference()
+000128d0: 0a20 2020 2020 2020 2073 656c 662e 6c6f  .        self.lo
+000128e0: 6164 5f63 6f6e 7465 7374 2829 0a0a 2020  ad_contest()..  
+000128f0: 2020 6465 6620 6564 6974 5f73 7461 7469    def edit_stati
+00012900: 6f6e 5f73 6574 7469 6e67 7328 7365 6c66  on_settings(self
+00012910: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00012920: 2020 2022 2222 0a20 2020 2020 2020 2053     """.        S
+00012930: 686f 7720 7365 7474 696e 6773 2064 6961  how settings dia
+00012940: 6c6f 6720 666f 7220 7374 6174 696f 6e2e  log for station.
+00012950: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+00012960: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
+00012970: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00012980: 4e6f 6e65 0a0a 2020 2020 2020 2020 5265  None..        Re
+00012990: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
+000129a0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 4e6f  -----.        No
+000129b0: 6e65 0a20 2020 2020 2020 2022 2222 0a0a  ne.        """..
+000129c0: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+000129d0: 6562 7567 2822 5374 6174 696f 6e20 5365  ebug("Station Se
+000129e0: 7474 696e 6773 2073 656c 6563 7465 6422  ttings selected"
+000129f0: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00012a00: 7365 7474 696e 6773 5f64 6961 6c6f 6720  settings_dialog 
+00012a10: 3d20 4564 6974 5374 6174 696f 6e28 6673  = EditStation(fs
+00012a20: 7574 696c 732e 4150 505f 4441 5441 5f50  utils.APP_DATA_P
+00012a30: 4154 4829 0a20 2020 2020 2020 2069 6620  ATH).        if 
+00012a40: 7365 6c66 2e63 7572 7265 6e74 5f70 616c  self.current_pal
+00012a50: 6574 7465 3a0a 2020 2020 2020 2020 2020  ette:.          
+00012a60: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
+00012a70: 6469 616c 6f67 2e73 6574 5061 6c65 7474  dialog.setPalett
+00012a80: 6528 7365 6c66 2e63 7572 7265 6e74 5f70  e(self.current_p
+00012a90: 616c 6574 7465 290a 0a20 2020 2020 2020  alette)..       
+00012aa0: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
+00012ab0: 6961 6c6f 672e 6163 6365 7074 6564 2e63  ialog.accepted.c
+00012ac0: 6f6e 6e65 6374 2873 656c 662e 7361 7665  onnect(self.save
+00012ad0: 5f73 6574 7469 6e67 7329 0a20 2020 2020  _settings).     
+00012ae0: 2020 2073 656c 662e 7365 7474 696e 6773     self.settings
+00012af0: 5f64 6961 6c6f 672e 4361 6c6c 2e73 6574  _dialog.Call.set
+00012b00: 5465 7874 2873 656c 662e 7374 6174 696f  Text(self.statio
+00012b10: 6e2e 6765 7428 2243 616c 6c22 2c20 2222  n.get("Call", ""
+00012b20: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+00012b30: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
+00012b40: 4e61 6d65 2e73 6574 5465 7874 2873 656c  Name.setText(sel
+00012b50: 662e 7374 6174 696f 6e2e 6765 7428 224e  f.station.get("N
+00012b60: 616d 6522 2c20 2222 2929 0a20 2020 2020  ame", "")).     
+00012b70: 2020 2073 656c 662e 7365 7474 696e 6773     self.settings
+00012b80: 5f64 6961 6c6f 672e 4164 6472 6573 7331  _dialog.Address1
+00012b90: 2e73 6574 5465 7874 2873 656c 662e 7374  .setText(self.st
+00012ba0: 6174 696f 6e2e 6765 7428 2253 7472 6565  ation.get("Stree
+00012bb0: 7431 222c 2022 2229 290a 2020 2020 2020  t1", "")).      
+00012bc0: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
+00012bd0: 6469 616c 6f67 2e41 6464 7265 7373 322e  dialog.Address2.
+00012be0: 7365 7454 6578 7428 7365 6c66 2e73 7461  setText(self.sta
+00012bf0: 7469 6f6e 2e67 6574 2822 5374 7265 6574  tion.get("Street
+00012c00: 3222 2c20 2222 2929 0a20 2020 2020 2020  2", "")).       
+00012c10: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
+00012c20: 6961 6c6f 672e 4369 7479 2e73 6574 5465  ialog.City.setTe
+00012c30: 7874 2873 656c 662e 7374 6174 696f 6e2e  xt(self.station.
+00012c40: 6765 7428 2243 6974 7922 2c20 2222 2929  get("City", ""))
+00012c50: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
+00012c60: 7474 696e 6773 5f64 6961 6c6f 672e 5374  ttings_dialog.St
+00012c70: 6174 652e 7365 7454 6578 7428 7365 6c66  ate.setText(self
+00012c80: 2e73 7461 7469 6f6e 2e67 6574 2822 5374  .station.get("St
+00012c90: 6174 6522 2c20 2222 2929 0a20 2020 2020  ate", "")).     
+00012ca0: 2020 2073 656c 662e 7365 7474 696e 6773     self.settings
+00012cb0: 5f64 6961 6c6f 672e 5a69 702e 7365 7454  _dialog.Zip.setT
+00012cc0: 6578 7428 7365 6c66 2e73 7461 7469 6f6e  ext(self.station
+00012cd0: 2e67 6574 2822 5a69 7022 2c20 2222 2929  .get("Zip", ""))
+00012ce0: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
+00012cf0: 7474 696e 6773 5f64 6961 6c6f 672e 436f  ttings_dialog.Co
+00012d00: 756e 7472 792e 7365 7454 6578 7428 7365  untry.setText(se
+00012d10: 6c66 2e73 7461 7469 6f6e 2e67 6574 2822  lf.station.get("
+00012d20: 436f 756e 7472 7922 2c20 2222 2929 0a20  Country", "")). 
+00012d30: 2020 2020 2020 2073 656c 662e 7365 7474         self.sett
+00012d40: 696e 6773 5f64 6961 6c6f 672e 4772 6964  ings_dialog.Grid
+00012d50: 5371 7561 7265 2e73 6574 5465 7874 2873  Square.setText(s
+00012d60: 656c 662e 7374 6174 696f 6e2e 6765 7428  elf.station.get(
+00012d70: 2247 7269 6453 7175 6172 6522 2c20 2222  "GridSquare", ""
+00012d80: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+00012d90: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
+00012da0: 4351 5a6f 6e65 2e73 6574 5465 7874 2873  CQZone.setText(s
+00012db0: 7472 2873 656c 662e 7374 6174 696f 6e2e  tr(self.station.
+00012dc0: 6765 7428 2243 515a 6f6e 6522 2c20 2222  get("CQZone", ""
+00012dd0: 2929 290a 2020 2020 2020 2020 7365 6c66  ))).        self
+00012de0: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+00012df0: 2e49 5455 5a6f 6e65 2e73 6574 5465 7874  .ITUZone.setText
+00012e00: 2873 7472 2873 656c 662e 7374 6174 696f  (str(self.statio
+00012e10: 6e2e 6765 7428 2249 4152 555a 6f6e 6522  n.get("IARUZone"
+00012e20: 2c20 2222 2929 290a 2020 2020 2020 2020  , ""))).        
+00012e30: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
+00012e40: 616c 6f67 2e4c 6963 656e 7365 2e73 6574  alog.License.set
+00012e50: 5465 7874 2873 656c 662e 7374 6174 696f  Text(self.statio
+00012e60: 6e2e 6765 7428 224c 6963 656e 7365 436c  n.get("LicenseCl
+00012e70: 6173 7322 2c20 2222 2929 0a20 2020 2020  ass", "")).     
+00012e80: 2020 2073 656c 662e 7365 7474 696e 6773     self.settings
+00012e90: 5f64 6961 6c6f 672e 4c61 7469 7475 6465  _dialog.Latitude
+00012ea0: 2e73 6574 5465 7874 2873 7472 2873 656c  .setText(str(sel
+00012eb0: 662e 7374 6174 696f 6e2e 6765 7428 224c  f.station.get("L
+00012ec0: 6174 6974 7564 6522 2c20 2222 2929 290a  atitude", ""))).
+00012ed0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+00012ee0: 7469 6e67 735f 6469 616c 6f67 2e4c 6f6e  tings_dialog.Lon
+00012ef0: 6769 7475 6465 2e73 6574 5465 7874 2873  gitude.setText(s
+00012f00: 7472 2873 656c 662e 7374 6174 696f 6e2e  tr(self.station.
+00012f10: 6765 7428 224c 6f6e 6769 7475 6465 222c  get("Longitude",
+00012f20: 2022 2229 2929 0a20 2020 2020 2020 2073   ""))).        s
+00012f30: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
+00012f40: 6c6f 672e 5374 6174 696f 6e54 5852 582e  log.StationTXRX.
+00012f50: 7365 7454 6578 7428 7365 6c66 2e73 7461  setText(self.sta
+00012f60: 7469 6f6e 2e67 6574 2822 7374 6174 696f  tion.get("statio
+00012f70: 6e74 7872 7822 2c20 2222 2929 0a20 2020  ntxrx", "")).   
+00012f80: 2020 2020 2073 656c 662e 7365 7474 696e       self.settin
+00012f90: 6773 5f64 6961 6c6f 672e 506f 7765 722e  gs_dialog.Power.
+00012fa0: 7365 7454 6578 7428 7365 6c66 2e73 7461  setText(self.sta
+00012fb0: 7469 6f6e 2e67 6574 2822 5350 6f77 6522  tion.get("SPowe"
+00012fc0: 2c20 2222 2929 0a20 2020 2020 2020 2073  , "")).        s
+00012fd0: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
+00012fe0: 6c6f 672e 416e 7465 6e6e 612e 7365 7454  log.Antenna.setT
+00012ff0: 6578 7428 7365 6c66 2e73 7461 7469 6f6e  ext(self.station
+00013000: 2e67 6574 2822 5341 6e74 6522 2c20 2222  .get("SAnte", ""
+00013010: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+00013020: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
+00013030: 416e 7448 6569 6768 742e 7365 7454 6578  AntHeight.setTex
+00013040: 7428 7365 6c66 2e73 7461 7469 6f6e 2e67  t(self.station.g
+00013050: 6574 2822 5341 6e74 4831 222c 2022 2229  et("SAntH1", "")
+00013060: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+00013070: 6574 7469 6e67 735f 6469 616c 6f67 2e41  ettings_dialog.A
+00013080: 534c 2e73 6574 5465 7874 2873 656c 662e  SL.setText(self.
+00013090: 7374 6174 696f 6e2e 6765 7428 2253 416e  station.get("SAn
+000130a0: 7448 3222 2c20 2222 2929 0a20 2020 2020  tH2", "")).     
+000130b0: 2020 2073 656c 662e 7365 7474 696e 6773     self.settings
+000130c0: 5f64 6961 6c6f 672e 4152 524c 5365 6374  _dialog.ARRLSect
+000130d0: 696f 6e2e 7365 7454 6578 7428 7365 6c66  ion.setText(self
+000130e0: 2e73 7461 7469 6f6e 2e67 6574 2822 4152  .station.get("AR
+000130f0: 524c 5365 6374 696f 6e22 2c20 2222 2929  RLSection", ""))
+00013100: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
+00013110: 7474 696e 6773 5f64 6961 6c6f 672e 526f  ttings_dialog.Ro
+00013120: 7665 7251 5448 2e73 6574 5465 7874 2873  verQTH.setText(s
+00013130: 656c 662e 7374 6174 696f 6e2e 6765 7428  elf.station.get(
+00013140: 2252 6f76 6572 5154 4822 2c20 2222 2929  "RoverQTH", ""))
+00013150: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
+00013160: 7474 696e 6773 5f64 6961 6c6f 672e 436c  ttings_dialog.Cl
+00013170: 7562 2e73 6574 5465 7874 2873 656c 662e  ub.setText(self.
+00013180: 7374 6174 696f 6e2e 6765 7428 2243 6c75  station.get("Clu
+00013190: 6222 2c20 2222 2929 0a20 2020 2020 2020  b", "")).       
+000131a0: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
+000131b0: 6961 6c6f 672e 456d 6169 6c2e 7365 7454  ialog.Email.setT
+000131c0: 6578 7428 7365 6c66 2e73 7461 7469 6f6e  ext(self.station
+000131d0: 2e67 6574 2822 456d 6169 6c22 2c20 2222  .get("Email", ""
+000131e0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+000131f0: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
+00013200: 6f70 656e 2829 0a0a 2020 2020 6465 6620  open()..    def 
+00013210: 7361 7665 5f73 6574 7469 6e67 7328 7365  save_settings(se
+00013220: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
+00013230: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00013240: 2053 6176 6520 7365 7474 696e 6773 2074   Save settings t
+00013250: 6f20 6461 7461 6261 7365 2e0a 0a20 2020  o database...   
+00013260: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
+00013270: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+00013280: 2d2d 0a20 2020 2020 2020 204e 6f6e 650a  --.        None.
+00013290: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
 000132a0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-000132b0: 2d2d 2d0a 2020 2020 2020 2020 4e6f 6e65  ---.        None
-000132c0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-000132d0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-000132e0: 2d0a 2020 2020 2020 2020 4e6f 6e65 0a20  -.        None. 
-000132f0: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
-00013300: 2020 2020 6373 203d 2073 656c 662e 7365      cs = self.se
-00013310: 7474 696e 6773 5f64 6961 6c6f 672e 4361  ttings_dialog.Ca
-00013320: 6c6c 2e74 6578 7428 290a 2020 2020 2020  ll.text().      
-00013330: 2020 7365 6c66 2e73 7461 7469 6f6e 203d    self.station =
-00013340: 207b 7d0a 2020 2020 2020 2020 7365 6c66   {}.        self
-00013350: 2e73 7461 7469 6f6e 5b22 4361 6c6c 225d  .station["Call"]
-00013360: 203d 2063 732e 7570 7065 7228 290a 2020   = cs.upper().  
-00013370: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
-00013380: 6f6e 5b22 4e61 6d65 225d 203d 2073 656c  on["Name"] = sel
-00013390: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
-000133a0: 672e 4e61 6d65 2e74 6578 7428 292e 7469  g.Name.text().ti
-000133b0: 746c 6528 290a 2020 2020 2020 2020 7365  tle().        se
-000133c0: 6c66 2e73 7461 7469 6f6e 5b22 5374 7265  lf.station["Stre
-000133d0: 6574 3122 5d20 3d20 7365 6c66 2e73 6574  et1"] = self.set
-000133e0: 7469 6e67 735f 6469 616c 6f67 2e41 6464  tings_dialog.Add
-000133f0: 7265 7373 312e 7465 7874 2829 2e74 6974  ress1.text().tit
-00013400: 6c65 2829 0a20 2020 2020 2020 2073 656c  le().        sel
-00013410: 662e 7374 6174 696f 6e5b 2253 7472 6565  f.station["Stree
-00013420: 7432 225d 203d 2073 656c 662e 7365 7474  t2"] = self.sett
-00013430: 696e 6773 5f64 6961 6c6f 672e 4164 6472  ings_dialog.Addr
-00013440: 6573 7332 2e74 6578 7428 292e 7469 746c  ess2.text().titl
-00013450: 6528 290a 2020 2020 2020 2020 7365 6c66  e().        self
-00013460: 2e73 7461 7469 6f6e 5b22 4369 7479 225d  .station["City"]
-00013470: 203d 2073 656c 662e 7365 7474 696e 6773   = self.settings
-00013480: 5f64 6961 6c6f 672e 4369 7479 2e74 6578  _dialog.City.tex
-00013490: 7428 292e 7469 746c 6528 290a 2020 2020  t().title().    
-000134a0: 2020 2020 7365 6c66 2e73 7461 7469 6f6e      self.station
-000134b0: 5b22 5374 6174 6522 5d20 3d20 7365 6c66  ["State"] = self
-000134c0: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
-000134d0: 2e53 7461 7465 2e74 6578 7428 292e 7570  .State.text().up
-000134e0: 7065 7228 290a 2020 2020 2020 2020 7365  per().        se
-000134f0: 6c66 2e73 7461 7469 6f6e 5b22 5a69 7022  lf.station["Zip"
-00013500: 5d20 3d20 7365 6c66 2e73 6574 7469 6e67  ] = self.setting
-00013510: 735f 6469 616c 6f67 2e5a 6970 2e74 6578  s_dialog.Zip.tex
-00013520: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
-00013530: 2e73 7461 7469 6f6e 5b22 436f 756e 7472  .station["Countr
-00013540: 7922 5d20 3d20 7365 6c66 2e73 6574 7469  y"] = self.setti
-00013550: 6e67 735f 6469 616c 6f67 2e43 6f75 6e74  ngs_dialog.Count
-00013560: 7279 2e74 6578 7428 292e 7469 746c 6528  ry.text().title(
-00013570: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-00013580: 7461 7469 6f6e 5b22 4772 6964 5371 7561  tation["GridSqua
-00013590: 7265 225d 203d 2073 656c 662e 7365 7474  re"] = self.sett
-000135a0: 696e 6773 5f64 6961 6c6f 672e 4772 6964  ings_dialog.Grid
-000135b0: 5371 7561 7265 2e74 6578 7428 290a 2020  Square.text().  
-000135c0: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
-000135d0: 6f6e 5b22 4351 5a6f 6e65 225d 203d 2073  on["CQZone"] = s
-000135e0: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
-000135f0: 6c6f 672e 4351 5a6f 6e65 2e74 6578 7428  log.CQZone.text(
-00013600: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-00013610: 7461 7469 6f6e 5b22 4941 5255 5a6f 6e65  tation["IARUZone
-00013620: 225d 203d 2073 656c 662e 7365 7474 696e  "] = self.settin
-00013630: 6773 5f64 6961 6c6f 672e 4954 555a 6f6e  gs_dialog.ITUZon
-00013640: 652e 7465 7874 2829 0a20 2020 2020 2020  e.text().       
-00013650: 2073 656c 662e 7374 6174 696f 6e5b 224c   self.station["L
-00013660: 6963 656e 7365 436c 6173 7322 5d20 3d20  icenseClass"] = 
-00013670: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
-00013680: 616c 6f67 2e4c 6963 656e 7365 2e74 6578  alog.License.tex
-00013690: 7428 292e 7469 746c 6528 290a 2020 2020  t().title().    
-000136a0: 2020 2020 7365 6c66 2e73 7461 7469 6f6e      self.station
-000136b0: 5b22 4c61 7469 7475 6465 225d 203d 2073  ["Latitude"] = s
-000136c0: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
-000136d0: 6c6f 672e 4c61 7469 7475 6465 2e74 6578  log.Latitude.tex
-000136e0: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
-000136f0: 2e73 7461 7469 6f6e 5b22 4c6f 6e67 6974  .station["Longit
-00013700: 7564 6522 5d20 3d20 7365 6c66 2e73 6574  ude"] = self.set
-00013710: 7469 6e67 735f 6469 616c 6f67 2e4c 6f6e  tings_dialog.Lon
-00013720: 6769 7475 6465 2e74 6578 7428 290a 2020  gitude.text().  
-00013730: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
-00013740: 6f6e 5b22 5354 5865 7122 5d20 3d20 7365  on["STXeq"] = se
-00013750: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
-00013760: 6f67 2e53 7461 7469 6f6e 5458 5258 2e74  og.StationTXRX.t
-00013770: 6578 7428 290a 2020 2020 2020 2020 7365  ext().        se
-00013780: 6c66 2e73 7461 7469 6f6e 5b22 5350 6f77  lf.station["SPow
-00013790: 6522 5d20 3d20 7365 6c66 2e73 6574 7469  e"] = self.setti
-000137a0: 6e67 735f 6469 616c 6f67 2e50 6f77 6572  ngs_dialog.Power
-000137b0: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
-000137c0: 7365 6c66 2e73 7461 7469 6f6e 5b22 5341  self.station["SA
-000137d0: 6e74 6522 5d20 3d20 7365 6c66 2e73 6574  nte"] = self.set
-000137e0: 7469 6e67 735f 6469 616c 6f67 2e41 6e74  tings_dialog.Ant
-000137f0: 656e 6e61 2e74 6578 7428 290a 2020 2020  enna.text().    
-00013800: 2020 2020 7365 6c66 2e73 7461 7469 6f6e      self.station
-00013810: 5b22 5341 6e74 4831 225d 203d 2073 656c  ["SAntH1"] = sel
-00013820: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
-00013830: 672e 416e 7448 6569 6768 742e 7465 7874  g.AntHeight.text
-00013840: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-00013850: 7374 6174 696f 6e5b 2253 416e 7448 3222  station["SAntH2"
-00013860: 5d20 3d20 7365 6c66 2e73 6574 7469 6e67  ] = self.setting
-00013870: 735f 6469 616c 6f67 2e41 534c 2e74 6578  s_dialog.ASL.tex
-00013880: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
-00013890: 2e73 7461 7469 6f6e 5b22 4152 524c 5365  .station["ARRLSe
-000138a0: 6374 696f 6e22 5d20 3d20 7365 6c66 2e73  ction"] = self.s
-000138b0: 6574 7469 6e67 735f 6469 616c 6f67 2e41  ettings_dialog.A
-000138c0: 5252 4c53 6563 7469 6f6e 2e74 6578 7428  RRLSection.text(
-000138d0: 292e 7570 7065 7228 290a 2020 2020 2020  ).upper().      
-000138e0: 2020 7365 6c66 2e73 7461 7469 6f6e 5b22    self.station["
-000138f0: 526f 7665 7251 5448 225d 203d 2073 656c  RoverQTH"] = sel
-00013900: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
-00013910: 672e 526f 7665 7251 5448 2e74 6578 7428  g.RoverQTH.text(
-00013920: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-00013930: 7461 7469 6f6e 5b22 436c 7562 225d 203d  tation["Club"] =
-00013940: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
-00013950: 6961 6c6f 672e 436c 7562 2e74 6578 7428  ialog.Club.text(
-00013960: 292e 7469 746c 6528 290a 2020 2020 2020  ).title().      
-00013970: 2020 7365 6c66 2e73 7461 7469 6f6e 5b22    self.station["
-00013980: 456d 6169 6c22 5d20 3d20 7365 6c66 2e73  Email"] = self.s
-00013990: 6574 7469 6e67 735f 6469 616c 6f67 2e45  ettings_dialog.E
-000139a0: 6d61 696c 2e74 6578 7428 290a 2020 2020  mail.text().    
-000139b0: 2020 2020 7365 6c66 2e64 6174 6162 6173      self.databas
-000139c0: 652e 6164 645f 7374 6174 696f 6e28 7365  e.add_station(se
-000139d0: 6c66 2e73 7461 7469 6f6e 290a 2020 2020  lf.station).    
-000139e0: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
-000139f0: 735f 6469 616c 6f67 2e63 6c6f 7365 2829  s_dialog.close()
-00013a00: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00013a10: 2e63 7572 7265 6e74 5f6f 7020 3d3d 2022  .current_op == "
-00013a20: 223a 0a20 2020 2020 2020 2020 2020 2073  ":.            s
-00013a30: 656c 662e 6375 7272 656e 745f 6f70 203d  elf.current_op =
-00013a40: 2073 656c 662e 7374 6174 696f 6e2e 6765   self.station.ge
-00013a50: 7428 2243 616c 6c22 2c20 2222 290a 2020  t("Call", "").  
-00013a60: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00013a70: 616b 655f 6f70 5f64 6972 2829 0a20 2020  ake_op_dir().   
-00013a80: 2020 2020 2063 6f6e 7465 7374 5f63 6f75       contest_cou
-00013a90: 6e74 203d 2073 656c 662e 6461 7461 6261  nt = self.databa
-00013aa0: 7365 2e66 6574 6368 5f61 6c6c 5f63 6f6e  se.fetch_all_con
-00013ab0: 7465 7374 7328 290a 2020 2020 2020 2020  tests().        
-00013ac0: 6966 206c 656e 2863 6f6e 7465 7374 5f63  if len(contest_c
-00013ad0: 6f75 6e74 2920 3d3d 2030 3a0a 2020 2020  ount) == 0:.    
-00013ae0: 2020 2020 2020 2020 7365 6c66 2e6e 6577          self.new
-00013af0: 5f63 6f6e 7465 7374 5f64 6961 6c6f 6728  _contest_dialog(
-00013b00: 290a 0a20 2020 2064 6566 2065 6469 745f  )..    def edit_
-00013b10: 6d61 6372 6f28 7365 6c66 2c20 6675 6e63  macro(self, func
-00013b20: 7469 6f6e 5f6b 6579 2920 2d3e 204e 6f6e  tion_key) -> Non
-00013b30: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
-00013b40: 2020 2020 2020 2053 686f 7720 6564 6974         Show edit
-00013b50: 206d 6163 726f 2064 6961 6c6f 6720 666f   macro dialog fo
-00013b60: 7220 6675 6e63 7469 6f6e 206b 6579 2e0a  r function key..
-00013b70: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-00013b80: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
-00013b90: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2066  ------.        f
-00013ba0: 756e 6374 696f 6e5f 6b65 7920 3a20 7374  unction_key : st
-00013bb0: 720a 2020 2020 2020 2020 4675 6e63 7469  r.        Functi
-00013bc0: 6f6e 206b 6579 2074 6f20 6564 6974 2e0a  on key to edit..
-00013bd0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00013be0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00013bf0: 0a20 2020 2020 2020 204e 6f6e 650a 2020  .        None.  
-00013c00: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
-00013c10: 2020 2073 656c 662e 6564 6974 5f6d 6163     self.edit_mac
-00013c20: 726f 5f64 6961 6c6f 6720 3d20 4564 6974  ro_dialog = Edit
-00013c30: 4d61 6372 6f28 6675 6e63 7469 6f6e 5f6b  Macro(function_k
-00013c40: 6579 2c20 6673 7574 696c 732e 4150 505f  ey, fsutils.APP_
-00013c50: 4441 5441 5f50 4154 4829 0a0a 2020 2020  DATA_PATH)..    
-00013c60: 2020 2020 6966 2073 656c 662e 6375 7272      if self.curr
-00013c70: 656e 745f 7061 6c65 7474 653a 0a20 2020  ent_palette:.   
-00013c80: 2020 2020 2020 2020 2073 656c 662e 6564           self.ed
-00013c90: 6974 5f6d 6163 726f 5f64 6961 6c6f 672e  it_macro_dialog.
-00013ca0: 7365 7450 616c 6574 7465 2873 656c 662e  setPalette(self.
-00013cb0: 6375 7272 656e 745f 7061 6c65 7474 6529  current_palette)
-00013cc0: 0a0a 2020 2020 2020 2020 7365 6c66 2e65  ..        self.e
-00013cd0: 6469 745f 6d61 6372 6f5f 6469 616c 6f67  dit_macro_dialog
-00013ce0: 2e61 6363 6570 7465 642e 636f 6e6e 6563  .accepted.connec
-00013cf0: 7428 7365 6c66 2e65 6469 7465 645f 6d61  t(self.edited_ma
-00013d00: 6372 6f29 0a20 2020 2020 2020 2073 656c  cro).        sel
-00013d10: 662e 6564 6974 5f6d 6163 726f 5f64 6961  f.edit_macro_dia
-00013d20: 6c6f 672e 6f70 656e 2829 0a0a 2020 2020  log.open()..    
-00013d30: 6465 6620 6564 6974 6564 5f6d 6163 726f  def edited_macro
-00013d40: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-00013d50: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00013d60: 2020 2020 5361 7665 2065 6469 7465 6420      Save edited 
-00013d70: 6d61 6372 6f20 746f 2064 6174 6162 6173  macro to databas
-00013d80: 652e 0a0a 2020 2020 2020 2020 5061 7261  e...        Para
-00013d90: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
-00013da0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-00013db0: 2020 4e6f 6e65 0a0a 2020 2020 2020 2020    None..        
-00013dc0: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
-00013dd0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-00013de0: 4e6f 6e65 0a20 2020 2020 2020 2022 2222  None.        """
-00013df0: 0a0a 2020 2020 2020 2020 7365 6c66 2e65  ..        self.e
-00013e00: 6469 745f 6d61 6372 6f5f 6469 616c 6f67  dit_macro_dialog
-00013e10: 2e66 756e 6374 696f 6e5f 6b65 792e 7365  .function_key.se
-00013e20: 7454 6578 7428 0a20 2020 2020 2020 2020  tText(.         
-00013e30: 2020 2073 656c 662e 6564 6974 5f6d 6163     self.edit_mac
-00013e40: 726f 5f64 6961 6c6f 672e 6d61 6372 6f5f  ro_dialog.macro_
-00013e50: 6c61 6265 6c2e 7465 7874 2829 0a20 2020  label.text().   
-00013e60: 2020 2020 2029 0a20 2020 2020 2020 2073       ).        s
-00013e70: 656c 662e 6564 6974 5f6d 6163 726f 5f64  elf.edit_macro_d
-00013e80: 6961 6c6f 672e 6675 6e63 7469 6f6e 5f6b  ialog.function_k
-00013e90: 6579 2e73 6574 546f 6f6c 5469 7028 0a20  ey.setToolTip(. 
-00013ea0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00013eb0: 6564 6974 5f6d 6163 726f 5f64 6961 6c6f  edit_macro_dialo
-00013ec0: 672e 7468 655f 6d61 6372 6f2e 7465 7874  g.the_macro.text
-00013ed0: 2829 0a20 2020 2020 2020 2029 0a20 2020  ().        ).   
-00013ee0: 2020 2020 2073 656c 662e 6564 6974 5f6d       self.edit_m
-00013ef0: 6163 726f 5f64 6961 6c6f 672e 636c 6f73  acro_dialog.clos
-00013f00: 6528 290a 0a20 2020 2064 6566 2070 726f  e()..    def pro
-00013f10: 6365 7373 5f6d 6163 726f 2873 656c 662c  cess_macro(self,
-00013f20: 206d 6163 726f 3a20 7374 7229 202d 3e20   macro: str) -> 
-00013f30: 7374 723a 0a20 2020 2020 2020 2022 2222  str:.        """
-00013f40: 0a20 2020 2020 2020 2050 726f 6365 7373  .        Process
-00013f50: 2043 5720 6d61 6372 6f20 7375 6273 7469   CW macro substi
-00013f60: 7475 7469 6f6e 7320 666f 7220 636f 6e74  tutions for cont
-00013f70: 6573 742e 0a0a 2020 2020 2020 2020 5061  est...        Pa
-00013f80: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
-00013f90: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00013fa0: 2020 2020 6d61 6372 6f20 3a20 7374 720a      macro : str.
-00013fb0: 2020 2020 2020 2020 4d61 6372 6f20 746f          Macro to
-00013fc0: 2070 726f 6365 7373 2e0a 0a20 2020 2020   process...     
-00013fd0: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
-00013fe0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
-00013ff0: 2020 2073 7472 0a20 2020 2020 2020 2050     str.        P
-00014000: 726f 6365 7373 6564 206d 6163 726f 2e0a  rocessed macro..
-00014010: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
-00014020: 2020 2020 2072 6573 756c 7420 3d20 7365       result = se
-00014030: 6c66 2e64 6174 6162 6173 652e 6765 745f  lf.database.get_
-00014040: 7365 7269 616c 2829 0a20 2020 2020 2020  serial().       
-00014050: 206e 6578 745f 7365 7269 616c 203d 2073   next_serial = s
-00014060: 7472 2872 6573 756c 742e 6765 7428 2273  tr(result.get("s
-00014070: 6572 6961 6c5f 6e72 222c 2022 3122 2929  erial_nr", "1"))
-00014080: 0a20 2020 2020 2020 2069 6620 6e65 7874  .        if next
-00014090: 5f73 6572 6961 6c20 3d3d 2022 4e6f 6e65  _serial == "None
-000140a0: 223a 0a20 2020 2020 2020 2020 2020 206e  ":.            n
-000140b0: 6578 745f 7365 7269 616c 203d 2022 3122  ext_serial = "1"
-000140c0: 0a20 2020 2020 2020 206d 6163 726f 203d  .        macro =
-000140d0: 206d 6163 726f 2e75 7070 6572 2829 0a20   macro.upper(). 
-000140e0: 2020 2020 2020 206d 6163 726f 203d 206d         macro = m
-000140f0: 6163 726f 2e72 6570 6c61 6365 2822 2322  acro.replace("#"
-00014100: 2c20 6e65 7874 5f73 6572 6961 6c29 0a20  , next_serial). 
-00014110: 2020 2020 2020 206d 6163 726f 203d 206d         macro = m
-00014120: 6163 726f 2e72 6570 6c61 6365 2822 7b4d  acro.replace("{M
-00014130: 5943 414c 4c7d 222c 2073 656c 662e 7374  YCALL}", self.st
-00014140: 6174 696f 6e2e 6765 7428 2243 616c 6c22  ation.get("Call"
-00014150: 2c20 2222 2929 0a20 2020 2020 2020 206d  , "")).        m
-00014160: 6163 726f 203d 206d 6163 726f 2e72 6570  acro = macro.rep
-00014170: 6c61 6365 2822 7b48 4953 4341 4c4c 7d22  lace("{HISCALL}"
-00014180: 2c20 7365 6c66 2e63 616c 6c73 6967 6e2e  , self.callsign.
-00014190: 7465 7874 2829 290a 2020 2020 2020 2020  text()).        
-000141a0: 6966 2073 656c 662e 7261 6469 6f5f 7374  if self.radio_st
-000141b0: 6174 652e 6765 7428 226d 6f64 6522 2920  ate.get("mode") 
-000141c0: 3d3d 2022 4357 223a 0a20 2020 2020 2020  == "CW":.       
-000141d0: 2020 2020 206d 6163 726f 203d 206d 6163       macro = mac
-000141e0: 726f 2e72 6570 6c61 6365 2822 7b53 4e54  ro.replace("{SNT
-000141f0: 7d22 2c20 7365 6c66 2e73 656e 742e 7465  }", self.sent.te
-00014200: 7874 2829 2e72 6570 6c61 6365 2822 3922  xt().replace("9"
-00014210: 2c20 226e 2229 290a 2020 2020 2020 2020  , "n")).        
-00014220: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00014230: 2020 6d61 6372 6f20 3d20 6d61 6372 6f2e    macro = macro.
-00014240: 7265 706c 6163 6528 227b 534e 547d 222c  replace("{SNT}",
-00014250: 2073 656c 662e 7365 6e74 2e74 6578 7428   self.sent.text(
-00014260: 2929 0a20 2020 2020 2020 206d 6163 726f  )).        macro
-00014270: 203d 206d 6163 726f 2e72 6570 6c61 6365   = macro.replace
-00014280: 2822 7b53 454e 544e 527d 222c 2073 656c  ("{SENTNR}", sel
-00014290: 662e 6f74 6865 725f 312e 7465 7874 2829  f.other_1.text()
-000142a0: 290a 2020 2020 2020 2020 6d61 6372 6f20  ).        macro 
-000142b0: 3d20 6d61 6372 6f2e 7265 706c 6163 6528  = macro.replace(
-000142c0: 0a20 2020 2020 2020 2020 2020 2022 7b45  .            "{E
-000142d0: 5843 487d 222c 2073 656c 662e 636f 6e74  XCH}", self.cont
-000142e0: 6573 745f 7365 7474 696e 6773 2e67 6574  est_settings.get
-000142f0: 2822 5365 6e74 4578 6368 616e 6765 222c  ("SentExchange",
-00014300: 2022 7878 7822 290a 2020 2020 2020 2020   "xxx").        
-00014310: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00014320: 206d 6163 726f 0a0a 2020 2020 6465 6620   macro..    def 
-00014330: 766f 6963 655f 7374 7269 6e67 2873 656c  voice_string(sel
-00014340: 662c 2074 6865 5f73 7472 696e 673a 2073  f, the_string: s
-00014350: 7472 2920 2d3e 204e 6f6e 653a 0a20 2020  tr) -> None:.   
-00014360: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00014370: 2076 6f69 6365 7320 7374 7269 6e67 2075   voices string u
-00014380: 7369 6e67 206e 6174 6f20 7068 6f6e 6574  sing nato phonet
-00014390: 6963 732e 0a0a 2020 2020 2020 2020 5061  ics...        Pa
-000143a0: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
-000143b0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-000143c0: 2020 2020 7468 655f 7374 7269 6e67 203a      the_string :
-000143d0: 2073 7472 0a20 2020 2020 2020 2053 7472   str.        Str
-000143e0: 696e 6720 746f 2076 6f69 6369 6679 2e0a  ing to voicify..
-000143f0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00014400: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00014410: 0a20 2020 2020 2020 204e 6f6e 650a 2020  .        None.  
-00014420: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
-00014430: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-00014440: 2256 6f69 6369 6e67 3a20 2573 222c 2074  "Voicing: %s", t
-00014450: 6865 5f73 7472 696e 6729 0a20 2020 2020  he_string).     
-00014460: 2020 206f 705f 7061 7468 203d 2066 7375     op_path = fsu
-00014470: 7469 6c73 2e55 5345 525f 4441 5441 5f50  tils.USER_DATA_P
-00014480: 4154 4820 2f20 7365 6c66 2e63 7572 7265  ATH / self.curre
-00014490: 6e74 5f6f 700a 2020 2020 2020 2020 6966  nt_op.        if
-000144a0: 2022 5b22 2069 6e20 7468 655f 7374 7269   "[" in the_stri
-000144b0: 6e67 3a0a 2020 2020 2020 2020 2020 2020  ng:.            
-000144c0: 7375 625f 7374 7269 6e67 203d 2074 6865  sub_string = the
-000144d0: 5f73 7472 696e 672e 7374 7269 7028 225b  _string.strip("[
-000144e0: 5d22 292e 6c6f 7765 7228 290a 2020 2020  ]").lower().    
-000144f0: 2020 2020 2020 2020 6669 6c65 6e61 6d65          filename
-00014500: 203d 2066 227b 7374 7228 6f70 5f70 6174   = f"{str(op_pat
-00014510: 6829 7d2f 7b73 7562 5f73 7472 696e 677d  h)}/{sub_string}
-00014520: 2e77 6176 220a 2020 2020 2020 2020 2020  .wav".          
-00014530: 2020 6966 2050 6174 6828 6669 6c65 6e61    if Path(filena
-00014540: 6d65 292e 6973 5f66 696c 6528 293a 0a20  me).is_file():. 
-00014550: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00014560: 6f67 6765 722e 6465 6275 6728 2256 6f69  ogger.debug("Voi
-00014570: 6369 6e67 3a20 2573 222c 2066 696c 656e  cing: %s", filen
-00014580: 616d 6529 0a20 2020 2020 2020 2020 2020  ame).           
-00014590: 2020 2020 2064 6174 612c 205f 6673 203d       data, _fs =
-000145a0: 2073 662e 7265 6164 2866 696c 656e 616d   sf.read(filenam
-000145b0: 652c 2064 7479 7065 3d22 666c 6f61 7433  e, dtype="float3
-000145c0: 3222 290a 2020 2020 2020 2020 2020 2020  2").            
-000145d0: 2020 2020 7365 6c66 2e70 7474 5f6f 6e28      self.ptt_on(
-000145e0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000145f0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-00014600: 2020 2020 2020 2020 2020 2073 642e 6465             sd.de
-00014610: 6661 756c 742e 6465 7669 6365 203d 2073  fault.device = s
-00014620: 656c 662e 7072 6566 2e67 6574 2822 736f  elf.pref.get("so
-00014630: 756e 6464 6576 6963 6522 2c20 2264 6566  unddevice", "def
-00014640: 6175 6c74 2229 0a20 2020 2020 2020 2020  ault").         
-00014650: 2020 2020 2020 2020 2020 2073 642e 6465             sd.de
-00014660: 6661 756c 742e 7361 6d70 6c65 7261 7465  fault.samplerate
-00014670: 203d 2034 3431 3030 2e30 0a20 2020 2020   = 44100.0.     
-00014680: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00014690: 642e 706c 6179 2864 6174 612c 2062 6c6f  d.play(data, blo
-000146a0: 636b 696e 673d 4661 6c73 6529 0a20 2020  cking=False).   
-000146b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000146c0: 2023 205f 7374 6174 7573 203d 2073 642e   # _status = sd.
-000146d0: 7761 6974 2829 0a20 2020 2020 2020 2020  wait().         
-000146e0: 2020 2020 2020 2020 2020 2023 2068 7474             # htt
-000146f0: 7073 3a2f 2f73 6e79 6b2e 696f 2f61 6476  ps://snyk.io/adv
-00014700: 6973 6f72 2f70 7974 686f 6e2f 736f 756e  isor/python/soun
-00014710: 6464 6576 6963 652f 6675 6e63 7469 6f6e  ddevice/function
-00014720: 732f 736f 756e 6464 6576 6963 652e 506f  s/sounddevice.Po
-00014730: 7274 4175 6469 6f45 7272 6f72 0a20 2020  rtAudioError.   
-00014740: 2020 2020 2020 2020 2020 2020 2065 7863               exc
-00014750: 6570 7420 7364 2e50 6f72 7441 7564 696f  ept sd.PortAudio
-00014760: 4572 726f 7220 6173 2065 7272 3a0a 2020  Error as err:.  
-00014770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014780: 2020 6c6f 6767 6572 2e77 6172 6e69 6e67    logger.warning
-00014790: 2822 2573 222c 2066 227b 6572 727d 2229  ("%s", f"{err}")
-000147a0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000147b0: 2020 7365 6c66 2e70 7474 5f6f 6666 2829    self.ptt_off()
-000147c0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000147d0: 7572 6e0a 2020 2020 2020 2020 7365 6c66  urn.        self
-000147e0: 2e70 7474 5f6f 6e28 290a 2020 2020 2020  .ptt_on().      
-000147f0: 2020 666f 7220 6c65 7474 6572 2069 6e20    for letter in 
-00014800: 7468 655f 7374 7269 6e67 2e6c 6f77 6572  the_string.lower
-00014810: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00014820: 6966 206c 6574 7465 7220 696e 2022 6162  if letter in "ab
-00014830: 6364 6566 6768 696a 6b6c 6d6e 6f70 7172  cdefghijklmnopqr
-00014840: 7374 7576 7778 797a 2031 3233 3435 3637  stuvwxyz 1234567
-00014850: 3839 3022 3a0a 2020 2020 2020 2020 2020  890":.          
-00014860: 2020 2020 2020 6966 206c 6574 7465 7220        if letter 
-00014870: 3d3d 2022 2022 3a0a 2020 2020 2020 2020  == " ":.        
-00014880: 2020 2020 2020 2020 2020 2020 6c65 7474              lett
-00014890: 6572 203d 2022 7370 6163 6522 0a20 2020  er = "space".   
-000148a0: 2020 2020 2020 2020 2020 2020 2066 696c               fil
-000148b0: 656e 616d 6520 3d20 6622 7b73 7472 286f  ename = f"{str(o
-000148c0: 705f 7061 7468 297d 2f7b 6c65 7474 6572  p_path)}/{letter
-000148d0: 7d2e 7761 7622 0a20 2020 2020 2020 2020  }.wav".         
-000148e0: 2020 2020 2020 2069 6620 5061 7468 2866         if Path(f
-000148f0: 696c 656e 616d 6529 2e69 735f 6669 6c65  ilename).is_file
-00014900: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00014910: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-00014920: 6562 7567 2822 566f 6963 696e 673a 2025  ebug("Voicing: %
-00014930: 7322 2c20 6669 6c65 6e61 6d65 290a 2020  s", filename).  
-00014940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014950: 2020 6461 7461 2c20 5f66 7320 3d20 7366    data, _fs = sf
-00014960: 2e72 6561 6428 6669 6c65 6e61 6d65 2c20  .read(filename, 
-00014970: 6474 7970 653d 2266 6c6f 6174 3332 2229  dtype="float32")
-00014980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014990: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-000149a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000149b0: 2020 7364 2e64 6566 6175 6c74 2e64 6576    sd.default.dev
-000149c0: 6963 6520 3d20 7365 6c66 2e70 7265 662e  ice = self.pref.
-000149d0: 6765 7428 2273 6f75 6e64 6465 7669 6365  get("sounddevice
-000149e0: 222c 2022 6465 6661 756c 7422 290a 2020  ", "default").  
-000149f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014a00: 2020 2020 2020 7364 2e64 6566 6175 6c74        sd.default
-00014a10: 2e73 616d 706c 6572 6174 6520 3d20 3434  .samplerate = 44
-00014a20: 3130 302e 300a 2020 2020 2020 2020 2020  100.0.          
-00014a30: 2020 2020 2020 2020 2020 2020 2020 7364                sd
-00014a40: 2e70 6c61 7928 6461 7461 2c20 626c 6f63  .play(data, bloc
-00014a50: 6b69 6e67 3d46 616c 7365 290a 2020 2020  king=False).    
-00014a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014a70: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-00014a80: 2822 2573 222c 2066 227b 7364 2e77 6169  ("%s", f"{sd.wai
-00014a90: 7428 297d 2229 0a20 2020 2020 2020 2020  t()}").         
-00014aa0: 2020 2020 2020 2020 2020 2065 7863 6570             excep
-00014ab0: 7420 7364 2e50 6f72 7441 7564 696f 4572  t sd.PortAudioEr
-00014ac0: 726f 7220 6173 2065 7272 3a0a 2020 2020  ror as err:.    
-00014ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ae0: 2020 2020 6c6f 6767 6572 2e77 6172 6e69      logger.warni
-00014af0: 6e67 2822 2573 222c 2066 227b 6572 727d  ng("%s", f"{err}
-00014b00: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00014b10: 7074 745f 6f66 6628 290a 0a20 2020 2064  ptt_off()..    d
-00014b20: 6566 2070 7474 5f6f 6e28 7365 6c66 2920  ef ptt_on(self) 
-00014b30: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00014b40: 2022 2222 0a20 2020 2020 2020 2054 7572   """.        Tur
-00014b50: 6e20 6f6e 2070 7474 2066 6f72 2072 6967  n on ptt for rig
-00014b60: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-00014b70: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
-00014b80: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-00014b90: 204e 6f6e 650a 0a20 2020 2020 2020 2052   None..        R
-00014ba0: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
-00014bb0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 204e  ------.        N
-00014bc0: 6f6e 650a 2020 2020 2020 2020 2222 220a  one.        """.
-00014bd0: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
-00014be0: 6465 6275 6728 2250 5454 204f 6e22 290a  debug("PTT On").
-00014bf0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00014c00: 7269 675f 636f 6e74 726f 6c3a 0a20 2020  rig_control:.   
-00014c10: 2020 2020 2020 2020 2073 656c 662e 6c65           self.le
-00014c20: 6674 646f 742e 7365 7450 6978 6d61 7028  ftdot.setPixmap(
-00014c30: 7365 6c66 2e67 7265 656e 646f 7429 0a20  self.greendot). 
-00014c40: 2020 2020 2020 2020 2020 2061 7070 2e70             app.p
-00014c50: 726f 6365 7373 4576 656e 7473 2829 0a20  rocessEvents(). 
-00014c60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00014c70: 7269 675f 636f 6e74 726f 6c2e 7074 745f  rig_control.ptt_
-00014c80: 6f6e 2829 0a0a 2020 2020 6465 6620 7074  on()..    def pt
-00014c90: 745f 6f66 6628 7365 6c66 2920 2d3e 204e  t_off(self) -> N
-00014ca0: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-00014cb0: 0a20 2020 2020 2020 2054 7572 6e20 6f66  .        Turn of
-00014cc0: 6620 7074 7420 666f 7220 7269 672e 0a0a  f ptt for rig...
-00014cd0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-00014ce0: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
-00014cf0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 4e6f  -----.        No
-00014d00: 6e65 0a0a 2020 2020 2020 2020 5265 7475  ne..        Retu
-00014d10: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
-00014d20: 2d2d 2d0a 2020 2020 2020 2020 4e6f 6e65  ---.        None
-00014d30: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00014d40: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-00014d50: 6728 2250 5454 204f 6666 2229 0a20 2020  g("PTT Off").   
-00014d60: 2020 2020 2069 6620 7365 6c66 2e72 6967       if self.rig
-00014d70: 5f63 6f6e 7472 6f6c 3a0a 2020 2020 2020  _control:.      
-00014d80: 2020 2020 2020 7365 6c66 2e6c 6566 7464        self.leftd
-00014d90: 6f74 2e73 6574 5069 786d 6170 2873 656c  ot.setPixmap(sel
-00014da0: 662e 7265 6464 6f74 290a 2020 2020 2020  f.reddot).      
-00014db0: 2020 2020 2020 6170 702e 7072 6f63 6573        app.proces
-00014dc0: 7345 7665 6e74 7328 290a 2020 2020 2020  sEvents().      
-00014dd0: 2020 2020 2020 7365 6c66 2e72 6967 5f63        self.rig_c
-00014de0: 6f6e 7472 6f6c 2e70 7474 5f6f 6666 2829  ontrol.ptt_off()
-00014df0: 0a0a 2020 2020 6465 6620 7072 6f63 6573  ..    def proces
-00014e00: 735f 6675 6e63 7469 6f6e 5f6b 6579 2873  s_function_key(s
-00014e10: 656c 662c 2066 756e 6374 696f 6e5f 6b65  elf, function_ke
-00014e20: 7929 202d 3e20 4e6f 6e65 3a0a 2020 2020  y) -> None:.    
-00014e30: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00014e40: 4361 6c6c 6564 2077 6865 6e20 6120 6675  Called when a fu
-00014e50: 6e63 7469 6f6e 206b 6579 2069 7320 636c  nction key is cl
-00014e60: 6963 6b65 642e 0a0a 2020 2020 2020 2020  icked...        
-00014e70: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
-00014e80: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-00014e90: 2020 2020 2020 6675 6e63 7469 6f6e 5f6b        function_k
-00014ea0: 6579 203a 2051 5075 7368 4275 7474 6f6e  ey : QPushButton
-00014eb0: 0a20 2020 2020 2020 2046 756e 6374 696f  .        Functio
-00014ec0: 6e20 6b65 7920 746f 2070 726f 6365 7373  n key to process
-00014ed0: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00014ee0: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
-00014ef0: 2d2d 0a20 2020 2020 2020 204e 6f6e 650a  --.        None.
-00014f00: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
-00014f10: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-00014f20: 6728 2246 756e 6374 696f 6e20 4b65 793a  g("Function Key:
-00014f30: 2025 7322 2c20 6675 6e63 7469 6f6e 5f6b   %s", function_k
-00014f40: 6579 2e74 6578 7428 2929 0a20 2020 2020  ey.text()).     
-00014f50: 2020 2069 6620 7365 6c66 2e6e 316d 6d3a     if self.n1mm:
-00014f60: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00014f70: 662e 6e31 6d6d 2e72 6164 696f 5f69 6e66  f.n1mm.radio_inf
-00014f80: 6f5b 2246 756e 6374 696f 6e4b 6579 4361  o["FunctionKeyCa
-00014f90: 7074 696f 6e22 5d20 3d20 6675 6e63 7469  ption"] = functi
-00014fa0: 6f6e 5f6b 6579 2e74 6578 7428 290a 2020  on_key.text().  
-00014fb0: 2020 2020 2020 6966 2073 656c 662e 7261        if self.ra
-00014fc0: 6469 6f5f 7374 6174 652e 6765 7428 226d  dio_state.get("m
-00014fd0: 6f64 6522 2920 696e 205b 224c 5342 222c  ode") in ["LSB",
-00014fe0: 2022 5553 4222 2c20 2253 5342 225d 3a0a   "USB", "SSB"]:.
-00014ff0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015000: 2e76 6f69 6365 5f73 7472 696e 6728 7365  .voice_string(se
-00015010: 6c66 2e70 726f 6365 7373 5f6d 6163 726f  lf.process_macro
-00015020: 2866 756e 6374 696f 6e5f 6b65 792e 746f  (function_key.to
-00015030: 6f6c 5469 7028 2929 290a 2020 2020 2020  olTip())).      
-00015040: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-00015050: 2020 2020 2069 6620 7365 6c66 2e63 773a       if self.cw:
-00015060: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00015070: 662e 6377 2e73 656e 6463 7728 7365 6c66  f.cw.sendcw(self
-00015080: 2e70 726f 6365 7373 5f6d 6163 726f 2866  .process_macro(f
-00015090: 756e 6374 696f 6e5f 6b65 792e 746f 6f6c  unction_key.tool
-000150a0: 5469 7028 2929 290a 0a20 2020 2064 6566  Tip()))..    def
-000150b0: 2072 756e 5f73 705f 6275 7474 6f6e 735f   run_sp_buttons_
-000150c0: 636c 6963 6b65 6428 7365 6c66 2920 2d3e  clicked(self) ->
-000150d0: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-000150e0: 2222 0a20 2020 2020 2020 2048 616e 646c  "".        Handl
-000150f0: 6520 5275 6e2f 5326 5020 6d6f 6465 2063  e Run/S&P mode c
-00015100: 6861 6e67 6573 2e0a 0a20 2020 2020 2020  hanges...       
-00015110: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-00015120: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-00015130: 2020 2020 2020 204e 6f6e 650a 0a20 2020         None..   
-00015140: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
-00015150: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
-00015160: 2020 2020 204e 6f6e 650a 2020 2020 2020       None.      
-00015170: 2020 2222 220a 2020 2020 2020 2020 7365    """.        se
-00015180: 6c66 2e70 7265 665b 2272 756e 5f73 7461  lf.pref["run_sta
-00015190: 7465 225d 203d 2073 656c 662e 7261 6469  te"] = self.radi
-000151a0: 6f42 7574 746f 6e5f 7275 6e2e 6973 4368  oButton_run.isCh
-000151b0: 6563 6b65 6428 290a 2020 2020 2020 2020  ecked().        
-000151c0: 7365 6c66 2e77 7269 7465 5f70 7265 6665  self.write_prefe
-000151d0: 7265 6e63 6528 290a 2020 2020 2020 2020  rence().        
-000151e0: 7365 6c66 2e72 6561 645f 6377 5f6d 6163  self.read_cw_mac
-000151f0: 726f 7328 290a 0a20 2020 2064 6566 2077  ros()..    def w
-00015200: 7269 7465 5f70 7265 6665 7265 6e63 6528  rite_preference(
-00015210: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
-00015220: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00015230: 2020 2057 7269 7465 2070 7265 6665 7265     Write prefere
-00015240: 6e63 6573 2074 6f20 6669 6c65 2e0a 0a20  nces to file... 
-00015250: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+000132b0: 0a20 2020 2020 2020 204e 6f6e 650a 2020  .        None.  
+000132c0: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
+000132d0: 2020 2063 7320 3d20 7365 6c66 2e73 6574     cs = self.set
+000132e0: 7469 6e67 735f 6469 616c 6f67 2e43 616c  tings_dialog.Cal
+000132f0: 6c2e 7465 7874 2829 0a20 2020 2020 2020  l.text().       
+00013300: 2073 656c 662e 7374 6174 696f 6e20 3d20   self.station = 
+00013310: 7b7d 0a20 2020 2020 2020 2073 656c 662e  {}.        self.
+00013320: 7374 6174 696f 6e5b 2243 616c 6c22 5d20  station["Call"] 
+00013330: 3d20 6373 2e75 7070 6572 2829 0a20 2020  = cs.upper().   
+00013340: 2020 2020 2073 656c 662e 7374 6174 696f       self.statio
+00013350: 6e5b 224e 616d 6522 5d20 3d20 7365 6c66  n["Name"] = self
+00013360: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+00013370: 2e4e 616d 652e 7465 7874 2829 2e74 6974  .Name.text().tit
+00013380: 6c65 2829 0a20 2020 2020 2020 2073 656c  le().        sel
+00013390: 662e 7374 6174 696f 6e5b 2253 7472 6565  f.station["Stree
+000133a0: 7431 225d 203d 2073 656c 662e 7365 7474  t1"] = self.sett
+000133b0: 696e 6773 5f64 6961 6c6f 672e 4164 6472  ings_dialog.Addr
+000133c0: 6573 7331 2e74 6578 7428 292e 7469 746c  ess1.text().titl
+000133d0: 6528 290a 2020 2020 2020 2020 7365 6c66  e().        self
+000133e0: 2e73 7461 7469 6f6e 5b22 5374 7265 6574  .station["Street
+000133f0: 3222 5d20 3d20 7365 6c66 2e73 6574 7469  2"] = self.setti
+00013400: 6e67 735f 6469 616c 6f67 2e41 6464 7265  ngs_dialog.Addre
+00013410: 7373 322e 7465 7874 2829 2e74 6974 6c65  ss2.text().title
+00013420: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+00013430: 7374 6174 696f 6e5b 2243 6974 7922 5d20  station["City"] 
+00013440: 3d20 7365 6c66 2e73 6574 7469 6e67 735f  = self.settings_
+00013450: 6469 616c 6f67 2e43 6974 792e 7465 7874  dialog.City.text
+00013460: 2829 2e74 6974 6c65 2829 0a20 2020 2020  ().title().     
+00013470: 2020 2073 656c 662e 7374 6174 696f 6e5b     self.station[
+00013480: 2253 7461 7465 225d 203d 2073 656c 662e  "State"] = self.
+00013490: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
+000134a0: 5374 6174 652e 7465 7874 2829 2e75 7070  State.text().upp
+000134b0: 6572 2829 0a20 2020 2020 2020 2073 656c  er().        sel
+000134c0: 662e 7374 6174 696f 6e5b 225a 6970 225d  f.station["Zip"]
+000134d0: 203d 2073 656c 662e 7365 7474 696e 6773   = self.settings
+000134e0: 5f64 6961 6c6f 672e 5a69 702e 7465 7874  _dialog.Zip.text
+000134f0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+00013500: 7374 6174 696f 6e5b 2243 6f75 6e74 7279  station["Country
+00013510: 225d 203d 2073 656c 662e 7365 7474 696e  "] = self.settin
+00013520: 6773 5f64 6961 6c6f 672e 436f 756e 7472  gs_dialog.Countr
+00013530: 792e 7465 7874 2829 2e74 6974 6c65 2829  y.text().title()
+00013540: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
+00013550: 6174 696f 6e5b 2247 7269 6453 7175 6172  ation["GridSquar
+00013560: 6522 5d20 3d20 7365 6c66 2e73 6574 7469  e"] = self.setti
+00013570: 6e67 735f 6469 616c 6f67 2e47 7269 6453  ngs_dialog.GridS
+00013580: 7175 6172 652e 7465 7874 2829 0a20 2020  quare.text().   
+00013590: 2020 2020 2073 656c 662e 7374 6174 696f       self.statio
+000135a0: 6e5b 2243 515a 6f6e 6522 5d20 3d20 7365  n["CQZone"] = se
+000135b0: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
+000135c0: 6f67 2e43 515a 6f6e 652e 7465 7874 2829  og.CQZone.text()
+000135d0: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
+000135e0: 6174 696f 6e5b 2249 4152 555a 6f6e 6522  ation["IARUZone"
+000135f0: 5d20 3d20 7365 6c66 2e73 6574 7469 6e67  ] = self.setting
+00013600: 735f 6469 616c 6f67 2e49 5455 5a6f 6e65  s_dialog.ITUZone
+00013610: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
+00013620: 7365 6c66 2e73 7461 7469 6f6e 5b22 4c69  self.station["Li
+00013630: 6365 6e73 6543 6c61 7373 225d 203d 2073  censeClass"] = s
+00013640: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
+00013650: 6c6f 672e 4c69 6365 6e73 652e 7465 7874  log.License.text
+00013660: 2829 2e74 6974 6c65 2829 0a20 2020 2020  ().title().     
+00013670: 2020 2073 656c 662e 7374 6174 696f 6e5b     self.station[
+00013680: 224c 6174 6974 7564 6522 5d20 3d20 7365  "Latitude"] = se
+00013690: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
+000136a0: 6f67 2e4c 6174 6974 7564 652e 7465 7874  og.Latitude.text
+000136b0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+000136c0: 7374 6174 696f 6e5b 224c 6f6e 6769 7475  station["Longitu
+000136d0: 6465 225d 203d 2073 656c 662e 7365 7474  de"] = self.sett
+000136e0: 696e 6773 5f64 6961 6c6f 672e 4c6f 6e67  ings_dialog.Long
+000136f0: 6974 7564 652e 7465 7874 2829 0a20 2020  itude.text().   
+00013700: 2020 2020 2073 656c 662e 7374 6174 696f       self.statio
+00013710: 6e5b 2253 5458 6571 225d 203d 2073 656c  n["STXeq"] = sel
+00013720: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
+00013730: 672e 5374 6174 696f 6e54 5852 582e 7465  g.StationTXRX.te
+00013740: 7874 2829 0a20 2020 2020 2020 2073 656c  xt().        sel
+00013750: 662e 7374 6174 696f 6e5b 2253 506f 7765  f.station["SPowe
+00013760: 225d 203d 2073 656c 662e 7365 7474 696e  "] = self.settin
+00013770: 6773 5f64 6961 6c6f 672e 506f 7765 722e  gs_dialog.Power.
+00013780: 7465 7874 2829 0a20 2020 2020 2020 2073  text().        s
+00013790: 656c 662e 7374 6174 696f 6e5b 2253 416e  elf.station["SAn
+000137a0: 7465 225d 203d 2073 656c 662e 7365 7474  te"] = self.sett
+000137b0: 696e 6773 5f64 6961 6c6f 672e 416e 7465  ings_dialog.Ante
+000137c0: 6e6e 612e 7465 7874 2829 0a20 2020 2020  nna.text().     
+000137d0: 2020 2073 656c 662e 7374 6174 696f 6e5b     self.station[
+000137e0: 2253 416e 7448 3122 5d20 3d20 7365 6c66  "SAntH1"] = self
+000137f0: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+00013800: 2e41 6e74 4865 6967 6874 2e74 6578 7428  .AntHeight.text(
+00013810: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+00013820: 7461 7469 6f6e 5b22 5341 6e74 4832 225d  tation["SAntH2"]
+00013830: 203d 2073 656c 662e 7365 7474 696e 6773   = self.settings
+00013840: 5f64 6961 6c6f 672e 4153 4c2e 7465 7874  _dialog.ASL.text
+00013850: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+00013860: 7374 6174 696f 6e5b 2241 5252 4c53 6563  station["ARRLSec
+00013870: 7469 6f6e 225d 203d 2073 656c 662e 7365  tion"] = self.se
+00013880: 7474 696e 6773 5f64 6961 6c6f 672e 4152  ttings_dialog.AR
+00013890: 524c 5365 6374 696f 6e2e 7465 7874 2829  RLSection.text()
+000138a0: 2e75 7070 6572 2829 0a20 2020 2020 2020  .upper().       
+000138b0: 2073 656c 662e 7374 6174 696f 6e5b 2252   self.station["R
+000138c0: 6f76 6572 5154 4822 5d20 3d20 7365 6c66  overQTH"] = self
+000138d0: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+000138e0: 2e52 6f76 6572 5154 482e 7465 7874 2829  .RoverQTH.text()
+000138f0: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
+00013900: 6174 696f 6e5b 2243 6c75 6222 5d20 3d20  ation["Club"] = 
+00013910: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
+00013920: 616c 6f67 2e43 6c75 622e 7465 7874 2829  alog.Club.text()
+00013930: 2e74 6974 6c65 2829 0a20 2020 2020 2020  .title().       
+00013940: 2073 656c 662e 7374 6174 696f 6e5b 2245   self.station["E
+00013950: 6d61 696c 225d 203d 2073 656c 662e 7365  mail"] = self.se
+00013960: 7474 696e 6773 5f64 6961 6c6f 672e 456d  ttings_dialog.Em
+00013970: 6169 6c2e 7465 7874 2829 0a20 2020 2020  ail.text().     
+00013980: 2020 2073 656c 662e 6461 7461 6261 7365     self.database
+00013990: 2e61 6464 5f73 7461 7469 6f6e 2873 656c  .add_station(sel
+000139a0: 662e 7374 6174 696f 6e29 0a20 2020 2020  f.station).     
+000139b0: 2020 2073 656c 662e 7365 7474 696e 6773     self.settings
+000139c0: 5f64 6961 6c6f 672e 636c 6f73 6528 290a  _dialog.close().
+000139d0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000139e0: 6375 7272 656e 745f 6f70 203d 3d20 2222  current_op == ""
+000139f0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00013a00: 6c66 2e63 7572 7265 6e74 5f6f 7020 3d20  lf.current_op = 
+00013a10: 7365 6c66 2e73 7461 7469 6f6e 2e67 6574  self.station.get
+00013a20: 2822 4361 6c6c 222c 2022 2229 0a20 2020  ("Call", "").   
+00013a30: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
+00013a40: 6b65 5f6f 705f 6469 7228 290a 2020 2020  ke_op_dir().    
+00013a50: 2020 2020 636f 6e74 6573 745f 636f 756e      contest_coun
+00013a60: 7420 3d20 7365 6c66 2e64 6174 6162 6173  t = self.databas
+00013a70: 652e 6665 7463 685f 616c 6c5f 636f 6e74  e.fetch_all_cont
+00013a80: 6573 7473 2829 0a20 2020 2020 2020 2069  ests().        i
+00013a90: 6620 6c65 6e28 636f 6e74 6573 745f 636f  f len(contest_co
+00013aa0: 756e 7429 203d 3d20 303a 0a20 2020 2020  unt) == 0:.     
+00013ab0: 2020 2020 2020 2073 656c 662e 6e65 775f         self.new_
+00013ac0: 636f 6e74 6573 745f 6469 616c 6f67 2829  contest_dialog()
+00013ad0: 0a0a 2020 2020 6465 6620 6564 6974 5f6d  ..    def edit_m
+00013ae0: 6163 726f 2873 656c 662c 2066 756e 6374  acro(self, funct
+00013af0: 696f 6e5f 6b65 7929 202d 3e20 4e6f 6e65  ion_key) -> None
+00013b00: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00013b10: 2020 2020 2020 5368 6f77 2065 6469 7420        Show edit 
+00013b20: 6d61 6372 6f20 6469 616c 6f67 2066 6f72  macro dialog for
+00013b30: 2066 756e 6374 696f 6e20 6b65 792e 0a0a   function key...
+00013b40: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+00013b50: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
+00013b60: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6675  -----.        fu
+00013b70: 6e63 7469 6f6e 5f6b 6579 203a 2073 7472  nction_key : str
+00013b80: 0a20 2020 2020 2020 2046 756e 6374 696f  .        Functio
+00013b90: 6e20 6b65 7920 746f 2065 6469 742e 0a0a  n key to edit...
+00013ba0: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
+00013bb0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
+00013bc0: 2020 2020 2020 2020 4e6f 6e65 0a20 2020          None.   
+00013bd0: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+00013be0: 2020 7365 6c66 2e65 6469 745f 6d61 6372    self.edit_macr
+00013bf0: 6f5f 6469 616c 6f67 203d 2045 6469 744d  o_dialog = EditM
+00013c00: 6163 726f 2866 756e 6374 696f 6e5f 6b65  acro(function_ke
+00013c10: 792c 2066 7375 7469 6c73 2e41 5050 5f44  y, fsutils.APP_D
+00013c20: 4154 415f 5041 5448 290a 0a20 2020 2020  ATA_PATH)..     
+00013c30: 2020 2069 6620 7365 6c66 2e63 7572 7265     if self.curre
+00013c40: 6e74 5f70 616c 6574 7465 3a0a 2020 2020  nt_palette:.    
+00013c50: 2020 2020 2020 2020 7365 6c66 2e65 6469          self.edi
+00013c60: 745f 6d61 6372 6f5f 6469 616c 6f67 2e73  t_macro_dialog.s
+00013c70: 6574 5061 6c65 7474 6528 7365 6c66 2e63  etPalette(self.c
+00013c80: 7572 7265 6e74 5f70 616c 6574 7465 290a  urrent_palette).
+00013c90: 0a20 2020 2020 2020 2073 656c 662e 6564  .        self.ed
+00013ca0: 6974 5f6d 6163 726f 5f64 6961 6c6f 672e  it_macro_dialog.
+00013cb0: 6163 6365 7074 6564 2e63 6f6e 6e65 6374  accepted.connect
+00013cc0: 2873 656c 662e 6564 6974 6564 5f6d 6163  (self.edited_mac
+00013cd0: 726f 290a 2020 2020 2020 2020 7365 6c66  ro).        self
+00013ce0: 2e65 6469 745f 6d61 6372 6f5f 6469 616c  .edit_macro_dial
+00013cf0: 6f67 2e6f 7065 6e28 290a 0a20 2020 2064  og.open()..    d
+00013d00: 6566 2065 6469 7465 645f 6d61 6372 6f28  ef edited_macro(
+00013d10: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
+00013d20: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00013d30: 2020 2053 6176 6520 6564 6974 6564 206d     Save edited m
+00013d40: 6163 726f 2074 6f20 6461 7461 6261 7365  acro to database
+00013d50: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+00013d60: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
+00013d70: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+00013d80: 204e 6f6e 650a 0a20 2020 2020 2020 2052   None..        R
+00013d90: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
+00013da0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 204e  ------.        N
+00013db0: 6f6e 650a 2020 2020 2020 2020 2222 220a  one.        """.
+00013dc0: 0a20 2020 2020 2020 2073 656c 662e 6564  .        self.ed
+00013dd0: 6974 5f6d 6163 726f 5f64 6961 6c6f 672e  it_macro_dialog.
+00013de0: 6675 6e63 7469 6f6e 5f6b 6579 2e73 6574  function_key.set
+00013df0: 5465 7874 280a 2020 2020 2020 2020 2020  Text(.          
+00013e00: 2020 7365 6c66 2e65 6469 745f 6d61 6372    self.edit_macr
+00013e10: 6f5f 6469 616c 6f67 2e6d 6163 726f 5f6c  o_dialog.macro_l
+00013e20: 6162 656c 2e74 6578 7428 290a 2020 2020  abel.text().    
+00013e30: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
+00013e40: 6c66 2e65 6469 745f 6d61 6372 6f5f 6469  lf.edit_macro_di
+00013e50: 616c 6f67 2e66 756e 6374 696f 6e5f 6b65  alog.function_ke
+00013e60: 792e 7365 7454 6f6f 6c54 6970 280a 2020  y.setToolTip(.  
+00013e70: 2020 2020 2020 2020 2020 7365 6c66 2e65            self.e
+00013e80: 6469 745f 6d61 6372 6f5f 6469 616c 6f67  dit_macro_dialog
+00013e90: 2e74 6865 5f6d 6163 726f 2e74 6578 7428  .the_macro.text(
+00013ea0: 290a 2020 2020 2020 2020 290a 2020 2020  ).        ).    
+00013eb0: 2020 2020 7365 6c66 2e65 6469 745f 6d61      self.edit_ma
+00013ec0: 6372 6f5f 6469 616c 6f67 2e63 6c6f 7365  cro_dialog.close
+00013ed0: 2829 0a0a 2020 2020 6465 6620 7072 6f63  ()..    def proc
+00013ee0: 6573 735f 6d61 6372 6f28 7365 6c66 2c20  ess_macro(self, 
+00013ef0: 6d61 6372 6f3a 2073 7472 2920 2d3e 2073  macro: str) -> s
+00013f00: 7472 3a0a 2020 2020 2020 2020 2222 220a  tr:.        """.
+00013f10: 2020 2020 2020 2020 5072 6f63 6573 7320          Process 
+00013f20: 4357 206d 6163 726f 2073 7562 7374 6974  CW macro substit
+00013f30: 7574 696f 6e73 2066 6f72 2063 6f6e 7465  utions for conte
+00013f40: 7374 2e0a 0a20 2020 2020 2020 2050 6172  st...        Par
+00013f50: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
+00013f60: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+00013f70: 2020 206d 6163 726f 203a 2073 7472 0a20     macro : str. 
+00013f80: 2020 2020 2020 204d 6163 726f 2074 6f20         Macro to 
+00013f90: 7072 6f63 6573 732e 0a0a 2020 2020 2020  process...      
+00013fa0: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
+00013fb0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+00013fc0: 2020 7374 720a 2020 2020 2020 2020 5072    str.        Pr
+00013fd0: 6f63 6573 7365 6420 6d61 6372 6f2e 0a20  ocessed macro.. 
+00013fe0: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
+00013ff0: 2020 2020 7265 7375 6c74 203d 2073 656c      result = sel
+00014000: 662e 6461 7461 6261 7365 2e67 6574 5f73  f.database.get_s
+00014010: 6572 6961 6c28 290a 2020 2020 2020 2020  erial().        
+00014020: 6e65 7874 5f73 6572 6961 6c20 3d20 7374  next_serial = st
+00014030: 7228 7265 7375 6c74 2e67 6574 2822 7365  r(result.get("se
+00014040: 7269 616c 5f6e 7222 2c20 2231 2229 290a  rial_nr", "1")).
+00014050: 2020 2020 2020 2020 6966 206e 6578 745f          if next_
+00014060: 7365 7269 616c 203d 3d20 224e 6f6e 6522  serial == "None"
+00014070: 3a0a 2020 2020 2020 2020 2020 2020 6e65  :.            ne
+00014080: 7874 5f73 6572 6961 6c20 3d20 2231 220a  xt_serial = "1".
+00014090: 2020 2020 2020 2020 6d61 6372 6f20 3d20          macro = 
+000140a0: 6d61 6372 6f2e 7570 7065 7228 290a 2020  macro.upper().  
+000140b0: 2020 2020 2020 6d61 6372 6f20 3d20 6d61        macro = ma
+000140c0: 6372 6f2e 7265 706c 6163 6528 2223 222c  cro.replace("#",
+000140d0: 206e 6578 745f 7365 7269 616c 290a 2020   next_serial).  
+000140e0: 2020 2020 2020 6d61 6372 6f20 3d20 6d61        macro = ma
+000140f0: 6372 6f2e 7265 706c 6163 6528 227b 4d59  cro.replace("{MY
+00014100: 4341 4c4c 7d22 2c20 7365 6c66 2e73 7461  CALL}", self.sta
+00014110: 7469 6f6e 2e67 6574 2822 4361 6c6c 222c  tion.get("Call",
+00014120: 2022 2229 290a 2020 2020 2020 2020 6d61   "")).        ma
+00014130: 6372 6f20 3d20 6d61 6372 6f2e 7265 706c  cro = macro.repl
+00014140: 6163 6528 227b 4849 5343 414c 4c7d 222c  ace("{HISCALL}",
+00014150: 2073 656c 662e 6361 6c6c 7369 676e 2e74   self.callsign.t
+00014160: 6578 7428 2929 0a20 2020 2020 2020 2069  ext()).        i
+00014170: 6620 7365 6c66 2e72 6164 696f 5f73 7461  f self.radio_sta
+00014180: 7465 2e67 6574 2822 6d6f 6465 2229 203d  te.get("mode") =
+00014190: 3d20 2243 5722 3a0a 2020 2020 2020 2020  = "CW":.        
+000141a0: 2020 2020 6d61 6372 6f20 3d20 6d61 6372      macro = macr
+000141b0: 6f2e 7265 706c 6163 6528 227b 534e 547d  o.replace("{SNT}
+000141c0: 222c 2073 656c 662e 7365 6e74 2e74 6578  ", self.sent.tex
+000141d0: 7428 292e 7265 706c 6163 6528 2239 222c  t().replace("9",
+000141e0: 2022 6e22 2929 0a20 2020 2020 2020 2065   "n")).        e
+000141f0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00014200: 206d 6163 726f 203d 206d 6163 726f 2e72   macro = macro.r
+00014210: 6570 6c61 6365 2822 7b53 4e54 7d22 2c20  eplace("{SNT}", 
+00014220: 7365 6c66 2e73 656e 742e 7465 7874 2829  self.sent.text()
+00014230: 290a 2020 2020 2020 2020 6d61 6372 6f20  ).        macro 
+00014240: 3d20 6d61 6372 6f2e 7265 706c 6163 6528  = macro.replace(
+00014250: 227b 5345 4e54 4e52 7d22 2c20 7365 6c66  "{SENTNR}", self
+00014260: 2e6f 7468 6572 5f31 2e74 6578 7428 2929  .other_1.text())
+00014270: 0a20 2020 2020 2020 206d 6163 726f 203d  .        macro =
+00014280: 206d 6163 726f 2e72 6570 6c61 6365 280a   macro.replace(.
+00014290: 2020 2020 2020 2020 2020 2020 227b 4558              "{EX
+000142a0: 4348 7d22 2c20 7365 6c66 2e63 6f6e 7465  CH}", self.conte
+000142b0: 7374 5f73 6574 7469 6e67 732e 6765 7428  st_settings.get(
+000142c0: 2253 656e 7445 7863 6861 6e67 6522 2c20  "SentExchange", 
+000142d0: 2278 7878 2229 0a20 2020 2020 2020 2029  "xxx").        )
+000142e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000142f0: 6d61 6372 6f0a 0a20 2020 2064 6566 2076  macro..    def v
+00014300: 6f69 6365 5f73 7472 696e 6728 7365 6c66  oice_string(self
+00014310: 2c20 7468 655f 7374 7269 6e67 3a20 7374  , the_string: st
+00014320: 7229 202d 3e20 4e6f 6e65 3a0a 2020 2020  r) -> None:.    
+00014330: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00014340: 766f 6963 6573 2073 7472 696e 6720 7573  voices string us
+00014350: 696e 6720 6e61 746f 2070 686f 6e65 7469  ing nato phoneti
+00014360: 6373 2e0a 0a20 2020 2020 2020 2050 6172  cs...        Par
+00014370: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
+00014380: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+00014390: 2020 2074 6865 5f73 7472 696e 6720 3a20     the_string : 
+000143a0: 7374 720a 2020 2020 2020 2020 5374 7269  str.        Stri
+000143b0: 6e67 2074 6f20 766f 6963 6966 792e 0a0a  ng to voicify...
+000143c0: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
+000143d0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
+000143e0: 2020 2020 2020 2020 4e6f 6e65 0a20 2020          None.   
+000143f0: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+00014400: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
+00014410: 566f 6963 696e 673a 2025 7322 2c20 7468  Voicing: %s", th
+00014420: 655f 7374 7269 6e67 290a 2020 2020 2020  e_string).      
+00014430: 2020 6f70 5f70 6174 6820 3d20 6673 7574    op_path = fsut
+00014440: 696c 732e 5553 4552 5f44 4154 415f 5041  ils.USER_DATA_PA
+00014450: 5448 202f 2073 656c 662e 6375 7272 656e  TH / self.curren
+00014460: 745f 6f70 0a20 2020 2020 2020 2069 6620  t_op.        if 
+00014470: 225b 2220 696e 2074 6865 5f73 7472 696e  "[" in the_strin
+00014480: 673a 0a20 2020 2020 2020 2020 2020 2073  g:.            s
+00014490: 7562 5f73 7472 696e 6720 3d20 7468 655f  ub_string = the_
+000144a0: 7374 7269 6e67 2e73 7472 6970 2822 5b5d  string.strip("[]
+000144b0: 2229 2e6c 6f77 6572 2829 0a20 2020 2020  ").lower().     
+000144c0: 2020 2020 2020 2066 696c 656e 616d 6520         filename 
+000144d0: 3d20 6622 7b73 7472 286f 705f 7061 7468  = f"{str(op_path
+000144e0: 297d 2f7b 7375 625f 7374 7269 6e67 7d2e  )}/{sub_string}.
+000144f0: 7761 7622 0a20 2020 2020 2020 2020 2020  wav".           
+00014500: 2069 6620 5061 7468 2866 696c 656e 616d   if Path(filenam
+00014510: 6529 2e69 735f 6669 6c65 2829 3a0a 2020  e).is_file():.  
+00014520: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00014530: 6767 6572 2e64 6562 7567 2822 566f 6963  gger.debug("Voic
+00014540: 696e 673a 2025 7322 2c20 6669 6c65 6e61  ing: %s", filena
+00014550: 6d65 290a 2020 2020 2020 2020 2020 2020  me).            
+00014560: 2020 2020 6461 7461 2c20 5f66 7320 3d20      data, _fs = 
+00014570: 7366 2e72 6561 6428 6669 6c65 6e61 6d65  sf.read(filename
+00014580: 2c20 6474 7970 653d 2266 6c6f 6174 3332  , dtype="float32
+00014590: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+000145a0: 2020 2073 656c 662e 7074 745f 6f6e 2829     self.ptt_on()
+000145b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000145c0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+000145d0: 2020 2020 2020 2020 2020 7364 2e64 6566            sd.def
+000145e0: 6175 6c74 2e64 6576 6963 6520 3d20 7365  ault.device = se
+000145f0: 6c66 2e70 7265 662e 6765 7428 2273 6f75  lf.pref.get("sou
+00014600: 6e64 6465 7669 6365 222c 2022 6465 6661  nddevice", "defa
+00014610: 756c 7422 290a 2020 2020 2020 2020 2020  ult").          
+00014620: 2020 2020 2020 2020 2020 7364 2e64 6566            sd.def
+00014630: 6175 6c74 2e73 616d 706c 6572 6174 6520  ault.samplerate 
+00014640: 3d20 3434 3130 302e 300a 2020 2020 2020  = 44100.0.      
+00014650: 2020 2020 2020 2020 2020 2020 2020 7364                sd
+00014660: 2e70 6c61 7928 6461 7461 2c20 626c 6f63  .play(data, bloc
+00014670: 6b69 6e67 3d46 616c 7365 290a 2020 2020  king=False).    
+00014680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014690: 2320 5f73 7461 7475 7320 3d20 7364 2e77  # _status = sd.w
+000146a0: 6169 7428 290a 2020 2020 2020 2020 2020  ait().          
+000146b0: 2020 2020 2020 2020 2020 2320 6874 7470            # http
+000146c0: 733a 2f2f 736e 796b 2e69 6f2f 6164 7669  s://snyk.io/advi
+000146d0: 736f 722f 7079 7468 6f6e 2f73 6f75 6e64  sor/python/sound
+000146e0: 6465 7669 6365 2f66 756e 6374 696f 6e73  device/functions
+000146f0: 2f73 6f75 6e64 6465 7669 6365 2e50 6f72  /sounddevice.Por
+00014700: 7441 7564 696f 4572 726f 720a 2020 2020  tAudioError.    
+00014710: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+00014720: 7074 2073 642e 506f 7274 4175 6469 6f45  pt sd.PortAudioE
+00014730: 7272 6f72 2061 7320 6572 723a 0a20 2020  rror as err:.   
+00014740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014750: 206c 6f67 6765 722e 7761 726e 696e 6728   logger.warning(
+00014760: 2225 7322 2c20 6622 7b65 7272 7d22 290a  "%s", f"{err}").
+00014770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014780: 2073 656c 662e 7074 745f 6f66 6628 290a   self.ptt_off().
+00014790: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000147a0: 726e 0a20 2020 2020 2020 2073 656c 662e  rn.        self.
+000147b0: 7074 745f 6f6e 2829 0a20 2020 2020 2020  ptt_on().       
+000147c0: 2066 6f72 206c 6574 7465 7220 696e 2074   for letter in t
+000147d0: 6865 5f73 7472 696e 672e 6c6f 7765 7228  he_string.lower(
+000147e0: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
+000147f0: 6620 6c65 7474 6572 2069 6e20 2261 6263  f letter in "abc
+00014800: 6465 6667 6869 6a6b 6c6d 6e6f 7071 7273  defghijklmnopqrs
+00014810: 7475 7677 7879 7a20 3132 3334 3536 3738  tuvwxyz 12345678
+00014820: 3930 223a 0a20 2020 2020 2020 2020 2020  90":.           
+00014830: 2020 2020 2069 6620 6c65 7474 6572 203d       if letter =
+00014840: 3d20 2220 223a 0a20 2020 2020 2020 2020  = " ":.         
+00014850: 2020 2020 2020 2020 2020 206c 6574 7465             lette
+00014860: 7220 3d20 2273 7061 6365 220a 2020 2020  r = "space".    
+00014870: 2020 2020 2020 2020 2020 2020 6669 6c65              file
+00014880: 6e61 6d65 203d 2066 227b 7374 7228 6f70  name = f"{str(op
+00014890: 5f70 6174 6829 7d2f 7b6c 6574 7465 727d  _path)}/{letter}
+000148a0: 2e77 6176 220a 2020 2020 2020 2020 2020  .wav".          
+000148b0: 2020 2020 2020 6966 2050 6174 6828 6669        if Path(fi
+000148c0: 6c65 6e61 6d65 292e 6973 5f66 696c 6528  lename).is_file(
+000148d0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000148e0: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+000148f0: 6275 6728 2256 6f69 6369 6e67 3a20 2573  bug("Voicing: %s
+00014900: 222c 2066 696c 656e 616d 6529 0a20 2020  ", filename).   
+00014910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014920: 2064 6174 612c 205f 6673 203d 2073 662e   data, _fs = sf.
+00014930: 7265 6164 2866 696c 656e 616d 652c 2064  read(filename, d
+00014940: 7479 7065 3d22 666c 6f61 7433 3222 290a  type="float32").
+00014950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014960: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+00014970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014980: 2073 642e 6465 6661 756c 742e 6465 7669   sd.default.devi
+00014990: 6365 203d 2073 656c 662e 7072 6566 2e67  ce = self.pref.g
+000149a0: 6574 2822 736f 756e 6464 6576 6963 6522  et("sounddevice"
+000149b0: 2c20 2264 6566 6175 6c74 2229 0a20 2020  , "default").   
+000149c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000149d0: 2020 2020 2073 642e 6465 6661 756c 742e       sd.default.
+000149e0: 7361 6d70 6c65 7261 7465 203d 2034 3431  samplerate = 441
+000149f0: 3030 2e30 0a20 2020 2020 2020 2020 2020  00.0.           
+00014a00: 2020 2020 2020 2020 2020 2020 2073 642e               sd.
+00014a10: 706c 6179 2864 6174 612c 2062 6c6f 636b  play(data, block
+00014a20: 696e 673d 4661 6c73 6529 0a20 2020 2020  ing=False).     
+00014a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014a40: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+00014a50: 2225 7322 2c20 6622 7b73 642e 7761 6974  "%s", f"{sd.wait
+00014a60: 2829 7d22 290a 2020 2020 2020 2020 2020  ()}").          
+00014a70: 2020 2020 2020 2020 2020 6578 6365 7074            except
+00014a80: 2073 642e 506f 7274 4175 6469 6f45 7272   sd.PortAudioErr
+00014a90: 6f72 2061 7320 6572 723a 0a20 2020 2020  or as err:.     
+00014aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ab0: 2020 206c 6f67 6765 722e 7761 726e 696e     logger.warnin
+00014ac0: 6728 2225 7322 2c20 6622 7b65 7272 7d22  g("%s", f"{err}"
+00014ad0: 290a 2020 2020 2020 2020 7365 6c66 2e70  ).        self.p
+00014ae0: 7474 5f6f 6666 2829 0a0a 2020 2020 6465  tt_off()..    de
+00014af0: 6620 7074 745f 6f6e 2873 656c 6629 202d  f ptt_on(self) -
+00014b00: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00014b10: 2222 220a 2020 2020 2020 2020 5475 726e  """.        Turn
+00014b20: 206f 6e20 7074 7420 666f 7220 7269 672e   on ptt for rig.
+00014b30: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+00014b40: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
+00014b50: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00014b60: 4e6f 6e65 0a0a 2020 2020 2020 2020 5265  None..        Re
+00014b70: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
+00014b80: 2d2d 2d2d 2d0a 2020 2020 2020 2020 4e6f  -----.        No
+00014b90: 6e65 0a20 2020 2020 2020 2022 2222 0a0a  ne.        """..
+00014ba0: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+00014bb0: 6562 7567 2822 5054 5420 4f6e 2229 0a20  ebug("PTT On"). 
+00014bc0: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+00014bd0: 6967 5f63 6f6e 7472 6f6c 3a0a 2020 2020  ig_control:.    
+00014be0: 2020 2020 2020 2020 7365 6c66 2e6c 6566          self.lef
+00014bf0: 7464 6f74 2e73 6574 5069 786d 6170 2873  tdot.setPixmap(s
+00014c00: 656c 662e 6772 6565 6e64 6f74 290a 2020  elf.greendot).  
+00014c10: 2020 2020 2020 2020 2020 6170 702e 7072            app.pr
+00014c20: 6f63 6573 7345 7665 6e74 7328 290a 2020  ocessEvents().  
+00014c30: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+00014c40: 6967 5f63 6f6e 7472 6f6c 2e70 7474 5f6f  ig_control.ptt_o
+00014c50: 6e28 290a 0a20 2020 2064 6566 2070 7474  n()..    def ptt
+00014c60: 5f6f 6666 2873 656c 6629 202d 3e20 4e6f  _off(self) -> No
+00014c70: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
+00014c80: 2020 2020 2020 2020 5475 726e 206f 6666          Turn off
+00014c90: 2070 7474 2066 6f72 2072 6967 2e0a 0a20   ptt for rig... 
+00014ca0: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+00014cb0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+00014cc0: 2d2d 2d2d 0a20 2020 2020 2020 204e 6f6e  ----.        Non
+00014cd0: 650a 0a20 2020 2020 2020 2052 6574 7572  e..        Retur
+00014ce0: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
+00014cf0: 2d2d 0a20 2020 2020 2020 204e 6f6e 650a  --.        None.
+00014d00: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00014d10: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+00014d20: 2822 5054 5420 4f66 6622 290a 2020 2020  ("PTT Off").    
+00014d30: 2020 2020 6966 2073 656c 662e 7269 675f      if self.rig_
+00014d40: 636f 6e74 726f 6c3a 0a20 2020 2020 2020  control:.       
+00014d50: 2020 2020 2073 656c 662e 6c65 6674 646f       self.leftdo
+00014d60: 742e 7365 7450 6978 6d61 7028 7365 6c66  t.setPixmap(self
+00014d70: 2e72 6564 646f 7429 0a20 2020 2020 2020  .reddot).       
+00014d80: 2020 2020 2061 7070 2e70 726f 6365 7373       app.process
+00014d90: 4576 656e 7473 2829 0a20 2020 2020 2020  Events().       
+00014da0: 2020 2020 2073 656c 662e 7269 675f 636f       self.rig_co
+00014db0: 6e74 726f 6c2e 7074 745f 6f66 6628 290a  ntrol.ptt_off().
+00014dc0: 0a20 2020 2064 6566 2070 726f 6365 7373  .    def process
+00014dd0: 5f66 756e 6374 696f 6e5f 6b65 7928 7365  _function_key(se
+00014de0: 6c66 2c20 6675 6e63 7469 6f6e 5f6b 6579  lf, function_key
+00014df0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00014e00: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
+00014e10: 616c 6c65 6420 7768 656e 2061 2066 756e  alled when a fun
+00014e20: 6374 696f 6e20 6b65 7920 6973 2063 6c69  ction key is cli
+00014e30: 636b 6564 2e0a 0a20 2020 2020 2020 2050  cked...        P
+00014e40: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+00014e50: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+00014e60: 2020 2020 2066 756e 6374 696f 6e5f 6b65       function_ke
+00014e70: 7920 3a20 5150 7573 6842 7574 746f 6e0a  y : QPushButton.
+00014e80: 2020 2020 2020 2020 4675 6e63 7469 6f6e          Function
+00014e90: 206b 6579 2074 6f20 7072 6f63 6573 732e   key to process.
+00014ea0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00014eb0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+00014ec0: 2d0a 2020 2020 2020 2020 4e6f 6e65 0a20  -.        None. 
+00014ed0: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
+00014ee0: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+00014ef0: 2822 4675 6e63 7469 6f6e 204b 6579 3a20  ("Function Key: 
+00014f00: 2573 222c 2066 756e 6374 696f 6e5f 6b65  %s", function_ke
+00014f10: 792e 7465 7874 2829 290a 2020 2020 2020  y.text()).      
+00014f20: 2020 6966 2073 656c 662e 6e31 6d6d 3a0a    if self.n1mm:.
+00014f30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00014f40: 2e6e 316d 6d2e 7261 6469 6f5f 696e 666f  .n1mm.radio_info
+00014f50: 5b22 4675 6e63 7469 6f6e 4b65 7943 6170  ["FunctionKeyCap
+00014f60: 7469 6f6e 225d 203d 2066 756e 6374 696f  tion"] = functio
+00014f70: 6e5f 6b65 792e 7465 7874 2829 0a20 2020  n_key.text().   
+00014f80: 2020 2020 2069 6620 7365 6c66 2e72 6164       if self.rad
+00014f90: 696f 5f73 7461 7465 2e67 6574 2822 6d6f  io_state.get("mo
+00014fa0: 6465 2229 2069 6e20 5b22 4c53 4222 2c20  de") in ["LSB", 
+00014fb0: 2255 5342 222c 2022 5353 4222 5d3a 0a20  "USB", "SSB"]:. 
+00014fc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00014fd0: 766f 6963 655f 7374 7269 6e67 2873 656c  voice_string(sel
+00014fe0: 662e 7072 6f63 6573 735f 6d61 6372 6f28  f.process_macro(
+00014ff0: 6675 6e63 7469 6f6e 5f6b 6579 2e74 6f6f  function_key.too
+00015000: 6c54 6970 2829 2929 0a20 2020 2020 2020  lTip())).       
+00015010: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+00015020: 2020 2020 6966 2073 656c 662e 6377 3a0a      if self.cw:.
+00015030: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015040: 2e63 772e 7365 6e64 6377 2873 656c 662e  .cw.sendcw(self.
+00015050: 7072 6f63 6573 735f 6d61 6372 6f28 6675  process_macro(fu
+00015060: 6e63 7469 6f6e 5f6b 6579 2e74 6f6f 6c54  nction_key.toolT
+00015070: 6970 2829 2929 0a0a 2020 2020 6465 6620  ip()))..    def 
+00015080: 7275 6e5f 7370 5f62 7574 746f 6e73 5f63  run_sp_buttons_c
+00015090: 6c69 636b 6564 2873 656c 6629 202d 3e20  licked(self) -> 
+000150a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+000150b0: 220a 2020 2020 2020 2020 4861 6e64 6c65  ".        Handle
+000150c0: 2052 756e 2f53 2650 206d 6f64 6520 6368   Run/S&P mode ch
+000150d0: 616e 6765 732e 0a0a 2020 2020 2020 2020  anges...        
+000150e0: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+000150f0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+00015100: 2020 2020 2020 4e6f 6e65 0a0a 2020 2020        None..    
+00015110: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
+00015120: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+00015130: 2020 2020 4e6f 6e65 0a20 2020 2020 2020      None.       
+00015140: 2022 2222 0a20 2020 2020 2020 2073 656c   """.        sel
+00015150: 662e 7072 6566 5b22 7275 6e5f 7374 6174  f.pref["run_stat
+00015160: 6522 5d20 3d20 7365 6c66 2e72 6164 696f  e"] = self.radio
+00015170: 4275 7474 6f6e 5f72 756e 2e69 7343 6865  Button_run.isChe
+00015180: 636b 6564 2829 0a20 2020 2020 2020 2073  cked().        s
+00015190: 656c 662e 7772 6974 655f 7072 6566 6572  elf.write_prefer
+000151a0: 656e 6365 2829 0a20 2020 2020 2020 2073  ence().        s
+000151b0: 656c 662e 7265 6164 5f63 775f 6d61 6372  elf.read_cw_macr
+000151c0: 6f73 2829 0a0a 2020 2020 6465 6620 7772  os()..    def wr
+000151d0: 6974 655f 7072 6566 6572 656e 6365 2873  ite_preference(s
+000151e0: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
+000151f0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00015200: 2020 5772 6974 6520 7072 6566 6572 656e    Write preferen
+00015210: 6365 7320 746f 2066 696c 652e 0a0a 2020  ces to file...  
+00015220: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+00015230: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00015240: 2d2d 2d0a 2020 2020 2020 2020 4e6f 6e65  ---.        None
+00015250: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
 00015260: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-00015270: 2d2d 2d2d 0a20 2020 2020 2020 204e 6f6e  ----.        Non
-00015280: 650a 0a20 2020 2020 2020 2052 6574 7572  e..        Retur
-00015290: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
-000152a0: 2d2d 0a20 2020 2020 2020 204e 6f6e 650a  --.        None.
-000152b0: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
-000152c0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-000152d0: 6728 2277 7269 7465 7072 6566 6572 656e  g("writepreferen
-000152e0: 6365 7322 290a 2020 2020 2020 2020 7472  ces").        tr
-000152f0: 793a 0a20 2020 2020 2020 2020 2020 2077  y:.            w
-00015300: 6974 6820 6f70 656e 2866 7375 7469 6c73  ith open(fsutils
-00015310: 2e43 4f4e 4649 475f 4649 4c45 2c20 2277  .CONFIG_FILE, "w
-00015320: 7422 2c20 656e 636f 6469 6e67 3d22 7574  t", encoding="ut
-00015330: 662d 3822 2920 6173 2066 696c 655f 6465  f-8") as file_de
-00015340: 7363 7269 7074 6f72 3a0a 2020 2020 2020  scriptor:.      
-00015350: 2020 2020 2020 2020 2020 6669 6c65 5f64            file_d
-00015360: 6573 6372 6970 746f 722e 7772 6974 6528  escriptor.write(
-00015370: 6475 6d70 7328 7365 6c66 2e70 7265 662c  dumps(self.pref,
-00015380: 2069 6e64 656e 743d 3429 290a 2020 2020   indent=4)).    
-00015390: 2020 2020 2020 2020 2020 2020 2320 6c6f              # lo
-000153a0: 6767 6572 2e69 6e66 6f28 2277 7269 7469  gger.info("writi
-000153b0: 6e67 3a20 2573 222c 2073 656c 662e 7072  ng: %s", self.pr
-000153c0: 6566 290a 2020 2020 2020 2020 6578 6365  ef).        exce
-000153d0: 7074 2049 4f45 7272 6f72 2061 7320 6578  pt IOError as ex
-000153e0: 6365 7074 696f 6e3a 0a20 2020 2020 2020  ception:.       
-000153f0: 2020 2020 206c 6f67 6765 722e 6372 6974       logger.crit
-00015400: 6963 616c 2822 7772 6974 6570 7265 6665  ical("writeprefe
-00015410: 7265 6e63 6573 3a20 2573 222c 2065 7863  rences: %s", exc
-00015420: 6570 7469 6f6e 290a 0a20 2020 2064 6566  eption)..    def
-00015430: 2072 6561 6470 7265 6665 7265 6e63 6573   readpreferences
-00015440: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-00015450: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00015460: 2020 2020 5265 7374 6f72 6520 7072 6566      Restore pref
-00015470: 6572 656e 6365 7320 6966 2074 6865 7920  erences if they 
-00015480: 6578 6973 742c 206f 7468 6572 7769 7365  exist, otherwise
-00015490: 2063 7265 6174 6520 736f 6d65 2073 616e   create some san
-000154a0: 6520 6465 6661 756c 7473 2e0a 0a20 2020  e defaults...   
-000154b0: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-000154c0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-000154d0: 2d2d 0a20 2020 2020 2020 204e 6f6e 650a  --.        None.
-000154e0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-000154f0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00015500: 0a20 2020 2020 2020 204e 6f6e 650a 2020  .        None.  
-00015510: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
-00015520: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-00015530: 2272 6561 6470 7265 6665 7265 6e63 6573  "readpreferences
-00015540: 2229 0a20 2020 2020 2020 2074 7279 3a0a  ").        try:.
-00015550: 2020 2020 2020 2020 2020 2020 6966 206f              if o
-00015560: 732e 7061 7468 2e65 7869 7374 7328 6673  s.path.exists(fs
-00015570: 7574 696c 732e 434f 4e46 4947 5f46 494c  utils.CONFIG_FIL
-00015580: 4529 3a0a 2020 2020 2020 2020 2020 2020  E):.            
-00015590: 2020 2020 7769 7468 206f 7065 6e28 0a20      with open(. 
-000155a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000155b0: 2020 2066 7375 7469 6c73 2e43 4f4e 4649     fsutils.CONFI
-000155c0: 475f 4649 4c45 2c20 2272 7422 2c20 656e  G_FILE, "rt", en
-000155d0: 636f 6469 6e67 3d22 7574 662d 3822 0a20  coding="utf-8". 
-000155e0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-000155f0: 2061 7320 6669 6c65 5f64 6573 6372 6970   as file_descrip
-00015600: 746f 723a 0a20 2020 2020 2020 2020 2020  tor:.           
-00015610: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-00015620: 6566 203d 206c 6f61 6473 2866 696c 655f  ef = loads(file_
-00015630: 6465 7363 7269 7074 6f72 2e72 6561 6428  descriptor.read(
-00015640: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-00015650: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
-00015660: 666f 2822 2573 222c 2073 656c 662e 7072  fo("%s", self.pr
-00015670: 6566 290a 2020 2020 2020 2020 2020 2020  ef).            
-00015680: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00015690: 2020 2020 2020 6c6f 6767 6572 2e69 6e66        logger.inf
-000156a0: 6f28 224e 6f20 7072 6566 6572 656e 6365  o("No preference
-000156b0: 2066 696c 652e 2057 7269 7469 6e67 2070   file. Writing p
-000156c0: 7265 6665 7265 6e63 652e 2229 0a20 2020  reference.").   
-000156d0: 2020 2020 2020 2020 2020 2020 2077 6974               wit
-000156e0: 6820 6f70 656e 280a 2020 2020 2020 2020  h open(.        
-000156f0: 2020 2020 2020 2020 2020 2020 6673 7574              fsut
-00015700: 696c 732e 434f 4e46 4947 5f46 494c 452c  ils.CONFIG_FILE,
-00015710: 2022 7774 222c 2065 6e63 6f64 696e 673d   "wt", encoding=
-00015720: 2275 7466 2d38 220a 2020 2020 2020 2020  "utf-8".        
-00015730: 2020 2020 2020 2020 2920 6173 2066 696c          ) as fil
-00015740: 655f 6465 7363 7269 7074 6f72 3a0a 2020  e_descriptor:.  
-00015750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015760: 2020 7365 6c66 2e70 7265 6620 3d20 7365    self.pref = se
-00015770: 6c66 2e70 7265 665f 7265 662e 636f 7079  lf.pref_ref.copy
-00015780: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00015790: 2020 2020 2020 2066 696c 655f 6465 7363         file_desc
-000157a0: 7269 7074 6f72 2e77 7269 7465 2864 756d  riptor.write(dum
-000157b0: 7073 2873 656c 662e 7072 6566 2c20 696e  ps(self.pref, in
-000157c0: 6465 6e74 3d34 2929 0a20 2020 2020 2020  dent=4)).       
-000157d0: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-000157e0: 6765 722e 696e 666f 2822 2573 222c 2073  ger.info("%s", s
-000157f0: 656c 662e 7072 6566 290a 2020 2020 2020  elf.pref).      
-00015800: 2020 6578 6365 7074 2049 4f45 7272 6f72    except IOError
-00015810: 2061 7320 6578 6365 7074 696f 6e3a 0a20   as exception:. 
-00015820: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-00015830: 722e 6372 6974 6963 616c 2822 4572 726f  r.critical("Erro
-00015840: 723a 2025 7322 2c20 6578 6365 7074 696f  r: %s", exceptio
-00015850: 6e29 0a0a 2020 2020 2020 2020 7365 6c66  n)..        self
-00015860: 2e6c 6f6f 6b5f 7570 203d 204e 6f6e 650a  .look_up = None.
-00015870: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00015880: 7072 6566 2e67 6574 2822 7573 6571 727a  pref.get("useqrz
-00015890: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
-000158a0: 7365 6c66 2e6c 6f6f 6b5f 7570 203d 2051  self.look_up = Q
-000158b0: 525a 6c6f 6f6b 7570 280a 2020 2020 2020  RZlookup(.      
+00015270: 2d0a 2020 2020 2020 2020 4e6f 6e65 0a20  -.        None. 
+00015280: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
+00015290: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+000152a0: 2822 7772 6974 6570 7265 6665 7265 6e63  ("writepreferenc
+000152b0: 6573 2229 0a20 2020 2020 2020 2074 7279  es").        try
+000152c0: 3a0a 2020 2020 2020 2020 2020 2020 7769  :.            wi
+000152d0: 7468 206f 7065 6e28 6673 7574 696c 732e  th open(fsutils.
+000152e0: 434f 4e46 4947 5f46 494c 452c 2022 7774  CONFIG_FILE, "wt
+000152f0: 222c 2065 6e63 6f64 696e 673d 2275 7466  ", encoding="utf
+00015300: 2d38 2229 2061 7320 6669 6c65 5f64 6573  -8") as file_des
+00015310: 6372 6970 746f 723a 0a20 2020 2020 2020  criptor:.       
+00015320: 2020 2020 2020 2020 2066 696c 655f 6465           file_de
+00015330: 7363 7269 7074 6f72 2e77 7269 7465 2864  scriptor.write(d
+00015340: 756d 7073 2873 656c 662e 7072 6566 2c20  umps(self.pref, 
+00015350: 696e 6465 6e74 3d34 2929 0a20 2020 2020  indent=4)).     
+00015360: 2020 2020 2020 2020 2020 2023 206c 6f67             # log
+00015370: 6765 722e 696e 666f 2822 7772 6974 696e  ger.info("writin
+00015380: 673a 2025 7322 2c20 7365 6c66 2e70 7265  g: %s", self.pre
+00015390: 6629 0a20 2020 2020 2020 2065 7863 6570  f).        excep
+000153a0: 7420 494f 4572 726f 7220 6173 2065 7863  t IOError as exc
+000153b0: 6570 7469 6f6e 3a0a 2020 2020 2020 2020  eption:.        
+000153c0: 2020 2020 6c6f 6767 6572 2e63 7269 7469      logger.criti
+000153d0: 6361 6c28 2277 7269 7465 7072 6566 6572  cal("writeprefer
+000153e0: 656e 6365 733a 2025 7322 2c20 6578 6365  ences: %s", exce
+000153f0: 7074 696f 6e29 0a0a 2020 2020 6465 6620  ption)..    def 
+00015400: 7265 6164 7072 6566 6572 656e 6365 7328  readpreferences(
+00015410: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
+00015420: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00015430: 2020 2052 6573 746f 7265 2070 7265 6665     Restore prefe
+00015440: 7265 6e63 6573 2069 6620 7468 6579 2065  rences if they e
+00015450: 7869 7374 2c20 6f74 6865 7277 6973 6520  xist, otherwise 
+00015460: 6372 6561 7465 2073 6f6d 6520 7361 6e65  create some sane
+00015470: 2064 6566 6175 6c74 732e 0a0a 2020 2020   defaults...    
+00015480: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+00015490: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+000154a0: 2d0a 2020 2020 2020 2020 4e6f 6e65 0a0a  -.        None..
+000154b0: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
+000154c0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
+000154d0: 2020 2020 2020 2020 4e6f 6e65 0a20 2020          None.   
+000154e0: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+000154f0: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
+00015500: 7265 6164 7072 6566 6572 656e 6365 7322  readpreferences"
+00015510: 290a 2020 2020 2020 2020 7472 793a 0a20  ).        try:. 
+00015520: 2020 2020 2020 2020 2020 2069 6620 6f73             if os
+00015530: 2e70 6174 682e 6578 6973 7473 2866 7375  .path.exists(fsu
+00015540: 7469 6c73 2e43 4f4e 4649 475f 4649 4c45  tils.CONFIG_FILE
+00015550: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00015560: 2020 2077 6974 6820 6f70 656e 280a 2020     with open(.  
+00015570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015580: 2020 6673 7574 696c 732e 434f 4e46 4947    fsutils.CONFIG
+00015590: 5f46 494c 452c 2022 7274 222c 2065 6e63  _FILE, "rt", enc
+000155a0: 6f64 696e 673d 2275 7466 2d38 220a 2020  oding="utf-8".  
+000155b0: 2020 2020 2020 2020 2020 2020 2020 2920                ) 
+000155c0: 6173 2066 696c 655f 6465 7363 7269 7074  as file_descript
+000155d0: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
+000155e0: 2020 2020 2020 2020 7365 6c66 2e70 7265          self.pre
+000155f0: 6620 3d20 6c6f 6164 7328 6669 6c65 5f64  f = loads(file_d
+00015600: 6573 6372 6970 746f 722e 7265 6164 2829  escriptor.read()
+00015610: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00015620: 2020 2020 2020 6c6f 6767 6572 2e69 6e66        logger.inf
+00015630: 6f28 2225 7322 2c20 7365 6c66 2e70 7265  o("%s", self.pre
+00015640: 6629 0a20 2020 2020 2020 2020 2020 2065  f).            e
+00015650: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00015660: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
+00015670: 2822 4e6f 2070 7265 6665 7265 6e63 6520  ("No preference 
+00015680: 6669 6c65 2e20 5772 6974 696e 6720 7072  file. Writing pr
+00015690: 6566 6572 656e 6365 2e22 290a 2020 2020  eference.").    
+000156a0: 2020 2020 2020 2020 2020 2020 7769 7468              with
+000156b0: 206f 7065 6e28 0a20 2020 2020 2020 2020   open(.         
+000156c0: 2020 2020 2020 2020 2020 2066 7375 7469             fsuti
+000156d0: 6c73 2e43 4f4e 4649 475f 4649 4c45 2c20  ls.CONFIG_FILE, 
+000156e0: 2277 7422 2c20 656e 636f 6469 6e67 3d22  "wt", encoding="
+000156f0: 7574 662d 3822 0a20 2020 2020 2020 2020  utf-8".         
+00015700: 2020 2020 2020 2029 2061 7320 6669 6c65         ) as file
+00015710: 5f64 6573 6372 6970 746f 723a 0a20 2020  _descriptor:.   
+00015720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015730: 2073 656c 662e 7072 6566 203d 2073 656c   self.pref = sel
+00015740: 662e 7072 6566 5f72 6566 2e63 6f70 7928  f.pref_ref.copy(
+00015750: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00015760: 2020 2020 2020 6669 6c65 5f64 6573 6372        file_descr
+00015770: 6970 746f 722e 7772 6974 6528 6475 6d70  iptor.write(dump
+00015780: 7328 7365 6c66 2e70 7265 662c 2069 6e64  s(self.pref, ind
+00015790: 656e 743d 3429 290a 2020 2020 2020 2020  ent=4)).        
+000157a0: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+000157b0: 6572 2e69 6e66 6f28 2225 7322 2c20 7365  er.info("%s", se
+000157c0: 6c66 2e70 7265 6629 0a20 2020 2020 2020  lf.pref).       
+000157d0: 2065 7863 6570 7420 494f 4572 726f 7220   except IOError 
+000157e0: 6173 2065 7863 6570 7469 6f6e 3a0a 2020  as exception:.  
+000157f0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+00015800: 2e63 7269 7469 6361 6c28 2245 7272 6f72  .critical("Error
+00015810: 3a20 2573 222c 2065 7863 6570 7469 6f6e  : %s", exception
+00015820: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00015830: 6c6f 6f6b 5f75 7020 3d20 4e6f 6e65 0a20  look_up = None. 
+00015840: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
+00015850: 7265 662e 6765 7428 2275 7365 7172 7a22  ref.get("useqrz"
+00015860: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+00015870: 656c 662e 6c6f 6f6b 5f75 7020 3d20 5152  elf.look_up = QR
+00015880: 5a6c 6f6f 6b75 7028 0a20 2020 2020 2020  Zlookup(.       
+00015890: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+000158a0: 6566 2e67 6574 2822 6c6f 6f6b 7570 7573  ef.get("lookupus
+000158b0: 6572 6e61 6d65 2229 2c0a 2020 2020 2020  ername"),.      
 000158c0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-000158d0: 7265 662e 6765 7428 226c 6f6f 6b75 7075  ref.get("lookupu
-000158e0: 7365 726e 616d 6522 292c 0a20 2020 2020  sername"),.     
-000158f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015900: 7072 6566 2e67 6574 2822 6c6f 6f6b 7570  pref.get("lookup
-00015910: 7061 7373 776f 7264 2229 2c0a 2020 2020  password"),.    
-00015920: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-00015930: 2020 2069 6620 7365 6c66 2e70 7265 662e     if self.pref.
-00015940: 6765 7428 2275 7365 6861 6d71 7468 2229  get("usehamqth")
-00015950: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00015960: 6c66 2e6c 6f6f 6b5f 7570 203d 2048 616d  lf.look_up = Ham
-00015970: 5154 4828 0a20 2020 2020 2020 2020 2020  QTH(.           
+000158d0: 7265 662e 6765 7428 226c 6f6f 6b75 7070  ref.get("lookupp
+000158e0: 6173 7377 6f72 6422 292c 0a20 2020 2020  assword"),.     
+000158f0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00015900: 2020 6966 2073 656c 662e 7072 6566 2e67    if self.pref.g
+00015910: 6574 2822 7573 6568 616d 7174 6822 293a  et("usehamqth"):
+00015920: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00015930: 662e 6c6f 6f6b 5f75 7020 3d20 4861 6d51  f.look_up = HamQ
+00015940: 5448 280a 2020 2020 2020 2020 2020 2020  TH(.            
+00015950: 2020 2020 7365 6c66 2e70 7265 662e 6765      self.pref.ge
+00015960: 7428 226c 6f6f 6b75 7075 7365 726e 616d  t("lookupusernam
+00015970: 6522 292c 0a20 2020 2020 2020 2020 2020  e"),.           
 00015980: 2020 2020 2073 656c 662e 7072 6566 2e67       self.pref.g
-00015990: 6574 2822 6c6f 6f6b 7570 7573 6572 6e61  et("lookupuserna
-000159a0: 6d65 2229 2c0a 2020 2020 2020 2020 2020  me"),.          
-000159b0: 2020 2020 2020 7365 6c66 2e70 7265 662e        self.pref.
-000159c0: 6765 7428 226c 6f6f 6b75 7070 6173 7377  get("lookuppassw
-000159d0: 6f72 6422 292c 0a20 2020 2020 2020 2020  ord"),.         
-000159e0: 2020 2029 0a0a 2020 2020 2020 2020 6966     )..        if
-000159f0: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
-00015a00: 7275 6e5f 7374 6174 6522 293a 0a20 2020  run_state"):.   
-00015a10: 2020 2020 2020 2020 2073 656c 662e 7261           self.ra
-00015a20: 6469 6f42 7574 746f 6e5f 7275 6e2e 7365  dioButton_run.se
-00015a30: 7443 6865 636b 6564 2854 7275 6529 0a20  tChecked(True). 
-00015a40: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00015a50: 2020 2020 2020 2020 2073 656c 662e 7261           self.ra
-00015a60: 6469 6f42 7574 746f 6e5f 7370 2e73 6574  dioButton_sp.set
-00015a70: 4368 6563 6b65 6428 5472 7565 290a 0a20  Checked(True).. 
-00015a80: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
-00015a90: 7265 662e 6765 7428 2263 6f6d 6d61 6e64  ref.get("command
-00015aa0: 5f62 7574 746f 6e73 2229 3a0a 2020 2020  _buttons"):.    
-00015ab0: 2020 2020 2020 2020 7365 6c66 2e61 6374          self.act
-00015ac0: 696f 6e43 6f6d 6d61 6e64 5f42 7574 746f  ionCommand_Butto
-00015ad0: 6e73 2e73 6574 4368 6563 6b65 6428 5472  ns.setChecked(Tr
-00015ae0: 7565 290a 2020 2020 2020 2020 656c 7365  ue).        else
-00015af0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00015b00: 6c66 2e61 6374 696f 6e43 6f6d 6d61 6e64  lf.actionCommand
-00015b10: 5f42 7574 746f 6e73 2e73 6574 4368 6563  _Buttons.setChec
-00015b20: 6b65 6428 4661 6c73 6529 0a0a 2020 2020  ked(False)..    
-00015b30: 2020 2020 6966 2073 656c 662e 7072 6566      if self.pref
-00015b40: 2e67 6574 2822 6377 5f6d 6163 726f 7322  .get("cw_macros"
-00015b50: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-00015b60: 656c 662e 6163 7469 6f6e 4357 5f4d 6163  elf.actionCW_Mac
-00015b70: 726f 732e 7365 7443 6865 636b 6564 2854  ros.setChecked(T
-00015b80: 7275 6529 0a20 2020 2020 2020 2065 6c73  rue).        els
-00015b90: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00015ba0: 656c 662e 6163 7469 6f6e 4357 5f4d 6163  elf.actionCW_Mac
-00015bb0: 726f 732e 7365 7443 6865 636b 6564 2846  ros.setChecked(F
-00015bc0: 616c 7365 290a 0a20 2020 2020 2020 2069  alse)..        i
-00015bd0: 6620 7365 6c66 2e70 7265 662e 6765 7428  f self.pref.get(
-00015be0: 2262 616e 6473 5f6d 6f64 6573 2229 3a0a  "bands_modes"):.
-00015bf0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015c00: 2e61 6374 696f 6e4d 6f64 655f 616e 645f  .actionMode_and_
-00015c10: 4261 6e64 732e 7365 7443 6865 636b 6564  Bands.setChecked
-00015c20: 2854 7275 6529 0a20 2020 2020 2020 2065  (True).        e
-00015c30: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00015c40: 2073 656c 662e 6163 7469 6f6e 4d6f 6465   self.actionMode
-00015c50: 5f61 6e64 5f42 616e 6473 2e73 6574 4368  _and_Bands.setCh
-00015c60: 6563 6b65 6428 4661 6c73 6529 0a0a 2020  ecked(False)..  
-00015c70: 2020 2020 2020 7365 6c66 2e6d 756c 7469        self.multi
-00015c80: 6361 7374 5f69 6e74 6572 6661 6365 203d  cast_interface =
-00015c90: 204d 756c 7469 6361 7374 280a 2020 2020   Multicast(.    
-00015ca0: 2020 2020 2020 2020 7365 6c66 2e70 7265          self.pre
-00015cb0: 662e 6765 7428 226d 756c 7469 6361 7374  f.get("multicast
-00015cc0: 5f67 726f 7570 222c 2022 3233 392e 312e  _group", "239.1.
-00015cd0: 312e 3122 292c 0a20 2020 2020 2020 2020  1.1"),.         
-00015ce0: 2020 2073 656c 662e 7072 6566 2e67 6574     self.pref.get
-00015cf0: 2822 6d75 6c74 6963 6173 745f 706f 7274  ("multicast_port
-00015d00: 222c 2032 3233 3929 2c0a 2020 2020 2020  ", 2239),.      
-00015d10: 2020 2020 2020 7365 6c66 2e70 7265 662e        self.pref.
-00015d20: 6765 7428 2269 6e74 6572 6661 6365 5f69  get("interface_i
-00015d30: 7022 2c20 2230 2e30 2e30 2e30 2229 2c0a  p", "0.0.0.0"),.
-00015d40: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00015d50: 2020 7365 6c66 2e6d 756c 7469 6361 7374    self.multicast
-00015d60: 5f69 6e74 6572 6661 6365 2e72 6561 6479  _interface.ready
-00015d70: 5f72 6561 645f 636f 6e6e 6563 7428 7365  _read_connect(se
-00015d80: 6c66 2e77 6174 6368 5f75 6470 290a 0a20  lf.watch_udp).. 
-00015d90: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
-00015da0: 7265 662e 6765 7428 2264 6172 6b6d 6f64  ref.get("darkmod
-00015db0: 6522 293a 0a20 2020 2020 2020 2020 2020  e"):.           
-00015dc0: 2073 656c 662e 6163 7469 6f6e 4461 726b   self.actionDark
-00015dd0: 5f4d 6f64 655f 322e 7365 7443 6865 636b  _Mode_2.setCheck
-00015de0: 6564 2854 7275 6529 0a20 2020 2020 2020  ed(True).       
+00015990: 6574 2822 6c6f 6f6b 7570 7061 7373 776f  et("lookuppasswo
+000159a0: 7264 2229 2c0a 2020 2020 2020 2020 2020  rd"),.          
+000159b0: 2020 290a 0a20 2020 2020 2020 2069 6620    )..        if 
+000159c0: 7365 6c66 2e70 7265 662e 6765 7428 2272  self.pref.get("r
+000159d0: 756e 5f73 7461 7465 2229 3a0a 2020 2020  un_state"):.    
+000159e0: 2020 2020 2020 2020 7365 6c66 2e72 6164          self.rad
+000159f0: 696f 4275 7474 6f6e 5f72 756e 2e73 6574  ioButton_run.set
+00015a00: 4368 6563 6b65 6428 5472 7565 290a 2020  Checked(True).  
+00015a10: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00015a20: 2020 2020 2020 2020 7365 6c66 2e72 6164          self.rad
+00015a30: 696f 4275 7474 6f6e 5f73 702e 7365 7443  ioButton_sp.setC
+00015a40: 6865 636b 6564 2854 7275 6529 0a0a 2020  hecked(True)..  
+00015a50: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
+00015a60: 6566 2e67 6574 2822 636f 6d6d 616e 645f  ef.get("command_
+00015a70: 6275 7474 6f6e 7322 293a 0a20 2020 2020  buttons"):.     
+00015a80: 2020 2020 2020 2073 656c 662e 6163 7469         self.acti
+00015a90: 6f6e 436f 6d6d 616e 645f 4275 7474 6f6e  onCommand_Button
+00015aa0: 732e 7365 7443 6865 636b 6564 2854 7275  s.setChecked(Tru
+00015ab0: 6529 0a20 2020 2020 2020 2065 6c73 653a  e).        else:
+00015ac0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00015ad0: 662e 6163 7469 6f6e 436f 6d6d 616e 645f  f.actionCommand_
+00015ae0: 4275 7474 6f6e 732e 7365 7443 6865 636b  Buttons.setCheck
+00015af0: 6564 2846 616c 7365 290a 0a20 2020 2020  ed(False)..     
+00015b00: 2020 2069 6620 7365 6c66 2e70 7265 662e     if self.pref.
+00015b10: 6765 7428 2263 775f 6d61 6372 6f73 2229  get("cw_macros")
+00015b20: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00015b30: 6c66 2e61 6374 696f 6e43 575f 4d61 6372  lf.actionCW_Macr
+00015b40: 6f73 2e73 6574 4368 6563 6b65 6428 5472  os.setChecked(Tr
+00015b50: 7565 290a 2020 2020 2020 2020 656c 7365  ue).        else
+00015b60: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00015b70: 6c66 2e61 6374 696f 6e43 575f 4d61 6372  lf.actionCW_Macr
+00015b80: 6f73 2e73 6574 4368 6563 6b65 6428 4661  os.setChecked(Fa
+00015b90: 6c73 6529 0a0a 2020 2020 2020 2020 6966  lse)..        if
+00015ba0: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
+00015bb0: 6261 6e64 735f 6d6f 6465 7322 293a 0a20  bands_modes"):. 
+00015bc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015bd0: 6163 7469 6f6e 4d6f 6465 5f61 6e64 5f42  actionMode_and_B
+00015be0: 616e 6473 2e73 6574 4368 6563 6b65 6428  ands.setChecked(
+00015bf0: 5472 7565 290a 2020 2020 2020 2020 656c  True).        el
+00015c00: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00015c10: 7365 6c66 2e61 6374 696f 6e4d 6f64 655f  self.actionMode_
+00015c20: 616e 645f 4261 6e64 732e 7365 7443 6865  and_Bands.setChe
+00015c30: 636b 6564 2846 616c 7365 290a 0a20 2020  cked(False)..   
+00015c40: 2020 2020 2073 656c 662e 6d75 6c74 6963       self.multic
+00015c50: 6173 745f 696e 7465 7266 6163 6520 3d20  ast_interface = 
+00015c60: 4d75 6c74 6963 6173 7428 0a20 2020 2020  Multicast(.     
+00015c70: 2020 2020 2020 2073 656c 662e 7072 6566         self.pref
+00015c80: 2e67 6574 2822 6d75 6c74 6963 6173 745f  .get("multicast_
+00015c90: 6772 6f75 7022 2c20 2232 3339 2e31 2e31  group", "239.1.1
+00015ca0: 2e31 2229 2c0a 2020 2020 2020 2020 2020  .1"),.          
+00015cb0: 2020 7365 6c66 2e70 7265 662e 6765 7428    self.pref.get(
+00015cc0: 226d 756c 7469 6361 7374 5f70 6f72 7422  "multicast_port"
+00015cd0: 2c20 3232 3339 292c 0a20 2020 2020 2020  , 2239),.       
+00015ce0: 2020 2020 2073 656c 662e 7072 6566 2e67       self.pref.g
+00015cf0: 6574 2822 696e 7465 7266 6163 655f 6970  et("interface_ip
+00015d00: 222c 2022 302e 302e 302e 3022 292c 0a20  ", "0.0.0.0"),. 
+00015d10: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00015d20: 2073 656c 662e 6d75 6c74 6963 6173 745f   self.multicast_
+00015d30: 696e 7465 7266 6163 652e 7265 6164 795f  interface.ready_
+00015d40: 7265 6164 5f63 6f6e 6e65 6374 2873 656c  read_connect(sel
+00015d50: 662e 7761 7463 685f 7564 7029 0a0a 2020  f.watch_udp)..  
+00015d60: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
+00015d70: 6566 2e67 6574 2822 6461 726b 6d6f 6465  ef.get("darkmode
+00015d80: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
+00015d90: 7365 6c66 2e61 6374 696f 6e44 6172 6b5f  self.actionDark_
+00015da0: 4d6f 6465 5f32 2e73 6574 4368 6563 6b65  Mode_2.setChecke
+00015db0: 6428 5472 7565 290a 2020 2020 2020 2020  d(True).        
+00015dc0: 2020 2020 7365 6c66 2e73 6574 4461 726b      self.setDark
+00015dd0: 4d6f 6465 2854 7275 6529 0a20 2020 2020  Mode(True).     
+00015de0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
 00015df0: 2020 2020 2073 656c 662e 7365 7444 6172       self.setDar
-00015e00: 6b4d 6f64 6528 5472 7565 290a 2020 2020  kMode(True).    
-00015e10: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00015e20: 2020 2020 2020 7365 6c66 2e73 6574 4461        self.setDa
-00015e30: 726b 4d6f 6465 2846 616c 7365 290a 2020  rkMode(False).  
-00015e40: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00015e50: 6374 696f 6e44 6172 6b5f 4d6f 6465 5f32  ctionDark_Mode_2
-00015e60: 2e73 6574 4368 6563 6b65 6428 4661 6c73  .setChecked(Fals
-00015e70: 6529 0a0a 2020 2020 2020 2020 7365 6c66  e)..        self
-00015e80: 2e72 6967 5f63 6f6e 7472 6f6c 203d 204e  .rig_control = N
-00015e90: 6f6e 650a 0a20 2020 2020 2020 2069 6620  one..        if 
-00015ea0: 7365 6c66 2e70 7265 662e 6765 7428 2275  self.pref.get("u
-00015eb0: 7365 666c 7269 6722 2c20 4661 6c73 6529  seflrig", False)
-00015ec0: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
-00015ed0: 6767 6572 2e64 6562 7567 280a 2020 2020  gger.debug(.    
-00015ee0: 2020 2020 2020 2020 2020 2020 2255 7369              "Usi
-00015ef0: 6e67 2066 6c72 6967 3a20 2573 222c 0a20  ng flrig: %s",. 
-00015f00: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00015f10: 227b 7365 6c66 2e70 7265 662e 6765 7428  "{self.pref.get(
-00015f20: 2743 4154 5f69 7027 297d 207b 7365 6c66  'CAT_ip')} {self
-00015f30: 2e70 7265 662e 6765 7428 2743 4154 5f70  .pref.get('CAT_p
-00015f40: 6f72 7427 297d 222c 0a20 2020 2020 2020  ort')}",.       
-00015f50: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00015f60: 2020 2073 656c 662e 7269 675f 636f 6e74     self.rig_cont
-00015f70: 726f 6c20 3d20 4341 5428 0a20 2020 2020  rol = CAT(.     
-00015f80: 2020 2020 2020 2020 2020 2022 666c 7269             "flri
-00015f90: 6722 2c0a 2020 2020 2020 2020 2020 2020  g",.            
-00015fa0: 2020 2020 7365 6c66 2e70 7265 662e 6765      self.pref.ge
-00015fb0: 7428 2243 4154 5f69 7022 2c20 2231 3237  t("CAT_ip", "127
-00015fc0: 2e30 2e30 2e31 2229 2c0a 2020 2020 2020  .0.0.1"),.      
-00015fd0: 2020 2020 2020 2020 2020 696e 7428 7365            int(se
-00015fe0: 6c66 2e70 7265 662e 6765 7428 2243 4154  lf.pref.get("CAT
-00015ff0: 5f70 6f72 7422 2c20 3132 3334 3529 292c  _port", 12345)),
-00016000: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-00016010: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00016020: 7072 6566 2e67 6574 2822 7573 6572 6967  pref.get("userig
-00016030: 6374 6c64 222c 2046 616c 7365 293a 0a20  ctld", False):. 
-00016040: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-00016050: 722e 6465 6275 6728 0a20 2020 2020 2020  r.debug(.       
-00016060: 2020 2020 2020 2020 2022 5573 696e 6720           "Using 
-00016070: 7269 6763 746c 643a 2025 7322 2c0a 2020  rigctld: %s",.  
-00016080: 2020 2020 2020 2020 2020 2020 2020 6622                f"
-00016090: 7b73 656c 662e 7072 6566 2e67 6574 2827  {self.pref.get('
-000160a0: 4341 545f 6970 2729 7d20 7b73 656c 662e  CAT_ip')} {self.
-000160b0: 7072 6566 2e67 6574 2827 4341 545f 706f  pref.get('CAT_po
-000160c0: 7274 2729 7d22 2c0a 2020 2020 2020 2020  rt')}",.        
-000160d0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-000160e0: 2020 7365 6c66 2e72 6967 5f63 6f6e 7472    self.rig_contr
-000160f0: 6f6c 203d 2043 4154 280a 2020 2020 2020  ol = CAT(.      
-00016100: 2020 2020 2020 2020 2020 2272 6967 6374            "rigct
-00016110: 6c64 222c 0a20 2020 2020 2020 2020 2020  ld",.           
-00016120: 2020 2020 2073 656c 662e 7072 6566 2e67       self.pref.g
-00016130: 6574 2822 4341 545f 6970 222c 2022 3132  et("CAT_ip", "12
-00016140: 372e 302e 302e 3122 292c 0a20 2020 2020  7.0.0.1"),.     
-00016150: 2020 2020 2020 2020 2020 2069 6e74 2873             int(s
-00016160: 656c 662e 7072 6566 2e67 6574 2822 4341  elf.pref.get("CA
-00016170: 545f 706f 7274 222c 2034 3533 3229 292c  T_port", 4532)),
-00016180: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-00016190: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000161a0: 7072 6566 2e67 6574 2822 6377 7479 7065  pref.get("cwtype
-000161b0: 222c 2030 2920 3d3d 2030 3a0a 2020 2020  ", 0) == 0:.    
-000161c0: 2020 2020 2020 2020 7365 6c66 2e63 7720          self.cw 
-000161d0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2065  = None.        e
-000161e0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-000161f0: 2073 656c 662e 6377 203d 2043 5728 0a20   self.cw = CW(. 
-00016200: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00016210: 6e74 2873 656c 662e 7072 6566 2e67 6574  nt(self.pref.get
-00016220: 2822 6377 7479 7065 2229 292c 0a20 2020  ("cwtype")),.   
-00016230: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00016240: 662e 7072 6566 2e67 6574 2822 6377 6970  f.pref.get("cwip
-00016250: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
-00016260: 2020 2020 696e 7428 7365 6c66 2e70 7265      int(self.pre
-00016270: 662e 6765 7428 2263 7770 6f72 7422 2c20  f.get("cwport", 
-00016280: 3637 3839 2929 2c0a 2020 2020 2020 2020  6789)),.        
-00016290: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-000162a0: 2020 7365 6c66 2e63 772e 7370 6565 6420    self.cw.speed 
-000162b0: 3d20 3230 0a20 2020 2020 2020 2020 2020  = 20.           
-000162c0: 2069 6620 7365 6c66 2e63 772e 7365 7276   if self.cw.serv
-000162d0: 6572 7479 7065 203d 3d20 323a 0a20 2020  ertype == 2:.   
-000162e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000162f0: 662e 6377 2e73 6574 5f77 696e 6b65 7965  f.cw.set_winkeye
-00016300: 725f 7370 6565 6428 3230 290a 0a20 2020  r_speed(20)..   
-00016310: 2020 2020 2073 656c 662e 6e31 6d6d 203d       self.n1mm =
-00016320: 204e 6f6e 650a 2020 2020 2020 2020 6966   None.        if
-00016330: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
-00016340: 7365 6e64 5f6e 316d 6d5f 7061 636b 6574  send_n1mm_packet
-00016350: 7322 2c20 4661 6c73 6529 3a0a 2020 2020  s", False):.    
-00016360: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-00016370: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00016380: 662e 6e31 6d6d 203d 204e 314d 4d28 0a20  f.n1mm = N1MM(. 
-00016390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000163a0: 2020 2073 656c 662e 7072 6566 2e67 6574     self.pref.get
-000163b0: 2822 6e31 6d6d 5f72 6164 696f 706f 7274  ("n1mm_radioport
-000163c0: 222c 2022 3132 372e 302e 302e 313a 3132  ", "127.0.0.1:12
-000163d0: 3036 3022 292c 0a20 2020 2020 2020 2020  060"),.         
-000163e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000163f0: 7072 6566 2e67 6574 2822 6e31 6d6d 5f63  pref.get("n1mm_c
-00016400: 6f6e 7461 6374 706f 7274 222c 2022 3132  ontactport", "12
-00016410: 372e 302e 302e 313a 3132 3036 3122 292c  7.0.0.1:12061"),
-00016420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016430: 2020 2020 2073 656c 662e 7072 6566 2e67       self.pref.g
-00016440: 6574 2822 6e31 6d6d 5f6c 6f6f 6b75 7070  et("n1mm_lookupp
-00016450: 6f72 7422 2c20 2231 3237 2e30 2e30 2e31  ort", "127.0.0.1
-00016460: 3a31 3230 3630 2229 2c0a 2020 2020 2020  :12060"),.      
-00016470: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00016480: 6c66 2e70 7265 662e 6765 7428 226e 316d  lf.pref.get("n1m
-00016490: 6d5f 7363 6f72 6570 6f72 7422 2c20 2231  m_scoreport", "1
-000164a0: 3237 2e30 2e30 2e31 3a31 3230 3630 2229  27.0.0.1:12060")
-000164b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000164c0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-000164d0: 6578 6365 7074 2056 616c 7565 4572 726f  except ValueErro
-000164e0: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
-000164f0: 2020 206c 6f67 6765 722e 7761 726e 696e     logger.warnin
-00016500: 6728 2225 7322 2c20 6622 7b56 616c 7565  g("%s", f"{Value
-00016510: 4572 726f 727d 2229 0a20 2020 2020 2020  Error}").       
-00016520: 2020 2020 2073 656c 662e 6e31 6d6d 2e73       self.n1mm.s
-00016530: 656e 645f 7261 6469 6f5f 7061 636b 6574  end_radio_packet
-00016540: 7320 3d20 7365 6c66 2e70 7265 662e 6765  s = self.pref.ge
-00016550: 7428 2273 656e 645f 6e31 6d6d 5f72 6164  t("send_n1mm_rad
-00016560: 696f 222c 2046 616c 7365 290a 2020 2020  io", False).    
-00016570: 2020 2020 2020 2020 7365 6c66 2e6e 316d          self.n1m
-00016580: 6d2e 7365 6e64 5f63 6f6e 7461 6374 5f70  m.send_contact_p
-00016590: 6163 6b65 7473 203d 2073 656c 662e 7072  ackets = self.pr
-000165a0: 6566 2e67 6574 2822 7365 6e64 5f6e 316d  ef.get("send_n1m
-000165b0: 6d5f 636f 6e74 6163 7422 2c20 4661 6c73  m_contact", Fals
-000165c0: 6529 0a20 2020 2020 2020 2020 2020 2073  e).            s
-000165d0: 656c 662e 6e31 6d6d 2e73 656e 645f 6c6f  elf.n1mm.send_lo
-000165e0: 6f6b 7570 5f70 6163 6b65 7473 203d 2073  okup_packets = s
-000165f0: 656c 662e 7072 6566 2e67 6574 2822 7365  elf.pref.get("se
-00016600: 6e64 5f6e 316d 6d5f 6c6f 6f6b 7570 222c  nd_n1mm_lookup",
-00016610: 2046 616c 7365 290a 2020 2020 2020 2020   False).        
-00016620: 2020 2020 7365 6c66 2e6e 316d 6d2e 7365      self.n1mm.se
-00016630: 6e64 5f73 636f 7265 5f70 6163 6b65 7473  nd_score_packets
-00016640: 203d 2073 656c 662e 7072 6566 2e67 6574   = self.pref.get
-00016650: 2822 7365 6e64 5f6e 316d 6d5f 7363 6f72  ("send_n1mm_scor
-00016660: 6522 2c20 4661 6c73 6529 0a20 2020 2020  e", False).     
-00016670: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
-00016680: 2e72 6164 696f 5f69 6e66 6f5b 2253 7461  .radio_info["Sta
-00016690: 7469 6f6e 4e61 6d65 225d 203d 2073 656c  tionName"] = sel
-000166a0: 662e 7072 6566 2e67 6574 2822 6e31 6d6d  f.pref.get("n1mm
-000166b0: 5f73 7461 7469 6f6e 5f6e 616d 6522 2c20  _station_name", 
-000166c0: 2222 290a 0a20 2020 2020 2020 2073 656c  "")..        sel
-000166d0: 662e 7368 6f77 5f63 6f6d 6d61 6e64 5f62  f.show_command_b
-000166e0: 7574 746f 6e73 2829 0a20 2020 2020 2020  uttons().       
-000166f0: 2073 656c 662e 7368 6f77 5f43 575f 6d61   self.show_CW_ma
-00016700: 6372 6f73 2829 0a0a 2020 2020 2020 2020  cros()..        
-00016710: 2320 4966 2062 616e 6473 206c 6973 7420  # If bands list 
-00016720: 6973 2065 6d70 7479 2066 696c 6c20 6974  is empty fill it
-00016730: 2077 6974 6820 4846 2e0a 2020 2020 2020   with HF..      
-00016740: 2020 6966 2073 656c 662e 7072 6566 2e67    if self.pref.g
-00016750: 6574 2822 6261 6e64 7322 2c20 5b5d 2920  et("bands", []) 
-00016760: 3d3d 205b 5d3a 0a20 2020 2020 2020 2020  == []:.         
-00016770: 2020 2073 656c 662e 7072 6566 5b22 6261     self.pref["ba
-00016780: 6e64 7322 5d20 3d20 5b22 3136 3022 2c20  nds"] = ["160", 
-00016790: 2238 3022 2c20 2234 3022 2c20 2232 3022  "80", "40", "20"
-000167a0: 2c20 2231 3522 2c20 2231 3022 5d0a 0a20  , "15", "10"].. 
-000167b0: 2020 2020 2020 2023 2048 6964 6520 616c         # Hide al
-000167c0: 6c20 7468 6520 6261 6e64 7320 616e 6420  l the bands and 
-000167d0: 7468 656e 2073 686f 7720 6f6e 6c79 2074  then show only t
-000167e0: 6865 2077 616e 7465 6420 6261 6e64 732e  he wanted bands.
-000167f0: 0a20 2020 2020 2020 2066 6f72 205f 696e  .        for _in
-00016800: 6469 6361 746f 7220 696e 205b 0a20 2020  dicator in [.   
-00016810: 2020 2020 2020 2020 2073 656c 662e 6261           self.ba
-00016820: 6e64 5f69 6e64 6963 6174 6f72 735f 6377  nd_indicators_cw
-00016830: 2c0a 2020 2020 2020 2020 2020 2020 7365  ,.            se
-00016840: 6c66 2e62 616e 645f 696e 6469 6361 746f  lf.band_indicato
-00016850: 7273 5f73 7362 2c0a 2020 2020 2020 2020  rs_ssb,.        
-00016860: 2020 2020 7365 6c66 2e62 616e 645f 696e      self.band_in
-00016870: 6469 6361 746f 7273 5f72 7474 792c 0a20  dicators_rtty,. 
-00016880: 2020 2020 2020 205d 3a0a 2020 2020 2020         ]:.      
-00016890: 2020 2020 2020 666f 7220 5f62 616e 6469        for _bandi
-000168a0: 6e64 2069 6e20 5f69 6e64 6963 6174 6f72  nd in _indicator
-000168b0: 2e76 616c 7565 7328 293a 0a20 2020 2020  .values():.     
-000168c0: 2020 2020 2020 2020 2020 205f 6261 6e64             _band
-000168d0: 696e 642e 6869 6465 2829 0a20 2020 2020  ind.hide().     
-000168e0: 2020 2020 2020 2066 6f72 2062 616e 645f         for band_
-000168f0: 746f 5f73 686f 7720 696e 2073 656c 662e  to_show in self.
-00016900: 7072 6566 2e67 6574 2822 6261 6e64 7322  pref.get("bands"
-00016910: 2c20 5b5d 293a 0a20 2020 2020 2020 2020  , []):.         
-00016920: 2020 2020 2020 2069 6620 6261 6e64 5f74         if band_t
-00016930: 6f5f 7368 6f77 2069 6e20 5f69 6e64 6963  o_show in _indic
-00016940: 6174 6f72 3a0a 2020 2020 2020 2020 2020  ator:.          
-00016950: 2020 2020 2020 2020 2020 5f69 6e64 6963            _indic
-00016960: 6174 6f72 5b62 616e 645f 746f 5f73 686f  ator[band_to_sho
-00016970: 775d 2e73 686f 7728 290a 2020 2020 2020  w].show().      
-00016980: 2020 2320 7365 6c66 2e73 686f 775f 6261    # self.show_ba
-00016990: 6e64 5f6d 6f64 6528 290a 0a20 2020 2064  nd_mode()..    d
-000169a0: 6566 2077 6174 6368 5f75 6470 2873 656c  ef watch_udp(sel
-000169b0: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
-000169c0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000169d0: 5761 7463 6820 7468 6520 5544 5020 736f  Watch the UDP so
-000169e0: 636b 6574 2066 6f72 2069 6e63 6f6d 696e  cket for incomin
-000169f0: 6720 6461 7461 2e0a 0a20 2020 2020 2020  g data...       
-00016a00: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-00016a10: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-00016a20: 2020 2020 2020 204e 6f6e 650a 0a20 2020         None..   
-00016a30: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
-00016a40: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
-00016a50: 2020 2020 204e 6f6e 650a 2020 2020 2020       None.      
-00016a60: 2020 2222 220a 0a20 2020 2020 2020 2077    """..        w
-00016a70: 6869 6c65 2073 656c 662e 6d75 6c74 6963  hile self.multic
-00016a80: 6173 745f 696e 7465 7266 6163 652e 6861  ast_interface.ha
-00016a90: 735f 7065 6e64 696e 675f 6461 7461 6772  s_pending_datagr
-00016aa0: 616d 7328 293a 0a20 2020 2020 2020 2020  ams():.         
-00016ab0: 2020 206a 736f 6e5f 6461 7461 203d 2073     json_data = s
-00016ac0: 656c 662e 6d75 6c74 6963 6173 745f 696e  elf.multicast_in
-00016ad0: 7465 7266 6163 652e 7265 6164 5f64 6174  terface.read_dat
-00016ae0: 6167 7261 6d5f 6173 5f6a 736f 6e28 290a  agram_as_json().
-00016af0: 2020 2020 2020 2020 2020 2020 6966 206a              if j
-00016b00: 736f 6e5f 6461 7461 3a0a 2020 2020 2020  son_data:.      
-00016b10: 2020 2020 2020 2020 2020 6966 2028 0a20            if (. 
-00016b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b30: 2020 206a 736f 6e5f 6461 7461 2e67 6574     json_data.get
-00016b40: 2822 636d 6422 2c20 2222 2920 3d3d 2022  ("cmd", "") == "
-00016b50: 4745 5443 4f4c 554d 4e53 220a 2020 2020  GETCOLUMNS".    
-00016b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b70: 616e 6420 6a73 6f6e 5f64 6174 612e 6765  and json_data.ge
-00016b80: 7428 2273 7461 7469 6f6e 222c 2022 2229  t("station", "")
-00016b90: 203d 3d20 706c 6174 666f 726d 2e6e 6f64   == platform.nod
-00016ba0: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
-00016bb0: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
-00016bc0: 2020 2020 2020 2020 2020 2069 6620 6861             if ha
-00016bd0: 7361 7474 7228 7365 6c66 2e63 6f6e 7465  sattr(self.conte
-00016be0: 7374 2c20 2263 6f6c 756d 6e73 2229 3a0a  st, "columns"):.
-00016bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c00: 2020 2020 2020 2020 636d 6420 3d20 7b7d          cmd = {}
-00016c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016c20: 2020 2020 2020 2020 2063 6d64 5b22 636d           cmd["cm
-00016c30: 6422 5d20 3d20 2253 484f 5743 4f4c 554d  d"] = "SHOWCOLUM
-00016c40: 4e53 220a 2020 2020 2020 2020 2020 2020  NS".            
-00016c50: 2020 2020 2020 2020 2020 2020 636d 645b              cmd[
-00016c60: 2273 7461 7469 6f6e 225d 203d 2070 6c61  "station"] = pla
-00016c70: 7466 6f72 6d2e 6e6f 6465 2829 0a20 2020  tform.node().   
-00016c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c90: 2020 2020 2063 6d64 5b22 434f 4c55 4d4e       cmd["COLUMN
-00016ca0: 5322 5d20 3d20 7365 6c66 2e63 6f6e 7465  S"] = self.conte
-00016cb0: 7374 2e63 6f6c 756d 6e73 0a20 2020 2020  st.columns.     
-00016cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016cd0: 2020 2073 656c 662e 6d75 6c74 6963 6173     self.multicas
-00016ce0: 745f 696e 7465 7266 6163 652e 7365 6e64  t_interface.send
-00016cf0: 5f61 735f 6a73 6f6e 2863 6d64 290a 2020  _as_json(cmd).  
+00015e00: 6b4d 6f64 6528 4661 6c73 6529 0a20 2020  kMode(False).   
+00015e10: 2020 2020 2020 2020 2073 656c 662e 6163           self.ac
+00015e20: 7469 6f6e 4461 726b 5f4d 6f64 655f 322e  tionDark_Mode_2.
+00015e30: 7365 7443 6865 636b 6564 2846 616c 7365  setChecked(False
+00015e40: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00015e50: 7269 675f 636f 6e74 726f 6c20 3d20 4e6f  rig_control = No
+00015e60: 6e65 0a0a 2020 2020 2020 2020 6966 2073  ne..        if s
+00015e70: 656c 662e 7072 6566 2e67 6574 2822 7573  elf.pref.get("us
+00015e80: 6566 6c72 6967 222c 2046 616c 7365 293a  eflrig", False):
+00015e90: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
+00015ea0: 6765 722e 6465 6275 6728 0a20 2020 2020  ger.debug(.     
+00015eb0: 2020 2020 2020 2020 2020 2022 5573 696e             "Usin
+00015ec0: 6720 666c 7269 673a 2025 7322 2c0a 2020  g flrig: %s",.  
+00015ed0: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+00015ee0: 7b73 656c 662e 7072 6566 2e67 6574 2827  {self.pref.get('
+00015ef0: 4341 545f 6970 2729 7d20 7b73 656c 662e  CAT_ip')} {self.
+00015f00: 7072 6566 2e67 6574 2827 4341 545f 706f  pref.get('CAT_po
+00015f10: 7274 2729 7d22 2c0a 2020 2020 2020 2020  rt')}",.        
+00015f20: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00015f30: 2020 7365 6c66 2e72 6967 5f63 6f6e 7472    self.rig_contr
+00015f40: 6f6c 203d 2043 4154 280a 2020 2020 2020  ol = CAT(.      
+00015f50: 2020 2020 2020 2020 2020 2266 6c72 6967            "flrig
+00015f60: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00015f70: 2020 2073 656c 662e 7072 6566 2e67 6574     self.pref.get
+00015f80: 2822 4341 545f 6970 222c 2022 3132 372e  ("CAT_ip", "127.
+00015f90: 302e 302e 3122 292c 0a20 2020 2020 2020  0.0.1"),.       
+00015fa0: 2020 2020 2020 2020 2069 6e74 2873 656c           int(sel
+00015fb0: 662e 7072 6566 2e67 6574 2822 4341 545f  f.pref.get("CAT_
+00015fc0: 706f 7274 222c 2031 3233 3435 2929 2c0a  port", 12345)),.
+00015fd0: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+00015fe0: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
+00015ff0: 7265 662e 6765 7428 2275 7365 7269 6763  ref.get("userigc
+00016000: 746c 6422 2c20 4661 6c73 6529 3a0a 2020  tld", False):.  
+00016010: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+00016020: 2e64 6562 7567 280a 2020 2020 2020 2020  .debug(.        
+00016030: 2020 2020 2020 2020 2255 7369 6e67 2072          "Using r
+00016040: 6967 6374 6c64 3a20 2573 222c 0a20 2020  igctld: %s",.   
+00016050: 2020 2020 2020 2020 2020 2020 2066 227b               f"{
+00016060: 7365 6c66 2e70 7265 662e 6765 7428 2743  self.pref.get('C
+00016070: 4154 5f69 7027 297d 207b 7365 6c66 2e70  AT_ip')} {self.p
+00016080: 7265 662e 6765 7428 2743 4154 5f70 6f72  ref.get('CAT_por
+00016090: 7427 297d 222c 0a20 2020 2020 2020 2020  t')}",.         
+000160a0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+000160b0: 2073 656c 662e 7269 675f 636f 6e74 726f   self.rig_contro
+000160c0: 6c20 3d20 4341 5428 0a20 2020 2020 2020  l = CAT(.       
+000160d0: 2020 2020 2020 2020 2022 7269 6763 746c           "rigctl
+000160e0: 6422 2c0a 2020 2020 2020 2020 2020 2020  d",.            
+000160f0: 2020 2020 7365 6c66 2e70 7265 662e 6765      self.pref.ge
+00016100: 7428 2243 4154 5f69 7022 2c20 2231 3237  t("CAT_ip", "127
+00016110: 2e30 2e30 2e31 2229 2c0a 2020 2020 2020  .0.0.1"),.      
+00016120: 2020 2020 2020 2020 2020 696e 7428 7365            int(se
+00016130: 6c66 2e70 7265 662e 6765 7428 2243 4154  lf.pref.get("CAT
+00016140: 5f70 6f72 7422 2c20 3435 3332 2929 2c0a  _port", 4532)),.
+00016150: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+00016160: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
+00016170: 7265 662e 6765 7428 2263 7774 7970 6522  ref.get("cwtype"
+00016180: 2c20 3029 203d 3d20 303a 0a20 2020 2020  , 0) == 0:.     
+00016190: 2020 2020 2020 2073 656c 662e 6377 203d         self.cw =
+000161a0: 204e 6f6e 650a 2020 2020 2020 2020 656c   None.        el
+000161b0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000161c0: 7365 6c66 2e63 7720 3d20 4357 280a 2020  self.cw = CW(.  
+000161d0: 2020 2020 2020 2020 2020 2020 2020 696e                in
+000161e0: 7428 7365 6c66 2e70 7265 662e 6765 7428  t(self.pref.get(
+000161f0: 2263 7774 7970 6522 2929 2c0a 2020 2020  "cwtype")),.    
+00016200: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016210: 2e70 7265 662e 6765 7428 2263 7769 7022  .pref.get("cwip"
+00016220: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00016230: 2020 2069 6e74 2873 656c 662e 7072 6566     int(self.pref
+00016240: 2e67 6574 2822 6377 706f 7274 222c 2036  .get("cwport", 6
+00016250: 3738 3929 292c 0a20 2020 2020 2020 2020  789)),.         
+00016260: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00016270: 2073 656c 662e 6377 2e73 7065 6564 203d   self.cw.speed =
+00016280: 2032 300a 2020 2020 2020 2020 2020 2020   20.            
+00016290: 6966 2073 656c 662e 6377 2e73 6572 7665  if self.cw.serve
+000162a0: 7274 7970 6520 3d3d 2032 3a0a 2020 2020  rtype == 2:.    
+000162b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000162c0: 2e63 772e 7365 745f 7769 6e6b 6579 6572  .cw.set_winkeyer
+000162d0: 5f73 7065 6564 2832 3029 0a0a 2020 2020  _speed(20)..    
+000162e0: 2020 2020 7365 6c66 2e6e 316d 6d20 3d20      self.n1mm = 
+000162f0: 4e6f 6e65 0a20 2020 2020 2020 2069 6620  None.        if 
+00016300: 7365 6c66 2e70 7265 662e 6765 7428 2273  self.pref.get("s
+00016310: 656e 645f 6e31 6d6d 5f70 6163 6b65 7473  end_n1mm_packets
+00016320: 222c 2046 616c 7365 293a 0a20 2020 2020  ", False):.     
+00016330: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+00016340: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016350: 2e6e 316d 6d20 3d20 4e31 4d4d 280a 2020  .n1mm = N1MM(.  
+00016360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016370: 2020 7365 6c66 2e70 7265 662e 6765 7428    self.pref.get(
+00016380: 226e 316d 6d5f 7261 6469 6f70 6f72 7422  "n1mm_radioport"
+00016390: 2c20 2231 3237 2e30 2e30 2e31 3a31 3230  , "127.0.0.1:120
+000163a0: 3630 2229 2c0a 2020 2020 2020 2020 2020  60"),.          
+000163b0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+000163c0: 7265 662e 6765 7428 226e 316d 6d5f 636f  ref.get("n1mm_co
+000163d0: 6e74 6163 7470 6f72 7422 2c20 2231 3237  ntactport", "127
+000163e0: 2e30 2e30 2e31 3a31 3230 3631 2229 2c0a  .0.0.1:12061"),.
+000163f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016400: 2020 2020 7365 6c66 2e70 7265 662e 6765      self.pref.ge
+00016410: 7428 226e 316d 6d5f 6c6f 6f6b 7570 706f  t("n1mm_lookuppo
+00016420: 7274 222c 2022 3132 372e 302e 302e 313a  rt", "127.0.0.1:
+00016430: 3132 3036 3022 292c 0a20 2020 2020 2020  12060"),.       
+00016440: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00016450: 662e 7072 6566 2e67 6574 2822 6e31 6d6d  f.pref.get("n1mm
+00016460: 5f73 636f 7265 706f 7274 222c 2022 3132  _scoreport", "12
+00016470: 372e 302e 302e 313a 3132 3036 3022 292c  7.0.0.1:12060"),
+00016480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016490: 2029 0a20 2020 2020 2020 2020 2020 2065   ).            e
+000164a0: 7863 6570 7420 5661 6c75 6545 7272 6f72  xcept ValueError
+000164b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000164c0: 2020 6c6f 6767 6572 2e77 6172 6e69 6e67    logger.warning
+000164d0: 2822 2573 222c 2066 227b 5661 6c75 6545  ("%s", f"{ValueE
+000164e0: 7272 6f72 7d22 290a 2020 2020 2020 2020  rror}").        
+000164f0: 2020 2020 7365 6c66 2e6e 316d 6d2e 7365      self.n1mm.se
+00016500: 6e64 5f72 6164 696f 5f70 6163 6b65 7473  nd_radio_packets
+00016510: 203d 2073 656c 662e 7072 6566 2e67 6574   = self.pref.get
+00016520: 2822 7365 6e64 5f6e 316d 6d5f 7261 6469  ("send_n1mm_radi
+00016530: 6f22 2c20 4661 6c73 6529 0a20 2020 2020  o", False).     
+00016540: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
+00016550: 2e73 656e 645f 636f 6e74 6163 745f 7061  .send_contact_pa
+00016560: 636b 6574 7320 3d20 7365 6c66 2e70 7265  ckets = self.pre
+00016570: 662e 6765 7428 2273 656e 645f 6e31 6d6d  f.get("send_n1mm
+00016580: 5f63 6f6e 7461 6374 222c 2046 616c 7365  _contact", False
+00016590: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+000165a0: 6c66 2e6e 316d 6d2e 7365 6e64 5f6c 6f6f  lf.n1mm.send_loo
+000165b0: 6b75 705f 7061 636b 6574 7320 3d20 7365  kup_packets = se
+000165c0: 6c66 2e70 7265 662e 6765 7428 2273 656e  lf.pref.get("sen
+000165d0: 645f 6e31 6d6d 5f6c 6f6f 6b75 7022 2c20  d_n1mm_lookup", 
+000165e0: 4661 6c73 6529 0a20 2020 2020 2020 2020  False).         
+000165f0: 2020 2073 656c 662e 6e31 6d6d 2e73 656e     self.n1mm.sen
+00016600: 645f 7363 6f72 655f 7061 636b 6574 7320  d_score_packets 
+00016610: 3d20 7365 6c66 2e70 7265 662e 6765 7428  = self.pref.get(
+00016620: 2273 656e 645f 6e31 6d6d 5f73 636f 7265  "send_n1mm_score
+00016630: 222c 2046 616c 7365 290a 2020 2020 2020  ", False).      
+00016640: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
+00016650: 7261 6469 6f5f 696e 666f 5b22 5374 6174  radio_info["Stat
+00016660: 696f 6e4e 616d 6522 5d20 3d20 7365 6c66  ionName"] = self
+00016670: 2e70 7265 662e 6765 7428 226e 316d 6d5f  .pref.get("n1mm_
+00016680: 7374 6174 696f 6e5f 6e61 6d65 222c 2022  station_name", "
+00016690: 2229 0a0a 2020 2020 2020 2020 7365 6c66  ")..        self
+000166a0: 2e73 686f 775f 636f 6d6d 616e 645f 6275  .show_command_bu
+000166b0: 7474 6f6e 7328 290a 2020 2020 2020 2020  ttons().        
+000166c0: 7365 6c66 2e73 686f 775f 4357 5f6d 6163  self.show_CW_mac
+000166d0: 726f 7328 290a 0a20 2020 2020 2020 2023  ros()..        #
+000166e0: 2049 6620 6261 6e64 7320 6c69 7374 2069   If bands list i
+000166f0: 7320 656d 7074 7920 6669 6c6c 2069 7420  s empty fill it 
+00016700: 7769 7468 2048 462e 0a20 2020 2020 2020  with HF..       
+00016710: 2069 6620 7365 6c66 2e70 7265 662e 6765   if self.pref.ge
+00016720: 7428 2262 616e 6473 222c 205b 5d29 203d  t("bands", []) =
+00016730: 3d20 5b5d 3a0a 2020 2020 2020 2020 2020  = []:.          
+00016740: 2020 7365 6c66 2e70 7265 665b 2262 616e    self.pref["ban
+00016750: 6473 225d 203d 205b 2231 3630 222c 2022  ds"] = ["160", "
+00016760: 3830 222c 2022 3430 222c 2022 3230 222c  80", "40", "20",
+00016770: 2022 3135 222c 2022 3130 225d 0a0a 2020   "15", "10"]..  
+00016780: 2020 2020 2020 2320 4869 6465 2061 6c6c        # Hide all
+00016790: 2074 6865 2062 616e 6473 2061 6e64 2074   the bands and t
+000167a0: 6865 6e20 7368 6f77 206f 6e6c 7920 7468  hen show only th
+000167b0: 6520 7761 6e74 6564 2062 616e 6473 2e0a  e wanted bands..
+000167c0: 2020 2020 2020 2020 666f 7220 5f69 6e64          for _ind
+000167d0: 6963 6174 6f72 2069 6e20 5b0a 2020 2020  icator in [.    
+000167e0: 2020 2020 2020 2020 7365 6c66 2e62 616e          self.ban
+000167f0: 645f 696e 6469 6361 746f 7273 5f63 772c  d_indicators_cw,
+00016800: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00016810: 662e 6261 6e64 5f69 6e64 6963 6174 6f72  f.band_indicator
+00016820: 735f 7373 622c 0a20 2020 2020 2020 2020  s_ssb,.         
+00016830: 2020 2073 656c 662e 6261 6e64 5f69 6e64     self.band_ind
+00016840: 6963 6174 6f72 735f 7274 7479 2c0a 2020  icators_rtty,.  
+00016850: 2020 2020 2020 5d3a 0a20 2020 2020 2020        ]:.       
+00016860: 2020 2020 2066 6f72 205f 6261 6e64 696e       for _bandin
+00016870: 6420 696e 205f 696e 6469 6361 746f 722e  d in _indicator.
+00016880: 7661 6c75 6573 2829 3a0a 2020 2020 2020  values():.      
+00016890: 2020 2020 2020 2020 2020 5f62 616e 6469            _bandi
+000168a0: 6e64 2e68 6964 6528 290a 2020 2020 2020  nd.hide().      
+000168b0: 2020 2020 2020 666f 7220 6261 6e64 5f74        for band_t
+000168c0: 6f5f 7368 6f77 2069 6e20 7365 6c66 2e70  o_show in self.p
+000168d0: 7265 662e 6765 7428 2262 616e 6473 222c  ref.get("bands",
+000168e0: 205b 5d29 3a0a 2020 2020 2020 2020 2020   []):.          
+000168f0: 2020 2020 2020 6966 2062 616e 645f 746f        if band_to
+00016900: 5f73 686f 7720 696e 205f 696e 6469 6361  _show in _indica
+00016910: 746f 723a 0a20 2020 2020 2020 2020 2020  tor:.           
+00016920: 2020 2020 2020 2020 205f 696e 6469 6361           _indica
+00016930: 746f 725b 6261 6e64 5f74 6f5f 7368 6f77  tor[band_to_show
+00016940: 5d2e 7368 6f77 2829 0a20 2020 2020 2020  ].show().       
+00016950: 2023 2073 656c 662e 7368 6f77 5f62 616e   # self.show_ban
+00016960: 645f 6d6f 6465 2829 0a0a 2020 2020 6465  d_mode()..    de
+00016970: 6620 7761 7463 685f 7564 7028 7365 6c66  f watch_udp(self
+00016980: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00016990: 2020 2022 2222 0a20 2020 2020 2020 2057     """.        W
+000169a0: 6174 6368 2074 6865 2055 4450 2073 6f63  atch the UDP soc
+000169b0: 6b65 7420 666f 7220 696e 636f 6d69 6e67  ket for incoming
+000169c0: 2064 6174 612e 0a0a 2020 2020 2020 2020   data...        
+000169d0: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+000169e0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+000169f0: 2020 2020 2020 4e6f 6e65 0a0a 2020 2020        None..    
+00016a00: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
+00016a10: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+00016a20: 2020 2020 4e6f 6e65 0a20 2020 2020 2020      None.       
+00016a30: 2022 2222 0a0a 2020 2020 2020 2020 7768   """..        wh
+00016a40: 696c 6520 7365 6c66 2e6d 756c 7469 6361  ile self.multica
+00016a50: 7374 5f69 6e74 6572 6661 6365 2e68 6173  st_interface.has
+00016a60: 5f70 656e 6469 6e67 5f64 6174 6167 7261  _pending_datagra
+00016a70: 6d73 2829 3a0a 2020 2020 2020 2020 2020  ms():.          
+00016a80: 2020 6a73 6f6e 5f64 6174 6120 3d20 7365    json_data = se
+00016a90: 6c66 2e6d 756c 7469 6361 7374 5f69 6e74  lf.multicast_int
+00016aa0: 6572 6661 6365 2e72 6561 645f 6461 7461  erface.read_data
+00016ab0: 6772 616d 5f61 735f 6a73 6f6e 2829 0a20  gram_as_json(). 
+00016ac0: 2020 2020 2020 2020 2020 2069 6620 6a73             if js
+00016ad0: 6f6e 5f64 6174 613a 0a20 2020 2020 2020  on_data:.       
+00016ae0: 2020 2020 2020 2020 2069 6620 280a 2020           if (.  
+00016af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016b00: 2020 6a73 6f6e 5f64 6174 612e 6765 7428    json_data.get(
+00016b10: 2263 6d64 222c 2022 2229 203d 3d20 2247  "cmd", "") == "G
+00016b20: 4554 434f 4c55 4d4e 5322 0a20 2020 2020  ETCOLUMNS".     
+00016b30: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00016b40: 6e64 206a 736f 6e5f 6461 7461 2e67 6574  nd json_data.get
+00016b50: 2822 7374 6174 696f 6e22 2c20 2222 2920  ("station", "") 
+00016b60: 3d3d 2070 6c61 7466 6f72 6d2e 6e6f 6465  == platform.node
+00016b70: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00016b80: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
+00016b90: 2020 2020 2020 2020 2020 6966 2068 6173            if has
+00016ba0: 6174 7472 2873 656c 662e 636f 6e74 6573  attr(self.contes
+00016bb0: 742c 2022 636f 6c75 6d6e 7322 293a 0a20  t, "columns"):. 
+00016bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016bd0: 2020 2020 2020 2063 6d64 203d 207b 7d0a         cmd = {}.
+00016be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016bf0: 2020 2020 2020 2020 636d 645b 2263 6d64          cmd["cmd
+00016c00: 225d 203d 2022 5348 4f57 434f 4c55 4d4e  "] = "SHOWCOLUMN
+00016c10: 5322 0a20 2020 2020 2020 2020 2020 2020  S".             
+00016c20: 2020 2020 2020 2020 2020 2063 6d64 5b22             cmd["
+00016c30: 7374 6174 696f 6e22 5d20 3d20 706c 6174  station"] = plat
+00016c40: 666f 726d 2e6e 6f64 6528 290a 2020 2020  form.node().    
+00016c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016c60: 2020 2020 636d 645b 2243 4f4c 554d 4e53      cmd["COLUMNS
+00016c70: 225d 203d 2073 656c 662e 636f 6e74 6573  "] = self.contes
+00016c80: 742e 636f 6c75 6d6e 730a 2020 2020 2020  t.columns.      
+00016c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ca0: 2020 7365 6c66 2e6d 756c 7469 6361 7374    self.multicast
+00016cb0: 5f69 6e74 6572 6661 6365 2e73 656e 645f  _interface.send_
+00016cc0: 6173 5f6a 736f 6e28 636d 6429 0a20 2020  as_json(cmd).   
+00016cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ce0: 2063 6f6e 7469 6e75 650a 2020 2020 2020   continue.      
+00016cf0: 2020 2020 2020 2020 2020 6966 2028 0a20            if (. 
 00016d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d10: 2020 636f 6e74 696e 7565 0a20 2020 2020    continue.     
-00016d20: 2020 2020 2020 2020 2020 2069 6620 280a             if (.
-00016d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d40: 2020 2020 6a73 6f6e 5f64 6174 612e 6765      json_data.ge
-00016d50: 7428 2263 6d64 222c 2022 2229 203d 3d20  t("cmd", "") == 
-00016d60: 2254 554e 4522 0a20 2020 2020 2020 2020  "TUNE".         
-00016d70: 2020 2020 2020 2020 2020 2061 6e64 206a             and j
-00016d80: 736f 6e5f 6461 7461 2e67 6574 2822 7374  son_data.get("st
-00016d90: 6174 696f 6e22 2c20 2222 2920 3d3d 2070  ation", "") == p
-00016da0: 6c61 7466 6f72 6d2e 6e6f 6465 2829 0a20  latform.node(). 
-00016db0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00016dc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00016dd0: 2020 2020 2020 2320 6227 7b22 636d 6422        # b'{"cmd"
-00016de0: 3a20 2254 554e 4522 2c20 2266 7265 7122  : "TUNE", "freq"
-00016df0: 3a20 372e 3032 3335 2c20 2273 706f 7422  : 7.0235, "spot"
-00016e00: 3a20 224d 4d30 4447 4922 7d27 0a20 2020  : "MM0DGI"}'.   
+00016d10: 2020 206a 736f 6e5f 6461 7461 2e67 6574     json_data.get
+00016d20: 2822 636d 6422 2c20 2222 2920 3d3d 2022  ("cmd", "") == "
+00016d30: 5455 4e45 220a 2020 2020 2020 2020 2020  TUNE".          
+00016d40: 2020 2020 2020 2020 2020 616e 6420 6a73            and js
+00016d50: 6f6e 5f64 6174 612e 6765 7428 2273 7461  on_data.get("sta
+00016d60: 7469 6f6e 222c 2022 2229 203d 3d20 706c  tion", "") == pl
+00016d70: 6174 666f 726d 2e6e 6f64 6528 290a 2020  atform.node().  
+00016d80: 2020 2020 2020 2020 2020 2020 2020 293a                ):
+00016d90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016da0: 2020 2020 2023 2062 277b 2263 6d64 223a       # b'{"cmd":
+00016db0: 2022 5455 4e45 222c 2022 6672 6571 223a   "TUNE", "freq":
+00016dc0: 2037 2e30 3233 352c 2022 7370 6f74 223a   7.0235, "spot":
+00016dd0: 2022 4d4d 3044 4749 227d 270a 2020 2020   "MM0DGI"}'.    
+00016de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016df0: 7666 6f20 3d20 6a73 6f6e 5f64 6174 612e  vfo = json_data.
+00016e00: 6765 7428 2266 7265 7122 290a 2020 2020  get("freq").    
 00016e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e20: 2076 666f 203d 206a 736f 6e5f 6461 7461   vfo = json_data
-00016e30: 2e67 6574 2822 6672 6571 2229 0a20 2020  .get("freq").   
-00016e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e50: 2076 666f 203d 2066 6c6f 6174 2876 666f   vfo = float(vfo
-00016e60: 2920 2a20 3130 3030 3030 300a 2020 2020  ) * 1000000.    
-00016e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e80: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
-00016e90: 5b22 7666 6f61 225d 203d 2069 6e74 2876  ["vfoa"] = int(v
-00016ea0: 666f 290a 2020 2020 2020 2020 2020 2020  fo).            
-00016eb0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00016ec0: 7269 675f 636f 6e74 726f 6c3a 0a20 2020  rig_control:.   
-00016ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ee0: 2020 2020 2073 656c 662e 7269 675f 636f       self.rig_co
-00016ef0: 6e74 726f 6c2e 7365 745f 7666 6f28 696e  ntrol.set_vfo(in
-00016f00: 7428 7666 6f29 290a 2020 2020 2020 2020  t(vfo)).        
-00016f10: 2020 2020 2020 2020 2020 2020 7370 6f74              spot
-00016f20: 203d 206a 736f 6e5f 6461 7461 2e67 6574   = json_data.get
-00016f30: 2822 7370 6f74 222c 2022 2229 0a20 2020  ("spot", "").   
+00016e20: 7666 6f20 3d20 666c 6f61 7428 7666 6f29  vfo = float(vfo)
+00016e30: 202a 2031 3030 3030 3030 0a20 2020 2020   * 1000000.     
+00016e40: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00016e50: 656c 662e 7261 6469 6f5f 7374 6174 655b  elf.radio_state[
+00016e60: 2276 666f 6122 5d20 3d20 696e 7428 7666  "vfoa"] = int(vf
+00016e70: 6f29 0a20 2020 2020 2020 2020 2020 2020  o).             
+00016e80: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+00016e90: 6967 5f63 6f6e 7472 6f6c 3a0a 2020 2020  ig_control:.    
+00016ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016eb0: 2020 2020 7365 6c66 2e72 6967 5f63 6f6e      self.rig_con
+00016ec0: 7472 6f6c 2e73 6574 5f76 666f 2869 6e74  trol.set_vfo(int
+00016ed0: 2876 666f 2929 0a20 2020 2020 2020 2020  (vfo)).         
+00016ee0: 2020 2020 2020 2020 2020 2073 706f 7420             spot 
+00016ef0: 3d20 6a73 6f6e 5f64 6174 612e 6765 7428  = json_data.get(
+00016f00: 2273 706f 7422 2c20 2222 290a 2020 2020  "spot", "").    
+00016f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016f20: 7365 6c66 2e63 616c 6c73 6967 6e2e 7365  self.callsign.se
+00016f30: 7454 6578 7428 7370 6f74 290a 2020 2020  tText(spot).    
 00016f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f50: 2073 656c 662e 6361 6c6c 7369 676e 2e73   self.callsign.s
-00016f60: 6574 5465 7874 2873 706f 7429 0a20 2020  etText(spot).   
-00016f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f80: 2073 656c 662e 6361 6c6c 7369 676e 5f63   self.callsign_c
-00016f90: 6861 6e67 6564 2829 0a20 2020 2020 2020  hanged().       
-00016fa0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00016fb0: 662e 6361 6c6c 7369 676e 2e73 6574 466f  f.callsign.setFo
-00016fc0: 6375 7328 290a 2020 2020 2020 2020 2020  cus().          
-00016fd0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00016fe0: 616c 6c73 6967 6e2e 6163 7469 7661 7465  allsign.activate
-00016ff0: 5769 6e64 6f77 2829 0a20 2020 2020 2020  Window().       
-00017000: 2020 2020 2020 2020 2020 2020 2077 696e               win
-00017010: 646f 772e 7261 6973 655f 2829 0a20 2020  dow.raise_().   
+00016f50: 7365 6c66 2e63 616c 6c73 6967 6e5f 6368  self.callsign_ch
+00016f60: 616e 6765 6428 290a 2020 2020 2020 2020  anged().        
+00016f70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016f80: 2e63 616c 6c73 6967 6e2e 7365 7446 6f63  .callsign.setFoc
+00016f90: 7573 2829 0a20 2020 2020 2020 2020 2020  us().           
+00016fa0: 2020 2020 2020 2020 2073 656c 662e 6361           self.ca
+00016fb0: 6c6c 7369 676e 2e61 6374 6976 6174 6557  llsign.activateW
+00016fc0: 696e 646f 7728 290a 2020 2020 2020 2020  indow().        
+00016fd0: 2020 2020 2020 2020 2020 2020 7769 6e64              wind
+00016fe0: 6f77 2e72 6169 7365 5f28 290a 2020 2020  ow.raise_().    
+00016ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017000: 636f 6e74 696e 7565 0a0a 2020 2020 2020  continue..      
+00017010: 2020 2020 2020 2020 2020 6966 2028 0a20            if (. 
 00017020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017030: 2063 6f6e 7469 6e75 650a 0a20 2020 2020   continue..     
-00017040: 2020 2020 2020 2020 2020 2069 6620 280a             if (.
-00017050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017060: 2020 2020 6a73 6f6e 5f64 6174 612e 6765      json_data.ge
-00017070: 7428 2263 6d64 222c 2022 2229 203d 3d20  t("cmd", "") == 
-00017080: 2247 4554 574f 524b 4544 4c49 5354 220a  "GETWORKEDLIST".
-00017090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000170a0: 2020 2020 616e 6420 6a73 6f6e 5f64 6174      and json_dat
-000170b0: 612e 6765 7428 2273 7461 7469 6f6e 222c  a.get("station",
-000170c0: 2022 2229 203d 3d20 706c 6174 666f 726d   "") == platform
-000170d0: 2e6e 6f64 6528 290a 2020 2020 2020 2020  .node().        
-000170e0: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
-000170f0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00017100: 6573 756c 7420 3d20 7365 6c66 2e64 6174  esult = self.dat
-00017110: 6162 6173 652e 6765 745f 6361 6c6c 735f  abase.get_calls_
-00017120: 616e 645f 6261 6e64 7328 290a 2020 2020  and_bands().    
-00017130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017140: 636d 6420 3d20 7b7d 0a20 2020 2020 2020  cmd = {}.       
-00017150: 2020 2020 2020 2020 2020 2020 2063 6d64               cmd
-00017160: 5b22 636d 6422 5d20 3d20 2257 4f52 4b45  ["cmd"] = "WORKE
-00017170: 4422 0a20 2020 2020 2020 2020 2020 2020  D".             
-00017180: 2020 2020 2020 2063 6d64 5b22 7374 6174         cmd["stat
-00017190: 696f 6e22 5d20 3d20 706c 6174 666f 726d  ion"] = platform
-000171a0: 2e6e 6f64 6528 290a 2020 2020 2020 2020  .node().        
-000171b0: 2020 2020 2020 2020 2020 2020 636d 645b              cmd[
-000171c0: 2277 6f72 6b65 6422 5d20 3d20 7265 7375  "worked"] = resu
-000171d0: 6c74 0a20 2020 2020 2020 2020 2020 2020  lt.             
-000171e0: 2020 2020 2020 2073 656c 662e 6d75 6c74         self.mult
-000171f0: 6963 6173 745f 696e 7465 7266 6163 652e  icast_interface.
-00017200: 7365 6e64 5f61 735f 6a73 6f6e 2863 6d64  send_as_json(cmd
-00017210: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00017220: 2020 2020 2020 636f 6e74 696e 7565 0a0a        continue..
-00017230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017240: 6966 2028 0a20 2020 2020 2020 2020 2020  if (.           
-00017250: 2020 2020 2020 2020 206a 736f 6e5f 6461           json_da
-00017260: 7461 2e67 6574 2822 636d 6422 2c20 2222  ta.get("cmd", ""
-00017270: 2920 3d3d 2022 4745 5443 4f4e 5445 5354  ) == "GETCONTEST
-00017280: 5354 4154 5553 220a 2020 2020 2020 2020  STATUS".        
-00017290: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-000172a0: 6a73 6f6e 5f64 6174 612e 6765 7428 2273  json_data.get("s
-000172b0: 7461 7469 6f6e 222c 2022 2229 203d 3d20  tation", "") == 
-000172c0: 706c 6174 666f 726d 2e6e 6f64 6528 290a  platform.node().
+00017030: 2020 206a 736f 6e5f 6461 7461 2e67 6574     json_data.get
+00017040: 2822 636d 6422 2c20 2222 2920 3d3d 2022  ("cmd", "") == "
+00017050: 4745 5457 4f52 4b45 444c 4953 5422 0a20  GETWORKEDLIST". 
+00017060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017070: 2020 2061 6e64 206a 736f 6e5f 6461 7461     and json_data
+00017080: 2e67 6574 2822 7374 6174 696f 6e22 2c20  .get("station", 
+00017090: 2222 2920 3d3d 2070 6c61 7466 6f72 6d2e  "") == platform.
+000170a0: 6e6f 6465 2829 0a20 2020 2020 2020 2020  node().         
+000170b0: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
+000170c0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+000170d0: 7375 6c74 203d 2073 656c 662e 6461 7461  sult = self.data
+000170e0: 6261 7365 2e67 6574 5f63 616c 6c73 5f61  base.get_calls_a
+000170f0: 6e64 5f62 616e 6473 2829 0a20 2020 2020  nd_bands().     
+00017100: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00017110: 6d64 203d 207b 7d0a 2020 2020 2020 2020  md = {}.        
+00017120: 2020 2020 2020 2020 2020 2020 636d 645b              cmd[
+00017130: 2263 6d64 225d 203d 2022 574f 524b 4544  "cmd"] = "WORKED
+00017140: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00017150: 2020 2020 2020 636d 645b 2273 7461 7469        cmd["stati
+00017160: 6f6e 225d 203d 2070 6c61 7466 6f72 6d2e  on"] = platform.
+00017170: 6e6f 6465 2829 0a20 2020 2020 2020 2020  node().         
+00017180: 2020 2020 2020 2020 2020 2063 6d64 5b22             cmd["
+00017190: 776f 726b 6564 225d 203d 2072 6573 756c  worked"] = resul
+000171a0: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+000171b0: 2020 2020 2020 7365 6c66 2e6d 756c 7469        self.multi
+000171c0: 6361 7374 5f69 6e74 6572 6661 6365 2e73  cast_interface.s
+000171d0: 656e 645f 6173 5f6a 736f 6e28 636d 6429  end_as_json(cmd)
+000171e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000171f0: 2020 2020 2063 6f6e 7469 6e75 650a 0a20       continue.. 
+00017200: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00017210: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
+00017220: 2020 2020 2020 2020 6a73 6f6e 5f64 6174          json_dat
+00017230: 612e 6765 7428 2263 6d64 222c 2022 2229  a.get("cmd", "")
+00017240: 203d 3d20 2247 4554 434f 4e54 4553 5453   == "GETCONTESTS
+00017250: 5441 5455 5322 0a20 2020 2020 2020 2020  TATUS".         
+00017260: 2020 2020 2020 2020 2020 2061 6e64 206a             and j
+00017270: 736f 6e5f 6461 7461 2e67 6574 2822 7374  son_data.get("st
+00017280: 6174 696f 6e22 2c20 2222 2920 3d3d 2070  ation", "") == p
+00017290: 6c61 7466 6f72 6d2e 6e6f 6465 2829 0a20  latform.node(). 
+000172a0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+000172b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000172c0: 2020 2020 2020 636d 6420 3d20 7b0a 2020        cmd = {.  
 000172d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000172e0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000172f0: 2020 2020 2020 2063 6d64 203d 207b 0a20         cmd = {. 
+000172e0: 2020 2020 2020 2263 6d64 223a 2022 434f        "cmd": "CO
+000172f0: 4e54 4553 5453 5441 5455 5322 2c0a 2020  NTESTSTATUS",.  
 00017300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017310: 2020 2020 2020 2022 636d 6422 3a20 2243         "cmd": "C
-00017320: 4f4e 5445 5354 5354 4154 5553 222c 0a20  ONTESTSTATUS",. 
-00017330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017340: 2020 2020 2020 2022 7374 6174 696f 6e22         "station"
-00017350: 3a20 706c 6174 666f 726d 2e6e 6f64 6528  : platform.node(
-00017360: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00017370: 2020 2020 2020 2020 2020 2022 636f 6e74             "cont
-00017380: 6573 7422 3a20 7365 6c66 2e63 6f6e 7465  est": self.conte
-00017390: 7374 5f73 6574 7469 6e67 732c 0a20 2020  st_settings,.   
-000173a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000173b0: 2020 2020 2022 6f70 6572 6174 6f72 223a       "operator":
-000173c0: 2073 656c 662e 6375 7272 656e 745f 6f70   self.current_op
-000173d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000173e0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-000173f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00017400: 2e6d 756c 7469 6361 7374 5f69 6e74 6572  .multicast_inter
-00017410: 6661 6365 2e73 656e 645f 6173 5f6a 736f  face.send_as_jso
-00017420: 6e28 636d 6429 0a20 2020 2020 2020 2020  n(cmd).         
-00017430: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
-00017440: 6e75 650a 0a20 2020 2020 2020 2020 2020  nue..           
-00017450: 2020 2020 2069 6620 280a 2020 2020 2020       if (.      
-00017460: 2020 2020 2020 2020 2020 2020 2020 6a73                js
-00017470: 6f6e 5f64 6174 612e 6765 7428 2263 6d64  on_data.get("cmd
-00017480: 222c 2022 2229 203d 3d20 2243 4841 4e47  ", "") == "CHANG
-00017490: 4543 414c 4c22 0a20 2020 2020 2020 2020  ECALL".         
-000174a0: 2020 2020 2020 2020 2020 2061 6e64 206a             and j
-000174b0: 736f 6e5f 6461 7461 2e67 6574 2822 7374  son_data.get("st
-000174c0: 6174 696f 6e22 2c20 2222 2920 3d3d 2070  ation", "") == p
-000174d0: 6c61 7466 6f72 6d2e 6e6f 6465 2829 0a20  latform.node(). 
-000174e0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-000174f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00017500: 2020 2020 2020 7365 6c66 2e63 616c 6c73        self.calls
-00017510: 6967 6e2e 7365 7454 6578 7428 6a73 6f6e  ign.setText(json
-00017520: 5f64 6174 612e 6765 7428 2263 616c 6c22  _data.get("call"
-00017530: 2c20 2222 2929 0a20 2020 2020 2020 2020  , "")).         
-00017540: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00017550: 6361 6c6c 7369 676e 2e73 6574 466f 6375  callsign.setFocu
-00017560: 7328 290a 0a20 2020 2064 6566 2064 6172  s()..    def dar
-00017570: 6b5f 6d6f 6465 5f73 7461 7465 5f63 6861  k_mode_state_cha
-00017580: 6e67 6564 2873 656c 6629 202d 3e20 4e6f  nged(self) -> No
-00017590: 6e65 3a0a 2020 2020 2020 2020 2222 2243  ne:.        """C
-000175a0: 616c 6c65 6420 7768 656e 2074 6865 2044  alled when the D
-000175b0: 6172 6b20 4d6f 6465 206d 656e 7520 7374  ark Mode menu st
-000175c0: 6174 6520 6973 2063 6861 6e67 6564 2e22  ate is changed."
-000175d0: 2222 0a20 2020 2020 2020 2073 656c 662e  "".        self.
-000175e0: 7072 6566 5b22 6461 726b 6d6f 6465 225d  pref["darkmode"]
-000175f0: 203d 2073 656c 662e 6163 7469 6f6e 4461   = self.actionDa
-00017600: 726b 5f4d 6f64 655f 322e 6973 4368 6563  rk_Mode_2.isChec
-00017610: 6b65 6428 290a 2020 2020 2020 2020 7365  ked().        se
-00017620: 6c66 2e77 7269 7465 5f70 7265 6665 7265  lf.write_prefere
-00017630: 6e63 6528 290a 2020 2020 2020 2020 7365  nce().        se
-00017640: 6c66 2e73 6574 4461 726b 4d6f 6465 2873  lf.setDarkMode(s
-00017650: 656c 662e 6163 7469 6f6e 4461 726b 5f4d  elf.actionDark_M
-00017660: 6f64 655f 322e 6973 4368 6563 6b65 6428  ode_2.isChecked(
-00017670: 2929 0a0a 2020 2020 6465 6620 6377 5f6d  ))..    def cw_m
-00017680: 6163 726f 735f 7374 6174 655f 6368 616e  acros_state_chan
-00017690: 6765 6428 7365 6c66 2920 2d3e 204e 6f6e  ged(self) -> Non
-000176a0: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
-000176b0: 2020 2020 2020 204d 656e 7520 6974 656d         Menu item
-000176c0: 2074 6f20 7368 6f77 2f68 6964 6520 6d61   to show/hide ma
-000176d0: 6372 6f20 6275 7474 6f6e 732e 0a0a 2020  cro buttons...  
-000176e0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+00017310: 2020 2020 2020 2273 7461 7469 6f6e 223a        "station":
+00017320: 2070 6c61 7466 6f72 6d2e 6e6f 6465 2829   platform.node()
+00017330: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00017340: 2020 2020 2020 2020 2020 2263 6f6e 7465            "conte
+00017350: 7374 223a 2073 656c 662e 636f 6e74 6573  st": self.contes
+00017360: 745f 7365 7474 696e 6773 2c0a 2020 2020  t_settings,.    
+00017370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017380: 2020 2020 226f 7065 7261 746f 7222 3a20      "operator": 
+00017390: 7365 6c66 2e63 7572 7265 6e74 5f6f 702c  self.current_op,
+000173a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000173b0: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
+000173c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000173d0: 6d75 6c74 6963 6173 745f 696e 7465 7266  multicast_interf
+000173e0: 6163 652e 7365 6e64 5f61 735f 6a73 6f6e  ace.send_as_json
+000173f0: 2863 6d64 290a 2020 2020 2020 2020 2020  (cmd).          
+00017400: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
+00017410: 7565 0a0a 2020 2020 2020 2020 2020 2020  ue..            
+00017420: 2020 2020 6966 2028 0a20 2020 2020 2020      if (.       
+00017430: 2020 2020 2020 2020 2020 2020 206a 736f               jso
+00017440: 6e5f 6461 7461 2e67 6574 2822 636d 6422  n_data.get("cmd"
+00017450: 2c20 2222 2920 3d3d 2022 4348 414e 4745  , "") == "CHANGE
+00017460: 4341 4c4c 220a 2020 2020 2020 2020 2020  CALL".          
+00017470: 2020 2020 2020 2020 2020 616e 6420 6a73            and js
+00017480: 6f6e 5f64 6174 612e 6765 7428 2273 7461  on_data.get("sta
+00017490: 7469 6f6e 222c 2022 2229 203d 3d20 706c  tion", "") == pl
+000174a0: 6174 666f 726d 2e6e 6f64 6528 290a 2020  atform.node().  
+000174b0: 2020 2020 2020 2020 2020 2020 2020 293a                ):
+000174c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000174d0: 2020 2020 2073 656c 662e 6361 6c6c 7369       self.callsi
+000174e0: 676e 2e73 6574 5465 7874 286a 736f 6e5f  gn.setText(json_
+000174f0: 6461 7461 2e67 6574 2822 6361 6c6c 222c  data.get("call",
+00017500: 2022 2229 290a 2020 2020 2020 2020 2020   "")).          
+00017510: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00017520: 616c 6c73 6967 6e2e 7365 7446 6f63 7573  allsign.setFocus
+00017530: 2829 0a0a 2020 2020 6465 6620 6461 726b  ()..    def dark
+00017540: 5f6d 6f64 655f 7374 6174 655f 6368 616e  _mode_state_chan
+00017550: 6765 6428 7365 6c66 2920 2d3e 204e 6f6e  ged(self) -> Non
+00017560: 653a 0a20 2020 2020 2020 2022 2222 4361  e:.        """Ca
+00017570: 6c6c 6564 2077 6865 6e20 7468 6520 4461  lled when the Da
+00017580: 726b 204d 6f64 6520 6d65 6e75 2073 7461  rk Mode menu sta
+00017590: 7465 2069 7320 6368 616e 6765 642e 2222  te is changed.""
+000175a0: 220a 2020 2020 2020 2020 7365 6c66 2e70  ".        self.p
+000175b0: 7265 665b 2264 6172 6b6d 6f64 6522 5d20  ref["darkmode"] 
+000175c0: 3d20 7365 6c66 2e61 6374 696f 6e44 6172  = self.actionDar
+000175d0: 6b5f 4d6f 6465 5f32 2e69 7343 6865 636b  k_Mode_2.isCheck
+000175e0: 6564 2829 0a20 2020 2020 2020 2073 656c  ed().        sel
+000175f0: 662e 7772 6974 655f 7072 6566 6572 656e  f.write_preferen
+00017600: 6365 2829 0a20 2020 2020 2020 2073 656c  ce().        sel
+00017610: 662e 7365 7444 6172 6b4d 6f64 6528 7365  f.setDarkMode(se
+00017620: 6c66 2e61 6374 696f 6e44 6172 6b5f 4d6f  lf.actionDark_Mo
+00017630: 6465 5f32 2e69 7343 6865 636b 6564 2829  de_2.isChecked()
+00017640: 290a 0a20 2020 2064 6566 2063 775f 6d61  )..    def cw_ma
+00017650: 6372 6f73 5f73 7461 7465 5f63 6861 6e67  cros_state_chang
+00017660: 6564 2873 656c 6629 202d 3e20 4e6f 6e65  ed(self) -> None
+00017670: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00017680: 2020 2020 2020 4d65 6e75 2069 7465 6d20        Menu item 
+00017690: 746f 2073 686f 772f 6869 6465 206d 6163  to show/hide mac
+000176a0: 726f 2062 7574 746f 6e73 2e0a 0a20 2020  ro buttons...   
+000176b0: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
+000176c0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+000176d0: 2d2d 0a20 2020 2020 2020 204e 6f6e 650a  --.        None.
+000176e0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
 000176f0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00017700: 2d2d 2d0a 2020 2020 2020 2020 4e6f 6e65  ---.        None
-00017710: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00017720: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-00017730: 2d0a 2020 2020 2020 2020 4e6f 6e65 0a20  -.        None. 
-00017740: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
-00017750: 2020 2020 7365 6c66 2e70 7265 665b 2263      self.pref["c
-00017760: 775f 6d61 6372 6f73 225d 203d 2073 656c  w_macros"] = sel
-00017770: 662e 6163 7469 6f6e 4357 5f4d 6163 726f  f.actionCW_Macro
-00017780: 732e 6973 4368 6563 6b65 6428 290a 2020  s.isChecked().  
-00017790: 2020 2020 2020 7365 6c66 2e77 7269 7465        self.write
-000177a0: 5f70 7265 6665 7265 6e63 6528 290a 2020  _preference().  
-000177b0: 2020 2020 2020 7365 6c66 2e73 686f 775f        self.show_
-000177c0: 4357 5f6d 6163 726f 7328 290a 0a20 2020  CW_macros()..   
-000177d0: 2064 6566 2073 686f 775f 4357 5f6d 6163   def show_CW_mac
-000177e0: 726f 7328 7365 6c66 2920 2d3e 204e 6f6e  ros(self) -> Non
-000177f0: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
-00017800: 2020 2020 2020 2053 686f 772f 4869 6465         Show/Hide
-00017810: 2074 6865 206d 6163 726f 2062 7574 746f   the macro butto
-00017820: 6e73 2e0a 0a20 2020 2020 2020 2050 6172  ns...        Par
-00017830: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
-00017840: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-00017850: 2020 204e 6f6e 650a 0a20 2020 2020 2020     None..       
-00017860: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
-00017870: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
-00017880: 204e 6f6e 650a 2020 2020 2020 2020 2222   None.        ""
-00017890: 220a 0a20 2020 2020 2020 2069 6620 7365  "..        if se
-000178a0: 6c66 2e70 7265 662e 6765 7428 2263 775f  lf.pref.get("cw_
-000178b0: 6d61 6372 6f73 2229 3a0a 2020 2020 2020  macros"):.      
-000178c0: 2020 2020 2020 7365 6c66 2e42 7574 746f        self.Butto
-000178d0: 6e5f 526f 7731 2e73 686f 7728 290a 2020  n_Row1.show().  
-000178e0: 2020 2020 2020 2020 2020 7365 6c66 2e42            self.B
-000178f0: 7574 746f 6e5f 526f 7732 2e73 686f 7728  utton_Row2.show(
-00017900: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-00017910: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00017920: 2e42 7574 746f 6e5f 526f 7731 2e68 6964  .Button_Row1.hid
-00017930: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
-00017940: 7365 6c66 2e42 7574 746f 6e5f 526f 7732  self.Button_Row2
-00017950: 2e68 6964 6528 290a 0a20 2020 2064 6566  .hide()..    def
-00017960: 2063 6f6d 6d61 6e64 5f62 7574 746f 6e73   command_buttons
-00017970: 5f73 7461 7465 5f63 6861 6e67 6528 7365  _state_change(se
-00017980: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
-00017990: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000179a0: 204d 656e 7520 6974 656d 2074 6f20 7368   Menu item to sh
-000179b0: 6f77 2f68 6964 6520 636f 6d6d 616e 6420  ow/hide command 
-000179c0: 6275 7474 6f6e 730a 0a20 2020 2020 2020  buttons..       
-000179d0: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-000179e0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-000179f0: 2020 2020 2020 204e 6f6e 650a 0a20 2020         None..   
-00017a00: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
-00017a10: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
-00017a20: 2020 2020 204e 6f6e 650a 2020 2020 2020       None.      
-00017a30: 2020 2222 220a 0a20 2020 2020 2020 2073    """..        s
-00017a40: 656c 662e 7072 6566 5b22 636f 6d6d 616e  elf.pref["comman
-00017a50: 645f 6275 7474 6f6e 7322 5d20 3d20 7365  d_buttons"] = se
-00017a60: 6c66 2e61 6374 696f 6e43 6f6d 6d61 6e64  lf.actionCommand
-00017a70: 5f42 7574 746f 6e73 2e69 7343 6865 636b  _Buttons.isCheck
-00017a80: 6564 2829 0a20 2020 2020 2020 2073 656c  ed().        sel
-00017a90: 662e 7772 6974 655f 7072 6566 6572 656e  f.write_preferen
-00017aa0: 6365 2829 0a20 2020 2020 2020 2073 656c  ce().        sel
-00017ab0: 662e 7368 6f77 5f63 6f6d 6d61 6e64 5f62  f.show_command_b
-00017ac0: 7574 746f 6e73 2829 0a0a 2020 2020 6465  uttons()..    de
-00017ad0: 6620 7368 6f77 5f63 6f6d 6d61 6e64 5f62  f show_command_b
-00017ae0: 7574 746f 6e73 2873 656c 6629 202d 3e20  uttons(self) -> 
-00017af0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-00017b00: 220a 2020 2020 2020 2020 5368 6f77 2f48  ".        Show/H
-00017b10: 6964 6520 7468 6520 636f 6d6d 616e 6420  ide the command 
-00017b20: 6275 7474 6f6e 7320 6465 7065 6e64 696e  buttons dependin
-00017b30: 6720 6f6e 2074 6865 2070 7265 6665 7265  g on the prefere
-00017b40: 6e63 652e 0a0a 2020 2020 2020 2020 5061  nce...        Pa
-00017b50: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
-00017b60: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00017b70: 2020 2020 4e6f 6e65 0a0a 2020 2020 2020      None..      
-00017b80: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
-00017b90: 2020 2d2d 2d2d 2d2d 2d0a 0a20 2020 2020    -------..     
-00017ba0: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
-00017bb0: 6966 2073 656c 662e 7072 6566 2e67 6574  if self.pref.get
-00017bc0: 2822 636f 6d6d 616e 645f 6275 7474 6f6e  ("command_button
-00017bd0: 7322 293a 0a20 2020 2020 2020 2020 2020  s"):.           
-00017be0: 2073 656c 662e 436f 6d6d 616e 645f 4275   self.Command_Bu
-00017bf0: 7474 6f6e 732e 7368 6f77 2829 0a20 2020  ttons.show().   
-00017c00: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00017c10: 2020 2020 2020 2073 656c 662e 436f 6d6d         self.Comm
-00017c20: 616e 645f 4275 7474 6f6e 732e 6869 6465  and_Buttons.hide
-00017c30: 2829 0a0a 2020 2020 6465 6620 6973 5f66  ()..    def is_f
-00017c40: 6c6f 6174 6162 6c65 2873 656c 662c 2069  loatable(self, i
-00017c50: 7465 6d3a 2073 7472 2920 2d3e 2062 6f6f  tem: str) -> boo
-00017c60: 6c3a 0a20 2020 2020 2020 2022 2222 0a20  l:.        """. 
-00017c70: 2020 2020 2020 2043 6865 636b 2074 6f20         Check to 
-00017c80: 7365 6520 6966 2073 7472 696e 6720 6361  see if string ca
-00017c90: 6e20 6265 2061 2066 6c6f 6174 2e0a 0a20  n be a float... 
-00017ca0: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-00017cb0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-00017cc0: 2d2d 2d2d 0a20 2020 2020 2020 2069 7465  ----.        ite
-00017cd0: 6d20 3a20 7374 720a 2020 2020 2020 2020  m : str.        
-00017ce0: 5468 6520 7374 7269 6e67 2074 6f20 7465  The string to te
-00017cf0: 7374 2e0a 0a20 2020 2020 2020 2052 6574  st...        Ret
-00017d00: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
-00017d10: 2d2d 2d2d 0a20 2020 2020 2020 2062 6f6f  ----.        boo
-00017d20: 6c0a 2020 2020 2020 2020 5472 7565 2069  l.        True i
-00017d30: 6620 7374 7269 6e67 2063 616e 2062 6520  f string can be 
-00017d40: 6120 666c 6f61 742c 2046 616c 7365 206f  a float, False o
-00017d50: 7468 6572 7769 7365 2e0a 2020 2020 2020  therwise..      
-00017d60: 2020 2222 220a 0a20 2020 2020 2020 2069    """..        i
-00017d70: 6620 6974 656d 2e69 736e 756d 6572 6963  f item.isnumeric
-00017d80: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00017d90: 7265 7475 726e 2054 7275 650a 2020 2020  return True.    
-00017da0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00017db0: 2020 2020 205f 7465 7374 203d 2066 6c6f       _test = flo
-00017dc0: 6174 2869 7465 6d29 0a20 2020 2020 2020  at(item).       
-00017dd0: 2065 7863 6570 7420 5661 6c75 6545 7272   except ValueErr
-00017de0: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
-00017df0: 7265 7475 726e 2046 616c 7365 0a20 2020  return False.   
-00017e00: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-00017e10: 0a0a 2020 2020 6465 6620 6f74 6865 725f  ..    def other_
-00017e20: 315f 6368 616e 6765 6428 7365 6c66 2920  1_changed(self) 
-00017e30: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00017e40: 2022 2222 0a20 2020 2020 2020 2054 6865   """.        The
-00017e50: 2074 6578 7420 696e 2074 6865 206f 7468   text in the oth
-00017e60: 6572 5f31 2066 6965 6c64 2068 6173 2063  er_1 field has c
-00017e70: 6861 6e67 6564 2e0a 2020 2020 2020 2020  hanged..        
-00017e80: 5374 7269 7020 6f75 7420 616e 7920 7370  Strip out any sp
-00017e90: 6163 6573 2061 6e64 2073 6574 2074 6865  aces and set the
-00017ea0: 2074 6578 742e 0a0a 2020 2020 2020 2020   text...        
-00017eb0: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
-00017ec0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-00017ed0: 2020 2020 2020 4e6f 6e65 0a0a 2020 2020        None..    
-00017ee0: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-00017ef0: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-00017f00: 2020 2020 4e6f 6e65 0a20 2020 2020 2020      None.       
-00017f10: 2022 2222 0a0a 2020 2020 2020 2020 6966   """..        if
-00017f20: 2073 656c 662e 636f 6e74 6573 743a 0a20   self.contest:. 
-00017f30: 2020 2020 2020 2020 2020 2069 6620 6861             if ha
-00017f40: 7361 7474 7228 7365 6c66 2e63 6f6e 7465  sattr(self.conte
-00017f50: 7374 2c20 2261 6476 616e 6365 5f6f 6e5f  st, "advance_on_
-00017f60: 7370 6163 6522 293a 0a20 2020 2020 2020  space"):.       
-00017f70: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00017f80: 2e63 6f6e 7465 7374 2e61 6476 616e 6365  .contest.advance
-00017f90: 5f6f 6e5f 7370 6163 655b 335d 3a0a 2020  _on_space[3]:.  
+00017700: 0a20 2020 2020 2020 204e 6f6e 650a 2020  .        None.  
+00017710: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
+00017720: 2020 2073 656c 662e 7072 6566 5b22 6377     self.pref["cw
+00017730: 5f6d 6163 726f 7322 5d20 3d20 7365 6c66  _macros"] = self
+00017740: 2e61 6374 696f 6e43 575f 4d61 6372 6f73  .actionCW_Macros
+00017750: 2e69 7343 6865 636b 6564 2829 0a20 2020  .isChecked().   
+00017760: 2020 2020 2073 656c 662e 7772 6974 655f       self.write_
+00017770: 7072 6566 6572 656e 6365 2829 0a20 2020  preference().   
+00017780: 2020 2020 2073 656c 662e 7368 6f77 5f43       self.show_C
+00017790: 575f 6d61 6372 6f73 2829 0a0a 2020 2020  W_macros()..    
+000177a0: 6465 6620 7368 6f77 5f43 575f 6d61 6372  def show_CW_macr
+000177b0: 6f73 2873 656c 6629 202d 3e20 4e6f 6e65  os(self) -> None
+000177c0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+000177d0: 2020 2020 2020 5368 6f77 2f48 6964 6520        Show/Hide 
+000177e0: 7468 6520 6d61 6372 6f20 6275 7474 6f6e  the macro button
+000177f0: 732e 0a0a 2020 2020 2020 2020 5061 7261  s...        Para
+00017800: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
+00017810: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+00017820: 2020 4e6f 6e65 0a0a 2020 2020 2020 2020    None..        
+00017830: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
+00017840: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00017850: 4e6f 6e65 0a20 2020 2020 2020 2022 2222  None.        """
+00017860: 0a0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
+00017870: 662e 7072 6566 2e67 6574 2822 6377 5f6d  f.pref.get("cw_m
+00017880: 6163 726f 7322 293a 0a20 2020 2020 2020  acros"):.       
+00017890: 2020 2020 2073 656c 662e 4275 7474 6f6e       self.Button
+000178a0: 5f52 6f77 312e 7368 6f77 2829 0a20 2020  _Row1.show().   
+000178b0: 2020 2020 2020 2020 2073 656c 662e 4275           self.Bu
+000178c0: 7474 6f6e 5f52 6f77 322e 7368 6f77 2829  tton_Row2.show()
+000178d0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+000178e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000178f0: 4275 7474 6f6e 5f52 6f77 312e 6869 6465  Button_Row1.hide
+00017900: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
+00017910: 656c 662e 4275 7474 6f6e 5f52 6f77 322e  elf.Button_Row2.
+00017920: 6869 6465 2829 0a0a 2020 2020 6465 6620  hide()..    def 
+00017930: 636f 6d6d 616e 645f 6275 7474 6f6e 735f  command_buttons_
+00017940: 7374 6174 655f 6368 616e 6765 2873 656c  state_change(sel
+00017950: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+00017960: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00017970: 4d65 6e75 2069 7465 6d20 746f 2073 686f  Menu item to sho
+00017980: 772f 6869 6465 2063 6f6d 6d61 6e64 2062  w/hide command b
+00017990: 7574 746f 6e73 0a0a 2020 2020 2020 2020  uttons..        
+000179a0: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+000179b0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+000179c0: 2020 2020 2020 4e6f 6e65 0a0a 2020 2020        None..    
+000179d0: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
+000179e0: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+000179f0: 2020 2020 4e6f 6e65 0a20 2020 2020 2020      None.       
+00017a00: 2022 2222 0a0a 2020 2020 2020 2020 7365   """..        se
+00017a10: 6c66 2e70 7265 665b 2263 6f6d 6d61 6e64  lf.pref["command
+00017a20: 5f62 7574 746f 6e73 225d 203d 2073 656c  _buttons"] = sel
+00017a30: 662e 6163 7469 6f6e 436f 6d6d 616e 645f  f.actionCommand_
+00017a40: 4275 7474 6f6e 732e 6973 4368 6563 6b65  Buttons.isChecke
+00017a50: 6428 290a 2020 2020 2020 2020 7365 6c66  d().        self
+00017a60: 2e77 7269 7465 5f70 7265 6665 7265 6e63  .write_preferenc
+00017a70: 6528 290a 2020 2020 2020 2020 7365 6c66  e().        self
+00017a80: 2e73 686f 775f 636f 6d6d 616e 645f 6275  .show_command_bu
+00017a90: 7474 6f6e 7328 290a 0a20 2020 2064 6566  ttons()..    def
+00017aa0: 2073 686f 775f 636f 6d6d 616e 645f 6275   show_command_bu
+00017ab0: 7474 6f6e 7328 7365 6c66 2920 2d3e 204e  ttons(self) -> N
+00017ac0: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+00017ad0: 0a20 2020 2020 2020 2053 686f 772f 4869  .        Show/Hi
+00017ae0: 6465 2074 6865 2063 6f6d 6d61 6e64 2062  de the command b
+00017af0: 7574 746f 6e73 2064 6570 656e 6469 6e67  uttons depending
+00017b00: 206f 6e20 7468 6520 7072 6566 6572 656e   on the preferen
+00017b10: 6365 2e0a 0a20 2020 2020 2020 2050 6172  ce...        Par
+00017b20: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
+00017b30: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+00017b40: 2020 204e 6f6e 650a 0a20 2020 2020 2020     None..       
+00017b50: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
+00017b60: 202d 2d2d 2d2d 2d2d 0a0a 2020 2020 2020   -------..      
+00017b70: 2020 2222 220a 0a20 2020 2020 2020 2069    """..        i
+00017b80: 6620 7365 6c66 2e70 7265 662e 6765 7428  f self.pref.get(
+00017b90: 2263 6f6d 6d61 6e64 5f62 7574 746f 6e73  "command_buttons
+00017ba0: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
+00017bb0: 7365 6c66 2e43 6f6d 6d61 6e64 5f42 7574  self.Command_But
+00017bc0: 746f 6e73 2e73 686f 7728 290a 2020 2020  tons.show().    
+00017bd0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00017be0: 2020 2020 2020 7365 6c66 2e43 6f6d 6d61        self.Comma
+00017bf0: 6e64 5f42 7574 746f 6e73 2e68 6964 6528  nd_Buttons.hide(
+00017c00: 290a 0a20 2020 2064 6566 2069 735f 666c  )..    def is_fl
+00017c10: 6f61 7461 626c 6528 7365 6c66 2c20 6974  oatable(self, it
+00017c20: 656d 3a20 7374 7229 202d 3e20 626f 6f6c  em: str) -> bool
+00017c30: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00017c40: 2020 2020 2020 4368 6563 6b20 746f 2073        Check to s
+00017c50: 6565 2069 6620 7374 7269 6e67 2063 616e  ee if string can
+00017c60: 2062 6520 6120 666c 6f61 742e 0a0a 2020   be a float...  
+00017c70: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+00017c80: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00017c90: 2d2d 2d0a 2020 2020 2020 2020 6974 656d  ---.        item
+00017ca0: 203a 2073 7472 0a20 2020 2020 2020 2054   : str.        T
+00017cb0: 6865 2073 7472 696e 6720 746f 2074 6573  he string to tes
+00017cc0: 742e 0a0a 2020 2020 2020 2020 5265 7475  t...        Retu
+00017cd0: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
+00017ce0: 2d2d 2d0a 2020 2020 2020 2020 626f 6f6c  ---.        bool
+00017cf0: 0a20 2020 2020 2020 2054 7275 6520 6966  .        True if
+00017d00: 2073 7472 696e 6720 6361 6e20 6265 2061   string can be a
+00017d10: 2066 6c6f 6174 2c20 4661 6c73 6520 6f74   float, False ot
+00017d20: 6865 7277 6973 652e 0a20 2020 2020 2020  herwise..       
+00017d30: 2022 2222 0a0a 2020 2020 2020 2020 6966   """..        if
+00017d40: 2069 7465 6d2e 6973 6e75 6d65 7269 6328   item.isnumeric(
+00017d50: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+00017d60: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
+00017d70: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00017d80: 2020 2020 5f74 6573 7420 3d20 666c 6f61      _test = floa
+00017d90: 7428 6974 656d 290a 2020 2020 2020 2020  t(item).        
+00017da0: 6578 6365 7074 2056 616c 7565 4572 726f  except ValueErro
+00017db0: 723a 0a20 2020 2020 2020 2020 2020 2072  r:.            r
+00017dc0: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
+00017dd0: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+00017de0: 0a20 2020 2064 6566 206f 7468 6572 5f31  .    def other_1
+00017df0: 5f63 6861 6e67 6564 2873 656c 6629 202d  _changed(self) -
+00017e00: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00017e10: 2222 220a 2020 2020 2020 2020 5468 6520  """.        The 
+00017e20: 7465 7874 2069 6e20 7468 6520 6f74 6865  text in the othe
+00017e30: 725f 3120 6669 656c 6420 6861 7320 6368  r_1 field has ch
+00017e40: 616e 6765 642e 0a20 2020 2020 2020 2053  anged..        S
+00017e50: 7472 6970 206f 7574 2061 6e79 2073 7061  trip out any spa
+00017e60: 6365 7320 616e 6420 7365 7420 7468 6520  ces and set the 
+00017e70: 7465 7874 2e0a 0a20 2020 2020 2020 2050  text...        P
+00017e80: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+00017e90: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+00017ea0: 2020 2020 204e 6f6e 650a 0a20 2020 2020       None..     
+00017eb0: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
+00017ec0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
+00017ed0: 2020 204e 6f6e 650a 2020 2020 2020 2020     None.        
+00017ee0: 2222 220a 0a20 2020 2020 2020 2069 6620  """..        if 
+00017ef0: 7365 6c66 2e63 6f6e 7465 7374 3a0a 2020  self.contest:.  
+00017f00: 2020 2020 2020 2020 2020 6966 2068 6173            if has
+00017f10: 6174 7472 2873 656c 662e 636f 6e74 6573  attr(self.contes
+00017f20: 742c 2022 6164 7661 6e63 655f 6f6e 5f73  t, "advance_on_s
+00017f30: 7061 6365 2229 3a0a 2020 2020 2020 2020  pace"):.        
+00017f40: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00017f50: 636f 6e74 6573 742e 6164 7661 6e63 655f  contest.advance_
+00017f60: 6f6e 5f73 7061 6365 5b33 5d3a 0a20 2020  on_space[3]:.   
+00017f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017f80: 2074 6578 7420 3d20 7365 6c66 2e6f 7468   text = self.oth
+00017f90: 6572 5f31 2e74 6578 7428 290a 2020 2020  er_1.text().    
 00017fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017fb0: 2020 7465 7874 203d 2073 656c 662e 6f74    text = self.ot
-00017fc0: 6865 725f 312e 7465 7874 2829 0a20 2020  her_1.text().   
-00017fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017fe0: 2074 6578 7420 3d20 7465 7874 2e75 7070   text = text.upp
-00017ff0: 6572 2829 0a20 2020 2020 2020 2020 2020  er().           
-00018000: 2020 2020 2020 2020 2023 2070 6f73 6974           # posit
-00018010: 696f 6e20 3d20 7365 6c66 2e6f 7468 6572  ion = self.other
-00018020: 5f31 2e63 7572 736f 7250 6f73 6974 696f  _1.cursorPositio
-00018030: 6e28 290a 2020 2020 2020 2020 2020 2020  n().            
-00018040: 2020 2020 2020 2020 7374 7269 7070 6564          stripped
-00018050: 5f74 6578 7420 3d20 7465 7874 2e73 7472  _text = text.str
-00018060: 6970 2829 2e72 6570 6c61 6365 2822 2022  ip().replace(" "
-00018070: 2c20 2222 290a 2020 2020 2020 2020 2020  , "").          
-00018080: 2020 2020 2020 2020 2020 7365 6c66 2e6f            self.o
-00018090: 7468 6572 5f31 2e73 6574 5465 7874 2873  ther_1.setText(s
-000180a0: 7472 6970 7065 645f 7465 7874 290a 2020  tripped_text).  
-000180b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000180c0: 2020 2320 7365 6c66 2e6f 7468 6572 5f31    # self.other_1
-000180d0: 2e73 6574 4375 7273 6f72 506f 7369 7469  .setCursorPositi
-000180e0: 6f6e 2870 6f73 6974 696f 6e29 0a20 2020  on(position).   
-000180f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018100: 2069 6620 2220 2220 696e 2074 6578 743a   if " " in text:
-00018110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018120: 2020 2020 2020 2020 206e 6578 745f 7461           next_ta
-00018130: 6220 3d20 7365 6c66 2e74 6162 5f6e 6578  b = self.tab_nex
-00018140: 742e 6765 7428 7365 6c66 2e6f 7468 6572  t.get(self.other
-00018150: 5f31 290a 2020 2020 2020 2020 2020 2020  _1).            
-00018160: 2020 2020 2020 2020 2020 2020 6e65 7874              next
-00018170: 5f74 6162 2e73 6574 466f 6375 7328 290a  _tab.setFocus().
+00017fb0: 7465 7874 203d 2074 6578 742e 7570 7065  text = text.uppe
+00017fc0: 7228 290a 2020 2020 2020 2020 2020 2020  r().            
+00017fd0: 2020 2020 2020 2020 2320 706f 7369 7469          # positi
+00017fe0: 6f6e 203d 2073 656c 662e 6f74 6865 725f  on = self.other_
+00017ff0: 312e 6375 7273 6f72 506f 7369 7469 6f6e  1.cursorPosition
+00018000: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00018010: 2020 2020 2020 2073 7472 6970 7065 645f         stripped_
+00018020: 7465 7874 203d 2074 6578 742e 7374 7269  text = text.stri
+00018030: 7028 292e 7265 706c 6163 6528 2220 222c  p().replace(" ",
+00018040: 2022 2229 0a20 2020 2020 2020 2020 2020   "").           
+00018050: 2020 2020 2020 2020 2073 656c 662e 6f74           self.ot
+00018060: 6865 725f 312e 7365 7454 6578 7428 7374  her_1.setText(st
+00018070: 7269 7070 6564 5f74 6578 7429 0a20 2020  ripped_text).   
+00018080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018090: 2023 2073 656c 662e 6f74 6865 725f 312e   # self.other_1.
+000180a0: 7365 7443 7572 736f 7250 6f73 6974 696f  setCursorPositio
+000180b0: 6e28 706f 7369 7469 6f6e 290a 2020 2020  n(position).    
+000180c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000180d0: 6966 2022 2022 2069 6e20 7465 7874 3a0a  if " " in text:.
+000180e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000180f0: 2020 2020 2020 2020 6e65 7874 5f74 6162          next_tab
+00018100: 203d 2073 656c 662e 7461 625f 6e65 7874   = self.tab_next
+00018110: 2e67 6574 2873 656c 662e 6f74 6865 725f  .get(self.other_
+00018120: 3129 0a20 2020 2020 2020 2020 2020 2020  1).             
+00018130: 2020 2020 2020 2020 2020 206e 6578 745f             next_
+00018140: 7461 622e 7365 7446 6f63 7573 2829 0a20  tab.setFocus(). 
+00018150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018160: 2020 2020 2020 206e 6578 745f 7461 622e         next_tab.
+00018170: 6465 7365 6c65 6374 2829 0a20 2020 2020  deselect().     
 00018180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018190: 2020 2020 2020 2020 6e65 7874 5f74 6162          next_tab
-000181a0: 2e64 6573 656c 6563 7428 290a 2020 2020  .deselect().    
-000181b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000181c0: 2020 2020 6e65 7874 5f74 6162 2e65 6e64      next_tab.end
-000181d0: 2846 616c 7365 290a 0a20 2020 2064 6566  (False)..    def
-000181e0: 206f 7468 6572 5f32 5f63 6861 6e67 6564   other_2_changed
-000181f0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-00018200: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00018210: 2020 2020 5465 7874 2069 6e20 6f74 6865      Text in othe
-00018220: 725f 3220 6861 7320 6368 616e 6765 642e  r_2 has changed.
-00018230: 0a20 2020 2020 2020 2053 7472 6970 206f  .        Strip o
-00018240: 7574 2061 6e79 2073 7061 6365 7320 616e  ut any spaces an
-00018250: 6420 7365 7420 7468 6520 7465 7874 2e0a  d set the text..
-00018260: 2020 2020 2020 2020 5061 7273 6520 7468          Parse th
-00018270: 6520 6578 6368 616e 6765 2069 6620 7468  e exchange if th
-00018280: 6520 636f 6e74 6573 7420 6973 2041 5252  e contest is ARR
-00018290: 4c20 5377 6565 7073 7461 6b65 732e 0a0a  L Sweepstakes...
-000182a0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-000182b0: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
-000182c0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 4e6f  -----.        No
-000182d0: 6e65 0a0a 2020 2020 2020 2020 5265 7475  ne..        Retu
-000182e0: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
-000182f0: 2d2d 2d0a 2020 2020 2020 2020 4e6f 6e65  ---.        None
-00018300: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
-00018310: 2020 2020 2020 6966 2073 656c 662e 636f        if self.co
-00018320: 6e74 6573 743a 0a20 2020 2020 2020 2020  ntest:.         
-00018330: 2020 2069 6620 2241 5252 4c20 5377 6565     if "ARRL Swee
-00018340: 7073 7461 6b65 7322 2069 6e20 7365 6c66  pstakes" in self
-00018350: 2e63 6f6e 7465 7374 2e6e 616d 653a 0a20  .contest.name:. 
-00018360: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00018370: 656c 662e 636f 6e74 6573 742e 7061 7273  elf.contest.pars
-00018380: 655f 6578 6368 616e 6765 2873 656c 6629  e_exchange(self)
-00018390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000183a0: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-000183b0: 2020 2020 6966 2068 6173 6174 7472 2873      if hasattr(s
-000183c0: 656c 662e 636f 6e74 6573 742c 2022 6164  elf.contest, "ad
-000183d0: 7661 6e63 655f 6f6e 5f73 7061 6365 2229  vance_on_space")
-000183e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000183f0: 2020 6966 2073 656c 662e 636f 6e74 6573    if self.contes
-00018400: 742e 6164 7661 6e63 655f 6f6e 5f73 7061  t.advance_on_spa
-00018410: 6365 5b33 5d3a 0a20 2020 2020 2020 2020  ce[3]:.         
-00018420: 2020 2020 2020 2020 2020 2074 6578 7420             text 
-00018430: 3d20 7365 6c66 2e6f 7468 6572 5f32 2e74  = self.other_2.t
-00018440: 6578 7428 290a 2020 2020 2020 2020 2020  ext().          
-00018450: 2020 2020 2020 2020 2020 7465 7874 203d            text =
-00018460: 2074 6578 742e 7570 7065 7228 290a 2020   text.upper().  
-00018470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018480: 2020 2320 706f 7369 7469 6f6e 203d 2073    # position = s
-00018490: 656c 662e 6f74 6865 725f 322e 6375 7273  elf.other_2.curs
-000184a0: 6f72 506f 7369 7469 6f6e 2829 0a20 2020  orPosition().   
-000184b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000184c0: 2073 7472 6970 7065 645f 7465 7874 203d   stripped_text =
-000184d0: 2074 6578 742e 7374 7269 7028 292e 7265   text.strip().re
-000184e0: 706c 6163 6528 2220 222c 2022 2229 0a20  place(" ", ""). 
-000184f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018500: 2020 2073 656c 662e 6f74 6865 725f 322e     self.other_2.
-00018510: 7365 7454 6578 7428 7374 7269 7070 6564  setText(stripped
-00018520: 5f74 6578 7429 0a20 2020 2020 2020 2020  _text).         
-00018530: 2020 2020 2020 2020 2020 2023 2073 656c             # sel
-00018540: 662e 6f74 6865 725f 322e 7365 7443 7572  f.other_2.setCur
-00018550: 736f 7250 6f73 6974 696f 6e28 706f 7369  sorPosition(posi
-00018560: 7469 6f6e 290a 2020 2020 2020 2020 2020  tion).          
-00018570: 2020 2020 2020 2020 2020 6966 2022 2022            if " "
-00018580: 2069 6e20 7465 7874 3a0a 2020 2020 2020   in text:.      
-00018590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000185a0: 2020 6e65 7874 5f74 6162 203d 2073 656c    next_tab = sel
-000185b0: 662e 7461 625f 6e65 7874 2e67 6574 2873  f.tab_next.get(s
-000185c0: 656c 662e 6f74 6865 725f 3229 0a20 2020  elf.other_2).   
+00018190: 2020 206e 6578 745f 7461 622e 656e 6428     next_tab.end(
+000181a0: 4661 6c73 6529 0a0a 2020 2020 6465 6620  False)..    def 
+000181b0: 6f74 6865 725f 325f 6368 616e 6765 6428  other_2_changed(
+000181c0: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
+000181d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000181e0: 2020 2054 6578 7420 696e 206f 7468 6572     Text in other
+000181f0: 5f32 2068 6173 2063 6861 6e67 6564 2e0a  _2 has changed..
+00018200: 2020 2020 2020 2020 5374 7269 7020 6f75          Strip ou
+00018210: 7420 616e 7920 7370 6163 6573 2061 6e64  t any spaces and
+00018220: 2073 6574 2074 6865 2074 6578 742e 0a20   set the text.. 
+00018230: 2020 2020 2020 2050 6172 7365 2074 6865         Parse the
+00018240: 2065 7863 6861 6e67 6520 6966 2074 6865   exchange if the
+00018250: 2063 6f6e 7465 7374 2069 7320 4152 524c   contest is ARRL
+00018260: 2053 7765 6570 7374 616b 6573 2e0a 0a20   Sweepstakes... 
+00018270: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+00018280: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+00018290: 2d2d 2d2d 0a20 2020 2020 2020 204e 6f6e  ----.        Non
+000182a0: 650a 0a20 2020 2020 2020 2052 6574 7572  e..        Retur
+000182b0: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
+000182c0: 2d2d 0a20 2020 2020 2020 204e 6f6e 650a  --.        None.
+000182d0: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
+000182e0: 2020 2020 2069 6620 7365 6c66 2e63 6f6e       if self.con
+000182f0: 7465 7374 3a0a 2020 2020 2020 2020 2020  test:.          
+00018300: 2020 6966 2022 4152 524c 2053 7765 6570    if "ARRL Sweep
+00018310: 7374 616b 6573 2220 696e 2073 656c 662e  stakes" in self.
+00018320: 636f 6e74 6573 742e 6e61 6d65 3a0a 2020  contest.name:.  
+00018330: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00018340: 6c66 2e63 6f6e 7465 7374 2e70 6172 7365  lf.contest.parse
+00018350: 5f65 7863 6861 6e67 6528 7365 6c66 290a  _exchange(self).
+00018360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018370: 7265 7475 726e 0a20 2020 2020 2020 2020  return.         
+00018380: 2020 2069 6620 6861 7361 7474 7228 7365     if hasattr(se
+00018390: 6c66 2e63 6f6e 7465 7374 2c20 2261 6476  lf.contest, "adv
+000183a0: 616e 6365 5f6f 6e5f 7370 6163 6522 293a  ance_on_space"):
+000183b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000183c0: 2069 6620 7365 6c66 2e63 6f6e 7465 7374   if self.contest
+000183d0: 2e61 6476 616e 6365 5f6f 6e5f 7370 6163  .advance_on_spac
+000183e0: 655b 335d 3a0a 2020 2020 2020 2020 2020  e[3]:.          
+000183f0: 2020 2020 2020 2020 2020 7465 7874 203d            text =
+00018400: 2073 656c 662e 6f74 6865 725f 322e 7465   self.other_2.te
+00018410: 7874 2829 0a20 2020 2020 2020 2020 2020  xt().           
+00018420: 2020 2020 2020 2020 2074 6578 7420 3d20           text = 
+00018430: 7465 7874 2e75 7070 6572 2829 0a20 2020  text.upper().   
+00018440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018450: 2023 2070 6f73 6974 696f 6e20 3d20 7365   # position = se
+00018460: 6c66 2e6f 7468 6572 5f32 2e63 7572 736f  lf.other_2.curso
+00018470: 7250 6f73 6974 696f 6e28 290a 2020 2020  rPosition().    
+00018480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018490: 7374 7269 7070 6564 5f74 6578 7420 3d20  stripped_text = 
+000184a0: 7465 7874 2e73 7472 6970 2829 2e72 6570  text.strip().rep
+000184b0: 6c61 6365 2822 2022 2c20 2222 290a 2020  lace(" ", "").  
+000184c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000184d0: 2020 7365 6c66 2e6f 7468 6572 5f32 2e73    self.other_2.s
+000184e0: 6574 5465 7874 2873 7472 6970 7065 645f  etText(stripped_
+000184f0: 7465 7874 290a 2020 2020 2020 2020 2020  text).          
+00018500: 2020 2020 2020 2020 2020 2320 7365 6c66            # self
+00018510: 2e6f 7468 6572 5f32 2e73 6574 4375 7273  .other_2.setCurs
+00018520: 6f72 506f 7369 7469 6f6e 2870 6f73 6974  orPosition(posit
+00018530: 696f 6e29 0a20 2020 2020 2020 2020 2020  ion).           
+00018540: 2020 2020 2020 2020 2069 6620 2220 2220           if " " 
+00018550: 696e 2074 6578 743a 0a20 2020 2020 2020  in text:.       
+00018560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018570: 206e 6578 745f 7461 6220 3d20 7365 6c66   next_tab = self
+00018580: 2e74 6162 5f6e 6578 742e 6765 7428 7365  .tab_next.get(se
+00018590: 6c66 2e6f 7468 6572 5f32 290a 2020 2020  lf.other_2).    
+000185a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000185b0: 2020 2020 6e65 7874 5f74 6162 2e73 6574      next_tab.set
+000185c0: 466f 6375 7328 290a 2020 2020 2020 2020  Focus().        
 000185d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000185e0: 2020 2020 206e 6578 745f 7461 622e 7365       next_tab.se
-000185f0: 7446 6f63 7573 2829 0a20 2020 2020 2020  tFocus().       
-00018600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018610: 206e 6578 745f 7461 622e 6465 7365 6c65   next_tab.desele
-00018620: 6374 2829 0a20 2020 2020 2020 2020 2020  ct().           
-00018630: 2020 2020 2020 2020 2020 2020 206e 6578               nex
-00018640: 745f 7461 622e 656e 6428 4661 6c73 6529  t_tab.end(False)
-00018650: 0a0a 2020 2020 6465 6620 6361 6c6c 7369  ..    def callsi
-00018660: 676e 5f63 6861 6e67 6564 2873 656c 6629  gn_changed(self)
-00018670: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00018680: 2020 2222 220a 2020 2020 2020 2020 4361    """.        Ca
-00018690: 6c6c 6564 2077 6865 6e20 7465 7874 2069  lled when text i
-000186a0: 6e20 7468 6520 6361 6c6c 7369 676e 2066  n the callsign f
-000186b0: 6965 6c64 2068 6173 2063 6861 6e67 6564  ield has changed
-000186c0: 2e0a 2020 2020 2020 2020 5374 7269 7020  ..        Strip 
-000186d0: 6f75 7420 616e 7920 7370 6163 6573 2061  out any spaces a
-000186e0: 6e64 2073 6574 2074 6865 2074 6578 742e  nd set the text.
-000186f0: 0a20 2020 2020 2020 2043 6865 636b 2069  .        Check i
-00018700: 6620 7468 6520 6669 656c 6420 636f 6e74  f the field cont
-00018710: 6169 6e73 2061 2063 6f6d 6d61 6e64 2e0a  ains a command..
-00018720: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-00018730: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
-00018740: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 204e  ------.        N
-00018750: 6f6e 650a 0a20 2020 2020 2020 2052 6574  one..        Ret
-00018760: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
-00018770: 2d2d 2d2d 0a20 2020 2020 2020 204e 6f6e  ----.        Non
-00018780: 650a 2020 2020 2020 2020 2222 220a 0a20  e.        """.. 
-00018790: 2020 2020 2020 2074 6578 7420 3d20 7365         text = se
-000187a0: 6c66 2e63 616c 6c73 6967 6e2e 7465 7874  lf.callsign.text
-000187b0: 2829 0a20 2020 2020 2020 2074 6578 7420  ().        text 
-000187c0: 3d20 7465 7874 2e75 7070 6572 2829 0a20  = text.upper(). 
-000187d0: 2020 2020 2020 2070 6f73 6974 696f 6e20         position 
-000187e0: 3d20 7365 6c66 2e63 616c 6c73 6967 6e2e  = self.callsign.
-000187f0: 6375 7273 6f72 506f 7369 7469 6f6e 2829  cursorPosition()
-00018800: 0a20 2020 2020 2020 2073 7472 6970 7065  .        strippe
-00018810: 645f 7465 7874 203d 2074 6578 742e 7374  d_text = text.st
-00018820: 7269 7028 292e 7265 706c 6163 6528 2220  rip().replace(" 
-00018830: 222c 2022 2229 0a20 2020 2020 2020 2073  ", "").        s
-00018840: 656c 662e 6361 6c6c 7369 676e 2e73 6574  elf.callsign.set
-00018850: 5465 7874 2873 7472 6970 7065 645f 7465  Text(stripped_te
-00018860: 7874 290a 2020 2020 2020 2020 7365 6c66  xt).        self
-00018870: 2e63 616c 6c73 6967 6e2e 7365 7443 7572  .callsign.setCur
-00018880: 736f 7250 6f73 6974 696f 6e28 706f 7369  sorPosition(posi
-00018890: 7469 6f6e 290a 0a20 2020 2020 2020 2069  tion)..        i
-000188a0: 6620 2220 2220 696e 2074 6578 743a 0a20  f " " in text:. 
-000188b0: 2020 2020 2020 2020 2020 2069 6620 7374             if st
-000188c0: 7269 7070 6564 5f74 6578 7420 3d3d 2022  ripped_text == "
-000188d0: 4357 223a 0a20 2020 2020 2020 2020 2020  CW":.           
-000188e0: 2020 2020 2073 656c 662e 6368 616e 6765       self.change
-000188f0: 5f6d 6f64 6528 7374 7269 7070 6564 5f74  _mode(stripped_t
-00018900: 6578 7429 0a20 2020 2020 2020 2020 2020  ext).           
-00018910: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-00018920: 2020 2020 2020 2020 6966 2073 7472 6970          if strip
-00018930: 7065 645f 7465 7874 203d 3d20 2252 5454  ped_text == "RTT
-00018940: 5922 3a0a 2020 2020 2020 2020 2020 2020  Y":.            
-00018950: 2020 2020 7365 6c66 2e63 6861 6e67 655f      self.change_
-00018960: 6d6f 6465 2873 7472 6970 7065 645f 7465  mode(stripped_te
-00018970: 7874 290a 2020 2020 2020 2020 2020 2020  xt).            
-00018980: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-00018990: 2020 2020 2020 2069 6620 7374 7269 7070         if stripp
-000189a0: 6564 5f74 6578 7420 3d3d 2022 5353 4222  ed_text == "SSB"
-000189b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000189c0: 2020 7365 6c66 2e63 6861 6e67 655f 6d6f    self.change_mo
-000189d0: 6465 2873 7472 6970 7065 645f 7465 7874  de(stripped_text
-000189e0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000189f0: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-00018a00: 2020 2020 2069 6620 7374 7269 7070 6564       if stripped
-00018a10: 5f74 6578 7420 3d3d 2022 4f50 4f4e 223a  _text == "OPON":
-00018a20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018a30: 2073 656c 662e 6765 745f 6f70 6f6e 2829   self.get_opon()
-00018a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018a50: 2073 656c 662e 636c 6561 7269 6e70 7574   self.clearinput
-00018a60: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
-00018a70: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-00018a80: 2020 2020 2020 2069 6620 7374 7269 7070         if stripp
-00018a90: 6564 5f74 6578 7420 3d3d 2022 4845 4c50  ed_text == "HELP
-00018aa0: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-00018ab0: 2020 2073 656c 662e 7368 6f77 5f68 656c     self.show_hel
-00018ac0: 705f 6469 616c 6f67 2829 0a20 2020 2020  p_dialog().     
-00018ad0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00018ae0: 636c 6561 7269 6e70 7574 7328 290a 2020  clearinputs().  
-00018af0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00018b00: 7475 726e 0a20 2020 2020 2020 2020 2020  turn.           
-00018b10: 2069 6620 7374 7269 7070 6564 5f74 6578   if stripped_tex
-00018b20: 7420 3d3d 2022 5445 5354 223a 0a20 2020  t == "TEST":.   
-00018b30: 2020 2020 2020 2020 2020 2020 2072 6573               res
-00018b40: 756c 7420 3d20 7365 6c66 2e64 6174 6162  ult = self.datab
-00018b50: 6173 652e 6765 745f 6361 6c6c 735f 616e  ase.get_calls_an
-00018b60: 645f 6261 6e64 7328 290a 2020 2020 2020  d_bands().      
-00018b70: 2020 2020 2020 2020 2020 636d 6420 3d20            cmd = 
-00018b80: 7b7d 0a20 2020 2020 2020 2020 2020 2020  {}.             
-00018b90: 2020 2063 6d64 5b22 636d 6422 5d20 3d20     cmd["cmd"] = 
-00018ba0: 2257 4f52 4b45 4422 0a20 2020 2020 2020  "WORKED".       
-00018bb0: 2020 2020 2020 2020 2063 6d64 5b22 7374           cmd["st
-00018bc0: 6174 696f 6e22 5d20 3d20 706c 6174 666f  ation"] = platfo
-00018bd0: 726d 2e6e 6f64 6528 290a 2020 2020 2020  rm.node().      
-00018be0: 2020 2020 2020 2020 2020 636d 645b 2277            cmd["w
-00018bf0: 6f72 6b65 6422 5d20 3d20 7265 7375 6c74  orked"] = result
-00018c00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018c10: 2073 656c 662e 6d75 6c74 6963 6173 745f   self.multicast_
-00018c20: 696e 7465 7266 6163 652e 7365 6e64 5f61  interface.send_a
-00018c30: 735f 6a73 6f6e 2863 6d64 290a 2020 2020  s_json(cmd).    
-00018c40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00018c50: 2e63 6c65 6172 696e 7075 7473 2829 0a20  .clearinputs(). 
-00018c60: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00018c70: 6574 7572 6e0a 2020 2020 2020 2020 2020  eturn.          
-00018c80: 2020 6966 2073 656c 662e 6973 5f66 6c6f    if self.is_flo
-00018c90: 6174 6162 6c65 2873 7472 6970 7065 645f  atable(stripped_
-00018ca0: 7465 7874 293a 0a20 2020 2020 2020 2020  text):.         
-00018cb0: 2020 2020 2020 2073 656c 662e 6368 616e         self.chan
-00018cc0: 6765 5f66 7265 7128 7374 7269 7070 6564  ge_freq(stripped
-00018cd0: 5f74 6578 7429 0a20 2020 2020 2020 2020  _text).         
-00018ce0: 2020 2020 2020 2072 6574 7572 6e0a 0a20         return.. 
-00018cf0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00018d00: 6368 6563 6b5f 6361 6c6c 7369 676e 2873  check_callsign(s
-00018d10: 7472 6970 7065 645f 7465 7874 290a 2020  tripped_text).  
-00018d20: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00018d30: 662e 6368 6563 6b5f 6475 7065 2873 7472  f.check_dupe(str
-00018d40: 6970 7065 645f 7465 7874 293a 0a20 2020  ipped_text):.   
-00018d50: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018d60: 662e 6475 7065 5f69 6e64 6963 6174 6f72  f.dupe_indicator
-00018d70: 2e73 686f 7728 290a 2020 2020 2020 2020  .show().        
-00018d80: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00018d90: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-00018da0: 7570 655f 696e 6469 6361 746f 722e 6869  upe_indicator.hi
-00018db0: 6465 2829 0a20 2020 2020 2020 2020 2020  de().           
-00018dc0: 205f 7468 6574 6872 6561 6420 3d20 7468   _thethread = th
-00018dd0: 7265 6164 696e 672e 5468 7265 6164 280a  reading.Thread(.
-00018de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018df0: 7461 7267 6574 3d73 656c 662e 6368 6563  target=self.chec
-00018e00: 6b5f 6361 6c6c 7369 676e 322c 0a20 2020  k_callsign2,.   
-00018e10: 2020 2020 2020 2020 2020 2020 2061 7267               arg
-00018e20: 733d 2874 6578 742c 292c 0a20 2020 2020  s=(text,),.     
-00018e30: 2020 2020 2020 2020 2020 2064 6165 6d6f             daemo
-00018e40: 6e3d 5472 7565 2c0a 2020 2020 2020 2020  n=True,.        
-00018e50: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00018e60: 2020 5f74 6865 7468 7265 6164 2e73 7461    _thethread.sta
-00018e70: 7274 2829 0a20 2020 2020 2020 2020 2020  rt().           
-00018e80: 2073 656c 662e 6e65 7874 5f66 6965 6c64   self.next_field
-00018e90: 2e73 6574 466f 6375 7328 290a 2020 2020  .setFocus().    
-00018ea0: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-00018eb0: 2020 2020 2020 2063 6d64 203d 207b 7d0a         cmd = {}.
-00018ec0: 2020 2020 2020 2020 636d 645b 2263 6d64          cmd["cmd
-00018ed0: 225d 203d 2022 4341 4c4c 4348 414e 4745  "] = "CALLCHANGE
-00018ee0: 4422 0a20 2020 2020 2020 2063 6d64 5b22  D".        cmd["
-00018ef0: 7374 6174 696f 6e22 5d20 3d20 706c 6174  station"] = plat
-00018f00: 666f 726d 2e6e 6f64 6528 290a 2020 2020  form.node().    
-00018f10: 2020 2020 636d 645b 2263 616c 6c22 5d20      cmd["call"] 
-00018f20: 3d20 7374 7269 7070 6564 5f74 6578 740a  = stripped_text.
-00018f30: 2020 2020 2020 2020 7365 6c66 2e6d 756c          self.mul
-00018f40: 7469 6361 7374 5f69 6e74 6572 6661 6365  ticast_interface
-00018f50: 2e73 656e 645f 6173 5f6a 736f 6e28 636d  .send_as_json(cm
-00018f60: 6429 0a20 2020 2020 2020 2073 656c 662e  d).        self.
-00018f70: 6368 6563 6b5f 6361 6c6c 7369 676e 2873  check_callsign(s
-00018f80: 7472 6970 7065 645f 7465 7874 290a 0a20  tripped_text).. 
-00018f90: 2020 2064 6566 2063 6861 6e67 655f 6672     def change_fr
-00018fa0: 6571 2873 656c 662c 2073 7472 6970 7065  eq(self, strippe
-00018fb0: 645f 7465 7874 3a20 7374 7229 202d 3e20  d_text: str) -> 
-00018fc0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-00018fd0: 220a 2020 2020 2020 2020 4368 616e 6765  ".        Change
-00018fe0: 2056 464f 2074 6f20 6769 7665 6e20 6672   VFO to given fr
-00018ff0: 6571 7565 6e63 7920 696e 204b 687a 2061  equency in Khz a
-00019000: 6e64 2073 6574 2074 6865 2062 616e 6420  nd set the band 
-00019010: 696e 6469 6361 746f 722e 0a20 2020 2020  indicator..     
-00019020: 2020 2053 656e 6420 7468 6520 6e65 7720     Send the new 
-00019030: 6672 6571 7565 6e63 7920 746f 2074 6865  frequency to the
-00019040: 2072 6967 2063 6f6e 7472 6f6c 2e0a 0a20   rig control... 
-00019050: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-00019060: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-00019070: 2d2d 2d2d 0a20 2020 2020 2020 2073 7472  ----.        str
-00019080: 6970 7065 645f 7465 7874 203a 2073 7472  ipped_text : str
-00019090: 0a20 2020 2020 2020 2053 7472 6970 7065  .        Strippe
-000190a0: 6420 6f66 2061 6e79 2073 7061 6365 732e  d of any spaces.
-000190b0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-000190c0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-000190d0: 2d0a 2020 2020 2020 2020 4e6f 6e65 0a20  -.        None. 
-000190e0: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
-000190f0: 2020 2020 7666 6f20 3d20 666c 6f61 7428      vfo = float(
-00019100: 7374 7269 7070 6564 5f74 6578 7429 0a20  stripped_text). 
-00019110: 2020 2020 2020 2076 666f 203d 2069 6e74         vfo = int
-00019120: 2876 666f 202a 2031 3030 3029 0a20 2020  (vfo * 1000).   
-00019130: 2020 2020 2062 616e 6420 3d20 6765 7462       band = getb
-00019140: 616e 6428 7374 7228 7666 6f29 290a 2020  and(str(vfo)).  
-00019150: 2020 2020 2020 7365 6c66 2e73 6574 5f62        self.set_b
-00019160: 616e 645f 696e 6469 6361 746f 7228 6261  and_indicator(ba
-00019170: 6e64 290a 2020 2020 2020 2020 7365 6c66  nd).        self
-00019180: 2e72 6164 696f 5f73 7461 7465 5b22 7666  .radio_state["vf
-00019190: 6f61 225d 203d 2076 666f 0a20 2020 2020  oa"] = vfo.     
-000191a0: 2020 2073 656c 662e 7261 6469 6f5f 7374     self.radio_st
-000191b0: 6174 655b 2262 616e 6422 5d20 3d20 6261  ate["band"] = ba
-000191c0: 6e64 0a20 2020 2020 2020 2073 656c 662e  nd.        self.
-000191d0: 636f 6e74 6163 745b 2242 616e 6422 5d20  contact["Band"] 
-000191e0: 3d20 6765 745f 6c6f 6767 6564 5f62 616e  = get_logged_ban
-000191f0: 6428 7374 7228 7666 6f29 290a 2020 2020  d(str(vfo)).    
-00019200: 2020 2020 7365 6c66 2e73 6574 5f77 696e      self.set_win
-00019210: 646f 775f 7469 746c 6528 290a 2020 2020  dow_title().    
-00019220: 2020 2020 7365 6c66 2e63 6c65 6172 696e      self.clearin
-00019230: 7075 7473 2829 0a20 2020 2020 2020 2069  puts().        i
-00019240: 6620 7365 6c66 2e72 6967 5f63 6f6e 7472  f self.rig_contr
-00019250: 6f6c 3a0a 2020 2020 2020 2020 2020 2020  ol:.            
-00019260: 7365 6c66 2e72 6967 5f63 6f6e 7472 6f6c  self.rig_control
-00019270: 2e73 6574 5f76 666f 2876 666f 290a 2020  .set_vfo(vfo).  
-00019280: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00019290: 0a20 2020 2020 2020 2063 6d64 203d 207b  .        cmd = {
-000192a0: 7d0a 2020 2020 2020 2020 636d 645b 2263  }.        cmd["c
-000192b0: 6d64 225d 203d 2022 5241 4449 4f5f 5354  md"] = "RADIO_ST
-000192c0: 4154 4522 0a20 2020 2020 2020 2063 6d64  ATE".        cmd
-000192d0: 5b22 7374 6174 696f 6e22 5d20 3d20 706c  ["station"] = pl
-000192e0: 6174 666f 726d 2e6e 6f64 6528 290a 2020  atform.node().  
-000192f0: 2020 2020 2020 636d 645b 2262 616e 6422        cmd["band"
-00019300: 5d20 3d20 6261 6e64 0a20 2020 2020 2020  ] = band.       
-00019310: 2063 6d64 5b22 7666 6f61 225d 203d 2076   cmd["vfoa"] = v
-00019320: 666f 0a20 2020 2020 2020 2073 656c 662e  fo.        self.
-00019330: 6d75 6c74 6963 6173 745f 696e 7465 7266  multicast_interf
-00019340: 6163 652e 7365 6e64 5f61 735f 6a73 6f6e  ace.send_as_json
-00019350: 2863 6d64 290a 0a20 2020 2064 6566 2063  (cmd)..    def c
-00019360: 6861 6e67 655f 6d6f 6465 2873 656c 662c  hange_mode(self,
-00019370: 206d 6f64 653a 2073 7472 2920 2d3e 204e   mode: str) -> N
-00019380: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-00019390: 0a20 2020 2020 2020 2043 6861 6e67 6520  .        Change 
-000193a0: 6d6f 6465 2074 6f20 6769 7665 6e20 6d6f  mode to given mo
-000193b0: 6465 2e0a 2020 2020 2020 2020 5365 6e64  de..        Send
-000193c0: 2074 6865 206e 6577 206d 6f64 6520 746f   the new mode to
-000193d0: 2074 6865 2072 6967 2063 6f6e 7472 6f6c   the rig control
-000193e0: 2e0a 2020 2020 2020 2020 5365 7420 7468  ..        Set th
-000193f0: 6520 6261 6e64 2069 6e64 6963 6174 6f72  e band indicator
-00019400: 2e0a 2020 2020 2020 2020 5365 7420 7468  ..        Set th
-00019410: 6520 7769 6e64 6f77 2074 6974 6c65 2e0a  e window title..
-00019420: 2020 2020 2020 2020 436c 6561 7220 7468          Clear th
-00019430: 6520 696e 7075 7473 2e0a 2020 2020 2020  e inputs..      
-00019440: 2020 5265 6164 2074 6865 2043 5720 6d61    Read the CW ma
-00019450: 6372 6f73 2e0a 0a20 2020 2020 2020 2050  cros...        P
-00019460: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-00019470: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-00019480: 2020 2020 206d 6f64 6520 3a20 7374 720a       mode : str.
-00019490: 2020 2020 2020 2020 4d6f 6465 2074 6f20          Mode to 
-000194a0: 6368 616e 6765 2074 6f2e 0a0a 2020 2020  change to...    
-000194b0: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-000194c0: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-000194d0: 2020 2020 4e6f 6e65 0a20 2020 2020 2020      None.       
-000194e0: 2022 2222 0a0a 2020 2020 2020 2020 6966   """..        if
-000194f0: 206d 6f64 6520 3d3d 2022 4357 223a 0a20   mode == "CW":. 
-00019500: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00019510: 7365 746d 6f64 6528 2243 5722 290a 2020  setmode("CW").  
-00019520: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-00019530: 6164 696f 5f73 7461 7465 5b22 6d6f 6465  adio_state["mode
-00019540: 225d 203d 2022 4357 220a 2020 2020 2020  "] = "CW".      
-00019550: 2020 2020 2020 6966 2073 656c 662e 7269        if self.ri
-00019560: 675f 636f 6e74 726f 6c3a 0a20 2020 2020  g_control:.     
-00019570: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00019580: 6c66 2e72 6967 5f63 6f6e 7472 6f6c 2e6f  lf.rig_control.o
-00019590: 6e6c 696e 653a 0a20 2020 2020 2020 2020  nline:.         
-000195a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000195b0: 7269 675f 636f 6e74 726f 6c2e 7365 745f  rig_control.set_
-000195c0: 6d6f 6465 2822 4357 2229 0a20 2020 2020  mode("CW").     
-000195d0: 2020 2020 2020 2062 616e 6420 3d20 6765         band = ge
-000195e0: 7462 616e 6428 7374 7228 7365 6c66 2e72  tband(str(self.r
-000195f0: 6164 696f 5f73 7461 7465 2e67 6574 2822  adio_state.get("
-00019600: 7666 6f61 222c 2022 302e 3022 2929 290a  vfoa", "0.0"))).
-00019610: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00019620: 2e73 6574 5f62 616e 645f 696e 6469 6361  .set_band_indica
-00019630: 746f 7228 6261 6e64 290a 2020 2020 2020  tor(band).      
-00019640: 2020 2020 2020 7365 6c66 2e73 6574 5f77        self.set_w
-00019650: 696e 646f 775f 7469 746c 6528 290a 2020  indow_title().  
-00019660: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00019670: 6c65 6172 696e 7075 7473 2829 0a20 2020  learinputs().   
-00019680: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
-00019690: 6164 5f63 775f 6d61 6372 6f73 2829 0a20  ad_cw_macros(). 
-000196a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000196b0: 6e0a 2020 2020 2020 2020 6966 206d 6f64  n.        if mod
-000196c0: 6520 3d3d 2022 5254 5459 223a 0a20 2020  e == "RTTY":.   
-000196d0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-000196e0: 746d 6f64 6528 2252 5454 5922 290a 2020  tmode("RTTY").  
-000196f0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00019700: 662e 7269 675f 636f 6e74 726f 6c3a 0a20  f.rig_control:. 
-00019710: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00019720: 6620 7365 6c66 2e72 6967 5f63 6f6e 7472  f self.rig_contr
-00019730: 6f6c 2e6f 6e6c 696e 653a 0a20 2020 2020  ol.online:.     
-00019740: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00019750: 656c 662e 7269 675f 636f 6e74 726f 6c2e  elf.rig_control.
-00019760: 7365 745f 6d6f 6465 2822 5254 5459 2229  set_mode("RTTY")
-00019770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019780: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00019790: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000197a0: 7261 6469 6f5f 7374 6174 655b 226d 6f64  radio_state["mod
-000197b0: 6522 5d20 3d20 2252 5454 5922 0a20 2020  e"] = "RTTY".   
-000197c0: 2020 2020 2020 2020 2062 616e 6420 3d20           band = 
-000197d0: 6765 7462 616e 6428 7374 7228 7365 6c66  getband(str(self
-000197e0: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
-000197f0: 2822 7666 6f61 222c 2022 302e 3022 2929  ("vfoa", "0.0"))
-00019800: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00019810: 6c66 2e73 6574 5f62 616e 645f 696e 6469  lf.set_band_indi
-00019820: 6361 746f 7228 6261 6e64 290a 2020 2020  cator(band).    
-00019830: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-00019840: 5f77 696e 646f 775f 7469 746c 6528 290a  _window_title().
-00019850: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00019860: 2e63 6c65 6172 696e 7075 7473 2829 0a20  .clearinputs(). 
-00019870: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00019880: 6e0a 2020 2020 2020 2020 6966 206d 6f64  n.        if mod
-00019890: 6520 3d3d 2022 5353 4222 3a0a 2020 2020  e == "SSB":.    
-000198a0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-000198b0: 6d6f 6465 2822 5353 4222 290a 2020 2020  mode("SSB").    
-000198c0: 2020 2020 2020 2020 6966 2069 6e74 2873          if int(s
-000198d0: 656c 662e 7261 6469 6f5f 7374 6174 652e  elf.radio_state.
-000198e0: 6765 7428 2276 666f 6122 2c20 3029 2920  get("vfoa", 0)) 
-000198f0: 3e20 3130 3030 3030 3030 3a0a 2020 2020  > 10000000:.    
-00019900: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00019910: 2e72 6164 696f 5f73 7461 7465 5b22 6d6f  .radio_state["mo
-00019920: 6465 225d 203d 2022 5553 4222 0a20 2020  de"] = "USB".   
-00019930: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00019940: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00019950: 656c 662e 7261 6469 6f5f 7374 6174 655b  elf.radio_state[
-00019960: 226d 6f64 6522 5d20 3d20 224c 5342 220a  "mode"] = "LSB".
-00019970: 2020 2020 2020 2020 2020 2020 6261 6e64              band
-00019980: 203d 2067 6574 6261 6e64 2873 7472 2873   = getband(str(s
-00019990: 656c 662e 7261 6469 6f5f 7374 6174 652e  elf.radio_state.
-000199a0: 6765 7428 2276 666f 6122 2c20 2230 2e30  get("vfoa", "0.0
-000199b0: 2229 2929 0a20 2020 2020 2020 2020 2020  "))).           
-000199c0: 2073 656c 662e 7365 745f 6261 6e64 5f69   self.set_band_i
-000199d0: 6e64 6963 6174 6f72 2862 616e 6429 0a20  ndicator(band). 
-000199e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000199f0: 7365 745f 7769 6e64 6f77 5f74 6974 6c65  set_window_title
-00019a00: 2829 0a20 2020 2020 2020 2020 2020 2069  ().            i
-00019a10: 6620 7365 6c66 2e72 6967 5f63 6f6e 7472  f self.rig_contr
-00019a20: 6f6c 3a0a 2020 2020 2020 2020 2020 2020  ol:.            
-00019a30: 2020 2020 7365 6c66 2e72 6967 5f63 6f6e      self.rig_con
-00019a40: 7472 6f6c 2e73 6574 5f6d 6f64 6528 7365  trol.set_mode(se
-00019a50: 6c66 2e72 6164 696f 5f73 7461 7465 2e67  lf.radio_state.g
-00019a60: 6574 2822 6d6f 6465 2229 290a 2020 2020  et("mode")).    
-00019a70: 2020 2020 2020 2020 7365 6c66 2e63 6c65          self.cle
-00019a80: 6172 696e 7075 7473 2829 0a20 2020 2020  arinputs().     
-00019a90: 2020 2020 2020 2073 656c 662e 7265 6164         self.read
-00019aa0: 5f63 775f 6d61 6372 6f73 2829 0a0a 2020  _cw_macros()..  
-00019ab0: 2020 6465 6620 6368 6563 6b5f 6361 6c6c    def check_call
-00019ac0: 7369 676e 2873 656c 662c 2063 616c 6c73  sign(self, calls
-00019ad0: 6967 6e29 202d 3e20 4e6f 6e65 3a0a 2020  ign) -> None:.  
-00019ae0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00019af0: 2020 4368 6563 6b20 6361 6c6c 7369 676e    Check callsign
-00019b00: 2061 7320 6974 2773 2062 6569 6e67 2065   as it's being e
-00019b10: 6e74 6572 6564 2069 6e20 7468 6520 6269  ntered in the bi
-00019b20: 675f 6374 7920 696e 6465 782e 0a20 2020  g_cty index..   
-00019b30: 2020 2020 2047 6574 2044 5820 656e 7469       Get DX enti
-00019b40: 7479 2c20 4351 2c20 4954 5520 616e 6420  ty, CQ, ITU and 
-00019b50: 636f 6e74 696e 656e 742e 0a20 2020 2020  continent..     
-00019b60: 2020 2047 656f 6772 6170 6869 6320 696e     Geographic in
-00019b70: 666f 726d 6174 696f 6e2e 2044 6973 7461  formation. Dista
-00019b80: 6e63 6520 616e 6420 4865 6164 696e 672e  nce and Heading.
-00019b90: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-00019ba0: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
-00019bb0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-00019bc0: 6361 6c6c 7369 676e 203a 2073 7472 0a20  callsign : str. 
-00019bd0: 2020 2020 2020 2043 616c 6c73 6967 6e20         Callsign 
-00019be0: 746f 2063 6865 636b 2e0a 0a20 2020 2020  to check...     
-00019bf0: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
-00019c00: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
-00019c10: 2020 204e 6f6e 650a 2020 2020 2020 2020     None.        
-00019c20: 2222 220a 0a20 2020 2020 2020 2072 6573  """..        res
-00019c30: 756c 7420 3d20 7365 6c66 2e63 7479 5f6c  ult = self.cty_l
-00019c40: 6f6f 6b75 7028 6361 6c6c 7369 676e 290a  ookup(callsign).
-00019c50: 2020 2020 2020 2020 6465 6275 675f 7265          debug_re
-00019c60: 7375 6c74 203d 2066 227b 7265 7375 6c74  sult = f"{result
-00019c70: 7d22 0a20 2020 2020 2020 206c 6f67 6765  }".        logge
-00019c80: 722e 6465 6275 6728 2225 7322 2c20 6465  r.debug("%s", de
-00019c90: 6275 675f 7265 7375 6c74 290a 2020 2020  bug_result).    
-00019ca0: 2020 2020 6966 2072 6573 756c 743a 0a20      if result:. 
-00019cb0: 2020 2020 2020 2020 2020 2066 6f72 2061             for a
-00019cc0: 2069 6e20 7265 7375 6c74 2e69 7465 6d73   in result.items
-00019cd0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00019ce0: 2020 2020 656e 7469 7479 203d 2061 5b31      entity = a[1
-00019cf0: 5d2e 6765 7428 2265 6e74 6974 7922 2c20  ].get("entity", 
-00019d00: 2222 290a 2020 2020 2020 2020 2020 2020  "").            
-00019d10: 2020 2020 6371 203d 2061 5b31 5d2e 6765      cq = a[1].ge
-00019d20: 7428 2263 7122 2c20 2222 290a 2020 2020  t("cq", "").    
-00019d30: 2020 2020 2020 2020 2020 2020 6974 7520              itu 
-00019d40: 3d20 615b 315d 2e67 6574 2822 6974 7522  = a[1].get("itu"
-00019d50: 2c20 2222 290a 2020 2020 2020 2020 2020  , "").          
-00019d60: 2020 2020 2020 636f 6e74 696e 656e 7420        continent 
-00019d70: 3d20 615b 315d 2e67 6574 2822 636f 6e74  = a[1].get("cont
-00019d80: 696e 656e 7422 290a 2020 2020 2020 2020  inent").        
-00019d90: 2020 2020 2020 2020 6c61 7420 3d20 666c          lat = fl
-00019da0: 6f61 7428 615b 315d 2e67 6574 2822 6c61  oat(a[1].get("la
-00019db0: 7422 2c20 2230 2e30 2229 290a 2020 2020  t", "0.0")).    
-00019dc0: 2020 2020 2020 2020 2020 2020 6c6f 6e20              lon 
-00019dd0: 3d20 666c 6f61 7428 615b 315d 2e67 6574  = float(a[1].get
-00019de0: 2822 6c6f 6e67 222c 2022 302e 3022 2929  ("long", "0.0"))
-00019df0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019e00: 206c 6f6e 203d 206c 6f6e 202a 202d 3120   lon = lon * -1 
-00019e10: 2023 2063 7479 2e64 6174 2066 696c 6520   # cty.dat file 
-00019e20: 696e 7665 7274 7320 6c6f 6e67 6974 7564  inverts longitud
-00019e30: 6573 0a20 2020 2020 2020 2020 2020 2020  es.             
-00019e40: 2020 2070 7269 6d61 7279 5f70 6678 203d     primary_pfx =
-00019e50: 2061 5b31 5d2e 6765 7428 2270 7269 6d61   a[1].get("prima
-00019e60: 7279 5f70 6678 222c 2022 2229 0a20 2020  ry_pfx", "").   
-00019e70: 2020 2020 2020 2020 2020 2020 2068 6561               hea
-00019e80: 6469 6e67 203d 2062 6561 7269 6e67 5f77  ding = bearing_w
-00019e90: 6974 685f 6c61 746c 6f6e 2873 656c 662e  ith_latlon(self.
-00019ea0: 7374 6174 696f 6e2e 6765 7428 2247 7269  station.get("Gri
-00019eb0: 6453 7175 6172 6522 292c 206c 6174 2c20  dSquare"), lat, 
-00019ec0: 6c6f 6e29 0a20 2020 2020 2020 2020 2020  lon).           
-00019ed0: 2020 2020 206b 696c 6f6d 6574 6572 7320       kilometers 
-00019ee0: 3d20 6469 7374 616e 6365 5f77 6974 685f  = distance_with_
-00019ef0: 6c61 746c 6f6e 280a 2020 2020 2020 2020  latlon(.        
-00019f00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00019f10: 2e73 7461 7469 6f6e 2e67 6574 2822 4772  .station.get("Gr
-00019f20: 6964 5371 7561 7265 2229 2c20 6c61 742c  idSquare"), lat,
-00019f30: 206c 6f6e 0a20 2020 2020 2020 2020 2020   lon.           
-00019f40: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00019f50: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
-00019f60: 696e 675f 6469 7374 616e 6365 2e73 6574  ing_distance.set
-00019f70: 5465 7874 280a 2020 2020 2020 2020 2020  Text(.          
-00019f80: 2020 2020 2020 2020 2020 6622 5265 6769            f"Regi
-00019f90: 6f6e 616c 2048 6467 207b 6865 6164 696e  onal Hdg {headin
-00019fa0: 677d c2b0 204c 5020 7b72 6563 6970 726f  g}.. LP {recipro
-00019fb0: 636f 6c28 6865 6164 696e 6729 7dc2 b020  col(heading)}.. 
-00019fc0: 2f20 220a 2020 2020 2020 2020 2020 2020  / ".            
-00019fd0: 2020 2020 2020 2020 6622 6469 7374 616e          f"distan
-00019fe0: 6365 207b 696e 7428 6b69 6c6f 6d65 7465  ce {int(kilomete
-00019ff0: 7273 2a30 2e36 3231 3337 3129 7d6d 6920  rs*0.621371)}mi 
-0001a000: 7b6b 696c 6f6d 6574 6572 737d 6b6d 220a  {kilometers}km".
-0001a010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a020: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001a030: 2020 7365 6c66 2e63 6f6e 7461 6374 5b22    self.contact["
-0001a040: 436f 756e 7472 7950 7265 6669 7822 5d20  CountryPrefix"] 
-0001a050: 3d20 7072 696d 6172 795f 7066 780a 2020  = primary_pfx.  
-0001a060: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0001a070: 6c66 2e63 6f6e 7461 6374 5b22 5a4e 225d  lf.contact["ZN"]
-0001a080: 203d 2069 6e74 2863 7129 0a20 2020 2020   = int(cq).     
-0001a090: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0001a0a0: 6c66 2e63 6f6e 7465 7374 3a0a 2020 2020  lf.contest:.    
-0001a0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a0c0: 6966 2073 656c 662e 636f 6e74 6573 742e  if self.contest.
-0001a0d0: 6e61 6d65 203d 3d20 2249 4152 5520 4846  name == "IARU HF
-0001a0e0: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-0001a0f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001a100: 636f 6e74 6163 745b 225a 4e22 5d20 3d20  contact["ZN"] = 
-0001a110: 696e 7428 6974 7529 0a20 2020 2020 2020  int(itu).       
-0001a120: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-0001a130: 6e74 6163 745b 2243 6f6e 7469 6e65 6e74  ntact["Continent
-0001a140: 225d 203d 2063 6f6e 7469 6e65 6e74 0a20  "] = continent. 
-0001a150: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0001a160: 656c 662e 6478 5f65 6e74 6974 792e 7365  elf.dx_entity.se
-0001a170: 7454 6578 7428 0a20 2020 2020 2020 2020  tText(.         
-0001a180: 2020 2020 2020 2020 2020 2066 227b 7072             f"{pr
-0001a190: 696d 6172 795f 7066 787d 3a20 7b63 6f6e  imary_pfx}: {con
-0001a1a0: 7469 6e65 6e74 7d2f 7b65 6e74 6974 797d  tinent}/{entity}
-0001a1b0: 2063 713a 7b63 717d 2069 7475 3a7b 6974   cq:{cq} itu:{it
-0001a1c0: 757d 220a 2020 2020 2020 2020 2020 2020  u}".            
-0001a1d0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0001a1e0: 2020 2020 2020 6966 206c 656e 2863 616c        if len(cal
-0001a1f0: 6c73 6967 6e29 203e 2032 3a0a 2020 2020  lsign) > 2:.    
-0001a200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a210: 6966 2073 656c 662e 636f 6e74 6573 743a  if self.contest:
-0001a220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a230: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-0001a240: 6e74 6573 742e 7072 6566 696c 6c28 7365  ntest.prefill(se
-0001a250: 6c66 290a 0a20 2020 2064 6566 2063 6865  lf)..    def che
-0001a260: 636b 5f63 616c 6c73 6967 6e32 2873 656c  ck_callsign2(sel
-0001a270: 662c 2063 616c 6c73 6967 6e29 202d 3e20  f, callsign) -> 
-0001a280: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-0001a290: 220a 2020 2020 2020 2020 4368 6563 6b20  ".        Check 
-0001a2a0: 7468 6520 6361 6c6c 7369 676e 2061 6674  the callsign aft
-0001a2b0: 6572 2069 7420 6861 7320 6265 656e 2065  er it has been e
-0001a2c0: 6e74 6572 6564 2e0a 2020 2020 2020 2020  ntered..        
-0001a2d0: 4c6f 6f6b 2075 7020 7468 6520 6361 6c6c  Look up the call
-0001a2e0: 7369 676e 2069 6e20 7468 6520 6361 6c6c  sign in the call
-0001a2f0: 7369 676e 2064 6174 6162 6173 652e 0a20  sign database.. 
-0001a300: 2020 2020 2020 2047 6574 2074 6865 2067         Get the g
-0001a310: 7269 6420 7371 7561 7265 2061 6e64 2063  rid square and c
-0001a320: 616c 6375 6c61 7465 2074 6865 2064 6973  alculate the dis
-0001a330: 7461 6e63 6520 616e 6420 6865 6164 696e  tance and headin
-0001a340: 672e 0a0a 2020 2020 2020 2020 5061 7261  g...        Para
-0001a350: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
-0001a360: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-0001a370: 2020 6361 6c6c 7369 676e 203a 2073 7472    callsign : str
-0001a380: 0a20 2020 2020 2020 2043 616c 6c73 6967  .        Callsig
-0001a390: 6e20 746f 2063 6865 636b 2e0a 0a20 2020  n to check...   
-0001a3a0: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
-0001a3b0: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
-0001a3c0: 2020 2020 204e 6f6e 650a 2020 2020 2020       None.      
-0001a3d0: 2020 2222 220a 0a20 2020 2020 2020 2063    """..        c
-0001a3e0: 616c 6c73 6967 6e20 3d20 6361 6c6c 7369  allsign = callsi
-0001a3f0: 676e 2e73 7472 6970 2829 0a20 2020 2020  gn.strip().     
-0001a400: 2020 2064 6562 7567 5f6c 6f6f 6b75 7020     debug_lookup 
-0001a410: 3d20 6622 7b73 656c 662e 6c6f 6f6b 5f75  = f"{self.look_u
-0001a420: 707d 220a 2020 2020 2020 2020 6c6f 6767  p}".        logg
-0001a430: 6572 2e64 6562 7567 2822 2573 2c20 2573  er.debug("%s, %s
-0001a440: 222c 2063 616c 6c73 6967 6e2c 2064 6562  ", callsign, deb
-0001a450: 7567 5f6c 6f6f 6b75 7029 0a20 2020 2020  ug_lookup).     
-0001a460: 2020 2069 6620 6861 7361 7474 7228 7365     if hasattr(se
-0001a470: 6c66 2e6c 6f6f 6b5f 7570 2c20 2273 6573  lf.look_up, "ses
-0001a480: 7369 6f6e 2229 3a0a 2020 2020 2020 2020  sion"):.        
-0001a490: 2020 2020 6966 2073 656c 662e 6c6f 6f6b      if self.look
-0001a4a0: 5f75 702e 7365 7373 696f 6e3a 0a20 2020  _up.session:.   
-0001a4b0: 2020 2020 2020 2020 2020 2020 2072 6573               res
-0001a4c0: 706f 6e73 6520 3d20 7365 6c66 2e6c 6f6f  ponse = self.loo
-0001a4d0: 6b5f 7570 2e6c 6f6f 6b75 7028 6361 6c6c  k_up.lookup(call
-0001a4e0: 7369 676e 290a 2020 2020 2020 2020 2020  sign).          
-0001a4f0: 2020 2020 2020 6465 6275 675f 7265 7370        debug_resp
-0001a500: 6f6e 7365 203d 2066 227b 7265 7370 6f6e  onse = f"{respon
-0001a510: 7365 7d22 0a20 2020 2020 2020 2020 2020  se}".           
-0001a520: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-0001a530: 6728 2254 6865 2052 6573 706f 6e73 653a  g("The Response:
-0001a540: 2025 735c 6e22 2c20 6465 6275 675f 7265   %s\n", debug_re
-0001a550: 7370 6f6e 7365 290a 2020 2020 2020 2020  sponse).        
-0001a560: 2020 2020 2020 2020 6966 2072 6573 706f          if respo
-0001a570: 6e73 653a 0a20 2020 2020 2020 2020 2020  nse:.           
-0001a580: 2020 2020 2020 2020 2074 6865 6972 6772           theirgr
-0001a590: 6964 203d 2072 6573 706f 6e73 652e 6765  id = response.ge
-0001a5a0: 7428 2267 7269 6422 2c20 2222 290a 2020  t("grid", "").  
-0001a5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a5c0: 2020 7365 6c66 2e63 6f6e 7461 6374 5b22    self.contact["
-0001a5d0: 4772 6964 5371 7561 7265 225d 203d 2074  GridSquare"] = t
-0001a5e0: 6865 6972 6772 6964 0a20 2020 2020 2020  heirgrid.       
-0001a5f0: 2020 2020 2020 2020 2020 2020 205f 7468               _th
-0001a600: 6569 7263 6f75 6e74 7279 203d 2072 6573  eircountry = res
-0001a610: 706f 6e73 652e 6765 7428 2263 6f75 6e74  ponse.get("count
-0001a620: 7279 222c 2022 2229 0a20 2020 2020 2020  ry", "").       
-0001a630: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0001a640: 7365 6c66 2e73 7461 7469 6f6e 2e67 6574  self.station.get
-0001a650: 2822 4772 6964 5371 7561 7265 222c 2022  ("GridSquare", "
-0001a660: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
-0001a670: 2020 2020 2020 2020 2020 2020 6865 6164              head
-0001a680: 696e 6720 3d20 6265 6172 696e 6728 7365  ing = bearing(se
-0001a690: 6c66 2e73 7461 7469 6f6e 2e67 6574 2822  lf.station.get("
-0001a6a0: 4772 6964 5371 7561 7265 222c 2022 2229  GridSquare", "")
-0001a6b0: 2c20 7468 6569 7267 7269 6429 0a20 2020  , theirgrid).   
+000185e0: 6e65 7874 5f74 6162 2e64 6573 656c 6563  next_tab.deselec
+000185f0: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
+00018600: 2020 2020 2020 2020 2020 2020 6e65 7874              next
+00018610: 5f74 6162 2e65 6e64 2846 616c 7365 290a  _tab.end(False).
+00018620: 0a20 2020 2064 6566 2063 616c 6c73 6967  .    def callsig
+00018630: 6e5f 6368 616e 6765 6428 7365 6c66 2920  n_changed(self) 
+00018640: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00018650: 2022 2222 0a20 2020 2020 2020 2043 616c   """.        Cal
+00018660: 6c65 6420 7768 656e 2074 6578 7420 696e  led when text in
+00018670: 2074 6865 2063 616c 6c73 6967 6e20 6669   the callsign fi
+00018680: 656c 6420 6861 7320 6368 616e 6765 642e  eld has changed.
+00018690: 0a20 2020 2020 2020 2053 7472 6970 206f  .        Strip o
+000186a0: 7574 2061 6e79 2073 7061 6365 7320 616e  ut any spaces an
+000186b0: 6420 7365 7420 7468 6520 7465 7874 2e0a  d set the text..
+000186c0: 2020 2020 2020 2020 4368 6563 6b20 6966          Check if
+000186d0: 2074 6865 2066 6965 6c64 2063 6f6e 7461   the field conta
+000186e0: 696e 7320 6120 636f 6d6d 616e 642e 0a0a  ins a command...
+000186f0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+00018700: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
+00018710: 2d2d 2d2d 2d0a 2020 2020 2020 2020 4e6f  -----.        No
+00018720: 6e65 0a0a 2020 2020 2020 2020 5265 7475  ne..        Retu
+00018730: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
+00018740: 2d2d 2d0a 2020 2020 2020 2020 4e6f 6e65  ---.        None
+00018750: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
+00018760: 2020 2020 2020 7465 7874 203d 2073 656c        text = sel
+00018770: 662e 6361 6c6c 7369 676e 2e74 6578 7428  f.callsign.text(
+00018780: 290a 2020 2020 2020 2020 7465 7874 203d  ).        text =
+00018790: 2074 6578 742e 7570 7065 7228 290a 2020   text.upper().  
+000187a0: 2020 2020 2020 706f 7369 7469 6f6e 203d        position =
+000187b0: 2073 656c 662e 6361 6c6c 7369 676e 2e63   self.callsign.c
+000187c0: 7572 736f 7250 6f73 6974 696f 6e28 290a  ursorPosition().
+000187d0: 2020 2020 2020 2020 7374 7269 7070 6564          stripped
+000187e0: 5f74 6578 7420 3d20 7465 7874 2e73 7472  _text = text.str
+000187f0: 6970 2829 2e72 6570 6c61 6365 2822 2022  ip().replace(" "
+00018800: 2c20 2222 290a 2020 2020 2020 2020 7365  , "").        se
+00018810: 6c66 2e63 616c 6c73 6967 6e2e 7365 7454  lf.callsign.setT
+00018820: 6578 7428 7374 7269 7070 6564 5f74 6578  ext(stripped_tex
+00018830: 7429 0a20 2020 2020 2020 2073 656c 662e  t).        self.
+00018840: 6361 6c6c 7369 676e 2e73 6574 4375 7273  callsign.setCurs
+00018850: 6f72 506f 7369 7469 6f6e 2870 6f73 6974  orPosition(posit
+00018860: 696f 6e29 0a0a 2020 2020 2020 2020 6966  ion)..        if
+00018870: 2022 2022 2069 6e20 7465 7874 3a0a 2020   " " in text:.  
+00018880: 2020 2020 2020 2020 2020 6966 2073 7472            if str
+00018890: 6970 7065 645f 7465 7874 203d 3d20 2243  ipped_text == "C
+000188a0: 5722 3a0a 2020 2020 2020 2020 2020 2020  W":.            
+000188b0: 2020 2020 7365 6c66 2e63 6861 6e67 655f      self.change_
+000188c0: 6d6f 6465 2873 7472 6970 7065 645f 7465  mode(stripped_te
+000188d0: 7874 290a 2020 2020 2020 2020 2020 2020  xt).            
+000188e0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+000188f0: 2020 2020 2020 2069 6620 7374 7269 7070         if stripp
+00018900: 6564 5f74 6578 7420 3d3d 2022 5254 5459  ed_text == "RTTY
+00018910: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
+00018920: 2020 2073 656c 662e 6368 616e 6765 5f6d     self.change_m
+00018930: 6f64 6528 7374 7269 7070 6564 5f74 6578  ode(stripped_tex
+00018940: 7429 0a20 2020 2020 2020 2020 2020 2020  t).             
+00018950: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+00018960: 2020 2020 2020 6966 2073 7472 6970 7065        if strippe
+00018970: 645f 7465 7874 203d 3d20 2253 5342 223a  d_text == "SSB":
+00018980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018990: 2073 656c 662e 6368 616e 6765 5f6d 6f64   self.change_mod
+000189a0: 6528 7374 7269 7070 6564 5f74 6578 7429  e(stripped_text)
+000189b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000189c0: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
+000189d0: 2020 2020 6966 2073 7472 6970 7065 645f      if stripped_
+000189e0: 7465 7874 203d 3d20 224f 504f 4e22 3a0a  text == "OPON":.
+000189f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018a00: 7365 6c66 2e67 6574 5f6f 706f 6e28 290a  self.get_opon().
+00018a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018a20: 7365 6c66 2e63 6c65 6172 696e 7075 7473  self.clearinputs
+00018a30: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00018a40: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+00018a50: 2020 2020 2020 6966 2073 7472 6970 7065        if strippe
+00018a60: 645f 7465 7874 203d 3d20 2248 454c 5022  d_text == "HELP"
+00018a70: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00018a80: 2020 7365 6c66 2e73 686f 775f 6865 6c70    self.show_help
+00018a90: 5f64 6961 6c6f 6728 290a 2020 2020 2020  _dialog().      
+00018aa0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00018ab0: 6c65 6172 696e 7075 7473 2829 0a20 2020  learinputs().   
+00018ac0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00018ad0: 7572 6e0a 2020 2020 2020 2020 2020 2020  urn.            
+00018ae0: 6966 2073 7472 6970 7065 645f 7465 7874  if stripped_text
+00018af0: 203d 3d20 2254 4553 5422 3a0a 2020 2020   == "TEST":.    
+00018b00: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00018b10: 6c74 203d 2073 656c 662e 6461 7461 6261  lt = self.databa
+00018b20: 7365 2e67 6574 5f63 616c 6c73 5f61 6e64  se.get_calls_and
+00018b30: 5f62 616e 6473 2829 0a20 2020 2020 2020  _bands().       
+00018b40: 2020 2020 2020 2020 2063 6d64 203d 207b           cmd = {
+00018b50: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00018b60: 2020 636d 645b 2263 6d64 225d 203d 2022    cmd["cmd"] = "
+00018b70: 574f 524b 4544 220a 2020 2020 2020 2020  WORKED".        
+00018b80: 2020 2020 2020 2020 636d 645b 2273 7461          cmd["sta
+00018b90: 7469 6f6e 225d 203d 2070 6c61 7466 6f72  tion"] = platfor
+00018ba0: 6d2e 6e6f 6465 2829 0a20 2020 2020 2020  m.node().       
+00018bb0: 2020 2020 2020 2020 2063 6d64 5b22 776f           cmd["wo
+00018bc0: 726b 6564 225d 203d 2072 6573 756c 740a  rked"] = result.
+00018bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018be0: 7365 6c66 2e6d 756c 7469 6361 7374 5f69  self.multicast_i
+00018bf0: 6e74 6572 6661 6365 2e73 656e 645f 6173  nterface.send_as
+00018c00: 5f6a 736f 6e28 636d 6429 0a20 2020 2020  _json(cmd).     
+00018c10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00018c20: 636c 6561 7269 6e70 7574 7328 290a 2020  clearinputs().  
+00018c30: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00018c40: 7475 726e 0a20 2020 2020 2020 2020 2020  turn.           
+00018c50: 2069 6620 7365 6c66 2e69 735f 666c 6f61   if self.is_floa
+00018c60: 7461 626c 6528 7374 7269 7070 6564 5f74  table(stripped_t
+00018c70: 6578 7429 3a0a 2020 2020 2020 2020 2020  ext):.          
+00018c80: 2020 2020 2020 7365 6c66 2e63 6861 6e67        self.chang
+00018c90: 655f 6672 6571 2873 7472 6970 7065 645f  e_freq(stripped_
+00018ca0: 7465 7874 290a 2020 2020 2020 2020 2020  text).          
+00018cb0: 2020 2020 2020 7265 7475 726e 0a0a 2020        return..  
+00018cc0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00018cd0: 6865 636b 5f63 616c 6c73 6967 6e28 7374  heck_callsign(st
+00018ce0: 7269 7070 6564 5f74 6578 7429 0a20 2020  ripped_text).   
+00018cf0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00018d00: 2e63 6865 636b 5f64 7570 6528 7374 7269  .check_dupe(stri
+00018d10: 7070 6564 5f74 6578 7429 3a0a 2020 2020  pped_text):.    
+00018d20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018d30: 2e64 7570 655f 696e 6469 6361 746f 722e  .dupe_indicator.
+00018d40: 7368 6f77 2829 0a20 2020 2020 2020 2020  show().         
+00018d50: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00018d60: 2020 2020 2020 2020 2073 656c 662e 6475           self.du
+00018d70: 7065 5f69 6e64 6963 6174 6f72 2e68 6964  pe_indicator.hid
+00018d80: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+00018d90: 5f74 6865 7468 7265 6164 203d 2074 6872  _thethread = thr
+00018da0: 6561 6469 6e67 2e54 6872 6561 6428 0a20  eading.Thread(. 
+00018db0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00018dc0: 6172 6765 743d 7365 6c66 2e63 6865 636b  arget=self.check
+00018dd0: 5f63 616c 6c73 6967 6e32 2c0a 2020 2020  _callsign2,.    
+00018de0: 2020 2020 2020 2020 2020 2020 6172 6773              args
+00018df0: 3d28 7465 7874 2c29 2c0a 2020 2020 2020  =(text,),.      
+00018e00: 2020 2020 2020 2020 2020 6461 656d 6f6e            daemon
+00018e10: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
+00018e20: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00018e30: 205f 7468 6574 6872 6561 642e 7374 6172   _thethread.star
+00018e40: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
+00018e50: 7365 6c66 2e6e 6578 745f 6669 656c 642e  self.next_field.
+00018e60: 7365 7446 6f63 7573 2829 0a20 2020 2020  setFocus().     
+00018e70: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+00018e80: 2020 2020 2020 636d 6420 3d20 7b7d 0a20        cmd = {}. 
+00018e90: 2020 2020 2020 2063 6d64 5b22 636d 6422         cmd["cmd"
+00018ea0: 5d20 3d20 2243 414c 4c43 4841 4e47 4544  ] = "CALLCHANGED
+00018eb0: 220a 2020 2020 2020 2020 636d 645b 2273  ".        cmd["s
+00018ec0: 7461 7469 6f6e 225d 203d 2070 6c61 7466  tation"] = platf
+00018ed0: 6f72 6d2e 6e6f 6465 2829 0a20 2020 2020  orm.node().     
+00018ee0: 2020 2063 6d64 5b22 6361 6c6c 225d 203d     cmd["call"] =
+00018ef0: 2073 7472 6970 7065 645f 7465 7874 0a20   stripped_text. 
+00018f00: 2020 2020 2020 2073 656c 662e 6d75 6c74         self.mult
+00018f10: 6963 6173 745f 696e 7465 7266 6163 652e  icast_interface.
+00018f20: 7365 6e64 5f61 735f 6a73 6f6e 2863 6d64  send_as_json(cmd
+00018f30: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+00018f40: 6865 636b 5f63 616c 6c73 6967 6e28 7374  heck_callsign(st
+00018f50: 7269 7070 6564 5f74 6578 7429 0a0a 2020  ripped_text)..  
+00018f60: 2020 6465 6620 6368 616e 6765 5f66 7265    def change_fre
+00018f70: 7128 7365 6c66 2c20 7374 7269 7070 6564  q(self, stripped
+00018f80: 5f74 6578 743a 2073 7472 2920 2d3e 204e  _text: str) -> N
+00018f90: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+00018fa0: 0a20 2020 2020 2020 2043 6861 6e67 6520  .        Change 
+00018fb0: 5646 4f20 746f 2067 6976 656e 2066 7265  VFO to given fre
+00018fc0: 7175 656e 6379 2069 6e20 4b68 7a20 616e  quency in Khz an
+00018fd0: 6420 7365 7420 7468 6520 6261 6e64 2069  d set the band i
+00018fe0: 6e64 6963 6174 6f72 2e0a 2020 2020 2020  ndicator..      
+00018ff0: 2020 5365 6e64 2074 6865 206e 6577 2066    Send the new f
+00019000: 7265 7175 656e 6379 2074 6f20 7468 6520  requency to the 
+00019010: 7269 6720 636f 6e74 726f 6c2e 0a0a 2020  rig control...  
+00019020: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+00019030: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00019040: 2d2d 2d0a 2020 2020 2020 2020 7374 7269  ---.        stri
+00019050: 7070 6564 5f74 6578 7420 3a20 7374 720a  pped_text : str.
+00019060: 2020 2020 2020 2020 5374 7269 7070 6564          Stripped
+00019070: 206f 6620 616e 7920 7370 6163 6573 2e0a   of any spaces..
+00019080: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00019090: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+000190a0: 0a20 2020 2020 2020 204e 6f6e 650a 2020  .        None.  
+000190b0: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
+000190c0: 2020 2076 666f 203d 2066 6c6f 6174 2873     vfo = float(s
+000190d0: 7472 6970 7065 645f 7465 7874 290a 2020  tripped_text).  
+000190e0: 2020 2020 2020 7666 6f20 3d20 696e 7428        vfo = int(
+000190f0: 7666 6f20 2a20 3130 3030 290a 2020 2020  vfo * 1000).    
+00019100: 2020 2020 6261 6e64 203d 2067 6574 6261      band = getba
+00019110: 6e64 2873 7472 2876 666f 2929 0a20 2020  nd(str(vfo)).   
+00019120: 2020 2020 2073 656c 662e 7365 745f 6261       self.set_ba
+00019130: 6e64 5f69 6e64 6963 6174 6f72 2862 616e  nd_indicator(ban
+00019140: 6429 0a20 2020 2020 2020 2073 656c 662e  d).        self.
+00019150: 7261 6469 6f5f 7374 6174 655b 2276 666f  radio_state["vfo
+00019160: 6122 5d20 3d20 7666 6f0a 2020 2020 2020  a"] = vfo.      
+00019170: 2020 7365 6c66 2e72 6164 696f 5f73 7461    self.radio_sta
+00019180: 7465 5b22 6261 6e64 225d 203d 2062 616e  te["band"] = ban
+00019190: 640a 2020 2020 2020 2020 7365 6c66 2e63  d.        self.c
+000191a0: 6f6e 7461 6374 5b22 4261 6e64 225d 203d  ontact["Band"] =
+000191b0: 2067 6574 5f6c 6f67 6765 645f 6261 6e64   get_logged_band
+000191c0: 2873 7472 2876 666f 2929 0a20 2020 2020  (str(vfo)).     
+000191d0: 2020 2073 656c 662e 7365 745f 7769 6e64     self.set_wind
+000191e0: 6f77 5f74 6974 6c65 2829 0a20 2020 2020  ow_title().     
+000191f0: 2020 2073 656c 662e 636c 6561 7269 6e70     self.clearinp
+00019200: 7574 7328 290a 2020 2020 2020 2020 6966  uts().        if
+00019210: 2073 656c 662e 7269 675f 636f 6e74 726f   self.rig_contro
+00019220: 6c3a 0a20 2020 2020 2020 2020 2020 2073  l:.            s
+00019230: 656c 662e 7269 675f 636f 6e74 726f 6c2e  elf.rig_control.
+00019240: 7365 745f 7666 6f28 7666 6f29 0a20 2020  set_vfo(vfo).   
+00019250: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+00019260: 2020 2020 2020 2020 636d 6420 3d20 7b7d          cmd = {}
+00019270: 0a20 2020 2020 2020 2063 6d64 5b22 636d  .        cmd["cm
+00019280: 6422 5d20 3d20 2252 4144 494f 5f53 5441  d"] = "RADIO_STA
+00019290: 5445 220a 2020 2020 2020 2020 636d 645b  TE".        cmd[
+000192a0: 2273 7461 7469 6f6e 225d 203d 2070 6c61  "station"] = pla
+000192b0: 7466 6f72 6d2e 6e6f 6465 2829 0a20 2020  tform.node().   
+000192c0: 2020 2020 2063 6d64 5b22 6261 6e64 225d       cmd["band"]
+000192d0: 203d 2062 616e 640a 2020 2020 2020 2020   = band.        
+000192e0: 636d 645b 2276 666f 6122 5d20 3d20 7666  cmd["vfoa"] = vf
+000192f0: 6f0a 2020 2020 2020 2020 7365 6c66 2e6d  o.        self.m
+00019300: 756c 7469 6361 7374 5f69 6e74 6572 6661  ulticast_interfa
+00019310: 6365 2e73 656e 645f 6173 5f6a 736f 6e28  ce.send_as_json(
+00019320: 636d 6429 0a0a 2020 2020 6465 6620 6368  cmd)..    def ch
+00019330: 616e 6765 5f6d 6f64 6528 7365 6c66 2c20  ange_mode(self, 
+00019340: 6d6f 6465 3a20 7374 7229 202d 3e20 4e6f  mode: str) -> No
+00019350: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
+00019360: 2020 2020 2020 2020 4368 616e 6765 206d          Change m
+00019370: 6f64 6520 746f 2067 6976 656e 206d 6f64  ode to given mod
+00019380: 652e 0a20 2020 2020 2020 2053 656e 6420  e..        Send 
+00019390: 7468 6520 6e65 7720 6d6f 6465 2074 6f20  the new mode to 
+000193a0: 7468 6520 7269 6720 636f 6e74 726f 6c2e  the rig control.
+000193b0: 0a20 2020 2020 2020 2053 6574 2074 6865  .        Set the
+000193c0: 2062 616e 6420 696e 6469 6361 746f 722e   band indicator.
+000193d0: 0a20 2020 2020 2020 2053 6574 2074 6865  .        Set the
+000193e0: 2077 696e 646f 7720 7469 746c 652e 0a20   window title.. 
+000193f0: 2020 2020 2020 2043 6c65 6172 2074 6865         Clear the
+00019400: 2069 6e70 7574 732e 0a20 2020 2020 2020   inputs..       
+00019410: 2052 6561 6420 7468 6520 4357 206d 6163   Read the CW mac
+00019420: 726f 732e 0a0a 2020 2020 2020 2020 5061  ros...        Pa
+00019430: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+00019440: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+00019450: 2020 2020 6d6f 6465 203a 2073 7472 0a20      mode : str. 
+00019460: 2020 2020 2020 204d 6f64 6520 746f 2063         Mode to c
+00019470: 6861 6e67 6520 746f 2e0a 0a20 2020 2020  hange to...     
+00019480: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
+00019490: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
+000194a0: 2020 204e 6f6e 650a 2020 2020 2020 2020     None.        
+000194b0: 2222 220a 0a20 2020 2020 2020 2069 6620  """..        if 
+000194c0: 6d6f 6465 203d 3d20 2243 5722 3a0a 2020  mode == "CW":.  
+000194d0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+000194e0: 6574 6d6f 6465 2822 4357 2229 0a20 2020  etmode("CW").   
+000194f0: 2020 2020 2020 2020 2073 656c 662e 7261           self.ra
+00019500: 6469 6f5f 7374 6174 655b 226d 6f64 6522  dio_state["mode"
+00019510: 5d20 3d20 2243 5722 0a20 2020 2020 2020  ] = "CW".       
+00019520: 2020 2020 2069 6620 7365 6c66 2e72 6967       if self.rig
+00019530: 5f63 6f6e 7472 6f6c 3a0a 2020 2020 2020  _control:.      
+00019540: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00019550: 662e 7269 675f 636f 6e74 726f 6c2e 6f6e  f.rig_control.on
+00019560: 6c69 6e65 3a0a 2020 2020 2020 2020 2020  line:.          
+00019570: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+00019580: 6967 5f63 6f6e 7472 6f6c 2e73 6574 5f6d  ig_control.set_m
+00019590: 6f64 6528 2243 5722 290a 2020 2020 2020  ode("CW").      
+000195a0: 2020 2020 2020 6261 6e64 203d 2067 6574        band = get
+000195b0: 6261 6e64 2873 7472 2873 656c 662e 7261  band(str(self.ra
+000195c0: 6469 6f5f 7374 6174 652e 6765 7428 2276  dio_state.get("v
+000195d0: 666f 6122 2c20 2230 2e30 2229 2929 0a20  foa", "0.0"))). 
+000195e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000195f0: 7365 745f 6261 6e64 5f69 6e64 6963 6174  set_band_indicat
+00019600: 6f72 2862 616e 6429 0a20 2020 2020 2020  or(band).       
+00019610: 2020 2020 2073 656c 662e 7365 745f 7769       self.set_wi
+00019620: 6e64 6f77 5f74 6974 6c65 2829 0a20 2020  ndow_title().   
+00019630: 2020 2020 2020 2020 2073 656c 662e 636c           self.cl
+00019640: 6561 7269 6e70 7574 7328 290a 2020 2020  earinputs().    
+00019650: 2020 2020 2020 2020 7365 6c66 2e72 6561          self.rea
+00019660: 645f 6377 5f6d 6163 726f 7328 290a 2020  d_cw_macros().  
+00019670: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00019680: 0a20 2020 2020 2020 2069 6620 6d6f 6465  .        if mode
+00019690: 203d 3d20 2252 5454 5922 3a0a 2020 2020   == "RTTY":.    
+000196a0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+000196b0: 6d6f 6465 2822 5254 5459 2229 0a20 2020  mode("RTTY").   
+000196c0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+000196d0: 2e72 6967 5f63 6f6e 7472 6f6c 3a0a 2020  .rig_control:.  
+000196e0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000196f0: 2073 656c 662e 7269 675f 636f 6e74 726f   self.rig_contro
+00019700: 6c2e 6f6e 6c69 6e65 3a0a 2020 2020 2020  l.online:.      
+00019710: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00019720: 6c66 2e72 6967 5f63 6f6e 7472 6f6c 2e73  lf.rig_control.s
+00019730: 6574 5f6d 6f64 6528 2252 5454 5922 290a  et_mode("RTTY").
+00019740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019750: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00019760: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+00019770: 6164 696f 5f73 7461 7465 5b22 6d6f 6465  adio_state["mode
+00019780: 225d 203d 2022 5254 5459 220a 2020 2020  "] = "RTTY".    
+00019790: 2020 2020 2020 2020 6261 6e64 203d 2067          band = g
+000197a0: 6574 6261 6e64 2873 7472 2873 656c 662e  etband(str(self.
+000197b0: 7261 6469 6f5f 7374 6174 652e 6765 7428  radio_state.get(
+000197c0: 2276 666f 6122 2c20 2230 2e30 2229 2929  "vfoa", "0.0")))
+000197d0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000197e0: 662e 7365 745f 6261 6e64 5f69 6e64 6963  f.set_band_indic
+000197f0: 6174 6f72 2862 616e 6429 0a20 2020 2020  ator(band).     
+00019800: 2020 2020 2020 2073 656c 662e 7365 745f         self.set_
+00019810: 7769 6e64 6f77 5f74 6974 6c65 2829 0a20  window_title(). 
+00019820: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00019830: 636c 6561 7269 6e70 7574 7328 290a 2020  clearinputs().  
+00019840: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00019850: 0a20 2020 2020 2020 2069 6620 6d6f 6465  .        if mode
+00019860: 203d 3d20 2253 5342 223a 0a20 2020 2020   == "SSB":.     
+00019870: 2020 2020 2020 2073 656c 662e 7365 746d         self.setm
+00019880: 6f64 6528 2253 5342 2229 0a20 2020 2020  ode("SSB").     
+00019890: 2020 2020 2020 2069 6620 696e 7428 7365         if int(se
+000198a0: 6c66 2e72 6164 696f 5f73 7461 7465 2e67  lf.radio_state.g
+000198b0: 6574 2822 7666 6f61 222c 2030 2929 203e  et("vfoa", 0)) >
+000198c0: 2031 3030 3030 3030 303a 0a20 2020 2020   10000000:.     
+000198d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000198e0: 7261 6469 6f5f 7374 6174 655b 226d 6f64  radio_state["mod
+000198f0: 6522 5d20 3d20 2255 5342 220a 2020 2020  e"] = "USB".    
+00019900: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00019910: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00019920: 6c66 2e72 6164 696f 5f73 7461 7465 5b22  lf.radio_state["
+00019930: 6d6f 6465 225d 203d 2022 4c53 4222 0a20  mode"] = "LSB". 
+00019940: 2020 2020 2020 2020 2020 2062 616e 6420             band 
+00019950: 3d20 6765 7462 616e 6428 7374 7228 7365  = getband(str(se
+00019960: 6c66 2e72 6164 696f 5f73 7461 7465 2e67  lf.radio_state.g
+00019970: 6574 2822 7666 6f61 222c 2022 302e 3022  et("vfoa", "0.0"
+00019980: 2929 290a 2020 2020 2020 2020 2020 2020  ))).            
+00019990: 7365 6c66 2e73 6574 5f62 616e 645f 696e  self.set_band_in
+000199a0: 6469 6361 746f 7228 6261 6e64 290a 2020  dicator(band).  
+000199b0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+000199c0: 6574 5f77 696e 646f 775f 7469 746c 6528  et_window_title(
+000199d0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+000199e0: 2073 656c 662e 7269 675f 636f 6e74 726f   self.rig_contro
+000199f0: 6c3a 0a20 2020 2020 2020 2020 2020 2020  l:.             
+00019a00: 2020 2073 656c 662e 7269 675f 636f 6e74     self.rig_cont
+00019a10: 726f 6c2e 7365 745f 6d6f 6465 2873 656c  rol.set_mode(sel
+00019a20: 662e 7261 6469 6f5f 7374 6174 652e 6765  f.radio_state.ge
+00019a30: 7428 226d 6f64 6522 2929 0a20 2020 2020  t("mode")).     
+00019a40: 2020 2020 2020 2073 656c 662e 636c 6561         self.clea
+00019a50: 7269 6e70 7574 7328 290a 2020 2020 2020  rinputs().      
+00019a60: 2020 2020 2020 7365 6c66 2e72 6561 645f        self.read_
+00019a70: 6377 5f6d 6163 726f 7328 290a 0a20 2020  cw_macros()..   
+00019a80: 2064 6566 2063 6865 636b 5f63 616c 6c73   def check_calls
+00019a90: 6967 6e28 7365 6c66 2c20 6361 6c6c 7369  ign(self, callsi
+00019aa0: 676e 2920 2d3e 204e 6f6e 653a 0a20 2020  gn) -> None:.   
+00019ab0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00019ac0: 2043 6865 636b 2063 616c 6c73 6967 6e20   Check callsign 
+00019ad0: 6173 2069 7427 7320 6265 696e 6720 656e  as it's being en
+00019ae0: 7465 7265 6420 696e 2074 6865 2062 6967  tered in the big
+00019af0: 5f63 7479 2069 6e64 6578 2e0a 2020 2020  _cty index..    
+00019b00: 2020 2020 4765 7420 4458 2065 6e74 6974      Get DX entit
+00019b10: 792c 2043 512c 2049 5455 2061 6e64 2063  y, CQ, ITU and c
+00019b20: 6f6e 7469 6e65 6e74 2e0a 2020 2020 2020  ontinent..      
+00019b30: 2020 4765 6f67 7261 7068 6963 2069 6e66    Geographic inf
+00019b40: 6f72 6d61 7469 6f6e 2e20 4469 7374 616e  ormation. Distan
+00019b50: 6365 2061 6e64 2048 6561 6469 6e67 2e0a  ce and Heading..
+00019b60: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00019b70: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+00019b80: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2063  ------.        c
+00019b90: 616c 6c73 6967 6e20 3a20 7374 720a 2020  allsign : str.  
+00019ba0: 2020 2020 2020 4361 6c6c 7369 676e 2074        Callsign t
+00019bb0: 6f20 6368 6563 6b2e 0a0a 2020 2020 2020  o check...      
+00019bc0: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
+00019bd0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+00019be0: 2020 4e6f 6e65 0a20 2020 2020 2020 2022    None.        "
+00019bf0: 2222 0a0a 2020 2020 2020 2020 7265 7375  ""..        resu
+00019c00: 6c74 203d 2073 656c 662e 6374 795f 6c6f  lt = self.cty_lo
+00019c10: 6f6b 7570 2863 616c 6c73 6967 6e29 0a20  okup(callsign). 
+00019c20: 2020 2020 2020 2064 6562 7567 5f72 6573         debug_res
+00019c30: 756c 7420 3d20 6622 7b72 6573 756c 747d  ult = f"{result}
+00019c40: 220a 2020 2020 2020 2020 6c6f 6767 6572  ".        logger
+00019c50: 2e64 6562 7567 2822 2573 222c 2064 6562  .debug("%s", deb
+00019c60: 7567 5f72 6573 756c 7429 0a20 2020 2020  ug_result).     
+00019c70: 2020 2069 6620 7265 7375 6c74 3a0a 2020     if result:.  
+00019c80: 2020 2020 2020 2020 2020 666f 7220 6120            for a 
+00019c90: 696e 2072 6573 756c 742e 6974 656d 7328  in result.items(
+00019ca0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00019cb0: 2020 2065 6e74 6974 7920 3d20 615b 315d     entity = a[1]
+00019cc0: 2e67 6574 2822 656e 7469 7479 222c 2022  .get("entity", "
+00019cd0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00019ce0: 2020 2063 7120 3d20 615b 315d 2e67 6574     cq = a[1].get
+00019cf0: 2822 6371 222c 2022 2229 0a20 2020 2020  ("cq", "").     
+00019d00: 2020 2020 2020 2020 2020 2069 7475 203d             itu =
+00019d10: 2061 5b31 5d2e 6765 7428 2269 7475 222c   a[1].get("itu",
+00019d20: 2022 2229 0a20 2020 2020 2020 2020 2020   "").           
+00019d30: 2020 2020 2063 6f6e 7469 6e65 6e74 203d       continent =
+00019d40: 2061 5b31 5d2e 6765 7428 2263 6f6e 7469   a[1].get("conti
+00019d50: 6e65 6e74 2229 0a20 2020 2020 2020 2020  nent").         
+00019d60: 2020 2020 2020 206c 6174 203d 2066 6c6f         lat = flo
+00019d70: 6174 2861 5b31 5d2e 6765 7428 226c 6174  at(a[1].get("lat
+00019d80: 222c 2022 302e 3022 2929 0a20 2020 2020  ", "0.0")).     
+00019d90: 2020 2020 2020 2020 2020 206c 6f6e 203d             lon =
+00019da0: 2066 6c6f 6174 2861 5b31 5d2e 6765 7428   float(a[1].get(
+00019db0: 226c 6f6e 6722 2c20 2230 2e30 2229 290a  "long", "0.0")).
+00019dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019dd0: 6c6f 6e20 3d20 6c6f 6e20 2a20 2d31 2020  lon = lon * -1  
+00019de0: 2320 6374 792e 6461 7420 6669 6c65 2069  # cty.dat file i
+00019df0: 6e76 6572 7473 206c 6f6e 6769 7475 6465  nverts longitude
+00019e00: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00019e10: 2020 7072 696d 6172 795f 7066 7820 3d20    primary_pfx = 
+00019e20: 615b 315d 2e67 6574 2822 7072 696d 6172  a[1].get("primar
+00019e30: 795f 7066 7822 2c20 2222 290a 2020 2020  y_pfx", "").    
+00019e40: 2020 2020 2020 2020 2020 2020 6865 6164              head
+00019e50: 696e 6720 3d20 6265 6172 696e 675f 7769  ing = bearing_wi
+00019e60: 7468 5f6c 6174 6c6f 6e28 7365 6c66 2e73  th_latlon(self.s
+00019e70: 7461 7469 6f6e 2e67 6574 2822 4772 6964  tation.get("Grid
+00019e80: 5371 7561 7265 2229 2c20 6c61 742c 206c  Square"), lat, l
+00019e90: 6f6e 290a 2020 2020 2020 2020 2020 2020  on).            
+00019ea0: 2020 2020 6b69 6c6f 6d65 7465 7273 203d      kilometers =
+00019eb0: 2064 6973 7461 6e63 655f 7769 7468 5f6c   distance_with_l
+00019ec0: 6174 6c6f 6e28 0a20 2020 2020 2020 2020  atlon(.         
+00019ed0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00019ee0: 7374 6174 696f 6e2e 6765 7428 2247 7269  station.get("Gri
+00019ef0: 6453 7175 6172 6522 292c 206c 6174 2c20  dSquare"), lat, 
+00019f00: 6c6f 6e0a 2020 2020 2020 2020 2020 2020  lon.            
+00019f10: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00019f20: 2020 2020 2020 7365 6c66 2e68 6561 6469        self.headi
+00019f30: 6e67 5f64 6973 7461 6e63 652e 7365 7454  ng_distance.setT
+00019f40: 6578 7428 0a20 2020 2020 2020 2020 2020  ext(.           
+00019f50: 2020 2020 2020 2020 2066 2252 6567 696f           f"Regio
+00019f60: 6e61 6c20 4864 6720 7b68 6561 6469 6e67  nal Hdg {heading
+00019f70: 7dc2 b020 4c50 207b 7265 6369 7072 6f63  }.. LP {reciproc
+00019f80: 6f6c 2868 6561 6469 6e67 297d c2b0 202f  ol(heading)}.. /
+00019f90: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+00019fa0: 2020 2020 2020 2066 2264 6973 7461 6e63         f"distanc
+00019fb0: 6520 7b69 6e74 286b 696c 6f6d 6574 6572  e {int(kilometer
+00019fc0: 732a 302e 3632 3133 3731 297d 6d69 207b  s*0.621371)}mi {
+00019fd0: 6b69 6c6f 6d65 7465 7273 7d6b 6d22 0a20  kilometers}km". 
+00019fe0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00019ff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a000: 2073 656c 662e 636f 6e74 6163 745b 2243   self.contact["C
+0001a010: 6f75 6e74 7279 5072 6566 6978 225d 203d  ountryPrefix"] =
+0001a020: 2070 7269 6d61 7279 5f70 6678 0a20 2020   primary_pfx.   
+0001a030: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0001a040: 662e 636f 6e74 6163 745b 225a 4e22 5d20  f.contact["ZN"] 
+0001a050: 3d20 696e 7428 6371 290a 2020 2020 2020  = int(cq).      
+0001a060: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0001a070: 662e 636f 6e74 6573 743a 0a20 2020 2020  f.contest:.     
+0001a080: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0001a090: 6620 7365 6c66 2e63 6f6e 7465 7374 2e6e  f self.contest.n
+0001a0a0: 616d 6520 3d3d 2022 4941 5255 2048 4622  ame == "IARU HF"
+0001a0b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001a0c0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0001a0d0: 6f6e 7461 6374 5b22 5a4e 225d 203d 2069  ontact["ZN"] = i
+0001a0e0: 6e74 2869 7475 290a 2020 2020 2020 2020  nt(itu).        
+0001a0f0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+0001a100: 7461 6374 5b22 436f 6e74 696e 656e 7422  tact["Continent"
+0001a110: 5d20 3d20 636f 6e74 696e 656e 740a 2020  ] = continent.  
+0001a120: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0001a130: 6c66 2e64 785f 656e 7469 7479 2e73 6574  lf.dx_entity.set
+0001a140: 5465 7874 280a 2020 2020 2020 2020 2020  Text(.          
+0001a150: 2020 2020 2020 2020 2020 6622 7b70 7269            f"{pri
+0001a160: 6d61 7279 5f70 6678 7d3a 207b 636f 6e74  mary_pfx}: {cont
+0001a170: 696e 656e 747d 2f7b 656e 7469 7479 7d20  inent}/{entity} 
+0001a180: 6371 3a7b 6371 7d20 6974 753a 7b69 7475  cq:{cq} itu:{itu
+0001a190: 7d22 0a20 2020 2020 2020 2020 2020 2020  }".             
+0001a1a0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+0001a1b0: 2020 2020 2069 6620 6c65 6e28 6361 6c6c       if len(call
+0001a1c0: 7369 676e 2920 3e20 323a 0a20 2020 2020  sign) > 2:.     
+0001a1d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0001a1e0: 6620 7365 6c66 2e63 6f6e 7465 7374 3a0a  f self.contest:.
+0001a1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a200: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+0001a210: 7465 7374 2e70 7265 6669 6c6c 2873 656c  test.prefill(sel
+0001a220: 6629 0a0a 2020 2020 6465 6620 6368 6563  f)..    def chec
+0001a230: 6b5f 6361 6c6c 7369 676e 3228 7365 6c66  k_callsign2(self
+0001a240: 2c20 6361 6c6c 7369 676e 2920 2d3e 204e  , callsign) -> N
+0001a250: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+0001a260: 0a20 2020 2020 2020 2043 6865 636b 2074  .        Check t
+0001a270: 6865 2063 616c 6c73 6967 6e20 6166 7465  he callsign afte
+0001a280: 7220 6974 2068 6173 2062 6565 6e20 656e  r it has been en
+0001a290: 7465 7265 642e 0a20 2020 2020 2020 204c  tered..        L
+0001a2a0: 6f6f 6b20 7570 2074 6865 2063 616c 6c73  ook up the calls
+0001a2b0: 6967 6e20 696e 2074 6865 2063 616c 6c73  ign in the calls
+0001a2c0: 6967 6e20 6461 7461 6261 7365 2e0a 2020  ign database..  
+0001a2d0: 2020 2020 2020 4765 7420 7468 6520 6772        Get the gr
+0001a2e0: 6964 2073 7175 6172 6520 616e 6420 6361  id square and ca
+0001a2f0: 6c63 756c 6174 6520 7468 6520 6469 7374  lculate the dist
+0001a300: 616e 6365 2061 6e64 2068 6561 6469 6e67  ance and heading
+0001a310: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+0001a320: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
+0001a330: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+0001a340: 2063 616c 6c73 6967 6e20 3a20 7374 720a   callsign : str.
+0001a350: 2020 2020 2020 2020 4361 6c6c 7369 676e          Callsign
+0001a360: 2074 6f20 6368 6563 6b2e 0a0a 2020 2020   to check...    
+0001a370: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
+0001a380: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+0001a390: 2020 2020 4e6f 6e65 0a20 2020 2020 2020      None.       
+0001a3a0: 2022 2222 0a0a 2020 2020 2020 2020 6361   """..        ca
+0001a3b0: 6c6c 7369 676e 203d 2063 616c 6c73 6967  llsign = callsig
+0001a3c0: 6e2e 7374 7269 7028 290a 2020 2020 2020  n.strip().      
+0001a3d0: 2020 6465 6275 675f 6c6f 6f6b 7570 203d    debug_lookup =
+0001a3e0: 2066 227b 7365 6c66 2e6c 6f6f 6b5f 7570   f"{self.look_up
+0001a3f0: 7d22 0a20 2020 2020 2020 206c 6f67 6765  }".        logge
+0001a400: 722e 6465 6275 6728 2225 732c 2025 7322  r.debug("%s, %s"
+0001a410: 2c20 6361 6c6c 7369 676e 2c20 6465 6275  , callsign, debu
+0001a420: 675f 6c6f 6f6b 7570 290a 2020 2020 2020  g_lookup).      
+0001a430: 2020 6966 2068 6173 6174 7472 2873 656c    if hasattr(sel
+0001a440: 662e 6c6f 6f6b 5f75 702c 2022 7365 7373  f.look_up, "sess
+0001a450: 696f 6e22 293a 0a20 2020 2020 2020 2020  ion"):.         
+0001a460: 2020 2069 6620 7365 6c66 2e6c 6f6f 6b5f     if self.look_
+0001a470: 7570 2e73 6573 7369 6f6e 3a0a 2020 2020  up.session:.    
+0001a480: 2020 2020 2020 2020 2020 2020 7265 7370              resp
+0001a490: 6f6e 7365 203d 2073 656c 662e 6c6f 6f6b  onse = self.look
+0001a4a0: 5f75 702e 6c6f 6f6b 7570 2863 616c 6c73  _up.lookup(calls
+0001a4b0: 6967 6e29 0a20 2020 2020 2020 2020 2020  ign).           
+0001a4c0: 2020 2020 2064 6562 7567 5f72 6573 706f       debug_respo
+0001a4d0: 6e73 6520 3d20 6622 7b72 6573 706f 6e73  nse = f"{respons
+0001a4e0: 657d 220a 2020 2020 2020 2020 2020 2020  e}".            
+0001a4f0: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+0001a500: 2822 5468 6520 5265 7370 6f6e 7365 3a20  ("The Response: 
+0001a510: 2573 5c6e 222c 2064 6562 7567 5f72 6573  %s\n", debug_res
+0001a520: 706f 6e73 6529 0a20 2020 2020 2020 2020  ponse).         
+0001a530: 2020 2020 2020 2069 6620 7265 7370 6f6e         if respon
+0001a540: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0001a550: 2020 2020 2020 2020 7468 6569 7267 7269          theirgri
+0001a560: 6420 3d20 7265 7370 6f6e 7365 2e67 6574  d = response.get
+0001a570: 2822 6772 6964 222c 2022 2229 0a20 2020  ("grid", "").   
+0001a580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a590: 2073 656c 662e 636f 6e74 6163 745b 2247   self.contact["G
+0001a5a0: 7269 6453 7175 6172 6522 5d20 3d20 7468  ridSquare"] = th
+0001a5b0: 6569 7267 7269 640a 2020 2020 2020 2020  eirgrid.        
+0001a5c0: 2020 2020 2020 2020 2020 2020 5f74 6865              _the
+0001a5d0: 6972 636f 756e 7472 7920 3d20 7265 7370  ircountry = resp
+0001a5e0: 6f6e 7365 2e67 6574 2822 636f 756e 7472  onse.get("countr
+0001a5f0: 7922 2c20 2222 290a 2020 2020 2020 2020  y", "").        
+0001a600: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0001a610: 656c 662e 7374 6174 696f 6e2e 6765 7428  elf.station.get(
+0001a620: 2247 7269 6453 7175 6172 6522 2c20 2222  "GridSquare", ""
+0001a630: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0001a640: 2020 2020 2020 2020 2020 2068 6561 6469             headi
+0001a650: 6e67 203d 2062 6561 7269 6e67 2873 656c  ng = bearing(sel
+0001a660: 662e 7374 6174 696f 6e2e 6765 7428 2247  f.station.get("G
+0001a670: 7269 6453 7175 6172 6522 2c20 2222 292c  ridSquare", ""),
+0001a680: 2074 6865 6972 6772 6964 290a 2020 2020   theirgrid).    
+0001a690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a6a0: 2020 2020 6b69 6c6f 6d65 7465 7273 203d      kilometers =
+0001a6b0: 2064 6973 7461 6e63 6528 0a20 2020 2020   distance(.     
 0001a6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a6d0: 2020 2020 206b 696c 6f6d 6574 6572 7320       kilometers 
-0001a6e0: 3d20 6469 7374 616e 6365 280a 2020 2020  = distance(.    
-0001a6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a700: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-0001a710: 7469 6f6e 2e67 6574 2822 4772 6964 5371  tion.get("GridSq
-0001a720: 7561 7265 222c 2022 2229 2c20 7468 6569  uare", ""), thei
-0001a730: 7267 7269 640a 2020 2020 2020 2020 2020  rgrid.          
-0001a740: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-0001a750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a760: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
-0001a770: 6469 6e67 5f64 6973 7461 6e63 652e 7365  ding_distance.se
-0001a780: 7454 6578 7428 0a20 2020 2020 2020 2020  tText(.         
-0001a790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a7a0: 2020 2066 227b 7468 6569 7267 7269 647d     f"{theirgrid}
-0001a7b0: 2048 6467 207b 6865 6164 696e 677d c2b0   Hdg {heading}..
-0001a7c0: 204c 5020 7b72 6563 6970 726f 636f 6c28   LP {reciprocol(
-0001a7d0: 6865 6164 696e 6729 7dc2 b020 2f20 220a  heading)}.. / ".
-0001a7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a7f0: 2020 2020 2020 2020 2020 2020 6622 6469              f"di
-0001a800: 7374 616e 6365 207b 696e 7428 6b69 6c6f  stance {int(kilo
-0001a810: 6d65 7465 7273 2a30 2e36 3231 3337 3129  meters*0.621371)
-0001a820: 7d6d 6920 7b6b 696c 6f6d 6574 6572 737d  }mi {kilometers}
-0001a830: 6b6d 220a 2020 2020 2020 2020 2020 2020  km".            
-0001a840: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-0001a850: 2020 2064 6566 2063 6865 636b 5f64 7570     def check_dup
-0001a860: 6528 7365 6c66 2c20 6361 6c6c 3a20 7374  e(self, call: st
-0001a870: 7229 202d 3e20 626f 6f6c 3a0a 2020 2020  r) -> bool:.    
-0001a880: 2020 2020 2222 2243 6865 636b 7320 6966      """Checks if
-0001a890: 2061 2063 616c 6c73 6967 6e20 6973 2061   a callsign is a
-0001a8a0: 2064 7570 6520 6f6e 2063 7572 7265 6e74   dupe on current
-0001a8b0: 2062 616e 642f 6d6f 6465 2e22 2222 0a20   band/mode.""". 
-0001a8c0: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-0001a8d0: 6f6e 7465 7374 2069 7320 4e6f 6e65 3a0a  ontest is None:.
-0001a8e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001a8f0: 2e73 686f 775f 6d65 7373 6167 655f 626f  .show_message_bo
-0001a900: 7828 2259 6f75 2068 6176 6520 6e6f 2063  x("You have no c
-0001a910: 6f6e 7465 7374 206c 6f61 6465 642e 2229  ontest loaded.")
-0001a920: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0001a930: 7572 6e20 4661 6c73 650a 2020 2020 2020  urn False.      
-0001a940: 2020 7365 6c66 2e63 6f6e 7465 7374 2e70    self.contest.p
-0001a950: 7265 6475 7065 2873 656c 6629 0a20 2020  redupe(self).   
-0001a960: 2020 2020 2062 616e 6420 3d20 666c 6f61       band = floa
-0001a970: 7428 6765 745f 6c6f 6767 6564 5f62 616e  t(get_logged_ban
-0001a980: 6428 7374 7228 7365 6c66 2e72 6164 696f  d(str(self.radio
-0001a990: 5f73 7461 7465 2e67 6574 2822 7666 6f61  _state.get("vfoa
-0001a9a0: 222c 2030 2e30 2929 2929 0a20 2020 2020  ", 0.0)))).     
-0001a9b0: 2020 206d 6f64 6520 3d20 7365 6c66 2e72     mode = self.r
-0001a9c0: 6164 696f 5f73 7461 7465 2e67 6574 2822  adio_state.get("
-0001a9d0: 6d6f 6465 222c 2022 2229 0a20 2020 2020  mode", "").     
-0001a9e0: 2020 2064 6562 7567 6c69 6e65 203d 2028     debugline = (
-0001a9f0: 0a20 2020 2020 2020 2020 2020 2066 2243  .            f"C
-0001aa00: 616c 6c3a 207b 6361 6c6c 7d20 4261 6e64  all: {call} Band
-0001aa10: 3a20 7b62 616e 647d 204d 6f64 653a 207b  : {band} Mode: {
-0001aa20: 6d6f 6465 7d20 4475 7065 7479 7065 3a20  mode} Dupetype: 
-0001aa30: 7b73 656c 662e 636f 6e74 6573 742e 6475  {self.contest.du
-0001aa40: 7065 5f74 7970 657d 220a 2020 2020 2020  pe_type}".      
-0001aa50: 2020 290a 2020 2020 2020 2020 6c6f 6767    ).        logg
-0001aa60: 6572 2e64 6562 7567 2822 2573 222c 2064  er.debug("%s", d
-0001aa70: 6562 7567 6c69 6e65 290a 2020 2020 2020  ebugline).      
-0001aa80: 2020 6966 2073 656c 662e 636f 6e74 6573    if self.contes
-0001aa90: 742e 6475 7065 5f74 7970 6520 3d3d 2031  t.dupe_type == 1
-0001aaa0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0001aab0: 7375 6c74 203d 2073 656c 662e 6461 7461  sult = self.data
-0001aac0: 6261 7365 2e63 6865 636b 5f64 7570 6528  base.check_dupe(
-0001aad0: 6361 6c6c 290a 2020 2020 2020 2020 6966  call).        if
-0001aae0: 2073 656c 662e 636f 6e74 6573 742e 6475   self.contest.du
-0001aaf0: 7065 5f74 7970 6520 3d3d 2032 3a0a 2020  pe_type == 2:.  
-0001ab00: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0001ab10: 203d 2073 656c 662e 6461 7461 6261 7365   = self.database
-0001ab20: 2e63 6865 636b 5f64 7570 655f 6f6e 5f62  .check_dupe_on_b
-0001ab30: 616e 6428 6361 6c6c 2c20 6261 6e64 290a  and(call, band).
-0001ab40: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0001ab50: 636f 6e74 6573 742e 6475 7065 5f74 7970  contest.dupe_typ
-0001ab60: 6520 3d3d 2033 3a0a 2020 2020 2020 2020  e == 3:.        
-0001ab70: 2020 2020 7265 7375 6c74 203d 2073 656c      result = sel
-0001ab80: 662e 6461 7461 6261 7365 2e63 6865 636b  f.database.check
-0001ab90: 5f64 7570 655f 6f6e 5f62 616e 645f 6d6f  _dupe_on_band_mo
-0001aba0: 6465 2863 616c 6c2c 2062 616e 642c 206d  de(call, band, m
-0001abb0: 6f64 6529 0a20 2020 2020 2020 2069 6620  ode).        if 
-0001abc0: 7365 6c66 2e63 6f6e 7465 7374 2e64 7570  self.contest.dup
-0001abd0: 655f 7479 7065 203d 3d20 343a 0a20 2020  e_type == 4:.   
-0001abe0: 2020 2020 2020 2020 2072 6573 756c 7420           result 
-0001abf0: 3d20 7b22 6973 6475 7065 223a 2046 616c  = {"isdupe": Fal
-0001ac00: 7365 7d0a 2020 2020 2020 2020 6465 6275  se}.        debu
-0001ac10: 676c 696e 6520 3d20 6622 7b72 6573 756c  gline = f"{resul
-0001ac20: 747d 220a 2020 2020 2020 2020 6c6f 6767  t}".        logg
-0001ac30: 6572 2e64 6562 7567 2822 2573 222c 2064  er.debug("%s", d
-0001ac40: 6562 7567 6c69 6e65 290a 2020 2020 2020  ebugline).      
-0001ac50: 2020 7265 7475 726e 2072 6573 756c 742e    return result.
-0001ac60: 6765 7428 2269 7364 7570 6522 2c20 4661  get("isdupe", Fa
-0001ac70: 6c73 6529 0a0a 2020 2020 6465 6620 7365  lse)..    def se
-0001ac80: 746d 6f64 6528 7365 6c66 2c20 6d6f 6465  tmode(self, mode
-0001ac90: 3a20 7374 7229 202d 3e20 4e6f 6e65 3a0a  : str) -> None:.
-0001aca0: 2020 2020 2020 2020 2222 2243 616c 6c20          """Call 
-0001acb0: 7768 656e 2074 6865 206d 6f64 6520 6368  when the mode ch
-0001acc0: 616e 6765 732e 2222 220a 2020 2020 2020  anges.""".      
-0001acd0: 2020 6966 206d 6f64 6520 3d3d 2022 4357    if mode == "CW
-0001ace0: 223a 0a20 2020 2020 2020 2020 2020 2069  ":.            i
-0001acf0: 6620 7365 6c66 2e63 7572 7265 6e74 5f6d  f self.current_m
-0001ad00: 6f64 6520 213d 2022 4357 223a 0a20 2020  ode != "CW":.   
-0001ad10: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0001ad20: 662e 6375 7272 656e 745f 6d6f 6465 203d  f.current_mode =
-0001ad30: 2022 4357 220a 2020 2020 2020 2020 2020   "CW".          
-0001ad40: 2020 2020 2020 2320 7365 6c66 2e6d 6f64        # self.mod
-0001ad50: 652e 7365 7454 6578 7428 2243 5722 290a  e.setText("CW").
-0001ad60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ad70: 7365 6c66 2e73 656e 742e 7365 7454 6578  self.sent.setTex
-0001ad80: 7428 2235 3939 2229 0a20 2020 2020 2020  t("599").       
-0001ad90: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
-0001ada0: 6365 6976 652e 7365 7454 6578 7428 2235  ceive.setText("5
-0001adb0: 3939 2229 0a20 2020 2020 2020 2020 2020  99").           
-0001adc0: 2020 2020 2073 656c 662e 7265 6164 5f63       self.read_c
-0001add0: 775f 6d61 6372 6f73 2829 0a20 2020 2020  w_macros().     
-0001ade0: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-0001adf0: 2020 2020 2020 6966 206d 6f64 6520 3d3d        if mode ==
-0001ae00: 2022 5353 4222 3a0a 2020 2020 2020 2020   "SSB":.        
-0001ae10: 2020 2020 6966 2073 656c 662e 6375 7272      if self.curr
-0001ae20: 656e 745f 6d6f 6465 2021 3d20 2253 5342  ent_mode != "SSB
-0001ae30: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-0001ae40: 2020 2073 656c 662e 6375 7272 656e 745f     self.current_
-0001ae50: 6d6f 6465 203d 2022 5353 4222 0a20 2020  mode = "SSB".   
-0001ae60: 2020 2020 2020 2020 2020 2020 2023 2073               # s
-0001ae70: 656c 662e 6d6f 6465 2e73 6574 5465 7874  elf.mode.setText
-0001ae80: 2822 5353 4222 290a 2020 2020 2020 2020  ("SSB").        
-0001ae90: 2020 2020 2020 2020 7365 6c66 2e73 656e          self.sen
-0001aea0: 742e 7365 7454 6578 7428 2235 3922 290a  t.setText("59").
-0001aeb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aec0: 7365 6c66 2e72 6563 6569 7665 2e73 6574  self.receive.set
-0001aed0: 5465 7874 2822 3539 2229 0a20 2020 2020  Text("59").     
-0001aee0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001aef0: 7265 6164 5f63 775f 6d61 6372 6f73 2829  read_cw_macros()
-0001af00: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0001af10: 7572 6e0a 2020 2020 2020 2020 6966 206d  urn.        if m
-0001af20: 6f64 6520 3d3d 2022 5254 5459 223a 0a20  ode == "RTTY":. 
-0001af30: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0001af40: 6c66 2e63 7572 7265 6e74 5f6d 6f64 6520  lf.current_mode 
-0001af50: 213d 2022 5254 5459 223a 0a20 2020 2020  != "RTTY":.     
-0001af60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001af70: 6375 7272 656e 745f 6d6f 6465 203d 2022  current_mode = "
-0001af80: 5254 5459 220a 2020 2020 2020 2020 2020  RTTY".          
-0001af90: 2020 2020 2020 2320 7365 6c66 2e6d 6f64        # self.mod
-0001afa0: 652e 7365 7454 6578 7428 2252 5454 5922  e.setText("RTTY"
-0001afb0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001afc0: 2020 7365 6c66 2e73 656e 742e 7365 7454    self.sent.setT
-0001afd0: 6578 7428 2235 3922 290a 2020 2020 2020  ext("59").      
-0001afe0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-0001aff0: 6563 6569 7665 2e73 6574 5465 7874 2822  eceive.setText("
-0001b000: 3539 2229 0a0a 2020 2020 6465 6620 6765  59")..    def ge
-0001b010: 745f 6f70 6f6e 2873 656c 6629 202d 3e20  t_opon(self) -> 
-0001b020: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-0001b030: 220a 2020 2020 2020 2020 4374 726c 2b4f  ".        Ctrl+O
-0001b040: 204f 7065 6e20 7468 6520 4f50 4f4e 2064   Open the OPON d
-0001b050: 6961 6c6f 672e 0a0a 2020 2020 2020 2020  ialog...        
-0001b060: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
-0001b070: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-0001b080: 2020 2020 2020 4e6f 6e65 0a0a 2020 2020        None..    
-0001b090: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-0001b0a0: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-0001b0b0: 2020 2020 4e6f 6e65 0a20 2020 2020 2020      None.       
-0001b0c0: 2022 2222 0a0a 2020 2020 2020 2020 7365   """..        se
-0001b0d0: 6c66 2e6f 706f 6e5f 6469 616c 6f67 203d  lf.opon_dialog =
-0001b0e0: 204f 704f 6e28 6673 7574 696c 732e 4150   OpOn(fsutils.AP
-0001b0f0: 505f 4441 5441 5f50 4154 4829 0a0a 2020  P_DATA_PATH)..  
-0001b100: 2020 2020 2020 6966 2073 656c 662e 6375        if self.cu
-0001b110: 7272 656e 745f 7061 6c65 7474 653a 0a20  rrent_palette:. 
-0001b120: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001b130: 6f70 6f6e 5f64 6961 6c6f 672e 7365 7450  opon_dialog.setP
-0001b140: 616c 6574 7465 2873 656c 662e 6375 7272  alette(self.curr
-0001b150: 656e 745f 7061 6c65 7474 6529 0a0a 2020  ent_palette)..  
-0001b160: 2020 2020 2020 7365 6c66 2e6f 706f 6e5f        self.opon_
-0001b170: 6469 616c 6f67 2e61 6363 6570 7465 642e  dialog.accepted.
-0001b180: 636f 6e6e 6563 7428 7365 6c66 2e6e 6577  connect(self.new
-0001b190: 5f6f 7029 0a20 2020 2020 2020 2073 656c  _op).        sel
-0001b1a0: 662e 6f70 6f6e 5f64 6961 6c6f 672e 6f70  f.opon_dialog.op
-0001b1b0: 656e 2829 0a0a 2020 2020 6465 6620 6e65  en()..    def ne
-0001b1c0: 775f 6f70 2873 656c 6629 202d 3e20 4e6f  w_op(self) -> No
-0001b1d0: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
-0001b1e0: 2020 2020 2020 2020 4361 6c6c 6564 2077          Called w
-0001b1f0: 6865 6e20 7468 6520 7573 6572 2063 6c69  hen the user cli
-0001b200: 636b 7320 7468 6520 4f4b 2062 7574 746f  cks the OK butto
-0001b210: 6e20 6f6e 2074 6865 204f 504f 4e20 6469  n on the OPON di
-0001b220: 616c 6f67 2e0a 2020 2020 2020 2020 4372  alog..        Cr
-0001b230: 6561 7465 2074 6865 206e 6577 2064 6972  eate the new dir
-0001b240: 6563 746f 7279 2061 6e64 2063 6f70 7920  ectory and copy 
-0001b250: 7468 6520 7068 6f6e 6574 6963 2066 696c  the phonetic fil
-0001b260: 6573 2e0a 0a20 2020 2020 2020 2050 6172  es...        Par
-0001b270: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
-0001b280: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-0001b290: 2020 204e 6f6e 650a 0a20 2020 2020 2020     None..       
-0001b2a0: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
-0001b2b0: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
-0001b2c0: 204e 6f6e 650a 2020 2020 2020 2020 2222   None.        ""
-0001b2d0: 220a 0a20 2020 2020 2020 2069 6620 7365  "..        if se
-0001b2e0: 6c66 2e6f 706f 6e5f 6469 616c 6f67 2e4e  lf.opon_dialog.N
-0001b2f0: 6577 4f70 6572 6174 6f72 2e74 6578 7428  ewOperator.text(
-0001b300: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-0001b310: 656c 662e 6375 7272 656e 745f 6f70 203d  elf.current_op =
-0001b320: 2073 656c 662e 6f70 6f6e 5f64 6961 6c6f   self.opon_dialo
-0001b330: 672e 4e65 774f 7065 7261 746f 722e 7465  g.NewOperator.te
-0001b340: 7874 2829 2e75 7070 6572 2829 0a20 2020  xt().upper().   
-0001b350: 2020 2020 2073 656c 662e 6f70 6f6e 5f64       self.opon_d
-0001b360: 6961 6c6f 672e 636c 6f73 6528 290a 2020  ialog.close().  
-0001b370: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-0001b380: 7567 2822 4e65 7720 4f70 3a20 2573 222c  ug("New Op: %s",
-0001b390: 2073 656c 662e 6375 7272 656e 745f 6f70   self.current_op
-0001b3a0: 290a 2020 2020 2020 2020 7365 6c66 2e6d  ).        self.m
-0001b3b0: 616b 655f 6f70 5f64 6972 2829 0a0a 2020  ake_op_dir()..  
-0001b3c0: 2020 6465 6620 6d61 6b65 5f6f 705f 6469    def make_op_di
-0001b3d0: 7228 7365 6c66 2920 2d3e 204e 6f6e 653a  r(self) -> None:
-0001b3e0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0001b3f0: 2020 2020 2043 7265 6174 6520 4f50 2064       Create OP d
-0001b400: 6972 6563 746f 7279 2069 6620 6974 2064  irectory if it d
-0001b410: 6f65 7320 6e6f 7420 6578 6973 742e 0a20  oes not exist.. 
-0001b420: 2020 2020 2020 2043 6f70 7920 7468 6520         Copy the 
-0001b430: 7068 6f6e 6574 6963 2066 696c 6573 2074  phonetic files t
-0001b440: 6f20 7468 6520 6e65 7720 6469 7265 6374  o the new direct
-0001b450: 6f72 792e 0a0a 2020 2020 2020 2020 5061  ory...        Pa
-0001b460: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
-0001b470: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-0001b480: 2020 2020 4e6f 6e65 0a0a 2020 2020 2020      None..      
-0001b490: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
-0001b4a0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
-0001b4b0: 2020 4e6f 6e65 0a20 2020 2020 2020 2022    None.        "
-0001b4c0: 2222 0a0a 2020 2020 2020 2020 6966 2073  ""..        if s
-0001b4d0: 656c 662e 6375 7272 656e 745f 6f70 3a0a  elf.current_op:.
-0001b4e0: 2020 2020 2020 2020 2020 2020 6f70 5f70              op_p
-0001b4f0: 6174 6820 3d20 6673 7574 696c 732e 5553  ath = fsutils.US
-0001b500: 4552 5f44 4154 415f 5041 5448 202f 2073  ER_DATA_PATH / s
-0001b510: 656c 662e 6375 7272 656e 745f 6f70 0a20  elf.current_op. 
-0001b520: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-0001b530: 722e 6465 6275 6728 226f 705f 7061 7468  r.debug("op_path
-0001b540: 3a20 2573 222c 2073 7472 286f 705f 7061  : %s", str(op_pa
-0001b550: 7468 2929 0a20 2020 2020 2020 2020 2020  th)).           
-0001b560: 2069 6620 6f70 5f70 6174 682e 6973 5f64   if op_path.is_d
-0001b570: 6972 2829 2069 7320 4661 6c73 653a 0a20  ir() is False:. 
-0001b580: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-0001b590: 6f67 6765 722e 6465 6275 6728 2243 7265  ogger.debug("Cre
-0001b5a0: 6174 696e 6720 4f70 2044 6972 6563 746f  ating Op Directo
-0001b5b0: 7279 3a20 2573 222c 2073 7472 286f 705f  ry: %s", str(op_
-0001b5c0: 7061 7468 2929 0a20 2020 2020 2020 2020  path)).         
-0001b5d0: 2020 2020 2020 206f 732e 6d6b 6469 7228         os.mkdir(
-0001b5e0: 7374 7228 6f70 5f70 6174 6829 290a 2020  str(op_path)).  
-0001b5f0: 2020 2020 2020 2020 2020 6966 206f 705f            if op_
-0001b600: 7061 7468 2e69 735f 6469 7228 293a 0a20  path.is_dir():. 
-0001b610: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0001b620: 6f75 7263 655f 7061 7468 203d 2066 7375  ource_path = fsu
-0001b630: 7469 6c73 2e41 5050 5f44 4154 415f 5041  tils.APP_DATA_PA
-0001b640: 5448 202f 2022 7068 6f6e 6574 6963 7322  TH / "phonetics"
-0001b650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b660: 206c 6f67 6765 722e 6465 6275 6728 2273   logger.debug("s
-0001b670: 6f75 7263 655f 7061 7468 3a20 2573 222c  ource_path: %s",
-0001b680: 2073 7472 2873 6f75 7263 655f 7061 7468   str(source_path
-0001b690: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-0001b6a0: 2020 2066 6f72 2063 6869 6c64 2069 6e20     for child in 
-0001b6b0: 736f 7572 6365 5f70 6174 682e 6974 6572  source_path.iter
-0001b6c0: 6469 7228 293a 0a20 2020 2020 2020 2020  dir():.         
-0001b6d0: 2020 2020 2020 2020 2020 2064 6573 7469             desti
-0001b6e0: 6e61 7469 6f6e 5f66 696c 6520 3d20 6f70  nation_file = op
-0001b6f0: 5f70 6174 6820 2f20 6368 696c 642e 6e61  _path / child.na
-0001b700: 6d65 0a20 2020 2020 2020 2020 2020 2020  me.             
-0001b710: 2020 2020 2020 2069 6620 6465 7374 696e         if destin
-0001b720: 6174 696f 6e5f 6669 6c65 2e69 735f 6669  ation_file.is_fi
-0001b730: 6c65 2829 2069 7320 4661 6c73 653a 0a20  le() is False:. 
-0001b740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b750: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-0001b760: 6275 6728 2244 6573 7469 6e61 7469 6f6e  bug("Destination
-0001b770: 3a20 2573 222c 2073 7472 2864 6573 7469  : %s", str(desti
-0001b780: 6e61 7469 6f6e 5f66 696c 6529 290a 2020  nation_file)).  
-0001b790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b7a0: 2020 2020 2020 6465 7374 696e 6174 696f        destinatio
-0001b7b0: 6e5f 6669 6c65 2e77 7269 7465 5f62 7974  n_file.write_byt
-0001b7c0: 6573 2863 6869 6c64 2e72 6561 645f 6279  es(child.read_by
-0001b7d0: 7465 7328 2929 0a0a 2020 2020 6465 6620  tes())..    def 
-0001b7e0: 706f 6c6c 5f72 6164 696f 2873 656c 6629  poll_radio(self)
-0001b7f0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-0001b800: 2020 2222 220a 2020 2020 2020 2020 506f    """.        Po
-0001b810: 6c6c 2072 6164 696f 2066 6f72 2056 464f  ll radio for VFO
-0001b820: 2c20 6d6f 6465 2c20 6261 6e64 7769 6474  , mode, bandwidt
-0001b830: 682e 0a20 2020 2020 2020 2053 656e 6420  h..        Send 
-0001b840: 7374 6174 6520 7669 6120 6d75 6c74 6963  state via multic
-0001b850: 6173 742e 0a0a 2020 2020 2020 2020 5061  ast...        Pa
-0001b860: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
-0001b870: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-0001b880: 2020 2020 4e6f 6e65 0a0a 2020 2020 2020      None..      
-0001b890: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
-0001b8a0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
-0001b8b0: 2020 4e6f 6e65 0a20 2020 2020 2020 2022    None.        "
-0001b8c0: 2222 0a0a 2020 2020 2020 2020 7365 6c66  ""..        self
-0001b8d0: 2e73 6574 5f72 6164 696f 5f69 636f 6e28  .set_radio_icon(
-0001b8e0: 3029 0a20 2020 2020 2020 2069 6620 7365  0).        if se
-0001b8f0: 6c66 2e72 6967 5f63 6f6e 7472 6f6c 3a0a  lf.rig_control:.
-0001b900: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0001b910: 656c 662e 7269 675f 636f 6e74 726f 6c2e  elf.rig_control.
-0001b920: 6f6e 6c69 6e65 2069 7320 4661 6c73 653a  online is False:
-0001b930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b940: 2073 656c 662e 7365 745f 7261 6469 6f5f   self.set_radio_
-0001b950: 6963 6f6e 2831 290a 2020 2020 2020 2020  icon(1).        
-0001b960: 2020 2020 2020 2020 7365 6c66 2e72 6967          self.rig
-0001b970: 5f63 6f6e 7472 6f6c 2e72 6569 6e69 7428  _control.reinit(
-0001b980: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-0001b990: 2073 656c 662e 7269 675f 636f 6e74 726f   self.rig_contro
-0001b9a0: 6c2e 6f6e 6c69 6e65 3a0a 2020 2020 2020  l.online:.      
-0001b9b0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-0001b9c0: 6574 5f72 6164 696f 5f69 636f 6e28 3229  et_radio_icon(2)
-0001b9d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b9e0: 2069 6e66 6f5f 6469 7274 7920 3d20 4661   info_dirty = Fa
-0001b9f0: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
-0001ba00: 2020 2020 7666 6f20 3d20 7365 6c66 2e72      vfo = self.r
-0001ba10: 6967 5f63 6f6e 7472 6f6c 2e67 6574 5f76  ig_control.get_v
-0001ba20: 666f 2829 0a20 2020 2020 2020 2020 2020  fo().           
-0001ba30: 2020 2020 206d 6f64 6520 3d20 7365 6c66       mode = self
+0001a6d0: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+0001a6e0: 696f 6e2e 6765 7428 2247 7269 6453 7175  ion.get("GridSqu
+0001a6f0: 6172 6522 2c20 2222 292c 2074 6865 6972  are", ""), their
+0001a700: 6772 6964 0a20 2020 2020 2020 2020 2020  grid.           
+0001a710: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+0001a720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a730: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
+0001a740: 696e 675f 6469 7374 616e 6365 2e73 6574  ing_distance.set
+0001a750: 5465 7874 280a 2020 2020 2020 2020 2020  Text(.          
+0001a760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a770: 2020 6622 7b74 6865 6972 6772 6964 7d20    f"{theirgrid} 
+0001a780: 4864 6720 7b68 6561 6469 6e67 7dc2 b020  Hdg {heading}.. 
+0001a790: 4c50 207b 7265 6369 7072 6f63 6f6c 2868  LP {reciprocol(h
+0001a7a0: 6561 6469 6e67 297d c2b0 202f 2022 0a20  eading)}.. / ". 
+0001a7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a7c0: 2020 2020 2020 2020 2020 2066 2264 6973             f"dis
+0001a7d0: 7461 6e63 6520 7b69 6e74 286b 696c 6f6d  tance {int(kilom
+0001a7e0: 6574 6572 732a 302e 3632 3133 3731 297d  eters*0.621371)}
+0001a7f0: 6d69 207b 6b69 6c6f 6d65 7465 7273 7d6b  mi {kilometers}k
+0001a800: 6d22 0a20 2020 2020 2020 2020 2020 2020  m".             
+0001a810: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+0001a820: 2020 6465 6620 6368 6563 6b5f 6475 7065    def check_dupe
+0001a830: 2873 656c 662c 2063 616c 6c3a 2073 7472  (self, call: str
+0001a840: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
+0001a850: 2020 2022 2222 4368 6563 6b73 2069 6620     """Checks if 
+0001a860: 6120 6361 6c6c 7369 676e 2069 7320 6120  a callsign is a 
+0001a870: 6475 7065 206f 6e20 6375 7272 656e 7420  dupe on current 
+0001a880: 6261 6e64 2f6d 6f64 652e 2222 220a 2020  band/mode.""".  
+0001a890: 2020 2020 2020 6966 2073 656c 662e 636f        if self.co
+0001a8a0: 6e74 6573 7420 6973 204e 6f6e 653a 0a20  ntest is None:. 
+0001a8b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0001a8c0: 7368 6f77 5f6d 6573 7361 6765 5f62 6f78  show_message_box
+0001a8d0: 2822 596f 7520 6861 7665 206e 6f20 636f  ("You have no co
+0001a8e0: 6e74 6573 7420 6c6f 6164 6564 2e22 290a  ntest loaded.").
+0001a8f0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0001a900: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
+0001a910: 2073 656c 662e 636f 6e74 6573 742e 7072   self.contest.pr
+0001a920: 6564 7570 6528 7365 6c66 290a 2020 2020  edupe(self).    
+0001a930: 2020 2020 6261 6e64 203d 2066 6c6f 6174      band = float
+0001a940: 2867 6574 5f6c 6f67 6765 645f 6261 6e64  (get_logged_band
+0001a950: 2873 7472 2873 656c 662e 7261 6469 6f5f  (str(self.radio_
+0001a960: 7374 6174 652e 6765 7428 2276 666f 6122  state.get("vfoa"
+0001a970: 2c20 302e 3029 2929 290a 2020 2020 2020  , 0.0)))).      
+0001a980: 2020 6d6f 6465 203d 2073 656c 662e 7261    mode = self.ra
+0001a990: 6469 6f5f 7374 6174 652e 6765 7428 226d  dio_state.get("m
+0001a9a0: 6f64 6522 2c20 2222 290a 2020 2020 2020  ode", "").      
+0001a9b0: 2020 6465 6275 676c 696e 6520 3d20 280a    debugline = (.
+0001a9c0: 2020 2020 2020 2020 2020 2020 6622 4361              f"Ca
+0001a9d0: 6c6c 3a20 7b63 616c 6c7d 2042 616e 643a  ll: {call} Band:
+0001a9e0: 207b 6261 6e64 7d20 4d6f 6465 3a20 7b6d   {band} Mode: {m
+0001a9f0: 6f64 657d 2044 7570 6574 7970 653a 207b  ode} Dupetype: {
+0001aa00: 7365 6c66 2e63 6f6e 7465 7374 2e64 7570  self.contest.dup
+0001aa10: 655f 7479 7065 7d22 0a20 2020 2020 2020  e_type}".       
+0001aa20: 2029 0a20 2020 2020 2020 206c 6f67 6765   ).        logge
+0001aa30: 722e 6465 6275 6728 2225 7322 2c20 6465  r.debug("%s", de
+0001aa40: 6275 676c 696e 6529 0a20 2020 2020 2020  bugline).       
+0001aa50: 2069 6620 7365 6c66 2e63 6f6e 7465 7374   if self.contest
+0001aa60: 2e64 7570 655f 7479 7065 203d 3d20 313a  .dupe_type == 1:
+0001aa70: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+0001aa80: 756c 7420 3d20 7365 6c66 2e64 6174 6162  ult = self.datab
+0001aa90: 6173 652e 6368 6563 6b5f 6475 7065 2863  ase.check_dupe(c
+0001aaa0: 616c 6c29 0a20 2020 2020 2020 2069 6620  all).        if 
+0001aab0: 7365 6c66 2e63 6f6e 7465 7374 2e64 7570  self.contest.dup
+0001aac0: 655f 7479 7065 203d 3d20 323a 0a20 2020  e_type == 2:.   
+0001aad0: 2020 2020 2020 2020 2072 6573 756c 7420           result 
+0001aae0: 3d20 7365 6c66 2e64 6174 6162 6173 652e  = self.database.
+0001aaf0: 6368 6563 6b5f 6475 7065 5f6f 6e5f 6261  check_dupe_on_ba
+0001ab00: 6e64 2863 616c 6c2c 2062 616e 6429 0a20  nd(call, band). 
+0001ab10: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+0001ab20: 6f6e 7465 7374 2e64 7570 655f 7479 7065  ontest.dupe_type
+0001ab30: 203d 3d20 333a 0a20 2020 2020 2020 2020   == 3:.         
+0001ab40: 2020 2072 6573 756c 7420 3d20 7365 6c66     result = self
+0001ab50: 2e64 6174 6162 6173 652e 6368 6563 6b5f  .database.check_
+0001ab60: 6475 7065 5f6f 6e5f 6261 6e64 5f6d 6f64  dupe_on_band_mod
+0001ab70: 6528 6361 6c6c 2c20 6261 6e64 2c20 6d6f  e(call, band, mo
+0001ab80: 6465 290a 2020 2020 2020 2020 6966 2073  de).        if s
+0001ab90: 656c 662e 636f 6e74 6573 742e 6475 7065  elf.contest.dupe
+0001aba0: 5f74 7970 6520 3d3d 2034 3a0a 2020 2020  _type == 4:.    
+0001abb0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+0001abc0: 207b 2269 7364 7570 6522 3a20 4661 6c73   {"isdupe": Fals
+0001abd0: 657d 0a20 2020 2020 2020 2064 6562 7567  e}.        debug
+0001abe0: 6c69 6e65 203d 2066 227b 7265 7375 6c74  line = f"{result
+0001abf0: 7d22 0a20 2020 2020 2020 206c 6f67 6765  }".        logge
+0001ac00: 722e 6465 6275 6728 2225 7322 2c20 6465  r.debug("%s", de
+0001ac10: 6275 676c 696e 6529 0a20 2020 2020 2020  bugline).       
+0001ac20: 2072 6574 7572 6e20 7265 7375 6c74 2e67   return result.g
+0001ac30: 6574 2822 6973 6475 7065 222c 2046 616c  et("isdupe", Fal
+0001ac40: 7365 290a 0a20 2020 2064 6566 2073 6574  se)..    def set
+0001ac50: 6d6f 6465 2873 656c 662c 206d 6f64 653a  mode(self, mode:
+0001ac60: 2073 7472 2920 2d3e 204e 6f6e 653a 0a20   str) -> None:. 
+0001ac70: 2020 2020 2020 2022 2222 4361 6c6c 2077         """Call w
+0001ac80: 6865 6e20 7468 6520 6d6f 6465 2063 6861  hen the mode cha
+0001ac90: 6e67 6573 2e22 2222 0a20 2020 2020 2020  nges.""".       
+0001aca0: 2069 6620 6d6f 6465 203d 3d20 2243 5722   if mode == "CW"
+0001acb0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+0001acc0: 2073 656c 662e 6375 7272 656e 745f 6d6f   self.current_mo
+0001acd0: 6465 2021 3d20 2243 5722 3a0a 2020 2020  de != "CW":.    
+0001ace0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001acf0: 2e63 7572 7265 6e74 5f6d 6f64 6520 3d20  .current_mode = 
+0001ad00: 2243 5722 0a20 2020 2020 2020 2020 2020  "CW".           
+0001ad10: 2020 2020 2023 2073 656c 662e 6d6f 6465       # self.mode
+0001ad20: 2e73 6574 5465 7874 2822 4357 2229 0a20  .setText("CW"). 
+0001ad30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001ad40: 656c 662e 7365 6e74 2e73 6574 5465 7874  elf.sent.setText
+0001ad50: 2822 3539 3922 290a 2020 2020 2020 2020  ("599").        
+0001ad60: 2020 2020 2020 2020 7365 6c66 2e72 6563          self.rec
+0001ad70: 6569 7665 2e73 6574 5465 7874 2822 3539  eive.setText("59
+0001ad80: 3922 290a 2020 2020 2020 2020 2020 2020  9").            
+0001ad90: 2020 2020 7365 6c66 2e72 6561 645f 6377      self.read_cw
+0001ada0: 5f6d 6163 726f 7328 290a 2020 2020 2020  _macros().      
+0001adb0: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+0001adc0: 2020 2020 2069 6620 6d6f 6465 203d 3d20       if mode == 
+0001add0: 2253 5342 223a 0a20 2020 2020 2020 2020  "SSB":.         
+0001ade0: 2020 2069 6620 7365 6c66 2e63 7572 7265     if self.curre
+0001adf0: 6e74 5f6d 6f64 6520 213d 2022 5353 4222  nt_mode != "SSB"
+0001ae00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001ae10: 2020 7365 6c66 2e63 7572 7265 6e74 5f6d    self.current_m
+0001ae20: 6f64 6520 3d20 2253 5342 220a 2020 2020  ode = "SSB".    
+0001ae30: 2020 2020 2020 2020 2020 2020 2320 7365              # se
+0001ae40: 6c66 2e6d 6f64 652e 7365 7454 6578 7428  lf.mode.setText(
+0001ae50: 2253 5342 2229 0a20 2020 2020 2020 2020  "SSB").         
+0001ae60: 2020 2020 2020 2073 656c 662e 7365 6e74         self.sent
+0001ae70: 2e73 6574 5465 7874 2822 3539 2229 0a20  .setText("59"). 
+0001ae80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001ae90: 656c 662e 7265 6365 6976 652e 7365 7454  elf.receive.setT
+0001aea0: 6578 7428 2235 3922 290a 2020 2020 2020  ext("59").      
+0001aeb0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+0001aec0: 6561 645f 6377 5f6d 6163 726f 7328 290a  ead_cw_macros().
+0001aed0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0001aee0: 726e 0a20 2020 2020 2020 2069 6620 6d6f  rn.        if mo
+0001aef0: 6465 203d 3d20 2252 5454 5922 3a0a 2020  de == "RTTY":.  
+0001af00: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0001af10: 662e 6375 7272 656e 745f 6d6f 6465 2021  f.current_mode !
+0001af20: 3d20 2252 5454 5922 3a0a 2020 2020 2020  = "RTTY":.      
+0001af30: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0001af40: 7572 7265 6e74 5f6d 6f64 6520 3d20 2252  urrent_mode = "R
+0001af50: 5454 5922 0a20 2020 2020 2020 2020 2020  TTY".           
+0001af60: 2020 2020 2023 2073 656c 662e 6d6f 6465       # self.mode
+0001af70: 2e73 6574 5465 7874 2822 5254 5459 2229  .setText("RTTY")
+0001af80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001af90: 2073 656c 662e 7365 6e74 2e73 6574 5465   self.sent.setTe
+0001afa0: 7874 2822 3539 2229 0a20 2020 2020 2020  xt("59").       
+0001afb0: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
+0001afc0: 6365 6976 652e 7365 7454 6578 7428 2235  ceive.setText("5
+0001afd0: 3922 290a 0a20 2020 2064 6566 2067 6574  9")..    def get
+0001afe0: 5f6f 706f 6e28 7365 6c66 2920 2d3e 204e  _opon(self) -> N
+0001aff0: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+0001b000: 0a20 2020 2020 2020 2043 7472 6c2b 4f20  .        Ctrl+O 
+0001b010: 4f70 656e 2074 6865 204f 504f 4e20 6469  Open the OPON di
+0001b020: 616c 6f67 2e0a 0a20 2020 2020 2020 2050  alog...        P
+0001b030: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+0001b040: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+0001b050: 2020 2020 204e 6f6e 650a 0a20 2020 2020       None..     
+0001b060: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
+0001b070: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
+0001b080: 2020 204e 6f6e 650a 2020 2020 2020 2020     None.        
+0001b090: 2222 220a 0a20 2020 2020 2020 2073 656c  """..        sel
+0001b0a0: 662e 6f70 6f6e 5f64 6961 6c6f 6720 3d20  f.opon_dialog = 
+0001b0b0: 4f70 4f6e 2866 7375 7469 6c73 2e41 5050  OpOn(fsutils.APP
+0001b0c0: 5f44 4154 415f 5041 5448 290a 0a20 2020  _DATA_PATH)..   
+0001b0d0: 2020 2020 2069 6620 7365 6c66 2e63 7572       if self.cur
+0001b0e0: 7265 6e74 5f70 616c 6574 7465 3a0a 2020  rent_palette:.  
+0001b0f0: 2020 2020 2020 2020 2020 7365 6c66 2e6f            self.o
+0001b100: 706f 6e5f 6469 616c 6f67 2e73 6574 5061  pon_dialog.setPa
+0001b110: 6c65 7474 6528 7365 6c66 2e63 7572 7265  lette(self.curre
+0001b120: 6e74 5f70 616c 6574 7465 290a 0a20 2020  nt_palette)..   
+0001b130: 2020 2020 2073 656c 662e 6f70 6f6e 5f64       self.opon_d
+0001b140: 6961 6c6f 672e 6163 6365 7074 6564 2e63  ialog.accepted.c
+0001b150: 6f6e 6e65 6374 2873 656c 662e 6e65 775f  onnect(self.new_
+0001b160: 6f70 290a 2020 2020 2020 2020 7365 6c66  op).        self
+0001b170: 2e6f 706f 6e5f 6469 616c 6f67 2e6f 7065  .opon_dialog.ope
+0001b180: 6e28 290a 0a20 2020 2064 6566 206e 6577  n()..    def new
+0001b190: 5f6f 7028 7365 6c66 2920 2d3e 204e 6f6e  _op(self) -> Non
+0001b1a0: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
+0001b1b0: 2020 2020 2020 2043 616c 6c65 6420 7768         Called wh
+0001b1c0: 656e 2074 6865 2075 7365 7220 636c 6963  en the user clic
+0001b1d0: 6b73 2074 6865 204f 4b20 6275 7474 6f6e  ks the OK button
+0001b1e0: 206f 6e20 7468 6520 4f50 4f4e 2064 6961   on the OPON dia
+0001b1f0: 6c6f 672e 0a20 2020 2020 2020 2043 7265  log..        Cre
+0001b200: 6174 6520 7468 6520 6e65 7720 6469 7265  ate the new dire
+0001b210: 6374 6f72 7920 616e 6420 636f 7079 2074  ctory and copy t
+0001b220: 6865 2070 686f 6e65 7469 6320 6669 6c65  he phonetic file
+0001b230: 732e 0a0a 2020 2020 2020 2020 5061 7261  s...        Para
+0001b240: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
+0001b250: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+0001b260: 2020 4e6f 6e65 0a0a 2020 2020 2020 2020    None..        
+0001b270: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
+0001b280: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+0001b290: 4e6f 6e65 0a20 2020 2020 2020 2022 2222  None.        """
+0001b2a0: 0a0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
+0001b2b0: 662e 6f70 6f6e 5f64 6961 6c6f 672e 4e65  f.opon_dialog.Ne
+0001b2c0: 774f 7065 7261 746f 722e 7465 7874 2829  wOperator.text()
+0001b2d0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0001b2e0: 6c66 2e63 7572 7265 6e74 5f6f 7020 3d20  lf.current_op = 
+0001b2f0: 7365 6c66 2e6f 706f 6e5f 6469 616c 6f67  self.opon_dialog
+0001b300: 2e4e 6577 4f70 6572 6174 6f72 2e74 6578  .NewOperator.tex
+0001b310: 7428 292e 7570 7065 7228 290a 2020 2020  t().upper().    
+0001b320: 2020 2020 7365 6c66 2e6f 706f 6e5f 6469      self.opon_di
+0001b330: 616c 6f67 2e63 6c6f 7365 2829 0a20 2020  alog.close().   
+0001b340: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+0001b350: 6728 224e 6577 204f 703a 2025 7322 2c20  g("New Op: %s", 
+0001b360: 7365 6c66 2e63 7572 7265 6e74 5f6f 7029  self.current_op)
+0001b370: 0a20 2020 2020 2020 2073 656c 662e 6d61  .        self.ma
+0001b380: 6b65 5f6f 705f 6469 7228 290a 0a20 2020  ke_op_dir()..   
+0001b390: 2064 6566 206d 616b 655f 6f70 5f64 6972   def make_op_dir
+0001b3a0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
+0001b3b0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0001b3c0: 2020 2020 4372 6561 7465 204f 5020 6469      Create OP di
+0001b3d0: 7265 6374 6f72 7920 6966 2069 7420 646f  rectory if it do
+0001b3e0: 6573 206e 6f74 2065 7869 7374 2e0a 2020  es not exist..  
+0001b3f0: 2020 2020 2020 436f 7079 2074 6865 2070        Copy the p
+0001b400: 686f 6e65 7469 6320 6669 6c65 7320 746f  honetic files to
+0001b410: 2074 6865 206e 6577 2064 6972 6563 746f   the new directo
+0001b420: 7279 2e0a 0a20 2020 2020 2020 2050 6172  ry...        Par
+0001b430: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
+0001b440: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+0001b450: 2020 204e 6f6e 650a 0a20 2020 2020 2020     None..       
+0001b460: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
+0001b470: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
+0001b480: 204e 6f6e 650a 2020 2020 2020 2020 2222   None.        ""
+0001b490: 220a 0a20 2020 2020 2020 2069 6620 7365  "..        if se
+0001b4a0: 6c66 2e63 7572 7265 6e74 5f6f 703a 0a20  lf.current_op:. 
+0001b4b0: 2020 2020 2020 2020 2020 206f 705f 7061             op_pa
+0001b4c0: 7468 203d 2066 7375 7469 6c73 2e55 5345  th = fsutils.USE
+0001b4d0: 525f 4441 5441 5f50 4154 4820 2f20 7365  R_DATA_PATH / se
+0001b4e0: 6c66 2e63 7572 7265 6e74 5f6f 700a 2020  lf.current_op.  
+0001b4f0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+0001b500: 2e64 6562 7567 2822 6f70 5f70 6174 683a  .debug("op_path:
+0001b510: 2025 7322 2c20 7374 7228 6f70 5f70 6174   %s", str(op_pat
+0001b520: 6829 290a 2020 2020 2020 2020 2020 2020  h)).            
+0001b530: 6966 206f 705f 7061 7468 2e69 735f 6469  if op_path.is_di
+0001b540: 7228 2920 6973 2046 616c 7365 3a0a 2020  r() is False:.  
+0001b550: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+0001b560: 6767 6572 2e64 6562 7567 2822 4372 6561  gger.debug("Crea
+0001b570: 7469 6e67 204f 7020 4469 7265 6374 6f72  ting Op Director
+0001b580: 793a 2025 7322 2c20 7374 7228 6f70 5f70  y: %s", str(op_p
+0001b590: 6174 6829 290a 2020 2020 2020 2020 2020  ath)).          
+0001b5a0: 2020 2020 2020 6f73 2e6d 6b64 6972 2873        os.mkdir(s
+0001b5b0: 7472 286f 705f 7061 7468 2929 0a20 2020  tr(op_path)).   
+0001b5c0: 2020 2020 2020 2020 2069 6620 6f70 5f70           if op_p
+0001b5d0: 6174 682e 6973 5f64 6972 2829 3a0a 2020  ath.is_dir():.  
+0001b5e0: 2020 2020 2020 2020 2020 2020 2020 736f                so
+0001b5f0: 7572 6365 5f70 6174 6820 3d20 6673 7574  urce_path = fsut
+0001b600: 696c 732e 4150 505f 4441 5441 5f50 4154  ils.APP_DATA_PAT
+0001b610: 4820 2f20 2270 686f 6e65 7469 6373 220a  H / "phonetics".
+0001b620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b630: 6c6f 6767 6572 2e64 6562 7567 2822 736f  logger.debug("so
+0001b640: 7572 6365 5f70 6174 683a 2025 7322 2c20  urce_path: %s", 
+0001b650: 7374 7228 736f 7572 6365 5f70 6174 6829  str(source_path)
+0001b660: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001b670: 2020 666f 7220 6368 696c 6420 696e 2073    for child in s
+0001b680: 6f75 7263 655f 7061 7468 2e69 7465 7264  ource_path.iterd
+0001b690: 6972 2829 3a0a 2020 2020 2020 2020 2020  ir():.          
+0001b6a0: 2020 2020 2020 2020 2020 6465 7374 696e            destin
+0001b6b0: 6174 696f 6e5f 6669 6c65 203d 206f 705f  ation_file = op_
+0001b6c0: 7061 7468 202f 2063 6869 6c64 2e6e 616d  path / child.nam
+0001b6d0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0001b6e0: 2020 2020 2020 6966 2064 6573 7469 6e61        if destina
+0001b6f0: 7469 6f6e 5f66 696c 652e 6973 5f66 696c  tion_file.is_fil
+0001b700: 6528 2920 6973 2046 616c 7365 3a0a 2020  e() is False:.  
+0001b710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b720: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+0001b730: 7567 2822 4465 7374 696e 6174 696f 6e3a  ug("Destination:
+0001b740: 2025 7322 2c20 7374 7228 6465 7374 696e   %s", str(destin
+0001b750: 6174 696f 6e5f 6669 6c65 2929 0a20 2020  ation_file)).   
+0001b760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b770: 2020 2020 2064 6573 7469 6e61 7469 6f6e       destination
+0001b780: 5f66 696c 652e 7772 6974 655f 6279 7465  _file.write_byte
+0001b790: 7328 6368 696c 642e 7265 6164 5f62 7974  s(child.read_byt
+0001b7a0: 6573 2829 290a 0a20 2020 2064 6566 2070  es())..    def p
+0001b7b0: 6f6c 6c5f 7261 6469 6f28 7365 6c66 2920  oll_radio(self) 
+0001b7c0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+0001b7d0: 2022 2222 0a20 2020 2020 2020 2050 6f6c   """.        Pol
+0001b7e0: 6c20 7261 6469 6f20 666f 7220 5646 4f2c  l radio for VFO,
+0001b7f0: 206d 6f64 652c 2062 616e 6477 6964 7468   mode, bandwidth
+0001b800: 2e0a 2020 2020 2020 2020 5365 6e64 2073  ..        Send s
+0001b810: 7461 7465 2076 6961 206d 756c 7469 6361  tate via multica
+0001b820: 7374 2e0a 0a20 2020 2020 2020 2050 6172  st...        Par
+0001b830: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
+0001b840: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+0001b850: 2020 204e 6f6e 650a 0a20 2020 2020 2020     None..       
+0001b860: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
+0001b870: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
+0001b880: 204e 6f6e 650a 2020 2020 2020 2020 2222   None.        ""
+0001b890: 220a 0a20 2020 2020 2020 2073 656c 662e  "..        self.
+0001b8a0: 7365 745f 7261 6469 6f5f 6963 6f6e 2830  set_radio_icon(0
+0001b8b0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+0001b8c0: 662e 7269 675f 636f 6e74 726f 6c3a 0a20  f.rig_control:. 
+0001b8d0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0001b8e0: 6c66 2e72 6967 5f63 6f6e 7472 6f6c 2e6f  lf.rig_control.o
+0001b8f0: 6e6c 696e 6520 6973 2046 616c 7365 3a0a  nline is False:.
+0001b900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b910: 7365 6c66 2e73 6574 5f72 6164 696f 5f69  self.set_radio_i
+0001b920: 636f 6e28 3129 0a20 2020 2020 2020 2020  con(1).         
+0001b930: 2020 2020 2020 2073 656c 662e 7269 675f         self.rig_
+0001b940: 636f 6e74 726f 6c2e 7265 696e 6974 2829  control.reinit()
+0001b950: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0001b960: 7365 6c66 2e72 6967 5f63 6f6e 7472 6f6c  self.rig_control
+0001b970: 2e6f 6e6c 696e 653a 0a20 2020 2020 2020  .online:.       
+0001b980: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+0001b990: 745f 7261 6469 6f5f 6963 6f6e 2832 290a  t_radio_icon(2).
+0001b9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b9b0: 696e 666f 5f64 6972 7479 203d 2046 616c  info_dirty = Fal
+0001b9c0: 7365 0a20 2020 2020 2020 2020 2020 2020  se.             
+0001b9d0: 2020 2076 666f 203d 2073 656c 662e 7269     vfo = self.ri
+0001b9e0: 675f 636f 6e74 726f 6c2e 6765 745f 7666  g_control.get_vf
+0001b9f0: 6f28 290a 2020 2020 2020 2020 2020 2020  o().            
+0001ba00: 2020 2020 6d6f 6465 203d 2073 656c 662e      mode = self.
+0001ba10: 7269 675f 636f 6e74 726f 6c2e 6765 745f  rig_control.get_
+0001ba20: 6d6f 6465 2829 0a20 2020 2020 2020 2020  mode().         
+0001ba30: 2020 2020 2020 2062 7720 3d20 7365 6c66         bw = self
 0001ba40: 2e72 6967 5f63 6f6e 7472 6f6c 2e67 6574  .rig_control.get
-0001ba50: 5f6d 6f64 6528 290a 2020 2020 2020 2020  _mode().        
-0001ba60: 2020 2020 2020 2020 6277 203d 2073 656c          bw = sel
-0001ba70: 662e 7269 675f 636f 6e74 726f 6c2e 6765  f.rig_control.ge
-0001ba80: 745f 6277 2829 0a0a 2020 2020 2020 2020  t_bw()..        
-0001ba90: 2020 2020 2020 2020 6966 206d 6f64 6520          if mode 
-0001baa0: 3d3d 2022 4357 223a 0a20 2020 2020 2020  == "CW":.       
-0001bab0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0001bac0: 662e 7365 746d 6f64 6528 6d6f 6465 290a  f.setmode(mode).
-0001bad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bae0: 6966 206d 6f64 6520 3d3d 2022 4c53 4222  if mode == "LSB"
-0001baf0: 206f 7220 6d6f 6465 203d 3d20 2255 5342   or mode == "USB
-0001bb00: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-0001bb10: 2020 2020 2020 2073 656c 662e 7365 746d         self.setm
-0001bb20: 6f64 6528 2253 5342 2229 0a20 2020 2020  ode("SSB").     
-0001bb30: 2020 2020 2020 2020 2020 2069 6620 6d6f             if mo
-0001bb40: 6465 203d 3d20 2252 5454 5922 3a0a 2020  de == "RTTY":.  
-0001bb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bb60: 2020 7365 6c66 2e73 6574 6d6f 6465 2822    self.setmode("
-0001bb70: 5254 5459 2229 0a0a 2020 2020 2020 2020  RTTY")..        
-0001bb80: 2020 2020 2020 2020 6966 2076 666f 203d          if vfo =
-0001bb90: 3d20 2222 3a0a 2020 2020 2020 2020 2020  = "":.          
-0001bba0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0001bbb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001bbc0: 2069 6620 7365 6c66 2e72 6164 696f 5f73   if self.radio_s
-0001bbd0: 7461 7465 2e67 6574 2822 7666 6f61 2229  tate.get("vfoa")
-0001bbe0: 2021 3d20 7666 6f3a 0a20 2020 2020 2020   != vfo:.       
-0001bbf0: 2020 2020 2020 2020 2020 2020 2069 6e66               inf
-0001bc00: 6f5f 6469 7274 7920 3d20 5472 7565 0a20  o_dirty = True. 
-0001bc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bc20: 2020 2073 656c 662e 7261 6469 6f5f 7374     self.radio_st
-0001bc30: 6174 655b 2276 666f 6122 5d20 3d20 7666  ate["vfoa"] = vf
-0001bc40: 6f0a 2020 2020 2020 2020 2020 2020 2020  o.              
-0001bc50: 2020 6261 6e64 203d 2067 6574 6261 6e64    band = getband
-0001bc60: 2873 7472 2876 666f 2929 0a20 2020 2020  (str(vfo)).     
-0001bc70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001bc80: 7261 6469 6f5f 7374 6174 655b 2262 616e  radio_state["ban
-0001bc90: 6422 5d20 3d20 6261 6e64 0a20 2020 2020  d"] = band.     
-0001bca0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001bcb0: 636f 6e74 6163 745b 2242 616e 6422 5d20  contact["Band"] 
-0001bcc0: 3d20 6765 745f 6c6f 6767 6564 5f62 616e  = get_logged_ban
-0001bcd0: 6428 7374 7228 7666 6f29 290a 2020 2020  d(str(vfo)).    
-0001bce0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001bcf0: 2e73 6574 5f62 616e 645f 696e 6469 6361  .set_band_indica
-0001bd00: 746f 7228 6261 6e64 290a 0a20 2020 2020  tor(band)..     
-0001bd10: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0001bd20: 6c66 2e72 6164 696f 5f73 7461 7465 2e67  lf.radio_state.g
-0001bd30: 6574 2822 6d6f 6465 2229 2021 3d20 6d6f  et("mode") != mo
-0001bd40: 6465 3a0a 2020 2020 2020 2020 2020 2020  de:.            
-0001bd50: 2020 2020 2020 2020 696e 666f 5f64 6972          info_dir
-0001bd60: 7479 203d 2054 7275 650a 2020 2020 2020  ty = True.      
-0001bd70: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0001bd80: 6c66 2e72 6164 696f 5f73 7461 7465 5b22  lf.radio_state["
-0001bd90: 6d6f 6465 225d 203d 206d 6f64 650a 0a20  mode"] = mode.. 
-0001bda0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0001bdb0: 6620 7365 6c66 2e72 6164 696f 5f73 7461  f self.radio_sta
-0001bdc0: 7465 2e67 6574 2822 6277 2229 2021 3d20  te.get("bw") != 
-0001bdd0: 6277 3a0a 2020 2020 2020 2020 2020 2020  bw:.            
-0001bde0: 2020 2020 2020 2020 696e 666f 5f64 6972          info_dir
-0001bdf0: 7479 203d 2054 7275 650a 2020 2020 2020  ty = True.      
-0001be00: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0001be10: 6c66 2e72 6164 696f 5f73 7461 7465 5b22  lf.radio_state["
-0001be20: 6277 225d 203d 2062 770a 0a20 2020 2020  bw"] = bw..     
-0001be30: 2020 2020 2020 2020 2020 2069 6620 6461             if da
-0001be40: 7465 7469 6d65 2e64 6174 6574 696d 652e  tetime.datetime.
-0001be50: 6e6f 7728 2920 3e20 676c 6f62 616c 7328  now() > globals(
-0001be60: 295b 2270 6f6c 6c5f 7469 6d65 225d 206f  )["poll_time"] o
-0001be70: 7220 696e 666f 5f64 6972 7479 3a0a 2020  r info_dirty:.  
-0001be80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001be90: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
-0001bea0: 5646 4f3a 2025 7320 204d 4f44 453a 2025  VFO: %s  MODE: %
-0001beb0: 7320 4257 3a20 2573 222c 2076 666f 2c20  s BW: %s", vfo, 
-0001bec0: 6d6f 6465 2c20 6277 290a 2020 2020 2020  mode, bw).      
-0001bed0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0001bee0: 6c66 2e73 6574 5f77 696e 646f 775f 7469  lf.set_window_ti
-0001bef0: 746c 6528 290a 2020 2020 2020 2020 2020  tle().          
-0001bf00: 2020 2020 2020 2020 2020 636d 6420 3d20            cmd = 
-0001bf10: 7b7d 0a20 2020 2020 2020 2020 2020 2020  {}.             
-0001bf20: 2020 2020 2020 2063 6d64 5b22 636d 6422         cmd["cmd"
-0001bf30: 5d20 3d20 2252 4144 494f 5f53 5441 5445  ] = "RADIO_STATE
-0001bf40: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0001bf50: 2020 2020 2020 636d 645b 2273 7461 7469        cmd["stati
-0001bf60: 6f6e 225d 203d 2070 6c61 7466 6f72 6d2e  on"] = platform.
-0001bf70: 6e6f 6465 2829 0a20 2020 2020 2020 2020  node().         
-0001bf80: 2020 2020 2020 2020 2020 2063 6d64 5b22             cmd["
-0001bf90: 6261 6e64 225d 203d 2062 616e 640a 2020  band"] = band.  
-0001bfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bfb0: 2020 636d 645b 2276 666f 6122 5d20 3d20    cmd["vfoa"] = 
-0001bfc0: 7666 6f0a 2020 2020 2020 2020 2020 2020  vfo.            
-0001bfd0: 2020 2020 2020 2020 636d 645b 226d 6f64          cmd["mod
-0001bfe0: 6522 5d20 3d20 6d6f 6465 0a20 2020 2020  e"] = mode.     
-0001bff0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0001c000: 6d64 5b22 6277 225d 203d 2062 770a 2020  md["bw"] = bw.  
-0001c010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c020: 2020 7365 6c66 2e6d 756c 7469 6361 7374    self.multicast
-0001c030: 5f69 6e74 6572 6661 6365 2e73 656e 645f  _interface.send_
-0001c040: 6173 5f6a 736f 6e28 636d 6429 0a20 2020  as_json(cmd).   
-0001c050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c060: 2069 6620 7365 6c66 2e6e 316d 6d3a 0a20   if self.n1mm:. 
-0001c070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c080: 2020 2020 2020 2069 6620 7365 6c66 2e6e         if self.n
-0001c090: 316d 6d2e 7365 6e64 5f72 6164 696f 5f70  1mm.send_radio_p
-0001c0a0: 6163 6b65 7473 3a0a 2020 2020 2020 2020  ackets:.        
-0001c0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c0c0: 2020 2020 7365 6c66 2e6e 316d 6d2e 7261      self.n1mm.ra
-0001c0d0: 6469 6f5f 696e 666f 5b22 4672 6571 225d  dio_info["Freq"]
-0001c0e0: 203d 2076 666f 5b3a 2d31 5d0a 2020 2020   = vfo[:-1].    
-0001c0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c100: 2020 2020 2020 2020 7365 6c66 2e6e 316d          self.n1m
-0001c110: 6d2e 7261 6469 6f5f 696e 666f 5b22 5458  m.radio_info["TX
-0001c120: 4672 6571 225d 203d 2076 666f 5b3a 2d31  Freq"] = vfo[:-1
-0001c130: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0001c140: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0001c150: 6c66 2e6e 316d 6d2e 7261 6469 6f5f 696e  lf.n1mm.radio_in
-0001c160: 666f 5b22 4d6f 6465 225d 203d 206d 6f64  fo["Mode"] = mod
-0001c170: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-0001c180: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0001c190: 6c66 2e6e 316d 6d2e 7261 6469 6f5f 696e  lf.n1mm.radio_in
-0001c1a0: 666f 5b22 4f70 4361 6c6c 225d 203d 2073  fo["OpCall"] = s
-0001c1b0: 656c 662e 6375 7272 656e 745f 6f70 0a20  elf.current_op. 
-0001c1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c1d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001c1e0: 6e31 6d6d 2e72 6164 696f 5f69 6e66 6f5b  n1mm.radio_info[
-0001c1f0: 2249 7352 756e 6e69 6e67 225d 203d 2073  "IsRunning"] = s
-0001c200: 7472 280a 2020 2020 2020 2020 2020 2020  tr(.            
-0001c210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c220: 2020 2020 7365 6c66 2e70 7265 662e 6765      self.pref.ge
-0001c230: 7428 2272 756e 5f73 7461 7465 222c 2046  t("run_state", F
-0001c240: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
-0001c250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c260: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-0001c270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c280: 7365 6c66 2e6e 316d 6d2e 7365 6e64 5f72  self.n1mm.send_r
-0001c290: 6164 696f 2829 0a20 2020 2020 2020 2020  adio().         
-0001c2a0: 2020 2020 2020 2020 2020 2067 6c6f 6261             globa
-0001c2b0: 6c73 2829 5b0a 2020 2020 2020 2020 2020  ls()[.          
-0001c2c0: 2020 2020 2020 2020 2020 2020 2020 2270                "p
-0001c2d0: 6f6c 6c5f 7469 6d65 220a 2020 2020 2020  oll_time".      
-0001c2e0: 2020 2020 2020 2020 2020 2020 2020 5d20                ] 
-0001c2f0: 3d20 6461 7465 7469 6d65 2e64 6174 6574  = datetime.datet
-0001c300: 696d 652e 6e6f 7728 2920 2b20 6461 7465  ime.now() + date
-0001c310: 7469 6d65 2e74 696d 6564 656c 7461 2873  time.timedelta(s
-0001c320: 6563 6f6e 6473 3d31 3029 0a0a 2020 2020  econds=10)..    
-0001c330: 6465 6620 6564 6974 5f63 775f 6d61 6372  def edit_cw_macr
-0001c340: 6f73 2873 656c 6629 202d 3e20 4e6f 6e65  os(self) -> None
-0001c350: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-0001c360: 2020 2020 2020 4361 6c6c 7320 7468 6520        Calls the 
-0001c370: 6465 6661 756c 7420 7465 7874 2065 6469  default text edi
-0001c380: 746f 7220 746f 2065 6469 7420 7468 6520  tor to edit the 
-0001c390: 4357 206d 6163 726f 2066 696c 652e 0a0a  CW macro file...
-0001c3a0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-0001c3b0: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
-0001c3c0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 4e6f  -----.        No
-0001c3d0: 6e65 0a0a 2020 2020 2020 2020 5265 7475  ne..        Retu
-0001c3e0: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
-0001c3f0: 2d2d 2d0a 2020 2020 2020 2020 4e6f 6e65  ---.        None
-0001c400: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0001c410: 2020 2020 2069 6620 7365 6c66 2e72 6164       if self.rad
-0001c420: 696f 5f73 7461 7465 2e67 6574 2822 6d6f  io_state.get("mo
-0001c430: 6465 2229 203d 3d20 2243 5722 3a0a 2020  de") == "CW":.  
-0001c440: 2020 2020 2020 2020 2020 6d61 6372 6f5f            macro_
-0001c450: 6669 6c65 203d 2022 6377 6d61 6372 6f73  file = "cwmacros
-0001c460: 2e74 7874 220a 2020 2020 2020 2020 656c  .txt".        el
-0001c470: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0001c480: 6d61 6372 6f5f 6669 6c65 203d 2022 7373  macro_file = "ss
-0001c490: 626d 6163 726f 732e 7478 7422 0a20 2020  bmacros.txt".   
-0001c4a0: 2020 2020 2069 6620 6e6f 7420 2866 7375       if not (fsu
-0001c4b0: 7469 6c73 2e55 5345 525f 4441 5441 5f50  tils.USER_DATA_P
-0001c4c0: 4154 4820 2f20 6d61 6372 6f5f 6669 6c65  ATH / macro_file
-0001c4d0: 292e 6578 6973 7473 2829 3a0a 2020 2020  ).exists():.    
-0001c4e0: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-0001c4f0: 6562 7567 2822 7265 6164 5f63 775f 6d61  ebug("read_cw_ma
-0001c500: 6372 6f73 3a20 636f 7079 696e 6720 6465  cros: copying de
-0001c510: 6661 756c 7420 6d61 6372 6f20 6669 6c65  fault macro file
-0001c520: 2e22 290a 2020 2020 2020 2020 2020 2020  .").            
-0001c530: 636f 7079 6669 6c65 280a 2020 2020 2020  copyfile(.      
-0001c540: 2020 2020 2020 2020 2020 6673 7574 696c            fsutil
-0001c550: 732e 4150 505f 4441 5441 5f50 4154 4820  s.APP_DATA_PATH 
-0001c560: 2f20 6d61 6372 6f5f 6669 6c65 2c20 6673  / macro_file, fs
-0001c570: 7574 696c 732e 5553 4552 5f44 4154 415f  utils.USER_DATA_
-0001c580: 5041 5448 202f 206d 6163 726f 5f66 696c  PATH / macro_fil
-0001c590: 650a 2020 2020 2020 2020 2020 2020 290a  e.            ).
-0001c5a0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-0001c5b0: 2020 2020 2020 2020 2066 7375 7469 6c73           fsutils
-0001c5c0: 2e6f 7065 6e46 696c 6557 6974 684f 5328  .openFileWithOS(
-0001c5d0: 6673 7574 696c 732e 5553 4552 5f44 4154  fsutils.USER_DAT
-0001c5e0: 415f 5041 5448 202f 206d 6163 726f 5f66  A_PATH / macro_f
-0001c5f0: 696c 6529 0a20 2020 2020 2020 2065 7863  ile).        exc
-0001c600: 6570 7420 4669 6c65 4e6f 7446 6f75 6e64  ept FileNotFound
-0001c610: 4572 726f 7220 7c20 5065 726d 6973 7369  Error | Permissi
-0001c620: 6f6e 4572 726f 7220 7c20 4f53 4572 726f  onError | OSErro
-0001c630: 7220 6173 2065 7272 3a0a 2020 2020 2020  r as err:.      
-0001c640: 2020 2020 2020 6c6f 6767 6572 2e63 7269        logger.cri
-0001c650: 7469 6361 6c28 0a20 2020 2020 2020 2020  tical(.         
-0001c660: 2020 2020 2020 2066 2243 6f75 6c64 206e         f"Could n
-0001c670: 6f74 206f 7065 6e20 6669 6c65 207b 6673  ot open file {fs
-0001c680: 7574 696c 732e 5553 4552 5f44 4154 415f  utils.USER_DATA_
-0001c690: 5041 5448 202f 206d 6163 726f 5f66 696c  PATH / macro_fil
-0001c6a0: 657d 207b 6572 727d 220a 2020 2020 2020  e} {err}".      
-0001c6b0: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
-0001c6c0: 2072 6561 645f 6377 5f6d 6163 726f 7328   read_cw_macros(
-0001c6d0: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
-0001c6e0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0001c6f0: 2020 2052 6561 6473 2069 6e20 7468 6520     Reads in the 
-0001c700: 4357 206d 6163 726f 732c 2066 6972 7374  CW macros, first
-0001c710: 7320 6974 2063 6865 636b 7320 746f 2073  s it checks to s
-0001c720: 6565 2069 6620 7468 6520 6669 6c65 2065  ee if the file e
-0001c730: 7869 7374 732e 2049 6620 6974 2064 6f65  xists. If it doe
-0001c740: 7320 6e6f 742c 0a20 2020 2020 2020 2061  s not,.        a
-0001c750: 6e64 2074 6869 7320 6861 7320 6265 656e  nd this has been
-0001c760: 2070 6163 6b61 6765 6420 7769 7468 2070   packaged with p
-0001c770: 7969 6e73 7461 6c6c 6572 2069 7420 7769  yinstaller it wi
-0001c780: 6c6c 2063 6f70 7920 7468 6520 6465 6661  ll copy the defa
-0001c790: 756c 7420 6669 6c65 2066 726f 6d20 7468  ult file from th
-0001c7a0: 650a 2020 2020 2020 2020 7465 6d70 2064  e.        temp d
-0001c7b0: 6972 6563 746f 7279 2074 6869 7320 6973  irectory this is
-0001c7c0: 2072 756e 6e69 6e67 2066 726f 6d2e 2e2e   running from...
-0001c7d0: 2049 6e20 7468 656f 7279 2e0a 2020 2020   In theory..    
-0001c7e0: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
-0001c7f0: 2069 6620 7365 6c66 2e72 6164 696f 5f73   if self.radio_s
-0001c800: 7461 7465 2e67 6574 2822 6d6f 6465 2229  tate.get("mode")
-0001c810: 203d 3d20 2243 5722 3a0a 2020 2020 2020   == "CW":.      
-0001c820: 2020 2020 2020 6d61 6372 6f5f 6669 6c65        macro_file
-0001c830: 203d 2022 6377 6d61 6372 6f73 2e74 7874   = "cwmacros.txt
-0001c840: 220a 2020 2020 2020 2020 656c 7365 3a0a  ".        else:.
-0001c850: 2020 2020 2020 2020 2020 2020 6d61 6372              macr
-0001c860: 6f5f 6669 6c65 203d 2022 7373 626d 6163  o_file = "ssbmac
-0001c870: 726f 732e 7478 7422 0a0a 2020 2020 2020  ros.txt"..      
-0001c880: 2020 6966 206e 6f74 2028 6673 7574 696c    if not (fsutil
-0001c890: 732e 5553 4552 5f44 4154 415f 5041 5448  s.USER_DATA_PATH
-0001c8a0: 202f 206d 6163 726f 5f66 696c 6529 2e65   / macro_file).e
-0001c8b0: 7869 7374 7328 293a 0a20 2020 2020 2020  xists():.       
-0001c8c0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-0001c8d0: 6728 2272 6561 645f 6377 5f6d 6163 726f  g("read_cw_macro
-0001c8e0: 733a 2063 6f70 7969 6e67 2064 6566 6175  s: copying defau
-0001c8f0: 6c74 206d 6163 726f 2066 696c 652e 2229  lt macro file.")
-0001c900: 0a20 2020 2020 2020 2020 2020 2063 6f70  .            cop
-0001c910: 7966 696c 6528 0a20 2020 2020 2020 2020  yfile(.         
-0001c920: 2020 2020 2020 2066 7375 7469 6c73 2e41         fsutils.A
-0001c930: 5050 5f44 4154 415f 5041 5448 202f 206d  PP_DATA_PATH / m
-0001c940: 6163 726f 5f66 696c 652c 2066 7375 7469  acro_file, fsuti
-0001c950: 6c73 2e55 5345 525f 4441 5441 5f50 4154  ls.USER_DATA_PAT
-0001c960: 4820 2f20 6d61 6372 6f5f 6669 6c65 0a20  H / macro_file. 
-0001c970: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0001c980: 2020 2020 2077 6974 6820 6f70 656e 280a       with open(.
-0001c990: 2020 2020 2020 2020 2020 2020 6673 7574              fsut
-0001c9a0: 696c 732e 5553 4552 5f44 4154 415f 5041  ils.USER_DATA_PA
-0001c9b0: 5448 202f 206d 6163 726f 5f66 696c 652c  TH / macro_file,
-0001c9c0: 2022 7222 2c20 656e 636f 6469 6e67 3d22   "r", encoding="
-0001c9d0: 7574 662d 3822 0a20 2020 2020 2020 2029  utf-8".        )
-0001c9e0: 2061 7320 6669 6c65 5f64 6573 6372 6970   as file_descrip
-0001c9f0: 746f 723a 0a20 2020 2020 2020 2020 2020  tor:.           
-0001ca00: 2066 6f72 206c 696e 6520 696e 2066 696c   for line in fil
-0001ca10: 655f 6465 7363 7269 7074 6f72 3a0a 2020  e_descriptor:.  
-0001ca20: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-0001ca30: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-0001ca40: 2020 2020 2020 206d 6f64 652c 2066 6b65         mode, fke
-0001ca50: 792c 2062 7574 746f 6e6e 616d 652c 2063  y, buttonname, c
-0001ca60: 7774 6578 7420 3d20 6c69 6e65 2e73 706c  wtext = line.spl
-0001ca70: 6974 2822 7c22 290a 2020 2020 2020 2020  it("|").        
-0001ca80: 2020 2020 2020 2020 2020 2020 6966 206d              if m
-0001ca90: 6f64 652e 7374 7269 7028 292e 7570 7065  ode.strip().uppe
-0001caa0: 7228 2920 3d3d 2022 5222 2061 6e64 2073  r() == "R" and s
-0001cab0: 656c 662e 7072 6566 2e67 6574 2822 7275  elf.pref.get("ru
-0001cac0: 6e5f 7374 6174 6522 293a 0a20 2020 2020  n_state"):.     
-0001cad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cae0: 2020 2073 656c 662e 666b 6579 735b 666b     self.fkeys[fk
-0001caf0: 6579 2e73 7472 6970 2829 5d20 3d20 2862  ey.strip()] = (b
-0001cb00: 7574 746f 6e6e 616d 652e 7374 7269 7028  uttonname.strip(
-0001cb10: 292c 2063 7774 6578 742e 7374 7269 7028  ), cwtext.strip(
-0001cb20: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-0001cb30: 2020 2020 2020 2069 6620 6d6f 6465 2e73         if mode.s
-0001cb40: 7472 6970 2829 2e75 7070 6572 2829 2021  trip().upper() !
-0001cb50: 3d20 2252 2220 616e 6420 6e6f 7420 7365  = "R" and not se
-0001cb60: 6c66 2e70 7265 662e 6765 7428 2272 756e  lf.pref.get("run
-0001cb70: 5f73 7461 7465 2229 3a0a 2020 2020 2020  _state"):.      
-0001cb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cb90: 2020 7365 6c66 2e66 6b65 7973 5b66 6b65    self.fkeys[fke
-0001cba0: 792e 7374 7269 7028 295d 203d 2028 6275  y.strip()] = (bu
-0001cbb0: 7474 6f6e 6e61 6d65 2e73 7472 6970 2829  ttonname.strip()
-0001cbc0: 2c20 6377 7465 7874 2e73 7472 6970 2829  , cwtext.strip()
-0001cbd0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001cbe0: 2020 6578 6365 7074 2056 616c 7565 4572    except ValueEr
-0001cbf0: 726f 7220 6173 2065 7272 3a0a 2020 2020  ror as err:.    
-0001cc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cc10: 6c6f 6767 6572 2e69 6e66 6f28 2272 6561  logger.info("rea
-0001cc20: 645f 6377 5f6d 6163 726f 733a 2025 7322  d_cw_macros: %s"
-0001cc30: 2c20 6572 7229 0a20 2020 2020 2020 206b  , err).        k
-0001cc40: 6579 7320 3d20 7365 6c66 2e66 6b65 7973  eys = self.fkeys
-0001cc50: 2e6b 6579 7328 290a 2020 2020 2020 2020  .keys().        
-0001cc60: 6966 2022 4631 2220 696e 206b 6579 733a  if "F1" in keys:
-0001cc70: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0001cc80: 662e 4631 2e73 6574 5465 7874 2866 2246  f.F1.setText(f"F
-0001cc90: 313a 207b 7365 6c66 2e66 6b65 7973 5b27  1: {self.fkeys['
-0001cca0: 4631 275d 5b30 5d7d 2229 0a20 2020 2020  F1'][0]}").     
-0001ccb0: 2020 2020 2020 2073 656c 662e 4631 2e73         self.F1.s
-0001ccc0: 6574 546f 6f6c 5469 7028 7365 6c66 2e66  etToolTip(self.f
-0001ccd0: 6b65 7973 5b22 4631 225d 5b31 5d29 0a20  keys["F1"][1]). 
-0001cce0: 2020 2020 2020 2069 6620 2246 3222 2069         if "F2" i
-0001ccf0: 6e20 6b65 7973 3a0a 2020 2020 2020 2020  n keys:.        
-0001cd00: 2020 2020 7365 6c66 2e46 322e 7365 7454      self.F2.setT
-0001cd10: 6578 7428 6622 4632 3a20 7b73 656c 662e  ext(f"F2: {self.
-0001cd20: 666b 6579 735b 2746 3227 5d5b 305d 7d22  fkeys['F2'][0]}"
-0001cd30: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-0001cd40: 6c66 2e46 322e 7365 7454 6f6f 6c54 6970  lf.F2.setToolTip
-0001cd50: 2873 656c 662e 666b 6579 735b 2246 3222  (self.fkeys["F2"
-0001cd60: 5d5b 315d 290a 2020 2020 2020 2020 6966  ][1]).        if
-0001cd70: 2022 4633 2220 696e 206b 6579 733a 0a20   "F3" in keys:. 
-0001cd80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001cd90: 4633 2e73 6574 5465 7874 2866 2246 333a  F3.setText(f"F3:
-0001cda0: 207b 7365 6c66 2e66 6b65 7973 5b27 4633   {self.fkeys['F3
-0001cdb0: 275d 5b30 5d7d 2229 0a20 2020 2020 2020  '][0]}").       
-0001cdc0: 2020 2020 2073 656c 662e 4633 2e73 6574       self.F3.set
-0001cdd0: 546f 6f6c 5469 7028 7365 6c66 2e66 6b65  ToolTip(self.fke
-0001cde0: 7973 5b22 4633 225d 5b31 5d29 0a20 2020  ys["F3"][1]).   
-0001cdf0: 2020 2020 2069 6620 2246 3422 2069 6e20       if "F4" in 
-0001ce00: 6b65 7973 3a0a 2020 2020 2020 2020 2020  keys:.          
-0001ce10: 2020 7365 6c66 2e46 342e 7365 7454 6578    self.F4.setTex
-0001ce20: 7428 6622 4634 3a20 7b73 656c 662e 666b  t(f"F4: {self.fk
-0001ce30: 6579 735b 2746 3427 5d5b 305d 7d22 290a  eys['F4'][0]}").
-0001ce40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001ce50: 2e46 342e 7365 7454 6f6f 6c54 6970 2873  .F4.setToolTip(s
-0001ce60: 656c 662e 666b 6579 735b 2246 3422 5d5b  elf.fkeys["F4"][
-0001ce70: 315d 290a 2020 2020 2020 2020 6966 2022  1]).        if "
-0001ce80: 4635 2220 696e 206b 6579 733a 0a20 2020  F5" in keys:.   
-0001ce90: 2020 2020 2020 2020 2073 656c 662e 4635           self.F5
-0001cea0: 2e73 6574 5465 7874 2866 2246 353a 207b  .setText(f"F5: {
-0001ceb0: 7365 6c66 2e66 6b65 7973 5b27 4635 275d  self.fkeys['F5']
-0001cec0: 5b30 5d7d 2229 0a20 2020 2020 2020 2020  [0]}").         
-0001ced0: 2020 2073 656c 662e 4635 2e73 6574 546f     self.F5.setTo
-0001cee0: 6f6c 5469 7028 7365 6c66 2e66 6b65 7973  olTip(self.fkeys
-0001cef0: 5b22 4635 225d 5b31 5d29 0a20 2020 2020  ["F5"][1]).     
-0001cf00: 2020 2069 6620 2246 3622 2069 6e20 6b65     if "F6" in ke
-0001cf10: 7973 3a0a 2020 2020 2020 2020 2020 2020  ys:.            
-0001cf20: 7365 6c66 2e46 362e 7365 7454 6578 7428  self.F6.setText(
-0001cf30: 6622 4636 3a20 7b73 656c 662e 666b 6579  f"F6: {self.fkey
-0001cf40: 735b 2746 3627 5d5b 305d 7d22 290a 2020  s['F6'][0]}").  
-0001cf50: 2020 2020 2020 2020 2020 7365 6c66 2e46            self.F
-0001cf60: 362e 7365 7454 6f6f 6c54 6970 2873 656c  6.setToolTip(sel
-0001cf70: 662e 666b 6579 735b 2246 3622 5d5b 315d  f.fkeys["F6"][1]
-0001cf80: 290a 2020 2020 2020 2020 6966 2022 4637  ).        if "F7
-0001cf90: 2220 696e 206b 6579 733a 0a20 2020 2020  " in keys:.     
-0001cfa0: 2020 2020 2020 2073 656c 662e 4637 2e73         self.F7.s
-0001cfb0: 6574 5465 7874 2866 2246 373a 207b 7365  etText(f"F7: {se
-0001cfc0: 6c66 2e66 6b65 7973 5b27 4637 275d 5b30  lf.fkeys['F7'][0
-0001cfd0: 5d7d 2229 0a20 2020 2020 2020 2020 2020  ]}").           
-0001cfe0: 2073 656c 662e 4637 2e73 6574 546f 6f6c   self.F7.setTool
-0001cff0: 5469 7028 7365 6c66 2e66 6b65 7973 5b22  Tip(self.fkeys["
-0001d000: 4637 225d 5b31 5d29 0a20 2020 2020 2020  F7"][1]).       
-0001d010: 2069 6620 2246 3822 2069 6e20 6b65 7973   if "F8" in keys
-0001d020: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0001d030: 6c66 2e46 382e 7365 7454 6578 7428 6622  lf.F8.setText(f"
-0001d040: 4638 3a20 7b73 656c 662e 666b 6579 735b  F8: {self.fkeys[
-0001d050: 2746 3827 5d5b 305d 7d22 290a 2020 2020  'F8'][0]}").    
-0001d060: 2020 2020 2020 2020 7365 6c66 2e46 382e          self.F8.
-0001d070: 7365 7454 6f6f 6c54 6970 2873 656c 662e  setToolTip(self.
-0001d080: 666b 6579 735b 2246 3822 5d5b 315d 290a  fkeys["F8"][1]).
-0001d090: 2020 2020 2020 2020 6966 2022 4639 2220          if "F9" 
-0001d0a0: 696e 206b 6579 733a 0a20 2020 2020 2020  in keys:.       
-0001d0b0: 2020 2020 2073 656c 662e 4639 2e73 6574       self.F9.set
-0001d0c0: 5465 7874 2866 2246 393a 207b 7365 6c66  Text(f"F9: {self
-0001d0d0: 2e66 6b65 7973 5b27 4639 275d 5b30 5d7d  .fkeys['F9'][0]}
-0001d0e0: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
-0001d0f0: 656c 662e 4639 2e73 6574 546f 6f6c 5469  elf.F9.setToolTi
-0001d100: 7028 7365 6c66 2e66 6b65 7973 5b22 4639  p(self.fkeys["F9
-0001d110: 225d 5b31 5d29 0a20 2020 2020 2020 2069  "][1]).        i
-0001d120: 6620 2246 3130 2220 696e 206b 6579 733a  f "F10" in keys:
-0001d130: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0001d140: 662e 4631 302e 7365 7454 6578 7428 6622  f.F10.setText(f"
-0001d150: 4631 303a 207b 7365 6c66 2e66 6b65 7973  F10: {self.fkeys
-0001d160: 5b27 4631 3027 5d5b 305d 7d22 290a 2020  ['F10'][0]}").  
-0001d170: 2020 2020 2020 2020 2020 7365 6c66 2e46            self.F
-0001d180: 3130 2e73 6574 546f 6f6c 5469 7028 7365  10.setToolTip(se
-0001d190: 6c66 2e66 6b65 7973 5b22 4631 3022 5d5b  lf.fkeys["F10"][
-0001d1a0: 315d 290a 2020 2020 2020 2020 6966 2022  1]).        if "
-0001d1b0: 4631 3122 2069 6e20 6b65 7973 3a0a 2020  F11" in keys:.  
-0001d1c0: 2020 2020 2020 2020 2020 7365 6c66 2e46            self.F
-0001d1d0: 3131 2e73 6574 5465 7874 2866 2246 3131  11.setText(f"F11
-0001d1e0: 3a20 7b73 656c 662e 666b 6579 735b 2746  : {self.fkeys['F
-0001d1f0: 3131 275d 5b30 5d7d 2229 0a20 2020 2020  11'][0]}").     
-0001d200: 2020 2020 2020 2073 656c 662e 4631 312e         self.F11.
-0001d210: 7365 7454 6f6f 6c54 6970 2873 656c 662e  setToolTip(self.
-0001d220: 666b 6579 735b 2246 3131 225d 5b31 5d29  fkeys["F11"][1])
-0001d230: 0a20 2020 2020 2020 2069 6620 2246 3132  .        if "F12
-0001d240: 2220 696e 206b 6579 733a 0a20 2020 2020  " in keys:.     
-0001d250: 2020 2020 2020 2073 656c 662e 4631 322e         self.F12.
-0001d260: 7365 7454 6578 7428 6622 4631 323a 207b  setText(f"F12: {
-0001d270: 7365 6c66 2e66 6b65 7973 5b27 4631 3227  self.fkeys['F12'
-0001d280: 5d5b 305d 7d22 290a 2020 2020 2020 2020  ][0]}").        
-0001d290: 2020 2020 7365 6c66 2e46 3132 2e73 6574      self.F12.set
-0001d2a0: 546f 6f6c 5469 7028 7365 6c66 2e66 6b65  ToolTip(self.fke
-0001d2b0: 7973 5b22 4631 3222 5d5b 315d 290a 0a20  ys["F12"][1]).. 
-0001d2c0: 2020 2064 6566 2067 656e 6572 6174 655f     def generate_
-0001d2d0: 6164 6966 2873 656c 6629 202d 3e20 4e6f  adif(self) -> No
-0001d2e0: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
-0001d2f0: 2020 2020 2020 2020 4361 6c6c 7320 7468          Calls th
-0001d300: 6520 636f 6e74 6573 7420 4144 4946 2066  e contest ADIF f
-0001d310: 696c 6520 6765 6e65 7261 746f 722e 0a0a  ile generator...
-0001d320: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-0001d330: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
-0001d340: 2d2d 2d2d 2d0a 2020 2020 2020 2020 4e6f  -----.        No
-0001d350: 6e65 0a0a 2020 2020 2020 2020 5265 7475  ne..        Retu
-0001d360: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
-0001d370: 2d2d 2d0a 2020 2020 2020 2020 4e6f 6e65  ---.        None
-0001d380: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
-0001d390: 2020 2020 2020 2320 6874 7470 733a 2f2f        # https://
-0001d3a0: 7777 772e 6164 6966 2e6f 7267 2f33 3135  www.adif.org/315
-0001d3b0: 2f41 4449 465f 3331 352e 6874 6d0a 2020  /ADIF_315.htm.  
-0001d3c0: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-0001d3d0: 7567 2822 2a2a 2a2a 2a2a 4144 4946 2a2a  ug("******ADIF**
-0001d3e0: 2a2a 2a22 290a 2020 2020 2020 2020 7365  ***").        se
-0001d3f0: 6c66 2e63 6f6e 7465 7374 2e61 6469 6628  lf.contest.adif(
-0001d400: 7365 6c66 290a 0a20 2020 2064 6566 2067  self)..    def g
-0001d410: 656e 6572 6174 655f 6361 6272 696c 6c6f  enerate_cabrillo
-0001d420: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-0001d430: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0001d440: 2020 2020 4361 6c6c 7320 7468 6520 636f      Calls the co
-0001d450: 6e74 6573 7420 4361 6272 696c 6c6f 2066  ntest Cabrillo f
-0001d460: 696c 6520 6765 6e65 7261 746f 722e 204d  ile generator. M
-0001d470: 6179 6265 2e0a 0a20 2020 2020 2020 2050  aybe...        P
-0001d480: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-0001d490: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-0001d4a0: 2020 2020 204e 6f6e 650a 0a20 2020 2020       None..     
-0001d4b0: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
-0001d4c0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
-0001d4d0: 2020 204e 6f6e 650a 2020 2020 2020 2020     None.        
-0001d4e0: 2222 220a 0a20 2020 2020 2020 206c 6f67  """..        log
-0001d4f0: 6765 722e 6465 6275 6728 222a 2a2a 2a2a  ger.debug("*****
-0001d500: 2a43 6162 7269 6c6c 6f2a 2a2a 2a2a 2229  *Cabrillo*****")
-0001d510: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-0001d520: 6e74 6573 742e 6361 6272 696c 6c6f 2873  ntest.cabrillo(s
-0001d530: 656c 6629 0a0a 0a64 6566 206c 6f61 645f  elf)...def load_
-0001d540: 666f 6e74 735f 6672 6f6d 5f64 6972 2864  fonts_from_dir(d
-0001d550: 6972 6563 746f 7279 3a20 7374 7229 202d  irectory: str) -
-0001d560: 3e20 7365 743a 0a20 2020 2022 2222 0a20  > set:.    """. 
-0001d570: 2020 2057 656c 6c20 6974 206c 6f61 6473     Well it loads
-0001d580: 2066 6f6e 7473 2066 726f 6d20 6120 6469   fonts from a di
-0001d590: 7265 6374 6f72 792e 2e2e 0a0a 2020 2020  rectory.....    
-0001d5a0: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
-0001d5b0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6469  ---------.    di
-0001d5c0: 7265 6374 6f72 7920 3a20 7374 720a 2020  rectory : str.  
-0001d5d0: 2020 5468 6520 6469 7265 6374 6f72 7920    The directory 
-0001d5e0: 746f 206c 6f61 6420 666f 6e74 7320 6672  to load fonts fr
-0001d5f0: 6f6d 2e0a 0a20 2020 2052 6574 7572 6e73  om...    Returns
-0001d600: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
-0001d610: 2073 6574 0a20 2020 2041 2073 6574 206f   set.    A set o
-0001d620: 6620 666f 6e74 2066 616d 696c 6965 7320  f font families 
-0001d630: 696e 7374 616c 6c65 6420 696e 2074 6865  installed in the
-0001d640: 2064 6972 6563 746f 7279 2e0a 2020 2020   directory..    
-0001d650: 2222 220a 2020 2020 666f 6e74 5f66 616d  """.    font_fam
-0001d660: 696c 6965 7320 3d20 7365 7428 290a 2020  ilies = set().  
-0001d670: 2020 666f 7220 5f66 6920 696e 2051 4469    for _fi in QDi
-0001d680: 7228 6469 7265 6374 6f72 7929 2e65 6e74  r(directory).ent
-0001d690: 7279 496e 666f 4c69 7374 285b 222a 2e74  ryInfoList(["*.t
-0001d6a0: 7466 222c 2022 2a2e 776f 6666 222c 2022  tf", "*.woff", "
-0001d6b0: 2a2e 776f 6666 3222 5d29 3a0a 2020 2020  *.woff2"]):.    
-0001d6c0: 2020 2020 5f69 6420 3d20 5146 6f6e 7444      _id = QFontD
-0001d6d0: 6174 6162 6173 652e 6164 6441 7070 6c69  atabase.addAppli
-0001d6e0: 6361 7469 6f6e 466f 6e74 285f 6669 2e61  cationFont(_fi.a
-0001d6f0: 6273 6f6c 7574 6546 696c 6550 6174 6828  bsoluteFilePath(
-0001d700: 2929 0a20 2020 2020 2020 2066 6f6e 745f  )).        font_
-0001d710: 6661 6d69 6c69 6573 207c 3d20 7365 7428  families |= set(
-0001d720: 5146 6f6e 7444 6174 6162 6173 652e 6170  QFontDatabase.ap
-0001d730: 706c 6963 6174 696f 6e46 6f6e 7446 616d  plicationFontFam
-0001d740: 696c 6965 7328 5f69 6429 290a 2020 2020  ilies(_id)).    
-0001d750: 7265 7475 726e 2066 6f6e 745f 6661 6d69  return font_fami
-0001d760: 6c69 6573 0a0a 0a64 6566 2069 6e73 7461  lies...def insta
-0001d770: 6c6c 5f69 636f 6e73 2829 202d 3e20 4e6f  ll_icons() -> No
-0001d780: 6e65 3a0a 2020 2020 2222 2249 6e73 7461  ne:.    """Insta
-0001d790: 6c6c 2069 636f 6e73 2222 220a 0a20 2020  ll icons"""..   
-0001d7a0: 2069 6620 7379 732e 706c 6174 666f 726d   if sys.platform
-0001d7b0: 203d 3d20 226c 696e 7578 223a 0a20 2020   == "linux":.   
-0001d7c0: 2020 2020 206f 732e 7379 7374 656d 280a       os.system(.
-0001d7d0: 2020 2020 2020 2020 2020 2020 2278 6467              "xdg
-0001d7e0: 2d69 636f 6e2d 7265 736f 7572 6365 2069  -icon-resource i
-0001d7f0: 6e73 7461 6c6c 202d 2d73 697a 6520 3332  nstall --size 32
-0001d800: 202d 2d63 6f6e 7465 7874 2061 7070 7320   --context apps 
-0001d810: 2d2d 6d6f 6465 2075 7365 7220 220a 2020  --mode user ".  
-0001d820: 2020 2020 2020 2020 2020 6622 7b66 7375            f"{fsu
-0001d830: 7469 6c73 2e41 5050 5f44 4154 415f 5041  tils.APP_DATA_PA
-0001d840: 5448 7d2f 6b36 6774 652e 6e6f 7431 6d6d  TH}/k6gte.not1mm
-0001d850: 2d33 322e 706e 6720 6b36 6774 652d 6e6f  -32.png k6gte-no
-0001d860: 7431 6d6d 220a 2020 2020 2020 2020 290a  t1mm".        ).
-0001d870: 2020 2020 2020 2020 6f73 2e73 7973 7465          os.syste
-0001d880: 6d28 0a20 2020 2020 2020 2020 2020 2022  m(.            "
-0001d890: 7864 672d 6963 6f6e 2d72 6573 6f75 7263  xdg-icon-resourc
-0001d8a0: 6520 696e 7374 616c 6c20 2d2d 7369 7a65  e install --size
-0001d8b0: 2036 3420 2d2d 636f 6e74 6578 7420 6170   64 --context ap
-0001d8c0: 7073 202d 2d6d 6f64 6520 7573 6572 2022  ps --mode user "
-0001d8d0: 0a20 2020 2020 2020 2020 2020 2066 227b  .            f"{
-0001d8e0: 6673 7574 696c 732e 4150 505f 4441 5441  fsutils.APP_DATA
-0001d8f0: 5f50 4154 487d 2f6b 3667 7465 2e6e 6f74  _PATH}/k6gte.not
-0001d900: 316d 6d2d 3634 2e70 6e67 206b 3667 7465  1mm-64.png k6gte
-0001d910: 2d6e 6f74 316d 6d22 0a20 2020 2020 2020  -not1mm".       
-0001d920: 2029 0a20 2020 2020 2020 206f 732e 7379   ).        os.sy
-0001d930: 7374 656d 280a 2020 2020 2020 2020 2020  stem(.          
-0001d940: 2020 2278 6467 2d69 636f 6e2d 7265 736f    "xdg-icon-reso
-0001d950: 7572 6365 2069 6e73 7461 6c6c 202d 2d73  urce install --s
-0001d960: 697a 6520 3132 3820 2d2d 636f 6e74 6578  ize 128 --contex
-0001d970: 7420 6170 7073 202d 2d6d 6f64 6520 7573  t apps --mode us
-0001d980: 6572 2022 0a20 2020 2020 2020 2020 2020  er ".           
-0001d990: 2066 227b 6673 7574 696c 732e 4150 505f   f"{fsutils.APP_
-0001d9a0: 4441 5441 5f50 4154 487d 2f6b 3667 7465  DATA_PATH}/k6gte
-0001d9b0: 2e6e 6f74 316d 6d2d 3132 382e 706e 6720  .not1mm-128.png 
-0001d9c0: 6b36 6774 652d 6e6f 7431 6d6d 220a 2020  k6gte-not1mm".  
-0001d9d0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0001d9e0: 6f73 2e73 7973 7465 6d28 0a20 2020 2020  os.system(.     
-0001d9f0: 2020 2020 2020 2066 2278 6467 2d64 6573         f"xdg-des
-0001da00: 6b74 6f70 2d6d 656e 7520 696e 7374 616c  ktop-menu instal
-0001da10: 6c20 7b66 7375 7469 6c73 2e41 5050 5f44  l {fsutils.APP_D
-0001da20: 4154 415f 5041 5448 7d2f 6b36 6774 652d  ATA_PATH}/k6gte-
-0001da30: 6e6f 7431 6d6d 2e64 6573 6b74 6f70 220a  not1mm.desktop".
-0001da40: 2020 2020 2020 2020 290a 0a0a 6465 6620          )...def 
-0001da50: 646f 696d 7028 6d6f 646e 616d 6529 202d  doimp(modname) -
-0001da60: 3e20 6f62 6a65 6374 3a0a 2020 2020 2222  > object:.    ""
-0001da70: 220a 2020 2020 496d 706f 7274 7320 6120  ".    Imports a 
-0001da80: 6d6f 6475 6c65 2e0a 0a20 2020 2050 6172  module...    Par
-0001da90: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
-0001daa0: 2d2d 2d2d 2d2d 0a20 2020 206d 6f64 6e61  ------.    modna
-0001dab0: 6d65 203a 2073 7472 0a20 2020 2054 6865  me : str.    The
-0001dac0: 206e 616d 6520 6f66 2074 6865 206d 6f64   name of the mod
-0001dad0: 756c 6520 746f 2069 6d70 6f72 742e 0a0a  ule to import...
-0001dae0: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-0001daf0: 2d2d 2d2d 2d2d 2d0a 2020 2020 6f62 6a65  -------.    obje
-0001db00: 6374 0a20 2020 2054 6865 206d 6f64 756c  ct.    The modul
-0001db10: 6520 6f62 6a65 6374 2e0a 2020 2020 2222  e object..    ""
-0001db20: 220a 0a20 2020 206c 6f67 6765 722e 6465  "..    logger.de
-0001db30: 6275 6728 2264 6f69 6d70 3a20 2573 222c  bug("doimp: %s",
-0001db40: 206d 6f64 6e61 6d65 290a 2020 2020 7265   modname).    re
-0001db50: 7475 726e 2069 6d70 6f72 746c 6962 2e69  turn importlib.i
-0001db60: 6d70 6f72 745f 6d6f 6475 6c65 2866 226e  mport_module(f"n
-0001db70: 6f74 316d 6d2e 706c 7567 696e 732e 7b6d  ot1mm.plugins.{m
-0001db80: 6f64 6e61 6d65 7d22 290a 0a0a 6465 6620  odname}")...def 
-0001db90: 7275 6e28 2920 2d3e 204e 6f6e 653a 0a20  run() -> None:. 
-0001dba0: 2020 2022 2222 0a20 2020 204d 6169 6e20     """.    Main 
-0001dbb0: 456e 7472 790a 2020 2020 2222 220a 2020  Entry.    """.  
-0001dbc0: 2020 6c6f 6767 6572 2e64 6562 7567 280a    logger.debug(.
-0001dbd0: 2020 2020 2020 2020 6622 5265 736f 6c76          f"Resolv
-0001dbe0: 6564 204f 5320 6669 6c65 2073 7973 7465  ed OS file syste
-0001dbf0: 6d20 7061 7468 733a 204d 4f44 554c 455f  m paths: MODULE_
-0001dc00: 5041 5448 207b 6673 7574 696c 732e 4d4f  PATH {fsutils.MO
-0001dc10: 4455 4c45 5f50 4154 487d 2c20 5553 4552  DULE_PATH}, USER
-0001dc20: 5f44 4154 415f 5041 5448 207b 6673 7574  _DATA_PATH {fsut
-0001dc30: 696c 732e 5553 4552 5f44 4154 415f 5041  ils.USER_DATA_PA
-0001dc40: 5448 7d2c 2043 4f4e 4649 475f 5041 5448  TH}, CONFIG_PATH
-0001dc50: 207b 6673 7574 696c 732e 434f 4e46 4947   {fsutils.CONFIG
-0001dc60: 5f50 4154 487d 220a 2020 2020 290a 2020  _PATH}".    ).  
-0001dc70: 2020 696e 7374 616c 6c5f 6963 6f6e 7328    install_icons(
-0001dc80: 290a 2020 2020 7469 6d65 722e 7374 6172  ).    timer.star
-0001dc90: 7428 3235 3029 0a20 2020 2073 7973 2e65  t(250).    sys.e
-0001dca0: 7869 7428 6170 702e 6578 6563 2829 290a  xit(app.exec()).
-0001dcb0: 0a0a 4445 4255 475f 454e 4142 4c45 4420  ..DEBUG_ENABLED 
-0001dcc0: 3d20 4661 6c73 650a 6966 2050 6174 6828  = False.if Path(
-0001dcd0: 222e 2f64 6562 7567 2229 2e65 7869 7374  "./debug").exist
-0001dce0: 7328 293a 0a20 2020 2044 4542 5547 5f45  s():.    DEBUG_E
-0001dcf0: 4e41 424c 4544 203d 2054 7275 650a 0a6c  NABLED = True..l
-0001dd00: 6f67 6765 7220 3d20 6c6f 6767 696e 672e  ogger = logging.
-0001dd10: 6765 744c 6f67 6765 7228 225f 5f6d 6169  getLogger("__mai
-0001dd20: 6e5f 5f22 290a 0a6c 6f67 6769 6e67 2e62  n__")..logging.b
-0001dd30: 6173 6963 436f 6e66 6967 280a 2020 2020  asicConfig(.    
-0001dd40: 6c65 7665 6c3d 6c6f 6767 696e 672e 4445  level=logging.DE
-0001dd50: 4255 4720 6966 2044 4542 5547 5f45 4e41  BUG if DEBUG_ENA
-0001dd60: 424c 4544 2065 6c73 6520 6c6f 6767 696e  BLED else loggin
-0001dd70: 672e 4352 4954 4943 414c 2c0a 2020 2020  g.CRITICAL,.    
-0001dd80: 666f 726d 6174 3d22 5b25 2861 7363 7469  format="[%(ascti
-0001dd90: 6d65 2973 5d20 2528 6c65 7665 6c6e 616d  me)s] %(levelnam
-0001dda0: 6529 7320 2528 6e61 6d65 2973 202d 2025  e)s %(name)s - %
-0001ddb0: 2866 756e 634e 616d 6529 7320 4c69 6e65  (funcName)s Line
-0001ddc0: 2025 286c 696e 656e 6f29 643a 2025 286d   %(lineno)d: %(m
-0001ddd0: 6573 7361 6765 2973 222c 0a20 2020 2068  essage)s",.    h
-0001dde0: 616e 646c 6572 733d 5b0a 2020 2020 2020  andlers=[.      
-0001ddf0: 2020 526f 7461 7469 6e67 4669 6c65 4861    RotatingFileHa
-0001de00: 6e64 6c65 7228 6673 7574 696c 732e 4c4f  ndler(fsutils.LO
-0001de10: 475f 4649 4c45 2c20 6d61 7842 7974 6573  G_FILE, maxBytes
-0001de20: 3d31 3034 3930 3030 302c 2062 6163 6b75  =10490000, backu
-0001de30: 7043 6f75 6e74 3d32 3029 2c0a 2020 2020  pCount=20),.    
-0001de40: 2020 2020 6c6f 6767 696e 672e 5374 7265      logging.Stre
-0001de50: 616d 4861 6e64 6c65 7228 292c 0a20 2020  amHandler(),.   
-0001de60: 205d 2c0a 290a 6c6f 6767 696e 672e 6765   ],.).logging.ge
-0001de70: 744c 6f67 6765 7228 2250 7951 7436 2e75  tLogger("PyQt6.u
-0001de80: 6963 2e75 6970 6172 7365 7222 292e 7365  ic.uiparser").se
-0001de90: 744c 6576 656c 2822 494e 464f 2229 0a6c  tLevel("INFO").l
-0001dea0: 6f67 6769 6e67 2e67 6574 4c6f 6767 6572  ogging.getLogger
-0001deb0: 2822 5079 5174 362e 7569 632e 7072 6f70  ("PyQt6.uic.prop
-0001dec0: 6572 7469 6573 2229 2e73 6574 4c65 7665  erties").setLeve
-0001ded0: 6c28 2249 4e46 4f22 290a 6170 7020 3d20  l("INFO").app = 
-0001dee0: 5174 5769 6467 6574 732e 5141 7070 6c69  QtWidgets.QAppli
-0001def0: 6361 7469 6f6e 2873 7973 2e61 7267 7629  cation(sys.argv)
-0001df00: 0a66 616d 696c 6965 7320 3d20 6c6f 6164  .families = load
-0001df10: 5f66 6f6e 7473 5f66 726f 6d5f 6469 7228  _fonts_from_dir(
-0001df20: 6f73 2e66 7370 6174 6828 6673 7574 696c  os.fspath(fsutil
-0001df30: 732e 4150 505f 4441 5441 5f50 4154 4829  s.APP_DATA_PATH)
-0001df40: 290a 6c6f 6767 6572 2e69 6e66 6f28 6622  ).logger.info(f"
-0001df50: 666f 6e74 2066 616d 696c 6965 7320 7b66  font families {f
-0001df60: 616d 696c 6965 737d 2229 0a77 696e 646f  amilies}").windo
-0001df70: 7720 3d20 4d61 696e 5769 6e64 6f77 2829  w = MainWindow()
-0001df80: 0a68 6569 6768 7420 3d20 7769 6e64 6f77  .height = window
-0001df90: 2e70 7265 662e 6765 7428 2277 696e 646f  .pref.get("windo
-0001dfa0: 775f 6865 6967 6874 222c 2033 3030 290a  w_height", 300).
-0001dfb0: 7769 6474 6820 3d20 7769 6e64 6f77 2e70  width = window.p
-0001dfc0: 7265 662e 6765 7428 2277 696e 646f 775f  ref.get("window_
-0001dfd0: 7769 6474 6822 2c20 3730 3029 0a78 203d  width", 700).x =
-0001dfe0: 2077 696e 646f 772e 7072 6566 2e67 6574   window.pref.get
-0001dff0: 2822 7769 6e64 6f77 5f78 222c 202d 3129  ("window_x", -1)
-0001e000: 0a79 203d 2077 696e 646f 772e 7072 6566  .y = window.pref
-0001e010: 2e67 6574 2822 7769 6e64 6f77 5f79 222c  .get("window_y",
-0001e020: 202d 3129 0a77 696e 646f 772e 7365 7447   -1).window.setG
-0001e030: 656f 6d65 7472 7928 782c 2079 2c20 7769  eometry(x, y, wi
-0001e040: 6474 682c 2068 6569 6768 7429 0a77 696e  dth, height).win
-0001e050: 646f 772e 6361 6c6c 7369 676e 2e73 6574  dow.callsign.set
-0001e060: 466f 6375 7328 290a 7769 6e64 6f77 2e73  Focus().window.s
-0001e070: 686f 7728 290a 7469 6d65 7220 3d20 5174  how().timer = Qt
-0001e080: 436f 7265 2e51 5469 6d65 7228 290a 7469  Core.QTimer().ti
-0001e090: 6d65 722e 7469 6d65 6f75 742e 636f 6e6e  mer.timeout.conn
-0001e0a0: 6563 7428 7769 6e64 6f77 2e70 6f6c 6c5f  ect(window.poll_
-0001e0b0: 7261 6469 6f29 0a0a 6966 205f 5f6e 616d  radio)..if __nam
-0001e0c0: 655f 5f20 3d3d 2022 5f5f 6d61 696e 5f5f  e__ == "__main__
-0001e0d0: 223a 0a20 2020 2072 756e 2829 0a         ":.    run().
+0001ba50: 5f62 7728 290a 0a20 2020 2020 2020 2020  _bw()..         
+0001ba60: 2020 2020 2020 2069 6620 6d6f 6465 203d         if mode =
+0001ba70: 3d20 2243 5722 3a0a 2020 2020 2020 2020  = "CW":.        
+0001ba80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001ba90: 2e73 6574 6d6f 6465 286d 6f64 6529 0a20  .setmode(mode). 
+0001baa0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0001bab0: 6620 6d6f 6465 203d 3d20 224c 5342 2220  f mode == "LSB" 
+0001bac0: 6f72 206d 6f64 6520 3d3d 2022 5553 4222  or mode == "USB"
+0001bad0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001bae0: 2020 2020 2020 7365 6c66 2e73 6574 6d6f        self.setmo
+0001baf0: 6465 2822 5353 4222 290a 2020 2020 2020  de("SSB").      
+0001bb00: 2020 2020 2020 2020 2020 6966 206d 6f64            if mod
+0001bb10: 6520 3d3d 2022 5254 5459 223a 0a20 2020  e == "RTTY":.   
+0001bb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bb30: 2073 656c 662e 7365 746d 6f64 6528 2252   self.setmode("R
+0001bb40: 5454 5922 290a 0a20 2020 2020 2020 2020  TTY")..         
+0001bb50: 2020 2020 2020 2069 6620 7666 6f20 3d3d         if vfo ==
+0001bb60: 2022 223a 0a20 2020 2020 2020 2020 2020   "":.           
+0001bb70: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+0001bb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bb90: 6966 2073 656c 662e 7261 6469 6f5f 7374  if self.radio_st
+0001bba0: 6174 652e 6765 7428 2276 666f 6122 2920  ate.get("vfoa") 
+0001bbb0: 213d 2076 666f 3a0a 2020 2020 2020 2020  != vfo:.        
+0001bbc0: 2020 2020 2020 2020 2020 2020 696e 666f              info
+0001bbd0: 5f64 6972 7479 203d 2054 7275 650a 2020  _dirty = True.  
+0001bbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bbf0: 2020 7365 6c66 2e72 6164 696f 5f73 7461    self.radio_sta
+0001bc00: 7465 5b22 7666 6f61 225d 203d 2076 666f  te["vfoa"] = vfo
+0001bc10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001bc20: 2062 616e 6420 3d20 6765 7462 616e 6428   band = getband(
+0001bc30: 7374 7228 7666 6f29 290a 2020 2020 2020  str(vfo)).      
+0001bc40: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+0001bc50: 6164 696f 5f73 7461 7465 5b22 6261 6e64  adio_state["band
+0001bc60: 225d 203d 2062 616e 640a 2020 2020 2020  "] = band.      
+0001bc70: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0001bc80: 6f6e 7461 6374 5b22 4261 6e64 225d 203d  ontact["Band"] =
+0001bc90: 2067 6574 5f6c 6f67 6765 645f 6261 6e64   get_logged_band
+0001bca0: 2873 7472 2876 666f 2929 0a20 2020 2020  (str(vfo)).     
+0001bcb0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0001bcc0: 7365 745f 6261 6e64 5f69 6e64 6963 6174  set_band_indicat
+0001bcd0: 6f72 2862 616e 6429 0a0a 2020 2020 2020  or(band)..      
+0001bce0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0001bcf0: 662e 7261 6469 6f5f 7374 6174 652e 6765  f.radio_state.ge
+0001bd00: 7428 226d 6f64 6522 2920 213d 206d 6f64  t("mode") != mod
+0001bd10: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0001bd20: 2020 2020 2020 2069 6e66 6f5f 6469 7274         info_dirt
+0001bd30: 7920 3d20 5472 7565 0a20 2020 2020 2020  y = True.       
+0001bd40: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0001bd50: 662e 7261 6469 6f5f 7374 6174 655b 226d  f.radio_state["m
+0001bd60: 6f64 6522 5d20 3d20 6d6f 6465 0a0a 2020  ode"] = mode..  
+0001bd70: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0001bd80: 2073 656c 662e 7261 6469 6f5f 7374 6174   self.radio_stat
+0001bd90: 652e 6765 7428 2262 7722 2920 213d 2062  e.get("bw") != b
+0001bda0: 773a 0a20 2020 2020 2020 2020 2020 2020  w:.             
+0001bdb0: 2020 2020 2020 2069 6e66 6f5f 6469 7274         info_dirt
+0001bdc0: 7920 3d20 5472 7565 0a20 2020 2020 2020  y = True.       
+0001bdd0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0001bde0: 662e 7261 6469 6f5f 7374 6174 655b 2262  f.radio_state["b
+0001bdf0: 7722 5d20 3d20 6277 0a0a 2020 2020 2020  w"] = bw..      
+0001be00: 2020 2020 2020 2020 2020 6966 2064 6174            if dat
+0001be10: 6574 696d 652e 6461 7465 7469 6d65 2e6e  etime.datetime.n
+0001be20: 6f77 2829 203e 2067 6c6f 6261 6c73 2829  ow() > globals()
+0001be30: 5b22 706f 6c6c 5f74 696d 6522 5d20 6f72  ["poll_time"] or
+0001be40: 2069 6e66 6f5f 6469 7274 793a 0a20 2020   info_dirty:.   
+0001be50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001be60: 206c 6f67 6765 722e 6465 6275 6728 2256   logger.debug("V
+0001be70: 464f 3a20 2573 2020 4d4f 4445 3a20 2573  FO: %s  MODE: %s
+0001be80: 2042 573a 2025 7322 2c20 7666 6f2c 206d   BW: %s", vfo, m
+0001be90: 6f64 652c 2062 7729 0a20 2020 2020 2020  ode, bw).       
+0001bea0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0001beb0: 662e 7365 745f 7769 6e64 6f77 5f74 6974  f.set_window_tit
+0001bec0: 6c65 2829 0a20 2020 2020 2020 2020 2020  le().           
+0001bed0: 2020 2020 2020 2020 2063 6d64 203d 207b           cmd = {
+0001bee0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+0001bef0: 2020 2020 2020 636d 645b 2263 6d64 225d        cmd["cmd"]
+0001bf00: 203d 2022 5241 4449 4f5f 5354 4154 4522   = "RADIO_STATE"
+0001bf10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001bf20: 2020 2020 2063 6d64 5b22 7374 6174 696f       cmd["statio
+0001bf30: 6e22 5d20 3d20 706c 6174 666f 726d 2e6e  n"] = platform.n
+0001bf40: 6f64 6528 290a 2020 2020 2020 2020 2020  ode().          
+0001bf50: 2020 2020 2020 2020 2020 636d 645b 2262            cmd["b
+0001bf60: 616e 6422 5d20 3d20 6261 6e64 0a20 2020  and"] = band.   
+0001bf70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bf80: 2063 6d64 5b22 7666 6f61 225d 203d 2076   cmd["vfoa"] = v
+0001bf90: 666f 0a20 2020 2020 2020 2020 2020 2020  fo.             
+0001bfa0: 2020 2020 2020 2063 6d64 5b22 6d6f 6465         cmd["mode
+0001bfb0: 225d 203d 206d 6f64 650a 2020 2020 2020  "] = mode.      
+0001bfc0: 2020 2020 2020 2020 2020 2020 2020 636d                cm
+0001bfd0: 645b 2262 7722 5d20 3d20 6277 0a20 2020  d["bw"] = bw.   
+0001bfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bff0: 2073 656c 662e 6d75 6c74 6963 6173 745f   self.multicast_
+0001c000: 696e 7465 7266 6163 652e 7365 6e64 5f61  interface.send_a
+0001c010: 735f 6a73 6f6e 2863 6d64 290a 2020 2020  s_json(cmd).    
+0001c020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c030: 6966 2073 656c 662e 6e31 6d6d 3a0a 2020  if self.n1mm:.  
+0001c040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c050: 2020 2020 2020 6966 2073 656c 662e 6e31        if self.n1
+0001c060: 6d6d 2e73 656e 645f 7261 6469 6f5f 7061  mm.send_radio_pa
+0001c070: 636b 6574 733a 0a20 2020 2020 2020 2020  ckets:.         
+0001c080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c090: 2020 2073 656c 662e 6e31 6d6d 2e72 6164     self.n1mm.rad
+0001c0a0: 696f 5f69 6e66 6f5b 2246 7265 7122 5d20  io_info["Freq"] 
+0001c0b0: 3d20 7666 6f5b 3a2d 315d 0a20 2020 2020  = vfo[:-1].     
+0001c0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c0d0: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
+0001c0e0: 2e72 6164 696f 5f69 6e66 6f5b 2254 5846  .radio_info["TXF
+0001c0f0: 7265 7122 5d20 3d20 7666 6f5b 3a2d 315d  req"] = vfo[:-1]
+0001c100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c110: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0001c120: 662e 6e31 6d6d 2e72 6164 696f 5f69 6e66  f.n1mm.radio_inf
+0001c130: 6f5b 224d 6f64 6522 5d20 3d20 6d6f 6465  o["Mode"] = mode
+0001c140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c150: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0001c160: 662e 6e31 6d6d 2e72 6164 696f 5f69 6e66  f.n1mm.radio_inf
+0001c170: 6f5b 224f 7043 616c 6c22 5d20 3d20 7365  o["OpCall"] = se
+0001c180: 6c66 2e63 7572 7265 6e74 5f6f 700a 2020  lf.current_op.  
+0001c190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c1a0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+0001c1b0: 316d 6d2e 7261 6469 6f5f 696e 666f 5b22  1mm.radio_info["
+0001c1c0: 4973 5275 6e6e 696e 6722 5d20 3d20 7374  IsRunning"] = st
+0001c1d0: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
+0001c1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c1f0: 2020 2073 656c 662e 7072 6566 2e67 6574     self.pref.get
+0001c200: 2822 7275 6e5f 7374 6174 6522 2c20 4661  ("run_state", Fa
+0001c210: 6c73 6529 0a20 2020 2020 2020 2020 2020  lse).           
+0001c220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c230: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+0001c240: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001c250: 656c 662e 6e31 6d6d 2e73 656e 645f 7261  elf.n1mm.send_ra
+0001c260: 6469 6f28 290a 2020 2020 2020 2020 2020  dio().          
+0001c270: 2020 2020 2020 2020 2020 676c 6f62 616c            global
+0001c280: 7328 295b 0a20 2020 2020 2020 2020 2020  s()[.           
+0001c290: 2020 2020 2020 2020 2020 2020 2022 706f               "po
+0001c2a0: 6c6c 5f74 696d 6522 0a20 2020 2020 2020  ll_time".       
+0001c2b0: 2020 2020 2020 2020 2020 2020 205d 203d               ] =
+0001c2c0: 2064 6174 6574 696d 652e 6461 7465 7469   datetime.dateti
+0001c2d0: 6d65 2e6e 6f77 2829 202b 2064 6174 6574  me.now() + datet
+0001c2e0: 696d 652e 7469 6d65 6465 6c74 6128 7365  ime.timedelta(se
+0001c2f0: 636f 6e64 733d 3130 290a 0a20 2020 2064  conds=10)..    d
+0001c300: 6566 2065 6469 745f 6377 5f6d 6163 726f  ef edit_cw_macro
+0001c310: 7328 7365 6c66 2920 2d3e 204e 6f6e 653a  s(self) -> None:
+0001c320: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0001c330: 2020 2020 2043 616c 6c73 2074 6865 2064       Calls the d
+0001c340: 6566 6175 6c74 2074 6578 7420 6564 6974  efault text edit
+0001c350: 6f72 2074 6f20 6564 6974 2074 6865 2043  or to edit the C
+0001c360: 5720 6d61 6372 6f20 6669 6c65 2e0a 0a20  W macro file... 
+0001c370: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+0001c380: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+0001c390: 2d2d 2d2d 0a20 2020 2020 2020 204e 6f6e  ----.        Non
+0001c3a0: 650a 0a20 2020 2020 2020 2052 6574 7572  e..        Retur
+0001c3b0: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
+0001c3c0: 2d2d 0a20 2020 2020 2020 204e 6f6e 650a  --.        None.
+0001c3d0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0001c3e0: 2020 2020 6966 2073 656c 662e 7261 6469      if self.radi
+0001c3f0: 6f5f 7374 6174 652e 6765 7428 226d 6f64  o_state.get("mod
+0001c400: 6522 2920 3d3d 2022 4357 223a 0a20 2020  e") == "CW":.   
+0001c410: 2020 2020 2020 2020 206d 6163 726f 5f66           macro_f
+0001c420: 696c 6520 3d20 2263 776d 6163 726f 732e  ile = "cwmacros.
+0001c430: 7478 7422 0a20 2020 2020 2020 2065 6c73  txt".        els
+0001c440: 653a 0a20 2020 2020 2020 2020 2020 206d  e:.            m
+0001c450: 6163 726f 5f66 696c 6520 3d20 2273 7362  acro_file = "ssb
+0001c460: 6d61 6372 6f73 2e74 7874 220a 2020 2020  macros.txt".    
+0001c470: 2020 2020 6966 206e 6f74 2028 6673 7574      if not (fsut
+0001c480: 696c 732e 5553 4552 5f44 4154 415f 5041  ils.USER_DATA_PA
+0001c490: 5448 202f 206d 6163 726f 5f66 696c 6529  TH / macro_file)
+0001c4a0: 2e65 7869 7374 7328 293a 0a20 2020 2020  .exists():.     
+0001c4b0: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+0001c4c0: 6275 6728 2272 6561 645f 6377 5f6d 6163  bug("read_cw_mac
+0001c4d0: 726f 733a 2063 6f70 7969 6e67 2064 6566  ros: copying def
+0001c4e0: 6175 6c74 206d 6163 726f 2066 696c 652e  ault macro file.
+0001c4f0: 2229 0a20 2020 2020 2020 2020 2020 2063  ").            c
+0001c500: 6f70 7966 696c 6528 0a20 2020 2020 2020  opyfile(.       
+0001c510: 2020 2020 2020 2020 2066 7375 7469 6c73           fsutils
+0001c520: 2e41 5050 5f44 4154 415f 5041 5448 202f  .APP_DATA_PATH /
+0001c530: 206d 6163 726f 5f66 696c 652c 2066 7375   macro_file, fsu
+0001c540: 7469 6c73 2e55 5345 525f 4441 5441 5f50  tils.USER_DATA_P
+0001c550: 4154 4820 2f20 6d61 6372 6f5f 6669 6c65  ATH / macro_file
+0001c560: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+0001c570: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+0001c580: 2020 2020 2020 2020 6673 7574 696c 732e          fsutils.
+0001c590: 6f70 656e 4669 6c65 5769 7468 4f53 2866  openFileWithOS(f
+0001c5a0: 7375 7469 6c73 2e55 5345 525f 4441 5441  sutils.USER_DATA
+0001c5b0: 5f50 4154 4820 2f20 6d61 6372 6f5f 6669  _PATH / macro_fi
+0001c5c0: 6c65 290a 2020 2020 2020 2020 6578 6365  le).        exce
+0001c5d0: 7074 2046 696c 654e 6f74 466f 756e 6445  pt FileNotFoundE
+0001c5e0: 7272 6f72 207c 2050 6572 6d69 7373 696f  rror | Permissio
+0001c5f0: 6e45 7272 6f72 207c 204f 5345 7272 6f72  nError | OSError
+0001c600: 2061 7320 6572 723a 0a20 2020 2020 2020   as err:.       
+0001c610: 2020 2020 206c 6f67 6765 722e 6372 6974       logger.crit
+0001c620: 6963 616c 280a 2020 2020 2020 2020 2020  ical(.          
+0001c630: 2020 2020 2020 6622 436f 756c 6420 6e6f        f"Could no
+0001c640: 7420 6f70 656e 2066 696c 6520 7b66 7375  t open file {fsu
+0001c650: 7469 6c73 2e55 5345 525f 4441 5441 5f50  tils.USER_DATA_P
+0001c660: 4154 4820 2f20 6d61 6372 6f5f 6669 6c65  ATH / macro_file
+0001c670: 7d20 7b65 7272 7d22 0a20 2020 2020 2020  } {err}".       
+0001c680: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
+0001c690: 7265 6164 5f63 775f 6d61 6372 6f73 2873  read_cw_macros(s
+0001c6a0: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
+0001c6b0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0001c6c0: 2020 5265 6164 7320 696e 2074 6865 2043    Reads in the C
+0001c6d0: 5720 6d61 6372 6f73 2c20 6669 7273 7473  W macros, firsts
+0001c6e0: 2069 7420 6368 6563 6b73 2074 6f20 7365   it checks to se
+0001c6f0: 6520 6966 2074 6865 2066 696c 6520 6578  e if the file ex
+0001c700: 6973 7473 2e20 4966 2069 7420 646f 6573  ists. If it does
+0001c710: 206e 6f74 2c0a 2020 2020 2020 2020 616e   not,.        an
+0001c720: 6420 7468 6973 2068 6173 2062 6565 6e20  d this has been 
+0001c730: 7061 636b 6167 6564 2077 6974 6820 7079  packaged with py
+0001c740: 696e 7374 616c 6c65 7220 6974 2077 696c  installer it wil
+0001c750: 6c20 636f 7079 2074 6865 2064 6566 6175  l copy the defau
+0001c760: 6c74 2066 696c 6520 6672 6f6d 2074 6865  lt file from the
+0001c770: 0a20 2020 2020 2020 2074 656d 7020 6469  .        temp di
+0001c780: 7265 6374 6f72 7920 7468 6973 2069 7320  rectory this is 
+0001c790: 7275 6e6e 696e 6720 6672 6f6d 2e2e 2e20  running from... 
+0001c7a0: 496e 2074 6865 6f72 792e 0a20 2020 2020  In theory..     
+0001c7b0: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
+0001c7c0: 6966 2073 656c 662e 7261 6469 6f5f 7374  if self.radio_st
+0001c7d0: 6174 652e 6765 7428 226d 6f64 6522 2920  ate.get("mode") 
+0001c7e0: 3d3d 2022 4357 223a 0a20 2020 2020 2020  == "CW":.       
+0001c7f0: 2020 2020 206d 6163 726f 5f66 696c 6520       macro_file 
+0001c800: 3d20 2263 776d 6163 726f 732e 7478 7422  = "cwmacros.txt"
+0001c810: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+0001c820: 2020 2020 2020 2020 2020 206d 6163 726f             macro
+0001c830: 5f66 696c 6520 3d20 2273 7362 6d61 6372  _file = "ssbmacr
+0001c840: 6f73 2e74 7874 220a 0a20 2020 2020 2020  os.txt"..       
+0001c850: 2069 6620 6e6f 7420 2866 7375 7469 6c73   if not (fsutils
+0001c860: 2e55 5345 525f 4441 5441 5f50 4154 4820  .USER_DATA_PATH 
+0001c870: 2f20 6d61 6372 6f5f 6669 6c65 292e 6578  / macro_file).ex
+0001c880: 6973 7473 2829 3a0a 2020 2020 2020 2020  ists():.        
+0001c890: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+0001c8a0: 2822 7265 6164 5f63 775f 6d61 6372 6f73  ("read_cw_macros
+0001c8b0: 3a20 636f 7079 696e 6720 6465 6661 756c  : copying defaul
+0001c8c0: 7420 6d61 6372 6f20 6669 6c65 2e22 290a  t macro file.").
+0001c8d0: 2020 2020 2020 2020 2020 2020 636f 7079              copy
+0001c8e0: 6669 6c65 280a 2020 2020 2020 2020 2020  file(.          
+0001c8f0: 2020 2020 2020 6673 7574 696c 732e 4150        fsutils.AP
+0001c900: 505f 4441 5441 5f50 4154 4820 2f20 6d61  P_DATA_PATH / ma
+0001c910: 6372 6f5f 6669 6c65 2c20 6673 7574 696c  cro_file, fsutil
+0001c920: 732e 5553 4552 5f44 4154 415f 5041 5448  s.USER_DATA_PATH
+0001c930: 202f 206d 6163 726f 5f66 696c 650a 2020   / macro_file.  
+0001c940: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0001c950: 2020 2020 7769 7468 206f 7065 6e28 0a20      with open(. 
+0001c960: 2020 2020 2020 2020 2020 2066 7375 7469             fsuti
+0001c970: 6c73 2e55 5345 525f 4441 5441 5f50 4154  ls.USER_DATA_PAT
+0001c980: 4820 2f20 6d61 6372 6f5f 6669 6c65 2c20  H / macro_file, 
+0001c990: 2272 222c 2065 6e63 6f64 696e 673d 2275  "r", encoding="u
+0001c9a0: 7466 2d38 220a 2020 2020 2020 2020 2920  tf-8".        ) 
+0001c9b0: 6173 2066 696c 655f 6465 7363 7269 7074  as file_descript
+0001c9c0: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
+0001c9d0: 666f 7220 6c69 6e65 2069 6e20 6669 6c65  for line in file
+0001c9e0: 5f64 6573 6372 6970 746f 723a 0a20 2020  _descriptor:.   
+0001c9f0: 2020 2020 2020 2020 2020 2020 2074 7279               try
+0001ca00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001ca10: 2020 2020 2020 6d6f 6465 2c20 666b 6579        mode, fkey
+0001ca20: 2c20 6275 7474 6f6e 6e61 6d65 2c20 6377  , buttonname, cw
+0001ca30: 7465 7874 203d 206c 696e 652e 7370 6c69  text = line.spli
+0001ca40: 7428 227c 2229 0a20 2020 2020 2020 2020  t("|").         
+0001ca50: 2020 2020 2020 2020 2020 2069 6620 6d6f             if mo
+0001ca60: 6465 2e73 7472 6970 2829 2e75 7070 6572  de.strip().upper
+0001ca70: 2829 203d 3d20 2252 2220 616e 6420 7365  () == "R" and se
+0001ca80: 6c66 2e70 7265 662e 6765 7428 2272 756e  lf.pref.get("run
+0001ca90: 5f73 7461 7465 2229 3a0a 2020 2020 2020  _state"):.      
+0001caa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cab0: 2020 7365 6c66 2e66 6b65 7973 5b66 6b65    self.fkeys[fke
+0001cac0: 792e 7374 7269 7028 295d 203d 2028 6275  y.strip()] = (bu
+0001cad0: 7474 6f6e 6e61 6d65 2e73 7472 6970 2829  ttonname.strip()
+0001cae0: 2c20 6377 7465 7874 2e73 7472 6970 2829  , cwtext.strip()
+0001caf0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001cb00: 2020 2020 2020 6966 206d 6f64 652e 7374        if mode.st
+0001cb10: 7269 7028 292e 7570 7065 7228 2920 213d  rip().upper() !=
+0001cb20: 2022 5222 2061 6e64 206e 6f74 2073 656c   "R" and not sel
+0001cb30: 662e 7072 6566 2e67 6574 2822 7275 6e5f  f.pref.get("run_
+0001cb40: 7374 6174 6522 293a 0a20 2020 2020 2020  state"):.       
+0001cb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cb60: 2073 656c 662e 666b 6579 735b 666b 6579   self.fkeys[fkey
+0001cb70: 2e73 7472 6970 2829 5d20 3d20 2862 7574  .strip()] = (but
+0001cb80: 746f 6e6e 616d 652e 7374 7269 7028 292c  tonname.strip(),
+0001cb90: 2063 7774 6578 742e 7374 7269 7028 2929   cwtext.strip())
+0001cba0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001cbb0: 2065 7863 6570 7420 5661 6c75 6545 7272   except ValueErr
+0001cbc0: 6f72 2061 7320 6572 723a 0a20 2020 2020  or as err:.     
+0001cbd0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0001cbe0: 6f67 6765 722e 696e 666f 2822 7265 6164  ogger.info("read
+0001cbf0: 5f63 775f 6d61 6372 6f73 3a20 2573 222c  _cw_macros: %s",
+0001cc00: 2065 7272 290a 2020 2020 2020 2020 6b65   err).        ke
+0001cc10: 7973 203d 2073 656c 662e 666b 6579 732e  ys = self.fkeys.
+0001cc20: 6b65 7973 2829 0a20 2020 2020 2020 2069  keys().        i
+0001cc30: 6620 2246 3122 2069 6e20 6b65 7973 3a0a  f "F1" in keys:.
+0001cc40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001cc50: 2e46 312e 7365 7454 6578 7428 6622 4631  .F1.setText(f"F1
+0001cc60: 3a20 7b73 656c 662e 666b 6579 735b 2746  : {self.fkeys['F
+0001cc70: 3127 5d5b 305d 7d22 290a 2020 2020 2020  1'][0]}").      
+0001cc80: 2020 2020 2020 7365 6c66 2e46 312e 7365        self.F1.se
+0001cc90: 7454 6f6f 6c54 6970 2873 656c 662e 666b  tToolTip(self.fk
+0001cca0: 6579 735b 2246 3122 5d5b 315d 290a 2020  eys["F1"][1]).  
+0001ccb0: 2020 2020 2020 6966 2022 4632 2220 696e        if "F2" in
+0001ccc0: 206b 6579 733a 0a20 2020 2020 2020 2020   keys:.         
+0001ccd0: 2020 2073 656c 662e 4632 2e73 6574 5465     self.F2.setTe
+0001cce0: 7874 2866 2246 323a 207b 7365 6c66 2e66  xt(f"F2: {self.f
+0001ccf0: 6b65 7973 5b27 4632 275d 5b30 5d7d 2229  keys['F2'][0]}")
+0001cd00: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0001cd10: 662e 4632 2e73 6574 546f 6f6c 5469 7028  f.F2.setToolTip(
+0001cd20: 7365 6c66 2e66 6b65 7973 5b22 4632 225d  self.fkeys["F2"]
+0001cd30: 5b31 5d29 0a20 2020 2020 2020 2069 6620  [1]).        if 
+0001cd40: 2246 3322 2069 6e20 6b65 7973 3a0a 2020  "F3" in keys:.  
+0001cd50: 2020 2020 2020 2020 2020 7365 6c66 2e46            self.F
+0001cd60: 332e 7365 7454 6578 7428 6622 4633 3a20  3.setText(f"F3: 
+0001cd70: 7b73 656c 662e 666b 6579 735b 2746 3327  {self.fkeys['F3'
+0001cd80: 5d5b 305d 7d22 290a 2020 2020 2020 2020  ][0]}").        
+0001cd90: 2020 2020 7365 6c66 2e46 332e 7365 7454      self.F3.setT
+0001cda0: 6f6f 6c54 6970 2873 656c 662e 666b 6579  oolTip(self.fkey
+0001cdb0: 735b 2246 3322 5d5b 315d 290a 2020 2020  s["F3"][1]).    
+0001cdc0: 2020 2020 6966 2022 4634 2220 696e 206b      if "F4" in k
+0001cdd0: 6579 733a 0a20 2020 2020 2020 2020 2020  eys:.           
+0001cde0: 2073 656c 662e 4634 2e73 6574 5465 7874   self.F4.setText
+0001cdf0: 2866 2246 343a 207b 7365 6c66 2e66 6b65  (f"F4: {self.fke
+0001ce00: 7973 5b27 4634 275d 5b30 5d7d 2229 0a20  ys['F4'][0]}"). 
+0001ce10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0001ce20: 4634 2e73 6574 546f 6f6c 5469 7028 7365  F4.setToolTip(se
+0001ce30: 6c66 2e66 6b65 7973 5b22 4634 225d 5b31  lf.fkeys["F4"][1
+0001ce40: 5d29 0a20 2020 2020 2020 2069 6620 2246  ]).        if "F
+0001ce50: 3522 2069 6e20 6b65 7973 3a0a 2020 2020  5" in keys:.    
+0001ce60: 2020 2020 2020 2020 7365 6c66 2e46 352e          self.F5.
+0001ce70: 7365 7454 6578 7428 6622 4635 3a20 7b73  setText(f"F5: {s
+0001ce80: 656c 662e 666b 6579 735b 2746 3527 5d5b  elf.fkeys['F5'][
+0001ce90: 305d 7d22 290a 2020 2020 2020 2020 2020  0]}").          
+0001cea0: 2020 7365 6c66 2e46 352e 7365 7454 6f6f    self.F5.setToo
+0001ceb0: 6c54 6970 2873 656c 662e 666b 6579 735b  lTip(self.fkeys[
+0001cec0: 2246 3522 5d5b 315d 290a 2020 2020 2020  "F5"][1]).      
+0001ced0: 2020 6966 2022 4636 2220 696e 206b 6579    if "F6" in key
+0001cee0: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
+0001cef0: 656c 662e 4636 2e73 6574 5465 7874 2866  elf.F6.setText(f
+0001cf00: 2246 363a 207b 7365 6c66 2e66 6b65 7973  "F6: {self.fkeys
+0001cf10: 5b27 4636 275d 5b30 5d7d 2229 0a20 2020  ['F6'][0]}").   
+0001cf20: 2020 2020 2020 2020 2073 656c 662e 4636           self.F6
+0001cf30: 2e73 6574 546f 6f6c 5469 7028 7365 6c66  .setToolTip(self
+0001cf40: 2e66 6b65 7973 5b22 4636 225d 5b31 5d29  .fkeys["F6"][1])
+0001cf50: 0a20 2020 2020 2020 2069 6620 2246 3722  .        if "F7"
+0001cf60: 2069 6e20 6b65 7973 3a0a 2020 2020 2020   in keys:.      
+0001cf70: 2020 2020 2020 7365 6c66 2e46 372e 7365        self.F7.se
+0001cf80: 7454 6578 7428 6622 4637 3a20 7b73 656c  tText(f"F7: {sel
+0001cf90: 662e 666b 6579 735b 2746 3727 5d5b 305d  f.fkeys['F7'][0]
+0001cfa0: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
+0001cfb0: 7365 6c66 2e46 372e 7365 7454 6f6f 6c54  self.F7.setToolT
+0001cfc0: 6970 2873 656c 662e 666b 6579 735b 2246  ip(self.fkeys["F
+0001cfd0: 3722 5d5b 315d 290a 2020 2020 2020 2020  7"][1]).        
+0001cfe0: 6966 2022 4638 2220 696e 206b 6579 733a  if "F8" in keys:
+0001cff0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0001d000: 662e 4638 2e73 6574 5465 7874 2866 2246  f.F8.setText(f"F
+0001d010: 383a 207b 7365 6c66 2e66 6b65 7973 5b27  8: {self.fkeys['
+0001d020: 4638 275d 5b30 5d7d 2229 0a20 2020 2020  F8'][0]}").     
+0001d030: 2020 2020 2020 2073 656c 662e 4638 2e73         self.F8.s
+0001d040: 6574 546f 6f6c 5469 7028 7365 6c66 2e66  etToolTip(self.f
+0001d050: 6b65 7973 5b22 4638 225d 5b31 5d29 0a20  keys["F8"][1]). 
+0001d060: 2020 2020 2020 2069 6620 2246 3922 2069         if "F9" i
+0001d070: 6e20 6b65 7973 3a0a 2020 2020 2020 2020  n keys:.        
+0001d080: 2020 2020 7365 6c66 2e46 392e 7365 7454      self.F9.setT
+0001d090: 6578 7428 6622 4639 3a20 7b73 656c 662e  ext(f"F9: {self.
+0001d0a0: 666b 6579 735b 2746 3927 5d5b 305d 7d22  fkeys['F9'][0]}"
+0001d0b0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+0001d0c0: 6c66 2e46 392e 7365 7454 6f6f 6c54 6970  lf.F9.setToolTip
+0001d0d0: 2873 656c 662e 666b 6579 735b 2246 3922  (self.fkeys["F9"
+0001d0e0: 5d5b 315d 290a 2020 2020 2020 2020 6966  ][1]).        if
+0001d0f0: 2022 4631 3022 2069 6e20 6b65 7973 3a0a   "F10" in keys:.
+0001d100: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001d110: 2e46 3130 2e73 6574 5465 7874 2866 2246  .F10.setText(f"F
+0001d120: 3130 3a20 7b73 656c 662e 666b 6579 735b  10: {self.fkeys[
+0001d130: 2746 3130 275d 5b30 5d7d 2229 0a20 2020  'F10'][0]}").   
+0001d140: 2020 2020 2020 2020 2073 656c 662e 4631           self.F1
+0001d150: 302e 7365 7454 6f6f 6c54 6970 2873 656c  0.setToolTip(sel
+0001d160: 662e 666b 6579 735b 2246 3130 225d 5b31  f.fkeys["F10"][1
+0001d170: 5d29 0a20 2020 2020 2020 2069 6620 2246  ]).        if "F
+0001d180: 3131 2220 696e 206b 6579 733a 0a20 2020  11" in keys:.   
+0001d190: 2020 2020 2020 2020 2073 656c 662e 4631           self.F1
+0001d1a0: 312e 7365 7454 6578 7428 6622 4631 313a  1.setText(f"F11:
+0001d1b0: 207b 7365 6c66 2e66 6b65 7973 5b27 4631   {self.fkeys['F1
+0001d1c0: 3127 5d5b 305d 7d22 290a 2020 2020 2020  1'][0]}").      
+0001d1d0: 2020 2020 2020 7365 6c66 2e46 3131 2e73        self.F11.s
+0001d1e0: 6574 546f 6f6c 5469 7028 7365 6c66 2e66  etToolTip(self.f
+0001d1f0: 6b65 7973 5b22 4631 3122 5d5b 315d 290a  keys["F11"][1]).
+0001d200: 2020 2020 2020 2020 6966 2022 4631 3222          if "F12"
+0001d210: 2069 6e20 6b65 7973 3a0a 2020 2020 2020   in keys:.      
+0001d220: 2020 2020 2020 7365 6c66 2e46 3132 2e73        self.F12.s
+0001d230: 6574 5465 7874 2866 2246 3132 3a20 7b73  etText(f"F12: {s
+0001d240: 656c 662e 666b 6579 735b 2746 3132 275d  elf.fkeys['F12']
+0001d250: 5b30 5d7d 2229 0a20 2020 2020 2020 2020  [0]}").         
+0001d260: 2020 2073 656c 662e 4631 322e 7365 7454     self.F12.setT
+0001d270: 6f6f 6c54 6970 2873 656c 662e 666b 6579  oolTip(self.fkey
+0001d280: 735b 2246 3132 225d 5b31 5d29 0a0a 2020  s["F12"][1])..  
+0001d290: 2020 6465 6620 6765 6e65 7261 7465 5f61    def generate_a
+0001d2a0: 6469 6628 7365 6c66 2920 2d3e 204e 6f6e  dif(self) -> Non
+0001d2b0: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
+0001d2c0: 2020 2020 2020 2043 616c 6c73 2074 6865         Calls the
+0001d2d0: 2063 6f6e 7465 7374 2041 4449 4620 6669   contest ADIF fi
+0001d2e0: 6c65 2067 656e 6572 6174 6f72 2e0a 0a20  le generator... 
+0001d2f0: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+0001d300: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+0001d310: 2d2d 2d2d 0a20 2020 2020 2020 204e 6f6e  ----.        Non
+0001d320: 650a 0a20 2020 2020 2020 2052 6574 7572  e..        Retur
+0001d330: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
+0001d340: 2d2d 0a20 2020 2020 2020 204e 6f6e 650a  --.        None.
+0001d350: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
+0001d360: 2020 2020 2023 2068 7474 7073 3a2f 2f77       # https://w
+0001d370: 7777 2e61 6469 662e 6f72 672f 3331 352f  ww.adif.org/315/
+0001d380: 4144 4946 5f33 3135 2e68 746d 0a20 2020  ADIF_315.htm.   
+0001d390: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+0001d3a0: 6728 222a 2a2a 2a2a 2a41 4449 462a 2a2a  g("******ADIF***
+0001d3b0: 2a2a 2229 0a20 2020 2020 2020 2073 656c  **").        sel
+0001d3c0: 662e 636f 6e74 6573 742e 6164 6966 2873  f.contest.adif(s
+0001d3d0: 656c 6629 0a0a 2020 2020 6465 6620 6765  elf)..    def ge
+0001d3e0: 6e65 7261 7465 5f63 6162 7269 6c6c 6f28  nerate_cabrillo(
+0001d3f0: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
+0001d400: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0001d410: 2020 2043 616c 6c73 2074 6865 2063 6f6e     Calls the con
+0001d420: 7465 7374 2043 6162 7269 6c6c 6f20 6669  test Cabrillo fi
+0001d430: 6c65 2067 656e 6572 6174 6f72 2e20 4d61  le generator. Ma
+0001d440: 7962 652e 0a0a 2020 2020 2020 2020 5061  ybe...        Pa
+0001d450: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+0001d460: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+0001d470: 2020 2020 4e6f 6e65 0a0a 2020 2020 2020      None..      
+0001d480: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
+0001d490: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+0001d4a0: 2020 4e6f 6e65 0a20 2020 2020 2020 2022    None.        "
+0001d4b0: 2222 0a0a 2020 2020 2020 2020 6c6f 6767  ""..        logg
+0001d4c0: 6572 2e64 6562 7567 2822 2a2a 2a2a 2a2a  er.debug("******
+0001d4d0: 4361 6272 696c 6c6f 2a2a 2a2a 2a22 290a  Cabrillo*****").
+0001d4e0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+0001d4f0: 7465 7374 2e63 6162 7269 6c6c 6f28 7365  test.cabrillo(se
+0001d500: 6c66 290a 0a0a 6465 6620 6c6f 6164 5f66  lf)...def load_f
+0001d510: 6f6e 7473 5f66 726f 6d5f 6469 7228 6469  onts_from_dir(di
+0001d520: 7265 6374 6f72 793a 2073 7472 2920 2d3e  rectory: str) ->
+0001d530: 2073 6574 3a0a 2020 2020 2222 220a 2020   set:.    """.  
+0001d540: 2020 5765 6c6c 2069 7420 6c6f 6164 7320    Well it loads 
+0001d550: 666f 6e74 7320 6672 6f6d 2061 2064 6972  fonts from a dir
+0001d560: 6563 746f 7279 2e2e 2e0a 0a20 2020 2050  ectory.....    P
+0001d570: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
+0001d580: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064 6972  --------.    dir
+0001d590: 6563 746f 7279 203a 2073 7472 0a20 2020  ectory : str.   
+0001d5a0: 2054 6865 2064 6972 6563 746f 7279 2074   The directory t
+0001d5b0: 6f20 6c6f 6164 2066 6f6e 7473 2066 726f  o load fonts fro
+0001d5c0: 6d2e 0a0a 2020 2020 5265 7475 726e 730a  m...    Returns.
+0001d5d0: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+0001d5e0: 7365 740a 2020 2020 4120 7365 7420 6f66  set.    A set of
+0001d5f0: 2066 6f6e 7420 6661 6d69 6c69 6573 2069   font families i
+0001d600: 6e73 7461 6c6c 6564 2069 6e20 7468 6520  nstalled in the 
+0001d610: 6469 7265 6374 6f72 792e 0a20 2020 2022  directory..    "
+0001d620: 2222 0a20 2020 2066 6f6e 745f 6661 6d69  "".    font_fami
+0001d630: 6c69 6573 203d 2073 6574 2829 0a20 2020  lies = set().   
+0001d640: 2066 6f72 205f 6669 2069 6e20 5144 6972   for _fi in QDir
+0001d650: 2864 6972 6563 746f 7279 292e 656e 7472  (directory).entr
+0001d660: 7949 6e66 6f4c 6973 7428 5b22 2a2e 7474  yInfoList(["*.tt
+0001d670: 6622 2c20 222a 2e77 6f66 6622 2c20 222a  f", "*.woff", "*
+0001d680: 2e77 6f66 6632 225d 293a 0a20 2020 2020  .woff2"]):.     
+0001d690: 2020 205f 6964 203d 2051 466f 6e74 4461     _id = QFontDa
+0001d6a0: 7461 6261 7365 2e61 6464 4170 706c 6963  tabase.addApplic
+0001d6b0: 6174 696f 6e46 6f6e 7428 5f66 692e 6162  ationFont(_fi.ab
+0001d6c0: 736f 6c75 7465 4669 6c65 5061 7468 2829  soluteFilePath()
+0001d6d0: 290a 2020 2020 2020 2020 666f 6e74 5f66  ).        font_f
+0001d6e0: 616d 696c 6965 7320 7c3d 2073 6574 2851  amilies |= set(Q
+0001d6f0: 466f 6e74 4461 7461 6261 7365 2e61 7070  FontDatabase.app
+0001d700: 6c69 6361 7469 6f6e 466f 6e74 4661 6d69  licationFontFami
+0001d710: 6c69 6573 285f 6964 2929 0a20 2020 2072  lies(_id)).    r
+0001d720: 6574 7572 6e20 666f 6e74 5f66 616d 696c  eturn font_famil
+0001d730: 6965 730a 0a0a 6465 6620 696e 7374 616c  ies...def instal
+0001d740: 6c5f 6963 6f6e 7328 2920 2d3e 204e 6f6e  l_icons() -> Non
+0001d750: 653a 0a20 2020 2022 2222 496e 7374 616c  e:.    """Instal
+0001d760: 6c20 6963 6f6e 7322 2222 0a0a 2020 2020  l icons"""..    
+0001d770: 6966 2073 7973 2e70 6c61 7466 6f72 6d20  if sys.platform 
+0001d780: 3d3d 2022 6c69 6e75 7822 3a0a 2020 2020  == "linux":.    
+0001d790: 2020 2020 6f73 2e73 7973 7465 6d28 0a20      os.system(. 
+0001d7a0: 2020 2020 2020 2020 2020 2022 7864 672d             "xdg-
+0001d7b0: 6963 6f6e 2d72 6573 6f75 7263 6520 696e  icon-resource in
+0001d7c0: 7374 616c 6c20 2d2d 7369 7a65 2033 3220  stall --size 32 
+0001d7d0: 2d2d 636f 6e74 6578 7420 6170 7073 202d  --context apps -
+0001d7e0: 2d6d 6f64 6520 7573 6572 2022 0a20 2020  -mode user ".   
+0001d7f0: 2020 2020 2020 2020 2066 227b 6673 7574           f"{fsut
+0001d800: 696c 732e 4150 505f 4441 5441 5f50 4154  ils.APP_DATA_PAT
+0001d810: 487d 2f6b 3667 7465 2e6e 6f74 316d 6d2d  H}/k6gte.not1mm-
+0001d820: 3332 2e70 6e67 206b 3667 7465 2d6e 6f74  32.png k6gte-not
+0001d830: 316d 6d22 0a20 2020 2020 2020 2029 0a20  1mm".        ). 
+0001d840: 2020 2020 2020 206f 732e 7379 7374 656d         os.system
+0001d850: 280a 2020 2020 2020 2020 2020 2020 2278  (.            "x
+0001d860: 6467 2d69 636f 6e2d 7265 736f 7572 6365  dg-icon-resource
+0001d870: 2069 6e73 7461 6c6c 202d 2d73 697a 6520   install --size 
+0001d880: 3634 202d 2d63 6f6e 7465 7874 2061 7070  64 --context app
+0001d890: 7320 2d2d 6d6f 6465 2075 7365 7220 220a  s --mode user ".
+0001d8a0: 2020 2020 2020 2020 2020 2020 6622 7b66              f"{f
+0001d8b0: 7375 7469 6c73 2e41 5050 5f44 4154 415f  sutils.APP_DATA_
+0001d8c0: 5041 5448 7d2f 6b36 6774 652e 6e6f 7431  PATH}/k6gte.not1
+0001d8d0: 6d6d 2d36 342e 706e 6720 6b36 6774 652d  mm-64.png k6gte-
+0001d8e0: 6e6f 7431 6d6d 220a 2020 2020 2020 2020  not1mm".        
+0001d8f0: 290a 2020 2020 2020 2020 6f73 2e73 7973  ).        os.sys
+0001d900: 7465 6d28 0a20 2020 2020 2020 2020 2020  tem(.           
+0001d910: 2022 7864 672d 6963 6f6e 2d72 6573 6f75   "xdg-icon-resou
+0001d920: 7263 6520 696e 7374 616c 6c20 2d2d 7369  rce install --si
+0001d930: 7a65 2031 3238 202d 2d63 6f6e 7465 7874  ze 128 --context
+0001d940: 2061 7070 7320 2d2d 6d6f 6465 2075 7365   apps --mode use
+0001d950: 7220 220a 2020 2020 2020 2020 2020 2020  r ".            
+0001d960: 6622 7b66 7375 7469 6c73 2e41 5050 5f44  f"{fsutils.APP_D
+0001d970: 4154 415f 5041 5448 7d2f 6b36 6774 652e  ATA_PATH}/k6gte.
+0001d980: 6e6f 7431 6d6d 2d31 3238 2e70 6e67 206b  not1mm-128.png k
+0001d990: 3667 7465 2d6e 6f74 316d 6d22 0a20 2020  6gte-not1mm".   
+0001d9a0: 2020 2020 2029 0a20 2020 2020 2020 206f       ).        o
+0001d9b0: 732e 7379 7374 656d 280a 2020 2020 2020  s.system(.      
+0001d9c0: 2020 2020 2020 6622 7864 672d 6465 736b        f"xdg-desk
+0001d9d0: 746f 702d 6d65 6e75 2069 6e73 7461 6c6c  top-menu install
+0001d9e0: 207b 6673 7574 696c 732e 4150 505f 4441   {fsutils.APP_DA
+0001d9f0: 5441 5f50 4154 487d 2f6b 3667 7465 2d6e  TA_PATH}/k6gte-n
+0001da00: 6f74 316d 6d2e 6465 736b 746f 7022 0a20  ot1mm.desktop". 
+0001da10: 2020 2020 2020 2029 0a0a 0a64 6566 2064         )...def d
+0001da20: 6f69 6d70 286d 6f64 6e61 6d65 2920 2d3e  oimp(modname) ->
+0001da30: 206f 626a 6563 743a 0a20 2020 2022 2222   object:.    """
+0001da40: 0a20 2020 2049 6d70 6f72 7473 2061 206d  .    Imports a m
+0001da50: 6f64 756c 652e 0a0a 2020 2020 5061 7261  odule...    Para
+0001da60: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
+0001da70: 2d2d 2d2d 2d0a 2020 2020 6d6f 646e 616d  -----.    modnam
+0001da80: 6520 3a20 7374 720a 2020 2020 5468 6520  e : str.    The 
+0001da90: 6e61 6d65 206f 6620 7468 6520 6d6f 6475  name of the modu
+0001daa0: 6c65 2074 6f20 696d 706f 7274 2e0a 0a20  le to import... 
+0001dab0: 2020 2052 6574 7572 6e73 0a20 2020 202d     Returns.    -
+0001dac0: 2d2d 2d2d 2d2d 0a20 2020 206f 626a 6563  ------.    objec
+0001dad0: 740a 2020 2020 5468 6520 6d6f 6475 6c65  t.    The module
+0001dae0: 206f 626a 6563 742e 0a20 2020 2022 2222   object..    """
+0001daf0: 0a0a 2020 2020 6c6f 6767 6572 2e64 6562  ..    logger.deb
+0001db00: 7567 2822 646f 696d 703a 2025 7322 2c20  ug("doimp: %s", 
+0001db10: 6d6f 646e 616d 6529 0a20 2020 2072 6574  modname).    ret
+0001db20: 7572 6e20 696d 706f 7274 6c69 622e 696d  urn importlib.im
+0001db30: 706f 7274 5f6d 6f64 756c 6528 6622 6e6f  port_module(f"no
+0001db40: 7431 6d6d 2e70 6c75 6769 6e73 2e7b 6d6f  t1mm.plugins.{mo
+0001db50: 646e 616d 657d 2229 0a0a 0a64 6566 2072  dname}")...def r
+0001db60: 756e 2829 202d 3e20 4e6f 6e65 3a0a 2020  un() -> None:.  
+0001db70: 2020 2222 220a 2020 2020 4d61 696e 2045    """.    Main E
+0001db80: 6e74 7279 0a20 2020 2022 2222 0a20 2020  ntry.    """.   
+0001db90: 206c 6f67 6765 722e 6465 6275 6728 0a20   logger.debug(. 
+0001dba0: 2020 2020 2020 2066 2252 6573 6f6c 7665         f"Resolve
+0001dbb0: 6420 4f53 2066 696c 6520 7379 7374 656d  d OS file system
+0001dbc0: 2070 6174 6873 3a20 4d4f 4455 4c45 5f50   paths: MODULE_P
+0001dbd0: 4154 4820 7b66 7375 7469 6c73 2e4d 4f44  ATH {fsutils.MOD
+0001dbe0: 554c 455f 5041 5448 7d2c 2055 5345 525f  ULE_PATH}, USER_
+0001dbf0: 4441 5441 5f50 4154 4820 7b66 7375 7469  DATA_PATH {fsuti
+0001dc00: 6c73 2e55 5345 525f 4441 5441 5f50 4154  ls.USER_DATA_PAT
+0001dc10: 487d 2c20 434f 4e46 4947 5f50 4154 4820  H}, CONFIG_PATH 
+0001dc20: 7b66 7375 7469 6c73 2e43 4f4e 4649 475f  {fsutils.CONFIG_
+0001dc30: 5041 5448 7d22 0a20 2020 2029 0a20 2020  PATH}".    ).   
+0001dc40: 2069 6e73 7461 6c6c 5f69 636f 6e73 2829   install_icons()
+0001dc50: 0a20 2020 2074 696d 6572 2e73 7461 7274  .    timer.start
+0001dc60: 2832 3530 290a 2020 2020 7379 732e 6578  (250).    sys.ex
+0001dc70: 6974 2861 7070 2e65 7865 6328 2929 0a0a  it(app.exec())..
+0001dc80: 0a44 4542 5547 5f45 4e41 424c 4544 203d  .DEBUG_ENABLED =
+0001dc90: 2046 616c 7365 0a69 6620 5061 7468 2822   False.if Path("
+0001dca0: 2e2f 6465 6275 6722 292e 6578 6973 7473  ./debug").exists
+0001dcb0: 2829 3a0a 2020 2020 4445 4255 475f 454e  ():.    DEBUG_EN
+0001dcc0: 4142 4c45 4420 3d20 5472 7565 0a0a 6c6f  ABLED = True..lo
+0001dcd0: 6767 6572 203d 206c 6f67 6769 6e67 2e67  gger = logging.g
+0001dce0: 6574 4c6f 6767 6572 2822 5f5f 6d61 696e  etLogger("__main
+0001dcf0: 5f5f 2229 0a0a 6c6f 6767 696e 672e 6261  __")..logging.ba
+0001dd00: 7369 6343 6f6e 6669 6728 0a20 2020 206c  sicConfig(.    l
+0001dd10: 6576 656c 3d6c 6f67 6769 6e67 2e44 4542  evel=logging.DEB
+0001dd20: 5547 2069 6620 4445 4255 475f 454e 4142  UG if DEBUG_ENAB
+0001dd30: 4c45 4420 656c 7365 206c 6f67 6769 6e67  LED else logging
+0001dd40: 2e43 5249 5449 4341 4c2c 0a20 2020 2066  .CRITICAL,.    f
+0001dd50: 6f72 6d61 743d 225b 2528 6173 6374 696d  ormat="[%(asctim
+0001dd60: 6529 735d 2025 286c 6576 656c 6e61 6d65  e)s] %(levelname
+0001dd70: 2973 2025 286e 616d 6529 7320 2d20 2528  )s %(name)s - %(
+0001dd80: 6675 6e63 4e61 6d65 2973 204c 696e 6520  funcName)s Line 
+0001dd90: 2528 6c69 6e65 6e6f 2964 3a20 2528 6d65  %(lineno)d: %(me
+0001dda0: 7373 6167 6529 7322 2c0a 2020 2020 6861  ssage)s",.    ha
+0001ddb0: 6e64 6c65 7273 3d5b 0a20 2020 2020 2020  ndlers=[.       
+0001ddc0: 2052 6f74 6174 696e 6746 696c 6548 616e   RotatingFileHan
+0001ddd0: 646c 6572 2866 7375 7469 6c73 2e4c 4f47  dler(fsutils.LOG
+0001dde0: 5f46 494c 452c 206d 6178 4279 7465 733d  _FILE, maxBytes=
+0001ddf0: 3130 3439 3030 3030 2c20 6261 636b 7570  10490000, backup
+0001de00: 436f 756e 743d 3230 292c 0a20 2020 2020  Count=20),.     
+0001de10: 2020 206c 6f67 6769 6e67 2e53 7472 6561     logging.Strea
+0001de20: 6d48 616e 646c 6572 2829 2c0a 2020 2020  mHandler(),.    
+0001de30: 5d2c 0a29 0a6c 6f67 6769 6e67 2e67 6574  ],.).logging.get
+0001de40: 4c6f 6767 6572 2822 5079 5174 362e 7569  Logger("PyQt6.ui
+0001de50: 632e 7569 7061 7273 6572 2229 2e73 6574  c.uiparser").set
+0001de60: 4c65 7665 6c28 2249 4e46 4f22 290a 6c6f  Level("INFO").lo
+0001de70: 6767 696e 672e 6765 744c 6f67 6765 7228  gging.getLogger(
+0001de80: 2250 7951 7436 2e75 6963 2e70 726f 7065  "PyQt6.uic.prope
+0001de90: 7274 6965 7322 292e 7365 744c 6576 656c  rties").setLevel
+0001dea0: 2822 494e 464f 2229 0a61 7070 203d 2051  ("INFO").app = Q
+0001deb0: 7457 6964 6765 7473 2e51 4170 706c 6963  tWidgets.QApplic
+0001dec0: 6174 696f 6e28 7379 732e 6172 6776 290a  ation(sys.argv).
+0001ded0: 6661 6d69 6c69 6573 203d 206c 6f61 645f  families = load_
+0001dee0: 666f 6e74 735f 6672 6f6d 5f64 6972 286f  fonts_from_dir(o
+0001def0: 732e 6673 7061 7468 2866 7375 7469 6c73  s.fspath(fsutils
+0001df00: 2e41 5050 5f44 4154 415f 5041 5448 2929  .APP_DATA_PATH))
+0001df10: 0a6c 6f67 6765 722e 696e 666f 2866 2266  .logger.info(f"f
+0001df20: 6f6e 7420 6661 6d69 6c69 6573 207b 6661  ont families {fa
+0001df30: 6d69 6c69 6573 7d22 290a 7769 6e64 6f77  milies}").window
+0001df40: 203d 204d 6169 6e57 696e 646f 7728 290a   = MainWindow().
+0001df50: 6865 6967 6874 203d 2077 696e 646f 772e  height = window.
+0001df60: 7072 6566 2e67 6574 2822 7769 6e64 6f77  pref.get("window
+0001df70: 5f68 6569 6768 7422 2c20 3330 3029 0a77  _height", 300).w
+0001df80: 6964 7468 203d 2077 696e 646f 772e 7072  idth = window.pr
+0001df90: 6566 2e67 6574 2822 7769 6e64 6f77 5f77  ef.get("window_w
+0001dfa0: 6964 7468 222c 2037 3030 290a 7820 3d20  idth", 700).x = 
+0001dfb0: 7769 6e64 6f77 2e70 7265 662e 6765 7428  window.pref.get(
+0001dfc0: 2277 696e 646f 775f 7822 2c20 2d31 290a  "window_x", -1).
+0001dfd0: 7920 3d20 7769 6e64 6f77 2e70 7265 662e  y = window.pref.
+0001dfe0: 6765 7428 2277 696e 646f 775f 7922 2c20  get("window_y", 
+0001dff0: 2d31 290a 7769 6e64 6f77 2e73 6574 4765  -1).window.setGe
+0001e000: 6f6d 6574 7279 2878 2c20 792c 2077 6964  ometry(x, y, wid
+0001e010: 7468 2c20 6865 6967 6874 290a 7769 6e64  th, height).wind
+0001e020: 6f77 2e63 616c 6c73 6967 6e2e 7365 7446  ow.callsign.setF
+0001e030: 6f63 7573 2829 0a77 696e 646f 772e 7368  ocus().window.sh
+0001e040: 6f77 2829 0a74 696d 6572 203d 2051 7443  ow().timer = QtC
+0001e050: 6f72 652e 5154 696d 6572 2829 0a74 696d  ore.QTimer().tim
+0001e060: 6572 2e74 696d 656f 7574 2e63 6f6e 6e65  er.timeout.conne
+0001e070: 6374 2877 696e 646f 772e 706f 6c6c 5f72  ct(window.poll_r
+0001e080: 6164 696f 290a 0a69 6620 5f5f 6e61 6d65  adio)..if __name
+0001e090: 5f5f 203d 3d20 225f 5f6d 6169 6e5f 5f22  __ == "__main__"
+0001e0a0: 3a0a 2020 2020 7275 6e28 290a            :.    run().
```

### Comparing `not1mm-24.4.9.2/not1mm/bandmap.py` & `not1mm-24.4.9.3/not1mm/bandmap.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/checkwindow.py` & `not1mm-24.4.9.3/not1mm/checkwindow.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/JetBrainsMono-Regular.ttf` & `not1mm-24.4.9.3/not1mm/data/JetBrainsMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/MASTER.SCP` & `not1mm-24.4.9.3/not1mm/data/MASTER.SCP`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/about.ui` & `not1mm-24.4.9.3/not1mm/data/about.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/bandmap.ui` & `not1mm-24.4.9.3/not1mm/data/bandmap.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/checkwindow.ui` & `not1mm-24.4.9.3/not1mm/data/checkwindow.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/configuration.ui` & `not1mm-24.4.9.3/not1mm/data/configuration.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/contests.sql` & `not1mm-24.4.9.3/not1mm/data/contests.sql`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/cty.json` & `not1mm-24.4.9.3/not1mm/data/cty.json`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/editcontact.ui` & `not1mm-24.4.9.3/not1mm/data/editcontact.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/editmacro.ui` & `not1mm-24.4.9.3/not1mm/data/editmacro.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/k6gte.not1mm-128.png` & `not1mm-24.4.9.3/not1mm/data/k6gte.not1mm-128.png`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/k6gte.not1mm-32.png` & `not1mm-24.4.9.3/not1mm/data/k6gte.not1mm-32.png`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/k6gte.not1mm-64.png` & `not1mm-24.4.9.3/not1mm/data/k6gte.not1mm-64.png`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/logwindow.ui` & `not1mm-24.4.9.3/not1mm/data/logwindow.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/logwindowx.ui` & `not1mm-24.4.9.3/not1mm/data/logwindowx.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/main.ui` & `not1mm-24.4.9.3/not1mm/data/main.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/new_contest.ui` & `not1mm-24.4.9.3/not1mm/data/new_contest.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/not1mm.html` & `not1mm-24.4.9.3/not1mm/data/not1mm.html`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/opon.ui` & `not1mm-24.4.9.3/not1mm/data/opon.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/0.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/0.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/1.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/1.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/2.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/2.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/3.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/3.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/4.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/4.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/5.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/5.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/6.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/6.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/7.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/7.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/73.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/73.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/8.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/8.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/9.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/9.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/a.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/a.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/again.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/again.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/b.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/b.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/c.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/c.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/contest.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/contest.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/cq.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/cq.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/d.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/d.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/e.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/e.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/f.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/f.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/g.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/g.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/h.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/h.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/i.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/i.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/j.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/j.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/k.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/k.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/k6gte.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/k6gte.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/l.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/l.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/m.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/m.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/mynumber.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/mynumber.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/n.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/n.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/nil.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/nil.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/o.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/o.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/p.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/p.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/q.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/q.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/r.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/r.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/roger.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/roger.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/s.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/s.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/space.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/space.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/t.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/t.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/thankyou.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/thankyou.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/thankyouqrz.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/thankyouqrz.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/u.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/u.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/v.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/v.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/w.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/w.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/x.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/x.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/y.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/y.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/yourcall.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/yourcall.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/phonetics/z.wav` & `not1mm-24.4.9.3/not1mm/data/phonetics/z.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/pickcontest.ui` & `not1mm-24.4.9.3/not1mm/data/pickcontest.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/radio_green.png` & `not1mm-24.4.9.3/not1mm/data/radio_green.png`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/radio_grey.png` & `not1mm-24.4.9.3/not1mm/data/radio_grey.png`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/radio_red.png` & `not1mm-24.4.9.3/not1mm/data/radio_red.png`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/reddot.png` & `not1mm-24.4.9.3/not1mm/data/reddot.png`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/settings.ui` & `not1mm-24.4.9.3/not1mm/data/settings.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/data/vfo.ui` & `not1mm-24.4.9.3/not1mm/data/vfo.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/fsutils.py` & `not1mm-24.4.9.3/not1mm/fsutils.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/lib/cat_interface.py` & `not1mm-24.4.9.3/not1mm/lib/cat_interface.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/lib/cwinterface.py` & `not1mm-24.4.9.3/not1mm/lib/cwinterface.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/lib/database.py` & `not1mm-24.4.9.3/not1mm/lib/database.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/lib/edit_macro.py` & `not1mm-24.4.9.3/not1mm/lib/edit_macro.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/lib/edit_station.py` & `not1mm-24.4.9.3/not1mm/lib/edit_station.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/lib/ft8_watcher.py` & `not1mm-24.4.9.3/not1mm/lib/ft8_watcher.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/lib/ham_utility.py` & `not1mm-24.4.9.3/not1mm/lib/ham_utility.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/lib/lookup.py` & `not1mm-24.4.9.3/not1mm/lib/lookup.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/lib/multicast.py` & `not1mm-24.4.9.3/not1mm/lib/multicast.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/lib/n1mm.py` & `not1mm-24.4.9.3/not1mm/lib/n1mm.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/lib/new_contest.py` & `not1mm-24.4.9.3/not1mm/lib/new_contest.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/lib/plugin_common.py` & `not1mm-24.4.9.3/not1mm/lib/plugin_common.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/lib/settings.py` & `not1mm-24.4.9.3/not1mm/lib/settings.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/lib/super_check_partial.py` & `not1mm-24.4.9.3/not1mm/lib/super_check_partial.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/lib/versiontest.py` & `not1mm-24.4.9.3/not1mm/lib/versiontest.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/logwindow.py` & `not1mm-24.4.9.3/not1mm/logwindow.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/plugins/10_10_fall_cw.py` & `not1mm-24.4.9.3/not1mm/plugins/10_10_fall_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/plugins/10_10_spring_cw.py` & `not1mm-24.4.9.3/not1mm/plugins/10_10_spring_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/plugins/10_10_summer_phone.py` & `not1mm-24.4.9.3/not1mm/plugins/10_10_summer_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/plugins/10_10_winter_phone.py` & `not1mm-24.4.9.3/not1mm/plugins/10_10_winter_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/plugins/arrl_10m.py` & `not1mm-24.4.9.3/not1mm/plugins/arrl_10m.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/plugins/arrl_dx_cw.py` & `not1mm-24.4.9.3/not1mm/plugins/arrl_dx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/plugins/arrl_dx_ssb.py` & `not1mm-24.4.9.3/not1mm/plugins/arrl_dx_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/plugins/arrl_field_day.py` & `not1mm-24.4.9.3/not1mm/plugins/arrl_field_day.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/plugins/arrl_rtty_ru.py` & `not1mm-24.4.9.3/not1mm/plugins/arrl_rtty_ru.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/plugins/arrl_ss_cw.py` & `not1mm-24.4.9.3/not1mm/plugins/arrl_ss_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/plugins/arrl_ss_phone.py` & `not1mm-24.4.9.3/not1mm/plugins/arrl_ss_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/plugins/arrl_vhf_jan.py` & `not1mm-24.4.9.3/not1mm/plugins/arrl_vhf_jan.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/plugins/arrl_vhf_jun.py` & `not1mm-24.4.9.3/not1mm/plugins/arrl_vhf_jun.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/plugins/arrl_vhf_sep.py` & `not1mm-24.4.9.3/not1mm/plugins/arrl_vhf_sep.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/plugins/canada_day.py` & `not1mm-24.4.9.3/not1mm/plugins/canada_day.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/plugins/cq_160_cw.py` & `not1mm-24.4.9.3/not1mm/plugins/cq_160_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/plugins/cq_160_ssb.py` & `not1mm-24.4.9.3/not1mm/plugins/cq_160_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/plugins/cq_wpx_cw.py` & `not1mm-24.4.9.3/not1mm/plugins/cq_wpx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/plugins/cq_wpx_ssb.py` & `not1mm-24.4.9.3/not1mm/plugins/cq_wpx_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/plugins/cq_ww_cw.py` & `not1mm-24.4.9.3/not1mm/plugins/cq_ww_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/plugins/cq_ww_ssb.py` & `not1mm-24.4.9.3/not1mm/plugins/cq_ww_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/plugins/cwt.py` & `not1mm-24.4.9.3/not1mm/plugins/cwt.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/plugins/general_logging.py` & `not1mm-24.4.9.3/not1mm/plugins/general_logging.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/plugins/iaru_hf.py` & `not1mm-24.4.9.3/not1mm/plugins/iaru_hf.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/plugins/jidx_cw.py` & `not1mm-24.4.9.3/not1mm/plugins/jidx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/plugins/jidx_ph.py` & `not1mm-24.4.9.3/not1mm/plugins/jidx_ph.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/plugins/naqp_cw.py` & `not1mm-24.4.9.3/not1mm/plugins/naqp_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/plugins/naqp_ssb.py` & `not1mm-24.4.9.3/not1mm/plugins/naqp_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/plugins/phone_weekly_test.py` & `not1mm-24.4.9.3/not1mm/plugins/phone_weekly_test.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/plugins/stew_perry_topband.py` & `not1mm-24.4.9.3/not1mm/plugins/stew_perry_topband.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/plugins/winter_field_day.py` & `not1mm-24.4.9.3/not1mm/plugins/winter_field_day.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm/vfo.py` & `not1mm-24.4.9.3/not1mm/vfo.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/not1mm.egg-info/PKG-INFO` & `not1mm-24.4.9.3/not1mm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: not1mm
-Version: 24.4.9.2
+Version: 24.4.9.3
 Summary: NOT1MM Logger
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/not1mm
 Project-URL: Bug Tracker, https://github.com/mbridak/not1mm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -173,14 +173,15 @@
 - Phone Weekly Test
 - RAC Canada Day
 - Stew Perry Topband
 - Winter Field Day
 
 ## Recent Changes
 
+- [24-4-9-3] Ugh. It's not a real day unless you forget to test.
 - [24-4-9-2] Put back the floatable dock widgets, 'cause Wayland strikes again.
 - [24-4-9-1] Removed DockWidgetFloatable from the dock widgets since my wee brain can't figure out how to add a dragable window frame to them once they are floating. Added a minimum size for the VFO LCD digits. Defaulted bandmap window to the right.
 - [24-4-9] Fixed Checkwindow not showing calls from logged contacts.
 - [24-4-7] Added FT8Watcher class to prep for FT8 support.
 - [24-4-4-1] Made docking widgets open state persistent.
 - [24-4-4] Added per-contest echange hint when adding new contest.
 - [24-4-2] Migrated to PyQt6. I'm sure there are broken things.
```

### Comparing `not1mm-24.4.9.2/not1mm.egg-info/SOURCES.txt` & `not1mm-24.4.9.3/not1mm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.2/pyproject.toml` & `not1mm-24.4.9.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "not1mm" 
-version = "24.4.9.2"
+version = "24.4.9.3"
 description = "NOT1MM Logger"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
 dependencies = [
```
