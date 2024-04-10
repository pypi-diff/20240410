# Comparing `tmp/python-bmob-1.2.tar.gz` & `tmp/python-bmob-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\python-bmob-1.2.tar", last modified: Tue Apr  9 14:55:33 2024, max compression
+gzip compressed data, was "dist\python-bmob-1.3.tar", last modified: Tue Apr  9 15:07:05 2024, max compression
```

## Comparing `python-bmob-1.2.tar` & `python-bmob-1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 14:55:33.656922 python-bmob-1.2/
--rw-rw-rw-   0        0        0      278 2024-04-09 14:55:33.656922 python-bmob-1.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-09 14:01:42.000000 python-bmob-1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 14:55:33.647743 python-bmob-1.2/bmobpy/
--rw-rw-rw-   0        0        0       25 2024-04-09 14:54:42.000000 python-bmob-1.2/bmobpy/__init__.py
--rw-rw-rw-   0        0        0    19744 2024-04-09 14:01:42.000000 python-bmob-1.2/bmobpy/bmob.py
-drwxrwxrwx   0        0        0        0 2024-04-09 14:55:33.656922 python-bmob-1.2/python_bmob.egg-info/
--rw-rw-rw-   0        0        0      278 2024-04-09 14:55:33.000000 python-bmob-1.2/python_bmob.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2024-04-09 14:55:33.000000 python-bmob-1.2/python_bmob.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 14:55:33.000000 python-bmob-1.2/python_bmob.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-09 14:55:33.000000 python-bmob-1.2/python_bmob.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 14:55:33.660472 python-bmob-1.2/setup.cfg
--rw-rw-rw-   0        0        0      406 2024-04-09 14:54:55.000000 python-bmob-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 15:07:05.631563 python-bmob-1.3/
+-rw-rw-rw-   0        0        0      278 2024-04-09 15:07:05.631563 python-bmob-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-09 14:01:42.000000 python-bmob-1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 15:07:05.615761 python-bmob-1.3/bmobpy/
+-rw-rw-rw-   0        0        0       25 2024-04-09 14:54:42.000000 python-bmob-1.3/bmobpy/__init__.py
+-rw-rw-rw-   0        0        0    19775 2024-04-09 15:06:06.000000 python-bmob-1.3/bmobpy/bmob.py
+drwxrwxrwx   0        0        0        0 2024-04-09 15:07:05.626018 python-bmob-1.3/python_bmob.egg-info/
+-rw-rw-rw-   0        0        0      278 2024-04-09 15:07:05.000000 python-bmob-1.3/python_bmob.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2024-04-09 15:07:05.000000 python-bmob-1.3/python_bmob.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 15:07:05.000000 python-bmob-1.3/python_bmob.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-09 15:07:05.000000 python-bmob-1.3/python_bmob.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 15:07:05.632804 python-bmob-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      391 2024-04-09 15:06:58.000000 python-bmob-1.3/setup.py
```

### Comparing `python-bmob-1.2/bmobpy/bmob.py` & `python-bmob-1.3/bmobpy/bmob.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,15 +234,15 @@
 		else:
 			isIn = "$notInQuery"
 		if isinstance(value, BmobQuerier):
 			innerQuery = {"className": className, "where": value.filter}
 		return self.putWhereFilter(key, value, isIn)
 
 class HttpResponse:
-	def __init__(self, code, status, headers, data, error = None):
+	def init(self, code, status, headers, data, error = None):
 		if code == None:
 			code = -100
 		if status == None:
 			status = 'Unknown Error'
 		if headers == None:
 			headers = {}
 		if data == None:
@@ -308,29 +308,29 @@
 		body = body.encode("utf-8")
 	req = import_urllib.Request(url=url, data=body, headers=headers)
 	if method != None:
 		req.get_method = lambda: method
 
 		try:
 			res = import_urllib.urlopen(req, timeout=timeout)
-			return HttpResponse(res.code, res.msg, res.headers, res.read())
+			return HttpResponse().init(res.code, res.msg, res.headers, res.read())
 		except import_urllib.URLError as e:
 			try:
 				if hasattr(e, "reason"):
 					reason = e.reason
 				else:
 					reason = None
-				return HttpResponse(e.code, e.msg, e.headers, e.read(), reason)
+				return HttpResponse().init(e.code, e.msg, e.headers, e.read(), reason)
 			except Exception as e:
 				print("Req failed wih response.init:", e)
 				errMsg = "Unknown Error"
-				return HttpResponse(-3, errMsg, {}, errMsg, repr(e))
+				return HttpResponse().init(-3, errMsg, {}, errMsg, repr(e))
 	else:
 		errMsg = "Unknown Error"
-		return HttpResponse(-4, errMsg, {}, errMsg, errMsg)
+		return HttpResponse().init(-4, errMsg, {}, errMsg, errMsg)
 
 class Bmob:
 	def __init__(self, application_id, rest_api_key):
 		"""初始化Bmob
 
 		Args:
 			application_id (string): 进入Bmob控制台，具体应用 -> 设置 -> 应用密钥 -> Application ID
@@ -592,15 +592,15 @@
 				params += '&where=' + quote(json.dumps(where, default=def_marshal))
 			if len(params) != 0:
 				url += '?' + params[1:]
 			return httpRequest(url = url, method = 'GET', headers = self.headers)
 		except Exception as e:
 			print(repr(e))
 			msg = 'Bad Query'
-			return HttpResponse(-1, msg, None, msg, msg)
+			return HttpResponse().init(-1, msg, None, msg, msg)
 	def findOne(self, className, objectId):
 		"""查询一条记录
 
 		Args:
 			className (string): 数据表名称
 			objectId (string): 这条记录的objectId
```

