# Comparing `tmp/chartpy-0.1.8.tar.gz` & `tmp/chartpy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\chartpy-0.1.8.tar", last modified: Mon Jun  8 10:45:55 2020, max compression
+gzip compressed data, was "chartpy-0.1.9.tar", last modified: Tue May  4 16:52:26 2021, max compression
```

## Comparing `chartpy-0.1.8.tar` & `chartpy-0.1.9.tar`

### file list

```diff
@@ -1,546 +1,547 @@
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/
--rw-rw-rw-   0        0        0       96 2017-11-15 10:15:02.000000 chartpy-0.1.8/.gitattributes
--rw-rw-rw-   0        0        0      887 2019-10-23 08:19:35.000000 chartpy-0.1.8/.gitignore
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy/
--rw-rw-rw-   0        0        0    19244 2020-03-30 13:42:58.000000 chartpy-0.1.8/chartpy/canvas.py
--rw-rw-rw-   0        0        0    12296 2019-02-13 18:04:54.000000 chartpy-0.1.8/chartpy/canvas.pyc
--rw-rw-rw-   0        0        0     4007 2018-02-24 17:51:36.000000 chartpy-0.1.8/chartpy/chart.py
--rw-rw-rw-   0        0        0     2855 2018-02-24 17:51:46.000000 chartpy-0.1.8/chartpy/chart.pyc
--rw-rw-rw-   0        0        0    11619 2019-08-06 10:14:40.000000 chartpy-0.1.8/chartpy/chartconstants.py
--rw-rw-rw-   0        0        0     9294 2019-08-06 21:30:48.000000 chartpy-0.1.8/chartpy/chartconstants.pyc
--rw-rw-rw-   0        0        0    85244 2020-06-08 10:41:12.000000 chartpy-0.1.8/chartpy/engine.py
--rw-rw-rw-   0        0        0    50632 2019-08-21 10:01:19.000000 chartpy-0.1.8/chartpy/engine.pyc
--rw-rw-rw-   0        0        0    25456 2019-08-06 10:07:26.000000 chartpy-0.1.8/chartpy/style.py
--rw-rw-rw-   0        0        0    29038 2019-08-06 21:30:48.000000 chartpy-0.1.8/chartpy/style.pyc
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy/stylesheets/
--rw-rw-rw-   0        0        0     1026 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy/stylesheets/538-chartpy.mplstyle
--rw-rw-rw-   0        0        0     1299 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy/stylesheets/chartpy-pyfolio.mplstyle
--rw-rw-rw-   0        0        0     1298 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy/stylesheets/chartpy.mplstyle
--rw-rw-rw-   0        0        0     1198 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy/stylesheets/ggplot-chartpy.mplstyle
--rw-rw-rw-   0        0        0     1111 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy/stylesheets/ggplot-tradtional.mplstyle
--rw-rw-rw-   0        0        0        0 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy/stylesheets/__init__.py
--rw-rw-rw-   0        0        0     1957 2018-01-30 10:54:40.000000 chartpy-0.1.8/chartpy/twitter.py
--rw-rw-rw-   0        0        0     1747 2018-01-30 10:56:06.000000 chartpy-0.1.8/chartpy/twitter.pyc
--rw-rw-rw-   0        0        0      217 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy/__init__.py
--rw-rw-rw-   0        0        0      468 2018-01-30 10:56:06.000000 chartpy-0.1.8/chartpy/__init__.pyc
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy/__pycache__/
--rw-rw-rw-   0        0        0    11360 2018-02-26 18:52:14.000000 chartpy-0.1.8/chartpy/__pycache__/canvas.cpython-35.pyc
--rw-rw-rw-   0        0        0    10705 2020-03-31 17:57:54.000000 chartpy-0.1.8/chartpy/__pycache__/canvas.cpython-36.pyc
--rw-rw-rw-   0        0        0     2493 2018-02-26 14:03:10.000000 chartpy-0.1.8/chartpy/__pycache__/chart.cpython-35.pyc
--rw-rw-rw-   0        0        0     2214 2020-03-10 09:41:12.000000 chartpy-0.1.8/chartpy/__pycache__/chart.cpython-36.pyc
--rw-rw-rw-   0        0        0     7608 2018-03-19 17:57:02.000000 chartpy-0.1.8/chartpy/__pycache__/chartconstants.cpython-35.pyc
--rw-rw-rw-   0        0        0     6721 2020-03-10 09:41:12.000000 chartpy-0.1.8/chartpy/__pycache__/chartconstants.cpython-36.pyc
--rw-rw-rw-   0        0        0      339 2018-04-21 19:57:14.000000 chartpy-0.1.8/chartpy/__pycache__/chartcred.cpython-35.pyc
--rw-rw-rw-   0        0        0      322 2020-06-08 10:33:26.000000 chartpy-0.1.8/chartpy/__pycache__/chartcred.cpython-36.pyc
--rw-rw-rw-   0        0        0    47318 2018-06-21 16:50:44.000000 chartpy-0.1.8/chartpy/__pycache__/engine.cpython-35.pyc
--rw-rw-rw-   0        0        0    44373 2020-06-08 10:32:54.000000 chartpy-0.1.8/chartpy/__pycache__/engine.cpython-36.pyc
--rw-rw-rw-   0        0        0    22806 2018-03-19 17:57:02.000000 chartpy-0.1.8/chartpy/__pycache__/style.cpython-35.pyc
--rw-rw-rw-   0        0        0    21488 2020-03-10 09:41:12.000000 chartpy-0.1.8/chartpy/__pycache__/style.cpython-36.pyc
--rw-rw-rw-   0        0        0     1512 2018-02-01 14:09:24.000000 chartpy-0.1.8/chartpy/__pycache__/twitter.cpython-35.pyc
--rw-rw-rw-   0        0        0     1409 2020-03-10 09:41:12.000000 chartpy-0.1.8/chartpy/__pycache__/twitter.cpython-36.pyc
--rw-rw-rw-   0        0        0      410 2017-11-16 12:36:36.000000 chartpy-0.1.8/chartpy/__pycache__/__init__.cpython-35.pyc
--rw-rw-rw-   0        0        0      388 2020-03-10 09:41:12.000000 chartpy-0.1.8/chartpy/__pycache__/__init__.cpython-36.pyc
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy.egg-info/
--rw-rw-rw-   0        0        0        1 2020-06-08 10:45:54.000000 chartpy-0.1.8/chartpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2018-07-30 17:13:30.000000 chartpy-0.1.8/chartpy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      939 2020-06-08 10:45:54.000000 chartpy-0.1.8/chartpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      102 2020-06-08 10:45:54.000000 chartpy-0.1.8/chartpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0    26687 2020-06-08 10:45:54.000000 chartpy-0.1.8/chartpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       29 2020-06-08 10:45:54.000000 chartpy-0.1.8/chartpy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/
--rw-rw-rw-   0        0        0   130032 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/barh.png
--rw-rw-rw-   0        0        0    16866 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/bokeh.html
--rw-rw-rw-   0        0        0   165869 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/canvas.png
--rw-rw-rw-   0        0        0     2490 2019-08-06 09:34:12.000000 chartpy-0.1.8/chartpy_examples/canvas_demo.py
--rw-rw-rw-   0        0        0     3847 2020-06-08 10:33:03.000000 chartpy-0.1.8/chartpy_examples/chart_demo.py
--rw-rw-rw-   0        0        0    71102 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/heatmap.png
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/notebooks/
--rw-rw-rw-   0        0        0  1322629 2018-04-20 09:14:22.000000 chartpy-0.1.8/chartpy_examples/notebooks/chart_examples.ipynb
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/css/
--rw-rw-rw-   0        0        0   109522 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/css/bootstrap.min.css
--rw-rw-rw-   0        0        0     6112 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/css/iThing.css
--rw-rw-rw-   0        0        0     1526 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/css/keen-dashboards.css
--rw-rw-rw-   0        0        0     2716 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/css/keen-static.css
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/fonts/
--rw-rw-rw-   0        0        0    20335 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/fonts/glyphicons-halflings-regular.eot
--rw-rw-rw-   0        0        0    63155 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/fonts/glyphicons-halflings-regular.svg
--rw-rw-rw-   0        0        0    41280 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/fonts/glyphicons-halflings-regular.ttf
--rw-rw-rw-   0        0        0    23320 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/fonts/glyphicons-halflings-regular.woff
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/
--rw-rw-rw-   0        0        0     1171 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/.bower.json
--rw-rw-rw-   0        0        0      887 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/bower.json
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/fonts/
--rw-rw-rw-   0        0        0    20335 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/fonts/glyphicons-halflings-regular.eot
--rw-rw-rw-   0        0        0    63155 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/fonts/glyphicons-halflings-regular.svg
--rw-rw-rw-   0        0        0    41280 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/fonts/glyphicons-halflings-regular.ttf
--rw-rw-rw-   0        0        0    23320 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/fonts/glyphicons-halflings-regular.woff
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/grunt/
--rw-rw-rw-   0        0        0     1434 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/grunt/bs-glyphicons-data-generator.js
--rw-rw-rw-   0        0        0     6301 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/grunt/bs-lessdoc-parser.js
--rw-rw-rw-   0        0        0     1422 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/grunt/bs-raw-files-generator.js
--rw-rw-rw-   0        0        0     1517 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/grunt/sauce_browsers.yml
--rw-rw-rw-   0        0        0    13428 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/Gruntfile.js
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/js/
--rw-rw-rw-   0        0        0     4244 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/js/affix.js
--rw-rw-rw-   0        0        0     2320 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/js/alert.js
--rw-rw-rw-   0        0        0     3085 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/js/button.js
--rw-rw-rw-   0        0        0     6749 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/js/carousel.js
--rw-rw-rw-   0        0        0     5042 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/js/collapse.js
--rw-rw-rw-   0        0        0     4536 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/js/dropdown.js
--rw-rw-rw-   0        0        0     8220 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/js/modal.js
--rw-rw-rw-   0        0        0     3373 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/js/popover.js
--rw-rw-rw-   0        0        0     4811 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/js/scrollspy.js
--rw-rw-rw-   0        0        0     3127 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/js/tab.js
--rw-rw-rw-   0        0        0    15099 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/js/tooltip.js
--rw-rw-rw-   0        0        0     1890 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/js/transition.js
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/
--rw-rw-rw-   0        0        0     1581 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/alerts.less
--rw-rw-rw-   0        0        0     1124 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/badges.less
--rw-rw-rw-   0        0        0     1171 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/bootstrap.less
--rw-rw-rw-   0        0        0      620 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/breadcrumbs.less
--rw-rw-rw-   0        0        0     5724 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/button-groups.less
--rw-rw-rw-   0        0        0     3657 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/buttons.less
--rw-rw-rw-   0        0        0     5002 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/carousel.less
--rw-rw-rw-   0        0        0      716 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/close.less
--rw-rw-rw-   0        0        0     1446 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/code.less
--rw-rw-rw-   0        0        0      616 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/component-animations.less
--rw-rw-rw-   0        0        0     4997 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/dropdowns.less
--rw-rw-rw-   0        0        0    14274 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/forms.less
--rw-rw-rw-   0        0        0    15095 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/glyphicons.less
--rw-rw-rw-   0        0        0     1471 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/grid.less
--rw-rw-rw-   0        0        0     4381 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/input-groups.less
--rw-rw-rw-   0        0        0     1013 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/jumbotron.less
--rw-rw-rw-   0        0        0     1143 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/labels.less
--rw-rw-rw-   0        0        0     3244 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/list-group.less
--rw-rw-rw-   0        0        0      904 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/media.less
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/
--rw-rw-rw-   0        0        0      271 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/alerts.less
--rw-rw-rw-   0        0        0      147 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/background-variant.less
--rw-rw-rw-   0        0        0      486 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/border-radius.less
--rw-rw-rw-   0        0        0     1106 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/buttons.less
--rw-rw-rw-   0        0        0      127 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/center-block.less
--rw-rw-rw-   0        0        0      627 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/clearfix.less
--rw-rw-rw-   0        0        0     2634 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/forms.less
--rw-rw-rw-   0        0        0     4447 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/gradients.less
--rw-rw-rw-   0        0        0     2911 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/grid-framework.less
--rw-rw-rw-   0        0        0     3216 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/grid.less
--rw-rw-rw-   0        0        0      600 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/hide-text.less
--rw-rw-rw-   0        0        0     1167 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/image.less
--rw-rw-rw-   0        0        0      175 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/labels.less
--rw-rw-rw-   0        0        0      562 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/list-group.less
--rw-rw-rw-   0        0        0      242 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/nav-divider.less
--rw-rw-rw-   0        0        0      373 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/nav-vertical-align.less
--rw-rw-rw-   0        0        0      156 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/opacity.less
--rw-rw-rw-   0        0        0      461 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/pagination.less
--rw-rw-rw-   0        0        0      561 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/panels.less
--rw-rw-rw-   0        0        0      201 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/progress-bar.less
--rw-rw-rw-   0        0        0      256 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/reset-filter.less
--rw-rw-rw-   0        0        0      202 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/resize.less
--rw-rw-rw-   0        0        0      358 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/responsive-visibility.less
--rw-rw-rw-   0        0        0      137 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/size.less
--rw-rw-rw-   0        0        0      168 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/tab-focus.less
--rw-rw-rw-   0        0        0      728 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/table-row.less
--rw-rw-rw-   0        0        0      124 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/text-emphasis.less
--rw-rw-rw-   0        0        0      170 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/text-overflow.less
--rw-rw-rw-   0        0        0     6870 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/vendor-prefixes.less
--rw-rw-rw-   0        0        0     1141 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins.less
--rw-rw-rw-   0        0        0     3725 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/modals.less
--rw-rw-rw-   0        0        0    15343 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/navbar.less
--rw-rw-rw-   0        0        0     5167 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/navs.less
--rw-rw-rw-   0        0        0     8060 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/normalize.less
--rw-rw-rw-   0        0        0      912 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/pager.less
--rw-rw-rw-   0        0        0     2084 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/pagination.less
--rw-rw-rw-   0        0        0     5848 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/panels.less
--rw-rw-rw-   0        0        0     3539 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/popovers.less
--rw-rw-rw-   0        0        0     1714 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/print.less
--rw-rw-rw-   0        0        0     2314 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/progress-bars.less
--rw-rw-rw-   0        0        0      589 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/responsive-embed.less
--rw-rw-rw-   0        0        0     4456 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/responsive-utilities.less
--rw-rw-rw-   0        0        0     2793 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/scaffolding.less
--rw-rw-rw-   0        0        0     4712 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/tables.less
--rw-rw-rw-   0        0        0     7431 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/theme.less
--rw-rw-rw-   0        0        0      786 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/thumbnails.less
--rw-rw-rw-   0        0        0     2685 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/tooltip.less
--rw-rw-rw-   0        0        0     6402 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/type.less
--rw-rw-rw-   0        0        0      862 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/utilities.less
--rw-rw-rw-   0        0        0    27071 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/variables.less
--rw-rw-rw-   0        0        0      556 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/wells.less
--rw-rw-rw-   0        0        0     1105 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/LICENSE
--rw-rw-rw-   0        0        0     2103 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/package.json
--rw-rw-rw-   0        0        0     6010 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/README.md
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/holderjs/
--rw-rw-rw-   0        0        0      406 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/holderjs/.bower.json
--rw-rw-rw-   0        0        0       78 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/holderjs/.gitattributes
--rw-rw-rw-   0        0        0       48 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/holderjs/.gitignore
--rw-rw-rw-   0        0        0      177 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/holderjs/.jshintrc
--rw-rw-rw-   0        0        0       75 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/holderjs/bower.json
--rw-rw-rw-   0        0        0      827 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/holderjs/composer.json
--rw-rw-rw-   0        0        0     1159 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/holderjs/Gruntfile.js
--rw-rw-rw-   0        0        0    20918 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/holderjs/holder.js
--rw-rw-rw-   0        0        0      899 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/holderjs/package.json
--rw-rw-rw-   0        0        0     6754 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/holderjs/README.md
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/
--rw-rw-rw-   0        0        0      772 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/.bower.json
--rw-rw-rw-   0        0        0      462 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/bower.json
--rw-rw-rw-   0        0        0     1120 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/MIT-LICENSE.txt
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/ajax/
--rw-rw-rw-   0        0        0     2605 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/ajax/jsonp.js
--rw-rw-rw-   0        0        0     1744 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/ajax/load.js
--rw-rw-rw-   0        0        0      235 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/ajax/parseJSON.js
--rw-rw-rw-   0        0        0      513 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/ajax/parseXML.js
--rw-rw-rw-   0        0        0     1335 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/ajax/script.js
--rw-rw-rw-   0        0        0     3624 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/ajax/xhr.js
--rw-rw-rw-   0        0        0    21954 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/ajax.js
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/attributes/
--rw-rw-rw-   0        0        0     3461 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/attributes/attr.js
--rw-rw-rw-   0        0        0     4313 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/attributes/classes.js
--rw-rw-rw-   0        0        0     1948 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/attributes/prop.js
--rw-rw-rw-   0        0        0      928 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/attributes/support.js
--rw-rw-rw-   0        0        0     4000 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/attributes/val.js
--rw-rw-rw-   0        0        0      211 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/attributes.js
--rw-rw-rw-   0        0        0     5711 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/callbacks.js
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/core/
--rw-rw-rw-   0        0        0     1270 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/core/access.js
--rw-rw-rw-   0        0        0     3524 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/core/init.js
--rw-rw-rw-   0        0        0      977 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/core/parseHTML.js
--rw-rw-rw-   0        0        0     2478 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/core/ready.js
--rw-rw-rw-   0        0        0    12077 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/core.js
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/css/
--rw-rw-rw-   0        0        0      531 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/css/addGetHookIf.js
--rw-rw-rw-   0        0        0     1509 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/css/curCSS.js
--rw-rw-rw-   0        0        0     1937 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/css/defaultDisplay.js
--rw-rw-rw-   0        0        0      395 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/css/hiddenVisibleSelectors.js
--rw-rw-rw-   0        0        0     3294 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/css/support.js
--rw-rw-rw-   0        0        0      583 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/css/swap.js
--rw-rw-rw-   0        0        0    12796 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/css.js
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/data/
--rw-rw-rw-   0        0        0      403 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/data/accepts.js
--rw-rw-rw-   0        0        0     5063 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/data/Data.js
--rw-rw-rw-   0        0        0     5120 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/data.js
--rw-rw-rw-   0        0        0     4563 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/deferred.js
--rw-rw-rw-   0        0        0      236 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/deprecated.js
--rw-rw-rw-   0        0        0     1826 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/dimensions.js
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/effects/
--rw-rw-rw-   0        0        0      238 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/effects/animatedSelector.js
--rw-rw-rw-   0        0        0     3142 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/effects/Tween.js
--rw-rw-rw-   0        0        0    17562 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/effects.js
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/event/
--rw-rw-rw-   0        0        0      335 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/event/ajax.js
--rw-rw-rw-   0        0        0     1133 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/event/alias.js
--rw-rw-rw-   0        0        0      132 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/event/support.js
--rw-rw-rw-   0        0        0    25343 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/event.js
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/exports/
--rw-rw-rw-   0        0        0     1030 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/exports/amd.js
--rw-rw-rw-   0        0        0      673 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/exports/global.js
--rw-rw-rw-   0        0        0     1437 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/intro.js
--rw-rw-rw-   0        0        0      611 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/jquery.js
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/manipulation/
--rw-rw-rw-   0        0        0     1007 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/manipulation/support.js
--rw-rw-rw-   0        0        0      258 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/manipulation/_evalUrl.js
--rw-rw-rw-   0        0        0    15619 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/manipulation.js
--rw-rw-rw-   0        0        0     5795 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/offset.js
--rw-rw-rw-   0        0        0        6 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/outro.js
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/queue/
--rw-rw-rw-   0        0        0      583 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/queue/delay.js
--rw-rw-rw-   0        0        0     3205 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/queue.js
--rw-rw-rw-   0        0        0     4606 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/selector-native.js
--rw-rw-rw-   0        0        0      308 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/selector-sizzle.js
--rw-rw-rw-   0        0        0       34 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/selector.js
--rw-rw-rw-   0        0        0     3325 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/serialize.js
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/traversing/
--rw-rw-rw-   0        0        0     2564 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/traversing/findFilter.js
--rw-rw-rw-   0        0        0     4734 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/traversing.js
--rw-rw-rw-   0        0        0     1575 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/wrap.js
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery-knob/
--rw-rw-rw-   0        0        0      615 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery-knob/.bower.json
--rw-rw-rw-   0        0        0       10 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery-knob/.gitignore
--rw-rw-rw-   0        0        0      286 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery-knob/bower.json
--rw-rw-rw-   0        0        0    27969 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery-knob/excanvas.js
--rw-rw-rw-   0        0        0    13363 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery-knob/index.html
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery-knob/js/
--rw-rw-rw-   0        0        0    26905 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery-knob/js/jquery.knob.js
--rw-rw-rw-   0        0        0     1021 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery-knob/knob.jquery.json
--rw-rw-rw-   0        0        0     1102 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery-knob/LICENSE
--rw-rw-rw-   0        0        0     3315 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery-knob/README.md
--rw-rw-rw-   0        0        0    33487 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery-knob/secretplan.jpg
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/keen-js/
--rw-rw-rw-   0        0        0     1525 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/keen-js/.bower.json
--rw-rw-rw-   0        0        0     1222 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/keen-js/bower.json
--rw-rw-rw-   0        0        0     1100 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/keen-js/LICENSE
--rw-rw-rw-   0        0        0     1260 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/meta.js
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/slider/
--rw-rw-rw-   0        0        0     3995 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/slider/jQDateRangeSlider.js
--rw-rw-rw-   0        0        0     5000 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/slider/jQDateRangeSliderHandle.js
--rw-rw-rw-   0        0        0    20306 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/slider/jQRangeSlider.js
--rw-rw-rw-   0        0        0    13611 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/slider/jQRangeSliderBar.js
--rw-rw-rw-   0        0        0     3730 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/slider/jQRangeSliderDraggable.js
--rw-rw-rw-   0        0        0     8489 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/slider/jQRangeSliderHandle.js
--rw-rw-rw-   0        0        0    12731 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/slider/jQRangeSliderLabel.js
--rw-rw-rw-   0        0        0     2777 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/slider/jQRangeSliderMouseTouch.js
--rw-rw-rw-   0        0        0     2983 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/slider/jQRuler.js
--rw-rw-rw-   0        0        0    94842 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/slider/jquery-1.7.2.min.js
--rw-rw-rw-   0        0        0   201856 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/slider/jquery-ui.min.js
--rw-rw-rw-   0        0        0     2395 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/static/js/slider/slider.js
--rw-rw-rw-   0        0        0    16107 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/s_bokeh.html
--rw-rw-rw-   0        0        0     3325 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/s_canvas.html
--rw-rw-rw-   0        0        0     3275 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/s_canvas_keen.html
--rw-rw-rw-   0        0        0     4320 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/s_canvas_plain.html
--rw-rw-rw-   0        0        0    35180 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/s_matplotlib.png
--rw-rw-rw-   0        0        0  1230282 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/s_plotly.html
--rw-rw-rw-   0        0        0    60965 2018-04-20 09:14:30.000000 chartpy-0.1.8/chartpy_examples/notebooks/web_page_examples.ipynb
--rw-rw-rw-   0        0        0        0 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/notebooks/__init__.py
--rw-rw-rw-   0        0        0  1231027 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/plotly.html
--rw-rw-rw-   0        0        0    45314 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/plotlyheatmap.png
--rw-rw-rw-   0        0        0    76404 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/screenshot.png
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/static/
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/static/css/
--rw-rw-rw-   0        0        0   109522 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/css/bootstrap.min.css
--rw-rw-rw-   0        0        0     6112 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/css/iThing.css
--rw-rw-rw-   0        0        0     1526 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/css/keen-dashboards.css
--rw-rw-rw-   0        0        0     2716 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/css/keen-static.css
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/static/fonts/
--rw-rw-rw-   0        0        0    20335 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/fonts/glyphicons-halflings-regular.eot
--rw-rw-rw-   0        0        0    63155 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/fonts/glyphicons-halflings-regular.svg
--rw-rw-rw-   0        0        0    41280 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/fonts/glyphicons-halflings-regular.ttf
--rw-rw-rw-   0        0        0    23320 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/fonts/glyphicons-halflings-regular.woff
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/static/js/
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/
--rw-rw-rw-   0        0        0     1171 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/.bower.json
--rw-rw-rw-   0        0        0      887 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/bower.json
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/fonts/
--rw-rw-rw-   0        0        0    20335 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/fonts/glyphicons-halflings-regular.eot
--rw-rw-rw-   0        0        0    63155 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/fonts/glyphicons-halflings-regular.svg
--rw-rw-rw-   0        0        0    41280 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/fonts/glyphicons-halflings-regular.ttf
--rw-rw-rw-   0        0        0    23320 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/fonts/glyphicons-halflings-regular.woff
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/grunt/
--rw-rw-rw-   0        0        0     1434 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/grunt/bs-glyphicons-data-generator.js
--rw-rw-rw-   0        0        0     6301 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/grunt/bs-lessdoc-parser.js
--rw-rw-rw-   0        0        0     1422 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/grunt/bs-raw-files-generator.js
--rw-rw-rw-   0        0        0     1517 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/grunt/sauce_browsers.yml
--rw-rw-rw-   0        0        0    13428 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/Gruntfile.js
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/js/
--rw-rw-rw-   0        0        0     4244 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/js/affix.js
--rw-rw-rw-   0        0        0     2320 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/js/alert.js
--rw-rw-rw-   0        0        0     3085 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/js/button.js
--rw-rw-rw-   0        0        0     6749 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/js/carousel.js
--rw-rw-rw-   0        0        0     5042 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/js/collapse.js
--rw-rw-rw-   0        0        0     4536 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/js/dropdown.js
--rw-rw-rw-   0        0        0     8220 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/js/modal.js
--rw-rw-rw-   0        0        0     3373 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/js/popover.js
--rw-rw-rw-   0        0        0     4811 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/js/scrollspy.js
--rw-rw-rw-   0        0        0     3127 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/js/tab.js
--rw-rw-rw-   0        0        0    15099 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/js/tooltip.js
--rw-rw-rw-   0        0        0     1890 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/js/transition.js
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/
--rw-rw-rw-   0        0        0     1581 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/alerts.less
--rw-rw-rw-   0        0        0     1124 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/badges.less
--rw-rw-rw-   0        0        0     1171 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/bootstrap.less
--rw-rw-rw-   0        0        0      620 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/breadcrumbs.less
--rw-rw-rw-   0        0        0     5724 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/button-groups.less
--rw-rw-rw-   0        0        0     3657 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/buttons.less
--rw-rw-rw-   0        0        0     5002 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/carousel.less
--rw-rw-rw-   0        0        0      716 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/close.less
--rw-rw-rw-   0        0        0     1446 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/code.less
--rw-rw-rw-   0        0        0      616 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/component-animations.less
--rw-rw-rw-   0        0        0     4997 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/dropdowns.less
--rw-rw-rw-   0        0        0    14274 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/forms.less
--rw-rw-rw-   0        0        0    15095 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/glyphicons.less
--rw-rw-rw-   0        0        0     1471 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/grid.less
--rw-rw-rw-   0        0        0     4381 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/input-groups.less
--rw-rw-rw-   0        0        0     1013 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/jumbotron.less
--rw-rw-rw-   0        0        0     1143 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/labels.less
--rw-rw-rw-   0        0        0     3244 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/list-group.less
--rw-rw-rw-   0        0        0      904 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/media.less
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/
--rw-rw-rw-   0        0        0      271 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/alerts.less
--rw-rw-rw-   0        0        0      147 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/background-variant.less
--rw-rw-rw-   0        0        0      486 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/border-radius.less
--rw-rw-rw-   0        0        0     1106 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/buttons.less
--rw-rw-rw-   0        0        0      127 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/center-block.less
--rw-rw-rw-   0        0        0      627 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/clearfix.less
--rw-rw-rw-   0        0        0     2634 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/forms.less
--rw-rw-rw-   0        0        0     4447 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/gradients.less
--rw-rw-rw-   0        0        0     2911 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/grid-framework.less
--rw-rw-rw-   0        0        0     3216 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/grid.less
--rw-rw-rw-   0        0        0      600 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/hide-text.less
--rw-rw-rw-   0        0        0     1167 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/image.less
--rw-rw-rw-   0        0        0      175 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/labels.less
--rw-rw-rw-   0        0        0      562 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/list-group.less
--rw-rw-rw-   0        0        0      242 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/nav-divider.less
--rw-rw-rw-   0        0        0      373 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/nav-vertical-align.less
--rw-rw-rw-   0        0        0      156 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/opacity.less
--rw-rw-rw-   0        0        0      461 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/pagination.less
--rw-rw-rw-   0        0        0      561 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/panels.less
--rw-rw-rw-   0        0        0      201 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/progress-bar.less
--rw-rw-rw-   0        0        0      256 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/reset-filter.less
--rw-rw-rw-   0        0        0      202 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/resize.less
--rw-rw-rw-   0        0        0      358 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/responsive-visibility.less
--rw-rw-rw-   0        0        0      137 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/size.less
--rw-rw-rw-   0        0        0      168 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/tab-focus.less
--rw-rw-rw-   0        0        0      728 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/table-row.less
--rw-rw-rw-   0        0        0      124 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/text-emphasis.less
--rw-rw-rw-   0        0        0      170 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/text-overflow.less
--rw-rw-rw-   0        0        0     6870 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/vendor-prefixes.less
--rw-rw-rw-   0        0        0     1141 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins.less
--rw-rw-rw-   0        0        0     3725 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/modals.less
--rw-rw-rw-   0        0        0    15343 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/navbar.less
--rw-rw-rw-   0        0        0     5167 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/navs.less
--rw-rw-rw-   0        0        0     8060 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/normalize.less
--rw-rw-rw-   0        0        0      912 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/pager.less
--rw-rw-rw-   0        0        0     2084 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/pagination.less
--rw-rw-rw-   0        0        0     5848 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/panels.less
--rw-rw-rw-   0        0        0     3539 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/popovers.less
--rw-rw-rw-   0        0        0     1714 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/print.less
--rw-rw-rw-   0        0        0     2314 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/progress-bars.less
--rw-rw-rw-   0        0        0      589 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/responsive-embed.less
--rw-rw-rw-   0        0        0     4456 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/responsive-utilities.less
--rw-rw-rw-   0        0        0     2793 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/scaffolding.less
--rw-rw-rw-   0        0        0     4712 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/tables.less
--rw-rw-rw-   0        0        0     7431 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/theme.less
--rw-rw-rw-   0        0        0      786 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/thumbnails.less
--rw-rw-rw-   0        0        0     2685 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/tooltip.less
--rw-rw-rw-   0        0        0     6402 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/type.less
--rw-rw-rw-   0        0        0      862 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/utilities.less
--rw-rw-rw-   0        0        0    27071 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/variables.less
--rw-rw-rw-   0        0        0      556 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/wells.less
--rw-rw-rw-   0        0        0     1105 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/LICENSE
--rw-rw-rw-   0        0        0     2103 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/package.json
--rw-rw-rw-   0        0        0     6010 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/bootstrap/README.md
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/static/js/holderjs/
--rw-rw-rw-   0        0        0      406 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/holderjs/.bower.json
--rw-rw-rw-   0        0        0       78 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/holderjs/.gitattributes
--rw-rw-rw-   0        0        0       48 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/holderjs/.gitignore
--rw-rw-rw-   0        0        0      177 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/holderjs/.jshintrc
--rw-rw-rw-   0        0        0       75 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/holderjs/bower.json
--rw-rw-rw-   0        0        0      827 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/holderjs/composer.json
--rw-rw-rw-   0        0        0     1159 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/holderjs/Gruntfile.js
--rw-rw-rw-   0        0        0    20918 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/holderjs/holder.js
--rw-rw-rw-   0        0        0      899 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/holderjs/package.json
--rw-rw-rw-   0        0        0     6754 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/holderjs/README.md
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/
--rw-rw-rw-   0        0        0      772 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/.bower.json
--rw-rw-rw-   0        0        0      462 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/bower.json
--rw-rw-rw-   0        0        0     1120 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/MIT-LICENSE.txt
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/ajax/
--rw-rw-rw-   0        0        0     2605 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/ajax/jsonp.js
--rw-rw-rw-   0        0        0     1744 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/ajax/load.js
--rw-rw-rw-   0        0        0      235 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/ajax/parseJSON.js
--rw-rw-rw-   0        0        0      513 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/ajax/parseXML.js
--rw-rw-rw-   0        0        0     1335 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/ajax/script.js
--rw-rw-rw-   0        0        0     3624 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/ajax/xhr.js
--rw-rw-rw-   0        0        0    21954 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/ajax.js
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/attributes/
--rw-rw-rw-   0        0        0     3461 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/attributes/attr.js
--rw-rw-rw-   0        0        0     4313 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/attributes/classes.js
--rw-rw-rw-   0        0        0     1948 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/attributes/prop.js
--rw-rw-rw-   0        0        0      928 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/attributes/support.js
--rw-rw-rw-   0        0        0     4000 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/attributes/val.js
--rw-rw-rw-   0        0        0      211 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/attributes.js
--rw-rw-rw-   0        0        0     5711 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/callbacks.js
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/core/
--rw-rw-rw-   0        0        0     1270 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/core/access.js
--rw-rw-rw-   0        0        0     3524 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/core/init.js
--rw-rw-rw-   0        0        0      977 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/core/parseHTML.js
--rw-rw-rw-   0        0        0     2478 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/core/ready.js
--rw-rw-rw-   0        0        0    12077 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/core.js
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/css/
--rw-rw-rw-   0        0        0      531 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/css/addGetHookIf.js
--rw-rw-rw-   0        0        0     1509 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/css/curCSS.js
--rw-rw-rw-   0        0        0     1937 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/css/defaultDisplay.js
--rw-rw-rw-   0        0        0      395 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/css/hiddenVisibleSelectors.js
--rw-rw-rw-   0        0        0     3294 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/css/support.js
--rw-rw-rw-   0        0        0      583 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/css/swap.js
--rw-rw-rw-   0        0        0    12796 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/css.js
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/data/
--rw-rw-rw-   0        0        0      403 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/data/accepts.js
--rw-rw-rw-   0        0        0     5063 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/data/Data.js
--rw-rw-rw-   0        0        0     5120 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/data.js
--rw-rw-rw-   0        0        0     4563 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/deferred.js
--rw-rw-rw-   0        0        0      236 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/deprecated.js
--rw-rw-rw-   0        0        0     1826 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/dimensions.js
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/effects/
--rw-rw-rw-   0        0        0      238 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/effects/animatedSelector.js
--rw-rw-rw-   0        0        0     3142 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/effects/Tween.js
--rw-rw-rw-   0        0        0    17562 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/effects.js
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/event/
--rw-rw-rw-   0        0        0      335 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/event/ajax.js
--rw-rw-rw-   0        0        0     1133 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/event/alias.js
--rw-rw-rw-   0        0        0      132 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/event/support.js
--rw-rw-rw-   0        0        0    25343 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/event.js
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/exports/
--rw-rw-rw-   0        0        0     1030 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/exports/amd.js
--rw-rw-rw-   0        0        0      673 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/exports/global.js
--rw-rw-rw-   0        0        0     1437 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/intro.js
--rw-rw-rw-   0        0        0      611 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/jquery.js
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/manipulation/
--rw-rw-rw-   0        0        0     1007 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/manipulation/support.js
--rw-rw-rw-   0        0        0      258 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/manipulation/_evalUrl.js
--rw-rw-rw-   0        0        0    15619 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/manipulation.js
--rw-rw-rw-   0        0        0     5795 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/offset.js
--rw-rw-rw-   0        0        0        6 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/outro.js
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/queue/
--rw-rw-rw-   0        0        0      583 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/queue/delay.js
--rw-rw-rw-   0        0        0     3205 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/queue.js
--rw-rw-rw-   0        0        0     4606 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/selector-native.js
--rw-rw-rw-   0        0        0      308 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/selector-sizzle.js
--rw-rw-rw-   0        0        0       34 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/selector.js
--rw-rw-rw-   0        0        0     3325 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/serialize.js
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/traversing/
--rw-rw-rw-   0        0        0     2564 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/traversing/findFilter.js
--rw-rw-rw-   0        0        0     4734 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/traversing.js
--rw-rw-rw-   0        0        0     1575 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery/src/wrap.js
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery-knob/
--rw-rw-rw-   0        0        0      615 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery-knob/.bower.json
--rw-rw-rw-   0        0        0       10 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery-knob/.gitignore
--rw-rw-rw-   0        0        0      286 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery-knob/bower.json
--rw-rw-rw-   0        0        0    27969 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery-knob/excanvas.js
--rw-rw-rw-   0        0        0    13363 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery-knob/index.html
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery-knob/js/
--rw-rw-rw-   0        0        0    26905 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery-knob/js/jquery.knob.js
--rw-rw-rw-   0        0        0     1021 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery-knob/knob.jquery.json
--rw-rw-rw-   0        0        0     1102 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery-knob/LICENSE
--rw-rw-rw-   0        0        0     3315 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery-knob/README.md
--rw-rw-rw-   0        0        0    33487 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/jquery-knob/secretplan.jpg
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/static/js/keen-js/
--rw-rw-rw-   0        0        0     1525 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/keen-js/.bower.json
--rw-rw-rw-   0        0        0     1222 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/keen-js/bower.json
--rw-rw-rw-   0        0        0     1100 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/keen-js/LICENSE
--rw-rw-rw-   0        0        0     1260 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/meta.js
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/chartpy_examples/static/js/slider/
--rw-rw-rw-   0        0        0     3995 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/slider/jQDateRangeSlider.js
--rw-rw-rw-   0        0        0     5000 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/slider/jQDateRangeSliderHandle.js
--rw-rw-rw-   0        0        0    20306 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/slider/jQRangeSlider.js
--rw-rw-rw-   0        0        0    13611 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/slider/jQRangeSliderBar.js
--rw-rw-rw-   0        0        0     3730 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/slider/jQRangeSliderDraggable.js
--rw-rw-rw-   0        0        0     8489 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/slider/jQRangeSliderHandle.js
--rw-rw-rw-   0        0        0    12731 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/slider/jQRangeSliderLabel.js
--rw-rw-rw-   0        0        0     2777 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/slider/jQRangeSliderMouseTouch.js
--rw-rw-rw-   0        0        0     2983 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/slider/jQRuler.js
--rw-rw-rw-   0        0        0    94842 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/slider/jquery-1.7.2.min.js
--rw-rw-rw-   0        0        0   201856 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/slider/jquery-ui.min.js
--rw-rw-rw-   0        0        0     2395 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/static/js/slider/slider.js
--rw-rw-rw-   0        0        0   397466 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/subplot.png
--rw-rw-rw-   0        0        0     2430 2018-02-19 16:08:04.000000 chartpy-0.1.8/chartpy_examples/subplot_examples.py
--rw-rw-rw-   0        0        0     1507 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/surface_examples.py
--rw-rw-rw-   0        0        0  1180464 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/temp.html
--rw-rw-rw-   0        0        0     4423 2017-11-15 12:21:28.000000 chartpy-0.1.8/chartpy_examples/vispy_demo.py
--rw-rw-rw-   0        0        0      628 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/volsurface.csv
--rw-rw-rw-   0        0        0   189742 2018-02-19 15:47:44.000000 chartpy-0.1.8/chartpy_examples/volsurface.png
--rw-rw-rw-   0        0        0     2143 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/xkcd_examples.py
--rw-rw-rw-   0        0        0       26 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_examples/__init__.py
--rw-rw-rw-   0        0        0    21473 2017-11-15 10:15:02.000000 chartpy-0.1.8/chartpy_logo.png
--rwxrwxrwx   0        0        0       41 2017-11-15 10:15:02.000000 chartpy-0.1.8/create_package.bat
--rw-rw-rw-   0        0        0      909 2019-02-12 12:18:14.000000 chartpy-0.1.8/create_python_package.md
-drwxrwxrwx   0        0        0        0 2020-06-08 10:45:55.000000 chartpy-0.1.8/doc/
--rw-rw-rw-   0        0        0        0 2017-11-15 10:15:02.000000 chartpy-0.1.8/doc/__init__.py
--rw-rw-rw-   0        0        0    11580 2017-11-15 10:15:02.000000 chartpy-0.1.8/LICENCE
--rw-rw-rw-   0        0        0      553 2019-02-12 12:20:00.000000 chartpy-0.1.8/longdesc.md
--rw-rw-rw-   0        0        0       29 2019-11-02 12:43:09.000000 chartpy-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0      939 2020-06-08 10:45:55.000000 chartpy-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     9358 2020-06-08 10:44:04.000000 chartpy-0.1.8/README.md
--rw-rw-rw-   0        0        0       42 2020-06-08 10:45:55.000000 chartpy-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1570 2020-06-08 10:45:45.000000 chartpy-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:26.851359 chartpy-0.1.9/
+-rw-rw-rw-   0        0        0       96 2017-11-15 10:15:02.000000 chartpy-0.1.9/.gitattributes
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:22.264597 chartpy-0.1.9/.github/
+-rw-rw-rw-   0        0        0      656 2020-07-01 07:02:55.000000 chartpy-0.1.9/.github/FUNDING.yml
+-rw-rw-rw-   0        0        0      887 2019-10-23 08:19:35.000000 chartpy-0.1.9/.gitignore
+-rw-rw-rw-   0        0        0    11580 2017-11-15 10:15:02.000000 chartpy-0.1.9/LICENCE
+-rw-rw-rw-   0        0        0       80 2021-01-23 00:06:30.000000 chartpy-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      939 2021-05-04 16:52:26.851359 chartpy-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0    10679 2021-05-04 16:49:07.000000 chartpy-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:22.301597 chartpy-0.1.9/chartpy/
+-rw-rw-rw-   0        0        0      217 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy/__init__.py
+-rw-rw-rw-   0        0        0    19244 2020-03-30 13:42:58.000000 chartpy-0.1.9/chartpy/canvas.py
+-rw-rw-rw-   0        0        0     4000 2021-05-03 18:07:33.000000 chartpy-0.1.9/chartpy/chart.py
+-rw-rw-rw-   0        0        0    12039 2021-05-03 18:07:33.000000 chartpy-0.1.9/chartpy/chartconstants.py
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:22.346599 chartpy-0.1.9/chartpy/dashboard/
+-rw-rw-rw-   0        0        0      223 2021-05-03 16:27:40.000000 chartpy-0.1.9/chartpy/dashboard/__init__.py
+-rw-rw-rw-   0        0        0     4179 2021-05-03 18:07:33.000000 chartpy-0.1.9/chartpy/dashboard/layoutcanvas.py
+-rw-rw-rw-   0        0        0    13350 2021-05-03 18:07:37.000000 chartpy-0.1.9/chartpy/dashboard/sessionmanager.py
+-rw-rw-rw-   0        0        0    30493 2021-05-04 12:50:44.000000 chartpy-0.1.9/chartpy/dashboard/sketchcomponents.py
+-rw-rw-rw-   0        0        0    97723 2021-04-19 10:31:03.000000 chartpy-0.1.9/chartpy/engine.py
+-rw-rw-rw-   0        0        0    31552 2021-04-19 10:10:05.000000 chartpy-0.1.9/chartpy/style.py
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:22.383116 chartpy-0.1.9/chartpy/stylesheets/
+-rw-rw-rw-   0        0        0     1026 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy/stylesheets/538-chartpy.mplstyle
+-rw-rw-rw-   0        0        0        0 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy/stylesheets/__init__.py
+-rw-rw-rw-   0        0        0     1299 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy/stylesheets/chartpy-pyfolio.mplstyle
+-rw-rw-rw-   0        0        0     1298 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy/stylesheets/chartpy.mplstyle
+-rw-rw-rw-   0        0        0     1198 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy/stylesheets/ggplot-chartpy.mplstyle
+-rw-rw-rw-   0        0        0     1111 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy/stylesheets/ggplot-tradtional.mplstyle
+-rw-rw-rw-   0        0        0     1957 2018-01-30 10:54:40.000000 chartpy-0.1.9/chartpy/twitter.py
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:22.337597 chartpy-0.1.9/chartpy.egg-info/
+-rw-rw-rw-   0        0        0      939 2021-05-04 16:52:21.000000 chartpy-0.1.9/chartpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    26967 2021-05-04 16:52:21.000000 chartpy-0.1.9/chartpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-05-04 16:52:21.000000 chartpy-0.1.9/chartpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2018-07-30 17:13:30.000000 chartpy-0.1.9/chartpy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      102 2021-05-04 16:52:21.000000 chartpy-0.1.9/chartpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2021-05-04 16:52:21.000000 chartpy-0.1.9/chartpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:23.061439 chartpy-0.1.9/chartpy_examples/
+-rw-rw-rw-   0        0        0       26 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/__init__.py
+-rw-rw-rw-   0        0        0   130032 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/barh.png
+-rw-rw-rw-   0        0        0    16866 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/bokeh.html
+-rw-rw-rw-   0        0        0   165869 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/canvas.png
+-rw-rw-rw-   0        0        0     2490 2019-08-06 09:34:12.000000 chartpy-0.1.9/chartpy_examples/canvas_demo.py
+-rw-rw-rw-   0        0        0     3847 2020-06-08 10:33:03.000000 chartpy-0.1.9/chartpy_examples/chart_demo.py
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:23.062441 chartpy-0.1.9/chartpy_examples/dashboard_examples/
+-rw-rw-rw-   0        0        0        0 2021-05-03 18:04:53.000000 chartpy-0.1.9/chartpy_examples/dashboard_examples/__init__.py
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:23.149448 chartpy-0.1.9/chartpy_examples/dashboard_examples/assets/
+-rw-rw-rw-   0        0        0    16326 2021-04-08 14:51:49.000000 chartpy-0.1.9/chartpy_examples/dashboard_examples/assets/android-chrome-192x192.png
+-rw-rw-rw-   0        0        0    24391 2021-04-08 14:51:49.000000 chartpy-0.1.9/chartpy_examples/dashboard_examples/assets/android-chrome-256x256.png
+-rw-rw-rw-   0        0        0    18838 2021-04-08 14:51:49.000000 chartpy-0.1.9/chartpy_examples/dashboard_examples/assets/android-chrome-512x512.png
+-rw-rw-rw-   0        0        0    14983 2021-04-08 14:51:49.000000 chartpy-0.1.9/chartpy_examples/dashboard_examples/assets/apple-touch-icon.png
+-rw-rw-rw-   0        0        0      246 2021-04-08 14:55:33.000000 chartpy-0.1.9/chartpy_examples/dashboard_examples/assets/browserconfig.xml
+-rw-rw-rw-   0        0        0      862 2021-04-08 14:51:49.000000 chartpy-0.1.9/chartpy_examples/dashboard_examples/assets/favicon-16x16.png
+-rw-rw-rw-   0        0        0     1558 2021-04-08 14:51:49.000000 chartpy-0.1.9/chartpy_examples/dashboard_examples/assets/favicon-32x32.png
+-rw-rw-rw-   0        0        0    10990 2021-04-08 14:51:49.000000 chartpy-0.1.9/chartpy_examples/dashboard_examples/assets/favicon.ico
+-rw-rw-rw-   0        0        0      418 2021-04-08 14:55:33.000000 chartpy-0.1.9/chartpy_examples/dashboard_examples/assets/head.htm
+-rw-rw-rw-   0        0        0    18369 2021-04-08 14:51:49.000000 chartpy-0.1.9/chartpy_examples/dashboard_examples/assets/logo.png
+-rw-rw-rw-   0        0        0    15426 2021-04-08 14:51:49.000000 chartpy-0.1.9/chartpy_examples/dashboard_examples/assets/logo_crop.png
+-rw-rw-rw-   0        0        0    11105 2021-04-08 14:51:49.000000 chartpy-0.1.9/chartpy_examples/dashboard_examples/assets/mstile-150x150.png
+-rw-rw-rw-   0        0        0    14297 2021-04-08 14:55:33.000000 chartpy-0.1.9/chartpy_examples/dashboard_examples/assets/safari-pinned-tab.svg
+-rw-rw-rw-   0        0        0      426 2021-04-08 14:55:33.000000 chartpy-0.1.9/chartpy_examples/dashboard_examples/assets/site.webmanifest
+-rw-rw-rw-   0        0        0    10516 2021-04-08 14:55:33.000000 chartpy-0.1.9/chartpy_examples/dashboard_examples/assets/tabs.css
+-rw-rw-rw-   0        0        0    71102 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/heatmap.png
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:23.625587 chartpy-0.1.9/chartpy_examples/notebooks/
+-rw-rw-rw-   0        0        0        0 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/__init__.py
+-rw-rw-rw-   0        0        0  1322629 2018-04-20 09:14:22.000000 chartpy-0.1.9/chartpy_examples/notebooks/chart_examples.ipynb
+-rw-rw-rw-   0        0        0    16107 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/s_bokeh.html
+-rw-rw-rw-   0        0        0     3325 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/s_canvas.html
+-rw-rw-rw-   0        0        0     3275 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/s_canvas_keen.html
+-rw-rw-rw-   0        0        0     4320 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/s_canvas_plain.html
+-rw-rw-rw-   0        0        0    35180 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/s_matplotlib.png
+-rw-rw-rw-   0        0        0  1230282 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/s_plotly.html
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:22.184423 chartpy-0.1.9/chartpy_examples/notebooks/static/
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:23.667585 chartpy-0.1.9/chartpy_examples/notebooks/static/css/
+-rw-rw-rw-   0        0        0   109522 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/css/bootstrap.min.css
+-rw-rw-rw-   0        0        0     6112 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/css/iThing.css
+-rw-rw-rw-   0        0        0     1526 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/css/keen-dashboards.css
+-rw-rw-rw-   0        0        0     2716 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/css/keen-static.css
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:23.712457 chartpy-0.1.9/chartpy_examples/notebooks/static/fonts/
+-rw-rw-rw-   0        0        0    20335 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/fonts/glyphicons-halflings-regular.eot
+-rw-rw-rw-   0        0        0    63155 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/fonts/glyphicons-halflings-regular.svg
+-rw-rw-rw-   0        0        0    41280 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/fonts/glyphicons-halflings-regular.ttf
+-rw-rw-rw-   0        0        0    23320 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/fonts/glyphicons-halflings-regular.woff
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:23.723547 chartpy-0.1.9/chartpy_examples/notebooks/static/js/
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:23.772065 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/
+-rw-rw-rw-   0        0        0     1171 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/.bower.json
+-rw-rw-rw-   0        0        0    13428 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/Gruntfile.js
+-rw-rw-rw-   0        0        0     1105 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/LICENSE
+-rw-rw-rw-   0        0        0     6010 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/README.md
+-rw-rw-rw-   0        0        0      887 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/bower.json
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:23.813064 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/fonts/
+-rw-rw-rw-   0        0        0    20335 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/fonts/glyphicons-halflings-regular.eot
+-rw-rw-rw-   0        0        0    63155 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/fonts/glyphicons-halflings-regular.svg
+-rw-rw-rw-   0        0        0    41280 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/fonts/glyphicons-halflings-regular.ttf
+-rw-rw-rw-   0        0        0    23320 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/fonts/glyphicons-halflings-regular.woff
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:23.856064 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/grunt/
+-rw-rw-rw-   0        0        0     1434 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/grunt/bs-glyphicons-data-generator.js
+-rw-rw-rw-   0        0        0     6301 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/grunt/bs-lessdoc-parser.js
+-rw-rw-rw-   0        0        0     1422 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/grunt/bs-raw-files-generator.js
+-rw-rw-rw-   0        0        0     1517 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/grunt/sauce_browsers.yml
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:24.005065 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/js/
+-rw-rw-rw-   0        0        0     4244 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/js/affix.js
+-rw-rw-rw-   0        0        0     2320 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/js/alert.js
+-rw-rw-rw-   0        0        0     3085 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/js/button.js
+-rw-rw-rw-   0        0        0     6749 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/js/carousel.js
+-rw-rw-rw-   0        0        0     5042 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/js/collapse.js
+-rw-rw-rw-   0        0        0     4536 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/js/dropdown.js
+-rw-rw-rw-   0        0        0     8220 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/js/modal.js
+-rw-rw-rw-   0        0        0     3373 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/js/popover.js
+-rw-rw-rw-   0        0        0     4811 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/js/scrollspy.js
+-rw-rw-rw-   0        0        0     3127 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/js/tab.js
+-rw-rw-rw-   0        0        0    15099 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/js/tooltip.js
+-rw-rw-rw-   0        0        0     1890 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/js/transition.js
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:24.421931 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/
+-rw-rw-rw-   0        0        0     1581 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/alerts.less
+-rw-rw-rw-   0        0        0     1124 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/badges.less
+-rw-rw-rw-   0        0        0     1171 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/bootstrap.less
+-rw-rw-rw-   0        0        0      620 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/breadcrumbs.less
+-rw-rw-rw-   0        0        0     5724 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/button-groups.less
+-rw-rw-rw-   0        0        0     3657 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/buttons.less
+-rw-rw-rw-   0        0        0     5002 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/carousel.less
+-rw-rw-rw-   0        0        0      716 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/close.less
+-rw-rw-rw-   0        0        0     1446 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/code.less
+-rw-rw-rw-   0        0        0      616 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/component-animations.less
+-rw-rw-rw-   0        0        0     4997 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/dropdowns.less
+-rw-rw-rw-   0        0        0    14274 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/forms.less
+-rw-rw-rw-   0        0        0    15095 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/glyphicons.less
+-rw-rw-rw-   0        0        0     1471 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/grid.less
+-rw-rw-rw-   0        0        0     4381 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/input-groups.less
+-rw-rw-rw-   0        0        0     1013 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/jumbotron.less
+-rw-rw-rw-   0        0        0     1143 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/labels.less
+-rw-rw-rw-   0        0        0     3244 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/list-group.less
+-rw-rw-rw-   0        0        0      904 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/media.less
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:24.714213 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/
+-rw-rw-rw-   0        0        0      271 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/alerts.less
+-rw-rw-rw-   0        0        0      147 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/background-variant.less
+-rw-rw-rw-   0        0        0      486 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/border-radius.less
+-rw-rw-rw-   0        0        0     1106 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/buttons.less
+-rw-rw-rw-   0        0        0      127 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/center-block.less
+-rw-rw-rw-   0        0        0      627 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/clearfix.less
+-rw-rw-rw-   0        0        0     2634 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/forms.less
+-rw-rw-rw-   0        0        0     4447 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/gradients.less
+-rw-rw-rw-   0        0        0     2911 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/grid-framework.less
+-rw-rw-rw-   0        0        0     3216 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/grid.less
+-rw-rw-rw-   0        0        0      600 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/hide-text.less
+-rw-rw-rw-   0        0        0     1167 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/image.less
+-rw-rw-rw-   0        0        0      175 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/labels.less
+-rw-rw-rw-   0        0        0      562 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/list-group.less
+-rw-rw-rw-   0        0        0      242 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/nav-divider.less
+-rw-rw-rw-   0        0        0      373 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/nav-vertical-align.less
+-rw-rw-rw-   0        0        0      156 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/opacity.less
+-rw-rw-rw-   0        0        0      461 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/pagination.less
+-rw-rw-rw-   0        0        0      561 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/panels.less
+-rw-rw-rw-   0        0        0      201 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/progress-bar.less
+-rw-rw-rw-   0        0        0      256 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/reset-filter.less
+-rw-rw-rw-   0        0        0      202 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/resize.less
+-rw-rw-rw-   0        0        0      358 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/responsive-visibility.less
+-rw-rw-rw-   0        0        0      137 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/size.less
+-rw-rw-rw-   0        0        0      168 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/tab-focus.less
+-rw-rw-rw-   0        0        0      728 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/table-row.less
+-rw-rw-rw-   0        0        0      124 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/text-emphasis.less
+-rw-rw-rw-   0        0        0      170 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/text-overflow.less
+-rw-rw-rw-   0        0        0     6870 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/vendor-prefixes.less
+-rw-rw-rw-   0        0        0     1141 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins.less
+-rw-rw-rw-   0        0        0     3725 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/modals.less
+-rw-rw-rw-   0        0        0    15343 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/navbar.less
+-rw-rw-rw-   0        0        0     5167 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/navs.less
+-rw-rw-rw-   0        0        0     8060 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/normalize.less
+-rw-rw-rw-   0        0        0      912 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/pager.less
+-rw-rw-rw-   0        0        0     2084 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/pagination.less
+-rw-rw-rw-   0        0        0     5848 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/panels.less
+-rw-rw-rw-   0        0        0     3539 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/popovers.less
+-rw-rw-rw-   0        0        0     1714 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/print.less
+-rw-rw-rw-   0        0        0     2314 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/progress-bars.less
+-rw-rw-rw-   0        0        0      589 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/responsive-embed.less
+-rw-rw-rw-   0        0        0     4456 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/responsive-utilities.less
+-rw-rw-rw-   0        0        0     2793 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/scaffolding.less
+-rw-rw-rw-   0        0        0     4712 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/tables.less
+-rw-rw-rw-   0        0        0     7431 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/theme.less
+-rw-rw-rw-   0        0        0      786 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/thumbnails.less
+-rw-rw-rw-   0        0        0     2685 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/tooltip.less
+-rw-rw-rw-   0        0        0     6402 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/type.less
+-rw-rw-rw-   0        0        0      862 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/utilities.less
+-rw-rw-rw-   0        0        0    27071 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/variables.less
+-rw-rw-rw-   0        0        0      556 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/wells.less
+-rw-rw-rw-   0        0        0     2103 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/package.json
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:24.802159 chartpy-0.1.9/chartpy_examples/notebooks/static/js/holderjs/
+-rw-rw-rw-   0        0        0      406 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/holderjs/.bower.json
+-rw-rw-rw-   0        0        0       78 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/holderjs/.gitattributes
+-rw-rw-rw-   0        0        0       48 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/holderjs/.gitignore
+-rw-rw-rw-   0        0        0      177 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/holderjs/.jshintrc
+-rw-rw-rw-   0        0        0     1159 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/holderjs/Gruntfile.js
+-rw-rw-rw-   0        0        0     6754 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/holderjs/README.md
+-rw-rw-rw-   0        0        0       75 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/holderjs/bower.json
+-rw-rw-rw-   0        0        0      827 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/holderjs/composer.json
+-rw-rw-rw-   0        0        0    20918 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/holderjs/holder.js
+-rw-rw-rw-   0        0        0      899 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/holderjs/package.json
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:24.823160 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/
+-rw-rw-rw-   0        0        0      772 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/.bower.json
+-rw-rw-rw-   0        0        0     1120 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/MIT-LICENSE.txt
+-rw-rw-rw-   0        0        0      462 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/bower.json
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:25.241654 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:25.311847 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/ajax/
+-rw-rw-rw-   0        0        0     2605 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/ajax/jsonp.js
+-rw-rw-rw-   0        0        0     1744 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/ajax/load.js
+-rw-rw-rw-   0        0        0      235 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/ajax/parseJSON.js
+-rw-rw-rw-   0        0        0      513 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/ajax/parseXML.js
+-rw-rw-rw-   0        0        0     1335 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/ajax/script.js
+-rw-rw-rw-   0        0        0     3624 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/ajax/xhr.js
+-rw-rw-rw-   0        0        0    21954 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/ajax.js
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:25.368846 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/attributes/
+-rw-rw-rw-   0        0        0     3461 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/attributes/attr.js
+-rw-rw-rw-   0        0        0     4313 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/attributes/classes.js
+-rw-rw-rw-   0        0        0     1948 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/attributes/prop.js
+-rw-rw-rw-   0        0        0      928 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/attributes/support.js
+-rw-rw-rw-   0        0        0     4000 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/attributes/val.js
+-rw-rw-rw-   0        0        0      211 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/attributes.js
+-rw-rw-rw-   0        0        0     5711 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/callbacks.js
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:25.413846 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/core/
+-rw-rw-rw-   0        0        0     1270 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/core/access.js
+-rw-rw-rw-   0        0        0     3524 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/core/init.js
+-rw-rw-rw-   0        0        0      977 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/core/parseHTML.js
+-rw-rw-rw-   0        0        0     2478 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/core/ready.js
+-rw-rw-rw-   0        0        0    12077 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/core.js
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:25.481849 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/css/
+-rw-rw-rw-   0        0        0      531 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/css/addGetHookIf.js
+-rw-rw-rw-   0        0        0     1509 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/css/curCSS.js
+-rw-rw-rw-   0        0        0     1937 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/css/defaultDisplay.js
+-rw-rw-rw-   0        0        0      395 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/css/hiddenVisibleSelectors.js
+-rw-rw-rw-   0        0        0     3294 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/css/support.js
+-rw-rw-rw-   0        0        0      583 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/css/swap.js
+-rw-rw-rw-   0        0        0    12796 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/css.js
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:25.504847 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/data/
+-rw-rw-rw-   0        0        0     5063 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/data/Data.js
+-rw-rw-rw-   0        0        0      403 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/data/accepts.js
+-rw-rw-rw-   0        0        0     5120 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/data.js
+-rw-rw-rw-   0        0        0     4563 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/deferred.js
+-rw-rw-rw-   0        0        0      236 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/deprecated.js
+-rw-rw-rw-   0        0        0     1826 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/dimensions.js
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:25.526849 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/effects/
+-rw-rw-rw-   0        0        0     3142 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/effects/Tween.js
+-rw-rw-rw-   0        0        0      238 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/effects/animatedSelector.js
+-rw-rw-rw-   0        0        0    17562 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/effects.js
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:25.557230 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/event/
+-rw-rw-rw-   0        0        0      335 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/event/ajax.js
+-rw-rw-rw-   0        0        0     1133 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/event/alias.js
+-rw-rw-rw-   0        0        0      132 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/event/support.js
+-rw-rw-rw-   0        0        0    25343 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/event.js
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:25.576230 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/exports/
+-rw-rw-rw-   0        0        0     1030 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/exports/amd.js
+-rw-rw-rw-   0        0        0      673 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/exports/global.js
+-rw-rw-rw-   0        0        0     1437 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/intro.js
+-rw-rw-rw-   0        0        0      611 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/jquery.js
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:25.597229 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/manipulation/
+-rw-rw-rw-   0        0        0      258 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/manipulation/_evalUrl.js
+-rw-rw-rw-   0        0        0     1007 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/manipulation/support.js
+-rw-rw-rw-   0        0        0    15619 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/manipulation.js
+-rw-rw-rw-   0        0        0     5795 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/offset.js
+-rw-rw-rw-   0        0        0        6 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/outro.js
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:25.607230 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/queue/
+-rw-rw-rw-   0        0        0      583 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/queue/delay.js
+-rw-rw-rw-   0        0        0     3205 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/queue.js
+-rw-rw-rw-   0        0        0     4606 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/selector-native.js
+-rw-rw-rw-   0        0        0      308 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/selector-sizzle.js
+-rw-rw-rw-   0        0        0       34 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/selector.js
+-rw-rw-rw-   0        0        0     3325 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/serialize.js
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:25.619230 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/traversing/
+-rw-rw-rw-   0        0        0     2564 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/traversing/findFilter.js
+-rw-rw-rw-   0        0        0     4734 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/traversing.js
+-rw-rw-rw-   0        0        0     1575 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/wrap.js
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:24.928162 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery-knob/
+-rw-rw-rw-   0        0        0      615 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery-knob/.bower.json
+-rw-rw-rw-   0        0        0       10 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery-knob/.gitignore
+-rw-rw-rw-   0        0        0     1102 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery-knob/LICENSE
+-rw-rw-rw-   0        0        0     3315 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery-knob/README.md
+-rw-rw-rw-   0        0        0      286 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery-knob/bower.json
+-rw-rw-rw-   0        0        0    27969 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery-knob/excanvas.js
+-rw-rw-rw-   0        0        0    13363 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery-knob/index.html
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:24.943160 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery-knob/js/
+-rw-rw-rw-   0        0        0    26905 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery-knob/js/jquery.knob.js
+-rw-rw-rw-   0        0        0     1021 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery-knob/knob.jquery.json
+-rw-rw-rw-   0        0        0    33487 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery-knob/secretplan.jpg
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:25.640230 chartpy-0.1.9/chartpy_examples/notebooks/static/js/keen-js/
+-rw-rw-rw-   0        0        0     1525 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/keen-js/.bower.json
+-rw-rw-rw-   0        0        0     1100 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/keen-js/LICENSE
+-rw-rw-rw-   0        0        0     1222 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/keen-js/bower.json
+-rw-rw-rw-   0        0        0     1260 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/meta.js
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:25.865901 chartpy-0.1.9/chartpy_examples/notebooks/static/js/slider/
+-rw-rw-rw-   0        0        0     3995 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/slider/jQDateRangeSlider.js
+-rw-rw-rw-   0        0        0     5000 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/slider/jQDateRangeSliderHandle.js
+-rw-rw-rw-   0        0        0    20306 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/slider/jQRangeSlider.js
+-rw-rw-rw-   0        0        0    13611 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/slider/jQRangeSliderBar.js
+-rw-rw-rw-   0        0        0     3730 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/slider/jQRangeSliderDraggable.js
+-rw-rw-rw-   0        0        0     8489 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/slider/jQRangeSliderHandle.js
+-rw-rw-rw-   0        0        0    12731 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/slider/jQRangeSliderLabel.js
+-rw-rw-rw-   0        0        0     2777 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/slider/jQRangeSliderMouseTouch.js
+-rw-rw-rw-   0        0        0     2983 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/slider/jQRuler.js
+-rw-rw-rw-   0        0        0    94842 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/slider/jquery-1.7.2.min.js
+-rw-rw-rw-   0        0        0   201856 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/slider/jquery-ui.min.js
+-rw-rw-rw-   0        0        0     2395 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/notebooks/static/js/slider/slider.js
+-rw-rw-rw-   0        0        0    60965 2018-04-20 09:14:30.000000 chartpy-0.1.9/chartpy_examples/notebooks/web_page_examples.ipynb
+-rw-rw-rw-   0        0        0  1231027 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/plotly.html
+-rw-rw-rw-   0        0        0    45314 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/plotlyheatmap.png
+-rw-rw-rw-   0        0        0    76404 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/screenshot.png
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:22.195088 chartpy-0.1.9/chartpy_examples/static/
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:25.890900 chartpy-0.1.9/chartpy_examples/static/css/
+-rw-rw-rw-   0        0        0   109522 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/css/bootstrap.min.css
+-rw-rw-rw-   0        0        0     6112 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/css/iThing.css
+-rw-rw-rw-   0        0        0     1526 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/css/keen-dashboards.css
+-rw-rw-rw-   0        0        0     2716 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/css/keen-static.css
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:25.931901 chartpy-0.1.9/chartpy_examples/static/fonts/
+-rw-rw-rw-   0        0        0    20335 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/fonts/glyphicons-halflings-regular.eot
+-rw-rw-rw-   0        0        0    63155 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/fonts/glyphicons-halflings-regular.svg
+-rw-rw-rw-   0        0        0    41280 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/fonts/glyphicons-halflings-regular.ttf
+-rw-rw-rw-   0        0        0    23320 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/fonts/glyphicons-halflings-regular.woff
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:25.934899 chartpy-0.1.9/chartpy_examples/static/js/
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:25.958945 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/
+-rw-rw-rw-   0        0        0     1171 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/.bower.json
+-rw-rw-rw-   0        0        0    13428 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/Gruntfile.js
+-rw-rw-rw-   0        0        0     1105 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/LICENSE
+-rw-rw-rw-   0        0        0     6010 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/README.md
+-rw-rw-rw-   0        0        0      887 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/bower.json
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:25.999945 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/fonts/
+-rw-rw-rw-   0        0        0    20335 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/fonts/glyphicons-halflings-regular.eot
+-rw-rw-rw-   0        0        0    63155 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/fonts/glyphicons-halflings-regular.svg
+-rw-rw-rw-   0        0        0    41280 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/fonts/glyphicons-halflings-regular.ttf
+-rw-rw-rw-   0        0        0    23320 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/fonts/glyphicons-halflings-regular.woff
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:26.007945 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/grunt/
+-rw-rw-rw-   0        0        0     1434 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/grunt/bs-glyphicons-data-generator.js
+-rw-rw-rw-   0        0        0     6301 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/grunt/bs-lessdoc-parser.js
+-rw-rw-rw-   0        0        0     1422 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/grunt/bs-raw-files-generator.js
+-rw-rw-rw-   0        0        0     1517 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/grunt/sauce_browsers.yml
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:26.097788 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/js/
+-rw-rw-rw-   0        0        0     4244 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/js/affix.js
+-rw-rw-rw-   0        0        0     2320 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/js/alert.js
+-rw-rw-rw-   0        0        0     3085 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/js/button.js
+-rw-rw-rw-   0        0        0     6749 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/js/carousel.js
+-rw-rw-rw-   0        0        0     5042 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/js/collapse.js
+-rw-rw-rw-   0        0        0     4536 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/js/dropdown.js
+-rw-rw-rw-   0        0        0     8220 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/js/modal.js
+-rw-rw-rw-   0        0        0     3373 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/js/popover.js
+-rw-rw-rw-   0        0        0     4811 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/js/scrollspy.js
+-rw-rw-rw-   0        0        0     3127 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/js/tab.js
+-rw-rw-rw-   0        0        0    15099 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/js/tooltip.js
+-rw-rw-rw-   0        0        0     1890 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/js/transition.js
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:26.256037 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/
+-rw-rw-rw-   0        0        0     1581 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/alerts.less
+-rw-rw-rw-   0        0        0     1124 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/badges.less
+-rw-rw-rw-   0        0        0     1171 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/bootstrap.less
+-rw-rw-rw-   0        0        0      620 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/breadcrumbs.less
+-rw-rw-rw-   0        0        0     5724 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/button-groups.less
+-rw-rw-rw-   0        0        0     3657 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/buttons.less
+-rw-rw-rw-   0        0        0     5002 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/carousel.less
+-rw-rw-rw-   0        0        0      716 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/close.less
+-rw-rw-rw-   0        0        0     1446 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/code.less
+-rw-rw-rw-   0        0        0      616 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/component-animations.less
+-rw-rw-rw-   0        0        0     4997 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/dropdowns.less
+-rw-rw-rw-   0        0        0    14274 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/forms.less
+-rw-rw-rw-   0        0        0    15095 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/glyphicons.less
+-rw-rw-rw-   0        0        0     1471 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/grid.less
+-rw-rw-rw-   0        0        0     4381 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/input-groups.less
+-rw-rw-rw-   0        0        0     1013 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/jumbotron.less
+-rw-rw-rw-   0        0        0     1143 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/labels.less
+-rw-rw-rw-   0        0        0     3244 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/list-group.less
+-rw-rw-rw-   0        0        0      904 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/media.less
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:26.312301 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/
+-rw-rw-rw-   0        0        0      271 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/alerts.less
+-rw-rw-rw-   0        0        0      147 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/background-variant.less
+-rw-rw-rw-   0        0        0      486 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/border-radius.less
+-rw-rw-rw-   0        0        0     1106 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/buttons.less
+-rw-rw-rw-   0        0        0      127 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/center-block.less
+-rw-rw-rw-   0        0        0      627 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/clearfix.less
+-rw-rw-rw-   0        0        0     2634 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/forms.less
+-rw-rw-rw-   0        0        0     4447 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/gradients.less
+-rw-rw-rw-   0        0        0     2911 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/grid-framework.less
+-rw-rw-rw-   0        0        0     3216 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/grid.less
+-rw-rw-rw-   0        0        0      600 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/hide-text.less
+-rw-rw-rw-   0        0        0     1167 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/image.less
+-rw-rw-rw-   0        0        0      175 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/labels.less
+-rw-rw-rw-   0        0        0      562 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/list-group.less
+-rw-rw-rw-   0        0        0      242 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/nav-divider.less
+-rw-rw-rw-   0        0        0      373 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/nav-vertical-align.less
+-rw-rw-rw-   0        0        0      156 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/opacity.less
+-rw-rw-rw-   0        0        0      461 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/pagination.less
+-rw-rw-rw-   0        0        0      561 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/panels.less
+-rw-rw-rw-   0        0        0      201 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/progress-bar.less
+-rw-rw-rw-   0        0        0      256 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/reset-filter.less
+-rw-rw-rw-   0        0        0      202 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/resize.less
+-rw-rw-rw-   0        0        0      358 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/responsive-visibility.less
+-rw-rw-rw-   0        0        0      137 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/size.less
+-rw-rw-rw-   0        0        0      168 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/tab-focus.less
+-rw-rw-rw-   0        0        0      728 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/table-row.less
+-rw-rw-rw-   0        0        0      124 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/text-emphasis.less
+-rw-rw-rw-   0        0        0      170 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/text-overflow.less
+-rw-rw-rw-   0        0        0     6870 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/vendor-prefixes.less
+-rw-rw-rw-   0        0        0     1141 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins.less
+-rw-rw-rw-   0        0        0     3725 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/modals.less
+-rw-rw-rw-   0        0        0    15343 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/navbar.less
+-rw-rw-rw-   0        0        0     5167 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/navs.less
+-rw-rw-rw-   0        0        0     8060 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/normalize.less
+-rw-rw-rw-   0        0        0      912 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/pager.less
+-rw-rw-rw-   0        0        0     2084 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/pagination.less
+-rw-rw-rw-   0        0        0     5848 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/panels.less
+-rw-rw-rw-   0        0        0     3539 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/popovers.less
+-rw-rw-rw-   0        0        0     1714 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/print.less
+-rw-rw-rw-   0        0        0     2314 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/progress-bars.less
+-rw-rw-rw-   0        0        0      589 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/responsive-embed.less
+-rw-rw-rw-   0        0        0     4456 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/responsive-utilities.less
+-rw-rw-rw-   0        0        0     2793 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/scaffolding.less
+-rw-rw-rw-   0        0        0     4712 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/tables.less
+-rw-rw-rw-   0        0        0     7431 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/theme.less
+-rw-rw-rw-   0        0        0      786 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/thumbnails.less
+-rw-rw-rw-   0        0        0     2685 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/tooltip.less
+-rw-rw-rw-   0        0        0     6402 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/type.less
+-rw-rw-rw-   0        0        0      862 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/utilities.less
+-rw-rw-rw-   0        0        0    27071 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/variables.less
+-rw-rw-rw-   0        0        0      556 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/wells.less
+-rw-rw-rw-   0        0        0     2103 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/bootstrap/package.json
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:26.360303 chartpy-0.1.9/chartpy_examples/static/js/holderjs/
+-rw-rw-rw-   0        0        0      406 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/holderjs/.bower.json
+-rw-rw-rw-   0        0        0       78 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/holderjs/.gitattributes
+-rw-rw-rw-   0        0        0       48 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/holderjs/.gitignore
+-rw-rw-rw-   0        0        0      177 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/holderjs/.jshintrc
+-rw-rw-rw-   0        0        0     1159 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/holderjs/Gruntfile.js
+-rw-rw-rw-   0        0        0     6754 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/holderjs/README.md
+-rw-rw-rw-   0        0        0       75 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/holderjs/bower.json
+-rw-rw-rw-   0        0        0      827 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/holderjs/composer.json
+-rw-rw-rw-   0        0        0    20918 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/holderjs/holder.js
+-rw-rw-rw-   0        0        0      899 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/holderjs/package.json
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:26.370303 chartpy-0.1.9/chartpy_examples/static/js/jquery/
+-rw-rw-rw-   0        0        0      772 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/.bower.json
+-rw-rw-rw-   0        0        0     1120 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/MIT-LICENSE.txt
+-rw-rw-rw-   0        0        0      462 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/bower.json
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:26.569287 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:26.581059 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/ajax/
+-rw-rw-rw-   0        0        0     2605 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/ajax/jsonp.js
+-rw-rw-rw-   0        0        0     1744 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/ajax/load.js
+-rw-rw-rw-   0        0        0      235 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/ajax/parseJSON.js
+-rw-rw-rw-   0        0        0      513 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/ajax/parseXML.js
+-rw-rw-rw-   0        0        0     1335 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/ajax/script.js
+-rw-rw-rw-   0        0        0     3624 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/ajax/xhr.js
+-rw-rw-rw-   0        0        0    21954 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/ajax.js
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:26.590061 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/attributes/
+-rw-rw-rw-   0        0        0     3461 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/attributes/attr.js
+-rw-rw-rw-   0        0        0     4313 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/attributes/classes.js
+-rw-rw-rw-   0        0        0     1948 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/attributes/prop.js
+-rw-rw-rw-   0        0        0      928 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/attributes/support.js
+-rw-rw-rw-   0        0        0     4000 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/attributes/val.js
+-rw-rw-rw-   0        0        0      211 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/attributes.js
+-rw-rw-rw-   0        0        0     5711 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/callbacks.js
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:26.603061 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/core/
+-rw-rw-rw-   0        0        0     1270 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/core/access.js
+-rw-rw-rw-   0        0        0     3524 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/core/init.js
+-rw-rw-rw-   0        0        0      977 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/core/parseHTML.js
+-rw-rw-rw-   0        0        0     2478 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/core/ready.js
+-rw-rw-rw-   0        0        0    12077 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/core.js
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:26.633060 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/css/
+-rw-rw-rw-   0        0        0      531 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/css/addGetHookIf.js
+-rw-rw-rw-   0        0        0     1509 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/css/curCSS.js
+-rw-rw-rw-   0        0        0     1937 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/css/defaultDisplay.js
+-rw-rw-rw-   0        0        0      395 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/css/hiddenVisibleSelectors.js
+-rw-rw-rw-   0        0        0     3294 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/css/support.js
+-rw-rw-rw-   0        0        0      583 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/css/swap.js
+-rw-rw-rw-   0        0        0    12796 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/css.js
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:26.646060 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/data/
+-rw-rw-rw-   0        0        0     5063 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/data/Data.js
+-rw-rw-rw-   0        0        0      403 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/data/accepts.js
+-rw-rw-rw-   0        0        0     5120 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/data.js
+-rw-rw-rw-   0        0        0     4563 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/deferred.js
+-rw-rw-rw-   0        0        0      236 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/deprecated.js
+-rw-rw-rw-   0        0        0     1826 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/dimensions.js
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:26.650062 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/effects/
+-rw-rw-rw-   0        0        0     3142 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/effects/Tween.js
+-rw-rw-rw-   0        0        0      238 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/effects/animatedSelector.js
+-rw-rw-rw-   0        0        0    17562 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/effects.js
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:26.657059 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/event/
+-rw-rw-rw-   0        0        0      335 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/event/ajax.js
+-rw-rw-rw-   0        0        0     1133 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/event/alias.js
+-rw-rw-rw-   0        0        0      132 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/event/support.js
+-rw-rw-rw-   0        0        0    25343 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/event.js
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:26.660060 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/exports/
+-rw-rw-rw-   0        0        0     1030 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/exports/amd.js
+-rw-rw-rw-   0        0        0      673 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/exports/global.js
+-rw-rw-rw-   0        0        0     1437 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/intro.js
+-rw-rw-rw-   0        0        0      611 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/jquery.js
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:26.663061 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/manipulation/
+-rw-rw-rw-   0        0        0      258 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/manipulation/_evalUrl.js
+-rw-rw-rw-   0        0        0     1007 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/manipulation/support.js
+-rw-rw-rw-   0        0        0    15619 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/manipulation.js
+-rw-rw-rw-   0        0        0     5795 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/offset.js
+-rw-rw-rw-   0        0        0        6 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/outro.js
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:26.665060 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/queue/
+-rw-rw-rw-   0        0        0      583 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/queue/delay.js
+-rw-rw-rw-   0        0        0     3205 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/queue.js
+-rw-rw-rw-   0        0        0     4606 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/selector-native.js
+-rw-rw-rw-   0        0        0      308 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/selector-sizzle.js
+-rw-rw-rw-   0        0        0       34 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/selector.js
+-rw-rw-rw-   0        0        0     3325 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/serialize.js
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:26.667060 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/traversing/
+-rw-rw-rw-   0        0        0     2564 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/traversing/findFilter.js
+-rw-rw-rw-   0        0        0     4734 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/traversing.js
+-rw-rw-rw-   0        0        0     1575 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery/src/wrap.js
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:26.428303 chartpy-0.1.9/chartpy_examples/static/js/jquery-knob/
+-rw-rw-rw-   0        0        0      615 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery-knob/.bower.json
+-rw-rw-rw-   0        0        0       10 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery-knob/.gitignore
+-rw-rw-rw-   0        0        0     1102 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery-knob/LICENSE
+-rw-rw-rw-   0        0        0     3315 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery-knob/README.md
+-rw-rw-rw-   0        0        0      286 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery-knob/bower.json
+-rw-rw-rw-   0        0        0    27969 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery-knob/excanvas.js
+-rw-rw-rw-   0        0        0    13363 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery-knob/index.html
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:26.444303 chartpy-0.1.9/chartpy_examples/static/js/jquery-knob/js/
+-rw-rw-rw-   0        0        0    26905 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery-knob/js/jquery.knob.js
+-rw-rw-rw-   0        0        0     1021 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery-knob/knob.jquery.json
+-rw-rw-rw-   0        0        0    33487 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/jquery-knob/secretplan.jpg
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:26.673060 chartpy-0.1.9/chartpy_examples/static/js/keen-js/
+-rw-rw-rw-   0        0        0     1525 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/keen-js/.bower.json
+-rw-rw-rw-   0        0        0     1100 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/keen-js/LICENSE
+-rw-rw-rw-   0        0        0     1222 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/keen-js/bower.json
+-rw-rw-rw-   0        0        0     1260 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/meta.js
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:26.849359 chartpy-0.1.9/chartpy_examples/static/js/slider/
+-rw-rw-rw-   0        0        0     3995 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/slider/jQDateRangeSlider.js
+-rw-rw-rw-   0        0        0     5000 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/slider/jQDateRangeSliderHandle.js
+-rw-rw-rw-   0        0        0    20306 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/slider/jQRangeSlider.js
+-rw-rw-rw-   0        0        0    13611 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/slider/jQRangeSliderBar.js
+-rw-rw-rw-   0        0        0     3730 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/slider/jQRangeSliderDraggable.js
+-rw-rw-rw-   0        0        0     8489 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/slider/jQRangeSliderHandle.js
+-rw-rw-rw-   0        0        0    12731 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/slider/jQRangeSliderLabel.js
+-rw-rw-rw-   0        0        0     2777 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/slider/jQRangeSliderMouseTouch.js
+-rw-rw-rw-   0        0        0     2983 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/slider/jQRuler.js
+-rw-rw-rw-   0        0        0    94842 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/slider/jquery-1.7.2.min.js
+-rw-rw-rw-   0        0        0   201856 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/slider/jquery-ui.min.js
+-rw-rw-rw-   0        0        0     2395 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/static/js/slider/slider.js
+-rw-rw-rw-   0        0        0   397466 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/subplot.png
+-rw-rw-rw-   0        0        0     2430 2018-02-19 16:08:04.000000 chartpy-0.1.9/chartpy_examples/subplot_examples.py
+-rw-rw-rw-   0        0        0     1507 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/surface_examples.py
+-rw-rw-rw-   0        0        0  1180464 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/temp.html
+-rw-rw-rw-   0        0        0     4423 2017-11-15 12:21:28.000000 chartpy-0.1.9/chartpy_examples/vispy_demo.py
+-rw-rw-rw-   0        0        0      628 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/volsurface.csv
+-rw-rw-rw-   0        0        0   189742 2018-02-19 15:47:44.000000 chartpy-0.1.9/chartpy_examples/volsurface.png
+-rw-rw-rw-   0        0        0     2143 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_examples/xkcd_examples.py
+-rw-rw-rw-   0        0        0    21473 2017-11-15 10:15:02.000000 chartpy-0.1.9/chartpy_logo.png
+-rwxrwxrwx   0        0        0       41 2017-11-15 10:15:02.000000 chartpy-0.1.9/create_package.bat
+-rw-rw-rw-   0        0        0      909 2019-02-12 12:18:14.000000 chartpy-0.1.9/create_python_package.md
+drwxrwxrwx   0        0        0        0 2021-05-04 16:52:26.850359 chartpy-0.1.9/doc/
+-rw-rw-rw-   0        0        0        0 2017-11-15 10:15:02.000000 chartpy-0.1.9/doc/__init__.py
+-rw-rw-rw-   0        0        0      553 2019-02-12 12:20:00.000000 chartpy-0.1.9/longdesc.md
+-rw-rw-rw-   0        0        0       42 2021-05-04 16:52:26.851359 chartpy-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1570 2021-05-04 16:46:10.000000 chartpy-0.1.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `chartpy-0.1.8/.gitignore` & `chartpy-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy/canvas.py` & `chartpy-0.1.9/chartpy/canvas.py`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy/chart.py` & `chartpy-0.1.9/chartpy/chart.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,34 @@
-from __future__ import division
-
-__author__ = 'saeedamen' # Saeed Amen
+__author__ = 'saeedamen'  # Saeed Amen
 
 #
 # Copyright 2016 Cuemacro
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the
 # License. You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and limitations under the License.
 #
 
