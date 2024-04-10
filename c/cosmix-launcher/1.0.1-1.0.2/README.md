# Comparing `tmp/cosmix_launcher-1.0.1.tar.gz` & `tmp/cosmix_launcher-1.0.2.tar.gz`

## Comparing `cosmix_launcher-1.0.1.tar` & `cosmix_launcher-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.1/license.txt
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.1/requirements.txt
--rwxr-xr-x   0        0        0      130 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.1/scripts/publish.sh
--rwxr-xr-x   0        0        0      343 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.1/scripts/test.sh
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.1/src/cosmix/__main__.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.1/src/cosmix/api/__init__.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.1/src/cosmix/api/config.py
--rw-r--r--   0        0        0     5332 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.1/src/cosmix/api/instance.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.1/src/cosmix/api/logger.py
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.1/src/cosmix/api/maven.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.1/src/cosmix/api/mod.py
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.1/src/cosmix/api/net.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.1/src/cosmix/api/paths.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.1/src/cosmix/api/versions.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.1/.gitignore
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.1/readme.md
--rw-r--r--   0        0        0     3770 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.2/cosmix.bat
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.2/license.txt
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.2/requirements.txt
+-rwxr-xr-x   0        0        0      130 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.2/scripts/publish.sh
+-rwxr-xr-x   0        0        0      343 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.2/scripts/test.sh
+-rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.2/src/cosmix/__main__.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.2/src/cosmix/api/__init__.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.2/src/cosmix/api/config.py
+-rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.2/src/cosmix/api/instance.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.2/src/cosmix/api/logger.py
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.2/src/cosmix/api/maven.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.2/src/cosmix/api/mod.py
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.2/src/cosmix/api/net.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.2/src/cosmix/api/paths.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.2/src/cosmix/api/versions.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.2/.gitignore
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.2/readme.md
+-rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.2/PKG-INFO
```

### Comparing `cosmix_launcher-1.0.1/license.txt` & `cosmix_launcher-1.0.2/license.txt`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.1/src/cosmix/__main__.py` & `cosmix_launcher-1.0.2/src/cosmix/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,16 +41,15 @@
 @click.option("--quilt-version", "-q", default="none", type=str, help="The Cosmic Quilt version to use.")
 @click.option("--display-name", "-n", default=None, type=str, help="An optional display name to use for the instance.")
 @click.argument("name")
 def add(version: str, quilt_version: str, display_name: Optional[str], name: str):
     if Instance.exists(name):
         logger.error("Instance already exists.")
         exit(1)
-    instance = Instance.make_instance(name, version, None if quilt_version == "none" else quilt_version)
-    instance.display_name = display_name
+    instance = Instance.make_instance(name, version, None if quilt_version == "none" else quilt_version, display_name)
     instance.download()
     logger.info("Made instance " + name)
 
 
 @cosmix.command()
 @click.option("--version", "-v", default="none", type=str, help="The version of Cosmic Reach to update to. Defaults to 'none'")
 @click.option("--quilt-version", "-q", default="none", type=str, help="The Cosmic Quilt version to update to. Defaults to 'none'")
@@ -80,17 +79,20 @@
 def instances():
     if not os.path.exists(paths.INSTANCES) or len(os.listdir(paths.INSTANCES)) <= 0:
         logger.error("No instances found.")
         exit(0)
 
     for instance_name in os.listdir(paths.INSTANCES):
         instance = Instance.get_or_throw(instance_name)
-        s = f" - {instance.display_name} ({instance.version})"
+        s = f" - \u001b[1m{instance.display_name}\u001b[0m"
+        if instance.display_name != instance.name:
+            s += f" ({instance.name})"
+        s += f" \u001b[33m(Version: {instance.version})\u001b[0m"
         if instance.quilt_version is not None:
-            s += f" (Quilt: {instance.quilt_version})"
+            s += f" \u001b[34m(Quilt: {instance.quilt_version})\u001b[0m"
         print(s)
 
 
 @cosmix.command()
 @click.argument("name")
 def trash(name: str):
     instance = Instance.get_or_throw(name)
@@ -119,29 +121,29 @@
 @click.argument("mod", type=click.Path(exists = True))
 def add_mod(name: str, mod):
     i = Instance.get_or_throw(name)
     if not i.is_modded():
         logger.error("Instance is not modded")
         exit(1)
 
-    path = os.path.join(i.path, "mods/")
+    path = os.path.join(i.path, "mods")
     os.makedirs(path, exist_ok = True)
-    shutil.copyfile(mod, os.path.join(path, mod.split("/")[-1]))
+    shutil.copyfile(mod, os.path.join(path, os.path.split(mod)[-1]))
 
 
 @cosmix.command("add-crm1-mod")
 @click.argument("name")
 @click.argument("mod")
 def add_crm1_mod(name: str, mod: str):
     i = Instance.get_or_throw(name)
 
     if not i.is_modded():
         logger.error("Instance is not modded")
         exit(1)
 
-    path = os.path.join(i.path, "mods/")
+    path = os.path.join(i.path, "mods")
     os.makedirs(path, exist_ok = True)
     net.download_crm1_mod(mod, path)
 
 
 if __name__ == "__main__":
     cosmix()
```

