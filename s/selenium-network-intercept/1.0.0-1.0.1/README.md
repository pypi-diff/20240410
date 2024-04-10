# Comparing `tmp/selenium-network-intercept-1.0.0.tar.gz` & `tmp/selenium-network-intercept-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium-network-intercept-1.0.0.tar", last modified: Mon Apr  8 20:44:30 2024, max compression
+gzip compressed data, was "selenium-network-intercept-1.0.1.tar", last modified: Wed Apr 10 06:00:16 2024, max compression
```

## Comparing `selenium-network-intercept-1.0.0.tar` & `selenium-network-intercept-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 20:44:30.683532 selenium-network-intercept-1.0.0/
--rw-rw-rw-   0        0        0     1093 2024-04-08 16:39:54.000000 selenium-network-intercept-1.0.0/LICENCE
--rw-rw-rw-   0        0        0     6485 2024-04-08 20:44:30.682535 selenium-network-intercept-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     6076 2024-04-08 20:42:57.000000 selenium-network-intercept-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 20:44:30.676069 selenium-network-intercept-1.0.0/selenium_network_intercept/
--rw-rw-rw-   0        0        0       37 2024-04-08 16:34:11.000000 selenium-network-intercept-1.0.0/selenium_network_intercept/__init__.py
--rw-rw-rw-   0        0        0       39 2024-04-08 18:15:43.000000 selenium-network-intercept-1.0.0/selenium_network_intercept/exceptions.py
--rw-rw-rw-   0        0        0     4446 2024-04-08 20:38:02.000000 selenium-network-intercept-1.0.0/selenium_network_intercept/intercept.py
--rw-rw-rw-   0        0        0     3542 2024-04-08 19:46:19.000000 selenium-network-intercept-1.0.0/selenium_network_intercept/objected.py
--rw-rw-rw-   0        0        0     2226 2024-04-08 20:38:02.000000 selenium-network-intercept-1.0.0/selenium_network_intercept/request.py
--rw-rw-rw-   0        0        0     1580 2024-04-08 20:38:02.000000 selenium-network-intercept-1.0.0/selenium_network_intercept/response.py
-drwxrwxrwx   0        0        0        0 2024-04-08 20:44:30.681069 selenium-network-intercept-1.0.0/selenium_network_intercept.egg-info/
--rw-rw-rw-   0        0        0     6485 2024-04-08 20:44:30.000000 selenium-network-intercept-1.0.0/selenium_network_intercept.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      462 2024-04-08 20:44:30.000000 selenium-network-intercept-1.0.0/selenium_network_intercept.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 20:44:30.000000 selenium-network-intercept-1.0.0/selenium_network_intercept.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-04-08 20:44:30.000000 selenium-network-intercept-1.0.0/selenium_network_intercept.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 20:44:30.683532 selenium-network-intercept-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      664 2024-04-08 20:43:25.000000 selenium-network-intercept-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 06:00:16.378982 selenium-network-intercept-1.0.1/
+-rw-rw-rw-   0        0        0     1093 2024-04-08 16:39:54.000000 selenium-network-intercept-1.0.1/LICENCE
+-rw-rw-rw-   0        0        0     6905 2024-04-10 06:00:16.377977 selenium-network-intercept-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6471 2024-04-10 05:59:09.000000 selenium-network-intercept-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 06:00:16.369979 selenium-network-intercept-1.0.1/selenium_network_intercept/
+-rw-rw-rw-   0        0        0       37 2024-04-08 16:34:11.000000 selenium-network-intercept-1.0.1/selenium_network_intercept/__init__.py
+-rw-rw-rw-   0        0        0       39 2024-04-08 18:15:43.000000 selenium-network-intercept-1.0.1/selenium_network_intercept/exceptions.py
+-rw-rw-rw-   0        0        0     4446 2024-04-08 20:38:02.000000 selenium-network-intercept-1.0.1/selenium_network_intercept/intercept.py
+-rw-rw-rw-   0        0        0     3542 2024-04-09 22:44:25.000000 selenium-network-intercept-1.0.1/selenium_network_intercept/objected.py
+-rw-rw-rw-   0        0        0     2226 2024-04-08 20:38:02.000000 selenium-network-intercept-1.0.1/selenium_network_intercept/request.py
+-rw-rw-rw-   0        0        0     1580 2024-04-08 20:38:02.000000 selenium-network-intercept-1.0.1/selenium_network_intercept/response.py
+drwxrwxrwx   0        0        0        0 2024-04-10 06:00:16.376978 selenium-network-intercept-1.0.1/selenium_network_intercept.egg-info/
+-rw-rw-rw-   0        0        0     6905 2024-04-10 06:00:16.000000 selenium-network-intercept-1.0.1/selenium_network_intercept.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      531 2024-04-10 06:00:16.000000 selenium-network-intercept-1.0.1/selenium_network_intercept.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 06:00:16.000000 selenium-network-intercept-1.0.1/selenium_network_intercept.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-10 06:00:16.000000 selenium-network-intercept-1.0.1/selenium_network_intercept.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 06:00:16.375979 selenium-network-intercept-1.0.1/selenium_search_file/
+-rw-rw-rw-   0        0        0       36 2024-04-10 05:46:53.000000 selenium-network-intercept-1.0.1/selenium_search_file/__init__.py
+-rw-rw-rw-   0        0        0     3417 2024-04-10 05:46:45.000000 selenium-network-intercept-1.0.1/selenium_search_file/search_file.py
+-rw-rw-rw-   0        0        0       42 2024-04-10 06:00:16.378982 selenium-network-intercept-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      714 2024-04-10 05:59:55.000000 selenium-network-intercept-1.0.1/setup.py
```

### Comparing `selenium-network-intercept-1.0.0/LICENCE` & `selenium-network-intercept-1.0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `selenium-network-intercept-1.0.0/PKG-INFO` & `selenium-network-intercept-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 Metadata-Version: 2.1
 Name: selenium-network-intercept
-Version: 1.0.0
+Version: 1.0.1
 Summary: Interceptador de requisições http não oficial do selenium 4
 Author: Alexandre Mariano
 Author-email: alexandre_mariano@hotmail.com.br
 License: MIT License
-Keywords: selenium,network,intercept,http,requests,selenium network intercept,selenium intercept
+Keywords: selenium,network,intercept,http,requests,selenium network intercept,selenium intercept,search download selenium
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
-## Atualização 1.0.0
+## Atualização 1.0.1
+
+Com a atualização da biblioteca agora é possível verificar se ao interagir com algum elemento em tela usando o selenium, se foi baixado um arquivo em um diretório específico.
+
+Siga o [repositório oficial](https://github.com/alexandremariano4/selenium_network_intercept/tree/main/selenium_search_file) desta funcionalidade para entendê-la e aplicá-la.
+
+
+
+## Atualização 1.0.1
 
 Agora é possível recuperar os parâmetros de queries e também é retornado a URL que foi capturado os parâmetros.
 Altamente recomendado utilizar o arquivo exemplo3.py do [repositório oficial](https://github.com/alexandremariano4/selenium_network_intercept/tree/main) para ter entendimento e aplicabilidade ao seu cenário.
 Em algumas situações não será viável usar essa funcionalidade, somente a busca do objeto com body,status e url terão que satisfazer.
 
 
 ## Get Started
```