-"""
-Chart
-
-Creates chart using several underlying plotting libraries (Matplotlib, Plotly and Bokeh) using the same interface
-
-"""
-
 from chartpy.twitter import Twitter
 from chartpy.chartconstants import ChartConstants
 from chartpy.style import Style
 from chartpy.engine import EngineMatplotlib, EngineBokeh, EngineBqplot, EnginePlotly, EngineVisPy
 
 import pandas
 
+
 class Chart(object):
+    """Creates chart using several underlying plotting libraries (Matplotlib, Plotly and Bokeh) using the same interface
+    """
 
-    def __init__(self, df = None, engine = None, chart_type = None, style = None):
+    def __init__(self, df=None, engine=None, chart_type=None, style=None):
 
         self.df = None
         self.engine = ChartConstants().chartfactory_default_engine
         self.style = Style()
         self.chart_type = 'line'  # default chart type is line chart
         self.is_plotted = False
 
@@ -47,15 +41,15 @@
 
     ##### implemented chart types:
     ##### heatmap (Plotly)
     ##### line (Bokeh, Matplotlib, Plotly, vispy)
     ##### bar (Bokeh, Matplotlib, Plotly)
     ##### stacked (Bokeh, Matplotlib, Plotly)
     ##### surface (Plotly)
-    def plot(self, df = None, engine = None, chart_type = None, style = None, twitter_msg = None, twitter_on = False):
+    def plot(self, df=None, engine=None, chart_type=None, style=None, twitter_msg=None, twitter_on=False):
 
         if style is None: style = self.style
         if df is None: df = self.df
 
         if engine is None:
             try:
                 engine = style.engine