### Comparing `cosmix_launcher-1.0.1/src/cosmix/api/config.py` & `cosmix_launcher-1.0.2/src/cosmix/api/config.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.1/src/cosmix/api/instance.py` & `cosmix_launcher-1.0.2/src/cosmix/api/instance.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         if not os.path.isfile(cr_path):
             net.download(f"{COSMIC_ARCHIVE_RAW_URL}/Cosmic Reach-{self.version}.jar", cr_path)
 
         if self.is_modded():
             logger.info("Downloading Cosmic Quilt dependencies...")
 
             pom = self.path_to("pom.xml")
-            deps = self.path_to("deps/")
+            deps = self.path_to("deps")
             had_existing_pom = True
             if not os.path.isfile(pom):
                 maven.make_pom(pom, self.quilt_version)
                 had_existing_pom = False
             if is_updating and os.path.exists(deps):
                 shutil.rmtree(deps)
             maven.copy_deps(self.path, deps)
@@ -91,15 +91,15 @@
     def save(self):
         os.makedirs(self.path, exist_ok = True)
         with open(self.path_to("config.hjson"), "w") as f:
             hjson.dump(Instance.get_hjson(self), f)
 
     def get_mods(self) -> list[str]:
         mods = []
-        mods_dir = self.path_to("mods/")
+        mods_dir = self.path_to("mods")
         if os.path.exists(mods_dir):
             for mod_file in os.listdir(mods_dir):
                 manifest = java_manifest.from_jar(os.path.join(mods_dir, mod_file))
                 mods.append(mod.Mod.from_data(manifest, mod_file))
         return mods
 
     # Static Methods
@@ -118,26 +118,26 @@
             ins.quilt_version = data["quilt-version"]
         if "display-name" in data:
             ins.display_name = data["display-name"]
 
         return ins
 
     @staticmethod
-    def make_instance(instance_name: str, cosmic_reach_version: str, quilt_version: Optional[str] = None) -> "Instance":
+    def make_instance(instance_name: str, cosmic_reach_version: str, quilt_version: Optional[str] = None, display_name: Optional[str] = None) -> "Instance":
         if not VALID_INSTANCE_NAME.match(instance_name):
             logger.error("Instance name must match `[a-zA-Z0-9_-]*`")
             exit(1)
 
         cosmic_reach_version = versions.get_version_or_latest_of("reach", cosmic_reach_version)
         quilt_version = versions.get_version_or_latest_of("quilt", quilt_version)
 
-        path = paths.INSTANCES + instance_name
+        path = os.path.join(paths.INSTANCES, instance_name)
         os.makedirs(path, exist_ok = True)
 
