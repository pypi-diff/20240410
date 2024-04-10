# Comparing `tmp/latex_rubber-1.6.3.tar.gz` & `tmp/latex_rubber-1.6.4.tar.gz`

## Comparing `latex_rubber-1.6.3.tar` & `latex_rubber-1.6.4.tar`

### file list

```diff
@@ -1,72 +1,74 @@
--rw-r--r--   0        0        0    74904 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/doc/rubber.html
--rw-r--r--   0        0        0    48721 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/doc/rubber.info
--rw-r--r--   0        0        0   178373 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/doc/rubber.pdf
--rw-r--r--   0        0        0    42055 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/doc/rubber.texi
--rw-r--r--   0        0        0    42677 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/doc/rubber.txt
--rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/doc/man-en/rubber-info.1
--rw-r--r--   0        0        0    18467 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/doc/man-en/rubber.1
--rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/doc/man-fr/rubber-info.1
--rw-r--r--   0        0        0    21029 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/doc/man-fr/rubber.1
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/__init__.py
--rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/biblio.py
--rw-r--r--   0        0        0    26287 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/cmdline.py
--rw-r--r--   0        0        0     4265 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/contents.py
--rw-r--r--   0        0        0     9270 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/convert.py
--rw-r--r--   0        0        0    11277 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/depend.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/dvip_tool.py
--rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/environment.py
--rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/index.py
--rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/module_interface.py
--rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/rules.ini
--rw-r--r--   0        0        0    14742 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/tex.py
--rw-r--r--   0        0        0    10336 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/util.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/converters/__init__.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/converters/compressor.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/converters/eps_gz.py
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/converters/fig2dev.py
--rw-r--r--   0        0        0    48052 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/converters/latex.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/converters/literate.py
--rw-r--r--   0        0        0     7804 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/converters/mpost.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/converters/shell.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/__init__.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/aleph.py
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/asymptote.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/backref.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/beamer.py
--rw-r--r--   0        0        0     4274 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/biblatex.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/bibtex.py
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/bibtopic.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/combine.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/dvipdfm.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/dvips.py
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/epsfig.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/glossaries.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/gnuplottex.py
--rw-r--r--   0        0        0     7513 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/graphics.py
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/graphicx.py -> graphics.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/hyperref.py
--rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/index.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/listings.py
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/ltxtable.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/lualatex.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/makeidx.py
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/minitoc-hyper.py -> minitoc.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/minitoc.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/moreverb.py
--rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/multibib.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/nomencl.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/ntheorem.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/omega.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/pdftex.py
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/ps2pdf.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/pythontex.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/verbatim.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/vtex.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/xelatex.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/xr.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/COPYING
--rw-r--r--   0        0        0     8269 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/hatch_build.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/pyproject.toml
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/PKG-INFO
+-rw-r--r--   0        0        0    74904 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/doc/rubber.html
+-rw-r--r--   0        0        0    48721 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/doc/rubber.info
+-rw-r--r--   0        0        0   178373 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/doc/rubber.pdf
+-rw-r--r--   0        0        0    42055 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/doc/rubber.texi
+-rw-r--r--   0        0        0    42677 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/doc/rubber.txt
+-rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/doc/man-en/rubber-info.1
+-rw-r--r--   0        0        0    18467 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/doc/man-en/rubber.1
+-rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/doc/man-fr/rubber-info.1
+-rw-r--r--   0        0        0    21029 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/doc/man-fr/rubber.1
+-rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/misc/zsh-completion
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/__init__.py
+-rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/biblio.py
+-rw-r--r--   0        0        0    26287 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/cmdline.py
+-rw-r--r--   0        0        0     4265 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/contents.py
+-rw-r--r--   0        0        0     9270 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/convert.py
+-rw-r--r--   0        0        0    11277 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/depend.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/dvip_tool.py
+-rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/environment.py
+-rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/index.py
+-rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/module_interface.py
+-rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/rules.ini
+-rw-r--r--   0        0        0    14742 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/tex.py
+-rw-r--r--   0        0        0    10336 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/util.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/converters/__init__.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/converters/compressor.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/converters/eps_gz.py
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/converters/fig2dev.py
+-rw-r--r--   0        0        0    48052 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/converters/latex.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/converters/literate.py
+-rw-r--r--   0        0        0     7804 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/converters/mpost.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/converters/shell.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/__init__.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/aleph.py
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/asymptote.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/backref.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/beamer.py
+-rw-r--r--   0        0        0     4274 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/biblatex.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/bibtex.py
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/bibtopic.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/combine.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/dvipdfm.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/dvips.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/epsfig.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/glossaries.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/gnuplottex.py
+-rw-r--r--   0        0        0     7513 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/graphics.py
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/graphicx.py -> graphics.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/hyperref.py
+-rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/index.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/listings.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/ltxtable.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/lualatex.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/makeidx.py
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/minitoc-hyper.py -> minitoc.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/minitoc.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/moreverb.py
+-rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/multibib.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/nomencl.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/ntheorem.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/omega.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/pdftex.py
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/ps2pdf.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/pythontex.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/verbatim.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/vtex.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/xelatex.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/xr.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/COPYING
+-rw-r--r--   0        0        0     6730 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/README.md
+-rw-r--r--   0        0        0    10043 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/hatch_build.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/pyproject.toml
+-rw-r--r--   0        0        0     7128 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/PKG-INFO
```

