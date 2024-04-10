# Comparing `tmp/ctf_architect-0.1.0a4.tar.gz` & `tmp/ctf_architect-0.1.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctf_architect-0.1.0a4.tar", max compression
+gzip compressed data, was "ctf_architect-0.1.0a5.tar", max compression
```

## Comparing `ctf_architect-0.1.0a4.tar` & `ctf_architect-0.1.0a5.tar`

### file list

```diff
@@ -1,20 +1,26 @@
--rw-r--r--   0        0        0     1066 2023-10-05 12:51:36.027026 ctf_architect-0.1.0a4/LICENSE
--rw-r--r--   0        0        0     1853 2023-10-05 12:51:36.027026 ctf_architect-0.1.0a4/README.md
--rw-r--r--   0        0        0      160 2023-10-05 12:51:36.027026 ctf_architect-0.1.0a4/ctf_architect/__init__.py
--rw-r--r--   0        0        0      153 2023-10-05 12:51:36.027026 ctf_architect-0.1.0a4/ctf_architect/__main__.py
--rw-r--r--   0        0        0      120 2023-10-05 12:51:36.027026 ctf_architect-0.1.0a4/ctf_architect/chall_architect/__main__.py
--rw-r--r--   0        0        0    13417 2023-10-05 12:51:36.027026 ctf_architect-0.1.0a4/ctf_architect/chall_architect/cli.py
--rw-r--r--   0        0        0     5613 2023-10-05 12:51:36.027026 ctf_architect-0.1.0a4/ctf_architect/chall_architect/create.py
--rw-r--r--   0        0        0     1195 2023-10-05 12:51:36.027026 ctf_architect-0.1.0a4/ctf_architect/chall_architect/utils.py
--rw-r--r--   0        0        0     4220 2023-10-05 12:51:36.027026 ctf_architect-0.1.0a4/ctf_architect/cli/__init__.py
--rw-r--r--   0        0        0     6332 2023-10-05 12:51:36.027026 ctf_architect-0.1.0a4/ctf_architect/cli/challenge.py
--rw-r--r--   0        0        0     3501 2023-10-05 12:51:36.027026 ctf_architect-0.1.0a4/ctf_architect/cli/stats.py
--rw-r--r--   0        0        0     4575 2023-10-05 12:51:36.027026 ctf_architect-0.1.0a4/ctf_architect/core/challenge.py
--rw-r--r--   0        0        0      614 2023-10-05 12:51:36.027026 ctf_architect-0.1.0a4/ctf_architect/core/config.py
--rw-r--r--   0        0        0       30 2023-10-05 12:51:36.027026 ctf_architect-0.1.0a4/ctf_architect/core/constants.py
--rw-r--r--   0        0        0     1395 2023-10-05 12:51:36.027026 ctf_architect-0.1.0a4/ctf_architect/core/initialize.py
--rw-r--r--   0        0        0     2510 2023-10-05 12:51:36.027026 ctf_architect-0.1.0a4/ctf_architect/core/models.py
--rw-r--r--   0        0        0     5373 2023-10-05 12:51:36.027026 ctf_architect-0.1.0a4/ctf_architect/core/stats.py
--rw-r--r--   0        0        0      999 2023-10-05 12:51:36.027026 ctf_architect-0.1.0a4/ctf_architect/core/unzip.py
--rw-r--r--   0        0        0      833 2023-10-05 12:51:36.027026 ctf_architect-0.1.0a4/pyproject.toml
--rw-r--r--   0        0        0     2667 1970-01-01 00:00:00.000000 ctf_architect-0.1.0a4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-10 11:20:14.658512 ctf_architect-0.1.0a5/LICENSE
+-rw-r--r--   0        0        0     1134 2024-04-10 11:20:14.658512 ctf_architect-0.1.0a5/README.md
+-rw-r--r--   0        0        0      330 2024-04-10 11:20:14.658512 ctf_architect-0.1.0a5/ctf_architect/__init__.py
+-rw-r--r--   0        0        0      153 2024-04-10 11:20:14.658512 ctf_architect-0.1.0a5/ctf_architect/__main__.py
+-rw-r--r--   0        0        0      120 2024-04-10 11:20:14.658512 ctf_architect-0.1.0a5/ctf_architect/chall_architect/__main__.py
+-rw-r--r--   0        0        0      265 2024-04-10 11:20:14.658512 ctf_architect-0.1.0a5/ctf_architect/chall_architect/cli.py
+-rw-r--r--   0        0        0     4388 2024-04-10 11:20:14.658512 ctf_architect-0.1.0a5/ctf_architect/chall_architect/create.py
+-rw-r--r--   0        0        0     5468 2024-04-10 11:20:14.658512 ctf_architect-0.1.0a5/ctf_architect/chall_architect/edit.py
+-rw-r--r--   0        0        0    15972 2024-04-10 11:20:14.658512 ctf_architect-0.1.0a5/ctf_architect/chall_architect/terminal/create.py
+-rw-r--r--   0        0        0      743 2024-04-10 11:20:14.658512 ctf_architect-0.1.0a5/ctf_architect/chall_architect/terminal/main.py
+-rw-r--r--   0        0        0     1353 2024-04-10 11:20:14.658512 ctf_architect-0.1.0a5/ctf_architect/chall_architect/utils.py
+-rw-r--r--   0        0        0     5583 2024-04-10 11:20:14.658512 ctf_architect-0.1.0a5/ctf_architect/cli/__init__.py
+-rw-r--r--   0        0        0     7610 2024-04-10 11:20:14.658512 ctf_architect-0.1.0a5/ctf_architect/cli/challenge.py
+-rw-r--r--   0        0        0     1272 2024-04-10 11:20:14.658512 ctf_architect-0.1.0a5/ctf_architect/cli/docker.py
+-rw-r--r--   0        0        0     2135 2024-04-10 11:20:14.662512 ctf_architect-0.1.0a5/ctf_architect/cli/mapping.py
+-rw-r--r--   0        0        0     4172 2024-04-10 11:20:14.662512 ctf_architect-0.1.0a5/ctf_architect/cli/stats.py
+-rw-r--r--   0        0        0     8169 2024-04-10 11:20:14.662512 ctf_architect-0.1.0a5/ctf_architect/core/challenge.py
+-rw-r--r--   0        0        0     1196 2024-04-10 11:20:14.662512 ctf_architect-0.1.0a5/ctf_architect/core/config.py
+-rw-r--r--   0        0        0     1203 2024-04-10 11:20:14.662512 ctf_architect-0.1.0a5/ctf_architect/core/constants.py
+-rw-r--r--   0        0        0     2234 2024-04-10 11:20:14.662512 ctf_architect-0.1.0a5/ctf_architect/core/docker.py
+-rw-r--r--   0        0        0     1644 2024-04-10 11:20:14.662512 ctf_architect-0.1.0a5/ctf_architect/core/initialize.py
+-rw-r--r--   0        0        0     2788 2024-04-10 11:20:14.662512 ctf_architect-0.1.0a5/ctf_architect/core/mapping.py
+-rw-r--r--   0        0        0     6532 2024-04-10 11:20:14.662512 ctf_architect-0.1.0a5/ctf_architect/core/models.py
+-rw-r--r--   0        0        0     6095 2024-04-10 11:20:14.662512 ctf_architect-0.1.0a5/ctf_architect/core/stats.py
+-rw-r--r--   0        0        0     1058 2024-04-10 11:20:14.662512 ctf_architect-0.1.0a5/pyproject.toml
+-rw-r--r--   0        0        0     2121 1970-01-01 00:00:00.000000 ctf_architect-0.1.0a5/PKG-INFO
```

### Comparing `ctf_architect-0.1.0a4/LICENSE` & `ctf_architect-0.1.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `ctf_architect-0.1.0a4/ctf_architect/cli/__init__.py` & `ctf_architect-0.1.0a5/ctf_architect/cli/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,130 +4,163 @@
 
 import typer
 from rich.console import Console
 from rich.panel import Panel
 from rich.prompt import Confirm, IntPrompt, Prompt
 
 from ctf_architect.cli.challenge import challenge_app
+from ctf_architect.cli.docker import docker_app
+from ctf_architect.cli.mapping import mapping_app
 from ctf_architect.cli.stats import stats_app
+from ctf_architect.core.constants import CTF_CONFIG_FILE
 from ctf_architect.core.initialize import init_no_config, init_with_config
 
 console = Console()
 
 
 app = typer.Typer()
 app.add_typer(challenge_app, name="challenge")
+app.add_typer(docker_app, name="docker")
+app.add_typer(mapping_app, name="mapping")
 app.add_typer(stats_app, name="stats")
 
 
 @app.command()
 def init(
-  port: int = typer.Option(8000, "--port", "-p", help="Specify the port."),
+  starting_port: int = typer.Option(None, "--starting-port", "-p", help="The starting port for the CTF Services"),
   config_only: bool = typer.Option(False, "--config-only", "-c", help="Only create the config file.")
 ):
   """
-  Initialize a new CTF repo.
+  Initialize a new CTF repository.
   """
 
-  if config_only and Path("ctf_config.yaml").exists():
-    console.print("[bright_red]ctf_config.yaml already exists.[/bright_red]")
-    return
-  
-  # Check if there is a ctf_config.yaml in the current directory, if so, use that config
-  # Otherwise, use the config specified in the command line arguments
-  if Path("ctf_config.yaml").exists():
+  # Check if the config file already exists
+  if Path(CTF_CONFIG_FILE).exists():
+    if config_only:
+      console.print("A config file already exists. Exiting...", style="bright_red")
+
+    if not Confirm.ask("[cyan]A config file already exists. Do you want to use this config?[/]"):
+      console.print("Aborting...", style="bright_red")
+      return
+
     try:
       init_with_config()
     except ValueError as e:
-      console.print(f"[bright_red]{e}[/bright_red]")
+      console.print(f"Error initializing the CTF repo: {e}", style="bright_red")
       return
     else:
-      console.print("[bright_green]Initialized CTF repo with the config in ctf_config.yaml.[/bright_green]")
-  
+      console.print("CTF repo initialized successfully!", style="bright_green")
+
   else:
+    ctf_name = None
+    while not ctf_name:
+      ctf_name = Prompt.ask("[cyan]Enter the name of the CTF[/]")
+    
+    if starting_port is None:
+      starting_port = IntPrompt.ask("[cyan]Starting port for the CTF Services[/]", default=8000)
 
-    # Get the categories and difficulties from the user
+    # Get the categories, difficulties and extras from the user
     categories = []
     difficulties = []
+    extras = []
 
     try:
-      console.rule("[bold yellow]CTF Categories[/]")
+      console.rule("[bright_yellow]CTF Categories[/bright_yellow]")
 
-      console.print("[bold cyan]Please enter the categories for your CTF. Enter an empty string to stop.[/]")
+      console.print("Enter the categories for the CTF (one per line, empty line to stop).", style="bright_cyan")
 
       while True:
         category = Prompt.ask("[cyan]Category name[/]", default="", show_default=False)
         if category == "":
           break
         categories.append(category.lower())
 
-        console.print(f"\n[green]Category {category} added.[/]\n")
+        console.print(f"Category {category} added.\n", style="green")
 
       if len(categories) == 0:
-        console.print("[bright_red]Please specify at least one category.[/bright_red]")
+        console.print("No categories specified. Exiting...", style="bright_red")
         return
       else:
-        console.print(f"\n[bold green]Categories:[/]")
+        console.print("Categories:", style="bright_green")
         for category in categories:
-          console.print(f"[green] - {category}[/]")
+          console.print(f"  - {category}", style="green")
 
 
-      console.rule("[bold yellow]CTF Difficulties[/]")
+      console.rule("[bright_yellow]CTF Difficulties[/bright_yellow]")
 
-      console.print("\n[bold cyan]Please enter the difficulties for your CTF. Enter an empty string to stop.[/]")
+      console.print("Enter the difficulties for the CTF (empty name to stop).", style="bright_cyan")
 
       while True:
         name = Prompt.ask("[cyan]Difficulty name[/]", default="", show_default=False)
         if name == "":
           break
         value = IntPrompt.ask("[cyan]Difficulty value[/]", default=500)
-        difficulties.append({
-          "name": name.lower(),
-          "value": value
-        })
+        difficulties.append({"name": name.lower(), "value": value})
 
-        console.print(f"\n[green]Difficulty {name} added. ({value} points)[/]\n")
+        console.print(f"Difficulty {name} added. ({value} points)\n", style="green")
 
       if len(difficulties) == 0:
-        console.print("[bright_red]Please specify at least one difficulty.[/bright_red]")
+        console.print("No difficulties specified. Exiting...", style="bright_red")
         return
       else:
-        console.print(f"\n[bold green]Difficulties:[/]")
+        console.print("Difficulties:", style="bright_green")
         for difficulty in difficulties:
-          console.print(f"[green] - {difficulty['name']} ({difficulty['value']} points)[/]")
+          console.print(f"  - {difficulty['name']} ({difficulty['value']} points)", style="green")
+
+      
+      console.rule("[bright_yellow]Extra Fields[/bright_yellow]")
+
+      console.print("Enter any extra fields challenges should specify (one per line, empty line to stop).", style="bright_cyan")
+
+      while True:
+        extra = Prompt.ask("[cyan]Extra field[/]", default="", show_default=False)
+        if extra == "":
+          break
+        extras.append(extra)
+
+        console.print(f"Extra field {extra} added.\n", style="green")
     except (KeyboardInterrupt, EOFError):
-      console.print("\n[bright_red]Aborting...[/bright_red]")
+      console.print("\nAborting...", style="bright_red")
       return
 
-
-    # Show panel of categories and difficulties
+    # Show panel of current configuration and ask for confirmation
     # If the user confirms, initialize the CTF repo
-    
-    config_text = ""
-    config_text += "[bold cyan]Categories:[/]\n"
+
+    config_text = "[bright_cyan]Categories:[/]\n"
     for category in categories:
-      config_text += f"[cyan] - {category}[/]\n"
-    config_text += "\n"
-    config_text += "[bold cyan]Difficulties:[/]\n"
+      config_text += f"[cyan]  - {category}[/]\n"
+    config_text += "\n[bright_cyan]Difficulties:[/]\n"
     for difficulty in difficulties:
-      config_text += f"[cyan] - {difficulty['name']} ({difficulty['value']} points)[/]\n"
+      config_text += f"[cyan]  - {difficulty['name']} ({difficulty['value']} points)[/]\n"
+    config_text += "\n[bright_cyan]Extras:[/]\n"
+    for extra in extras:
+      config_text += f"[cyan]  - {extra}[/]\n"
+
+    config_text += f"\n[bright_cyan]Starting Port:[/]\n[cyan]  - {starting_port}[/]"
 
     console.print(
       Panel(
         config_text,
-        title="[bright_yellow]CTF Config[/bright_yellow]",
+        title=f"[bright_yellow]{ctf_name} Configuration[/bright_yellow]",
         border_style="green"
       )
     )
 
-    if not Confirm.ask("[cyan]Is this correct?[/]"):
-      console.print("[bright_red]Aborting...[/bright_red]")
+    if not Confirm.ask("[cyan]Is this configuration correct?[/]"):
+      console.print("Aborting...", style="bright_red")
       return
-
     
+
     try:
-      init_no_config(categories, difficulties, port, config_only)
+      init_no_config(
+        name=ctf_name,
+        categories=categories,
+        difficulties=difficulties,
+        starting_port=starting_port,
+        extras=extras,
+        config_only=config_only
+      )
     except ValueError as e:
-      console.print(f"[bright_red]{e}[/bright_red]")
+      console.print(f"Error initializing the CTF repo:\n{e}", style="bright_red")
       return
     else:
-      console.print("[bright_green]Initialized CTF repo with specified config.[/bright_green]")
+      console.print("CTF repo initialized successfully.", style="bright_green")
```

