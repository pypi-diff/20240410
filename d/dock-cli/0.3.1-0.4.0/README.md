# Comparing `tmp/dock-cli-0.3.1.tar.gz` & `tmp/dock-cli-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dock-cli-0.3.1.tar", last modified: Tue Apr  2 07:58:38 2024, max compression
+gzip compressed data, was "dock-cli-0.4.0.tar", last modified: Tue Apr  9 17:13:55 2024, max compression
```

## Comparing `dock-cli-0.3.1.tar` & `dock-cli-0.4.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 posen      (501) staff       (20)        0 2024-04-02 07:58:38.916898 dock-cli-0.3.1/
--rw-r--r--   0 posen      (501) staff       (20)     1062 2024-03-05 06:48:54.000000 dock-cli-0.3.1/LICENSE
--rw-r--r--   0 posen      (501) staff       (20)     1957 2024-04-02 07:58:38.916599 dock-cli-0.3.1/PKG-INFO
--rw-r--r--   0 posen      (501) staff       (20)     1693 2024-03-25 15:48:25.000000 dock-cli-0.3.1/README.md
-drwxr-xr-x   0 posen      (501) staff       (20)        0 2024-04-02 07:58:38.911925 dock-cli-0.3.1/dock_cli/
--rw-r--r--   0 posen      (501) staff       (20)        0 2024-03-21 16:14:08.000000 dock-cli-0.3.1/dock_cli/__init__.py
-drwxr-xr-x   0 posen      (501) staff       (20)        0 2024-04-02 07:58:38.913801 dock-cli-0.3.1/dock_cli/cli/
--rw-r--r--   0 posen      (501) staff       (20)        0 2024-03-21 16:14:08.000000 dock-cli-0.3.1/dock_cli/cli/__init__.py
--rw-r--r--   0 posen      (501) staff       (20)     3934 2024-04-01 06:10:49.000000 dock-cli-0.3.1/dock_cli/cli/chart.py
--rw-r--r--   0 posen      (501) staff       (20)     5507 2024-04-01 06:10:50.000000 dock-cli-0.3.1/dock_cli/cli/image.py
--rw-r--r--   0 posen      (501) staff       (20)     2246 2024-04-01 06:39:15.000000 dock-cli-0.3.1/dock_cli/main.py
-drwxr-xr-x   0 posen      (501) staff       (20)        0 2024-04-02 07:58:38.915929 dock-cli-0.3.1/dock_cli/utils/
--rw-r--r--   0 posen      (501) staff       (20)        0 2024-03-21 16:14:08.000000 dock-cli-0.3.1/dock_cli/utils/__init__.py
--rw-r--r--   0 posen      (501) staff       (20)      797 2024-04-01 14:33:14.000000 dock-cli-0.3.1/dock_cli/utils/callback.py
--rw-r--r--   0 posen      (501) staff       (20)      629 2024-03-21 16:14:08.000000 dock-cli-0.3.1/dock_cli/utils/commands.py
--rw-r--r--   0 posen      (501) staff       (20)     4767 2024-04-02 03:20:25.000000 dock-cli-0.3.1/dock_cli/utils/helpers.py
--rw-r--r--   0 posen      (501) staff       (20)      530 2024-04-02 03:22:43.000000 dock-cli-0.3.1/dock_cli/utils/schema.py
--rw-r--r--   0 posen      (501) staff       (20)     2021 2024-04-01 06:22:14.000000 dock-cli-0.3.1/dock_cli/utils/utils.py
-drwxr-xr-x   0 posen      (501) staff       (20)        0 2024-04-02 07:58:38.916279 dock-cli-0.3.1/dock_cli.egg-info/
--rw-r--r--   0 posen      (501) staff       (20)     1957 2024-04-02 07:58:38.000000 dock-cli-0.3.1/dock_cli.egg-info/PKG-INFO
--rw-r--r--   0 posen      (501) staff       (20)      483 2024-04-02 07:58:38.000000 dock-cli-0.3.1/dock_cli.egg-info/SOURCES.txt
--rw-r--r--   0 posen      (501) staff       (20)        1 2024-04-02 07:58:38.000000 dock-cli-0.3.1/dock_cli.egg-info/dependency_links.txt
--rw-r--r--   0 posen      (501) staff       (20)       43 2024-04-02 07:58:38.000000 dock-cli-0.3.1/dock_cli.egg-info/entry_points.txt
--rw-r--r--   0 posen      (501) staff       (20)       13 2024-04-02 07:58:38.000000 dock-cli-0.3.1/dock_cli.egg-info/requires.txt
--rw-r--r--   0 posen      (501) staff       (20)        9 2024-04-02 07:58:38.000000 dock-cli-0.3.1/dock_cli.egg-info/top_level.txt
--rw-r--r--   0 posen      (501) staff       (20)       38 2024-04-02 07:58:38.916949 dock-cli-0.3.1/setup.cfg
--rw-r--r--   0 posen      (501) staff       (20)      619 2024-04-01 06:46:51.000000 dock-cli-0.3.1/setup.py
+drwxr-xr-x   0 posen      (501) staff       (20)        0 2024-04-09 17:13:55.047094 dock-cli-0.4.0/
+-rw-r--r--   0 posen      (501) staff       (20)     1062 2024-03-05 06:48:54.000000 dock-cli-0.4.0/LICENSE
+-rw-r--r--   0 posen      (501) staff       (20)     1957 2024-04-09 17:13:55.046790 dock-cli-0.4.0/PKG-INFO
+-rw-r--r--   0 posen      (501) staff       (20)     1693 2024-03-25 15:48:25.000000 dock-cli-0.4.0/README.md
+drwxr-xr-x   0 posen      (501) staff       (20)        0 2024-04-09 17:13:55.042715 dock-cli-0.4.0/dock_cli/
+-rw-r--r--   0 posen      (501) staff       (20)        0 2024-03-21 16:14:08.000000 dock-cli-0.4.0/dock_cli/__init__.py
+drwxr-xr-x   0 posen      (501) staff       (20)        0 2024-04-09 17:13:55.044591 dock-cli-0.4.0/dock_cli/cli/
+-rw-r--r--   0 posen      (501) staff       (20)        0 2024-03-21 16:14:08.000000 dock-cli-0.4.0/dock_cli/cli/__init__.py
+-rw-r--r--   0 posen      (501) staff       (20)     4041 2024-04-09 16:22:11.000000 dock-cli-0.4.0/dock_cli/cli/chart.py
+-rw-r--r--   0 posen      (501) staff       (20)     5822 2024-04-09 16:21:37.000000 dock-cli-0.4.0/dock_cli/cli/image.py
+-rw-r--r--   0 posen      (501) staff       (20)     2246 2024-04-02 09:30:09.000000 dock-cli-0.4.0/dock_cli/main.py
+drwxr-xr-x   0 posen      (501) staff       (20)        0 2024-04-09 17:13:55.046116 dock-cli-0.4.0/dock_cli/utils/
+-rw-r--r--   0 posen      (501) staff       (20)        0 2024-03-21 16:14:08.000000 dock-cli-0.4.0/dock_cli/utils/__init__.py
+-rw-r--r--   0 posen      (501) staff       (20)      797 2024-04-01 14:33:14.000000 dock-cli-0.4.0/dock_cli/utils/callback.py
+-rw-r--r--   0 posen      (501) staff       (20)      629 2024-03-21 16:14:08.000000 dock-cli-0.4.0/dock_cli/utils/commands.py
+-rw-r--r--   0 posen      (501) staff       (20)     5357 2024-04-09 17:10:08.000000 dock-cli-0.4.0/dock_cli/utils/helpers.py
+-rw-r--r--   0 posen      (501) staff       (20)      530 2024-04-02 03:22:43.000000 dock-cli-0.4.0/dock_cli/utils/schema.py
+-rw-r--r--   0 posen      (501) staff       (20)     2021 2024-04-01 06:22:14.000000 dock-cli-0.4.0/dock_cli/utils/utils.py
+drwxr-xr-x   0 posen      (501) staff       (20)        0 2024-04-09 17:13:55.046499 dock-cli-0.4.0/dock_cli.egg-info/
+-rw-r--r--   0 posen      (501) staff       (20)     1957 2024-04-09 17:13:55.000000 dock-cli-0.4.0/dock_cli.egg-info/PKG-INFO
+-rw-r--r--   0 posen      (501) staff       (20)      483 2024-04-09 17:13:55.000000 dock-cli-0.4.0/dock_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 posen      (501) staff       (20)        1 2024-04-09 17:13:55.000000 dock-cli-0.4.0/dock_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 posen      (501) staff       (20)       43 2024-04-09 17:13:55.000000 dock-cli-0.4.0/dock_cli.egg-info/entry_points.txt
+-rw-r--r--   0 posen      (501) staff       (20)       13 2024-04-09 17:13:55.000000 dock-cli-0.4.0/dock_cli.egg-info/requires.txt
+-rw-r--r--   0 posen      (501) staff       (20)        9 2024-04-09 17:13:55.000000 dock-cli-0.4.0/dock_cli.egg-info/top_level.txt
+-rw-r--r--   0 posen      (501) staff       (20)       38 2024-04-09 17:13:55.047144 dock-cli-0.4.0/setup.cfg
+-rw-r--r--   0 posen      (501) staff       (20)      619 2024-04-09 17:08:01.000000 dock-cli-0.4.0/setup.py
```

### Comparing `dock-cli-0.3.1/LICENSE` & `dock-cli-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dock-cli-0.3.1/PKG-INFO` & `dock-cli-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dock-cli
-Version: 0.3.1
+Version: 0.4.0
 Summary: CLI for manage container applications
 Author: Posen
 Author-email: posen2101024@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click==8.1.7