### Comparing `latex_rubber-1.6.3/doc/rubber.html` & `latex_rubber-1.6.4/doc/rubber.html`

 * *Files 0% similar despite different names*

```diff
@@ -21,18 +21,18 @@
 under the above conditions for modified versions,
 except that this permission notice may be stated in a
 translation approved by the Free Software Foundation.
 
 Copyright © 2002-2006 Emmanuel Beffara.
 
 Copyright © 2006-2015 Sebastian Kapfer. -->
-<title>Rubber Manual 1.6.3</title>
+<title>Rubber Manual 1.6.4</title>
 
-<meta name="description" content="Rubber Manual 1.6.3">
-<meta name="keywords" content="Rubber Manual 1.6.3">
+<meta name="description" content="Rubber Manual 1.6.4">
+<meta name="keywords" content="Rubber Manual 1.6.4">
 <meta name="resource-type" content="document">
 <meta name="distribution" content="global">
 <meta name="Generator" content="makeinfo">
 <meta name="viewport" content="width=device-width,initial-scale=1">
 
 <link href="#Top" rel="start" title="Top">
 <link href="#Introduction" rel="next" title="Introduction">
```

### Comparing `latex_rubber-1.6.3/doc/rubber.info` & `latex_rubber-1.6.4/doc/rubber.info`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/doc/rubber.pdf` & `latex_rubber-1.6.4/doc/rubber.pdf`

 * *Files 2% similar despite different names*

#### Comparing `latex_rubber-1.6.3/doc/rubber.pdf` & `latex_rubber-1.6.4/doc/rubber.pdf`

 * *Document info*

```diff
@@ -1,6 +1,6 @@
-CreationDate: "D:20240408222723+02'00'"
+CreationDate: "D:20240410175245+02'00'"
 Creator: 'TeX'
-ModDate: "D:20240408222723+02'00'"
+ModDate: "D:20240410175245+02'00'"
 PTEX.Fullbanner: 'This is pdfTeX, Version 3.141592653-2.6-1.40.22 (TeX Live 2021 Gentoo Linux) kpathsea version 6.3.3'
 Producer: 'pdfTeX-1.40.22'
 Trapped: '/False'
```

#### pdftotext {} -

```diff
@@ -1,9 +1,9 @@
 Rubber
-Documentation for version 1.6.3
+Documentation for version 1.6.4
 
 Sebastian Kapfer
 
 Permission is granted to make and distribute verbatim copies of this manual provided the
 copyright notice and this permission notice are preserved on all copies.
 Permission is granted to copy and distribute modified versions of this manual under the
 conditions for verbatim copying, provided also that the sections entitled “Copying” and
```

### Comparing `latex_rubber-1.6.3/doc/rubber.texi` & `latex_rubber-1.6.4/doc/rubber.texi`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 \input texinfo
 @c %**start of header
 @setfilename rubber.info
