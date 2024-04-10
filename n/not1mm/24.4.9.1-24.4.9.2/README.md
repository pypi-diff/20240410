# Comparing `tmp/not1mm-24.4.9.1.tar.gz` & `tmp/not1mm-24.4.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "not1mm-24.4.9.1.tar", last modified: Tue Apr  9 19:37:15 2024, max compression
+gzip compressed data, was "not1mm-24.4.9.2.tar", last modified: Wed Apr 10 00:24:43 2024, max compression
```

## Comparing `not1mm-24.4.9.1.tar` & `not1mm-24.4.9.2.tar`

### file list

```diff
@@ -1,159 +1,159 @@
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-09 19:37:15.391234 not1mm-24.4.9.1/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/LICENSE
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    27070 2024-04-09 19:37:15.390234 not1mm-24.4.9.1/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    25997 2024-04-09 19:35:24.000000 not1mm-24.4.9.1/README.md
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-09 19:37:15.200231 not1mm-24.4.9.1/not1mm/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   123101 2024-04-09 19:25:19.000000 not1mm-24.4.9.1/not1mm/__main__.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    34256 2024-04-09 19:20:10.000000 not1mm-24.4.9.1/not1mm/bandmap.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10403 2024-04-09 19:20:33.000000 not1mm-24.4.9.1/not1mm/checkwindow.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-09 19:37:15.262232 not1mm-24.4.9.1/not1mm/data/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/JetBrainsMono-Regular.ttf
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   366478 2024-04-02 17:57:36.000000 not1mm-24.4.9.1/not1mm/data/MASTER.SCP
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2067 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/about.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      224 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/alpha bravo charlie delta.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7125 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/bandmap.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      387 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/check.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4614 2024-04-09 18:40:45.000000 not1mm-24.4.9.1/not1mm/data/checkwindow.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51643 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/configuration.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    89307 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/contests.sql
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)  4790698 2024-04-02 16:11:52.000000 not1mm-24.4.9.1/not1mm/data/cty.json
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      451 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/cwmacros.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      116 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/donors.html
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    27404 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/editcontact.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2689 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/editmacro.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      474 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/greendot.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/k6gte-not1mm.desktop
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6076 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/k6gte.not1mm-128.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1526 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/k6gte.not1mm-32.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2925 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/k6gte.not1mm-64.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1436 2024-04-01 23:54:49.000000 not1mm-24.4.9.1/not1mm/data/logwindow.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1610 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/logwindowx.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54341 2024-04-04 21:22:08.000000 not1mm-24.4.9.1/not1mm/data/main.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    21823 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/new_contest.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    23273 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/not1mm.html
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2247 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/opon.ui
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-09 19:37:15.324233 not1mm-24.4.9.1/not1mm/data/phonetics/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42590 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/0.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30248 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/1.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29584 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/2.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32072 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/3.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43052 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/4.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51976 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/5.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58634 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/6.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49154 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/7.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32842 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/73.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35636 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/8.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39592 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/9.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46800 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/a.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44594 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/again.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40976 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/b.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46746 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/c.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    62558 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/contest.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    92498 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/cq.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52524 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/d.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    45700 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/e.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    53438 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/f.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42766 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/g.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50040 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/h.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46372 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/i.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43434 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/j.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49066 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/k.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   185562 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/k6gte.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43154 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/l.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54352 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/m.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56798 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/mynumber.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52204 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/n.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   154544 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/nil.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47440 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/o.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    38300 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/p.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    55288 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/q.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47432 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/r.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46122 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/roger.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    60698 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/s.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    70424 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/space.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58196 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/t.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56320 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/thankyou.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    94980 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/thankyouqrz.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    65922 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/u.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50142 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/v.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    37638 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/w.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    61870 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/x.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56524 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/y.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46510 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/yourcall.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51768 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/phonetics/z.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1600 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/pickcontest.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1234 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/radio_green.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1258 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/radio_grey.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      957 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/radio_red.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/reddot.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40028 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/settings.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      470 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/data/ssbmacros.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2054 2024-04-09 19:27:50.000000 not1mm-24.4.9.1/not1mm/data/vfo.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1652 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/fsutils.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-09 19:37:15.348234 not1mm-24.4.9.1/not1mm/lib/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/lib/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      416 2024-04-02 16:43:54.000000 not1mm-24.4.9.1/not1mm/lib/about.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15127 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/lib/cat_interface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3126 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/lib/cwinterface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42480 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/lib/database.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      353 2024-04-02 16:43:38.000000 not1mm-24.4.9.1/not1mm/lib/edit_contact.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      517 2024-04-02 16:43:30.000000 not1mm-24.4.9.1/not1mm/lib/edit_macro.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      359 2024-04-02 16:43:21.000000 not1mm-24.4.9.1/not1mm/lib/edit_opon.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1965 2024-04-02 16:43:09.000000 not1mm-24.4.9.1/not1mm/lib/edit_station.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4220 2024-04-08 02:01:24.000000 not1mm-24.4.9.1/not1mm/lib/ft8_watcher.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10978 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/lib/ham_utility.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13952 2024-04-03 03:28:34.000000 not1mm-24.4.9.1/not1mm/lib/lookup.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3249 2024-04-02 17:02:22.000000 not1mm-24.4.9.1/not1mm/lib/multicast.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5712 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/lib/n1mm.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      816 2024-04-04 17:56:24.000000 not1mm-24.4.9.1/not1mm/lib/new_contest.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8605 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/lib/plugin_common.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      359 2024-04-02 16:41:42.000000 not1mm-24.4.9.1/not1mm/lib/select_contest.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8877 2024-04-02 16:41:49.000000 not1mm-24.4.9.1/not1mm/lib/settings.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2334 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/lib/super_check_partial.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       49 2024-04-09 19:35:58.000000 not1mm-24.4.9.1/not1mm/lib/version.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1286 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/lib/versiontest.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    44838 2024-04-09 19:20:52.000000 not1mm-24.4.9.1/not1mm/logwindow.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-09 19:37:15.385234 not1mm-24.4.9.1/not1mm/plugins/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10873 2024-04-04 18:50:36.000000 not1mm-24.4.9.1/not1mm/plugins/10_10_fall_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10878 2024-04-04 18:58:51.000000 not1mm-24.4.9.1/not1mm/plugins/10_10_spring_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10887 2024-04-04 18:58:54.000000 not1mm-24.4.9.1/not1mm/plugins/10_10_summer_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10890 2024-04-04 18:58:56.000000 not1mm-24.4.9.1/not1mm/plugins/10_10_winter_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2024-03-31 16:17:00.000000 not1mm-24.4.9.1/not1mm/plugins/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13677 2024-04-04 19:07:30.000000 not1mm-24.4.9.1/not1mm/plugins/arrl_10m.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13722 2024-04-04 19:09:51.000000 not1mm-24.4.9.1/not1mm/plugins/arrl_dx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13725 2024-04-04 19:10:06.000000 not1mm-24.4.9.1/not1mm/plugins/arrl_dx_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10052 2024-04-04 18:11:53.000000 not1mm-24.4.9.1/not1mm/plugins/arrl_field_day.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7994 2024-04-04 19:10:45.000000 not1mm-24.4.9.1/not1mm/plugins/arrl_rtty_ru.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12989 2024-04-04 20:51:30.000000 not1mm-24.4.9.1/not1mm/plugins/arrl_ss_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12977 2024-04-04 20:53:34.000000 not1mm-24.4.9.1/not1mm/plugins/arrl_ss_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12481 2024-04-04 19:17:41.000000 not1mm-24.4.9.1/not1mm/plugins/arrl_vhf_jan.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11500 2024-04-04 19:18:17.000000 not1mm-24.4.9.1/not1mm/plugins/arrl_vhf_jun.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11500 2024-04-04 19:18:29.000000 not1mm-24.4.9.1/not1mm/plugins/arrl_vhf_sep.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11907 2024-04-04 19:23:16.000000 not1mm-24.4.9.1/not1mm/plugins/canada_day.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14059 2024-04-04 19:27:40.000000 not1mm-24.4.9.1/not1mm/plugins/cq_160_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14102 2024-04-04 19:27:52.000000 not1mm-24.4.9.1/not1mm/plugins/cq_160_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12399 2024-04-04 19:29:11.000000 not1mm-24.4.9.1/not1mm/plugins/cq_wpx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12487 2024-04-04 19:29:08.000000 not1mm-24.4.9.1/not1mm/plugins/cq_wpx_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11114 2024-04-04 19:31:31.000000 not1mm-24.4.9.1/not1mm/plugins/cq_ww_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11119 2024-04-04 19:31:27.000000 not1mm-24.4.9.1/not1mm/plugins/cq_ww_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12020 2024-04-04 19:46:16.000000 not1mm-24.4.9.1/not1mm/plugins/cwt.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3387 2024-04-04 17:53:54.000000 not1mm-24.4.9.1/not1mm/plugins/general_logging.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11461 2024-04-04 19:46:13.000000 not1mm-24.4.9.1/not1mm/plugins/iaru_hf.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11090 2024-04-04 19:47:46.000000 not1mm-24.4.9.1/not1mm/plugins/jidx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11092 2024-04-04 19:47:59.000000 not1mm-24.4.9.1/not1mm/plugins/jidx_ph.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11510 2024-04-04 19:50:33.000000 not1mm-24.4.9.1/not1mm/plugins/naqp_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11515 2024-04-04 19:50:44.000000 not1mm-24.4.9.1/not1mm/plugins/naqp_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12316 2024-04-04 19:51:26.000000 not1mm-24.4.9.1/not1mm/plugins/phone_weekly_test.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10588 2024-04-04 19:52:18.000000 not1mm-24.4.9.1/not1mm/plugins/stew_perry_topband.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10238 2024-04-04 18:05:44.000000 not1mm-24.4.9.1/not1mm/plugins/winter_field_day.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12405 2024-04-09 19:18:40.000000 not1mm-24.4.9.1/not1mm/vfo.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-09 19:37:15.389234 not1mm-24.4.9.1/not1mm.egg-info/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    27070 2024-04-09 19:37:15.000000 not1mm-24.4.9.1/not1mm.egg-info/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4105 2024-04-09 19:37:15.000000 not1mm-24.4.9.1/not1mm.egg-info/SOURCES.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2024-04-09 19:37:15.000000 not1mm-24.4.9.1/not1mm.egg-info/dependency_links.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2024-04-09 19:37:15.000000 not1mm-24.4.9.1/not1mm.egg-info/entry_points.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      131 2024-04-09 19:37:15.000000 not1mm-24.4.9.1/not1mm.egg-info/requires.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       25 2024-04-09 19:37:15.000000 not1mm-24.4.9.1/not1mm.egg-info/top_level.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1427 2024-04-09 19:35:40.000000 not1mm-24.4.9.1/pyproject.toml
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2024-04-09 19:37:15.391234 not1mm-24.4.9.1/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-10 00:24:43.979837 not1mm-24.4.9.2/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/LICENSE
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    27150 2024-04-10 00:24:43.975837 not1mm-24.4.9.2/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    26077 2024-04-09 23:24:41.000000 not1mm-24.4.9.2/README.md
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-10 00:24:43.645831 not1mm-24.4.9.2/not1mm/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   123101 2024-04-09 22:52:19.000000 not1mm-24.4.9.2/not1mm/__main__.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    34021 2024-04-09 23:22:19.000000 not1mm-24.4.9.2/not1mm/bandmap.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10168 2024-04-09 23:22:21.000000 not1mm-24.4.9.2/not1mm/checkwindow.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-10 00:24:43.745833 not1mm-24.4.9.2/not1mm/data/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/JetBrainsMono-Regular.ttf
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   366478 2024-04-02 17:57:36.000000 not1mm-24.4.9.2/not1mm/data/MASTER.SCP
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2067 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/about.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      224 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/alpha bravo charlie delta.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7125 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/bandmap.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      387 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/check.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4614 2024-04-09 18:40:45.000000 not1mm-24.4.9.2/not1mm/data/checkwindow.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51643 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/configuration.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    89307 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/contests.sql
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)  4790698 2024-04-02 16:11:52.000000 not1mm-24.4.9.2/not1mm/data/cty.json
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      451 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/cwmacros.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      116 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/donors.html
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    27404 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/editcontact.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2689 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/editmacro.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      474 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/greendot.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/k6gte-not1mm.desktop
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6076 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/k6gte.not1mm-128.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1526 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/k6gte.not1mm-32.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2925 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/k6gte.not1mm-64.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1436 2024-04-01 23:54:49.000000 not1mm-24.4.9.2/not1mm/data/logwindow.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1610 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/logwindowx.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54341 2024-04-04 21:22:08.000000 not1mm-24.4.9.2/not1mm/data/main.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    21823 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/new_contest.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    23273 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/not1mm.html
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2247 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/opon.ui
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-10 00:24:43.842835 not1mm-24.4.9.2/not1mm/data/phonetics/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42590 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/0.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30248 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/1.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29584 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/2.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32072 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/3.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43052 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/4.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51976 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/5.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58634 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/6.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49154 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/7.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32842 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/73.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35636 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/8.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39592 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/9.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46800 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/a.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44594 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/again.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40976 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/b.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46746 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/c.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    62558 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/contest.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    92498 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/cq.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52524 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/d.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    45700 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/e.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    53438 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/f.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42766 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/g.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50040 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/h.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46372 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/i.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43434 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/j.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49066 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/k.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   185562 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/k6gte.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43154 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/l.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54352 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/m.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56798 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/mynumber.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52204 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/n.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   154544 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/nil.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47440 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/o.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    38300 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/p.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    55288 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/q.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47432 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/r.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46122 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/roger.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    60698 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/s.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    70424 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/space.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58196 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/t.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56320 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/thankyou.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    94980 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/thankyouqrz.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    65922 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/u.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50142 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/v.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    37638 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/w.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    61870 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/x.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56524 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/y.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46510 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/yourcall.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51768 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/phonetics/z.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1600 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/pickcontest.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1234 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/radio_green.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1258 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/radio_grey.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      957 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/radio_red.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/reddot.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40028 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/settings.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      470 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/data/ssbmacros.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2054 2024-04-09 22:51:54.000000 not1mm-24.4.9.2/not1mm/data/vfo.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1652 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/fsutils.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-10 00:24:43.878835 not1mm-24.4.9.2/not1mm/lib/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/lib/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      416 2024-04-02 16:43:54.000000 not1mm-24.4.9.2/not1mm/lib/about.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15127 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/lib/cat_interface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3126 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/lib/cwinterface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42480 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/lib/database.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      353 2024-04-02 16:43:38.000000 not1mm-24.4.9.2/not1mm/lib/edit_contact.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      517 2024-04-02 16:43:30.000000 not1mm-24.4.9.2/not1mm/lib/edit_macro.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      359 2024-04-02 16:43:21.000000 not1mm-24.4.9.2/not1mm/lib/edit_opon.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1965 2024-04-02 16:43:09.000000 not1mm-24.4.9.2/not1mm/lib/edit_station.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4220 2024-04-08 02:01:24.000000 not1mm-24.4.9.2/not1mm/lib/ft8_watcher.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10978 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/lib/ham_utility.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13952 2024-04-03 03:28:34.000000 not1mm-24.4.9.2/not1mm/lib/lookup.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3249 2024-04-02 17:02:22.000000 not1mm-24.4.9.2/not1mm/lib/multicast.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5712 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/lib/n1mm.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      816 2024-04-04 17:56:24.000000 not1mm-24.4.9.2/not1mm/lib/new_contest.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8605 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/lib/plugin_common.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      359 2024-04-02 16:41:42.000000 not1mm-24.4.9.2/not1mm/lib/select_contest.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8877 2024-04-02 16:41:49.000000 not1mm-24.4.9.2/not1mm/lib/settings.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2334 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/lib/super_check_partial.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       49 2024-04-09 23:23:17.000000 not1mm-24.4.9.2/not1mm/lib/version.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1286 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/lib/versiontest.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    44603 2024-04-09 23:22:17.000000 not1mm-24.4.9.2/not1mm/logwindow.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-10 00:24:43.970837 not1mm-24.4.9.2/not1mm/plugins/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10873 2024-04-04 18:50:36.000000 not1mm-24.4.9.2/not1mm/plugins/10_10_fall_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10878 2024-04-04 18:58:51.000000 not1mm-24.4.9.2/not1mm/plugins/10_10_spring_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10887 2024-04-04 18:58:54.000000 not1mm-24.4.9.2/not1mm/plugins/10_10_summer_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10890 2024-04-04 18:58:56.000000 not1mm-24.4.9.2/not1mm/plugins/10_10_winter_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2024-03-31 16:17:00.000000 not1mm-24.4.9.2/not1mm/plugins/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13677 2024-04-04 19:07:30.000000 not1mm-24.4.9.2/not1mm/plugins/arrl_10m.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13722 2024-04-04 19:09:51.000000 not1mm-24.4.9.2/not1mm/plugins/arrl_dx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13725 2024-04-04 19:10:06.000000 not1mm-24.4.9.2/not1mm/plugins/arrl_dx_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10052 2024-04-04 18:11:53.000000 not1mm-24.4.9.2/not1mm/plugins/arrl_field_day.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7994 2024-04-04 19:10:45.000000 not1mm-24.4.9.2/not1mm/plugins/arrl_rtty_ru.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12989 2024-04-04 20:51:30.000000 not1mm-24.4.9.2/not1mm/plugins/arrl_ss_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12977 2024-04-04 20:53:34.000000 not1mm-24.4.9.2/not1mm/plugins/arrl_ss_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12481 2024-04-04 19:17:41.000000 not1mm-24.4.9.2/not1mm/plugins/arrl_vhf_jan.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11500 2024-04-04 19:18:17.000000 not1mm-24.4.9.2/not1mm/plugins/arrl_vhf_jun.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11500 2024-04-04 19:18:29.000000 not1mm-24.4.9.2/not1mm/plugins/arrl_vhf_sep.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11907 2024-04-04 19:23:16.000000 not1mm-24.4.9.2/not1mm/plugins/canada_day.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14059 2024-04-04 19:27:40.000000 not1mm-24.4.9.2/not1mm/plugins/cq_160_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14102 2024-04-04 19:27:52.000000 not1mm-24.4.9.2/not1mm/plugins/cq_160_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12399 2024-04-04 19:29:11.000000 not1mm-24.4.9.2/not1mm/plugins/cq_wpx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12487 2024-04-04 19:29:08.000000 not1mm-24.4.9.2/not1mm/plugins/cq_wpx_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11114 2024-04-04 19:31:31.000000 not1mm-24.4.9.2/not1mm/plugins/cq_ww_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11119 2024-04-04 19:31:27.000000 not1mm-24.4.9.2/not1mm/plugins/cq_ww_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12020 2024-04-04 19:46:16.000000 not1mm-24.4.9.2/not1mm/plugins/cwt.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3387 2024-04-04 17:53:54.000000 not1mm-24.4.9.2/not1mm/plugins/general_logging.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11461 2024-04-04 19:46:13.000000 not1mm-24.4.9.2/not1mm/plugins/iaru_hf.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11090 2024-04-04 19:47:46.000000 not1mm-24.4.9.2/not1mm/plugins/jidx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11092 2024-04-04 19:47:59.000000 not1mm-24.4.9.2/not1mm/plugins/jidx_ph.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11510 2024-04-04 19:50:33.000000 not1mm-24.4.9.2/not1mm/plugins/naqp_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11515 2024-04-04 19:50:44.000000 not1mm-24.4.9.2/not1mm/plugins/naqp_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12316 2024-04-04 19:51:26.000000 not1mm-24.4.9.2/not1mm/plugins/phone_weekly_test.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10588 2024-04-04 19:52:18.000000 not1mm-24.4.9.2/not1mm/plugins/stew_perry_topband.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10238 2024-04-04 18:05:44.000000 not1mm-24.4.9.2/not1mm/plugins/winter_field_day.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12169 2024-04-09 23:22:14.000000 not1mm-24.4.9.2/not1mm/vfo.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-04-10 00:24:43.973837 not1mm-24.4.9.2/not1mm.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    27150 2024-04-10 00:24:43.000000 not1mm-24.4.9.2/not1mm.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4105 2024-04-10 00:24:43.000000 not1mm-24.4.9.2/not1mm.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2024-04-10 00:24:43.000000 not1mm-24.4.9.2/not1mm.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2024-04-10 00:24:43.000000 not1mm-24.4.9.2/not1mm.egg-info/entry_points.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      131 2024-04-10 00:24:43.000000 not1mm-24.4.9.2/not1mm.egg-info/requires.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       25 2024-04-10 00:24:43.000000 not1mm-24.4.9.2/not1mm.egg-info/top_level.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1427 2024-04-09 23:23:27.000000 not1mm-24.4.9.2/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2024-04-10 00:24:43.979837 not1mm-24.4.9.2/setup.cfg
```

### Comparing `not1mm-24.4.9.1/LICENSE` & `not1mm-24.4.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/PKG-INFO` & `not1mm-24.4.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: not1mm
-Version: 24.4.9.1
+Version: 24.4.9.2
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
 