```

### Comparing `dock-cli-0.3.1/README.md` & `dock-cli-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `dock-cli-0.3.1/dock_cli/cli/chart.py` & `dock-cli-0.4.0/dock_cli/cli/chart.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import configparser
+import logging
 import click
 from dock_cli.utils import callback as cb
 from dock_cli.utils import commands as cmd
 from dock_cli.utils import helpers as hlp
 from dock_cli.utils import utils
 from dock_cli.utils.schema import ChartConfigOptions as Chart, SectionType
 
@@ -54,41 +55,46 @@
 @click.option('--destination', required=False, type=click.Path(file_okay=False, writable=True), default='.')
 def chart_push(obj, sections, destination):
     for section in sections:
         cmd.run([obj.command.helm, 'push',
                  obj.helper.get_chart_archive_file(section, destination),
                  obj.helper.get_section_registry(section)])
 
-@cli.group(name='config', invoke_without_command=True, cls=hlp.OrderedGroup)
-@click.pass_context
-def config_cli(ctx):
+@cli.group(name='config', cls=hlp.OrderedGroup)
+def config_cli():
     """Manage charts' configuration
 
     This is a command line interface for manage charts' configuration
     """
-    if ctx.invoked_subcommand is None:
-        for section in ctx.obj.helper.get_charts():
-            utils.print_chart_config(ctx.obj.config, section)
-
-@config_cli.command(name='init',
-                    help='Initialize chart default settings in the configuration')
-@click.pass_obj
-@click.option('--registry', required=False, type=str, default='oci://registry-1.docker.io/namespace', show_default=True,
-              help='Default oci registry for all charts.')
-def config_init(obj, registry):
-    utils.set_config_option(obj.config, configparser.DEFAULTSECT, Chart.REGISTRY, registry)
+
+@config_cli.command(name='view',
+                    help="View current charts' configuration")
+@click.pass_obj
+def config_view(obj):
+    sections = obj.helper.get_charts()
+    if not sections:
+        logging.getLogger(__name__).warning('No charts found.')
     for section in obj.helper.get_charts():
         utils.print_chart_config(obj.config, section)
-    utils.update_config(obj.config, obj.config_file)
 
-@config_cli.command(name='add',
+@config_cli.command(name='set',
                     help='Add or update an chart section in the configuration')
 @click.pass_obj
 @click.argument('section', required=True, type=click.Path(exists=True, file_okay=False),
                 callback=cb.transform_to_section)
 def config_set(obj, section):
     if obj.config.has_section(section) is False:
         obj.config.add_section(section)
     utils.set_config_option(obj.config, section, Chart.TYPE, SectionType.CHART)
     obj.helper.validate_section(section)
     utils.print_chart_config(obj.config, section)
     utils.update_config(obj.config, obj.config_file)
+
+@config_cli.command(name='set-registry',
+                    help='Set default registry for all charts in the configuration')
+@click.pass_obj
+@click.argument('registry', required=False, type=str, default='oci://registry-1.docker.io/namespace')
+def config_set_registry(obj, registry):
+    utils.set_config_option(obj.config, configparser.DEFAULTSECT, Chart.REGISTRY, registry)
+    for section in obj.helper.get_charts():
+        utils.print_chart_config(obj.config, section)
+    utils.update_config(obj.config, obj.config_file)
```

