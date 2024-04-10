# Comparing `tmp/streamlit-google-auth-1.0.4.tar.gz` & `tmp/streamlit-google-auth-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-google-auth-1.0.4.tar", last modified: Thu Mar 28 10:49:44 2024, max compression
+gzip compressed data, was "streamlit-google-auth-1.1.tar", last modified: Wed Apr 10 07:09:40 2024, max compression
```

## Comparing `streamlit-google-auth-1.0.4.tar` & `streamlit-google-auth-1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-03-28 10:49:44.605019 streamlit-google-auth-1.0.4/
--rw-rw-rw-   0        0        0     1088 2024-03-27 19:48:55.000000 streamlit-google-auth-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     6725 2024-03-28 10:49:44.605019 streamlit-google-auth-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     4759 2024-03-28 10:42:11.000000 streamlit-google-auth-1.0.4/README.md
--rw-rw-rw-   0        0        0      827 2024-03-28 10:49:39.000000 streamlit-google-auth-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-28 10:49:44.606022 streamlit-google-auth-1.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-28 10:49:44.591020 streamlit-google-auth-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-03-28 10:49:44.595020 streamlit-google-auth-1.0.4/src/streamlit_google_auth/
--rw-rw-rw-   0        0        0     3191 2024-03-28 10:36:24.000000 streamlit-google-auth-1.0.4/src/streamlit_google_auth/__init__.py
--rw-rw-rw-   0        0        0     3824 2024-03-28 10:32:26.000000 streamlit-google-auth-1.0.4/src/streamlit_google_auth/_auth.py
--rw-rw-rw-   0        0        0     1881 2024-03-28 10:36:28.000000 streamlit-google-auth-1.0.4/src/streamlit_google_auth/_cookies.py
-drwxrwxrwx   0        0        0        0 2024-03-28 10:49:44.604021 streamlit-google-auth-1.0.4/src/streamlit_google_auth.egg-info/
--rw-rw-rw-   0        0        0     6725 2024-03-28 10:49:44.000000 streamlit-google-auth-1.0.4/src/streamlit_google_auth.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      387 2024-03-28 10:49:44.000000 streamlit-google-auth-1.0.4/src/streamlit_google_auth.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-28 10:49:44.000000 streamlit-google-auth-1.0.4/src/streamlit_google_auth.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2024-03-28 10:49:44.000000 streamlit-google-auth-1.0.4/src/streamlit_google_auth.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-03-28 10:49:44.000000 streamlit-google-auth-1.0.4/src/streamlit_google_auth.egg-info/top_level.txt
+drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 07:09:40.508722 streamlit-google-auth-1.1/
+-rw-r--r--   0 adrien     (501) staff       (20)     1088 2024-04-09 14:41:40.000000 streamlit-google-auth-1.1/LICENSE
+-rw-r--r--   0 adrien     (501) staff       (20)     5983 2024-04-10 07:09:40.508478 streamlit-google-auth-1.1/PKG-INFO
+-rw-r--r--   0 adrien     (501) staff       (20)     4157 2024-04-09 15:21:39.000000 streamlit-google-auth-1.1/README.md
+-rw-r--r--   0 adrien     (501) staff       (20)      827 2024-04-10 07:09:27.000000 streamlit-google-auth-1.1/pyproject.toml
+-rw-r--r--   0 adrien     (501) staff       (20)       38 2024-04-10 07:09:40.508767 streamlit-google-auth-1.1/setup.cfg
+drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 07:09:40.506293 streamlit-google-auth-1.1/src/
+drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 07:09:40.506895 streamlit-google-auth-1.1/src/streamlit_google_auth/
+-rw-r--r--   0 adrien     (501) staff       (20)     5998 2024-04-09 15:56:05.000000 streamlit-google-auth-1.1/src/streamlit_google_auth/__init__.py
+drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 07:09:40.507948 streamlit-google-auth-1.1/src/streamlit_google_auth/cookie/
+-rw-r--r--   0 adrien     (501) staff       (20)     3599 2024-04-09 15:36:22.000000 streamlit-google-auth-1.1/src/streamlit_google_auth/cookie/__init__.py
+drwxr-xr-x   0 adrien     (501) staff       (20)        0 2024-04-10 07:09:40.508229 streamlit-google-auth-1.1/src/streamlit_google_auth.egg-info/
+-rw-r--r--   0 adrien     (501) staff       (20)     5983 2024-04-10 07:09:40.000000 streamlit-google-auth-1.1/src/streamlit_google_auth.egg-info/PKG-INFO
+-rw-r--r--   0 adrien     (501) staff       (20)      359 2024-04-10 07:09:40.000000 streamlit-google-auth-1.1/src/streamlit_google_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 adrien     (501) staff       (20)        1 2024-04-10 07:09:40.000000 streamlit-google-auth-1.1/src/streamlit_google_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 adrien     (501) staff       (20)       89 2024-04-10 07:09:40.000000 streamlit-google-auth-1.1/src/streamlit_google_auth.egg-info/requires.txt
+-rw-r--r--   0 adrien     (501) staff       (20)       22 2024-04-10 07:09:40.000000 streamlit-google-auth-1.1/src/streamlit_google_auth.egg-info/top_level.txt
```

### Comparing `streamlit-google-auth-1.0.4/LICENSE` & `streamlit-google-auth-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-google-auth-1.0.4/README.md` & `streamlit-google-auth-1.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,132 +1,98 @@
-# streamlit-google-auth
-
-`streamlit-google-auth` is a simple package to add google authentification in your streamlit app.  
-For that I use the google API, so you will need a google cloud account and to create credentials.  
-
-## 1. Get your google credentials json
-
-1. Go to google cloud
-2. Create an account and a project
-3. Go to APIs & services
-4. On the left sidebar, go to Credentials
-5. Anable the API
-6. On the top bar, click on + CREATE CREDENTIALS and select OAuth client ID
-7. Select Web application and name the it as you want
-8. Add the URLs of your apps in both origins and redirect (Recommend adding `http:localhost:8501` for dev)
-9. You should see a new row in OAuth 2.0 Client IDs where you can download the json
-
-## 2. Install the package
+# Streamlit Google Auth
+This package provides a simple and easy-to-use integration of Google authentication in your Streamlit application.
 