+- [24-4-9-2] Put back the floatable dock widgets, 'cause Wayland strikes again.
 - [24-4-9-1] Removed DockWidgetFloatable from the dock widgets since my wee brain can't figure out how to add a dragable window frame to them once they are floating. Added a minimum size for the VFO LCD digits. Defaulted bandmap window to the right.
 - [24-4-9] Fixed Checkwindow not showing calls from logged contacts.
 - [24-4-7] Added FT8Watcher class to prep for FT8 support.
 - [24-4-4-1] Made docking widgets open state persistent.
 - [24-4-4] Added per-contest echange hint when adding new contest.
 - [24-4-2] Migrated to PyQt6. I'm sure there are broken things.
 - [24-4-1-2] Added color text indicators to the Check Partial window. Poached the code from @kyleboyle. Thanks! Fixed the Log, VFO and Check Partial windows to be actual docking widgets. Refocus call field after double clicking on item in the check partial window.
```

### Comparing `not1mm-24.4.9.1/README.md` & `not1mm-24.4.9.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -141,14 +141,15 @@
 - Phone Weekly Test
 - RAC Canada Day
 - Stew Perry Topband
 - Winter Field Day
 
 ## Recent Changes
 
+- [24-4-9-2] Put back the floatable dock widgets, 'cause Wayland strikes again.
 - [24-4-9-1] Removed DockWidgetFloatable from the dock widgets since my wee brain can't figure out how to add a dragable window frame to them once they are floating. Added a minimum size for the VFO LCD digits. Defaulted bandmap window to the right.
 - [24-4-9] Fixed Checkwindow not showing calls from logged contacts.
 - [24-4-7] Added FT8Watcher class to prep for FT8 support.
 - [24-4-4-1] Made docking widgets open state persistent.
 - [24-4-4] Added per-contest echange hint when adding new contest.
 - [24-4-2] Migrated to PyQt6. I'm sure there are broken things.
 - [24-4-1-2] Added color text indicators to the Check Partial window. Poached the code from @kyleboyle. Thanks! Fixed the Log, VFO and Check Partial windows to be actual docking widgets. Refocus call field after double clicking on item in the check partial window.