### Comparing `ctf_architect-0.1.0a4/ctf_architect/cli/challenge.py` & `ctf_architect-0.1.0a5/ctf_architect/cli/challenge.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,193 +1,244 @@
 from __future__ import annotations
 
-from pathlib import Path
 import shutil
+from collections import deque
+from pathlib import Path
+from zipfile import ZipFile
 
 import typer
-from rich import print
+from rich.console import Console
 from rich.panel import Panel
+from rich.prompt import Confirm, Prompt
 
-from ctf_architect.core.challenge import add_challenge, find_challenge
+from ctf_architect.core.challenge import (add_challenge, find_challenge,
+                                          is_challenge_folder,
+                                          is_challenge_repo,
+                                          verify_challenge_config,
+                                          walk_challenges)
 from ctf_architect.core.config import load_config
-from ctf_architect.core.constants import APP_CMD_NAME
-from ctf_architect.core.stats import (update_category_readme,
-                         update_root_readme)
-from ctf_architect.core.unzip import unzip
-
+from ctf_architect.core.constants import APP_CMD_NAME, CTF_CONFIG_FILE
+from ctf_architect.core.stats import update_category_readme, update_root_readme
 
-def is_challenge_repo() -> bool:
-  """
-  Checks if the current working directory is a challenge repo.
-
-  A challenge repo is considered valid if it has a ctf_config.yaml and a challenges folder.
-  """
-  return Path("ctf_config.yaml").exists() and Path("challenges").exists()
+console = Console()
 
 
 challenge_app = typer.Typer()
 
 
 @challenge_app.callback()
 def callback():
   """
-  Commands to manage challenges.
+  Commands to manage challenges in the CTF repo.
   """
 
 
 @challenge_app.command("import")
 def challenge_import(
-  path: str = typer.Option(default="./", help="Specify the path to the challenge zip files."),
+  path: str = typer.Option(default=".", help="Specify the path to ther challenge zip files."),
   delete_on_error: bool = typer.Option(False, "--delete-on-error", "-d", help="Delete the challenge folder if an error occurs."),
-  replace: bool = typer.Option(False, "--replace", "-r", help="Replace all existing challenges."),
-  update_stats: bool = typer.Option(True, "--update-stats", "-u", help="Update the stats after importing.")
+  replace: bool = typer.Option(False, "--replace", "-r", help="Replace the challenge if it already exists."),
+  update_stats: bool = typer.Option(True, "--update-stats", "-u", help="Update the stats after importing the challenge.")
 ):
   """
-  Imports challenges from zip files in the specified path.
+  Imports all challenges from the specified directory to the CTF repo.
   """