-@settitle Rubber Manual 1.6.3
+@settitle Rubber Manual 1.6.4
 @c %**end of header
 
 @copying
 Permission is granted to make and distribute verbatim
 copies of this manual provided the copyright notice and
 this permission notice are preserved on all copies.
 
@@ -27,15 +27,15 @@
 Copyright @copyright{} 2002--2006 Emmanuel Beffara.
 
 Copyright @copyright{} 2006--2015 Sebastian Kapfer.
 @end copying
 
 @titlepage
 @title Rubber
-@subtitle Documentation for version 1.6.3
+@subtitle Documentation for version 1.6.4
 @author Sebastian Kapfer
 @page
 @vskip 0pt plus 1fill
 @insertcopying
 @end titlepage
 
 @iftex
```

### Comparing `latex_rubber-1.6.3/doc/rubber.txt` & `latex_rubber-1.6.4/doc/rubber.txt`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/doc/man-en/rubber-info.1` & `latex_rubber-1.6.4/doc/man-en/rubber-info.1`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 Stupidly enumerate all LaTeX warnings, i.e. all the lines in the log file that
 contain the string "Warning".
 .PP
 
 .SH BUGS
 There are surely a some...
 
-This page documents Rubber version 1.6.3.
+This page documents Rubber version 1.6.4.
 The program and this man-page are maintained by Florian Schmaus <flo@geekplace.eu>.
 The homepage for Rubber can be found at https://gitlab.com/latex-rubber/rubber.
 
 .SH SEE ALSO
 The full documentation for
 .B rubber
 is maintained as a Texinfo manual.  If the
```

### Comparing `latex_rubber-1.6.3/doc/man-en/rubber.1` & `latex_rubber-1.6.4/doc/man-en/rubber.1`

 * *Files 0% similar despite different names*

```diff
@@ -636,15 +636,15 @@
 module, which may be used to specify the list of bibliographies the command
 applies to.
 .PP
 .
 .SH BUGS
 There are surely a some...
 .PP
-This page documents Rubber version 1.6.3.
+This page documents Rubber version 1.6.4.
 The program and this man-page are maintained by Florian Schmaus <flo@geekplace.eu>.
 The homepage for Rubber can be found at https://gitlab.com/latex-rubber/rubber.
 .
 .SH SEE ALSO
 The full documentation for
 .B rubber
 is maintained as a Texinfo manual.  If the
```

### Comparing `latex_rubber-1.6.3/doc/man-fr/rubber-info.1` & `latex_rubber-1.6.4/doc/man-fr/rubber-info.1`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 Affiche stupidement la liste de tous les avertissements de LaTeX, c'est-à-dire
 toutes les lignes du fichier log qui contiennent « Warning ».
 .PP
 
 .SH BUGS
 Il y en a surement quelques uns...
 
-Cette page se rapporte à la version 1.6.3 de Rubber. Le programme et cette
+Cette page se rapporte à la version 1.6.4 de Rubber. Le programme et cette
 documentation sont maintenus par Florian Schmaus <flo@geekplace.eu>.
 La page web du programme se trouve à l'adresse https://gitlab.com/latex-rubber/rubber.
 
 .SH VOIR AUSSI
 La documentation complète de
 .B rubber
 est maintenue en tant que manuel en Texinfo. Si les programmes
```

### Comparing `latex_rubber-1.6.3/doc/man-fr/rubber.1` & `latex_rubber-1.6.4/doc/man-fr/rubber.1`

 * *Files 1% similar despite different names*

```diff
@@ -657,15 +657,15 @@
 qui permet de spécifier la liste des bibliographies auxquelles s’applique la
 commande.
 .PP
 .
 .SH BUGS
 Il y en a surement quelques uns...
 .PP
-Cette page se rapporte à la version 1.6.3 de Rubber. Le programme et cette
+Cette page se rapporte à la version 1.6.4 de Rubber. Le programme et cette
 documentation sont maintenus par Florian Schmaus <flo@geekplace.eu>.
 La page web du programme se trouve à l’adresse https://gitlab.com/latex-rubber/rubber.
 .
 .SH VOIR AUSSI
 La documentation complète de
 .B rubber
 est maintenue en tant que manuel en Texinfo.
```