@@ -94,22 +88,27 @@
 
         self.is_plotted = True
 
         return fig
 
     def get_engine(self, engine):
 
-        if engine is None:          return self.get_engine(self.engine)
-        elif engine == 'matplotlib':  return EngineMatplotlib()
-        elif engine == 'bokeh':     return EngineBokeh()
-        elif engine == 'bqplot':    return EngineBqplot()
-        elif engine == 'vispy':     return EngineVisPy()
-        elif engine == 'plotly':    return EnginePlotly()
+        if engine is None:
+            return self.get_engine(self.engine)
+        elif engine == 'matplotlib':
+            return EngineMatplotlib()
+        elif engine == 'bokeh':
+            return EngineBokeh()
+        elif engine == 'bqplot':
+            return EngineBqplot()
+        elif engine == 'vispy':
+            return EngineVisPy()
+        elif engine == 'plotly':
+            return EnginePlotly()
 
         return None
 
     # TODO fix this
     def _iplot(self, data_frame, engine=None, chart_type=None, style=None):
         return Chart.get_engine(engine).plot_chart(data_frame, style, chart_type)
 
 #######################################################################################################################
-
```

### Comparing `chartpy-0.1.8/chartpy/chartconstants.py` & `chartpy-0.1.9/chartpy/chartconstants.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import division
-
 __author__ = 'saeedamen' # Saeed Amen
 
 #
 # Copyright 2016 Cuemacro
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the
 # License. You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