+
   try:
     config = load_config()
   except FileNotFoundError:
-    print(f"[bright_red]Challenge repo not found, are you in the correct directory? If so, please run `{APP_CMD_NAME} init` first.")
+    console.print("Could not find CTF config file. Are you in the right directory?", style="bright_red")
     return
-  
+
   zip_path = Path(path)
   extracted_path = Path("extracted")
 
   if not zip_path.exists():
-    print(f"[bright_red]Path `{zip_path}` does not exist.[/bright_red]")
+    console.print(f"Could not find the specified path: {zip_path}", style="bright_red")
+    return
+  
+  if not zip_path.is_dir():
+    console.print("The specified path must be a directory", style="bright_red")
     return
   
   success = 0
   unzip_failed = 0
-  add_failed = 0
+  import_failed = 0
 
   for zip_file in zip_path.glob("*.zip"):
+    new_path = extracted_path / zip_file.name.rsplit(".", 1)[0]
+
     try:
-      # Unzip the file
-      extracted = unzip(zip_file, extracted_path, delete=False)
+      # Extract the files to the "extracted" folder
+      with ZipFile(zip_file, "r") as zip_ref:
+        zip_ref.extractall(new_path)
     except Exception as e:
-      print(f"[bright_red]Failed to unzip challenge `{zip_file.name}`:[/bright_red]")
-      print(f"[bright_red]{e}[/bright_red]")
+      console.print(f"Error extracting {zip_file}:\n{e}", style="bright_red")
       unzip_failed += 1
       continue