### Comparing `latex_rubber-1.6.3/rubber/biblio.py` & `latex_rubber-1.6.4/rubber/biblio.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/rubber/cmdline.py` & `latex_rubber-1.6.4/rubber/cmdline.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/rubber/contents.py` & `latex_rubber-1.6.4/rubber/contents.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/rubber/convert.py` & `latex_rubber-1.6.4/rubber/convert.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/rubber/depend.py` & `latex_rubber-1.6.4/rubber/depend.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/rubber/dvip_tool.py` & `latex_rubber-1.6.4/rubber/dvip_tool.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/rubber/environment.py` & `latex_rubber-1.6.4/rubber/environment.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/rubber/index.py` & `latex_rubber-1.6.4/rubber/index.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/rubber/module_interface.py` & `latex_rubber-1.6.4/rubber/module_interface.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/rubber/rules.ini` & `latex_rubber-1.6.4/rubber/rules.ini`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/rubber/tex.py` & `latex_rubber-1.6.4/rubber/tex.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/rubber/util.py` & `latex_rubber-1.6.4/rubber/util.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/rubber/converters/compressor.py` & `latex_rubber-1.6.4/rubber/converters/compressor.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/rubber/converters/eps_gz.py` & `latex_rubber-1.6.4/rubber/converters/eps_gz.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/rubber/converters/fig2dev.py` & `latex_rubber-1.6.4/rubber/converters/fig2dev.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/rubber/converters/latex.py` & `latex_rubber-1.6.4/rubber/converters/latex.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/rubber/converters/literate.py` & `latex_rubber-1.6.4/rubber/converters/literate.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/rubber/converters/mpost.py` & `latex_rubber-1.6.4/rubber/converters/mpost.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/rubber/converters/shell.py` & `latex_rubber-1.6.4/rubber/converters/shell.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/rubber/latex_modules/asymptote.py` & `latex_rubber-1.6.4/rubber/latex_modules/asymptote.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/rubber/latex_modules/beamer.py` & `latex_rubber-1.6.4/rubber/latex_modules/beamer.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/rubber/latex_modules/biblatex.py` & `latex_rubber-1.6.4/rubber/latex_modules/biblatex.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/rubber/latex_modules/bibtex.py` & `latex_rubber-1.6.4/rubber/latex_modules/bibtex.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/rubber/latex_modules/bibtopic.py` & `latex_rubber-1.6.4/rubber/latex_modules/bibtopic.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/rubber/latex_modules/combine.py` & `latex_rubber-1.6.4/rubber/latex_modules/combine.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/rubber/latex_modules/epsfig.py` & `latex_rubber-1.6.4/rubber/latex_modules/epsfig.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/rubber/latex_modules/glossaries.py` & `latex_rubber-1.6.4/rubber/latex_modules/glossaries.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/rubber/latex_modules/graphics.py` & `latex_rubber-1.6.4/rubber/latex_modules/graphics.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/rubber/latex_modules/index.py` & `latex_rubber-1.6.4/rubber/latex_modules/index.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/rubber/latex_modules/listings.py` & `latex_rubber-1.6.4/rubber/latex_modules/listings.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/rubber/latex_modules/ltxtable.py` & `latex_rubber-1.6.4/rubber/latex_modules/ltxtable.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/rubber/latex_modules/minitoc.py` & `latex_rubber-1.6.4/rubber/latex_modules/minitoc.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/rubber/latex_modules/moreverb.py` & `latex_rubber-1.6.4/rubber/latex_modules/moreverb.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/rubber/latex_modules/multibib.py` & `latex_rubber-1.6.4/rubber/latex_modules/multibib.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/rubber/latex_modules/pdftex.py` & `latex_rubber-1.6.4/rubber/latex_modules/pdftex.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/rubber/latex_modules/ps2pdf.py` & `latex_rubber-1.6.4/rubber/latex_modules/ps2pdf.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/rubber/latex_modules/pythontex.py` & `latex_rubber-1.6.4/rubber/latex_modules/pythontex.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/rubber/latex_modules/verbatim.py` & `latex_rubber-1.6.4/rubber/latex_modules/verbatim.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/rubber/latex_modules/vtex.py` & `latex_rubber-1.6.4/rubber/latex_modules/vtex.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/rubber/latex_modules/xr.py` & `latex_rubber-1.6.4/rubber/latex_modules/xr.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/COPYING` & `latex_rubber-1.6.4/COPYING`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.3/hatch_build.py` & `latex_rubber-1.6.4/hatch_build.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 # Copyright 2024      Sebastian Pipping
 
 import logging
 import os
 import re
 import shlex
 import subprocess