@@ -305,20 +303,32 @@
         'wheat':			 '#F5DEB3',
         'white':			 '#FFFFFF',
         'whitesmoke':		 '#F5F5F5',
         'yellow':			 '#FBC15E', #'#ffff33',
         'yellowgreen':		 '#9ACD32'
     }
 
+    override_fields = {}
+
     # or we can store credentials in a file "chartcred.py" in the same folder, which will overwrite the above
     # eg. TWITTER_APP_KEY, TWITTER_APP_SECRET, TWITTER_OAUTH_TOKEN, TWITTER_TOKEN_SECRET
-    # overwrite field variables with those listed in ChartCred
-    def __init__(self):
+    # overwrite field variables with those listed in ChartCred or we can pass through an dictionary to override any fields
+    def __init__(self, override_fields={}):
         try:
             from chartpy.util.chartcred import ChartCred
             cred_keys = ChartCred.__dict__.keys()
 
             for k in ChartConstants.__dict__.keys():
                 if k in cred_keys and '__' not in k:
                     setattr(ChartConstants, k, getattr(ChartCred, k))
         except:
             pass
+
+        # Store overrided fields
+        if override_fields == {}:
+            override_fields = ChartConstants.override_fields
+        else:
+            ChartConstants.override_fields = override_fields
+
+        for k in override_fields.keys():
+            if '__' not in k:
+                setattr(ChartConstants, k, override_fields[k])
```

### Comparing `chartpy-0.1.8/chartpy/engine.py` & `chartpy-0.1.9/chartpy/engine.py`

 * *Files 10% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
     def split_data_frame_to_list(self, data_frame, style):
         data_frame_list = []
 
         if isinstance(data_frame, list):
             data_frame_list = data_frame
         else:
-            if style.subplots == True:
+            if style.subplots == True and isinstance(data_frame, pandas.DataFrame):
 
                 for col in data_frame.columns:
                     data_frame_list.append(
                         pandas.DataFrame(index=data_frame.index, columns=[col], data=data_frame[col]))
             else:
                 data_frame_list.append(data_frame)
 
@@ -461,15 +461,14 @@
 # vispy based plots
 
 try:
     from vispy import plot as vp
 except:
     pass
 
-
 class EngineVisPy(EngineTemplate):
     def plot_chart(self, data_frame, style, chart_type):
 
         cm = ColorMaster()
 
         scale_factor = abs(style.scale_factor)
 
@@ -604,21 +603,27 @@
     pass
 
 try:
     from mpl_toolkits.mplot3d import Axes3D  # need to import in order to do 3D plots (even if not called)
 except:
     pass
 
+# Later version of Pandas will need to register converters
+try:
+    from pandas.plotting import register_matplotlib_converters
+    register_matplotlib_converters()
+except:
+    pass
+
 try:
     from matplotlib.dates import YearLocator, MonthLocator, DayLocator, HourLocator, MinuteLocator
     from matplotlib.ticker import MultipleLocator
 except:
     pass
 
-
 class EngineMatplotlib(EngineTemplate):
 
     def plot_chart(self, data_frame, style, chart_type):
 
         self.apply_style_sheet(style)
 
         if style.xkcd:
@@ -715,18 +720,18 @@
                                                                     vmax=maxz, vmin=minz))
                         else:
                             movie_frame.append(ax_temp.plot_surface(X, Y, Z, cmap=color, rstride=1, cstride=1))
 
                         has_matrix = '3d-matrix'
 
                 if (has_matrix == 'no'):
-                    # plot the lines (using custom palettes as appropriate)
+                    # Plot the lines (using custom palettes as appropriate)
                     color_spec = cm.create_color_list(style, data_frame)
 
-                    # some lines we should exclude from the color and use the default palette
+                    # Some lines we should exclude from the color and use the default palette
                     for i in range(0, len(data_frame.columns.values)):
 
                         if isinstance(chart_type, list):
                             chart_type_ord = chart_type[i]
                         else:
                             chart_type_ord = chart_type
 
@@ -796,23 +801,23 @@
         try:
             ax_temp.set_zlim(minz, maxz)
         except:
             pass
 
         anim = None
 
-        # should we animate the figure?
+        # Should we animate the figure?
         if style.animate_figure:
 
             if style.animate_titles is None:
                 titles = range(1, len(data_frame_list) + 1)
             else:
                 titles = style.animate_titles
 
-            # initialization function: weirdly need to plot the last one (otherwise get ghosting!)
+            # Initialization function: weirdly need to plot the last one (otherwise get ghosting!)
             def init():
                 return [movie_frame[-1]]
 
             def update(i):
                 fig.canvas.set_window_title(str(titles[i]))
 
                 return [movie_frame[i]]
@@ -1324,23 +1329,25 @@
     pass
 
 
 class EnginePlotly(EngineTemplate):
 
     def start_orca(self, path=None):
         # orca is a seperate plotly application for converting Plotly figures to PNG format
+        # Note, now recommended to use kaleido https://github.com/plotly/Kaleido, which is
+        # much easier to install
         if path is not None:
             plotly.io.orca.config.executable = path
 
         plotly.io.orca.ensure_server()
 
     def plot_chart(self, data_frame, style, chart_type):
 
-        # special case if we have a precreated Plotly object
-        if isinstance(data_frame, go.Figure):
+        # Special case if we have a pre-created Plotly object
+        if isinstance(data_frame, Figure):
             return self.publish_plot(data_frame, style)
 
         mode = 'lines'
 
         if style is None: style = Style()
 
         marker_size = 1
@@ -1348,314 +1355,548 @@
         x = '';
         y = '';
         z = ''
 
         scale = 1
 
         try:
-            # adjust sizing if offline_html format
+            # Adjust sizing if offline_html format
             if (style.plotly_plot_mode == 'offline_html' and style.scale_factor > 0):
                 scale = float(2.0 / 3.0)
         except:
             pass
 
-        # check other plots implemented by Cufflinks
+        # Check other plots implemented by Cufflinks
         cm = ColorMaster()
 
-        # create figure
+        # Create figure
         data_frame_list = self.split_data_frame_to_list(data_frame, style)
         fig_list = []
         cols = []
 
-        for data_frame in data_frame_list:
-            cols.append(data_frame.columns)
+        # If we provide a list of Figures this will get ignored
+        try:
+            for data_frame in data_frame_list:
+                cols.append(data_frame.columns)
 
-        cols = list(numpy.array(cols).flat)
+            cols = list(numpy.array(cols).flat)
 
-        # get all the correct colors (and construct gradients if necessary eg. from 'Blues')
-        # need to change to strings for cufflinks
-        color_list = cm.create_color_list(style, [], cols=cols)
-        color_spec = []
+            # Get all the correct colors (and construct gradients if necessary eg. from 'Blues')
+            # need to change to strings for cufflinks
+            color_list = cm.create_color_list(style, [], cols=cols)
+            color_spec = []
 
-        # if no colors are specified then just use our default color set from chart constants
-        if color_list == [None] * len(color_list):
-            color_spec = [None] * len(color_list)
+            # If no colors are specified then just use our default color set from chart constants
+            if color_list == [None] * len(color_list):
+                color_spec = [None] * len(color_list)
 
-            for i in range(0, len(color_list)):
+                for i in range(0, len(color_list)):
 
-                # get the color
-                if color_spec[i] is None:
-                    color_spec[i] = self.get_color_list(i)
+                    # Get the color
+                    if color_spec[i] is None:
+                        color_spec[i] = self.get_color_list(i)
 
-                try:
-                    color_spec[i] = matplotlib.colors.rgb2hex(color_spec[i])
-                except:
-                    pass
+                    try:
+                        color_spec[i] = matplotlib.colors.rgb2hex(color_spec[i])
+                    except:
+                        pass
 
-        else:
-            # otherwise assume all the colors are rgba
-            for color in color_list:
-                color = 'rgba' + str(color)
-                color_spec.append(color)
+            else:
+                # Otherwise assume all the colors are rgba
+                for color in color_list:
+                    color = 'rgba' + str(color)
+                    color_spec.append(color)
+        except Exception as e:
+            pass
 
         start = 0
 
-        # go through each data_frame in the list and plot
+        title_list = style.title
+
+        if not(isinstance(title_list, list)):
+            title_list = [style.title] * len(data_frame_list)
+
+        # Go through each data_frame in the list and plot
         for i in range(0, len(data_frame_list)):
             data_frame = data_frame_list[i]
+            title = title_list[i]
 
-            if isinstance(chart_type, list):
-                chart_type_ord = chart_type[i]
+            if isinstance(data_frame, Figure):
+                fig = data_frame
             else:
-                chart_type_ord = chart_type
 
-            end = start + len(data_frame.columns)
-            color_spec1 = color_spec[start:start + end]
-            start = end
-
-            # special call for choropleth (uses Plotly API directly)
-            # special case for map/choropleth which has yet to be implemented in Cufflinks
-            # will likely remove this in the future
-            if chart_type_ord == 'choropleth':
-
-                for col in data_frame.columns:
-                    try:
-                        data_frame[col] = data_frame[col].astype(str)
-                    except:
-                        pass
+                if style.drop_na:
+                    data_frame = data_frame.dropna()
 
-                if style.color != []:
-                    color = style.color
+                if isinstance(chart_type, list):
+                    chart_type_ord = chart_type[i]
                 else:
-                    color = [[0.0, 'rgb(242,240,247)'], [0.2, 'rgb(218,218,235)'], [0.4, 'rgb(188,189,220)'], \
-                             [0.6, 'rgb(158,154,200)'], [0.8, 'rgb(117,107,177)'], [1.0, 'rgb(84,39,143)']]
+                    chart_type_ord = chart_type
 
-                text = ''
+                end = start + len(data_frame.columns)
+                color_spec1 = color_spec[start:start + end]
+                start = end
+
+                # Special call for choropleth (uses Plotly API directly)
+                # Special case for map/choropleth which has yet to be implemented in Cufflinks
+                # will likely remove this in the future
+                if chart_type_ord == 'choropleth':
 
-                if 'text' in data_frame.columns:
-                    text = data_frame['Text']
+                    for col in data_frame.columns:
+                        try:
+                            data_frame[col] = data_frame[col].astype(str)
+                        except:
+                            pass
+
+                    if style.color != []:
+                        color = style.color
+                    else:
+                        color = [[0.0, 'rgb(242,240,247)'], [0.2, 'rgb(218,218,235)'], [0.4, 'rgb(188,189,220)'], \
+                                 [0.6, 'rgb(158,154,200)'], [0.8, 'rgb(117,107,177)'], [1.0, 'rgb(84,39,143)']]
 
-                data = [dict(
-                    type='choropleth',
-                    colorscale=color,
-                    autocolorscale=False,
-                    locations=data_frame['Code'],
-                    z=data_frame[style.plotly_choropleth_field].astype(float),
-                    locationmode=style.plotly_location_mode,
-                    text=text,
-                    marker=dict(
-                        line=dict(
-                            color='rgb(255,255,255)',
-                            width=1
+                    text = ''
+
+                    if 'text' in data_frame.columns:
+                        text = data_frame['Text']
+
+                    data = [dict(
+                        type='choropleth',
+                        colorscale=color,
+                        autocolorscale=False,
+                        locations=data_frame['Code'],
+                        z=data_frame[style.plotly_choropleth_field].astype(float),
+                        locationmode=style.plotly_location_mode,
+                        text=text,
+                        marker=dict(
+                            line=dict(
+                                color='rgb(255,255,255)',
+                                width=1
+                            )
+                        ),
+                        colorbar=dict(
+                            title=style.units
                         )
-                    ),
-                    colorbar=dict(
-                        title=style.units
+                    )]
+
+                    layout = dict(
+                        title=title,
+                        geo=dict(
+                            scope=style.plotly_scope,
+                            projection=dict(type=style.plotly_projection),
+                            showlakes=True,
+                            lakecolor='rgb(255, 255, 255)',
+                        ),
                     )
-                )]
 
-                layout = dict(
-                    title=style.title,
-                    geo=dict(
-                        scope=style.plotly_scope,
-                        projection=dict(type=style.plotly_projection),
-                        showlakes=True,
-                        lakecolor='rgb(255, 255, 255)',
-                    ),
-                )
+                    fig = dict(data=data, layout=layout)
 
-                fig = dict(data=data, layout=layout)
+                # Otherwise underlying Cufflinks library underneath
+                elif style.plotly_helper == 'cufflinks':
 
-            # otherwise underlying Cufflinks library underneath
-            elif style.plotly_helper == 'cufflinks':
+                    # NOTE: we use cufflinks library, which simplifies plotting DataFrames in plotly
+                    if chart_type_ord == 'surface':
+                        fig = data_frame.iplot(kind=chart_type,
+                                                title=title,
+                                                xTitle=style.x_title,
+                                                yTitle=style.y_title,
+                                                x=x, y=y, z=z,
+                                                mode=mode,
+                                                size=marker_size,
+                                                sharing=style.plotly_sharing,
+                                                theme=style.plotly_theme,
+                                                bestfit=style.line_of_best_fit,
+                                                legend=style.display_legend,
+                                                colorscale=style.color,
+                                                dimensions=(style.width * abs(style.scale_factor) * scale,
+                                                               style.height * abs(style.scale_factor) * scale),
+                                                asFigure=True)
+
+                        # Setting axis is different with a surface
+                        if style.x_axis_range is not None:
+                            fig.update_layout(scene=dict(xaxis=dict(range=style.x_axis_range)))
+
+                        if style.y_axis_range is not None:
+                            fig.update_layout(scene=dict(xaxis=dict(range=style.y_axis_range)))
+
+                        if style.z_axis_range is not None:
+                            fig.update_layout(scene=dict(xaxis=dict(range=style.z_axis_range)))
 
-                # NOTE: we use cufflinks library, which simplifies plotting DataFrames in plotly
-                if chart_type_ord == 'surface':
+                    elif chart_type_ord == 'heatmap':
                         fig = data_frame.iplot(kind=chart_type,
-                                               title=style.title,
+                                               title=title,
                                                xTitle=style.x_title,
                                                yTitle=style.y_title,
-                                               x=x, y=y, z=z,
+                                               x=x, y=y,
                                                mode=mode,
                                                size=marker_size,
                                                sharing=style.plotly_sharing,
                                                theme=style.plotly_theme,
                                                bestfit=style.line_of_best_fit,
                                                legend=style.display_legend,
                                                colorscale=style.color,
                                                dimensions=(style.width * abs(style.scale_factor) * scale,
                                                            style.height * abs(style.scale_factor) * scale),
                                                asFigure=True)
 
-                elif chart_type_ord == 'heatmap':
-                    fig = data_frame.iplot(kind=chart_type,
-                                           title=style.title,
-                                           xTitle=style.x_title,
-                                           yTitle=style.y_title,
-                                           x=x, y=y,
-                                           mode=mode,
-                                           size=marker_size,
-                                           sharing=style.plotly_sharing,
-                                           theme=style.plotly_theme,
-                                           bestfit=style.line_of_best_fit,
-                                           legend=style.display_legend,
-                                           colorscale=style.color,
-                                           dimensions=(style.width * abs(style.scale_factor) * scale,
-                                                       style.height * abs(style.scale_factor) * scale),
-                                           asFigure=True)
+                    # Otherwise we have a line plot (or similar such as a scatter plot, or bar chart etc)
+                    else:
 
-                # otherwise we have a line plot (or similar such as a scatter plot, or bar chart etc)
-                else:
+                        full_line = style.connect_line_gaps
 
-                    full_line = style.connect_line_gaps
+                        if chart_type_ord == 'line':
+                            full_line = True
 
-                    if chart_type_ord == 'line':
-                        full_line = True
+                            # chart_type_ord = 'scatter'
+                            mode = 'lines'
+                        elif chart_type_ord in ['dash', 'dashdot', 'dot']:
+                            chart_type_ord = 'scatter'
+
+                        elif chart_type_ord == 'line+markers':
+                            full_line = True
+
+                            chart_type_ord = 'line'
+                            mode = 'lines+markers'
+                            marker_size = 5
+                        elif chart_type_ord == 'scatter':
+                            mode = 'markers'
+                            marker_size = 5
+                        elif chart_type_ord == 'bubble':
+                            chart_type_ord = 'scatter'
+
+                            mode = 'markers'
+
+                        # TODO check this!
+                        # Can have issues calling cufflinks with a theme which is None, so split up the cases
+                        if style.plotly_theme is None:
+                            plotly_theme = 'pearl'
+                        else:
+                            plotly_theme = style.plotly_theme
 
-                        # chart_type_ord = 'scatter'
-                        mode = 'lines'
-                    elif chart_type_ord in ['dash', 'dashdot', 'dot']:
-                        chart_type_ord = 'scatter'
-
-                    elif chart_type_ord == 'line+markers':
-                        full_line = True
-
-                        chart_type_ord = 'line'
-                        mode = 'lines+markers'
-                        marker_size = 5
-                    elif chart_type_ord == 'scatter':
-                        mode = 'markers'
-                        marker_size = 5
-                    elif chart_type_ord == 'bubble':
-                        chart_type_ord = 'scatter'
-
-                        mode = 'markers'
-
-                    # TODO check this!
-                    # can have issues calling cufflinks with a theme which is None, so split up the cases
-                    if style.plotly_theme is None:
-                        plotly_theme = 'pearl'
-                    else:
-                        plotly_theme = style.plotly_theme
+                        m = 0
 
-                    m = 0
+                        y_axis_2_series = [x for x in style.y_axis_2_series if x in data_frame.columns]
 
-                    # sometimes Plotly has issues generating figures in dash, so if fails first, try again
-                    while m < 10:
-                        try:
-                            fig = data_frame.iplot(kind=chart_type_ord,
-                                                   title=style.title,
-                                                   xTitle=style.x_title,
-                                                   yTitle=style.y_title,
-                                                   x=x, y=y, z=z,
-                                                   subplots=False,
-                                                   sharing=style.plotly_sharing,
-                                                   mode=mode,
-                                                   secondary_y=style.y_axis_2_series,
-                                                   size=marker_size,
-                                                   theme=plotly_theme,
-                                                   colorscale='dflt',
-                                                   bestfit=style.line_of_best_fit,
-                                                   legend=style.display_legend,
-                                                   width=style.linewidth,
-                                                   color=color_spec1,
-                                                   dimensions=(style.width * abs(style.scale_factor) * scale,
-                                                               style.height * abs(style.scale_factor) * scale),
-                                                   asFigure=True)
+                        vspan = None
 
-                            m = 10;
-                            break
-                        except Exception as e:
-                            print("Will attempt to re-render: " + str(e))
-
-                            import time
-                            time.sleep(0.3)
-
-                        m = m + 1
-
-                    # for lines set the property of connectgaps (cannot specify directly in cufflinks)
-                    if full_line:
-                        for z in range(0, len(fig['data'])):
-                            fig['data'][z].connectgaps = style.connect_line_gaps
+                        if style.x_shade_dates is not None:
+                            vspan = {'x0': data_frame.index[0].strftime("%Y-%m-%d"),
+                                     'x1': data_frame.index[-1].strftime("%Y-%m-%d"), 'color': 'rgba(30,30,30,0.3)',
+                                     'fill': True, 'opacity': .4}
+
+                        # Sometimes Plotly has issues generating figures in dash, so if fails first, try again
+                        while m < 10:
+
+                            if True:
+                                if vspan is None:
+                                    fig = data_frame.iplot(kind=chart_type_ord,
+                                                           title=title,
+                                                           xTitle=style.x_title,
+                                                           yTitle=style.y_title,
+                                                           x=x, y=y, z=z,
+                                                           subplots=False,
+                                                           sharing=style.plotly_sharing,
+                                                           mode=mode,
+                                                           secondary_y=y_axis_2_series,
+                                                           size=marker_size,
+                                                           theme=plotly_theme,
+                                                           colorscale='dflt',
+                                                           bestfit=style.line_of_best_fit,
+                                                           legend=style.display_legend,
+                                                           width=style.linewidth,
+                                                           color=color_spec1,
+                                                           dimensions=(style.width * abs(style.scale_factor) * scale,
+                                                                       style.height * abs(style.scale_factor) * scale),
+                                                           asFigure=True)
+                                else:
+                                    fig = data_frame.iplot(kind=chart_type_ord,
+                                                           title=title,
+                                                           xTitle=style.x_title,
+                                                           yTitle=style.y_title,
+                                                           x=x, y=y, z=z,
+                                                           subplots=False,
+                                                           sharing=style.plotly_sharing,
+                                                           mode=mode,
+                                                           secondary_y=y_axis_2_series,
+                                                           size=marker_size,
+                                                           theme=plotly_theme,
+                                                           colorscale='dflt',
+                                                           bestfit=style.line_of_best_fit,
+                                                           legend=style.display_legend,
+                                                           width=style.linewidth,
+                                                           color=color_spec1,
+                                                           dimensions=(style.width * abs(style.scale_factor) * scale,
+                                                                       style.height * abs(style.scale_factor) * scale),
+                                                           vspan=vspan,
+                                                           asFigure=True)
+
+                                m = 10;
+                                break
+                            #except Exception as e:
+                                print("Will attempt to re-render: " + str(e))
+
+                                import time
+                                time.sleep(0.3)
+
+                            m = m + 1
+
+                        # For lines set the property of connectgaps (cannot specify directly in cufflinks)
+                        if full_line:
+                            for z in range(0, len(fig['data'])):
+                                fig['data'][z].connectgaps = style.connect_line_gaps
+
+                                for k in range(0, len(fig['data'])):
+                                    if full_line:
+                                        fig['data'][k].connectgaps = style.connect_line_gaps
+
+                        if style.line_shape != None:
+                            if isinstance(style.line_shape, str):
+                                line_shape = [style.line_shape] * len(fig['data'])
+                            else:
+                                line_shape = style.line_shape
 
                             for k in range(0, len(fig['data'])):
-                                if full_line:
-                                    fig['data'][k].connectgaps = style.connect_line_gaps
+                                fig['data'][k].line.shape = line_shape[k]
 
-                    if style.line_shape != None:
-                        if isinstance(style.line_shape, str):
-                            line_shape = [style.line_shape] * len(fig['data'])
-                        else:
-                            line_shape = style.line_shape
+                        if style.plotly_webgl:
+                            for k in range(0, len(fig['data'])):
+                                if fig['data'][k].type == 'scatter':
+                                    fig['data'][k].type = 'scattergl'
+
+                # Use plotly express (not implemented yet)
+                elif style.plotly_helper == 'plotly_express':
+                    # TODO
+                    pass
 
-                        for k in range(0, len(fig['data'])):
-                            fig['data'][k].line.shape = line_shape[k]
+            # Common properties
+            # Override other properties, which cannot be set directly by cufflinks/or you want to reset later
+            if style.title is not None:
+                try:
+                    fig.update_layout(title=style.title)
+                except:
+                    pass
 
-                    if style.plotly_webgl:
-                        for k in range(0, len(fig['data'])):
-                            if fig['data'][k].type == 'scatter':
-                                fig['data'][k].type = 'scattergl'
+            # Add second y axis title
+            if style.y_2_title is not None:
+                if style.y_2_title != '':
+                    try:
+                        fig['layout'].update(yaxis2=dict(title=style.y_2_title))
+                    except:
+                        pass
 
-            # use plotly express (not implemented yet)
-            elif style.plotly_helper == 'plotly_express':
-                # TODO
-                pass
+            if style.x_axis_range is not None:
+                try:
+                    fig['layout'].update(xaxis=dict(range=style.x_axis_range, autorange=False))
+                except:
+                    pass
 
             if style.y_axis_range is not None:
-                # override other properties, which cannot be set directly by cufflinks
-                fig.update(dict(layout=dict(yaxis=dict(
-                    range=style.y_axis_range
-                ))))
 
-            if style.x_axis_range is not None:
-                # override other properties, which cannot be set directly by cufflinks
-                fig.update(dict(layout=dict(xaxis=dict(
-                    range=style.x_axis_range
-                ))))
+                try:
+                    fig['layout'].update(yaxis=dict(range=style.y_axis_range, autorange=False))
+                except:
+                    pass
 
-            fig.update(dict(layout=dict(legend=dict(
+            if style.y_axis_2_range is not None:
+                try:
+                    fig['layout'].update(yaxis2=dict(range=style.y_axis_2_range, autorange=False))
+                except:
+                    pass
+
+            if style.z_axis_range is not None:
+                try:
+                    fig['layout'].update(zaxis=dict(range=style.z_axis_range, autorange=False))
+                except:
+                    pass
+
+            if style.font_family is not None:
+                try:
+                    fig.update_layout(font_family=style.font_family)
+                except:
+                    pass
+
+            if style.x_axis_type is not None:
+                try:
+                    fig.update_xaxes(type=style.x_axis_type)
+                except:
+                    pass
+
+            if style.y_axis_type is not None:
+                try:
+                    fig.update_yaxes(type=style.y_axis_type)
+                except:
+                    pass
+
+            if style.x_dtick is not None:
+                try:
+                    fig.update_layout(xaxis=dict(tickmode='linear', dtick=style.x_dtick))
+                except:
+                    pass
+
+            if style.y_dtick is not None:
+                try:
+                    fig.update_layout(yaxis=dict(tickmode='linear', dtick=style.y_dtick))
+                except:
+                    pass
+
+            # Add shaded regions
+            fig = self._multi_shade(fig, style)
+
+            # Legend Properties
+            if style.legend_x_anchor is not None:
+                try: fig.update_layout(legend=dict(xanchor=style.legend_x_anchor))
+                except: pass
+
+            if style.legend_y_anchor is not None:
+                try: fig.update_layout(legend=dict(yanchor=style.legend_y_anchor))
+                except: pass
+                
+            if style.legend_x_pos is not None:
+                try: fig.update_layout(legend=dict(x=style.legend_x_pos))
+                except: pass
+
+            if style.legend_y_pos is not None:
+                try: fig.update_layout(legend=dict(y=style.legend_y_pos))
+                except: pass
+
+            if style.legend_bgcolor is not None:
+                try: fig.update_layout(legend=dict(bgcolor=style.legend_bgcolor))
+                except: pass
+
+            if style.legend_orientation is not None:
+                try: fig.update_layout(legend=dict(orientation=style.legend_orientation))
+                except: pass
+
+            fig_list.append(fig)
+
+        #### Plotted all the lines
+
+        # Create subplots if more than one figure
+        if len(fig_list) > 1 and style.animate_figure == False:
+            fig = cf.subplots(fig_list, base_layout=fig_list[0].to_dict()['layout'], shape=(1, len(fig_list)),
+                              shared_xaxes=False, shared_yaxes=False)
+
+            if not(isinstance(style.title, list)):
+                fig['layout'].update(title=style.title)
+
+        elif style.animate_figure:
+
+            fig = fig_list[0]
+
+            # Add buttons to play/pause
+            fig["layout"]["updatemenus"] = [
+                {
+                    "buttons": [
+                        {
+                            "args": [None, {"frame": {"duration": style.animate_frame_ms, "redraw": True},
+                                            "fromcurrent": True, "transition": {"duration": style.animate_frame_ms,
+                                                                                "easing": "quadratic-in-out"}}],
+                            "label": "Play",
+                            "method": "animate"
+                        },
+                        {
+                            "args": [[None], {"frame": {"duration": 0, "redraw": True},
+                                              "mode": "immediate",
+                                              "transition": {"duration": 0}}],
+                            "label": "Pause",
+                            "method": "animate"
+                        }
+                    ],
+                    "direction": "left",
+                    "pad": {"r": 10, "t": 87},
+                    "showactive": False,
+                    "type": "buttons",
+                    "x": 0.1,
+                    "xanchor": "right",
+                    "y": 0,
+                    "yanchor": "top"
+                }
+            ]
+
+            if style.animate_titles is not None:
+                animate_titles = style.animate_titles
+            else:
+                animate_titles = list(range(0, len(fig_list)))
+
+            # Add an animation frame for each data frame
+            frames = []
+
+            for fig_temp, title_temp in zip(fig_list, animate_titles):
+                frames.append(go.Frame(data=fig_temp['data'],
+                                           name=str(title_temp),
+                                           layout=go.Layout(title=str(title_temp))))
+
+            fig.update(frames=frames)
+
+            # Add a slider, with the frame labels
+            sliders_dict = {
+                    "active": 0,
+                    "yanchor": "top",
+                    "xanchor": "left",
+                    "currentvalue": {
+                        "visible": True,
+                        "xanchor": "right"
+                    },
+                    "transition": {"duration": style.animate_frame_ms, "easing": "cubic-in-out"},
+                    "pad": {"b": 10, "t": 50},
+                    "len": 0.9,
+                    "x": 0.1,
+                    "y": 0,
+                    "steps": []
+            }
+
+            for i in range(0, len(fig_list)):
+                slider_step = {"args": [
+                    [animate_titles[i]],
+                    {"frame" : {"duration": style.animate_frame_ms, "redraw": True},
+                    "mode" : "immediate",
+                    "transition" : {"duration": style.animate_frame_ms}}
+                ],
+                    "label" : str(animate_titles[i]),
+                    "method" : "animate"}
+
+                sliders_dict["steps"].append(slider_step)
+
+            fig["layout"]["sliders"] = [sliders_dict]
+
+            #else:
+                # Add an animation frame for each data frame
+            #    fig.update(frames=[go.Frame(data=fig_temp['data']) for fig_temp in fig_list])
+
+        else:
+            fig = fig_list[0]
+
+        fig.update(dict(layout=dict(legend=dict(
                 x=0.05,
                 y=1
             ))))
 
-            # adjust margins
-            if style.thin_margin:
+        # Adjust margins
+        if style.thin_margin:
                 fig.update(dict(layout=dict(margin=go.layout.Margin(
                     l=20,
                     r=20,
                     b=40,
                     t=40,
                     pad=0
                 ))))
 
-            # change background color
-            fig.update(dict(layout=dict(paper_bgcolor='rgba(0,0,0,0)')))
-            fig.update(dict(layout=dict(plot_bgcolor='rgba(0,0,0,0)')))
-
-            # deal with grids
-            if (not (style.x_axis_showgrid)): fig.update(dict(layout=dict(xaxis=dict(showgrid=style.x_axis_showgrid))))
-            if (not (style.y_axis_showgrid)): fig.update(dict(layout=dict(yaxis=dict(showgrid=style.y_axis_showgrid))))
-            if (not (style.y_axis_2_showgrid)): fig.update(
-                dict(layout=dict(yaxis2=dict(showgrid=style.y_axis_2_showgrid))))
-
-            fig_list.append(fig)
-
-        #### plotted all the lines
-
-        if len(fig_list) > 1:
-            fig = cf.subplots(fig_list)
+        # Change background color
+        fig.update(dict(layout=dict(paper_bgcolor='rgba(0,0,0,0)')))
+        fig.update(dict(layout=dict(plot_bgcolor='rgba(0,0,0,0)')))
 
-            fig['layout'].update(title=style.title)
-        else:
-            fig = fig_list[0]
+        # Deal with grids
+        if (not(style.x_axis_showgrid)): fig.update(dict(layout=dict(xaxis=dict(showgrid=style.x_axis_showgrid))))
+        if (not(style.y_axis_showgrid)): fig.update(dict(layout=dict(yaxis=dict(showgrid=style.y_axis_showgrid))))
+        if (not(style.y_axis_2_showgrid)): fig.update(
+                dict(layout=dict(yaxis2=dict(showgrid=style.y_axis_2_showgrid))))
 
-        # override properties, which cannot be set directly by cufflinks
+        # Override properties, which cannot be set directly by cufflinks
 
-        # for the type of line (ie. line or scatter)
-        # for making the lined dashed, dotted etc.
+        # For the type of line (ie. line or scatter)
+        # For making the lined dashed, dotted etc.
         if style.subplots == False and isinstance(chart_type, list):
             for j in range(0, len(fig['data'])):
                 mode = None;
                 dash = None;
                 line_shape = None;
 
                 if chart_type[j] == 'line':
@@ -1688,15 +1929,15 @@
 
                 if dash is not None:
                     fig['data'][j].line.dash = dash
 
                 if line_shape is not None:
                     fig['data'][j].line.shape = line_shape
 
-        # if candlestick specified add that (needed to be appended on top of the Plotly figure's data
+        # If candlestick specified add that (needed to be appended on top of the Plotly figure's data
         if style.candlestick_series is not None and not (style.plotly_webgl):
 
             # self.logger.debug("About to create candlesticks")
 
             if isinstance(style.candlestick_series, Figure):
                 fig_candle = style.candlestick_series
             else:
@@ -1705,33 +1946,37 @@
                                                 style.candlestick_series['high'],
                                                 style.candlestick_series['low'],
                                                 style.candlestick_series['close'],
                                                 dates=style.candlestick_series['close'].index
                                                 )
 
             if style.candlestick_increasing_color is not None:
-                # increasing
+                # Increasing
                 fig_candle['data'][0].fillcolor = cm.get_color_code(style.candlestick_increasing_color)
                 fig_candle['data'][0].line.color = cm.get_color_code(style.candlestick_increasing_line_color)
 
             if style.candlestick_decreasing_color is not None:
-                # descreasing
+                # Decreasing
                 fig_candle['data'][1].fillcolor = cm.get_color_code(style.candlestick_decreasing_color)
                 fig_candle['data'][1].line.color = cm.get_color_code(style.candlestick_decreasing_line_color)
 
             try:
-                # append the data to the existing Plotly figure, plotted earlier
+                # Append the data to the existing Plotly figure, plotted earlier
                 fig.data.append(fig_candle.data[0]);
                 fig.data.append(fig_candle.data[1])
             except:
-                # plotly 3.0
+                # Later version of Plotly
                 fig.add_trace(fig_candle.data[0])
                 fig.add_trace(fig_candle.data[1])
 
-            # self.logger.debug("Rendered candlesticks")
+        # Overlay other Plotly figures on top of
+        if style.overlay_fig is not None:
+
+            for d in style.overlay_fig.data:
+                fig.add_trace(d)
 
         x_y_line_list = []
 
         # fig.layout.yrange
         # add x-line:
         for x_y_line in style.x_y_line:
             start = x_y_line[0]
@@ -1767,14 +2012,49 @@
         if len(x_y_line_list) > 0:
             fig.layout.shapes = x_y_line_list
 
         # publish the plot (depending on the output mode eg. to HTML file/Jupyter notebook)
         # also return as a Figure object for plotting by a web server app (eg. Flask/Dash)
         return self.publish_plot(fig, style)
 
+    def _multi_shade(self, fig, style):
+        """ Adds shaded areas for specified dates in a plotly plot.
+            The lines of the areas are set to transparent using rgba(0,0,0,0)
+        """
+        import copy
+
+        if style.x_shade_dates is None:
+            return fig
+
+        if isinstance(style.x_shade_dates, list):
+            x0 = style.x_shade_dates[0]
+            x1 = style.x_shade_dates[1]
+        else:
+            x0 = list(style.x_shade_dates.keys())
+            x1 = list(style.x_shade_dates.values())
+
+        # Get dict from tuple made by vspan()
+        x_elem = fig['layout']['shapes'][0]
+
+        # Container (list) for dicts / shapes
+        shp_lst = []
+
+        # Make dicts according to x0 and X1
+        # and edit elements of those dicts
+        for i in range(0,len(x0)):
+            shp_lst.append(copy.deepcopy(x_elem))
+            shp_lst[i]['x0'] = x0[i]
+            shp_lst[i]['x1'] = x1[i]
+            shp_lst[i]['line']['color'] = 'rgba(0,0,0,0)'
+
+        # Replace shape in fig with multiple new shapes
+        fig['layout']['shapes']= tuple(shp_lst)
+
+        return fig
+
     def publish_plot(self, fig, style):
         # change background color
         fig.update(dict(layout=dict(paper_bgcolor='rgba(0,0,0,0)')))
         fig.update(dict(layout=dict(plot_bgcolor='rgba(0,0,0,0)')))
 
         if style is None: style = Style()
 
@@ -1845,23 +2125,23 @@
         color_palette = cc.plotly_palette
 
         return color_palette[i % len(color_palette)]
 
 
 #######################################################################################################################
 
-# create color lists to be used in plots
+# Create color lists to be used in plots
 
-class ColorMaster:
+class ColorMaster(object):
 
     def create_color_list(self, style, data_frame, cols=None):
         if cols is None:
             cols = data_frame.columns
 
-        # get all the correct colors (and construct gradients if necessary eg. from 'blues')
+        # Get all the correct colors (and construct gradients if necessary eg. from 'blues')
         color = self.construct_color(style, 'color', len(cols) - len(style.color_2_series))
         color_2 = self.construct_color(style, 'color_2', len(style.color_2_series))
 
         return self.assign_color(cols, color, color_2,
                                  style.exclude_from_color, style.color_2_series)
 
     def construct_color(self, style, color_field_name, no_of_entries):
@@ -2149,19 +2429,19 @@
 
     # if dates is not None:
     #     utils.validate_equal_length(open, high, low, close, dates)
     # else:
     #     utils.validate_equal_length(open, high, low, close)
     # validate_ohlc(open, high, low, close, direction, **kwargs)
 
-    if direction is 'increasing':
+    if direction == 'increasing':
         candle_incr_data = make_increasing_candle(open, high, low, close,
                                                   dates, **kwargs)
         data = candle_incr_data
-    elif direction is 'decreasing':
+    elif direction == 'decreasing':
         candle_decr_data = make_decreasing_candle(open, high, low, close,
                                                   dates, **kwargs)
         data = candle_decr_data
     else:
         candle_incr_data = make_increasing_candle(open, high, low, close,
                                                   dates, **kwargs)
         candle_decr_data = make_decreasing_candle(open, high, low, close,
```