-    
-    try:
-      # Add the challenge
-      add_challenge(extracted, replace=replace)
-    except FileExistsError:
-      # Prompt the user if they want to replace the challenge
-      print(f"[bright_red]Challenge `{extracted.name}` already exists.[/bright_red]")
-      if typer.confirm("Do you want to replace it?"):
-        add_challenge(extracted, replace=True)
-        print(f"[green]Successfully added challenge `{extracted.name}`[/green]")
-        success += 1
+
+    # Zipfile could contain multiple folders, recurse through every folder
+    # as deep as possible until there is a challenge config file
+    challenge_folders = []
+
+    queue = deque()
+    queue.append(new_path)
+    # BFS through the extracted folder
+    while queue:
+      current = queue.popleft()
+      if is_challenge_folder(current):
+        challenge_folders.append(current)
       else:
-        print(f"[bright_red]Skipping challenge `{extracted.name}`[/bright_red]")
-        add_failed += 1
-        continue
-    except Exception as e:
-      print(f"[bright_red]Failed to add challenge `{extracted.name}`:[/bright_red]")
-      print(f"[bright_red]{e}[/bright_red]")
-      # Delete the challenge folder if it exists
-      if extracted.exists() and delete_on_error:
-        shutil.rmtree(extracted)
-      add_failed += 1
+        for item in current.iterdir():
+          if item.is_dir():
+            queue.append(item)
+
+    if not challenge_folders:
+      console.print(f"No challenge folders found in {zip_file}, skipping...", style="yellow")
       continue
-    else:
-      print(f"[green]Successfully added challenge `{extracted.name}`[/green]")
-      success += 1
-
-  print(f"[green]Successfully imported {success} challenges[/green]")
-  if unzip_failed > 0:
-    print(f"[bright_red]Failed to unzip {unzip_failed} challenges[/bright_red]")
-  if add_failed > 0:
-    print(f"[bright_red]Failed to add {add_failed} challenges[/bright_red]")
 
-  # Update the stats
+    for extracted in challenge_folders:
+      try:
+        add_challenge(extracted, replace=replace)
+      except FileExistsError:
+        if Confirm.ask(f"[cyan]Challenge {extracted.name} already exists. Do you want to replace it?[/]"):
+          try:
+            add_challenge(extracted, replace=True)
+          except Exception as e:
+            console.print(f"Error importing {extracted.name}:\n{e}", style="bright_red")
+            # Delete the challenge folder if it exists
+            if extracted.exists() and delete_on_error:
+              shutil.rmtree(extracted)
+            import_failed += 1
+            continue
+          else:
+            console.print(f"Challenge \"{extracted.name}\" imported successfully.", style="green")
+            success += 1
+        else:
+          console.print(f"Skipping \"{extracted.name}\"", style="yellow")
+      except Exception as e:
+        console.print(f"Error importing {extracted.name}:\n{e}", style="bright_red")
+        # Delete the challenge folder if it exists
+        if extracted.exists() and delete_on_error:
+          shutil.rmtree(extracted)
+        import_failed += 1
+        continue
+      else:
+        console.print(f"Challenge \"{extracted.name}\" imported successfully.", style="green")
+        success += 1
+
   if update_stats and success > 0:
     for category in config.categories:
-      update_category_readme(category)
-    
+      update_category_readme(category) 
+
     update_root_readme()
 
-    print("[green]Repo READMEs updated successfully.")
+    console.print("Repo READMEs updated successfully.", style="green")
 
 
 @challenge_app.command("export")
 def challenge_export(
-  name: str = typer.Argument(..., help="The name of the challenge to export."),
-  path: str = typer.Option("./", "--path", "-p", help="Specify the path to export the challenge to."),
-  filename: str = typer.Option(None, "--filename", "-f", help="Specify the filename of the exported challenge."),
+  name: str = typer.Argument(..., help="Name of the challenge to export."),
+  path: str = typer.Option(".", "--path", "-p", help="Path to export the challenge to."),
+  filename: str = typer.Option(None, "--filename", "-f", help="Filename of the exported challenge."),
 ):
   """
   Exports the challenge as a zip file
-
-  NOTE: For some reason if a directory is created where the zip file is supposed to be, admin privileges are required to delete the directory.
   """