-from contextlib import contextmanager, suppress
-from os.path import abspath, join
+from contextlib import contextmanager
+from os.path import abspath, join, lexists
 
 from hatchling.builders.hooks.plugin.interface import BuildHookInterface
 
 _logger = logging.getLogger(__name__)
 
 
 class _RubberDocumentationBuilder:
@@ -29,42 +29,61 @@
     Builds Rubber documentaton by (1) substituting placeholders
     and (2) calling out to GNU Texinfo for rendering.
     """
 
     # A file f is generated from f.in by replacing @author@, @version@ by
     # sensible values (as ./configure does in the autoconf world).
     _FILES_WITH_SUBSTITUTIONS = (
-        os.path.join("doc", "man-en", "rubber.1"),
-        os.path.join("doc", "man-en", "rubber-info.1"),
-        os.path.join("doc", "man-fr", "rubber.1"),
-        os.path.join("doc", "man-fr", "rubber-info.1"),
-        os.path.join("doc", "rubber.texi"),
+        join("doc", "man-en", "rubber.1"),
+        join("doc", "man-en", "rubber-info.1"),
+        join("doc", "man-fr", "rubber.1"),
+        join("doc", "man-fr", "rubber-info.1"),
+        join("doc", "rubber.texi"),
     )
 
-    _MANUAL_BASENAME = os.path.join("doc", "rubber.")
+    _MANUAL_BASENAME = join("doc", "rubber.")
 
     _DOC_RECIPES = (
         ("html", ("makeinfo", "--html", "--no-split")),
         ("info", ("makeinfo", "--info")),
         ("pdf", ("texi2dvi", "--pdf", "--quiet", "--tidy")),
         ("txt", ("makeinfo", "--plaintext")),
     )
 
     def __init__(self, metadata):
         self.__metadata = metadata
 
     def _remove_file(self, filename):
-        _logger.info(f"Removing {filename!r}...")
-        with suppress(FileNotFoundError):
+        if lexists(filename):
+            _logger.info(f"Removing {filename!r}...")
             os.remove(filename)
 
     def _make_file(self, infile, outfile, func, args):
         """
