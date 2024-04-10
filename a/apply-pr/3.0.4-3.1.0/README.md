# Comparing `tmp/apply_pr-3.0.4.tar.gz` & `tmp/apply_pr-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/apply_pr/apply_pr/dist/tmpF9oAy1/apply_pr-3.0.4.tar", last modified: Thu Mar 14 11:29:10 2024, max compression
+gzip compressed data, was "/home/runner/work/apply_pr/apply_pr/dist/tmp_P9j7N/apply_pr-3.1.0.tar", last modified: Wed Apr 10 08:12:20 2024, max compression
```

## Comparing `apply_pr-3.0.4.tar` & `apply_pr-3.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 11:29:10.000000 apply_pr-3.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-03-14 11:28:24.000000 apply_pr-3.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 11:29:10.000000 apply_pr-3.0.4/apply_pr/
--rw-r--r--   0 runner    (1001) docker     (127)    47438 2024-03-14 11:28:24.000000 apply_pr-3.0.4/apply_pr/fabfile.py
--rw-r--r--   0 runner    (1001) docker     (127)    11891 2024-03-14 11:28:24.000000 apply_pr-3.0.4/apply_pr/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-14 11:28:24.000000 apply_pr-3.0.4/apply_pr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-03-14 11:28:24.000000 apply_pr-3.0.4/apply_pr/version.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-14 11:28:24.000000 apply_pr-3.0.4/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 11:29:10.000000 apply_pr-3.0.4/apply_pr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-14 11:29:10.000000 apply_pr-3.0.4/apply_pr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-14 11:29:10.000000 apply_pr-3.0.4/apply_pr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-14 11:29:10.000000 apply_pr-3.0.4/apply_pr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 11:29:10.000000 apply_pr-3.0.4/apply_pr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-14 11:29:10.000000 apply_pr-3.0.4/apply_pr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-14 11:29:10.000000 apply_pr-3.0.4/apply_pr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-14 11:28:24.000000 apply_pr-3.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-14 11:29:10.000000 apply_pr-3.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 11:29:10.000000 apply_pr-3.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-14 11:28:24.000000 apply_pr-3.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:12:20.000000 apply_pr-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-10 08:11:37.000000 apply_pr-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:12:20.000000 apply_pr-3.1.0/apply_pr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-10 08:12:20.000000 apply_pr-3.1.0/apply_pr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 08:12:20.000000 apply_pr-3.1.0/apply_pr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 08:12:20.000000 apply_pr-3.1.0/apply_pr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-10 08:12:20.000000 apply_pr-3.1.0/apply_pr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-10 08:12:20.000000 apply_pr-3.1.0/apply_pr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-10 08:12:20.000000 apply_pr-3.1.0/apply_pr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-10 08:11:37.000000 apply_pr-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 08:12:20.000000 apply_pr-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-04-10 08:11:37.000000 apply_pr-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-10 08:11:37.000000 apply_pr-3.1.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:12:20.000000 apply_pr-3.1.0/apply_pr/
+-rw-r--r--   0 runner    (1001) docker     (127)    48313 2024-04-10 08:11:37.000000 apply_pr-3.1.0/apply_pr/fabfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-10 08:11:37.000000 apply_pr-3.1.0/apply_pr/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11891 2024-04-10 08:11:37.000000 apply_pr-3.1.0/apply_pr/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-10 08:11:37.000000 apply_pr-3.1.0/apply_pr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-10 08:12:20.000000 apply_pr-3.1.0/PKG-INFO
```

### Comparing `apply_pr-3.0.4/README.md` & `apply_pr-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `apply_pr-3.0.4/apply_pr/fabfile.py` & `apply_pr-3.1.0/apply_pr/fabfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -876,14 +876,15 @@
         'Authorization': 'token %s' % github_config()['token']
     }
     prs = re.sub('{}+'.format(separator), separator, prs)
     pr_list = prs.split(separator)
     PRS = {}
     ERRORS = []
     TO_APPLY = []
+    TO_APPLY_CAUSE_PROJECT_VERSION_ERROR = []
     CLOSED_PRS = []
     IN_PROJECTS = []
     rep = GHAPIRequester(owner, repository)
     def get_prs_info(plist):
         res = []
         for _pr in tqdm(list(set(plist)), desc='Getting pr data from Github'):
             try:
@@ -900,14 +901,23 @@
                 res, key=lambda _p: (
                     _p['pullRequest'].get('mergedAt', max_meged_at) or max_meged_at,
                     _p['pullRequest'].get('createdAt') if (_p['pullRequest'].get('mergedAt', max_meged_at) or max_meged_at) == max_meged_at else ''
                 )
             )
         return res
 
+    def check_version_project_done(project_items):
+        if version:
+            parsed_version = version.split('.')
+            parsed_version = '{}.{}'.format(parsed_version[0], parsed_version[1])
+            for _project in project_items:
+                if _project['project_name'].startswith(parsed_version) and _project['card_state'] != 'Done':
+                    return False
+        return True
+
     for pull_info in tqdm(get_prs_info(pr_list), desc='Process PRs info'):
         pr_number = pull_info['pullRequest']['number']
         try:
             pull = pull_info['pullRequest']
             projects_info = pull_info['projectItems']
             projects_show = ''
             to_apply = '{}'.format(str(pr_number))
@@ -947,14 +957,17 @@
                             IN_PROJECTS.append(to_apply)
                     else:
                         message = colors.green(message)
                 else:
                     message = colors.red(message)
                     if not projects:
                         TO_APPLY.append(to_apply)
+                    elif not check_version_project_done(projects_info):
+                        TO_APPLY.append('{}'.format(str(pr_number)))
+                        TO_APPLY_CAUSE_PROJECT_VERSION_ERROR.append(to_apply)
                     else:
                         IN_PROJECTS.append(to_apply)
             PRS.setdefault(milestone, [])
             PRS[milestone] += [message]
         except Exception as e:
             # logger.error('Error PR {0}'.format(pr_number))
             err_msg = colors.red(
@@ -970,14 +983,17 @@
             print('\t{}'.format(prmsg))
     for prmsg in ERRORS:
             print('ERR\t{}'.format(prmsg))
     if version:
         print(colors.magenta('\nIncluded in projects\n'))
         for x in IN_PROJECTS:
             print(colors.magenta('* {}'.format(x)))
+        print(colors.red('\nIncluded in version project but in Error State\n'))
+        for _pr_project in TO_APPLY_CAUSE_PROJECT_VERSION_ERROR:
+            print(colors.red('* {}'.format(_pr_project)))
         if CLOSED_PRS:
             print(colors.red('\nClosed PRS: "{}"\n'.format(
                 ' '.join(CLOSED_PRS)
             )))
         print(colors.yellow(
             '\nNot Included: "{}"\n'.format(' '.join(TO_APPLY))
         ))
```

### Comparing `apply_pr-3.0.4/apply_pr/cli.py` & `apply_pr-3.1.0/apply_pr/cli.py`

 * *Files identical despite different names*

### Comparing `apply_pr-3.0.4/apply_pr/version.py` & `apply_pr-3.1.0/apply_pr/version.py`

 * *Files identical despite different names*

### Comparing `apply_pr-3.0.4/setup.py` & `apply_pr-3.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt', 'r') as f:
     INSTALL_REQUIRES = f.readlines()
 
 setup(
     name='apply_pr',
-    version='3.0.4',
+    version='3.1.0',
     packages=find_packages(),
     url='https://github.com/gisce/apply_pr',
     license='MIT',
     author='GISCE-TI, S.L.',
     author_email='devel@gisce.net',
     description='Apply Pull Requests from GitHub',
     entry_points='''
```