+
   if not is_challenge_repo():
-    print(f"[bright_red]Challenge repo not found, are you in the correct directory? If so, please run `{APP_CMD_NAME} init` first.")
+    console.print("Not a valid challenge repo. Exiting...", style="bright_red")
     return
   
   challenge = find_challenge(name)
 
   if challenge is None:
-    print(f"[bright_red]Challenge `{name}` not found.[/bright_red]")
+    console.print(f"Could not find challenge: {name}", style="bright_red")
     return
   
   challenge_path = challenge[1]
 
   if filename is None:
     filename = challenge_path.name
 
   path = Path(path) / filename
 
-  archive_path = shutil.make_archive(path, "zip", challenge_path)
+  zip_path = shutil.make_archive(path, "zip", challenge_path)
 
-  print(f"[green]Successfully exported challenge `{name}` to `{archive_path}`[/green]")
+  console.print(f"Challenge exported to {zip_path}", style="green")
 
 
 @challenge_app.command("info")
-def challenge_info(name: str = typer.Argument(..., help="The name of the challenge to get info for.")):
+def challenge_info(name: str = typer.Argument(..., help="Name of the challenge.")):
   """
-  Gets the info of a challenge.
+  Display information about a challenge
   """
-  try:
-    config = load_config()
-  except FileNotFoundError:
-    print(f"[bright_red]Challenge repo not found, are you in the correct directory? If so, please run `{APP_CMD_NAME} init` first.")
+
+  if not is_challenge_repo():
+    console.print("Not a valid challenge repo. Exiting...", style="bright_red")
     return
   
   challenge = find_challenge(name)
 
   if challenge is None:
-    print(f"[bright_red]Challenge `{name}` not found.[/bright_red]")
+    console.print(f"Could not find challenge: {name}", style="bright_red")
     return
   
-  challenge_info, challenge_path = challenge
+  config, path = challenge
 
   info = (
-    f"[bold]Name:[/] {challenge_info.name}\n"
-    f"[bold]Description:[/] {challenge_info.description.strip()}\n\n"
+    f"[bold]Name:[/] {config.name}\n"
+    f"[bold]Description:[/] {config.description.strip()}\n\n"
 
-    f"[bold]Difficulty:[/] {challenge_info.difficulty.capitalize()}\n"
-    f"[bold]Category:[/] {challenge_info.category.capitalize()}\n"
-    f"[bold]Author:[/] {challenge_info.author}\n"
-    f"[bold]Discord:[/] {challenge_info.discord}\n"
+    f"[bold]Difficulty:[/] {config.difficulty.capitalize()}\n"
+    f"[bold]Category:[/] {config.category.capitalize()}\n"
+    f"[bold]Author:[/] {config.author}\n"
   )
 
-  if challenge_info.services is not None:
-    info += "\n[bold]Services:[/]"
-    for service in challenge_info.services:
+  for extra in config.extras:
+    info += f"[bold]{extra.capitalize()}[/]: {config.extras[extra]}\n"
+
+  if config.services is not None:
+    info += "\n[bold]Services[/]:\n"
+    for service in config.services:
       info += (
         f"\n - [bold]Name:[/] {service.name}\n"
-        f" - [bold]Path:[/] {service.path}\n"
-        # f" - [bold]Path:[/] {(challenge_path / service.path).resolve()}\n"
+        # f" - [bold]Path:[/] {service.path}\n"
+        f" - [bold]Path:[/] {(path / service.path).resolve()}\n"
         f" - [bold]Port:[/] {service.port}\n"
+        f" - [bold]Type:[/] {service.type.capitalize()}\n"
       )
 
-  print(Panel.fit(
+  console.print(Panel.fit(
     info,
-    title=f"Challenge Info for {challenge_info.name}",
-    border_style="bright_cyan",
-    padding=(1, 2)
-  ))
+    title=f"Challenge Info for \"{config.name}\" ({path.resolve()})",
+    border_style="bright_cyan"
+  ))
+
+
+@challenge_app.command("verify")
+def challenge_verify():
+  """
+  Verify the challenges in the CTF repo
+  """
+
+  if not is_challenge_repo():
+    console.print("Not a valid challenge repo. Exiting...", style="bright_red")
+    return
+  
+  config = load_config()
+
+  total = 0
+  failed = 0
+
+  for chall in walk_challenges():
+    total += 1
+    try:
+      verify_challenge_config(chall, config)
+    except Exception as e:
+      console.print(f"Error verifying {chall.name}:\n{e}", style="bright_red")
+      failed += 1
+
+  if failed == 0:
+    console.print("All challenges verified successfully.", style="green")
+  else:
+    console.print(f"{failed}/{total} challenges failed verification.", style="bright_red")
```

### Comparing `ctf_architect-0.1.0a4/ctf_architect/cli/stats.py` & `ctf_architect-0.1.0a5/ctf_architect/cli/stats.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,110 +1,130 @@
 from __future__ import annotations
 
 import typer
-from rich import print
+from rich.console import Console
 from rich.table import Table
 
 from ctf_architect.core.config import load_config
 from ctf_architect.core.constants import APP_CMD_NAME
-from ctf_architect.core.stats import (get_category_diff_stats, update_category_readme,
-                         update_root_readme)
+from ctf_architect.core.challenge import walk_challenges
+from ctf_architect.core.stats import (get_category_difficulty_distribution,
+                                      update_category_readme,
+                                      update_challenge_readme,
+                                      update_root_readme)
+
+
+console = Console()
 
 
 stats_app = typer.Typer()
 
 
 @stats_app.callback()
 def callback():
   """
-  Commands to manage the stats of the challenge repo.
+  Commands to manage challenge statistics in the challenge repository
   """
 
 
 @stats_app.command("update")