-        instance = Instance(instance_name, cosmic_reach_version, [], quilt_version)
+        instance = Instance(instance_name, cosmic_reach_version, [], quilt_version, display_name)
         instance.save()
         return instance
 
     @staticmethod
     def get_hjson(instance: "Instance") -> dict:
         d = {
             "name": instance.name,
```

### Comparing `cosmix_launcher-1.0.1/src/cosmix/api/logger.py` & `cosmix_launcher-1.0.2/src/cosmix/api/logger.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.1/src/cosmix/api/maven.py` & `cosmix_launcher-1.0.2/src/cosmix/api/maven.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.1/src/cosmix/api/mod.py` & `cosmix_launcher-1.0.2/src/cosmix/api/mod.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.1/src/cosmix/api/net.py` & `cosmix_launcher-1.0.2/src/cosmix/api/net.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 def download(url: str, dest: str):
     stream = requests.get(url, stream = True)
     size = int(stream.headers.get("content-length", 0))
 
     logger.debug("Downloading: " + url)
 
     with tqdm.tqdm(total = size, unit = "B", unit_scale = True) as bar:
-        folder = dest.removesuffix("/" + dest.split("/")[-1])
+        folder = os.path.dirname(dest)
         if not os.path.exists(folder):
-            os.makedirs(folder, exist_ok=True)
+            os.makedirs(folder, exist_ok = True)
 
         with open(dest, "wb") as file:
             for data in stream.iter_content(BLOCK_SIZE):
                 bar.update(len(data))
                 file.write(data)
 
     if size != 0 and bar.n != size:
@@ -62,8 +62,8 @@
         logger.error(f"Failed to find mod '{mod}' in repo '{repo}'")
         return
 
     download(mod.meta.url, os.path.join(dest_folder, mod.id + ".jar"))
 
     for dep_data in mod.depends:
         dep = dep_data.resolve(pool)
-        download(dep.meta.url, dest)
+        download(dep.meta.url, os.path.join(dest_folder, dep.id + ".jar"))
```

### Comparing `cosmix_launcher-1.0.1/src/cosmix/api/versions.py` & `cosmix_launcher-1.0.2/src/cosmix/api/versions.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.1/readme.md` & `cosmix_launcher-1.0.2/readme.md`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 ```
 
 I recommend making an alias to `python3 -m cosmix`. In Zsh you can do this by adding the following to your `.zshrc`:
 ```zsh
 alias cosmix="python3 -m cosmix"
 ```
 
+On windows download the cosmix.bat file and put it in ```C:\Windows\System32```
+
 **Arch Linux:**
 > Arch Linux and it's derivatives may complain with this `error: externally-managed-environment`
 >
 > To get around this, use the `--user --break-system-packages` options with `pip install`
 >
 > Obviously this has a chance of breaking something, but in my testing I have yet to have that happen. Though be aware and know that I am not responsible if you break your system.
 
@@ -42,14 +44,15 @@
     prints a lot of debug information related to cosmix
 
 cosmix add [instance]
     adds and downloads a new instance
     options:
     --version -v VERSION        specify a Cosmic Reach version to use. defaults to "latest"
     --quilt-version -q VERSION  specify a Cosmic Quilt version to use. defaults to "none"
+    --display-name -n NAME      optionally specify a display name for the instance
 
 cosmix update [instance]
     updates an existing version
     options:
     --version -v VERSION        specify a Cosimc Reach version to use. defaults to "latest"
     --quilt-version -q VERSION  specify a Cosmic Quilt version to use. defaults to "none"
 
@@ -84,15 +87,15 @@
     cosmix add-crm1-mod test dev.crmodders.flux
 # Update the `latest` instance to the latest available versions of Cosmic Reach and Cosmic Quilt
     cosmix update latest -v latest -q latest
 ```
 
 ## Folder Structure
 
-Cosmix stores all of its data in your `XDG_DATA_HOME` (typically `~/.local/share/`) on Linux and `APPDATA` on Windows and in the `cosmix` folder.
+Cosmix stores all of its data in your `XDG_DATA_HOME` (typically `~/.local/share/`) on Linux and `%appdata%` on Windows and in the `cosmix` folder.
 
 This folder will contain the following extra folders:
 ```
 cosmix/
     deps/
         cosmic-reach/
             Contains JARs for each downloaded Cosmic Reach version.
```

### Comparing `cosmix_launcher-1.0.1/PKG-INFO` & `cosmix_launcher-1.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 Metadata-Version: 2.3
 Name: cosmix-launcher
-Version: 1.0.1
+Version: 1.0.2
 Summary: A dead simple CLI-based launcher for Cosmic Reach and Cosmic Quilt
 Project-URL: Homepage, https://codeberg.org/EmmaTheMartian/cosmix
 Project-URL: Issues, https://codeberg.org/EmmaTheMartian/cosmix/issues
 Author-email: EmmaTheMartian <emmathemartian@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
+Requires-Dist: click
+Requires-Dist: crm1
+Requires-Dist: hjson
+Requires-Dist: java-manifest
+Requires-Dist: requests
+Requires-Dist: send2trash
+Requires-Dist: tqdm
 Description-Content-Type: text/markdown
 
 # Cosmix
 
 A dead simple CLI-based launcher for Cosmic Reach and Cosmic Quilt.
 
 ## Installation
@@ -31,14 +38,16 @@
 ```
 
 I recommend making an alias to `python3 -m cosmix`. In Zsh you can do this by adding the following to your `.zshrc`:
 ```zsh
 alias cosmix="python3 -m cosmix"
 ```
 
+On windows download the cosmix.bat file and put it in ```C:\Windows\System32```
+
 **Arch Linux:**
 > Arch Linux and it's derivatives may complain with this `error: externally-managed-environment`
 >
 > To get around this, use the `--user --break-system-packages` options with `pip install`
 >
 > Obviously this has a chance of breaking something, but in my testing I have yet to have that happen. Though be aware and know that I am not responsible if you break your system.
 
@@ -54,14 +63,15 @@
     prints a lot of debug information related to cosmix
 
 cosmix add [instance]
     adds and downloads a new instance
     options:
     --version -v VERSION        specify a Cosmic Reach version to use. defaults to "latest"
     --quilt-version -q VERSION  specify a Cosmic Quilt version to use. defaults to "none"
+    --display-name -n NAME      optionally specify a display name for the instance
 
 cosmix update [instance]
     updates an existing version
     options:
     --version -v VERSION        specify a Cosimc Reach version to use. defaults to "latest"
     --quilt-version -q VERSION  specify a Cosmic Quilt version to use. defaults to "none"
 
@@ -96,15 +106,15 @@
     cosmix add-crm1-mod test dev.crmodders.flux
 # Update the `latest` instance to the latest available versions of Cosmic Reach and Cosmic Quilt
     cosmix update latest -v latest -q latest
 ```
 
 ## Folder Structure
 
-Cosmix stores all of its data in your `XDG_DATA_HOME` (typically `~/.local/share/`) on Linux and `APPDATA` on Windows and in the `cosmix` folder.
+Cosmix stores all of its data in your `XDG_DATA_HOME` (typically `~/.local/share/`) on Linux and `%appdata%` on Windows and in the `cosmix` folder.
 
 This folder will contain the following extra folders:
 ```
 cosmix/
     deps/
         cosmic-reach/
             Contains JARs for each downloaded Cosmic Reach version.
```