```

### Comparing `not1mm-24.4.9.1/not1mm/__main__.py` & `not1mm-24.4.9.2/not1mm/__main__.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/bandmap.py` & `not1mm-24.4.9.2/not1mm/bandmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,19 +322,14 @@
     text_color = QtGui.QColor(45, 45, 45)
 
     def __init__(self):
         super().__init__()
         self._udpwatch = None
 
         uic.loadUi(fsutils.APP_DATA_PATH / "bandmap.ui", self)
-        self.setFeatures(
-            QDockWidget.DockWidgetFeature.DockWidgetMovable
-            | QDockWidget.DockWidgetFeature.DockWidgetClosable
-        )
-        # self.setAllowedAreas(QtCore.Qt.DockWidgetArea.AllDockWidgetAreas)
         self.settings = self.get_settings()
         self.agetime = self.clear_spot_olderSpinBox.value()
         self.clear_spot_olderSpinBox.valueChanged.connect(self.spot_aging_changed)
         self.clearButton.clicked.connect(self.clear_spots)
         self.zoominButton.clicked.connect(self.dec_zoom)
         self.zoomoutButton.clicked.connect(self.inc_zoom)
         self.connectButton.clicked.connect(self.connect)
```

### Comparing `not1mm-24.4.9.1/not1mm/checkwindow.py` & `not1mm-24.4.9.2/not1mm/checkwindow.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,19 +46,14 @@
         self.dbname = fsutils.USER_DATA_PATH / self.pref.get(
             "current_database", "ham.db"
         )
         self.database = DataBase(self.dbname, fsutils.APP_DATA_PATH)
         self.database.current_contest = self.pref.get("contest", 0)
 
         uic.loadUi(fsutils.APP_DATA_PATH / "checkwindow.ui", self)