### Comparing `chartpy-0.1.8/chartpy/style.py` & `chartpy-0.1.9/chartpy/style.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,101 +25,132 @@
 
 from chartpy.chartconstants import ChartConstants
 
 class Style(object):
     cc = ChartConstants()
 
     def __init__(self,
-                 # captions
+                 # Captions
                  title='',
                  x_title='',
                  y_title='',
+                 y_2_title='',
+                 z_title='',
                  units='',
 
-                 # type of plot (can be defined as list)
+                 font_family=None,
+
+                 # Type of plot (can be defined as list)
                  engine=None,
                  chart_type=None,
+                 
+                 # Drop NaN points before plotting
+                 drop_na=False,
 
-                 # colors
+                 # Colors
                  color=[],
                  color_2=[],
                  color_2_series=[],
                  exclude_from_color=[],
                  normalize_colormap=True,
 
-                 # bubble charts
+                 # Bubble charts
                  bubble_series=None,
                  bubble_size_scalar=cc.chartfactory_bubble_size_scalar,
 
-                 # candlestick charts
+                 # Candlestick charts
                  candlestick_series=None,
                  candlestick_increasing_color=None,
                  candlestick_increasing_line_color=None,
                  candlestick_decreasing_color=None,
                  candlestick_decreasing_line_color=None,
+                 
+                 # Overlay figures
+                 overlay_fig=None,
 
-                 # subplot
+                 # Subplot
                  subplots=False,
                  share_subplot_x=False,
 
-                 # display sizes
+                 # Display sizes
                  scale_factor=cc.chartfactory_scale_factor,
                  dpi=cc.chartfactory_dpi,
                  width=cc.chartfactory_width,
                  height=cc.chartfactory_height,
                  resample=None,
                  thin_margin=False,
 
-                 # should we block display of new screens?
+                 # Should we block display of new screens?
                  block_new_plots=False,
 
                  # show this be an animation?
                  animate_figure=False,
                  animate_titles=None,
                  animate_frame_ms=250,
 
-                 # lines and multiple y-axis
+                 # Lines and multiple y-axis
                  y_axis_2_series=[],
                  linewidth_2_series=[],
                  linewidth=None,
                  linewidth_2=None,
                  marker_size=1,
                  line_of_best_fit=False,
                  line_shape=None,
 
-                 # grid
+                 # Shaded regions
+                 x_shade_dates=None,
+
+                 # Grid
                  x_axis_showgrid = True,
                  y_axis_showgrid = True,
                  y_axis_2_showgrid = True,
+                 z_axis_showgrid=True,
 
-                 # vertical and horizontal lines from axis
+                 # Vertical and horizontal lines from axis
                  x_y_line=[],
                  x_axis_range=None,
                  y_axis_range=None,
+                 z_axis_range=None,
+                 y_axis_2_range=None,
+
+                 # Are x-axis of style category?
+                 x_axis_type=None,
+                 y_axis_type=None,
 
-                 # connect gaps
+                 x_dtick=None,
+                 y_dtick=None,
+
+                 # Connect gaps
                  connect_line_gaps=False,
 
-                 # labelling of sources
+                 # Labelling of sources
                  brand_label=cc.chartfactory_brand_label,
                  display_brand_label=cc.chartfactory_display_brand_label,
                  source=cc.chartfactory_source,
                  source_color='black',
                  display_source_label=cc.chartfactory_display_source_label,
                  display_legend=True,
 
+                 # Legend properties
+                 legend_x_anchor=None,
+                 legend_y_anchor=None,
+                 legend_x_pos=None,
+                 legend_y_pos=None,
+                 legend_bgcolor=None,
+                 legend_orientation=None,
+
                  # matplotlib only
                  xkcd=False,
 
-                 # display output
+                 # Display output
                  silent_display=False,
                  file_output=None,
                  date_formatter=None,
 
-                 # output
+                 # Output
                  html_file_output=None,
                  display_mpld3=False,
                  auto_generate_filename=False,
                  auto_generate_html_filename=False,
                  save_fig=True,
 
                  # plotly only
@@ -130,125 +161,162 @@
                  plotly_world_readable=cc.plotly_world_readable,
                  plotly_sharing=cc.plotly_sharing,
                  plotly_theme=None,
                  plotly_plot_mode=cc.plotly_plot_mode,
                  plotly_webgl=cc.plotly_webgl,
                  plotly_helper=cc.plotly_helper,
 
-                 # bokeh
+                 # Bokeh
                  bokeh_plot_mode=cc.bokeh_plot_mode,
 
                  # plotly choropleth fields
 
 
-                 # matplotlib only
+                 # Matplotlib only
                  style_sheet=cc.chartfactory_default_stylesheet,
                  convert_matplotlib_to_plotly=False
                  ):
 
         self.engine = engine
 
