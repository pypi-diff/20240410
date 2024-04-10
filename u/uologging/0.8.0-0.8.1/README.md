# Comparing `tmp/uologging-0.8.0.tar.gz` & `tmp/uologging-0.8.1.tar.gz`

## Comparing `uologging-0.8.0.tar` & `uologging-0.8.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 uologging-0.8.0/Jenkinsfile
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 uologging-0.8.0/MANIFEST.in
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 uologging-0.8.0/README.md
--rw-r--r--   0        0        0     9420 2020-02-02 00:00:00.000000 uologging-0.8.0/coverage-sources.zip
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 uologging-0.8.0/mkdocs.yml
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 uologging-0.8.0/.vscode/extensions.json
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 uologging-0.8.0/.vscode/settings.json
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 uologging-0.8.0/coverage/src_uologging___init__.py.zip
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 uologging-0.8.0/coverage/src_uologging_cli.py.zip
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 uologging-0.8.0/coverage/src_uologging_downloads.py.zip
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 uologging-0.8.0/coverage/src_uologging_performance.py.zip
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 uologging-0.8.0/coverage/src_uologging_uologging.py.zip
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 uologging-0.8.0/docs/README.md
--rw-r--r--   0        0        0     3212 2020-02-02 00:00:00.000000 uologging-0.8.0/docs/changelog.md
--rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 uologging-0.8.0/docs/development.md
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 uologging-0.8.0/docs/package-deployment.md
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 uologging-0.8.0/src/uologging/__init__.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 uologging-0.8.0/src/uologging/cli.py
--rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 uologging-0.8.0/src/uologging/downloads.py
--rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 uologging-0.8.0/src/uologging/performance.py
--rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 uologging-0.8.0/src/uologging/uologging.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 uologging-0.8.0/tests/test_downloads.py
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 uologging-0.8.0/tests/test_performance.py
--rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 uologging-0.8.0/tests/test_uologging.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uologging-0.8.0/tests/example/__init__.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 uologging-0.8.0/tests/example/__main__.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 uologging-0.8.0/tests/example/hello.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uologging-0.8.0/tests/example2/__init__.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 uologging-0.8.0/tests/example2/__main__.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 uologging-0.8.0/tests/example2/hello.py
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 uologging-0.8.0/.gitignore
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 uologging-0.8.0/hatch.toml
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 uologging-0.8.0/hatch_build.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 uologging-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     6976 2020-02-02 00:00:00.000000 uologging-0.8.0/docs/user-guide.md
--rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 uologging-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 uologging-0.8.1/Jenkinsfile
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 uologging-0.8.1/MANIFEST.in
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 uologging-0.8.1/README.md
+-rw-r--r--   0        0        0     9419 2020-02-02 00:00:00.000000 uologging-0.8.1/coverage-sources.zip
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 uologging-0.8.1/mkdocs.yml
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 uologging-0.8.1/.vscode/extensions.json
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 uologging-0.8.1/.vscode/settings.json
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 uologging-0.8.1/coverage/src_uologging___init__.py.zip
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 uologging-0.8.1/coverage/src_uologging_cli.py.zip
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 uologging-0.8.1/coverage/src_uologging_downloads.py.zip
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 uologging-0.8.1/coverage/src_uologging_performance.py.zip
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 uologging-0.8.1/coverage/src_uologging_uologging.py.zip
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 uologging-0.8.1/docs/README.md
+-rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 uologging-0.8.1/docs/changelog.md
+-rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 uologging-0.8.1/docs/development.md
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 uologging-0.8.1/docs/package-deployment.md
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 uologging-0.8.1/src/uologging/__init__.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 uologging-0.8.1/src/uologging/cli.py
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 uologging-0.8.1/src/uologging/downloads.py
+-rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 uologging-0.8.1/src/uologging/performance.py
+-rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 uologging-0.8.1/src/uologging/uologging.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 uologging-0.8.1/tests/test_downloads.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 uologging-0.8.1/tests/test_performance.py
+-rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 uologging-0.8.1/tests/test_uologging.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uologging-0.8.1/tests/example/__init__.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 uologging-0.8.1/tests/example/__main__.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 uologging-0.8.1/tests/example/hello.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uologging-0.8.1/tests/example2/__init__.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 uologging-0.8.1/tests/example2/__main__.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 uologging-0.8.1/tests/example2/hello.py
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 uologging-0.8.1/.gitignore
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 uologging-0.8.1/hatch.toml
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 uologging-0.8.1/hatch_build.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 uologging-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     6976 2020-02-02 00:00:00.000000 uologging-0.8.1/docs/user-guide.md
+-rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 uologging-0.8.1/PKG-INFO
```

### Comparing `uologging-0.8.0/.vscode/settings.json` & `uologging-0.8.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `uologging-0.8.0/coverage/src_uologging___init__.py.zip` & `uologging-0.8.1/coverage/src_uologging___init__.py.zip`

 * *Files 19% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 1594 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    10169 bl defN 23-Dec-13 13:59 src_uologging___init__.py