### Comparing `selenium-network-intercept-1.0.0/README.md` & `selenium-network-intercept-1.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,16 @@
-## Atualização 1.0.0
+## Atualização 1.0.1
+
+Com a atualização da biblioteca agora é possível verificar se ao interagir com algum elemento em tela usando o selenium, se foi baixado um arquivo em um diretório específico.
+
+Siga o [repositório oficial](https://github.com/alexandremariano4/selenium_network_intercept/tree/main/selenium_search_file) desta funcionalidade para entendê-la e aplicá-la.
+
+
+
+## Atualização 1.0.1
 
 Agora é possível recuperar os parâmetros de queries e também é retornado a URL que foi capturado os parâmetros.
 Altamente recomendado utilizar o arquivo exemplo3.py do [repositório oficial](https://github.com/alexandremariano4/selenium_network_intercept/tree/main) para ter entendimento e aplicabilidade ao seu cenário.
 Em algumas situações não será viável usar essa funcionalidade, somente a busca do objeto com body,status e url terão que satisfazer.
 
 
 ## Get Started
```

### Comparing `selenium-network-intercept-1.0.0/selenium_network_intercept/intercept.py` & `selenium-network-intercept-1.0.1/selenium_network_intercept/intercept.py`

 * *Files identical despite different names*

### Comparing `selenium-network-intercept-1.0.0/selenium_network_intercept/objected.py` & `selenium-network-intercept-1.0.1/selenium_network_intercept/objected.py`

 * *Files identical despite different names*

### Comparing `selenium-network-intercept-1.0.0/selenium_network_intercept/request.py` & `selenium-network-intercept-1.0.1/selenium_network_intercept/request.py`

 * *Files identical despite different names*

### Comparing `selenium-network-intercept-1.0.0/selenium_network_intercept/response.py` & `selenium-network-intercept-1.0.1/selenium_network_intercept/response.py`

 * *Files identical despite different names*

### Comparing `selenium-network-intercept-1.0.0/selenium_network_intercept.egg-info/PKG-INFO` & `selenium-network-intercept-1.0.1/selenium_network_intercept.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 Metadata-Version: 2.1
 Name: selenium-network-intercept
-Version: 1.0.0
+Version: 1.0.1
 Summary: Interceptador de requisições http não oficial do selenium 4
 Author: Alexandre Mariano
 Author-email: alexandre_mariano@hotmail.com.br
 License: MIT License
-Keywords: selenium,network,intercept,http,requests,selenium network intercept,selenium intercept
+Keywords: selenium,network,intercept,http,requests,selenium network intercept,selenium intercept,search download selenium
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
-## Atualização 1.0.0
+## Atualização 1.0.1
+
+Com a atualização da biblioteca agora é possível verificar se ao interagir com algum elemento em tela usando o selenium, se foi baixado um arquivo em um diretório específico.
+
+Siga o [repositório oficial](https://github.com/alexandremariano4/selenium_network_intercept/tree/main/selenium_search_file) desta funcionalidade para entendê-la e aplicá-la.
+
+
+
+## Atualização 1.0.1
 
 Agora é possível recuperar os parâmetros de queries e também é retornado a URL que foi capturado os parâmetros.
 Altamente recomendado utilizar o arquivo exemplo3.py do [repositório oficial](https://github.com/alexandremariano4/selenium_network_intercept/tree/main) para ter entendimento e aplicabilidade ao seu cenário.
 Em algumas situações não será viável usar essa funcionalidade, somente a busca do objeto com body,status e url terão que satisfazer.
 
 
 ## Get Started
```

### Comparing `selenium-network-intercept-1.0.0/setup.py` & `selenium-network-intercept-1.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 file = open('README.md', 'r',encoding='utf-8')
 readme = file.read()
 
 
 setup(
     name='selenium-network-intercept',
-    version='1.0.0',
+    version='1.0.1',
     license='MIT License',
     author='Alexandre Mariano',
     long_description=readme,
     long_description_content_type='text/markdown',
     author_email='alexandre_mariano@hotmail.com.br',
-    keywords=['selenium', 'network', 'intercept','http','requests','selenium network intercept','selenium intercept'],
+    keywords=['selenium', 'network', 'intercept','http','requests','selenium network intercept','selenium intercept','search download selenium'],
     description='Interceptador de requisições http não oficial do selenium 4',
-    packages=['selenium_network_intercept'],
+    packages=['selenium_network_intercept','selenium_search_file'],
     install_requires=[]
 )
 
 file.close()
```