-        # captions
+        # Captions
         self.title = title
         self.x_title = x_title
         self.y_title = y_title
+        self.y_2_title = y_2_title
+        self.z_title = z_title
         self.units = units
 
-        # chart type
+        self.font_family = font_family
+
+        # Chart type
         self.chart_type = chart_type
+        
+        # Drop NaN before plotting
+        self.drop_na = drop_na
 
-        # colors
+        # Colors
         self.color = color
         self.color_2 = color_2
         self.color_2_series = color_2_series
         self.exclude_from_color = exclude_from_color
         self.normalize_colormap = normalize_colormap
 
-        # bubble specific fields
+        # Bubble specific fields
         self.bubble_series = bubble_series
         self.bubble_size_scalar = bubble_size_scalar
 
-        # candlestick specific fields
+        # Candlestick specific fields
         self.candlestick_series = candlestick_series
         self.candlestick_increasing_color = candlestick_increasing_color
         self.candlestick_increasing_line_color = candlestick_increasing_line_color
         self.candlestick_decreasing_color = candlestick_decreasing_color
         self.candlestick_decreasing_line_color = candlestick_decreasing_line_color
-
-        # subplots
+        
+        # Overlay plots
+        self.overlay_fig = overlay_fig
+        
+        # Subplots
         self.subplots = subplots
         self.share_subplot_x = share_subplot_x
 