+?rw-r--r--  2.0 unx    10169 bl defN 24-Apr-10 14:36 src_uologging___init__.py
 1 file, 10169 bytes uncompressed, 1430 bytes compressed:  85.9%
```

#### src_uologging___init__.py

```diff
@@ -1 +1 @@
-<tr class="noCover"><td class="line"><a name="1">1</a></td><td class="hits"></td><td class="code"></td></tr><tr class="coverFull" data-html-tooltip="Covered at least once"><td class="line"><a name="2">2</a></td><td class="hits">1</td><td class="code">from warnings import warn</td></tr><tr class="noCover"><td class="line"><a name="3">3</a></td><td class="hits"></td><td class="code"></td></tr><tr class="coverFull" data-html-tooltip="Covered at least once"><td class="line"><a name="4">4</a></td><td class="hits">1</td><td class="code">from uologging.cli import add_verbosity_flag, get_default_parser</td></tr><tr class="coverFull" data-html-tooltip="Covered at least once"><td class="line"><a name="5">5</a></td><td class="hits">1</td><td class="code">from uologging.downloads import DownloadTracer</td></tr><tr class="coverFull" data-html-tooltip="Covered at least once"><td class="line"><a name="6">6</a></td><td class="hits">1</td><td class="code">from uologging.performance import trace</td></tr><tr class="coverFull" data-html-tooltip="Covered at least once"><td class="line"><a name="7">7</a></td><td class="hits">1</td><td class="code">from uologging.uologging import init_console, init_syslog, set_verbosity</td></tr><tr class="noCover"><td class="line"><a name="8">8</a></td><td class="hits"></td><td class="code"></td></tr><tr class="noCover"><td class="line"><a name="9">9</a></td><td class="hits"></td><td class="code"></td></tr><tr class="coverFull" data-html-tooltip="Covered at least once"><td class="line"><a name="10">10</a></td><td class="hits">1</td><td class="code">def function_renamed(function, old_name):</td></tr><tr class="noCover"><td class="line"><a name="11">11</a></td><td class="hits"></td><td class="code">    &#34;&#34;&#34;Want to change the name of some function in your python library?</td></tr><tr class="noCover"><td class="line"><a name="12">12</a></td><td class="hits"></td><td class="code">    But you don&#39;t want to break your users&#39; code?</td></tr><tr class="noCover"><td class="line"><a name="13">13</a></td><td class="hits"></td><td class="code"></td></tr><tr class="noCover"><td class="line"><a name="14">14</a></td><td class="hits"></td><td class="code">    This function will wrap any function with a deprecated alias.</td></tr><tr class="noCover"><td class="line"><a name="15">15</a></td><td class="hits"></td><td class="code">    </td></tr><tr class="noCover"><td class="line"><a name="16">16</a></td><td class="hits"></td><td class="code">    Example:</td></tr><tr class="noCover"><td class="line"><a name="17">17</a></td><td class="hits"></td><td class="code"></td></tr><tr class="noCover"><td class="line"><a name="18">18</a></td><td class="hits"></td><td class="code">    Imagine you have the &#39;say_hello&#39; function in your library.</td></tr><tr class="noCover"><td class="line"><a name="19">19</a></td><td class="hits"></td><td class="code"></td></tr><tr class="noCover"><td class="line"><a name="20">20</a></td><td class="hits"></td><td class="code">        &gt;&gt;&gt; def say_hello():</td></tr><tr class="noCover"><td class="line"><a name="21">21</a></td><td class="hits"></td><td class="code">        ...     print(&#39;Hello, world!&#39;)</td></tr><tr class="noCover"><td class="line"><a name="22">22</a></td><td class="hits"></td><td class="code">    </td></tr><tr class="noCover"><td class="line"><a name="23">23</a></td><td class="hits"></td><td class="code">    You want to change the name to &#39;hello,&#39; and so you do!</td></tr><tr class="noCover"><td class="line"><a name="24">24</a></td><td class="hits"></td><td class="code"></td></tr><tr class="noCover"><td class="line"><a name="25">25</a></td><td class="hits"></td><td class="code">        &gt;&gt;&gt; def hello():</td></tr><tr class="noCover"><td class="line"><a name="26">26</a></td><td class="hits"></td><td class="code">        ...     print(&#39;Hello, world!&#39;)</td></tr><tr class="noCover"><td class="line"><a name="27">27</a></td><td class="hits"></td><td class="code"></td></tr><tr class="noCover"><td class="line"><a name="28">28</a></td><td class="hits"></td><td class="code">    But, you don&#39;t want to break your users&#39; code.</td></tr><tr class="noCover"><td class="line"><a name="29">29</a></td><td class="hits"></td><td class="code"></td></tr><tr class="noCover"><td class="line"><a name="30">30</a></td><td class="hits"></td><td class="code">    </td></tr><tr class="noCover"><td class="line"><a name="31">31</a></td><td class="hits"></td><td class="code">        &gt;&gt;&gt; say_hello &#61; function_renamed(hello, &#39;say_hello&#39;)</td></tr><tr class="noCover"><td class="line"><a name="32">32</a></td><td class="hits"></td><td class="code">        &gt;&gt;&gt; __all__ &#61; [&#39;hello&#39;, &#39;say_hello&#39;]</td></tr><tr class="noCover"><td class="line"><a name="33">33</a></td><td class="hits"></td><td class="code"></td></tr><tr class="noCover"><td class="line"><a name="34">34</a></td><td class="hits"></td><td class="code"></td></tr><tr class="noCover"><td class="line"><a name="35">35</a></td><td class="hits"></td><td class="code">    Args:</td></tr><tr class="noCover"><td class="line"><a name="36">36</a></td><td class="hits"></td><td class="code">        new_function (_type_): _description_</td></tr><tr class="noCover"><td class="line"><a name="37">37</a></td><td class="hits"></td><td class="code">        deprecated_function_name (_type_): _description_</td></tr><tr class="noCover"><td class="line"><a name="38">38</a></td><td class="hits"></td><td class="code">    &#34;&#34;&#34;</td></tr><tr class="coverFull" data-html-tooltip="Covered at least once"><td class="line"><a name="39">39</a></td><td class="hits">1</td><td class="code">    def deprecated_function(*args, **kwargs):</td></tr><tr class="coverNone" data-html-tooltip="Not covered"><td class="line"><a name="40">40</a></td><td class="hits">0</td><td class="code">        deprecation_warning &#61; f&#39;{old_name}() is deprecated (we plan to remove it in next major-version). Please use {function.__name__}() instead.&#39;</td></tr><tr class="coverNone" data-html-tooltip="Not covered"><td class="line"><a name="41">41</a></td><td class="hits">0</td><td class="code">        warn(deprecation_warning, DeprecationWarning, stacklevel&#61;2)</td></tr><tr class="noCover"><td class="line"><a name="42">42</a></td><td class="hits"></td><td class="code">        # NOW, only after warning, pass on to the underlying function</td></tr><tr class="coverNone" data-html-tooltip="Not covered"><td class="line"><a name="43">43</a></td><td class="hits">0</td><td class="code">        function(*args, **kwargs)</td></tr><tr class="coverFull" data-html-tooltip="Covered at least once"><td class="line"><a name="44">44</a></td><td class="hits">1</td><td class="code">    return deprecated_function</td></tr><tr class="noCover"><td class="line"><a name="45">45</a></td><td class="hits"></td><td class="code"></td></tr><tr class="noCover"><td class="line"><a name="46">46</a></td><td class="hits"></td><td class="code"></td></tr><tr class="coverFull" data-html-tooltip="Covered at least once"><td class="line"><a name="47">47</a></td><td class="hits">1</td><td class="code">init_console_logging &#61; function_renamed(init_console, old_name&#61;&#39;init_console_logging&#39;)</td></tr><tr class="coverFull" data-html-tooltip="Covered at least once"><td class="line"><a name="48">48</a></td><td class="hits">1</td><td class="code">init_syslog_logging &#61; function_renamed(init_syslog, old_name&#61;&#39;init_syslog_logging&#39;)</td></tr><tr class="coverFull" data-html-tooltip="Covered at least once"><td class="line"><a name="49">49</a></td><td class="hits">1</td><td class="code">set_logging_verbosity &#61; function_renamed(set_verbosity, old_name&#61;&#39;set_logging_verbosity&#39;)</td></tr><tr class="noCover"><td class="line"><a name="50">50</a></td><td class="hits"></td><td class="code"></td></tr><tr class="coverFull" data-html-tooltip="Covered at least once"><td class="line"><a name="51">51</a></td><td class="hits">1</td><td class="code">__version__ &#61; &#39;0.8.0&#39;</td></tr><tr class="coverFull" data-html-tooltip="Covered at least once"><td class="line"><a name="52">52</a></td><td class="hits">1</td><td class="code">__all__ &#61; [</td></tr><tr class="noCover"><td class="line"><a name="53">53</a></td><td class="hits"></td><td class="code">    &#39;add_verbosity_flag&#39;, </td></tr><tr class="noCover"><td class="line"><a name="54">54</a></td><td class="hits"></td><td class="code">    &#39;DownloadTracer&#39;,</td></tr><tr class="noCover"><td class="line"><a name="55">55</a></td><td class="hits"></td><td class="code">    &#39;get_default_parser&#39;, </td></tr><tr class="noCover"><td class="line"><a name="56">56</a></td><td class="hits"></td><td class="code">    &#39;init_console_logging&#39;, </td></tr><tr class="noCover"><td class="line"><a name="57">57</a></td><td class="hits"></td><td class="code">    &#39;init_console&#39;, </td></tr><tr class="noCover"><td class="line"><a name="58">58</a></td><td class="hits"></td><td class="code">    &#39;init_syslog_logging&#39;,</td></tr><tr class="noCover"><td class="line"><a name="59">59</a></td><td class="hits"></td><td class="code">    &#39;init_syslog&#39;,</td></tr><tr class="noCover"><td class="line"><a name="60">60</a></td><td class="hits"></td><td class="code">    &#39;set_logging_verbosity&#39;, </td></tr><tr class="noCover"><td class="line"><a name="61">61</a></td><td class="hits"></td><td class="code">    &#39;set_verbosity&#39;,</td></tr><tr class="noCover"><td class="line"><a name="62">62</a></td><td class="hits"></td><td class="code">    &#39;trace&#39;,</td></tr><tr class="noCover"><td class="line"><a name="63">63</a></td><td class="hits"></td><td class="code">]</td></tr>
+<tr class="noCover"><td class="line"><a name="1">1</a></td><td class="hits"></td><td class="code"></td></tr><tr class="coverFull" data-html-tooltip="Covered at least once"><td class="line"><a name="2">2</a></td><td class="hits">1</td><td class="code">from warnings import warn</td></tr><tr class="noCover"><td class="line"><a name="3">3</a></td><td class="hits"></td><td class="code"></td></tr><tr class="coverFull" data-html-tooltip="Covered at least once"><td class="line"><a name="4">4</a></td><td class="hits">1</td><td class="code">from uologging.cli import add_verbosity_flag, get_default_parser</td></tr><tr class="coverFull" data-html-tooltip="Covered at least once"><td class="line"><a name="5">5</a></td><td class="hits">1</td><td class="code">from uologging.downloads import DownloadTracer</td></tr><tr class="coverFull" data-html-tooltip="Covered at least once"><td class="line"><a name="6">6</a></td><td class="hits">1</td><td class="code">from uologging.performance import trace</td></tr><tr class="coverFull" data-html-tooltip="Covered at least once"><td class="line"><a name="7">7</a></td><td class="hits">1</td><td class="code">from uologging.uologging import init_console, init_syslog, set_verbosity</td></tr><tr class="noCover"><td class="line"><a name="8">8</a></td><td class="hits"></td><td class="code"></td></tr><tr class="noCover"><td class="line"><a name="9">9</a></td><td class="hits"></td><td class="code"></td></tr><tr class="coverFull" data-html-tooltip="Covered at least once"><td class="line"><a name="10">10</a></td><td class="hits">1</td><td class="code">def function_renamed(function, old_name):</td></tr><tr class="noCover"><td class="line"><a name="11">11</a></td><td class="hits"></td><td class="code">    &#34;&#34;&#34;Want to change the name of some function in your python library?</td></tr><tr class="noCover"><td class="line"><a name="12">12</a></td><td class="hits"></td><td class="code">    But you don&#39;t want to break your users&#39; code?</td></tr><tr class="noCover"><td class="line"><a name="13">13</a></td><td class="hits"></td><td class="code"></td></tr><tr class="noCover"><td class="line"><a name="14">14</a></td><td class="hits"></td><td class="code">    This function will wrap any function with a deprecated alias.</td></tr><tr class="noCover"><td class="line"><a name="15">15</a></td><td class="hits"></td><td class="code">    </td></tr><tr class="noCover"><td class="line"><a name="16">16</a></td><td class="hits"></td><td class="code">    Example:</td></tr><tr class="noCover"><td class="line"><a name="17">17</a></td><td class="hits"></td><td class="code"></td></tr><tr class="noCover"><td class="line"><a name="18">18</a></td><td class="hits"></td><td class="code">    Imagine you have the &#39;say_hello&#39; function in your library.</td></tr><tr class="noCover"><td class="line"><a name="19">19</a></td><td class="hits"></td><td class="code"></td></tr><tr class="noCover"><td class="line"><a name="20">20</a></td><td class="hits"></td><td class="code">        &gt;&gt;&gt; def say_hello():</td></tr><tr class="noCover"><td class="line"><a name="21">21</a></td><td class="hits"></td><td class="code">        ...     print(&#39;Hello, world!&#39;)</td></tr><tr class="noCover"><td class="line"><a name="22">22</a></td><td class="hits"></td><td class="code">    </td></tr><tr class="noCover"><td class="line"><a name="23">23</a></td><td class="hits"></td><td class="code">    You want to change the name to &#39;hello,&#39; and so you do!</td></tr><tr class="noCover"><td class="line"><a name="24">24</a></td><td class="hits"></td><td class="code"></td></tr><tr class="noCover"><td class="line"><a name="25">25</a></td><td class="hits"></td><td class="code">        &gt;&gt;&gt; def hello():</td></tr><tr class="noCover"><td class="line"><a name="26">26</a></td><td class="hits"></td><td class="code">        ...     print(&#39;Hello, world!&#39;)</td></tr><tr class="noCover"><td class="line"><a name="27">27</a></td><td class="hits"></td><td class="code"></td></tr><tr class="noCover"><td class="line"><a name="28">28</a></td><td class="hits"></td><td class="code">    But, you don&#39;t want to break your users&#39; code.</td></tr><tr class="noCover"><td class="line"><a name="29">29</a></td><td class="hits"></td><td class="code"></td></tr><tr class="noCover"><td class="line"><a name="30">30</a></td><td class="hits"></td><td class="code">    </td></tr><tr class="noCover"><td class="line"><a name="31">31</a></td><td class="hits"></td><td class="code">        &gt;&gt;&gt; say_hello &#61; function_renamed(hello, &#39;say_hello&#39;)</td></tr><tr class="noCover"><td class="line"><a name="32">32</a></td><td class="hits"></td><td class="code">        &gt;&gt;&gt; __all__ &#61; [&#39;hello&#39;, &#39;say_hello&#39;]</td></tr><tr class="noCover"><td class="line"><a name="33">33</a></td><td class="hits"></td><td class="code"></td></tr><tr class="noCover"><td class="line"><a name="34">34</a></td><td class="hits"></td><td class="code"></td></tr><tr class="noCover"><td class="line"><a name="35">35</a></td><td class="hits"></td><td class="code">    Args:</td></tr><tr class="noCover"><td class="line"><a name="36">36</a></td><td class="hits"></td><td class="code">        new_function (_type_): _description_</td></tr><tr class="noCover"><td class="line"><a name="37">37</a></td><td class="hits"></td><td class="code">        deprecated_function_name (_type_): _description_</td></tr><tr class="noCover"><td class="line"><a name="38">38</a></td><td class="hits"></td><td class="code">    &#34;&#34;&#34;</td></tr><tr class="coverFull" data-html-tooltip="Covered at least once"><td class="line"><a name="39">39</a></td><td class="hits">1</td><td class="code">    def deprecated_function(*args, **kwargs):</td></tr><tr class="coverNone" data-html-tooltip="Not covered"><td class="line"><a name="40">40</a></td><td class="hits">0</td><td class="code">        deprecation_warning &#61; f&#39;{old_name}() is deprecated (we plan to remove it in next major-version). Please use {function.__name__}() instead.&#39;</td></tr><tr class="coverNone" data-html-tooltip="Not covered"><td class="line"><a name="41">41</a></td><td class="hits">0</td><td class="code">        warn(deprecation_warning, DeprecationWarning, stacklevel&#61;2)</td></tr><tr class="noCover"><td class="line"><a name="42">42</a></td><td class="hits"></td><td class="code">        # NOW, only after warning, pass on to the underlying function</td></tr><tr class="coverNone" data-html-tooltip="Not covered"><td class="line"><a name="43">43</a></td><td class="hits">0</td><td class="code">        function(*args, **kwargs)</td></tr><tr class="coverFull" data-html-tooltip="Covered at least once"><td class="line"><a name="44">44</a></td><td class="hits">1</td><td class="code">    return deprecated_function</td></tr><tr class="noCover"><td class="line"><a name="45">45</a></td><td class="hits"></td><td class="code"></td></tr><tr class="noCover"><td class="line"><a name="46">46</a></td><td class="hits"></td><td class="code"></td></tr><tr class="coverFull" data-html-tooltip="Covered at least once"><td class="line"><a name="47">47</a></td><td class="hits">1</td><td class="code">init_console_logging &#61; function_renamed(init_console, old_name&#61;&#39;init_console_logging&#39;)</td></tr><tr class="coverFull" data-html-tooltip="Covered at least once"><td class="line"><a name="48">48</a></td><td class="hits">1</td><td class="code">init_syslog_logging &#61; function_renamed(init_syslog, old_name&#61;&#39;init_syslog_logging&#39;)</td></tr><tr class="coverFull" data-html-tooltip="Covered at least once"><td class="line"><a name="49">49</a></td><td class="hits">1</td><td class="code">set_logging_verbosity &#61; function_renamed(set_verbosity, old_name&#61;&#39;set_logging_verbosity&#39;)</td></tr><tr class="noCover"><td class="line"><a name="50">50</a></td><td class="hits"></td><td class="code"></td></tr><tr class="coverFull" data-html-tooltip="Covered at least once"><td class="line"><a name="51">51</a></td><td class="hits">1</td><td class="code">__version__ &#61; &#39;0.8.1&#39;</td></tr><tr class="coverFull" data-html-tooltip="Covered at least once"><td class="line"><a name="52">52</a></td><td class="hits">1</td><td class="code">__all__ &#61; [</td></tr><tr class="noCover"><td class="line"><a name="53">53</a></td><td class="hits"></td><td class="code">    &#39;add_verbosity_flag&#39;, </td></tr><tr class="noCover"><td class="line"><a name="54">54</a></td><td class="hits"></td><td class="code">    &#39;DownloadTracer&#39;,</td></tr><tr class="noCover"><td class="line"><a name="55">55</a></td><td class="hits"></td><td class="code">    &#39;get_default_parser&#39;, </td></tr><tr class="noCover"><td class="line"><a name="56">56</a></td><td class="hits"></td><td class="code">    &#39;init_console_logging&#39;, </td></tr><tr class="noCover"><td class="line"><a name="57">57</a></td><td class="hits"></td><td class="code">    &#39;init_console&#39;, </td></tr><tr class="noCover"><td class="line"><a name="58">58</a></td><td class="hits"></td><td class="code">    &#39;init_syslog_logging&#39;,</td></tr><tr class="noCover"><td class="line"><a name="59">59</a></td><td class="hits"></td><td class="code">    &#39;init_syslog&#39;,</td></tr><tr class="noCover"><td class="line"><a name="60">60</a></td><td class="hits"></td><td class="code">    &#39;set_logging_verbosity&#39;, </td></tr><tr class="noCover"><td class="line"><a name="61">61</a></td><td class="hits"></td><td class="code">    &#39;set_verbosity&#39;,</td></tr><tr class="noCover"><td class="line"><a name="62">62</a></td><td class="hits"></td><td class="code">    &#39;trace&#39;,</td></tr><tr class="noCover"><td class="line"><a name="63">63</a></td><td class="hits"></td><td class="code">]</td></tr>
```

### Comparing `uologging-0.8.0/coverage/src_uologging_cli.py.zip` & `uologging-0.8.1/coverage/src_uologging_cli.py.zip`

 * *Files 5% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 1292 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx     8770 bl defN 23-Dec-13 13:59 src_uologging_cli.py
+?rw-r--r--  2.0 unx     8770 bl defN 24-Apr-10 14:36 src_uologging_cli.py
 1 file, 8770 bytes uncompressed, 1138 bytes compressed:  87.0%
```