-def stats_update():
+def stats_update(
+  update_challenges: bool = typer.Option(False, "--update-challenges", "-u", help="Update all challenge READMe.md's")
+):
   """
-  Updates all the stats in the READMEs.
+  Update the challenge statistics in the challenge repository
   """
   try:
     config = load_config()
   except FileNotFoundError:
-    print(f"[bright_red]Challenge repo not found, are you in the correct directory? If so, please run `{APP_CMD_NAME} init` first.")
+    console.print("Could not find CTF config file. Are you in the right directory?", style="bright_red")
     return
-
+  
+  if update_challenges:
+    for challenge in walk_challenges():
+      update_challenge_readme(challenge)
+  
   try:
     for category in config.categories:
       update_category_readme(category)
-    
+
     update_root_readme()
   except FileNotFoundError:
-    print(f"[bright_red]README not found. Please run `{APP_CMD_NAME} init` first.")
+    console.print(f"README not found. Please run `{APP_CMD_NAME} init` first", style="bright_red")
   else:
-    print("[green]READMEs updated successfully.")
+    print("Stats updated successfully", style="green")
 
 
 @stats_app.command("show")
 def stats_show(category: str = typer.Argument(None)):
   """
   Shows the stats of a category.
 
-  If no category is specified, shows the stats of all categories.
+  If no category is provided, shows the stats of all categories.
   """
   try:
     config = load_config()
   except FileNotFoundError:
-    print(f"[bright_red]Challenge repo not found, are you in the correct directory? If so, please run `{APP_CMD_NAME} init` first.")
+    console.print("Could not find CTF config file. Are you in the right directory?", style="bright_red")
     return
-
+  
   if category is None:
     table = Table(title="Overall Difficulty Distribution")
-    # Create a table in the following format
+    # TABLE FORMAT:
     # | Category | Easy | Medium | ... | Total |
     # | -------- | ---- | ------ | --- | ----- |
     # | ...      | ...  | ...    | ... | ...   |
     # | ...      | ...  | ...    | ... | ...   |
     # | Total    | ...  | ...    | ... | ...   |
     table.add_column("Category", header_style="bright_cyan", style="cyan", no_wrap=True)
-    for difficulty in config.diff_names:
-      table.add_column(difficulty.capitalize(), header_style="magenta", style="magenta", justify="center")
-    table.add_column("Total", header_style="bright_yellow", style="yellow", justify="center")
-
-    stats = {category: get_category_diff_stats(category) for category in config.categories}
+    for difficulty in config.difficulties:
+      table.add_column(difficulty.name, header_style="bright_magenta", style="magenta", justify="center")
+    table.add_coloumn("Total", header_style="bright_green", style="green", justify="center")
+
+    stats = {
+      category: get_category_difficulty_distribution(category)
+      for category in config.categories
+    }
 
     for category in stats:
-      # Check if it is the last category to add to the list
       is_last = category == config.categories[-1]
       table.add_row(
         category.capitalize(),
-        *[str(stats[category][difficulty]) for difficulty in config.diff_names],
+        *[str(stats[category][difficulty.name]) for difficulty in config.difficulties],
         str(sum(stats[category].values())),
         end_section=is_last
       )
 
-    # Add the total row
-    total_row = []
-    for difficulty in config.diff_names:
-      total_row.append(sum(stats[category][difficulty] for category in config.categories))
-
-    table.add_row(
-      "Total",
-      *map(str, total_row),
-      str(sum(total_row))
-    )
-    
+    total_row = ["Total"]
+    total_count = 0
+
+    for difficulty in config.difficulties:
+      count = sum(stats[category][difficulty.name] for category in stats)
+      total_row.append(str(count))
+      total_count += count
+
+    table.add_row(*total_row, str(total_count))
+
+  elif category.lower() not in config.categories:
+    console.print(f"Unknown category \"{category}\"", style="bright_red")
+    return
+  
   else:
-    table = Table(title=f"{category.capitalize()} Difficulty Distribution")
-    # Create a table in the following format
+    table = Table(title=f"Difficulty Distribution for {category.capitalize()}")
+    # TABLE FORMAT:
     # | Difficulty | Count |
     # | ---------- | ----- |
-    # | Easy       | ...   |
-    # | Medium     | ...   |
     # | ...        | ...   |
+    # | ...        | ...   |
+    # | Total      | ...   |
     table.add_column("Difficulty", header_style="bright_cyan", style="cyan")
-    table.add_column("Count", header_style="bright_yellow", style="yellow", justify="center")
+    table.add_column("Count", header_style="bright_green", style="green", justify="center")
+
+    stats = get_category_difficulty_distribution(category)
 
-    stats = get_category_diff_stats(category)
+    for difficulty in config.difficulties:
+      is_last = difficulty == config.difficulties[-1]
+      table.add_row(difficulty.name, str(stats[difficulty.name]), end_section=is_last)
 
-    for difficulty, count in stats.items():
-      table.add_row(difficulty.capitalize(), str(count))
+    table.add_row("Total", str(sum(stats.values())))
 
-  print(table)
+  console.print(table)
```

### Comparing `ctf_architect-0.1.0a4/ctf_architect/core/initialize.py` & `ctf_architect-0.1.0a5/ctf_architect/core/initialize.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,61 +1,71 @@
 """
-Contains the code to initialize a new CTF repo
+Implements challenge repo initialization.
 """
 
 from __future__ import annotations
 
 from pathlib import Path
 
 from ctf_architect.core.config import load_config, save_config
-from ctf_architect.core.models import Config
+from ctf_architect.core.models import CTFConfig
 from ctf_architect.core.stats import update_category_readme, update_root_readme
 
 
 def init_no_config(
+  name: str,
   categories: list[str],
   difficulties: list[dict[str, str | int]],
-  port: int,
+  starting_port: int,
+  extras: list[str] | None = None,
   config_only: bool = False
 ):
   """
-  Initialize the repo with the given config.
+  Initialize a challenge repo without a config file.
   """