-        self.setFeatures(
-            QDockWidget.DockWidgetFeature.DockWidgetMovable
-            | QDockWidget.DockWidgetFeature.DockWidgetClosable
-        )
-        # self.setAllowedAreas(QtCore.Qt.DockWidgetArea.AllDockWidgetAreas)
         self.mscp = SCP(fsutils.APP_DATA_PATH)
         self._udpwatch = None
         self.udp_fifo = queue.Queue()
         self.multicast_interface = Multicast(
             self.pref.get("multicast_group", "239.1.1.1"),
             self.pref.get("multicast_port", 2239),
             self.pref.get("interface_ip", "0.0.0.0"),
```

### Comparing `not1mm-24.4.9.1/not1mm/data/JetBrainsMono-Regular.ttf` & `not1mm-24.4.9.2/not1mm/data/JetBrainsMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/MASTER.SCP` & `not1mm-24.4.9.2/not1mm/data/MASTER.SCP`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/about.ui` & `not1mm-24.4.9.2/not1mm/data/about.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/bandmap.ui` & `not1mm-24.4.9.2/not1mm/data/bandmap.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/checkwindow.ui` & `not1mm-24.4.9.2/not1mm/data/checkwindow.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/configuration.ui` & `not1mm-24.4.9.2/not1mm/data/configuration.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/contests.sql` & `not1mm-24.4.9.2/not1mm/data/contests.sql`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/cty.json` & `not1mm-24.4.9.2/not1mm/data/cty.json`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/editcontact.ui` & `not1mm-24.4.9.2/not1mm/data/editcontact.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/editmacro.ui` & `not1mm-24.4.9.2/not1mm/data/editmacro.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/k6gte.not1mm-128.png` & `not1mm-24.4.9.2/not1mm/data/k6gte.not1mm-128.png`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/k6gte.not1mm-32.png` & `not1mm-24.4.9.2/not1mm/data/k6gte.not1mm-32.png`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/k6gte.not1mm-64.png` & `not1mm-24.4.9.2/not1mm/data/k6gte.not1mm-64.png`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/logwindow.ui` & `not1mm-24.4.9.2/not1mm/data/logwindow.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/logwindowx.ui` & `not1mm-24.4.9.2/not1mm/data/logwindowx.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/main.ui` & `not1mm-24.4.9.2/not1mm/data/main.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/new_contest.ui` & `not1mm-24.4.9.2/not1mm/data/new_contest.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/not1mm.html` & `not1mm-24.4.9.2/not1mm/data/not1mm.html`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/opon.ui` & `not1mm-24.4.9.2/not1mm/data/opon.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/0.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/0.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/1.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/1.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/2.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/2.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/3.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/3.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/4.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/4.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/5.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/5.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/6.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/6.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/7.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/7.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/73.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/73.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/8.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/8.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/9.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/9.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/a.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/a.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/again.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/again.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/b.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/b.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/c.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/c.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/contest.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/contest.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/cq.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/cq.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/d.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/d.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/e.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/e.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/f.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/f.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/g.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/g.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/h.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/h.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/i.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/i.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/j.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/j.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/k.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/k.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/k6gte.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/k6gte.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/l.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/l.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/m.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/m.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/mynumber.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/mynumber.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/n.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/n.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/nil.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/nil.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/o.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/o.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/p.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/p.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/q.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/q.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/r.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/r.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/roger.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/roger.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/s.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/s.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/space.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/space.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/t.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/t.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/thankyou.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/thankyou.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/thankyouqrz.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/thankyouqrz.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/u.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/u.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/v.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/v.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/w.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/w.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/x.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/x.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/y.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/y.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/yourcall.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/yourcall.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/phonetics/z.wav` & `not1mm-24.4.9.2/not1mm/data/phonetics/z.wav`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/pickcontest.ui` & `not1mm-24.4.9.2/not1mm/data/pickcontest.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/radio_green.png` & `not1mm-24.4.9.2/not1mm/data/radio_green.png`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/radio_grey.png` & `not1mm-24.4.9.2/not1mm/data/radio_grey.png`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/radio_red.png` & `not1mm-24.4.9.2/not1mm/data/radio_red.png`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/reddot.png` & `not1mm-24.4.9.2/not1mm/data/reddot.png`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/settings.ui` & `not1mm-24.4.9.2/not1mm/data/settings.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/data/vfo.ui` & `not1mm-24.4.9.2/not1mm/data/vfo.ui`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/fsutils.py` & `not1mm-24.4.9.2/not1mm/fsutils.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/lib/cat_interface.py` & `not1mm-24.4.9.2/not1mm/lib/cat_interface.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/lib/cwinterface.py` & `not1mm-24.4.9.2/not1mm/lib/cwinterface.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/lib/database.py` & `not1mm-24.4.9.2/not1mm/lib/database.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/lib/edit_macro.py` & `not1mm-24.4.9.2/not1mm/lib/edit_macro.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/lib/edit_station.py` & `not1mm-24.4.9.2/not1mm/lib/edit_station.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/lib/ft8_watcher.py` & `not1mm-24.4.9.2/not1mm/lib/ft8_watcher.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/lib/ham_utility.py` & `not1mm-24.4.9.2/not1mm/lib/ham_utility.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/lib/lookup.py` & `not1mm-24.4.9.2/not1mm/lib/lookup.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/lib/multicast.py` & `not1mm-24.4.9.2/not1mm/lib/multicast.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/lib/n1mm.py` & `not1mm-24.4.9.2/not1mm/lib/n1mm.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/lib/new_contest.py` & `not1mm-24.4.9.2/not1mm/lib/new_contest.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/lib/plugin_common.py` & `not1mm-24.4.9.2/not1mm/lib/plugin_common.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/lib/settings.py` & `not1mm-24.4.9.2/not1mm/lib/settings.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/lib/super_check_partial.py` & `not1mm-24.4.9.2/not1mm/lib/super_check_partial.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/lib/versiontest.py` & `not1mm-24.4.9.2/not1mm/lib/versiontest.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/logwindow.py` & `not1mm-24.4.9.2/not1mm/logwindow.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,19 +99,14 @@
             "current_database", "ham.db"
         )
         self.database = DataBase(self.dbname, fsutils.USER_DATA_PATH)
 
         self.database.current_contest = self.pref.get("contest", 0)
         self.contact = self.database.empty_contact
         uic.loadUi(fsutils.APP_DATA_PATH / "logwindow.ui", self)
-        self.setFeatures(
-            QDockWidget.DockWidgetFeature.DockWidgetMovable
-            | QDockWidget.DockWidgetFeature.DockWidgetClosable
-        )
-        # self.setAllowedAreas(QtCore.Qt.DockWidgetArea.AllDockWidgetAreas)
         self.setWindowTitle(
             f"QSO History - {self.pref.get('current_database', 'ham.db')}"
         )
         self.generalLog.setColumnCount(len(self.columns))
         self.focusedLog.setColumnCount(len(self.columns))
 
         self.checkmark = QtGui.QPixmap(str(fsutils.APP_DATA_PATH / "check.png"))
```

### Comparing `not1mm-24.4.9.1/not1mm/plugins/10_10_fall_cw.py` & `not1mm-24.4.9.2/not1mm/plugins/10_10_fall_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/plugins/10_10_spring_cw.py` & `not1mm-24.4.9.2/not1mm/plugins/10_10_spring_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/plugins/10_10_summer_phone.py` & `not1mm-24.4.9.2/not1mm/plugins/10_10_summer_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/plugins/10_10_winter_phone.py` & `not1mm-24.4.9.2/not1mm/plugins/10_10_winter_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/plugins/arrl_10m.py` & `not1mm-24.4.9.2/not1mm/plugins/arrl_10m.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/plugins/arrl_dx_cw.py` & `not1mm-24.4.9.2/not1mm/plugins/arrl_dx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/plugins/arrl_dx_ssb.py` & `not1mm-24.4.9.2/not1mm/plugins/arrl_dx_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/plugins/arrl_field_day.py` & `not1mm-24.4.9.2/not1mm/plugins/arrl_field_day.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/plugins/arrl_rtty_ru.py` & `not1mm-24.4.9.2/not1mm/plugins/arrl_rtty_ru.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/plugins/arrl_ss_cw.py` & `not1mm-24.4.9.2/not1mm/plugins/arrl_ss_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/plugins/arrl_ss_phone.py` & `not1mm-24.4.9.2/not1mm/plugins/arrl_ss_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/plugins/arrl_vhf_jan.py` & `not1mm-24.4.9.2/not1mm/plugins/arrl_vhf_jan.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/plugins/arrl_vhf_jun.py` & `not1mm-24.4.9.2/not1mm/plugins/arrl_vhf_jun.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/plugins/arrl_vhf_sep.py` & `not1mm-24.4.9.2/not1mm/plugins/arrl_vhf_sep.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/plugins/canada_day.py` & `not1mm-24.4.9.2/not1mm/plugins/canada_day.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/plugins/cq_160_cw.py` & `not1mm-24.4.9.2/not1mm/plugins/cq_160_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/plugins/cq_160_ssb.py` & `not1mm-24.4.9.2/not1mm/plugins/cq_160_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/plugins/cq_wpx_cw.py` & `not1mm-24.4.9.2/not1mm/plugins/cq_wpx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/plugins/cq_wpx_ssb.py` & `not1mm-24.4.9.2/not1mm/plugins/cq_wpx_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/plugins/cq_ww_cw.py` & `not1mm-24.4.9.2/not1mm/plugins/cq_ww_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/plugins/cq_ww_ssb.py` & `not1mm-24.4.9.2/not1mm/plugins/cq_ww_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/plugins/cwt.py` & `not1mm-24.4.9.2/not1mm/plugins/cwt.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/plugins/general_logging.py` & `not1mm-24.4.9.2/not1mm/plugins/general_logging.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/plugins/iaru_hf.py` & `not1mm-24.4.9.2/not1mm/plugins/iaru_hf.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/plugins/jidx_cw.py` & `not1mm-24.4.9.2/not1mm/plugins/jidx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/plugins/jidx_ph.py` & `not1mm-24.4.9.2/not1mm/plugins/jidx_ph.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/plugins/naqp_cw.py` & `not1mm-24.4.9.2/not1mm/plugins/naqp_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/plugins/naqp_ssb.py` & `not1mm-24.4.9.2/not1mm/plugins/naqp_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/plugins/phone_weekly_test.py` & `not1mm-24.4.9.2/not1mm/plugins/phone_weekly_test.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/plugins/stew_perry_topband.py` & `not1mm-24.4.9.2/not1mm/plugins/stew_perry_topband.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/plugins/winter_field_day.py` & `not1mm-24.4.9.2/not1mm/plugins/winter_field_day.py`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/not1mm/vfo.py` & `not1mm-24.4.9.2/not1mm/vfo.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,20 +35,14 @@
     message_shown = False
     multicast_interface = None
     current_palette = None
 
     def __init__(self):
         super().__init__()
         uic.loadUi(fsutils.APP_DATA_PATH / "vfo.ui", self)
-
-        self.setFeatures(
-            QDockWidget.DockWidgetFeature.DockWidgetMovable
-            | QDockWidget.DockWidgetFeature.DockWidgetClosable
-        )
-        # self.setAllowedAreas(QtCore.Qt.DockWidgetArea.AllDockWidgetAreas)
         self.setWindowTitle("VFO Window")
 
         self.rig_control = None
         self.timer = QTimer()
         self.timer.timeout.connect(self.getwaiting)
         self.load_pref()
         self.lcdNumber.display(0)
```

### Comparing `not1mm-24.4.9.1/not1mm.egg-info/PKG-INFO` & `not1mm-24.4.9.2/not1mm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: not1mm
-Version: 24.4.9.1
+Version: 24.4.9.2
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
 
+- [24-4-9-2] Put back the floatable dock widgets, 'cause Wayland strikes again.
 - [24-4-9-1] Removed DockWidgetFloatable from the dock widgets since my wee brain can't figure out how to add a dragable window frame to them once they are floating. Added a minimum size for the VFO LCD digits. Defaulted bandmap window to the right.
 - [24-4-9] Fixed Checkwindow not showing calls from logged contacts.
 - [24-4-7] Added FT8Watcher class to prep for FT8 support.
 - [24-4-4-1] Made docking widgets open state persistent.
 - [24-4-4] Added per-contest echange hint when adding new contest.
 - [24-4-2] Migrated to PyQt6. I'm sure there are broken things.
 - [24-4-1-2] Added color text indicators to the Check Partial window. Poached the code from @kyleboyle. Thanks! Fixed the Log, VFO and Check Partial windows to be actual docking widgets. Refocus call field after double clicking on item in the check partial window.
```

### Comparing `not1mm-24.4.9.1/not1mm.egg-info/SOURCES.txt` & `not1mm-24.4.9.2/not1mm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `not1mm-24.4.9.1/pyproject.toml` & `not1mm-24.4.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "not1mm" 
-version = "24.4.9.1"
+version = "24.4.9.2"
 description = "NOT1MM Logger"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
 dependencies = [
```