### Comparing `uologging-0.8.0/coverage/src_uologging_downloads.py.zip` & `uologging-0.8.1/coverage/src_uologging_downloads.py.zip`

 * *Files 16% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 1643 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    10763 bl defN 23-Dec-13 13:59 src_uologging_downloads.py
+?rw-r--r--  2.0 unx    10763 bl defN 24-Apr-10 14:36 src_uologging_downloads.py
 1 file, 10763 bytes uncompressed, 1477 bytes compressed:  86.3%
```

### Comparing `uologging-0.8.0/coverage/src_uologging_performance.py.zip` & `uologging-0.8.1/coverage/src_uologging_performance.py.zip`

 * *Files 7% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 1904 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    13899 bl defN 23-Dec-13 13:59 src_uologging_performance.py
+?rw-r--r--  2.0 unx    13899 bl defN 24-Apr-10 14:36 src_uologging_performance.py
 1 file, 13899 bytes uncompressed, 1734 bytes compressed:  87.5%
```

### Comparing `uologging-0.8.0/coverage/src_uologging_uologging.py.zip` & `uologging-0.8.1/coverage/src_uologging_uologging.py.zip`

 * *Files 4% similar despite different names*

#### zipinfo {}

```diff
@@ -1,3 +1,3 @@
 Zip file size: 2035 bytes, number of entries: 1
-?rw-rw-r--  2.0 unx    15124 bl defN 23-Dec-13 13:59 src_uologging_uologging.py
+?rw-r--r--  2.0 unx    15124 bl defN 24-Apr-10 14:36 src_uologging_uologging.py
 1 file, 15124 bytes uncompressed, 1869 bytes compressed:  87.6%
```