### Comparing `dock-cli-0.3.1/dock_cli/cli/image.py` & `dock-cli-0.4.0/dock_cli/cli/image.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import configparser
 import itertools
+import logging
 import click
 from dock_cli.utils import callback as cb
 from dock_cli.utils import commands as cmd
 from dock_cli.utils import helpers as hlp
 from dock_cli.utils import utils
 from dock_cli.utils.schema import ImageConfigOptions as Image, SectionType
 
@@ -72,53 +73,61 @@
               help='Specify one or multiple tags for the image')
 def image_clean(obj, sections, tags):
     for section in sections:
         obj.helper.validate_section(section)
         for tag in tags:
             cmd.run([obj.command.docker, 'rmi', '--force', obj.helper.get_image(section, tag)])
 
-@cli.group(name='config', invoke_without_command=True, cls=hlp.OrderedGroup)
-@click.pass_context
-def config_cli(ctx):
+@cli.group(name='config', cls=hlp.OrderedGroup)
+def config_cli():
     """Manage images' configuration
 
     This is a command line interface for manage images' configuration
     """
-    if ctx.invoked_subcommand is None:
-        for section in ctx.obj.helper.get_images():
-            utils.print_image_config(ctx.obj.config, section)
-
-@config_cli.command(name='init',
-                    help='Initialize image default settings in the configuration')
-@click.pass_obj
-@click.option('--registry', required=False, type=str, default='namespace',
-              help='Default registry for all images.')
-def config_init(obj, registry):
-    utils.set_config_option(obj.config, configparser.DEFAULTSECT, Image.REGISTRY, registry)
-    for section in obj.helper.get_images():
+
+@config_cli.command(name='view',
+                    help="View current images' configuration")
+@click.pass_obj
+def config_view(obj):
+    sections = obj.helper.get_images()
+    if not sections:
+        logging.getLogger(__name__).warning('No images found.')
+    for section in sections:
         utils.print_image_config(obj.config, section)