-        # display sizes
+        # Display sizes
         self.scale_factor = scale_factor
         self.dpi = dpi
         self.width = width
         self.height = height
         self.resample = resample
         self.thin_margin = thin_margin
 
-        # block display
+        # Block display
         self.block_new_plots = block_new_plots
         
-        # animation parameters
+        # Animation parameters
         self.animate_figure = animate_figure
         self.animate_titles = animate_titles
         self.animate_frame_ms = animate_frame_ms
 
-        # lines and multiple y-axis
+        # Lines and multiple y-axis
         self.y_axis_2_series = y_axis_2_series
         self.linewidth_2_series = linewidth_2_series
         self.linewidth = linewidth
         self.linewidth_2 = linewidth_2
         self.marker_size = marker_size
         self.line_of_best_fit = line_of_best_fit
         self.line_shape = line_shape
 
-        # grids
+        # Shaded regions
+        self.x_shade_dates = x_shade_dates
+
+        # Grids
         self.x_axis_showgrid = x_axis_showgrid
         self.y_axis_showgrid = y_axis_showgrid
+        self.z_axis_showgrid = z_axis_showgrid
         self.y_axis_2_showgrid = y_axis_2_showgrid
 
-        # arbitrary line
+        # Arbitrary line
         self.x_y_line = x_y_line
         self.x_axis_range = x_axis_range
         self.y_axis_range = y_axis_range
+        self.y_axis_2_range = y_axis_2_range
+        self.z_axis_range = z_axis_range
+
+        # x and y axis type (eg. category)
+        self.x_axis_type = x_axis_type
+        self.y_axis_type = y_axis_type
+        
+        # Gaps between tick labels
+        self.x_dtick = x_dtick
+        self.y_dtick = y_dtick
 
-        # connect line gaps
+        # Connect line gaps
         self.connect_line_gaps = connect_line_gaps
 
-        # labelling of sources
+        # Labelling of sources
         self.brand_label = brand_label
         self.display_brand_label = display_brand_label
         self.source = source
         self.source_color = source_color
         self.display_source_label = display_source_label
         self.display_legend = display_legend
 
+        # Legend Properties
+        self.legend_x_anchor = legend_x_anchor
+        self.legend_y_anchor = legend_y_anchor
+        self.legend_x_pos = legend_x_pos
+        self.legend_y_pos = legend_y_pos
+        self.legend_bgcolor = legend_bgcolor
+        self.legend_orientation = legend_orientation
+
         # matplotlib only
         self.xkcd = xkcd
 
-        # display output
+        # Display output
         self.silent_display = silent_display
         self.file_output = file_output
         self.save_fig = save_fig
         self.date_formatter = date_formatter
 
-        # output
+        # Output
         self.html_file_output = html_file_output
         self.display_mpld3 = display_mpld3
         self.auto_generate_filename = auto_generate_filename
         self.auto_generate_html_filename = auto_generate_html_filename
 
         # bokeh only
         self.bokeh_plot_mode = bokeh_plot_mode  # 'online', 'offline_html', 'offline_jupyter'
 
         # plotly only
         if plotly_url is None:
-            plotly_url = title + datetime.datetime.utcnow().strftime("%b-%d-%Y-%H-%M-%S")
+            if isinstance(title, list):
+                plotly_url = str(title[0])
+            else:
+                plotly_url = title
+
+            plotly_url = plotly_url +  datetime.datetime.utcnow().strftime("%b-%d-%Y-%H-%M-%S")
 
         self.plotly_url = plotly_url
         self.plotly_as_image = plotly_as_image
         self.plotly_username = plotly_username
         self.plotly_webgl = plotly_webgl
         self.plotly_helper = plotly_helper
 
@@ -310,31 +378,64 @@
     @property
     def y_title(self):
         return self.__y_title
 
     @y_title.setter
     def y_title(self, y_title):
         self.__y_title = y_title
+        
+    @property
+    def y_2_title(self):
+        return self.__y_2_title
+
+    @y_2_title.setter
+    def y_2_title(self, y_2_title):
+        self.__y_2_title = y_2_title
+
+    @property
+    def z_title(self):
+        return self.__z_title
+
+    @y_title.setter
+    def z_title(self, z_title):
+        self.__z_title = z_title
 
     @property
     def units(self):
         return self.__units
 
     @units.setter
     def units(self, units):
         self.__units = units
+        
+    @property
+    def font_family(self):
+        return self.__font_family
+
+    @font_family.setter
+    def font_family(self, font_family):
+        self.__font_family = font_family
 
     ###### chart type
     @property
     def chart_type(self):
         return self.__chart_type
 
     @chart_type.setter
     def chart_type(self, chart_type):
         self.__chart_type = chart_type
+        
+    ###### drop na
+    @property
+    def drop_na(self):
+        return self.__drop_na
+
+    @drop_na.setter
+    def drop_na(self, drop_na):
+        self.__drop_na = drop_na
 
     ###### colors
     @property
     def color(self):
         return self.__color
 
     @color.setter
@@ -427,16 +528,25 @@
     @property
     def candlestick_decreasing_line_color(self):
         return self.__candlestick_decreasing_line_color
 
     @candlestick_decreasing_line_color.setter
     def candlestick_decreasing_line_color(self, candlestick_decreasing_line_color):
         self.__candlestick_decreasing_line_color = candlestick_decreasing_line_color
+    
+    ###### Overlay figures
+    @property
+    def overlay_fig(self):
+        return self.__overlay_fig
 
-    ###### subplots
+    @overlay_fig.setter
+    def overlay_fig(self, overlay_fig):
+        self.__overlay_fig = overlay_fig
+    
+    ###### Subplots
     @property
     def subplots(self):
         return self.__subplots
 
     @subplots.setter
     def subplots(self, subplots):
         self.__subplots = subplots
@@ -584,17 +694,27 @@
     @property
     def line_shape(self):
         return self.__line_shape
 
     @line_shape.setter
     def line_shape(self, line_shape):
         self.__line_shape = line_shape
-
         
-    ###### grids
+    
+    ###### Shaded regions
+    
+    @property
+    def x_shade_dates(self):
+        return self.__x_shade_dates
+
+    @x_shade_dates.setter
+    def x_shade_dates(self, x_shade_dates):
+        self.__x_shade_dates = x_shade_dates
+        
+    ###### Grids
     @property
     def x_axis_showgrid(self):
         return self.__x_axis_showgrid
 
     @x_axis_showgrid.setter
     def x_axis_showgrid(self, x_axis_showgrid):
         self.__x_axis_showgrid = x_axis_showgrid
@@ -602,14 +722,22 @@
     @property
     def y_axis_showgrid(self):
         return self.__y_axis_showgrid
 
     @y_axis_showgrid.setter
     def y_axis_showgrid(self, y_axis_showgrid):
         self.__y_axis_showgrid = y_axis_showgrid
+        
+    @property
+    def z_axis_showgrid(self):
+        return self.__z_axis_showgrid
+
+    @z_axis_showgrid.setter
+    def z_axis_showgrid(self, z_axis_showgrid):
+        self.__z_axis_showgrid = z_axis_showgrid
 
     @property
     def y_axis_2_showgrid(self):
         return self.__y_axis_2_showgrid
 
     @y_axis_2_showgrid.setter
     def y_axis_2_showgrid(self, y_axis_2_showgrid):
@@ -635,14 +763,65 @@
     @property
     def y_axis_range(self):
         return self.__y_axis_range
 
     @y_axis_range.setter
     def y_axis_range(self, y_axis_range):
         self.__y_axis_range = y_axis_range
+        
+    @property
+    def y_axis_2_range(self):
+        return self.__y_axis_2_range
+
+    @y_axis_2_range.setter
+    def y_axis_2_range(self, y_axis_2_range):
+        self.__y_axis_2_range = y_axis_2_range
+
+    @property
+    def z_axis_range(self):
+        return self.__z_axis_range
+
+    @z_axis_range.setter
+    def z_axis_range(self, z_axis_range):
+        self.__z_axis_range = z_axis_range
+        
+    ###### axis type
+
+    @property
+    def x_axis_type(self):
+        return self.__x_axis_type
+
+    @x_axis_type.setter
+    def x_axis_type(self, x_axis_type):
+        self.__x_axis_type = x_axis_type
+
+    @property
+    def y_axis_type(self):
+        return self.__y_axis_type
+
+    @y_axis_type.setter
+    def y_axis_type(self, y_axis_type):
+        self.__y_axis_type = y_axis_type
+    
+    ###### gaps between tick labels
+    @property
+    def x_dtick(self):
+        return self.__x_dtick
+
+    @x_dtick.setter
+    def x_dtick(self, x_dtick):
+        self.__x_dtick = x_dtick
+
+    @property
+    def y_dtick(self):
+        return self.__y_dtick
+
+    @y_dtick.setter
+    def y_dtick(self, y_dtick):
+        self.__y_dtick = y_dtick
 
     ###### connect line gaps
     @property
     def connect_line_gaps(self):
         return self.__connect_line_gaps
 
     @connect_line_gaps.setter
@@ -694,16 +873,65 @@
     @property
     def display_legend(self):
         return self.__display_legend
 
     @display_legend.setter
     def display_legend(self, display_legend):
         self.__display_legend = display_legend
+    
+    ###### Legend properties
+    
+    @property
+    def legend_x_anchor(self):
+        return self.__legend_x_anchor
+
+    @legend_x_anchor.setter
+    def legend_x_anchor(self, legend_x_anchor):
+        self.__legend_x_anchor = legend_x_anchor
+        
+    @property
+    def legend_y_anchor(self):
+        return self.__legend_y_anchor
+
+    @legend_y_anchor.setter
+    def legend_y_anchor(self, legend_y_anchor):
+        self.__legend_y_anchor = legend_y_anchor
+
+    @property
+    def legend_x_pos(self):
+        return self.__legend_x_pos
+
+    @legend_x_pos.setter
+    def legend_x_pos(self, legend_x_pos):
+        self.__legend_x_pos = legend_x_pos
 
+    @property
+    def legend_y_pos(self):
+        return self.__legend_y_pos
+
+    @legend_y_pos.setter
+    def legend_y_pos(self, legend_y_pos):
+        self.__legend_y_pos = legend_y_pos
+        
+    @property
+    def legend_bgcolor(self):
+        return self.__legend_bgcolor
 
+    @legend_bgcolor.setter
+    def legend_bgcolor(self, legend_bgcolor):
+        self.__legend_bgcolor = legend_bgcolor
+
+    @property
+    def legend_orientation(self):
+        return self.__legend_orientation
+
+    @legend_orientation.setter
+    def legend_orientation(self, legend_orientation):
+        self.__legend_orientation = legend_orientation
+        
     ###### matplotlib only
     @property
     def xkcd(self):
         return self.__xkcd
 
     @xkcd.setter
     def xkcd(self, xkcd):
```

### Comparing `chartpy-0.1.8/chartpy/stylesheets/538-chartpy.mplstyle` & `chartpy-0.1.9/chartpy/stylesheets/538-chartpy.mplstyle`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy/stylesheets/chartpy-pyfolio.mplstyle` & `chartpy-0.1.9/chartpy/stylesheets/chartpy-pyfolio.mplstyle`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy/stylesheets/chartpy.mplstyle` & `chartpy-0.1.9/chartpy/stylesheets/chartpy.mplstyle`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy/stylesheets/ggplot-chartpy.mplstyle` & `chartpy-0.1.9/chartpy/stylesheets/ggplot-chartpy.mplstyle`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy/stylesheets/ggplot-tradtional.mplstyle` & `chartpy-0.1.9/chartpy/stylesheets/ggplot-tradtional.mplstyle`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy/twitter.py` & `chartpy-0.1.9/chartpy/twitter.py`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy.egg-info/PKG-INFO` & `chartpy-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: chartpy
-Version: 0.1.8
+Version: 0.1.9
 Summary: chartpy creates a simple easy to use API to plot in a number of great Python chart libraries
 Home-page: https://github.com/cuemacro/chartpy
 Author: Saeed Amen
 Author-email: saeed@cuemacro.com
 License: Apache 2.0
 Description: chartpy creates a simple easy to use API to plot in a number of great Python chart libraries like plotly (via cufflinks),
         bokeh and matplotlib, with a unified interface. You simply need to change a single keyword to change which chart engine
```

### Comparing `chartpy-0.1.8/chartpy.egg-info/SOURCES.txt` & `chartpy-0.1.9/chartpy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,50 +4,32 @@
 MANIFEST.in
 README.md
 chartpy_logo.png
 create_package.bat
 create_python_package.md
 longdesc.md
 setup.py
+.github/FUNDING.yml
 chartpy/__init__.py
-chartpy/__init__.pyc
 chartpy/canvas.py
-chartpy/canvas.pyc
 chartpy/chart.py
-chartpy/chart.pyc
 chartpy/chartconstants.py
-chartpy/chartconstants.pyc
 chartpy/engine.py
-chartpy/engine.pyc
 chartpy/style.py
-chartpy/style.pyc
 chartpy/twitter.py
-chartpy/twitter.pyc
 chartpy.egg-info/PKG-INFO
 chartpy.egg-info/SOURCES.txt
 chartpy.egg-info/dependency_links.txt
 chartpy.egg-info/not-zip-safe
 chartpy.egg-info/requires.txt
 chartpy.egg-info/top_level.txt
-chartpy/__pycache__/__init__.cpython-35.pyc
-chartpy/__pycache__/__init__.cpython-36.pyc
-chartpy/__pycache__/canvas.cpython-35.pyc
-chartpy/__pycache__/canvas.cpython-36.pyc
-chartpy/__pycache__/chart.cpython-35.pyc
-chartpy/__pycache__/chart.cpython-36.pyc
-chartpy/__pycache__/chartconstants.cpython-35.pyc
-chartpy/__pycache__/chartconstants.cpython-36.pyc
-chartpy/__pycache__/chartcred.cpython-35.pyc
-chartpy/__pycache__/chartcred.cpython-36.pyc
-chartpy/__pycache__/engine.cpython-35.pyc
-chartpy/__pycache__/engine.cpython-36.pyc
-chartpy/__pycache__/style.cpython-35.pyc
-chartpy/__pycache__/style.cpython-36.pyc
-chartpy/__pycache__/twitter.cpython-35.pyc
-chartpy/__pycache__/twitter.cpython-36.pyc
+chartpy/dashboard/__init__.py
+chartpy/dashboard/layoutcanvas.py
+chartpy/dashboard/sessionmanager.py
+chartpy/dashboard/sketchcomponents.py
 chartpy/stylesheets/538-chartpy.mplstyle
 chartpy/stylesheets/__init__.py
 chartpy/stylesheets/chartpy-pyfolio.mplstyle
 chartpy/stylesheets/chartpy.mplstyle
 chartpy/stylesheets/ggplot-chartpy.mplstyle
 chartpy/stylesheets/ggplot-tradtional.mplstyle
 chartpy_examples/__init__.py
@@ -64,14 +46,30 @@
 chartpy_examples/subplot_examples.py
 chartpy_examples/surface_examples.py
 chartpy_examples/temp.html
 chartpy_examples/vispy_demo.py
 chartpy_examples/volsurface.csv
 chartpy_examples/volsurface.png
 chartpy_examples/xkcd_examples.py
+chartpy_examples/dashboard_examples/__init__.py
+chartpy_examples/dashboard_examples/assets/android-chrome-192x192.png
+chartpy_examples/dashboard_examples/assets/android-chrome-256x256.png
+chartpy_examples/dashboard_examples/assets/android-chrome-512x512.png
+chartpy_examples/dashboard_examples/assets/apple-touch-icon.png
+chartpy_examples/dashboard_examples/assets/browserconfig.xml
+chartpy_examples/dashboard_examples/assets/favicon-16x16.png
+chartpy_examples/dashboard_examples/assets/favicon-32x32.png
+chartpy_examples/dashboard_examples/assets/favicon.ico
+chartpy_examples/dashboard_examples/assets/head.htm
+chartpy_examples/dashboard_examples/assets/logo.png
+chartpy_examples/dashboard_examples/assets/logo_crop.png
+chartpy_examples/dashboard_examples/assets/mstile-150x150.png
+chartpy_examples/dashboard_examples/assets/safari-pinned-tab.svg
+chartpy_examples/dashboard_examples/assets/site.webmanifest
+chartpy_examples/dashboard_examples/assets/tabs.css
 chartpy_examples/notebooks/__init__.py
 chartpy_examples/notebooks/chart_examples.ipynb
 chartpy_examples/notebooks/s_bokeh.html
 chartpy_examples/notebooks/s_canvas.html
 chartpy_examples/notebooks/s_canvas_keen.html
 chartpy_examples/notebooks/s_canvas_plain.html
 chartpy_examples/notebooks/s_matplotlib.png