+## Getting Started
+1. Install the package:  
 `pip install streamlit-google-auth`
 
-## 3. login and logout
-
-The `login` function will first check the cookies if the user already exist.  
-And create a button that the user can use.
-
-In the other hand, `logout` is just a function and a button need to be created.
-
-```python
-import streamlit as st
-from streamlit_google_auth import login, logout
-
-secret_credentials_path = 'google_credentials.json'
-cookie_name = 'my_cookie_name'
-cookie_key = 'this_is_secret'
-cookie_expiry_days = 30
-app_url = 'http://localhost:8501'
-color = 'blue' # Or 'white'
-justify_content = 'center'
-
-st.title('Streamlit Google Auth Example 1')
-
-
-login(
-    secret_credentials_path=secret_credentials_path,
-    cookie_name=cookie_name,
-    cookie_key=cookie_key,
-    cookie_expiry_days=cookie_expiry_days,
-    app_url=app_url,
-    color=color,
-    justify_content=justify_content
-)
-
-if st.session_state['connected']:
-    st.image(st.session_state['user_info'].get('picture'))
-    st.write('Hello, '+ st.session_state['user_info'].get('name'))
-    st.write('Your email is '+ st.session_state['user_info'].get('email'))
-    if st.button('Log out'):
-        logout(cookie_name)
-```
-
-Once the login function run, session_state will have 3 new keys ,  and ``.
-- `connected` : A Boolean True if connected, False if not
-- `oauth_id` : Is a unique identifier from Google
-- `user_info` : Is user infos provided by google:
-    - `name`
-    - `email`
-    - `picture`
-    - Note: you can request more when creating the google credentials json. The user will se what you are asking in the google login page.
-
-## 4. check_cookies, get_authorization_url and check_authentification
-
-If you want to implement the login in another way, you can use the `check_cookies`, `get_authorization_url` and `check_authentification` functions.  
-At the start of you app, you can call `check_cookies` and if the cookie exist, the user is automatically log.  
-`check_cookies` also add the keys `connected`, `oauth_id` and `user_info` to session_state.
-
-```python
-from streamlit_google_auth import check_cookies
-
-check_cookies(cookie_name, cookie_key)
-```
+2. Create a Google Cloud Platform project and obtain the client ID and client secret. You can follow the instructions [here](https://developers.google.com/identity/protocols/oauth2/web-server#creatingcred) to create the credentials.
 
-And if you just want the url that the user need to use to access the login google url.  
-This is usefull if you want to do a custom button, ect.
+3. Save the client ID and client secret in a JSON file (e.g., google_credentials.json).
 
-```python
-from streamlit_google_auth import get_authorization_url
-
-get_authorization_url(secret_credentials_path, app_url)
-```
-
-Note: You can check for cookies before calling `login`
-
-Now the last function to use is `check_authentification`.  
-This function will catch when the user come back from the google authentification URL and log the user in.
-
-```python
-from streamlit_google_auth import check_authentification
+4. Import the necessary modules and initialize the Authenticate class:  
+    ```python
+    import streamlit as st
+    from streamlit_google_auth import Authenticate
+
+    authenticator = Authenticate(
+        secret_credentials_path='google_credentials.json',
+        cookie_name='my_cookie_name',
+        cookie_key='this_is_secret',
+        redirect_uri='http://localhost:8501',
+    )
+    ```
+
+5. Check if the user is already authenticated and handle the login/logout flow:
+    ```python
+    # Check if the user is already authenticated
+    authenticator.check_authentification()
+
+    # Display the login button if the user is not authenticated
+    if not st.session_state.get('connected', False):
+        authorization_url = authenticator.get_authorization_url()
+        st.markdown(f'[Login]({authorization_url})')
+        st.link_button('Login', authorization_url)
+    # Display the user information and logout button if the user is authenticated
+    else:
+        st.image(st.session_state['user_info'].get('picture'))
+        st.write(f"Hello, {st.session_state['user_info'].get('name')}")
+        st.write(f"Your email is {st.session_state['user_info'].get('email')}")
+        if st.button('Log out'):
+            authenticator.logout()
+    ```
+
+That's it! Your Streamlit app now has Google authentication integrated.
+
+## Configuration
+The Authenticate class takes the following parameters:
+
+- `secret_credentials_path`: The path to the Google Cloud Platform credentials JSON file.
+- `cookie_name`: The name of the cookie used to store the authentication information.
+- `cookie_key`: The secret key used to encrypt the cookie.
+- `redirect_uri`: The redirect URI of your Streamlit application.
+- `cookie_expiry_days`: Optional, The number of days the cookie stay valid.
+
+## Functions
+The Authenticate class provides the following functions:
+- `check_authentification()`: Catch the event when the user come back from the google login page and log it.
+- `login()`: Displays the login button and handles the authentication flow.
+- `logout()`: Logs out the user and clears the session state.
+- `get_authorization_url()`: Returns the URL for the Google authentication page.
+
+## Session State
+The Authenticate class updates the following keys in the Streamlit session state:
+- `connected`: A boolean indicating whether the user is authenticated or not.
+- `oauth_id`: The unique identifier for the authenticated user.
+- `user_info`: A dictionary containing the user's name, email, and profile picture URL.
 
-check_authentification(secret_credentials_path, cookie_name, cookie_key, cookie_expiry_days, app_url)
-```
+## Example
+Here's a complete example of how to use the Authenticate class in a Streamlit app:
 
-Here a simple example implemented:  
 ```python
 import streamlit as st
-from streamlit_google_auth import logout, check_cookies, get_authorization_url, check_authentification
+from streamlit_google_auth import Authenticate
 
-secret_credentials_path = 'google_credentials.json'
-cookie_name = 'my_cookie_name'
-cookie_key = 'this_is_secret'
-cookie_expiry_days = 30
-app_url = 'http://localhost:8501'
+st.title('Streamlit Google Auth Example')
 
-# Check the cookies for authentication
+if 'connected' not in st.session_state:
+    authenticator = Authenticate(
+        secret_credentials_path = 'google_credentials.json',
+        cookie_name='my_cookie_name',
+        cookie_key='this_is_secret',
+        redirect_uri = 'http://localhost:8501',
+    )
+    st.session_state["authenticator"] = authenticator
 
-st.title('Streamlit Google Auth Example 2')
+# Catch the login event
+st.session_state["authenticator"].check_authentification()
 
-if not check_cookies(cookie_name, cookie_key):
-    check_authentification(secret_credentials_path, cookie_name, cookie_key, cookie_expiry_days, app_url)
+# Create the login button
+st.session_state["authenticator"].login()
 
 if st.session_state['connected']:
     st.image(st.session_state['user_info'].get('picture'))
     st.write('Hello, '+ st.session_state['user_info'].get('name'))
     st.write('Your email is '+ st.session_state['user_info'].get('email'))
     if st.button('Log out'):
-        logout(cookie_name)
-else:
-    st.write('You are not connected')
-    authorization_url = get_authorization_url(secret_credentials_path, app_url)
-    st.markdown(f'[Login]({authorization_url})')
-    st.link_button('Login', authorization_url)
+        st.session_state["authenticator"].logout()
 ```
```

### Comparing `streamlit-google-auth-1.0.4/pyproject.toml` & `streamlit-google-auth-1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "streamlit-google-auth"
-version = "1.0.4"
+version = "1.1"
 description = "Use Google authentification in streamlit"
 readme = "README.md"
 authors = [{ name = "Adrien Bouvais", email = "adrien.bouvais.pro@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -21,8 +21,8 @@
     "extra-streamlit-components",
     "google-auth-oauthlib",
     "google-api-python-client"
 ]
 requires-python = ">=3.9.7"
 
 [project.urls]
-Homepage = "https://github.com/MrBounty/streamlit-google-auth"
+Homepage = "https://github.com/MrBounty/streamlit-google-auth"
```