-    utils.update_config(obj.config, obj.config_file)
 
-@config_cli.command(name='add',
+@config_cli.command(name='set',
                     help='Add or update an image section in the configuration')
 @click.pass_obj
 @click.argument('section', required=True, type=click.Path(exists=True, file_okay=False),
                 callback=cb.transform_to_section)
+@click.option('--registry', required=False, type=str,
+              help='Name of the registry for this section.')
 @click.option('--file', required=False, type=str, default='Dockerfile', show_default=True,
               help='Name of the Dockerfile for this section.')
 @click.option('--name', required=False, type=str,
               help='Name of the image for this section.')
 @click.option('--depends-on', required=False, multiple=True,
               type=click.Path(exists=True, file_okay=False),
               callback=cb.multiline_sections,
               help='List of sections or paths that this section depends on.')
-def config_add(obj, section, file, name, depends_on):
+def config_set(obj, section, registry, file, name, depends_on):
     # pylint: disable=too-many-arguments
     if obj.config.has_section(section) is False:
         obj.config.add_section(section)
+    utils.set_config_option(obj.config, section, Image.REGISTRY, registry)
     utils.set_config_option(obj.config, section, Image.FILE, file)
     utils.set_config_option(obj.config, section, Image.NAME, name)
     utils.set_config_option(obj.config, section, Image.DEPENDS_ON, depends_on)
     utils.set_config_option(obj.config, section, Image.TYPE, SectionType.IMAGE)
     obj.helper.validate_section(section)
     utils.print_image_config(obj.config, section)
     utils.update_config(obj.config, obj.config_file)
+
+@config_cli.command(name='set-registry',
+                    help='Set default registry for all images in the configuration')
+@click.pass_obj
+@click.argument('registry', required=False, type=str, default='namespace')
+def config_set_registry(obj, registry):
+    utils.set_config_option(obj.config, configparser.DEFAULTSECT, Image.REGISTRY, registry)
+    for section in obj.helper.get_images():
+        utils.print_image_config(obj.config, section)
+    utils.update_config(obj.config, obj.config_file)
```

### Comparing `dock-cli-0.3.1/dock_cli/main.py` & `dock-cli-0.4.0/dock_cli/main.py`

 * *Files identical despite different names*

### Comparing `dock-cli-0.3.1/dock_cli/utils/callback.py` & `dock-cli-0.4.0/dock_cli/utils/callback.py`

 * *Files identical despite different names*

### Comparing `dock-cli-0.3.1/dock_cli/utils/commands.py` & `dock-cli-0.4.0/dock_cli/utils/commands.py`

 * *Files identical despite different names*

### Comparing `dock-cli-0.3.1/dock_cli/utils/helpers.py` & `dock-cli-0.4.0/dock_cli/utils/helpers.py`

 * *Files 22% similar despite different names*

```diff
@@ -32,40 +32,50 @@
         self.config = config
         self.config_dir = config_dir
         self.command = command
 
     def get_section_path(self, section):
         return self.config_dir / pathlib.Path(section)
 
-    @functools.lru_cache()
-    def is_updated_section(self, section, commit1, commit2):
-        return cmd.getoutput([self.command.git, 'diff', commit1, commit2, '--', self.get_section_path(section)]) != ''
+    def validate_section(self, section):
+        assert section in self.config, (
+               f"The section '{section}' is not in the configuration.")
+        assert not pathlib.Path(section).is_absolute(), (
+               f"The section '{section}' should be a relative path.")
 
     def is_valid_section(self, section):
-        return section in self.config and not pathlib.Path(section).is_absolute()
+        try:
+            self.validate_section(section)
+        except AssertionError:
+            return False
+        return True
 
-    def validate_section(self, section):
-        assert self.is_valid_section(section), f"Expected the section '{section}' is valid."
+    @functools.lru_cache()
+    def is_updated_section(self, section, commit1, commit2):
+        return cmd.getoutput([self.command.git, 'diff', commit1, commit2, '--', self.get_section_path(section)]) != ''
 
 
 class ChartHelper(ConfigHelper):
     def get_section_file(self, section):
         return self.get_section_path(section) / 'Chart.yaml'
 
     def get_section_type(self, section):
         return self.config.get(section, Chart.TYPE, fallback='')
 
     def get_section_registry(self, section):
         return self.config.get(section, Chart.REGISTRY, fallback='')
 
-    def is_valid_section(self, section):
-        return all([super().is_valid_section(section),
-                    self.get_section_file(section).exists(),
-                    self.get_section_type(section) == SectionType.CHART,
-                    self.get_section_registry(section)])
+    def validate_section(self, section):
+        super().validate_section(section)
+        assert self.get_section_file(section).exists(), (
+               f"File does not exist: {self.get_section_file(section)}.")
+        assert self.get_section_type(section) == SectionType.CHART, (
+               f"The section '{section}' type should be {SectionType.CHART}.")
+        assert self.get_section_registry(section), (
+               f"The section '{section}' registry should exist.")
 
     def get_chart_info(self, section):
         return cmd.getoutput([self.command.helm, 'show', 'chart', self.get_section_path(section)])
 
     def get_chart_name(self, section):
         return re.search(r'^name:\s*(\S+)', self.get_chart_info(section), flags=re.MULTILINE).group(1)
 
@@ -97,19 +107,22 @@
 
     def get_section_dependencies(self, section):
         return self.config.get(section, Image.DEPENDS_ON, fallback='').strip().splitlines()
 
     def get_section_registry(self, section):
         return self.config.get(section, Image.REGISTRY, fallback='')
 
-    def is_valid_section(self, section):
-        return all([super().is_valid_section(section),
-                    self.get_section_file(section).exists(),
-                    self.get_section_type(section) == SectionType.IMAGE,
-                    self.get_section_registry(section)])
+    def validate_section(self, section):
+        super().validate_section(section)
+        assert self.get_section_file(section).exists(), (
+               f"File does not exist: {self.get_section_file(section)}.")
+        assert self.get_section_type(section) == SectionType.IMAGE, (
+               f"The section '{section}' type should be {SectionType.IMAGE}.")
+        assert self.get_section_registry(section), (
+               f"The section '{section}' registry should exist.")
 
     def get_image(self, section, image_tag):
         return f'{self.get_section_registry(section)}/{self.get_section_name(section)}:{image_tag}'
 
     def get_images(self):
         return topological_sort({section: set(self.get_section_dependencies(section))
                                  for section in self.config.sections() if self.is_valid_section(section)})
```

### Comparing `dock-cli-0.3.1/dock_cli/utils/schema.py` & `dock-cli-0.4.0/dock_cli/utils/schema.py`

 * *Files identical despite different names*

### Comparing `dock-cli-0.3.1/dock_cli/utils/utils.py` & `dock-cli-0.4.0/dock_cli/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dock-cli-0.3.1/dock_cli.egg-info/PKG-INFO` & `dock-cli-0.4.0/dock_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dock-cli
-Version: 0.3.1
+Version: 0.4.0
 Summary: CLI for manage container applications
 Author: Posen
 Author-email: posen2101024@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click==8.1.7
```

### Comparing `dock-cli-0.3.1/setup.py` & `dock-cli-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(
     name='dock-cli',
-    version='0.3.1',
+    version='0.4.0',
     author='Posen',
     author_email='posen2101024@gmail.com',
     description='CLI for manage container applications',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     include_package_data=True,
```