-        Simplified fork of ``distutils.cmd.Command.make_file``
+        Remake of ``distutils.cmd.Command.make_file``
         """
+        try:
+            in_mod_time = os.stat(infile).st_mtime
+        except FileNotFoundError:
+            in_mod_time = 0  # i.e. Unix epoch 1970-01-01
+
+        try:
+            out_mod_time = os.stat(outfile).st_mtime
+        except FileNotFoundError:
+            # NOTE: This is intended to fake an out-of-date output file
+            #       which will trigger a build below.
+            #       If both input and ouput files are missing, an error
+            #       is to be expected below in ``func(..)``.
+            out_mod_time = in_mod_time - 1
+
+        if out_mod_time >= in_mod_time:
+            # Either (a) output present and input missing
+            #     or (b) output present and up to date
+            return
+
         _logger.info(f"Generating {outfile!r} from {infile!r}...")
         func(*args)
 
     def _spawn(self, *args):
         command_display = " ".join(shlex.quote(a) for a in args)
         _logger.info(f"Running...... # {command_display}")
         subprocess.check_call(args)
@@ -130,52 +149,78 @@
 def _logging_ensured(logger, target_level):
     original_level = None
     if logger.level < target_level:
         original_level = logger.level
         logger.setLevel(target_level)
 
     added_handler = None
-    if not logger.handlers:
+    if not logger.hasHandlers():
         added_handler = logging.StreamHandler()
         logger.addHandler(added_handler)
 
     try:
         yield
     finally:
         if original_level is not None:
             logger.setLevel(original_level)
         if added_handler is not None:
-            logger.handlers.remove(added_handler)
+            logger.removeHandler(added_handler)
 
 
 class CustomBuildHook(BuildHookInterface):
     """
     Hatchling integration to build additional files, and
     make them get included with ``sdist`` and ``wheel`` archives.
     """
 
+    __generated_during_sdist = False
+
     def initialize(self, version, build_data):
         with _logging_ensured(_logger, logging.INFO):
+            _logger.info(f"Hooking into target {self.target_name!r}...")
             doc_builder = _RubberDocumentationBuilder(self.metadata)
 
             if self.target_name == "sdist":
                 doc_builder.clean()
                 doc_builder.build()
+                self.__generated_during_sdist = True
                 build_data["artifacts"].extend(doc_builder.iterate_filenames())
             elif self.target_name == "wheel":
+                if not self.__generated_during_sdist:
+                    doc_builder.build()
+
                 pypi_project_name = self.metadata.name.replace("-", "_")
                 wheel_data_prefix = join(f"{pypi_project_name}-{self.metadata.version}.data",
                                          "data", "share")
                 for filename in doc_builder.iterate_filenames():
                     build_data["force_include"][abspath(filename)] = join(
                         wheel_data_prefix, filename)
 
+                build_data["force_include"][abspath(join("misc", "zsh-completion"))] = join(
+                    wheel_data_prefix, "zsh", "site-functions", "_rubber")
+
         return super().initialize(version, build_data)
 
 
+def _run_clean_command(config):
+    from hatchling.metadata.core import ProjectMetadata
+    from hatchling.plugin.manager import PluginManager
+
+    logging.basicConfig(level=logging.INFO)
+
+    metadata = ProjectMetadata(root=".", plugin_manager=PluginManager())
+
+    _logger.info(f"Cleaning generated files for {metadata.name} version {metadata.version}...")
+
+    doc_builder = _RubberDocumentationBuilder(metadata)
+    doc_builder.clean()
+
+    _logger.info("Done.")
+
+
 def _run_generate_command(_config):
     from hatchling.metadata.core import ProjectMetadata
     from hatchling.plugin.manager import PluginManager
 
     logging.basicConfig(level=logging.INFO)
 
     metadata = ProjectMetadata(root=".", plugin_manager=PluginManager())
@@ -216,14 +261,18 @@
     parser = argparse.ArgumentParser(description=("Run custom build commands for Rubber."
                                                   " Direct invocation is purely optional"
                                                   ", `python3 -m build` has you covered!"))
     subparsers = parser.add_subparsers(required=True,
                                        title="subcommands",
                                        help="call with --help for details")
 
+    clean_command = subparsers.add_parser("clean",
+                                          description="Clean generated files shipped with Rubber")
+    clean_command.set_defaults(func=_run_clean_command)
+
     generate_command = subparsers.add_parser("generate",
                                              description="Generate files needed to ship Rubber")
     generate_command.set_defaults(func=_run_generate_command)
 
     tar_command = subparsers.add_parser("tar", description='Wrapper for "git archive"')
     tar_command.add_argument(
         "--revision",
```

### Comparing `latex_rubber-1.6.3/pyproject.toml` & `latex_rubber-1.6.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "latex-rubber"
 dynamic = ["version"]
 description = "an automated system for building LaTeX documents"
+readme = {file = "README.md", content-type = "text/markdown"}
 license = {text = "GPL-3.0-or-later"}
 requires-python = ">=3.8"
 authors = [
     { name = "Sebastian Kapfer", email = "sebastian.kapfer@fau.de" },
 ]
 maintainers = [
     { name = "Florian Schmaus", email = "flo@geekplace.eu" },
@@ -25,14 +26,15 @@
 rubber-pipe = "rubber.cmdline:main_rubber_pipe"
 
 [tool.hatch.version]
 path = "rubber/version.py"
 
 [tool.hatch.build.targets.sdist]
 include = [
+    "/misc/zsh-completion",
     "/rubber",
 ]
 
 [tool.hatch.build.targets.wheel]
 packages = ["rubber"]
 
 # These two empty sections enable the custom build hook
```