### Comparing `uologging-0.8.0/docs/README.md` & `uologging-0.8.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `uologging-0.8.0/docs/changelog.md` & `uologging-0.8.1/docs/changelog.md`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,22 @@
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 > ℹ Adhering to 'Keep a Changelog' began at version [[0.8.0]](#080---2023-03-05)
 
 ## [Unreleased]
 
-## [0.8.0] - 2023-03-05
+## [0.8.1] - Apr 8, 2024
+
+### Changed
+
+* Internal-only change: Update CICD workflows to use [`ntsjenkins` shared library](https://confluence.uoregon.edu/x/TQRaGw)
+
+
+## [0.8.0] - March 5, 2023
 
 ### Added
 
 * `uologging.DownloadTracer`
     * See [examples of "Tracing Concurrent Downloads" in the User Guide](./user-guide.md#tracing-concurrent-downloads)
 * Emit a `DeprecationWarning` when a deprecated alias is used.
```

### Comparing `uologging-0.8.0/docs/development.md` & `uologging-0.8.1/docs/development.md`

 * *Files identical despite different names*

### Comparing `uologging-0.8.0/docs/package-deployment.md` & `uologging-0.8.1/docs/package-deployment.md`

 * *Files identical despite different names*

### Comparing `uologging-0.8.0/src/uologging/__init__.py` & `uologging-0.8.1/src/uologging/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     return deprecated_function
 
 
 init_console_logging = function_renamed(init_console, old_name='init_console_logging')
 init_syslog_logging = function_renamed(init_syslog, old_name='init_syslog_logging')
 set_logging_verbosity = function_renamed(set_verbosity, old_name='set_logging_verbosity')
 
-__version__ = '0.8.0'
+__version__ = '0.8.1'
 __all__ = [
     'add_verbosity_flag', 
     'DownloadTracer',
     'get_default_parser', 
     'init_console_logging', 
     'init_console', 
     'init_syslog_logging',
```

### Comparing `uologging-0.8.0/src/uologging/cli.py` & `uologging-0.8.1/src/uologging/cli.py`

 * *Files identical despite different names*

### Comparing `uologging-0.8.0/src/uologging/downloads.py` & `uologging-0.8.1/src/uologging/downloads.py`

 * *Files identical despite different names*

### Comparing `uologging-0.8.0/src/uologging/performance.py` & `uologging-0.8.1/src/uologging/performance.py`

 * *Files identical despite different names*

### Comparing `uologging-0.8.0/src/uologging/uologging.py` & `uologging-0.8.1/src/uologging/uologging.py`

 * *Files identical despite different names*

### Comparing `uologging-0.8.0/tests/test_downloads.py` & `uologging-0.8.1/tests/test_downloads.py`

 * *Files identical despite different names*

### Comparing `uologging-0.8.0/tests/test_performance.py` & `uologging-0.8.1/tests/test_performance.py`

 * *Files identical despite different names*

### Comparing `uologging-0.8.0/tests/test_uologging.py` & `uologging-0.8.1/tests/test_uologging.py`

 * *Files identical despite different names*

### Comparing `uologging-0.8.0/.gitignore` & `uologging-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `uologging-0.8.0/hatch.toml` & `uologging-0.8.1/hatch.toml`

 * *Files identical despite different names*

### Comparing `uologging-0.8.0/hatch_build.py` & `uologging-0.8.1/hatch_build.py`

 * *Files identical despite different names*

### Comparing `uologging-0.8.0/pyproject.toml` & `uologging-0.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `uologging-0.8.0/docs/user-guide.md` & `uologging-0.8.1/docs/user-guide.md`

 * *Files identical despite different names*

### Comparing `uologging-0.8.0/PKG-INFO` & `uologging-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: uologging
-Version: 0.8.0
+Version: 0.8.1
 Summary: Auto-Configuration solution for Python built-in logging.
 Author-email: University of Oregon <ntsjenkins@uoregon.edu>
 License-Expression: MIT
 Keywords: NTS,UO
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