-  config = Config(
+
+  config = CTFConfig(
+    name=name,
     categories=categories,
     difficulties=difficulties,
-    port=port
+    starting_port=starting_port,
+    extras=extras
   )
 
   save_config(config)
 
   if not config_only:
     # Create the challenge folder
     Path("challenges").mkdir(exist_ok=True)
 
     # Create the folders for each category
     for category in categories:
-      (Path("challenges") / category.lower()).mkdir(exist_ok=True)
+      Path(f"challenges/{category.lower()}").mkdir(exist_ok=True)
 
+    # Update the root README
     update_root_readme()
 
+    # Update the README for each category
     for category in categories:
       update_category_readme(category)
 
 
 def init_with_config():
   """
-  Initialize the repo with the config in ctf_config.yaml
+  Initialize a challenge repo with a config file.
   """
+
   config = load_config()
 
   # Create the challenge folder
   Path("challenges").mkdir(exist_ok=True)
 
   # Create the folders for each category
   for category in config.categories:
-    (Path("challenges") / category.lower()).mkdir(exist_ok=True)
+    Path(f"challenges/{category.lower()}").mkdir(exist_ok=True)
 
+  # Update the root README
   update_root_readme()
 
+  # Update the README for each category
   for category in config.categories:
     update_category_readme(category)
```

### Comparing `ctf_architect-0.1.0a4/ctf_architect/core/stats.py` & `ctf_architect-0.1.0a5/ctf_architect/core/stats.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,180 +1,198 @@
 from __future__ import annotations
 
 from pathlib import Path
+from warnings import warn
 
-from ctf_architect.core.challenge import get_challenge_info
+from ctf_architect.core.challenge import (create_challenge_readme,
+                                          get_chall_config)
 from ctf_architect.core.config import load_config
+from ctf_architect.core.constants import (CATEGORY_README_TEMPLATE,
+                                          ROOT_README_TEMPLATE)
+from ctf_architect.core.models import Challenge
 
 
-CATEGORY_README_TEMPLATE = """# {name} Challenges
-This directory contains challenges related to {name}.
-
-## Difficulty Distribution
-| Difficulty | Number of Challenges |
-| ---------- |:--------------------:|
-{diff_table}
-
-## Challenges ({count} total)
-| Name | Description | Difficulty | Author |
-| ---- | ----------- | ---------- | ------ |
-{challenges_table}
-"""
-
-ROOT_README_TEMPLATE = """# Challenges
-This directory contains all challenges.
-
-## Difficulty Distribution
-{diff_table}
-
-## Challenges ({count} total)
-| Name | Description | Category | Difficulty | Author |
-| ---- | ----------- | -------- | ---------- | ------ |
-{challenges_table}
-"""
-
-
-def get_category_diff_stats(name: str) -> dict[str, int]:
+def get_category_difficulty_distribution(name: str) -> dict[str, int]:
   """
-  Gets the difficulty distribution of a category.
+  Get the difficulty distribution of challenges in a category.
   """
   config = load_config()
 
   if name.lower() not in config.categories:
-    raise ValueError(f"Category {name} does not exist.")
+    raise ValueError(f"Category {name} does not exist")
   
   category_path = Path("challenges") / name.lower()
 
   difficulties = config.difficulties
 
-  stats = {difficulty["name"]: 0 for difficulty in difficulties}
+  stats = {
+    difficulty.name: 0
+    for difficulty in difficulties
+  }
 
   for challenge_path in category_path.iterdir():
     if challenge_path.is_dir():
-      info = get_challenge_info(challenge_path)
-      stats[info.difficulty.lower()] += 1
+      chall_config = get_chall_config(challenge_path)
+
+      if chall_config.difficulty.lower() not in stats:
+        warn(f"Ignoring unknown difficulty \"{chall_config.difficulty}\" in {challenge_path.absolute()}")
+        continue
+
+      stats[chall_config.difficulty.lower()] += 1
 
   return stats
 
 
+def update_challenge_readme(challenge: Challenge):
+
+  readme = create_challenge_readme(challenge)
+
+  with open(challenge.full_path / "README.md", "w" , encoding="utf-8") as f:
+    f.write(readme)
+
+
 def update_category_readme(name: str):
   """
   Updates the category's README.md file.
   """
   config = load_config()
 
   if name.lower() not in config.categories:
-    raise ValueError(f"Category {name} does not exist.")
+    raise ValueError(f"Category {name} does not exist")
   
-  challenges_path = Path("challenges")
+  category_path = Path("challenges") / name.lower()
 
-  # Check if the challenges directory exists
-  if not challenges_path.exists():
-    raise FileNotFoundError("Challenges directory does not exist, are you sure you are in the right directory?")
-  
-  category_path = challenges_path / name.lower()
+  # Check if the category directory exists
+  if not category_path.exists():
+    raise FileNotFoundError(f"The directory {category_path.absolute()} does not exist, are you in the right directory?")
 
-  # Get all challenge info
   challenges: list[list[str]] = []
-  
+
   for challenge_path in category_path.iterdir():
     if challenge_path.is_dir():
-      info = get_challenge_info(challenge_path)
-      challenges.append([info.name, info.description, info.difficulty, info.author])
+      config = get_chall_config(challenge_path)
+      challenges.append([
+        config.name,
+        config.folder_name,
+        config.description,
+        config.difficulty,
+        config.author
+      ])
 
-  # Get the difficulty stats
-  stats = get_category_diff_stats(name)
+  # Get the difficulty distribution
+  distribution = get_category_difficulty_distribution(name)
 
   # Create the challenges table
   challenges_table = "\n".join(
-    f"| [{name}](<./{name}>) |" +
+    f"| [{name}](<./{folder_name}>) |" +
     f" {description if len(description) <= 20 else description[:20]+'...'} |" +
     f" {difficulty.capitalize()} |" +
     f" {author} |"
-    for name, description, difficulty, author in challenges
+    for name, folder_name, description, difficulty, author in challenges
   )
 
-  # Create the difficulty table
+  # Create the difficulty distribution table
   diff_table = "\n".join(
     f"| {difficulty.capitalize()} | {count} |"
-    for difficulty, count in stats.items()
+    for difficulty, count in distribution.items()
   )
 
-  # Add the total row
-  diff_table += f"\n| Total | {sum(stats.values())} |"
+  # Total row
+  diff_table += f"\n| Total | {sum(distribution.values())} |"
 
   # Create the README
   readme = CATEGORY_README_TEMPLATE.format(
     name=name.capitalize(),
+    diff_table=diff_table,
     count=len(challenges),
-    challenges_table=challenges_table,  
-    diff_table=diff_table
+    challenges_table=challenges_table
   )
 
   # Write the README
-  with (category_path / "README.md").open("w") as f:
+  with open(category_path / "README.md", "w", encoding="utf-8") as f:
     f.write(readme)
 
 
 def update_root_readme():
   """
   Updates the root challenges README.md file.
   """
   config = load_config()
 
+  difficulties = config.difficulties
+
   challenges_path = Path("challenges")
 
   # Check if the challenges directory exists
   if not challenges_path.exists():
-    raise FileNotFoundError("Challenges directory does not exist, are you sure you are in the right directory?")
-
-  # Get all challenge info
-  challenges: list[list[str]] = []
+    raise FileNotFoundError(f"The directory {challenges_path.absolute()} does not exist, are you in the right directory?")
   
+  challenges: list[list[str]] = []
+  distributions: dict[str, dict[str, int]] = {}
+
   for category in config.categories:
     category_path = challenges_path / category.lower()
 
+    stats = {
+      difficulty.name: 0
+      for difficulty in difficulties
+    }
+
     for challenge_path in category_path.iterdir():
       if challenge_path.is_dir():
-        info = get_challenge_info(challenge_path)
-        challenges.append([info.name, info.description, info.category, info.difficulty, info.author])
+        chall_config = get_chall_config(challenge_path)
 
-  # Get the difficulty stats
-  stats = {category: get_category_diff_stats(category) for category in config.categories}
+        if chall_config.difficulty.lower() in stats:
+          stats[chall_config.difficulty.lower()] += 1
+        else:
+          warn(f"Ignoring unknown difficulty \"{chall_config.difficulty}\" in {challenge_path.absolute()}")
+
+        challenges.append([
+          chall_config.name,
+          chall_config.folder_name,
+          chall_config.description,
+          category,
+          chall_config.difficulty,
+          chall_config.author
+        ])
+    
+    distributions[category] = stats
 
   # Create the challenges table
   challenges_table = "\n".join(
-    f"| [{name}](<./{category.lower()}/{name}>) |" +
+    f"| [{name}](<./{category.lower()}/{folder_name}>) |" +
     f" {description if len(description) <= 20 else description[:20]+'...'} |" +
     f" {category.capitalize()} |" +
     f" {difficulty.capitalize()} |" +
     f" {author} |"
-    for name, description, category, difficulty, author in challenges
+    for name, folder_name, description, category, difficulty, author in challenges
   )
 
-  # Create the difficulty table
-  diff_table_header = "| Category | " + " | ".join(d.capitalize() for d in config.diff_names) + " | Total |\n"
-  diff_table_header += "| -------- |:" + ":|:".join("-" * len(diff) for diff in config.diff_names) + ":|:-----:|\n"
+  # Create the difficulty distribution table
+  diff_table_header = diff_table_header = "| Category | " + " | ".join(d.name.capitalize() for d in config.difficulties) + " | Total |\n"
+  diff_table_header += "| -------- |:" + ":|:".join("-" * len(diff.name) for diff in config.difficulties) + ":|:-----:|\n"
 
   diff_table_body = "\n".join(
-    f"| {category.capitalize()} | " + " | ".join(str(stats[category][diff]) for diff in config.diff_names) + f" | {sum(stats[category].values())} |"
-    for category in stats
+    f"| {category.capitalize()} | " +
+    " | ".join(str(distributions[category][diff.name]) for diff in config.difficulties) +
+    f" | {sum(distributions[category].values())} |"
+    for category in config.categories
   )
 
   diff_table_total = (
-    "\n| Total | " +
-    " | ".join(str(sum(stats[category][diff] for category in config.categories)) for diff in config.diff_names) +
-    f" | {sum(sum(stats[category].values()) for category in config.categories)} |\n"
+    "| Total | " +
+   " | ".join(str(sum(distributions[category][diff.name] for category in config.categories)) for diff in config.difficulties) +
+    f" | {sum(sum(distributions[category].values()) for category in config.categories)} |"
   )
 
-  diff_table = diff_table_header + diff_table_body + diff_table_total
+  diff_table =  f"{diff_table_header}{diff_table_body}\n{diff_table_total}\n"
 
   # Create the README
   readme = ROOT_README_TEMPLATE.format(
+    diff_table=diff_table,
     count=len(challenges),
-    challenges_table=challenges_table,  
-    diff_table=diff_table
+    challenges_table=challenges_table
   )
 
   # Write the README
-  with (challenges_path / "README.md").open("w") as f:
-    f.write(readme)
+  with open(challenges_path / "README.md", "w", encoding="utf-8") as f:
+    f.write(readme)
```

### Comparing `ctf_architect-0.1.0a4/pyproject.toml` & `ctf_architect-0.1.0a5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ctf-architect"
-version = "0.1.0a4"
+version = "0.1.0a5"
 description = "A tool for managing challenges for CTFs."
 authors = ["Jus-Codin <70018166+Jus-Codin@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
@@ -20,12 +20,23 @@
 ctf-architect = "ctf_architect.cli:app"
 chall-architect = "ctf_architect.chall_architect.cli:app"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 typer = {extras = ["all"], version = "^0.9.0"}
 pyyaml = "^6.0.1"
+tomlkit = "^0.12.3"
+pydantic = "^2.6.1"
+rich = "^13.7.1"
+
+
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+mkdocs-material = "^9.5.16"
+mkdocstrings = {extras = ["python"], version = "^0.24.1"}
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