```

### Comparing `chartpy-0.1.8/chartpy_examples/barh.png` & `chartpy-0.1.9/chartpy_examples/barh.png`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/bokeh.html` & `chartpy-0.1.9/chartpy_examples/bokeh.html`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/canvas.png` & `chartpy-0.1.9/chartpy_examples/canvas.png`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/canvas_demo.py` & `chartpy-0.1.9/chartpy_examples/canvas_demo.py`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/chart_demo.py` & `chartpy-0.1.9/chartpy_examples/chart_demo.py`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/heatmap.png` & `chartpy-0.1.9/chartpy_examples/heatmap.png`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/chart_examples.ipynb` & `chartpy-0.1.9/chartpy_examples/notebooks/chart_examples.ipynb`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/css/bootstrap.min.css` & `chartpy-0.1.9/chartpy_examples/notebooks/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/css/iThing.css` & `chartpy-0.1.9/chartpy_examples/notebooks/static/css/iThing.css`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/css/keen-dashboards.css` & `chartpy-0.1.9/chartpy_examples/notebooks/static/css/keen-dashboards.css`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/css/keen-static.css` & `chartpy-0.1.9/chartpy_examples/notebooks/static/css/keen-static.css`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/fonts/glyphicons-halflings-regular.eot` & `chartpy-0.1.9/chartpy_examples/notebooks/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/fonts/glyphicons-halflings-regular.svg` & `chartpy-0.1.9/chartpy_examples/notebooks/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/fonts/glyphicons-halflings-regular.ttf` & `chartpy-0.1.9/chartpy_examples/notebooks/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/fonts/glyphicons-halflings-regular.woff` & `chartpy-0.1.9/chartpy_examples/notebooks/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/.bower.json` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/.bower.json`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/bower.json` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/bower.json`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/fonts/glyphicons-halflings-regular.eot` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/fonts/glyphicons-halflings-regular.svg` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/fonts/glyphicons-halflings-regular.ttf` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/fonts/glyphicons-halflings-regular.woff` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/grunt/bs-glyphicons-data-generator.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/grunt/bs-glyphicons-data-generator.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/grunt/bs-lessdoc-parser.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/grunt/bs-lessdoc-parser.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/grunt/bs-raw-files-generator.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/grunt/bs-raw-files-generator.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/grunt/sauce_browsers.yml` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/grunt/sauce_browsers.yml`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/Gruntfile.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/Gruntfile.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/js/affix.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/js/affix.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/js/alert.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/js/alert.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/js/button.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/js/button.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/js/carousel.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/js/carousel.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/js/collapse.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/js/collapse.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/js/dropdown.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/js/dropdown.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/js/modal.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/js/modal.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/js/popover.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/js/popover.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/js/scrollspy.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/js/scrollspy.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/js/tab.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/js/tab.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/js/tooltip.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/js/tooltip.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/js/transition.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/js/transition.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/alerts.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/alerts.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/badges.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/badges.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/bootstrap.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/bootstrap.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/breadcrumbs.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/breadcrumbs.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/button-groups.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/button-groups.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/buttons.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/buttons.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/carousel.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/carousel.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/close.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/close.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/code.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/code.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/component-animations.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/component-animations.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/dropdowns.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/dropdowns.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/forms.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/forms.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/glyphicons.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/glyphicons.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/grid.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/grid.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/input-groups.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/input-groups.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/jumbotron.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/jumbotron.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/labels.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/labels.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/list-group.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/list-group.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/media.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/media.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/buttons.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/buttons.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/clearfix.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/clearfix.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/forms.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/forms.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/gradients.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/gradients.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/grid-framework.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/grid-framework.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/grid.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/grid.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/hide-text.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/hide-text.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/image.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/image.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/list-group.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/list-group.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/panels.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/panels.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/table-row.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/table-row.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/vendor-prefixes.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins/vendor-prefixes.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/mixins.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/mixins.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/modals.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/modals.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/navbar.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/navbar.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/navs.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/navs.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/normalize.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/normalize.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/pager.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/pager.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/pagination.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/pagination.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/panels.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/panels.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/popovers.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/popovers.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/print.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/print.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/progress-bars.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/progress-bars.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/responsive-embed.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/responsive-embed.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/responsive-utilities.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/responsive-utilities.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/scaffolding.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/scaffolding.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/tables.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/tables.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/theme.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/theme.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/thumbnails.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/thumbnails.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/tooltip.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/tooltip.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/type.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/type.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/utilities.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/utilities.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/variables.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/variables.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/less/wells.less` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/less/wells.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/LICENSE` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/LICENSE`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/package.json` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/package.json`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/bootstrap/README.md` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/bootstrap/README.md`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/holderjs/composer.json` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/holderjs/composer.json`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/holderjs/Gruntfile.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/holderjs/Gruntfile.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/holderjs/holder.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/holderjs/holder.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/holderjs/package.json` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/holderjs/package.json`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/holderjs/README.md` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/holderjs/README.md`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/.bower.json` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/.bower.json`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/MIT-LICENSE.txt` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/ajax/jsonp.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/ajax/jsonp.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/ajax/load.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/ajax/load.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/ajax/parseXML.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/ajax/parseXML.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/ajax/script.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/ajax/script.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/ajax/xhr.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/ajax/xhr.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/ajax.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/ajax.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/attributes/attr.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/attributes/attr.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/attributes/classes.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/attributes/classes.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/attributes/prop.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/attributes/prop.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/attributes/support.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/attributes/support.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/attributes/val.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/attributes/val.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/callbacks.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/callbacks.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/core/access.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/core/access.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/core/init.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/core/init.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/core/parseHTML.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/core/parseHTML.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/core/ready.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/core/ready.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/core.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/core.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/css/addGetHookIf.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/css/addGetHookIf.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/css/curCSS.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/css/curCSS.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/css/defaultDisplay.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/css/defaultDisplay.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/css/support.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/css/support.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/css/swap.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/css/swap.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/css.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/css.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/data/Data.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/data/Data.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/data.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/data.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/deferred.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/deferred.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/dimensions.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/dimensions.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/effects/Tween.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/effects/Tween.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/effects.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/effects.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/event/alias.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/event/alias.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/event.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/event.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/exports/amd.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/exports/amd.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/exports/global.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/exports/global.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/intro.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/intro.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/jquery.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/jquery.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/manipulation/support.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/manipulation/support.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/manipulation.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/manipulation.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/offset.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/offset.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/queue/delay.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/queue/delay.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/queue.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/queue.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/selector-native.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/selector-native.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/serialize.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/serialize.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/traversing/findFilter.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/traversing/findFilter.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/traversing.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/traversing.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery/src/wrap.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery/src/wrap.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery-knob/.bower.json` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery-knob/.bower.json`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery-knob/excanvas.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery-knob/excanvas.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery-knob/index.html` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery-knob/index.html`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery-knob/js/jquery.knob.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery-knob/js/jquery.knob.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery-knob/knob.jquery.json` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery-knob/knob.jquery.json`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery-knob/LICENSE` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery-knob/LICENSE`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery-knob/README.md` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery-knob/README.md`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/jquery-knob/secretplan.jpg` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/jquery-knob/secretplan.jpg`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/keen-js/.bower.json` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/keen-js/.bower.json`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/keen-js/bower.json` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/keen-js/bower.json`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/keen-js/LICENSE` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/keen-js/LICENSE`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/meta.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/meta.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/slider/jQDateRangeSlider.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/slider/jQDateRangeSlider.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/slider/jQDateRangeSliderHandle.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/slider/jQDateRangeSliderHandle.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/slider/jQRangeSlider.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/slider/jQRangeSlider.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/slider/jQRangeSliderBar.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/slider/jQRangeSliderBar.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/slider/jQRangeSliderDraggable.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/slider/jQRangeSliderDraggable.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/slider/jQRangeSliderHandle.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/slider/jQRangeSliderHandle.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/slider/jQRangeSliderLabel.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/slider/jQRangeSliderLabel.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/slider/jQRangeSliderMouseTouch.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/slider/jQRangeSliderMouseTouch.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/slider/jQRuler.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/slider/jQRuler.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/slider/jquery-1.7.2.min.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/slider/jquery-1.7.2.min.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/slider/jquery-ui.min.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/slider/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/static/js/slider/slider.js` & `chartpy-0.1.9/chartpy_examples/notebooks/static/js/slider/slider.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/s_bokeh.html` & `chartpy-0.1.9/chartpy_examples/notebooks/s_bokeh.html`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/s_canvas.html` & `chartpy-0.1.9/chartpy_examples/notebooks/s_canvas.html`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/s_canvas_keen.html` & `chartpy-0.1.9/chartpy_examples/notebooks/s_canvas_keen.html`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/s_canvas_plain.html` & `chartpy-0.1.9/chartpy_examples/notebooks/s_canvas_plain.html`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/s_matplotlib.png` & `chartpy-0.1.9/chartpy_examples/notebooks/s_matplotlib.png`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/s_plotly.html` & `chartpy-0.1.9/chartpy_examples/notebooks/s_plotly.html`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/notebooks/web_page_examples.ipynb` & `chartpy-0.1.9/chartpy_examples/notebooks/web_page_examples.ipynb`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/plotly.html` & `chartpy-0.1.9/chartpy_examples/plotly.html`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/plotlyheatmap.png` & `chartpy-0.1.9/chartpy_examples/plotlyheatmap.png`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/screenshot.png` & `chartpy-0.1.9/chartpy_examples/screenshot.png`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/css/bootstrap.min.css` & `chartpy-0.1.9/chartpy_examples/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/css/iThing.css` & `chartpy-0.1.9/chartpy_examples/static/css/iThing.css`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/css/keen-dashboards.css` & `chartpy-0.1.9/chartpy_examples/static/css/keen-dashboards.css`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/css/keen-static.css` & `chartpy-0.1.9/chartpy_examples/static/css/keen-static.css`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/fonts/glyphicons-halflings-regular.eot` & `chartpy-0.1.9/chartpy_examples/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/fonts/glyphicons-halflings-regular.svg` & `chartpy-0.1.9/chartpy_examples/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/fonts/glyphicons-halflings-regular.ttf` & `chartpy-0.1.9/chartpy_examples/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/fonts/glyphicons-halflings-regular.woff` & `chartpy-0.1.9/chartpy_examples/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/.bower.json` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/.bower.json`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/bower.json` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/bower.json`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/fonts/glyphicons-halflings-regular.eot` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/fonts/glyphicons-halflings-regular.svg` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/fonts/glyphicons-halflings-regular.ttf` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/fonts/glyphicons-halflings-regular.woff` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/grunt/bs-glyphicons-data-generator.js` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/grunt/bs-glyphicons-data-generator.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/grunt/bs-lessdoc-parser.js` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/grunt/bs-lessdoc-parser.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/grunt/bs-raw-files-generator.js` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/grunt/bs-raw-files-generator.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/grunt/sauce_browsers.yml` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/grunt/sauce_browsers.yml`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/Gruntfile.js` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/Gruntfile.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/js/affix.js` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/js/affix.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/js/alert.js` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/js/alert.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/js/button.js` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/js/button.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/js/carousel.js` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/js/carousel.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/js/collapse.js` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/js/collapse.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/js/dropdown.js` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/js/dropdown.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/js/modal.js` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/js/modal.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/js/popover.js` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/js/popover.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/js/scrollspy.js` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/js/scrollspy.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/js/tab.js` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/js/tab.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/js/tooltip.js` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/js/tooltip.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/js/transition.js` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/js/transition.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/alerts.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/alerts.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/badges.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/badges.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/bootstrap.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/bootstrap.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/breadcrumbs.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/breadcrumbs.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/button-groups.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/button-groups.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/buttons.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/buttons.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/carousel.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/carousel.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/close.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/close.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/code.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/code.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/component-animations.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/component-animations.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/dropdowns.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/dropdowns.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/forms.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/forms.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/glyphicons.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/glyphicons.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/grid.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/grid.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/input-groups.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/input-groups.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/jumbotron.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/jumbotron.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/labels.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/labels.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/list-group.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/list-group.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/media.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/media.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/buttons.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/buttons.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/clearfix.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/clearfix.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/forms.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/forms.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/gradients.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/gradients.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/grid-framework.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/grid-framework.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/grid.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/grid.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/hide-text.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/hide-text.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/image.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/image.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/list-group.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/list-group.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/panels.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/panels.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/table-row.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/table-row.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins/vendor-prefixes.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins/vendor-prefixes.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/mixins.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/mixins.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/modals.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/modals.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/navbar.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/navbar.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/navs.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/navs.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/normalize.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/normalize.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/pager.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/pager.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/pagination.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/pagination.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/panels.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/panels.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/popovers.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/popovers.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/print.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/print.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/progress-bars.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/progress-bars.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/responsive-embed.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/responsive-embed.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/responsive-utilities.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/responsive-utilities.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/scaffolding.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/scaffolding.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/tables.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/tables.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/theme.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/theme.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/thumbnails.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/thumbnails.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/tooltip.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/tooltip.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/type.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/type.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/utilities.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/utilities.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/variables.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/variables.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/less/wells.less` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/less/wells.less`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/LICENSE` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/LICENSE`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/package.json` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/package.json`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/bootstrap/README.md` & `chartpy-0.1.9/chartpy_examples/static/js/bootstrap/README.md`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/holderjs/composer.json` & `chartpy-0.1.9/chartpy_examples/static/js/holderjs/composer.json`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/holderjs/Gruntfile.js` & `chartpy-0.1.9/chartpy_examples/static/js/holderjs/Gruntfile.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/holderjs/holder.js` & `chartpy-0.1.9/chartpy_examples/static/js/holderjs/holder.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/holderjs/package.json` & `chartpy-0.1.9/chartpy_examples/static/js/holderjs/package.json`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/holderjs/README.md` & `chartpy-0.1.9/chartpy_examples/static/js/holderjs/README.md`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/.bower.json` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/.bower.json`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/MIT-LICENSE.txt` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/ajax/jsonp.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/ajax/jsonp.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/ajax/load.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/ajax/load.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/ajax/parseXML.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/ajax/parseXML.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/ajax/script.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/ajax/script.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/ajax/xhr.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/ajax/xhr.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/ajax.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/ajax.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/attributes/attr.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/attributes/attr.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/attributes/classes.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/attributes/classes.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/attributes/prop.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/attributes/prop.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/attributes/support.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/attributes/support.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/attributes/val.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/attributes/val.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/callbacks.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/callbacks.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/core/access.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/core/access.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/core/init.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/core/init.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/core/parseHTML.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/core/parseHTML.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/core/ready.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/core/ready.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/core.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/core.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/css/addGetHookIf.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/css/addGetHookIf.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/css/curCSS.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/css/curCSS.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/css/defaultDisplay.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/css/defaultDisplay.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/css/support.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/css/support.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/css/swap.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/css/swap.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/css.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/css.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/data/Data.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/data/Data.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/data.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/data.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/deferred.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/deferred.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/dimensions.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/dimensions.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/effects/Tween.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/effects/Tween.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/effects.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/effects.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/event/alias.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/event/alias.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/event.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/event.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/exports/amd.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/exports/amd.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/exports/global.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/exports/global.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/intro.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/intro.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/jquery.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/jquery.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/manipulation/support.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/manipulation/support.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/manipulation.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/manipulation.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/offset.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/offset.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/queue/delay.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/queue/delay.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/queue.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/queue.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/selector-native.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/selector-native.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/serialize.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/serialize.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/traversing/findFilter.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/traversing/findFilter.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/traversing.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/traversing.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery/src/wrap.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery/src/wrap.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery-knob/.bower.json` & `chartpy-0.1.9/chartpy_examples/static/js/jquery-knob/.bower.json`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery-knob/excanvas.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery-knob/excanvas.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery-knob/index.html` & `chartpy-0.1.9/chartpy_examples/static/js/jquery-knob/index.html`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery-knob/js/jquery.knob.js` & `chartpy-0.1.9/chartpy_examples/static/js/jquery-knob/js/jquery.knob.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery-knob/knob.jquery.json` & `chartpy-0.1.9/chartpy_examples/static/js/jquery-knob/knob.jquery.json`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery-knob/LICENSE` & `chartpy-0.1.9/chartpy_examples/static/js/jquery-knob/LICENSE`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery-knob/README.md` & `chartpy-0.1.9/chartpy_examples/static/js/jquery-knob/README.md`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/jquery-knob/secretplan.jpg` & `chartpy-0.1.9/chartpy_examples/static/js/jquery-knob/secretplan.jpg`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/keen-js/.bower.json` & `chartpy-0.1.9/chartpy_examples/static/js/keen-js/.bower.json`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/keen-js/bower.json` & `chartpy-0.1.9/chartpy_examples/static/js/keen-js/bower.json`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/keen-js/LICENSE` & `chartpy-0.1.9/chartpy_examples/static/js/keen-js/LICENSE`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/meta.js` & `chartpy-0.1.9/chartpy_examples/static/js/meta.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/slider/jQDateRangeSlider.js` & `chartpy-0.1.9/chartpy_examples/static/js/slider/jQDateRangeSlider.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/slider/jQDateRangeSliderHandle.js` & `chartpy-0.1.9/chartpy_examples/static/js/slider/jQDateRangeSliderHandle.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/slider/jQRangeSlider.js` & `chartpy-0.1.9/chartpy_examples/static/js/slider/jQRangeSlider.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/slider/jQRangeSliderBar.js` & `chartpy-0.1.9/chartpy_examples/static/js/slider/jQRangeSliderBar.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/slider/jQRangeSliderDraggable.js` & `chartpy-0.1.9/chartpy_examples/static/js/slider/jQRangeSliderDraggable.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/slider/jQRangeSliderHandle.js` & `chartpy-0.1.9/chartpy_examples/static/js/slider/jQRangeSliderHandle.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/slider/jQRangeSliderLabel.js` & `chartpy-0.1.9/chartpy_examples/static/js/slider/jQRangeSliderLabel.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/slider/jQRangeSliderMouseTouch.js` & `chartpy-0.1.9/chartpy_examples/static/js/slider/jQRangeSliderMouseTouch.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/slider/jQRuler.js` & `chartpy-0.1.9/chartpy_examples/static/js/slider/jQRuler.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/slider/jquery-1.7.2.min.js` & `chartpy-0.1.9/chartpy_examples/static/js/slider/jquery-1.7.2.min.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/slider/jquery-ui.min.js` & `chartpy-0.1.9/chartpy_examples/static/js/slider/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/static/js/slider/slider.js` & `chartpy-0.1.9/chartpy_examples/static/js/slider/slider.js`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/subplot.png` & `chartpy-0.1.9/chartpy_examples/subplot.png`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/subplot_examples.py` & `chartpy-0.1.9/chartpy_examples/subplot_examples.py`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/surface_examples.py` & `chartpy-0.1.9/chartpy_examples/surface_examples.py`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/temp.html` & `chartpy-0.1.9/chartpy_examples/temp.html`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/vispy_demo.py` & `chartpy-0.1.9/chartpy_examples/vispy_demo.py`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/volsurface.csv` & `chartpy-0.1.9/chartpy_examples/volsurface.csv`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/volsurface.png` & `chartpy-0.1.9/chartpy_examples/volsurface.png`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_examples/xkcd_examples.py` & `chartpy-0.1.9/chartpy_examples/xkcd_examples.py`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/chartpy_logo.png` & `chartpy-0.1.9/chartpy_logo.png`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/create_python_package.md` & `chartpy-0.1.9/create_python_package.md`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/LICENCE` & `chartpy-0.1.9/LICENCE`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/longdesc.md` & `chartpy-0.1.9/longdesc.md`

 * *Files identical despite different names*

### Comparing `chartpy-0.1.8/PKG-INFO` & `chartpy-0.1.9/chartpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: chartpy
-Version: 0.1.8
+Version: 0.1.9
 Summary: chartpy creates a simple easy to use API to plot in a number of great Python chart libraries
 Home-page: https://github.com/cuemacro/chartpy
 Author: Saeed Amen
 Author-email: saeed@cuemacro.com
 License: Apache 2.0
 Description: chartpy creates a simple easy to use API to plot in a number of great Python chart libraries like plotly (via cufflinks),
         bokeh and matplotlib, with a unified interface. You simply need to change a single keyword to change which chart engine
```

### Comparing `chartpy-0.1.8/README.md` & `chartpy-0.1.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 and text, with just a few lines of Python! The HTML file can then be uploaded to a webserver for display (or sent around by e-mail etc)
 
 <img src="https://github.com/cuemacro/chartpy/blob/master/chartpy_examples/canvas.png?raw=true" width="543"/>
 
 # Requirements
 
 Major requirements
-* Required: Python 3.4, 3.5, 3.6
+* Required: Python 3.7
 * Required: pandas, matplotlib, plotly, cufflinks, bokeh, numpy etc.
 
 # To install Open Sans font
 
 My chartpy stylesheet for matplotlib uses the free Open Sans font. For it to display properly you need to install Open Sans font
 on your computer
 * First download font from https://www.fontsquirrel.com/fonts/open-sans
@@ -121,33 +121,65 @@
 concentrate on analysing data, rather than getting caught up in complex API visualisation calls. Rather than
 having to totally edit my code each time, a single keyword is enough to switch between for example plotly and matplotlib.
 
 I've also tried to design the library so that adding a new plotting engine is fairly straightforward (extend EngineTemplate
 and edit the get_engine method in Chart), so it's basically future proof for whatever new chart libraries come along, with
 relatively small changes to your code base.
 
+# Interactive Web Dashboards with chartpy/dash
+
+chartpy also has interactive dashboards based on Plotly's Dash package, but with a lot less of the boilerplate code
+which Dash uses. Users extend `LayoutCanvas` to create their own Dash layouts and `SketchComponents` can be used
+to quickly create Dash components/HTML components, with relatively few lines of code.
+
+Hence, it's a lot quicker to create Dash based dashboards in chartpy! In the future, we want
+to also support other Python dashboards like [H2O Wave](https://www.h2o.ai/products/h2o-wave/).
+
+You'll need to install Dash as an extra
+to use them as they aren't part of the default installation, which we can see below:
+
+    pip install cufflinks==0.17.3 plotly==4.14.3 kaleido dash==1.20.0 \
+      dash-html-components==1.1.3 dash-core-components==1.16.0 dash-table==4.11.3 \
+      jupyter-dash==0.4.0 chart_studio==1.1.0
+
 # Contributors
 
 Contributors are always welcome for finmarketpy, findatapy and chartpy. If you'd like to contribute, have a look at
 [Planned Features](https://github.com/cuemacro/finmarketpy/blob/master/PLANNED_FEATURES.md) for areas we're looking for help on. 
 Or if you have any ideas for improvements to the libriares please let us know too!
 
 # chartpy examples
 
 In chartpy/examples you will find several demos
 
 # Recent Release Notes
 
-* 08 Jun 2020 - v0.1.7
+* 04 May 2021 - v0.1.9
+* 08 Jun 2020 - v0.1.8
+* 06 May 2020 - v0.1.7
 * 06 Apr 2020 - v0.1.6
 * 02 Apr 2020 - v0.1.5
 * 23 Oct 2019 - v0.1.4 
 
 # Coding log
 
+* 04 May 2021
+  * Changed default widths for dashboard
+* 03 May 2021
+  * Spinning out some Dash visualization tools from tcapy to chartpy
+* 19 Apr 2021
+  * Add region plot
+* 15 Apr 2021
+  * Constant overrides now persist
+* 13 Apr 2021
+    * Can add second y-axis labels for Plotly
+* 22 Mar 2021
+    * Added more formatting for Plotly (eg. text font etc.)
+* 02 Dec 2020
+    * Added animation for Plotly
 * 08 Jun 2020
     * Now requires Plotly >=4.5.1
     * Fixed setup.py to install chart-studio
 * 06 May 2020 - Plotly can now export to PNG
 * 02 Apr 2020 - Plotly can now produce SVG
 * 02 Nov 2019 - Now supports Plotly 4.x with Cufflinks 0.17
 * 23 Oct 2019 - Added advisory on Plotly 3.10 and Cufflinks 0.16
```

### Comparing `chartpy-0.1.8/setup.py` & `chartpy-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 long_description = """chartpy creates a simple easy to use API to plot in a number of great Python chart libraries like plotly (via cufflinks),
 bokeh and matplotlib, with a unified interface. You simply need to change a single keyword to change which chart engine
 to use (see below), rather than having to learn the low level details of each library. I've also created new stylesheets
 and formatting to ensure that the default matplotlib styling looks more modern using Open Sans font. The library
 also works well with Dash, plotly's web server library built on top of Flask."""
 
 setup(name='chartpy',
-      version='0.1.8',
+      version='0.1.9',
       description='chartpy creates a simple easy to use API to plot in a number of great Python chart libraries',
       author='Saeed Amen',
       author_email='saeed@cuemacro.com',
       long_description=long_description,
       license='Apache 2.0',
       keywords=['pandas', 'chart', 'plot', 'plotly'],
       url='https://github.com/cuemacro/chartpy',
```

