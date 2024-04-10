# Comparing `tmp/widget_bandsplot-0.6.4.tar.gz` & `tmp/widget_bandsplot-0.7.0.tar.gz`

## Comparing `widget_bandsplot-0.6.4.tar` & `widget_bandsplot-0.7.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 widget_bandsplot-0.6.4/src/widget_bandsplot/__init__.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 widget_bandsplot-0.6.4/src/widget_bandsplot/static/widget.css
--rw-r--r--   0        0        0   539253 2020-02-02 00:00:00.000000 widget_bandsplot-0.6.4/src/widget_bandsplot/static/widget.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 widget_bandsplot-0.6.4/.gitignore
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 widget_bandsplot-0.6.4/README.md
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 widget_bandsplot-0.6.4/pyproject.toml
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 widget_bandsplot-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 widget_bandsplot-0.7.0/src/widget_bandsplot/__init__.py
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 widget_bandsplot-0.7.0/src/widget_bandsplot/static/widget.css
+-rw-r--r--   0        0        0   539001 2020-02-02 00:00:00.000000 widget_bandsplot-0.7.0/src/widget_bandsplot/static/widget.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 widget_bandsplot-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 widget_bandsplot-0.7.0/README.md
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 widget_bandsplot-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 widget_bandsplot-0.7.0/PKG-INFO
```

### Comparing `widget_bandsplot-0.6.4/src/widget_bandsplot/static/widget.css` & `widget_bandsplot-0.7.0/src/widget_bandsplot/static/widget.css`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-.bands-widget-all{width:100%;display:flex;flex-direction:column;align-items:center;text-align:center}.plots-container{width:100%;display:flex;align-items:center;justify-content:center}.bands-plot{width:60%;height:450px;float:left}.bands-plot-single{width:95%;height:450px}.dos-plot{width:40%;height:450px;float:right}.dos-plot-single{width:95%;height:300px}.bands-path-input{align-self:stretch;margin-bottom:2px}.span-label{width:10%;font-size:medium;font-weight:700}.bands-input{width:70%;max-width:700px;font-size:medium;font-size:bold}.button{border-radius:4px;border:1px solid #3560a0;background-color:#3560a0;color:#fff;margin:3px 4px;font-size:medium;cursor:pointer;height:25px;padding:0 4px}.button-white{border-radius:4px;border:1px solid #3560a0;background:#fff;color:#3560a0;margin:3px 4px;height:25px;font-size:medium;cursor:pointer;padding:0 4px}.button:hover{filter:brightness(90%)}.drag-button-container{width:fit-content;font-size:medium;margin:3px 4px;height:25px;overflow:hidden;display:flex;flex-direction:row;flex-wrap:no-wrap;align-items:center;border:1px solid rgb(88,88,88);border-radius:4px}.drag-radio-buttons{display:flex;flex-direction:row;flex-wrap:no-wrap;align-items:center;color:#3560a0}.drag-radio-buttons input{display:none}.drag-radio-buttons label{font-family:sans-serif;border-right:1px solid #ccc;cursor:pointer;transition:all .3s;background:#fff;padding:10px 4px}.drag-radio-buttons label:last-of-type{border-right:0}.drag-radio-buttons label:hover{filter:brightness(90%)}.drag-radio-buttons input:checked+label{background:#3560a0;color:#fff}.band-widget-buttons{display:flex;flex-wrap:wrap;justify-content:center}
+.bands-widget-all{width:100%;display:flex;flex-direction:column;align-items:center;text-align:center}.plots-container{width:100%;display:flex;align-items:center;justify-content:center}.bands-plot{width:60%;height:450px;float:left}.bands-plot-single{width:95%;height:450px}.dos-plot{width:40%;height:450px;float:right}.dos-plot-single{width:95%;height:300px}.bands-path-input{align-self:stretch;margin-bottom:2px}.span-label{width:10%;font-size:medium;font-weight:700}.bands-input{width:70%;max-width:700px;font-size:medium;font-size:bold}.button{border-radius:4px;border:1px solid #3560a0;background-color:#3560a0;color:#fff;margin:3px 4px;font-size:medium;cursor:pointer;height:25px;padding:0 4px}.button-white{border-radius:4px;border:1px solid #3560a0;background:#fff;color:#3560a0;margin:3px 4px;height:25px;font-size:medium;cursor:pointer;padding:0 4px}.button:hover{filter:brightness(90%)}.drag-button-container{box-sizing:border-box;width:fit-content;font-size:medium;border:1px solid rgb(88,88,88);margin:3px 4px;height:25px;overflow:hidden;display:flex;flex-direction:row;flex-wrap:no-wrap;align-items:center;border-radius:4px}.drag-radio-buttons{display:flex;flex-direction:row;flex-wrap:no-wrap;align-items:center;color:#3560a0}.drag-radio-buttons input{display:none}.drag-radio-buttons label{font-family:sans-serif;border-right:1px solid #ccc;cursor:pointer;transition:all .3s;background:#fff;padding:10px 4px}.drag-radio-buttons label:last-of-type{border-right:0}.drag-radio-buttons label:hover{filter:brightness(90%)}.drag-radio-buttons input:checked+label{background:#3560a0;color:#fff}.band-widget-buttons{display:flex;flex-wrap:wrap;justify-content:center}
```

### Comparing `widget_bandsplot-0.6.4/src/widget_bandsplot/static/widget.js` & `widget_bandsplot-0.7.0/src/widget_bandsplot/static/widget.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,31 +1,31 @@
 var X_ = Object.create;
 var xm = Object.defineProperty;
 var q_ = Object.getOwnPropertyDescriptor;
 var Z_ = Object.getOwnPropertyNames;
-var G_ = Object.getPrototypeOf,
-    Q_ = Object.prototype.hasOwnProperty;
+var K_ = Object.getPrototypeOf,
+    G_ = Object.prototype.hasOwnProperty;
 var mr = (t, e) => () => (e || t((e = {
     exports: {}
 }).exports, e), e.exports);
-var K_ = (t, e, n, i) => {
+var Q_ = (t, e, n, i) => {
     if (e && typeof e == "object" || typeof e == "function")
-        for (let r of Z_(e)) !Q_.call(t, r) && r !== n && xm(t, r, {
+        for (let r of Z_(e)) !G_.call(t, r) && r !== n && xm(t, r, {
             get: () => e[r],
             enumerable: !(i = q_(e, r)) || i.enumerable
         });
     return t
 };
-var fa = (t, e, n) => (n = t != null ? X_(G_(t)) : {}, K_(e || !t || !t.__esModule ? xm(n, "default", {
+var da = (t, e, n) => (n = t != null ? X_(K_(t)) : {}, Q_(e || !t || !t.__esModule ? xm(n, "default", {
     value: t,
     enumerable: !0
 }) : n, t));
-var Dm = mr(Le => {
+var Mm = mr(Le => {
     "use strict";
-    var da = Symbol.for("react.element"),
+    var ha = Symbol.for("react.element"),
         J_ = Symbol.for("react.portal"),
         ew = Symbol.for("react.fragment"),
         tw = Symbol.for("react.strict_mode"),
         nw = Symbol.for("react.profiler"),
         iw = Symbol.for("react.provider"),
         rw = Symbol.for("react.context"),
         ow = Symbol.for("react.forward_ref"),
@@ -33,149 +33,149 @@
         aw = Symbol.for("react.memo"),
         lw = Symbol.for("react.lazy"),
         bm = Symbol.iterator;
 
     function uw(t) {
         return t === null || typeof t != "object" ? null : (t = bm && t[bm] || t["@@iterator"], typeof t == "function" ? t : null)
     }
-    var km = {
+    var Sm = {
             isMounted: function() {
                 return !1
             },
             enqueueForceUpdate: function() {},
             enqueueReplaceState: function() {},
             enqueueSetState: function() {}
         },
-        Sm = Object.assign,
+        km = Object.assign,
         Cm = {};
 
     function es(t, e, n) {
-        this.props = t, this.context = e, this.refs = Cm, this.updater = n || km
+        this.props = t, this.context = e, this.refs = Cm, this.updater = n || Sm
     }
     es.prototype.isReactComponent = {};
     es.prototype.setState = function(t, e) {
         if (typeof t != "object" && typeof t != "function" && t != null) throw Error("setState(...): takes an object of state variables to update or a function which returns an object of state variables.");
         this.updater.enqueueSetState(this, t, e, "setState")
     };
     es.prototype.forceUpdate = function(t) {
         this.updater.enqueueForceUpdate(this, t, "forceUpdate")
     };
 
     function Em() {}
     Em.prototype = es.prototype;
 
-    function Jf(t, e, n) {
-        this.props = t, this.context = e, this.refs = Cm, this.updater = n || km
+    function Qf(t, e, n) {
+        this.props = t, this.context = e, this.refs = Cm, this.updater = n || Sm
     }
-    var ed = Jf.prototype = new Em;
-    ed.constructor = Jf;
-    Sm(ed, es.prototype);
-    ed.isPureReactComponent = !0;
+    var Jf = Qf.prototype = new Em;
+    Jf.constructor = Qf;
+    km(Jf, es.prototype);
+    Jf.isPureReactComponent = !0;
     var _m = Array.isArray,
         Tm = Object.prototype.hasOwnProperty,
-        td = {
+        ed = {
             current: null
         },
-        Pm = {
+        Dm = {
             key: !0,
             ref: !0,
             __self: !0,
             __source: !0
         };
 
-    function Mm(t, e, n) {
+    function Pm(t, e, n) {
         var i, r = {},
             o = null,
             s = null;
         if (e != null)
-            for (i in e.ref !== void 0 && (s = e.ref), e.key !== void 0 && (o = "" + e.key), e) Tm.call(e, i) && !Pm.hasOwnProperty(i) && (r[i] = e[i]);
+            for (i in e.ref !== void 0 && (s = e.ref), e.key !== void 0 && (o = "" + e.key), e) Tm.call(e, i) && !Dm.hasOwnProperty(i) && (r[i] = e[i]);
         var a = arguments.length - 2;
         if (a === 1) r.children = n;
         else if (1 < a) {
             for (var l = Array(a), c = 0; c < a; c++) l[c] = arguments[c + 2];
             r.children = l
         }
         if (t && t.defaultProps)
             for (i in a = t.defaultProps, a) r[i] === void 0 && (r[i] = a[i]);
         return {
-            $$typeof: da,
+            $$typeof: ha,
             type: t,
             key: o,
             ref: s,
             props: r,
-            _owner: td.current
+            _owner: ed.current
         }
     }
 
     function cw(t, e) {
         return {
-            $$typeof: da,
+            $$typeof: ha,
             type: t.type,
             key: e,
             ref: t.ref,
             props: t.props,
             _owner: t._owner
         }
     }
 
-    function nd(t) {
-        return typeof t == "object" && t !== null && t.$$typeof === da
+    function td(t) {
+        return typeof t == "object" && t !== null && t.$$typeof === ha
     }
 
     function fw(t) {
         var e = {
             "=": "=0",
             ":": "=2"
         };
         return "$" + t.replace(/[=:]/g, function(n) {
             return e[n]
         })
     }
     var wm = /\/+/g;
 
-    function Kf(t, e) {
+    function Gf(t, e) {
         return typeof t == "object" && t !== null && t.key != null ? fw("" + t.key) : e.toString(36)
     }
 
-    function tu(t, e, n, i, r) {
+    function nu(t, e, n, i, r) {
         var o = typeof t;
         (o === "undefined" || o === "boolean") && (t = null);
         var s = !1;
         if (t === null) s = !0;
         else switch (o) {
             case "string":
             case "number":
                 s = !0;
                 break;
             case "object":
                 switch (t.$$typeof) {
-                    case da:
+                    case ha:
                     case J_:
                         s = !0
                 }
         }
-        if (s) return s = t, r = r(s), t = i === "" ? "." + Kf(s, 0) : i, _m(r) ? (n = "", t != null && (n = t.replace(wm, "$&/") + "/"), tu(r, e, n, "", function(c) {
+        if (s) return s = t, r = r(s), t = i === "" ? "." + Gf(s, 0) : i, _m(r) ? (n = "", t != null && (n = t.replace(wm, "$&/") + "/"), nu(r, e, n, "", function(c) {
             return c
-        })) : r != null && (nd(r) && (r = cw(r, n + (!r.key || s && s.key === r.key ? "" : ("" + r.key).replace(wm, "$&/") + "/") + t)), e.push(r)), 1;
+        })) : r != null && (td(r) && (r = cw(r, n + (!r.key || s && s.key === r.key ? "" : ("" + r.key).replace(wm, "$&/") + "/") + t)), e.push(r)), 1;
         if (s = 0, i = i === "" ? "." : i + ":", _m(t))
             for (var a = 0; a < t.length; a++) {
                 o = t[a];
-                var l = i + Kf(o, a);
-                s += tu(o, e, n, l, r)
+                var l = i + Gf(o, a);
+                s += nu(o, e, n, l, r)
             } else if (l = uw(t), typeof l == "function")
-                for (t = l.call(t), a = 0; !(o = t.next()).done;) o = o.value, l = i + Kf(o, a++), s += tu(o, e, n, l, r);
+                for (t = l.call(t), a = 0; !(o = t.next()).done;) o = o.value, l = i + Gf(o, a++), s += nu(o, e, n, l, r);
             else if (o === "object") throw e = String(t), Error("Objects are not valid as a React child (found: " + (e === "[object Object]" ? "object with keys {" + Object.keys(t).join(", ") + "}" : e) + "). If you meant to render a collection of children, use an array instead.");
         return s
     }
 
-    function eu(t, e, n) {
+    function tu(t, e, n) {
         if (t == null) return t;
         var i = [],
             r = 0;
-        return tu(t, i, "", "", function(o) {
+        return nu(t, i, "", "", function(o) {
             return e.call(n, o, r++)
         }), i
     }
 
     function dw(t) {
         if (t._status === -1) {
             var e = t._result;
@@ -187,71 +187,71 @@
         }
         if (t._status === 1) return t._result.default;
         throw t._result
     }
     var en = {
             current: null
         },
-        nu = {
+        iu = {
             transition: null
         },
         hw = {
             ReactCurrentDispatcher: en,
-            ReactCurrentBatchConfig: nu,
-            ReactCurrentOwner: td
+            ReactCurrentBatchConfig: iu,
+            ReactCurrentOwner: ed
         };
     Le.Children = {
-        map: eu,
+        map: tu,
         forEach: function(t, e, n) {
-            eu(t, function() {
+            tu(t, function() {
                 e.apply(this, arguments)
             }, n)
         },
         count: function(t) {
             var e = 0;
-            return eu(t, function() {
+            return tu(t, function() {
                 e++
             }), e
         },
         toArray: function(t) {
-            return eu(t, function(e) {
+            return tu(t, function(e) {
                 return e
             }) || []
         },
         only: function(t) {
-            if (!nd(t)) throw Error("React.Children.only expected to receive a single React element child.");
+            if (!td(t)) throw Error("React.Children.only expected to receive a single React element child.");
             return t
         }
     };
     Le.Component = es;
     Le.Fragment = ew;
     Le.Profiler = nw;
-    Le.PureComponent = Jf;
+    Le.PureComponent = Qf;
     Le.StrictMode = tw;
     Le.Suspense = sw;
     Le.__SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED = hw;
     Le.cloneElement = function(t, e, n) {
         if (t == null) throw Error("React.cloneElement(...): The argument must be a React element, but you passed " + t + ".");
-        var i = Sm({}, t.props),
+        var i = km({}, t.props),
             r = t.key,
             o = t.ref,
             s = t._owner;
         if (e != null) {
-            if (e.ref !== void 0 && (o = e.ref, s = td.current), e.key !== void 0 && (r = "" + e.key), t.type && t.type.defaultProps) var a = t.type.defaultProps;
-            for (l in e) Tm.call(e, l) && !Pm.hasOwnProperty(l) && (i[l] = e[l] === void 0 && a !== void 0 ? a[l] : e[l])
+            if (e.ref !== void 0 && (o = e.ref, s = ed.current), e.key !== void 0 && (r = "" + e.key), t.type && t.type.defaultProps) var a = t.type.defaultProps;
+            for (l in e) Tm.call(e, l) && !Dm.hasOwnProperty(l) && (i[l] = e[l] === void 0 && a !== void 0 ? a[l] : e[l])
         }
         var l = arguments.length - 2;
         if (l === 1) i.children = n;
         else if (1 < l) {
             a = Array(l);
             for (var c = 0; c < l; c++) a[c] = arguments[c + 2];
             i.children = a
         }
         return {
-            $$typeof: da,
+            $$typeof: ha,
             type: t.type,
             key: r,
             ref: o,
             props: i,
             _owner: s
         }
     };
@@ -266,31 +266,31 @@
             _defaultValue: null,
             _globalName: null
         }, t.Provider = {
             $$typeof: iw,
             _context: t
         }, t.Consumer = t
     };
-    Le.createElement = Mm;
+    Le.createElement = Pm;
     Le.createFactory = function(t) {
-        var e = Mm.bind(null, t);
+        var e = Pm.bind(null, t);
         return e.type = t, e
     };
     Le.createRef = function() {
         return {
             current: null
         }
     };
     Le.forwardRef = function(t) {
         return {
             $$typeof: ow,
             render: t
         }
     };
-    Le.isValidElement = nd;
+    Le.isValidElement = td;
     Le.lazy = function(t) {
         return {
             $$typeof: lw,
             _payload: {
                 _status: -1,
                 _result: t
             },
@@ -301,20 +301,20 @@
         return {
             $$typeof: aw,
             type: t,
             compare: e === void 0 ? null : e
         }
     };
     Le.startTransition = function(t) {
-        var e = nu.transition;
-        nu.transition = {};
+        var e = iu.transition;
+        iu.transition = {};
         try {
             t()
         } finally {
-            nu.transition = e
+            iu.transition = e
         }
     };
     Le.unstable_act = function() {
         throw Error("act(...) is not supported in production builds of React.")
     };
     Le.useCallback = function(t, e) {
         return en.current.useCallback(t, e)
@@ -357,170 +357,170 @@
         return en.current.useSyncExternalStore(t, e, n)
     };
     Le.useTransition = function() {
         return en.current.useTransition()
     };
     Le.version = "18.2.0"
 });
-var ha = mr((QM, Om) => {
+var pa = mr((ZP, Om) => {
     "use strict";
-    Om.exports = Dm()
+    Om.exports = Mm()
 });
 var Bm = mr(Je => {
     "use strict";
 
-    function sd(t, e) {
+    function od(t, e) {
         var n = t.length;
         t.push(e);
         e: for (; 0 < n;) {
             var i = n - 1 >>> 1,
                 r = t[i];
-            if (0 < iu(r, e)) t[i] = e, t[n] = r, n = i;
+            if (0 < ru(r, e)) t[i] = e, t[n] = r, n = i;
             else break e
         }
     }
 
     function ti(t) {
         return t.length === 0 ? null : t[0]
     }
 
-    function ou(t) {
+    function su(t) {
         if (t.length === 0) return null;
         var e = t[0],
             n = t.pop();
         if (n !== e) {
             t[0] = n;
             e: for (var i = 0, r = t.length, o = r >>> 1; i < o;) {
                 var s = 2 * (i + 1) - 1,
                     a = t[s],
                     l = s + 1,
                     c = t[l];
-                if (0 > iu(a, n)) l < r && 0 > iu(c, a) ? (t[i] = c, t[l] = n, i = l) : (t[i] = a, t[s] = n, i = s);
-                else if (l < r && 0 > iu(c, n)) t[i] = c, t[l] = n, i = l;
+                if (0 > ru(a, n)) l < r && 0 > ru(c, a) ? (t[i] = c, t[l] = n, i = l) : (t[i] = a, t[s] = n, i = s);
+                else if (l < r && 0 > ru(c, n)) t[i] = c, t[l] = n, i = l;
                 else break e
             }
         }
         return e
     }
 
-    function iu(t, e) {
+    function ru(t, e) {
         var n = t.sortIndex - e.sortIndex;
         return n !== 0 ? n : t.id - e.id
     }
     typeof performance == "object" && typeof performance.now == "function" ? (Am = performance, Je.unstable_now = function() {
         return Am.now()
-    }) : (id = Date, Lm = id.now(), Je.unstable_now = function() {
-        return id.now() - Lm
+    }) : (nd = Date, Lm = nd.now(), Je.unstable_now = function() {
+        return nd.now() - Lm
     });
-    var Am, id, Lm, vi = [],
+    var Am, nd, Lm, vi = [],
         yr = [],
         pw = 1,
         Vn = null,
         qt = 3,
-        su = !1,
+        au = !1,
         co = !1,
-        ga = !1,
+        ma = !1,
         Nm = typeof setTimeout == "function" ? setTimeout : null,
         zm = typeof clearTimeout == "function" ? clearTimeout : null,
         Rm = typeof setImmediate < "u" ? setImmediate : null;
     typeof navigator < "u" && navigator.scheduling !== void 0 && navigator.scheduling.isInputPending !== void 0 && navigator.scheduling.isInputPending.bind(navigator.scheduling);
 
-    function ad(t) {
+    function sd(t) {
         for (var e = ti(yr); e !== null;) {
-            if (e.callback === null) ou(yr);
-            else if (e.startTime <= t) ou(yr), e.sortIndex = e.expirationTime, sd(vi, e);
+            if (e.callback === null) su(yr);
+            else if (e.startTime <= t) su(yr), e.sortIndex = e.expirationTime, od(vi, e);
             else break;
             e = ti(yr)
         }
     }
 
-    function ld(t) {
-        if (ga = !1, ad(t), !co)
-            if (ti(vi) !== null) co = !0, cd(ud);
+    function ad(t) {
+        if (ma = !1, sd(t), !co)
+            if (ti(vi) !== null) co = !0, ud(ld);
             else {
                 var e = ti(yr);
-                e !== null && fd(ld, e.startTime - t)
+                e !== null && cd(ad, e.startTime - t)
             }
     }
 
-    function ud(t, e) {
-        co = !1, ga && (ga = !1, zm(ma), ma = -1), su = !0;
+    function ld(t, e) {
+        co = !1, ma && (ma = !1, zm(ya), ya = -1), au = !0;
         var n = qt;
         try {
-            for (ad(e), Vn = ti(vi); Vn !== null && (!(Vn.expirationTime > e) || t && !Hm());) {
+            for (sd(e), Vn = ti(vi); Vn !== null && (!(Vn.expirationTime > e) || t && !Hm());) {
                 var i = Vn.callback;
                 if (typeof i == "function") {
                     Vn.callback = null, qt = Vn.priorityLevel;
                     var r = i(Vn.expirationTime <= e);
-                    e = Je.unstable_now(), typeof r == "function" ? Vn.callback = r : Vn === ti(vi) && ou(vi), ad(e)
-                } else ou(vi);
+                    e = Je.unstable_now(), typeof r == "function" ? Vn.callback = r : Vn === ti(vi) && su(vi), sd(e)
+                } else su(vi);
                 Vn = ti(vi)
             }
             if (Vn !== null) var o = !0;
             else {
                 var s = ti(yr);
-                s !== null && fd(ld, s.startTime - e), o = !1
+                s !== null && cd(ad, s.startTime - e), o = !1
             }
             return o
         } finally {
-            Vn = null, qt = n, su = !1
+            Vn = null, qt = n, au = !1
         }
     }
-    var au = !1,
-        ru = null,
-        ma = -1,
+    var lu = !1,
+        ou = null,
+        ya = -1,
         Fm = 5,
         jm = -1;
 
     function Hm() {
         return !(Je.unstable_now() - jm < Fm)
     }
 
-    function rd() {
-        if (ru !== null) {
+    function id() {
+        if (ou !== null) {
             var t = Je.unstable_now();
             jm = t;
             var e = !0;
             try {
-                e = ru(!0, t)
+                e = ou(!0, t)
             } finally {
-                e ? pa() : (au = !1, ru = null)
+                e ? ga() : (lu = !1, ou = null)
             }
-        } else au = !1
+        } else lu = !1
     }
-    var pa;
-    typeof Rm == "function" ? pa = function() {
-        Rm(rd)
-    } : typeof MessageChannel < "u" ? (od = new MessageChannel, Im = od.port2, od.port1.onmessage = rd, pa = function() {
+    var ga;
+    typeof Rm == "function" ? ga = function() {
+        Rm(id)
+    } : typeof MessageChannel < "u" ? (rd = new MessageChannel, Im = rd.port2, rd.port1.onmessage = id, ga = function() {
         Im.postMessage(null)
-    }) : pa = function() {
-        Nm(rd, 0)
+    }) : ga = function() {
+        Nm(id, 0)
     };
-    var od, Im;
+    var rd, Im;
 
-    function cd(t) {
-        ru = t, au || (au = !0, pa())
+    function ud(t) {
+        ou = t, lu || (lu = !0, ga())
     }
 
-    function fd(t, e) {
-        ma = Nm(function() {
+    function cd(t, e) {
+        ya = Nm(function() {
             t(Je.unstable_now())
         }, e)
     }
     Je.unstable_IdlePriority = 5;
     Je.unstable_ImmediatePriority = 1;
     Je.unstable_LowPriority = 4;
     Je.unstable_NormalPriority = 3;
     Je.unstable_Profiling = null;
     Je.unstable_UserBlockingPriority = 2;
     Je.unstable_cancelCallback = function(t) {
         t.callback = null
     };
     Je.unstable_continueExecution = function() {
-        co || su || (co = !0, cd(ud))
+        co || au || (co = !0, ud(ld))
     };
     Je.unstable_forceFrameRate = function(t) {
         0 > t || 125 < t ? console.error("forceFrameRate takes a positive int between 0 and 125, forcing frame rates higher than 125 fps is not supported") : Fm = 0 < t ? Math.floor(1e3 / t) : 5
     };
     Je.unstable_getCurrentPriorityLevel = function() {
         return qt
     };
@@ -587,15 +587,15 @@
         return r = n + r, t = {
             id: pw++,
             callback: e,
             priorityLevel: t,
             startTime: n,
             expirationTime: r,
             sortIndex: -1
-        }, n > i ? (t.sortIndex = n, sd(yr, t), ti(vi) === null && t === ti(yr) && (ga ? (zm(ma), ma = -1) : ga = !0, fd(ld, n - i))) : (t.sortIndex = r, sd(vi, t), co || su || (co = !0, cd(ud))), t
+        }, n > i ? (t.sortIndex = n, od(yr, t), ti(vi) === null && t === ti(yr) && (ma ? (zm(ya), ya = -1) : ma = !0, cd(ad, n - i))) : (t.sortIndex = r, od(vi, t), co || au || (co = !0, ud(ld))), t
     };
     Je.unstable_shouldYield = Hm;
     Je.unstable_wrapCallback = function(t) {
         var e = qt;
         return function() {
             var n = qt;
             qt = e;
@@ -603,45 +603,45 @@
                 return t.apply(this, arguments)
             } finally {
                 qt = n
             }
         }
     }
 });
-var Vm = mr((JM, Wm) => {
+var Vm = mr((GP, Wm) => {
     "use strict";
     Wm.exports = Bm()
 });
 var Zv = mr(Nn => {
     "use strict";
-    var G0 = ha(),
+    var K0 = pa(),
         Rn = Vm();
 
-    function ne(t) {
+    function te(t) {
         for (var e = "https://reactjs.org/docs/error-decoder.html?invariant=" + t, n = 1; n < arguments.length; n++) e += "&args[]=" + encodeURIComponent(arguments[n]);
         return "Minified React error #" + t + "; visit " + e + " for the full message or use the non-minified dev environment for full errors and additional helpful warnings."
     }
-    var Q0 = new Set,
-        Fa = {};
+    var G0 = new Set,
+        ja = {};
 
-    function So(t, e) {
+    function ko(t, e) {
         _s(t, e), _s(t + "Capture", e)
     }
 
     function _s(t, e) {
-        for (Fa[t] = e, t = 0; t < e.length; t++) Q0.add(e[t])
+        for (ja[t] = e, t = 0; t < e.length; t++) G0.add(e[t])
     }
     var qi = !(typeof window > "u" || typeof window.document > "u" || typeof window.document.createElement > "u"),
-        Rd = Object.prototype.hasOwnProperty,
+        Ld = Object.prototype.hasOwnProperty,
         gw = /^[:A-Z_a-z\u00C0-\u00D6\u00D8-\u00F6\u00F8-\u02FF\u0370-\u037D\u037F-\u1FFF\u200C-\u200D\u2070-\u218F\u2C00-\u2FEF\u3001-\uD7FF\uF900-\uFDCF\uFDF0-\uFFFD][:A-Z_a-z\u00C0-\u00D6\u00D8-\u00F6\u00F8-\u02FF\u0370-\u037D\u037F-\u1FFF\u200C-\u200D\u2070-\u218F\u2C00-\u2FEF\u3001-\uD7FF\uF900-\uFDCF\uFDF0-\uFFFD\-.0-9\u00B7\u0300-\u036F\u203F-\u2040]*$/,
         Um = {},
         $m = {};
 
     function mw(t) {
-        return Rd.call($m, t) ? !0 : Rd.call(Um, t) ? !1 : gw.test(t) ? $m[t] = !0 : (Um[t] = !0, !1)
+        return Ld.call($m, t) ? !0 : Ld.call(Um, t) ? !1 : gw.test(t) ? $m[t] = !0 : (Um[t] = !0, !1)
     }
 
     function yw(t, e, n, i) {
         if (n !== null && n.type === 0) return !1;
         switch (typeof e) {
             case "function":
             case "symbol":
@@ -702,85 +702,85 @@
     });
     ["cols", "rows", "size", "span"].forEach(function(t) {
         Wt[t] = new rn(t, 6, !1, t, null, !1, !1)
     });
     ["rowSpan", "start"].forEach(function(t) {
         Wt[t] = new rn(t, 5, !1, t.toLowerCase(), null, !1, !1)
     });
-    var Eh = /[\-:]([a-z])/g;
+    var Ch = /[\-:]([a-z])/g;
 
-    function Th(t) {
+    function Eh(t) {
         return t[1].toUpperCase()
     }
     "accent-height alignment-baseline arabic-form baseline-shift cap-height clip-path clip-rule color-interpolation color-interpolation-filters color-profile color-rendering dominant-baseline enable-background fill-opacity fill-rule flood-color flood-opacity font-family font-size font-size-adjust font-stretch font-style font-variant font-weight glyph-name glyph-orientation-horizontal glyph-orientation-vertical horiz-adv-x horiz-origin-x image-rendering letter-spacing lighting-color marker-end marker-mid marker-start overline-position overline-thickness paint-order panose-1 pointer-events rendering-intent shape-rendering stop-color stop-opacity strikethrough-position strikethrough-thickness stroke-dasharray stroke-dashoffset stroke-linecap stroke-linejoin stroke-miterlimit stroke-opacity stroke-width text-anchor text-decoration text-rendering underline-position underline-thickness unicode-bidi unicode-range units-per-em v-alphabetic v-hanging v-ideographic v-mathematical vector-effect vert-adv-y vert-origin-x vert-origin-y word-spacing writing-mode xmlns:xlink x-height".split(" ").forEach(function(t) {
-        var e = t.replace(Eh, Th);
+        var e = t.replace(Ch, Eh);
         Wt[e] = new rn(e, 1, !1, t, null, !1, !1)
     });
     "xlink:actuate xlink:arcrole xlink:role xlink:show xlink:title xlink:type".split(" ").forEach(function(t) {
-        var e = t.replace(Eh, Th);
+        var e = t.replace(Ch, Eh);
         Wt[e] = new rn(e, 1, !1, t, "http://www.w3.org/1999/xlink", !1, !1)
     });
     ["xml:base", "xml:lang", "xml:space"].forEach(function(t) {
-        var e = t.replace(Eh, Th);
+        var e = t.replace(Ch, Eh);
         Wt[e] = new rn(e, 1, !1, t, "http://www.w3.org/XML/1998/namespace", !1, !1)
     });
     ["tabIndex", "crossOrigin"].forEach(function(t) {
         Wt[t] = new rn(t, 1, !1, t.toLowerCase(), null, !1, !1)
     });
     Wt.xlinkHref = new rn("xlinkHref", 1, !1, "xlink:href", "http://www.w3.org/1999/xlink", !0, !1);
     ["src", "href", "action", "formAction"].forEach(function(t) {
         Wt[t] = new rn(t, 1, !1, t.toLowerCase(), null, !0, !0)
     });
 
-    function Ph(t, e, n, i) {
+    function Th(t, e, n, i) {
         var r = Wt.hasOwnProperty(e) ? Wt[e] : null;
         (r !== null ? r.type !== 0 : i || !(2 < e.length) || e[0] !== "o" && e[0] !== "O" || e[1] !== "n" && e[1] !== "N") && (vw(e, n, r, i) && (n = null), i || r === null ? mw(e) && (n === null ? t.removeAttribute(e) : t.setAttribute(e, "" + n)) : r.mustUseProperty ? t[r.propertyName] = n === null ? r.type === 3 ? !1 : "" : n : (e = r.attributeName, i = r.attributeNamespace, n === null ? t.removeAttribute(e) : (r = r.type, n = r === 3 || r === 4 && n === !0 ? "" : "" + n, i ? t.setAttributeNS(i, e, n) : t.setAttribute(e, n))))
     }
-    var Ki = G0.__SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED,
-        lu = Symbol.for("react.element"),
+    var Qi = K0.__SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED,
+        uu = Symbol.for("react.element"),
         is = Symbol.for("react.portal"),
         rs = Symbol.for("react.fragment"),
-        Mh = Symbol.for("react.strict_mode"),
-        Id = Symbol.for("react.profiler"),
-        K0 = Symbol.for("react.provider"),
+        Dh = Symbol.for("react.strict_mode"),
+        Rd = Symbol.for("react.profiler"),
+        Q0 = Symbol.for("react.provider"),
         J0 = Symbol.for("react.context"),
-        Dh = Symbol.for("react.forward_ref"),
-        Nd = Symbol.for("react.suspense"),
-        zd = Symbol.for("react.suspense_list"),
-        Oh = Symbol.for("react.memo"),
+        Ph = Symbol.for("react.forward_ref"),
+        Id = Symbol.for("react.suspense"),
+        Nd = Symbol.for("react.suspense_list"),
+        Mh = Symbol.for("react.memo"),
         xr = Symbol.for("react.lazy");
     Symbol.for("react.scope");
     Symbol.for("react.debug_trace_mode");
     var ey = Symbol.for("react.offscreen");
     Symbol.for("react.legacy_hidden");
     Symbol.for("react.cache");
     Symbol.for("react.tracing_marker");
     var Ym = Symbol.iterator;
 
-    function ya(t) {
+    function va(t) {
         return t === null || typeof t != "object" ? null : (t = Ym && t[Ym] || t["@@iterator"], typeof t == "function" ? t : null)
     }
     var ht = Object.assign,
-        dd;
+        fd;
 
-    function Ca(t) {
-        if (dd === void 0) try {
+    function Ea(t) {
+        if (fd === void 0) try {
             throw Error()
         } catch (n) {
             var e = n.stack.trim().match(/\n( *(at )?)/);
-            dd = e && e[1] || ""
+            fd = e && e[1] || ""
         }
         return `
-` + dd + t
+` + fd + t
     }
-    var hd = !1;
+    var dd = !1;
 
-    function pd(t, e) {
-        if (!t || hd) return "";
-        hd = !0;
+    function hd(t, e) {
+        if (!t || dd) return "";
+        dd = !0;
         var n = Error.prepareStackTrace;
         Error.prepareStackTrace = void 0;
         try {
             if (e)
                 if (e = function() {
                         throw Error()
                     }, Object.defineProperty(e.prototype, "props", {
@@ -824,74 +824,74 @@
 ` + r[s].replace(" at new ", " at ");
                                     return t.displayName && l.includes("<anonymous>") && (l = l.replace("<anonymous>", t.displayName)), l
                                 } while (1 <= s && 0 <= a);
                         break
                     }
             }
         } finally {
-            hd = !1, Error.prepareStackTrace = n
+            dd = !1, Error.prepareStackTrace = n
         }
-        return (t = t ? t.displayName || t.name : "") ? Ca(t) : ""
+        return (t = t ? t.displayName || t.name : "") ? Ea(t) : ""
     }
 
     function xw(t) {
         switch (t.tag) {
             case 5:
-                return Ca(t.type);
+                return Ea(t.type);
             case 16:
-                return Ca("Lazy");
+                return Ea("Lazy");
             case 13:
-                return Ca("Suspense");
+                return Ea("Suspense");
             case 19:
-                return Ca("SuspenseList");
+                return Ea("SuspenseList");
             case 0:
             case 2:
             case 15:
-                return t = pd(t.type, !1), t;
+                return t = hd(t.type, !1), t;
             case 11:
-                return t = pd(t.type.render, !1), t;
+                return t = hd(t.type.render, !1), t;
             case 1:
-                return t = pd(t.type, !0), t;
+                return t = hd(t.type, !0), t;
             default:
                 return ""
         }
     }
 
-    function Fd(t) {
+    function zd(t) {
         if (t == null) return null;
         if (typeof t == "function") return t.displayName || t.name || null;
         if (typeof t == "string") return t;
         switch (t) {
             case rs:
                 return "Fragment";
             case is:
                 return "Portal";
-            case Id:
+            case Rd:
                 return "Profiler";
-            case Mh:
+            case Dh:
                 return "StrictMode";
-            case Nd:
+            case Id:
                 return "Suspense";
-            case zd:
+            case Nd:
                 return "SuspenseList"
         }
         if (typeof t == "object") switch (t.$$typeof) {
             case J0:
                 return (t.displayName || "Context") + ".Consumer";
-            case K0:
+            case Q0:
                 return (t._context.displayName || "Context") + ".Provider";
-            case Dh:
+            case Ph:
                 var e = t.render;
                 return t = t.displayName, t || (t = e.displayName || e.name || "", t = t !== "" ? "ForwardRef(" + t + ")" : "ForwardRef"), t;
-            case Oh:
-                return e = t.displayName || null, e !== null ? e : Fd(t.type) || "Memo";
+            case Mh:
+                return e = t.displayName || null, e !== null ? e : zd(t.type) || "Memo";
             case xr:
                 e = t._payload, t = t._init;
                 try {
-                    return Fd(t(e))
+                    return zd(t(e))
                 } catch {}
         }
         return null
     }
 
     function bw(t) {
         var e = t.type;
@@ -913,17 +913,17 @@
             case 4:
                 return "Portal";
             case 3:
                 return "Root";
             case 6:
                 return "Text";
             case 16:
-                return Fd(e);
+                return zd(e);
             case 8:
-                return e === Mh ? "StrictMode" : "Mode";
+                return e === Dh ? "StrictMode" : "Mode";
             case 22:
                 return "Offscreen";
             case 12:
                 return "Profiler";
             case 21:
                 return "Scope";
             case 13:
@@ -990,37 +990,37 @@
                 stopTracking: function() {
                     t._valueTracker = null, delete t[e]
                 }
             }
         }
     }
 
-    function uu(t) {
+    function cu(t) {
         t._valueTracker || (t._valueTracker = _w(t))
     }
 
     function ny(t) {
         if (!t) return !1;
         var e = t._valueTracker;
         if (!e) return !0;
         var n = e.getValue(),
             i = "";
         return t && (i = ty(t) ? t.checked ? "true" : "false" : t.value), t = i, t !== n ? (e.setValue(t), !0) : !1
     }
 
-    function zu(t) {
+    function Fu(t) {
         if (t = t || (typeof document < "u" ? document : void 0), typeof t > "u") return null;
         try {
             return t.activeElement || t.body
         } catch {
             return t.body
         }
     }
 
-    function jd(t, e) {
+    function Fd(t, e) {
         var n = e.checked;
         return ht({}, e, {
             defaultChecked: void 0,
             defaultValue: void 0,
             value: void 0,
             checked: n ?? t._wrapperState.initialChecked
         })
@@ -1033,42 +1033,42 @@
             initialChecked: i,
             initialValue: n,
             controlled: e.type === "checkbox" || e.type === "radio" ? e.checked != null : e.value != null
         }
     }
 
     function iy(t, e) {
-        e = e.checked, e != null && Ph(t, "checked", e, !1)
+        e = e.checked, e != null && Th(t, "checked", e, !1)
     }
 
-    function Hd(t, e) {
+    function jd(t, e) {
         iy(t, e);
         var n = Lr(e.value),
             i = e.type;
         if (n != null) i === "number" ? (n === 0 && t.value === "" || t.value != n) && (t.value = "" + n) : t.value !== "" + n && (t.value = "" + n);
         else if (i === "submit" || i === "reset") {
             t.removeAttribute("value");
             return
         }
-        e.hasOwnProperty("value") ? Bd(t, e.type, n) : e.hasOwnProperty("defaultValue") && Bd(t, e.type, Lr(e.defaultValue)), e.checked == null && e.defaultChecked != null && (t.defaultChecked = !!e.defaultChecked)
+        e.hasOwnProperty("value") ? Hd(t, e.type, n) : e.hasOwnProperty("defaultValue") && Hd(t, e.type, Lr(e.defaultValue)), e.checked == null && e.defaultChecked != null && (t.defaultChecked = !!e.defaultChecked)
     }
 
     function qm(t, e, n) {
         if (e.hasOwnProperty("value") || e.hasOwnProperty("defaultValue")) {
             var i = e.type;
             if (!(i !== "submit" && i !== "reset" || e.value !== void 0 && e.value !== null)) return;
             e = "" + t._wrapperState.initialValue, n || e === t.value || (t.value = e), t.defaultValue = e
         }
         n = t.name, n !== "" && (t.name = ""), t.defaultChecked = !!t._wrapperState.initialChecked, n !== "" && (t.name = n)
     }
 
-    function Bd(t, e, n) {
-        (e !== "number" || zu(t.ownerDocument) !== t) && (n == null ? t.defaultValue = "" + t._wrapperState.initialValue : t.defaultValue !== "" + n && (t.defaultValue = "" + n))
+    function Hd(t, e, n) {
+        (e !== "number" || Fu(t.ownerDocument) !== t) && (n == null ? t.defaultValue = "" + t._wrapperState.initialValue : t.defaultValue !== "" + n && (t.defaultValue = "" + n))
     }
-    var Ea = Array.isArray;
+    var Ta = Array.isArray;
 
     function gs(t, e, n, i) {
         if (t = t.options, e) {
             e = {};
             for (var r = 0; r < n.length; r++) e["$" + n[r]] = !0;
             for (n = 0; n < t.length; n++) r = e.hasOwnProperty("$" + t[n].value), t[n].selected !== r && (t[n].selected = r), r && i && (t[n].defaultSelected = !0)
         } else {
@@ -1079,30 +1079,30 @@
                 }
                 e !== null || t[r].disabled || (e = t[r])
             }
             e !== null && (e.selected = !0)
         }
     }
 
-    function Wd(t, e) {
-        if (e.dangerouslySetInnerHTML != null) throw Error(ne(91));
+    function Bd(t, e) {
+        if (e.dangerouslySetInnerHTML != null) throw Error(te(91));
         return ht({}, e, {
             value: void 0,
             defaultValue: void 0,
             children: "" + t._wrapperState.initialValue
         })
     }
 
     function Zm(t, e) {
         var n = e.value;
         if (n == null) {
             if (n = e.children, e = e.defaultValue, n != null) {
-                if (e != null) throw Error(ne(92));
-                if (Ea(n)) {
-                    if (1 < n.length) throw Error(ne(93));
+                if (e != null) throw Error(te(92));
+                if (Ta(n)) {
+                    if (1 < n.length) throw Error(te(93));
                     n = n[0]
                 }
                 e = n
             }
             e == null && (e = ""), n = e
         }
         t._wrapperState = {
@@ -1112,15 +1112,15 @@
 
     function ry(t, e) {
         var n = Lr(e.value),
             i = Lr(e.defaultValue);
         n != null && (n = "" + n, n !== t.value && (t.value = n), e.defaultValue == null && t.defaultValue !== n && (t.defaultValue = n)), i != null && (t.defaultValue = "" + i)
     }
 
-    function Gm(t) {
+    function Km(t) {
         var e = t.textContent;
         e === t._wrapperState.initialValue && e !== "" && e !== null && (t.value = e)
     }
 
     function oy(t) {
         switch (t) {
             case "svg":
@@ -1128,32 +1128,32 @@
             case "math":
                 return "http://www.w3.org/1998/Math/MathML";
             default:
                 return "http://www.w3.org/1999/xhtml"
         }
     }
 
-    function Vd(t, e) {
+    function Wd(t, e) {
         return t == null || t === "http://www.w3.org/1999/xhtml" ? oy(e) : t === "http://www.w3.org/2000/svg" && e === "foreignObject" ? "http://www.w3.org/1999/xhtml" : t
     }
-    var cu, sy = function(t) {
+    var fu, sy = function(t) {
         return typeof MSApp < "u" && MSApp.execUnsafeLocalFunction ? function(e, n, i, r) {
             MSApp.execUnsafeLocalFunction(function() {
                 return t(e, n, i, r)
             })
         } : t
     }(function(t, e) {
         if (t.namespaceURI !== "http://www.w3.org/2000/svg" || "innerHTML" in t) t.innerHTML = e;
         else {
-            for (cu = cu || document.createElement("div"), cu.innerHTML = "<svg>" + e.valueOf().toString() + "</svg>", e = cu.firstChild; t.firstChild;) t.removeChild(t.firstChild);
+            for (fu = fu || document.createElement("div"), fu.innerHTML = "<svg>" + e.valueOf().toString() + "</svg>", e = fu.firstChild; t.firstChild;) t.removeChild(t.firstChild);
             for (; e.firstChild;) t.appendChild(e.firstChild)
         }
     });
 
-    function ja(t, e) {
+    function Ha(t, e) {
         if (e) {
             var n = t.firstChild;
             if (n && n === t.lastChild && n.nodeType === 3) {
                 n.nodeValue = e;
                 return
             }
         }
@@ -1220,15 +1220,15 @@
         for (var n in e)
             if (e.hasOwnProperty(n)) {
                 var i = n.indexOf("--") === 0,
                     r = ay(n, e[n], i);
                 n === "float" && (n = "cssFloat"), i ? t.setProperty(n, r) : t[n] = r
             }
     }
-    var kw = ht({
+    var Sw = ht({
         menuitem: !0
     }, {
         area: !0,
         base: !0,
         br: !0,
         col: !0,
         embed: !0,
@@ -1240,26 +1240,26 @@
         meta: !0,
         param: !0,
         source: !0,
         track: !0,
         wbr: !0
     });
 
-    function Ud(t, e) {
+    function Vd(t, e) {
         if (e) {
-            if (kw[t] && (e.children != null || e.dangerouslySetInnerHTML != null)) throw Error(ne(137, t));
+            if (Sw[t] && (e.children != null || e.dangerouslySetInnerHTML != null)) throw Error(te(137, t));
             if (e.dangerouslySetInnerHTML != null) {
-                if (e.children != null) throw Error(ne(60));
-                if (typeof e.dangerouslySetInnerHTML != "object" || !("__html" in e.dangerouslySetInnerHTML)) throw Error(ne(61))
+                if (e.children != null) throw Error(te(60));
+                if (typeof e.dangerouslySetInnerHTML != "object" || !("__html" in e.dangerouslySetInnerHTML)) throw Error(te(61))
             }
-            if (e.style != null && typeof e.style != "object") throw Error(ne(62))
+            if (e.style != null && typeof e.style != "object") throw Error(te(62))
         }
     }
 
-    function $d(t, e) {
+    function Ud(t, e) {
         if (t.indexOf("-") === -1) return typeof e.is == "string";
         switch (t) {
             case "annotation-xml":
             case "color-profile":
             case "font-face":
             case "font-face-src":
             case "font-face-uri":
@@ -1267,65 +1267,65 @@
             case "font-face-name":
             case "missing-glyph":
                 return !1;
             default:
                 return !0
         }
     }
-    var Yd = null;
+    var $d = null;
 
-    function Ah(t) {
+    function Oh(t) {
         return t = t.target || t.srcElement || window, t.correspondingUseElement && (t = t.correspondingUseElement), t.nodeType === 3 ? t.parentNode : t
     }
-    var Xd = null,
+    var Yd = null,
         ms = null,
         ys = null;
 
-    function Qm(t) {
-        if (t = il(t)) {
-            if (typeof Xd != "function") throw Error(ne(280));
+    function Gm(t) {
+        if (t = rl(t)) {
+            if (typeof Yd != "function") throw Error(te(280));
             var e = t.stateNode;
-            e && (e = fc(e), Xd(t.stateNode, t.type, e))
+            e && (e = dc(e), Yd(t.stateNode, t.type, e))
         }
     }
 
     function uy(t) {
         ms ? ys ? ys.push(t) : ys = [t] : ms = t
     }
 
     function cy() {
         if (ms) {
             var t = ms,
                 e = ys;
-            if (ys = ms = null, Qm(t), e)
-                for (t = 0; t < e.length; t++) Qm(e[t])
+            if (ys = ms = null, Gm(t), e)
+                for (t = 0; t < e.length; t++) Gm(e[t])
         }
     }
 
     function fy(t, e) {
         return t(e)
     }
 
     function dy() {}
-    var gd = !1;
+    var pd = !1;
 
     function hy(t, e, n) {
-        if (gd) return t(e, n);
-        gd = !0;
+        if (pd) return t(e, n);
+        pd = !0;
         try {
             return fy(t, e, n)
         } finally {
-            gd = !1, (ms !== null || ys !== null) && (dy(), cy())
+            pd = !1, (ms !== null || ys !== null) && (dy(), cy())
         }
     }
 
-    function Ha(t, e) {
+    function Ba(t, e) {
         var n = t.stateNode;
         if (n === null) return null;
-        var i = fc(n);
+        var i = dc(n);
         if (i === null) return null;
         n = i[e];
         e: switch (e) {
             case "onClick":
             case "onClickCapture":
             case "onDoubleClick":
             case "onDoubleClickCapture":
@@ -1338,58 +1338,58 @@
             case "onMouseEnter":
                 (i = !i.disabled) || (t = t.type, i = !(t === "button" || t === "input" || t === "select" || t === "textarea")), t = !i;
                 break e;
             default:
                 t = !1
         }
         if (t) return null;
-        if (n && typeof n != "function") throw Error(ne(231, e, typeof n));
+        if (n && typeof n != "function") throw Error(te(231, e, typeof n));
         return n
     }
-    var qd = !1;
+    var Xd = !1;
     if (qi) try {
         ts = {}, Object.defineProperty(ts, "passive", {
             get: function() {
-                qd = !0
+                Xd = !0
             }
         }), window.addEventListener("test", ts, ts), window.removeEventListener("test", ts, ts)
     } catch {
-        qd = !1
+        Xd = !1
     }
     var ts;
 
-    function Sw(t, e, n, i, r, o, s, a, l) {
+    function kw(t, e, n, i, r, o, s, a, l) {
         var c = Array.prototype.slice.call(arguments, 3);
         try {
             e.apply(n, c)
         } catch (d) {
             this.onError(d)
         }
     }
-    var Da = !1,
-        Fu = null,
-        ju = !1,
-        Zd = null,
+    var Oa = !1,
+        ju = null,
+        Hu = !1,
+        qd = null,
         Cw = {
             onError: function(t) {
-                Da = !0, Fu = t
+                Oa = !0, ju = t
             }
         };
 
     function Ew(t, e, n, i, r, o, s, a, l) {
-        Da = !1, Fu = null, Sw.apply(Cw, arguments)
+        Oa = !1, ju = null, kw.apply(Cw, arguments)
     }
 
     function Tw(t, e, n, i, r, o, s, a, l) {
-        if (Ew.apply(this, arguments), Da) {
-            if (Da) {
-                var c = Fu;
-                Da = !1, Fu = null
-            } else throw Error(ne(198));
-            ju || (ju = !0, Zd = c)
+        if (Ew.apply(this, arguments), Oa) {
+            if (Oa) {
+                var c = ju;
+                Oa = !1, ju = null
+            } else throw Error(te(198));
+            Hu || (Hu = !0, qd = c)
         }
     }
 
     function Co(t) {
         var e = t,
             n = t;
         if (t.alternate)
@@ -1405,22 +1405,22 @@
         if (t.tag === 13) {
             var e = t.memoizedState;
             if (e === null && (t = t.alternate, t !== null && (e = t.memoizedState)), e !== null) return e.dehydrated
         }
         return null
     }
 
-    function Km(t) {
-        if (Co(t) !== t) throw Error(ne(188))
+    function Qm(t) {
+        if (Co(t) !== t) throw Error(te(188))
     }
 
-    function Pw(t) {
+    function Dw(t) {
         var e = t.alternate;
         if (!e) {
-            if (e = Co(t), e === null) throw Error(ne(188));
+            if (e = Co(t), e === null) throw Error(te(188));
             return e !== t ? null : t
         }
         for (var n = t, i = e;;) {
             var r = n.return;
             if (r === null) break;
             var o = r.alternate;
             if (o === null) {
@@ -1428,19 +1428,19 @@
                     n = i;
                     continue
                 }
                 break
             }
             if (r.child === o.child) {
                 for (o = r.child; o;) {
-                    if (o === n) return Km(r), t;
-                    if (o === i) return Km(r), e;
+                    if (o === n) return Qm(r), t;
+                    if (o === i) return Qm(r), e;
                     o = o.sibling
                 }
-                throw Error(ne(188))
+                throw Error(te(188))
             }
             if (n.return !== i.return) n = r, i = o;
             else {
                 for (var s = !1, a = r.child; a;) {
                     if (a === n) {
                         s = !0, n = r, i = o;
                         break
@@ -1459,66 +1459,66 @@
                         }
                         if (a === i) {
                             s = !0, i = o, n = r;
                             break
                         }
                         a = a.sibling
                     }
-                    if (!s) throw Error(ne(189))
+                    if (!s) throw Error(te(189))
                 }
             }
-            if (n.alternate !== i) throw Error(ne(190))
+            if (n.alternate !== i) throw Error(te(190))
         }
-        if (n.tag !== 3) throw Error(ne(188));
+        if (n.tag !== 3) throw Error(te(188));
         return n.stateNode.current === n ? t : e
     }
 
     function gy(t) {
-        return t = Pw(t), t !== null ? my(t) : null
+        return t = Dw(t), t !== null ? my(t) : null
     }
 
     function my(t) {
         if (t.tag === 5 || t.tag === 6) return t;
         for (t = t.child; t !== null;) {
             var e = my(t);
             if (e !== null) return e;
             t = t.sibling
         }
         return null
     }
     var yy = Rn.unstable_scheduleCallback,
         Jm = Rn.unstable_cancelCallback,
-        Mw = Rn.unstable_shouldYield,
-        Dw = Rn.unstable_requestPaint,
+        Pw = Rn.unstable_shouldYield,
+        Mw = Rn.unstable_requestPaint,
         xt = Rn.unstable_now,
         Ow = Rn.unstable_getCurrentPriorityLevel,
-        Lh = Rn.unstable_ImmediatePriority,
+        Ah = Rn.unstable_ImmediatePriority,
         vy = Rn.unstable_UserBlockingPriority,
-        Hu = Rn.unstable_NormalPriority,
+        Bu = Rn.unstable_NormalPriority,
         Aw = Rn.unstable_LowPriority,
         xy = Rn.unstable_IdlePriority,
-        ac = null,
+        lc = null,
         wi = null;
 
     function Lw(t) {
         if (wi && typeof wi.onCommitFiberRoot == "function") try {
-            wi.onCommitFiberRoot(ac, t, void 0, (t.current.flags & 128) === 128)
+            wi.onCommitFiberRoot(lc, t, void 0, (t.current.flags & 128) === 128)
         } catch {}
     }
     var si = Math.clz32 ? Math.clz32 : Nw,
         Rw = Math.log,
         Iw = Math.LN2;
 
     function Nw(t) {
         return t >>>= 0, t === 0 ? 32 : 31 - (Rw(t) / Iw | 0) | 0
     }
-    var fu = 64,
-        du = 4194304;
+    var du = 64,
+        hu = 4194304;
 
-    function Ta(t) {
+    function Da(t) {
         switch (t & -t) {
             case 1:
                 return 1;
             case 2:
                 return 2;
             case 4:
                 return 4;
@@ -1560,25 +1560,25 @@
             case 1073741824:
                 return 1073741824;
             default:
                 return t
         }
     }
 
-    function Bu(t, e) {
+    function Wu(t, e) {
         var n = t.pendingLanes;
         if (n === 0) return 0;
         var i = 0,
             r = t.suspendedLanes,
             o = t.pingedLanes,
             s = n & 268435455;
         if (s !== 0) {
             var a = s & ~r;
-            a !== 0 ? i = Ta(a) : (o &= s, o !== 0 && (i = Ta(o)))
-        } else s = n & ~r, s !== 0 ? i = Ta(s) : o !== 0 && (i = Ta(o));
+            a !== 0 ? i = Da(a) : (o &= s, o !== 0 && (i = Da(o)))
+        } else s = n & ~r, s !== 0 ? i = Da(s) : o !== 0 && (i = Da(o));
         if (i === 0) return 0;
         if (e !== 0 && e !== i && !(e & r) && (r = i & -i, o = e & -e, r >= o || r === 16 && (o & 4194240) !== 0)) return e;
         if (i & 4 && (i |= n & 16), e = t.entangledLanes, e !== 0)
             for (t = t.entanglements, e &= i; 0 < e;) n = 31 - si(e), r = 1 << n, i |= t[n], e &= ~r;
         return i
     }
 
@@ -1629,63 +1629,63 @@
             var s = 31 - si(o),
                 a = 1 << s,
                 l = r[s];
             l === -1 ? (!(a & n) || a & i) && (r[s] = zw(a, e)) : l <= e && (t.expiredLanes |= a), o &= ~a
         }
     }
 
-    function Gd(t) {
+    function Zd(t) {
         return t = t.pendingLanes & -1073741825, t !== 0 ? t : t & 1073741824 ? 1073741824 : 0
     }
 
     function by() {
-        var t = fu;
-        return fu <<= 1, !(fu & 4194240) && (fu = 64), t
+        var t = du;
+        return du <<= 1, !(du & 4194240) && (du = 64), t
     }
 
-    function md(t) {
+    function gd(t) {
         for (var e = [], n = 0; 31 > n; n++) e.push(t);
         return e
     }
 
-    function tl(t, e, n) {
+    function nl(t, e, n) {
         t.pendingLanes |= e, e !== 536870912 && (t.suspendedLanes = 0, t.pingedLanes = 0), t = t.eventTimes, e = 31 - si(e), t[e] = n
     }
 
     function jw(t, e) {
         var n = t.pendingLanes & ~e;
         t.pendingLanes = e, t.suspendedLanes = 0, t.pingedLanes = 0, t.expiredLanes &= e, t.mutableReadLanes &= e, t.entangledLanes &= e, e = t.entanglements;
         var i = t.eventTimes;
         for (t = t.expirationTimes; 0 < n;) {
             var r = 31 - si(n),
                 o = 1 << r;
             e[r] = 0, i[r] = -1, t[r] = -1, n &= ~o
         }
     }
 
-    function Rh(t, e) {
+    function Lh(t, e) {
         var n = t.entangledLanes |= e;
         for (t = t.entanglements; n;) {
             var i = 31 - si(n),
                 r = 1 << i;
             r & e | t[i] & e && (t[i] |= e), n &= ~r
         }
     }
     var Be = 0;
 
     function _y(t) {
         return t &= -t, 1 < t ? 4 < t ? t & 268435455 ? 16 : 536870912 : 4 : 1
     }
-    var wy, Ih, ky, Sy, Cy, Qd = !1,
-        hu = [],
+    var wy, Rh, Sy, ky, Cy, Kd = !1,
+        pu = [],
         Cr = null,
         Er = null,
         Tr = null,
-        Ba = new Map,
         Wa = new Map,
+        Va = new Map,
         _r = [],
         Hw = "mousedown mouseup touchcancel touchend touchstart auxclick dblclick pointercancel pointerdown pointerup dragend dragstart drop compositionend compositionstart keydown keypress keyup input textInput copy cut paste click change contextmenu reset submit".split(" ");
 
     function e0(t, e) {
         switch (t) {
             case "focusin":
             case "focusout":
@@ -1697,163 +1697,163 @@
                 break;
             case "mouseover":
             case "mouseout":
                 Tr = null;
                 break;
             case "pointerover":
             case "pointerout":
-                Ba.delete(e.pointerId);
+                Wa.delete(e.pointerId);
                 break;
             case "gotpointercapture":
             case "lostpointercapture":
-                Wa.delete(e.pointerId)
+                Va.delete(e.pointerId)
         }
     }
 
-    function va(t, e, n, i, r, o) {
+    function xa(t, e, n, i, r, o) {
         return t === null || t.nativeEvent !== o ? (t = {
             blockedOn: e,
             domEventName: n,
             eventSystemFlags: i,
             nativeEvent: o,
             targetContainers: [r]
-        }, e !== null && (e = il(e), e !== null && Ih(e)), t) : (t.eventSystemFlags |= i, e = t.targetContainers, r !== null && e.indexOf(r) === -1 && e.push(r), t)
+        }, e !== null && (e = rl(e), e !== null && Rh(e)), t) : (t.eventSystemFlags |= i, e = t.targetContainers, r !== null && e.indexOf(r) === -1 && e.push(r), t)
     }
 
     function Bw(t, e, n, i, r) {
         switch (e) {
             case "focusin":
-                return Cr = va(Cr, t, e, n, i, r), !0;
+                return Cr = xa(Cr, t, e, n, i, r), !0;
             case "dragenter":
-                return Er = va(Er, t, e, n, i, r), !0;
+                return Er = xa(Er, t, e, n, i, r), !0;
             case "mouseover":
-                return Tr = va(Tr, t, e, n, i, r), !0;
+                return Tr = xa(Tr, t, e, n, i, r), !0;
             case "pointerover":
                 var o = r.pointerId;
-                return Ba.set(o, va(Ba.get(o) || null, t, e, n, i, r)), !0;
+                return Wa.set(o, xa(Wa.get(o) || null, t, e, n, i, r)), !0;
             case "gotpointercapture":
-                return o = r.pointerId, Wa.set(o, va(Wa.get(o) || null, t, e, n, i, r)), !0
+                return o = r.pointerId, Va.set(o, xa(Va.get(o) || null, t, e, n, i, r)), !0
         }
         return !1
     }
 
     function Ey(t) {
         var e = po(t.target);
         if (e !== null) {
             var n = Co(e);
             if (n !== null) {
                 if (e = n.tag, e === 13) {
                     if (e = py(n), e !== null) {
                         t.blockedOn = e, Cy(t.priority, function() {
-                            ky(n)
+                            Sy(n)
                         });
                         return
                     }
                 } else if (e === 3 && n.stateNode.current.memoizedState.isDehydrated) {
                     t.blockedOn = n.tag === 3 ? n.stateNode.containerInfo : null;
                     return
                 }
             }
         }
         t.blockedOn = null
     }
 
-    function Tu(t) {
+    function Du(t) {
         if (t.blockedOn !== null) return !1;
         for (var e = t.targetContainers; 0 < e.length;) {
-            var n = Kd(t.domEventName, t.eventSystemFlags, e[0], t.nativeEvent);
+            var n = Gd(t.domEventName, t.eventSystemFlags, e[0], t.nativeEvent);
             if (n === null) {
                 n = t.nativeEvent;
                 var i = new n.constructor(n.type, n);
-                Yd = i, n.target.dispatchEvent(i), Yd = null
-            } else return e = il(n), e !== null && Ih(e), t.blockedOn = n, !1;
+                $d = i, n.target.dispatchEvent(i), $d = null
+            } else return e = rl(n), e !== null && Rh(e), t.blockedOn = n, !1;
             e.shift()
         }
         return !0
     }
 
     function t0(t, e, n) {
-        Tu(t) && n.delete(e)
+        Du(t) && n.delete(e)
     }
 
     function Ww() {
-        Qd = !1, Cr !== null && Tu(Cr) && (Cr = null), Er !== null && Tu(Er) && (Er = null), Tr !== null && Tu(Tr) && (Tr = null), Ba.forEach(t0), Wa.forEach(t0)
+        Kd = !1, Cr !== null && Du(Cr) && (Cr = null), Er !== null && Du(Er) && (Er = null), Tr !== null && Du(Tr) && (Tr = null), Wa.forEach(t0), Va.forEach(t0)
     }
 
-    function xa(t, e) {
-        t.blockedOn === e && (t.blockedOn = null, Qd || (Qd = !0, Rn.unstable_scheduleCallback(Rn.unstable_NormalPriority, Ww)))
+    function ba(t, e) {
+        t.blockedOn === e && (t.blockedOn = null, Kd || (Kd = !0, Rn.unstable_scheduleCallback(Rn.unstable_NormalPriority, Ww)))
     }
 
-    function Va(t) {
+    function Ua(t) {
         function e(r) {
-            return xa(r, t)
+            return ba(r, t)
         }
-        if (0 < hu.length) {
-            xa(hu[0], t);
-            for (var n = 1; n < hu.length; n++) {
-                var i = hu[n];
+        if (0 < pu.length) {
+            ba(pu[0], t);
+            for (var n = 1; n < pu.length; n++) {
+                var i = pu[n];
                 i.blockedOn === t && (i.blockedOn = null)
             }
         }
-        for (Cr !== null && xa(Cr, t), Er !== null && xa(Er, t), Tr !== null && xa(Tr, t), Ba.forEach(e), Wa.forEach(e), n = 0; n < _r.length; n++) i = _r[n], i.blockedOn === t && (i.blockedOn = null);
+        for (Cr !== null && ba(Cr, t), Er !== null && ba(Er, t), Tr !== null && ba(Tr, t), Wa.forEach(e), Va.forEach(e), n = 0; n < _r.length; n++) i = _r[n], i.blockedOn === t && (i.blockedOn = null);
         for (; 0 < _r.length && (n = _r[0], n.blockedOn === null);) Ey(n), n.blockedOn === null && _r.shift()
     }
-    var vs = Ki.ReactCurrentBatchConfig,
-        Wu = !0;
+    var vs = Qi.ReactCurrentBatchConfig,
+        Vu = !0;
 
     function Vw(t, e, n, i) {
         var r = Be,
             o = vs.transition;
         vs.transition = null;
         try {
-            Be = 1, Nh(t, e, n, i)
+            Be = 1, Ih(t, e, n, i)
         } finally {
             Be = r, vs.transition = o
         }
     }
 
     function Uw(t, e, n, i) {
         var r = Be,
             o = vs.transition;
         vs.transition = null;
         try {
-            Be = 4, Nh(t, e, n, i)
+            Be = 4, Ih(t, e, n, i)
         } finally {
             Be = r, vs.transition = o
         }
     }
 
-    function Nh(t, e, n, i) {
-        if (Wu) {
-            var r = Kd(t, e, n, i);
-            if (r === null) kd(t, e, i, Vu, n), e0(t, i);
+    function Ih(t, e, n, i) {
+        if (Vu) {
+            var r = Gd(t, e, n, i);
+            if (r === null) wd(t, e, i, Uu, n), e0(t, i);
             else if (Bw(r, t, e, n, i)) i.stopPropagation();
             else if (e0(t, i), e & 4 && -1 < Hw.indexOf(t)) {
                 for (; r !== null;) {
-                    var o = il(r);
-                    if (o !== null && wy(o), o = Kd(t, e, n, i), o === null && kd(t, e, i, Vu, n), o === r) break;
+                    var o = rl(r);
+                    if (o !== null && wy(o), o = Gd(t, e, n, i), o === null && wd(t, e, i, Uu, n), o === r) break;
                     r = o
                 }
                 r !== null && i.stopPropagation()
-            } else kd(t, e, i, null, n)
+            } else wd(t, e, i, null, n)
         }
     }
-    var Vu = null;
+    var Uu = null;
 
-    function Kd(t, e, n, i) {
-        if (Vu = null, t = Ah(i), t = po(t), t !== null)
+    function Gd(t, e, n, i) {
+        if (Uu = null, t = Oh(i), t = po(t), t !== null)
             if (e = Co(t), e === null) t = null;
             else if (n = e.tag, n === 13) {
             if (t = py(e), t !== null) return t;
             t = null
         } else if (n === 3) {
             if (e.stateNode.current.memoizedState.isDehydrated) return e.tag === 3 ? e.stateNode.containerInfo : null;
             t = null
         } else e !== t && (t = null);
-        return Vu = t, null
+        return Uu = t, null
     }
 
     function Ty(t) {
         switch (t) {
             case "cancel":
             case "click":
             case "close":
@@ -1924,159 +1924,159 @@
             case "mouseenter":
             case "mouseleave":
             case "pointerenter":
             case "pointerleave":
                 return 4;
             case "message":
                 switch (Ow()) {
-                    case Lh:
+                    case Ah:
                         return 1;
                     case vy:
                         return 4;
-                    case Hu:
+                    case Bu:
                     case Aw:
                         return 16;
                     case xy:
                         return 536870912;
                     default:
                         return 16
                 }
             default:
                 return 16
         }
     }
-    var kr = null,
-        zh = null,
+    var Sr = null,
+        Nh = null,
         Pu = null;
 
-    function Py() {
+    function Dy() {
         if (Pu) return Pu;
-        var t, e = zh,
+        var t, e = Nh,
             n = e.length,
-            i, r = "value" in kr ? kr.value : kr.textContent,
+            i, r = "value" in Sr ? Sr.value : Sr.textContent,
             o = r.length;
         for (t = 0; t < n && e[t] === r[t]; t++);
         var s = n - t;
         for (i = 1; i <= s && e[n - i] === r[o - i]; i++);
         return Pu = r.slice(t, 1 < i ? 1 - i : void 0)
     }
 
     function Mu(t) {
         var e = t.keyCode;
         return "charCode" in t ? (t = t.charCode, t === 0 && e === 13 && (t = 13)) : t = e, t === 10 && (t = 13), 32 <= t || t === 13 ? t : 0
     }
 
-    function pu() {
+    function gu() {
         return !0
     }
 
     function n0() {
         return !1
     }
 
     function In(t) {
         function e(n, i, r, o, s) {
             this._reactName = n, this._targetInst = r, this.type = i, this.nativeEvent = o, this.target = s, this.currentTarget = null;
             for (var a in t) t.hasOwnProperty(a) && (n = t[a], this[a] = n ? n(o) : o[a]);
-            return this.isDefaultPrevented = (o.defaultPrevented != null ? o.defaultPrevented : o.returnValue === !1) ? pu : n0, this.isPropagationStopped = n0, this
+            return this.isDefaultPrevented = (o.defaultPrevented != null ? o.defaultPrevented : o.returnValue === !1) ? gu : n0, this.isPropagationStopped = n0, this
         }
         return ht(e.prototype, {
             preventDefault: function() {
                 this.defaultPrevented = !0;
                 var n = this.nativeEvent;
-                n && (n.preventDefault ? n.preventDefault() : typeof n.returnValue != "unknown" && (n.returnValue = !1), this.isDefaultPrevented = pu)
+                n && (n.preventDefault ? n.preventDefault() : typeof n.returnValue != "unknown" && (n.returnValue = !1), this.isDefaultPrevented = gu)
             },
             stopPropagation: function() {
                 var n = this.nativeEvent;
-                n && (n.stopPropagation ? n.stopPropagation() : typeof n.cancelBubble != "unknown" && (n.cancelBubble = !0), this.isPropagationStopped = pu)
+                n && (n.stopPropagation ? n.stopPropagation() : typeof n.cancelBubble != "unknown" && (n.cancelBubble = !0), this.isPropagationStopped = gu)
             },
             persist: function() {},
-            isPersistent: pu
+            isPersistent: gu
         }), e
     }
-    var Ps = {
+    var Ds = {
             eventPhase: 0,
             bubbles: 0,
             cancelable: 0,
             timeStamp: function(t) {
                 return t.timeStamp || Date.now()
             },
             defaultPrevented: 0,
             isTrusted: 0
         },
-        Fh = In(Ps),
-        nl = ht({}, Ps, {
+        zh = In(Ds),
+        il = ht({}, Ds, {
             view: 0,
             detail: 0
         }),
-        $w = In(nl),
-        yd, vd, ba, lc = ht({}, nl, {
+        $w = In(il),
+        md, yd, _a, uc = ht({}, il, {
             screenX: 0,
             screenY: 0,
             clientX: 0,
             clientY: 0,
             pageX: 0,
             pageY: 0,
             ctrlKey: 0,
             shiftKey: 0,
             altKey: 0,
             metaKey: 0,
-            getModifierState: jh,
+            getModifierState: Fh,
             button: 0,
             buttons: 0,
             relatedTarget: function(t) {
                 return t.relatedTarget === void 0 ? t.fromElement === t.srcElement ? t.toElement : t.fromElement : t.relatedTarget
             },
             movementX: function(t) {
-                return "movementX" in t ? t.movementX : (t !== ba && (ba && t.type === "mousemove" ? (yd = t.screenX - ba.screenX, vd = t.screenY - ba.screenY) : vd = yd = 0, ba = t), yd)
+                return "movementX" in t ? t.movementX : (t !== _a && (_a && t.type === "mousemove" ? (md = t.screenX - _a.screenX, yd = t.screenY - _a.screenY) : yd = md = 0, _a = t), md)
             },
             movementY: function(t) {
-                return "movementY" in t ? t.movementY : vd
+                return "movementY" in t ? t.movementY : yd
             }
         }),
-        i0 = In(lc),
-        Yw = ht({}, lc, {
+        i0 = In(uc),
+        Yw = ht({}, uc, {
             dataTransfer: 0
         }),
         Xw = In(Yw),
-        qw = ht({}, nl, {
+        qw = ht({}, il, {
             relatedTarget: 0
         }),
-        xd = In(qw),
-        Zw = ht({}, Ps, {
+        vd = In(qw),
+        Zw = ht({}, Ds, {
             animationName: 0,
             elapsedTime: 0,
             pseudoElement: 0
         }),
-        Gw = In(Zw),
-        Qw = ht({}, Ps, {
+        Kw = In(Zw),
+        Gw = ht({}, Ds, {
             clipboardData: function(t) {
                 return "clipboardData" in t ? t.clipboardData : window.clipboardData
             }
         }),
-        Kw = In(Qw),
-        Jw = ht({}, Ps, {
+        Qw = In(Gw),
+        Jw = ht({}, Ds, {
             data: 0
         }),
         r0 = In(Jw),
-        ek = {
+        eS = {
             Esc: "Escape",
             Spacebar: " ",
             Left: "ArrowLeft",
             Up: "ArrowUp",
             Right: "ArrowRight",
             Down: "ArrowDown",
             Del: "Delete",
             Win: "OS",
             Menu: "ContextMenu",
             Apps: "ContextMenu",
             Scroll: "ScrollLock",
             MozPrintableKey: "Unidentified"
         },
-        tk = {
+        tS = {
             8: "Backspace",
             9: "Tab",
             12: "Clear",
             13: "Enter",
             16: "Shift",
             17: "Control",
             18: "Alt",
@@ -2106,111 +2106,111 @@
             121: "F10",
             122: "F11",
             123: "F12",
             144: "NumLock",
             145: "ScrollLock",
             224: "Meta"
         },
-        nk = {
+        nS = {
             Alt: "altKey",
             Control: "ctrlKey",
             Meta: "metaKey",
             Shift: "shiftKey"
         };
 
-    function ik(t) {
+    function iS(t) {
         var e = this.nativeEvent;
-        return e.getModifierState ? e.getModifierState(t) : (t = nk[t]) ? !!e[t] : !1
+        return e.getModifierState ? e.getModifierState(t) : (t = nS[t]) ? !!e[t] : !1
     }
 
-    function jh() {
-        return ik
+    function Fh() {
+        return iS
     }
-    var rk = ht({}, nl, {
+    var rS = ht({}, il, {
             key: function(t) {
                 if (t.key) {
-                    var e = ek[t.key] || t.key;
+                    var e = eS[t.key] || t.key;
                     if (e !== "Unidentified") return e
                 }
-                return t.type === "keypress" ? (t = Mu(t), t === 13 ? "Enter" : String.fromCharCode(t)) : t.type === "keydown" || t.type === "keyup" ? tk[t.keyCode] || "Unidentified" : ""
+                return t.type === "keypress" ? (t = Mu(t), t === 13 ? "Enter" : String.fromCharCode(t)) : t.type === "keydown" || t.type === "keyup" ? tS[t.keyCode] || "Unidentified" : ""
             },
             code: 0,
             location: 0,
             ctrlKey: 0,
             shiftKey: 0,
             altKey: 0,
             metaKey: 0,
             repeat: 0,
             locale: 0,
-            getModifierState: jh,
+            getModifierState: Fh,
             charCode: function(t) {
                 return t.type === "keypress" ? Mu(t) : 0
             },
             keyCode: function(t) {
                 return t.type === "keydown" || t.type === "keyup" ? t.keyCode : 0
             },
             which: function(t) {
                 return t.type === "keypress" ? Mu(t) : t.type === "keydown" || t.type === "keyup" ? t.keyCode : 0
             }
         }),
-        ok = In(rk),
-        sk = ht({}, lc, {
+        oS = In(rS),
+        sS = ht({}, uc, {
             pointerId: 0,
             width: 0,
             height: 0,
             pressure: 0,
             tangentialPressure: 0,
             tiltX: 0,
             tiltY: 0,
             twist: 0,
             pointerType: 0,
             isPrimary: 0
         }),
-        o0 = In(sk),
-        ak = ht({}, nl, {
+        o0 = In(sS),
+        aS = ht({}, il, {
             touches: 0,
             targetTouches: 0,
             changedTouches: 0,
             altKey: 0,
             metaKey: 0,
             ctrlKey: 0,
             shiftKey: 0,
-            getModifierState: jh
+            getModifierState: Fh
         }),
-        lk = In(ak),
-        uk = ht({}, Ps, {
+        lS = In(aS),
+        uS = ht({}, Ds, {
             propertyName: 0,
             elapsedTime: 0,
             pseudoElement: 0
         }),
-        ck = In(uk),
-        fk = ht({}, lc, {
+        cS = In(uS),
+        fS = ht({}, uc, {
             deltaX: function(t) {
                 return "deltaX" in t ? t.deltaX : "wheelDeltaX" in t ? -t.wheelDeltaX : 0
             },
             deltaY: function(t) {
                 return "deltaY" in t ? t.deltaY : "wheelDeltaY" in t ? -t.wheelDeltaY : "wheelDelta" in t ? -t.wheelDelta : 0
             },
             deltaZ: 0,
             deltaMode: 0
         }),
-        dk = In(fk),
-        hk = [9, 13, 27, 32],
-        Hh = qi && "CompositionEvent" in window,
-        Oa = null;
-    qi && "documentMode" in document && (Oa = document.documentMode);
-    var pk = qi && "TextEvent" in window && !Oa,
-        My = qi && (!Hh || Oa && 8 < Oa && 11 >= Oa),
+        dS = In(fS),
+        hS = [9, 13, 27, 32],
+        jh = qi && "CompositionEvent" in window,
+        Aa = null;
+    qi && "documentMode" in document && (Aa = document.documentMode);
+    var pS = qi && "TextEvent" in window && !Aa,
+        Py = qi && (!jh || Aa && 8 < Aa && 11 >= Aa),
         s0 = " ",
         a0 = !1;
 
-    function Dy(t, e) {
+    function My(t, e) {
         switch (t) {
             case "keyup":
-                return hk.indexOf(e.keyCode) !== -1;
+                return hS.indexOf(e.keyCode) !== -1;
             case "keydown":
                 return e.keyCode !== 229;
             case "keypress":
             case "mousedown":
             case "focusout":
                 return !0;
             default:
@@ -2219,45 +2219,45 @@
     }
 
     function Oy(t) {
         return t = t.detail, typeof t == "object" && "data" in t ? t.data : null
     }
     var os = !1;
 
-    function gk(t, e) {
+    function gS(t, e) {
         switch (t) {
             case "compositionend":
                 return Oy(e);
             case "keypress":
                 return e.which !== 32 ? null : (a0 = !0, s0);
             case "textInput":
                 return t = e.data, t === s0 && a0 ? null : t;
             default:
                 return null
         }
     }
 
-    function mk(t, e) {
-        if (os) return t === "compositionend" || !Hh && Dy(t, e) ? (t = Py(), Pu = zh = kr = null, os = !1, t) : null;
+    function mS(t, e) {
+        if (os) return t === "compositionend" || !jh && My(t, e) ? (t = Dy(), Pu = Nh = Sr = null, os = !1, t) : null;
         switch (t) {
             case "paste":
                 return null;
             case "keypress":
                 if (!(e.ctrlKey || e.altKey || e.metaKey) || e.ctrlKey && e.altKey) {
                     if (e.char && 1 < e.char.length) return e.char;
                     if (e.which) return String.fromCharCode(e.which)
                 }
                 return null;
             case "compositionend":
-                return My && e.locale !== "ko" ? null : e.data;
+                return Py && e.locale !== "ko" ? null : e.data;
             default:
                 return null
         }
     }
-    var yk = {
+    var yS = {
         color: !0,
         date: !0,
         datetime: !0,
         "datetime-local": !0,
         email: !0,
         month: !0,
         number: !0,
@@ -2269,83 +2269,83 @@
         time: !0,
         url: !0,
         week: !0
     };
 
     function l0(t) {
         var e = t && t.nodeName && t.nodeName.toLowerCase();
-        return e === "input" ? !!yk[t.type] : e === "textarea"
+        return e === "input" ? !!yS[t.type] : e === "textarea"
     }
 
     function Ay(t, e, n, i) {
-        uy(i), e = Uu(e, "onChange"), 0 < e.length && (n = new Fh("onChange", "change", null, n, i), t.push({
+        uy(i), e = $u(e, "onChange"), 0 < e.length && (n = new zh("onChange", "change", null, n, i), t.push({
             event: n,
             listeners: e
         }))
     }
-    var Aa = null,
-        Ua = null;
+    var La = null,
+        $a = null;
 
-    function vk(t) {
+    function vS(t) {
         Vy(t, 0)
     }
 
-    function uc(t) {
+    function cc(t) {
         var e = ls(t);
         if (ny(e)) return t
     }
 
-    function xk(t, e) {
+    function xS(t, e) {
         if (t === "change") return e
     }
     var Ly = !1;
-    qi && (qi ? (mu = "oninput" in document, mu || (bd = document.createElement("div"), bd.setAttribute("oninput", "return;"), mu = typeof bd.oninput == "function"), gu = mu) : gu = !1, Ly = gu && (!document.documentMode || 9 < document.documentMode));
-    var gu, mu, bd;
+    qi && (qi ? (yu = "oninput" in document, yu || (xd = document.createElement("div"), xd.setAttribute("oninput", "return;"), yu = typeof xd.oninput == "function"), mu = yu) : mu = !1, Ly = mu && (!document.documentMode || 9 < document.documentMode));
+    var mu, yu, xd;
 
     function u0() {
-        Aa && (Aa.detachEvent("onpropertychange", Ry), Ua = Aa = null)
+        La && (La.detachEvent("onpropertychange", Ry), $a = La = null)
     }
 
     function Ry(t) {
-        if (t.propertyName === "value" && uc(Ua)) {
+        if (t.propertyName === "value" && cc($a)) {
             var e = [];
-            Ay(e, Ua, t, Ah(t)), hy(vk, e)
+            Ay(e, $a, t, Oh(t)), hy(vS, e)
         }
     }
 
-    function bk(t, e, n) {
-        t === "focusin" ? (u0(), Aa = e, Ua = n, Aa.attachEvent("onpropertychange", Ry)) : t === "focusout" && u0()
+    function bS(t, e, n) {
+        t === "focusin" ? (u0(), La = e, $a = n, La.attachEvent("onpropertychange", Ry)) : t === "focusout" && u0()
     }
 
-    function _k(t) {
-        if (t === "selectionchange" || t === "keyup" || t === "keydown") return uc(Ua)
+    function _S(t) {
+        if (t === "selectionchange" || t === "keyup" || t === "keydown") return cc($a)
     }
 
-    function wk(t, e) {
-        if (t === "click") return uc(e)
+    function wS(t, e) {
+        if (t === "click") return cc(e)
     }
 
-    function kk(t, e) {
-        if (t === "input" || t === "change") return uc(e)
+    function SS(t, e) {
+        if (t === "input" || t === "change") return cc(e)
     }
 
-    function Sk(t, e) {
+    function kS(t, e) {
         return t === e && (t !== 0 || 1 / t === 1 / e) || t !== t && e !== e
     }
-    var li = typeof Object.is == "function" ? Object.is : Sk;
+    var li = typeof Object.is == "function" ? Object.is : kS;
 
-    function $a(t, e) {
+    function Ya(t, e) {
         if (li(t, e)) return !0;
         if (typeof t != "object" || t === null || typeof e != "object" || e === null) return !1;
         var n = Object.keys(t),
             i = Object.keys(e);
         if (n.length !== i.length) return !1;
         for (i = 0; i < n.length; i++) {
             var r = n[i];
-            if (!Rd.call(e, r) || !li(t[r], e[r])) return !1
+            if (!Ld.call(e, r) || !li(t[r], e[r])) return !1
         }
         return !0
     }
 
     function c0(t) {
         for (; t && t.firstChild;) t = t.firstChild;
         return t
@@ -2377,38 +2377,38 @@
     }
 
     function Iy(t, e) {
         return t && e ? t === e ? !0 : t && t.nodeType === 3 ? !1 : e && e.nodeType === 3 ? Iy(t, e.parentNode) : "contains" in t ? t.contains(e) : t.compareDocumentPosition ? !!(t.compareDocumentPosition(e) & 16) : !1 : !1
     }
 
     function Ny() {
-        for (var t = window, e = zu(); e instanceof t.HTMLIFrameElement;) {
+        for (var t = window, e = Fu(); e instanceof t.HTMLIFrameElement;) {
             try {
                 var n = typeof e.contentWindow.location.href == "string"
             } catch {
                 n = !1
             }
             if (n) t = e.contentWindow;
             else break;
-            e = zu(t.document)
+            e = Fu(t.document)
         }
         return e
     }
 
-    function Bh(t) {
+    function Hh(t) {
         var e = t && t.nodeName && t.nodeName.toLowerCase();
         return e && (e === "input" && (t.type === "text" || t.type === "search" || t.type === "tel" || t.type === "url" || t.type === "password") || e === "textarea" || t.contentEditable === "true")
     }
 
-    function Ck(t) {
+    function CS(t) {
         var e = Ny(),
             n = t.focusedElem,
             i = t.selectionRange;
         if (e !== n && n && n.ownerDocument && Iy(n.ownerDocument.documentElement, n)) {
-            if (i !== null && Bh(n)) {
+            if (i !== null && Hh(n)) {
                 if (e = i.start, t = i.end, t === void 0 && (t = e), "selectionStart" in n) n.selectionStart = e, n.selectionEnd = Math.min(t, n.value.length);
                 else if (t = (e = n.ownerDocument || document) && e.defaultView || window, t.getSelection) {
                     t = t.getSelection();
                     var r = n.textContent.length,
                         o = Math.min(i.start, r);
                     i = i.end === void 0 ? o : Math.min(i.end, r), !t.extend && o > i && (r = i, i = o, o = r), r = f0(n, o);
                     var s = f0(n, i);
@@ -2419,90 +2419,90 @@
                 element: t,
                 left: t.scrollLeft,
                 top: t.scrollTop
             });
             for (typeof n.focus == "function" && n.focus(), n = 0; n < e.length; n++) t = e[n], t.element.scrollLeft = t.left, t.element.scrollTop = t.top
         }
     }
-    var Ek = qi && "documentMode" in document && 11 >= document.documentMode,
+    var ES = qi && "documentMode" in document && 11 >= document.documentMode,
         ss = null,
-        Jd = null,
-        La = null,
-        eh = !1;
+        Qd = null,
+        Ra = null,
+        Jd = !1;
 
     function d0(t, e, n) {
         var i = n.window === n ? n.document : n.nodeType === 9 ? n : n.ownerDocument;
-        eh || ss == null || ss !== zu(i) || (i = ss, "selectionStart" in i && Bh(i) ? i = {
+        Jd || ss == null || ss !== Fu(i) || (i = ss, "selectionStart" in i && Hh(i) ? i = {
             start: i.selectionStart,
             end: i.selectionEnd
         } : (i = (i.ownerDocument && i.ownerDocument.defaultView || window).getSelection(), i = {
             anchorNode: i.anchorNode,
             anchorOffset: i.anchorOffset,
             focusNode: i.focusNode,
             focusOffset: i.focusOffset
-        }), La && $a(La, i) || (La = i, i = Uu(Jd, "onSelect"), 0 < i.length && (e = new Fh("onSelect", "select", null, e, n), t.push({
+        }), Ra && Ya(Ra, i) || (Ra = i, i = $u(Qd, "onSelect"), 0 < i.length && (e = new zh("onSelect", "select", null, e, n), t.push({
             event: e,
             listeners: i
         }), e.target = ss)))
     }
 
-    function yu(t, e) {
+    function vu(t, e) {
         var n = {};
         return n[t.toLowerCase()] = e.toLowerCase(), n["Webkit" + t] = "webkit" + e, n["Moz" + t] = "moz" + e, n
     }
     var as = {
-            animationend: yu("Animation", "AnimationEnd"),
-            animationiteration: yu("Animation", "AnimationIteration"),
-            animationstart: yu("Animation", "AnimationStart"),
-            transitionend: yu("Transition", "TransitionEnd")
+            animationend: vu("Animation", "AnimationEnd"),
+            animationiteration: vu("Animation", "AnimationIteration"),
+            animationstart: vu("Animation", "AnimationStart"),
+            transitionend: vu("Transition", "TransitionEnd")
         },
-        _d = {},
+        bd = {},
         zy = {};
     qi && (zy = document.createElement("div").style, "AnimationEvent" in window || (delete as.animationend.animation, delete as.animationiteration.animation, delete as.animationstart.animation), "TransitionEvent" in window || delete as.transitionend.transition);
 
-    function cc(t) {
-        if (_d[t]) return _d[t];
+    function fc(t) {
+        if (bd[t]) return bd[t];
         if (!as[t]) return t;
         var e = as[t],
             n;
         for (n in e)
-            if (e.hasOwnProperty(n) && n in zy) return _d[t] = e[n];
+            if (e.hasOwnProperty(n) && n in zy) return bd[t] = e[n];
         return t
     }
-    var Fy = cc("animationend"),
-        jy = cc("animationiteration"),
-        Hy = cc("animationstart"),
-        By = cc("transitionend"),
+    var Fy = fc("animationend"),
+        jy = fc("animationiteration"),
+        Hy = fc("animationstart"),
+        By = fc("transitionend"),
         Wy = new Map,
         h0 = "abort auxClick cancel canPlay canPlayThrough click close contextMenu copy cut drag dragEnd dragEnter dragExit dragLeave dragOver dragStart drop durationChange emptied encrypted ended error gotPointerCapture input invalid keyDown keyPress keyUp load loadedData loadedMetadata loadStart lostPointerCapture mouseDown mouseMove mouseOut mouseOver mouseUp paste pause play playing pointerCancel pointerDown pointerMove pointerOut pointerOver pointerUp progress rateChange reset resize seeked seeking stalled submit suspend timeUpdate touchCancel touchEnd touchStart volumeChange scroll toggle touchMove waiting wheel".split(" ");
 
     function Ir(t, e) {
-        Wy.set(t, e), So(e, [t])
+        Wy.set(t, e), ko(e, [t])
     }
-    for (vu = 0; vu < h0.length; vu++) xu = h0[vu], p0 = xu.toLowerCase(), g0 = xu[0].toUpperCase() + xu.slice(1), Ir(p0, "on" + g0);
-    var xu, p0, g0, vu;
+    for (xu = 0; xu < h0.length; xu++) bu = h0[xu], p0 = bu.toLowerCase(), g0 = bu[0].toUpperCase() + bu.slice(1), Ir(p0, "on" + g0);
+    var bu, p0, g0, xu;
     Ir(Fy, "onAnimationEnd");
     Ir(jy, "onAnimationIteration");
     Ir(Hy, "onAnimationStart");
     Ir("dblclick", "onDoubleClick");
     Ir("focusin", "onFocus");
     Ir("focusout", "onBlur");
     Ir(By, "onTransitionEnd");
     _s("onMouseEnter", ["mouseout", "mouseover"]);
     _s("onMouseLeave", ["mouseout", "mouseover"]);
     _s("onPointerEnter", ["pointerout", "pointerover"]);
     _s("onPointerLeave", ["pointerout", "pointerover"]);
-    So("onChange", "change click focusin focusout input keydown keyup selectionchange".split(" "));
-    So("onSelect", "focusout contextmenu dragend focusin keydown keyup mousedown mouseup selectionchange".split(" "));
-    So("onBeforeInput", ["compositionend", "keypress", "textInput", "paste"]);
-    So("onCompositionEnd", "compositionend focusout keydown keypress keyup mousedown".split(" "));
-    So("onCompositionStart", "compositionstart focusout keydown keypress keyup mousedown".split(" "));
-    So("onCompositionUpdate", "compositionupdate focusout keydown keypress keyup mousedown".split(" "));
+    ko("onChange", "change click focusin focusout input keydown keyup selectionchange".split(" "));
+    ko("onSelect", "focusout contextmenu dragend focusin keydown keyup mousedown mouseup selectionchange".split(" "));
+    ko("onBeforeInput", ["compositionend", "keypress", "textInput", "paste"]);
+    ko("onCompositionEnd", "compositionend focusout keydown keypress keyup mousedown".split(" "));
+    ko("onCompositionStart", "compositionstart focusout keydown keypress keyup mousedown".split(" "));
+    ko("onCompositionUpdate", "compositionupdate focusout keydown keypress keyup mousedown".split(" "));
     var Pa = "abort canplay canplaythrough durationchange emptied encrypted ended error loadeddata loadedmetadata loadstart pause play playing progress ratechange resize seeked seeking stalled suspend timeupdate volumechange waiting".split(" "),
-        Tk = new Set("cancel close invalid load scroll toggle".split(" ").concat(Pa));
+        TS = new Set("cancel close invalid load scroll toggle".split(" ").concat(Pa));
 
     function m0(t, e, n) {
         var i = t.type || "unknown-event";
         t.currentTarget = n, Tw(i, e, void 0, t), t.currentTarget = null
     }
 
     function Vy(t, e) {
@@ -2523,60 +2523,60 @@
                     } else
                         for (s = 0; s < i.length; s++) {
                             if (a = i[s], l = a.instance, c = a.currentTarget, a = a.listener, l !== o && r.isPropagationStopped()) break e;
                             m0(r, a, c), o = l
                         }
             }
         }
-        if (ju) throw t = Zd, ju = !1, Zd = null, t
+        if (Hu) throw t = qd, Hu = !1, qd = null, t
     }
 
     function nt(t, e) {
-        var n = e[oh];
-        n === void 0 && (n = e[oh] = new Set);
+        var n = e[rh];
+        n === void 0 && (n = e[rh] = new Set);
         var i = t + "__bubble";
         n.has(i) || (Uy(e, t, 2, !1), n.add(i))
     }
 
-    function wd(t, e, n) {
+    function _d(t, e, n) {
         var i = 0;
         e && (i |= 4), Uy(n, t, i, e)
     }
-    var bu = "_reactListening" + Math.random().toString(36).slice(2);
+    var _u = "_reactListening" + Math.random().toString(36).slice(2);
 
-    function Ya(t) {
-        if (!t[bu]) {
-            t[bu] = !0, Q0.forEach(function(n) {
-                n !== "selectionchange" && (Tk.has(n) || wd(n, !1, t), wd(n, !0, t))
+    function Xa(t) {
+        if (!t[_u]) {
+            t[_u] = !0, G0.forEach(function(n) {
+                n !== "selectionchange" && (TS.has(n) || _d(n, !1, t), _d(n, !0, t))
             });
             var e = t.nodeType === 9 ? t : t.ownerDocument;
-            e === null || e[bu] || (e[bu] = !0, wd("selectionchange", !1, e))
+            e === null || e[_u] || (e[_u] = !0, _d("selectionchange", !1, e))
         }
     }
 
     function Uy(t, e, n, i) {
         switch (Ty(e)) {
             case 1:
                 var r = Vw;
                 break;
             case 4:
                 r = Uw;
                 break;
             default:
-                r = Nh
+                r = Ih
         }
-        n = r.bind(null, e, n, t), r = void 0, !qd || e !== "touchstart" && e !== "touchmove" && e !== "wheel" || (r = !0), i ? r !== void 0 ? t.addEventListener(e, n, {
+        n = r.bind(null, e, n, t), r = void 0, !Xd || e !== "touchstart" && e !== "touchmove" && e !== "wheel" || (r = !0), i ? r !== void 0 ? t.addEventListener(e, n, {
             capture: !0,
             passive: r
         }) : t.addEventListener(e, n, !0) : r !== void 0 ? t.addEventListener(e, n, {
             passive: r
         }) : t.addEventListener(e, n, !1)
     }
 
-    function kd(t, e, n, i, r) {
+    function wd(t, e, n, i, r) {
         var o = i;
         if (!(e & 1) && !(e & 2) && i !== null) e: for (;;) {
             if (i === null) return;
             var s = i.tag;
             if (s === 3 || s === 4) {
                 var a = i.stateNode.containerInfo;
                 if (a === r || a.nodeType === 8 && a.parentNode === r) break;
@@ -2595,37 +2595,37 @@
                     a = a.parentNode
                 }
             }
             i = i.return
         }
         hy(function() {
             var c = o,
-                d = Ah(n),
+                d = Oh(n),
                 g = [];
             e: {
                 var y = Wy.get(t);
                 if (y !== void 0) {
-                    var x = Fh,
-                        w = t;
+                    var x = zh,
+                        _ = t;
                     switch (t) {
                         case "keypress":
                             if (Mu(n) === 0) break e;
                         case "keydown":
                         case "keyup":
-                            x = ok;
+                            x = oS;
                             break;
                         case "focusin":
-                            w = "focus", x = xd;
+                            _ = "focus", x = vd;
                             break;
                         case "focusout":
-                            w = "blur", x = xd;
+                            _ = "blur", x = vd;
                             break;
                         case "beforeblur":
                         case "afterblur":
-                            x = xd;
+                            x = vd;
                             break;
                         case "click":
                             if (n.button === 2) break e;
                         case "auxclick":
                         case "dblclick":
                         case "mousedown":
                         case "mousemove":
@@ -2645,160 +2645,160 @@
                         case "drop":
                             x = Xw;
                             break;
                         case "touchcancel":
                         case "touchend":
                         case "touchmove":
                         case "touchstart":
-                            x = lk;
+                            x = lS;
                             break;
                         case Fy:
                         case jy:
                         case Hy:
-                            x = Gw;
+                            x = Kw;
                             break;
                         case By:
-                            x = ck;
+                            x = cS;
                             break;
                         case "scroll":
                             x = $w;
                             break;
                         case "wheel":
-                            x = dk;
+                            x = dS;
                             break;
                         case "copy":
                         case "cut":
                         case "paste":
-                            x = Kw;
+                            x = Qw;
                             break;
                         case "gotpointercapture":
                         case "lostpointercapture":
                         case "pointercancel":
                         case "pointerdown":
                         case "pointermove":
                         case "pointerout":
                         case "pointerover":
                         case "pointerup":
                             x = o0
                     }
-                    var S = (e & 4) !== 0,
-                        A = !S && t === "scroll",
-                        _ = S ? y !== null ? y + "Capture" : null : y;
-                    S = [];
-                    for (var C = c, M; C !== null;) {
-                        M = C;
-                        var z = M.stateNode;
-                        if (M.tag === 5 && z !== null && (M = z, _ !== null && (z = Ha(C, _), z != null && S.push(Xa(C, z, M)))), A) break;
-                        C = C.return
+                    var C = (e & 4) !== 0,
+                        A = !C && t === "scroll",
+                        w = C ? y !== null ? y + "Capture" : null : y;
+                    C = [];
+                    for (var k = c, P; k !== null;) {
+                        P = k;
+                        var z = P.stateNode;
+                        if (P.tag === 5 && z !== null && (P = z, w !== null && (z = Ba(k, w), z != null && C.push(qa(k, z, P)))), A) break;
+                        k = k.return
                     }
-                    0 < S.length && (y = new x(y, w, null, n, d), g.push({
+                    0 < C.length && (y = new x(y, _, null, n, d), g.push({
                         event: y,
-                        listeners: S
+                        listeners: C
                     }))
                 }
             }
             if (!(e & 7)) {
                 e: {
-                    if (y = t === "mouseover" || t === "pointerover", x = t === "mouseout" || t === "pointerout", y && n !== Yd && (w = n.relatedTarget || n.fromElement) && (po(w) || w[Zi])) break e;
-                    if ((x || y) && (y = d.window === d ? d : (y = d.ownerDocument) ? y.defaultView || y.parentWindow : window, x ? (w = n.relatedTarget || n.toElement, x = c, w = w ? po(w) : null, w !== null && (A = Co(w), w !== A || w.tag !== 5 && w.tag !== 6) && (w = null)) : (x = null, w = c), x !== w)) {
-                        if (S = i0, z = "onMouseLeave", _ = "onMouseEnter", C = "mouse", (t === "pointerout" || t === "pointerover") && (S = o0, z = "onPointerLeave", _ = "onPointerEnter", C = "pointer"), A = x == null ? y : ls(x), M = w == null ? y : ls(w), y = new S(z, C + "leave", x, n, d), y.target = A, y.relatedTarget = M, z = null, po(d) === c && (S = new S(_, C + "enter", w, n, d), S.target = M, S.relatedTarget = A, z = S), A = z, x && w) t: {
-                            for (S = x, _ = w, C = 0, M = S; M; M = ns(M)) C++;
-                            for (M = 0, z = _; z; z = ns(z)) M++;
-                            for (; 0 < C - M;) S = ns(S),
-                            C--;
-                            for (; 0 < M - C;) _ = ns(_),
-                            M--;
-                            for (; C--;) {
-                                if (S === _ || _ !== null && S === _.alternate) break t;
-                                S = ns(S), _ = ns(_)
+                    if (y = t === "mouseover" || t === "pointerover", x = t === "mouseout" || t === "pointerout", y && n !== $d && (_ = n.relatedTarget || n.fromElement) && (po(_) || _[Zi])) break e;
+                    if ((x || y) && (y = d.window === d ? d : (y = d.ownerDocument) ? y.defaultView || y.parentWindow : window, x ? (_ = n.relatedTarget || n.toElement, x = c, _ = _ ? po(_) : null, _ !== null && (A = Co(_), _ !== A || _.tag !== 5 && _.tag !== 6) && (_ = null)) : (x = null, _ = c), x !== _)) {
+                        if (C = i0, z = "onMouseLeave", w = "onMouseEnter", k = "mouse", (t === "pointerout" || t === "pointerover") && (C = o0, z = "onPointerLeave", w = "onPointerEnter", k = "pointer"), A = x == null ? y : ls(x), P = _ == null ? y : ls(_), y = new C(z, k + "leave", x, n, d), y.target = A, y.relatedTarget = P, z = null, po(d) === c && (C = new C(w, k + "enter", _, n, d), C.target = P, C.relatedTarget = A, z = C), A = z, x && _) t: {
+                            for (C = x, w = _, k = 0, P = C; P; P = ns(P)) k++;
+                            for (P = 0, z = w; z; z = ns(z)) P++;
+                            for (; 0 < k - P;) C = ns(C),
+                            k--;
+                            for (; 0 < P - k;) w = ns(w),
+                            P--;
+                            for (; k--;) {
+                                if (C === w || w !== null && C === w.alternate) break t;
+                                C = ns(C), w = ns(w)
                             }
-                            S = null
+                            C = null
                         }
-                        else S = null;
-                        x !== null && y0(g, y, x, S, !1), w !== null && A !== null && y0(g, A, w, S, !0)
+                        else C = null;
+                        x !== null && y0(g, y, x, C, !1), _ !== null && A !== null && y0(g, A, _, C, !0)
                     }
                 }
                 e: {
-                    if (y = c ? ls(c) : window, x = y.nodeName && y.nodeName.toLowerCase(), x === "select" || x === "input" && y.type === "file") var F = xk;
+                    if (y = c ? ls(c) : window, x = y.nodeName && y.nodeName.toLowerCase(), x === "select" || x === "input" && y.type === "file") var F = xS;
                     else if (l0(y))
-                        if (Ly) F = kk;
+                        if (Ly) F = SS;
                         else {
-                            F = _k;
-                            var h = bk
+                            F = _S;
+                            var h = bS
                         }
-                    else(x = y.nodeName) && x.toLowerCase() === "input" && (y.type === "checkbox" || y.type === "radio") && (F = wk);
+                    else(x = y.nodeName) && x.toLowerCase() === "input" && (y.type === "checkbox" || y.type === "radio") && (F = wS);
                     if (F && (F = F(t, c))) {
                         Ay(g, F, n, d);
                         break e
                     }
                     h && h(t, y, c),
-                    t === "focusout" && (h = y._wrapperState) && h.controlled && y.type === "number" && Bd(y, "number", y.value)
+                    t === "focusout" && (h = y._wrapperState) && h.controlled && y.type === "number" && Hd(y, "number", y.value)
                 }
                 switch (h = c ? ls(c) : window, t) {
                     case "focusin":
-                        (l0(h) || h.contentEditable === "true") && (ss = h, Jd = c, La = null);
+                        (l0(h) || h.contentEditable === "true") && (ss = h, Qd = c, Ra = null);
                         break;
                     case "focusout":
-                        La = Jd = ss = null;
+                        Ra = Qd = ss = null;
                         break;
                     case "mousedown":
-                        eh = !0;
+                        Jd = !0;
                         break;
                     case "contextmenu":
                     case "mouseup":
                     case "dragend":
-                        eh = !1, d0(g, n, d);
+                        Jd = !1, d0(g, n, d);
                         break;
                     case "selectionchange":
-                        if (Ek) break;
+                        if (ES) break;
                     case "keydown":
                     case "keyup":
                         d0(g, n, d)
                 }
-                var Y;
-                if (Hh) e: {
+                var $;
+                if (jh) e: {
                     switch (t) {
                         case "compositionstart":
-                            var V = "onCompositionStart";
+                            var Y = "onCompositionStart";
                             break e;
                         case "compositionend":
-                            V = "onCompositionEnd";
+                            Y = "onCompositionEnd";
                             break e;
                         case "compositionupdate":
-                            V = "onCompositionUpdate";
+                            Y = "onCompositionUpdate";
                             break e
                     }
-                    V = void 0
+                    Y = void 0
                 }
-                else os ? Dy(t, n) && (V = "onCompositionEnd") : t === "keydown" && n.keyCode === 229 && (V = "onCompositionStart");V && (My && n.locale !== "ko" && (os || V !== "onCompositionStart" ? V === "onCompositionEnd" && os && (Y = Py()) : (kr = d, zh = "value" in kr ? kr.value : kr.textContent, os = !0)), h = Uu(c, V), 0 < h.length && (V = new r0(V, t, null, n, d), g.push({
-                    event: V,
+                else os ? My(t, n) && (Y = "onCompositionEnd") : t === "keydown" && n.keyCode === 229 && (Y = "onCompositionStart");Y && (Py && n.locale !== "ko" && (os || Y !== "onCompositionStart" ? Y === "onCompositionEnd" && os && ($ = Dy()) : (Sr = d, Nh = "value" in Sr ? Sr.value : Sr.textContent, os = !0)), h = $u(c, Y), 0 < h.length && (Y = new r0(Y, t, null, n, d), g.push({
+                    event: Y,
                     listeners: h
-                }), Y ? V.data = Y : (Y = Oy(n), Y !== null && (V.data = Y)))),
-                (Y = pk ? gk(t, n) : mk(t, n)) && (c = Uu(c, "onBeforeInput"), 0 < c.length && (d = new r0("onBeforeInput", "beforeinput", null, n, d), g.push({
+                }), $ ? Y.data = $ : ($ = Oy(n), $ !== null && (Y.data = $)))),
+                ($ = pS ? gS(t, n) : mS(t, n)) && (c = $u(c, "onBeforeInput"), 0 < c.length && (d = new r0("onBeforeInput", "beforeinput", null, n, d), g.push({
                     event: d,
                     listeners: c
-                }), d.data = Y))
+                }), d.data = $))
             }
             Vy(g, e)
         })
     }
 
-    function Xa(t, e, n) {
+    function qa(t, e, n) {
         return {
             instance: t,
             listener: e,
             currentTarget: n
         }
     }
 
-    function Uu(t, e) {
+    function $u(t, e) {
         for (var n = e + "Capture", i = []; t !== null;) {
             var r = t,
                 o = r.stateNode;
-            r.tag === 5 && o !== null && (r = o, o = Ha(t, n), o != null && i.unshift(Xa(t, o, r)), o = Ha(t, e), o != null && i.push(Xa(t, o, r))), t = t.return
+            r.tag === 5 && o !== null && (r = o, o = Ba(t, n), o != null && i.unshift(qa(t, o, r)), o = Ba(t, e), o != null && i.push(qa(t, o, r))), t = t.return
         }
         return i
     }
 
     function ns(t) {
         if (t === null) return null;
         do t = t.return; while (t && t.tag !== 5);
@@ -2807,72 +2807,72 @@
 
     function y0(t, e, n, i, r) {
         for (var o = e._reactName, s = []; n !== null && n !== i;) {
             var a = n,
                 l = a.alternate,
                 c = a.stateNode;
             if (l !== null && l === i) break;
-            a.tag === 5 && c !== null && (a = c, r ? (l = Ha(n, o), l != null && s.unshift(Xa(n, l, a))) : r || (l = Ha(n, o), l != null && s.push(Xa(n, l, a)))), n = n.return
+            a.tag === 5 && c !== null && (a = c, r ? (l = Ba(n, o), l != null && s.unshift(qa(n, l, a))) : r || (l = Ba(n, o), l != null && s.push(qa(n, l, a)))), n = n.return
         }
         s.length !== 0 && t.push({
             event: e,
             listeners: s
         })
     }
-    var Pk = /\r\n?/g,
-        Mk = /\u0000|\uFFFD/g;
+    var DS = /\r\n?/g,
+        PS = /\u0000|\uFFFD/g;
 
     function v0(t) {
-        return (typeof t == "string" ? t : "" + t).replace(Pk, `
-`).replace(Mk, "")
+        return (typeof t == "string" ? t : "" + t).replace(DS, `
+`).replace(PS, "")
     }
 
-    function _u(t, e, n) {
-        if (e = v0(e), v0(t) !== e && n) throw Error(ne(425))
+    function wu(t, e, n) {
+        if (e = v0(e), v0(t) !== e && n) throw Error(te(425))
     }
 
-    function $u() {}
-    var th = null,
-        nh = null;
+    function Yu() {}
+    var eh = null,
+        th = null;
 
-    function ih(t, e) {
+    function nh(t, e) {
         return t === "textarea" || t === "noscript" || typeof e.children == "string" || typeof e.children == "number" || typeof e.dangerouslySetInnerHTML == "object" && e.dangerouslySetInnerHTML !== null && e.dangerouslySetInnerHTML.__html != null
     }
-    var rh = typeof setTimeout == "function" ? setTimeout : void 0,
-        Dk = typeof clearTimeout == "function" ? clearTimeout : void 0,
+    var ih = typeof setTimeout == "function" ? setTimeout : void 0,
+        MS = typeof clearTimeout == "function" ? clearTimeout : void 0,
         x0 = typeof Promise == "function" ? Promise : void 0,
-        Ok = typeof queueMicrotask == "function" ? queueMicrotask : typeof x0 < "u" ? function(t) {
-            return x0.resolve(null).then(t).catch(Ak)
-        } : rh;
+        OS = typeof queueMicrotask == "function" ? queueMicrotask : typeof x0 < "u" ? function(t) {
+            return x0.resolve(null).then(t).catch(AS)
+        } : ih;
 
-    function Ak(t) {
+    function AS(t) {
         setTimeout(function() {
             throw t
         })
     }
 
     function Sd(t, e) {
         var n = e,
             i = 0;
         do {
             var r = n.nextSibling;
             if (t.removeChild(n), r && r.nodeType === 8)
                 if (n = r.data, n === "/$") {
                     if (i === 0) {
-                        t.removeChild(r), Va(e);
+                        t.removeChild(r), Ua(e);
                         return
                     }
                     i--
                 } else n !== "$" && n !== "$?" && n !== "$!" || i++;
             n = r
         } while (n);
-        Va(e)
+        Ua(e)
     }
 
-    function Pr(t) {
+    function Dr(t) {
         for (; t != null; t = t.nextSibling) {
             var e = t.nodeType;
             if (e === 1 || e === 3) break;
             if (e === 8) {
                 if (e = t.data, e === "$" || e === "$!" || e === "$?") break;
                 if (e === "/$") return null
             }
@@ -2890,21 +2890,21 @@
                     e--
                 } else n === "/$" && e++
             }
             t = t.previousSibling
         }
         return null
     }
-    var Ms = Math.random().toString(36).slice(2),
-        _i = "__reactFiber$" + Ms,
-        qa = "__reactProps$" + Ms,
-        Zi = "__reactContainer$" + Ms,
-        oh = "__reactEvents$" + Ms,
-        Lk = "__reactListeners$" + Ms,
-        Rk = "__reactHandles$" + Ms;
+    var Ps = Math.random().toString(36).slice(2),
+        _i = "__reactFiber$" + Ps,
+        Za = "__reactProps$" + Ps,
+        Zi = "__reactContainer$" + Ps,
+        rh = "__reactEvents$" + Ps,
+        LS = "__reactListeners$" + Ps,
+        RS = "__reactHandles$" + Ps;
 
     function po(t) {
         var e = t[_i];
         if (e) return e;
         for (var n = t.parentNode; n;) {
             if (e = n[Zi] || n[_i]) {
                 if (n = e.alternate, e.child !== null || n !== null && n.child !== null)
@@ -2915,44 +2915,44 @@
                 return e
             }
             t = n, n = t.parentNode
         }
         return null
     }
 
-    function il(t) {
+    function rl(t) {
         return t = t[_i] || t[Zi], !t || t.tag !== 5 && t.tag !== 6 && t.tag !== 13 && t.tag !== 3 ? null : t
     }
 
     function ls(t) {
         if (t.tag === 5 || t.tag === 6) return t.stateNode;
-        throw Error(ne(33))
+        throw Error(te(33))
     }
 
-    function fc(t) {
-        return t[qa] || null
+    function dc(t) {
+        return t[Za] || null
     }
-    var sh = [],
+    var oh = [],
         us = -1;
 
     function Nr(t) {
         return {
             current: t
         }
     }
 
     function it(t) {
-        0 > us || (t.current = sh[us], sh[us] = null, us--)
+        0 > us || (t.current = oh[us], oh[us] = null, us--)
     }
 
     function et(t, e) {
-        us++, sh[us] = t.current, t.current = e
+        us++, oh[us] = t.current, t.current = e
     }
     var Rr = {},
-        Kt = Nr(Rr),
+        Qt = Nr(Rr),
         mn = Nr(!1),
         xo = Rr;
 
     function ws(t, e) {
         var n = t.type.contextTypes;
         if (!n) return Rr;
         var i = t.stateNode;
@@ -2963,85 +2963,85 @@
         return i && (t = t.stateNode, t.__reactInternalMemoizedUnmaskedChildContext = e, t.__reactInternalMemoizedMaskedChildContext = r), r
     }
 
     function yn(t) {
         return t = t.childContextTypes, t != null
     }
 
-    function Yu() {
-        it(mn), it(Kt)
+    function Xu() {
+        it(mn), it(Qt)
     }
 
     function _0(t, e, n) {
-        if (Kt.current !== Rr) throw Error(ne(168));
-        et(Kt, e), et(mn, n)
+        if (Qt.current !== Rr) throw Error(te(168));
+        et(Qt, e), et(mn, n)
     }
 
     function $y(t, e, n) {
         var i = t.stateNode;
         if (e = e.childContextTypes, typeof i.getChildContext != "function") return n;
         i = i.getChildContext();
         for (var r in i)
-            if (!(r in e)) throw Error(ne(108, bw(t) || "Unknown", r));
+            if (!(r in e)) throw Error(te(108, bw(t) || "Unknown", r));
         return ht({}, n, i)
     }
 
-    function Xu(t) {
-        return t = (t = t.stateNode) && t.__reactInternalMemoizedMergedChildContext || Rr, xo = Kt.current, et(Kt, t), et(mn, mn.current), !0
+    function qu(t) {
+        return t = (t = t.stateNode) && t.__reactInternalMemoizedMergedChildContext || Rr, xo = Qt.current, et(Qt, t), et(mn, mn.current), !0
     }
 
     function w0(t, e, n) {
         var i = t.stateNode;
-        if (!i) throw Error(ne(169));
-        n ? (t = $y(t, e, xo), i.__reactInternalMemoizedMergedChildContext = t, it(mn), it(Kt), et(Kt, t)) : it(mn), et(mn, n)
+        if (!i) throw Error(te(169));
+        n ? (t = $y(t, e, xo), i.__reactInternalMemoizedMergedChildContext = t, it(mn), it(Qt), et(Qt, t)) : it(mn), et(mn, n)
     }
     var Ui = null,
-        dc = !1,
-        Cd = !1;
+        hc = !1,
+        kd = !1;
 
     function Yy(t) {
         Ui === null ? Ui = [t] : Ui.push(t)
     }
 
-    function Ik(t) {
-        dc = !0, Yy(t)
+    function IS(t) {
+        hc = !0, Yy(t)
     }
 
     function zr() {
-        if (!Cd && Ui !== null) {
-            Cd = !0;
+        if (!kd && Ui !== null) {
+            kd = !0;
             var t = 0,
                 e = Be;
             try {
                 var n = Ui;
                 for (Be = 1; t < n.length; t++) {
                     var i = n[t];
                     do i = i(!0); while (i !== null)
                 }
-                Ui = null, dc = !1
+                Ui = null, hc = !1
             } catch (r) {
-                throw Ui !== null && (Ui = Ui.slice(t + 1)), yy(Lh, zr), r
+                throw Ui !== null && (Ui = Ui.slice(t + 1)), yy(Ah, zr), r
             } finally {
-                Be = e, Cd = !1
+                Be = e, kd = !1
             }
         }
         return null
     }
     var cs = [],
         fs = 0,
-        qu = null,
-        Zu = 0,
+        Zu = null,
+        Ku = 0,
         Un = [],
         $n = 0,
         bo = null,
         $i = 1,
         Yi = "";
 
     function fo(t, e) {
-        cs[fs++] = Zu, cs[fs++] = qu, qu = t, Zu = e
+        cs[fs++] = Ku, cs[fs++] = Zu, Zu = t, Ku = e
     }
 
     function Xy(t, e, n) {
         Un[$n++] = $i, Un[$n++] = Yi, Un[$n++] = bo, bo = t;
         var i = $i;
         t = Yi;
         var r = 32 - si(i) - 1;
@@ -3049,37 +3049,37 @@
         var o = 32 - si(e) + r;
         if (30 < o) {
             var s = r - r % 5;
             o = (i & (1 << s) - 1).toString(32), i >>= s, r -= s, $i = 1 << 32 - si(e) + r | n << r | i, Yi = o + t
         } else $i = 1 << o | n << r | i, Yi = t
     }
 
-    function Wh(t) {
+    function Bh(t) {
         t.return !== null && (fo(t, 1), Xy(t, 1, 0))
     }
 
-    function Vh(t) {
-        for (; t === qu;) qu = cs[--fs], cs[fs] = null, Zu = cs[--fs], cs[fs] = null;
+    function Wh(t) {
+        for (; t === Zu;) Zu = cs[--fs], cs[fs] = null, Ku = cs[--fs], cs[fs] = null;
         for (; t === bo;) bo = Un[--$n], Un[$n] = null, Yi = Un[--$n], Un[$n] = null, $i = Un[--$n], Un[$n] = null
     }
     var Ln = null,
         An = null,
         at = !1,
         oi = null;
 
     function qy(t, e) {
         var n = Yn(5, null, null, 0);
         n.elementType = "DELETED", n.stateNode = e, n.return = t, e = t.deletions, e === null ? (t.deletions = [n], t.flags |= 16) : e.push(n)
     }
 
-    function k0(t, e) {
+    function S0(t, e) {
         switch (t.tag) {
             case 5:
                 var n = t.type;
-                return e = e.nodeType !== 1 || n.toLowerCase() !== e.nodeName.toLowerCase() ? null : e, e !== null ? (t.stateNode = e, Ln = t, An = Pr(e.firstChild), !0) : !1;
+                return e = e.nodeType !== 1 || n.toLowerCase() !== e.nodeName.toLowerCase() ? null : e, e !== null ? (t.stateNode = e, Ln = t, An = Dr(e.firstChild), !0) : !1;
             case 6:
                 return e = t.pendingProps === "" || e.nodeType !== 3 ? null : e, e !== null ? (t.stateNode = e, Ln = t, An = null, !0) : !1;
             case 13:
                 return e = e.nodeType !== 8 ? null : e, e !== null ? (n = bo !== null ? {
                     id: $i,
                     overflow: Yi
                 } : null, t.memoizedState = {
@@ -3088,168 +3088,168 @@
                     retryLane: 1073741824
                 }, n = Yn(18, null, null, 0), n.stateNode = e, n.return = t, t.child = n, Ln = t, An = null, !0) : !1;
             default:
                 return !1
         }
     }
 
-    function ah(t) {
+    function sh(t) {
         return (t.mode & 1) !== 0 && (t.flags & 128) === 0
     }
 
-    function lh(t) {
+    function ah(t) {
         if (at) {
             var e = An;
             if (e) {
                 var n = e;
-                if (!k0(t, e)) {
-                    if (ah(t)) throw Error(ne(418));
-                    e = Pr(n.nextSibling);
+                if (!S0(t, e)) {
+                    if (sh(t)) throw Error(te(418));
+                    e = Dr(n.nextSibling);
                     var i = Ln;
-                    e && k0(t, e) ? qy(i, n) : (t.flags = t.flags & -4097 | 2, at = !1, Ln = t)
+                    e && S0(t, e) ? qy(i, n) : (t.flags = t.flags & -4097 | 2, at = !1, Ln = t)
                 }
             } else {
-                if (ah(t)) throw Error(ne(418));
+                if (sh(t)) throw Error(te(418));
                 t.flags = t.flags & -4097 | 2, at = !1, Ln = t
             }
         }
     }
 
-    function S0(t) {
+    function k0(t) {
         for (t = t.return; t !== null && t.tag !== 5 && t.tag !== 3 && t.tag !== 13;) t = t.return;
         Ln = t
     }
 
-    function wu(t) {
+    function Su(t) {
         if (t !== Ln) return !1;
-        if (!at) return S0(t), at = !0, !1;
+        if (!at) return k0(t), at = !0, !1;
         var e;
-        if ((e = t.tag !== 3) && !(e = t.tag !== 5) && (e = t.type, e = e !== "head" && e !== "body" && !ih(t.type, t.memoizedProps)), e && (e = An)) {
-            if (ah(t)) throw Zy(), Error(ne(418));
-            for (; e;) qy(t, e), e = Pr(e.nextSibling)
+        if ((e = t.tag !== 3) && !(e = t.tag !== 5) && (e = t.type, e = e !== "head" && e !== "body" && !nh(t.type, t.memoizedProps)), e && (e = An)) {
+            if (sh(t)) throw Zy(), Error(te(418));
+            for (; e;) qy(t, e), e = Dr(e.nextSibling)
         }
-        if (S0(t), t.tag === 13) {
-            if (t = t.memoizedState, t = t !== null ? t.dehydrated : null, !t) throw Error(ne(317));
+        if (k0(t), t.tag === 13) {
+            if (t = t.memoizedState, t = t !== null ? t.dehydrated : null, !t) throw Error(te(317));
             e: {
                 for (t = t.nextSibling, e = 0; t;) {
                     if (t.nodeType === 8) {
                         var n = t.data;
                         if (n === "/$") {
                             if (e === 0) {
-                                An = Pr(t.nextSibling);
+                                An = Dr(t.nextSibling);
                                 break e
                             }
                             e--
                         } else n !== "$" && n !== "$!" && n !== "$?" || e++
                     }
                     t = t.nextSibling
                 }
                 An = null
             }
-        } else An = Ln ? Pr(t.stateNode.nextSibling) : null;
+        } else An = Ln ? Dr(t.stateNode.nextSibling) : null;
         return !0
     }
 
     function Zy() {
-        for (var t = An; t;) t = Pr(t.nextSibling)
+        for (var t = An; t;) t = Dr(t.nextSibling)
     }
 
-    function ks() {
+    function Ss() {
         An = Ln = null, at = !1
     }
 
-    function Uh(t) {
+    function Vh(t) {
         oi === null ? oi = [t] : oi.push(t)
     }
-    var Nk = Ki.ReactCurrentBatchConfig;
+    var NS = Qi.ReactCurrentBatchConfig;
 
     function ii(t, e) {
         if (t && t.defaultProps) {
             e = ht({}, e), t = t.defaultProps;
             for (var n in t) e[n] === void 0 && (e[n] = t[n]);
             return e
         }
         return e
     }
     var Gu = Nr(null),
         Qu = null,
         ds = null,
-        $h = null;
+        Uh = null;
 
-    function Yh() {
-        $h = ds = Qu = null
+    function $h() {
+        Uh = ds = Qu = null
     }
 
-    function Xh(t) {
+    function Yh(t) {
         var e = Gu.current;
         it(Gu), t._currentValue = e
     }
 
-    function uh(t, e, n) {
+    function lh(t, e, n) {
         for (; t !== null;) {
             var i = t.alternate;
             if ((t.childLanes & e) !== e ? (t.childLanes |= e, i !== null && (i.childLanes |= e)) : i !== null && (i.childLanes & e) !== e && (i.childLanes |= e), t === n) break;
             t = t.return
         }
     }
 
     function xs(t, e) {
-        Qu = t, $h = ds = null, t = t.dependencies, t !== null && t.firstContext !== null && (t.lanes & e && (gn = !0), t.firstContext = null)
+        Qu = t, Uh = ds = null, t = t.dependencies, t !== null && t.firstContext !== null && (t.lanes & e && (gn = !0), t.firstContext = null)
     }
 
     function qn(t) {
         var e = t._currentValue;
-        if ($h !== t)
+        if (Uh !== t)
             if (t = {
                     context: t,
                     memoizedValue: e,
                     next: null
                 }, ds === null) {
-                if (Qu === null) throw Error(ne(308));
+                if (Qu === null) throw Error(te(308));
                 ds = t, Qu.dependencies = {
                     lanes: 0,
                     firstContext: t
                 }
             } else ds = ds.next = t;
         return e
     }
     var go = null;
 
-    function qh(t) {
+    function Xh(t) {
         go === null ? go = [t] : go.push(t)
     }
 
-    function Gy(t, e, n, i) {
+    function Ky(t, e, n, i) {
         var r = e.interleaved;
-        return r === null ? (n.next = n, qh(e)) : (n.next = r.next, r.next = n), e.interleaved = n, Gi(t, i)
+        return r === null ? (n.next = n, Xh(e)) : (n.next = r.next, r.next = n), e.interleaved = n, Ki(t, i)
     }
 
-    function Gi(t, e) {
+    function Ki(t, e) {
         t.lanes |= e;
         var n = t.alternate;
         for (n !== null && (n.lanes |= e), n = t, t = t.return; t !== null;) t.childLanes |= e, n = t.alternate, n !== null && (n.childLanes |= e), n = t, t = t.return;
         return n.tag === 3 ? n.stateNode : null
     }
     var br = !1;
 
-    function Zh(t) {
+    function qh(t) {
         t.updateQueue = {
             baseState: t.memoizedState,
             firstBaseUpdate: null,
             lastBaseUpdate: null,
             shared: {
                 pending: null,
                 interleaved: null,
                 lanes: 0
             },
             effects: null
         }
     }
 
-    function Qy(t, e) {
+    function Gy(t, e) {
         t = t.updateQueue, e.updateQueue === t && (e.updateQueue = {
             baseState: t.baseState,
             firstBaseUpdate: t.firstBaseUpdate,
             lastBaseUpdate: t.lastBaseUpdate,
             shared: t.shared,
             effects: t.effects
         })
@@ -3262,28 +3262,28 @@
             tag: 0,
             payload: null,
             callback: null,
             next: null
         }
     }
 
-    function Mr(t, e, n) {
+    function Pr(t, e, n) {
         var i = t.updateQueue;
         if (i === null) return null;
         if (i = i.shared, Ne & 2) {
             var r = i.pending;
-            return r === null ? e.next = e : (e.next = r.next, r.next = e), i.pending = e, Gi(t, n)
+            return r === null ? e.next = e : (e.next = r.next, r.next = e), i.pending = e, Ki(t, n)
         }
-        return r = i.interleaved, r === null ? (e.next = e, qh(i)) : (e.next = r.next, r.next = e), i.interleaved = e, Gi(t, n)
+        return r = i.interleaved, r === null ? (e.next = e, Xh(i)) : (e.next = r.next, r.next = e), i.interleaved = e, Ki(t, n)
     }
 
-    function Du(t, e, n) {
+    function Ou(t, e, n) {
         if (e = e.updateQueue, e !== null && (e = e.shared, (n & 4194240) !== 0)) {
             var i = e.lanes;
-            i &= t.pendingLanes, n |= i, e.lanes = n, Rh(t, n)
+            i &= t.pendingLanes, n |= i, e.lanes = n, Lh(t, n)
         }
     }
 
     function C0(t, e) {
         var n = t.updateQueue,
             i = t.alternate;
         if (i !== null && (i = i.updateQueue, n === i)) {
@@ -3311,15 +3311,15 @@
                 effects: i.effects
             }, t.updateQueue = n;
             return
         }
         t = n.lastBaseUpdate, t === null ? n.firstBaseUpdate = e : t.next = e, n.lastBaseUpdate = e
     }
 
-    function Ku(t, e, n, i) {
+    function Ju(t, e, n, i) {
         var r = t.updateQueue;
         br = !1;
         var o = r.firstBaseUpdate,
             s = r.lastBaseUpdate,
             a = r.shared.pending;
         if (a !== null) {
             r.shared.pending = null;
@@ -3341,28 +3341,28 @@
                         lane: 0,
                         tag: a.tag,
                         payload: a.payload,
                         callback: a.callback,
                         next: null
                     });
                     e: {
-                        var w = t,
-                            S = a;
-                        switch (y = e, x = n, S.tag) {
+                        var _ = t,
+                            C = a;
+                        switch (y = e, x = n, C.tag) {
                             case 1:
-                                if (w = S.payload, typeof w == "function") {
-                                    g = w.call(x, g, y);
+                                if (_ = C.payload, typeof _ == "function") {
+                                    g = _.call(x, g, y);
                                     break e
                                 }
-                                g = w;
+                                g = _;
                                 break e;
                             case 3:
-                                w.flags = w.flags & -65537 | 128;
+                                _.flags = _.flags & -65537 | 128;
                             case 0:
-                                if (w = S.payload, y = typeof w == "function" ? w.call(x, g, y) : w, y == null) break e;
+                                if (_ = C.payload, y = typeof _ == "function" ? _.call(x, g, y) : _, y == null) break e;
                                 g = ht({}, g, y);
                                 break e;
                             case 2:
                                 br = !0
                         }
                     }
                     a.callback !== null && a.lane !== 0 && (t.flags |= 64, y = r.effects, y === null ? r.effects = [a] : y.push(a))
@@ -3389,345 +3389,345 @@
 
     function E0(t, e, n) {
         if (t = e.effects, e.effects = null, t !== null)
             for (e = 0; e < t.length; e++) {
                 var i = t[e],
                     r = i.callback;
                 if (r !== null) {
-                    if (i.callback = null, i = n, typeof r != "function") throw Error(ne(191, r));
+                    if (i.callback = null, i = n, typeof r != "function") throw Error(te(191, r));
                     r.call(i)
                 }
             }
     }
-    var Ky = new G0.Component().refs;
+    var Qy = new K0.Component().refs;
 
-    function ch(t, e, n, i) {
+    function uh(t, e, n, i) {
         e = t.memoizedState, n = n(i, e), n = n == null ? e : ht({}, e, n), t.memoizedState = n, t.lanes === 0 && (t.updateQueue.baseState = n)
     }
-    var hc = {
+    var pc = {
         isMounted: function(t) {
             return (t = t._reactInternals) ? Co(t) === t : !1
         },
         enqueueSetState: function(t, e, n) {
             t = t._reactInternals;
             var i = nn(),
                 r = Or(t),
                 o = Xi(i, r);
-            o.payload = e, n != null && (o.callback = n), e = Mr(t, o, r), e !== null && (ai(e, t, r, i), Du(e, t, r))
+            o.payload = e, n != null && (o.callback = n), e = Pr(t, o, r), e !== null && (ai(e, t, r, i), Ou(e, t, r))
         },
         enqueueReplaceState: function(t, e, n) {
             t = t._reactInternals;
             var i = nn(),
                 r = Or(t),
                 o = Xi(i, r);
-            o.tag = 1, o.payload = e, n != null && (o.callback = n), e = Mr(t, o, r), e !== null && (ai(e, t, r, i), Du(e, t, r))
+            o.tag = 1, o.payload = e, n != null && (o.callback = n), e = Pr(t, o, r), e !== null && (ai(e, t, r, i), Ou(e, t, r))
         },
         enqueueForceUpdate: function(t, e) {
             t = t._reactInternals;
             var n = nn(),
                 i = Or(t),
                 r = Xi(n, i);
-            r.tag = 2, e != null && (r.callback = e), e = Mr(t, r, i), e !== null && (ai(e, t, i, n), Du(e, t, i))
+            r.tag = 2, e != null && (r.callback = e), e = Pr(t, r, i), e !== null && (ai(e, t, i, n), Ou(e, t, i))
         }
     };
 
     function T0(t, e, n, i, r, o, s) {
-        return t = t.stateNode, typeof t.shouldComponentUpdate == "function" ? t.shouldComponentUpdate(i, o, s) : e.prototype && e.prototype.isPureReactComponent ? !$a(n, i) || !$a(r, o) : !0
+        return t = t.stateNode, typeof t.shouldComponentUpdate == "function" ? t.shouldComponentUpdate(i, o, s) : e.prototype && e.prototype.isPureReactComponent ? !Ya(n, i) || !Ya(r, o) : !0
     }
 
     function Jy(t, e, n) {
         var i = !1,
             r = Rr,
             o = e.contextType;
-        return typeof o == "object" && o !== null ? o = qn(o) : (r = yn(e) ? xo : Kt.current, i = e.contextTypes, o = (i = i != null) ? ws(t, r) : Rr), e = new e(n, o), t.memoizedState = e.state !== null && e.state !== void 0 ? e.state : null, e.updater = hc, t.stateNode = e, e._reactInternals = t, i && (t = t.stateNode, t.__reactInternalMemoizedUnmaskedChildContext = r, t.__reactInternalMemoizedMaskedChildContext = o), e
+        return typeof o == "object" && o !== null ? o = qn(o) : (r = yn(e) ? xo : Qt.current, i = e.contextTypes, o = (i = i != null) ? ws(t, r) : Rr), e = new e(n, o), t.memoizedState = e.state !== null && e.state !== void 0 ? e.state : null, e.updater = pc, t.stateNode = e, e._reactInternals = t, i && (t = t.stateNode, t.__reactInternalMemoizedUnmaskedChildContext = r, t.__reactInternalMemoizedMaskedChildContext = o), e
     }
 
-    function P0(t, e, n, i) {
-        t = e.state, typeof e.componentWillReceiveProps == "function" && e.componentWillReceiveProps(n, i), typeof e.UNSAFE_componentWillReceiveProps == "function" && e.UNSAFE_componentWillReceiveProps(n, i), e.state !== t && hc.enqueueReplaceState(e, e.state, null)
+    function D0(t, e, n, i) {
+        t = e.state, typeof e.componentWillReceiveProps == "function" && e.componentWillReceiveProps(n, i), typeof e.UNSAFE_componentWillReceiveProps == "function" && e.UNSAFE_componentWillReceiveProps(n, i), e.state !== t && pc.enqueueReplaceState(e, e.state, null)
     }
 
-    function fh(t, e, n, i) {
+    function ch(t, e, n, i) {
         var r = t.stateNode;
-        r.props = n, r.state = t.memoizedState, r.refs = Ky, Zh(t);
+        r.props = n, r.state = t.memoizedState, r.refs = Qy, qh(t);
         var o = e.contextType;
-        typeof o == "object" && o !== null ? r.context = qn(o) : (o = yn(e) ? xo : Kt.current, r.context = ws(t, o)), r.state = t.memoizedState, o = e.getDerivedStateFromProps, typeof o == "function" && (ch(t, e, o, n), r.state = t.memoizedState), typeof e.getDerivedStateFromProps == "function" || typeof r.getSnapshotBeforeUpdate == "function" || typeof r.UNSAFE_componentWillMount != "function" && typeof r.componentWillMount != "function" || (e = r.state, typeof r.componentWillMount == "function" && r.componentWillMount(), typeof r.UNSAFE_componentWillMount == "function" && r.UNSAFE_componentWillMount(), e !== r.state && hc.enqueueReplaceState(r, r.state, null), Ku(t, n, r, i), r.state = t.memoizedState), typeof r.componentDidMount == "function" && (t.flags |= 4194308)
+        typeof o == "object" && o !== null ? r.context = qn(o) : (o = yn(e) ? xo : Qt.current, r.context = ws(t, o)), r.state = t.memoizedState, o = e.getDerivedStateFromProps, typeof o == "function" && (uh(t, e, o, n), r.state = t.memoizedState), typeof e.getDerivedStateFromProps == "function" || typeof r.getSnapshotBeforeUpdate == "function" || typeof r.UNSAFE_componentWillMount != "function" && typeof r.componentWillMount != "function" || (e = r.state, typeof r.componentWillMount == "function" && r.componentWillMount(), typeof r.UNSAFE_componentWillMount == "function" && r.UNSAFE_componentWillMount(), e !== r.state && pc.enqueueReplaceState(r, r.state, null), Ju(t, n, r, i), r.state = t.memoizedState), typeof r.componentDidMount == "function" && (t.flags |= 4194308)
     }
 
-    function _a(t, e, n) {
+    function wa(t, e, n) {
         if (t = n.ref, t !== null && typeof t != "function" && typeof t != "object") {
             if (n._owner) {
                 if (n = n._owner, n) {
-                    if (n.tag !== 1) throw Error(ne(309));
+                    if (n.tag !== 1) throw Error(te(309));
                     var i = n.stateNode
                 }
-                if (!i) throw Error(ne(147, t));
+                if (!i) throw Error(te(147, t));
                 var r = i,
                     o = "" + t;
                 return e !== null && e.ref !== null && typeof e.ref == "function" && e.ref._stringRef === o ? e.ref : (e = function(s) {
                     var a = r.refs;
-                    a === Ky && (a = r.refs = {}), s === null ? delete a[o] : a[o] = s
+                    a === Qy && (a = r.refs = {}), s === null ? delete a[o] : a[o] = s
                 }, e._stringRef = o, e)
             }
-            if (typeof t != "string") throw Error(ne(284));
-            if (!n._owner) throw Error(ne(290, t))
+            if (typeof t != "string") throw Error(te(284));
+            if (!n._owner) throw Error(te(290, t))
         }
         return t
     }
 
     function ku(t, e) {
-        throw t = Object.prototype.toString.call(e), Error(ne(31, t === "[object Object]" ? "object with keys {" + Object.keys(e).join(", ") + "}" : t))
+        throw t = Object.prototype.toString.call(e), Error(te(31, t === "[object Object]" ? "object with keys {" + Object.keys(e).join(", ") + "}" : t))
     }
 
-    function M0(t) {
+    function P0(t) {
         var e = t._init;
         return e(t._payload)
     }
 
     function ev(t) {
-        function e(_, C) {
+        function e(w, k) {
             if (t) {
-                var M = _.deletions;
-                M === null ? (_.deletions = [C], _.flags |= 16) : M.push(C)
+                var P = w.deletions;
+                P === null ? (w.deletions = [k], w.flags |= 16) : P.push(k)
             }
         }
 
-        function n(_, C) {
+        function n(w, k) {
             if (!t) return null;
-            for (; C !== null;) e(_, C), C = C.sibling;
+            for (; k !== null;) e(w, k), k = k.sibling;
             return null
         }
 
-        function i(_, C) {
-            for (_ = new Map; C !== null;) C.key !== null ? _.set(C.key, C) : _.set(C.index, C), C = C.sibling;
-            return _
+        function i(w, k) {
+            for (w = new Map; k !== null;) k.key !== null ? w.set(k.key, k) : w.set(k.index, k), k = k.sibling;
+            return w
         }
 
-        function r(_, C) {
-            return _ = Ar(_, C), _.index = 0, _.sibling = null, _
+        function r(w, k) {
+            return w = Ar(w, k), w.index = 0, w.sibling = null, w
         }
 
-        function o(_, C, M) {
-            return _.index = M, t ? (M = _.alternate, M !== null ? (M = M.index, M < C ? (_.flags |= 2, C) : M) : (_.flags |= 2, C)) : (_.flags |= 1048576, C)
+        function o(w, k, P) {
+            return w.index = P, t ? (P = w.alternate, P !== null ? (P = P.index, P < k ? (w.flags |= 2, k) : P) : (w.flags |= 2, k)) : (w.flags |= 1048576, k)
         }
 
-        function s(_) {
-            return t && _.alternate === null && (_.flags |= 2), _
+        function s(w) {
+            return t && w.alternate === null && (w.flags |= 2), w
         }
 
-        function a(_, C, M, z) {
-            return C === null || C.tag !== 6 ? (C = Ad(M, _.mode, z), C.return = _, C) : (C = r(C, M), C.return = _, C)
+        function a(w, k, P, z) {
+            return k === null || k.tag !== 6 ? (k = Od(P, w.mode, z), k.return = w, k) : (k = r(k, P), k.return = w, k)
         }
 
-        function l(_, C, M, z) {
-            var F = M.type;
-            return F === rs ? d(_, C, M.props.children, z, M.key) : C !== null && (C.elementType === F || typeof F == "object" && F !== null && F.$$typeof === xr && M0(F) === C.type) ? (z = r(C, M.props), z.ref = _a(_, C, M), z.return = _, z) : (z = Nu(M.type, M.key, M.props, null, _.mode, z), z.ref = _a(_, C, M), z.return = _, z)
+        function l(w, k, P, z) {
+            var F = P.type;
+            return F === rs ? d(w, k, P.props.children, z, P.key) : k !== null && (k.elementType === F || typeof F == "object" && F !== null && F.$$typeof === xr && P0(F) === k.type) ? (z = r(k, P.props), z.ref = wa(w, k, P), z.return = w, z) : (z = zu(P.type, P.key, P.props, null, w.mode, z), z.ref = wa(w, k, P), z.return = w, z)
         }
 
-        function c(_, C, M, z) {
-            return C === null || C.tag !== 4 || C.stateNode.containerInfo !== M.containerInfo || C.stateNode.implementation !== M.implementation ? (C = Ld(M, _.mode, z), C.return = _, C) : (C = r(C, M.children || []), C.return = _, C)
+        function c(w, k, P, z) {
+            return k === null || k.tag !== 4 || k.stateNode.containerInfo !== P.containerInfo || k.stateNode.implementation !== P.implementation ? (k = Ad(P, w.mode, z), k.return = w, k) : (k = r(k, P.children || []), k.return = w, k)
         }
 
-        function d(_, C, M, z, F) {
-            return C === null || C.tag !== 7 ? (C = vo(M, _.mode, z, F), C.return = _, C) : (C = r(C, M), C.return = _, C)
+        function d(w, k, P, z, F) {
+            return k === null || k.tag !== 7 ? (k = vo(P, w.mode, z, F), k.return = w, k) : (k = r(k, P), k.return = w, k)
         }
 
-        function g(_, C, M) {
-            if (typeof C == "string" && C !== "" || typeof C == "number") return C = Ad("" + C, _.mode, M), C.return = _, C;
-            if (typeof C == "object" && C !== null) {
-                switch (C.$$typeof) {
-                    case lu:
-                        return M = Nu(C.type, C.key, C.props, null, _.mode, M), M.ref = _a(_, null, C), M.return = _, M;
+        function g(w, k, P) {
+            if (typeof k == "string" && k !== "" || typeof k == "number") return k = Od("" + k, w.mode, P), k.return = w, k;
+            if (typeof k == "object" && k !== null) {
+                switch (k.$$typeof) {
+                    case uu:
+                        return P = zu(k.type, k.key, k.props, null, w.mode, P), P.ref = wa(w, null, k), P.return = w, P;
                     case is:
-                        return C = Ld(C, _.mode, M), C.return = _, C;
+                        return k = Ad(k, w.mode, P), k.return = w, k;
                     case xr:
-                        var z = C._init;
-                        return g(_, z(C._payload), M)
+                        var z = k._init;
+                        return g(w, z(k._payload), P)
                 }
-                if (Ea(C) || ya(C)) return C = vo(C, _.mode, M, null), C.return = _, C;
-                ku(_, C)
+                if (Ta(k) || va(k)) return k = vo(k, w.mode, P, null), k.return = w, k;
+                ku(w, k)
             }
             return null
         }
 
-        function y(_, C, M, z) {
-            var F = C !== null ? C.key : null;
-            if (typeof M == "string" && M !== "" || typeof M == "number") return F !== null ? null : a(_, C, "" + M, z);
-            if (typeof M == "object" && M !== null) {
-                switch (M.$$typeof) {
-                    case lu:
-                        return M.key === F ? l(_, C, M, z) : null;
+        function y(w, k, P, z) {
+            var F = k !== null ? k.key : null;
+            if (typeof P == "string" && P !== "" || typeof P == "number") return F !== null ? null : a(w, k, "" + P, z);
+            if (typeof P == "object" && P !== null) {
+                switch (P.$$typeof) {
+                    case uu:
+                        return P.key === F ? l(w, k, P, z) : null;
                     case is:
-                        return M.key === F ? c(_, C, M, z) : null;
+                        return P.key === F ? c(w, k, P, z) : null;
                     case xr:
-                        return F = M._init, y(_, C, F(M._payload), z)
+                        return F = P._init, y(w, k, F(P._payload), z)
                 }
-                if (Ea(M) || ya(M)) return F !== null ? null : d(_, C, M, z, null);
-                ku(_, M)
+                if (Ta(P) || va(P)) return F !== null ? null : d(w, k, P, z, null);
+                ku(w, P)
             }
             return null
         }
 
-        function x(_, C, M, z, F) {
-            if (typeof z == "string" && z !== "" || typeof z == "number") return _ = _.get(M) || null, a(C, _, "" + z, F);
+        function x(w, k, P, z, F) {
+            if (typeof z == "string" && z !== "" || typeof z == "number") return w = w.get(P) || null, a(k, w, "" + z, F);
             if (typeof z == "object" && z !== null) {
                 switch (z.$$typeof) {
-                    case lu:
-                        return _ = _.get(z.key === null ? M : z.key) || null, l(C, _, z, F);
+                    case uu:
+                        return w = w.get(z.key === null ? P : z.key) || null, l(k, w, z, F);
                     case is:
-                        return _ = _.get(z.key === null ? M : z.key) || null, c(C, _, z, F);
+                        return w = w.get(z.key === null ? P : z.key) || null, c(k, w, z, F);
                     case xr:
                         var h = z._init;
-                        return x(_, C, M, h(z._payload), F)
+                        return x(w, k, P, h(z._payload), F)
                 }
-                if (Ea(z) || ya(z)) return _ = _.get(M) || null, d(C, _, z, F, null);
-                ku(C, z)
+                if (Ta(z) || va(z)) return w = w.get(P) || null, d(k, w, z, F, null);
+                ku(k, z)
             }
             return null
         }
 
-        function w(_, C, M, z) {
-            for (var F = null, h = null, Y = C, V = C = 0, te = null; Y !== null && V < M.length; V++) {
-                Y.index > V ? (te = Y, Y = null) : te = Y.sibling;
-                var ie = y(_, Y, M[V], z);
+        function _(w, k, P, z) {
+            for (var F = null, h = null, $ = k, Y = k = 0, ne = null; $ !== null && Y < P.length; Y++) {
+                $.index > Y ? (ne = $, $ = null) : ne = $.sibling;
+                var ie = y(w, $, P[Y], z);
                 if (ie === null) {
-                    Y === null && (Y = te);
+                    $ === null && ($ = ne);
                     break
                 }
-                t && Y && ie.alternate === null && e(_, Y), C = o(ie, C, V), h === null ? F = ie : h.sibling = ie, h = ie, Y = te
+                t && $ && ie.alternate === null && e(w, $), k = o(ie, k, Y), h === null ? F = ie : h.sibling = ie, h = ie, $ = ne
             }
-            if (V === M.length) return n(_, Y), at && fo(_, V), F;
-            if (Y === null) {
-                for (; V < M.length; V++) Y = g(_, M[V], z), Y !== null && (C = o(Y, C, V), h === null ? F = Y : h.sibling = Y, h = Y);
-                return at && fo(_, V), F
-            }
-            for (Y = i(_, Y); V < M.length; V++) te = x(Y, _, V, M[V], z), te !== null && (t && te.alternate !== null && Y.delete(te.key === null ? V : te.key), C = o(te, C, V), h === null ? F = te : h.sibling = te, h = te);
-            return t && Y.forEach(function(ce) {
-                return e(_, ce)
-            }), at && fo(_, V), F
-        }
-
-        function S(_, C, M, z) {
-            var F = ya(M);
-            if (typeof F != "function") throw Error(ne(150));
-            if (M = F.call(M), M == null) throw Error(ne(151));
-            for (var h = F = null, Y = C, V = C = 0, te = null, ie = M.next(); Y !== null && !ie.done; V++, ie = M.next()) {
-                Y.index > V ? (te = Y, Y = null) : te = Y.sibling;
-                var ce = y(_, Y, ie.value, z);
+            if (Y === P.length) return n(w, $), at && fo(w, Y), F;
+            if ($ === null) {
+                for (; Y < P.length; Y++) $ = g(w, P[Y], z), $ !== null && (k = o($, k, Y), h === null ? F = $ : h.sibling = $, h = $);
+                return at && fo(w, Y), F
+            }
+            for ($ = i(w, $); Y < P.length; Y++) ne = x($, w, Y, P[Y], z), ne !== null && (t && ne.alternate !== null && $.delete(ne.key === null ? Y : ne.key), k = o(ne, k, Y), h === null ? F = ne : h.sibling = ne, h = ne);
+            return t && $.forEach(function(ce) {
+                return e(w, ce)
+            }), at && fo(w, Y), F
+        }
+
+        function C(w, k, P, z) {
+            var F = va(P);
+            if (typeof F != "function") throw Error(te(150));
+            if (P = F.call(P), P == null) throw Error(te(151));
+            for (var h = F = null, $ = k, Y = k = 0, ne = null, ie = P.next(); $ !== null && !ie.done; Y++, ie = P.next()) {
+                $.index > Y ? (ne = $, $ = null) : ne = $.sibling;
+                var ce = y(w, $, ie.value, z);
                 if (ce === null) {
-                    Y === null && (Y = te);
+                    $ === null && ($ = ne);
                     break
                 }
-                t && Y && ce.alternate === null && e(_, Y), C = o(ce, C, V), h === null ? F = ce : h.sibling = ce, h = ce, Y = te
+                t && $ && ce.alternate === null && e(w, $), k = o(ce, k, Y), h === null ? F = ce : h.sibling = ce, h = ce, $ = ne
             }
-            if (ie.done) return n(_, Y), at && fo(_, V), F;
-            if (Y === null) {
-                for (; !ie.done; V++, ie = M.next()) ie = g(_, ie.value, z), ie !== null && (C = o(ie, C, V), h === null ? F = ie : h.sibling = ie, h = ie);
-                return at && fo(_, V), F
-            }
-            for (Y = i(_, Y); !ie.done; V++, ie = M.next()) ie = x(Y, _, V, ie.value, z), ie !== null && (t && ie.alternate !== null && Y.delete(ie.key === null ? V : ie.key), C = o(ie, C, V), h === null ? F = ie : h.sibling = ie, h = ie);
-            return t && Y.forEach(function(he) {
-                return e(_, he)
-            }), at && fo(_, V), F
-        }
-
-        function A(_, C, M, z) {
-            if (typeof M == "object" && M !== null && M.type === rs && M.key === null && (M = M.props.children), typeof M == "object" && M !== null) {
-                switch (M.$$typeof) {
-                    case lu:
+            if (ie.done) return n(w, $), at && fo(w, Y), F;
+            if ($ === null) {
+                for (; !ie.done; Y++, ie = P.next()) ie = g(w, ie.value, z), ie !== null && (k = o(ie, k, Y), h === null ? F = ie : h.sibling = ie, h = ie);
+                return at && fo(w, Y), F
+            }
+            for ($ = i(w, $); !ie.done; Y++, ie = P.next()) ie = x($, w, Y, ie.value, z), ie !== null && (t && ie.alternate !== null && $.delete(ie.key === null ? Y : ie.key), k = o(ie, k, Y), h === null ? F = ie : h.sibling = ie, h = ie);
+            return t && $.forEach(function(he) {
+                return e(w, he)
+            }), at && fo(w, Y), F
+        }
+
+        function A(w, k, P, z) {
+            if (typeof P == "object" && P !== null && P.type === rs && P.key === null && (P = P.props.children), typeof P == "object" && P !== null) {
+                switch (P.$$typeof) {
+                    case uu:
                         e: {
-                            for (var F = M.key, h = C; h !== null;) {
+                            for (var F = P.key, h = k; h !== null;) {
                                 if (h.key === F) {
-                                    if (F = M.type, F === rs) {
+                                    if (F = P.type, F === rs) {
                                         if (h.tag === 7) {
-                                            n(_, h.sibling), C = r(h, M.props.children), C.return = _, _ = C;
+                                            n(w, h.sibling), k = r(h, P.props.children), k.return = w, w = k;
                                             break e
                                         }
-                                    } else if (h.elementType === F || typeof F == "object" && F !== null && F.$$typeof === xr && M0(F) === h.type) {
-                                        n(_, h.sibling), C = r(h, M.props), C.ref = _a(_, h, M), C.return = _, _ = C;
+                                    } else if (h.elementType === F || typeof F == "object" && F !== null && F.$$typeof === xr && P0(F) === h.type) {
+                                        n(w, h.sibling), k = r(h, P.props), k.ref = wa(w, h, P), k.return = w, w = k;
                                         break e
                                     }
-                                    n(_, h);
+                                    n(w, h);
                                     break
-                                } else e(_, h);
+                                } else e(w, h);
                                 h = h.sibling
                             }
-                            M.type === rs ? (C = vo(M.props.children, _.mode, z, M.key), C.return = _, _ = C) : (z = Nu(M.type, M.key, M.props, null, _.mode, z), z.ref = _a(_, C, M), z.return = _, _ = z)
+                            P.type === rs ? (k = vo(P.props.children, w.mode, z, P.key), k.return = w, w = k) : (z = zu(P.type, P.key, P.props, null, w.mode, z), z.ref = wa(w, k, P), z.return = w, w = z)
                         }
-                        return s(_);
+                        return s(w);
                     case is:
                         e: {
-                            for (h = M.key; C !== null;) {
-                                if (C.key === h)
-                                    if (C.tag === 4 && C.stateNode.containerInfo === M.containerInfo && C.stateNode.implementation === M.implementation) {
-                                        n(_, C.sibling), C = r(C, M.children || []), C.return = _, _ = C;
+                            for (h = P.key; k !== null;) {
+                                if (k.key === h)
+                                    if (k.tag === 4 && k.stateNode.containerInfo === P.containerInfo && k.stateNode.implementation === P.implementation) {
+                                        n(w, k.sibling), k = r(k, P.children || []), k.return = w, w = k;
                                         break e
                                     } else {
-                                        n(_, C);
+                                        n(w, k);
                                         break
                                     }
-                                else e(_, C);
-                                C = C.sibling
+                                else e(w, k);
+                                k = k.sibling
                             }
-                            C = Ld(M, _.mode, z),
-                            C.return = _,
-                            _ = C
+                            k = Ad(P, w.mode, z),
+                            k.return = w,
+                            w = k
                         }
-                        return s(_);
+                        return s(w);
                     case xr:
-                        return h = M._init, A(_, C, h(M._payload), z)
+                        return h = P._init, A(w, k, h(P._payload), z)
                 }
-                if (Ea(M)) return w(_, C, M, z);
-                if (ya(M)) return S(_, C, M, z);
-                ku(_, M)
+                if (Ta(P)) return _(w, k, P, z);
+                if (va(P)) return C(w, k, P, z);
+                ku(w, P)
             }
-            return typeof M == "string" && M !== "" || typeof M == "number" ? (M = "" + M, C !== null && C.tag === 6 ? (n(_, C.sibling), C = r(C, M), C.return = _, _ = C) : (n(_, C), C = Ad(M, _.mode, z), C.return = _, _ = C), s(_)) : n(_, C)
+            return typeof P == "string" && P !== "" || typeof P == "number" ? (P = "" + P, k !== null && k.tag === 6 ? (n(w, k.sibling), k = r(k, P), k.return = w, w = k) : (n(w, k), k = Od(P, w.mode, z), k.return = w, w = k), s(w)) : n(w, k)
         }
         return A
     }
-    var Ss = ev(!0),
+    var ks = ev(!0),
         tv = ev(!1),
-        rl = {},
-        ki = Nr(rl),
-        Za = Nr(rl),
-        Ga = Nr(rl);
+        ol = {},
+        Si = Nr(ol),
+        Ka = Nr(ol),
+        Ga = Nr(ol);
 
     function mo(t) {
-        if (t === rl) throw Error(ne(174));
+        if (t === ol) throw Error(te(174));
         return t
     }
 
-    function Gh(t, e) {
-        switch (et(Ga, e), et(Za, t), et(ki, rl), t = e.nodeType, t) {
+    function Zh(t, e) {
+        switch (et(Ga, e), et(Ka, t), et(Si, ol), t = e.nodeType, t) {
             case 9:
             case 11:
-                e = (e = e.documentElement) ? e.namespaceURI : Vd(null, "");
+                e = (e = e.documentElement) ? e.namespaceURI : Wd(null, "");
                 break;
             default:
-                t = t === 8 ? e.parentNode : e, e = t.namespaceURI || null, t = t.tagName, e = Vd(e, t)
+                t = t === 8 ? e.parentNode : e, e = t.namespaceURI || null, t = t.tagName, e = Wd(e, t)
         }
-        it(ki), et(ki, e)
+        it(Si), et(Si, e)
     }
 
     function Cs() {
-        it(ki), it(Za), it(Ga)
+        it(Si), it(Ka), it(Ga)
     }
 
     function nv(t) {
         mo(Ga.current);
-        var e = mo(ki.current),
-            n = Vd(e, t.type);
-        e !== n && (et(Za, t), et(ki, n))
+        var e = mo(Si.current),
+            n = Wd(e, t.type);
+        e !== n && (et(Ka, t), et(Si, n))
     }
 
-    function Qh(t) {
-        Za.current === t && (it(ki), it(Za))
+    function Kh(t) {
+        Ka.current === t && (it(Si), it(Ka))
     }
     var ft = Nr(0);
 
-    function Ju(t) {
+    function ec(t) {
         for (var e = t; e !== null;) {
             if (e.tag === 13) {
                 var n = e.memoizedState;
                 if (n !== null && (n = n.dehydrated, n === null || n.data === "$?" || n.data === "$!")) return e
             } else if (e.tag === 19 && e.memoizedProps.revealOrder !== void 0) {
                 if (e.flags & 128) return e
             } else if (e.child !== null) {
@@ -3739,55 +3739,55 @@
                 if (e.return === null || e.return === t) return null;
                 e = e.return
             }
             e.sibling.return = e.return, e = e.sibling
         }
         return null
     }
-    var Ed = [];
+    var Cd = [];
 
-    function Kh() {
-        for (var t = 0; t < Ed.length; t++) Ed[t]._workInProgressVersionPrimary = null;
-        Ed.length = 0
+    function Gh() {
+        for (var t = 0; t < Cd.length; t++) Cd[t]._workInProgressVersionPrimary = null;
+        Cd.length = 0
     }
-    var Ou = Ki.ReactCurrentDispatcher,
-        Td = Ki.ReactCurrentBatchConfig,
+    var Au = Qi.ReactCurrentDispatcher,
+        Ed = Qi.ReactCurrentBatchConfig,
         _o = 0,
         dt = null,
-        Mt = null,
+        Pt = null,
         Rt = null,
-        ec = !1,
-        Ra = !1,
+        tc = !1,
+        Ia = !1,
         Qa = 0,
-        zk = 0;
+        zS = 0;
 
     function Zt() {
-        throw Error(ne(321))
+        throw Error(te(321))
     }
 
-    function Jh(t, e) {
+    function Qh(t, e) {
         if (e === null) return !1;
         for (var n = 0; n < e.length && n < t.length; n++)
             if (!li(t[n], e[n])) return !1;
         return !0
     }
 
-    function ep(t, e, n, i, r, o) {
-        if (_o = o, dt = e, e.memoizedState = null, e.updateQueue = null, e.lanes = 0, Ou.current = t === null || t.memoizedState === null ? Bk : Wk, t = n(i, r), Ra) {
+    function Jh(t, e, n, i, r, o) {
+        if (_o = o, dt = e, e.memoizedState = null, e.updateQueue = null, e.lanes = 0, Au.current = t === null || t.memoizedState === null ? BS : WS, t = n(i, r), Ia) {
             o = 0;
             do {
-                if (Ra = !1, Qa = 0, 25 <= o) throw Error(ne(301));
-                o += 1, Rt = Mt = null, e.updateQueue = null, Ou.current = Vk, t = n(i, r)
-            } while (Ra)
+                if (Ia = !1, Qa = 0, 25 <= o) throw Error(te(301));
+                o += 1, Rt = Pt = null, e.updateQueue = null, Au.current = VS, t = n(i, r)
+            } while (Ia)
         }
-        if (Ou.current = tc, e = Mt !== null && Mt.next !== null, _o = 0, Rt = Mt = dt = null, ec = !1, e) throw Error(ne(300));
+        if (Au.current = nc, e = Pt !== null && Pt.next !== null, _o = 0, Rt = Pt = dt = null, tc = !1, e) throw Error(te(300));
         return t
     }
 
-    function tp() {
+    function ep() {
         var t = Qa !== 0;
         return Qa = 0, t
     }
 
     function bi() {
         var t = {
             memoizedState: null,
@@ -3796,43 +3796,43 @@
             queue: null,
             next: null
         };
         return Rt === null ? dt.memoizedState = Rt = t : Rt = Rt.next = t, Rt
     }
 
     function Zn() {
-        if (Mt === null) {
+        if (Pt === null) {
             var t = dt.alternate;
             t = t !== null ? t.memoizedState : null
-        } else t = Mt.next;
+        } else t = Pt.next;
         var e = Rt === null ? dt.memoizedState : Rt.next;
-        if (e !== null) Rt = e, Mt = t;
+        if (e !== null) Rt = e, Pt = t;
         else {
-            if (t === null) throw Error(ne(310));
-            Mt = t, t = {
-                memoizedState: Mt.memoizedState,
-                baseState: Mt.baseState,
-                baseQueue: Mt.baseQueue,
-                queue: Mt.queue,
+            if (t === null) throw Error(te(310));
+            Pt = t, t = {
+                memoizedState: Pt.memoizedState,
+                baseState: Pt.baseState,
+                baseQueue: Pt.baseQueue,
+                queue: Pt.queue,
                 next: null
             }, Rt === null ? dt.memoizedState = Rt = t : Rt = Rt.next = t
         }
         return Rt
     }
 
-    function Ka(t, e) {
+    function Ja(t, e) {
         return typeof e == "function" ? e(t) : e
     }
 
-    function Pd(t) {
+    function Td(t) {
         var e = Zn(),
             n = e.queue;
-        if (n === null) throw Error(ne(311));
+        if (n === null) throw Error(te(311));
         n.lastRenderedReducer = t;
-        var i = Mt,
+        var i = Pt,
             r = i.baseQueue,
             o = n.pending;
         if (o !== null) {
             if (r !== null) {
                 var s = r.next;
                 r.next = o.next, o.next = s
             }
@@ -3869,18 +3869,18 @@
         if (t = n.interleaved, t !== null) {
             r = t;
             do o = r.lane, dt.lanes |= o, wo |= o, r = r.next; while (r !== t)
         } else r === null && (n.lanes = 0);
         return [e.memoizedState, n.dispatch]
     }
 
-    function Md(t) {
+    function Dd(t) {
         var e = Zn(),
             n = e.queue;
-        if (n === null) throw Error(ne(311));
+        if (n === null) throw Error(te(311));
         n.lastRenderedReducer = t;
         var i = n.dispatch,
             r = n.pending,
             o = e.memoizedState;
         if (r !== null) {
             n.pending = null;
             var s = r = r.next;
@@ -3893,16 +3893,16 @@
     function iv() {}
 
     function rv(t, e) {
         var n = dt,
             i = Zn(),
             r = e(),
             o = !li(i.memoizedState, r);
-        if (o && (i.memoizedState = r, gn = !0), i = i.queue, np(av.bind(null, n, i, t), [t]), i.getSnapshot !== e || o || Rt !== null && Rt.memoizedState.tag & 1) {
-            if (n.flags |= 2048, Ja(9, sv.bind(null, n, i, r, e), void 0, null), It === null) throw Error(ne(349));
+        if (o && (i.memoizedState = r, gn = !0), i = i.queue, tp(av.bind(null, n, i, t), [t]), i.getSnapshot !== e || o || Rt !== null && Rt.memoizedState.tag & 1) {
+            if (n.flags |= 2048, el(9, sv.bind(null, n, i, r, e), void 0, null), It === null) throw Error(te(349));
             _o & 30 || ov(n, e, r)
         }
         return r
     }
 
     function ov(t, e, n) {
         t.flags |= 16384, t = {
@@ -3932,31 +3932,31 @@
             return !li(t, n)
         } catch {
             return !0
         }
     }
 
     function uv(t) {
-        var e = Gi(t, 1);
+        var e = Ki(t, 1);
         e !== null && ai(e, t, 1, -1)
     }
 
-    function D0(t) {
+    function M0(t) {
         var e = bi();
         return typeof t == "function" && (t = t()), e.memoizedState = e.baseState = t, t = {
             pending: null,
             interleaved: null,
             lanes: 0,
             dispatch: null,
-            lastRenderedReducer: Ka,
+            lastRenderedReducer: Ja,
             lastRenderedState: t
-        }, e.queue = t, t = t.dispatch = Hk.bind(null, dt, t), [e.memoizedState, t]
+        }, e.queue = t, t = t.dispatch = HS.bind(null, dt, t), [e.memoizedState, t]
     }
 
-    function Ja(t, e, n, i) {
+    function el(t, e, n, i) {
         return t = {
             tag: t,
             create: e,
             destroy: n,
             deps: i,
             next: null
         }, e = dt.updateQueue, e === null ? (e = {
@@ -3965,116 +3965,116 @@
         }, dt.updateQueue = e, e.lastEffect = t.next = t) : (n = e.lastEffect, n === null ? e.lastEffect = t.next = t : (i = n.next, n.next = t, t.next = i, e.lastEffect = t)), t
     }
 
     function cv() {
         return Zn().memoizedState
     }
 
-    function Au(t, e, n, i) {
+    function Lu(t, e, n, i) {
         var r = bi();
-        dt.flags |= t, r.memoizedState = Ja(1 | e, n, void 0, i === void 0 ? null : i)
+        dt.flags |= t, r.memoizedState = el(1 | e, n, void 0, i === void 0 ? null : i)
     }
 
-    function pc(t, e, n, i) {
+    function gc(t, e, n, i) {
         var r = Zn();
         i = i === void 0 ? null : i;
         var o = void 0;
-        if (Mt !== null) {
-            var s = Mt.memoizedState;
-            if (o = s.destroy, i !== null && Jh(i, s.deps)) {
-                r.memoizedState = Ja(e, n, o, i);
+        if (Pt !== null) {
+            var s = Pt.memoizedState;
+            if (o = s.destroy, i !== null && Qh(i, s.deps)) {
+                r.memoizedState = el(e, n, o, i);
                 return
             }
         }
-        dt.flags |= t, r.memoizedState = Ja(1 | e, n, o, i)
+        dt.flags |= t, r.memoizedState = el(1 | e, n, o, i)
     }
 
     function O0(t, e) {
-        return Au(8390656, 8, t, e)
+        return Lu(8390656, 8, t, e)
     }
 
-    function np(t, e) {
-        return pc(2048, 8, t, e)
+    function tp(t, e) {
+        return gc(2048, 8, t, e)
     }
 
     function fv(t, e) {
-        return pc(4, 2, t, e)
+        return gc(4, 2, t, e)
     }
 
     function dv(t, e) {
-        return pc(4, 4, t, e)
+        return gc(4, 4, t, e)
     }
 
     function hv(t, e) {
         if (typeof e == "function") return t = t(), e(t),
             function() {
                 e(null)
             };
         if (e != null) return t = t(), e.current = t,
             function() {
                 e.current = null
             }
     }
 
     function pv(t, e, n) {
-        return n = n != null ? n.concat([t]) : null, pc(4, 4, hv.bind(null, e, t), n)
+        return n = n != null ? n.concat([t]) : null, gc(4, 4, hv.bind(null, e, t), n)
     }
 
-    function ip() {}
+    function np() {}
 
     function gv(t, e) {
         var n = Zn();
         e = e === void 0 ? null : e;
         var i = n.memoizedState;
-        return i !== null && e !== null && Jh(e, i[1]) ? i[0] : (n.memoizedState = [t, e], t)
+        return i !== null && e !== null && Qh(e, i[1]) ? i[0] : (n.memoizedState = [t, e], t)
     }
 
     function mv(t, e) {
         var n = Zn();
         e = e === void 0 ? null : e;
         var i = n.memoizedState;
-        return i !== null && e !== null && Jh(e, i[1]) ? i[0] : (t = t(), n.memoizedState = [t, e], t)
+        return i !== null && e !== null && Qh(e, i[1]) ? i[0] : (t = t(), n.memoizedState = [t, e], t)
     }
 
     function yv(t, e, n) {
         return _o & 21 ? (li(n, e) || (n = by(), dt.lanes |= n, wo |= n, t.baseState = !0), e) : (t.baseState && (t.baseState = !1, gn = !0), t.memoizedState = n)
     }
 
-    function Fk(t, e) {
+    function FS(t, e) {
         var n = Be;
         Be = n !== 0 && 4 > n ? n : 4, t(!0);
-        var i = Td.transition;
-        Td.transition = {};
+        var i = Ed.transition;
+        Ed.transition = {};
         try {
             t(!1), e()
         } finally {
-            Be = n, Td.transition = i
+            Be = n, Ed.transition = i
         }
     }
 
     function vv() {
         return Zn().memoizedState
     }
 
-    function jk(t, e, n) {
+    function jS(t, e, n) {
         var i = Or(t);
         if (n = {
                 lane: i,
                 action: n,
                 hasEagerState: !1,
                 eagerState: null,
                 next: null
             }, xv(t)) bv(e, n);
-        else if (n = Gy(t, e, n, i), n !== null) {
+        else if (n = Ky(t, e, n, i), n !== null) {
             var r = nn();
             ai(n, t, i, r), _v(n, e, i)
         }
     }
 
-    function Hk(t, e, n) {
+    function HS(t, e, n) {
         var i = Or(t),
             r = {
                 lane: i,
                 action: n,
                 hasEagerState: !1,
                 eagerState: null,
                 next: null
@@ -4083,40 +4083,40 @@
         else {
             var o = t.alternate;
             if (t.lanes === 0 && (o === null || o.lanes === 0) && (o = e.lastRenderedReducer, o !== null)) try {
                 var s = e.lastRenderedState,
                     a = o(s, n);
                 if (r.hasEagerState = !0, r.eagerState = a, li(a, s)) {
                     var l = e.interleaved;
-                    l === null ? (r.next = r, qh(e)) : (r.next = l.next, l.next = r), e.interleaved = r;
+                    l === null ? (r.next = r, Xh(e)) : (r.next = l.next, l.next = r), e.interleaved = r;
                     return
                 }
             } catch {} finally {}
-            n = Gy(t, e, r, i), n !== null && (r = nn(), ai(n, t, i, r), _v(n, e, i))
+            n = Ky(t, e, r, i), n !== null && (r = nn(), ai(n, t, i, r), _v(n, e, i))
         }
     }
 
     function xv(t) {
         var e = t.alternate;
         return t === dt || e !== null && e === dt
     }
 
     function bv(t, e) {
-        Ra = ec = !0;
+        Ia = tc = !0;
         var n = t.pending;
         n === null ? e.next = e : (e.next = n.next, n.next = e), t.pending = e
     }
 
     function _v(t, e, n) {
         if (n & 4194240) {
             var i = e.lanes;
-            i &= t.pendingLanes, n |= i, e.lanes = n, Rh(t, n)
+            i &= t.pendingLanes, n |= i, e.lanes = n, Lh(t, n)
         }
     }
-    var tc = {
+    var nc = {
             readContext: qn,
             useCallback: Zt,
             useContext: Zt,
             useEffect: Zt,
             useImperativeHandle: Zt,
             useInsertionEffect: Zt,
             useLayoutEffect: Zt,
@@ -4128,141 +4128,141 @@
             useDeferredValue: Zt,
             useTransition: Zt,
             useMutableSource: Zt,
             useSyncExternalStore: Zt,
             useId: Zt,
             unstable_isNewReconciler: !1
         },
-        Bk = {
+        BS = {
             readContext: qn,
             useCallback: function(t, e) {
                 return bi().memoizedState = [t, e === void 0 ? null : e], t
             },
             useContext: qn,
             useEffect: O0,
             useImperativeHandle: function(t, e, n) {
-                return n = n != null ? n.concat([t]) : null, Au(4194308, 4, hv.bind(null, e, t), n)
+                return n = n != null ? n.concat([t]) : null, Lu(4194308, 4, hv.bind(null, e, t), n)
             },
             useLayoutEffect: function(t, e) {
-                return Au(4194308, 4, t, e)
+                return Lu(4194308, 4, t, e)
             },
             useInsertionEffect: function(t, e) {
-                return Au(4, 2, t, e)
+                return Lu(4, 2, t, e)
             },
             useMemo: function(t, e) {
                 var n = bi();
                 return e = e === void 0 ? null : e, t = t(), n.memoizedState = [t, e], t
             },
             useReducer: function(t, e, n) {
                 var i = bi();
                 return e = n !== void 0 ? n(e) : e, i.memoizedState = i.baseState = e, t = {
                     pending: null,
                     interleaved: null,
                     lanes: 0,
                     dispatch: null,
                     lastRenderedReducer: t,
                     lastRenderedState: e
-                }, i.queue = t, t = t.dispatch = jk.bind(null, dt, t), [i.memoizedState, t]
+                }, i.queue = t, t = t.dispatch = jS.bind(null, dt, t), [i.memoizedState, t]
             },
             useRef: function(t) {
                 var e = bi();
                 return t = {
                     current: t
                 }, e.memoizedState = t
             },
-            useState: D0,
-            useDebugValue: ip,
+            useState: M0,
+            useDebugValue: np,
             useDeferredValue: function(t) {
                 return bi().memoizedState = t
             },
             useTransition: function() {
-                var t = D0(!1),
+                var t = M0(!1),
                     e = t[0];
-                return t = Fk.bind(null, t[1]), bi().memoizedState = t, [e, t]
+                return t = FS.bind(null, t[1]), bi().memoizedState = t, [e, t]
             },
             useMutableSource: function() {},
             useSyncExternalStore: function(t, e, n) {
                 var i = dt,
                     r = bi();
                 if (at) {
-                    if (n === void 0) throw Error(ne(407));
+                    if (n === void 0) throw Error(te(407));
                     n = n()
                 } else {
-                    if (n = e(), It === null) throw Error(ne(349));
+                    if (n = e(), It === null) throw Error(te(349));
                     _o & 30 || ov(i, e, n)
                 }
                 r.memoizedState = n;
                 var o = {
                     value: n,
                     getSnapshot: e
                 };
-                return r.queue = o, O0(av.bind(null, i, o, t), [t]), i.flags |= 2048, Ja(9, sv.bind(null, i, o, n, e), void 0, null), n
+                return r.queue = o, O0(av.bind(null, i, o, t), [t]), i.flags |= 2048, el(9, sv.bind(null, i, o, n, e), void 0, null), n
             },
             useId: function() {
                 var t = bi(),
                     e = It.identifierPrefix;
                 if (at) {
                     var n = Yi,
                         i = $i;
                     n = (i & ~(1 << 32 - si(i) - 1)).toString(32) + n, e = ":" + e + "R" + n, n = Qa++, 0 < n && (e += "H" + n.toString(32)), e += ":"
-                } else n = zk++, e = ":" + e + "r" + n.toString(32) + ":";
+                } else n = zS++, e = ":" + e + "r" + n.toString(32) + ":";
                 return t.memoizedState = e
             },
             unstable_isNewReconciler: !1
         },
-        Wk = {
+        WS = {
             readContext: qn,
             useCallback: gv,
             useContext: qn,
-            useEffect: np,
+            useEffect: tp,
             useImperativeHandle: pv,
             useInsertionEffect: fv,
             useLayoutEffect: dv,
             useMemo: mv,
-            useReducer: Pd,
+            useReducer: Td,
             useRef: cv,
             useState: function() {
-                return Pd(Ka)
+                return Td(Ja)
             },
-            useDebugValue: ip,
+            useDebugValue: np,
             useDeferredValue: function(t) {
                 var e = Zn();
-                return yv(e, Mt.memoizedState, t)
+                return yv(e, Pt.memoizedState, t)
             },
             useTransition: function() {
-                var t = Pd(Ka)[0],
+                var t = Td(Ja)[0],
                     e = Zn().memoizedState;
                 return [t, e]
             },
             useMutableSource: iv,
             useSyncExternalStore: rv,
             useId: vv,
             unstable_isNewReconciler: !1
         },
-        Vk = {
+        VS = {
             readContext: qn,
             useCallback: gv,
             useContext: qn,
-            useEffect: np,
+            useEffect: tp,
             useImperativeHandle: pv,
             useInsertionEffect: fv,
             useLayoutEffect: dv,
             useMemo: mv,
-            useReducer: Md,
+            useReducer: Dd,
             useRef: cv,
             useState: function() {
-                return Md(Ka)
+                return Dd(Ja)
             },
-            useDebugValue: ip,
+            useDebugValue: np,
             useDeferredValue: function(t) {
                 var e = Zn();
-                return Mt === null ? e.memoizedState = t : yv(e, Mt.memoizedState, t)
+                return Pt === null ? e.memoizedState = t : yv(e, Pt.memoizedState, t)
             },
             useTransition: function() {
-                var t = Md(Ka)[0],
+                var t = Dd(Ja)[0],
                     e = Zn().memoizedState;
                 return [t, e]
             },
             useMutableSource: iv,
             useSyncExternalStore: rv,
             useId: vv,
             unstable_isNewReconciler: !1
@@ -4283,120 +4283,120 @@
             value: t,
             source: e,
             stack: r,
             digest: null
         }
     }
 
-    function Dd(t, e, n) {
+    function Pd(t, e, n) {
         return {
             value: t,
             source: null,
             stack: n ?? null,
             digest: e ?? null
         }
     }
 
-    function dh(t, e) {
+    function fh(t, e) {
         try {
             console.error(e.value)
         } catch (n) {
             setTimeout(function() {
                 throw n
             })
         }
     }
-    var Uk = typeof WeakMap == "function" ? WeakMap : Map;
+    var US = typeof WeakMap == "function" ? WeakMap : Map;
 
     function wv(t, e, n) {
         n = Xi(-1, n), n.tag = 3, n.payload = {
             element: null
         };
         var i = e.value;
         return n.callback = function() {
-            ic || (ic = !0, wh = i), dh(t, e)
+            rc || (rc = !0, _h = i), fh(t, e)
         }, n
     }
 
-    function kv(t, e, n) {
+    function Sv(t, e, n) {
         n = Xi(-1, n), n.tag = 3;
         var i = t.type.getDerivedStateFromError;
         if (typeof i == "function") {
             var r = e.value;
             n.payload = function() {
                 return i(r)
             }, n.callback = function() {
-                dh(t, e)
+                fh(t, e)
             }
         }
         var o = t.stateNode;
         return o !== null && typeof o.componentDidCatch == "function" && (n.callback = function() {
-            dh(t, e), typeof i != "function" && (Dr === null ? Dr = new Set([this]) : Dr.add(this));
+            fh(t, e), typeof i != "function" && (Mr === null ? Mr = new Set([this]) : Mr.add(this));
             var s = e.stack;
             this.componentDidCatch(e.value, {
                 componentStack: s !== null ? s : ""
             })
         }), n
     }
 
     function A0(t, e, n) {
         var i = t.pingCache;
         if (i === null) {
-            i = t.pingCache = new Uk;
+            i = t.pingCache = new US;
             var r = new Set;
             i.set(e, r)
         } else r = i.get(e), r === void 0 && (r = new Set, i.set(e, r));
-        r.has(n) || (r.add(n), t = rS.bind(null, t, e, n), e.then(t, t))
+        r.has(n) || (r.add(n), t = rk.bind(null, t, e, n), e.then(t, t))
     }
 
     function L0(t) {
         do {
             var e;
             if ((e = t.tag === 13) && (e = t.memoizedState, e = e !== null ? e.dehydrated !== null : !0), e) return t;
             t = t.return
         } while (t !== null);
         return null
     }
 
     function R0(t, e, n, i, r) {
-        return t.mode & 1 ? (t.flags |= 65536, t.lanes = r, t) : (t === e ? t.flags |= 65536 : (t.flags |= 128, n.flags |= 131072, n.flags &= -52805, n.tag === 1 && (n.alternate === null ? n.tag = 17 : (e = Xi(-1, 1), e.tag = 2, Mr(n, e, 1))), n.lanes |= 1), t)
+        return t.mode & 1 ? (t.flags |= 65536, t.lanes = r, t) : (t === e ? t.flags |= 65536 : (t.flags |= 128, n.flags |= 131072, n.flags &= -52805, n.tag === 1 && (n.alternate === null ? n.tag = 17 : (e = Xi(-1, 1), e.tag = 2, Pr(n, e, 1))), n.lanes |= 1), t)
     }
-    var $k = Ki.ReactCurrentOwner,
+    var $S = Qi.ReactCurrentOwner,
         gn = !1;
 
     function tn(t, e, n, i) {
-        e.child = t === null ? tv(e, null, n, i) : Ss(e, t.child, n, i)
+        e.child = t === null ? tv(e, null, n, i) : ks(e, t.child, n, i)
     }
 
     function I0(t, e, n, i, r) {
         n = n.render;
         var o = e.ref;
-        return xs(e, r), i = ep(t, e, n, i, o, r), n = tp(), t !== null && !gn ? (e.updateQueue = t.updateQueue, e.flags &= -2053, t.lanes &= ~r, Qi(t, e, r)) : (at && n && Wh(e), e.flags |= 1, tn(t, e, i, r), e.child)
+        return xs(e, r), i = Jh(t, e, n, i, o, r), n = ep(), t !== null && !gn ? (e.updateQueue = t.updateQueue, e.flags &= -2053, t.lanes &= ~r, Gi(t, e, r)) : (at && n && Bh(e), e.flags |= 1, tn(t, e, i, r), e.child)
     }
 
     function N0(t, e, n, i, r) {
         if (t === null) {
             var o = n.type;
-            return typeof o == "function" && !fp(o) && o.defaultProps === void 0 && n.compare === null && n.defaultProps === void 0 ? (e.tag = 15, e.type = o, Sv(t, e, o, i, r)) : (t = Nu(n.type, null, i, e, e.mode, r), t.ref = e.ref, t.return = e, e.child = t)
+            return typeof o == "function" && !cp(o) && o.defaultProps === void 0 && n.compare === null && n.defaultProps === void 0 ? (e.tag = 15, e.type = o, kv(t, e, o, i, r)) : (t = zu(n.type, null, i, e, e.mode, r), t.ref = e.ref, t.return = e, e.child = t)
         }
         if (o = t.child, !(t.lanes & r)) {
             var s = o.memoizedProps;
-            if (n = n.compare, n = n !== null ? n : $a, n(s, i) && t.ref === e.ref) return Qi(t, e, r)
+            if (n = n.compare, n = n !== null ? n : Ya, n(s, i) && t.ref === e.ref) return Gi(t, e, r)
         }
         return e.flags |= 1, t = Ar(o, i), t.ref = e.ref, t.return = e, e.child = t
     }
 
-    function Sv(t, e, n, i, r) {
+    function kv(t, e, n, i, r) {
         if (t !== null) {
             var o = t.memoizedProps;
-            if ($a(o, i) && t.ref === e.ref)
+            if (Ya(o, i) && t.ref === e.ref)
                 if (gn = !1, e.pendingProps = i = o, (t.lanes & r) !== 0) t.flags & 131072 && (gn = !0);
-                else return e.lanes = t.lanes, Qi(t, e, r)
+                else return e.lanes = t.lanes, Gi(t, e, r)
         }
-        return hh(t, e, n, i, r)
+        return dh(t, e, n, i, r)
     }
 
     function Cv(t, e, n) {
         var i = e.pendingProps,
             r = i.children,
             o = t !== null ? t.memoizedState : null;
         if (i.mode === "hidden")
@@ -4422,127 +4422,127 @@
     }
 
     function Ev(t, e) {
         var n = e.ref;
         (t === null && n !== null || t !== null && t.ref !== n) && (e.flags |= 512, e.flags |= 2097152)
     }
 
-    function hh(t, e, n, i, r) {
-        var o = yn(n) ? xo : Kt.current;
-        return o = ws(e, o), xs(e, r), n = ep(t, e, n, i, o, r), i = tp(), t !== null && !gn ? (e.updateQueue = t.updateQueue, e.flags &= -2053, t.lanes &= ~r, Qi(t, e, r)) : (at && i && Wh(e), e.flags |= 1, tn(t, e, n, r), e.child)
+    function dh(t, e, n, i, r) {
+        var o = yn(n) ? xo : Qt.current;
+        return o = ws(e, o), xs(e, r), n = Jh(t, e, n, i, o, r), i = ep(), t !== null && !gn ? (e.updateQueue = t.updateQueue, e.flags &= -2053, t.lanes &= ~r, Gi(t, e, r)) : (at && i && Bh(e), e.flags |= 1, tn(t, e, n, r), e.child)
     }
 
     function z0(t, e, n, i, r) {
         if (yn(n)) {
             var o = !0;
-            Xu(e)
+            qu(e)
         } else o = !1;
-        if (xs(e, r), e.stateNode === null) Lu(t, e), Jy(e, n, i), fh(e, n, i, r), i = !0;
+        if (xs(e, r), e.stateNode === null) Ru(t, e), Jy(e, n, i), ch(e, n, i, r), i = !0;
         else if (t === null) {
             var s = e.stateNode,
                 a = e.memoizedProps;
             s.props = a;
             var l = s.context,
                 c = n.contextType;
-            typeof c == "object" && c !== null ? c = qn(c) : (c = yn(n) ? xo : Kt.current, c = ws(e, c));
+            typeof c == "object" && c !== null ? c = qn(c) : (c = yn(n) ? xo : Qt.current, c = ws(e, c));
             var d = n.getDerivedStateFromProps,
                 g = typeof d == "function" || typeof s.getSnapshotBeforeUpdate == "function";
-            g || typeof s.UNSAFE_componentWillReceiveProps != "function" && typeof s.componentWillReceiveProps != "function" || (a !== i || l !== c) && P0(e, s, i, c), br = !1;
+            g || typeof s.UNSAFE_componentWillReceiveProps != "function" && typeof s.componentWillReceiveProps != "function" || (a !== i || l !== c) && D0(e, s, i, c), br = !1;
             var y = e.memoizedState;
-            s.state = y, Ku(e, i, s, r), l = e.memoizedState, a !== i || y !== l || mn.current || br ? (typeof d == "function" && (ch(e, n, d, i), l = e.memoizedState), (a = br || T0(e, n, a, i, y, l, c)) ? (g || typeof s.UNSAFE_componentWillMount != "function" && typeof s.componentWillMount != "function" || (typeof s.componentWillMount == "function" && s.componentWillMount(), typeof s.UNSAFE_componentWillMount == "function" && s.UNSAFE_componentWillMount()), typeof s.componentDidMount == "function" && (e.flags |= 4194308)) : (typeof s.componentDidMount == "function" && (e.flags |= 4194308), e.memoizedProps = i, e.memoizedState = l), s.props = i, s.state = l, s.context = c, i = a) : (typeof s.componentDidMount == "function" && (e.flags |= 4194308), i = !1)
+            s.state = y, Ju(e, i, s, r), l = e.memoizedState, a !== i || y !== l || mn.current || br ? (typeof d == "function" && (uh(e, n, d, i), l = e.memoizedState), (a = br || T0(e, n, a, i, y, l, c)) ? (g || typeof s.UNSAFE_componentWillMount != "function" && typeof s.componentWillMount != "function" || (typeof s.componentWillMount == "function" && s.componentWillMount(), typeof s.UNSAFE_componentWillMount == "function" && s.UNSAFE_componentWillMount()), typeof s.componentDidMount == "function" && (e.flags |= 4194308)) : (typeof s.componentDidMount == "function" && (e.flags |= 4194308), e.memoizedProps = i, e.memoizedState = l), s.props = i, s.state = l, s.context = c, i = a) : (typeof s.componentDidMount == "function" && (e.flags |= 4194308), i = !1)
         } else {
-            s = e.stateNode, Qy(t, e), a = e.memoizedProps, c = e.type === e.elementType ? a : ii(e.type, a), s.props = c, g = e.pendingProps, y = s.context, l = n.contextType, typeof l == "object" && l !== null ? l = qn(l) : (l = yn(n) ? xo : Kt.current, l = ws(e, l));
+            s = e.stateNode, Gy(t, e), a = e.memoizedProps, c = e.type === e.elementType ? a : ii(e.type, a), s.props = c, g = e.pendingProps, y = s.context, l = n.contextType, typeof l == "object" && l !== null ? l = qn(l) : (l = yn(n) ? xo : Qt.current, l = ws(e, l));
             var x = n.getDerivedStateFromProps;
-            (d = typeof x == "function" || typeof s.getSnapshotBeforeUpdate == "function") || typeof s.UNSAFE_componentWillReceiveProps != "function" && typeof s.componentWillReceiveProps != "function" || (a !== g || y !== l) && P0(e, s, i, l), br = !1, y = e.memoizedState, s.state = y, Ku(e, i, s, r);
-            var w = e.memoizedState;
-            a !== g || y !== w || mn.current || br ? (typeof x == "function" && (ch(e, n, x, i), w = e.memoizedState), (c = br || T0(e, n, c, i, y, w, l) || !1) ? (d || typeof s.UNSAFE_componentWillUpdate != "function" && typeof s.componentWillUpdate != "function" || (typeof s.componentWillUpdate == "function" && s.componentWillUpdate(i, w, l), typeof s.UNSAFE_componentWillUpdate == "function" && s.UNSAFE_componentWillUpdate(i, w, l)), typeof s.componentDidUpdate == "function" && (e.flags |= 4), typeof s.getSnapshotBeforeUpdate == "function" && (e.flags |= 1024)) : (typeof s.componentDidUpdate != "function" || a === t.memoizedProps && y === t.memoizedState || (e.flags |= 4), typeof s.getSnapshotBeforeUpdate != "function" || a === t.memoizedProps && y === t.memoizedState || (e.flags |= 1024), e.memoizedProps = i, e.memoizedState = w), s.props = i, s.state = w, s.context = l, i = c) : (typeof s.componentDidUpdate != "function" || a === t.memoizedProps && y === t.memoizedState || (e.flags |= 4), typeof s.getSnapshotBeforeUpdate != "function" || a === t.memoizedProps && y === t.memoizedState || (e.flags |= 1024), i = !1)
+            (d = typeof x == "function" || typeof s.getSnapshotBeforeUpdate == "function") || typeof s.UNSAFE_componentWillReceiveProps != "function" && typeof s.componentWillReceiveProps != "function" || (a !== g || y !== l) && D0(e, s, i, l), br = !1, y = e.memoizedState, s.state = y, Ju(e, i, s, r);
+            var _ = e.memoizedState;
+            a !== g || y !== _ || mn.current || br ? (typeof x == "function" && (uh(e, n, x, i), _ = e.memoizedState), (c = br || T0(e, n, c, i, y, _, l) || !1) ? (d || typeof s.UNSAFE_componentWillUpdate != "function" && typeof s.componentWillUpdate != "function" || (typeof s.componentWillUpdate == "function" && s.componentWillUpdate(i, _, l), typeof s.UNSAFE_componentWillUpdate == "function" && s.UNSAFE_componentWillUpdate(i, _, l)), typeof s.componentDidUpdate == "function" && (e.flags |= 4), typeof s.getSnapshotBeforeUpdate == "function" && (e.flags |= 1024)) : (typeof s.componentDidUpdate != "function" || a === t.memoizedProps && y === t.memoizedState || (e.flags |= 4), typeof s.getSnapshotBeforeUpdate != "function" || a === t.memoizedProps && y === t.memoizedState || (e.flags |= 1024), e.memoizedProps = i, e.memoizedState = _), s.props = i, s.state = _, s.context = l, i = c) : (typeof s.componentDidUpdate != "function" || a === t.memoizedProps && y === t.memoizedState || (e.flags |= 4), typeof s.getSnapshotBeforeUpdate != "function" || a === t.memoizedProps && y === t.memoizedState || (e.flags |= 1024), i = !1)
         }
-        return ph(t, e, n, i, o, r)
+        return hh(t, e, n, i, o, r)
     }
 
-    function ph(t, e, n, i, r, o) {
+    function hh(t, e, n, i, r, o) {
         Ev(t, e);
         var s = (e.flags & 128) !== 0;
-        if (!i && !s) return r && w0(e, n, !1), Qi(t, e, o);
-        i = e.stateNode, $k.current = e;
+        if (!i && !s) return r && w0(e, n, !1), Gi(t, e, o);
+        i = e.stateNode, $S.current = e;
         var a = s && typeof n.getDerivedStateFromError != "function" ? null : i.render();
-        return e.flags |= 1, t !== null && s ? (e.child = Ss(e, t.child, null, o), e.child = Ss(e, null, a, o)) : tn(t, e, a, o), e.memoizedState = i.state, r && w0(e, n, !0), e.child
+        return e.flags |= 1, t !== null && s ? (e.child = ks(e, t.child, null, o), e.child = ks(e, null, a, o)) : tn(t, e, a, o), e.memoizedState = i.state, r && w0(e, n, !0), e.child
     }
 
     function Tv(t) {
         var e = t.stateNode;
-        e.pendingContext ? _0(t, e.pendingContext, e.pendingContext !== e.context) : e.context && _0(t, e.context, !1), Gh(t, e.containerInfo)
+        e.pendingContext ? _0(t, e.pendingContext, e.pendingContext !== e.context) : e.context && _0(t, e.context, !1), Zh(t, e.containerInfo)
     }
 
     function F0(t, e, n, i, r) {
-        return ks(), Uh(r), e.flags |= 256, tn(t, e, n, i), e.child
+        return Ss(), Vh(r), e.flags |= 256, tn(t, e, n, i), e.child
     }
-    var gh = {
+    var ph = {
         dehydrated: null,
         treeContext: null,
         retryLane: 0
     };
 
-    function mh(t) {
+    function gh(t) {
         return {
             baseLanes: t,
             cachePool: null,
             transitions: null
         }
     }
 
-    function Pv(t, e, n) {
+    function Dv(t, e, n) {
         var i = e.pendingProps,
             r = ft.current,
             o = !1,
             s = (e.flags & 128) !== 0,
             a;
-        if ((a = s) || (a = t !== null && t.memoizedState === null ? !1 : (r & 2) !== 0), a ? (o = !0, e.flags &= -129) : (t === null || t.memoizedState !== null) && (r |= 1), et(ft, r & 1), t === null) return lh(e), t = e.memoizedState, t !== null && (t = t.dehydrated, t !== null) ? (e.mode & 1 ? t.data === "$!" ? e.lanes = 8 : e.lanes = 1073741824 : e.lanes = 1, null) : (s = i.children, t = i.fallback, o ? (i = e.mode, o = e.child, s = {
+        if ((a = s) || (a = t !== null && t.memoizedState === null ? !1 : (r & 2) !== 0), a ? (o = !0, e.flags &= -129) : (t === null || t.memoizedState !== null) && (r |= 1), et(ft, r & 1), t === null) return ah(e), t = e.memoizedState, t !== null && (t = t.dehydrated, t !== null) ? (e.mode & 1 ? t.data === "$!" ? e.lanes = 8 : e.lanes = 1073741824 : e.lanes = 1, null) : (s = i.children, t = i.fallback, o ? (i = e.mode, o = e.child, s = {
             mode: "hidden",
             children: s
-        }, !(i & 1) && o !== null ? (o.childLanes = 0, o.pendingProps = s) : o = yc(s, i, 0, null), t = vo(t, i, n, null), o.return = e, t.return = e, o.sibling = t, e.child = o, e.child.memoizedState = mh(n), e.memoizedState = gh, t) : rp(e, s));
-        if (r = t.memoizedState, r !== null && (a = r.dehydrated, a !== null)) return Yk(t, e, s, i, a, r, n);
+        }, !(i & 1) && o !== null ? (o.childLanes = 0, o.pendingProps = s) : o = vc(s, i, 0, null), t = vo(t, i, n, null), o.return = e, t.return = e, o.sibling = t, e.child = o, e.child.memoizedState = gh(n), e.memoizedState = ph, t) : ip(e, s));
+        if (r = t.memoizedState, r !== null && (a = r.dehydrated, a !== null)) return YS(t, e, s, i, a, r, n);
         if (o) {
             o = i.fallback, s = e.mode, r = t.child, a = r.sibling;
             var l = {
                 mode: "hidden",
                 children: i.children
             };
-            return !(s & 1) && e.child !== r ? (i = e.child, i.childLanes = 0, i.pendingProps = l, e.deletions = null) : (i = Ar(r, l), i.subtreeFlags = r.subtreeFlags & 14680064), a !== null ? o = Ar(a, o) : (o = vo(o, s, n, null), o.flags |= 2), o.return = e, i.return = e, i.sibling = o, e.child = i, i = o, o = e.child, s = t.child.memoizedState, s = s === null ? mh(n) : {
+            return !(s & 1) && e.child !== r ? (i = e.child, i.childLanes = 0, i.pendingProps = l, e.deletions = null) : (i = Ar(r, l), i.subtreeFlags = r.subtreeFlags & 14680064), a !== null ? o = Ar(a, o) : (o = vo(o, s, n, null), o.flags |= 2), o.return = e, i.return = e, i.sibling = o, e.child = i, i = o, o = e.child, s = t.child.memoizedState, s = s === null ? gh(n) : {
                 baseLanes: s.baseLanes | n,
                 cachePool: null,
                 transitions: s.transitions
-            }, o.memoizedState = s, o.childLanes = t.childLanes & ~n, e.memoizedState = gh, i
+            }, o.memoizedState = s, o.childLanes = t.childLanes & ~n, e.memoizedState = ph, i
         }
         return o = t.child, t = o.sibling, i = Ar(o, {
             mode: "visible",
             children: i.children
         }), !(e.mode & 1) && (i.lanes = n), i.return = e, i.sibling = null, t !== null && (n = e.deletions, n === null ? (e.deletions = [t], e.flags |= 16) : n.push(t)), e.child = i, e.memoizedState = null, i
     }
 
-    function rp(t, e) {
-        return e = yc({
+    function ip(t, e) {
+        return e = vc({
             mode: "visible",
             children: e
         }, t.mode, 0, null), e.return = t, t.child = e
     }
 
-    function Su(t, e, n, i) {
-        return i !== null && Uh(i), Ss(e, t.child, null, n), t = rp(e, e.pendingProps.children), t.flags |= 2, e.memoizedState = null, t
+    function Cu(t, e, n, i) {
+        return i !== null && Vh(i), ks(e, t.child, null, n), t = ip(e, e.pendingProps.children), t.flags |= 2, e.memoizedState = null, t
     }
 
-    function Yk(t, e, n, i, r, o, s) {
-        if (n) return e.flags & 256 ? (e.flags &= -257, i = Dd(Error(ne(422))), Su(t, e, s, i)) : e.memoizedState !== null ? (e.child = t.child, e.flags |= 128, null) : (o = i.fallback, r = e.mode, i = yc({
+    function YS(t, e, n, i, r, o, s) {
+        if (n) return e.flags & 256 ? (e.flags &= -257, i = Pd(Error(te(422))), Cu(t, e, s, i)) : e.memoizedState !== null ? (e.child = t.child, e.flags |= 128, null) : (o = i.fallback, r = e.mode, i = vc({
             mode: "visible",
             children: i.children
-        }, r, 0, null), o = vo(o, r, s, null), o.flags |= 2, i.return = e, o.return = e, i.sibling = o, e.child = i, e.mode & 1 && Ss(e, t.child, null, s), e.child.memoizedState = mh(s), e.memoizedState = gh, o);
-        if (!(e.mode & 1)) return Su(t, e, s, null);
+        }, r, 0, null), o = vo(o, r, s, null), o.flags |= 2, i.return = e, o.return = e, i.sibling = o, e.child = i, e.mode & 1 && ks(e, t.child, null, s), e.child.memoizedState = gh(s), e.memoizedState = ph, o);
+        if (!(e.mode & 1)) return Cu(t, e, s, null);
         if (r.data === "$!") {
             if (i = r.nextSibling && r.nextSibling.dataset, i) var a = i.dgst;
-            return i = a, o = Error(ne(419)), i = Dd(o, i, void 0), Su(t, e, s, i)
+            return i = a, o = Error(te(419)), i = Pd(o, i, void 0), Cu(t, e, s, i)
         }
         if (a = (s & t.childLanes) !== 0, gn || a) {
             if (i = It, i !== null) {
                 switch (s & -s) {
                     case 4:
                         r = 2;
                         break;
@@ -4574,40 +4574,40 @@
                         break;
                     case 536870912:
                         r = 268435456;
                         break;
                     default:
                         r = 0
                 }
-                r = r & (i.suspendedLanes | s) ? 0 : r, r !== 0 && r !== o.retryLane && (o.retryLane = r, Gi(t, r), ai(i, t, r, -1))
+                r = r & (i.suspendedLanes | s) ? 0 : r, r !== 0 && r !== o.retryLane && (o.retryLane = r, Ki(t, r), ai(i, t, r, -1))
             }
-            return cp(), i = Dd(Error(ne(421))), Su(t, e, s, i)
+            return up(), i = Pd(Error(te(421))), Cu(t, e, s, i)
         }
-        return r.data === "$?" ? (e.flags |= 128, e.child = t.child, e = oS.bind(null, t), r._reactRetry = e, null) : (t = o.treeContext, An = Pr(r.nextSibling), Ln = e, at = !0, oi = null, t !== null && (Un[$n++] = $i, Un[$n++] = Yi, Un[$n++] = bo, $i = t.id, Yi = t.overflow, bo = e), e = rp(e, i.children), e.flags |= 4096, e)
+        return r.data === "$?" ? (e.flags |= 128, e.child = t.child, e = ok.bind(null, t), r._reactRetry = e, null) : (t = o.treeContext, An = Dr(r.nextSibling), Ln = e, at = !0, oi = null, t !== null && (Un[$n++] = $i, Un[$n++] = Yi, Un[$n++] = bo, $i = t.id, Yi = t.overflow, bo = e), e = ip(e, i.children), e.flags |= 4096, e)
     }
 
     function j0(t, e, n) {
         t.lanes |= e;
         var i = t.alternate;
-        i !== null && (i.lanes |= e), uh(t.return, e, n)
+        i !== null && (i.lanes |= e), lh(t.return, e, n)
     }
 
-    function Od(t, e, n, i, r) {
+    function Md(t, e, n, i, r) {
         var o = t.memoizedState;
         o === null ? t.memoizedState = {
             isBackwards: e,
             rendering: null,
             renderingStartTime: 0,
             last: i,
             tail: n,
             tailMode: r
         } : (o.isBackwards = e, o.rendering = null, o.renderingStartTime = 0, o.last = i, o.tail = n, o.tailMode = r)
     }
 
-    function Mv(t, e, n) {
+    function Pv(t, e, n) {
         var i = e.pendingProps,
             r = i.revealOrder,
             o = i.tail;
         if (tn(t, e, i.children, n), i = ft.current, i & 2) i = i & 1 | 2, e.flags |= 128;
         else {
             if (t !== null && t.flags & 128) e: for (t = e.child; t !== null;) {
                 if (t.tag === 13) t.memoizedState !== null && j0(t, n, e);
@@ -4624,209 +4624,209 @@
                 t.sibling.return = t.return, t = t.sibling
             }
             i &= 1
         }
         if (et(ft, i), !(e.mode & 1)) e.memoizedState = null;
         else switch (r) {
             case "forwards":
-                for (n = e.child, r = null; n !== null;) t = n.alternate, t !== null && Ju(t) === null && (r = n), n = n.sibling;
-                n = r, n === null ? (r = e.child, e.child = null) : (r = n.sibling, n.sibling = null), Od(e, !1, r, n, o);
+                for (n = e.child, r = null; n !== null;) t = n.alternate, t !== null && ec(t) === null && (r = n), n = n.sibling;
+                n = r, n === null ? (r = e.child, e.child = null) : (r = n.sibling, n.sibling = null), Md(e, !1, r, n, o);
                 break;
             case "backwards":
                 for (n = null, r = e.child, e.child = null; r !== null;) {
-                    if (t = r.alternate, t !== null && Ju(t) === null) {
+                    if (t = r.alternate, t !== null && ec(t) === null) {
                         e.child = r;
                         break
                     }
                     t = r.sibling, r.sibling = n, n = r, r = t
                 }
-                Od(e, !0, n, null, o);
+                Md(e, !0, n, null, o);
                 break;
             case "together":
-                Od(e, !1, null, null, void 0);
+                Md(e, !1, null, null, void 0);
                 break;
             default:
                 e.memoizedState = null
         }
         return e.child
     }
 
-    function Lu(t, e) {
+    function Ru(t, e) {
         !(e.mode & 1) && t !== null && (t.alternate = null, e.alternate = null, e.flags |= 2)
     }
 
-    function Qi(t, e, n) {
+    function Gi(t, e, n) {
         if (t !== null && (e.dependencies = t.dependencies), wo |= e.lanes, !(n & e.childLanes)) return null;
-        if (t !== null && e.child !== t.child) throw Error(ne(153));
+        if (t !== null && e.child !== t.child) throw Error(te(153));
         if (e.child !== null) {
             for (t = e.child, n = Ar(t, t.pendingProps), e.child = n, n.return = e; t.sibling !== null;) t = t.sibling, n = n.sibling = Ar(t, t.pendingProps), n.return = e;
             n.sibling = null
         }
         return e.child
     }
 
-    function Xk(t, e, n) {
+    function XS(t, e, n) {
         switch (e.tag) {
             case 3:
-                Tv(e), ks();
+                Tv(e), Ss();
                 break;
             case 5:
                 nv(e);
                 break;
             case 1:
-                yn(e.type) && Xu(e);
+                yn(e.type) && qu(e);
                 break;
             case 4:
-                Gh(e, e.stateNode.containerInfo);
+                Zh(e, e.stateNode.containerInfo);
                 break;
             case 10:
                 var i = e.type._context,
                     r = e.memoizedProps.value;
                 et(Gu, i._currentValue), i._currentValue = r;
                 break;
             case 13:
-                if (i = e.memoizedState, i !== null) return i.dehydrated !== null ? (et(ft, ft.current & 1), e.flags |= 128, null) : n & e.child.childLanes ? Pv(t, e, n) : (et(ft, ft.current & 1), t = Qi(t, e, n), t !== null ? t.sibling : null);
+                if (i = e.memoizedState, i !== null) return i.dehydrated !== null ? (et(ft, ft.current & 1), e.flags |= 128, null) : n & e.child.childLanes ? Dv(t, e, n) : (et(ft, ft.current & 1), t = Gi(t, e, n), t !== null ? t.sibling : null);
                 et(ft, ft.current & 1);
                 break;
             case 19:
                 if (i = (n & e.childLanes) !== 0, t.flags & 128) {
-                    if (i) return Mv(t, e, n);
+                    if (i) return Pv(t, e, n);
                     e.flags |= 128
                 }
                 if (r = e.memoizedState, r !== null && (r.rendering = null, r.tail = null, r.lastEffect = null), et(ft, ft.current), i) break;
                 return null;
             case 22:
             case 23:
                 return e.lanes = 0, Cv(t, e, n)
         }
-        return Qi(t, e, n)
+        return Gi(t, e, n)
     }
-    var Dv, yh, Ov, Av;
-    Dv = function(t, e) {
+    var Mv, mh, Ov, Av;
+    Mv = function(t, e) {
         for (var n = e.child; n !== null;) {
             if (n.tag === 5 || n.tag === 6) t.appendChild(n.stateNode);
             else if (n.tag !== 4 && n.child !== null) {
                 n.child.return = n, n = n.child;
                 continue
             }
             if (n === e) break;
             for (; n.sibling === null;) {
                 if (n.return === null || n.return === e) return;
                 n = n.return
             }
             n.sibling.return = n.return, n = n.sibling
         }
     };
-    yh = function() {};
+    mh = function() {};
     Ov = function(t, e, n, i) {
         var r = t.memoizedProps;
         if (r !== i) {
-            t = e.stateNode, mo(ki.current);
+            t = e.stateNode, mo(Si.current);
             var o = null;
             switch (n) {
                 case "input":
-                    r = jd(t, r), i = jd(t, i), o = [];
+                    r = Fd(t, r), i = Fd(t, i), o = [];
                     break;
                 case "select":
                     r = ht({}, r, {
                         value: void 0
                     }), i = ht({}, i, {
                         value: void 0
                     }), o = [];
                     break;
                 case "textarea":
-                    r = Wd(t, r), i = Wd(t, i), o = [];
+                    r = Bd(t, r), i = Bd(t, i), o = [];
                     break;
                 default:
-                    typeof r.onClick != "function" && typeof i.onClick == "function" && (t.onclick = $u)
+                    typeof r.onClick != "function" && typeof i.onClick == "function" && (t.onclick = Yu)
             }
-            Ud(n, i);
+            Vd(n, i);
             var s;
             n = null;
             for (c in r)
                 if (!i.hasOwnProperty(c) && r.hasOwnProperty(c) && r[c] != null)
                     if (c === "style") {
                         var a = r[c];
                         for (s in a) a.hasOwnProperty(s) && (n || (n = {}), n[s] = "")
-                    } else c !== "dangerouslySetInnerHTML" && c !== "children" && c !== "suppressContentEditableWarning" && c !== "suppressHydrationWarning" && c !== "autoFocus" && (Fa.hasOwnProperty(c) ? o || (o = []) : (o = o || []).push(c, null));
+                    } else c !== "dangerouslySetInnerHTML" && c !== "children" && c !== "suppressContentEditableWarning" && c !== "suppressHydrationWarning" && c !== "autoFocus" && (ja.hasOwnProperty(c) ? o || (o = []) : (o = o || []).push(c, null));
             for (c in i) {
                 var l = i[c];
                 if (a = r?.[c], i.hasOwnProperty(c) && l !== a && (l != null || a != null))
                     if (c === "style")
                         if (a) {
                             for (s in a) !a.hasOwnProperty(s) || l && l.hasOwnProperty(s) || (n || (n = {}), n[s] = "");
                             for (s in l) l.hasOwnProperty(s) && a[s] !== l[s] && (n || (n = {}), n[s] = l[s])
                         } else n || (o || (o = []), o.push(c, n)), n = l;
-                else c === "dangerouslySetInnerHTML" ? (l = l ? l.__html : void 0, a = a ? a.__html : void 0, l != null && a !== l && (o = o || []).push(c, l)) : c === "children" ? typeof l != "string" && typeof l != "number" || (o = o || []).push(c, "" + l) : c !== "suppressContentEditableWarning" && c !== "suppressHydrationWarning" && (Fa.hasOwnProperty(c) ? (l != null && c === "onScroll" && nt("scroll", t), o || a === l || (o = [])) : (o = o || []).push(c, l))
+                else c === "dangerouslySetInnerHTML" ? (l = l ? l.__html : void 0, a = a ? a.__html : void 0, l != null && a !== l && (o = o || []).push(c, l)) : c === "children" ? typeof l != "string" && typeof l != "number" || (o = o || []).push(c, "" + l) : c !== "suppressContentEditableWarning" && c !== "suppressHydrationWarning" && (ja.hasOwnProperty(c) ? (l != null && c === "onScroll" && nt("scroll", t), o || a === l || (o = [])) : (o = o || []).push(c, l))
             }
             n && (o = o || []).push("style", n);
             var c = o;
             (e.updateQueue = c) && (e.flags |= 4)
         }
     };
     Av = function(t, e, n, i) {
         n !== i && (e.flags |= 4)
     };
 
-    function wa(t, e) {
+    function Sa(t, e) {
         if (!at) switch (t.tailMode) {
             case "hidden":
                 e = t.tail;
                 for (var n = null; e !== null;) e.alternate !== null && (n = e), e = e.sibling;
                 n === null ? t.tail = null : n.sibling = null;
                 break;
             case "collapsed":
                 n = t.tail;
                 for (var i = null; n !== null;) n.alternate !== null && (i = n), n = n.sibling;
                 i === null ? e || t.tail === null ? t.tail = null : t.tail.sibling = null : i.sibling = null
         }
     }
 
-    function Gt(t) {
+    function Kt(t) {
         var e = t.alternate !== null && t.alternate.child === t.child,
             n = 0,
             i = 0;
         if (e)
             for (var r = t.child; r !== null;) n |= r.lanes | r.childLanes, i |= r.subtreeFlags & 14680064, i |= r.flags & 14680064, r.return = t, r = r.sibling;
         else
             for (r = t.child; r !== null;) n |= r.lanes | r.childLanes, i |= r.subtreeFlags, i |= r.flags, r.return = t, r = r.sibling;
         return t.subtreeFlags |= i, t.childLanes = n, e
     }
 
-    function qk(t, e, n) {
+    function qS(t, e, n) {
         var i = e.pendingProps;
-        switch (Vh(e), e.tag) {
+        switch (Wh(e), e.tag) {
             case 2:
             case 16:
             case 15:
             case 0:
             case 11:
             case 7:
             case 8:
             case 12:
             case 9:
             case 14:
-                return Gt(e), null;
+                return Kt(e), null;
             case 1:
-                return yn(e.type) && Yu(), Gt(e), null;
+                return yn(e.type) && Xu(), Kt(e), null;
             case 3:
-                return i = e.stateNode, Cs(), it(mn), it(Kt), Kh(), i.pendingContext && (i.context = i.pendingContext, i.pendingContext = null), (t === null || t.child === null) && (wu(e) ? e.flags |= 4 : t === null || t.memoizedState.isDehydrated && !(e.flags & 256) || (e.flags |= 1024, oi !== null && (Ch(oi), oi = null))), yh(t, e), Gt(e), null;
+                return i = e.stateNode, Cs(), it(mn), it(Qt), Gh(), i.pendingContext && (i.context = i.pendingContext, i.pendingContext = null), (t === null || t.child === null) && (Su(e) ? e.flags |= 4 : t === null || t.memoizedState.isDehydrated && !(e.flags & 256) || (e.flags |= 1024, oi !== null && (kh(oi), oi = null))), mh(t, e), Kt(e), null;
             case 5:
-                Qh(e);
+                Kh(e);
                 var r = mo(Ga.current);
                 if (n = e.type, t !== null && e.stateNode != null) Ov(t, e, n, i, r), t.ref !== e.ref && (e.flags |= 512, e.flags |= 2097152);
                 else {
                     if (!i) {
-                        if (e.stateNode === null) throw Error(ne(166));
-                        return Gt(e), null
+                        if (e.stateNode === null) throw Error(te(166));
+                        return Kt(e), null
                     }
-                    if (t = mo(ki.current), wu(e)) {
+                    if (t = mo(Si.current), Su(e)) {
                         i = e.stateNode, n = e.type;
                         var o = e.memoizedProps;
-                        switch (i[_i] = e, i[qa] = o, t = (e.mode & 1) !== 0, n) {
+                        switch (i[_i] = e, i[Za] = o, t = (e.mode & 1) !== 0, n) {
                             case "dialog":
                                 nt("cancel", i), nt("close", i);
                                 break;
                             case "iframe":
                             case "object":
                             case "embed":
                                 nt("load", i);
@@ -4853,39 +4853,39 @@
                                 i._wrapperState = {
                                     wasMultiple: !!o.multiple
                                 }, nt("invalid", i);
                                 break;
                             case "textarea":
                                 Zm(i, o), nt("invalid", i)
                         }
-                        Ud(n, o), r = null;
+                        Vd(n, o), r = null;
                         for (var s in o)
                             if (o.hasOwnProperty(s)) {
                                 var a = o[s];
-                                s === "children" ? typeof a == "string" ? i.textContent !== a && (o.suppressHydrationWarning !== !0 && _u(i.textContent, a, t), r = ["children", a]) : typeof a == "number" && i.textContent !== "" + a && (o.suppressHydrationWarning !== !0 && _u(i.textContent, a, t), r = ["children", "" + a]) : Fa.hasOwnProperty(s) && a != null && s === "onScroll" && nt("scroll", i)
+                                s === "children" ? typeof a == "string" ? i.textContent !== a && (o.suppressHydrationWarning !== !0 && wu(i.textContent, a, t), r = ["children", a]) : typeof a == "number" && i.textContent !== "" + a && (o.suppressHydrationWarning !== !0 && wu(i.textContent, a, t), r = ["children", "" + a]) : ja.hasOwnProperty(s) && a != null && s === "onScroll" && nt("scroll", i)
                             } switch (n) {
                             case "input":
-                                uu(i), qm(i, o, !0);
+                                cu(i), qm(i, o, !0);
                                 break;
                             case "textarea":
-                                uu(i), Gm(i);
+                                cu(i), Km(i);
                                 break;
                             case "select":
                             case "option":
                                 break;
                             default:
-                                typeof o.onClick == "function" && (i.onclick = $u)
+                                typeof o.onClick == "function" && (i.onclick = Yu)
                         }
                         i = r, e.updateQueue = i, i !== null && (e.flags |= 4)
                     } else {
                         s = r.nodeType === 9 ? r : r.ownerDocument, t === "http://www.w3.org/1999/xhtml" && (t = oy(n)), t === "http://www.w3.org/1999/xhtml" ? n === "script" ? (t = s.createElement("div"), t.innerHTML = "<script><\/script>", t = t.removeChild(t.firstChild)) : typeof i.is == "string" ? t = s.createElement(n, {
                             is: i.is
-                        }) : (t = s.createElement(n), n === "select" && (s = t, i.multiple ? s.multiple = !0 : i.size && (s.size = i.size))) : t = s.createElementNS(t, n), t[_i] = e, t[qa] = i, Dv(t, e, !1, !1), e.stateNode = t;
+                        }) : (t = s.createElement(n), n === "select" && (s = t, i.multiple ? s.multiple = !0 : i.size && (s.size = i.size))) : t = s.createElementNS(t, n), t[_i] = e, t[Za] = i, Mv(t, e, !1, !1), e.stateNode = t;
                         e: {
-                            switch (s = $d(n, i), n) {
+                            switch (s = Ud(n, i), n) {
                                 case "dialog":
                                     nt("cancel", t), nt("close", t), r = i;
                                     break;
                                 case "iframe":
                                 case "object":
                                 case "embed":
                                     nt("load", t), r = i;
@@ -4903,53 +4903,53 @@
                                 case "link":
                                     nt("error", t), nt("load", t), r = i;
                                     break;
                                 case "details":
                                     nt("toggle", t), r = i;
                                     break;
                                 case "input":
-                                    Xm(t, i), r = jd(t, i), nt("invalid", t);
+                                    Xm(t, i), r = Fd(t, i), nt("invalid", t);
                                     break;
                                 case "option":
                                     r = i;
                                     break;
                                 case "select":
                                     t._wrapperState = {
                                         wasMultiple: !!i.multiple
                                     }, r = ht({}, i, {
                                         value: void 0
                                     }), nt("invalid", t);
                                     break;
                                 case "textarea":
-                                    Zm(t, i), r = Wd(t, i), nt("invalid", t);
+                                    Zm(t, i), r = Bd(t, i), nt("invalid", t);
                                     break;
                                 default:
                                     r = i
                             }
-                            Ud(n, r),
+                            Vd(n, r),
                             a = r;
                             for (o in a)
                                 if (a.hasOwnProperty(o)) {
                                     var l = a[o];
-                                    o === "style" ? ly(t, l) : o === "dangerouslySetInnerHTML" ? (l = l ? l.__html : void 0, l != null && sy(t, l)) : o === "children" ? typeof l == "string" ? (n !== "textarea" || l !== "") && ja(t, l) : typeof l == "number" && ja(t, "" + l) : o !== "suppressContentEditableWarning" && o !== "suppressHydrationWarning" && o !== "autoFocus" && (Fa.hasOwnProperty(o) ? l != null && o === "onScroll" && nt("scroll", t) : l != null && Ph(t, o, l, s))
+                                    o === "style" ? ly(t, l) : o === "dangerouslySetInnerHTML" ? (l = l ? l.__html : void 0, l != null && sy(t, l)) : o === "children" ? typeof l == "string" ? (n !== "textarea" || l !== "") && Ha(t, l) : typeof l == "number" && Ha(t, "" + l) : o !== "suppressContentEditableWarning" && o !== "suppressHydrationWarning" && o !== "autoFocus" && (ja.hasOwnProperty(o) ? l != null && o === "onScroll" && nt("scroll", t) : l != null && Th(t, o, l, s))
                                 } switch (n) {
                                 case "input":
-                                    uu(t), qm(t, i, !1);
+                                    cu(t), qm(t, i, !1);
                                     break;
                                 case "textarea":
-                                    uu(t), Gm(t);
+                                    cu(t), Km(t);
                                     break;
                                 case "option":
                                     i.value != null && t.setAttribute("value", "" + Lr(i.value));
                                     break;
                                 case "select":
                                     t.multiple = !!i.multiple, o = i.value, o != null ? gs(t, !!i.multiple, o, !1) : i.defaultValue != null && gs(t, !!i.multiple, i.defaultValue, !0);
                                     break;
                                 default:
-                                    typeof r.onClick == "function" && (t.onclick = $u)
+                                    typeof r.onClick == "function" && (t.onclick = Yu)
                             }
                             switch (n) {
                                 case "button":
                                 case "input":
                                 case "select":
                                 case "textarea":
                                     i = !!i.autoFocus;
@@ -4961,143 +4961,143 @@
                                     i = !1
                             }
                         }
                         i && (e.flags |= 4)
                     }
                     e.ref !== null && (e.flags |= 512, e.flags |= 2097152)
                 }
-                return Gt(e), null;
+                return Kt(e), null;
             case 6:
                 if (t && e.stateNode != null) Av(t, e, t.memoizedProps, i);
                 else {
-                    if (typeof i != "string" && e.stateNode === null) throw Error(ne(166));
-                    if (n = mo(Ga.current), mo(ki.current), wu(e)) {
+                    if (typeof i != "string" && e.stateNode === null) throw Error(te(166));
+                    if (n = mo(Ga.current), mo(Si.current), Su(e)) {
                         if (i = e.stateNode, n = e.memoizedProps, i[_i] = e, (o = i.nodeValue !== n) && (t = Ln, t !== null)) switch (t.tag) {
                             case 3:
-                                _u(i.nodeValue, n, (t.mode & 1) !== 0);
+                                wu(i.nodeValue, n, (t.mode & 1) !== 0);
                                 break;
                             case 5:
-                                t.memoizedProps.suppressHydrationWarning !== !0 && _u(i.nodeValue, n, (t.mode & 1) !== 0)
+                                t.memoizedProps.suppressHydrationWarning !== !0 && wu(i.nodeValue, n, (t.mode & 1) !== 0)
                         }
                         o && (e.flags |= 4)
                     } else i = (n.nodeType === 9 ? n : n.ownerDocument).createTextNode(i), i[_i] = e, e.stateNode = i
                 }
-                return Gt(e), null;
+                return Kt(e), null;
             case 13:
                 if (it(ft), i = e.memoizedState, t === null || t.memoizedState !== null && t.memoizedState.dehydrated !== null) {
-                    if (at && An !== null && e.mode & 1 && !(e.flags & 128)) Zy(), ks(), e.flags |= 98560, o = !1;
-                    else if (o = wu(e), i !== null && i.dehydrated !== null) {
+                    if (at && An !== null && e.mode & 1 && !(e.flags & 128)) Zy(), Ss(), e.flags |= 98560, o = !1;
+                    else if (o = Su(e), i !== null && i.dehydrated !== null) {
                         if (t === null) {
-                            if (!o) throw Error(ne(318));
-                            if (o = e.memoizedState, o = o !== null ? o.dehydrated : null, !o) throw Error(ne(317));
+                            if (!o) throw Error(te(318));
+                            if (o = e.memoizedState, o = o !== null ? o.dehydrated : null, !o) throw Error(te(317));
                             o[_i] = e
-                        } else ks(), !(e.flags & 128) && (e.memoizedState = null), e.flags |= 4;
-                        Gt(e), o = !1
-                    } else oi !== null && (Ch(oi), oi = null), o = !0;
+                        } else Ss(), !(e.flags & 128) && (e.memoizedState = null), e.flags |= 4;
+                        Kt(e), o = !1
+                    } else oi !== null && (kh(oi), oi = null), o = !0;
                     if (!o) return e.flags & 65536 ? e : null
                 }
-                return e.flags & 128 ? (e.lanes = n, e) : (i = i !== null, i !== (t !== null && t.memoizedState !== null) && i && (e.child.flags |= 8192, e.mode & 1 && (t === null || ft.current & 1 ? Dt === 0 && (Dt = 3) : cp())), e.updateQueue !== null && (e.flags |= 4), Gt(e), null);
+                return e.flags & 128 ? (e.lanes = n, e) : (i = i !== null, i !== (t !== null && t.memoizedState !== null) && i && (e.child.flags |= 8192, e.mode & 1 && (t === null || ft.current & 1 ? Mt === 0 && (Mt = 3) : up())), e.updateQueue !== null && (e.flags |= 4), Kt(e), null);
             case 4:
-                return Cs(), yh(t, e), t === null && Ya(e.stateNode.containerInfo), Gt(e), null;
+                return Cs(), mh(t, e), t === null && Xa(e.stateNode.containerInfo), Kt(e), null;
             case 10:
-                return Xh(e.type._context), Gt(e), null;
+                return Yh(e.type._context), Kt(e), null;
             case 17:
-                return yn(e.type) && Yu(), Gt(e), null;
+                return yn(e.type) && Xu(), Kt(e), null;
             case 19:
-                if (it(ft), o = e.memoizedState, o === null) return Gt(e), null;
+                if (it(ft), o = e.memoizedState, o === null) return Kt(e), null;
                 if (i = (e.flags & 128) !== 0, s = o.rendering, s === null)
-                    if (i) wa(o, !1);
+                    if (i) Sa(o, !1);
                     else {
-                        if (Dt !== 0 || t !== null && t.flags & 128)
+                        if (Mt !== 0 || t !== null && t.flags & 128)
                             for (t = e.child; t !== null;) {
-                                if (s = Ju(t), s !== null) {
-                                    for (e.flags |= 128, wa(o, !1), i = s.updateQueue, i !== null && (e.updateQueue = i, e.flags |= 4), e.subtreeFlags = 0, i = n, n = e.child; n !== null;) o = n, t = i, o.flags &= 14680066, s = o.alternate, s === null ? (o.childLanes = 0, o.lanes = t, o.child = null, o.subtreeFlags = 0, o.memoizedProps = null, o.memoizedState = null, o.updateQueue = null, o.dependencies = null, o.stateNode = null) : (o.childLanes = s.childLanes, o.lanes = s.lanes, o.child = s.child, o.subtreeFlags = 0, o.deletions = null, o.memoizedProps = s.memoizedProps, o.memoizedState = s.memoizedState, o.updateQueue = s.updateQueue, o.type = s.type, t = s.dependencies, o.dependencies = t === null ? null : {
+                                if (s = ec(t), s !== null) {
+                                    for (e.flags |= 128, Sa(o, !1), i = s.updateQueue, i !== null && (e.updateQueue = i, e.flags |= 4), e.subtreeFlags = 0, i = n, n = e.child; n !== null;) o = n, t = i, o.flags &= 14680066, s = o.alternate, s === null ? (o.childLanes = 0, o.lanes = t, o.child = null, o.subtreeFlags = 0, o.memoizedProps = null, o.memoizedState = null, o.updateQueue = null, o.dependencies = null, o.stateNode = null) : (o.childLanes = s.childLanes, o.lanes = s.lanes, o.child = s.child, o.subtreeFlags = 0, o.deletions = null, o.memoizedProps = s.memoizedProps, o.memoizedState = s.memoizedState, o.updateQueue = s.updateQueue, o.type = s.type, t = s.dependencies, o.dependencies = t === null ? null : {
                                         lanes: t.lanes,
                                         firstContext: t.firstContext
                                     }), n = n.sibling;
                                     return et(ft, ft.current & 1 | 2), e.child
                                 }
                                 t = t.sibling
                             }
-                        o.tail !== null && xt() > Ts && (e.flags |= 128, i = !0, wa(o, !1), e.lanes = 4194304)
+                        o.tail !== null && xt() > Ts && (e.flags |= 128, i = !0, Sa(o, !1), e.lanes = 4194304)
                     }
                 else {
                     if (!i)
-                        if (t = Ju(s), t !== null) {
-                            if (e.flags |= 128, i = !0, n = t.updateQueue, n !== null && (e.updateQueue = n, e.flags |= 4), wa(o, !0), o.tail === null && o.tailMode === "hidden" && !s.alternate && !at) return Gt(e), null
-                        } else 2 * xt() - o.renderingStartTime > Ts && n !== 1073741824 && (e.flags |= 128, i = !0, wa(o, !1), e.lanes = 4194304);
+                        if (t = ec(s), t !== null) {
+                            if (e.flags |= 128, i = !0, n = t.updateQueue, n !== null && (e.updateQueue = n, e.flags |= 4), Sa(o, !0), o.tail === null && o.tailMode === "hidden" && !s.alternate && !at) return Kt(e), null
+                        } else 2 * xt() - o.renderingStartTime > Ts && n !== 1073741824 && (e.flags |= 128, i = !0, Sa(o, !1), e.lanes = 4194304);
                     o.isBackwards ? (s.sibling = e.child, e.child = s) : (n = o.last, n !== null ? n.sibling = s : e.child = s, o.last = s)
                 }
-                return o.tail !== null ? (e = o.tail, o.rendering = e, o.tail = e.sibling, o.renderingStartTime = xt(), e.sibling = null, n = ft.current, et(ft, i ? n & 1 | 2 : n & 1), e) : (Gt(e), null);
+                return o.tail !== null ? (e = o.tail, o.rendering = e, o.tail = e.sibling, o.renderingStartTime = xt(), e.sibling = null, n = ft.current, et(ft, i ? n & 1 | 2 : n & 1), e) : (Kt(e), null);
             case 22:
             case 23:
-                return up(), i = e.memoizedState !== null, t !== null && t.memoizedState !== null !== i && (e.flags |= 8192), i && e.mode & 1 ? On & 1073741824 && (Gt(e), e.subtreeFlags & 6 && (e.flags |= 8192)) : Gt(e), null;
+                return lp(), i = e.memoizedState !== null, t !== null && t.memoizedState !== null !== i && (e.flags |= 8192), i && e.mode & 1 ? On & 1073741824 && (Kt(e), e.subtreeFlags & 6 && (e.flags |= 8192)) : Kt(e), null;
             case 24:
                 return null;
             case 25:
                 return null
         }
-        throw Error(ne(156, e.tag))
+        throw Error(te(156, e.tag))
     }
 
-    function Zk(t, e) {
-        switch (Vh(e), e.tag) {
+    function ZS(t, e) {
+        switch (Wh(e), e.tag) {
             case 1:
-                return yn(e.type) && Yu(), t = e.flags, t & 65536 ? (e.flags = t & -65537 | 128, e) : null;
+                return yn(e.type) && Xu(), t = e.flags, t & 65536 ? (e.flags = t & -65537 | 128, e) : null;
             case 3:
-                return Cs(), it(mn), it(Kt), Kh(), t = e.flags, t & 65536 && !(t & 128) ? (e.flags = t & -65537 | 128, e) : null;
+                return Cs(), it(mn), it(Qt), Gh(), t = e.flags, t & 65536 && !(t & 128) ? (e.flags = t & -65537 | 128, e) : null;
             case 5:
-                return Qh(e), null;
+                return Kh(e), null;
             case 13:
                 if (it(ft), t = e.memoizedState, t !== null && t.dehydrated !== null) {
-                    if (e.alternate === null) throw Error(ne(340));
-                    ks()
+                    if (e.alternate === null) throw Error(te(340));
+                    Ss()
                 }
                 return t = e.flags, t & 65536 ? (e.flags = t & -65537 | 128, e) : null;
             case 19:
                 return it(ft), null;
             case 4:
                 return Cs(), null;
             case 10:
-                return Xh(e.type._context), null;
+                return Yh(e.type._context), null;
             case 22:
             case 23:
-                return up(), null;
+                return lp(), null;
             case 24:
                 return null;
             default:
                 return null
         }
     }
-    var Cu = !1,
-        Qt = !1,
-        Gk = typeof WeakSet == "function" ? WeakSet : Set,
+    var Eu = !1,
+        Gt = !1,
+        KS = typeof WeakSet == "function" ? WeakSet : Set,
         ue = null;
 
     function hs(t, e) {
         var n = t.ref;
         if (n !== null)
             if (typeof n == "function") try {
                 n(null)
             } catch (i) {
                 vt(t, e, i)
             } else n.current = null
     }
 
-    function vh(t, e, n) {
+    function yh(t, e, n) {
         try {
             n()
         } catch (i) {
             vt(t, e, i)
         }
     }
     var H0 = !1;
 
-    function Qk(t, e) {
-        if (th = Wu, t = Ny(), Bh(t)) {
+    function GS(t, e) {
+        if (eh = Vu, t = Ny(), Hh(t)) {
             if ("selectionStart" in t) var n = {
                 start: t.selectionStart,
                 end: t.selectionEnd
             };
             else e: {
                 n = (n = t.ownerDocument) && n.defaultView || window;
                 var i = n.getSelection && n.getSelection();
@@ -5135,90 +5135,90 @@
                 } else n = null
             }
             n = n || {
                 start: 0,
                 end: 0
             }
         } else n = null;
-        for (nh = {
+        for (th = {
                 focusedElem: t,
                 selectionRange: n
-            }, Wu = !1, ue = e; ue !== null;)
+            }, Vu = !1, ue = e; ue !== null;)
             if (e = ue, t = e.child, (e.subtreeFlags & 1028) !== 0 && t !== null) t.return = e, ue = t;
             else
                 for (; ue !== null;) {
                     e = ue;
                     try {
-                        var w = e.alternate;
+                        var _ = e.alternate;
                         if (e.flags & 1024) switch (e.tag) {
                             case 0:
                             case 11:
                             case 15:
                                 break;
                             case 1:
-                                if (w !== null) {
-                                    var S = w.memoizedProps,
-                                        A = w.memoizedState,
-                                        _ = e.stateNode,
-                                        C = _.getSnapshotBeforeUpdate(e.elementType === e.type ? S : ii(e.type, S), A);
-                                    _.__reactInternalSnapshotBeforeUpdate = C
+                                if (_ !== null) {
+                                    var C = _.memoizedProps,
+                                        A = _.memoizedState,
+                                        w = e.stateNode,
+                                        k = w.getSnapshotBeforeUpdate(e.elementType === e.type ? C : ii(e.type, C), A);
+                                    w.__reactInternalSnapshotBeforeUpdate = k
                                 }
                                 break;
                             case 3:
-                                var M = e.stateNode.containerInfo;
-                                M.nodeType === 1 ? M.textContent = "" : M.nodeType === 9 && M.documentElement && M.removeChild(M.documentElement);
+                                var P = e.stateNode.containerInfo;
+                                P.nodeType === 1 ? P.textContent = "" : P.nodeType === 9 && P.documentElement && P.removeChild(P.documentElement);
                                 break;
                             case 5:
                             case 6:
                             case 4:
                             case 17:
                                 break;
                             default:
-                                throw Error(ne(163))
+                                throw Error(te(163))
                         }
                     } catch (z) {
                         vt(e, e.return, z)
                     }
                     if (t = e.sibling, t !== null) {
                         t.return = e.return, ue = t;
                         break
                     }
                     ue = e.return
                 }
-        return w = H0, H0 = !1, w
+        return _ = H0, H0 = !1, _
     }
 
-    function Ia(t, e, n) {
+    function Na(t, e, n) {
         var i = e.updateQueue;
         if (i = i !== null ? i.lastEffect : null, i !== null) {
             var r = i = i.next;
             do {
                 if ((r.tag & t) === t) {
                     var o = r.destroy;
-                    r.destroy = void 0, o !== void 0 && vh(e, n, o)
+                    r.destroy = void 0, o !== void 0 && yh(e, n, o)
                 }
                 r = r.next
             } while (r !== i)
         }
     }
 
-    function gc(t, e) {
+    function mc(t, e) {
         if (e = e.updateQueue, e = e !== null ? e.lastEffect : null, e !== null) {
             var n = e = e.next;
             do {
                 if ((n.tag & t) === t) {
                     var i = n.create;
                     n.destroy = i()
                 }
                 n = n.next
             } while (n !== e)
         }
     }
 
-    function xh(t) {
+    function vh(t) {
         var e = t.ref;
         if (e !== null) {
             var n = t.stateNode;
             switch (t.tag) {
                 case 5:
                     t = n;
                     break;
@@ -5227,15 +5227,15 @@
             }
             typeof e == "function" ? e(t) : e.current = t
         }
     }
 
     function Lv(t) {
         var e = t.alternate;
-        e !== null && (t.alternate = null, Lv(e)), t.child = null, t.deletions = null, t.sibling = null, t.tag === 5 && (e = t.stateNode, e !== null && (delete e[_i], delete e[qa], delete e[oh], delete e[Lk], delete e[Rk])), t.stateNode = null, t.return = null, t.dependencies = null, t.memoizedProps = null, t.memoizedState = null, t.pendingProps = null, t.stateNode = null, t.updateQueue = null
+        e !== null && (t.alternate = null, Lv(e)), t.child = null, t.deletions = null, t.sibling = null, t.tag === 5 && (e = t.stateNode, e !== null && (delete e[_i], delete e[Za], delete e[rh], delete e[LS], delete e[RS])), t.stateNode = null, t.return = null, t.dependencies = null, t.memoizedProps = null, t.memoizedState = null, t.pendingProps = null, t.stateNode = null, t.updateQueue = null
     }
 
     function Rv(t) {
         return t.tag === 5 || t.tag === 3 || t.tag === 4
     }
 
     function B0(t) {
@@ -5248,92 +5248,92 @@
                 if (t.flags & 2 || t.child === null || t.tag === 4) continue e;
                 t.child.return = t, t = t.child
             }
             if (!(t.flags & 2)) return t.stateNode
         }
     }
 
-    function bh(t, e, n) {
+    function xh(t, e, n) {
         var i = t.tag;
-        if (i === 5 || i === 6) t = t.stateNode, e ? n.nodeType === 8 ? n.parentNode.insertBefore(t, e) : n.insertBefore(t, e) : (n.nodeType === 8 ? (e = n.parentNode, e.insertBefore(t, n)) : (e = n, e.appendChild(t)), n = n._reactRootContainer, n != null || e.onclick !== null || (e.onclick = $u));
+        if (i === 5 || i === 6) t = t.stateNode, e ? n.nodeType === 8 ? n.parentNode.insertBefore(t, e) : n.insertBefore(t, e) : (n.nodeType === 8 ? (e = n.parentNode, e.insertBefore(t, n)) : (e = n, e.appendChild(t)), n = n._reactRootContainer, n != null || e.onclick !== null || (e.onclick = Yu));
         else if (i !== 4 && (t = t.child, t !== null))
-            for (bh(t, e, n), t = t.sibling; t !== null;) bh(t, e, n), t = t.sibling
+            for (xh(t, e, n), t = t.sibling; t !== null;) xh(t, e, n), t = t.sibling
     }
 
-    function _h(t, e, n) {
+    function bh(t, e, n) {
         var i = t.tag;
         if (i === 5 || i === 6) t = t.stateNode, e ? n.insertBefore(t, e) : n.appendChild(t);
         else if (i !== 4 && (t = t.child, t !== null))
-            for (_h(t, e, n), t = t.sibling; t !== null;) _h(t, e, n), t = t.sibling
+            for (bh(t, e, n), t = t.sibling; t !== null;) bh(t, e, n), t = t.sibling
     }
     var Ht = null,
         ri = !1;
 
     function vr(t, e, n) {
         for (n = n.child; n !== null;) Iv(t, e, n), n = n.sibling
     }
 
     function Iv(t, e, n) {
         if (wi && typeof wi.onCommitFiberUnmount == "function") try {
-            wi.onCommitFiberUnmount(ac, n)
+            wi.onCommitFiberUnmount(lc, n)
         } catch {}
         switch (n.tag) {
             case 5:
-                Qt || hs(n, e);
+                Gt || hs(n, e);
             case 6:
                 var i = Ht,
                     r = ri;
                 Ht = null, vr(t, e, n), Ht = i, ri = r, Ht !== null && (ri ? (t = Ht, n = n.stateNode, t.nodeType === 8 ? t.parentNode.removeChild(n) : t.removeChild(n)) : Ht.removeChild(n.stateNode));
                 break;
             case 18:
-                Ht !== null && (ri ? (t = Ht, n = n.stateNode, t.nodeType === 8 ? Sd(t.parentNode, n) : t.nodeType === 1 && Sd(t, n), Va(t)) : Sd(Ht, n.stateNode));
+                Ht !== null && (ri ? (t = Ht, n = n.stateNode, t.nodeType === 8 ? Sd(t.parentNode, n) : t.nodeType === 1 && Sd(t, n), Ua(t)) : Sd(Ht, n.stateNode));
                 break;
             case 4:
                 i = Ht, r = ri, Ht = n.stateNode.containerInfo, ri = !0, vr(t, e, n), Ht = i, ri = r;
                 break;
             case 0:
             case 11:
             case 14:
             case 15:
-                if (!Qt && (i = n.updateQueue, i !== null && (i = i.lastEffect, i !== null))) {
+                if (!Gt && (i = n.updateQueue, i !== null && (i = i.lastEffect, i !== null))) {
                     r = i = i.next;
                     do {
                         var o = r,
                             s = o.destroy;
-                        o = o.tag, s !== void 0 && (o & 2 || o & 4) && vh(n, e, s), r = r.next
+                        o = o.tag, s !== void 0 && (o & 2 || o & 4) && yh(n, e, s), r = r.next
                     } while (r !== i)
                 }
                 vr(t, e, n);
                 break;
             case 1:
-                if (!Qt && (hs(n, e), i = n.stateNode, typeof i.componentWillUnmount == "function")) try {
+                if (!Gt && (hs(n, e), i = n.stateNode, typeof i.componentWillUnmount == "function")) try {
                     i.props = n.memoizedProps, i.state = n.memoizedState, i.componentWillUnmount()
                 } catch (a) {
                     vt(n, e, a)
                 }
                 vr(t, e, n);
                 break;
             case 21:
                 vr(t, e, n);
                 break;
             case 22:
-                n.mode & 1 ? (Qt = (i = Qt) || n.memoizedState !== null, vr(t, e, n), Qt = i) : vr(t, e, n);
+                n.mode & 1 ? (Gt = (i = Gt) || n.memoizedState !== null, vr(t, e, n), Gt = i) : vr(t, e, n);
                 break;
             default:
                 vr(t, e, n)
         }
     }
 
     function W0(t) {
         var e = t.updateQueue;
         if (e !== null) {
             t.updateQueue = null;
             var n = t.stateNode;
-            n === null && (n = t.stateNode = new Gk), e.forEach(function(i) {
-                var r = sS.bind(null, t, i);
+            n === null && (n = t.stateNode = new KS), e.forEach(function(i) {
+                var r = sk.bind(null, t, i);
                 n.has(i) || (n.add(i), i.then(r, r))
             })
         }
     }
 
     function ni(t, e) {
         var n = e.deletions;
@@ -5354,15 +5354,15 @@
                                 break e;
                             case 4:
                                 Ht = a.stateNode.containerInfo, ri = !0;
                                 break e
                         }
                         a = a.return
                     }
-                    if (Ht === null) throw Error(ne(160));
+                    if (Ht === null) throw Error(te(160));
                     Iv(o, s, r), Ht = null, ri = !1;
                     var l = r.alternate;
                     l !== null && (l.return = null), r.return = null
                 } catch (c) {
                     vt(r, e, c)
                 }
             }
@@ -5376,114 +5376,114 @@
         switch (t.tag) {
             case 0:
             case 11:
             case 14:
             case 15:
                 if (ni(e, t), xi(t), i & 4) {
                     try {
-                        Ia(3, t, t.return), gc(3, t)
-                    } catch (S) {
-                        vt(t, t.return, S)
+                        Na(3, t, t.return), mc(3, t)
+                    } catch (C) {
+                        vt(t, t.return, C)
                     }
                     try {
-                        Ia(5, t, t.return)
-                    } catch (S) {
-                        vt(t, t.return, S)
+                        Na(5, t, t.return)
+                    } catch (C) {
+                        vt(t, t.return, C)
                     }
                 }
                 break;
             case 1:
                 ni(e, t), xi(t), i & 512 && n !== null && hs(n, n.return);
                 break;
             case 5:
                 if (ni(e, t), xi(t), i & 512 && n !== null && hs(n, n.return), t.flags & 32) {
                     var r = t.stateNode;
                     try {
-                        ja(r, "")
-                    } catch (S) {
-                        vt(t, t.return, S)
+                        Ha(r, "")
+                    } catch (C) {
+                        vt(t, t.return, C)
                     }
                 }
                 if (i & 4 && (r = t.stateNode, r != null)) {
                     var o = t.memoizedProps,
                         s = n !== null ? n.memoizedProps : o,
                         a = t.type,
                         l = t.updateQueue;
                     if (t.updateQueue = null, l !== null) try {
-                        a === "input" && o.type === "radio" && o.name != null && iy(r, o), $d(a, s);
-                        var c = $d(a, o);
+                        a === "input" && o.type === "radio" && o.name != null && iy(r, o), Ud(a, s);
+                        var c = Ud(a, o);
                         for (s = 0; s < l.length; s += 2) {
                             var d = l[s],
                                 g = l[s + 1];
-                            d === "style" ? ly(r, g) : d === "dangerouslySetInnerHTML" ? sy(r, g) : d === "children" ? ja(r, g) : Ph(r, d, g, c)
+                            d === "style" ? ly(r, g) : d === "dangerouslySetInnerHTML" ? sy(r, g) : d === "children" ? Ha(r, g) : Th(r, d, g, c)
                         }
                         switch (a) {
                             case "input":
-                                Hd(r, o);
+                                jd(r, o);
                                 break;
                             case "textarea":
                                 ry(r, o);
                                 break;
                             case "select":
                                 var y = r._wrapperState.wasMultiple;
                                 r._wrapperState.wasMultiple = !!o.multiple;
                                 var x = o.value;
                                 x != null ? gs(r, !!o.multiple, x, !1) : y !== !!o.multiple && (o.defaultValue != null ? gs(r, !!o.multiple, o.defaultValue, !0) : gs(r, !!o.multiple, o.multiple ? [] : "", !1))
                         }
-                        r[qa] = o
-                    } catch (S) {
-                        vt(t, t.return, S)
+                        r[Za] = o
+                    } catch (C) {
+                        vt(t, t.return, C)
                     }
                 }
                 break;
             case 6:
                 if (ni(e, t), xi(t), i & 4) {
-                    if (t.stateNode === null) throw Error(ne(162));
+                    if (t.stateNode === null) throw Error(te(162));
                     r = t.stateNode, o = t.memoizedProps;
                     try {
                         r.nodeValue = o
-                    } catch (S) {
-                        vt(t, t.return, S)
+                    } catch (C) {
+                        vt(t, t.return, C)
                     }
                 }
                 break;
             case 3:
                 if (ni(e, t), xi(t), i & 4 && n !== null && n.memoizedState.isDehydrated) try {
-                    Va(e.containerInfo)
-                } catch (S) {
-                    vt(t, t.return, S)
+                    Ua(e.containerInfo)
+                } catch (C) {
+                    vt(t, t.return, C)
                 }
                 break;
             case 4:
                 ni(e, t), xi(t);
                 break;
             case 13:
-                ni(e, t), xi(t), r = t.child, r.flags & 8192 && (o = r.memoizedState !== null, r.stateNode.isHidden = o, !o || r.alternate !== null && r.alternate.memoizedState !== null || (ap = xt())), i & 4 && W0(t);
+                ni(e, t), xi(t), r = t.child, r.flags & 8192 && (o = r.memoizedState !== null, r.stateNode.isHidden = o, !o || r.alternate !== null && r.alternate.memoizedState !== null || (sp = xt())), i & 4 && W0(t);
                 break;
             case 22:
-                if (d = n !== null && n.memoizedState !== null, t.mode & 1 ? (Qt = (c = Qt) || d, ni(e, t), Qt = c) : ni(e, t), xi(t), i & 8192) {
+                if (d = n !== null && n.memoizedState !== null, t.mode & 1 ? (Gt = (c = Gt) || d, ni(e, t), Gt = c) : ni(e, t), xi(t), i & 8192) {
                     if (c = t.memoizedState !== null, (t.stateNode.isHidden = c) && !d && t.mode & 1)
                         for (ue = t, d = t.child; d !== null;) {
                             for (g = ue = d; ue !== null;) {
                                 switch (y = ue, x = y.child, y.tag) {
                                     case 0:
                                     case 11:
                                     case 14:
                                     case 15:
-                                        Ia(4, y, y.return);
+                                        Na(4, y, y.return);
                                         break;
                                     case 1:
                                         hs(y, y.return);
-                                        var w = y.stateNode;
-                                        if (typeof w.componentWillUnmount == "function") {
+                                        var _ = y.stateNode;
+                                        if (typeof _.componentWillUnmount == "function") {
                                             i = y, n = y.return;
                                             try {
-                                                e = i, w.props = e.memoizedProps, w.state = e.memoizedState, w.componentWillUnmount()
-                                            } catch (S) {
-                                                vt(i, n, S)
+                                                e = i, _.props = e.memoizedProps, _.state = e.memoizedState, _.componentWillUnmount()
+                                            } catch (C) {
+                                                vt(i, n, C)
                                             }
                                         }
                                         break;
                                     case 5:
                                         hs(y, y.return);
                                         break;
                                     case 22:
@@ -5498,23 +5498,23 @@
                         }
                     e: for (d = null, g = t;;) {
                         if (g.tag === 5) {
                             if (d === null) {
                                 d = g;
                                 try {
                                     r = g.stateNode, c ? (o = r.style, typeof o.setProperty == "function" ? o.setProperty("display", "none", "important") : o.display = "none") : (a = g.stateNode, l = g.memoizedProps.style, s = l != null && l.hasOwnProperty("display") ? l.display : null, a.style.display = ay("display", s))
-                                } catch (S) {
-                                    vt(t, t.return, S)
+                                } catch (C) {
+                                    vt(t, t.return, C)
                                 }
                             }
                         } else if (g.tag === 6) {
                             if (d === null) try {
                                 g.stateNode.nodeValue = c ? "" : g.memoizedProps
-                            } catch (S) {
-                                vt(t, t.return, S)
+                            } catch (C) {
+                                vt(t, t.return, C)
                             }
                         } else if ((g.tag !== 22 && g.tag !== 23 || g.memoizedState === null || g === t) && g.child !== null) {
                             g.child.return = g, g = g.child;
                             continue
                         }
                         if (g === t) break e;
                         for (; g.sibling === null;) {
@@ -5543,60 +5543,60 @@
                     for (var n = t.return; n !== null;) {
                         if (Rv(n)) {
                             var i = n;
                             break e
                         }
                         n = n.return
                     }
-                    throw Error(ne(160))
+                    throw Error(te(160))
                 }
                 switch (i.tag) {
                     case 5:
                         var r = i.stateNode;
-                        i.flags & 32 && (ja(r, ""), i.flags &= -33);
+                        i.flags & 32 && (Ha(r, ""), i.flags &= -33);
                         var o = B0(t);
-                        _h(t, o, r);
+                        bh(t, o, r);
                         break;
                     case 3:
                     case 4:
                         var s = i.stateNode.containerInfo,
                             a = B0(t);
-                        bh(t, a, s);
+                        xh(t, a, s);
                         break;
                     default:
-                        throw Error(ne(161))
+                        throw Error(te(161))
                 }
             }
             catch (l) {
                 vt(t, t.return, l)
             }
             t.flags &= -3
         }
         e & 4096 && (t.flags &= -4097)
     }
 
-    function Kk(t, e, n) {
+    function QS(t, e, n) {
         ue = t, zv(t, e, n)
     }
 
     function zv(t, e, n) {
         for (var i = (t.mode & 1) !== 0; ue !== null;) {
             var r = ue,
                 o = r.child;
             if (r.tag === 22 && i) {
-                var s = r.memoizedState !== null || Cu;
+                var s = r.memoizedState !== null || Eu;
                 if (!s) {
                     var a = r.alternate,
-                        l = a !== null && a.memoizedState !== null || Qt;
-                    a = Cu;
-                    var c = Qt;
-                    if (Cu = s, (Qt = l) && !c)
+                        l = a !== null && a.memoizedState !== null || Gt;
+                    a = Eu;
+                    var c = Gt;
+                    if (Eu = s, (Gt = l) && !c)
                         for (ue = r; ue !== null;) s = ue, l = s.child, s.tag === 22 && s.memoizedState !== null ? $0(r) : l !== null ? (l.return = s, ue = l) : $0(r);
                     for (; o !== null;) ue = o, zv(o, e, n), o = o.sibling;
-                    ue = r, Cu = a, Qt = c
+                    ue = r, Eu = a, Gt = c
                 }
                 V0(t, e, n)
             } else r.subtreeFlags & 8772 && o !== null ? (o.return = r, ue = o) : V0(t, e, n)
         }
     }
 
     function V0(t) {
@@ -5605,19 +5605,19 @@
             if (e.flags & 8772) {
                 var n = e.alternate;
                 try {
                     if (e.flags & 8772) switch (e.tag) {
                         case 0:
                         case 11:
                         case 15:
-                            Qt || gc(5, e);
+                            Gt || mc(5, e);
                             break;
                         case 1:
                             var i = e.stateNode;
-                            if (e.flags & 4 && !Qt)
+                            if (e.flags & 4 && !Gt)
                                 if (n === null) i.componentDidMount();
                                 else {
                                     var r = e.elementType === e.type ? n.memoizedProps : ii(e.type, n.memoizedProps);
                                     i.componentDidUpdate(r, n.memoizedState, i.__reactInternalSnapshotBeforeUpdate)
                                 } var o = e.updateQueue;
                             o !== null && E0(e, o, i);
                             break;
@@ -5660,30 +5660,30 @@
                         case 13:
                             if (e.memoizedState === null) {
                                 var c = e.alternate;
                                 if (c !== null) {
                                     var d = c.memoizedState;
                                     if (d !== null) {
                                         var g = d.dehydrated;
-                                        g !== null && Va(g)
+                                        g !== null && Ua(g)
                                     }
                                 }
                             }
                             break;
                         case 19:
                         case 17:
                         case 21:
                         case 22:
                         case 23:
                         case 25:
                             break;
                         default:
-                            throw Error(ne(163))
+                            throw Error(te(163))
                     }
-                    Qt || e.flags & 512 && xh(e)
+                    Gt || e.flags & 512 && vh(e)
                 } catch (y) {
                     vt(e, e.return, y)
                 }
             }
             if (e === t) {
                 ue = null;
                 break
@@ -5718,15 +5718,15 @@
             try {
                 switch (e.tag) {
                     case 0:
                     case 11:
                     case 15:
                         var n = e.return;
                         try {
-                            gc(4, e)
+                            mc(4, e)
                         } catch (l) {
                             vt(e, n, l)
                         }
                         break;
                     case 1:
                         var i = e.stateNode;
                         if (typeof i.componentDidMount == "function") {
@@ -5735,23 +5735,23 @@
                                 i.componentDidMount()
                             } catch (l) {
                                 vt(e, r, l)
                             }
                         }
                         var o = e.return;
                         try {
-                            xh(e)
+                            vh(e)
                         } catch (l) {
                             vt(e, o, l)
                         }
                         break;
                     case 5:
                         var s = e.return;
                         try {
-                            xh(e)
+                            vh(e)
                         } catch (l) {
                             vt(e, s, l)
                         }
                 }
             } catch (l) {
                 vt(e, e.return, l)
             }
@@ -5763,169 +5763,169 @@
             if (a !== null) {
                 a.return = e.return, ue = a;
                 break
             }
             ue = e.return
         }
     }
-    var Jk = Math.ceil,
-        nc = Ki.ReactCurrentDispatcher,
-        op = Ki.ReactCurrentOwner,
-        Xn = Ki.ReactCurrentBatchConfig,
+    var JS = Math.ceil,
+        ic = Qi.ReactCurrentDispatcher,
+        rp = Qi.ReactCurrentOwner,
+        Xn = Qi.ReactCurrentBatchConfig,
         Ne = 0,
         It = null,
-        kt = null,
+        St = null,
         Bt = 0,
         On = 0,
         ps = Nr(0),
-        Dt = 0,
-        el = null,
+        Mt = 0,
+        tl = null,
         wo = 0,
-        mc = 0,
-        sp = 0,
-        Na = null,
+        yc = 0,
+        op = 0,
+        za = null,
         pn = null,
-        ap = 0,
+        sp = 0,
         Ts = 1 / 0,
         Vi = null,
-        ic = !1,
+        rc = !1,
+        _h = null,
+        Mr = null,
+        Tu = !1,
+        kr = null,
+        oc = 0,
+        Fa = 0,
         wh = null,
-        Dr = null,
-        Eu = !1,
-        Sr = null,
-        rc = 0,
-        za = 0,
-        kh = null,
-        Ru = -1,
-        Iu = 0;
+        Iu = -1,
+        Nu = 0;
 
     function nn() {
-        return Ne & 6 ? xt() : Ru !== -1 ? Ru : Ru = xt()
+        return Ne & 6 ? xt() : Iu !== -1 ? Iu : Iu = xt()
     }
 
     function Or(t) {
-        return t.mode & 1 ? Ne & 2 && Bt !== 0 ? Bt & -Bt : Nk.transition !== null ? (Iu === 0 && (Iu = by()), Iu) : (t = Be, t !== 0 || (t = window.event, t = t === void 0 ? 16 : Ty(t.type)), t) : 1
+        return t.mode & 1 ? Ne & 2 && Bt !== 0 ? Bt & -Bt : NS.transition !== null ? (Nu === 0 && (Nu = by()), Nu) : (t = Be, t !== 0 || (t = window.event, t = t === void 0 ? 16 : Ty(t.type)), t) : 1
     }
 
     function ai(t, e, n, i) {
-        if (50 < za) throw za = 0, kh = null, Error(ne(185));
-        tl(t, n, i), (!(Ne & 2) || t !== It) && (t === It && (!(Ne & 2) && (mc |= n), Dt === 4 && wr(t, Bt)), vn(t, i), n === 1 && Ne === 0 && !(e.mode & 1) && (Ts = xt() + 500, dc && zr()))
+        if (50 < Fa) throw Fa = 0, wh = null, Error(te(185));
+        nl(t, n, i), (!(Ne & 2) || t !== It) && (t === It && (!(Ne & 2) && (yc |= n), Mt === 4 && wr(t, Bt)), vn(t, i), n === 1 && Ne === 0 && !(e.mode & 1) && (Ts = xt() + 500, hc && zr()))
     }
 
     function vn(t, e) {
         var n = t.callbackNode;
         Fw(t, e);
-        var i = Bu(t, t === It ? Bt : 0);
+        var i = Wu(t, t === It ? Bt : 0);
         if (i === 0) n !== null && Jm(n), t.callbackNode = null, t.callbackPriority = 0;
         else if (e = i & -i, t.callbackPriority !== e) {
-            if (n != null && Jm(n), e === 1) t.tag === 0 ? Ik(Y0.bind(null, t)) : Yy(Y0.bind(null, t)), Ok(function() {
+            if (n != null && Jm(n), e === 1) t.tag === 0 ? IS(Y0.bind(null, t)) : Yy(Y0.bind(null, t)), OS(function() {
                 !(Ne & 6) && zr()
             }), n = null;
             else {
                 switch (_y(i)) {
                     case 1:
-                        n = Lh;
+                        n = Ah;
                         break;
                     case 4:
                         n = vy;
                         break;
                     case 16:
-                        n = Hu;
+                        n = Bu;
                         break;
                     case 536870912:
                         n = xy;
                         break;
                     default:
-                        n = Hu
+                        n = Bu
                 }
                 n = $v(n, Fv.bind(null, t))
             }
             t.callbackPriority = e, t.callbackNode = n
         }
     }
 
     function Fv(t, e) {
-        if (Ru = -1, Iu = 0, Ne & 6) throw Error(ne(327));
+        if (Iu = -1, Nu = 0, Ne & 6) throw Error(te(327));
         var n = t.callbackNode;
         if (bs() && t.callbackNode !== n) return null;
-        var i = Bu(t, t === It ? Bt : 0);
+        var i = Wu(t, t === It ? Bt : 0);
         if (i === 0) return null;
-        if (i & 30 || i & t.expiredLanes || e) e = oc(t, i);
+        if (i & 30 || i & t.expiredLanes || e) e = sc(t, i);
         else {
             e = i;
             var r = Ne;
             Ne |= 2;
             var o = Hv();
             (It !== t || Bt !== e) && (Vi = null, Ts = xt() + 500, yo(t, e));
             do try {
-                nS();
+                nk();
                 break
             } catch (a) {
                 jv(t, a)
             }
             while (!0);
-            Yh(), nc.current = o, Ne = r, kt !== null ? e = 0 : (It = null, Bt = 0, e = Dt)
+            $h(), ic.current = o, Ne = r, St !== null ? e = 0 : (It = null, Bt = 0, e = Mt)
         }
         if (e !== 0) {
-            if (e === 2 && (r = Gd(t), r !== 0 && (i = r, e = Sh(t, r))), e === 1) throw n = el, yo(t, 0), wr(t, i), vn(t, xt()), n;
+            if (e === 2 && (r = Zd(t), r !== 0 && (i = r, e = Sh(t, r))), e === 1) throw n = tl, yo(t, 0), wr(t, i), vn(t, xt()), n;
             if (e === 6) wr(t, i);
             else {
-                if (r = t.current.alternate, !(i & 30) && !eS(r) && (e = oc(t, i), e === 2 && (o = Gd(t), o !== 0 && (i = o, e = Sh(t, o))), e === 1)) throw n = el, yo(t, 0), wr(t, i), vn(t, xt()), n;
+                if (r = t.current.alternate, !(i & 30) && !ek(r) && (e = sc(t, i), e === 2 && (o = Zd(t), o !== 0 && (i = o, e = Sh(t, o))), e === 1)) throw n = tl, yo(t, 0), wr(t, i), vn(t, xt()), n;
                 switch (t.finishedWork = r, t.finishedLanes = i, e) {
                     case 0:
                     case 1:
-                        throw Error(ne(345));
+                        throw Error(te(345));
                     case 2:
                         ho(t, pn, Vi);
                         break;
                     case 3:
-                        if (wr(t, i), (i & 130023424) === i && (e = ap + 500 - xt(), 10 < e)) {
-                            if (Bu(t, 0) !== 0) break;
+                        if (wr(t, i), (i & 130023424) === i && (e = sp + 500 - xt(), 10 < e)) {
+                            if (Wu(t, 0) !== 0) break;
                             if (r = t.suspendedLanes, (r & i) !== i) {
                                 nn(), t.pingedLanes |= t.suspendedLanes & r;
                                 break
                             }
-                            t.timeoutHandle = rh(ho.bind(null, t, pn, Vi), e);
+                            t.timeoutHandle = ih(ho.bind(null, t, pn, Vi), e);
                             break
                         }
                         ho(t, pn, Vi);
                         break;
                     case 4:
                         if (wr(t, i), (i & 4194240) === i) break;
                         for (e = t.eventTimes, r = -1; 0 < i;) {
                             var s = 31 - si(i);
                             o = 1 << s, s = e[s], s > r && (r = s), i &= ~o
                         }
-                        if (i = r, i = xt() - i, i = (120 > i ? 120 : 480 > i ? 480 : 1080 > i ? 1080 : 1920 > i ? 1920 : 3e3 > i ? 3e3 : 4320 > i ? 4320 : 1960 * Jk(i / 1960)) - i, 10 < i) {
-                            t.timeoutHandle = rh(ho.bind(null, t, pn, Vi), i);
+                        if (i = r, i = xt() - i, i = (120 > i ? 120 : 480 > i ? 480 : 1080 > i ? 1080 : 1920 > i ? 1920 : 3e3 > i ? 3e3 : 4320 > i ? 4320 : 1960 * JS(i / 1960)) - i, 10 < i) {
+                            t.timeoutHandle = ih(ho.bind(null, t, pn, Vi), i);
                             break
                         }
                         ho(t, pn, Vi);
                         break;
                     case 5:
                         ho(t, pn, Vi);
                         break;
                     default:
-                        throw Error(ne(329))
+                        throw Error(te(329))
                 }
             }
         }
         return vn(t, xt()), t.callbackNode === n ? Fv.bind(null, t) : null
     }
 
     function Sh(t, e) {
-        var n = Na;
-        return t.current.memoizedState.isDehydrated && (yo(t, e).flags |= 256), t = oc(t, e), t !== 2 && (e = pn, pn = n, e !== null && Ch(e)), t
+        var n = za;
+        return t.current.memoizedState.isDehydrated && (yo(t, e).flags |= 256), t = sc(t, e), t !== 2 && (e = pn, pn = n, e !== null && kh(e)), t
     }
 
-    function Ch(t) {
+    function kh(t) {
         pn === null ? pn = t : pn.push.apply(pn, t)
     }
 
-    function eS(t) {
+    function ek(t) {
         for (var e = t;;) {
             if (e.flags & 16384) {
                 var n = e.updateQueue;
                 if (n !== null && (n = n.stores, n !== null))
                     for (var i = 0; i < n.length; i++) {
                         var r = n[i],
                             o = r.getSnapshot;
@@ -5947,98 +5947,98 @@
                 e.sibling.return = e.return, e = e.sibling
             }
         }
         return !0
     }
 
     function wr(t, e) {
-        for (e &= ~sp, e &= ~mc, t.suspendedLanes |= e, t.pingedLanes &= ~e, t = t.expirationTimes; 0 < e;) {
+        for (e &= ~op, e &= ~yc, t.suspendedLanes |= e, t.pingedLanes &= ~e, t = t.expirationTimes; 0 < e;) {
             var n = 31 - si(e),
                 i = 1 << n;
             t[n] = -1, e &= ~i
         }
     }
 
     function Y0(t) {
-        if (Ne & 6) throw Error(ne(327));
+        if (Ne & 6) throw Error(te(327));
         bs();
-        var e = Bu(t, 0);
+        var e = Wu(t, 0);
         if (!(e & 1)) return vn(t, xt()), null;
-        var n = oc(t, e);
+        var n = sc(t, e);
         if (t.tag !== 0 && n === 2) {
-            var i = Gd(t);
+            var i = Zd(t);
             i !== 0 && (e = i, n = Sh(t, i))
         }
-        if (n === 1) throw n = el, yo(t, 0), wr(t, e), vn(t, xt()), n;
-        if (n === 6) throw Error(ne(345));
+        if (n === 1) throw n = tl, yo(t, 0), wr(t, e), vn(t, xt()), n;
+        if (n === 6) throw Error(te(345));
         return t.finishedWork = t.current.alternate, t.finishedLanes = e, ho(t, pn, Vi), vn(t, xt()), null
     }
 
-    function lp(t, e) {
+    function ap(t, e) {
         var n = Ne;
         Ne |= 1;
         try {
             return t(e)
         } finally {
-            Ne = n, Ne === 0 && (Ts = xt() + 500, dc && zr())
+            Ne = n, Ne === 0 && (Ts = xt() + 500, hc && zr())
         }
     }
 
-    function ko(t) {
-        Sr !== null && Sr.tag === 0 && !(Ne & 6) && bs();
+    function So(t) {
+        kr !== null && kr.tag === 0 && !(Ne & 6) && bs();
         var e = Ne;
         Ne |= 1;
         var n = Xn.transition,
             i = Be;
         try {
             if (Xn.transition = null, Be = 1, t) return t()
         } finally {
             Be = i, Xn.transition = n, Ne = e, !(Ne & 6) && zr()
         }
     }
 
-    function up() {
+    function lp() {
         On = ps.current, it(ps)
     }
 
     function yo(t, e) {
         t.finishedWork = null, t.finishedLanes = 0;
         var n = t.timeoutHandle;
-        if (n !== -1 && (t.timeoutHandle = -1, Dk(n)), kt !== null)
-            for (n = kt.return; n !== null;) {
+        if (n !== -1 && (t.timeoutHandle = -1, MS(n)), St !== null)
+            for (n = St.return; n !== null;) {
                 var i = n;
-                switch (Vh(i), i.tag) {
+                switch (Wh(i), i.tag) {
                     case 1:
-                        i = i.type.childContextTypes, i != null && Yu();
+                        i = i.type.childContextTypes, i != null && Xu();
                         break;
                     case 3:
-                        Cs(), it(mn), it(Kt), Kh();
+                        Cs(), it(mn), it(Qt), Gh();
                         break;
                     case 5:
-                        Qh(i);
+                        Kh(i);
                         break;
                     case 4:
                         Cs();
                         break;
                     case 13:
                         it(ft);
                         break;
                     case 19:
                         it(ft);
                         break;
                     case 10:
-                        Xh(i.type._context);
+                        Yh(i.type._context);
                         break;
                     case 22:
                     case 23:
-                        up()
+                        lp()
                 }
                 n = n.return
             }
-        if (It = t, kt = t = Ar(t.current, null), Bt = On = e, Dt = 0, el = null, sp = mc = wo = 0, pn = Na = null, go !== null) {
+        if (It = t, St = t = Ar(t.current, null), Bt = On = e, Mt = 0, tl = null, op = yc = wo = 0, pn = za = null, go !== null) {
             for (e = 0; e < go.length; e++)
                 if (n = go[e], i = n.interleaved, i !== null) {
                     n.interleaved = null;
                     var r = i.next,
                         o = n.pending;
                     if (o !== null) {
                         var s = o.next;
@@ -6048,25 +6048,25 @@
                 } go = null
         }
         return t
     }
 
     function jv(t, e) {
         do {
-            var n = kt;
+            var n = St;
             try {
-                if (Yh(), Ou.current = tc, ec) {
+                if ($h(), Au.current = nc, tc) {
                     for (var i = dt.memoizedState; i !== null;) {
                         var r = i.queue;
                         r !== null && (r.pending = null), i = i.next
                     }
-                    ec = !1
+                    tc = !1
                 }
-                if (_o = 0, Rt = Mt = dt = null, Ra = !1, Qa = 0, op.current = null, n === null || n.return === null) {
-                    Dt = 1, el = e, kt = null;
+                if (_o = 0, Rt = Pt = dt = null, Ia = !1, Qa = 0, rp.current = null, n === null || n.return === null) {
+                    Mt = 1, tl = e, St = null;
                     break
                 }
                 e: {
                     var o = t,
                         s = n.return,
                         a = n,
                         l = e;
@@ -6077,179 +6077,179 @@
                         if (!(d.mode & 1) && (g === 0 || g === 11 || g === 15)) {
                             var y = d.alternate;
                             y ? (d.updateQueue = y.updateQueue, d.memoizedState = y.memoizedState, d.lanes = y.lanes) : (d.updateQueue = null, d.memoizedState = null)
                         }
                         var x = L0(s);
                         if (x !== null) {
                             x.flags &= -257, R0(x, s, a, o, e), x.mode & 1 && A0(o, c, e), e = x, l = c;
-                            var w = e.updateQueue;
-                            if (w === null) {
-                                var S = new Set;
-                                S.add(l), e.updateQueue = S
-                            } else w.add(l);
+                            var _ = e.updateQueue;
+                            if (_ === null) {
+                                var C = new Set;
+                                C.add(l), e.updateQueue = C
+                            } else _.add(l);
                             break e
                         } else {
                             if (!(e & 1)) {
-                                A0(o, c, e), cp();
+                                A0(o, c, e), up();
                                 break e
                             }
-                            l = Error(ne(426))
+                            l = Error(te(426))
                         }
                     } else if (at && a.mode & 1) {
                         var A = L0(s);
                         if (A !== null) {
-                            !(A.flags & 65536) && (A.flags |= 256), R0(A, s, a, o, e), Uh(Es(l, a));
+                            !(A.flags & 65536) && (A.flags |= 256), R0(A, s, a, o, e), Vh(Es(l, a));
                             break e
                         }
                     }
                     o = l = Es(l, a),
-                    Dt !== 4 && (Dt = 2),
-                    Na === null ? Na = [o] : Na.push(o),
+                    Mt !== 4 && (Mt = 2),
+                    za === null ? za = [o] : za.push(o),
                     o = s;do {
                         switch (o.tag) {
                             case 3:
                                 o.flags |= 65536, e &= -e, o.lanes |= e;
-                                var _ = wv(o, l, e);
-                                C0(o, _);
+                                var w = wv(o, l, e);
+                                C0(o, w);
                                 break e;
                             case 1:
                                 a = l;
-                                var C = o.type,
-                                    M = o.stateNode;
-                                if (!(o.flags & 128) && (typeof C.getDerivedStateFromError == "function" || M !== null && typeof M.componentDidCatch == "function" && (Dr === null || !Dr.has(M)))) {
+                                var k = o.type,
+                                    P = o.stateNode;
+                                if (!(o.flags & 128) && (typeof k.getDerivedStateFromError == "function" || P !== null && typeof P.componentDidCatch == "function" && (Mr === null || !Mr.has(P)))) {
                                     o.flags |= 65536, e &= -e, o.lanes |= e;
-                                    var z = kv(o, a, e);
+                                    var z = Sv(o, a, e);
                                     C0(o, z);
                                     break e
                                 }
                         }
                         o = o.return
                     } while (o !== null)
                 }
                 Wv(n)
             } catch (F) {
-                e = F, kt === n && n !== null && (kt = n = n.return);
+                e = F, St === n && n !== null && (St = n = n.return);
                 continue
             }
             break
         } while (!0)
     }
 
     function Hv() {
-        var t = nc.current;
-        return nc.current = tc, t === null ? tc : t
+        var t = ic.current;
+        return ic.current = nc, t === null ? nc : t
     }
 
-    function cp() {
-        (Dt === 0 || Dt === 3 || Dt === 2) && (Dt = 4), It === null || !(wo & 268435455) && !(mc & 268435455) || wr(It, Bt)
+    function up() {
+        (Mt === 0 || Mt === 3 || Mt === 2) && (Mt = 4), It === null || !(wo & 268435455) && !(yc & 268435455) || wr(It, Bt)
     }
 
-    function oc(t, e) {
+    function sc(t, e) {
         var n = Ne;
         Ne |= 2;
         var i = Hv();
         (It !== t || Bt !== e) && (Vi = null, yo(t, e));
         do try {
-            tS();
+            tk();
             break
         } catch (r) {
             jv(t, r)
         }
         while (!0);
-        if (Yh(), Ne = n, nc.current = i, kt !== null) throw Error(ne(261));
-        return It = null, Bt = 0, Dt
+        if ($h(), Ne = n, ic.current = i, St !== null) throw Error(te(261));
+        return It = null, Bt = 0, Mt
     }
 
-    function tS() {
-        for (; kt !== null;) Bv(kt)
+    function tk() {
+        for (; St !== null;) Bv(St)
     }
 
-    function nS() {
-        for (; kt !== null && !Mw();) Bv(kt)
+    function nk() {
+        for (; St !== null && !Pw();) Bv(St)
     }
 
     function Bv(t) {
         var e = Uv(t.alternate, t, On);
-        t.memoizedProps = t.pendingProps, e === null ? Wv(t) : kt = e, op.current = null
+        t.memoizedProps = t.pendingProps, e === null ? Wv(t) : St = e, rp.current = null
     }
 
     function Wv(t) {
         var e = t;
         do {
             var n = e.alternate;
             if (t = e.return, e.flags & 32768) {
-                if (n = Zk(n, e), n !== null) {
-                    n.flags &= 32767, kt = n;
+                if (n = ZS(n, e), n !== null) {
+                    n.flags &= 32767, St = n;
                     return
                 }
                 if (t !== null) t.flags |= 32768, t.subtreeFlags = 0, t.deletions = null;
                 else {
-                    Dt = 6, kt = null;
+                    Mt = 6, St = null;
                     return
                 }
-            } else if (n = qk(n, e, On), n !== null) {
-                kt = n;
+            } else if (n = qS(n, e, On), n !== null) {
+                St = n;
                 return
             }
             if (e = e.sibling, e !== null) {
-                kt = e;
+                St = e;
                 return
             }
-            kt = e = t
+            St = e = t
         } while (e !== null);
-        Dt === 0 && (Dt = 5)
+        Mt === 0 && (Mt = 5)
     }
 
     function ho(t, e, n) {
         var i = Be,
             r = Xn.transition;
         try {
-            Xn.transition = null, Be = 1, iS(t, e, n, i)
+            Xn.transition = null, Be = 1, ik(t, e, n, i)
         } finally {
             Xn.transition = r, Be = i
         }
         return null
     }
 
-    function iS(t, e, n, i) {
-        do bs(); while (Sr !== null);
-        if (Ne & 6) throw Error(ne(327));
+    function ik(t, e, n, i) {
+        do bs(); while (kr !== null);
+        if (Ne & 6) throw Error(te(327));
         n = t.finishedWork;
         var r = t.finishedLanes;
         if (n === null) return null;
-        if (t.finishedWork = null, t.finishedLanes = 0, n === t.current) throw Error(ne(177));
+        if (t.finishedWork = null, t.finishedLanes = 0, n === t.current) throw Error(te(177));
         t.callbackNode = null, t.callbackPriority = 0;
         var o = n.lanes | n.childLanes;
-        if (jw(t, o), t === It && (kt = It = null, Bt = 0), !(n.subtreeFlags & 2064) && !(n.flags & 2064) || Eu || (Eu = !0, $v(Hu, function() {
+        if (jw(t, o), t === It && (St = It = null, Bt = 0), !(n.subtreeFlags & 2064) && !(n.flags & 2064) || Tu || (Tu = !0, $v(Bu, function() {
                 return bs(), null
             })), o = (n.flags & 15990) !== 0, n.subtreeFlags & 15990 || o) {
             o = Xn.transition, Xn.transition = null;
             var s = Be;
             Be = 1;
             var a = Ne;
-            Ne |= 4, op.current = null, Qk(t, n), Nv(n, t), Ck(nh), Wu = !!th, nh = th = null, t.current = n, Kk(n, t, r), Dw(), Ne = a, Be = s, Xn.transition = o
+            Ne |= 4, rp.current = null, GS(t, n), Nv(n, t), CS(th), Vu = !!eh, th = eh = null, t.current = n, QS(n, t, r), Mw(), Ne = a, Be = s, Xn.transition = o
         } else t.current = n;
-        if (Eu && (Eu = !1, Sr = t, rc = r), o = t.pendingLanes, o === 0 && (Dr = null), Lw(n.stateNode, i), vn(t, xt()), e !== null)
+        if (Tu && (Tu = !1, kr = t, oc = r), o = t.pendingLanes, o === 0 && (Mr = null), Lw(n.stateNode, i), vn(t, xt()), e !== null)
             for (i = t.onRecoverableError, n = 0; n < e.length; n++) r = e[n], i(r.value, {
                 componentStack: r.stack,
                 digest: r.digest
             });
-        if (ic) throw ic = !1, t = wh, wh = null, t;
-        return rc & 1 && t.tag !== 0 && bs(), o = t.pendingLanes, o & 1 ? t === kh ? za++ : (za = 0, kh = t) : za = 0, zr(), null
+        if (rc) throw rc = !1, t = _h, _h = null, t;
+        return oc & 1 && t.tag !== 0 && bs(), o = t.pendingLanes, o & 1 ? t === wh ? Fa++ : (Fa = 0, wh = t) : Fa = 0, zr(), null
     }
 
     function bs() {
-        if (Sr !== null) {
-            var t = _y(rc),
+        if (kr !== null) {
+            var t = _y(oc),
                 e = Xn.transition,
                 n = Be;
             try {
-                if (Xn.transition = null, Be = 16 > t ? 16 : t, Sr === null) var i = !1;
+                if (Xn.transition = null, Be = 16 > t ? 16 : t, kr === null) var i = !1;
                 else {
-                    if (t = Sr, Sr = null, rc = 0, Ne & 6) throw Error(ne(331));
+                    if (t = kr, kr = null, oc = 0, Ne & 6) throw Error(te(331));
                     var r = Ne;
                     for (Ne |= 4, ue = t.current; ue !== null;) {
                         var o = ue,
                             s = o.child;
                         if (ue.flags & 16) {
                             var a = o.deletions;
                             if (a !== null) {
@@ -6257,15 +6257,15 @@
                                     var c = a[l];
                                     for (ue = c; ue !== null;) {
                                         var d = ue;
                                         switch (d.tag) {
                                             case 0:
                                             case 11:
                                             case 15:
-                                                Ia(8, d, o)
+                                                Na(8, d, o)
                                         }
                                         var g = d.child;
                                         if (g !== null) g.return = d, ue = g;
                                         else
                                             for (; ue !== null;) {
                                                 d = ue;
                                                 var y = d.sibling,
@@ -6278,56 +6278,56 @@
                                                     y.return = x, ue = y;
                                                     break
                                                 }
                                                 ue = x
                                             }
                                     }
                                 }
-                                var w = o.alternate;
-                                if (w !== null) {
-                                    var S = w.child;
-                                    if (S !== null) {
-                                        w.child = null;
+                                var _ = o.alternate;
+                                if (_ !== null) {
+                                    var C = _.child;
+                                    if (C !== null) {
+                                        _.child = null;
                                         do {
-                                            var A = S.sibling;
-                                            S.sibling = null, S = A
-                                        } while (S !== null)
+                                            var A = C.sibling;
+                                            C.sibling = null, C = A
+                                        } while (C !== null)
                                     }
                                 }
                                 ue = o
                             }
                         }
                         if (o.subtreeFlags & 2064 && s !== null) s.return = o, ue = s;
                         else e: for (; ue !== null;) {
                             if (o = ue, o.flags & 2048) switch (o.tag) {
                                 case 0:
                                 case 11:
                                 case 15:
-                                    Ia(9, o, o.return)
+                                    Na(9, o, o.return)
                             }
-                            var _ = o.sibling;
-                            if (_ !== null) {
-                                _.return = o.return, ue = _;
+                            var w = o.sibling;
+                            if (w !== null) {
+                                w.return = o.return, ue = w;
                                 break e
                             }
                             ue = o.return
                         }
                     }
-                    var C = t.current;
-                    for (ue = C; ue !== null;) {
+                    var k = t.current;
+                    for (ue = k; ue !== null;) {
                         s = ue;
-                        var M = s.child;
-                        if (s.subtreeFlags & 2064 && M !== null) M.return = s, ue = M;
-                        else e: for (s = C; ue !== null;) {
+                        var P = s.child;
+                        if (s.subtreeFlags & 2064 && P !== null) P.return = s, ue = P;
+                        else e: for (s = k; ue !== null;) {
                             if (a = ue, a.flags & 2048) try {
                                 switch (a.tag) {
                                     case 0:
                                     case 11:
                                     case 15:
-                                        gc(9, a)
+                                        mc(9, a)
                                 }
                             } catch (F) {
                                 vt(a, a.return, F)
                             }
                             if (a === s) {
                                 ue = null;
                                 break e
@@ -6337,177 +6337,177 @@
                                 z.return = a.return, ue = z;
                                 break e
                             }
                             ue = a.return
                         }
                     }
                     if (Ne = r, zr(), wi && typeof wi.onPostCommitFiberRoot == "function") try {
-                        wi.onPostCommitFiberRoot(ac, t)
+                        wi.onPostCommitFiberRoot(lc, t)
                     } catch {}
                     i = !0
                 }
                 return i
             } finally {
                 Be = n, Xn.transition = e
             }
         }
         return !1
     }
 
     function X0(t, e, n) {
-        e = Es(n, e), e = wv(t, e, 1), t = Mr(t, e, 1), e = nn(), t !== null && (tl(t, 1, e), vn(t, e))
+        e = Es(n, e), e = wv(t, e, 1), t = Pr(t, e, 1), e = nn(), t !== null && (nl(t, 1, e), vn(t, e))
     }
 
     function vt(t, e, n) {
         if (t.tag === 3) X0(t, t, n);
         else
             for (; e !== null;) {
                 if (e.tag === 3) {
                     X0(e, t, n);
                     break
                 } else if (e.tag === 1) {
                     var i = e.stateNode;
-                    if (typeof e.type.getDerivedStateFromError == "function" || typeof i.componentDidCatch == "function" && (Dr === null || !Dr.has(i))) {
-                        t = Es(n, t), t = kv(e, t, 1), e = Mr(e, t, 1), t = nn(), e !== null && (tl(e, 1, t), vn(e, t));
+                    if (typeof e.type.getDerivedStateFromError == "function" || typeof i.componentDidCatch == "function" && (Mr === null || !Mr.has(i))) {
+                        t = Es(n, t), t = Sv(e, t, 1), e = Pr(e, t, 1), t = nn(), e !== null && (nl(e, 1, t), vn(e, t));
                         break
                     }
                 }
                 e = e.return
             }
     }
 
-    function rS(t, e, n) {
+    function rk(t, e, n) {
         var i = t.pingCache;
-        i !== null && i.delete(e), e = nn(), t.pingedLanes |= t.suspendedLanes & n, It === t && (Bt & n) === n && (Dt === 4 || Dt === 3 && (Bt & 130023424) === Bt && 500 > xt() - ap ? yo(t, 0) : sp |= n), vn(t, e)
+        i !== null && i.delete(e), e = nn(), t.pingedLanes |= t.suspendedLanes & n, It === t && (Bt & n) === n && (Mt === 4 || Mt === 3 && (Bt & 130023424) === Bt && 500 > xt() - sp ? yo(t, 0) : op |= n), vn(t, e)
     }
 
     function Vv(t, e) {
-        e === 0 && (t.mode & 1 ? (e = du, du <<= 1, !(du & 130023424) && (du = 4194304)) : e = 1);
+        e === 0 && (t.mode & 1 ? (e = hu, hu <<= 1, !(hu & 130023424) && (hu = 4194304)) : e = 1);
         var n = nn();
-        t = Gi(t, e), t !== null && (tl(t, e, n), vn(t, n))
+        t = Ki(t, e), t !== null && (nl(t, e, n), vn(t, n))
     }
 
-    function oS(t) {
+    function ok(t) {
         var e = t.memoizedState,
             n = 0;
         e !== null && (n = e.retryLane), Vv(t, n)
     }
 
-    function sS(t, e) {
+    function sk(t, e) {
         var n = 0;
         switch (t.tag) {
             case 13:
                 var i = t.stateNode,
                     r = t.memoizedState;
                 r !== null && (n = r.retryLane);
                 break;
             case 19:
                 i = t.stateNode;
                 break;
             default:
-                throw Error(ne(314))
+                throw Error(te(314))
         }
         i !== null && i.delete(e), Vv(t, n)
     }
     var Uv;
     Uv = function(t, e, n) {
         if (t !== null)
             if (t.memoizedProps !== e.pendingProps || mn.current) gn = !0;
             else {
-                if (!(t.lanes & n) && !(e.flags & 128)) return gn = !1, Xk(t, e, n);
+                if (!(t.lanes & n) && !(e.flags & 128)) return gn = !1, XS(t, e, n);
                 gn = !!(t.flags & 131072)
             }
-        else gn = !1, at && e.flags & 1048576 && Xy(e, Zu, e.index);
+        else gn = !1, at && e.flags & 1048576 && Xy(e, Ku, e.index);
         switch (e.lanes = 0, e.tag) {
             case 2:
                 var i = e.type;
-                Lu(t, e), t = e.pendingProps;
-                var r = ws(e, Kt.current);
-                xs(e, n), r = ep(null, e, i, t, r, n);
-                var o = tp();
-                return e.flags |= 1, typeof r == "object" && r !== null && typeof r.render == "function" && r.$$typeof === void 0 ? (e.tag = 1, e.memoizedState = null, e.updateQueue = null, yn(i) ? (o = !0, Xu(e)) : o = !1, e.memoizedState = r.state !== null && r.state !== void 0 ? r.state : null, Zh(e), r.updater = hc, e.stateNode = r, r._reactInternals = e, fh(e, i, t, n), e = ph(null, e, i, !0, o, n)) : (e.tag = 0, at && o && Wh(e), tn(null, e, r, n), e = e.child), e;
+                Ru(t, e), t = e.pendingProps;
+                var r = ws(e, Qt.current);
+                xs(e, n), r = Jh(null, e, i, t, r, n);
+                var o = ep();
+                return e.flags |= 1, typeof r == "object" && r !== null && typeof r.render == "function" && r.$$typeof === void 0 ? (e.tag = 1, e.memoizedState = null, e.updateQueue = null, yn(i) ? (o = !0, qu(e)) : o = !1, e.memoizedState = r.state !== null && r.state !== void 0 ? r.state : null, qh(e), r.updater = pc, e.stateNode = r, r._reactInternals = e, ch(e, i, t, n), e = hh(null, e, i, !0, o, n)) : (e.tag = 0, at && o && Bh(e), tn(null, e, r, n), e = e.child), e;
             case 16:
                 i = e.elementType;
                 e: {
-                    switch (Lu(t, e), t = e.pendingProps, r = i._init, i = r(i._payload), e.type = i, r = e.tag = lS(i), t = ii(i, t), r) {
+                    switch (Ru(t, e), t = e.pendingProps, r = i._init, i = r(i._payload), e.type = i, r = e.tag = lk(i), t = ii(i, t), r) {
                         case 0:
-                            e = hh(null, e, i, t, n);
+                            e = dh(null, e, i, t, n);
                             break e;
                         case 1:
                             e = z0(null, e, i, t, n);
                             break e;
                         case 11:
                             e = I0(null, e, i, t, n);
                             break e;
                         case 14:
                             e = N0(null, e, i, ii(i.type, t), n);
                             break e
                     }
-                    throw Error(ne(306, i, ""))
+                    throw Error(te(306, i, ""))
                 }
                 return e;
             case 0:
-                return i = e.type, r = e.pendingProps, r = e.elementType === i ? r : ii(i, r), hh(t, e, i, r, n);
+                return i = e.type, r = e.pendingProps, r = e.elementType === i ? r : ii(i, r), dh(t, e, i, r, n);
             case 1:
                 return i = e.type, r = e.pendingProps, r = e.elementType === i ? r : ii(i, r), z0(t, e, i, r, n);
             case 3:
                 e: {
-                    if (Tv(e), t === null) throw Error(ne(387));i = e.pendingProps,
+                    if (Tv(e), t === null) throw Error(te(387));i = e.pendingProps,
                     o = e.memoizedState,
                     r = o.element,
-                    Qy(t, e),
-                    Ku(e, i, null, n);
+                    Gy(t, e),
+                    Ju(e, i, null, n);
                     var s = e.memoizedState;
                     if (i = s.element, o.isDehydrated)
                         if (o = {
                                 element: i,
                                 isDehydrated: !1,
                                 cache: s.cache,
                                 pendingSuspenseBoundaries: s.pendingSuspenseBoundaries,
                                 transitions: s.transitions
                             }, e.updateQueue.baseState = o, e.memoizedState = o, e.flags & 256) {
-                            r = Es(Error(ne(423)), e), e = F0(t, e, i, n, r);
+                            r = Es(Error(te(423)), e), e = F0(t, e, i, n, r);
                             break e
                         } else if (i !== r) {
-                        r = Es(Error(ne(424)), e), e = F0(t, e, i, n, r);
+                        r = Es(Error(te(424)), e), e = F0(t, e, i, n, r);
                         break e
                     } else
-                        for (An = Pr(e.stateNode.containerInfo.firstChild), Ln = e, at = !0, oi = null, n = tv(e, null, i, n), e.child = n; n;) n.flags = n.flags & -3 | 4096, n = n.sibling;
+                        for (An = Dr(e.stateNode.containerInfo.firstChild), Ln = e, at = !0, oi = null, n = tv(e, null, i, n), e.child = n; n;) n.flags = n.flags & -3 | 4096, n = n.sibling;
                     else {
-                        if (ks(), i === r) {
-                            e = Qi(t, e, n);
+                        if (Ss(), i === r) {
+                            e = Gi(t, e, n);
                             break e
                         }
                         tn(t, e, i, n)
                     }
                     e = e.child
                 }
                 return e;
             case 5:
-                return nv(e), t === null && lh(e), i = e.type, r = e.pendingProps, o = t !== null ? t.memoizedProps : null, s = r.children, ih(i, r) ? s = null : o !== null && ih(i, o) && (e.flags |= 32), Ev(t, e), tn(t, e, s, n), e.child;
+                return nv(e), t === null && ah(e), i = e.type, r = e.pendingProps, o = t !== null ? t.memoizedProps : null, s = r.children, nh(i, r) ? s = null : o !== null && nh(i, o) && (e.flags |= 32), Ev(t, e), tn(t, e, s, n), e.child;
             case 6:
-                return t === null && lh(e), null;
+                return t === null && ah(e), null;
             case 13:
-                return Pv(t, e, n);
+                return Dv(t, e, n);
             case 4:
-                return Gh(e, e.stateNode.containerInfo), i = e.pendingProps, t === null ? e.child = Ss(e, null, i, n) : tn(t, e, i, n), e.child;
+                return Zh(e, e.stateNode.containerInfo), i = e.pendingProps, t === null ? e.child = ks(e, null, i, n) : tn(t, e, i, n), e.child;
             case 11:
                 return i = e.type, r = e.pendingProps, r = e.elementType === i ? r : ii(i, r), I0(t, e, i, r, n);
             case 7:
                 return tn(t, e, e.pendingProps, n), e.child;
             case 8:
                 return tn(t, e, e.pendingProps.children, n), e.child;
             case 12:
                 return tn(t, e, e.pendingProps.children, n), e.child;
             case 10:
                 e: {
                     if (i = e.type._context, r = e.pendingProps, o = e.memoizedProps, s = r.value, et(Gu, i._currentValue), i._currentValue = s, o !== null)
                         if (li(o.value, s)) {
                             if (o.children === r.children && !mn.current) {
-                                e = Qi(t, e, n);
+                                e = Gi(t, e, n);
                                 break e
                             }
                         } else
                             for (o = e.child, o !== null && (o.return = e); o !== null;) {
                                 var a = o.dependencies;
                                 if (a !== null) {
                                     s = o.child;
@@ -6518,23 +6518,23 @@
                                                 var c = o.updateQueue;
                                                 if (c !== null) {
                                                     c = c.shared;
                                                     var d = c.pending;
                                                     d === null ? l.next = l : (l.next = d.next, d.next = l), c.pending = l
                                                 }
                                             }
-                                            o.lanes |= n, l = o.alternate, l !== null && (l.lanes |= n), uh(o.return, n, e), a.lanes |= n;
+                                            o.lanes |= n, l = o.alternate, l !== null && (l.lanes |= n), lh(o.return, n, e), a.lanes |= n;
                                             break
                                         }
                                         l = l.next
                                     }
                                 } else if (o.tag === 10) s = o.type === e.type ? null : o.child;
                                 else if (o.tag === 18) {
-                                    if (s = o.return, s === null) throw Error(ne(341));
-                                    s.lanes |= n, a = s.alternate, a !== null && (a.lanes |= n), uh(s, n, e), s = o.sibling
+                                    if (s = o.return, s === null) throw Error(te(341));
+                                    s.lanes |= n, a = s.alternate, a !== null && (a.lanes |= n), lh(s, n, e), s = o.sibling
                                 } else s = o.child;
                                 if (s !== null) s.return = o;
                                 else
                                     for (s = o; s !== null;) {
                                         if (s === e) {
                                             s = null;
                                             break
@@ -6552,187 +6552,187 @@
                 }
                 return e;
             case 9:
                 return r = e.type, i = e.pendingProps.children, xs(e, n), r = qn(r), i = i(r), e.flags |= 1, tn(t, e, i, n), e.child;
             case 14:
                 return i = e.type, r = ii(i, e.pendingProps), r = ii(i.type, r), N0(t, e, i, r, n);
             case 15:
-                return Sv(t, e, e.type, e.pendingProps, n);
+                return kv(t, e, e.type, e.pendingProps, n);
             case 17:
-                return i = e.type, r = e.pendingProps, r = e.elementType === i ? r : ii(i, r), Lu(t, e), e.tag = 1, yn(i) ? (t = !0, Xu(e)) : t = !1, xs(e, n), Jy(e, i, r), fh(e, i, r, n), ph(null, e, i, !0, t, n);
+                return i = e.type, r = e.pendingProps, r = e.elementType === i ? r : ii(i, r), Ru(t, e), e.tag = 1, yn(i) ? (t = !0, qu(e)) : t = !1, xs(e, n), Jy(e, i, r), ch(e, i, r, n), hh(null, e, i, !0, t, n);
             case 19:
-                return Mv(t, e, n);
+                return Pv(t, e, n);
             case 22:
                 return Cv(t, e, n)
         }
-        throw Error(ne(156, e.tag))
+        throw Error(te(156, e.tag))
     };
 
     function $v(t, e) {
         return yy(t, e)
     }
 
-    function aS(t, e, n, i) {
+    function ak(t, e, n, i) {
         this.tag = t, this.key = n, this.sibling = this.child = this.return = this.stateNode = this.type = this.elementType = null, this.index = 0, this.ref = null, this.pendingProps = e, this.dependencies = this.memoizedState = this.updateQueue = this.memoizedProps = null, this.mode = i, this.subtreeFlags = this.flags = 0, this.deletions = null, this.childLanes = this.lanes = 0, this.alternate = null
     }
 
     function Yn(t, e, n, i) {
-        return new aS(t, e, n, i)
+        return new ak(t, e, n, i)
     }
 
-    function fp(t) {
+    function cp(t) {
         return t = t.prototype, !(!t || !t.isReactComponent)
     }
 
-    function lS(t) {
-        if (typeof t == "function") return fp(t) ? 1 : 0;
+    function lk(t) {
+        if (typeof t == "function") return cp(t) ? 1 : 0;
         if (t != null) {
-            if (t = t.$$typeof, t === Dh) return 11;
-            if (t === Oh) return 14
+            if (t = t.$$typeof, t === Ph) return 11;
+            if (t === Mh) return 14
         }
         return 2
     }
 
     function Ar(t, e) {
         var n = t.alternate;
         return n === null ? (n = Yn(t.tag, e, t.key, t.mode), n.elementType = t.elementType, n.type = t.type, n.stateNode = t.stateNode, n.alternate = t, t.alternate = n) : (n.pendingProps = e, n.type = t.type, n.flags = 0, n.subtreeFlags = 0, n.deletions = null), n.flags = t.flags & 14680064, n.childLanes = t.childLanes, n.lanes = t.lanes, n.child = t.child, n.memoizedProps = t.memoizedProps, n.memoizedState = t.memoizedState, n.updateQueue = t.updateQueue, e = t.dependencies, n.dependencies = e === null ? null : {
             lanes: e.lanes,
             firstContext: e.firstContext
         }, n.sibling = t.sibling, n.index = t.index, n.ref = t.ref, n
     }
 
-    function Nu(t, e, n, i, r, o) {
+    function zu(t, e, n, i, r, o) {
         var s = 2;
-        if (i = t, typeof t == "function") fp(t) && (s = 1);
+        if (i = t, typeof t == "function") cp(t) && (s = 1);
         else if (typeof t == "string") s = 5;
         else e: switch (t) {
             case rs:
                 return vo(n.children, r, o, e);
-            case Mh:
+            case Dh:
                 s = 8, r |= 8;
                 break;
+            case Rd:
+                return t = Yn(12, n, e, r | 2), t.elementType = Rd, t.lanes = o, t;
             case Id:
-                return t = Yn(12, n, e, r | 2), t.elementType = Id, t.lanes = o, t;
+                return t = Yn(13, n, e, r), t.elementType = Id, t.lanes = o, t;
             case Nd:
-                return t = Yn(13, n, e, r), t.elementType = Nd, t.lanes = o, t;
-            case zd:
-                return t = Yn(19, n, e, r), t.elementType = zd, t.lanes = o, t;
+                return t = Yn(19, n, e, r), t.elementType = Nd, t.lanes = o, t;
             case ey:
-                return yc(n, r, o, e);
+                return vc(n, r, o, e);
             default:
                 if (typeof t == "object" && t !== null) switch (t.$$typeof) {
-                    case K0:
+                    case Q0:
                         s = 10;
                         break e;
                     case J0:
                         s = 9;
                         break e;
-                    case Dh:
+                    case Ph:
                         s = 11;
                         break e;
-                    case Oh:
+                    case Mh:
                         s = 14;
                         break e;
                     case xr:
                         s = 16, i = null;
                         break e
                 }
-                throw Error(ne(130, t == null ? t : typeof t, ""))
+                throw Error(te(130, t == null ? t : typeof t, ""))
         }
         return e = Yn(s, n, e, r), e.elementType = t, e.type = i, e.lanes = o, e
     }
 
     function vo(t, e, n, i) {
         return t = Yn(7, t, i, e), t.lanes = n, t
     }
 
-    function yc(t, e, n, i) {
+    function vc(t, e, n, i) {
         return t = Yn(22, t, i, e), t.elementType = ey, t.lanes = n, t.stateNode = {
             isHidden: !1
         }, t
     }
 
-    function Ad(t, e, n) {
+    function Od(t, e, n) {
         return t = Yn(6, t, null, e), t.lanes = n, t
     }
 
-    function Ld(t, e, n) {
+    function Ad(t, e, n) {
         return e = Yn(4, t.children !== null ? t.children : [], t.key, e), e.lanes = n, e.stateNode = {
             containerInfo: t.containerInfo,
             pendingChildren: null,
             implementation: t.implementation
         }, e
     }
 
-    function uS(t, e, n, i, r) {
-        this.tag = e, this.containerInfo = t, this.finishedWork = this.pingCache = this.current = this.pendingChildren = null, this.timeoutHandle = -1, this.callbackNode = this.pendingContext = this.context = null, this.callbackPriority = 0, this.eventTimes = md(0), this.expirationTimes = md(-1), this.entangledLanes = this.finishedLanes = this.mutableReadLanes = this.expiredLanes = this.pingedLanes = this.suspendedLanes = this.pendingLanes = 0, this.entanglements = md(0), this.identifierPrefix = i, this.onRecoverableError = r, this.mutableSourceEagerHydrationData = null
+    function uk(t, e, n, i, r) {
+        this.tag = e, this.containerInfo = t, this.finishedWork = this.pingCache = this.current = this.pendingChildren = null, this.timeoutHandle = -1, this.callbackNode = this.pendingContext = this.context = null, this.callbackPriority = 0, this.eventTimes = gd(0), this.expirationTimes = gd(-1), this.entangledLanes = this.finishedLanes = this.mutableReadLanes = this.expiredLanes = this.pingedLanes = this.suspendedLanes = this.pendingLanes = 0, this.entanglements = gd(0), this.identifierPrefix = i, this.onRecoverableError = r, this.mutableSourceEagerHydrationData = null
     }
 
-    function dp(t, e, n, i, r, o, s, a, l) {
-        return t = new uS(t, e, n, a, l), e === 1 ? (e = 1, o === !0 && (e |= 8)) : e = 0, o = Yn(3, null, null, e), t.current = o, o.stateNode = t, o.memoizedState = {
+    function fp(t, e, n, i, r, o, s, a, l) {
+        return t = new uk(t, e, n, a, l), e === 1 ? (e = 1, o === !0 && (e |= 8)) : e = 0, o = Yn(3, null, null, e), t.current = o, o.stateNode = t, o.memoizedState = {
             element: i,
             isDehydrated: n,
             cache: null,
             transitions: null,
             pendingSuspenseBoundaries: null
-        }, Zh(o), t
+        }, qh(o), t
     }
 
-    function cS(t, e, n) {
+    function ck(t, e, n) {
         var i = 3 < arguments.length && arguments[3] !== void 0 ? arguments[3] : null;
         return {
             $$typeof: is,
             key: i == null ? null : "" + i,
             children: t,
             containerInfo: e,
             implementation: n
         }
     }
 
     function Yv(t) {
         if (!t) return Rr;
         t = t._reactInternals;
         e: {
-            if (Co(t) !== t || t.tag !== 1) throw Error(ne(170));
+            if (Co(t) !== t || t.tag !== 1) throw Error(te(170));
             var e = t;do {
                 switch (e.tag) {
                     case 3:
                         e = e.stateNode.context;
                         break e;
                     case 1:
                         if (yn(e.type)) {
                             e = e.stateNode.__reactInternalMemoizedMergedChildContext;
                             break e
                         }
                 }
                 e = e.return
             } while (e !== null);
-            throw Error(ne(171))
+            throw Error(te(171))
         }
         if (t.tag === 1) {
             var n = t.type;
             if (yn(n)) return $y(t, n, e)
         }
         return e
     }
 
     function Xv(t, e, n, i, r, o, s, a, l) {
-        return t = dp(n, i, !0, t, r, o, s, a, l), t.context = Yv(null), n = t.current, i = nn(), r = Or(n), o = Xi(i, r), o.callback = e ?? null, Mr(n, o, r), t.current.lanes = r, tl(t, r, i), vn(t, i), t
+        return t = fp(n, i, !0, t, r, o, s, a, l), t.context = Yv(null), n = t.current, i = nn(), r = Or(n), o = Xi(i, r), o.callback = e ?? null, Pr(n, o, r), t.current.lanes = r, nl(t, r, i), vn(t, i), t
     }
 
-    function vc(t, e, n, i) {
+    function xc(t, e, n, i) {
         var r = e.current,
             o = nn(),
             s = Or(r);
         return n = Yv(n), e.context === null ? e.context = n : e.pendingContext = n, e = Xi(o, s), e.payload = {
             element: t
-        }, i = i === void 0 ? null : i, i !== null && (e.callback = i), t = Mr(r, e, s), t !== null && (ai(t, r, s, o), Du(t, r, s)), s
+        }, i = i === void 0 ? null : i, i !== null && (e.callback = i), t = Pr(r, e, s), t !== null && (ai(t, r, s, o), Ou(t, r, s)), s
     }
 
-    function sc(t) {
+    function ac(t) {
         if (t = t.current, !t.child) return null;
         switch (t.child.tag) {
             case 5:
                 return t.child.stateNode;
             default:
                 return t.child.stateNode
         }
@@ -6741,1119 +6741,1119 @@
     function q0(t, e) {
         if (t = t.memoizedState, t !== null && t.dehydrated !== null) {
             var n = t.retryLane;
             t.retryLane = n !== 0 && n < e ? n : e
         }
     }
 
-    function hp(t, e) {
+    function dp(t, e) {
         q0(t, e), (t = t.alternate) && q0(t, e)
     }
 
-    function fS() {
+    function fk() {
         return null
     }
     var qv = typeof reportError == "function" ? reportError : function(t) {
         console.error(t)
     };
 
-    function pp(t) {
+    function hp(t) {
         this._internalRoot = t
     }
-    xc.prototype.render = pp.prototype.render = function(t) {
+    bc.prototype.render = hp.prototype.render = function(t) {
         var e = this._internalRoot;
-        if (e === null) throw Error(ne(409));
-        vc(t, e, null, null)
+        if (e === null) throw Error(te(409));
+        xc(t, e, null, null)
     };
-    xc.prototype.unmount = pp.prototype.unmount = function() {
+    bc.prototype.unmount = hp.prototype.unmount = function() {
         var t = this._internalRoot;
         if (t !== null) {
             this._internalRoot = null;
             var e = t.containerInfo;
-            ko(function() {
-                vc(null, t, null, null)
+            So(function() {
+                xc(null, t, null, null)
             }), e[Zi] = null
         }
     };
 
-    function xc(t) {
+    function bc(t) {
         this._internalRoot = t
     }
-    xc.prototype.unstable_scheduleHydration = function(t) {
+    bc.prototype.unstable_scheduleHydration = function(t) {
         if (t) {
-            var e = Sy();
+            var e = ky();
             t = {
                 blockedOn: null,
                 target: t,
                 priority: e
             };
             for (var n = 0; n < _r.length && e !== 0 && e < _r[n].priority; n++);
             _r.splice(n, 0, t), n === 0 && Ey(t)
         }
     };
 
-    function gp(t) {
+    function pp(t) {
         return !(!t || t.nodeType !== 1 && t.nodeType !== 9 && t.nodeType !== 11)
     }
 
-    function bc(t) {
+    function _c(t) {
         return !(!t || t.nodeType !== 1 && t.nodeType !== 9 && t.nodeType !== 11 && (t.nodeType !== 8 || t.nodeValue !== " react-mount-point-unstable "))
     }
 
     function Z0() {}
 
-    function dS(t, e, n, i, r) {
+    function dk(t, e, n, i, r) {
         if (r) {
             if (typeof i == "function") {
                 var o = i;
                 i = function() {
-                    var c = sc(s);
+                    var c = ac(s);
                     o.call(c)
                 }
             }
             var s = Xv(e, i, t, 0, null, !1, !1, "", Z0);
-            return t._reactRootContainer = s, t[Zi] = s.current, Ya(t.nodeType === 8 ? t.parentNode : t), ko(), s
+            return t._reactRootContainer = s, t[Zi] = s.current, Xa(t.nodeType === 8 ? t.parentNode : t), So(), s
         }
         for (; r = t.lastChild;) t.removeChild(r);
         if (typeof i == "function") {
             var a = i;
             i = function() {
-                var c = sc(l);
+                var c = ac(l);
                 a.call(c)
             }
         }
-        var l = dp(t, 0, !1, null, null, !1, !1, "", Z0);
-        return t._reactRootContainer = l, t[Zi] = l.current, Ya(t.nodeType === 8 ? t.parentNode : t), ko(function() {
-            vc(e, l, n, i)
+        var l = fp(t, 0, !1, null, null, !1, !1, "", Z0);
+        return t._reactRootContainer = l, t[Zi] = l.current, Xa(t.nodeType === 8 ? t.parentNode : t), So(function() {
+            xc(e, l, n, i)
         }), l
     }
 
-    function _c(t, e, n, i, r) {
+    function wc(t, e, n, i, r) {
         var o = n._reactRootContainer;
         if (o) {
             var s = o;
             if (typeof r == "function") {
                 var a = r;
                 r = function() {
-                    var l = sc(s);
+                    var l = ac(s);
                     a.call(l)
                 }
             }
-            vc(e, s, t, r)
-        } else s = dS(n, e, t, r, i);
-        return sc(s)
+            xc(e, s, t, r)
+        } else s = dk(n, e, t, r, i);
+        return ac(s)
     }
     wy = function(t) {
         switch (t.tag) {
             case 3:
                 var e = t.stateNode;
                 if (e.current.memoizedState.isDehydrated) {
-                    var n = Ta(e.pendingLanes);
-                    n !== 0 && (Rh(e, n | 1), vn(e, xt()), !(Ne & 6) && (Ts = xt() + 500, zr()))
+                    var n = Da(e.pendingLanes);
+                    n !== 0 && (Lh(e, n | 1), vn(e, xt()), !(Ne & 6) && (Ts = xt() + 500, zr()))
                 }
                 break;
             case 13:
-                ko(function() {
-                    var i = Gi(t, 1);
+                So(function() {
+                    var i = Ki(t, 1);
                     if (i !== null) {
                         var r = nn();
                         ai(i, t, 1, r)
                     }
-                }), hp(t, 1)
+                }), dp(t, 1)
         }
     };
-    Ih = function(t) {
+    Rh = function(t) {
         if (t.tag === 13) {
-            var e = Gi(t, 134217728);
+            var e = Ki(t, 134217728);
             if (e !== null) {
                 var n = nn();
                 ai(e, t, 134217728, n)
             }
-            hp(t, 134217728)
+            dp(t, 134217728)
         }
     };
-    ky = function(t) {
+    Sy = function(t) {
         if (t.tag === 13) {
             var e = Or(t),
-                n = Gi(t, e);
+                n = Ki(t, e);
             if (n !== null) {
                 var i = nn();
                 ai(n, t, e, i)
             }
-            hp(t, e)
+            dp(t, e)
         }
     };
-    Sy = function() {
+    ky = function() {
         return Be
     };
     Cy = function(t, e) {
         var n = Be;
         try {
             return Be = t, e()
         } finally {
             Be = n
         }
     };
-    Xd = function(t, e, n) {
+    Yd = function(t, e, n) {
         switch (e) {
             case "input":
-                if (Hd(t, n), e = n.name, n.type === "radio" && e != null) {
+                if (jd(t, n), e = n.name, n.type === "radio" && e != null) {
                     for (n = t; n.parentNode;) n = n.parentNode;
                     for (n = n.querySelectorAll("input[name=" + JSON.stringify("" + e) + '][type="radio"]'), e = 0; e < n.length; e++) {
                         var i = n[e];
                         if (i !== t && i.form === t.form) {
-                            var r = fc(i);
-                            if (!r) throw Error(ne(90));
-                            ny(i), Hd(i, r)
+                            var r = dc(i);
+                            if (!r) throw Error(te(90));
+                            ny(i), jd(i, r)
                         }
                     }
                 }
                 break;
             case "textarea":
                 ry(t, n);
                 break;
             case "select":
                 e = n.value, e != null && gs(t, !!n.multiple, e, !1)
         }
     };
-    fy = lp;
-    dy = ko;
-    var hS = {
+    fy = ap;
+    dy = So;
+    var hk = {
             usingClientEntryPoint: !1,
-            Events: [il, ls, fc, uy, cy, lp]
+            Events: [rl, ls, dc, uy, cy, ap]
         },
         ka = {
             findFiberByHostInstance: po,
             bundleType: 0,
             version: "18.2.0",
             rendererPackageName: "react-dom"
         },
-        pS = {
+        pk = {
             bundleType: ka.bundleType,
             version: ka.version,
             rendererPackageName: ka.rendererPackageName,
             rendererConfig: ka.rendererConfig,
             overrideHookState: null,
             overrideHookStateDeletePath: null,
             overrideHookStateRenamePath: null,
             overrideProps: null,
             overridePropsDeletePath: null,
             overridePropsRenamePath: null,
             setErrorHandler: null,
             setSuspenseHandler: null,
             scheduleUpdate: null,
-            currentDispatcherRef: Ki.ReactCurrentDispatcher,
+            currentDispatcherRef: Qi.ReactCurrentDispatcher,
             findHostInstanceByFiber: function(t) {
                 return t = gy(t), t === null ? null : t.stateNode
             },
-            findFiberByHostInstance: ka.findFiberByHostInstance || fS,
+            findFiberByHostInstance: ka.findFiberByHostInstance || fk,
             findHostInstancesForRefresh: null,
             scheduleRefresh: null,
             scheduleRoot: null,
             setRefreshHandler: null,
             getCurrentFiber: null,
             reconcilerVersion: "18.2.0-next-9e3b772b8-20220608"
         };
-    if (typeof __REACT_DEVTOOLS_GLOBAL_HOOK__ < "u" && (Sa = __REACT_DEVTOOLS_GLOBAL_HOOK__, !Sa.isDisabled && Sa.supportsFiber)) try {
-        ac = Sa.inject(pS), wi = Sa
+    if (typeof __REACT_DEVTOOLS_GLOBAL_HOOK__ < "u" && (Ca = __REACT_DEVTOOLS_GLOBAL_HOOK__, !Ca.isDisabled && Ca.supportsFiber)) try {
+        lc = Ca.inject(pk), wi = Ca
     } catch {}
-    var Sa;
-    Nn.__SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED = hS;
+    var Ca;
+    Nn.__SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED = hk;
     Nn.createPortal = function(t, e) {
         var n = 2 < arguments.length && arguments[2] !== void 0 ? arguments[2] : null;
-        if (!gp(e)) throw Error(ne(200));
-        return cS(t, e, null, n)
+        if (!pp(e)) throw Error(te(200));
+        return ck(t, e, null, n)
     };
     Nn.createRoot = function(t, e) {
-        if (!gp(t)) throw Error(ne(299));
+        if (!pp(t)) throw Error(te(299));
         var n = !1,
             i = "",
             r = qv;
-        return e != null && (e.unstable_strictMode === !0 && (n = !0), e.identifierPrefix !== void 0 && (i = e.identifierPrefix), e.onRecoverableError !== void 0 && (r = e.onRecoverableError)), e = dp(t, 1, !1, null, null, n, !1, i, r), t[Zi] = e.current, Ya(t.nodeType === 8 ? t.parentNode : t), new pp(e)
+        return e != null && (e.unstable_strictMode === !0 && (n = !0), e.identifierPrefix !== void 0 && (i = e.identifierPrefix), e.onRecoverableError !== void 0 && (r = e.onRecoverableError)), e = fp(t, 1, !1, null, null, n, !1, i, r), t[Zi] = e.current, Xa(t.nodeType === 8 ? t.parentNode : t), new hp(e)
     };
     Nn.findDOMNode = function(t) {
         if (t == null) return null;
         if (t.nodeType === 1) return t;
         var e = t._reactInternals;
-        if (e === void 0) throw typeof t.render == "function" ? Error(ne(188)) : (t = Object.keys(t).join(","), Error(ne(268, t)));
+        if (e === void 0) throw typeof t.render == "function" ? Error(te(188)) : (t = Object.keys(t).join(","), Error(te(268, t)));
         return t = gy(e), t = t === null ? null : t.stateNode, t
     };
     Nn.flushSync = function(t) {
-        return ko(t)
+        return So(t)
     };
     Nn.hydrate = function(t, e, n) {
-        if (!bc(e)) throw Error(ne(200));
-        return _c(null, t, e, !0, n)
+        if (!_c(e)) throw Error(te(200));
+        return wc(null, t, e, !0, n)
     };
     Nn.hydrateRoot = function(t, e, n) {
-        if (!gp(t)) throw Error(ne(405));
+        if (!pp(t)) throw Error(te(405));
         var i = n != null && n.hydratedSources || null,
             r = !1,
             o = "",
             s = qv;
-        if (n != null && (n.unstable_strictMode === !0 && (r = !0), n.identifierPrefix !== void 0 && (o = n.identifierPrefix), n.onRecoverableError !== void 0 && (s = n.onRecoverableError)), e = Xv(e, null, t, 1, n ?? null, r, !1, o, s), t[Zi] = e.current, Ya(t), i)
+        if (n != null && (n.unstable_strictMode === !0 && (r = !0), n.identifierPrefix !== void 0 && (o = n.identifierPrefix), n.onRecoverableError !== void 0 && (s = n.onRecoverableError)), e = Xv(e, null, t, 1, n ?? null, r, !1, o, s), t[Zi] = e.current, Xa(t), i)
             for (t = 0; t < i.length; t++) n = i[t], r = n._getVersion, r = r(n._source), e.mutableSourceEagerHydrationData == null ? e.mutableSourceEagerHydrationData = [n, r] : e.mutableSourceEagerHydrationData.push(n, r);
-        return new xc(e)
+        return new bc(e)
     };
     Nn.render = function(t, e, n) {
-        if (!bc(e)) throw Error(ne(200));
-        return _c(null, t, e, !1, n)
+        if (!_c(e)) throw Error(te(200));
+        return wc(null, t, e, !1, n)
     };
     Nn.unmountComponentAtNode = function(t) {
-        if (!bc(t)) throw Error(ne(40));
-        return t._reactRootContainer ? (ko(function() {
-            _c(null, null, t, !1, function() {
+        if (!_c(t)) throw Error(te(40));
+        return t._reactRootContainer ? (So(function() {
+            wc(null, null, t, !1, function() {
                 t._reactRootContainer = null, t[Zi] = null
             })
         }), !0) : !1
     };
-    Nn.unstable_batchedUpdates = lp;
+    Nn.unstable_batchedUpdates = ap;
     Nn.unstable_renderSubtreeIntoContainer = function(t, e, n, i) {
-        if (!bc(n)) throw Error(ne(200));
-        if (t == null || t._reactInternals === void 0) throw Error(ne(38));
-        return _c(t, e, n, !1, i)
+        if (!_c(n)) throw Error(te(200));
+        if (t == null || t._reactInternals === void 0) throw Error(te(38));
+        return wc(t, e, n, !1, i)
     };
     Nn.version = "18.2.0-next-9e3b772b8-20220608"
 });
-var Kv = mr((tD, Qv) => {
+var Qv = mr((JP, Gv) => {
     "use strict";
 
-    function Gv() {
+    function Kv() {
         if (!(typeof __REACT_DEVTOOLS_GLOBAL_HOOK__ > "u" || typeof __REACT_DEVTOOLS_GLOBAL_HOOK__.checkDCE != "function")) try {
-            __REACT_DEVTOOLS_GLOBAL_HOOK__.checkDCE(Gv)
+            __REACT_DEVTOOLS_GLOBAL_HOOK__.checkDCE(Kv)
         } catch (t) {
             console.error(t)
         }
     }
-    Gv(), Qv.exports = Zv()
+    Kv(), Gv.exports = Zv()
 });
-var ex = mr(mp => {
+var ex = mr(gp => {
     "use strict";
-    var Jv = Kv();
-    mp.createRoot = Jv.createRoot, mp.hydrateRoot = Jv.hydrateRoot;
-    var nD
+    var Jv = Qv();
+    gp.createRoot = Jv.createRoot, gp.hydrateRoot = Jv.hydrateRoot;
+    var eM
 });
-var p1 = mr((vD, kf) => {
+var p1 = mr((mM, wf) => {
     (function(t, e, n, i) {
         "use strict";
         var r = ["", "webkit", "Moz", "MS", "ms", "o"],
             o = e.createElement("div"),
             s = "function",
             a = Math.round,
             l = Math.abs,
             c = Date.now;
 
-        function d(k, P, N) {
-            return setTimeout(C(k, N), P)
+        function d(S, D, N) {
+            return setTimeout(k(S, N), D)
         }
 
-        function g(k, P, N) {
-            return Array.isArray(k) ? (y(k, N[P], N), !0) : !1
+        function g(S, D, N) {
+            return Array.isArray(S) ? (y(S, N[D], N), !0) : !1
         }
 
-        function y(k, P, N) {
-            var $;
-            if (k)
-                if (k.forEach) k.forEach(P, N);
-                else if (k.length !== i)
-                for ($ = 0; $ < k.length;) P.call(N, k[$], $, k), $++;
+        function y(S, D, N) {
+            var U;
+            if (S)
+                if (S.forEach) S.forEach(D, N);
+                else if (S.length !== i)
+                for (U = 0; U < S.length;) D.call(N, S[U], U, S), U++;
             else
-                for ($ in k) k.hasOwnProperty($) && P.call(N, k[$], $, k)
+                for (U in S) S.hasOwnProperty(U) && D.call(N, S[U], U, S)
         }
 
-        function x(k, P, N) {
-            var $ = "DEPRECATED METHOD: " + P + `
+        function x(S, D, N) {
+            var U = "DEPRECATED METHOD: " + D + `
 ` + N + ` AT 
 `;
             return function() {
                 var J = new Error("get-stack-trace"),
                     se = J && J.stack ? J.stack.replace(/^[^\(]+?[\n$]/gm, "").replace(/^\s+at\s+/gm, "").replace(/^Object.<anonymous>\s*\(/gm, "{anonymous}()@") : "Unknown Stack Trace",
-                    ke = t.console && (t.console.warn || t.console.log);
-                return ke && ke.call(t.console, $, se), k.apply(this, arguments)
+                    Se = t.console && (t.console.warn || t.console.log);
+                return Se && Se.call(t.console, U, se), S.apply(this, arguments)
             }
         }
-        var w;
-        typeof Object.assign != "function" ? w = function(P) {
-            if (P === i || P === null) throw new TypeError("Cannot convert undefined or null to object");
-            for (var N = Object(P), $ = 1; $ < arguments.length; $++) {
-                var J = arguments[$];
+        var _;
+        typeof Object.assign != "function" ? _ = function(D) {
+            if (D === i || D === null) throw new TypeError("Cannot convert undefined or null to object");
+            for (var N = Object(D), U = 1; U < arguments.length; U++) {
+                var J = arguments[U];
                 if (J !== i && J !== null)
                     for (var se in J) J.hasOwnProperty(se) && (N[se] = J[se])
             }
             return N
-        } : w = Object.assign;
-        var S = x(function(P, N, $) {
-                for (var J = Object.keys(N), se = 0; se < J.length;)(!$ || $ && P[J[se]] === i) && (P[J[se]] = N[J[se]]), se++;
-                return P
+        } : _ = Object.assign;
+        var C = x(function(D, N, U) {
+                for (var J = Object.keys(N), se = 0; se < J.length;)(!U || U && D[J[se]] === i) && (D[J[se]] = N[J[se]]), se++;
+                return D
             }, "extend", "Use `assign`."),
-            A = x(function(P, N) {
-                return S(P, N, !0)
+            A = x(function(D, N) {
+                return C(D, N, !0)
             }, "merge", "Use `assign`.");
 
-        function _(k, P, N) {
-            var $ = P.prototype,
+        function w(S, D, N) {
+            var U = D.prototype,
                 J;
-            J = k.prototype = Object.create($), J.constructor = k, J._super = $, N && w(J, N)
+            J = S.prototype = Object.create(U), J.constructor = S, J._super = U, N && _(J, N)
         }
 
-        function C(k, P) {
+        function k(S, D) {
             return function() {
-                return k.apply(P, arguments)
+                return S.apply(D, arguments)
             }
         }
 
-        function M(k, P) {
-            return typeof k == s ? k.apply(P && P[0] || i, P) : k
+        function P(S, D) {
+            return typeof S == s ? S.apply(D && D[0] || i, D) : S
         }
 
-        function z(k, P) {
-            return k === i ? P : k
+        function z(S, D) {
+            return S === i ? D : S
         }
 
-        function F(k, P, N) {
-            y(te(P), function($) {
-                k.addEventListener($, N, !1)
+        function F(S, D, N) {
+            y(ne(D), function(U) {
+                S.addEventListener(U, N, !1)
             })
         }
 
-        function h(k, P, N) {
-            y(te(P), function($) {
-                k.removeEventListener($, N, !1)
+        function h(S, D, N) {
+            y(ne(D), function(U) {
+                S.removeEventListener(U, N, !1)
             })
         }
 
-        function Y(k, P) {
-            for (; k;) {
-                if (k == P) return !0;
-                k = k.parentNode
+        function $(S, D) {
+            for (; S;) {
+                if (S == D) return !0;
+                S = S.parentNode
             }
             return !1
         }
 
-        function V(k, P) {
-            return k.indexOf(P) > -1
+        function Y(S, D) {
+            return S.indexOf(D) > -1
         }
 
-        function te(k) {
-            return k.trim().split(/\s+/g)
+        function ne(S) {
+            return S.trim().split(/\s+/g)
         }
 
-        function ie(k, P, N) {
-            if (k.indexOf && !N) return k.indexOf(P);
-            for (var $ = 0; $ < k.length;) {
-                if (N && k[$][N] == P || !N && k[$] === P) return $;
-                $++
+        function ie(S, D, N) {
+            if (S.indexOf && !N) return S.indexOf(D);
+            for (var U = 0; U < S.length;) {
+                if (N && S[U][N] == D || !N && S[U] === D) return U;
+                U++
             }
             return -1
         }
 
-        function ce(k) {
-            return Array.prototype.slice.call(k, 0)
+        function ce(S) {
+            return Array.prototype.slice.call(S, 0)
         }
 
-        function he(k, P, N) {
-            for (var $ = [], J = [], se = 0; se < k.length;) {
-                var ke = P ? k[se][P] : k[se];
-                ie(J, ke) < 0 && $.push(k[se]), J[se] = ke, se++
+        function he(S, D, N) {
+            for (var U = [], J = [], se = 0; se < S.length;) {
+                var Se = D ? S[se][D] : S[se];
+                ie(J, Se) < 0 && U.push(S[se]), J[se] = Se, se++
             }
-            return N && (P ? $ = $.sort(function(Et, Lt) {
-                return Et[P] > Lt[P]
-            }) : $ = $.sort()), $
+            return N && (D ? U = U.sort(function(Et, Lt) {
+                return Et[D] > Lt[D]
+            }) : U = U.sort()), U
         }
 
-        function Fe(k, P) {
-            for (var N, $, J = P[0].toUpperCase() + P.slice(1), se = 0; se < r.length;) {
-                if (N = r[se], $ = N ? N + J : P, $ in k) return $;
+        function Fe(S, D) {
+            for (var N, U, J = D[0].toUpperCase() + D.slice(1), se = 0; se < r.length;) {
+                if (N = r[se], U = N ? N + J : D, U in S) return U;
                 se++
             }
             return i
         }
         var Ze = 1;
 
         function Ee() {
             return Ze++
         }
 
-        function Te(k) {
-            var P = k.ownerDocument || k;
-            return P.defaultView || P.parentWindow || t
+        function Te(S) {
+            var D = S.ownerDocument || S;
+            return D.defaultView || D.parentWindow || t
         }
         var Ye = /mobile|tablet|ip(ad|hone|od)|android/i,
             Ot = "ontouchstart" in t,
             lt = Fe(t, "PointerEvent") !== i,
             Oe = Ot && Ye.test(navigator.userAgent),
-            Ge = "touch",
+            Ke = "touch",
             ot = "pen",
             At = "mouse",
             $t = "kinect",
             mt = 25,
             je = 1,
             ln = 2,
             Ve = 4,
             Ae = 8,
             Yt = 1,
-            Di = 2,
+            Mi = 2,
             Oi = 4,
-            D = 8,
+            M = 8,
             H = 16,
-            O = Di | Oi,
-            X = D | H,
+            O = Mi | Oi,
+            X = M | H,
             re = O | X,
             le = ["x", "y"],
-            Pe = ["clientX", "clientY"];
+            De = ["clientX", "clientY"];
 
-        function Me(k, P) {
+        function Pe(S, D) {
             var N = this;
-            this.manager = k, this.callback = P, this.element = k.element, this.target = k.options.inputTarget, this.domHandler = function($) {
-                M(k.options.enable, [k]) && N.handler($)
+            this.manager = S, this.callback = D, this.element = S.element, this.target = S.options.inputTarget, this.domHandler = function(U) {
+                P(S.options.enable, [S]) && N.handler(U)
             }, this.init()
         }
-        Me.prototype = {
+        Pe.prototype = {
             handler: function() {},
             init: function() {
                 this.evEl && F(this.element, this.evEl, this.domHandler), this.evTarget && F(this.target, this.evTarget, this.domHandler), this.evWin && F(Te(this.element), this.evWin, this.domHandler)
             },
             destroy: function() {
                 this.evEl && h(this.element, this.evEl, this.domHandler), this.evTarget && h(this.target, this.evTarget, this.domHandler), this.evWin && h(Te(this.element), this.evWin, this.domHandler)
             }
         };
 
-        function Qe(k) {
-            var P, N = k.options.inputClass;
-            return N ? P = N : lt ? P = Js : Oe ? P = Yo : Ot ? P = na : P = Ct, new P(k, Ft)
+        function Ge(S) {
+            var D, N = S.options.inputClass;
+            return N ? D = N : lt ? D = ea : Oe ? D = Yo : Ot ? D = ia : D = Ct, new D(S, Ft)
         }
 
-        function Ft(k, P, N) {
-            var $ = N.pointers.length,
+        function Ft(S, D, N) {
+            var U = N.pointers.length,
                 J = N.changedPointers.length,
-                se = P & je && $ - J === 0,
-                ke = P & (Ve | Ae) && $ - J === 0;
-            N.isFirst = !!se, N.isFinal = !!ke, se && (k.session = {}), N.eventType = P, Sn(k, N), k.emit("hammer.input", N), k.recognize(N), k.session.prevInput = N
+                se = D & je && U - J === 0,
+                Se = D & (Ve | Ae) && U - J === 0;
+            N.isFirst = !!se, N.isFinal = !!Se, se && (S.session = {}), N.eventType = D, kn(S, N), S.emit("hammer.input", N), S.recognize(N), S.session.prevInput = N
         }
 
-        function Sn(k, P) {
-            var N = k.session,
-                $ = P.pointers,
-                J = $.length;
-            N.firstInput || (N.firstInput = Li(P)), J > 1 && !N.firstMultiple ? N.firstMultiple = Li(P) : J === 1 && (N.firstMultiple = !1);
+        function kn(S, D) {
+            var N = S.session,
+                U = D.pointers,
+                J = U.length;
+            N.firstInput || (N.firstInput = Li(D)), J > 1 && !N.firstMultiple ? N.firstMultiple = Li(D) : J === 1 && (N.firstMultiple = !1);
             var se = N.firstInput,
-                ke = N.firstMultiple,
-                yt = ke ? ke.center : se.center,
-                Et = P.center = jl($);
-            P.timeStamp = c(), P.deltaTime = P.timeStamp - se.timeStamp, P.angle = Gs(yt, Et), P.distance = eo(yt, Et), ut(N, P), P.offsetDirection = Zs(P.deltaX, P.deltaY);
-            var Lt = Jr(P.deltaTime, P.deltaX, P.deltaY);
-            P.overallVelocityX = Lt.x, P.overallVelocityY = Lt.y, P.overallVelocity = l(Lt.x) > l(Lt.y) ? Lt.x : Lt.y, P.scale = ke ? to(ke.pointers, $) : 1, P.rotation = ke ? ar(ke.pointers, $) : 0, P.maxPointers = N.prevInput ? P.pointers.length > N.prevInput.maxPointers ? P.pointers.length : N.prevInput.maxPointers : P.pointers.length, Ai(N, P);
-            var Bn = k.element;
-            Y(P.srcEvent.target, Bn) && (Bn = P.srcEvent.target), P.target = Bn
-        }
-
-        function ut(k, P) {
-            var N = P.center,
-                $ = k.offsetDelta || {},
-                J = k.prevDelta || {},
-                se = k.prevInput || {};
-            (P.eventType === je || se.eventType === Ve) && (J = k.prevDelta = {
+                Se = N.firstMultiple,
+                yt = Se ? Se.center : se.center,
+                Et = D.center = Hl(U);
+            D.timeStamp = c(), D.deltaTime = D.timeStamp - se.timeStamp, D.angle = Gs(yt, Et), D.distance = eo(yt, Et), ut(N, D), D.offsetDirection = Ks(D.deltaX, D.deltaY);
+            var Lt = Jr(D.deltaTime, D.deltaX, D.deltaY);
+            D.overallVelocityX = Lt.x, D.overallVelocityY = Lt.y, D.overallVelocity = l(Lt.x) > l(Lt.y) ? Lt.x : Lt.y, D.scale = Se ? to(Se.pointers, U) : 1, D.rotation = Se ? ar(Se.pointers, U) : 0, D.maxPointers = N.prevInput ? D.pointers.length > N.prevInput.maxPointers ? D.pointers.length : N.prevInput.maxPointers : D.pointers.length, Ai(N, D);
+            var Bn = S.element;
+            $(D.srcEvent.target, Bn) && (Bn = D.srcEvent.target), D.target = Bn
+        }
+
+        function ut(S, D) {
+            var N = D.center,
+                U = S.offsetDelta || {},
+                J = S.prevDelta || {},
+                se = S.prevInput || {};
+            (D.eventType === je || se.eventType === Ve) && (J = S.prevDelta = {
                 x: se.deltaX || 0,
                 y: se.deltaY || 0
-            }, $ = k.offsetDelta = {
+            }, U = S.offsetDelta = {
                 x: N.x,
                 y: N.y
-            }), P.deltaX = J.x + (N.x - $.x), P.deltaY = J.y + (N.y - $.y)
+            }), D.deltaX = J.x + (N.x - U.x), D.deltaY = J.y + (N.y - U.y)
         }
 
-        function Ai(k, P) {
-            var N = k.lastInterval || P,
-                $ = P.timeStamp - N.timeStamp,
-                J, se, ke, yt;
-            if (P.eventType != Ae && ($ > mt || N.velocity === i)) {
-                var Et = P.deltaX - N.deltaX,
-                    Lt = P.deltaY - N.deltaY,
-                    Bn = Jr($, Et, Lt);
-                se = Bn.x, ke = Bn.y, J = l(Bn.x) > l(Bn.y) ? Bn.x : Bn.y, yt = Zs(Et, Lt), k.lastInterval = P
-            } else J = N.velocity, se = N.velocityX, ke = N.velocityY, yt = N.direction;
-            P.velocity = J, P.velocityX = se, P.velocityY = ke, P.direction = yt
-        }
-
-        function Li(k) {
-            for (var P = [], N = 0; N < k.pointers.length;) P[N] = {
-                clientX: a(k.pointers[N].clientX),
-                clientY: a(k.pointers[N].clientY)
+        function Ai(S, D) {
+            var N = S.lastInterval || D,
+                U = D.timeStamp - N.timeStamp,
+                J, se, Se, yt;
+            if (D.eventType != Ae && (U > mt || N.velocity === i)) {
+                var Et = D.deltaX - N.deltaX,
+                    Lt = D.deltaY - N.deltaY,
+                    Bn = Jr(U, Et, Lt);
+                se = Bn.x, Se = Bn.y, J = l(Bn.x) > l(Bn.y) ? Bn.x : Bn.y, yt = Ks(Et, Lt), S.lastInterval = D
+            } else J = N.velocity, se = N.velocityX, Se = N.velocityY, yt = N.direction;
+            D.velocity = J, D.velocityX = se, D.velocityY = Se, D.direction = yt
+        }
+
+        function Li(S) {
+            for (var D = [], N = 0; N < S.pointers.length;) D[N] = {
+                clientX: a(S.pointers[N].clientX),
+                clientY: a(S.pointers[N].clientY)
             }, N++;
             return {
                 timeStamp: c(),
-                pointers: P,
-                center: jl(P),
-                deltaX: k.deltaX,
-                deltaY: k.deltaY
+                pointers: D,
+                center: Hl(D),
+                deltaX: S.deltaX,
+                deltaY: S.deltaY
             }
         }
 
-        function jl(k) {
-            var P = k.length;
-            if (P === 1) return {
-                x: a(k[0].clientX),
-                y: a(k[0].clientY)
+        function Hl(S) {
+            var D = S.length;
+            if (D === 1) return {
+                x: a(S[0].clientX),
+                y: a(S[0].clientY)
             };
-            for (var N = 0, $ = 0, J = 0; J < P;) N += k[J].clientX, $ += k[J].clientY, J++;
+            for (var N = 0, U = 0, J = 0; J < D;) N += S[J].clientX, U += S[J].clientY, J++;
             return {
-                x: a(N / P),
-                y: a($ / P)
+                x: a(N / D),
+                y: a(U / D)
             }
         }
 
-        function Jr(k, P, N) {
+        function Jr(S, D, N) {
             return {
-                x: P / k || 0,
-                y: N / k || 0
+                x: D / S || 0,
+                y: N / S || 0
             }
         }
 
-        function Zs(k, P) {
-            return k === P ? Yt : l(k) >= l(P) ? k < 0 ? Di : Oi : P < 0 ? D : H
+        function Ks(S, D) {
+            return S === D ? Yt : l(S) >= l(D) ? S < 0 ? Mi : Oi : D < 0 ? M : H
         }
 
-        function eo(k, P, N) {
+        function eo(S, D, N) {
             N || (N = le);
-            var $ = P[N[0]] - k[N[0]],
-                J = P[N[1]] - k[N[1]];
-            return Math.sqrt($ * $ + J * J)
+            var U = D[N[0]] - S[N[0]],
+                J = D[N[1]] - S[N[1]];
+            return Math.sqrt(U * U + J * J)
         }
 
-        function Gs(k, P, N) {
+        function Gs(S, D, N) {
             N || (N = le);
-            var $ = P[N[0]] - k[N[0]],
-                J = P[N[1]] - k[N[1]];
-            return Math.atan2(J, $) * 180 / Math.PI
+            var U = D[N[0]] - S[N[0]],
+                J = D[N[1]] - S[N[1]];
+            return Math.atan2(J, U) * 180 / Math.PI
         }
 
-        function ar(k, P) {
-            return Gs(P[1], P[0], Pe) + Gs(k[1], k[0], Pe)
+        function ar(S, D) {
+            return Gs(D[1], D[0], De) + Gs(S[1], S[0], De)
         }
 
-        function to(k, P) {
-            return eo(P[0], P[1], Pe) / eo(k[0], k[1], Pe)
+        function to(S, D) {
+            return eo(D[0], D[1], De) / eo(S[0], S[1], De)
         }
-        var Hl = {
+        var Bl = {
                 mousedown: je,
                 mousemove: ln,
                 mouseup: Ve
             },
-            Bl = "mousedown",
+            Wl = "mousedown",
             un = "mousemove mouseup";
 
         function Ct() {
-            this.evEl = Bl, this.evWin = un, this.pressed = !1, Me.apply(this, arguments)
+            this.evEl = Wl, this.evWin = un, this.pressed = !1, Pe.apply(this, arguments)
         }
-        _(Ct, Me, {
-            handler: function(P) {
-                var N = Hl[P.type];
-                N & je && P.button === 0 && (this.pressed = !0), N & ln && P.which !== 1 && (N = Ve), this.pressed && (N & Ve && (this.pressed = !1), this.callback(this.manager, N, {
-                    pointers: [P],
-                    changedPointers: [P],
+        w(Ct, Pe, {
+            handler: function(D) {
+                var N = Bl[D.type];
+                N & je && D.button === 0 && (this.pressed = !0), N & ln && D.which !== 1 && (N = Ve), this.pressed && (N & Ve && (this.pressed = !1), this.callback(this.manager, N, {
+                    pointers: [D],
+                    changedPointers: [D],
                     pointerType: At,
-                    srcEvent: P
+                    srcEvent: D
                 }))
             }
         });
         var Qs = {
                 pointerdown: je,
                 pointermove: ln,
                 pointerup: Ve,
                 pointercancel: Ae,
                 pointerout: Ae
             },
-            Of = {
-                2: Ge,
+            Mf = {
+                2: Ke,
                 3: ot,
                 4: At,
                 5: $t
             },
-            Ks = "pointerdown",
-            Wl = "pointermove pointerup pointercancel";
-        t.MSPointerEvent && !t.PointerEvent && (Ks = "MSPointerDown", Wl = "MSPointerMove MSPointerUp MSPointerCancel");
+            Js = "pointerdown",
+            Vl = "pointermove pointerup pointercancel";
+        t.MSPointerEvent && !t.PointerEvent && (Js = "MSPointerDown", Vl = "MSPointerMove MSPointerUp MSPointerCancel");
 
-        function Js() {
-            this.evEl = Ks, this.evWin = Wl, Me.apply(this, arguments), this.store = this.manager.session.pointerEvents = []
+        function ea() {
+            this.evEl = Js, this.evWin = Vl, Pe.apply(this, arguments), this.store = this.manager.session.pointerEvents = []
         }
-        _(Js, Me, {
-            handler: function(P) {
+        w(ea, Pe, {
+            handler: function(D) {
                 var N = this.store,
-                    $ = !1,
-                    J = P.type.toLowerCase().replace("ms", ""),
+                    U = !1,
+                    J = D.type.toLowerCase().replace("ms", ""),
                     se = Qs[J],
-                    ke = Of[P.pointerType] || P.pointerType,
-                    yt = ke == Ge,
-                    Et = ie(N, P.pointerId, "pointerId");
-                se & je && (P.button === 0 || yt) ? Et < 0 && (N.push(P), Et = N.length - 1) : se & (Ve | Ae) && ($ = !0), !(Et < 0) && (N[Et] = P, this.callback(this.manager, se, {
+                    Se = Mf[D.pointerType] || D.pointerType,
+                    yt = Se == Ke,
+                    Et = ie(N, D.pointerId, "pointerId");
+                se & je && (D.button === 0 || yt) ? Et < 0 && (N.push(D), Et = N.length - 1) : se & (Ve | Ae) && (U = !0), !(Et < 0) && (N[Et] = D, this.callback(this.manager, se, {
                     pointers: N,
-                    changedPointers: [P],
-                    pointerType: ke,
-                    srcEvent: P
-                }), $ && N.splice(Et, 1))
+                    changedPointers: [D],
+                    pointerType: Se,
+                    srcEvent: D
+                }), U && N.splice(Et, 1))
             }
         });
-        var Vl = {
+        var Ul = {
                 touchstart: je,
                 touchmove: ln,
                 touchend: Ve,
                 touchcancel: Ae
             },
             lr = "touchstart",
             ur = "touchstart touchmove touchend touchcancel";
 
-        function Ul() {
-            this.evTarget = lr, this.evWin = ur, this.started = !1, Me.apply(this, arguments)
+        function $l() {
+            this.evTarget = lr, this.evWin = ur, this.started = !1, Pe.apply(this, arguments)
         }
-        _(Ul, Me, {
-            handler: function(P) {
-                var N = Vl[P.type];
+        w($l, Pe, {
+            handler: function(D) {
+                var N = Ul[D.type];
                 if (N === je && (this.started = !0), !!this.started) {
-                    var $ = Af.call(this, P, N);
-                    N & (Ve | Ae) && $[0].length - $[1].length === 0 && (this.started = !1), this.callback(this.manager, N, {
-                        pointers: $[0],
-                        changedPointers: $[1],
-                        pointerType: Ge,
-                        srcEvent: P
+                    var U = Of.call(this, D, N);
+                    N & (Ve | Ae) && U[0].length - U[1].length === 0 && (this.started = !1), this.callback(this.manager, N, {
+                        pointers: U[0],
+                        changedPointers: U[1],
+                        pointerType: Ke,
+                        srcEvent: D
                     })
                 }
             }
         });
 
-        function Af(k, P) {
-            var N = ce(k.touches),
-                $ = ce(k.changedTouches);
-            return P & (Ve | Ae) && (N = he(N.concat($), "identifier", !0)), [N, $]
+        function Of(S, D) {
+            var N = ce(S.touches),
+                U = ce(S.changedTouches);
+            return D & (Ve | Ae) && (N = he(N.concat(U), "identifier", !0)), [N, U]
         }
-        var ea = {
+        var ta = {
                 touchstart: je,
                 touchmove: ln,
                 touchend: Ve,
                 touchcancel: Ae
             },
             $o = "touchstart touchmove touchend touchcancel";
 
         function Yo() {
-            this.evTarget = $o, this.targetIds = {}, Me.apply(this, arguments)
+            this.evTarget = $o, this.targetIds = {}, Pe.apply(this, arguments)
         }
-        _(Yo, Me, {
-            handler: function(P) {
-                var N = ea[P.type],
-                    $ = Lf.call(this, P, N);
-                $ && this.callback(this.manager, N, {
-                    pointers: $[0],
-                    changedPointers: $[1],
-                    pointerType: Ge,
-                    srcEvent: P
+        w(Yo, Pe, {
+            handler: function(D) {
+                var N = ta[D.type],
+                    U = Af.call(this, D, N);
+                U && this.callback(this.manager, N, {
+                    pointers: U[0],
+                    changedPointers: U[1],
+                    pointerType: Ke,
+                    srcEvent: D
                 })
             }
         });
 
-        function Lf(k, P) {
-            var N = ce(k.touches),
-                $ = this.targetIds;
-            if (P & (je | ln) && N.length === 1) return $[N[0].identifier] = !0, [N, N];
-            var J, se, ke = ce(k.changedTouches),
+        function Af(S, D) {
+            var N = ce(S.touches),
+                U = this.targetIds;
+            if (D & (je | ln) && N.length === 1) return U[N[0].identifier] = !0, [N, N];
+            var J, se, Se = ce(S.changedTouches),
                 yt = [],
                 Et = this.target;
             if (se = N.filter(function(Lt) {
-                    return Y(Lt.target, Et)
-                }), P === je)
-                for (J = 0; J < se.length;) $[se[J].identifier] = !0, J++;
-            for (J = 0; J < ke.length;) $[ke[J].identifier] && yt.push(ke[J]), P & (Ve | Ae) && delete $[ke[J].identifier], J++;
+                    return $(Lt.target, Et)
+                }), D === je)
+                for (J = 0; J < se.length;) U[se[J].identifier] = !0, J++;
+            for (J = 0; J < Se.length;) U[Se[J].identifier] && yt.push(Se[J]), D & (Ve | Ae) && delete U[Se[J].identifier], J++;
             if (yt.length) return [he(se.concat(yt), "identifier", !0), yt]
         }
-        var Rf = 2500,
-            ta = 25;
+        var Lf = 2500,
+            na = 25;
 
-        function na() {
-            Me.apply(this, arguments);
-            var k = C(this.handler, this);
-            this.touch = new Yo(this.manager, k), this.mouse = new Ct(this.manager, k), this.primaryTouch = null, this.lastTouches = []
-        }
-        _(na, Me, {
-            handler: function(P, N, $) {
-                var J = $.pointerType == Ge,
-                    se = $.pointerType == At;
-                if (!(se && $.sourceCapabilities && $.sourceCapabilities.firesTouchEvents)) {
-                    if (J) If.call(this, N, $);
-                    else if (se && Nf.call(this, $)) return;
-                    this.callback(P, N, $)
+        function ia() {
+            Pe.apply(this, arguments);
+            var S = k(this.handler, this);
+            this.touch = new Yo(this.manager, S), this.mouse = new Ct(this.manager, S), this.primaryTouch = null, this.lastTouches = []
+        }
+        w(ia, Pe, {
+            handler: function(D, N, U) {
+                var J = U.pointerType == Ke,
+                    se = U.pointerType == At;
+                if (!(se && U.sourceCapabilities && U.sourceCapabilities.firesTouchEvents)) {
+                    if (J) Rf.call(this, N, U);
+                    else if (se && If.call(this, U)) return;
+                    this.callback(D, N, U)
                 }
             },
             destroy: function() {
                 this.touch.destroy(), this.mouse.destroy()
             }
         });
 
-        function If(k, P) {
-            k & je ? (this.primaryTouch = P.changedPointers[0].identifier, ia.call(this, P)) : k & (Ve | Ae) && ia.call(this, P)
+        function Rf(S, D) {
+            S & je ? (this.primaryTouch = D.changedPointers[0].identifier, ra.call(this, D)) : S & (Ve | Ae) && ra.call(this, D)
         }
 
-        function ia(k) {
-            var P = k.changedPointers[0];
-            if (P.identifier === this.primaryTouch) {
+        function ra(S) {
+            var D = S.changedPointers[0];
+            if (D.identifier === this.primaryTouch) {
                 var N = {
-                    x: P.clientX,
-                    y: P.clientY
+                    x: D.clientX,
+                    y: D.clientY
                 };
                 this.lastTouches.push(N);
-                var $ = this.lastTouches,
+                var U = this.lastTouches,
                     J = function() {
-                        var se = $.indexOf(N);
-                        se > -1 && $.splice(se, 1)
+                        var se = U.indexOf(N);
+                        se > -1 && U.splice(se, 1)
                     };
-                setTimeout(J, Rf)
+                setTimeout(J, Lf)
             }
         }
 
-        function Nf(k) {
-            for (var P = k.srcEvent.clientX, N = k.srcEvent.clientY, $ = 0; $ < this.lastTouches.length; $++) {
-                var J = this.lastTouches[$],
-                    se = Math.abs(P - J.x),
-                    ke = Math.abs(N - J.y);
-                if (se <= ta && ke <= ta) return !0
+        function If(S) {
+            for (var D = S.srcEvent.clientX, N = S.srcEvent.clientY, U = 0; U < this.lastTouches.length; U++) {
+                var J = this.lastTouches[U],
+                    se = Math.abs(D - J.x),
+                    Se = Math.abs(N - J.y);
+                if (se <= na && Se <= na) return !0
             }
             return !1
         }
         var Ri = Fe(o.style, "touchAction"),
-            ra = Ri !== i,
+            oa = Ri !== i,
             Xo = "compute",
             no = "auto",
             qo = "manipulation",
             Ii = "none",
-            Qn = "pan-x",
+            Gn = "pan-x",
             cr = "pan-y",
-            io = zf();
+            io = Nf();
 
-        function Zo(k, P) {
-            this.manager = k, this.set(P)
+        function Zo(S, D) {
+            this.manager = S, this.set(D)
         }
         Zo.prototype = {
-            set: function(k) {
-                k == Xo && (k = this.compute()), ra && this.manager.element.style && io[k] && (this.manager.element.style[Ri] = k), this.actions = k.toLowerCase().trim()
+            set: function(S) {
+                S == Xo && (S = this.compute()), oa && this.manager.element.style && io[S] && (this.manager.element.style[Ri] = S), this.actions = S.toLowerCase().trim()
             },
             update: function() {
                 this.set(this.manager.options.touchAction)
             },
             compute: function() {
-                var k = [];
-                return y(this.manager.recognizers, function(P) {
-                    M(P.options.enable, [P]) && (k = k.concat(P.getTouchAction()))
-                }), $l(k.join(" "))
-            },
-            preventDefaults: function(k) {
-                var P = k.srcEvent,
-                    N = k.offsetDirection;
+                var S = [];
+                return y(this.manager.recognizers, function(D) {
+                    P(D.options.enable, [D]) && (S = S.concat(D.getTouchAction()))
+                }), Yl(S.join(" "))
+            },
+            preventDefaults: function(S) {
+                var D = S.srcEvent,
+                    N = S.offsetDirection;
                 if (this.manager.session.prevented) {
-                    P.preventDefault();
+                    D.preventDefault();
                     return
                 }
-                var $ = this.actions,
-                    J = V($, Ii) && !io[Ii],
-                    se = V($, cr) && !io[cr],
-                    ke = V($, Qn) && !io[Qn];
+                var U = this.actions,
+                    J = Y(U, Ii) && !io[Ii],
+                    se = Y(U, cr) && !io[cr],
+                    Se = Y(U, Gn) && !io[Gn];
                 if (J) {
-                    var yt = k.pointers.length === 1,
-                        Et = k.distance < 2,
-                        Lt = k.deltaTime < 250;
+                    var yt = S.pointers.length === 1,
+                        Et = S.distance < 2,
+                        Lt = S.deltaTime < 250;
                     if (yt && Et && Lt) return
                 }
-                if (!(ke && se) && (J || se && N & O || ke && N & X)) return this.preventSrc(P)
+                if (!(Se && se) && (J || se && N & O || Se && N & X)) return this.preventSrc(D)
             },
-            preventSrc: function(k) {
-                this.manager.session.prevented = !0, k.preventDefault()
+            preventSrc: function(S) {
+                this.manager.session.prevented = !0, S.preventDefault()
             }
         };
 
-        function $l(k) {
-            if (V(k, Ii)) return Ii;
-            var P = V(k, Qn),
-                N = V(k, cr);
-            return P && N ? Ii : P || N ? P ? Qn : cr : V(k, qo) ? qo : no
+        function Yl(S) {
+            if (Y(S, Ii)) return Ii;
+            var D = Y(S, Gn),
+                N = Y(S, cr);
+            return D && N ? Ii : D || N ? D ? Gn : cr : Y(S, qo) ? qo : no
         }
 
-        function zf() {
-            if (!ra) return !1;
-            var k = {},
-                P = t.CSS && t.CSS.supports;
+        function Nf() {
+            if (!oa) return !1;
+            var S = {},
+                D = t.CSS && t.CSS.supports;
             return ["auto", "manipulation", "pan-y", "pan-x", "pan-x pan-y", "none"].forEach(function(N) {
-                k[N] = P ? t.CSS.supports("touch-action", N) : !0
-            }), k
+                S[N] = D ? t.CSS.supports("touch-action", N) : !0
+            }), S
         }
         var fr = 1,
             cn = 2,
             Ni = 4,
             yi = 8,
             jn = yi,
             dr = 16,
             fn = 32;
 
-        function Hn(k) {
-            this.options = w({}, this.defaults, k || {}), this.id = Ee(), this.manager = null, this.options.enable = z(this.options.enable, !0), this.state = fr, this.simultaneous = {}, this.requireFail = []
+        function Hn(S) {
+            this.options = _({}, this.defaults, S || {}), this.id = Ee(), this.manager = null, this.options.enable = z(this.options.enable, !0), this.state = fr, this.simultaneous = {}, this.requireFail = []
         }
         Hn.prototype = {
             defaults: {},
-            set: function(k) {
-                return w(this.options, k), this.manager && this.manager.touchAction.update(), this
+            set: function(S) {
+                return _(this.options, S), this.manager && this.manager.touchAction.update(), this
             },
-            recognizeWith: function(k) {
-                if (g(k, "recognizeWith", this)) return this;
-                var P = this.simultaneous;
-                return k = Fi(k, this), P[k.id] || (P[k.id] = k, k.recognizeWith(this)), this
-            },
-            dropRecognizeWith: function(k) {
-                return g(k, "dropRecognizeWith", this) ? this : (k = Fi(k, this), delete this.simultaneous[k.id], this)
-            },
-            requireFailure: function(k) {
-                if (g(k, "requireFailure", this)) return this;
-                var P = this.requireFail;
-                return k = Fi(k, this), ie(P, k) === -1 && (P.push(k), k.requireFailure(this)), this
-            },
-            dropRequireFailure: function(k) {
-                if (g(k, "dropRequireFailure", this)) return this;
-                k = Fi(k, this);
-                var P = ie(this.requireFail, k);
-                return P > -1 && this.requireFail.splice(P, 1), this
+            recognizeWith: function(S) {
+                if (g(S, "recognizeWith", this)) return this;
+                var D = this.simultaneous;
+                return S = Fi(S, this), D[S.id] || (D[S.id] = S, S.recognizeWith(this)), this
+            },
+            dropRecognizeWith: function(S) {
+                return g(S, "dropRecognizeWith", this) ? this : (S = Fi(S, this), delete this.simultaneous[S.id], this)
+            },
+            requireFailure: function(S) {
+                if (g(S, "requireFailure", this)) return this;
+                var D = this.requireFail;
+                return S = Fi(S, this), ie(D, S) === -1 && (D.push(S), S.requireFailure(this)), this
+            },
+            dropRequireFailure: function(S) {
+                if (g(S, "dropRequireFailure", this)) return this;
+                S = Fi(S, this);
+                var D = ie(this.requireFail, S);
+                return D > -1 && this.requireFail.splice(D, 1), this
             },
             hasRequireFailures: function() {
                 return this.requireFail.length > 0
             },
-            canRecognizeWith: function(k) {
-                return !!this.simultaneous[k.id]
+            canRecognizeWith: function(S) {
+                return !!this.simultaneous[S.id]
             },
-            emit: function(k) {
-                var P = this,
+            emit: function(S) {
+                var D = this,
                     N = this.state;
 
-                function $(J) {
-                    P.manager.emit(J, k)
+                function U(J) {
+                    D.manager.emit(J, S)
                 }
-                N < yi && $(P.options.event + jt(N)), $(P.options.event), k.additionalEvent && $(k.additionalEvent), N >= yi && $(P.options.event + jt(N))
+                N < yi && U(D.options.event + jt(N)), U(D.options.event), S.additionalEvent && U(S.additionalEvent), N >= yi && U(D.options.event + jt(N))
             },
-            tryEmit: function(k) {
-                if (this.canEmit()) return this.emit(k);
+            tryEmit: function(S) {
+                if (this.canEmit()) return this.emit(S);
                 this.state = fn
             },
             canEmit: function() {
-                for (var k = 0; k < this.requireFail.length;) {
-                    if (!(this.requireFail[k].state & (fn | fr))) return !1;
-                    k++
+                for (var S = 0; S < this.requireFail.length;) {
+                    if (!(this.requireFail[S].state & (fn | fr))) return !1;
+                    S++
                 }
                 return !0
             },
-            recognize: function(k) {
-                var P = w({}, k);
-                if (!M(this.options.enable, [this, P])) {
+            recognize: function(S) {
+                var D = _({}, S);
+                if (!P(this.options.enable, [this, D])) {
                     this.reset(), this.state = fn;
                     return
                 }
-                this.state & (jn | dr | fn) && (this.state = fr), this.state = this.process(P), this.state & (cn | Ni | yi | dr) && this.tryEmit(P)
+                this.state & (jn | dr | fn) && (this.state = fr), this.state = this.process(D), this.state & (cn | Ni | yi | dr) && this.tryEmit(D)
             },
-            process: function(k) {},
+            process: function(S) {},
             getTouchAction: function() {},
             reset: function() {}
         };
 
-        function jt(k) {
-            return k & dr ? "cancel" : k & yi ? "end" : k & Ni ? "move" : k & cn ? "start" : ""
+        function jt(S) {
+            return S & dr ? "cancel" : S & yi ? "end" : S & Ni ? "move" : S & cn ? "start" : ""
         }
 
-        function zi(k) {
-            return k == H ? "down" : k == D ? "up" : k == Di ? "left" : k == Oi ? "right" : ""
+        function zi(S) {
+            return S == H ? "down" : S == M ? "up" : S == Mi ? "left" : S == Oi ? "right" : ""
         }
 
-        function Fi(k, P) {
-            var N = P.manager;
-            return N ? N.get(k) : k
+        function Fi(S, D) {
+            var N = D.manager;
+            return N ? N.get(S) : S
         }
 
         function Cn() {
             Hn.apply(this, arguments)
         }
-        _(Cn, Hn, {
+        w(Cn, Hn, {
             defaults: {
                 pointers: 1
             },
-            attrTest: function(k) {
-                var P = this.options.pointers;
-                return P === 0 || k.pointers.length === P
-            },
-            process: function(k) {
-                var P = this.state,
-                    N = k.eventType,
-                    $ = P & (cn | Ni),
-                    J = this.attrTest(k);
-                return $ && (N & Ae || !J) ? P | dr : $ || J ? N & Ve ? P | yi : P & cn ? P | Ni : cn : fn
+            attrTest: function(S) {
+                var D = this.options.pointers;
+                return D === 0 || S.pointers.length === D
+            },
+            process: function(S) {
+                var D = this.state,
+                    N = S.eventType,
+                    U = D & (cn | Ni),
+                    J = this.attrTest(S);
+                return U && (N & Ae || !J) ? D | dr : U || J ? N & Ve ? D | yi : D & cn ? D | Ni : cn : fn
             }
         });
 
-        function Go() {
+        function Ko() {
             Cn.apply(this, arguments), this.pX = null, this.pY = null
         }
-        _(Go, Cn, {
+        w(Ko, Cn, {
             defaults: {
                 event: "pan",
                 threshold: 10,
                 pointers: 1,
                 direction: re
             },
             getTouchAction: function() {
-                var k = this.options.direction,
-                    P = [];
-                return k & O && P.push(cr), k & X && P.push(Qn), P
+                var S = this.options.direction,
+                    D = [];
+                return S & O && D.push(cr), S & X && D.push(Gn), D
             },
-            directionTest: function(k) {
-                var P = this.options,
+            directionTest: function(S) {
+                var D = this.options,
                     N = !0,
-                    $ = k.distance,
-                    J = k.direction,
-                    se = k.deltaX,
-                    ke = k.deltaY;
-                return J & P.direction || (P.direction & O ? (J = se === 0 ? Yt : se < 0 ? Di : Oi, N = se != this.pX, $ = Math.abs(k.deltaX)) : (J = ke === 0 ? Yt : ke < 0 ? D : H, N = ke != this.pY, $ = Math.abs(k.deltaY))), k.direction = J, N && $ > P.threshold && J & P.direction
-            },
-            attrTest: function(k) {
-                return Cn.prototype.attrTest.call(this, k) && (this.state & cn || !(this.state & cn) && this.directionTest(k))
-            },
-            emit: function(k) {
-                this.pX = k.deltaX, this.pY = k.deltaY;
-                var P = zi(k.direction);
-                P && (k.additionalEvent = this.options.event + P), this._super.emit.call(this, k)
+                    U = S.distance,
+                    J = S.direction,
+                    se = S.deltaX,
+                    Se = S.deltaY;
+                return J & D.direction || (D.direction & O ? (J = se === 0 ? Yt : se < 0 ? Mi : Oi, N = se != this.pX, U = Math.abs(S.deltaX)) : (J = Se === 0 ? Yt : Se < 0 ? M : H, N = Se != this.pY, U = Math.abs(S.deltaY))), S.direction = J, N && U > D.threshold && J & D.direction
+            },
+            attrTest: function(S) {
+                return Cn.prototype.attrTest.call(this, S) && (this.state & cn || !(this.state & cn) && this.directionTest(S))
+            },
+            emit: function(S) {
+                this.pX = S.deltaX, this.pY = S.deltaY;
+                var D = zi(S.direction);
+                D && (S.additionalEvent = this.options.event + D), this._super.emit.call(this, S)
             }
         });
 
         function ro() {
             Cn.apply(this, arguments)
         }
-        _(ro, Cn, {
+        w(ro, Cn, {
             defaults: {
                 event: "pinch",
                 threshold: 0,
                 pointers: 2
             },
             getTouchAction: function() {
                 return [Ii]
             },
-            attrTest: function(k) {
-                return this._super.attrTest.call(this, k) && (Math.abs(k.scale - 1) > this.options.threshold || this.state & cn)
+            attrTest: function(S) {
+                return this._super.attrTest.call(this, S) && (Math.abs(S.scale - 1) > this.options.threshold || this.state & cn)
             },
-            emit: function(k) {
-                if (k.scale !== 1) {
-                    var P = k.scale < 1 ? "in" : "out";
-                    k.additionalEvent = this.options.event + P
+            emit: function(S) {
+                if (S.scale !== 1) {
+                    var D = S.scale < 1 ? "in" : "out";
+                    S.additionalEvent = this.options.event + D
                 }
-                this._super.emit.call(this, k)
+                this._super.emit.call(this, S)
             }
         });
 
-        function Qo() {
+        function Go() {
             Hn.apply(this, arguments), this._timer = null, this._input = null
         }
-        _(Qo, Hn, {
+        w(Go, Hn, {
             defaults: {
                 event: "press",
                 pointers: 1,
                 time: 251,
                 threshold: 9
             },
             getTouchAction: function() {
                 return [no]
             },
-            process: function(k) {
-                var P = this.options,
-                    N = k.pointers.length === P.pointers,
-                    $ = k.distance < P.threshold,
-                    J = k.deltaTime > P.time;
-                if (this._input = k, !$ || !N || k.eventType & (Ve | Ae) && !J) this.reset();
-                else if (k.eventType & je) this.reset(), this._timer = d(function() {
+            process: function(S) {
+                var D = this.options,
+                    N = S.pointers.length === D.pointers,
+                    U = S.distance < D.threshold,
+                    J = S.deltaTime > D.time;
+                if (this._input = S, !U || !N || S.eventType & (Ve | Ae) && !J) this.reset();
+                else if (S.eventType & je) this.reset(), this._timer = d(function() {
                     this.state = jn, this.tryEmit()
-                }, P.time, this);
-                else if (k.eventType & Ve) return jn;
+                }, D.time, this);
+                else if (S.eventType & Ve) return jn;
                 return fn
             },
             reset: function() {
                 clearTimeout(this._timer)
             },
-            emit: function(k) {
-                this.state === jn && (k && k.eventType & Ve ? this.manager.emit(this.options.event + "up", k) : (this._input.timeStamp = c(), this.manager.emit(this.options.event, this._input)))
+            emit: function(S) {
+                this.state === jn && (S && S.eventType & Ve ? this.manager.emit(this.options.event + "up", S) : (this._input.timeStamp = c(), this.manager.emit(this.options.event, this._input)))
             }
         });
 
         function hr() {
             Cn.apply(this, arguments)
         }
-        _(hr, Cn, {
+        w(hr, Cn, {
             defaults: {
                 event: "rotate",
                 threshold: 0,
                 pointers: 2
             },
             getTouchAction: function() {
                 return [Ii]
             },
-            attrTest: function(k) {
-                return this._super.attrTest.call(this, k) && (Math.abs(k.rotation) > this.options.threshold || this.state & cn)
+            attrTest: function(S) {
+                return this._super.attrTest.call(this, S) && (Math.abs(S.rotation) > this.options.threshold || this.state & cn)
             }
         });
 
-        function Ko() {
+        function Qo() {
             Cn.apply(this, arguments)
         }
-        _(Ko, Cn, {
+        w(Qo, Cn, {
             defaults: {
                 event: "swipe",
                 threshold: 10,
                 velocity: .3,
                 direction: O | X,
                 pointers: 1
             },
             getTouchAction: function() {
-                return Go.prototype.getTouchAction.call(this)
+                return Ko.prototype.getTouchAction.call(this)
             },
-            attrTest: function(k) {
-                var P = this.options.direction,
+            attrTest: function(S) {
+                var D = this.options.direction,
                     N;
-                return P & (O | X) ? N = k.overallVelocity : P & O ? N = k.overallVelocityX : P & X && (N = k.overallVelocityY), this._super.attrTest.call(this, k) && P & k.offsetDirection && k.distance > this.options.threshold && k.maxPointers == this.options.pointers && l(N) > this.options.velocity && k.eventType & Ve
+                return D & (O | X) ? N = S.overallVelocity : D & O ? N = S.overallVelocityX : D & X && (N = S.overallVelocityY), this._super.attrTest.call(this, S) && D & S.offsetDirection && S.distance > this.options.threshold && S.maxPointers == this.options.pointers && l(N) > this.options.velocity && S.eventType & Ve
             },
-            emit: function(k) {
-                var P = zi(k.offsetDirection);
-                P && this.manager.emit(this.options.event + P, k), this.manager.emit(this.options.event, k)
+            emit: function(S) {
+                var D = zi(S.offsetDirection);
+                D && this.manager.emit(this.options.event + D, S), this.manager.emit(this.options.event, S)
             }
         });
 
         function Jo() {
             Hn.apply(this, arguments), this.pTime = !1, this.pCenter = !1, this._timer = null, this._input = null, this.count = 0
         }
-        _(Jo, Hn, {
+        w(Jo, Hn, {
             defaults: {
                 event: "tap",
                 pointers: 1,
                 taps: 1,
                 interval: 300,
                 time: 250,
                 threshold: 9,
                 posThreshold: 10
             },
             getTouchAction: function() {
                 return [qo]
             },
-            process: function(k) {
-                var P = this.options,
-                    N = k.pointers.length === P.pointers,
-                    $ = k.distance < P.threshold,
-                    J = k.deltaTime < P.time;
-                if (this.reset(), k.eventType & je && this.count === 0) return this.failTimeout();
-                if ($ && J && N) {
-                    if (k.eventType != Ve) return this.failTimeout();
-                    var se = this.pTime ? k.timeStamp - this.pTime < P.interval : !0,
-                        ke = !this.pCenter || eo(this.pCenter, k.center) < P.posThreshold;
-                    this.pTime = k.timeStamp, this.pCenter = k.center, !ke || !se ? this.count = 1 : this.count += 1, this._input = k;
-                    var yt = this.count % P.taps;
+            process: function(S) {
+                var D = this.options,
+                    N = S.pointers.length === D.pointers,
+                    U = S.distance < D.threshold,
+                    J = S.deltaTime < D.time;
+                if (this.reset(), S.eventType & je && this.count === 0) return this.failTimeout();
+                if (U && J && N) {
+                    if (S.eventType != Ve) return this.failTimeout();
+                    var se = this.pTime ? S.timeStamp - this.pTime < D.interval : !0,
+                        Se = !this.pCenter || eo(this.pCenter, S.center) < D.posThreshold;
+                    this.pTime = S.timeStamp, this.pCenter = S.center, !Se || !se ? this.count = 1 : this.count += 1, this._input = S;
+                    var yt = this.count % D.taps;
                     if (yt === 0) return this.hasRequireFailures() ? (this._timer = d(function() {
                         this.state = jn, this.tryEmit()
-                    }, P.interval, this), cn) : jn
+                    }, D.interval, this), cn) : jn
                 }
                 return fn
             },
             failTimeout: function() {
                 return this._timer = d(function() {
                     this.state = fn
                 }, this.options.interval, this), fn
@@ -7862,214 +7862,214 @@
                 clearTimeout(this._timer)
             },
             emit: function() {
                 this.state == jn && (this._input.tapCount = this.count, this.manager.emit(this.options.event, this._input))
             }
         });
 
-        function Kn(k, P) {
-            return P = P || {}, P.recognizers = z(P.recognizers, Kn.defaults.preset), new ji(k, P)
+        function Qn(S, D) {
+            return D = D || {}, D.recognizers = z(D.recognizers, Qn.defaults.preset), new ji(S, D)
         }
-        Kn.VERSION = "2.0.7", Kn.defaults = {
+        Qn.VERSION = "2.0.7", Qn.defaults = {
             domEvents: !1,
             touchAction: Xo,
             enable: !0,
             inputTarget: null,
             inputClass: null,
             preset: [
                 [hr, {
                     enable: !1
                 }],
                 [ro, {
                         enable: !1
                     },
                     ["rotate"]
                 ],
-                [Ko, {
+                [Qo, {
                     direction: O
                 }],
-                [Go, {
+                [Ko, {
                         direction: O
                     },
                     ["swipe"]
                 ],
                 [Jo],
                 [Jo, {
                         event: "doubletap",
                         taps: 2
                     },
                     ["tap"]
                 ],
-                [Qo]
+                [Go]
             ],
             cssProps: {
                 userSelect: "none",
                 touchSelect: "none",
                 touchCallout: "none",
                 contentZooming: "none",
                 userDrag: "none",
                 tapHighlightColor: "rgba(0,0,0,0)"
             }
         };
         var En = 1,
-            oa = 2;
+            sa = 2;
 
-        function ji(k, P) {
-            this.options = w({}, Kn.defaults, P || {}), this.options.inputTarget = this.options.inputTarget || k, this.handlers = {}, this.session = {}, this.recognizers = [], this.oldCssProps = {}, this.element = k, this.input = Qe(this), this.touchAction = new Zo(this, this.options.touchAction), Yl(this, !0), y(this.options.recognizers, function(N) {
-                var $ = this.add(new N[0](N[1]));
-                N[2] && $.recognizeWith(N[2]), N[3] && $.requireFailure(N[3])
+        function ji(S, D) {
+            this.options = _({}, Qn.defaults, D || {}), this.options.inputTarget = this.options.inputTarget || S, this.handlers = {}, this.session = {}, this.recognizers = [], this.oldCssProps = {}, this.element = S, this.input = Ge(this), this.touchAction = new Zo(this, this.options.touchAction), Xl(this, !0), y(this.options.recognizers, function(N) {
+                var U = this.add(new N[0](N[1]));
+                N[2] && U.recognizeWith(N[2]), N[3] && U.requireFailure(N[3])
             }, this)
         }
         ji.prototype = {
-            set: function(k) {
-                return w(this.options, k), k.touchAction && this.touchAction.update(), k.inputTarget && (this.input.destroy(), this.input.target = k.inputTarget, this.input.init()), this
+            set: function(S) {
+                return _(this.options, S), S.touchAction && this.touchAction.update(), S.inputTarget && (this.input.destroy(), this.input.target = S.inputTarget, this.input.init()), this
             },
-            stop: function(k) {
-                this.session.stopped = k ? oa : En
+            stop: function(S) {
+                this.session.stopped = S ? sa : En
             },
-            recognize: function(k) {
-                var P = this.session;
-                if (!P.stopped) {
-                    this.touchAction.preventDefaults(k);
-                    var N, $ = this.recognizers,
-                        J = P.curRecognizer;
-                    (!J || J && J.state & jn) && (J = P.curRecognizer = null);
-                    for (var se = 0; se < $.length;) N = $[se], P.stopped !== oa && (!J || N == J || N.canRecognizeWith(J)) ? N.recognize(k) : N.reset(), !J && N.state & (cn | Ni | yi) && (J = P.curRecognizer = N), se++
-                }
-            },
-            get: function(k) {
-                if (k instanceof Hn) return k;
-                for (var P = this.recognizers, N = 0; N < P.length; N++)
-                    if (P[N].options.event == k) return P[N];
+            recognize: function(S) {
+                var D = this.session;
+                if (!D.stopped) {
+                    this.touchAction.preventDefaults(S);
+                    var N, U = this.recognizers,
+                        J = D.curRecognizer;
+                    (!J || J && J.state & jn) && (J = D.curRecognizer = null);
+                    for (var se = 0; se < U.length;) N = U[se], D.stopped !== sa && (!J || N == J || N.canRecognizeWith(J)) ? N.recognize(S) : N.reset(), !J && N.state & (cn | Ni | yi) && (J = D.curRecognizer = N), se++
+                }
+            },
+            get: function(S) {
+                if (S instanceof Hn) return S;
+                for (var D = this.recognizers, N = 0; N < D.length; N++)
+                    if (D[N].options.event == S) return D[N];
                 return null
             },
-            add: function(k) {
-                if (g(k, "add", this)) return this;
-                var P = this.get(k.options.event);
-                return P && this.remove(P), this.recognizers.push(k), k.manager = this, this.touchAction.update(), k
-            },
-            remove: function(k) {
-                if (g(k, "remove", this)) return this;
-                if (k = this.get(k), k) {
-                    var P = this.recognizers,
-                        N = ie(P, k);
-                    N !== -1 && (P.splice(N, 1), this.touchAction.update())
+            add: function(S) {
+                if (g(S, "add", this)) return this;
+                var D = this.get(S.options.event);
+                return D && this.remove(D), this.recognizers.push(S), S.manager = this, this.touchAction.update(), S
+            },
+            remove: function(S) {
+                if (g(S, "remove", this)) return this;
+                if (S = this.get(S), S) {
+                    var D = this.recognizers,
+                        N = ie(D, S);
+                    N !== -1 && (D.splice(N, 1), this.touchAction.update())
                 }
                 return this
             },
-            on: function(k, P) {
-                if (k !== i && P !== i) {
+            on: function(S, D) {
+                if (S !== i && D !== i) {
                     var N = this.handlers;
-                    return y(te(k), function($) {
-                        N[$] = N[$] || [], N[$].push(P)
+                    return y(ne(S), function(U) {
+                        N[U] = N[U] || [], N[U].push(D)
                     }), this
                 }
             },
-            off: function(k, P) {
-                if (k !== i) {
+            off: function(S, D) {
+                if (S !== i) {
                     var N = this.handlers;
-                    return y(te(k), function($) {
-                        P ? N[$] && N[$].splice(ie(N[$], P), 1) : delete N[$]
+                    return y(ne(S), function(U) {
+                        D ? N[U] && N[U].splice(ie(N[U], D), 1) : delete N[U]
                     }), this
                 }
             },
-            emit: function(k, P) {
-                this.options.domEvents && Ff(k, P);
-                var N = this.handlers[k] && this.handlers[k].slice();
+            emit: function(S, D) {
+                this.options.domEvents && zf(S, D);
+                var N = this.handlers[S] && this.handlers[S].slice();
                 if (!(!N || !N.length)) {
-                    P.type = k, P.preventDefault = function() {
-                        P.srcEvent.preventDefault()
+                    D.type = S, D.preventDefault = function() {
+                        D.srcEvent.preventDefault()
                     };
-                    for (var $ = 0; $ < N.length;) N[$](P), $++
+                    for (var U = 0; U < N.length;) N[U](D), U++
                 }
             },
             destroy: function() {
-                this.element && Yl(this, !1), this.handlers = {}, this.session = {}, this.input.destroy(), this.element = null
+                this.element && Xl(this, !1), this.handlers = {}, this.session = {}, this.input.destroy(), this.element = null
             }
         };
 
-        function Yl(k, P) {
-            var N = k.element;
+        function Xl(S, D) {
+            var N = S.element;
             if (N.style) {
-                var $;
-                y(k.options.cssProps, function(J, se) {
-                    $ = Fe(N.style, se), P ? (k.oldCssProps[$] = N.style[$], N.style[$] = J) : N.style[$] = k.oldCssProps[$] || ""
-                }), P || (k.oldCssProps = {})
+                var U;
+                y(S.options.cssProps, function(J, se) {
+                    U = Fe(N.style, se), D ? (S.oldCssProps[U] = N.style[U], N.style[U] = J) : N.style[U] = S.oldCssProps[U] || ""
+                }), D || (S.oldCssProps = {})
             }
         }
 
-        function Ff(k, P) {
+        function zf(S, D) {
             var N = e.createEvent("Event");
-            N.initEvent(k, !0, !0), N.gesture = P, P.target.dispatchEvent(N)
+            N.initEvent(S, !0, !0), N.gesture = D, D.target.dispatchEvent(N)
         }
-        w(Kn, {
+        _(Qn, {
             INPUT_START: je,
             INPUT_MOVE: ln,
             INPUT_END: Ve,
             INPUT_CANCEL: Ae,
             STATE_POSSIBLE: fr,
             STATE_BEGAN: cn,
             STATE_CHANGED: Ni,
             STATE_ENDED: yi,
             STATE_RECOGNIZED: jn,
             STATE_CANCELLED: dr,
             STATE_FAILED: fn,
             DIRECTION_NONE: Yt,
-            DIRECTION_LEFT: Di,
+            DIRECTION_LEFT: Mi,
             DIRECTION_RIGHT: Oi,
-            DIRECTION_UP: D,
+            DIRECTION_UP: M,
             DIRECTION_DOWN: H,
             DIRECTION_HORIZONTAL: O,
             DIRECTION_VERTICAL: X,
             DIRECTION_ALL: re,
             Manager: ji,
-            Input: Me,
+            Input: Pe,
             TouchAction: Zo,
             TouchInput: Yo,
             MouseInput: Ct,
-            PointerEventInput: Js,
-            TouchMouseInput: na,
-            SingleTouchInput: Ul,
+            PointerEventInput: ea,
+            TouchMouseInput: ia,
+            SingleTouchInput: $l,
             Recognizer: Hn,
             AttrRecognizer: Cn,
             Tap: Jo,
-            Pan: Go,
-            Swipe: Ko,
+            Pan: Ko,
+            Swipe: Qo,
             Pinch: ro,
             Rotate: hr,
-            Press: Qo,
+            Press: Go,
             on: F,
             off: h,
             each: y,
             merge: A,
-            extend: S,
-            assign: w,
-            inherit: _,
-            bindFn: C,
+            extend: C,
+            assign: _,
+            inherit: w,
+            bindFn: k,
             prefixed: Fe
         });
         var Hi = typeof t < "u" ? t : typeof self < "u" ? self : {};
-        Hi.Hammer = Kn, typeof define == "function" && define.amd ? define(function() {
-            return Kn
-        }) : typeof kf < "u" && kf.exports ? kf.exports = Kn : t[n] = Kn
+        Hi.Hammer = Qn, typeof define == "function" && define.amd ? define(function() {
+            return Qn
+        }) : typeof wf < "u" && wf.exports ? wf.exports = Qn : t[n] = Qn
     })(window, document, "Hammer")
 });
-var v_ = fa(ha());
-var xn = fa(ha(), 1),
-    tx = fa(ex(), 1),
+var v_ = da(pa());
+var xn = da(pa(), 1),
+    tx = da(ex(), 1),
     nx = xn.createContext(null);
 
-function gS() {
+function gk() {
     let t = xn.useContext(nx);
     if (!t) throw new Error("Model not found");
     return t
 }
 
 function Eo(t) {
-    let e = gS(),
+    let e = gk(),
         [n, i] = xn.useState(e.get(t));
     return xn.useEffect(() => {
         let r = () => i(e.get(t));
         return e.on(`change:${t}`, r), () => e.off(`change:${t}`, r)
     }, [e, t]), [n, r => {
         e.set(t, r), e.save_changes()
     }]
@@ -8082,37 +8082,37 @@
     }) => {
         let i = tx.createRoot(n);
         return i.render(xn.createElement(xn.StrictMode, null, xn.createElement(nx.Provider, {
             value: e
         }, xn.createElement(t)))), () => i.unmount()
     }
 }
-var wf = fa(ha(), 1);
+var Bs = da(pa(), 1);
 
-function al(t) {
+function ll(t) {
     return t + .5 | 0
 }
 var Fr = (t, e, n) => Math.max(Math.min(t, n), e);
 
-function ol(t) {
-    return Fr(al(t * 2.55), 0, 255)
+function sl(t) {
+    return Fr(ll(t * 2.55), 0, 255)
 }
 
 function jr(t) {
-    return Fr(al(t * 255), 0, 255)
+    return Fr(ll(t * 255), 0, 255)
 }
 
 function Ji(t) {
-    return Fr(al(t / 2.55) / 100, 0, 1)
+    return Fr(ll(t / 2.55) / 100, 0, 1)
 }
 
 function rx(t) {
-    return Fr(al(t * 100), 0, 100)
+    return Fr(ll(t * 100), 0, 100)
 }
-var Gn = {
+var Kn = {
         0: 0,
         1: 1,
         2: 2,
         3: 3,
         4: 4,
         5: 5,
         6: 6,
@@ -8128,121 +8128,121 @@
         a: 10,
         b: 11,
         c: 12,
         d: 13,
         e: 14,
         f: 15
     },
-    vp = [..."0123456789ABCDEF"],
-    mS = t => vp[t & 15],
-    yS = t => vp[(t & 240) >> 4] + vp[t & 15],
-    wc = t => (t & 240) >> 4 === (t & 15),
-    vS = t => wc(t.r) && wc(t.g) && wc(t.b) && wc(t.a);
+    yp = [..."0123456789ABCDEF"],
+    mk = t => yp[t & 15],
+    yk = t => yp[(t & 240) >> 4] + yp[t & 15],
+    Sc = t => (t & 240) >> 4 === (t & 15),
+    vk = t => Sc(t.r) && Sc(t.g) && Sc(t.b) && Sc(t.a);
 
-function xS(t) {
+function xk(t) {
     var e = t.length,
         n;
     return t[0] === "#" && (e === 4 || e === 5 ? n = {
-        r: 255 & Gn[t[1]] * 17,
-        g: 255 & Gn[t[2]] * 17,
-        b: 255 & Gn[t[3]] * 17,
-        a: e === 5 ? Gn[t[4]] * 17 : 255
+        r: 255 & Kn[t[1]] * 17,
+        g: 255 & Kn[t[2]] * 17,
+        b: 255 & Kn[t[3]] * 17,
+        a: e === 5 ? Kn[t[4]] * 17 : 255
     } : (e === 7 || e === 9) && (n = {
-        r: Gn[t[1]] << 4 | Gn[t[2]],
-        g: Gn[t[3]] << 4 | Gn[t[4]],
-        b: Gn[t[5]] << 4 | Gn[t[6]],
-        a: e === 9 ? Gn[t[7]] << 4 | Gn[t[8]] : 255
+        r: Kn[t[1]] << 4 | Kn[t[2]],
+        g: Kn[t[3]] << 4 | Kn[t[4]],
+        b: Kn[t[5]] << 4 | Kn[t[6]],
+        a: e === 9 ? Kn[t[7]] << 4 | Kn[t[8]] : 255
     })), n
 }
-var bS = (t, e) => t < 255 ? e(t) : "";
+var bk = (t, e) => t < 255 ? e(t) : "";
 
-function _S(t) {
-    var e = vS(t) ? mS : yS;
-    return t ? "#" + e(t.r) + e(t.g) + e(t.b) + bS(t.a, e) : void 0
+function _k(t) {
+    var e = vk(t) ? mk : yk;
+    return t ? "#" + e(t.r) + e(t.g) + e(t.b) + bk(t.a, e) : void 0
 }
-var wS = /^(hsla?|hwb|hsv)\(\s*([-+.e\d]+)(?:deg)?[\s,]+([-+.e\d]+)%[\s,]+([-+.e\d]+)%(?:[\s,]+([-+.e\d]+)(%)?)?\s*\)$/;
+var wk = /^(hsla?|hwb|hsv)\(\s*([-+.e\d]+)(?:deg)?[\s,]+([-+.e\d]+)%[\s,]+([-+.e\d]+)%(?:[\s,]+([-+.e\d]+)(%)?)?\s*\)$/;
 
 function lx(t, e, n) {
     let i = e * Math.min(n, 1 - n),
         r = (o, s = (o + t / 30) % 12) => n - i * Math.max(Math.min(s - 3, 9 - s, 1), -1);
     return [r(0), r(8), r(4)]
 }
 
-function kS(t, e, n) {
+function Sk(t, e, n) {
     let i = (r, o = (r + t / 60) % 6) => n - n * e * Math.max(Math.min(o, 4 - o, 1), 0);
     return [i(5), i(3), i(1)]
 }
 
-function SS(t, e, n) {
+function kk(t, e, n) {
     let i = lx(t, 1, .5),
         r;
     for (e + n > 1 && (r = 1 / (e + n), e *= r, n *= r), r = 0; r < 3; r++) i[r] *= 1 - e - n, i[r] += e;
     return i
 }
 
-function CS(t, e, n, i, r) {
+function Ck(t, e, n, i, r) {
     return t === r ? (e - n) / i + (e < n ? 6 : 0) : e === r ? (n - t) / i + 2 : (t - e) / i + 4
 }
 
-function xp(t) {
+function vp(t) {
     let n = t.r / 255,
         i = t.g / 255,
         r = t.b / 255,
         o = Math.max(n, i, r),
         s = Math.min(n, i, r),
         a = (o + s) / 2,
         l, c, d;
-    return o !== s && (d = o - s, c = a > .5 ? d / (2 - o - s) : d / (o + s), l = CS(n, i, r, d, o), l = l * 60 + .5), [l | 0, c || 0, a]
+    return o !== s && (d = o - s, c = a > .5 ? d / (2 - o - s) : d / (o + s), l = Ck(n, i, r, d, o), l = l * 60 + .5), [l | 0, c || 0, a]
 }
 
-function bp(t, e, n, i) {
+function xp(t, e, n, i) {
     return (Array.isArray(e) ? t(e[0], e[1], e[2]) : t(e, n, i)).map(jr)
 }
 
-function _p(t, e, n) {
-    return bp(lx, t, e, n)
+function bp(t, e, n) {
+    return xp(lx, t, e, n)
 }
 
-function ES(t, e, n) {
-    return bp(SS, t, e, n)
+function Ek(t, e, n) {
+    return xp(kk, t, e, n)
 }
 
-function TS(t, e, n) {
-    return bp(kS, t, e, n)
+function Tk(t, e, n) {
+    return xp(Sk, t, e, n)
 }
 
 function ux(t) {
     return (t % 360 + 360) % 360
 }
 
-function PS(t) {
-    let e = wS.exec(t),
+function Dk(t) {
+    let e = wk.exec(t),
         n = 255,
         i;
     if (!e) return;
-    e[5] !== i && (n = e[6] ? ol(+e[5]) : jr(+e[5]));
+    e[5] !== i && (n = e[6] ? sl(+e[5]) : jr(+e[5]));
     let r = ux(+e[2]),
         o = +e[3] / 100,
         s = +e[4] / 100;
-    return e[1] === "hwb" ? i = ES(r, o, s) : e[1] === "hsv" ? i = TS(r, o, s) : i = _p(r, o, s), {
+    return e[1] === "hwb" ? i = Ek(r, o, s) : e[1] === "hsv" ? i = Tk(r, o, s) : i = bp(r, o, s), {
         r: i[0],
         g: i[1],
         b: i[2],
         a: n
     }
 }
 
-function MS(t, e) {
-    var n = xp(t);
-    n[0] = ux(n[0] + e), n = _p(n), t.r = n[0], t.g = n[1], t.b = n[2]
+function Pk(t, e) {
+    var n = vp(t);
+    n[0] = ux(n[0] + e), n = bp(n), t.r = n[0], t.g = n[1], t.b = n[2]
 }
 
-function DS(t) {
+function Mk(t) {
     if (!t) return;
-    let e = xp(t),
+    let e = vp(t),
         n = e[0],
         i = rx(e[1]),
         r = rx(e[2]);
     return t.a < 255 ? `hsla(${n}, ${i}%, ${r}%, ${Ji(t.a)})` : `hsl(${n}, ${i}%, ${r}%)`
 }
 var ox = {
         x: "dark",
@@ -8420,79 +8420,79 @@
         JHt: "f5deb3",
         wEte: "ffffff",
         wEtesmoke: "f5f5f5",
         Lw: "ffff00",
         LwgYF: "9acd32"
     };
 
-function OS() {
+function Ok() {
     let t = {},
         e = Object.keys(sx),
         n = Object.keys(ox),
         i, r, o, s, a;
     for (i = 0; i < e.length; i++) {
         for (s = a = e[i], r = 0; r < n.length; r++) o = n[r], a = a.replace(o, ox[o]);
         o = parseInt(sx[s], 16), t[a] = [o >> 16 & 255, o >> 8 & 255, o & 255]
     }
     return t
 }
 var kc;
 
-function AS(t) {
-    kc || (kc = OS(), kc.transparent = [0, 0, 0, 0]);
+function Ak(t) {
+    kc || (kc = Ok(), kc.transparent = [0, 0, 0, 0]);
     let e = kc[t.toLowerCase()];
     return e && {
         r: e[0],
         g: e[1],
         b: e[2],
         a: e.length === 4 ? e[3] : 255
     }
 }
-var LS = /^rgba?\(\s*([-+.\d]+)(%)?[\s,]+([-+.e\d]+)(%)?[\s,]+([-+.e\d]+)(%)?(?:[\s,/]+([-+.e\d]+)(%)?)?\s*\)$/;
+var Lk = /^rgba?\(\s*([-+.\d]+)(%)?[\s,]+([-+.e\d]+)(%)?[\s,]+([-+.e\d]+)(%)?(?:[\s,/]+([-+.e\d]+)(%)?)?\s*\)$/;
 
-function RS(t) {
-    let e = LS.exec(t),
+function Rk(t) {
+    let e = Lk.exec(t),
         n = 255,
         i, r, o;
     if (e) {
         if (e[7] !== i) {
             let s = +e[7];
-            n = e[8] ? ol(s) : Fr(s * 255, 0, 255)
+            n = e[8] ? sl(s) : Fr(s * 255, 0, 255)
         }
-        return i = +e[1], r = +e[3], o = +e[5], i = 255 & (e[2] ? ol(i) : Fr(i, 0, 255)), r = 255 & (e[4] ? ol(r) : Fr(r, 0, 255)), o = 255 & (e[6] ? ol(o) : Fr(o, 0, 255)), {
+        return i = +e[1], r = +e[3], o = +e[5], i = 255 & (e[2] ? sl(i) : Fr(i, 0, 255)), r = 255 & (e[4] ? sl(r) : Fr(r, 0, 255)), o = 255 & (e[6] ? sl(o) : Fr(o, 0, 255)), {
             r: i,
             g: r,
             b: o,
             a: n
         }
     }
 }
 
-function IS(t) {
+function Ik(t) {
     return t && (t.a < 255 ? `rgba(${t.r}, ${t.g}, ${t.b}, ${Ji(t.a)})` : `rgb(${t.r}, ${t.g}, ${t.b})`)
 }
-var yp = t => t <= .0031308 ? t * 12.92 : Math.pow(t, 1 / 2.4) * 1.055 - .055,
-    Ds = t => t <= .04045 ? t / 12.92 : Math.pow((t + .055) / 1.055, 2.4);
+var mp = t => t <= .0031308 ? t * 12.92 : Math.pow(t, 1 / 2.4) * 1.055 - .055,
+    Ms = t => t <= .04045 ? t / 12.92 : Math.pow((t + .055) / 1.055, 2.4);
 
-function NS(t, e, n) {
-    let i = Ds(Ji(t.r)),
-        r = Ds(Ji(t.g)),
-        o = Ds(Ji(t.b));
+function Nk(t, e, n) {
+    let i = Ms(Ji(t.r)),
+        r = Ms(Ji(t.g)),
+        o = Ms(Ji(t.b));
     return {
-        r: jr(yp(i + n * (Ds(Ji(e.r)) - i))),
-        g: jr(yp(r + n * (Ds(Ji(e.g)) - r))),
-        b: jr(yp(o + n * (Ds(Ji(e.b)) - o))),
+        r: jr(mp(i + n * (Ms(Ji(e.r)) - i))),
+        g: jr(mp(r + n * (Ms(Ji(e.g)) - r))),
+        b: jr(mp(o + n * (Ms(Ji(e.b)) - o))),
         a: t.a + n * (e.a - t.a)
     }
 }
 
-function Sc(t, e, n) {
+function Cc(t, e, n) {
     if (t) {
-        let i = xp(t);
-        i[e] = Math.max(0, Math.min(i[e] + i[e] * n, e === 0 ? 360 : 1)), i = _p(i), t.r = i[0], t.g = i[1], t.b = i[2]
+        let i = vp(t);
+        i[e] = Math.max(0, Math.min(i[e] + i[e] * n, e === 0 ? 360 : 1)), i = bp(i), t.r = i[0], t.g = i[1], t.b = i[2]
     }
 }
 
 function cx(t, e) {
     return t && Object.assign(e || {}, t)
 }
 
@@ -8512,95 +8512,95 @@
         r: 0,
         g: 0,
         b: 0,
         a: 1
     }), e.a = jr(e.a)), e
 }
 
-function zS(t) {
-    return t.charAt(0) === "r" ? RS(t) : PS(t)
+function zk(t) {
+    return t.charAt(0) === "r" ? Rk(t) : Dk(t)
 }
-var sl = class t {
+var al = class t {
     constructor(e) {
         if (e instanceof t) return e;
         let n = typeof e,
             i;
-        n === "object" ? i = ax(e) : n === "string" && (i = xS(e) || AS(e) || zS(e)), this._rgb = i, this._valid = !!i
+        n === "object" ? i = ax(e) : n === "string" && (i = xk(e) || Ak(e) || zk(e)), this._rgb = i, this._valid = !!i
     }
     get valid() {
         return this._valid
     }
     get rgb() {
         var e = cx(this._rgb);
         return e && (e.a = Ji(e.a)), e
     }
     set rgb(e) {
         this._rgb = ax(e)
     }
     rgbString() {
-        return this._valid ? IS(this._rgb) : void 0
+        return this._valid ? Ik(this._rgb) : void 0
     }
     hexString() {
-        return this._valid ? _S(this._rgb) : void 0
+        return this._valid ? _k(this._rgb) : void 0
     }
     hslString() {
-        return this._valid ? DS(this._rgb) : void 0
+        return this._valid ? Mk(this._rgb) : void 0
     }
     mix(e, n) {
         if (e) {
             let i = this.rgb,
                 r = e.rgb,
                 o, s = n === o ? .5 : n,
                 a = 2 * s - 1,
                 l = i.a - r.a,
                 c = ((a * l === -1 ? a : (a + l) / (1 + a * l)) + 1) / 2;
             o = 1 - c, i.r = 255 & c * i.r + o * r.r + .5, i.g = 255 & c * i.g + o * r.g + .5, i.b = 255 & c * i.b + o * r.b + .5, i.a = s * i.a + (1 - s) * r.a, this.rgb = i
         }
         return this
     }
     interpolate(e, n) {
-        return e && (this._rgb = NS(this._rgb, e._rgb, n)), this
+        return e && (this._rgb = Nk(this._rgb, e._rgb, n)), this
     }
     clone() {
         return new t(this.rgb)
     }
     alpha(e) {
         return this._rgb.a = jr(e), this
     }
     clearer(e) {
         let n = this._rgb;
         return n.a *= 1 - e, this
     }
     greyscale() {
         let e = this._rgb,
-            n = al(e.r * .3 + e.g * .59 + e.b * .11);
+            n = ll(e.r * .3 + e.g * .59 + e.b * .11);
         return e.r = e.g = e.b = n, this
     }
     opaquer(e) {
         let n = this._rgb;
         return n.a *= 1 + e, this
     }
     negate() {
         let e = this._rgb;
         return e.r = 255 - e.r, e.g = 255 - e.g, e.b = 255 - e.b, this
     }
     lighten(e) {
-        return Sc(this._rgb, 2, e), this
+        return Cc(this._rgb, 2, e), this
     }
     darken(e) {
-        return Sc(this._rgb, 2, -e), this
+        return Cc(this._rgb, 2, -e), this
     }
     saturate(e) {
-        return Sc(this._rgb, 1, e), this
+        return Cc(this._rgb, 1, e), this
     }
     desaturate(e) {
-        return Sc(this._rgb, 1, -e), this
+        return Cc(this._rgb, 1, -e), this
     }
     rotate(e) {
-        return MS(this._rgb, e), this
+        return Pk(this._rgb, e), this
     }
 };
 
 function fi() {}
 var Sp = (() => {
     let t = 0;
     return () => t++
@@ -8627,22 +8627,22 @@
 function an(t, e) {
     return qe(t) ? t : e
 }
 
 function pe(t, e) {
     return typeof t > "u" ? e : t
 }
-var Cp = (t, e) => typeof t == "string" && t.endsWith("%") ? parseFloat(t) / 100 : +t / e,
-    Dc = (t, e) => typeof t == "string" && t.endsWith("%") ? parseFloat(t) / 100 * e : +t;
+var kp = (t, e) => typeof t == "string" && t.endsWith("%") ? parseFloat(t) / 100 : +t / e,
+    Oc = (t, e) => typeof t == "string" && t.endsWith("%") ? parseFloat(t) / 100 * e : +t;
 
 function ve(t, e, n) {
     if (t && typeof t.call == "function") return t.apply(n, e)
 }
 
-function Se(t, e, n, i) {
+function ke(t, e, n, i) {
     let r, o, s;
     if (Re(t))
         if (o = t.length, i)
             for (r = o - 1; r >= 0; r--) e.call(n, t[r], r);
         else
             for (r = 0; r < o; r++) e.call(n, t[r], r);
     else if (we(t))
@@ -8653,171 +8653,171 @@
     let n, i, r, o;
     if (!t || !e || t.length !== e.length) return !1;
     for (n = 0, i = t.length; n < i; ++n)
         if (r = t[n], o = e[n], r.datasetIndex !== o.datasetIndex || r.index !== o.index) return !1;
     return !0
 }
 
-function ul(t) {
-    if (Re(t)) return t.map(ul);
+function cl(t) {
+    if (Re(t)) return t.map(cl);
     if (we(t)) {
         let e = Object.create(null),
             n = Object.keys(t),
             i = n.length,
             r = 0;
-        for (; r < i; ++r) e[n[r]] = ul(t[n[r]]);
+        for (; r < i; ++r) e[n[r]] = cl(t[n[r]]);
         return e
     }
     return t
 }
 
 function bx(t) {
     return ["__proto__", "prototype", "constructor"].indexOf(t) === -1
 }
 
 function _x(t, e, n, i) {
     if (!bx(t)) return;
     let r = e[t],
         o = n[t];
-    we(r) && we(o) ? Mo(r, o, i) : e[t] = ul(o)
+    we(r) && we(o) ? Po(r, o, i) : e[t] = cl(o)
 }
 
-function Mo(t, e, n) {
+function Po(t, e, n) {
     let i = Re(e) ? e : [e],
         r = i.length;
     if (!we(t)) return t;
     n = n || {};
     let o = n.merger || _x,
         s;
     for (let a = 0; a < r; ++a) {
         if (s = i[a], !we(s)) continue;
         let l = Object.keys(s);
         for (let c = 0, d = l.length; c < d; ++c) o(l[c], t, s, n)
     }
     return t
 }
 
-function Do(t, e) {
-    return Mo(t, e, {
+function Mo(t, e) {
+    return Po(t, e, {
         merger: wx
     })
 }
 
 function wx(t, e, n) {
     if (!bx(t)) return;
     let i = e[t],
         r = n[t];
-    we(i) && we(r) ? Do(i, r) : Object.prototype.hasOwnProperty.call(e, t) || (e[t] = ul(r))
+    we(i) && we(r) ? Mo(i, r) : Object.prototype.hasOwnProperty.call(e, t) || (e[t] = cl(r))
 }
 var fx = {
     "": t => t,
     x: t => t.x,
     y: t => t.y
 };
 
-function kx(t) {
+function Sx(t) {
     let e = t.split("."),
         n = [],
         i = "";
     for (let r of e) i += r, i.endsWith("\\") ? i = i.slice(0, -1) + "." : (n.push(i), i = "");
     return n
 }
 
-function FS(t) {
-    let e = kx(t);
+function Fk(t) {
+    let e = Sx(t);
     return n => {
         for (let i of e) {
             if (i === "") break;
             n = n && n[i]
         }
         return n
     }
 }
 
 function Ci(t, e) {
-    return (fx[e] || (fx[e] = FS(e)))(t)
+    return (fx[e] || (fx[e] = Fk(e)))(t)
 }
 
-function fl(t) {
+function dl(t) {
     return t.charAt(0).toUpperCase() + t.slice(1)
 }
 var Ut = t => typeof t < "u",
     Vt = t => typeof t == "function",
-    Oc = (t, e) => {
+    Ac = (t, e) => {
         if (t.size !== e.size) return !1;
         for (let n of t)
             if (!e.has(n)) return !1;
         return !0
     };
 
-function Ep(t) {
+function Cp(t) {
     return t.type === "mouseup" || t.type === "click" || t.type === "contextmenu"
 }
 var Ce = Math.PI,
     We = 2 * Ce,
-    Sx = We + Ce,
-    cl = Number.POSITIVE_INFINITY,
-    dl = Ce / 180,
+    kx = We + Ce,
+    fl = Number.POSITIVE_INFINITY,
+    hl = Ce / 180,
     $e = Ce / 2,
     bn = Ce / 4,
     Os = Ce * 2 / 3,
-    Si = Math.log10,
+    ki = Math.log10,
     sn = Math.sign;
 
 function Oo(t, e, n) {
     return Math.abs(t - e) < n
 }
 
-function Ac(t) {
+function Lc(t) {
     let e = Math.round(t);
     t = Oo(t, e, t / 1e3) ? e : t;
-    let n = Math.pow(10, Math.floor(Si(t))),
+    let n = Math.pow(10, Math.floor(ki(t))),
         i = t / n;
     return (i <= 1 ? 1 : i <= 2 ? 2 : i <= 5 ? 5 : 10) * n
 }
 
-function Tp(t) {
+function Ep(t) {
     let e = [],
         n = Math.sqrt(t),
         i;
     for (i = 1; i < n; i++) t % i === 0 && (e.push(i), e.push(t / i));
     return n === (n | 0) && e.push(n), e.sort((r, o) => r - o).pop(), e
 }
 
 function di(t) {
     return !isNaN(parseFloat(t)) && isFinite(t)
 }
 
-function Pp(t, e) {
+function Tp(t, e) {
     let n = Math.round(t);
     return n - e <= t && n + e >= t
 }
 
-function Lc(t, e, n) {
+function Rc(t, e, n) {
     let i, r, o;
     for (i = 0, r = t.length; i < r; i++) o = t[i][n], isNaN(o) || (e.min = Math.min(e.min, o), e.max = Math.max(e.max, o))
 }
 
 function pt(t) {
     return t * (Ce / 180)
 }
 
 function Ao(t) {
     return t * (180 / Ce)
 }
 
-function Rc(t) {
+function Ic(t) {
     if (!qe(t)) return;
     let e = 1,
         n = 0;
     for (; Math.round(t * e) / e !== t;) e *= 10, n++;
     return n
 }
 
-function Ic(t, e) {
+function Nc(t, e) {
     let n = e.x - t.x,
         i = e.y - t.y,
         r = Math.sqrt(n * n + i * i),
         o = Math.atan2(i, n);
     return o < -.5 * Ce && (o += We), {
         angle: o,
         distance: r
@@ -8825,15 +8825,15 @@
 }
 
 function tr(t, e) {
     return Math.sqrt(Math.pow(e.x - t.x, 2) + Math.pow(e.y - t.y, 2))
 }
 
 function Cx(t, e) {
-    return (t - e + Sx) % We - Ce
+    return (t - e + kx) % We - Ce
 }
 
 function on(t) {
     return (t % We + We) % We
 }
 
 function Lo(t, e, n, i) {
@@ -8843,157 +8843,157 @@
         a = on(o - r),
         l = on(s - r),
         c = on(r - o),
         d = on(r - s);
     return r === o || r === s || i && o === s || a > l && c < d
 }
 
-function St(t, e, n) {
+function kt(t, e, n) {
     return Math.max(e, Math.min(n, t))
 }
 
-function Mp(t) {
-    return St(t, -32768, 32767)
+function Dp(t) {
+    return kt(t, -32768, 32767)
 }
 
 function hi(t, e, n, i = 1e-6) {
     return t >= Math.min(e, n) - i && t <= Math.max(e, n) + i
 }
 
-function hl(t, e, n) {
+function pl(t, e, n) {
     n = n || (s => t[s] < e);
     let i = t.length - 1,
         r = 0,
         o;
     for (; i - r > 1;) o = r + i >> 1, n(o) ? r = o : i = o;
     return {
         lo: r,
         hi: i
     }
 }
-var ui = (t, e, n, i) => hl(t, n, i ? r => {
+var ui = (t, e, n, i) => pl(t, n, i ? r => {
         let o = t[r][e];
         return o < n || o === n && t[r + 1][e] === n
     } : r => t[r][e] < n),
-    Dp = (t, e, n) => hl(t, n, i => t[i][e] >= n);
+    Pp = (t, e, n) => pl(t, n, i => t[i][e] >= n);
 
-function Op(t, e, n) {
+function Mp(t, e, n) {
     let i = 0,
         r = t.length;
     for (; i < r && t[i] < e;) i++;
     for (; r > i && t[r - 1] > n;) r--;
     return i > 0 || r < t.length ? t.slice(i, r) : t
 }
 var Ex = ["push", "pop", "shift", "splice", "unshift"];
 
-function Ap(t, e) {
+function Op(t, e) {
     if (t._chartjs) {
         t._chartjs.listeners.push(e);
         return
     }
     Object.defineProperty(t, "_chartjs", {
         configurable: !0,
         enumerable: !1,
         value: {
             listeners: [e]
         }
     }), Ex.forEach(n => {
-        let i = "_onData" + fl(n),
+        let i = "_onData" + dl(n),
             r = t[n];
         Object.defineProperty(t, n, {
             configurable: !0,
             enumerable: !1,
             value(...o) {
                 let s = r.apply(this, o);
                 return t._chartjs.listeners.forEach(a => {
                     typeof a[i] == "function" && a[i](...o)
                 }), s
             }
         })
     })
 }
 
-function Nc(t, e) {
+function zc(t, e) {
     let n = t._chartjs;
     if (!n) return;
     let i = n.listeners,
         r = i.indexOf(e);
     r !== -1 && i.splice(r, 1), !(i.length > 0) && (Ex.forEach(o => {
         delete t[o]
     }), delete t._chartjs)
 }
 
-function zc(t) {
+function Fc(t) {
     let e = new Set(t);
     return e.size === t.length ? t : Array.from(e)
 }
-var Fc = function() {
+var jc = function() {
     return typeof window > "u" ? function(t) {
         return t()
     } : window.requestAnimationFrame
 }();
 
-function jc(t, e) {
+function Hc(t, e) {
     let n = [],
         i = !1;
     return function(...r) {
-        n = r, i || (i = !0, Fc.call(window, () => {
+        n = r, i || (i = !0, jc.call(window, () => {
             i = !1, t.apply(e, n)
         }))
     }
 }
 
-function Lp(t, e) {
+function Ap(t, e) {
     let n;
     return function(...i) {
         return e ? (clearTimeout(n), n = setTimeout(t, e, i)) : t.apply(this, i), e
     }
 }
-var pl = t => t === "start" ? "left" : t === "end" ? "right" : "center",
+var gl = t => t === "start" ? "left" : t === "end" ? "right" : "center",
     Nt = (t, e, n) => t === "start" ? e : t === "end" ? n : (e + n) / 2,
-    Rp = (t, e, n, i) => t === (i ? "left" : "right") ? n : t === "center" ? (e + n) / 2 : e;
+    Lp = (t, e, n, i) => t === (i ? "left" : "right") ? n : t === "center" ? (e + n) / 2 : e;
 
-function Hc(t, e, n) {
+function Bc(t, e, n) {
     let i = e.length,
         r = 0,
         o = i;
     if (t._sorted) {
         let {
             iScale: s,
             _parsed: a
         } = t, l = s.axis, {
             min: c,
             max: d,
             minDefined: g,
             maxDefined: y
         } = s.getUserBounds();
-        g && (r = St(Math.min(ui(a, l, c).lo, n ? i : ui(e, l, s.getPixelForValue(c)).lo), 0, i - 1)), y ? o = St(Math.max(ui(a, s.axis, d, !0).hi + 1, n ? 0 : ui(e, l, s.getPixelForValue(d), !0).hi + 1), r, i) - r : o = i - r
+        g && (r = kt(Math.min(ui(a, l, c).lo, n ? i : ui(e, l, s.getPixelForValue(c)).lo), 0, i - 1)), y ? o = kt(Math.max(ui(a, s.axis, d, !0).hi + 1, n ? 0 : ui(e, l, s.getPixelForValue(d), !0).hi + 1), r, i) - r : o = i - r
     }
     return {
         start: r,
         count: o
     }
 }
 
-function Bc(t) {
+function Wc(t) {
     let {
         xScale: e,
         yScale: n,
         _scaleRanges: i
     } = t, r = {
         xmin: e.min,
         xmax: e.max,
         ymin: n.min,
         ymax: n.max
     };
     if (!i) return t._scaleRanges = r, !0;
     let o = i.xmin !== e.min || i.xmax !== e.max || i.ymin !== n.min || i.ymax !== n.max;
     return Object.assign(i, r), o
 }
-var Cc = t => t === 0 || t === 1,
+var Ec = t => t === 0 || t === 1,
     dx = (t, e, n) => -(Math.pow(2, 10 * (t -= 1)) * Math.sin((t - e) * We / n)),
     hx = (t, e, n) => Math.pow(2, -10 * t) * Math.sin((t - e) * We / n) + 1,
     To = {
         linear: t => t,
         easeInQuad: t => t * t,
         easeOutQuad: t => -t * (t - 2),
         easeInOutQuad: t => (t /= .5) < 1 ? .5 * t * t : -.5 * (--t * (t - 2) - 1),
@@ -9007,22 +9007,22 @@
         easeOutQuint: t => (t -= 1) * t * t * t * t + 1,
         easeInOutQuint: t => (t /= .5) < 1 ? .5 * t * t * t * t * t : .5 * ((t -= 2) * t * t * t * t + 2),
         easeInSine: t => -Math.cos(t * $e) + 1,
         easeOutSine: t => Math.sin(t * $e),
         easeInOutSine: t => -.5 * (Math.cos(Ce * t) - 1),
         easeInExpo: t => t === 0 ? 0 : Math.pow(2, 10 * (t - 1)),
         easeOutExpo: t => t === 1 ? 1 : -Math.pow(2, -10 * t) + 1,
-        easeInOutExpo: t => Cc(t) ? t : t < .5 ? .5 * Math.pow(2, 10 * (t * 2 - 1)) : .5 * (-Math.pow(2, -10 * (t * 2 - 1)) + 2),
+        easeInOutExpo: t => Ec(t) ? t : t < .5 ? .5 * Math.pow(2, 10 * (t * 2 - 1)) : .5 * (-Math.pow(2, -10 * (t * 2 - 1)) + 2),
         easeInCirc: t => t >= 1 ? t : -(Math.sqrt(1 - t * t) - 1),
         easeOutCirc: t => Math.sqrt(1 - (t -= 1) * t),
         easeInOutCirc: t => (t /= .5) < 1 ? -.5 * (Math.sqrt(1 - t * t) - 1) : .5 * (Math.sqrt(1 - (t -= 2) * t) + 1),
-        easeInElastic: t => Cc(t) ? t : dx(t, .075, .3),
-        easeOutElastic: t => Cc(t) ? t : hx(t, .075, .3),
+        easeInElastic: t => Ec(t) ? t : dx(t, .075, .3),
+        easeOutElastic: t => Ec(t) ? t : hx(t, .075, .3),
         easeInOutElastic(t) {
-            return Cc(t) ? t : t < .5 ? .5 * dx(t * 2, .1125, .45) : .5 + .5 * hx(t * 2 - 1, .1125, .45)
+            return Ec(t) ? t : t < .5 ? .5 * dx(t * 2, .1125, .45) : .5 + .5 * hx(t * 2 - 1, .1125, .45)
         },
         easeInBack(t) {
             return t * t * ((1.70158 + 1) * t - 1.70158)
         },
         easeOutBack(t) {
             return (t -= 1) * t * ((1.70158 + 1) * t + 1.70158) + 1
         },
@@ -9033,33 +9033,33 @@
         easeInBounce: t => 1 - To.easeOutBounce(1 - t),
         easeOutBounce(t) {
             return t < 1 / 2.75 ? 7.5625 * t * t : t < 2 / 2.75 ? 7.5625 * (t -= 1.5 / 2.75) * t + .75 : t < 2.5 / 2.75 ? 7.5625 * (t -= 2.25 / 2.75) * t + .9375 : 7.5625 * (t -= 2.625 / 2.75) * t + .984375
         },
         easeInOutBounce: t => t < .5 ? To.easeInBounce(t * 2) * .5 : To.easeOutBounce(t * 2 - 1) * .5 + .5
     };
 
-function Wc(t) {
+function Vc(t) {
     if (t && typeof t == "object") {
         let e = t.toString();
         return e === "[object CanvasPattern]" || e === "[object CanvasGradient]"
     }
     return !1
 }
 
-function Vc(t) {
-    return Wc(t) ? t : new sl(t)
+function Uc(t) {
+    return Vc(t) ? t : new al(t)
 }
 
 function Pc(t) {
-    return Wc(t) ? t : new sl(t).saturate(.5).darken(.1).hexString()
+    return Vc(t) ? t : new al(t).saturate(.5).darken(.1).hexString()
 }
-var jS = ["x", "y", "borderWidth", "radius", "tension"],
-    HS = ["color", "borderColor", "backgroundColor"];
+var jk = ["x", "y", "borderWidth", "radius", "tension"],
+    Hk = ["color", "borderColor", "backgroundColor"];
 
-function BS(t) {
+function Bk(t) {
     t.set("animation", {
         delay: void 0,
         duration: 1e3,
         easing: "easeOutQuart",
         fn: void 0,
         from: void 0,
         loop: void 0,
@@ -9068,19 +9068,19 @@
     }), t.describe("animation", {
         _fallback: !1,
         _indexable: !1,
         _scriptable: e => e !== "onProgress" && e !== "onComplete" && e !== "fn"
     }), t.set("animations", {
         colors: {
             type: "color",
-            properties: HS
+            properties: Hk
         },
         numbers: {
             type: "number",
-            properties: jS
+            properties: jk
         }
     }), t.describe("animations", {
         _fallback: "animation"
     }), t.set("transitions", {
         active: {
             animation: {
                 duration: 400
@@ -9113,74 +9113,74 @@
                     fn: e => e | 0
                 }
             }
         }
     })
 }
 
-function WS(t) {
+function Wk(t) {
     t.set("layout", {
         autoPadding: !0,
         padding: {
             top: 0,
             right: 0,
             bottom: 0,
             left: 0
         }
     })
 }
 var px = new Map;
 
-function VS(t, e) {
+function Vk(t, e) {
     e = e || {};
     let n = t + JSON.stringify(e),
         i = px.get(n);
     return i || (i = new Intl.NumberFormat(t, e), px.set(n, i)), i
 }
 
 function Ro(t, e, n) {
-    return VS(e, n).format(t)
+    return Vk(e, n).format(t)
 }
 var Tx = {
     values(t) {
         return Re(t) ? t : "" + t
     },
     numeric(t, e, n) {
         if (t === 0) return "0";
         let i = this.chart.options.locale,
             r, o = t;
         if (n.length > 1) {
             let c = Math.max(Math.abs(n[0].value), Math.abs(n[n.length - 1].value));
-            (c < 1e-4 || c > 1e15) && (r = "scientific"), o = US(t, n)
+            (c < 1e-4 || c > 1e15) && (r = "scientific"), o = Uk(t, n)
         }
-        let s = Si(Math.abs(o)),
+        let s = ki(Math.abs(o)),
             a = isNaN(s) ? 1 : Math.max(Math.min(-1 * Math.floor(s), 20), 0),
             l = {
                 notation: r,
                 minimumFractionDigits: a,
                 maximumFractionDigits: a
             };
         return Object.assign(l, this.options.ticks.format), Ro(t, i, l)
     },
     logarithmic(t, e, n) {
         if (t === 0) return "0";
-        let i = n[e].significand || t / Math.pow(10, Math.floor(Si(t)));
+        let i = n[e].significand || t / Math.pow(10, Math.floor(ki(t)));
         return [1, 2, 3, 5, 10, 15].includes(i) || e > .8 * n.length ? Tx.numeric.call(this, t, e, n) : ""
     }
 };
 
-function US(t, e) {
+function Uk(t, e) {
     let n = e.length > 3 ? e[2].value - e[1].value : e[1].value - e[0].value;
     return Math.abs(n) >= 1 && t !== Math.floor(t) && (n = t - Math.floor(t)), n
 }
-var gl = {
+var ml = {
     formatters: Tx
 };
 
-function $S(t) {
+function $k(t) {
     t.set("scale", {
         display: !0,
         offset: !1,
         reverse: !1,
         beginAtZero: !1,
         bounds: "ticks",
         clip: !0,
@@ -9216,15 +9216,15 @@
             textStrokeWidth: 0,
             textStrokeColor: "",
             padding: 3,
             display: !0,
             autoSkip: !0,
             autoSkipPadding: 3,
             labelOffset: 0,
-            callback: gl.formatters.values,
+            callback: ml.formatters.values,
             minor: {},
             major: {},
             align: "center",
             crossAlign: "near",
             showLabelBackdrop: !1,
             backdropColor: "rgba(255, 255, 255, 0.75)",
             backdropPadding: 2
@@ -9237,58 +9237,58 @@
         _fallback: "scale"
     }), t.describe("scale.ticks", {
         _scriptable: e => e !== "backdropPadding" && e !== "callback",
         _indexable: e => e !== "backdropPadding"
     })
 }
 var Br = Object.create(null),
-    Uc = Object.create(null);
+    $c = Object.create(null);
 
-function ll(t, e) {
+function ul(t, e) {
     if (!e) return t;
     let n = e.split(".");
     for (let i = 0, r = n.length; i < r; ++i) {
         let o = n[i];
         t = t[o] || (t[o] = Object.create(null))
     }
     return t
 }
 
-function wp(t, e, n) {
-    return typeof e == "string" ? Mo(ll(t, e), n) : Mo(ll(t, ""), e)
+function _p(t, e, n) {
+    return typeof e == "string" ? Po(ul(t, e), n) : Po(ul(t, ""), e)
 }
-var kp = class {
+var wp = class {
         constructor(e, n) {
             this.animation = void 0, this.backgroundColor = "rgba(0,0,0,0.1)", this.borderColor = "rgba(0,0,0,0.1)", this.color = "#666", this.datasets = {}, this.devicePixelRatio = i => i.chart.platform.getDevicePixelRatio(), this.elements = {}, this.events = ["mousemove", "mouseout", "click", "touchstart", "touchmove"], this.font = {
                 family: "'Helvetica Neue', 'Helvetica', 'Arial', sans-serif",
                 size: 12,
                 style: "normal",
                 lineHeight: 1.2,
                 weight: null
             }, this.hover = {}, this.hoverBackgroundColor = (i, r) => Pc(r.backgroundColor), this.hoverBorderColor = (i, r) => Pc(r.borderColor), this.hoverColor = (i, r) => Pc(r.color), this.indexAxis = "x", this.interaction = {
                 mode: "nearest",
                 intersect: !0,
                 includeInvisible: !1
             }, this.maintainAspectRatio = !0, this.onHover = null, this.onClick = null, this.parsing = !0, this.plugins = {}, this.responsive = !0, this.scale = void 0, this.scales = {}, this.showLine = !0, this.drawActiveElementsOnTop = !0, this.describe(e), this.apply(n)
         }
         set(e, n) {
-            return wp(this, e, n)
+            return _p(this, e, n)
         }
         get(e) {
-            return ll(this, e)
+            return ul(this, e)
         }
         describe(e, n) {
-            return wp(Uc, e, n)
+            return _p($c, e, n)
         }
         override(e, n) {
-            return wp(Br, e, n)
+            return _p(Br, e, n)
         }
         route(e, n, i, r) {
-            let o = ll(this, e),
-                s = ll(this, i),
+            let o = ul(this, e),
+                s = ul(this, i),
                 a = "_" + n;
             Object.defineProperties(o, {
                 [a]: {
                     value: o[n],
                     writable: !0
                 },
                 [n]: {
@@ -9304,36 +9304,36 @@
                 }
             })
         }
         apply(e) {
             e.forEach(n => n(this))
         }
     },
-    rt = new kp({
+    rt = new wp({
         _scriptable: t => !t.startsWith("on"),
         _indexable: t => t !== "events",
         hover: {
             _fallback: "interaction"
         },
         interaction: {
             _scriptable: !1,
             _indexable: !1
         }
-    }, [BS, WS, $S]);
+    }, [Bk, Wk, $k]);
 
-function Px(t) {
+function Dx(t) {
     return !t || Ie(t.size) || Ie(t.family) ? null : (t.style ? t.style + " " : "") + (t.weight ? t.weight + " " : "") + t.size + "px " + t.family
 }
 
 function As(t, e, n, i, r) {
     let o = e[r];
     return o || (o = e[r] = t.measureText(r).width, n.push(r)), o > i && (i = o), i
 }
 
-function Ip(t, e, n, i) {
+function Rp(t, e, n, i) {
     i = i || {};
     let r = i.data = i.data || {},
         o = i.garbageCollect = i.garbageCollect || [];
     i.font !== e && (r = i.data = {}, o = i.garbageCollect = [], i.font = e), t.save(), t.font = e;
     let s = 0,
         a = n.length,
         l, c, d, g, y;
@@ -9352,64 +9352,64 @@
 
 function nr(t, e, n) {
     let i = t.currentDevicePixelRatio,
         r = n !== 0 ? Math.max(n / 2, .5) : 0;
     return Math.round((e - r) * i) / i + r
 }
 
-function $c(t, e) {
+function Yc(t, e) {
     e = e || t.getContext("2d"), e.save(), e.resetTransform(), e.clearRect(0, 0, t.width, t.height), e.restore()
 }
 
-function ml(t, e, n, i) {
-    Yc(t, e, n, i, null)
+function yl(t, e, n, i) {
+    Xc(t, e, n, i, null)
 }
 
-function Yc(t, e, n, i, r) {
+function Xc(t, e, n, i, r) {
     let o, s, a, l, c, d, g, y, x = e.pointStyle,
-        w = e.rotation,
-        S = e.radius,
-        A = (w || 0) * dl;
+        _ = e.rotation,
+        C = e.radius,
+        A = (_ || 0) * hl;
     if (x && typeof x == "object" && (o = x.toString(), o === "[object HTMLImageElement]" || o === "[object HTMLCanvasElement]")) {
         t.save(), t.translate(n, i), t.rotate(A), t.drawImage(x, -x.width / 2, -x.height / 2, x.width, x.height), t.restore();
         return
     }
-    if (!(isNaN(S) || S <= 0)) {
+    if (!(isNaN(C) || C <= 0)) {
         switch (t.beginPath(), x) {
             default:
-                r ? t.ellipse(n, i, r / 2, S, 0, 0, We) : t.arc(n, i, S, 0, We), t.closePath();
+                r ? t.ellipse(n, i, r / 2, C, 0, 0, We) : t.arc(n, i, C, 0, We), t.closePath();
                 break;
             case "triangle":
-                d = r ? r / 2 : S, t.moveTo(n + Math.sin(A) * d, i - Math.cos(A) * S), A += Os, t.lineTo(n + Math.sin(A) * d, i - Math.cos(A) * S), A += Os, t.lineTo(n + Math.sin(A) * d, i - Math.cos(A) * S), t.closePath();
+                d = r ? r / 2 : C, t.moveTo(n + Math.sin(A) * d, i - Math.cos(A) * C), A += Os, t.lineTo(n + Math.sin(A) * d, i - Math.cos(A) * C), A += Os, t.lineTo(n + Math.sin(A) * d, i - Math.cos(A) * C), t.closePath();
                 break;
             case "rectRounded":
-                c = S * .516, l = S - c, s = Math.cos(A + bn) * l, g = Math.cos(A + bn) * (r ? r / 2 - c : l), a = Math.sin(A + bn) * l, y = Math.sin(A + bn) * (r ? r / 2 - c : l), t.arc(n - g, i - a, c, A - Ce, A - $e), t.arc(n + y, i - s, c, A - $e, A), t.arc(n + g, i + a, c, A, A + $e), t.arc(n - y, i + s, c, A + $e, A + Ce), t.closePath();
+                c = C * .516, l = C - c, s = Math.cos(A + bn) * l, g = Math.cos(A + bn) * (r ? r / 2 - c : l), a = Math.sin(A + bn) * l, y = Math.sin(A + bn) * (r ? r / 2 - c : l), t.arc(n - g, i - a, c, A - Ce, A - $e), t.arc(n + y, i - s, c, A - $e, A), t.arc(n + g, i + a, c, A, A + $e), t.arc(n - y, i + s, c, A + $e, A + Ce), t.closePath();
                 break;
             case "rect":
-                if (!w) {
-                    l = Math.SQRT1_2 * S, d = r ? r / 2 : l, t.rect(n - d, i - l, 2 * d, 2 * l);
+                if (!_) {
+                    l = Math.SQRT1_2 * C, d = r ? r / 2 : l, t.rect(n - d, i - l, 2 * d, 2 * l);
                     break
                 }
                 A += bn;
             case "rectRot":
-                g = Math.cos(A) * (r ? r / 2 : S), s = Math.cos(A) * S, a = Math.sin(A) * S, y = Math.sin(A) * (r ? r / 2 : S), t.moveTo(n - g, i - a), t.lineTo(n + y, i - s), t.lineTo(n + g, i + a), t.lineTo(n - y, i + s), t.closePath();
+                g = Math.cos(A) * (r ? r / 2 : C), s = Math.cos(A) * C, a = Math.sin(A) * C, y = Math.sin(A) * (r ? r / 2 : C), t.moveTo(n - g, i - a), t.lineTo(n + y, i - s), t.lineTo(n + g, i + a), t.lineTo(n - y, i + s), t.closePath();
                 break;
             case "crossRot":
                 A += bn;
             case "cross":
-                g = Math.cos(A) * (r ? r / 2 : S), s = Math.cos(A) * S, a = Math.sin(A) * S, y = Math.sin(A) * (r ? r / 2 : S), t.moveTo(n - g, i - a), t.lineTo(n + g, i + a), t.moveTo(n + y, i - s), t.lineTo(n - y, i + s);
+                g = Math.cos(A) * (r ? r / 2 : C), s = Math.cos(A) * C, a = Math.sin(A) * C, y = Math.sin(A) * (r ? r / 2 : C), t.moveTo(n - g, i - a), t.lineTo(n + g, i + a), t.moveTo(n + y, i - s), t.lineTo(n - y, i + s);
                 break;
             case "star":
-                g = Math.cos(A) * (r ? r / 2 : S), s = Math.cos(A) * S, a = Math.sin(A) * S, y = Math.sin(A) * (r ? r / 2 : S), t.moveTo(n - g, i - a), t.lineTo(n + g, i + a), t.moveTo(n + y, i - s), t.lineTo(n - y, i + s), A += bn, g = Math.cos(A) * (r ? r / 2 : S), s = Math.cos(A) * S, a = Math.sin(A) * S, y = Math.sin(A) * (r ? r / 2 : S), t.moveTo(n - g, i - a), t.lineTo(n + g, i + a), t.moveTo(n + y, i - s), t.lineTo(n - y, i + s);
+                g = Math.cos(A) * (r ? r / 2 : C), s = Math.cos(A) * C, a = Math.sin(A) * C, y = Math.sin(A) * (r ? r / 2 : C), t.moveTo(n - g, i - a), t.lineTo(n + g, i + a), t.moveTo(n + y, i - s), t.lineTo(n - y, i + s), A += bn, g = Math.cos(A) * (r ? r / 2 : C), s = Math.cos(A) * C, a = Math.sin(A) * C, y = Math.sin(A) * (r ? r / 2 : C), t.moveTo(n - g, i - a), t.lineTo(n + g, i + a), t.moveTo(n + y, i - s), t.lineTo(n - y, i + s);
                 break;
             case "line":
-                s = r ? r / 2 : Math.cos(A) * S, a = Math.sin(A) * S, t.moveTo(n - s, i - a), t.lineTo(n + s, i + a);
+                s = r ? r / 2 : Math.cos(A) * C, a = Math.sin(A) * C, t.moveTo(n - s, i - a), t.lineTo(n + s, i + a);
                 break;
             case "dash":
-                t.moveTo(n, i), t.lineTo(n + Math.cos(A) * (r ? r / 2 : S), i + Math.sin(A) * S);
+                t.moveTo(n, i), t.lineTo(n + Math.cos(A) * (r ? r / 2 : C), i + Math.sin(A) * C);
                 break;
             case !1:
                 t.closePath();
                 break
         }
         t.fill(), e.borderWidth > 0 && t.stroke()
     }
@@ -9423,168 +9423,168 @@
     t.save(), t.beginPath(), t.rect(e.left, e.top, e.right - e.left, e.bottom - e.top), t.clip()
 }
 
 function Vr(t) {
     t.restore()
 }
 
-function Np(t, e, n, i, r) {
+function Ip(t, e, n, i, r) {
     if (!e) return t.lineTo(n.x, n.y);
     if (r === "middle") {
         let o = (e.x + n.x) / 2;
         t.lineTo(o, e.y), t.lineTo(o, n.y)
     } else r === "after" != !!i ? t.lineTo(e.x, n.y) : t.lineTo(n.x, e.y);
     t.lineTo(n.x, n.y)
 }
 
-function zp(t, e, n, i) {
+function Np(t, e, n, i) {
     if (!e) return t.lineTo(n.x, n.y);
     t.bezierCurveTo(i ? e.cp1x : e.cp2x, i ? e.cp1y : e.cp2y, i ? n.cp2x : n.cp1x, i ? n.cp2y : n.cp1y, n.x, n.y)
 }
 
-function YS(t, e) {
+function Yk(t, e) {
     e.translation && t.translate(e.translation[0], e.translation[1]), Ie(e.rotation) || t.rotate(e.rotation), e.color && (t.fillStyle = e.color), e.textAlign && (t.textAlign = e.textAlign), e.textBaseline && (t.textBaseline = e.textBaseline)
 }
 
-function XS(t, e, n, i, r) {
+function Xk(t, e, n, i, r) {
     if (r.strikethrough || r.underline) {
         let o = t.measureText(i),
             s = e - o.actualBoundingBoxLeft,
             a = e + o.actualBoundingBoxRight,
             l = n - o.actualBoundingBoxAscent,
             c = n + o.actualBoundingBoxDescent,
             d = r.strikethrough ? (l + c) / 2 : c;
         t.strokeStyle = t.fillStyle, t.beginPath(), t.lineWidth = r.decorationWidth || 2, t.moveTo(s, d), t.lineTo(a, d), t.stroke()
     }
 }
 
-function qS(t, e) {
+function qk(t, e) {
     let n = t.fillStyle;
     t.fillStyle = e.color, t.fillRect(e.left, e.top, e.width, e.height), t.fillStyle = n
 }
 
 function ir(t, e, n, i, r, o = {}) {
     let s = Re(e) ? e : [e],
         a = o.strokeWidth > 0 && o.strokeColor !== "",
         l, c;
-    for (t.save(), t.font = r.string, YS(t, o), l = 0; l < s.length; ++l) c = s[l], o.backdrop && qS(t, o.backdrop), a && (o.strokeColor && (t.strokeStyle = o.strokeColor), Ie(o.strokeWidth) || (t.lineWidth = o.strokeWidth), t.strokeText(c, n, i, o.maxWidth)), t.fillText(c, n, i, o.maxWidth), XS(t, n, i, c, o), i += Number(r.lineHeight);
+    for (t.save(), t.font = r.string, Yk(t, o), l = 0; l < s.length; ++l) c = s[l], o.backdrop && qk(t, o.backdrop), a && (o.strokeColor && (t.strokeStyle = o.strokeColor), Ie(o.strokeWidth) || (t.lineWidth = o.strokeWidth), t.strokeText(c, n, i, o.maxWidth)), t.fillText(c, n, i, o.maxWidth), Xk(t, n, i, c, o), i += Number(r.lineHeight);
     t.restore()
 }
 
 function rr(t, e) {
     let {
         x: n,
         y: i,
         w: r,
         h: o,
         radius: s
     } = e;
     t.arc(n + s.topLeft, i + s.topLeft, s.topLeft, 1.5 * Ce, Ce, !0), t.lineTo(n, i + o - s.bottomLeft), t.arc(n + s.bottomLeft, i + o - s.bottomLeft, s.bottomLeft, Ce, $e, !0), t.lineTo(n + r - s.bottomRight, i + o), t.arc(n + r - s.bottomRight, i + o - s.bottomRight, s.bottomRight, $e, 0, !0), t.lineTo(n + r, i + s.topRight), t.arc(n + r - s.topRight, i + s.topRight, s.topRight, 0, -$e, !0), t.lineTo(n + s.topLeft, i)
 }
-var ZS = /^(normal|(\d+(?:\.\d+)?)(px|em|%)?)$/,
-    GS = /^(normal|italic|initial|inherit|unset|(oblique( -?[0-9]?[0-9]deg)?))$/;
+var Zk = /^(normal|(\d+(?:\.\d+)?)(px|em|%)?)$/,
+    Kk = /^(normal|italic|initial|inherit|unset|(oblique( -?[0-9]?[0-9]deg)?))$/;
 
-function Mx(t, e) {
-    let n = ("" + t).match(ZS);
+function Px(t, e) {
+    let n = ("" + t).match(Zk);
     if (!n || n[1] === "normal") return e * 1.2;
     switch (t = +n[2], n[3]) {
         case "px":
             return t;
         case "%":
             t /= 100;
             break
     }
     return e * t
 }
-var QS = t => +t || 0;
+var Gk = t => +t || 0;
 
-function yl(t, e) {
+function vl(t, e) {
     let n = {},
         i = we(e),
         r = i ? Object.keys(e) : e,
         o = we(t) ? i ? s => pe(t[s], t[e[s]]) : s => t[s] : () => t;
-    for (let s of r) n[s] = QS(o(s));
+    for (let s of r) n[s] = Gk(o(s));
     return n
 }
 
-function Xc(t) {
-    return yl(t, {
+function qc(t) {
+    return vl(t, {
         top: "y",
         right: "x",
         bottom: "y",
         left: "x"
     })
 }
 
 function pi(t) {
-    return yl(t, ["topLeft", "topRight", "bottomLeft", "bottomRight"])
+    return vl(t, ["topLeft", "topRight", "bottomLeft", "bottomRight"])
 }
 
 function gt(t) {
-    let e = Xc(t);
+    let e = qc(t);
     return e.width = e.left + e.right, e.height = e.top + e.bottom, e
 }
 
 function tt(t, e) {
     t = t || {}, e = e || rt.font;
     let n = pe(t.size, e.size);
     typeof n == "string" && (n = parseInt(n, 10));
     let i = pe(t.style, e.style);
-    i && !("" + i).match(GS) && (console.warn('Invalid font style specified: "' + i + '"'), i = void 0);
+    i && !("" + i).match(Kk) && (console.warn('Invalid font style specified: "' + i + '"'), i = void 0);
     let r = {
         family: pe(t.family, e.family),
-        lineHeight: Mx(pe(t.lineHeight, e.lineHeight), n),
+        lineHeight: Px(pe(t.lineHeight, e.lineHeight), n),
         size: n,
         style: i,
         weight: pe(t.weight, e.weight),
         string: ""
     };
-    return r.string = Px(r), r
+    return r.string = Dx(r), r
 }
 
 function Io(t, e, n, i) {
     let r = !0,
         o, s, a;
     for (o = 0, s = t.length; o < s; ++o)
         if (a = t[o], a !== void 0 && (e !== void 0 && typeof a == "function" && (a = a(e), r = !1), n !== void 0 && Re(a) && (a = a[n % a.length], r = !1), a !== void 0)) return i && !r && (i.cacheable = !1), a
 }
 
-function Fp(t, e, n) {
+function zp(t, e, n) {
     let {
         min: i,
         max: r
-    } = t, o = Dc(e, (r - i) / 2), s = (a, l) => n && a === 0 ? 0 : a + l;
+    } = t, o = Oc(e, (r - i) / 2), s = (a, l) => n && a === 0 ? 0 : a + l;
     return {
         min: s(i, -Math.abs(o)),
         max: s(r, o)
     }
 }
 
 function Ei(t, e) {
     return Object.assign(Object.create(t), e)
 }
 
-function vl(t, e = [""], n, i, r = () => t[0]) {
+function xl(t, e = [""], n, i, r = () => t[0]) {
     let o = n || t;
     typeof i > "u" && (i = Ax("_fallback", t));
     let s = {
         [Symbol.toStringTag]: "Object",
         _cacheable: !0,
         _scopes: t,
         _rootScopes: o,
         _fallback: i,
         _getTarget: r,
-        override: a => vl([a, ...t], e, o, i)
+        override: a => xl([a, ...t], e, o, i)
     };
     return new Proxy(s, {
         deleteProperty(a, l) {
             return delete a[l], delete a._keys, delete t[0][l], !0
         },
         get(a, l) {
-            return Dx(a, l, () => oC(l, e, t, a))
+            return Mx(a, l, () => oC(l, e, t, a))
         },
         getOwnPropertyDescriptor(a, l) {
             return Reflect.getOwnPropertyDescriptor(a._scopes[0], l)
         },
         getPrototypeOf() {
             return Reflect.getPrototypeOf(t[0])
         },
@@ -9604,24 +9604,24 @@
 function Hr(t, e, n, i) {
     let r = {
         _cacheable: !1,
         _proxy: t,
         _context: e,
         _subProxy: n,
         _stack: new Set,
-        _descriptors: qc(t, i),
+        _descriptors: Zc(t, i),
         setContext: o => Hr(t, o, n, i),
         override: o => Hr(t.override(o), e, n, i)
     };
     return new Proxy(r, {
         deleteProperty(o, s) {
             return delete o[s], delete t[s], !0
         },
         get(o, s, a) {
-            return Dx(o, s, () => JS(o, s, a))
+            return Mx(o, s, () => Jk(o, s, a))
         },
         getOwnPropertyDescriptor(o, s) {
             return o._descriptors.allKeys ? Reflect.has(t, s) ? {
                 enumerable: !0,
                 configurable: !0
             } : void 0 : Reflect.getOwnPropertyDescriptor(t, s)
         },
@@ -9636,15 +9636,15 @@
         },
         set(o, s, a) {
             return t[s] = a, delete o[s], !0
         }
     })
 }
 
-function qc(t, e = {
+function Zc(t, e = {
     scriptable: !0,
     indexable: !0
 }) {
     let {
         _scriptable: n = e.scriptable,
         _indexable: i = e.indexable,
         _allKeys: r = e.allKeys
@@ -9653,44 +9653,44 @@
         allKeys: r,
         scriptable: n,
         indexable: i,
         isScriptable: Vt(n) ? n : () => n,
         isIndexable: Vt(i) ? i : () => i
     }
 }
-var KS = (t, e) => t ? t + fl(e) : e,
-    jp = (t, e) => we(e) && t !== "adapters" && (Object.getPrototypeOf(e) === null || e.constructor === Object);
+var Qk = (t, e) => t ? t + dl(e) : e,
+    Fp = (t, e) => we(e) && t !== "adapters" && (Object.getPrototypeOf(e) === null || e.constructor === Object);
 
-function Dx(t, e, n) {
+function Mx(t, e, n) {
     if (Object.prototype.hasOwnProperty.call(t, e)) return t[e];
     let i = n();
     return t[e] = i, i
 }
 
-function JS(t, e, n) {
+function Jk(t, e, n) {
     let {
         _proxy: i,
         _context: r,
         _subProxy: o,
         _descriptors: s
     } = t, a = i[e];
-    return Vt(a) && s.isScriptable(e) && (a = eC(e, a, t, n)), Re(a) && a.length && (a = tC(e, a, t, s.isIndexable)), jp(e, a) && (a = Hr(a, r, o && o[e], s)), a
+    return Vt(a) && s.isScriptable(e) && (a = eC(e, a, t, n)), Re(a) && a.length && (a = tC(e, a, t, s.isIndexable)), Fp(e, a) && (a = Hr(a, r, o && o[e], s)), a
 }
 
 function eC(t, e, n, i) {
     let {
         _proxy: r,
         _context: o,
         _subProxy: s,
         _stack: a
     } = n;
     if (a.has(t)) throw new Error("Recursion detected: " + Array.from(a).join("->") + "->" + t);
     a.add(t);
     let l = e(o, s || i);
-    return a.delete(t), jp(t, l) && (l = Hp(r._scopes, r, t, l)), l
+    return a.delete(t), Fp(t, l) && (l = jp(r._scopes, r, t, l)), l
 }
 
 function tC(t, e, n, i) {
     let {
         _proxy: r,
         _context: o,
         _subProxy: s,
@@ -9698,15 +9698,15 @@
     } = n;
     if (typeof o.index < "u" && i(t)) return e[o.index % e.length];
     if (we(e[0])) {
         let l = e,
             c = r._scopes.filter(d => d !== l);
         e = [];
         for (let d of l) {
-            let g = Hp(c, r, t, d);
+            let g = jp(c, r, t, d);
             e.push(Hr(g, o, s && s[t], a))
         }
     }
     return e
 }
 
 function Ox(t, e, n) {
@@ -9722,22 +9722,22 @@
             let a = Ox(s._fallback, n, r);
             if (typeof a < "u" && a !== n && a !== i) return a
         } else if (s === !1 && typeof i < "u" && n !== i) return null
     }
     return !1
 }
 
-function Hp(t, e, n, i) {
+function jp(t, e, n, i) {
     let r = e._rootScopes,
         o = Ox(e._fallback, n, i),
         s = [...t, ...r],
         a = new Set;
     a.add(i);
     let l = gx(a, s, n, o || n, i);
-    return l === null || typeof o < "u" && o !== n && (l = gx(a, s, o, l, i), l === null) ? !1 : vl(Array.from(a), [""], r, o, () => rC(e, n, i))
+    return l === null || typeof o < "u" && o !== n && (l = gx(a, s, o, l, i), l === null) ? !1 : xl(Array.from(a), [""], r, o, () => rC(e, n, i))
 }
 
 function gx(t, e, n, i, r) {
     for (; n;) n = iC(t, e, n, i, r);
     return n
 }
 
@@ -9747,15 +9747,15 @@
     let r = i[e];
     return Re(r) && we(n) ? n : r || {}
 }
 
 function oC(t, e, n, i) {
     let r;
     for (let o of e)
-        if (r = Ax(KS(o, t), n), typeof r < "u") return jp(t, r) ? Hp(n, i, t, r) : r
+        if (r = Ax(Qk(o, t), n), typeof r < "u") return Fp(t, r) ? jp(n, i, t, r) : r
 }
 
 function Ax(t, e) {
     for (let n of e) {
         if (!n) continue;
         let i = n[t];
         if (typeof i < "u") return i
@@ -9770,15 +9770,15 @@
 function sC(t) {
     let e = new Set;
     for (let n of t)
         for (let i of Object.keys(n).filter(r => !r.startsWith("_"))) e.add(i);
     return Array.from(e)
 }
 
-function Zc(t, e, n, i) {
+function Kc(t, e, n, i) {
     let {
         iScale: r
     } = t, {
         key: o = "r"
     } = this._parsing, s = new Array(i), a, l, c, d;
     for (a = 0, l = i; a < l; ++a) c = a + n, d = e[c], s[a] = {
         r: r.parse(Ci(d, o), c)
@@ -9849,38 +9849,38 @@
                 let d = c[e] - l[e];
                 r[s] = d !== 0 ? (c[n] - l[n]) / d : 0
             }
             o[s] = a ? c ? sn(r[s - 1]) !== sn(r[s]) ? 0 : (r[s - 1] + r[s]) / 2 : r[s - 1] : r[s]
         } lC(t, r, o), uC(t, o, e)
 }
 
-function Ec(t, e, n) {
+function Tc(t, e, n) {
     return Math.max(Math.min(t, n), e)
 }
 
 function cC(t, e) {
     let n, i, r, o, s, a = ci(t[0], e);
-    for (n = 0, i = t.length; n < i; ++n) s = o, o = a, a = n < i - 1 && ci(t[n + 1], e), o && (r = t[n], s && (r.cp1x = Ec(r.cp1x, e.left, e.right), r.cp1y = Ec(r.cp1y, e.top, e.bottom)), a && (r.cp2x = Ec(r.cp2x, e.left, e.right), r.cp2y = Ec(r.cp2y, e.top, e.bottom)))
+    for (n = 0, i = t.length; n < i; ++n) s = o, o = a, a = n < i - 1 && ci(t[n + 1], e), o && (r = t[n], s && (r.cp1x = Tc(r.cp1x, e.left, e.right), r.cp1y = Tc(r.cp1y, e.top, e.bottom)), a && (r.cp2x = Tc(r.cp2x, e.left, e.right), r.cp2y = Tc(r.cp2y, e.top, e.bottom)))
 }
 
-function Bp(t, e, n, i, r) {
+function Hp(t, e, n, i, r) {
     let o, s, a, l;
     if (e.spanGaps && (t = t.filter(c => !c.skip)), e.cubicInterpolationMode === "monotone") Ix(t, r);
     else {
         let c = i ? t[t.length - 1] : t[0];
         for (o = 0, s = t.length; o < s; ++o) a = t[o], l = Rx(c, a, t[Math.min(o + 1, s - (i ? 0 : 1)) % s], e.tension), a.cp1x = l.previous.x, a.cp1y = l.previous.y, a.cp2x = l.next.x, a.cp2y = l.next.y, c = a
     }
     e.capBezierPoints && cC(t, n)
 }
 
-function xl() {
+function bl() {
     return typeof window < "u" && typeof document < "u"
 }
 
-function bl(t) {
+function _l(t) {
     let e = t.parentNode;
     return e && e.toString() === "[object ShadowRoot]" && (e = e.host), e
 }
 
 function Mc(t, e, n) {
     let i;
     return typeof t == "string" ? (i = parseInt(t, 10), t.indexOf("%") !== -1 && (i = i / 100 * e.parentNode[n])) : i = t, i
@@ -9888,15 +9888,15 @@
 var Gc = t => t.ownerDocument.defaultView.getComputedStyle(t, null);
 
 function Nx(t, e) {
     return Gc(t).getPropertyValue(e)
 }
 var fC = ["top", "right", "bottom", "left"];
 
-function Po(t, e, n) {
+function Do(t, e, n) {
     let i = {};
     n = n ? "-" + n : "";
     for (let r = 0; r < 4; r++) {
         let o = fC[r];
         i[o] = parseFloat(t[e + "-" + o + n]) || 0
     }
     return i.width = i.left + i.right, i.height = i.top + i.bottom, i
@@ -9925,113 +9925,113 @@
 }
 
 function zn(t, e) {
     if ("native" in t) return t;
     let {
         canvas: n,
         currentDevicePixelRatio: i
-    } = e, r = Gc(n), o = r.boxSizing === "border-box", s = Po(r, "padding"), a = Po(r, "border", "width"), {
+    } = e, r = Gc(n), o = r.boxSizing === "border-box", s = Do(r, "padding"), a = Do(r, "border", "width"), {
         x: l,
         y: c,
         box: d
     } = hC(t, n), g = s.left + (d && a.left), y = s.top + (d && a.top), {
         width: x,
-        height: w
+        height: _
     } = e;
-    return o && (x -= s.width + a.width, w -= s.height + a.height), {
+    return o && (x -= s.width + a.width, _ -= s.height + a.height), {
         x: Math.round((l - g) / x * n.width / i),
-        y: Math.round((c - y) / w * n.height / i)
+        y: Math.round((c - y) / _ * n.height / i)
     }
 }
 
 function pC(t, e, n) {
     let i, r;
     if (e === void 0 || n === void 0) {
-        let o = bl(t);
+        let o = _l(t);
         if (!o) e = t.clientWidth, n = t.clientHeight;
         else {
             let s = o.getBoundingClientRect(),
                 a = Gc(o),
-                l = Po(a, "border", "width"),
-                c = Po(a, "padding");
+                l = Do(a, "border", "width"),
+                c = Do(a, "padding");
             e = s.width - c.width - l.width, n = s.height - c.height - l.height, i = Mc(a.maxWidth, o, "clientWidth"), r = Mc(a.maxHeight, o, "clientHeight")
         }
     }
     return {
         width: e,
         height: n,
-        maxWidth: i || cl,
-        maxHeight: r || cl
+        maxWidth: i || fl,
+        maxHeight: r || fl
     }
 }
-var Tc = t => Math.round(t * 10) / 10;
+var Dc = t => Math.round(t * 10) / 10;
 
-function Wp(t, e, n, i) {
+function Bp(t, e, n, i) {
     let r = Gc(t),
-        o = Po(r, "margin"),
-        s = Mc(r.maxWidth, t, "clientWidth") || cl,
-        a = Mc(r.maxHeight, t, "clientHeight") || cl,
+        o = Do(r, "margin"),
+        s = Mc(r.maxWidth, t, "clientWidth") || fl,
+        a = Mc(r.maxHeight, t, "clientHeight") || fl,
         l = pC(t, e, n),
         {
             width: c,
             height: d
         } = l;
     if (r.boxSizing === "content-box") {
-        let y = Po(r, "border", "width"),
-            x = Po(r, "padding");
+        let y = Do(r, "border", "width"),
+            x = Do(r, "padding");
         c -= x.width + y.width, d -= x.height + y.height
     }
-    return c = Math.max(0, c - o.width), d = Math.max(0, i ? c / i : d - o.height), c = Tc(Math.min(c, s, l.maxWidth)), d = Tc(Math.min(d, a, l.maxHeight)), c && !d && (d = Tc(c / 2)), (e !== void 0 || n !== void 0) && i && l.height && d > l.height && (d = l.height, c = Tc(Math.floor(d * i))), {
+    return c = Math.max(0, c - o.width), d = Math.max(0, i ? c / i : d - o.height), c = Dc(Math.min(c, s, l.maxWidth)), d = Dc(Math.min(d, a, l.maxHeight)), c && !d && (d = Dc(c / 2)), (e !== void 0 || n !== void 0) && i && l.height && d > l.height && (d = l.height, c = Dc(Math.floor(d * i))), {
         width: c,
         height: d
     }
 }
 
 function Qc(t, e, n) {
     let i = e || 1,
         r = Math.floor(t.height * i),
         o = Math.floor(t.width * i);
     t.height = Math.floor(t.height), t.width = Math.floor(t.width);
     let s = t.canvas;
     return s.style && (n || !s.style.height && !s.style.width) && (s.style.height = `${t.height}px`, s.style.width = `${t.width}px`), t.currentDevicePixelRatio !== i || s.height !== r || s.width !== o ? (t.currentDevicePixelRatio = i, s.height = r, s.width = o, t.ctx.setTransform(i, 0, 0, i, 0, 0), !0) : !1
 }
-var Vp = function() {
+var Wp = function() {
     let t = !1;
     try {
         let e = {
             get passive() {
                 return t = !0, !1
             }
         };
-        xl() && (window.addEventListener("test", null, e), window.removeEventListener("test", null, e))
+        bl() && (window.addEventListener("test", null, e), window.removeEventListener("test", null, e))
     } catch {}
     return t
 }();
 
-function Kc(t, e) {
+function Jc(t, e) {
     let n = Nx(t, e),
         i = n && n.match(/^(\d+)(\.\d+)?px$/);
     return i ? +i[1] : void 0
 }
 
 function er(t, e, n, i) {
     return {
         x: t.x + n * (e.x - t.x),
         y: t.y + n * (e.y - t.y)
     }
 }
 
-function Up(t, e, n, i) {
+function Vp(t, e, n, i) {
     return {
         x: t.x + n * (e.x - t.x),
         y: i === "middle" ? n < .5 ? t.y : e.y : i === "after" ? n < 1 ? t.y : e.y : n > 0 ? e.y : t.y
     }
 }
 
-function $p(t, e, n, i) {
+function Up(t, e, n, i) {
     let r = {
             x: t.cp2x,
             y: t.cp2y
         },
         o = {
             x: e.cp1x,
             y: e.cp1y
@@ -10080,20 +10080,20 @@
         }
     };
 
 function Ur(t, e, n) {
     return t ? gC(e, n) : mC()
 }
 
-function Jc(t, e) {
+function ef(t, e) {
     let n, i;
     (e === "ltr" || e === "rtl") && (n = t.canvas.style, i = [n.getPropertyValue("direction"), n.getPropertyPriority("direction")], n.setProperty("direction", e, "important"), t.prevTextDirection = i)
 }
 
-function ef(t, e) {
+function tf(t, e) {
     e !== void 0 && (delete t.prevTextDirection, t.canvas.style.setProperty("direction", e[0], e[1]))
 }
 
 function zx(t) {
     return t === "angle" ? {
         between: Lo,
         compare: Cx,
@@ -10141,51 +10141,51 @@
         start: c,
         end: d,
         loop: g,
         style: t.style
     }
 }
 
-function tf(t, e, n) {
+function nf(t, e, n) {
     if (!n) return [t];
     let {
         property: i,
         start: r,
         end: o
     } = n, s = e.length, {
         compare: a,
         between: l,
         normalize: c
     } = zx(i), {
         start: d,
         end: g,
         loop: y,
         style: x
-    } = yC(t, e, n), w = [], S = !1, A = null, _, C, M, z = () => l(r, M, _) && a(r, M) !== 0, F = () => a(o, _) === 0 || l(o, M, _), h = () => S || z(), Y = () => !S || F();
-    for (let V = d, te = d; V <= g; ++V) C = e[V % s], !C.skip && (_ = c(C[i]), _ !== M && (S = l(_, r, o), A === null && h() && (A = a(_, r) === 0 ? V : te), A !== null && Y() && (w.push(yx({
+    } = yC(t, e, n), _ = [], C = !1, A = null, w, k, P, z = () => l(r, P, w) && a(r, P) !== 0, F = () => a(o, w) === 0 || l(o, P, w), h = () => C || z(), $ = () => !C || F();
+    for (let Y = d, ne = d; Y <= g; ++Y) k = e[Y % s], !k.skip && (w = c(k[i]), w !== P && (C = l(w, r, o), A === null && h() && (A = a(w, r) === 0 ? Y : ne), A !== null && $() && (_.push(yx({
         start: A,
-        end: V,
+        end: Y,
         loop: y,
         count: s,
         style: x
-    })), A = null), te = V, M = _));
-    return A !== null && w.push(yx({
+    })), A = null), ne = Y, P = w));
+    return A !== null && _.push(yx({
         start: A,
         end: g,
         loop: y,
         count: s,
         style: x
-    })), w
+    })), _
 }
 
-function nf(t, e) {
+function rf(t, e) {
     let n = [],
         i = t.segments;
     for (let r = 0; r < i.length; r++) {
-        let o = tf(i[r], t.points, e);
+        let o = nf(i[r], t.points, e);
         o.length && n.push(...o)
     }
     return n
 }
 
 function vC(t, e, n, i) {
     let r = 0,
@@ -10217,15 +10217,15 @@
     return s !== null && o.push({
         start: e % r,
         end: s % r,
         loop: i
     }), o
 }
 
-function Yp(t, e) {
+function $p(t, e) {
     let n = t.points,
         i = t.options.spanGaps,
         r = n.length;
     if (!r) return [];
     let o = !!t._loop,
         {
             start: s,
@@ -10256,43 +10256,43 @@
         } = t,
         l = n.length,
         c = [],
         d = o,
         g = e[0].start,
         y = g;
 
-    function x(w, S, A, _) {
-        let C = a ? -1 : 1;
-        if (w !== S) {
-            for (w += l; n[w % l].skip;) w -= C;
-            for (; n[S % l].skip;) S += C;
-            w % l !== S % l && (c.push({
-                start: w % l,
-                end: S % l,
+    function x(_, C, A, w) {
+        let k = a ? -1 : 1;
+        if (_ !== C) {
+            for (_ += l; n[_ % l].skip;) _ -= k;
+            for (; n[C % l].skip;) C += k;
+            _ % l !== C % l && (c.push({
+                start: _ % l,
+                end: C % l,
                 loop: A,
-                style: _
-            }), d = _, g = S % l)
+                style: w
+            }), d = w, g = C % l)
         }
     }
-    for (let w of e) {
-        g = a ? g : w.start;
-        let S = n[g % l],
+    for (let _ of e) {
+        g = a ? g : _.start;
+        let C = n[g % l],
             A;
-        for (y = g + 1; y <= w.end; y++) {
-            let _ = n[y % l];
+        for (y = g + 1; y <= _.end; y++) {
+            let w = n[y % l];
             A = xx(i.setContext(Ei(r, {
                 type: "segment",
-                p0: S,
-                p1: _,
+                p0: C,
+                p1: w,
                 p0DataIndex: (y - 1) % l,
                 p1DataIndex: y % l,
                 datasetIndex: s
-            }))), _C(A, d) && x(g, y - 1, w.loop, d), S = _, d = A
+            }))), _C(A, d) && x(g, y - 1, _.loop, d), C = w, d = A
         }
-        g < y - 1 && x(g, y - 1, w.loop, d)
+        g < y - 1 && x(g, y - 1, _.loop, d)
     }
     return c
 }
 
 function xx(t) {
     return {
         backgroundColor: t.backgroundColor,
@@ -10305,34 +10305,34 @@
     }
 }
 
 function _C(t, e) {
     if (!e) return !1;
     let n = [],
         i = function(r, o) {
-            return Wc(o) ? (n.includes(o) || n.push(o), n.indexOf(o)) : o
+            return Vc(o) ? (n.includes(o) || n.push(o), n.indexOf(o)) : o
         };
     return JSON.stringify(t, i) !== JSON.stringify(e, i)
 }
-var ng = class {
+var tg = class {
         constructor() {
             this._request = null, this._charts = new Map, this._running = !1, this._lastDate = void 0
         }
         _notify(e, n, i, r) {
             let o = n.listeners[r],
                 s = n.duration;
             o.forEach(a => a({
                 chart: e,
                 initial: n.initial,
                 numSteps: s,
                 currentStep: Math.min(i - n.start, s)
             }))
         }
         _refresh() {
-            this._request || (this._running = !0, this._request = Fc.call(window, () => {
+            this._request || (this._running = !0, this._request = jc.call(window, () => {
                 this._update(), this._request = null, this._running && this._refresh()
             }))
         }
         _update(e = Date.now()) {
             let n = 0;
             this._charts.forEach((i, r) => {
                 if (!i.running || !i.items.length) return;
@@ -10383,30 +10383,30 @@
             for (; r >= 0; --r) i[r].cancel();
             n.items = [], this._notify(e, n, Date.now(), "complete")
         }
         remove(e) {
             return this._charts.delete(e)
         }
     },
-    or = new ng,
+    or = new tg,
     Fx = "transparent",
     wC = {
         boolean(t, e, n) {
             return n > .5 ? e : t
         },
         color(t, e, n) {
-            let i = Vc(t || Fx),
-                r = i.valid && Vc(e || Fx);
+            let i = Uc(t || Fx),
+                r = i.valid && Uc(e || Fx);
             return r && r.valid ? r.mix(i, n).hexString() : e
         },
         number(t, e, n) {
             return t + (e - t) * n
         }
     },
-    ig = class {
+    ng = class {
         constructor(e, n, i, r) {
             let o = n[i];
             r = Io([e.to, r, o, e.from]);
             let s = Io([e.from, o, r]);
             this._active = !0, this._fn = e.fn || wC[e.type || typeof s], this._easing = To[e.easing] || To.linear, this._start = Math.floor(Date.now() + (e.delay || 0)), this._duration = this._total = Math.floor(e.duration), this._loop = !!e.loop, this._target = n, this._prop = i, this._from = s, this._to = r, this._promises = void 0
         }
         active() {
@@ -10473,18 +10473,18 @@
                 (Re(o.properties) && o.properties || [r]).forEach(a => {
                     (a === r || !i.has(a)) && i.set(a, s)
                 })
             })
         }
         _animateOptions(e, n) {
             let i = n.options,
-                r = SC(e, i);
+                r = kC(e, i);
             if (!r) return [];
             let o = this._createAnimations(r, i);
-            return i.$shared && kC(e.options.$animations, i).then(() => {
+            return i.$shared && SC(e.options.$animations, i).then(() => {
                 e.options = i
             }, () => {}), o
         }
         _createAnimations(e, n) {
             let i = this._properties,
                 r = [],
                 o = e.$animations || (e.$animations = {}),
@@ -10506,39 +10506,39 @@
                         g.update(y, d, a);
                         continue
                     } else g.cancel();
                 if (!y || !y.duration) {
                     e[c] = d;
                     continue
                 }
-                o[c] = g = new ig(y, e, c, d), r.push(g)
+                o[c] = g = new ng(y, e, c, d), r.push(g)
             }
             return r
         }
         update(e, n) {
             if (this._properties.size === 0) {
                 Object.assign(e, n);
                 return
             }
             let i = this._createAnimations(e, n);
             if (i.length) return or.add(this._chart, i), !0
         }
     };
 
-function kC(t, e) {
+function SC(t, e) {
     let n = [],
         i = Object.keys(e);
     for (let r = 0; r < i.length; r++) {
         let o = t[i[r]];
         o && o.active() && n.push(o.wait())
     }
     return Promise.all(n)
 }
 
-function SC(t, e) {
+function kC(t, e) {
     if (!e) return;
     let n = t.options;
     if (!n) {
         t.options = e;
         return
     }
     return n.$shared && (t.options = n = Object.assign({}, n, {
@@ -10617,32 +10617,32 @@
 }
 
 function Bx(t, e) {
     let n = t && t.options.stacked;
     return n || n === void 0 && e.stack !== void 0
 }
 
-function PC(t, e, n) {
+function DC(t, e, n) {
     return `${t.id}.${e.id}.${n.stack||n.type}`
 }
 
-function MC(t) {
+function PC(t) {
     let {
         min: e,
         max: n,
         minDefined: i,
         maxDefined: r
     } = t.getUserBounds();
     return {
         min: i ? e : Number.NEGATIVE_INFINITY,
         max: r ? n : Number.POSITIVE_INFINITY
     }
 }
 
-function DC(t, e, n) {
+function MC(t, e, n) {
     let i = t[e] || (t[e] = {});
     return i[n] || (i[n] = {})
 }
 
 function Wx(t, e, n, i) {
     for (let r of e.getMatchingVisibleMetas(i).reverse()) {
         let o = t[r.index];
@@ -10655,29 +10655,29 @@
     let {
         chart: n,
         _cachedMeta: i
     } = t, r = n._stacks || (n._stacks = {}), {
         iScale: o,
         vScale: s,
         index: a
-    } = i, l = o.axis, c = s.axis, d = PC(o, s, i), g = e.length, y;
+    } = i, l = o.axis, c = s.axis, d = DC(o, s, i), g = e.length, y;
     for (let x = 0; x < g; ++x) {
-        let w = e[x],
+        let _ = e[x],
             {
-                [l]: S,
+                [l]: C,
                 [c]: A
-            } = w,
-            _ = w._stacks || (w._stacks = {});
-        y = _[c] = DC(r, d, S), y[a] = A, y._top = Wx(y, s, !0, i.type), y._bottom = Wx(y, s, !1, i.type);
-        let C = y._visualValues || (y._visualValues = {});
-        C[a] = A
+            } = _,
+            w = _._stacks || (_._stacks = {});
+        y = w[c] = MC(r, d, C), y[a] = A, y._top = Wx(y, s, !0, i.type), y._bottom = Wx(y, s, !1, i.type);
+        let k = y._visualValues || (y._visualValues = {});
+        k[a] = A
     }
 }
 
-function Xp(t, e) {
+function Yp(t, e) {
     let n = t.scales;
     return Object.keys(n).filter(i => n[i].axis === e).shift()
 }
 
 function OC(t, e) {
     return Ei(t, {
         active: !1,
@@ -10698,54 +10698,54 @@
         element: n,
         index: e,
         mode: "default",
         type: "data"
     })
 }
 
-function _l(t, e) {
+function wl(t, e) {
     let n = t.controller.index,
         i = t.vScale && t.vScale.axis;
     if (i) {
         e = e || t._parsed;
         for (let r of e) {
             let o = r._stacks;
             if (!o || o[i] === void 0 || o[i][n] === void 0) return;
             delete o[i][n], o[i]._visualValues !== void 0 && o[i]._visualValues[n] !== void 0 && delete o[i]._visualValues[n]
         }
     }
 }
-var qp = t => t === "reset" || t === "none",
+var Xp = t => t === "reset" || t === "none",
     Ux = (t, e) => e ? t : Object.assign({}, t),
     LC = (t, e, n) => t && !e.hidden && e._stacked && {
         keys: Fb(n, !0),
         values: null
     },
-    Mi = class {
+    Pi = class {
         static defaults = {};
         static datasetElementType = null;
         static dataElementType = null;
         constructor(e, n) {
             this.chart = e, this._ctx = e.ctx, this.index = n, this._cachedDataOpts = {}, this._cachedMeta = this.getMeta(), this._type = this._cachedMeta.type, this.options = void 0, this._parsing = !1, this._data = void 0, this._objectData = void 0, this._sharedOptions = void 0, this._drawStart = void 0, this._drawCount = void 0, this.enableOptionSharing = !1, this.supportsDecimation = !1, this.$context = void 0, this._syncList = [], this.datasetElementType = new.target.datasetElementType, this.dataElementType = new.target.dataElementType, this.initialize()
         }
         initialize() {
             let e = this._cachedMeta;
             this.configure(), this.linkScales(), e._stacked = Bx(e.vScale, e), this.addElements(), this.options.fill && !this.chart.isPluginEnabled("filler") && console.warn("Tried to use the 'fill' option without the 'Filler' plugin enabled. Please import and register the 'Filler' plugin and make sure it is not disabled in the options")
         }
         updateIndex(e) {
-            this.index !== e && _l(this._cachedMeta), this.index = e
+            this.index !== e && wl(this._cachedMeta), this.index = e
         }
         linkScales() {
             let e = this.chart,
                 n = this._cachedMeta,
                 i = this.getDataset(),
-                r = (g, y, x, w) => g === "x" ? y : g === "r" ? w : x,
-                o = n.xAxisID = pe(i.xAxisID, Xp(e, "x")),
-                s = n.yAxisID = pe(i.yAxisID, Xp(e, "y")),
-                a = n.rAxisID = pe(i.rAxisID, Xp(e, "r")),
+                r = (g, y, x, _) => g === "x" ? y : g === "r" ? _ : x,
+                o = n.xAxisID = pe(i.xAxisID, Yp(e, "x")),
+                s = n.yAxisID = pe(i.yAxisID, Yp(e, "y")),
+                a = n.rAxisID = pe(i.rAxisID, Yp(e, "r")),
                 l = n.indexAxis,
                 c = n.iAxisID = r(l, o, s, a),
                 d = n.vAxisID = r(l, s, o, a);
             n.xScale = this.getScaleForId(o), n.yScale = this.getScaleForId(s), n.rScale = this.getScaleForId(a), n.iScale = this.getScaleForId(c), n.vScale = this.getScaleForId(d)
         }
         getDataset() {
             return this.chart.data.datasets[this.index]
@@ -10761,41 +10761,41 @@
             return e === n.iScale ? n.vScale : n.iScale
         }
         reset() {
             this._update("reset")
         }
         _destroy() {
             let e = this._cachedMeta;
-            this._data && Nc(this._data, this), e._stacked && _l(e)
+            this._data && zc(this._data, this), e._stacked && wl(e)
         }
         _dataCheck() {
             let e = this.getDataset(),
                 n = e.data || (e.data = []),
                 i = this._data;
             if (we(n)) this._data = TC(n);
             else if (i !== n) {
                 if (i) {
-                    Nc(i, this);
+                    zc(i, this);
                     let r = this._cachedMeta;
-                    _l(r), r._parsed = []
+                    wl(r), r._parsed = []
                 }
-                n && Object.isExtensible(n) && Ap(n, this), this._syncList = [], this._data = n
+                n && Object.isExtensible(n) && Op(n, this), this._syncList = [], this._data = n
             }
         }
         addElements() {
             let e = this._cachedMeta;
             this._dataCheck(), this.datasetElementType && (e.dataset = new this.datasetElementType)
         }
         buildOrUpdateElements(e) {
             let n = this._cachedMeta,
                 i = this.getDataset(),
                 r = !1;
             this._dataCheck();
             let o = n._stacked;
-            n._stacked = Bx(n.vScale, n), n.stack !== i.stack && (r = !0, _l(n), n.stack = i.stack), this._resyncElements(e), (r || o !== n._stacked) && Vx(this, n._parsed)
+            n._stacked = Bx(n.vScale, n), n.stack !== i.stack && (r = !0, wl(n), n.stack = i.stack), this._resyncElements(e), (r || o !== n._stacked) && Vx(this, n._parsed)
         }
         configure() {
             let e = this.chart.config,
                 n = e.datasetScopeKeys(this._type),
                 i = e.getOptionScopes(this.getDataset(), n, !0);
             this.options = e.createResolver(i, this.getContext()), this._parsing = this.options.parsing, this._cachedDataOpts = {}
         }
@@ -10816,18 +10816,18 @@
             }
             s && Vx(this, y)
         }
         parsePrimitiveData(e, n, i, r) {
             let {
                 iScale: o,
                 vScale: s
-            } = e, a = o.axis, l = s.axis, c = o.getLabels(), d = o === s, g = new Array(r), y, x, w;
-            for (y = 0, x = r; y < x; ++y) w = y + i, g[y] = {
-                [a]: d || o.parse(c[w], w),
-                [l]: s.parse(n[w], w)
+            } = e, a = o.axis, l = s.axis, c = o.getLabels(), d = o === s, g = new Array(r), y, x, _;
+            for (y = 0, x = r; y < x; ++y) _ = y + i, g[y] = {
+                [a]: d || o.parse(c[_], _),
+                [l]: s.parse(n[_], _)
             };
             return g
         }
         parseArrayData(e, n, i, r) {
             let {
                 xScale: o,
                 yScale: s
@@ -10886,26 +10886,26 @@
                 c = {
                     min: Number.POSITIVE_INFINITY,
                     max: Number.NEGATIVE_INFINITY
                 },
                 {
                     min: d,
                     max: g
-                } = MC(a),
+                } = PC(a),
                 y, x;
 
-            function w() {
+            function _() {
                 x = r[y];
-                let S = x[a.axis];
-                return !qe(x[e.axis]) || d > S || g < S
+                let C = x[a.axis];
+                return !qe(x[e.axis]) || d > C || g < C
             }
-            for (y = 0; y < s && !(!w() && (this.updateRangeFromParsed(c, e, x, l), o)); ++y);
+            for (y = 0; y < s && !(!_() && (this.updateRangeFromParsed(c, e, x, l), o)); ++y);
             if (o) {
                 for (y = s - 1; y >= 0; --y)
-                    if (!w()) {
+                    if (!_()) {
                         this.updateRangeFromParsed(c, e, x, l);
                         break
                     }
             }
             return c
         }
         getAllParsedValues(e) {
@@ -10977,17 +10977,17 @@
                 l = this.enableOptionSharing && Ut(i);
             if (a) return Ux(a, l);
             let c = this.chart.config,
                 d = c.datasetElementScopeKeys(this._type, e),
                 g = r ? [`${e}Hover`, "hover", e, ""] : [e, ""],
                 y = c.getOptionScopes(this.getDataset(), d),
                 x = Object.keys(rt.elements[e]),
-                w = () => this.getContext(i, r, n),
-                S = c.resolveNamedOptions(y, x, w, g);
-            return S.$shared && (S.$shared = l, o[s] = Object.freeze(Ux(S, l))), S
+                _ = () => this.getContext(i, r, n),
+                C = c.resolveNamedOptions(y, x, _, g);
+            return C.$shared && (C.$shared = l, o[s] = Object.freeze(Ux(C, l))), C
         }
         _resolveAnimations(e, n, i) {
             let r = this.chart,
                 o = this._cachedDataOpts,
                 s = `animation-${n}`,
                 a = o[s];
             if (a) return a;
@@ -11001,31 +11001,31 @@
             let c = new zs(r, l && l.animations);
             return l && l._cacheable && (o[s] = Object.freeze(c)), c
         }
         getSharedOptions(e) {
             if (e.$shared) return this._sharedOptions || (this._sharedOptions = Object.assign({}, e))
         }
         includeOptions(e, n) {
-            return !n || qp(e) || this.chart._animationsDisabled
+            return !n || Xp(e) || this.chart._animationsDisabled
         }
         _getSharedOptions(e, n) {
             let i = this.resolveDataElementOptions(e, n),
                 r = this._sharedOptions,
                 o = this.getSharedOptions(i),
                 s = this.includeOptions(n, o) || o !== r;
             return this.updateSharedOptions(o, n, i), {
                 sharedOptions: o,
                 includeOptions: s
             }
         }
         updateElement(e, n, i, r) {
-            qp(r) ? Object.assign(e, i) : this._resolveAnimations(n, r).update(e, i)
+            Xp(r) ? Object.assign(e, i) : this._resolveAnimations(n, r).update(e, i)
         }
         updateSharedOptions(e, n, i) {
-            e && !qp(n) && this._resolveAnimations(void 0, n).update(e, i)
+            e && !Xp(n) && this._resolveAnimations(void 0, n).update(e, i)
         }
         _setStyle(e, n, i, r) {
             e.active = r;
             let o = this.getStyle(n, r);
             this._resolveAnimations(n, i, r).update(e, {
                 options: !r && this.getSharedOptions(o) || o
             })
@@ -11065,15 +11065,15 @@
             this._parsing && l(r._parsed), this.parse(e, n), i && this.updateElements(o, e, n, "reset")
         }
         updateElements(e, n, i, r) {}
         _removeElements(e, n) {
             let i = this._cachedMeta;
             if (this._parsing) {
                 let r = i._parsed.splice(e, n);
-                i._stacked && _l(i, r)
+                i._stacked && wl(i, r)
             }
             i.data.splice(e, n)
         }
         _sync(e) {
             if (this._parsing) this._syncList.push(e);
             else {
                 let [n, i, r] = e;
@@ -11102,15 +11102,15 @@
     };
 
 function RC(t, e) {
     if (!t._cache.$bar) {
         let n = t.getMatchingVisibleMetas(e),
             i = [];
         for (let r = 0, o = n.length; r < o; r++) i = i.concat(n[r].controller.getAllParsedValues(t));
-        t._cache.$bar = zc(i.sort((r, o) => r - o))
+        t._cache.$bar = Fc(i.sort((r, o) => r - o))
     }
     return t._cache.$bar
 }
 
 function IC(t) {
     let e = t.iScale,
         n = RC(e, t.type),
@@ -11176,15 +11176,15 @@
         a = r === o,
         l = [],
         c, d, g, y;
     for (c = n, d = n + i; c < d; ++c) y = e[c], g = {}, g[r.axis] = a || r.parse(s[c], c), l.push(jb(y, g, o, c));
     return l
 }
 
-function Zp(t) {
+function qp(t) {
     return t && t.barStart !== void 0 && t.barEnd !== void 0
 }
 
 function jC(t, e, n) {
     return t !== 0 ? sn(t) : (e.isHorizontal() ? 1 : -1) * (e.min >= n ? 1 : -1)
 }
 
@@ -11238,15 +11238,15 @@
 }
 
 function VC(t, {
     inflateAmount: e
 }, n) {
     t.inflateAmount = e === "auto" ? n === 1 ? .33 : 0 : e
 }
-var rg = class extends Mi {
+var ig = class extends Pi {
         static id = "bar";
         static defaults = {
             datasetElementType: !1,
             dataElementType: "bar",
             categoryPercentage: .8,
             barPercentage: .9,
             grouped: !0,
@@ -11281,16 +11281,16 @@
         parseObjectData(e, n, i, r) {
             let {
                 iScale: o,
                 vScale: s
             } = e, {
                 xAxisKey: a = "x",
                 yAxisKey: l = "y"
-            } = this._parsing, c = o.axis === "x" ? a : l, d = s.axis === "x" ? a : l, g = [], y, x, w, S;
-            for (y = i, x = i + r; y < x; ++y) S = n[y], w = {}, w[o.axis] = o.parse(Ci(S, c), y), g.push(jb(Ci(S, d), w, s, y));
+            } = this._parsing, c = o.axis === "x" ? a : l, d = s.axis === "x" ? a : l, g = [], y, x, _, C;
+            for (y = i, x = i + r; y < x; ++y) C = n[y], _ = {}, _[o.axis] = o.parse(Ci(C, c), y), g.push(jb(Ci(C, d), _, s, y));
             return g
         }
         updateRangeFromParsed(e, n, i, r) {
             super.updateRangeFromParsed(e, n, i, r);
             let o = i._custom;
             o && n === this._cachedMeta.vScale && (e.min = Math.min(e.min, o.min), e.max = Math.max(e.max, o.max))
         }
@@ -11301,15 +11301,15 @@
             let n = this._cachedMeta,
                 {
                     iScale: i,
                     vScale: r
                 } = n,
                 o = this.getParsed(e),
                 s = o._custom,
-                a = Zp(s) ? "[" + s.start + ", " + s.end + "]" : "" + r.getLabelForValue(o[r.axis]);
+                a = qp(s) ? "[" + s.start + ", " + s.end + "]" : "" + r.getLabelForValue(o[r.axis]);
             return {
                 label: "" + i.getLabelForValue(o[i.axis]),
                 value: a
             }
         }
         initialize() {
             this.enableOptionSharing = !0, super.initialize();
@@ -11332,33 +11332,33 @@
                 c = a.isHorizontal(),
                 d = this._getRuler(),
                 {
                     sharedOptions: g,
                     includeOptions: y
                 } = this._getSharedOptions(n, r);
             for (let x = n; x < n + i; x++) {
-                let w = this.getParsed(x),
-                    S = o || Ie(w[a.axis]) ? {
+                let _ = this.getParsed(x),
+                    C = o || Ie(_[a.axis]) ? {
                         base: l,
                         head: l
                     } : this._calculateBarValuePixels(x),
                     A = this._calculateBarIndexPixels(x, d),
-                    _ = (w._stacks || {})[a.axis],
-                    C = {
+                    w = (_._stacks || {})[a.axis],
+                    k = {
                         horizontal: c,
-                        base: S.base,
-                        enableBorderRadius: !_ || Zp(w._custom) || s === _._top || s === _._bottom,
-                        x: c ? S.head : A.center,
-                        y: c ? A.center : S.head,
-                        height: c ? A.size : Math.abs(S.size),
-                        width: c ? Math.abs(S.size) : A.size
+                        base: C.base,
+                        enableBorderRadius: !w || qp(_._custom) || s === w._top || s === w._bottom,
+                        x: c ? C.head : A.center,
+                        y: c ? A.center : C.head,
+                        height: c ? A.size : Math.abs(C.size),
+                        width: c ? Math.abs(C.size) : A.size
                     };
-                y && (C.options = g || this.resolveDataElementOptions(x, e[x].active ? "active" : r));
-                let M = C.options || e[x].options;
-                BC(C, M, _, s), VC(C, M, d.ratio), this.updateElement(e[x], x, C, r)
+                y && (k.options = g || this.resolveDataElementOptions(x, e[x].active ? "active" : r));
+                let P = k.options || e[x].options;
+                BC(k, P, w, s), VC(k, P, d.ratio), this.updateElement(e[x], x, k, r)
             }
         }
         _getStacks(e, n) {
             let {
                 iScale: i
             } = this._cachedMeta, r = i.getMatchingVisibleMetas(this._type).filter(l => l.controller.options.grouped), o = i.options.stacked, s = [], a = l => {
                 let c = l.controller.getParsed(n),
@@ -11403,35 +11403,35 @@
                     _stacked: i,
                     index: r
                 },
                 options: {
                     base: o,
                     minBarLength: s
                 }
-            } = this, a = o || 0, l = this.getParsed(e), c = l._custom, d = Zp(c), g = l[n.axis], y = 0, x = i ? this.applyStack(n, l, i) : g, w, S;
+            } = this, a = o || 0, l = this.getParsed(e), c = l._custom, d = qp(c), g = l[n.axis], y = 0, x = i ? this.applyStack(n, l, i) : g, _, C;
             x !== g && (y = x - g, x = g), d && (g = c.barStart, x = c.barEnd - c.barStart, g !== 0 && sn(g) !== sn(c.barEnd) && (y = 0), y += g);
             let A = !Ie(o) && !d ? o : y,
-                _ = n.getPixelForValue(A);
-            if (this.chart.getDataVisibility(e) ? w = n.getPixelForValue(y + x) : w = _, S = w - _, Math.abs(S) < s) {
-                S = jC(S, n, a) * s, g === a && (_ -= S / 2);
-                let C = n.getPixelForDecimal(0),
-                    M = n.getPixelForDecimal(1),
-                    z = Math.min(C, M),
-                    F = Math.max(C, M);
-                _ = Math.max(Math.min(_, F), z), w = _ + S, i && !d && (l._stacks[n.axis]._visualValues[r] = n.getValueForPixel(w) - n.getValueForPixel(_))
-            }
-            if (_ === n.getPixelForValue(a)) {
-                let C = sn(S) * n.getLineWidthForValue(a) / 2;
-                _ += C, S -= C
+                w = n.getPixelForValue(A);
+            if (this.chart.getDataVisibility(e) ? _ = n.getPixelForValue(y + x) : _ = w, C = _ - w, Math.abs(C) < s) {
+                C = jC(C, n, a) * s, g === a && (w -= C / 2);
+                let k = n.getPixelForDecimal(0),
+                    P = n.getPixelForDecimal(1),
+                    z = Math.min(k, P),
+                    F = Math.max(k, P);
+                w = Math.max(Math.min(w, F), z), _ = w + C, i && !d && (l._stacks[n.axis]._visualValues[r] = n.getValueForPixel(_) - n.getValueForPixel(w))
+            }
+            if (w === n.getPixelForValue(a)) {
+                let k = sn(C) * n.getLineWidthForValue(a) / 2;
+                w += k, C -= k
             }
             return {
-                size: S,
-                base: _,
-                head: w,
-                center: w + S / 2
+                size: C,
+                base: w,
+                head: _,
+                center: _ + C / 2
             }
         }
         _calculateBarIndexPixels(e, n) {
             let i = n.scale,
                 r = this.options,
                 o = r.skipNull,
                 s = pe(r.maxBarThickness, 1 / 0),
@@ -11454,15 +11454,15 @@
                 n = e.vScale,
                 i = e.data,
                 r = i.length,
                 o = 0;
             for (; o < r; ++o) this.getParsed(o)[n.axis] !== null && i[o].draw(this._ctx)
         }
     },
-    og = class extends Mi {
+    rg = class extends Pi {
         static id = "bubble";
         static defaults = {
             datasetElementType: !1,
             dataElementType: "point",
             animations: {
                 numbers: {
                     type: "number",
@@ -11540,19 +11540,19 @@
                     sharedOptions: l,
                     includeOptions: c
                 } = this._getSharedOptions(n, r),
                 d = s.axis,
                 g = a.axis;
             for (let y = n; y < n + i; y++) {
                 let x = e[y],
-                    w = !o && this.getParsed(y),
-                    S = {},
-                    A = S[d] = o ? s.getPixelForDecimal(.5) : s.getPixelForValue(w[d]),
-                    _ = S[g] = o ? a.getBasePixel() : a.getPixelForValue(w[g]);
-                S.skip = isNaN(A) || isNaN(_), c && (S.options = l || this.resolveDataElementOptions(y, x.active ? "active" : r), o && (S.options.radius = 0)), this.updateElement(x, y, S, r)
+                    _ = !o && this.getParsed(y),
+                    C = {},
+                    A = C[d] = o ? s.getPixelForDecimal(.5) : s.getPixelForValue(_[d]),
+                    w = C[g] = o ? a.getBasePixel() : a.getPixelForValue(_[g]);
+                C.skip = isNaN(A) || isNaN(w), c && (C.options = l || this.resolveDataElementOptions(y, x.active ? "active" : r), o && (C.options.radius = 0)), this.updateElement(x, y, C, r)
             }
         }
         resolveDataElementOptions(e, n) {
             let i = this.getParsed(e),
                 r = super.resolveDataElementOptions(e, n);
             r.$shared && (r = Object.assign({}, r, {
                 $shared: !1
@@ -11570,30 +11570,30 @@
     if (e < We) {
         let a = t,
             l = a + e,
             c = Math.cos(a),
             d = Math.sin(a),
             g = Math.cos(l),
             y = Math.sin(l),
-            x = (M, z, F) => Lo(M, a, l, !0) ? 1 : Math.max(z, z * n, F, F * n),
-            w = (M, z, F) => Lo(M, a, l, !0) ? -1 : Math.min(z, z * n, F, F * n),
-            S = x(0, c, g),
+            x = (P, z, F) => Lo(P, a, l, !0) ? 1 : Math.max(z, z * n, F, F * n),
+            _ = (P, z, F) => Lo(P, a, l, !0) ? -1 : Math.min(z, z * n, F, F * n),
+            C = x(0, c, g),
             A = x($e, d, y),
-            _ = w(Ce, c, g),
-            C = w(Ce + $e, d, y);
-        i = (S - _) / 2, r = (A - C) / 2, o = -(S + _) / 2, s = -(A + C) / 2
+            w = _(Ce, c, g),
+            k = _(Ce + $e, d, y);
+        i = (C - w) / 2, r = (A - k) / 2, o = -(C + w) / 2, s = -(A + k) / 2
     }
     return {
         ratioX: i,
         ratioY: r,
         offsetX: o,
         offsetY: s
     }
 }
-var Pl = class extends Mi {
+var Pl = class extends Pi {
         static id = "doughnut";
         static defaults = {
             datasetElementType: !1,
             dataElementType: "arc",
             animation: {
                 animateRotate: !0,
                 animateScale: !1
@@ -11697,33 +11697,33 @@
                 {
                     chartArea: i
                 } = n,
                 r = this._cachedMeta,
                 o = r.data,
                 s = this.getMaxBorderWidth() + this.getMaxOffset(o) + this.options.spacing,
                 a = Math.max((Math.min(i.width, i.height) - s) / 2, 0),
-                l = Math.min(Cp(this.options.cutout, a), 1),
+                l = Math.min(kp(this.options.cutout, a), 1),
                 c = this._getRingWeight(this.index),
                 {
                     circumference: d,
                     rotation: g
                 } = this._getRotationExtents(),
                 {
                     ratioX: y,
                     ratioY: x,
-                    offsetX: w,
-                    offsetY: S
+                    offsetX: _,
+                    offsetY: C
                 } = UC(g, d, l),
                 A = (i.width - s) / y,
-                _ = (i.height - s) / x,
-                C = Math.max(Math.min(A, _) / 2, 0),
-                M = Dc(this.options.radius, C),
-                z = Math.max(M * l, 0),
-                F = (M - z) / this._getVisibleDatasetWeightTotal();
-            this.offsetX = w * M, this.offsetY = S * M, r.total = this.calculateTotal(), this.outerRadius = M - F * this._getRingWeightOffset(this.index), this.innerRadius = Math.max(this.outerRadius - F * c, 0), this.updateElements(o, 0, o.length, e)
+                w = (i.height - s) / x,
+                k = Math.max(Math.min(A, w) / 2, 0),
+                P = Oc(this.options.radius, k),
+                z = Math.max(P * l, 0),
+                F = (P - z) / this._getVisibleDatasetWeightTotal();
+            this.offsetX = _ * P, this.offsetY = C * P, r.total = this.calculateTotal(), this.outerRadius = P - F * this._getRingWeightOffset(this.index), this.innerRadius = Math.max(this.outerRadius - F * c, 0), this.updateElements(o, 0, o.length, e)
         }
         _circumference(e, n) {
             let i = this.options,
                 r = this._cachedMeta,
                 o = this._getCircumference();
             return n && i.animation.animateRotate || !this.chart.getDataVisibility(e) || r._parsed[e] === null || r.data[e].hidden ? 0 : this.calculateCircumference(r._parsed[e] * o / We)
         }
@@ -11732,35 +11732,35 @@
                 s = this.chart,
                 a = s.chartArea,
                 c = s.options.animation,
                 d = (a.left + a.right) / 2,
                 g = (a.top + a.bottom) / 2,
                 y = o && c.animateScale,
                 x = y ? 0 : this.innerRadius,
-                w = y ? 0 : this.outerRadius,
+                _ = y ? 0 : this.outerRadius,
                 {
-                    sharedOptions: S,
+                    sharedOptions: C,
                     includeOptions: A
                 } = this._getSharedOptions(n, r),
-                _ = this._getRotation(),
-                C;
-            for (C = 0; C < n; ++C) _ += this._circumference(C, o);
-            for (C = n; C < n + i; ++C) {
-                let M = this._circumference(C, o),
-                    z = e[C],
+                w = this._getRotation(),
+                k;
+            for (k = 0; k < n; ++k) w += this._circumference(k, o);
+            for (k = n; k < n + i; ++k) {
+                let P = this._circumference(k, o),
+                    z = e[k],
                     F = {
                         x: d + this.offsetX,
                         y: g + this.offsetY,
-                        startAngle: _,
-                        endAngle: _ + M,
-                        circumference: M,
-                        outerRadius: w,
+                        startAngle: w,
+                        endAngle: w + P,
+                        circumference: P,
+                        outerRadius: _,
                         innerRadius: x
                     };
-                A && (F.options = S || this.resolveDataElementOptions(C, z.active ? "active" : r)), _ += M, this.updateElement(z, C, F, r)
+                A && (F.options = C || this.resolveDataElementOptions(k, z.active ? "active" : r)), w += P, this.updateElement(z, k, F, r)
             }
         }
         calculateTotal() {
             let e = this._cachedMeta,
                 n = e.data,
                 i = 0,
                 r;
@@ -11815,15 +11815,15 @@
         _getRingWeight(e) {
             return Math.max(pe(this.chart.data.datasets[e].weight, 1), 0)
         }
         _getVisibleDatasetWeightTotal() {
             return this._getRingWeightOffset(this.chart.data.datasets.length) || 1
         }
     },
-    sg = class extends Mi {
+    og = class extends Pi {
         static id = "line";
         static defaults = {
             datasetElementType: "line",
             dataElementType: "point",
             showLine: !0,
             spanGaps: !1
         };
@@ -11847,16 +11847,16 @@
                     data: r = [],
                     _dataset: o
                 } = n,
                 s = this.chart._animationsDisabled,
                 {
                     start: a,
                     count: l
-                } = Hc(n, r, s);
-            this._drawStart = a, this._drawCount = l, Bc(n) && (a = 0, l = r.length), i._chart = this.chart, i._datasetIndex = this.index, i._decimated = !!o._decimated, i.points = r;
+                } = Bc(n, r, s);
+            this._drawStart = a, this._drawCount = l, Wc(n) && (a = 0, l = r.length), i._chart = this.chart, i._datasetIndex = this.index, i._decimated = !!o._decimated, i.points = r;
             let c = this.resolveDatasetElementOptions(e);
             this.options.showLine || (c.borderWidth = 0), c.segment = this.options.segment, this.updateElement(i, void 0, {
                 animated: !s,
                 options: c
             }, e), this.updateElements(r, a, l, e)
         }
         updateElements(e, n, i, r) {
@@ -11870,34 +11870,34 @@
                 {
                     sharedOptions: d,
                     includeOptions: g
                 } = this._getSharedOptions(n, r),
                 y = s.axis,
                 x = a.axis,
                 {
-                    spanGaps: w,
-                    segment: S
+                    spanGaps: _,
+                    segment: C
                 } = this.options,
-                A = di(w) ? w : Number.POSITIVE_INFINITY,
-                _ = this.chart._animationsDisabled || o || r === "none",
-                C = n + i,
-                M = e.length,
+                A = di(_) ? _ : Number.POSITIVE_INFINITY,
+                w = this.chart._animationsDisabled || o || r === "none",
+                k = n + i,
+                P = e.length,
                 z = n > 0 && this.getParsed(n - 1);
-            for (let F = 0; F < M; ++F) {
+            for (let F = 0; F < P; ++F) {
                 let h = e[F],
-                    Y = _ ? h : {};
-                if (F < n || F >= C) {
-                    Y.skip = !0;
+                    $ = w ? h : {};
+                if (F < n || F >= k) {
+                    $.skip = !0;
                     continue
                 }
-                let V = this.getParsed(F),
-                    te = Ie(V[x]),
-                    ie = Y[y] = s.getPixelForValue(V[y], F),
-                    ce = Y[x] = o || te ? a.getBasePixel() : a.getPixelForValue(l ? this.applyStack(a, V, l) : V[x], F);
-                Y.skip = isNaN(ie) || isNaN(ce) || te, Y.stop = F > 0 && Math.abs(V[y] - z[y]) > A, S && (Y.parsed = V, Y.raw = c.data[F]), g && (Y.options = d || this.resolveDataElementOptions(F, h.active ? "active" : r)), _ || this.updateElement(h, F, Y, r), z = V
+                let Y = this.getParsed(F),
+                    ne = Ie(Y[x]),
+                    ie = $[y] = s.getPixelForValue(Y[y], F),
+                    ce = $[x] = o || ne ? a.getBasePixel() : a.getPixelForValue(l ? this.applyStack(a, Y, l) : Y[x], F);
+                $.skip = isNaN(ie) || isNaN(ce) || ne, $.stop = F > 0 && Math.abs(Y[y] - z[y]) > A, C && ($.parsed = Y, $.raw = c.data[F]), g && ($.options = d || this.resolveDataElementOptions(F, h.active ? "active" : r)), w || this.updateElement(h, F, $, r), z = Y
             }
         }
         getMaxOverflow() {
             let e = this._cachedMeta,
                 n = e.dataset,
                 i = n.options && n.options.borderWidth || 0,
                 r = e.data || [];
@@ -11907,15 +11907,15 @@
             return Math.max(i, o, s) / 2
         }
         draw() {
             let e = this._cachedMeta;
             e.dataset.updateControlPoints(this.chart.chartArea, e.iScale.axis), super.draw()
         }
     },
-    hf = class extends Mi {
+    pf = class extends Pi {
         static id = "polarArea";
         static defaults = {
             dataElementType: "arc",
             animation: {
                 animateRotate: !0,
                 animateScale: !0
             },
@@ -11991,15 +11991,15 @@
                 o = Ro(n._parsed[e].r, i.options.locale);
             return {
                 label: r[e] || "",
                 value: o
             }
         }
         parseObjectData(e, n, i, r) {
-            return Zc.bind(this)(e, n, i, r)
+            return Kc.bind(this)(e, n, i, r)
         }
         update(e) {
             let n = this._cachedMeta.data;
             this._updateRadius(), this.updateElements(n, 0, n.length, e)
         }
         getMinMax() {
             let e = this._cachedMeta,
@@ -12027,55 +12027,55 @@
                 s = this.chart,
                 l = s.options.animation,
                 c = this._cachedMeta.rScale,
                 d = c.xCenter,
                 g = c.yCenter,
                 y = c.getIndexAngle(0) - .5 * Ce,
                 x = y,
-                w, S = 360 / this.countVisibleElements();
-            for (w = 0; w < n; ++w) x += this._computeAngle(w, r, S);
-            for (w = n; w < n + i; w++) {
-                let A = e[w],
-                    _ = x,
-                    C = x + this._computeAngle(w, r, S),
-                    M = s.getDataVisibility(w) ? c.getDistanceFromCenterForValue(this.getParsed(w).r) : 0;
-                x = C, o && (l.animateScale && (M = 0), l.animateRotate && (_ = C = y));
+                _, C = 360 / this.countVisibleElements();
+            for (_ = 0; _ < n; ++_) x += this._computeAngle(_, r, C);
+            for (_ = n; _ < n + i; _++) {
+                let A = e[_],
+                    w = x,
+                    k = x + this._computeAngle(_, r, C),
+                    P = s.getDataVisibility(_) ? c.getDistanceFromCenterForValue(this.getParsed(_).r) : 0;
+                x = k, o && (l.animateScale && (P = 0), l.animateRotate && (w = k = y));
                 let z = {
                     x: d,
                     y: g,
                     innerRadius: 0,
-                    outerRadius: M,
-                    startAngle: _,
-                    endAngle: C,
-                    options: this.resolveDataElementOptions(w, A.active ? "active" : r)
+                    outerRadius: P,
+                    startAngle: w,
+                    endAngle: k,
+                    options: this.resolveDataElementOptions(_, A.active ? "active" : r)
                 };
-                this.updateElement(A, w, z, r)
+                this.updateElement(A, _, z, r)
             }
         }
         countVisibleElements() {
             let e = this._cachedMeta,
                 n = 0;
             return e.data.forEach((i, r) => {
                 !isNaN(this.getParsed(r).r) && this.chart.getDataVisibility(r) && n++
             }), n
         }
         _computeAngle(e, n, i) {
             return this.chart.getDataVisibility(e) ? pt(this.resolveDataElementOptions(e, n).angle || i) : 0
         }
     },
-    ag = class extends Pl {
+    sg = class extends Pl {
         static id = "pie";
         static defaults = {
             cutout: 0,
             rotation: 0,
             circumference: 360,
             radius: "100%"
         }
     },
-    lg = class extends Mi {
+    ag = class extends Pi {
         static id = "radar";
         static defaults = {
             datasetElementType: "line",
             dataElementType: "point",
             indexAxis: "r",
             showLine: !0,
             elements: {
@@ -12097,15 +12097,15 @@
                 i = this.getParsed(e);
             return {
                 label: n.getLabels()[e],
                 value: "" + n.getLabelForValue(i[n.axis])
             }
         }
         parseObjectData(e, n, i, r) {
-            return Zc.bind(this)(e, n, i, r)
+            return Kc.bind(this)(e, n, i, r)
         }
         update(e) {
             let n = this._cachedMeta,
                 i = n.dataset,
                 r = n.data || [],
                 o = n.iScale.getLabels();
             if (i.points = r, e !== "resize") {
@@ -12136,15 +12136,15 @@
                         skip: isNaN(g) || isNaN(y),
                         options: c
                     };
                 this.updateElement(l, a, x, r)
             }
         }
     },
-    ug = class extends Mi {
+    lg = class extends Pi {
         static id = "scatter";
         static defaults = {
             datasetElementType: !1,
             dataElementType: "point",
             showLine: !1,
             fill: !1
         };
@@ -12181,16 +12181,16 @@
                 {
                     data: i = []
                 } = n,
                 r = this.chart._animationsDisabled,
                 {
                     start: o,
                     count: s
-                } = Hc(n, i, r);
-            if (this._drawStart = o, this._drawCount = s, Bc(n) && (o = 0, s = i.length), this.options.showLine) {
+                } = Bc(n, i, r);
+            if (this._drawStart = o, this._drawCount = s, Wc(n) && (o = 0, s = i.length), this.options.showLine) {
                 this.datasetElementType || this.addElements();
                 let {
                     dataset: a,
                     _dataset: l
                 } = n;
                 a._chart = this.chart, a._datasetIndex = this.index, a._decimated = !!l._decimated, a.points = i;
                 let c = this.resolveDatasetElementOptions(e);
@@ -12215,30 +12215,30 @@
                     _stacked: l,
                     _dataset: c
                 } = this._cachedMeta,
                 d = this.resolveDataElementOptions(n, r),
                 g = this.getSharedOptions(d),
                 y = this.includeOptions(r, g),
                 x = s.axis,
-                w = a.axis,
+                _ = a.axis,
                 {
-                    spanGaps: S,
+                    spanGaps: C,
                     segment: A
                 } = this.options,
-                _ = di(S) ? S : Number.POSITIVE_INFINITY,
-                C = this.chart._animationsDisabled || o || r === "none",
-                M = n > 0 && this.getParsed(n - 1);
+                w = di(C) ? C : Number.POSITIVE_INFINITY,
+                k = this.chart._animationsDisabled || o || r === "none",
+                P = n > 0 && this.getParsed(n - 1);
             for (let z = n; z < n + i; ++z) {
                 let F = e[z],
                     h = this.getParsed(z),
-                    Y = C ? F : {},
-                    V = Ie(h[w]),
-                    te = Y[x] = s.getPixelForValue(h[x], z),
-                    ie = Y[w] = o || V ? a.getBasePixel() : a.getPixelForValue(l ? this.applyStack(a, h, l) : h[w], z);
-                Y.skip = isNaN(te) || isNaN(ie) || V, Y.stop = z > 0 && Math.abs(h[x] - M[x]) > _, A && (Y.parsed = h, Y.raw = c.data[z]), y && (Y.options = g || this.resolveDataElementOptions(z, F.active ? "active" : r)), C || this.updateElement(F, z, Y, r), M = h
+                    $ = k ? F : {},
+                    Y = Ie(h[_]),
+                    ne = $[x] = s.getPixelForValue(h[x], z),
+                    ie = $[_] = o || Y ? a.getBasePixel() : a.getPixelForValue(l ? this.applyStack(a, h, l) : h[_], z);
+                $.skip = isNaN(ne) || isNaN(ie) || Y, $.stop = z > 0 && Math.abs(h[x] - P[x]) > w, A && ($.parsed = h, $.raw = c.data[z]), y && ($.options = g || this.resolveDataElementOptions(z, F.active ? "active" : r)), k || this.updateElement(F, z, $, r), P = h
             }
             this.updateSharedOptions(g, r, d)
         }
         getMaxOverflow() {
             let e = this._cachedMeta,
                 n = e.data || [];
             if (!this.options.showLine) {
@@ -12252,28 +12252,28 @@
             let o = n[0].size(this.resolveDataElementOptions(0)),
                 s = n[n.length - 1].size(this.resolveDataElementOptions(n.length - 1));
             return Math.max(r, o, s) / 2
         }
     },
     $C = Object.freeze({
         __proto__: null,
-        BarController: rg,
-        BubbleController: og,
+        BarController: ig,
+        BubbleController: rg,
         DoughnutController: Pl,
-        LineController: sg,
-        PieController: ag,
-        PolarAreaController: hf,
-        RadarController: lg,
-        ScatterController: ug
+        LineController: og,
+        PieController: sg,
+        PolarAreaController: pf,
+        RadarController: ag,
+        ScatterController: lg
     });
 
 function No() {
     throw new Error("This method is not implemented: Check that a complete date adapter is provided.")
 }
-var cg = class t {
+var ug = class t {
         static override(e) {
             Object.assign(t.prototype, e)
         }
         options;
         constructor(e) {
             this.options = e || {}
         }
@@ -12297,25 +12297,25 @@
             return No()
         }
         endOf() {
             return No()
         }
     },
     YC = {
-        _date: cg
+        _date: ug
     };
 
 function XC(t, e, n, i) {
     let {
         controller: r,
         data: o,
         _sorted: s
     } = t, a = r._cachedMeta.iScale;
     if (a && e === a.axis && e !== "r" && s && o.length) {
-        let l = a._reversePixels ? Dp : ui;
+        let l = a._reversePixels ? Pp : ui;
         if (i) {
             if (r._sharedOptions) {
                 let c = o[0],
                     d = typeof c.getRange == "function" && c.getRange(e);
                 if (d) {
                     let g = l(o, e, n - d),
                         y = l(o, e, n + d);
@@ -12329,45 +12329,45 @@
     }
     return {
         lo: 0,
         hi: o.length - 1
     }
 }
 
-function Ll(t, e, n, i, r) {
+function Rl(t, e, n, i, r) {
     let o = t.getSortedVisibleDatasetMetas(),
         s = n[e];
     for (let a = 0, l = o.length; a < l; ++a) {
         let {
             index: c,
             data: d
         } = o[a], {
             lo: g,
             hi: y
         } = XC(o[a], e, s, r);
         for (let x = g; x <= y; ++x) {
-            let w = d[x];
-            w.skip || i(w, c, x)
+            let _ = d[x];
+            _.skip || i(_, c, x)
         }
     }
 }
 
 function qC(t) {
     let e = t.indexOf("x") !== -1,
         n = t.indexOf("y") !== -1;
     return function(i, r) {
         let o = e ? Math.abs(i.x - r.x) : 0,
             s = n ? Math.abs(i.y - r.y) : 0;
         return Math.sqrt(Math.pow(o, 2) + Math.pow(s, 2))
     }
 }
 
-function Gp(t, e, n, i, r) {
+function Zp(t, e, n, i, r) {
     let o = [];
-    return !r && !t.isPointInArea(e) || Ll(t, n, e, function(a, l, c) {
+    return !r && !t.isPointInArea(e) || Rl(t, n, e, function(a, l, c) {
         !r && !ci(a, t.chartArea, 0) || a.inRange(e.x, e.y, i) && o.push({
             element: a,
             datasetIndex: l,
             index: c
         })
     }, !0), o
 }
@@ -12377,75 +12377,75 @@
 
     function o(s, a, l) {
         let {
             startAngle: c,
             endAngle: d
         } = s.getProps(["startAngle", "endAngle"], i), {
             angle: g
-        } = Ic(s, {
+        } = Nc(s, {
             x: e.x,
             y: e.y
         });
         Lo(g, c, d) && r.push({
             element: s,
             datasetIndex: a,
             index: l
         })
     }
-    return Ll(t, n, e, o), r
+    return Rl(t, n, e, o), r
 }
 
-function GC(t, e, n, i, r, o) {
+function KC(t, e, n, i, r, o) {
     let s = [],
         a = qC(n),
         l = Number.POSITIVE_INFINITY;
 
     function c(d, g, y) {
         let x = d.inRange(e.x, e.y, r);
         if (i && !x) return;
-        let w = d.getCenterPoint(r);
-        if (!(!!o || t.isPointInArea(w)) && !x) return;
-        let A = a(e, w);
+        let _ = d.getCenterPoint(r);
+        if (!(!!o || t.isPointInArea(_)) && !x) return;
+        let A = a(e, _);
         A < l ? (s = [{
             element: d,
             datasetIndex: g,
             index: y
         }], l = A) : A === l && s.push({
             element: d,
             datasetIndex: g,
             index: y
         })
     }
-    return Ll(t, n, e, c), s
+    return Rl(t, n, e, c), s
 }
 
-function Qp(t, e, n, i, r, o) {
-    return !o && !t.isPointInArea(e) ? [] : n === "r" && !i ? ZC(t, e, n, r) : GC(t, e, n, i, r, o)
+function Kp(t, e, n, i, r, o) {
+    return !o && !t.isPointInArea(e) ? [] : n === "r" && !i ? ZC(t, e, n, r) : KC(t, e, n, i, r, o)
 }
 
 function qx(t, e, n, i, r) {
     let o = [],
         s = n === "x" ? "inXRange" : "inYRange",
         a = !1;
-    return Ll(t, n, e, (l, c, d) => {
+    return Rl(t, n, e, (l, c, d) => {
         l[s](e[n], r) && (o.push({
             element: l,
             datasetIndex: c,
             index: d
         }), a = a || l.inRange(e.x, e.y, r))
     }), i && !a ? [] : o
 }
-var QC = {
-        evaluateInteractionItems: Ll,
+var GC = {
+        evaluateInteractionItems: Rl,
         modes: {
             index(t, e, n, i) {
                 let r = zn(e, t),
                     o = n.axis || "x",
                     s = n.includeInvisible || !1,
-                    a = n.intersect ? Gp(t, r, o, i, s) : Qp(t, r, o, !1, i, s),
+                    a = n.intersect ? Zp(t, r, o, i, s) : Kp(t, r, o, !1, i, s),
                     l = [];
                 return a.length ? (t.getSortedVisibleDatasetMetas().forEach(c => {
                     let d = a[0].index,
                         g = c.data[d];
                     g && !g.skip && l.push({
                         element: g,
                         datasetIndex: c.index,
@@ -12453,15 +12453,15 @@
                     })
                 }), l) : []
             },
             dataset(t, e, n, i) {
                 let r = zn(e, t),
                     o = n.axis || "xy",
                     s = n.includeInvisible || !1,
-                    a = n.intersect ? Gp(t, r, o, i, s) : Qp(t, r, o, !1, i, s);
+                    a = n.intersect ? Zp(t, r, o, i, s) : Kp(t, r, o, !1, i, s);
                 if (a.length > 0) {
                     let l = a[0].datasetIndex,
                         c = t.getDatasetMeta(l).data;
                     a = [];
                     for (let d = 0; d < c.length; ++d) a.push({
                         element: c[d],
                         datasetIndex: l,
@@ -12470,35 +12470,35 @@
                 }
                 return a
             },
             point(t, e, n, i) {
                 let r = zn(e, t),
                     o = n.axis || "xy",
                     s = n.includeInvisible || !1;
-                return Gp(t, r, o, i, s)
+                return Zp(t, r, o, i, s)
             },
             nearest(t, e, n, i) {
                 let r = zn(e, t),
                     o = n.axis || "xy",
                     s = n.includeInvisible || !1;
-                return Qp(t, r, o, n.intersect, i, s)
+                return Kp(t, r, o, n.intersect, i, s)
             },
             x(t, e, n, i) {
                 let r = zn(e, t);
                 return qx(t, r, "x", n.intersect, i)
             },
             y(t, e, n, i) {
                 let r = zn(e, t);
                 return qx(t, r, "y", n.intersect, i)
             }
         }
     },
     Hb = ["left", "top", "right", "bottom"];
 
-function wl(t, e) {
+function Sl(t, e) {
     return t.filter(n => n.pos === e)
 }
 
 function Zx(t, e) {
     return t.filter(n => Hb.indexOf(n.pos) === -1 && n.box.axis === e)
 }
 
@@ -12506,15 +12506,15 @@
     return t.sort((n, i) => {
         let r = e ? i : n,
             o = e ? n : i;
         return r.weight === o.weight ? r.index - o.index : r.weight - o.weight
     })
 }
 
-function KC(t) {
+function QC(t) {
     let e = [],
         n, i, r, o, s, a;
     for (n = 0, i = (t || []).length; n < i; ++n) r = t[n], {
         position: o,
         options: {
             stack: s,
             stackWeight: a = 1
@@ -12565,33 +12565,33 @@
         } = a.box, c = n[a.stack], d = c && a.stackWeight / c.weight;
         a.horizontal ? (a.width = d ? d * i : l && e.availableWidth, a.height = r) : (a.width = i, a.height = d ? d * r : l && e.availableHeight)
     }
     return n
 }
 
 function tE(t) {
-    let e = KC(t),
+    let e = QC(t),
         n = kl(e.filter(c => c.box.fullSize), !0),
-        i = kl(wl(e, "left"), !0),
-        r = kl(wl(e, "right")),
-        o = kl(wl(e, "top"), !0),
-        s = kl(wl(e, "bottom")),
+        i = kl(Sl(e, "left"), !0),
+        r = kl(Sl(e, "right")),
+        o = kl(Sl(e, "top"), !0),
+        s = kl(Sl(e, "bottom")),
         a = Zx(e, "x"),
         l = Zx(e, "y");
     return {
         fullSize: n,
         leftAndTop: i.concat(o),
         rightAndBottom: r.concat(l).concat(s).concat(a),
-        chartArea: wl(e, "chartArea"),
+        chartArea: Sl(e, "chartArea"),
         vertical: i.concat(r).concat(l),
         horizontal: o.concat(s).concat(a)
     }
 }
 
-function Gx(t, e, n, i) {
+function Kx(t, e, n, i) {
     return Math.max(t[n], e[n]) + Math.max(t[i], e[i])
 }
 
 function Bb(t, e) {
     t.top = Math.max(t.top, e.top), t.left = Math.max(t.left, e.left), t.bottom = Math.max(t.bottom, e.bottom), t.right = Math.max(t.right, e.right)
 }
 
@@ -12605,16 +12605,16 @@
         let g = i[n.stack] || {
             size: 0,
             count: 1
         };
         g.size = Math.max(g.size, n.horizontal ? o.height : o.width), n.size = g.size / g.count, t[r] += n.size
     }
     o.getPadding && Bb(s, o.getPadding());
-    let a = Math.max(0, e.outerWidth - Gx(s, t, "left", "right")),
-        l = Math.max(0, e.outerHeight - Gx(s, t, "top", "bottom")),
+    let a = Math.max(0, e.outerWidth - Kx(s, t, "left", "right")),
+        l = Math.max(0, e.outerHeight - Kx(s, t, "top", "bottom")),
         c = a !== t.w,
         d = l !== t.h;
     return t.w = a, t.h = l, n.horizontal ? {
         same: c,
         other: d
     } : {
         same: d,
@@ -12645,33 +12645,33 @@
         return r.forEach(s => {
             o[s] = Math.max(e[s], n[s])
         }), o
     }
     return i(t ? ["left", "right"] : ["top", "bottom"])
 }
 
-function El(t, e, n, i) {
+function Tl(t, e, n, i) {
     let r = [],
         o, s, a, l, c, d;
     for (o = 0, s = t.length, c = 0; o < s; ++o) {
         a = t[o], l = a.box, l.update(a.width || e.w, a.height || e.h, rE(a.horizontal, e));
         let {
             same: g,
             other: y
         } = nE(e, n, a, i);
         c |= g && r.length, d = d || y, l.fullSize || r.push(a)
     }
-    return c && El(r, e, n, i) || d
+    return c && Tl(r, e, n, i) || d
 }
 
-function rf(t, e, n, i, r) {
+function of(t, e, n, i, r) {
     t.top = n, t.left = e, t.right = e + i, t.bottom = n + r, t.width = i, t.height = r
 }
 
-function Qx(t, e, n, i) {
+function Gx(t, e, n, i) {
     let r = n.padding,
         {
             x: o,
             y: s
         } = e;
     for (let a of t) {
         let l = a.box,
@@ -12680,19 +12680,19 @@
                 placed: 0,
                 weight: 1
             },
             d = a.stackWeight / c.weight || 1;
         if (a.horizontal) {
             let g = e.w * d,
                 y = c.size || l.height;
-            Ut(c.start) && (s = c.start), l.fullSize ? rf(l, r.left, s, n.outerWidth - r.right - r.left, y) : rf(l, e.left + c.placed, s, g, y), c.start = s, c.placed += g, s = l.bottom
+            Ut(c.start) && (s = c.start), l.fullSize ? of(l, r.left, s, n.outerWidth - r.right - r.left, y) : of(l, e.left + c.placed, s, g, y), c.start = s, c.placed += g, s = l.bottom
         } else {
             let g = e.h * d,
                 y = c.size || l.width;
-            Ut(c.start) && (o = c.start), l.fullSize ? rf(l, o, r.top, y, n.outerHeight - r.bottom - r.top) : rf(l, o, e.top + c.placed, y, g), c.start = o, c.placed += g, o = l.right
+            Ut(c.start) && (o = c.start), l.fullSize ? of(l, o, r.top, y, n.outerHeight - r.bottom - r.top) : of(l, o, e.top + c.placed, y, g), c.start = o, c.placed += g, o = l.right
         }
     }
     e.x = o, e.y = s
 }
 var Jt = {
         addBox(t, e) {
             t.boxes || (t.boxes = []), e.fullSize = e.fullSize || !1, e.position = e.position || "top", e.weight = e.weight || 0, e._layers = e._layers || function() {
@@ -12715,18 +12715,18 @@
             if (!t) return;
             let r = gt(t.options.layout.padding),
                 o = Math.max(e - r.width, 0),
                 s = Math.max(n - r.height, 0),
                 a = tE(t.boxes),
                 l = a.vertical,
                 c = a.horizontal;
-            Se(t.boxes, S => {
-                typeof S.beforeLayout == "function" && S.beforeLayout()
+            ke(t.boxes, C => {
+                typeof C.beforeLayout == "function" && C.beforeLayout()
             });
-            let d = l.reduce((S, A) => A.box.options && A.box.options.display === !1 ? S : S + 1, 0) || 1,
+            let d = l.reduce((C, A) => A.box.options && A.box.options.display === !1 ? C : C + 1, 0) || 1,
                 g = Object.freeze({
                     outerWidth: e,
                     outerHeight: n,
                     padding: r,
                     availableWidth: o,
                     availableHeight: s,
                     vBoxMaxWidth: o / 2 / d,
@@ -12737,34 +12737,34 @@
             let x = Object.assign({
                     maxPadding: y,
                     w: o,
                     h: s,
                     x: r.left,
                     y: r.top
                 }, r),
-                w = eE(l.concat(c), g);
-            El(a.fullSize, x, g, w), El(l, x, g, w), El(c, x, g, w) && El(l, x, g, w), iE(x), Qx(a.leftAndTop, x, g, w), x.x += x.w, x.y += x.h, Qx(a.rightAndBottom, x, g, w), t.chartArea = {
+                _ = eE(l.concat(c), g);
+            Tl(a.fullSize, x, g, _), Tl(l, x, g, _), Tl(c, x, g, _) && Tl(l, x, g, _), iE(x), Gx(a.leftAndTop, x, g, _), x.x += x.w, x.y += x.h, Gx(a.rightAndBottom, x, g, _), t.chartArea = {
                 left: x.left,
                 top: x.top,
                 right: x.left + x.w,
                 bottom: x.top + x.h,
                 height: x.h,
                 width: x.w
-            }, Se(a.chartArea, S => {
-                let A = S.box;
+            }, ke(a.chartArea, C => {
+                let A = C.box;
                 Object.assign(A, t.chartArea), A.update(x.w, x.h, {
                     left: 0,
                     top: 0,
                     right: 0,
                     bottom: 0
                 })
             })
         }
     },
-    pf = class {
+    gf = class {
         acquireContext(e, n) {}
         releaseContext(e) {
             return !1
         }
         addEventListener(e, n, i) {}
         removeEventListener(e, n, i) {}
         getDevicePixelRatio() {
@@ -12777,62 +12777,62 @@
             }
         }
         isAttached(e) {
             return !0
         }
         updateConfig(e) {}
     },
-    fg = class extends pf {
+    cg = class extends gf {
         acquireContext(e) {
             return e && e.getContext && e.getContext("2d") || null
         }
         updateConfig(e) {
             e.options.animation = !1
         }
     },
-    ff = "$chartjs",
+    df = "$chartjs",
     oE = {
         touchstart: "mousedown",
         touchmove: "mousemove",
         touchend: "mouseup",
         pointerenter: "mouseenter",
         pointerdown: "mousedown",
         pointermove: "mousemove",
         pointerup: "mouseup",
         pointerleave: "mouseout",
         pointerout: "mouseout"
     },
-    Kx = t => t === null || t === "";
+    Qx = t => t === null || t === "";
 
 function sE(t, e) {
     let n = t.style,
         i = t.getAttribute("height"),
         r = t.getAttribute("width");
-    if (t[ff] = {
+    if (t[df] = {
             initial: {
                 height: i,
                 width: r,
                 style: {
                     display: n.display,
                     height: n.height,
                     width: n.width
                 }
             }
-        }, n.display = n.display || "block", n.boxSizing = n.boxSizing || "border-box", Kx(r)) {
-        let o = Kc(t, "width");
+        }, n.display = n.display || "block", n.boxSizing = n.boxSizing || "border-box", Qx(r)) {
+        let o = Jc(t, "width");
         o !== void 0 && (t.width = o)
     }
-    if (Kx(i))
+    if (Qx(i))
         if (t.style.height === "") t.height = t.width / (e || 2);
         else {
-            let o = Kc(t, "height");
+            let o = Jc(t, "height");
             o !== void 0 && (t.height = o)
         } return t
 }
-var Wb = Vp ? {
+var Wb = Wp ? {
     passive: !0
 } : !1;
 
 function aE(t, e, n) {
     t && t.addEventListener(e, n, Wb)
 }
 
@@ -12851,37 +12851,37 @@
         chart: e,
         native: t,
         x: i !== void 0 ? i : null,
         y: r !== void 0 ? r : null
     }
 }
 
-function gf(t, e) {
+function mf(t, e) {
     for (let n of t)
         if (n === e || n.contains(e)) return !0
 }
 
 function cE(t, e, n) {
     let i = t.canvas,
         r = new MutationObserver(o => {
             let s = !1;
-            for (let a of o) s = s || gf(a.addedNodes, i), s = s && !gf(a.removedNodes, i);
+            for (let a of o) s = s || mf(a.addedNodes, i), s = s && !mf(a.removedNodes, i);
             s && n()
         });
     return r.observe(document, {
         childList: !0,
         subtree: !0
     }), r
 }
 
 function fE(t, e, n) {
     let i = t.canvas,
         r = new MutationObserver(o => {
             let s = !1;
-            for (let a of o) s = s || gf(a.removedNodes, i), s = s && !gf(a.addedNodes, i);
+            for (let a of o) s = s || mf(a.removedNodes, i), s = s && !mf(a.addedNodes, i);
             s && n()
         });
     return r.observe(document, {
         childList: !0,
         subtree: !0
     }), r
 }
@@ -12901,57 +12901,57 @@
 
 function hE(t) {
     Ml.delete(t), Ml.size || window.removeEventListener("resize", Vb)
 }
 
 function pE(t, e, n) {
     let i = t.canvas,
-        r = i && bl(i);
+        r = i && _l(i);
     if (!r) return;
-    let o = jc((a, l) => {
+    let o = Hc((a, l) => {
             let c = r.clientWidth;
             n(a, l), c < r.clientWidth && n()
         }, window),
         s = new ResizeObserver(a => {
             let l = a[0],
                 c = l.contentRect.width,
                 d = l.contentRect.height;
             c === 0 && d === 0 || o(c, d)
         });
     return s.observe(r), dE(t, o), s
 }
 
-function Kp(t, e, n) {
+function Gp(t, e, n) {
     n && n.disconnect(), e === "resize" && hE(t)
 }
 
 function gE(t, e, n) {
     let i = t.canvas,
-        r = jc(o => {
+        r = Hc(o => {
             t.ctx !== null && n(uE(o, t))
         }, t);
     return aE(i, e, r), r
 }
-var dg = class extends pf {
+var fg = class extends gf {
     acquireContext(e, n) {
         let i = e && e.getContext && e.getContext("2d");
         return i && i.canvas === e ? (sE(e, n), i) : null
     }
     releaseContext(e) {
         let n = e.canvas;
-        if (!n[ff]) return !1;
-        let i = n[ff].initial;
+        if (!n[df]) return !1;
+        let i = n[df].initial;
         ["height", "width"].forEach(o => {
             let s = i[o];
             Ie(s) ? n.removeAttribute(o) : n.setAttribute(o, s)
         });
         let r = i.style || {};
         return Object.keys(r).forEach(o => {
             n.style[o] = r[o]
-        }), n.width = n.width, delete n[ff], !0
+        }), n.width = n.width, delete n[df], !0
     }
     addEventListener(e, n, i) {
         this.removeEventListener(e, n);
         let r = e.$proxies || (e.$proxies = {}),
             s = {
                 attach: cE,
                 detach: fE,
@@ -12960,33 +12960,33 @@
         r[n] = s(e, n, i)
     }
     removeEventListener(e, n) {
         let i = e.$proxies || (e.$proxies = {}),
             r = i[n];
         if (!r) return;
         ({
-            attach: Kp,
-            detach: Kp,
-            resize: Kp
+            attach: Gp,
+            detach: Gp,
+            resize: Gp
         } [n] || lE)(e, n, r), i[n] = void 0
     }
     getDevicePixelRatio() {
         return window.devicePixelRatio
     }
     getMaximumSize(e, n, i, r) {
-        return Wp(e, n, i, r)
+        return Bp(e, n, i, r)
     }
     isAttached(e) {
-        let n = bl(e);
+        let n = _l(e);
         return !!(n && n.isConnected)
     }
 };
 
 function mE(t) {
-    return !xl() || typeof OffscreenCanvas < "u" && t instanceof OffscreenCanvas ? fg : dg
+    return !bl() || typeof OffscreenCanvas < "u" && t instanceof OffscreenCanvas ? cg : fg
 }
 var zt = class {
     static defaults = {};
     static defaultRoutes = void 0;
     x;
     y;
     active = !1;
@@ -13024,33 +13024,33 @@
         a = o[0],
         l = o[s - 1],
         c = [];
     if (s > r) return _E(e, c, o, s / r), c;
     let d = xE(o, e, r);
     if (s > 0) {
         let g, y, x = s > 1 ? Math.round((l - a) / (s - 1)) : null;
-        for (of(e, c, d, Ie(x) ? 0 : a - x, a), g = 0, y = s - 1; g < y; g++) of(e, c, d, o[g], o[g + 1]);
-        return of(e, c, d, l, Ie(x) ? e.length : l + x), c
+        for (sf(e, c, d, Ie(x) ? 0 : a - x, a), g = 0, y = s - 1; g < y; g++) sf(e, c, d, o[g], o[g + 1]);
+        return sf(e, c, d, l, Ie(x) ? e.length : l + x), c
     }
-    return of(e, c, d), c
+    return sf(e, c, d), c
 }
 
 function vE(t) {
     let e = t.options.offset,
         n = t._tickSize(),
         i = t._length / n + (e ? 0 : 1),
         r = t._maxLength / n;
     return Math.floor(Math.min(i, r))
 }
 
 function xE(t, e, n) {
     let i = wE(t),
         r = e.length / n;
     if (!i) return Math.max(r, 1);
-    let o = Tp(i);
+    let o = Ep(i);
     for (let s = 0, a = o.length - 1; s < a; s++) {
         let l = o[s];
         if (l > r) return l
     }
     return Math.max(r, 1)
 }
 
@@ -13064,15 +13064,15 @@
 function _E(t, e, n, i) {
     let r = 0,
         o = n[0],
         s;
     for (i = Math.ceil(i), s = 0; s < t.length; s++) s === o && (e.push(t[s]), r++, o = n[r * i])
 }
 
-function of(t, e, n, i, r) {
+function sf(t, e, n, i, r) {
     let o = pe(i, 0),
         s = Math.min(pe(r, t.length), t.length),
         a = 0,
         l, c, d;
     for (n = Math.ceil(n), r && (l = r - i, n = l / Math.floor(l / n)), d = o; d < 0;) a++, d = Math.round(o + a * n);
     for (c = Math.max(o, 0); c < s; c++) c === d && (e.push(t[c]), a++, d = Math.round(o + a * n))
 }
@@ -13081,51 +13081,51 @@
     let e = t.length,
         n, i;
     if (e < 2) return !1;
     for (i = t[0], n = 1; n < e; ++n)
         if (t[n] - t[n - 1] !== i) return !1;
     return i
 }
-var kE = t => t === "left" ? "right" : t === "right" ? "left" : t,
+var SE = t => t === "left" ? "right" : t === "right" ? "left" : t,
     eb = (t, e, n) => e === "top" || e === "left" ? t[e] + n : t[e] - n,
     tb = (t, e) => Math.min(e || t, t);
 
 function nb(t, e) {
     let n = [],
         i = t.length / e,
         r = t.length,
         o = 0;
     for (; o < r; o += i) n.push(t[Math.floor(o)]);
     return n
 }
 
-function SE(t, e, n) {
+function kE(t, e, n) {
     let i = t.ticks.length,
         r = Math.min(e, i - 1),
         o = t._startPixel,
         s = t._endPixel,
         a = 1e-6,
         l = t.getPixelForTick(r),
         c;
     if (!(n && (i === 1 ? c = Math.max(l - o, s - l) : e === 0 ? c = (t.getPixelForTick(1) - l) / 2 : c = (l - t.getPixelForTick(r - 1)) / 2, l += r < e ? c : -c, l < o - a || l > s + a))) return l
 }
 
 function CE(t, e) {
-    Se(t, n => {
+    ke(t, n => {
         let i = n.gc,
             r = i.length / 2,
             o;
         if (r > e) {
             for (o = 0; o < r; ++o) delete n.data[i[o]];
             i.splice(0, r)
         }
     })
 }
 
-function Sl(t) {
+function Cl(t) {
     return t.drawTicks ? t.tickLength : 0
 }
 
 function ib(t, e) {
     if (!t.display) return 0;
     let n = tt(t.font, e),
         i = gt(t.padding);
@@ -13143,48 +13143,48 @@
     return Ei(t, {
         tick: n,
         index: e,
         type: "tick"
     })
 }
 
-function PE(t, e, n) {
-    let i = pl(t);
-    return (n && e !== "right" || !n && e === "right") && (i = kE(i)), i
+function DE(t, e, n) {
+    let i = gl(t);
+    return (n && e !== "right" || !n && e === "right") && (i = SE(i)), i
 }
 
-function ME(t, e, n, i) {
+function PE(t, e, n, i) {
     let {
         top: r,
         left: o,
         bottom: s,
         right: a,
         chart: l
     } = t, {
         chartArea: c,
         scales: d
-    } = l, g = 0, y, x, w, S = s - r, A = a - o;
+    } = l, g = 0, y, x, _, C = s - r, A = a - o;
     if (t.isHorizontal()) {
         if (x = Nt(i, o, a), we(n)) {
-            let _ = Object.keys(n)[0],
-                C = n[_];
-            w = d[_].getPixelForValue(C) + S - e
-        } else n === "center" ? w = (c.bottom + c.top) / 2 + S - e : w = eb(t, n, e);
+            let w = Object.keys(n)[0],
+                k = n[w];
+            _ = d[w].getPixelForValue(k) + C - e
+        } else n === "center" ? _ = (c.bottom + c.top) / 2 + C - e : _ = eb(t, n, e);
         y = a - o
     } else {
         if (we(n)) {
-            let _ = Object.keys(n)[0],
-                C = n[_];
-            x = d[_].getPixelForValue(C) - A + e
+            let w = Object.keys(n)[0],
+                k = n[w];
+            x = d[w].getPixelForValue(k) - A + e
         } else n === "center" ? x = (c.left + c.right) / 2 - A + e : x = eb(t, n, e);
-        w = Nt(i, s, r), g = n === "left" ? -$e : $e
+        _ = Nt(i, s, r), g = n === "left" ? -$e : $e
     }
     return {
         titleX: x,
-        titleY: w,
+        titleY: _,
         maxWidth: y,
         rotation: g
     }
 }
 var Fo = class t extends zt {
         constructor(e) {
             super(), this.id = e.id, this.type = e.type, this.options = void 0, this.ctx = e.ctx, this.chart = e.chart, this.top = void 0, this.bottom = void 0, this.left = void 0, this.right = void 0, this.width = void 0, this.height = void 0, this._margins = {
@@ -13263,15 +13263,15 @@
                 ticks: s
             } = this.options, a = s.sampleSize;
             this.beforeUpdate(), this.maxWidth = e, this.maxHeight = n, this._margins = i = Object.assign({
                 left: 0,
                 right: 0,
                 top: 0,
                 bottom: 0
-            }, i), this.ticks = null, this._labelSizes = null, this._gridLineItems = null, this._labelItems = null, this.beforeSetDimensions(), this.setDimensions(), this.afterSetDimensions(), this._maxLength = this.isHorizontal() ? this.width + i.left + i.right : this.height + i.top + i.bottom, this._dataLimitsCached || (this.beforeDataLimits(), this.determineDataLimits(), this.afterDataLimits(), this._range = Fp(this, o, r), this._dataLimitsCached = !0), this.beforeBuildTicks(), this.ticks = this.buildTicks() || [], this.afterBuildTicks();
+            }, i), this.ticks = null, this._labelSizes = null, this._gridLineItems = null, this._labelItems = null, this.beforeSetDimensions(), this.setDimensions(), this.afterSetDimensions(), this._maxLength = this.isHorizontal() ? this.width + i.left + i.right : this.height + i.top + i.bottom, this._dataLimitsCached || (this.beforeDataLimits(), this.determineDataLimits(), this.afterDataLimits(), this._range = zp(this, o, r), this._dataLimitsCached = !0), this.beforeBuildTicks(), this.ticks = this.buildTicks() || [], this.afterBuildTicks();
             let l = a < this.ticks.length;
             this._convertTicksToLabels(l ? nb(this.ticks, a) : this.ticks), this.configure(), this.beforeCalculateLabelRotation(), this.calculateLabelRotation(), this.afterCalculateLabelRotation(), s.display && (s.autoSkip || s.source === "auto") && (this.ticks = yE(this, this.ticks), this._labelSizes = null, this.afterAutoSkip()), l && this._convertTicksToLabels(this.ticks), this.beforeFit(), this.fit(), this.afterFit(), this.afterUpdate()
         }
         configure() {
             let e = this.options.reverse,
                 n, i;
             this.isHorizontal() ? (n = this.left, i = this.right) : (n = this.top, i = this.bottom, e = !e), this._startPixel = n, this._endPixel = i, this._reversePixels = e, this._length = i - n, this._alignToPixels = this.options.alignToPixels
@@ -13332,16 +13332,16 @@
             if (!this._isVisible() || !n.display || r >= o || i <= 1 || !this.isHorizontal()) {
                 this.labelRotation = r;
                 return
             }
             let d = this._getLabelSizes(),
                 g = d.widest.width,
                 y = d.highest.height,
-                x = St(this.chart.width - g, 0, this.maxWidth);
-            a = e.offset ? this.maxWidth / i : x / (i - 1), g + 6 > a && (a = x / (i - (e.offset ? .5 : 1)), l = this.maxHeight - Sl(e.grid) - n.padding - ib(e.title, this.chart.options.font), c = Math.sqrt(g * g + y * y), s = Ao(Math.min(Math.asin(St((d.highest.height + 6) / a, -1, 1)), Math.asin(St(l / c, -1, 1)) - Math.asin(St(y / c, -1, 1)))), s = Math.max(r, Math.min(o, s))), this.labelRotation = s
+                x = kt(this.chart.width - g, 0, this.maxWidth);
+            a = e.offset ? this.maxWidth / i : x / (i - 1), g + 6 > a && (a = x / (i - (e.offset ? .5 : 1)), l = this.maxHeight - Cl(e.grid) - n.padding - ib(e.title, this.chart.options.font), c = Math.sqrt(g * g + y * y), s = Ao(Math.min(Math.asin(kt((d.highest.height + 6) / a, -1, 1)), Math.asin(kt(l / c, -1, 1)) - Math.asin(kt(y / c, -1, 1)))), s = Math.max(r, Math.min(o, s))), this.labelRotation = s
         }
         afterCalculateLabelRotation() {
             ve(this.options.afterCalculateLabelRotation, [this])
         }
         afterAutoSkip() {}
         beforeFit() {
             ve(this.options.beforeFit, [this])
@@ -13359,29 +13359,29 @@
                         grid: o
                     }
                 } = this,
                 s = this._isVisible(),
                 a = this.isHorizontal();
             if (s) {
                 let l = ib(r, n.options.font);
-                if (a ? (e.width = this.maxWidth, e.height = Sl(o) + l) : (e.height = this.maxHeight, e.width = Sl(o) + l), i.display && this.ticks.length) {
+                if (a ? (e.width = this.maxWidth, e.height = Cl(o) + l) : (e.height = this.maxHeight, e.width = Cl(o) + l), i.display && this.ticks.length) {
                     let {
                         first: c,
                         last: d,
                         widest: g,
                         highest: y
-                    } = this._getLabelSizes(), x = i.padding * 2, w = pt(this.labelRotation), S = Math.cos(w), A = Math.sin(w);
+                    } = this._getLabelSizes(), x = i.padding * 2, _ = pt(this.labelRotation), C = Math.cos(_), A = Math.sin(_);
                     if (a) {
-                        let _ = i.mirror ? 0 : A * g.width + S * y.height;
-                        e.height = Math.min(this.maxHeight, e.height + _ + x)
+                        let w = i.mirror ? 0 : A * g.width + C * y.height;
+                        e.height = Math.min(this.maxHeight, e.height + w + x)
                     } else {
-                        let _ = i.mirror ? 0 : S * g.width + A * y.height;
-                        e.width = Math.min(this.maxWidth, e.width + _ + x)
+                        let w = i.mirror ? 0 : C * g.width + A * y.height;
+                        e.width = Math.min(this.maxWidth, e.width + w + x)
                     }
-                    this._calculatePadding(c, d, A, S)
+                    this._calculatePadding(c, d, A, C)
                 }
             }
             this._handleMargins(), a ? (this.width = this._length = n.width - this._margins.left - this._margins.right, this.height = e.height) : (this.width = e.width, this.height = this._length = n.height - this._margins.top - this._margins.bottom)
         }
         _calculatePadding(e, n, i, r) {
             let {
                 ticks: {
@@ -13433,36 +13433,36 @@
             }
             return e
         }
         _computeLabelSizes(e, n, i) {
             let {
                 ctx: r,
                 _longestTextCache: o
-            } = this, s = [], a = [], l = Math.floor(n / tb(n, i)), c = 0, d = 0, g, y, x, w, S, A, _, C, M, z, F;
+            } = this, s = [], a = [], l = Math.floor(n / tb(n, i)), c = 0, d = 0, g, y, x, _, C, A, w, k, P, z, F;
             for (g = 0; g < n; g += l) {
-                if (w = e[g].label, S = this._resolveTickFontOptions(g), r.font = A = S.string, _ = o[A] = o[A] || {
+                if (_ = e[g].label, C = this._resolveTickFontOptions(g), r.font = A = C.string, w = o[A] = o[A] || {
                         data: {},
                         gc: []
-                    }, C = S.lineHeight, M = z = 0, !Ie(w) && !Re(w)) M = As(r, _.data, _.gc, M, w), z = C;
-                else if (Re(w))
-                    for (y = 0, x = w.length; y < x; ++y) F = w[y], !Ie(F) && !Re(F) && (M = As(r, _.data, _.gc, M, F), z += C);
-                s.push(M), a.push(z), c = Math.max(M, c), d = Math.max(z, d)
+                    }, k = C.lineHeight, P = z = 0, !Ie(_) && !Re(_)) P = As(r, w.data, w.gc, P, _), z = k;
+                else if (Re(_))
+                    for (y = 0, x = _.length; y < x; ++y) F = _[y], !Ie(F) && !Re(F) && (P = As(r, w.data, w.gc, P, F), z += k);
+                s.push(P), a.push(z), c = Math.max(P, c), d = Math.max(z, d)
             }
             CE(o, n);
             let h = s.indexOf(c),
-                Y = a.indexOf(d),
-                V = te => ({
-                    width: s[te] || 0,
-                    height: a[te] || 0
+                $ = a.indexOf(d),
+                Y = ne => ({
+                    width: s[ne] || 0,
+                    height: a[ne] || 0
                 });
             return {
-                first: V(0),
-                last: V(n - 1),
-                widest: V(h),
-                highest: V(Y),
+                first: Y(0),
+                last: Y(n - 1),
+                widest: Y(h),
+                highest: Y($),
                 widths: s,
                 heights: a
             }
         }
         getLabelForValue(e) {
             return e
         }
@@ -13473,15 +13473,15 @@
         getPixelForTick(e) {
             let n = this.ticks;
             return e < 0 || e > n.length - 1 ? null : this.getPixelForValue(n[e].value)
         }
         getPixelForDecimal(e) {
             this._reversePixels && (e = 1 - e);
             let n = this._startPixel + e * this._length;
-            return Mp(this._alignToPixels ? nr(this.chart, n, 0) : n)
+            return Dp(this._alignToPixels ? nr(this.chart, n, 0) : n)
         }
         getDecimalForPixel(e) {
             let n = (e - this._startPixel) / this._length;
             return this._reversePixels ? 1 - n : n
         }
         getBasePixel() {
             return this.getPixelForValue(this.getBaseValue())
@@ -13524,78 +13524,78 @@
                     grid: o,
                     position: s,
                     border: a
                 } = r,
                 l = o.offset,
                 c = this.isHorizontal(),
                 g = this.ticks.length + (l ? 1 : 0),
-                y = Sl(o),
+                y = Cl(o),
                 x = [],
-                w = a.setContext(this.getContext()),
-                S = w.display ? w.width : 0,
-                A = S / 2,
-                _ = function(Te) {
-                    return nr(i, Te, S)
+                _ = a.setContext(this.getContext()),
+                C = _.display ? _.width : 0,
+                A = C / 2,
+                w = function(Te) {
+                    return nr(i, Te, C)
                 },
-                C, M, z, F, h, Y, V, te, ie, ce, he, Fe;
-            if (s === "top") C = _(this.bottom), Y = this.bottom - y, te = C - A, ce = _(e.top) + A, Fe = e.bottom;
-            else if (s === "bottom") C = _(this.top), ce = e.top, Fe = _(e.bottom) - A, Y = C + A, te = this.top + y;
-            else if (s === "left") C = _(this.right), h = this.right - y, V = C - A, ie = _(e.left) + A, he = e.right;
-            else if (s === "right") C = _(this.left), ie = e.left, he = _(e.right) - A, h = C + A, V = this.left + y;
+                k, P, z, F, h, $, Y, ne, ie, ce, he, Fe;
+            if (s === "top") k = w(this.bottom), $ = this.bottom - y, ne = k - A, ce = w(e.top) + A, Fe = e.bottom;
+            else if (s === "bottom") k = w(this.top), ce = e.top, Fe = w(e.bottom) - A, $ = k + A, ne = this.top + y;
+            else if (s === "left") k = w(this.right), h = this.right - y, Y = k - A, ie = w(e.left) + A, he = e.right;
+            else if (s === "right") k = w(this.left), ie = e.left, he = w(e.right) - A, h = k + A, Y = this.left + y;
             else if (n === "x") {
-                if (s === "center") C = _((e.top + e.bottom) / 2 + .5);
+                if (s === "center") k = w((e.top + e.bottom) / 2 + .5);
                 else if (we(s)) {
                     let Te = Object.keys(s)[0],
                         Ye = s[Te];
-                    C = _(this.chart.scales[Te].getPixelForValue(Ye))
+                    k = w(this.chart.scales[Te].getPixelForValue(Ye))
                 }
-                ce = e.top, Fe = e.bottom, Y = C + A, te = Y + y
+                ce = e.top, Fe = e.bottom, $ = k + A, ne = $ + y
             } else if (n === "y") {
-                if (s === "center") C = _((e.left + e.right) / 2);
+                if (s === "center") k = w((e.left + e.right) / 2);
                 else if (we(s)) {
                     let Te = Object.keys(s)[0],
                         Ye = s[Te];
-                    C = _(this.chart.scales[Te].getPixelForValue(Ye))
+                    k = w(this.chart.scales[Te].getPixelForValue(Ye))
                 }
-                h = C - A, V = h - y, ie = e.left, he = e.right
+                h = k - A, Y = h - y, ie = e.left, he = e.right
             }
             let Ze = pe(r.ticks.maxTicksLimit, g),
                 Ee = Math.max(1, Math.ceil(g / Ze));
-            for (M = 0; M < g; M += Ee) {
-                let Te = this.getContext(M),
+            for (P = 0; P < g; P += Ee) {
+                let Te = this.getContext(P),
                     Ye = o.setContext(Te),
                     Ot = a.setContext(Te),
                     lt = Ye.lineWidth,
                     Oe = Ye.color,
-                    Ge = Ot.dash || [],
+                    Ke = Ot.dash || [],
                     ot = Ot.dashOffset,
                     At = Ye.tickWidth,
                     $t = Ye.tickColor,
                     mt = Ye.tickBorderDash || [],
                     je = Ye.tickBorderDashOffset;
-                z = SE(this, M, l), z !== void 0 && (F = nr(i, z, lt), c ? h = V = ie = he = F : Y = te = ce = Fe = F, x.push({
+                z = kE(this, P, l), z !== void 0 && (F = nr(i, z, lt), c ? h = Y = ie = he = F : $ = ne = ce = Fe = F, x.push({
                     tx1: h,
-                    ty1: Y,
-                    tx2: V,
-                    ty2: te,
+                    ty1: $,
+                    tx2: Y,
+                    ty2: ne,
                     x1: ie,
                     y1: ce,
                     x2: he,
                     y2: Fe,
                     width: lt,
                     color: Oe,
-                    borderDash: Ge,
+                    borderDash: Ke,
                     borderDashOffset: ot,
                     tickWidth: At,
                     tickColor: $t,
                     tickBorderDash: mt,
                     tickBorderDashOffset: je
                 }))
             }
-            return this._ticksLength = g, this._borderValue = C, x
+            return this._ticksLength = g, this._borderValue = k, x
         }
         _computeLabelItems(e) {
             let n = this.axis,
                 i = this.options,
                 {
                     position: r,
                     ticks: o
@@ -13604,104 +13604,104 @@
                 a = this.ticks,
                 {
                     align: l,
                     crossAlign: c,
                     padding: d,
                     mirror: g
                 } = o,
-                y = Sl(i.grid),
+                y = Cl(i.grid),
                 x = y + d,
-                w = g ? -d : x,
-                S = -pt(this.labelRotation),
+                _ = g ? -d : x,
+                C = -pt(this.labelRotation),
                 A = [],
-                _, C, M, z, F, h, Y, V, te, ie, ce, he, Fe = "middle";
-            if (r === "top") h = this.bottom - w, Y = this._getXAxisLabelAlignment();
-            else if (r === "bottom") h = this.top + w, Y = this._getXAxisLabelAlignment();
+                w, k, P, z, F, h, $, Y, ne, ie, ce, he, Fe = "middle";
+            if (r === "top") h = this.bottom - _, $ = this._getXAxisLabelAlignment();
+            else if (r === "bottom") h = this.top + _, $ = this._getXAxisLabelAlignment();
             else if (r === "left") {
                 let Ee = this._getYAxisLabelAlignment(y);
-                Y = Ee.textAlign, F = Ee.x
+                $ = Ee.textAlign, F = Ee.x
             } else if (r === "right") {
                 let Ee = this._getYAxisLabelAlignment(y);
-                Y = Ee.textAlign, F = Ee.x
+                $ = Ee.textAlign, F = Ee.x
             } else if (n === "x") {
                 if (r === "center") h = (e.top + e.bottom) / 2 + x;
                 else if (we(r)) {
                     let Ee = Object.keys(r)[0],
                         Te = r[Ee];
                     h = this.chart.scales[Ee].getPixelForValue(Te) + x
                 }
-                Y = this._getXAxisLabelAlignment()
+                $ = this._getXAxisLabelAlignment()
             } else if (n === "y") {
                 if (r === "center") F = (e.left + e.right) / 2 - x;
                 else if (we(r)) {
                     let Ee = Object.keys(r)[0],
                         Te = r[Ee];
                     F = this.chart.scales[Ee].getPixelForValue(Te)
                 }
-                Y = this._getYAxisLabelAlignment(y).textAlign
+                $ = this._getYAxisLabelAlignment(y).textAlign
             }
             n === "y" && (l === "start" ? Fe = "top" : l === "end" && (Fe = "bottom"));
             let Ze = this._getLabelSizes();
-            for (_ = 0, C = a.length; _ < C; ++_) {
-                M = a[_], z = M.label;
-                let Ee = o.setContext(this.getContext(_));
-                V = this.getPixelForTick(_) + o.labelOffset, te = this._resolveTickFontOptions(_), ie = te.lineHeight, ce = Re(z) ? z.length : 1;
+            for (w = 0, k = a.length; w < k; ++w) {
+                P = a[w], z = P.label;
+                let Ee = o.setContext(this.getContext(w));
+                Y = this.getPixelForTick(w) + o.labelOffset, ne = this._resolveTickFontOptions(w), ie = ne.lineHeight, ce = Re(z) ? z.length : 1;
                 let Te = ce / 2,
                     Ye = Ee.color,
                     Ot = Ee.textStrokeColor,
                     lt = Ee.textStrokeWidth,
-                    Oe = Y;
-                s ? (F = V, Y === "inner" && (_ === C - 1 ? Oe = this.options.reverse ? "left" : "right" : _ === 0 ? Oe = this.options.reverse ? "right" : "left" : Oe = "center"), r === "top" ? c === "near" || S !== 0 ? he = -ce * ie + ie / 2 : c === "center" ? he = -Ze.highest.height / 2 - Te * ie + ie : he = -Ze.highest.height + ie / 2 : c === "near" || S !== 0 ? he = ie / 2 : c === "center" ? he = Ze.highest.height / 2 - Te * ie : he = Ze.highest.height - ce * ie, g && (he *= -1), S !== 0 && !Ee.showLabelBackdrop && (F += ie / 2 * Math.sin(S))) : (h = V, he = (1 - ce) * ie / 2);
-                let Ge;
+                    Oe = $;
+                s ? (F = Y, $ === "inner" && (w === k - 1 ? Oe = this.options.reverse ? "left" : "right" : w === 0 ? Oe = this.options.reverse ? "right" : "left" : Oe = "center"), r === "top" ? c === "near" || C !== 0 ? he = -ce * ie + ie / 2 : c === "center" ? he = -Ze.highest.height / 2 - Te * ie + ie : he = -Ze.highest.height + ie / 2 : c === "near" || C !== 0 ? he = ie / 2 : c === "center" ? he = Ze.highest.height / 2 - Te * ie : he = Ze.highest.height - ce * ie, g && (he *= -1), C !== 0 && !Ee.showLabelBackdrop && (F += ie / 2 * Math.sin(C))) : (h = Y, he = (1 - ce) * ie / 2);
+                let Ke;
                 if (Ee.showLabelBackdrop) {
                     let ot = gt(Ee.backdropPadding),
-                        At = Ze.heights[_],
-                        $t = Ze.widths[_],
+                        At = Ze.heights[w],
+                        $t = Ze.widths[w],
                         mt = he - ot.top,
                         je = 0 - ot.left;
                     switch (Fe) {
                         case "middle":
                             mt -= At / 2;
                             break;
                         case "bottom":
                             mt -= At;
                             break
                     }
-                    switch (Y) {
+                    switch ($) {
                         case "center":
                             je -= $t / 2;
                             break;
                         case "right":
                             je -= $t;
                             break;
                         case "inner":
-                            _ === C - 1 ? je -= $t : _ > 0 && (je -= $t / 2);
+                            w === k - 1 ? je -= $t : w > 0 && (je -= $t / 2);
                             break
                     }
-                    Ge = {
+                    Ke = {
                         left: je,
                         top: mt,
                         width: $t + ot.width,
                         height: At + ot.height,
                         color: Ee.backdropColor
                     }
                 }
                 A.push({
                     label: z,
-                    font: te,
+                    font: ne,
                     textOffset: he,
                     options: {
-                        rotation: S,
+                        rotation: C,
                         color: Ye,
                         strokeColor: Ot,
                         strokeWidth: lt,
                         textAlign: Oe,
                         textBaseline: Fe,
                         translation: [F, h],
-                        backdrop: Ge
+                        backdrop: Ke
                     }
                 })
             }
             return A
         }
         _getXAxisLabelAlignment() {
             let {
@@ -13838,20 +13838,20 @@
                 l = o.lineHeight / 2;
             n === "bottom" || n === "center" || we(n) ? (l += s.bottom, Re(i.text) && (l += o.lineHeight * (i.text.length - 1))) : l += s.top;
             let {
                 titleX: c,
                 titleY: d,
                 maxWidth: g,
                 rotation: y
-            } = ME(this, l, n, a);
+            } = PE(this, l, n, a);
             ir(e, i.text, 0, 0, o, {
                 color: i.color,
                 maxWidth: g,
                 rotation: y,
-                textAlign: PE(a, n, r),
+                textAlign: DE(a, n, r),
                 textBaseline: "middle",
                 translation: [c, d]
             })
         }
         draw(e) {
             this._isVisible() && (this.drawBackground(), this.drawGrid(e), this.drawBorder(), this.drawTitle(), this.drawLabels(e))
         }
@@ -13913,29 +13913,29 @@
             let n = Object.getPrototypeOf(e),
                 i;
             AE(n) && (i = this.register(n));
             let r = this.items,
                 o = e.id,
                 s = this.scope + "." + o;
             if (!o) throw new Error("class does not have id: " + e);
-            return o in r || (r[o] = e, DE(e, s, i), this.override && rt.override(e.id, e.overrides)), s
+            return o in r || (r[o] = e, ME(e, s, i), this.override && rt.override(e.id, e.overrides)), s
         }
         get(e) {
             return this.items[e]
         }
         unregister(e) {
             let n = this.items,
                 i = e.id,
                 r = this.scope;
             i in n && delete n[i], r && i in rt[r] && (delete rt[r][i], this.override && delete Br[i])
         }
     };
 
-function DE(t, e, n) {
-    let i = Mo(Object.create(null), [n ? rt.get(n) : {}, rt.get(e), t.defaults]);
+function ME(t, e, n) {
+    let i = Po(Object.create(null), [n ? rt.get(n) : {}, rt.get(e), t.defaults]);
     rt.set(e, i), t.defaultRoutes && OE(e, t.defaultRoutes), t.descriptors && rt.describe(e, t.descriptors)
 }
 
 function OE(t, e) {
     Object.keys(e).forEach(n => {
         let i = n.split("."),
             r = i.pop(),
@@ -13946,17 +13946,17 @@
         rt.route(o, r, l, a)
     })
 }
 
 function AE(t) {
     return "id" in t && "defaults" in t
 }
-var hg = class {
+var dg = class {
         constructor() {
-            this.controllers = new Ns(Mi, "datasets", !0), this.elements = new Ns(zt, "elements"), this.plugins = new Ns(Object, "plugins"), this.scales = new Ns(Fo, "scales"), this._typedRegistries = [this.controllers, this.scales, this.elements]
+            this.controllers = new Ns(Pi, "datasets", !0), this.elements = new Ns(zt, "elements"), this.plugins = new Ns(Object, "plugins"), this.scales = new Ns(Fo, "scales"), this._typedRegistries = [this.controllers, this.scales, this.elements]
         }
         add(...e) {
             this._each("register", e)
         }
         remove(...e) {
             this._each("unregister", e)
         }
@@ -13995,22 +13995,22 @@
         }
         removeScales(...e) {
             this._each("unregister", e, this.scales)
         }
         _each(e, n, i) {
             [...n].forEach(r => {
                 let o = i || this._getRegistryForType(r);
-                i || o.isForType(r) || o === this.plugins && r.id ? this._exec(e, o, r) : Se(r, s => {
+                i || o.isForType(r) || o === this.plugins && r.id ? this._exec(e, o, r) : ke(r, s => {
                     let a = i || this._getRegistryForType(s);
                     this._exec(e, a, s)
                 })
             })
         }
         _exec(e, n, i) {
-            let r = fl(e);
+            let r = dl(e);
             ve(i["before" + r], [], i), n[e](i), ve(i["after" + r], [], i)
         }
         _getRegistryForType(e) {
             for (let n = 0; n < this._typedRegistries.length; n++) {
                 let i = this._typedRegistries[n];
                 if (i.isForType(e)) return i
             }
@@ -14018,16 +14018,16 @@
         }
         _get(e, n, i) {
             let r = n.get(e);
             if (r === void 0) throw new Error('"' + e + '" is not a registered ' + i + ".");
             return r
         }
     },
-    Pi = new hg,
-    pg = class {
+    Di = new dg,
+    hg = class {
         constructor() {
             this._init = []
         }
         notify(e, n, i, r) {
             n === "beforeInit" && (this._init = this._createDescriptors(e, !0), this._notify(this._init, e, "install"));
             let o = r ? this._descriptors(e).filter(r) : this._descriptors(e),
                 s = this._notify(o, e, n, i);
@@ -14064,16 +14064,16 @@
             this._notify(r(n, i), e, "stop"), this._notify(r(i, n), e, "start")
         }
     };
 
 function LE(t) {
     let e = {},
         n = [],
-        i = Object.keys(Pi.plugins.items);
-    for (let o = 0; o < i.length; o++) n.push(Pi.getPlugin(i[o]));
+        i = Object.keys(Di.plugins.items);
+    for (let o = 0; o < i.length; o++) n.push(Di.getPlugin(i[o]));
     let r = t.plugins || [];
     for (let o = 0; o < r.length; o++) {
         let s = r[o];
         n.indexOf(s) === -1 && (n.push(s), e[s.id] = !0)
     }
     return {
         plugins: n,
@@ -14114,15 +14114,15 @@
     return n && e.defaults && s.push(e.defaults), t.createResolver(s, r, [""], {
         scriptable: !1,
         indexable: !1,
         allKeys: !0
     })
 }
 
-function gg(t, e) {
+function pg(t, e) {
     let n = rt.datasets[t] || {};
     return ((e.datasets || {})[t] || {}).indexAxis || e.indexAxis || n.indexAxis || "x"
 }
 
 function zE(t, e) {
     let n = t;
     return t === "_index_" ? n = e : t === "_value_" && (n = e === "x" ? "y" : "x"), n
@@ -14137,15 +14137,15 @@
 }
 
 function jE(t) {
     if (t === "top" || t === "bottom") return "x";
     if (t === "left" || t === "right") return "y"
 }
 
-function mg(t, ...e) {
+function gg(t, ...e) {
     if (rb(t)) return t;
     for (let n of e) {
         let i = n.axis || jE(n.position) || t.length > 1 && rb(t[0].toLowerCase());
         if (i) return i
     }
     throw new Error(`Cannot determine type of '${t}' axis. Please provide 'axis' or 'position' option.`)
 }
@@ -14165,40 +14165,40 @@
 }
 
 function BE(t, e) {
     let n = Br[t.type] || {
             scales: {}
         },
         i = e.scales || {},
-        r = gg(t.type, e),
+        r = pg(t.type, e),
         o = Object.create(null);
     return Object.keys(i).forEach(s => {
         let a = i[s];
         if (!we(a)) return console.error(`Invalid scale configuration for scale: ${s}`);
         if (a._proxy) return console.warn(`Ignoring resolver passed as options for scale: ${s}`);
-        let l = mg(s, a, HE(s, t), rt.scales[a.type]),
+        let l = gg(s, a, HE(s, t), rt.scales[a.type]),
             c = FE(l, r),
             d = n.scales || {};
-        o[s] = Do(Object.create(null), [{
+        o[s] = Mo(Object.create(null), [{
             axis: l
         }, a, d[l], d[c]])
     }), t.data.datasets.forEach(s => {
         let a = s.type || t.type,
-            l = s.indexAxis || gg(a, e),
+            l = s.indexAxis || pg(a, e),
             d = (Br[a] || {}).scales || {};
         Object.keys(d).forEach(g => {
             let y = zE(g, l),
                 x = s[y + "AxisID"] || y;
-            o[x] = o[x] || Object.create(null), Do(o[x], [{
+            o[x] = o[x] || Object.create(null), Mo(o[x], [{
                 axis: y
             }, i[x], d[g]])
         })
     }), Object.keys(o).forEach(s => {
         let a = o[s];
-        Do(a, [rt.scales[a.type], rt.scale])
+        Mo(a, [rt.scales[a.type], rt.scale])
     }), o
 }
 
 function Ub(t) {
     let e = t.options || (t.options = {});
     e.plugins = pe(e.plugins, {}), e.scales = BE(t, e)
 }
@@ -14209,23 +14209,23 @@
 
 function WE(t) {
     return t = t || {}, t.data = $b(t.data), Ub(t), t
 }
 var sb = new Map,
     Yb = new Set;
 
-function sf(t, e) {
+function af(t, e) {
     let n = sb.get(t);
     return n || (n = e(), sb.set(t, n), Yb.add(n)), n
 }
-var Cl = (t, e, n) => {
+var El = (t, e, n) => {
         let i = Ci(e, n);
         i !== void 0 && t.add(i)
     },
-    yg = class {
+    mg = class {
         constructor(e) {
             this._config = WE(e), this._scopeCache = new Map, this._resolverCache = new Map
         }
         get platform() {
             return this._config.platform
         }
         get type() {
@@ -14253,33 +14253,33 @@
             let e = this._config;
             this.clearCache(), Ub(e)
         }
         clearCache() {
             this._scopeCache.clear(), this._resolverCache.clear()
         }
         datasetScopeKeys(e) {
-            return sf(e, () => [
+            return af(e, () => [
                 [`datasets.${e}`, ""]
             ])
         }
         datasetAnimationScopeKeys(e, n) {
-            return sf(`${e}.transition.${n}`, () => [
+            return af(`${e}.transition.${n}`, () => [
                 [`datasets.${e}.transitions.${n}`, `transitions.${n}`],
                 [`datasets.${e}`, ""]
             ])
         }
         datasetElementScopeKeys(e, n) {
-            return sf(`${e}-${n}`, () => [
+            return af(`${e}-${n}`, () => [
                 [`datasets.${e}.elements.${n}`, `datasets.${e}`, `elements.${n}`, ""]
             ])
         }
         pluginScopeKeys(e) {
             let n = e.id,
                 i = this.type;
-            return sf(`${i}-plugin-${n}`, () => [
+            return af(`${i}-plugin-${n}`, () => [
                 [`plugins.${n}`, ...e.additionalOptionScopes || []]
             ])
         }
         _cachedScopes(e, n) {
             let i = this._scopeCache,
                 r = i.get(e);
             return (!r || n) && (r = new Map, i.set(e, r)), r
@@ -14288,27 +14288,27 @@
             let {
                 options: r,
                 type: o
             } = this, s = this._cachedScopes(e, i), a = s.get(n);
             if (a) return a;
             let l = new Set;
             n.forEach(d => {
-                e && (l.add(e), d.forEach(g => Cl(l, e, g))), d.forEach(g => Cl(l, r, g)), d.forEach(g => Cl(l, Br[o] || {}, g)), d.forEach(g => Cl(l, rt, g)), d.forEach(g => Cl(l, Uc, g))
+                e && (l.add(e), d.forEach(g => El(l, e, g))), d.forEach(g => El(l, r, g)), d.forEach(g => El(l, Br[o] || {}, g)), d.forEach(g => El(l, rt, g)), d.forEach(g => El(l, $c, g))
             });
             let c = Array.from(l);
             return c.length === 0 && c.push(Object.create(null)), Yb.has(n) && s.set(n, c), c
         }
         chartOptionScopes() {
             let {
                 options: e,
                 type: n
             } = this;
             return [e, Br[n] || {}, rt.datasets[n] || {}, {
                 type: n
-            }, rt, Uc]
+            }, rt, $c]
         }
         resolveNamedOptions(e, n, i, r = [""]) {
             let o = {
                     $shared: !0
                 },
                 {
                     resolver: s,
@@ -14333,25 +14333,25 @@
 
 function ab(t, e, n) {
     let i = t.get(e);
     i || (i = new Map, t.set(e, i));
     let r = n.join(),
         o = i.get(r);
     return o || (o = {
-        resolver: vl(e, n),
+        resolver: xl(e, n),
         subPrefixes: n.filter(a => !a.toLowerCase().includes("hover"))
     }, i.set(r, o)), o
 }
 var VE = t => we(t) && Object.getOwnPropertyNames(t).some(e => Vt(t[e]));
 
 function UE(t, e) {
     let {
         isScriptable: n,
         isIndexable: i
-    } = qc(t);
+    } = Zc(t);
     for (let r of e) {
         let o = n(r),
             s = i(r),
             a = (s || o) && t[r];
         if (o && (Vt(a) || VE(a)) || s && Re(a)) return !0
     }
     return !1
@@ -14378,20 +14378,20 @@
 function XE(t) {
     let e = t.chart,
         n = e.options.animation;
     ve(n && n.onProgress, [t], e)
 }
 
 function Xb(t) {
-    return xl() && typeof t == "string" ? t = document.getElementById(t) : t && t.length && (t = t[0]), t && t.canvas && (t = t.canvas), t
+    return bl() && typeof t == "string" ? t = document.getElementById(t) : t && t.length && (t = t[0]), t && t.canvas && (t = t.canvas), t
 }
-var df = {},
+var hf = {},
     fb = t => {
         let e = Xb(t);
-        return Object.values(df).filter(n => n.canvas === e).pop()
+        return Object.values(hf).filter(n => n.canvas === e).pop()
     };
 
 function qE(t, e, n) {
     let i = Object.keys(t);
     for (let r of i) {
         let o = +r;
         if (o >= e) {
@@ -14401,55 +14401,55 @@
     }
 }
 
 function ZE(t, e, n, i) {
     return !n || t.type === "mouseout" ? null : i ? e : t
 }
 
-function af(t, e, n) {
+function lf(t, e, n) {
     return t.options.clip ? t[n] : e[n]
 }
 
-function GE(t, e) {
+function KE(t, e) {
     let {
         xScale: n,
         yScale: i
     } = t;
     return n && i ? {
-        left: af(n, e, "left"),
-        right: af(n, e, "right"),
-        top: af(i, e, "top"),
-        bottom: af(i, e, "bottom")
+        left: lf(n, e, "left"),
+        right: lf(n, e, "right"),
+        top: lf(i, e, "top"),
+        bottom: lf(i, e, "bottom")
     } : e
 }
 var Fn = class {
     static defaults = rt;
-    static instances = df;
+    static instances = hf;
     static overrides = Br;
-    static registry = Pi;
+    static registry = Di;
     static version = $E;
     static getChart = fb;
     static register(...e) {
-        Pi.add(...e), db()
+        Di.add(...e), db()
     }
     static unregister(...e) {
-        Pi.remove(...e), db()
+        Di.remove(...e), db()
     }
     constructor(e, n) {
-        let i = this.config = new yg(n),
+        let i = this.config = new mg(n),
             r = Xb(e),
             o = fb(r);
         if (o) throw new Error("Canvas is already in use. Chart with ID '" + o.id + "' must be destroyed before the canvas with ID '" + o.canvas.id + "' can be reused.");
         let s = i.createResolver(i.chartOptionScopes(), this.getContext());
         this.platform = new(i.platform || mE(r)), this.platform.updateConfig(i);
         let a = this.platform.acquireContext(r, s.aspectRatio),
             l = a && a.canvas,
             c = l && l.height,
             d = l && l.width;
-        if (this.id = Sp(), this.ctx = a, this.canvas = l, this.width = d, this.height = c, this._options = s, this._aspectRatio = this.aspectRatio, this._layers = [], this._metasets = [], this._stacks = void 0, this.boxes = [], this.currentDevicePixelRatio = void 0, this.chartArea = void 0, this._active = [], this._lastEvent = void 0, this._listeners = {}, this._responsiveListeners = void 0, this._sortedMetasets = [], this.scales = {}, this._plugins = new pg, this.$proxies = {}, this._hiddenIndices = {}, this.attached = !1, this._animationsDisabled = void 0, this.$context = void 0, this._doResize = Lp(g => this.update(g), s.resizeDelay || 0), this._dataChanges = [], df[this.id] = this, !a || !l) {
+        if (this.id = Sp(), this.ctx = a, this.canvas = l, this.width = d, this.height = c, this._options = s, this._aspectRatio = this.aspectRatio, this._layers = [], this._metasets = [], this._stacks = void 0, this.boxes = [], this.currentDevicePixelRatio = void 0, this.chartArea = void 0, this._active = [], this._lastEvent = void 0, this._listeners = {}, this._responsiveListeners = void 0, this._sortedMetasets = [], this.scales = {}, this._plugins = new hg, this.$proxies = {}, this._hiddenIndices = {}, this.attached = !1, this._animationsDisabled = void 0, this.$context = void 0, this._doResize = Ap(g => this.update(g), s.resizeDelay || 0), this._dataChanges = [], hf[this.id] = this, !a || !l) {
             console.error("Failed to create chart: can't acquire context from the given item");
             return
         }
         or.listen(this, "complete", cb), or.listen(this, "progress", XE), this._initialize(), this.attached && this.update()
     }
     get aspectRatio() {
         let {
@@ -14472,21 +14472,21 @@
     get options() {
         return this._options
     }
     set options(e) {
         this.config.options = e
     }
     get registry() {
-        return Pi
+        return Di
     }
     _initialize() {
         return this.notifyPlugins("beforeInit"), this.options.responsive ? this.resize() : Qc(this, this.options.devicePixelRatio), this.bindEvents(), this.notifyPlugins("afterInit"), this
     }
     clear() {
-        return $c(this.canvas, this.ctx), this
+        return Yc(this.canvas, this.ctx), this
     }
     stop() {
         return or.stop(this), this
     }
     resize(e, n) {
         or.running(this) ? this._resizeBeforeDraw = {
             width: e,
@@ -14502,55 +14502,55 @@
             l = this.width ? "resize" : "attach";
         this.width = s.width, this.height = s.height, this._aspectRatio = this.aspectRatio, Qc(this, a, !0) && (this.notifyPlugins("resize", {
             size: s
         }), ve(i.onResize, [this, s], this), this.attached && this._doResize(l) && this.render())
     }
     ensureScalesHaveIDs() {
         let n = this.options.scales || {};
-        Se(n, (i, r) => {
+        ke(n, (i, r) => {
             i.id = r
         })
     }
     buildOrUpdateScales() {
         let e = this.options,
             n = e.scales,
             i = this.scales,
             r = Object.keys(i).reduce((s, a) => (s[a] = !1, s), {}),
             o = [];
         n && (o = o.concat(Object.keys(n).map(s => {
             let a = n[s],
-                l = mg(s, a),
+                l = gg(s, a),
                 c = l === "r",
                 d = l === "x";
             return {
                 options: a,
                 dposition: c ? "chartArea" : d ? "bottom" : "left",
                 dtype: c ? "radialLinear" : d ? "category" : "linear"
             }
-        }))), Se(o, s => {
+        }))), ke(o, s => {
             let a = s.options,
                 l = a.id,
-                c = mg(l, a),
+                c = gg(l, a),
                 d = pe(a.type, s.dtype);
             (a.position === void 0 || lb(a.position, c) !== lb(s.dposition)) && (a.position = s.dposition), r[l] = !0;
             let g = null;
             if (l in i && i[l].type === d) g = i[l];
             else {
-                let y = Pi.getScale(d);
+                let y = Di.getScale(d);
                 g = new y({
                     id: l,
                     type: d,
                     ctx: this.ctx,
                     chart: this
                 }), i[g.id] = g
             }
             g.init(a, e)
-        }), Se(r, (s, a) => {
+        }), ke(r, (s, a) => {
             s || delete i[a]
-        }), Se(i, s => {
+        }), ke(i, s => {
             Jt.configure(this, s, s.options), Jt.addBox(this, s)
         })
     }
     _updateMetasets() {
         let e = this._metasets,
             n = this.data.datasets.length,
             i = e.length;
@@ -14575,31 +14575,31 @@
         let e = [],
             n = this.data.datasets,
             i, r;
         for (this._removeUnreferencedMetasets(), i = 0, r = n.length; i < r; i++) {
             let o = n[i],
                 s = this.getDatasetMeta(i),
                 a = o.type || this.config.type;
-            if (s.type && s.type !== a && (this._destroyDatasetMeta(i), s = this.getDatasetMeta(i)), s.type = a, s.indexAxis = o.indexAxis || gg(a, this.options), s.order = o.order || 0, s.index = i, s.label = "" + o.label, s.visible = this.isDatasetVisible(i), s.controller) s.controller.updateIndex(i), s.controller.linkScales();
+            if (s.type && s.type !== a && (this._destroyDatasetMeta(i), s = this.getDatasetMeta(i)), s.type = a, s.indexAxis = o.indexAxis || pg(a, this.options), s.order = o.order || 0, s.index = i, s.label = "" + o.label, s.visible = this.isDatasetVisible(i), s.controller) s.controller.updateIndex(i), s.controller.linkScales();
             else {
-                let l = Pi.getController(a),
+                let l = Di.getController(a),
                     {
                         datasetElementType: c,
                         dataElementType: d
                     } = rt.datasets[a];
                 Object.assign(l, {
-                    dataElementType: Pi.getElement(d),
-                    datasetElementType: c && Pi.getElement(c)
+                    dataElementType: Di.getElement(d),
+                    datasetElementType: c && Di.getElement(c)
                 }), s.controller = new l(this, i), e.push(s.controller)
             }
         }
         return this._updateMetasets(), e
     }
     _resetElements() {
-        Se(this.data.datasets, (e, n) => {
+        ke(this.data.datasets, (e, n) => {
             this.getDatasetMeta(n).controller.reset()
         }, this)
     }
     reset() {
         this._resetElements(), this.notifyPlugins("reset")
     }
     update(e) {
@@ -14616,35 +14616,35 @@
         let s = 0;
         for (let c = 0, d = this.data.datasets.length; c < d; c++) {
             let {
                 controller: g
             } = this.getDatasetMeta(c), y = !r && o.indexOf(g) === -1;
             g.buildOrUpdateElements(y), s = Math.max(+g.getMaxOverflow(), s)
         }
-        s = this._minPadding = i.layout.autoPadding ? s : 0, this._updateLayout(s), r || Se(o, c => {
+        s = this._minPadding = i.layout.autoPadding ? s : 0, this._updateLayout(s), r || ke(o, c => {
             c.reset()
         }), this._updateDatasets(e), this.notifyPlugins("afterUpdate", {
             mode: e
         }), this._layers.sort(ub("z", "_idx"));
         let {
             _active: a,
             _lastEvent: l
         } = this;
         l ? this._eventHandler(l, !0) : a.length && this._updateHoverStyles(a, a, !0), this.render()
     }
     _updateScales() {
-        Se(this.scales, e => {
+        ke(this.scales, e => {
             Jt.removeBox(this, e)
         }), this.ensureScalesHaveIDs(), this.buildOrUpdateScales()
     }
     _checkEventBindings() {
         let e = this.options,
             n = new Set(Object.keys(this._listeners)),
             i = new Set(e.events);
-        (!Oc(n, i) || !!this._responsiveListeners !== e.responsive) && (this.unbindEvents(), this.bindEvents())
+        (!Ac(n, i) || !!this._responsiveListeners !== e.responsive) && (this.unbindEvents(), this.bindEvents())
     }
     _updateHiddenIndices() {
         let {
             _hiddenIndices: e
         } = this, n = this._getUniformDataChanges() || [];
         for (let {
                 method: i,
@@ -14660,29 +14660,29 @@
         let e = this._dataChanges;
         if (!e || !e.length) return;
         this._dataChanges = [];
         let n = this.data.datasets.length,
             i = o => new Set(e.filter(s => s[0] === o).map((s, a) => a + "," + s.splice(1).join(","))),
             r = i(0);
         for (let o = 1; o < n; o++)
-            if (!Oc(r, i(o))) return;
+            if (!Ac(r, i(o))) return;
         return Array.from(r).map(o => o.split(",")).map(o => ({
             method: o[1],
             start: +o[2],
             count: +o[3]
         }))
     }
     _updateLayout(e) {
         if (this.notifyPlugins("beforeLayout", {
                 cancelable: !0
             }) === !1) return;
         Jt.update(this, this.width, this.height, e);
         let n = this.chartArea,
             i = n.width <= 0 || n.height <= 0;
-        this._layers = [], Se(this.boxes, r => {
+        this._layers = [], ke(this.boxes, r => {
             i && r.position === "chartArea" || (r.configure && r.configure(), this._layers.push(...r._layers()))
         }, this), this._layers.forEach((r, o) => {
             r._idx = o
         }), this.notifyPlugins("afterLayout")
     }
     _updateDatasets(e) {
         if (this.notifyPlugins("beforeDatasetsUpdate", {
@@ -14753,15 +14753,15 @@
         for (let n = e.length - 1; n >= 0; --n) this._drawDataset(e[n]);
         this.notifyPlugins("afterDatasetsDraw")
     }
     _drawDataset(e) {
         let n = this.ctx,
             i = e._clip,
             r = !i.disabled,
-            o = GE(e, this.chartArea),
+            o = KE(e, this.chartArea),
             s = {
                 meta: e,
                 index: e.index,
                 cancelable: !0
             };
         this.notifyPlugins("beforeDatasetDraw", s) !== !1 && (r && Wr(n, {
             left: i.left === !1 ? 0 : o.left - i.left,
@@ -14770,15 +14770,15 @@
             bottom: i.bottom === !1 ? this.height : o.bottom + i.bottom
         }), e.controller.draw(), r && Vr(n), s.cancelable = !1, this.notifyPlugins("afterDatasetDraw", s))
     }
     isPointInArea(e) {
         return ci(e, this.chartArea, this._minPadding)
     }
     getElementsAtEventForMode(e, n, i, r) {
-        let o = QC.modes[n];
+        let o = GC.modes[n];
         return typeof o == "function" ? o(this, e, i, r) : []
     }
     getDatasetMeta(e) {
         let n = this.data.datasets[e],
             i = this._metasets,
             r = i.filter(o => o && o._dataset === n).pop();
         return r || (r = {
@@ -14845,15 +14845,15 @@
     }
     destroy() {
         this.notifyPlugins("beforeDestroy");
         let {
             canvas: e,
             ctx: n
         } = this;
-        this._stop(), this.config.clearCache(), e && (this.unbindEvents(), $c(e, n), this.platform.releaseContext(n), this.canvas = null, this.ctx = null), delete df[this.id], this.notifyPlugins("afterDestroy")
+        this._stop(), this.config.clearCache(), e && (this.unbindEvents(), Yc(e, n), this.platform.releaseContext(n), this.canvas = null, this.ctx = null), delete hf[this.id], this.notifyPlugins("afterDestroy")
     }
     toBase64Image(...e) {
         return this.canvas.toDataURL(...e)
     }
     bindEvents() {
         this.bindUserEvents(), this.options.responsive ? this.bindResponsiveEvents() : this.attached = !0
     }
@@ -14862,15 +14862,15 @@
             n = this.platform,
             i = (o, s) => {
                 n.addEventListener(this, o, s), e[o] = s
             },
             r = (o, s, a) => {
                 o.offsetX = s, o.offsetY = a, this._eventHandler(o)
             };
-        Se(this.options.events, o => i(o, r))
+        ke(this.options.events, o => i(o, r))
     }
     bindResponsiveEvents() {
         this._responsiveListeners || (this._responsiveListeners = {});
         let e = this._responsiveListeners,
             n = this.platform,
             i = (l, c) => {
                 n.addEventListener(this, l, c), e[l] = c
@@ -14885,17 +14885,17 @@
                 r("attach", a), this.attached = !0, this.resize(), i("resize", o), i("detach", s)
             };
         s = () => {
             this.attached = !1, r("resize", o), this._stop(), this._resize(0, 0), i("attach", a)
         }, n.isAttached(this.canvas) ? a() : s()
     }
     unbindEvents() {
-        Se(this._listeners, (e, n) => {
+        ke(this._listeners, (e, n) => {
             this.platform.removeEventListener(this, n, e)
-        }), this._listeners = {}, Se(this._responsiveListeners, (e, n) => {
+        }), this._listeners = {}, ke(this._responsiveListeners, (e, n) => {
             this.platform.removeEventListener(this, n, e)
         }), this._responsiveListeners = void 0
     }
     updateHoverStyle(e, n, i) {
         let r = i ? "set" : "remove",
             o, s, a, l;
         for (n === "dataset" && (o = this.getDatasetMeta(e[0].datasetIndex), o.controller["_" + r + "DatasetHoverStyle"]()), a = 0, l = e.length; a < l; ++a) {
@@ -14948,128 +14948,128 @@
         let o = this._handleEvent(e, n, i.inChartArea);
         return i.cancelable = !1, this.notifyPlugins("afterEvent", i, r), (o || i.changed) && this.render(), this
     }
     _handleEvent(e, n, i) {
         let {
             _active: r = [],
             options: o
-        } = this, s = n, a = this._getActiveElements(e, r, i, s), l = Ep(e), c = ZE(e, this._lastEvent, i, l);
+        } = this, s = n, a = this._getActiveElements(e, r, i, s), l = Cp(e), c = ZE(e, this._lastEvent, i, l);
         i && (this._lastEvent = null, ve(o.onHover, [e, a, this], this), l && ve(o.onClick, [e, a, this], this));
         let d = !Rs(a, r);
         return (d || n) && (this._active = a, this._updateHoverStyles(a, r, n)), this._lastEvent = c, d
     }
     _getActiveElements(e, n, i, r) {
         if (e.type === "mouseout") return [];
         if (!i) return n;
         let o = this.options.hover;
         return this.getElementsAtEventForMode(e, o.mode, o, r)
     }
 };
 
 function db() {
-    return Se(Fn.instances, t => t._plugins.invalidate())
+    return ke(Fn.instances, t => t._plugins.invalidate())
 }
 
-function QE(t, e, n) {
+function GE(t, e, n) {
     let {
         startAngle: i,
         pixelMargin: r,
         x: o,
         y: s,
         outerRadius: a,
         innerRadius: l
     } = e, c = r / a;
     t.beginPath(), t.arc(o, s, a, i - c, n + c), l > r ? (c = r / l, t.arc(o, s, l, n + c, i - c, !0)) : t.arc(o, s, r, n + $e, i - $e), t.closePath(), t.clip()
 }
 
-function KE(t) {
-    return yl(t, ["outerStart", "outerEnd", "innerStart", "innerEnd"])
+function QE(t) {
+    return vl(t, ["outerStart", "outerEnd", "innerStart", "innerEnd"])
 }
 
 function JE(t, e, n, i) {
-    let r = KE(t.options.borderRadius),
+    let r = QE(t.options.borderRadius),
         o = (n - e) / 2,
         s = Math.min(o, i * e / 2),
         a = l => {
             let c = (n - Math.min(o, l)) * i / 2;
-            return St(l, 0, Math.min(o, c))
+            return kt(l, 0, Math.min(o, c))
         };
     return {
         outerStart: a(r.outerStart),
         outerEnd: a(r.outerEnd),
-        innerStart: St(r.innerStart, 0, s),
-        innerEnd: St(r.innerEnd, 0, s)
+        innerStart: kt(r.innerStart, 0, s),
+        innerEnd: kt(r.innerEnd, 0, s)
     }
 }
 
 function Is(t, e, n, i) {
     return {
         x: n + t * Math.cos(e),
         y: i + t * Math.sin(e)
     }
 }
 
-function mf(t, e, n, i, r, o) {
+function yf(t, e, n, i, r, o) {
     let {
         x: s,
         y: a,
         startAngle: l,
         pixelMargin: c,
         innerRadius: d
-    } = e, g = Math.max(e.outerRadius + i + n - c, 0), y = d > 0 ? d + i + n + c : 0, x = 0, w = r - l;
+    } = e, g = Math.max(e.outerRadius + i + n - c, 0), y = d > 0 ? d + i + n + c : 0, x = 0, _ = r - l;
     if (i) {
         let Ee = d > 0 ? d - i : 0,
             Te = g > 0 ? g - i : 0,
             Ye = (Ee + Te) / 2,
-            Ot = Ye !== 0 ? w * Ye / (Ye + i) : w;
-        x = (w - Ot) / 2
+            Ot = Ye !== 0 ? _ * Ye / (Ye + i) : _;
+        x = (_ - Ot) / 2
     }
-    let S = Math.max(.001, w * g - n / Ce) / g,
-        A = (w - S) / 2,
-        _ = l + A + x,
-        C = r - A - x,
+    let C = Math.max(.001, _ * g - n / Ce) / g,
+        A = (_ - C) / 2,
+        w = l + A + x,
+        k = r - A - x,
         {
-            outerStart: M,
+            outerStart: P,
             outerEnd: z,
             innerStart: F,
             innerEnd: h
-        } = JE(e, y, g, C - _),
-        Y = g - M,
-        V = g - z,
-        te = _ + M / Y,
-        ie = C - z / V,
+        } = JE(e, y, g, k - w),
+        $ = g - P,
+        Y = g - z,
+        ne = w + P / $,
+        ie = k - z / Y,
         ce = y + F,
         he = y + h,
-        Fe = _ + F / ce,
-        Ze = C - h / he;
+        Fe = w + F / ce,
+        Ze = k - h / he;
     if (t.beginPath(), o) {
-        let Ee = (te + ie) / 2;
-        if (t.arc(s, a, g, te, Ee), t.arc(s, a, g, Ee, ie), z > 0) {
-            let lt = Is(V, ie, s, a);
-            t.arc(lt.x, lt.y, z, ie, C + $e)
+        let Ee = (ne + ie) / 2;
+        if (t.arc(s, a, g, ne, Ee), t.arc(s, a, g, Ee, ie), z > 0) {
+            let lt = Is(Y, ie, s, a);
+            t.arc(lt.x, lt.y, z, ie, k + $e)
         }
-        let Te = Is(he, C, s, a);
+        let Te = Is(he, k, s, a);
         if (t.lineTo(Te.x, Te.y), h > 0) {
             let lt = Is(he, Ze, s, a);
-            t.arc(lt.x, lt.y, h, C + $e, Ze + Math.PI)
+            t.arc(lt.x, lt.y, h, k + $e, Ze + Math.PI)
         }
-        let Ye = (C - h / y + (_ + F / y)) / 2;
-        if (t.arc(s, a, y, C - h / y, Ye, !0), t.arc(s, a, y, Ye, _ + F / y, !0), F > 0) {
+        let Ye = (k - h / y + (w + F / y)) / 2;
+        if (t.arc(s, a, y, k - h / y, Ye, !0), t.arc(s, a, y, Ye, w + F / y, !0), F > 0) {
             let lt = Is(ce, Fe, s, a);
-            t.arc(lt.x, lt.y, F, Fe + Math.PI, _ - $e)
+            t.arc(lt.x, lt.y, F, Fe + Math.PI, w - $e)
         }
-        let Ot = Is(Y, _, s, a);
-        if (t.lineTo(Ot.x, Ot.y), M > 0) {
-            let lt = Is(Y, te, s, a);
-            t.arc(lt.x, lt.y, M, _ - $e, te)
+        let Ot = Is($, w, s, a);
+        if (t.lineTo(Ot.x, Ot.y), P > 0) {
+            let lt = Is($, ne, s, a);
+            t.arc(lt.x, lt.y, P, w - $e, ne)
         }
     } else {
         t.moveTo(s, a);
-        let Ee = Math.cos(te) * g + s,
-            Te = Math.sin(te) * g + a;
+        let Ee = Math.cos(ne) * g + s,
+            Te = Math.sin(ne) * g + a;
         t.lineTo(Ee, Te);
         let Ye = Math.cos(ie) * g + s,
             Ot = Math.sin(ie) * g + a;
         t.lineTo(Ye, Ot)
     }
     t.closePath()
 }
@@ -15077,19 +15077,19 @@
 function eT(t, e, n, i, r) {
     let {
         fullCircles: o,
         startAngle: s,
         circumference: a
     } = e, l = e.endAngle;
     if (o) {
-        mf(t, e, n, i, l, r);
+        yf(t, e, n, i, l, r);
         for (let c = 0; c < o; ++c) t.fill();
         isNaN(a) || (l = s + (a % We || We))
     }
-    return mf(t, e, n, i, l, r), t.fill(), l
+    return yf(t, e, n, i, l, r), t.fill(), l
 }
 
 function tT(t, e, n, i, r) {
     let {
         fullCircles: o,
         startAngle: s,
         circumference: a,
@@ -15098,23 +15098,23 @@
         borderWidth: c,
         borderJoinStyle: d,
         borderDash: g,
         borderDashOffset: y
     } = l, x = l.borderAlign === "inner";
     if (!c) return;
     t.setLineDash(g || []), t.lineDashOffset = y, x ? (t.lineWidth = c * 2, t.lineJoin = d || "round") : (t.lineWidth = c, t.lineJoin = d || "bevel");
-    let w = e.endAngle;
+    let _ = e.endAngle;
     if (o) {
-        mf(t, e, n, i, w, r);
-        for (let S = 0; S < o; ++S) t.stroke();
-        isNaN(a) || (w = s + (a % We || We))
+        yf(t, e, n, i, _, r);
+        for (let C = 0; C < o; ++C) t.stroke();
+        isNaN(a) || (_ = s + (a % We || We))
     }
-    x && QE(t, e, w), o || (mf(t, e, n, i, w, r), t.stroke())
+    x && GE(t, e, _), o || (yf(t, e, n, i, _, r), t.stroke())
 }
-var vg = class extends zt {
+var yg = class extends zt {
     static id = "arc";
     static defaults = {
         borderAlign: "center",
         borderColor: "#fff",
         borderDash: [],
         borderDashOffset: 0,
         borderJoinStyle: void 0,
@@ -15143,29 +15143,29 @@
         super(), this.options = void 0, this.circumference = void 0, this.startAngle = void 0, this.endAngle = void 0, this.innerRadius = void 0, this.outerRadius = void 0, this.pixelMargin = 0, this.fullCircles = 0, e && Object.assign(this, e)
     }
     inRange(e, n, i) {
         let r = this.getProps(["x", "y"], i),
             {
                 angle: o,
                 distance: s
-            } = Ic(r, {
+            } = Nc(r, {
                 x: e,
                 y: n
             }),
             {
                 startAngle: a,
                 endAngle: l,
                 innerRadius: c,
                 outerRadius: d,
                 circumference: g
             } = this.getProps(["startAngle", "endAngle", "innerRadius", "outerRadius", "circumference"], i),
             y = (this.options.spacing + this.options.borderWidth) / 2,
-            w = pe(g, l - a) >= We || Lo(o, a, l),
-            S = hi(s, c + y, d + y);
-        return w && S
+            _ = pe(g, l - a) >= We || Lo(o, a, l),
+            C = hi(s, c + y, d + y);
+        return _ && C
     }
     getCenterPoint(e) {
         let {
             x: n,
             y: i,
             startAngle: r,
             endAngle: o,
@@ -15203,15 +15203,15 @@
 }
 
 function nT(t, e, n) {
     t.lineTo(n.x, n.y)
 }
 
 function iT(t) {
-    return t.stepped ? Np : t.tension || t.cubicInterpolationMode === "monotone" ? zp : nT
+    return t.stepped ? Ip : t.tension || t.cubicInterpolationMode === "monotone" ? Np : nT
 }
 
 function Zb(t, e, n = {}) {
     let i = t.length,
         {
             start: r = 0,
             end: o = i - 1
@@ -15239,17 +15239,17 @@
         count: s,
         start: a,
         loop: l,
         ilen: c
     } = Zb(r, n, i), d = iT(o), {
         move: g = !0,
         reverse: y
-    } = i || {}, x, w, S;
-    for (x = 0; x <= c; ++x) w = r[(a + (y ? c - x : x)) % s], !w.skip && (g ? (t.moveTo(w.x, w.y), g = !1) : d(t, S, w, y, o.stepped), S = w);
-    return l && (w = r[(a + (y ? c : 0)) % s], d(t, S, w, y, o.stepped)), !!l
+    } = i || {}, x, _, C;
+    for (x = 0; x <= c; ++x) _ = r[(a + (y ? c - x : x)) % s], !_.skip && (g ? (t.moveTo(_.x, _.y), g = !1) : d(t, C, _, y, o.stepped), C = _);
+    return l && (_ = r[(a + (y ? c : 0)) % s], d(t, C, _, y, o.stepped)), !!l
 }
 
 function oT(t, e, n, i) {
     let r = e.points,
         {
             count: o,
             start: s,
@@ -15257,48 +15257,48 @@
         } = Zb(r, n, i),
         {
             move: l = !0,
             reverse: c
         } = i || {},
         d = 0,
         g = 0,
-        y, x, w, S, A, _, C = z => (s + (c ? a - z : z)) % o,
-        M = () => {
-            S !== A && (t.lineTo(d, A), t.lineTo(d, S), t.lineTo(d, _))
+        y, x, _, C, A, w, k = z => (s + (c ? a - z : z)) % o,
+        P = () => {
+            C !== A && (t.lineTo(d, A), t.lineTo(d, C), t.lineTo(d, w))
         };
-    for (l && (x = r[C(0)], t.moveTo(x.x, x.y)), y = 0; y <= a; ++y) {
-        if (x = r[C(y)], x.skip) continue;
+    for (l && (x = r[k(0)], t.moveTo(x.x, x.y)), y = 0; y <= a; ++y) {
+        if (x = r[k(y)], x.skip) continue;
         let z = x.x,
             F = x.y,
             h = z | 0;
-        h === w ? (F < S ? S = F : F > A && (A = F), d = (g * d + z) / ++g) : (M(), t.lineTo(z, F), w = h, g = 0, S = A = F), _ = F
+        h === _ ? (F < C ? C = F : F > A && (A = F), d = (g * d + z) / ++g) : (P(), t.lineTo(z, F), _ = h, g = 0, C = A = F), w = F
     }
-    M()
+    P()
 }
 
-function xg(t) {
+function vg(t) {
     let e = t.options,
         n = e.borderDash && e.borderDash.length;
     return !t._decimated && !t._loop && !e.tension && e.cubicInterpolationMode !== "monotone" && !e.stepped && !n ? oT : rT
 }
 
 function sT(t) {
-    return t.stepped ? Up : t.tension || t.cubicInterpolationMode === "monotone" ? $p : er
+    return t.stepped ? Vp : t.tension || t.cubicInterpolationMode === "monotone" ? Up : er
 }
 
 function aT(t, e, n, i) {
     let r = e._path;
     r || (r = e._path = new Path2D, e.path(r, n, i) && r.closePath()), qb(t, e.options), t.stroke(r)
 }
 
 function lT(t, e, n, i) {
     let {
         segments: r,
         options: o
-    } = e, s = xg(e);
+    } = e, s = vg(e);
     for (let a of r) qb(t, o, a.style), t.beginPath(), s(t, e, a, {
         start: n,
         end: n + i - 1
     }) && t.closePath(), t.stroke()
 }
 var uT = typeof Path2D == "function";
 
@@ -15331,25 +15331,25 @@
     constructor(e) {
         super(), this.animated = !0, this.options = void 0, this._chart = void 0, this._loop = void 0, this._fullLoop = void 0, this._path = void 0, this._points = void 0, this._segments = void 0, this._decimated = !1, this._pointsUpdated = !1, this._datasetIndex = void 0, e && Object.assign(this, e)
     }
     updateControlPoints(e, n) {
         let i = this.options;
         if ((i.tension || i.cubicInterpolationMode === "monotone") && !i.stepped && !this._pointsUpdated) {
             let r = i.spanGaps ? this._loop : this._fullLoop;
-            Bp(this._points, i, e, r, n), this._pointsUpdated = !0
+            Hp(this._points, i, e, r, n), this._pointsUpdated = !0
         }
     }
     set points(e) {
         this._points = e, delete this._segments, delete this._path, this._pointsUpdated = !1
     }
     get points() {
         return this._points
     }
     get segments() {
-        return this._segments || (this._segments = Yp(this, this.options.segment))
+        return this._segments || (this._segments = $p(this, this.options.segment))
     }
     first() {
         let e = this.segments,
             n = this.points;
         return e.length && n[e[0].start]
     }
     last() {
@@ -15358,44 +15358,44 @@
             i = e.length;
         return i && n[e[i - 1].end]
     }
     interpolate(e, n) {
         let i = this.options,
             r = e[n],
             o = this.points,
-            s = nf(this, {
+            s = rf(this, {
                 property: n,
                 start: r,
                 end: r
             });
         if (!s.length) return;
         let a = [],
             l = sT(i),
             c, d;
         for (c = 0, d = s.length; c < d; ++c) {
             let {
                 start: g,
                 end: y
-            } = s[c], x = o[g], w = o[y];
-            if (x === w) {
+            } = s[c], x = o[g], _ = o[y];
+            if (x === _) {
                 a.push(x);
                 continue
             }
-            let S = Math.abs((r - x[n]) / (w[n] - x[n])),
-                A = l(x, w, S, i.stepped);
+            let C = Math.abs((r - x[n]) / (_[n] - x[n])),
+                A = l(x, _, C, i.stepped);
             A[n] = e[n], a.push(A)
         }
         return a.length === 1 ? a[0] : a
     }
     pathSegment(e, n, i) {
-        return xg(this)(e, this, n, i)
+        return vg(this)(e, this, n, i)
     }
     path(e, n, i) {
         let r = this.segments,
-            o = xg(this),
+            o = vg(this),
             s = this._loop;
         n = n || 0, i = i || this.points.length - n;
         for (let a of r) s &= o(e, this, a, {
             start: n,
             end: n + i - 1
         });
         return !!s
@@ -15409,15 +15409,15 @@
 function hb(t, e, n, i) {
     let r = t.options,
         {
             [n]: o
         } = t.getProps([n], i);
     return Math.abs(e - o) < r.radius + r.hitRadius
 }
-var bg = class extends zt {
+var xg = class extends zt {
     static id = "point";
     parsed;
     skip;
     stop;
     static defaults = {
         borderWidth: 1,
         hitRadius: 1,
@@ -15463,23 +15463,23 @@
         let n = e.radius || 0;
         n = Math.max(n, n && e.hoverRadius || 0);
         let i = n && e.borderWidth || 0;
         return (n + i) * 2
     }
     draw(e, n) {
         let i = this.options;
-        this.skip || i.radius < .1 || !ci(this, n, this.size(i) / 2) || (e.strokeStyle = i.borderColor, e.lineWidth = i.borderWidth, e.fillStyle = i.backgroundColor, ml(e, i, this.x, this.y))
+        this.skip || i.radius < .1 || !ci(this, n, this.size(i) / 2) || (e.strokeStyle = i.borderColor, e.lineWidth = i.borderWidth, e.fillStyle = i.backgroundColor, yl(e, i, this.x, this.y))
     }
     getRange() {
         let e = this.options || {};
         return e.radius + e.hitRadius
     }
 };
 
-function Gb(t, e) {
+function Kb(t, e) {
     let {
         x: n,
         y: i,
         base: r,
         width: o,
         height: s
     } = t.getProps(["x", "y", "base", "width", "height"], e), a, l, c, d, g;
@@ -15488,21 +15488,21 @@
         top: c,
         right: l,
         bottom: d
     }
 }
 
 function $r(t, e, n, i) {
-    return t ? 0 : St(e, n, i)
+    return t ? 0 : kt(e, n, i)
 }
 
 function fT(t, e, n) {
     let i = t.options.borderWidth,
         r = t.borderSkipped,
-        o = Xc(i);
+        o = qc(i);
     return {
         t: $r(r.top, o.top, 0, n),
         r: $r(r.right, o.right, 0, e),
         b: $r(r.bottom, o.bottom, 0, n),
         l: $r(r.left, o.left, 0, e)
     }
 }
@@ -15516,15 +15516,15 @@
         topRight: $r(!l || a.top || a.right, o.topRight, 0, s),
         bottomLeft: $r(!l || a.bottom || a.left, o.bottomLeft, 0, s),
         bottomRight: $r(!l || a.bottom || a.right, o.bottomRight, 0, s)
     }
 }
 
 function hT(t) {
-    let e = Gb(t),
+    let e = Kb(t),
         n = e.right - e.left,
         i = e.bottom - e.top,
         r = fT(t, n / 2, i / 2),
         o = dT(t, n / 2, i / 2);
     return {
         outer: {
             x: e.left,
@@ -15544,43 +15544,43 @@
                 bottomLeft: Math.max(0, o.bottomLeft - Math.max(r.b, r.l)),
                 bottomRight: Math.max(0, o.bottomRight - Math.max(r.b, r.r))
             }
         }
     }
 }
 
-function Jp(t, e, n, i) {
+function Qp(t, e, n, i) {
     let r = e === null,
         o = n === null,
-        a = t && !(r && o) && Gb(t, i);
+        a = t && !(r && o) && Kb(t, i);
     return a && (r || hi(e, a.left, a.right)) && (o || hi(n, a.top, a.bottom))
 }
 
 function pT(t) {
     return t.topLeft || t.topRight || t.bottomLeft || t.bottomRight
 }
 
 function gT(t, e) {
     t.rect(e.x, e.y, e.w, e.h)
 }
 
-function eg(t, e, n = {}) {
+function Jp(t, e, n = {}) {
     let i = t.x !== n.x ? -e : 0,
         r = t.y !== n.y ? -e : 0,
         o = (t.x + t.w !== n.x + n.w ? e : 0) - i,
         s = (t.y + t.h !== n.y + n.h ? e : 0) - r;
     return {
         x: t.x + i,
         y: t.y + r,
         w: t.w + o,
         h: t.h + s,
         radius: t.radius
     }
 }
-var _g = class extends zt {
+var bg = class extends zt {
         static id = "bar";
         static defaults = {
             borderSkipped: "start",
             borderWidth: 0,
             borderRadius: 0,
             inflateAmount: "auto",
             pointStyle: void 0
@@ -15599,24 +15599,24 @@
                     borderColor: i,
                     backgroundColor: r
                 }
             } = this, {
                 inner: o,
                 outer: s
             } = hT(this), a = pT(s.radius) ? rr : gT;
-            e.save(), (s.w !== o.w || s.h !== o.h) && (e.beginPath(), a(e, eg(s, n, o)), e.clip(), a(e, eg(o, -n, s)), e.fillStyle = i, e.fill("evenodd")), e.beginPath(), a(e, eg(o, n)), e.fillStyle = r, e.fill(), e.restore()
+            e.save(), (s.w !== o.w || s.h !== o.h) && (e.beginPath(), a(e, Jp(s, n, o)), e.clip(), a(e, Jp(o, -n, s)), e.fillStyle = i, e.fill("evenodd")), e.beginPath(), a(e, Jp(o, n)), e.fillStyle = r, e.fill(), e.restore()
         }
         inRange(e, n, i) {
-            return Jp(this, e, n, i)
+            return Qp(this, e, n, i)
         }
         inXRange(e, n) {
-            return Jp(this, e, null, n)
+            return Qp(this, e, null, n)
         }
         inYRange(e, n) {
-            return Jp(this, null, e, n)
+            return Qp(this, null, e, n)
         }
         getCenterPoint(e) {
             let {
                 x: n,
                 y: i,
                 base: r,
                 horizontal: o
@@ -15628,47 +15628,47 @@
         }
         getRange(e) {
             return e === "x" ? this.width / 2 : this.height / 2
         }
     },
     mT = Object.freeze({
         __proto__: null,
-        ArcElement: vg,
-        BarElement: _g,
+        ArcElement: yg,
+        BarElement: bg,
         LineElement: Fs,
-        PointElement: bg
+        PointElement: xg
     }),
-    wg = ["rgb(54, 162, 235)", "rgb(255, 99, 132)", "rgb(255, 159, 64)", "rgb(255, 205, 86)", "rgb(75, 192, 192)", "rgb(153, 102, 255)", "rgb(201, 203, 207)"],
-    pb = wg.map(t => t.replace("rgb(", "rgba(").replace(")", ", 0.5)"));
+    _g = ["rgb(54, 162, 235)", "rgb(255, 99, 132)", "rgb(255, 159, 64)", "rgb(255, 205, 86)", "rgb(75, 192, 192)", "rgb(153, 102, 255)", "rgb(201, 203, 207)"],
+    pb = _g.map(t => t.replace("rgb(", "rgba(").replace(")", ", 0.5)"));
 
-function Qb(t) {
-    return wg[t % wg.length]
+function Gb(t) {
+    return _g[t % _g.length]
 }
 
-function Kb(t) {
+function Qb(t) {
     return pb[t % pb.length]
 }
 
 function yT(t, e) {
-    return t.borderColor = Qb(e), t.backgroundColor = Kb(e), ++e
+    return t.borderColor = Gb(e), t.backgroundColor = Qb(e), ++e
 }
 
 function vT(t, e) {
-    return t.backgroundColor = t.data.map(() => Qb(e++)), e
+    return t.backgroundColor = t.data.map(() => Gb(e++)), e
 }
 
 function xT(t, e) {
-    return t.backgroundColor = t.data.map(() => Kb(e++)), e
+    return t.backgroundColor = t.data.map(() => Qb(e++)), e
 }
 
 function bT(t) {
     let e = 0;
     return (n, i) => {
         let r = t.getDatasetMeta(i).controller;
-        r instanceof Pl ? e = vT(n, e) : r instanceof hf ? e = xT(n, e) : r && (e = yT(n, e))
+        r instanceof Pl ? e = vT(n, e) : r instanceof pf ? e = xT(n, e) : r && (e = yT(n, e))
     }
 }
 
 function gb(t) {
     let e;
     for (e in t)
         if (t[e].borderColor || t[e].backgroundColor) return !0;
@@ -15696,68 +15696,68 @@
         } = r;
         if (!n.forceOverride && (gb(i) || _T(r) || o && gb(o))) return;
         let s = bT(t);
         i.forEach(s)
     }
 };
 
-function kT(t, e, n, i, r) {
+function ST(t, e, n, i, r) {
     let o = r.samples || i;
     if (o >= n) return t.slice(e, e + n);
     let s = [],
         a = (n - 2) / (o - 2),
         l = 0,
         c = e + n - 1,
         d = e,
-        g, y, x, w, S;
+        g, y, x, _, C;
     for (s[l++] = t[d], g = 0; g < o - 2; g++) {
         let A = 0,
-            _ = 0,
-            C, M = Math.floor((g + 1) * a) + 1 + e,
+            w = 0,
+            k, P = Math.floor((g + 1) * a) + 1 + e,
             z = Math.min(Math.floor((g + 2) * a) + 1, n) + e,
-            F = z - M;
-        for (C = M; C < z; C++) A += t[C].x, _ += t[C].y;
-        A /= F, _ /= F;
+            F = z - P;
+        for (k = P; k < z; k++) A += t[k].x, w += t[k].y;
+        A /= F, w /= F;
         let h = Math.floor(g * a) + 1 + e,
-            Y = Math.min(Math.floor((g + 1) * a) + 1, n) + e,
+            $ = Math.min(Math.floor((g + 1) * a) + 1, n) + e,
             {
-                x: V,
-                y: te
+                x: Y,
+                y: ne
             } = t[d];
-        for (x = w = -1, C = h; C < Y; C++) w = .5 * Math.abs((V - A) * (t[C].y - te) - (V - t[C].x) * (_ - te)), w > x && (x = w, y = t[C], S = C);
-        s[l++] = y, d = S
+        for (x = _ = -1, k = h; k < $; k++) _ = .5 * Math.abs((Y - A) * (t[k].y - ne) - (Y - t[k].x) * (w - ne)), _ > x && (x = _, y = t[k], C = k);
+        s[l++] = y, d = C
     }
     return s[l++] = t[c], s
 }
 
-function ST(t, e, n, i) {
+function kT(t, e, n, i) {
     let r = 0,
         o = 0,
-        s, a, l, c, d, g, y, x, w, S, A = [],
-        _ = e + n - 1,
-        C = t[e].x,
-        z = t[_].x - C;
+        s, a, l, c, d, g, y, x, _, C, A = [],
+        w = e + n - 1,
+        k = t[e].x,
+        z = t[w].x - k;
     for (s = e; s < e + n; ++s) {
-        a = t[s], l = (a.x - C) / z * i, c = a.y;
+        a = t[s], l = (a.x - k) / z * i, c = a.y;
         let F = l | 0;
-        if (F === d) c < w ? (w = c, g = s) : c > S && (S = c, y = s), r = (o * r + a.x) / ++o;
+        if (F === d) c < _ ? (_ = c, g = s) : c > C && (C = c, y = s), r = (o * r + a.x) / ++o;
         else {
             let h = s - 1;
             if (!Ie(g) && !Ie(y)) {
-                let Y = Math.min(g, y),
-                    V = Math.max(g, y);
-                Y !== x && Y !== h && A.push({
-                    ...t[Y],
+                let $ = Math.min(g, y),
+                    Y = Math.max(g, y);
+                $ !== x && $ !== h && A.push({
+                    ...t[$],
                     x: r
-                }), V !== x && V !== h && A.push({
-                    ...t[V],
+                }), Y !== x && Y !== h && A.push({
+                    ...t[Y],
                     x: r
                 })
             }
-            s > 0 && h !== x && A.push(t[h]), A.push(a), d = F, o = 0, w = S = c, g = y = x = s
+            s > 0 && h !== x && A.push(t[h]), A.push(a), d = F, o = 0, _ = C = c, g = y = x = s
         }
     }
     return A
 }
 
 function Jb(t) {
     if (t._decimated) {
@@ -15785,15 +15785,15 @@
         } = t,
         {
             min: s,
             max: a,
             minDefined: l,
             maxDefined: c
         } = o.getUserBounds();
-    return l && (i = St(ui(e, o.axis, s).lo, 0, n - 1)), c ? r = St(ui(e, o.axis, a).hi + 1, i, n) - i : r = n - i, {
+    return l && (i = kt(ui(e, o.axis, s).lo, 0, n - 1)), c ? r = kt(ui(e, o.axis, a).hi + 1, i, n) - i : r = n - i, {
         start: i,
         count: r
     }
 }
 var ET = {
     id: "decimation",
     defaults: {
@@ -15824,30 +15824,30 @@
             }
             Ie(s) && (r._data = c, delete r.data, Object.defineProperty(r, "data", {
                 configurable: !0,
                 enumerable: !0,
                 get: function() {
                     return this._decimated
                 },
-                set: function(S) {
-                    this._data = S
+                set: function(C) {
+                    this._data = C
                 }
             }));
-            let w;
+            let _;
             switch (n.algorithm) {
                 case "lttb":
-                    w = kT(c, g, y, i, n);
+                    _ = ST(c, g, y, i, n);
                     break;
                 case "min-max":
-                    w = ST(c, g, y, i);
+                    _ = kT(c, g, y, i);
                     break;
                 default:
                     throw new Error(`Unsupported decimation algorithm '${n.algorithm}'`)
             }
-            r._decimated = w
+            r._decimated = _
         })
     },
     destroy(t) {
         mb(t)
     }
 };
 
@@ -15857,65 +15857,65 @@
         o = e.points,
         s = [];
     for (let a of i) {
         let {
             start: l,
             end: c
         } = a;
-        c = Dg(l, c, r);
-        let d = kg(n, r[l], r[c], a.loop);
+        c = Pg(l, c, r);
+        let d = wg(n, r[l], r[c], a.loop);
         if (!e.segments) {
             s.push({
                 source: a,
                 target: d,
                 start: r[l],
                 end: r[c]
             });
             continue
         }
-        let g = nf(e, d);
+        let g = rf(e, d);
         for (let y of g) {
-            let x = kg(n, o[y.start], o[y.end], y.loop),
-                w = tf(a, r, x);
-            for (let S of w) s.push({
-                source: S,
+            let x = wg(n, o[y.start], o[y.end], y.loop),
+                _ = nf(a, r, x);
+            for (let C of _) s.push({
+                source: C,
                 target: y,
                 start: {
                     [n]: yb(d, x, "start", Math.max)
                 },
                 end: {
                     [n]: yb(d, x, "end", Math.min)
                 }
             })
         }
     }
     return s
 }
 
-function kg(t, e, n, i) {
+function wg(t, e, n, i) {
     if (i) return;
     let r = e[t],
         o = n[t];
     return t === "angle" && (r = on(r), o = on(o)), {
         property: t,
         start: r,
         end: o
     }
 }
 
-function PT(t, e) {
+function DT(t, e) {
     let {
         x: n = null,
         y: i = null
     } = t || {}, r = e.points, o = [];
     return e.segments.forEach(({
         start: s,
         end: a
     }) => {
-        a = Dg(s, a, r);
+        a = Pg(s, a, r);
         let l = r[s],
             c = r[a];
         i !== null ? (o.push({
             x: l.x,
             y: i
         }), o.push({
             x: c.x,
@@ -15926,58 +15926,58 @@
         }), o.push({
             x: n,
             y: c.y
         }))
     }), o
 }
 
-function Dg(t, e, n) {
+function Pg(t, e, n) {
     for (; e > t; e--) {
         let i = n[e];
         if (!isNaN(i.x) && !isNaN(i.y)) break
     }
     return e
 }
 
 function yb(t, e, n, i) {
     return t && e ? i(t[n], e[n]) : t ? t[n] : e ? e[n] : 0
 }
 
 function e1(t, e) {
     let n = [],
         i = !1;
-    return Re(t) ? (i = !0, n = t) : n = PT(t, e), n.length ? new Fs({
+    return Re(t) ? (i = !0, n = t) : n = DT(t, e), n.length ? new Fs({
         points: n,
         options: {
             tension: 0
         },
         _loop: i,
         _fullLoop: i
     }) : null
 }
 
 function vb(t) {
     return t && t.fill !== !1
 }
 
-function MT(t, e, n) {
+function PT(t, e, n) {
     let r = t[e].fill,
         o = [e],
         s;
     if (!n) return r;
     for (; r !== !1 && o.indexOf(r) === -1;) {
         if (!qe(r)) return r;
         if (s = t[r], !s) return !1;
         if (s.visible) return r;
         o.push(r), r = s.fill
     }
     return !1
 }
 
-function DT(t, e, n) {
+function MT(t, e, n) {
     let i = RT(t);
     if (we(i)) return isNaN(i.value) ? !1 : i;
     let r = parseFloat(i);
     return qe(r) && Math.floor(r) === r ? OT(i[0], e, r, n) : ["origin", "start", "end", "stack", "shape"].indexOf(i) >= 0 && i
 }
 
 function OT(t, e, n, i) {
@@ -16068,15 +16068,15 @@
     }
     return {
         first: a,
         last: l,
         point: i
     }
 }
-var yf = class {
+var vf = class {
     constructor(e) {
         this.x = e.x, this.y = e.y, this.radius = e.radius
     }
     pathSegment(e, n, i) {
         let {
             x: r,
             y: o,
@@ -16107,15 +16107,15 @@
         fill: n,
         line: i
     } = t;
     if (qe(n)) return HT(e, n);
     if (n === "stack") return IT(t);
     if (n === "shape") return !0;
     let r = BT(t);
-    return r instanceof yf ? r : e1(r, i)
+    return r instanceof vf ? r : e1(r, i)
 }
 
 function HT(t, e) {
     let n = t.getDatasetMeta(e);
     return n && t.isDatasetVisible(e) ? n.dataset : null
 }
 
@@ -16141,25 +16141,25 @@
 function VT(t) {
     let {
         scale: e,
         fill: n
     } = t, i = e.options, r = e.getLabels().length, o = i.reverse ? e.max : e.min, s = LT(n, e, o), a = [];
     if (i.grid.circular) {
         let l = e.getPointPositionForValue(0, o);
-        return new yf({
+        return new vf({
             x: l.x,
             y: l.y,
             radius: e.getDistanceFromCenterForValue(s)
         })
     }
     for (let l = 0; l < r; ++l) a.push(e.getPointPositionForValue(l, s));
     return a
 }
 
-function tg(t, e, n) {
+function eg(t, e, n) {
     let i = jT(e),
         {
             line: r,
             scale: o,
             axis: s
         } = e,
         a = r.options,
@@ -16210,15 +16210,15 @@
         points: r
     } = e, o = !0, s = !1;
     t.beginPath();
     for (let a of i) {
         let {
             start: l,
             end: c
-        } = a, d = r[l], g = r[Dg(l, c, r)];
+        } = a, d = r[l], g = r[Pg(l, c, r)];
         o ? (t.moveTo(d.x, d.y), o = !1) : (t.lineTo(d.x, n), t.lineTo(d.x, d.y)), s = !!e.pathSegment(t, a, {
             move: s
         }), s ? t.closePath() : t.lineTo(g.x, n)
     }
     t.lineTo(e.first().x, n), t.closePath(), t.clip()
 }
 
@@ -16238,26 +16238,26 @@
         }
         of a) {
         let {
             style: {
                 backgroundColor: y = o
             } = {}
         } = l, x = i !== !0;
-        t.save(), t.fillStyle = y, $T(t, s, x && kg(r, d, g)), t.beginPath();
-        let w = !!n.pathSegment(t, l),
-            S;
+        t.save(), t.fillStyle = y, $T(t, s, x && wg(r, d, g)), t.beginPath();
+        let _ = !!n.pathSegment(t, l),
+            C;
         if (x) {
-            w ? t.closePath() : _b(t, i, g, r);
+            _ ? t.closePath() : _b(t, i, g, r);
             let A = !!i.pathSegment(t, c, {
-                move: w,
+                move: _,
                 reverse: !0
             });
-            S = w && A, S || _b(t, i, d, r)
+            C = _ && A, C || _b(t, i, d, r)
         }
-        t.closePath(), t.fill(S ? "evenodd" : "nonzero"), t.restore()
+        t.closePath(), t.fill(C ? "evenodd" : "nonzero"), t.restore()
     }
 }
 
 function $T(t, e, n) {
     let {
         top: i,
         bottom: r
@@ -16278,42 +16278,42 @@
         afterDatasetsUpdate(t, e, n) {
             let i = (t.data.datasets || []).length,
                 r = [],
                 o, s, a, l;
             for (s = 0; s < i; ++s) o = t.getDatasetMeta(s), a = o.dataset, l = null, a && a.options && a instanceof Fs && (l = {
                 visible: t.isDatasetVisible(s),
                 index: s,
-                fill: DT(a, s, i),
+                fill: MT(a, s, i),
                 chart: t,
                 axis: o.controller.options.indexAxis,
                 scale: o.vScale,
                 line: a
             }), o.$filler = l, r.push(l);
-            for (s = 0; s < i; ++s) l = r[s], !(!l || l.fill === !1) && (l.fill = MT(r, s, n.propagate))
+            for (s = 0; s < i; ++s) l = r[s], !(!l || l.fill === !1) && (l.fill = PT(r, s, n.propagate))
         },
         beforeDraw(t, e, n) {
             let i = n.drawTime === "beforeDraw",
                 r = t.getSortedVisibleDatasetMetas(),
                 o = t.chartArea;
             for (let s = r.length - 1; s >= 0; --s) {
                 let a = r[s].$filler;
-                a && (a.line.updateControlPoints(o, a.axis), i && a.fill && tg(t.ctx, a, o))
+                a && (a.line.updateControlPoints(o, a.axis), i && a.fill && eg(t.ctx, a, o))
             }
         },
         beforeDatasetsDraw(t, e, n) {
             if (n.drawTime !== "beforeDatasetsDraw") return;
             let i = t.getSortedVisibleDatasetMetas();
             for (let r = i.length - 1; r >= 0; --r) {
                 let o = i[r].$filler;
-                vb(o) && tg(t.ctx, o, t.chartArea)
+                vb(o) && eg(t.ctx, o, t.chartArea)
             }
         },
         beforeDatasetDraw(t, e, n) {
             let i = e.meta.$filler;
-            !vb(i) || n.drawTime !== "beforeDatasetDraw" || tg(t.ctx, i, t.chartArea)
+            !vb(i) || n.drawTime !== "beforeDatasetDraw" || eg(t.ctx, i, t.chartArea)
         },
         defaults: {
             propagate: !0,
             drawTime: "beforeDatasetDraw"
         }
     },
     wb = (t, e) => {
@@ -16324,15 +16324,15 @@
         return t.usePointStyle && (n = Math.min(n, e), i = t.pointStyleWidth || Math.min(i, e)), {
             boxWidth: i,
             boxHeight: n,
             itemHeight: Math.max(e, n)
         }
     },
     XT = (t, e) => t !== null && e !== null && t.datasetIndex === e.datasetIndex && t.index === e.index,
-    vf = class extends zt {
+    xf = class extends zt {
         constructor(e) {
             super(), this._added = !1, this.legendHitBoxes = [], this._hoveredItem = null, this.doughnutMode = !1, this.chart = e.chart, this.options = e.options, this.ctx = e.ctx, this.legendItems = void 0, this.columnSizes = void 0, this.lineWidths = void 0, this.maxHeight = void 0, this.maxWidth = void 0, this.top = void 0, this.bottom = void 0, this.left = void 0, this.right = void 0, this.height = void 0, this.width = void 0, this._margins = void 0, this.position = void 0, this.weight = void 0, this.fullSize = void 0
         }
         update(e, n, i) {
             this.maxWidth = e, this.maxHeight = n, this._margins = i, this.setDimensions(), this.buildLabels(), this.fit()
         }
         setDimensions() {
@@ -16372,17 +16372,17 @@
                         padding: a
                     }
                 }
             } = this, l = this.legendHitBoxes = [], c = this.lineWidths = [0], d = r + a, g = e;
             o.textAlign = "left", o.textBaseline = "middle";
             let y = -1,
                 x = -d;
-            return this.legendItems.forEach((w, S) => {
-                let A = i + n / 2 + o.measureText(w.text).width;
-                (S === 0 || c[c.length - 1] + A + 2 * a > s) && (g += d, c[c.length - (S > 0 ? 0 : 1)] = 0, x += d, y++), l[S] = {
+            return this.legendItems.forEach((_, C) => {
+                let A = i + n / 2 + o.measureText(_.text).width;
+                (C === 0 || c[c.length - 1] + A + 2 * a > s) && (g += d, c[c.length - (C > 0 ? 0 : 1)] = 0, x += d, y++), l[C] = {
                     left: 0,
                     top: x,
                     row: y,
                     width: A,
                     height: r
                 }, c[c.length - 1] += A + a
             }), g
@@ -16392,30 +16392,30 @@
                 ctx: o,
                 maxHeight: s,
                 options: {
                     labels: {
                         padding: a
                     }
                 }
-            } = this, l = this.legendHitBoxes = [], c = this.columnSizes = [], d = s - e, g = a, y = 0, x = 0, w = 0, S = 0;
-            return this.legendItems.forEach((A, _) => {
+            } = this, l = this.legendHitBoxes = [], c = this.columnSizes = [], d = s - e, g = a, y = 0, x = 0, _ = 0, C = 0;
+            return this.legendItems.forEach((A, w) => {
                 let {
-                    itemWidth: C,
-                    itemHeight: M
+                    itemWidth: k,
+                    itemHeight: P
                 } = qT(i, n, o, A, r);
-                _ > 0 && x + M + 2 * a > d && (g += y + a, c.push({
+                w > 0 && x + P + 2 * a > d && (g += y + a, c.push({
                     width: y,
                     height: x
-                }), w += y + a, S++, y = x = 0), l[_] = {
-                    left: w,
+                }), _ += y + a, C++, y = x = 0), l[w] = {
+                    left: _,
                     top: x,
-                    col: S,
-                    width: C,
-                    height: M
-                }, y = Math.max(y, C), x += M + a
+                    col: C,
+                    width: k,
+                    height: P
+                }, y = Math.max(y, k), x += P + a
             }), g += y, c.push({
                 width: y,
                 height: x
             }), g
         }
         adjustHitBoxes() {
             if (!this.options.display) return;
@@ -16460,75 +16460,75 @@
                 align: o,
                 labels: s
             } = e, a = rt.color, l = Ur(e.rtl, this.left, this.width), c = tt(s.font), {
                 padding: d
             } = s, g = c.size, y = g / 2, x;
             this.drawTitle(), r.textAlign = l.textAlign("left"), r.textBaseline = "middle", r.lineWidth = .5, r.font = c.string;
             let {
-                boxWidth: w,
-                boxHeight: S,
+                boxWidth: _,
+                boxHeight: C,
                 itemHeight: A
-            } = wb(s, g), _ = function(h, Y, V) {
-                if (isNaN(w) || w <= 0 || isNaN(S) || S < 0) return;
+            } = wb(s, g), w = function(h, $, Y) {
+                if (isNaN(_) || _ <= 0 || isNaN(C) || C < 0) return;
                 r.save();
-                let te = pe(V.lineWidth, 1);
-                if (r.fillStyle = pe(V.fillStyle, a), r.lineCap = pe(V.lineCap, "butt"), r.lineDashOffset = pe(V.lineDashOffset, 0), r.lineJoin = pe(V.lineJoin, "miter"), r.lineWidth = te, r.strokeStyle = pe(V.strokeStyle, a), r.setLineDash(pe(V.lineDash, [])), s.usePointStyle) {
+                let ne = pe(Y.lineWidth, 1);
+                if (r.fillStyle = pe(Y.fillStyle, a), r.lineCap = pe(Y.lineCap, "butt"), r.lineDashOffset = pe(Y.lineDashOffset, 0), r.lineJoin = pe(Y.lineJoin, "miter"), r.lineWidth = ne, r.strokeStyle = pe(Y.strokeStyle, a), r.setLineDash(pe(Y.lineDash, [])), s.usePointStyle) {
                     let ie = {
-                            radius: S * Math.SQRT2 / 2,
-                            pointStyle: V.pointStyle,
-                            rotation: V.rotation,
-                            borderWidth: te
+                            radius: C * Math.SQRT2 / 2,
+                            pointStyle: Y.pointStyle,
+                            rotation: Y.rotation,
+                            borderWidth: ne
                         },
-                        ce = l.xPlus(h, w / 2),
-                        he = Y + y;
-                    Yc(r, ie, ce, he, s.pointStyleWidth && w)
+                        ce = l.xPlus(h, _ / 2),
+                        he = $ + y;
+                    Xc(r, ie, ce, he, s.pointStyleWidth && _)
                 } else {
-                    let ie = Y + Math.max((g - S) / 2, 0),
-                        ce = l.leftForLtr(h, w),
-                        he = pi(V.borderRadius);
+                    let ie = $ + Math.max((g - C) / 2, 0),
+                        ce = l.leftForLtr(h, _),
+                        he = pi(Y.borderRadius);
                     r.beginPath(), Object.values(he).some(Fe => Fe !== 0) ? rr(r, {
                         x: ce,
                         y: ie,
-                        w,
-                        h: S,
+                        w: _,
+                        h: C,
                         radius: he
-                    }) : r.rect(ce, ie, w, S), r.fill(), te !== 0 && r.stroke()
+                    }) : r.rect(ce, ie, _, C), r.fill(), ne !== 0 && r.stroke()
                 }
                 r.restore()
-            }, C = function(h, Y, V) {
-                ir(r, V.text, h, Y + A / 2, c, {
-                    strikethrough: V.hidden,
-                    textAlign: l.textAlign(V.textAlign)
+            }, k = function(h, $, Y) {
+                ir(r, Y.text, h, $ + A / 2, c, {
+                    strikethrough: Y.hidden,
+                    textAlign: l.textAlign(Y.textAlign)
                 })
-            }, M = this.isHorizontal(), z = this._computeTitleHeight();
-            M ? x = {
+            }, P = this.isHorizontal(), z = this._computeTitleHeight();
+            P ? x = {
                 x: Nt(o, this.left + d, this.right - i[0]),
                 y: this.top + d + z,
                 line: 0
             } : x = {
                 x: this.left + d,
                 y: Nt(o, this.top + z + d, this.bottom - n[0].height),
                 line: 0
-            }, Jc(this.ctx, e.textDirection);
+            }, ef(this.ctx, e.textDirection);
             let F = A + d;
-            this.legendItems.forEach((h, Y) => {
+            this.legendItems.forEach((h, $) => {
                 r.strokeStyle = h.fontColor, r.fillStyle = h.fontColor;
-                let V = r.measureText(h.text).width,
-                    te = l.textAlign(h.textAlign || (h.textAlign = s.textAlign)),
-                    ie = w + y + V,
+                let Y = r.measureText(h.text).width,
+                    ne = l.textAlign(h.textAlign || (h.textAlign = s.textAlign)),
+                    ie = _ + y + Y,
                     ce = x.x,
                     he = x.y;
-                l.setWidth(this.width), M ? Y > 0 && ce + ie + d > this.right && (he = x.y += F, x.line++, ce = x.x = Nt(o, this.left + d, this.right - i[x.line])) : Y > 0 && he + F > this.bottom && (ce = x.x = ce + n[x.line].width + d, x.line++, he = x.y = Nt(o, this.top + z + d, this.bottom - n[x.line].height));
+                l.setWidth(this.width), P ? $ > 0 && ce + ie + d > this.right && (he = x.y += F, x.line++, ce = x.x = Nt(o, this.left + d, this.right - i[x.line])) : $ > 0 && he + F > this.bottom && (ce = x.x = ce + n[x.line].width + d, x.line++, he = x.y = Nt(o, this.top + z + d, this.bottom - n[x.line].height));
                 let Fe = l.x(ce);
-                if (_(Fe, he, h), ce = Rp(te, ce + w + y, M ? ce + ie : this.right, e.rtl), C(l.x(ce), he, h), M) x.x += ie + d;
+                if (w(Fe, he, h), ce = Lp(ne, ce + _ + y, P ? ce + ie : this.right, e.rtl), k(l.x(ce), he, h), P) x.x += ie + d;
                 else if (typeof h.text != "string") {
                     let Ze = c.lineHeight;
                     x.y += t1(h, Ze) + d
                 } else x.y += F
-            }), ef(this.ctx, e.textDirection)
+            }), tf(this.ctx, e.textDirection)
         }
         drawTitle() {
             let e = this.options,
                 n = e.title,
                 i = tt(n.font),
                 r = gt(n.padding);
             if (!n.display) return;
@@ -16537,19 +16537,19 @@
                 a = n.position,
                 l = i.size / 2,
                 c = r.top + l,
                 d, g = this.left,
                 y = this.width;
             if (this.isHorizontal()) y = Math.max(...this.lineWidths), d = this.top + c, g = Nt(e.align, g, this.right - y);
             else {
-                let w = this.columnSizes.reduce((S, A) => Math.max(S, A.height), 0);
-                d = c + Nt(e.align, this.top, this.bottom - w - e.labels.padding - this._computeTitleHeight())
+                let _ = this.columnSizes.reduce((C, A) => Math.max(C, A.height), 0);
+                d = c + Nt(e.align, this.top, this.bottom - _ - e.labels.padding - this._computeTitleHeight())
             }
             let x = Nt(a, g, g + y);
-            s.textAlign = o.textAlign(pl(a)), s.textBaseline = "middle", s.strokeStyle = n.color, s.fillStyle = n.color, s.font = i.string, ir(s, n.text, x, d, i)
+            s.textAlign = o.textAlign(gl(a)), s.textBaseline = "middle", s.strokeStyle = n.color, s.fillStyle = n.color, s.font = i.string, ir(s, n.text, x, d, i)
         }
         _computeTitleHeight() {
             let e = this.options.title,
                 n = tt(e.font),
                 i = gt(e.padding);
             return e.display ? n.lineHeight + i.height : 0
         }
@@ -16559,56 +16559,56 @@
                 for (o = this.legendHitBoxes, i = 0; i < o.length; ++i)
                     if (r = o[i], hi(e, r.left, r.left + r.width) && hi(n, r.top, r.top + r.height)) return this.legendItems[i]
             }
             return null
         }
         handleEvent(e) {
             let n = this.options;
-            if (!QT(e.type, n)) return;
+            if (!GT(e.type, n)) return;
             let i = this._getLegendItemAt(e.x, e.y);
             if (e.type === "mousemove" || e.type === "mouseout") {
                 let r = this._hoveredItem,
                     o = XT(r, i);
                 r && !o && ve(n.onLeave, [e, r, this], this), this._hoveredItem = i, i && !o && ve(n.onHover, [e, i, this], this)
             } else i && ve(n.onClick, [e, i, this], this)
         }
     };
 
 function qT(t, e, n, i, r) {
     let o = ZT(i, t, e, n),
-        s = GT(r, i, e.lineHeight);
+        s = KT(r, i, e.lineHeight);
     return {
         itemWidth: o,
         itemHeight: s
     }
 }
 
 function ZT(t, e, n, i) {
     let r = t.text;
     return r && typeof r != "string" && (r = r.reduce((o, s) => o.length > s.length ? o : s)), e + n.size / 2 + i.measureText(r).width
 }
 
-function GT(t, e, n) {
+function KT(t, e, n) {
     let i = t;
     return typeof e.text != "string" && (i = t1(e, n)), i
 }
 
 function t1(t, e) {
     let n = t.text ? t.text.length : 0;
     return e * n
 }
 
-function QT(t, e) {
+function GT(t, e) {
     return !!((t === "mousemove" || t === "mouseout") && (e.onHover || e.onLeave) || e.onClick && (t === "click" || t === "mouseup"))
 }
-var KT = {
+var QT = {
         id: "legend",
-        _element: vf,
+        _element: xf,
         start(t, e, n) {
-            let i = t.legend = new vf({
+            let i = t.legend = new xf({
                 ctx: t.ctx,
                 options: n,
                 chart: t
             });
             Jt.configure(t, i, n), Jt.addBox(t, i)
         },
         stop(t) {
@@ -16688,15 +16688,15 @@
         descriptors: {
             _scriptable: t => !t.startsWith("on"),
             labels: {
                 _scriptable: t => !["generateLabels", "filter", "sort"].includes(t)
             }
         }
     },
-    Dl = class extends zt {
+    Ol = class extends zt {
         constructor(e) {
             super(), this.chart = e.chart, this.options = e.options, this.ctx = e.ctx, this._padding = void 0, this.top = void 0, this.bottom = void 0, this.left = void 0, this.right = void 0, this.width = void 0, this.height = void 0, this.position = void 0, this.weight = void 0, this.fullSize = void 0
         }
         update(e, n) {
             let i = this.options;
             if (this.left = 0, this.top = 0, !i.display) {
                 this.width = this.height = this.right = this.bottom = 0;
@@ -16739,32 +16739,32 @@
                     maxWidth: l,
                     rotation: c
                 } = this._drawArgs(o);
             ir(e, n.text, 0, 0, i, {
                 color: n.color,
                 maxWidth: l,
                 rotation: c,
-                textAlign: pl(n.align),
+                textAlign: gl(n.align),
                 textBaseline: "middle",
                 translation: [s, a]
             })
         }
     };
 
 function JT(t, e) {
-    let n = new Dl({
+    let n = new Ol({
         ctx: t.ctx,
         options: e,
         chart: t
     });
     Jt.configure(t, n, e), Jt.addBox(t, n), t.titleBlock = n
 }
 var e2 = {
         id: "title",
-        _element: Dl,
+        _element: Ol,
         start(t, e, n) {
             JT(t, n)
         },
         stop(t) {
             let e = t.titleBlock;
             Jt.removeBox(t, e), delete t.titleBlock
         },
@@ -16788,30 +16788,30 @@
             color: "color"
         },
         descriptors: {
             _scriptable: !0,
             _indexable: !1
         }
     },
-    lf = new WeakMap,
+    uf = new WeakMap,
     t2 = {
         id: "subtitle",
         start(t, e, n) {
-            let i = new Dl({
+            let i = new Ol({
                 ctx: t.ctx,
                 options: n,
                 chart: t
             });
-            Jt.configure(t, i, n), Jt.addBox(t, i), lf.set(t, i)
+            Jt.configure(t, i, n), Jt.addBox(t, i), uf.set(t, i)
         },
         stop(t) {
-            Jt.removeBox(t, lf.get(t)), lf.delete(t)
+            Jt.removeBox(t, uf.get(t)), uf.delete(t)
         },
         beforeUpdate(t, e, n) {
-            let i = lf.get(t);
+            let i = uf.get(t);
             Jt.configure(t, i, n), i.options = n
         },
         defaults: {
             align: "center",
             display: !1,
             font: {
                 weight: "normal"
@@ -16826,15 +16826,15 @@
             color: "color"
         },
         descriptors: {
             _scriptable: !0,
             _indexable: !1
         }
     },
-    Tl = {
+    Dl = {
         average(t) {
             if (!t.length) return !1;
             let e, n, i = new Set,
                 r = 0,
                 o = 0;
             for (e = 0, n = t.length; e < n; ++e) {
                 let a = t[e].element;
@@ -16901,15 +16901,15 @@
         dataset: o.getDataset(),
         dataIndex: r,
         datasetIndex: i,
         element: n
     }
 }
 
-function kb(t, e) {
+function Sb(t, e) {
     let n = t.chart.ctx,
         {
             body: i,
             footer: r,
             title: o
         } = t,
         {
@@ -16918,32 +16918,32 @@
         } = e,
         l = tt(e.bodyFont),
         c = tt(e.titleFont),
         d = tt(e.footerFont),
         g = o.length,
         y = r.length,
         x = i.length,
-        w = gt(e.padding),
-        S = w.height,
+        _ = gt(e.padding),
+        C = _.height,
         A = 0,
-        _ = i.reduce((z, F) => z + F.before.length + F.lines.length + F.after.length, 0);
-    if (_ += t.beforeBody.length + t.afterBody.length, g && (S += g * c.lineHeight + (g - 1) * e.titleSpacing + e.titleMarginBottom), _) {
+        w = i.reduce((z, F) => z + F.before.length + F.lines.length + F.after.length, 0);
+    if (w += t.beforeBody.length + t.afterBody.length, g && (C += g * c.lineHeight + (g - 1) * e.titleSpacing + e.titleMarginBottom), w) {
         let z = e.displayColors ? Math.max(a, l.lineHeight) : l.lineHeight;
-        S += x * z + (_ - x) * l.lineHeight + (_ - 1) * e.bodySpacing
+        C += x * z + (w - x) * l.lineHeight + (w - 1) * e.bodySpacing
     }
-    y && (S += e.footerMarginTop + y * d.lineHeight + (y - 1) * e.footerSpacing);
-    let C = 0,
-        M = function(z) {
-            A = Math.max(A, n.measureText(z).width + C)
+    y && (C += e.footerMarginTop + y * d.lineHeight + (y - 1) * e.footerSpacing);
+    let k = 0,
+        P = function(z) {
+            A = Math.max(A, n.measureText(z).width + k)
         };
-    return n.save(), n.font = c.string, Se(t.title, M), n.font = l.string, Se(t.beforeBody.concat(t.afterBody), M), C = e.displayColors ? s + 2 + e.boxPadding : 0, Se(i, z => {
-        Se(z.before, M), Se(z.lines, M), Se(z.after, M)
-    }), C = 0, n.font = d.string, Se(t.footer, M), n.restore(), A += w.width, {
+    return n.save(), n.font = c.string, ke(t.title, P), n.font = l.string, ke(t.beforeBody.concat(t.afterBody), P), k = e.displayColors ? s + 2 + e.boxPadding : 0, ke(i, z => {
+        ke(z.before, P), ke(z.lines, P), ke(z.after, P)
+    }), k = 0, n.font = d.string, ke(t.footer, P), n.restore(), A += _.width, {
         width: A,
-        height: S
+        height: C
     }
 }
 
 function i2(t, e) {
     let {
         y: n,
         height: i
@@ -16969,15 +16969,15 @@
             left: a,
             right: l
         }
     } = t, c = "center";
     return i === "center" ? c = r <= (a + l) / 2 ? "left" : "right" : r <= o / 2 ? c = "left" : r >= s - o / 2 && (c = "right"), r2(c, t, e, n) && (c = "center"), c
 }
 
-function Sb(t, e, n) {
+function kb(t, e, n) {
     let i = n.yAlign || e.yAlign || i2(t, n);
     return {
         xAlign: n.xAlign || e.xAlign || o2(t, e, n, i),
         yAlign: i
     }
 }
 
@@ -17006,22 +17006,22 @@
         xAlign: a,
         yAlign: l
     } = n, c = r + o, {
         topLeft: d,
         topRight: g,
         bottomLeft: y,
         bottomRight: x
-    } = pi(s), w = s2(e, a), S = a2(e, l, c);
-    return l === "center" ? a === "left" ? w += c : a === "right" && (w -= c) : a === "left" ? w -= Math.max(d, y) + r : a === "right" && (w += Math.max(g, x) + r), {
-        x: St(w, 0, i.width - e.width),
-        y: St(S, 0, i.height - e.height)
+    } = pi(s), _ = s2(e, a), C = a2(e, l, c);
+    return l === "center" ? a === "left" ? _ += c : a === "right" && (_ -= c) : a === "left" ? _ -= Math.max(d, y) + r : a === "right" && (_ += Math.max(g, x) + r), {
+        x: kt(_, 0, i.width - e.width),
+        y: kt(C, 0, i.height - e.height)
     }
 }
 
-function uf(t, e, n) {
+function cf(t, e, n) {
     let i = gt(n.padding);
     return e === "center" ? t.x + t.width / 2 : e === "right" ? t.x + t.width - i.right : t.x + i.left
 }
 
 function Eb(t) {
     return Ti([], sr(t))
 }
@@ -17089,16 +17089,16 @@
     afterFooter: fi
 };
 
 function _n(t, e, n, i) {
     let r = t[e].call(n, i);
     return typeof r > "u" ? n1[e].call(n, i) : r
 }
-var xf = class extends zt {
-        static positioners = Tl;
+var bf = class extends zt {
+        static positioners = Dl;
         constructor(e) {
             super(), this.opacity = 0, this._active = [], this._eventPosition = void 0, this._size = void 0, this._cachedAnimations = void 0, this._tooltipItems = [], this.$animations = void 0, this.$context = void 0, this.chart = e.chart, this.options = e.options, this.dataPoints = void 0, this.title = void 0, this.beforeBody = void 0, this.body = void 0, this.afterBody = void 0, this.footer = void 0, this.xAlign = void 0, this.yAlign = void 0, this.x = void 0, this.y = void 0, this.height = void 0, this.width = void 0, this.caretX = void 0, this.caretY = void 0, this.labelColors = void 0, this.labelPointStyles = void 0, this.labelTextColors = void 0
         }
         initialize(e) {
             this.options = e, this._cachedAnimations = void 0, this.$context = void 0
         }
         _resolveAnimations() {
@@ -17122,15 +17122,15 @@
         getBeforeBody(e, n) {
             return Eb(_n(n.callbacks, "beforeBody", this, e))
         }
         getBody(e, n) {
             let {
                 callbacks: i
             } = n, r = [];
-            return Se(e, o => {
+            return ke(e, o => {
                 let s = {
                         before: [],
                         lines: [],
                         after: []
                     },
                     a = Tb(i, o);
                 Ti(s.before, sr(_n(a, "beforeLabel", this, o))), Ti(s.lines, _n(a, "label", this, o)), Ti(s.after, sr(_n(a, "afterLabel", this, o))), r.push(s)
@@ -17150,32 +17150,32 @@
                 i = this.chart.data,
                 r = [],
                 o = [],
                 s = [],
                 a = [],
                 l, c;
             for (l = 0, c = n.length; l < c; ++l) a.push(n2(this.chart, n[l]));
-            return e.filter && (a = a.filter((d, g, y) => e.filter(d, g, y, i))), e.itemSort && (a = a.sort((d, g) => e.itemSort(d, g, i))), Se(a, d => {
+            return e.filter && (a = a.filter((d, g, y) => e.filter(d, g, y, i))), e.itemSort && (a = a.sort((d, g) => e.itemSort(d, g, i))), ke(a, d => {
                 let g = Tb(e.callbacks, d);
                 r.push(_n(g, "labelColor", this, d)), o.push(_n(g, "labelPointStyle", this, d)), s.push(_n(g, "labelTextColor", this, d))
             }), this.labelColors = r, this.labelPointStyles = o, this.labelTextColors = s, this.dataPoints = a, a
         }
         update(e, n) {
             let i = this.options.setContext(this.getContext()),
                 r = this._active,
                 o, s = [];
             if (!r.length) this.opacity !== 0 && (o = {
                 opacity: 0
             });
             else {
-                let a = Tl[i.position].call(this, r, this._eventPosition);
+                let a = Dl[i.position].call(this, r, this._eventPosition);
                 s = this._createItems(i), this.title = this.getTitle(s, i), this.beforeBody = this.getBeforeBody(s, i), this.body = this.getBody(s, i), this.afterBody = this.getAfterBody(s, i), this.footer = this.getFooter(s, i);
-                let l = this._size = kb(this, i),
+                let l = this._size = Sb(this, i),
                     c = Object.assign({}, a, l),
-                    d = Sb(this.chart, i, c),
+                    d = kb(this.chart, i, c),
                     g = Cb(i, c, d, this.chart);
                 this.xAlign = d.xAlign, this.yAlign = d.yAlign, o = {
                     opacity: 1,
                     x: g.x,
                     y: g.y,
                     width: l.width,
                     height: l.height,
@@ -17205,104 +17205,104 @@
                 topRight: c,
                 bottomLeft: d,
                 bottomRight: g
             } = pi(a), {
                 x: y,
                 y: x
             } = e, {
-                width: w,
-                height: S
-            } = n, A, _, C, M, z, F;
-            return o === "center" ? (z = x + S / 2, r === "left" ? (A = y, _ = A - s, M = z + s, F = z - s) : (A = y + w, _ = A + s, M = z - s, F = z + s), C = A) : (r === "left" ? _ = y + Math.max(l, d) + s : r === "right" ? _ = y + w - Math.max(c, g) - s : _ = this.caretX, o === "top" ? (M = x, z = M - s, A = _ - s, C = _ + s) : (M = x + S, z = M + s, A = _ + s, C = _ - s), F = M), {
+                width: _,
+                height: C
+            } = n, A, w, k, P, z, F;
+            return o === "center" ? (z = x + C / 2, r === "left" ? (A = y, w = A - s, P = z + s, F = z - s) : (A = y + _, w = A + s, P = z - s, F = z + s), k = A) : (r === "left" ? w = y + Math.max(l, d) + s : r === "right" ? w = y + _ - Math.max(c, g) - s : w = this.caretX, o === "top" ? (P = x, z = P - s, A = w - s, k = w + s) : (P = x + C, z = P + s, A = w + s, k = w - s), F = P), {
                 x1: A,
-                x2: _,
-                x3: C,
-                y1: M,
+                x2: w,
+                x3: k,
+                y1: P,
                 y2: z,
                 y3: F
             }
         }
         drawTitle(e, n, i) {
             let r = this.title,
                 o = r.length,
                 s, a, l;
             if (o) {
                 let c = Ur(i.rtl, this.x, this.width);
-                for (e.x = uf(this, i.titleAlign, i), n.textAlign = c.textAlign(i.titleAlign), n.textBaseline = "middle", s = tt(i.titleFont), a = i.titleSpacing, n.fillStyle = i.titleColor, n.font = s.string, l = 0; l < o; ++l) n.fillText(r[l], c.x(e.x), e.y + s.lineHeight / 2), e.y += s.lineHeight + a, l + 1 === o && (e.y += i.titleMarginBottom - a)
+                for (e.x = cf(this, i.titleAlign, i), n.textAlign = c.textAlign(i.titleAlign), n.textBaseline = "middle", s = tt(i.titleFont), a = i.titleSpacing, n.fillStyle = i.titleColor, n.font = s.string, l = 0; l < o; ++l) n.fillText(r[l], c.x(e.x), e.y + s.lineHeight / 2), e.y += s.lineHeight + a, l + 1 === o && (e.y += i.titleMarginBottom - a)
             }
         }
         _drawColorBox(e, n, i, r, o) {
             let s = this.labelColors[i],
                 a = this.labelPointStyles[i],
                 {
                     boxHeight: l,
                     boxWidth: c
                 } = o,
                 d = tt(o.bodyFont),
-                g = uf(this, "left", o),
+                g = cf(this, "left", o),
                 y = r.x(g),
                 x = l < d.lineHeight ? (d.lineHeight - l) / 2 : 0,
-                w = n.y + x;
+                _ = n.y + x;
             if (o.usePointStyle) {
-                let S = {
+                let C = {
                         radius: Math.min(c, l) / 2,
                         pointStyle: a.pointStyle,
                         rotation: a.rotation,
                         borderWidth: 1
                     },
                     A = r.leftForLtr(y, c) + c / 2,
-                    _ = w + l / 2;
-                e.strokeStyle = o.multiKeyBackground, e.fillStyle = o.multiKeyBackground, ml(e, S, A, _), e.strokeStyle = s.borderColor, e.fillStyle = s.backgroundColor, ml(e, S, A, _)
+                    w = _ + l / 2;
+                e.strokeStyle = o.multiKeyBackground, e.fillStyle = o.multiKeyBackground, yl(e, C, A, w), e.strokeStyle = s.borderColor, e.fillStyle = s.backgroundColor, yl(e, C, A, w)
             } else {
                 e.lineWidth = we(s.borderWidth) ? Math.max(...Object.values(s.borderWidth)) : s.borderWidth || 1, e.strokeStyle = s.borderColor, e.setLineDash(s.borderDash || []), e.lineDashOffset = s.borderDashOffset || 0;
-                let S = r.leftForLtr(y, c),
+                let C = r.leftForLtr(y, c),
                     A = r.leftForLtr(r.xPlus(y, 1), c - 2),
-                    _ = pi(s.borderRadius);
-                Object.values(_).some(C => C !== 0) ? (e.beginPath(), e.fillStyle = o.multiKeyBackground, rr(e, {
-                    x: S,
-                    y: w,
+                    w = pi(s.borderRadius);
+                Object.values(w).some(k => k !== 0) ? (e.beginPath(), e.fillStyle = o.multiKeyBackground, rr(e, {
+                    x: C,
+                    y: _,
                     w: c,
                     h: l,
-                    radius: _
+                    radius: w
                 }), e.fill(), e.stroke(), e.fillStyle = s.backgroundColor, e.beginPath(), rr(e, {
                     x: A,
-                    y: w + 1,
+                    y: _ + 1,
                     w: c - 2,
                     h: l - 2,
-                    radius: _
-                }), e.fill()) : (e.fillStyle = o.multiKeyBackground, e.fillRect(S, w, c, l), e.strokeRect(S, w, c, l), e.fillStyle = s.backgroundColor, e.fillRect(A, w + 1, c - 2, l - 2))
+                    radius: w
+                }), e.fill()) : (e.fillStyle = o.multiKeyBackground, e.fillRect(C, _, c, l), e.strokeRect(C, _, c, l), e.fillStyle = s.backgroundColor, e.fillRect(A, _ + 1, c - 2, l - 2))
             }
             e.fillStyle = this.labelTextColors[i]
         }
         drawBody(e, n, i) {
             let {
                 body: r
             } = this, {
                 bodySpacing: o,
                 bodyAlign: s,
                 displayColors: a,
                 boxHeight: l,
                 boxWidth: c,
                 boxPadding: d
-            } = i, g = tt(i.bodyFont), y = g.lineHeight, x = 0, w = Ur(i.rtl, this.x, this.width), S = function(V) {
-                n.fillText(V, w.x(e.x + x), e.y + y / 2), e.y += y + o
-            }, A = w.textAlign(s), _, C, M, z, F, h, Y;
-            for (n.textAlign = s, n.textBaseline = "middle", n.font = g.string, e.x = uf(this, A, i), n.fillStyle = i.bodyColor, Se(this.beforeBody, S), x = a && A !== "right" ? s === "center" ? c / 2 + d : c + 2 + d : 0, z = 0, h = r.length; z < h; ++z) {
-                for (_ = r[z], C = this.labelTextColors[z], n.fillStyle = C, Se(_.before, S), M = _.lines, a && M.length && (this._drawColorBox(n, e, z, w, i), y = Math.max(g.lineHeight, l)), F = 0, Y = M.length; F < Y; ++F) S(M[F]), y = g.lineHeight;
-                Se(_.after, S)
+            } = i, g = tt(i.bodyFont), y = g.lineHeight, x = 0, _ = Ur(i.rtl, this.x, this.width), C = function(Y) {
+                n.fillText(Y, _.x(e.x + x), e.y + y / 2), e.y += y + o
+            }, A = _.textAlign(s), w, k, P, z, F, h, $;
+            for (n.textAlign = s, n.textBaseline = "middle", n.font = g.string, e.x = cf(this, A, i), n.fillStyle = i.bodyColor, ke(this.beforeBody, C), x = a && A !== "right" ? s === "center" ? c / 2 + d : c + 2 + d : 0, z = 0, h = r.length; z < h; ++z) {
+                for (w = r[z], k = this.labelTextColors[z], n.fillStyle = k, ke(w.before, C), P = w.lines, a && P.length && (this._drawColorBox(n, e, z, _, i), y = Math.max(g.lineHeight, l)), F = 0, $ = P.length; F < $; ++F) C(P[F]), y = g.lineHeight;
+                ke(w.after, C)
             }
-            x = 0, y = g.lineHeight, Se(this.afterBody, S), e.y -= o
+            x = 0, y = g.lineHeight, ke(this.afterBody, C), e.y -= o
         }
         drawFooter(e, n, i) {
             let r = this.footer,
                 o = r.length,
                 s, a;
             if (o) {
                 let l = Ur(i.rtl, this.x, this.width);
-                for (e.x = uf(this, i.footerAlign, i), e.y += i.footerMarginTop, n.textAlign = l.textAlign(i.footerAlign), n.textBaseline = "middle", s = tt(i.footerFont), n.fillStyle = i.footerColor, n.font = s.string, a = 0; a < o; ++a) n.fillText(r[a], l.x(e.x), e.y + s.lineHeight / 2), e.y += s.lineHeight + i.footerSpacing
+                for (e.x = cf(this, i.footerAlign, i), e.y += i.footerMarginTop, n.textAlign = l.textAlign(i.footerAlign), n.textBaseline = "middle", s = tt(i.footerFont), n.fillStyle = i.footerColor, n.font = s.string, a = 0; a < o; ++a) n.fillText(r[a], l.x(e.x), e.y + s.lineHeight / 2), e.y += s.lineHeight + i.footerSpacing
             }
         }
         drawBackground(e, n, i, r) {
             let {
                 xAlign: o,
                 yAlign: s
             } = this, {
@@ -17311,29 +17311,29 @@
             } = e, {
                 width: c,
                 height: d
             } = i, {
                 topLeft: g,
                 topRight: y,
                 bottomLeft: x,
-                bottomRight: w
+                bottomRight: _
             } = pi(r.cornerRadius);
-            n.fillStyle = r.backgroundColor, n.strokeStyle = r.borderColor, n.lineWidth = r.borderWidth, n.beginPath(), n.moveTo(a + g, l), s === "top" && this.drawCaret(e, n, i, r), n.lineTo(a + c - y, l), n.quadraticCurveTo(a + c, l, a + c, l + y), s === "center" && o === "right" && this.drawCaret(e, n, i, r), n.lineTo(a + c, l + d - w), n.quadraticCurveTo(a + c, l + d, a + c - w, l + d), s === "bottom" && this.drawCaret(e, n, i, r), n.lineTo(a + x, l + d), n.quadraticCurveTo(a, l + d, a, l + d - x), s === "center" && o === "left" && this.drawCaret(e, n, i, r), n.lineTo(a, l + g), n.quadraticCurveTo(a, l, a + g, l), n.closePath(), n.fill(), r.borderWidth > 0 && n.stroke()
+            n.fillStyle = r.backgroundColor, n.strokeStyle = r.borderColor, n.lineWidth = r.borderWidth, n.beginPath(), n.moveTo(a + g, l), s === "top" && this.drawCaret(e, n, i, r), n.lineTo(a + c - y, l), n.quadraticCurveTo(a + c, l, a + c, l + y), s === "center" && o === "right" && this.drawCaret(e, n, i, r), n.lineTo(a + c, l + d - _), n.quadraticCurveTo(a + c, l + d, a + c - _, l + d), s === "bottom" && this.drawCaret(e, n, i, r), n.lineTo(a + x, l + d), n.quadraticCurveTo(a, l + d, a, l + d - x), s === "center" && o === "left" && this.drawCaret(e, n, i, r), n.lineTo(a, l + g), n.quadraticCurveTo(a, l, a + g, l), n.closePath(), n.fill(), r.borderWidth > 0 && n.stroke()
         }
         _updateAnimationTarget(e) {
             let n = this.chart,
                 i = this.$animations,
                 r = i && i.x,
                 o = i && i.y;
             if (r || o) {
-                let s = Tl[e.position].call(this, this._active, this._eventPosition);
+                let s = Dl[e.position].call(this, this._active, this._eventPosition);
                 if (!s) return;
-                let a = this._size = kb(this, e),
+                let a = this._size = Sb(this, e),
                     l = Object.assign({}, s, this._size),
-                    c = Sb(n, e, l),
+                    c = kb(n, e, l),
                     d = Cb(e, l, c, n);
                 (r._to !== d.x || o._to !== d.y) && (this.xAlign = c.xAlign, this.yAlign = c.yAlign, this.width = a.width, this.height = a.height, this.caretX = s.x, this.caretY = s.y, this._resolveAnimations().update(this, d))
             }
         }
         _willRender() {
             return !!this.opacity
         }
@@ -17349,15 +17349,15 @@
                 o = {
                     x: this.x,
                     y: this.y
                 };
             i = Math.abs(i) < .001 ? 0 : i;
             let s = gt(n.padding),
                 a = this.title.length || this.beforeBody.length || this.body.length || this.afterBody.length || this.footer.length;
-            n.enabled && a && (e.save(), e.globalAlpha = i, this.drawBackground(o, e, r, n), Jc(e, n.textDirection), o.y += s.top, this.drawTitle(o, e, n), this.drawBody(o, e, n), this.drawFooter(o, e, n), ef(e, n.textDirection), e.restore())
+            n.enabled && a && (e.save(), e.globalAlpha = i, this.drawBackground(o, e, r, n), ef(e, n.textDirection), o.y += s.top, this.drawTitle(o, e, n), this.drawBody(o, e, n), this.drawFooter(o, e, n), tf(e, n.textDirection), e.restore())
         }
         getActiveElements() {
             return this._active || []
         }
         setActiveElements(e, n) {
             let i = this._active,
                 r = e.map(({
@@ -17397,24 +17397,24 @@
             return o.reverse && s.reverse(), s
         }
         _positionChanged(e, n) {
             let {
                 caretX: i,
                 caretY: r,
                 options: o
-            } = this, s = Tl[o.position].call(this, e, n);
+            } = this, s = Dl[o.position].call(this, e, n);
             return s !== !1 && (i !== s.x || r !== s.y)
         }
     },
     u2 = {
         id: "tooltip",
-        _element: xf,
-        positioners: Tl,
+        _element: bf,
+        positioners: Dl,
         afterInit(t, e, n) {
-            n && (t.tooltip = new xf({
+            n && (t.tooltip = new bf({
                 chart: t,
                 options: n
             }))
         },
         beforeUpdate(t, e, n) {
             t.tooltip && t.tooltip.initialize(n)
         },
@@ -17512,15 +17512,15 @@
         additionalOptionScopes: ["interaction"]
     },
     c2 = Object.freeze({
         __proto__: null,
         Colors: wT,
         Decimation: ET,
         Filler: YT,
-        Legend: KT,
+        Legend: QT,
         SubTitle: t2,
         Title: e2,
         Tooltip: u2
     }),
     f2 = (t, e, n, i) => (typeof e == "string" ? (n = t.push(e) - 1, i.unshift({
         index: n,
         label: e
@@ -17528,25 +17528,25 @@
 
 function d2(t, e, n, i) {
     let r = t.indexOf(e);
     if (r === -1) return f2(t, e, n, i);
     let o = t.lastIndexOf(e);
     return r !== o ? n : r
 }
-var h2 = (t, e) => t === null ? null : St(Math.round(t), 0, e);
+var h2 = (t, e) => t === null ? null : kt(Math.round(t), 0, e);
 
-function Pb(t) {
+function Db(t) {
     let e = this.getLabels();
     return t >= 0 && t < e.length ? e[t] : t
 }
 var Sg = class extends Fo {
     static id = "category";
     static defaults = {
         ticks: {
-            callback: Pb
+            callback: Db
         }
     };
     constructor(e) {
         super(e), this._startValue = void 0, this._valueRange = 0, this._addedLabels = []
     }
     init(e) {
         let n = this._addedLabels;
@@ -17585,15 +17585,15 @@
         o = e === 0 && n === o.length - 1 ? o : o.slice(e, n + 1), this._valueRange = Math.max(o.length - (i ? 0 : 1), 1), this._startValue = this.min - (i ? .5 : 0);
         for (let s = e; s <= n; s++) r.push({
             value: s
         });
         return r
     }
     getLabelForValue(e) {
-        return Pb.call(this, e)
+        return Db.call(this, e)
     }
     configure() {
         super.configure(), this.isHorizontal() || (this._reversePixels = !this._reversePixels)
     }
     getPixelForValue(e) {
         return typeof e != "number" && (e = this.parse(e)), e === null ? NaN : this.getPixelForDecimal((e - this._startValue) / this._valueRange)
     }
@@ -17619,51 +17619,51 @@
             precision: l,
             count: c,
             maxTicks: d,
             maxDigits: g,
             includeBounds: y
         } = t,
         x = o || 1,
-        w = d - 1,
+        _ = d - 1,
         {
-            min: S,
+            min: C,
             max: A
         } = e,
-        _ = !Ie(s),
-        C = !Ie(a),
-        M = !Ie(c),
-        z = (A - S) / (g + 1),
-        F = Ac((A - S) / w / x) * x,
-        h, Y, V, te;
-    if (F < 1e-14 && !_ && !C) return [{
-        value: S
+        w = !Ie(s),
+        k = !Ie(a),
+        P = !Ie(c),
+        z = (A - C) / (g + 1),
+        F = Lc((A - C) / _ / x) * x,
+        h, $, Y, ne;
+    if (F < 1e-14 && !w && !k) return [{
+        value: C
     }, {
         value: A
     }];
-    te = Math.ceil(A / F) - Math.floor(S / F), te > w && (F = Ac(te * F / w / x) * x), Ie(l) || (h = Math.pow(10, l), F = Math.ceil(F * h) / h), r === "ticks" ? (Y = Math.floor(S / F) * F, V = Math.ceil(A / F) * F) : (Y = S, V = A), _ && C && o && Pp((a - s) / o, F / 1e3) ? (te = Math.round(Math.min((a - s) / F, d)), F = (a - s) / te, Y = s, V = a) : M ? (Y = _ ? s : Y, V = C ? a : V, te = c - 1, F = (V - Y) / te) : (te = (V - Y) / F, Oo(te, Math.round(te), F / 1e3) ? te = Math.round(te) : te = Math.ceil(te));
-    let ie = Math.max(Rc(F), Rc(Y));
-    h = Math.pow(10, Ie(l) ? ie : l), Y = Math.round(Y * h) / h, V = Math.round(V * h) / h;
+    ne = Math.ceil(A / F) - Math.floor(C / F), ne > _ && (F = Lc(ne * F / _ / x) * x), Ie(l) || (h = Math.pow(10, l), F = Math.ceil(F * h) / h), r === "ticks" ? ($ = Math.floor(C / F) * F, Y = Math.ceil(A / F) * F) : ($ = C, Y = A), w && k && o && Tp((a - s) / o, F / 1e3) ? (ne = Math.round(Math.min((a - s) / F, d)), F = (a - s) / ne, $ = s, Y = a) : P ? ($ = w ? s : $, Y = k ? a : Y, ne = c - 1, F = (Y - $) / ne) : (ne = (Y - $) / F, Oo(ne, Math.round(ne), F / 1e3) ? ne = Math.round(ne) : ne = Math.ceil(ne));
+    let ie = Math.max(Ic(F), Ic($));
+    h = Math.pow(10, Ie(l) ? ie : l), $ = Math.round($ * h) / h, Y = Math.round(Y * h) / h;
     let ce = 0;
-    for (_ && (y && Y !== s ? (n.push({
+    for (w && (y && $ !== s ? (n.push({
             value: s
-        }), Y < s && ce++, Oo(Math.round((Y + ce * F) * h) / h, s, Mb(s, z, t)) && ce++) : Y < s && ce++); ce < te; ++ce) {
-        let he = Math.round((Y + ce * F) * h) / h;
-        if (C && he > a) break;
+        }), $ < s && ce++, Oo(Math.round(($ + ce * F) * h) / h, s, Pb(s, z, t)) && ce++) : $ < s && ce++); ce < ne; ++ce) {
+        let he = Math.round(($ + ce * F) * h) / h;
+        if (k && he > a) break;
         n.push({
             value: he
         })
     }
-    return C && y && V !== a ? n.length && Oo(n[n.length - 1].value, a, Mb(a, z, t)) ? n[n.length - 1].value = a : n.push({
+    return k && y && Y !== a ? n.length && Oo(n[n.length - 1].value, a, Pb(a, z, t)) ? n[n.length - 1].value = a : n.push({
         value: a
-    }) : (!C || V === a) && n.push({
-        value: V
+    }) : (!k || Y === a) && n.push({
+        value: Y
     }), n
 }
 
-function Mb(t, e, {
+function Pb(t, e, {
     horizontal: n,
     minRotation: i
 }) {
     let r = pt(i),
         o = (n ? Math.sin(r) : Math.cos(r)) || .001,
         s = .75 * e * ("" + t).length;
     return Math.min(e / o, s)
@@ -17724,15 +17724,15 @@
                     maxDigits: this._maxDigits(),
                     horizontal: this.isHorizontal(),
                     minRotation: n.minRotation || 0,
                     includeBounds: n.includeBounds !== !1
                 },
                 o = this._range || this,
                 s = p2(r, o);
-            return e.bounds === "ticks" && Lc(s, this, "value"), e.reverse ? (s.reverse(), this.start = this.max, this.end = this.min) : (this.start = this.min, this.end = this.max), s
+            return e.bounds === "ticks" && Rc(s, this, "value"), e.reverse ? (s.reverse(), this.start = this.max, this.end = this.min) : (this.start = this.min, this.end = this.max), s
         }
         configure() {
             let e = this.ticks,
                 n = this.min,
                 i = this.max;
             if (super.configure(), this.options.offset && e.length) {
                 let r = (i - n) / Math.max(e.length - 1, 1) / 2;
@@ -17740,19 +17740,19 @@
             }
             this._startValue = n, this._endValue = i, this._valueRange = i - n
         }
         getLabelForValue(e) {
             return Ro(e, this.chart.options.locale, this.options.ticks.format)
         }
     },
-    Cg = class extends js {
+    kg = class extends js {
         static id = "linear";
         static defaults = {
             ticks: {
-                callback: gl.formatters.numeric
+                callback: ml.formatters.numeric
             }
         };
         determineDataLimits() {
             let {
                 min: e,
                 max: n
             } = this.getMinMax(!0);
@@ -17769,67 +17769,67 @@
         getPixelForValue(e) {
             return e === null ? NaN : this.getPixelForDecimal((e - this._startValue) / this._valueRange)
         }
         getValueForPixel(e) {
             return this._startValue + this.getDecimalForPixel(e) * this._valueRange
         }
     },
-    Ol = t => Math.floor(Si(t)),
-    zo = (t, e) => Math.pow(10, Ol(t) + e);
+    Al = t => Math.floor(ki(t)),
+    zo = (t, e) => Math.pow(10, Al(t) + e);
 
-function Db(t) {
-    return t / Math.pow(10, Ol(t)) === 1
+function Mb(t) {
+    return t / Math.pow(10, Al(t)) === 1
 }
 
 function Ob(t, e, n) {
     let i = Math.pow(10, n),
         r = Math.floor(t / i);
     return Math.ceil(e / i) - r
 }
 
 function g2(t, e) {
     let n = e - t,
-        i = Ol(n);
+        i = Al(n);
     for (; Ob(t, e, i) > 10;) i++;
     for (; Ob(t, e, i) < 10;) i--;
-    return Math.min(i, Ol(t))
+    return Math.min(i, Al(t))
 }
 
 function m2(t, {
     min: e,
     max: n
 }) {
     e = an(t.min, e);
     let i = [],
-        r = Ol(e),
+        r = Al(e),
         o = g2(e, n),
         s = o < 0 ? Math.pow(10, Math.abs(o)) : 1,
         a = Math.pow(10, o),
         l = r > o ? Math.pow(10, r) : 0,
         c = Math.round((e - l) * s) / s,
         d = Math.floor((e - l) / a / 10) * a * 10,
         g = Math.floor((c - d) / Math.pow(10, o)),
         y = an(t.min, Math.round((l + d + g * Math.pow(10, o)) * s) / s);
     for (; y < n;) i.push({
         value: y,
-        major: Db(y),
+        major: Mb(y),
         significand: g
     }), g >= 10 ? g = g < 15 ? 15 : 20 : g++, g >= 20 && (o++, g = 2, s = o >= 0 ? 1 : s), y = Math.round((l + d + g * Math.pow(10, o)) * s) / s;
     let x = an(t.max, y);
     return i.push({
         value: x,
-        major: Db(x),
+        major: Mb(x),
         significand: g
     }), i
 }
-var Eg = class extends Fo {
+var Cg = class extends Fo {
     static id = "logarithmic";
     static defaults = {
         ticks: {
-            callback: gl.formatters.logarithmic,
+            callback: ml.formatters.logarithmic,
             major: {
                 enabled: !0
             }
         }
     };
     constructor(e) {
         super(e), this.start = void 0, this.end = void 0, this._startValue = void 0, this._valueRange = 0
@@ -17859,44 +17859,44 @@
     buildTicks() {
         let e = this.options,
             n = {
                 min: this._userMin,
                 max: this._userMax
             },
             i = m2(n, this);
-        return e.bounds === "ticks" && Lc(i, this, "value"), e.reverse ? (i.reverse(), this.start = this.max, this.end = this.min) : (this.start = this.min, this.end = this.max), i
+        return e.bounds === "ticks" && Rc(i, this, "value"), e.reverse ? (i.reverse(), this.start = this.max, this.end = this.min) : (this.start = this.min, this.end = this.max), i
     }
     getLabelForValue(e) {
         return e === void 0 ? "0" : Ro(e, this.chart.options.locale, this.options.ticks.format)
     }
     configure() {
         let e = this.min;
-        super.configure(), this._startValue = Si(e), this._valueRange = Si(this.max) - Si(e)
+        super.configure(), this._startValue = ki(e), this._valueRange = ki(this.max) - ki(e)
     }
     getPixelForValue(e) {
-        return (e === void 0 || e === 0) && (e = this.min), e === null || isNaN(e) ? NaN : this.getPixelForDecimal(e === this.min ? 0 : (Si(e) - this._startValue) / this._valueRange)
+        return (e === void 0 || e === 0) && (e = this.min), e === null || isNaN(e) ? NaN : this.getPixelForDecimal(e === this.min ? 0 : (ki(e) - this._startValue) / this._valueRange)
     }
     getValueForPixel(e) {
         let n = this.getDecimalForPixel(e);
         return Math.pow(10, this._startValue + n * this._valueRange)
     }
 };
 
-function Tg(t) {
+function Eg(t) {
     let e = t.ticks;
     if (e.display && t.display) {
         let n = gt(e.backdropPadding);
         return pe(e.font && e.font.size, rt.font.size) + n.height
     }
     return 0
 }
 
 function y2(t, e, n) {
     return n = Re(n) ? n : [n], {
-        w: Ip(t, e.string, n),
+        w: Rp(t, e.string, n),
         h: n.length * e.lineHeight
     }
 }
 
 function Ab(t, e, n, i, r) {
     return t === i || t === r ? {
         start: e - n / 2,
@@ -17927,18 +17927,18 @@
         let c = s.setContext(t.getPointLabelContext(l));
         r[l] = c.padding;
         let d = t.getPointPosition(l, t.drawingArea + r[l], a),
             g = tt(c.font),
             y = y2(t.ctx, g, t._pointLabels[l]);
         i[l] = y;
         let x = on(t.getIndexAngle(l) + a),
-            w = Math.round(Ao(x)),
-            S = Ab(w, d.x, y.w, 0, 180),
-            A = Ab(w, d.y, y.h, 90, 270);
-        x2(n, e, x, S, A)
+            _ = Math.round(Ao(x)),
+            C = Ab(_, d.x, y.w, 0, 180),
+            A = Ab(_, d.y, y.h, 90, 270);
+        x2(n, e, x, C, A)
     }
     t.setCenterPoint(e.l - n.l, n.r - e.r, e.t - n.t, n.b - e.b), t._pointLabelItems = w2(t, i, r)
 }
 
 function x2(t, e, n, i, r) {
     let o = Math.abs(Math.sin(n)),
         s = Math.abs(Math.cos(n)),
@@ -17954,16 +17954,16 @@
             additionalAngle: o,
             padding: s,
             size: a
         } = n,
         l = t.getPointPosition(e, i + r + s, o),
         c = Math.round(Ao(on(l.angle + $e))),
         d = C2(l.y, a.h, c),
-        g = k2(c),
-        y = S2(l.x, a.w, g);
+        g = S2(c),
+        y = k2(l.x, a.w, g);
     return {
         visible: !0,
         x: l.x,
         y: d,
         textAlign: g,
         left: y,
         top: d,
@@ -18000,31 +18000,31 @@
         r = t._pointLabels.length,
         o = t.options,
         {
             centerPointLabels: s,
             display: a
         } = o.pointLabels,
         l = {
-            extra: Tg(o) / 2,
+            extra: Eg(o) / 2,
             additionalAngle: s ? Ce / r : 0
         },
         c;
     for (let d = 0; d < r; d++) {
         l.padding = n[d], l.size = e[d];
         let g = b2(t, d, l);
         i.push(g), a === "auto" && (g.visible = _2(g, c), g.visible && (c = g))
     }
     return i
 }
 
-function k2(t) {
+function S2(t) {
     return t === 0 || t === 180 ? "center" : t < 180 ? "left" : "right"
 }
 
-function S2(t, e, n) {
+function k2(t, e, n) {
     return n === "right" ? t -= e : n === "center" && (t -= e / 2), t
 }
 
 function C2(t, e, n) {
     return n === 90 || n === 270 ? t -= e / 2 : (n > 270 || n < 90) && (t -= e), t
 }
 
@@ -18041,15 +18041,15 @@
         let l = pi(e.borderRadius),
             c = gt(e.backdropPadding);
         t.fillStyle = a;
         let d = i - c.left,
             g = r - c.top,
             y = o - i + c.width,
             x = s - r + c.height;
-        Object.values(l).some(w => w !== 0) ? (t.beginPath(), rr(t, {
+        Object.values(l).some(_ => _ !== 0) ? (t.beginPath(), rr(t, {
             x: d,
             y: g,
             w: y,
             h: x,
             radius: l
         }), t.fill()) : t.fillRect(d, g, y, x)
     }
@@ -18089,32 +18089,32 @@
     else {
         let o = t.getPointPosition(0, e);
         r.moveTo(o.x, o.y);
         for (let s = 1; s < i; s++) o = t.getPointPosition(s, e), r.lineTo(o.x, o.y)
     }
 }
 
-function P2(t, e, n, i, r) {
+function D2(t, e, n, i, r) {
     let o = t.ctx,
         s = e.circular,
         {
             color: a,
             lineWidth: l
         } = e;
     !s && !i || !a || !l || n < 0 || (o.save(), o.strokeStyle = a, o.lineWidth = l, o.setLineDash(r.dash), o.lineDashOffset = r.dashOffset, o.beginPath(), i1(t, n, s, i), o.closePath(), o.stroke(), o.restore())
 }
 
-function M2(t, e, n) {
+function P2(t, e, n) {
     return Ei(t, {
         label: n,
         index: e,
         type: "pointLabel"
     })
 }
-var Pg = class extends js {
+var Tg = class extends js {
         static id = "radialLinear";
         static defaults = {
             display: !0,
             animate: !0,
             position: "chartArea",
             angleLines: {
                 display: !0,
@@ -18124,15 +18124,15 @@
             },
             grid: {
                 circular: !1
             },
             startAngle: 0,
             ticks: {
                 showLabelBackdrop: !0,
-                callback: gl.formatters.numeric
+                callback: ml.formatters.numeric
             },
             pointLabels: {
                 backdropColor: void 0,
                 backdropPadding: 2,
                 display: !0,
                 font: {
                     size: 10
@@ -18154,28 +18154,28 @@
                 _fallback: "grid"
             }
         };
         constructor(e) {
             super(e), this.xCenter = void 0, this.yCenter = void 0, this.drawingArea = void 0, this._pointLabels = [], this._pointLabelItems = []
         }
         setDimensions() {
-            let e = this._padding = gt(Tg(this.options) / 2),
+            let e = this._padding = gt(Eg(this.options) / 2),
                 n = this.width = this.maxWidth - e.width,
                 i = this.height = this.maxHeight - e.height;
             this.xCenter = Math.floor(this.left + n / 2 + e.left), this.yCenter = Math.floor(this.top + i / 2 + e.top), this.drawingArea = Math.floor(Math.min(n, i) / 2)
         }
         determineDataLimits() {
             let {
                 min: e,
                 max: n
             } = this.getMinMax(!1);
             this.min = qe(e) && !isNaN(e) ? e : 0, this.max = qe(n) && !isNaN(n) ? n : 0, this.handleTickRangeOptions()
         }
         computeTickLimit() {
-            return Math.ceil(this.drawingArea / Tg(this.options))
+            return Math.ceil(this.drawingArea / Eg(this.options))
         }
         generateTickLabels(e) {
             js.prototype.generateTickLabels.call(this, e), this._pointLabels = this.getLabels().map((n, i) => {
                 let r = ve(this.options.pointLabels.callback, [n, i], this);
                 return r || r === 0 ? r : ""
             }).filter((n, i) => this.chart.getDataVisibility(i))
         }
@@ -18201,15 +18201,15 @@
             let n = e / (this.drawingArea / (this.max - this.min));
             return this.options.reverse ? this.max - n : this.min + n
         }
         getPointLabelContext(e) {
             let n = this._pointLabels || [];
             if (e >= 0 && e < n.length) {
                 let i = n[e];
-                return M2(this.getContext(), e, i)
+                return P2(this.getContext(), e, i)
             }
         }
         getPointPosition(e, n, i = 0) {
             let r = this.getIndexAngle(e) - $e + i;
             return {
                 x: Math.cos(r) * n + this.xCenter,
                 y: Math.sin(r) * n + this.yCenter,
@@ -18259,16 +18259,16 @@
                 s = this._pointLabels.length,
                 a, l, c;
             if (n.pointLabels.display && T2(this, s), r.display && this.ticks.forEach((d, g) => {
                     if (g !== 0 || g === 0 && this.min < 0) {
                         l = this.getDistanceFromCenterForValue(d.value);
                         let y = this.getContext(g),
                             x = r.setContext(y),
-                            w = o.setContext(y);
-                        P2(this, x, l, s, w)
+                            _ = o.setContext(y);
+                        D2(this, x, l, s, _)
                     }
                 }), i.display) {
                 for (e.save(), a = s - 1; a >= 0; a--) {
                     let d = i.setContext(this.getPointLabelContext(a)),
                         {
                             color: g,
                             lineWidth: y
@@ -18300,15 +18300,15 @@
                     strokeColor: c.textStrokeColor,
                     strokeWidth: c.textStrokeWidth
                 })
             }), e.restore()
         }
         drawTitle() {}
     },
-    bf = {
+    _f = {
         millisecond: {
             common: !0,
             size: 1,
             steps: 1e3
         },
         second: {
             common: !0,
@@ -18346,15 +18346,15 @@
             steps: 4
         },
         year: {
             common: !0,
             size: 3154e7
         }
     },
-    wn = Object.keys(bf);
+    wn = Object.keys(_f);
 
 function Lb(t, e) {
     return t - e
 }
 
 function Rb(t, e) {
     if (Ie(e)) return null;
@@ -18367,41 +18367,41 @@
         s = e;
     return typeof i == "function" && (s = i(s)), qe(s) || (s = typeof i == "string" ? n.parse(s, i) : n.parse(s)), s === null ? null : (r && (s = r === "week" && (di(o) || o === !0) ? n.startOf(s, "isoWeek", o) : n.startOf(s, r)), +s)
 }
 
 function Ib(t, e, n, i) {
     let r = wn.length;
     for (let o = wn.indexOf(t); o < r - 1; ++o) {
-        let s = bf[wn[o]],
+        let s = _f[wn[o]],
             a = s.steps ? s.steps : Number.MAX_SAFE_INTEGER;
         if (s.common && Math.ceil((n - e) / (a * s.size)) <= i) return wn[o]
     }
     return wn[r - 1]
 }
 
-function D2(t, e, n, i, r) {
+function M2(t, e, n, i, r) {
     for (let o = wn.length - 1; o >= wn.indexOf(n); o--) {
         let s = wn[o];
-        if (bf[s].common && t._adapter.diff(r, i, s) >= e - 1) return s
+        if (_f[s].common && t._adapter.diff(r, i, s) >= e - 1) return s
     }
     return wn[n ? wn.indexOf(n) : 0]
 }
 
 function O2(t) {
     for (let e = wn.indexOf(t) + 1, n = wn.length; e < n; ++e)
-        if (bf[wn[e]].common) return wn[e]
+        if (_f[wn[e]].common) return wn[e]
 }
 
 function Nb(t, e, n) {
     if (!n) t[e] = !0;
     else if (n.length) {
         let {
             lo: i,
             hi: r
-        } = hl(n, e), o = n[i] >= e ? n[i] : n[r];
+        } = pl(n, e), o = n[i] >= e ? n[i] : n[r];
         t[o] = !0
     }
 }
 
 function A2(t, e, n, i) {
     let r = t._adapter,
         o = +r.startOf(e[0].value, i),
@@ -18418,15 +18418,15 @@
         s, a;
     for (s = 0; s < o; ++s) a = e[s], r[a] = s, i.push({
         value: a,
         major: !1
     });
     return o === 0 || !n ? i : A2(t, i, r, n)
 }
-var Al = class extends Fo {
+var Ll = class extends Fo {
     static id = "time";
     static defaults = {
         bounds: "data",
         adapters: {},
         time: {
             parser: !1,
             unit: !1,
@@ -18449,15 +18449,15 @@
             labels: [],
             all: []
         }, this._unit = "day", this._majorUnit = void 0, this._offsets = {}, this._normalized = !1, this._parseOpts = void 0
     }
     init(e, n = {}) {
         let i = e.time || (e.time = {}),
             r = this._adapter = new YC._date(e.adapters.date);
-        r.init(n), Do(i.displayFormats, r.formats()), this._parseOpts = {
+        r.init(n), Mo(i.displayFormats, r.formats()), this._parseOpts = {
             parser: i.parser,
             round: i.round,
             isoWeekday: i.isoWeekday
         }, super.init(e), this._normalized = n.normalized
     }
     parse(e, n) {
         return e === void 0 ? null : Rb(this, e)
@@ -18497,27 +18497,27 @@
         let e = this.options,
             n = e.time,
             i = e.ticks,
             r = i.source === "labels" ? this.getLabelTimestamps() : this._generate();
         e.bounds === "ticks" && r.length && (this.min = this._userMin || r[0], this.max = this._userMax || r[r.length - 1]);
         let o = this.min,
             s = this.max,
-            a = Op(r, o, s);
-        return this._unit = n.unit || (i.autoSkip ? Ib(n.minUnit, this.min, this.max, this._getLabelCapacity(o)) : D2(this, a.length, n.minUnit, this.min, this.max)), this._majorUnit = !i.major.enabled || this._unit === "year" ? void 0 : O2(this._unit), this.initOffsets(r), e.reverse && a.reverse(), zb(this, a, this._majorUnit)
+            a = Mp(r, o, s);
+        return this._unit = n.unit || (i.autoSkip ? Ib(n.minUnit, this.min, this.max, this._getLabelCapacity(o)) : M2(this, a.length, n.minUnit, this.min, this.max)), this._majorUnit = !i.major.enabled || this._unit === "year" ? void 0 : O2(this._unit), this.initOffsets(r), e.reverse && a.reverse(), zb(this, a, this._majorUnit)
     }
     afterAutoSkip() {
         this.options.offsetAfterAutoskip && this.initOffsets(this.ticks.map(e => +e.value))
     }
     initOffsets(e = []) {
         let n = 0,
             i = 0,
             r, o;
         this.options.offset && e.length && (r = this.getDecimalForValue(e[0]), e.length === 1 ? n = 1 - r : n = (this.getDecimalForValue(e[1]) - r) / 2, o = this.getDecimalForValue(e[e.length - 1]), e.length === 1 ? i = o : i = (o - this.getDecimalForValue(e[e.length - 2])) / 2);
         let s = e.length < 3 ? .5 : .25;
-        n = St(n, 0, s), i = St(i, 0, s), this._offsets = {
+        n = kt(n, 0, s), i = kt(i, 0, s), this._offsets = {
             start: n,
             end: i,
             factor: 1 / (n + 1 + i)
         }
     }
     _generate() {
         let e = this._adapter,
@@ -18529,17 +18529,17 @@
             a = pe(r.ticks.stepSize, 1),
             l = s === "week" ? o.isoWeekday : !1,
             c = di(l) || l === !0,
             d = {},
             g = n,
             y, x;
         if (c && (g = +e.startOf(g, "isoWeek", l)), g = +e.startOf(g, c ? "day" : s), e.diff(i, n, s) > 1e5 * a) throw new Error(n + " and " + i + " are too far apart with stepSize of " + a + " " + s);
-        let w = r.ticks.source === "data" && this.getDataTimestamps();
-        for (y = g, x = 0; y < i; y = +e.add(y, a, s), x++) Nb(d, y, w);
-        return (y === i || r.bounds === "ticks" || x === 1) && Nb(d, y, w), Object.keys(d).sort(Lb).map(S => +S)
+        let _ = r.ticks.source === "data" && this.getDataTimestamps();
+        for (y = g, x = 0; y < i; y = +e.add(y, a, s), x++) Nb(d, y, _);
+        return (y === i || r.bounds === "ticks" || x === 1) && Nb(d, y, _), Object.keys(d).sort(Lb).map(C => +C)
     }
     getLabelForValue(e) {
         let n = this._adapter,
             i = this.options.time;
         return i.tooltipFormat ? n.format(e, i.tooltipFormat) : n.format(e, i.displayFormats.datetime)
     }
     format(e, n) {
@@ -18613,19 +18613,19 @@
             n, i;
         if (e.length) return e;
         let r = this.getLabels();
         for (n = 0, i = r.length; n < i; ++n) e.push(Rb(this, r[n]));
         return this._cache.labels = this._normalized ? e : this.normalize(e)
     }
     normalize(e) {
-        return zc(e.sort(Lb))
+        return Fc(e.sort(Lb))
     }
 };
 
-function cf(t, e, n) {
+function ff(t, e, n) {
     let i = 0,
         r = t.length - 1,
         o, s, a, l;
     n ? (e >= t[i].pos && e <= t[r].pos && ({
         lo: i,
         hi: r
     } = ui(t, "pos", e)), {
@@ -18643,24 +18643,24 @@
     } = t[i], {
         time: s,
         pos: l
     } = t[r]);
     let c = s - o;
     return c ? a + (l - a) * (e - o) / c : a
 }
-var Mg = class extends Al {
+var Dg = class extends Ll {
         static id = "timeseries";
-        static defaults = Al.defaults;
+        static defaults = Ll.defaults;
         constructor(e) {
             super(e), this._table = [], this._minPos = void 0, this._tableRange = void 0
         }
         initOffsets() {
             let e = this._getTimestampsForTable(),
                 n = this._table = this.buildLookupTable(e);
-            this._minPos = cf(n, this.min), this._tableRange = cf(n, this.max) - this._minPos, super.initOffsets(e)
+            this._minPos = ff(n, this.min), this._tableRange = ff(n, this.max) - this._minPos, super.initOffsets(e)
         }
         buildLookupTable(e) {
             let {
                 min: n,
                 max: i
             } = this, r = [], o = [], s, a, l, c, d;
             for (s = 0, a = e.length; s < a; ++s) c = e[s], c >= n && c <= i && r.push(c);
@@ -18687,47 +18687,47 @@
             let e = this._cache.all || [];
             if (e.length) return e;
             let n = this.getDataTimestamps(),
                 i = this.getLabelTimestamps();
             return n.length && i.length ? e = this.normalize(n.concat(i)) : e = n.length ? n : i, e = this._cache.all = e, e
         }
         getDecimalForValue(e) {
-            return (cf(this._table, e) - this._minPos) / this._tableRange
+            return (ff(this._table, e) - this._minPos) / this._tableRange
         }
         getValueForPixel(e) {
             let n = this._offsets,
                 i = this.getDecimalForPixel(e) / n.factor - n.end;
-            return cf(this._table, i * this._tableRange + this._minPos, !0)
+            return ff(this._table, i * this._tableRange + this._minPos, !0)
         }
     },
     L2 = Object.freeze({
         __proto__: null,
         CategoryScale: Sg,
-        LinearScale: Cg,
-        LogarithmicScale: Eg,
-        RadialLinearScale: Pg,
-        TimeScale: Al,
-        TimeSeriesScale: Mg
+        LinearScale: kg,
+        LogarithmicScale: Cg,
+        RadialLinearScale: Tg,
+        TimeScale: Ll,
+        TimeSeriesScale: Dg
     }),
     r1 = [$C, mT, c2, L2];
 var R2 = typeof globalThis < "u" ? globalThis : typeof window < "u" ? window : typeof global < "u" ? global : typeof self < "u" ? self : {};
 
 function l1(t) {
     return t && t.__esModule && Object.prototype.hasOwnProperty.call(t, "default") ? t.default : t
 }
 var u1 = {
         exports: {}
     },
-    Rl = {};
+    Il = {};
 var o1;
 
 function I2() {
-    if (o1) return Rl;
+    if (o1) return Il;
     o1 = 1;
-    var t = wf.default,
+    var t = Bs.default,
         e = Symbol.for("react.element"),
         n = Symbol.for("react.fragment"),
         i = Object.prototype.hasOwnProperty,
         r = t.__SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED.ReactCurrentOwner,
         o = {
             key: !0,
             ref: !0,
@@ -18748,15 +18748,15 @@
             type: a,
             key: y,
             ref: x,
             props: g,
             _owner: r.current
         }
     }
-    return Rl.Fragment = n, Rl.jsx = s, Rl.jsxs = s, Rl
+    return Il.Fragment = n, Il.jsx = s, Il.jsxs = s, Il
 }
 u1.exports = I2();
 var bt = u1.exports,
     c1 = {
         exports: {}
     };
 (function(t) {
@@ -18765,19 +18765,19 @@
             i = /\s+$/,
             r = 0,
             o = e.round,
             s = e.min,
             a = e.max,
             l = e.random;
 
-        function c(D, H) {
-            if (D = D || "", H = H || {}, D instanceof c) return D;
-            if (!(this instanceof c)) return new c(D, H);
-            var O = d(D);
-            this._originalInput = D, this._r = O.r, this._g = O.g, this._b = O.b, this._a = O.a, this._roundA = o(100 * this._a) / 100, this._format = H.format || O.format, this._gradientType = H.gradientType, this._r < 1 && (this._r = o(this._r)), this._g < 1 && (this._g = o(this._g)), this._b < 1 && (this._b = o(this._b)), this._ok = O.ok, this._tc_id = r++
+        function c(M, H) {
+            if (M = M || "", H = H || {}, M instanceof c) return M;
+            if (!(this instanceof c)) return new c(M, H);
+            var O = d(M);
+            this._originalInput = M, this._r = O.r, this._g = O.g, this._b = O.b, this._a = O.a, this._roundA = o(100 * this._a) / 100, this._format = H.format || O.format, this._gradientType = H.gradientType, this._r < 1 && (this._r = o(this._r)), this._g < 1 && (this._g = o(this._g)), this._b < 1 && (this._b = o(this._b)), this._ok = O.ok, this._tc_id = r++
         }
         c.prototype = {
             isDark: function() {
                 return this.getBrightness() < 128
             },
             isLight: function() {
                 return !this.isDark()
@@ -18791,68 +18791,68 @@
             getFormat: function() {
                 return this._format
             },
             getAlpha: function() {
                 return this._a
             },
             getBrightness: function() {
-                var D = this.toRgb();
-                return (D.r * 299 + D.g * 587 + D.b * 114) / 1e3
+                var M = this.toRgb();
+                return (M.r * 299 + M.g * 587 + M.b * 114) / 1e3
             },
             getLuminance: function() {
-                var D = this.toRgb(),
-                    H, O, X, re, le, Pe;
-                return H = D.r / 255, O = D.g / 255, X = D.b / 255, H <= .03928 ? re = H / 12.92 : re = e.pow((H + .055) / 1.055, 2.4), O <= .03928 ? le = O / 12.92 : le = e.pow((O + .055) / 1.055, 2.4), X <= .03928 ? Pe = X / 12.92 : Pe = e.pow((X + .055) / 1.055, 2.4), .2126 * re + .7152 * le + .0722 * Pe
+                var M = this.toRgb(),
+                    H, O, X, re, le, De;
+                return H = M.r / 255, O = M.g / 255, X = M.b / 255, H <= .03928 ? re = H / 12.92 : re = e.pow((H + .055) / 1.055, 2.4), O <= .03928 ? le = O / 12.92 : le = e.pow((O + .055) / 1.055, 2.4), X <= .03928 ? De = X / 12.92 : De = e.pow((X + .055) / 1.055, 2.4), .2126 * re + .7152 * le + .0722 * De
             },
-            setAlpha: function(D) {
-                return this._a = lt(D), this._roundA = o(100 * this._a) / 100, this
+            setAlpha: function(M) {
+                return this._a = lt(M), this._roundA = o(100 * this._a) / 100, this
             },
             toHsv: function() {
-                var D = w(this._r, this._g, this._b);
+                var M = _(this._r, this._g, this._b);
                 return {
-                    h: D.h * 360,
-                    s: D.s,
-                    v: D.v,
+                    h: M.h * 360,
+                    s: M.s,
+                    v: M.v,
                     a: this._a
                 }
             },
             toHsvString: function() {
-                var D = w(this._r, this._g, this._b),
-                    H = o(D.h * 360),
-                    O = o(D.s * 100),
-                    X = o(D.v * 100);
+                var M = _(this._r, this._g, this._b),
+                    H = o(M.h * 360),
+                    O = o(M.s * 100),
+                    X = o(M.v * 100);
                 return this._a == 1 ? "hsv(" + H + ", " + O + "%, " + X + "%)" : "hsva(" + H + ", " + O + "%, " + X + "%, " + this._roundA + ")"
             },
             toHsl: function() {
-                var D = y(this._r, this._g, this._b);
+                var M = y(this._r, this._g, this._b);
                 return {
-                    h: D.h * 360,
-                    s: D.s,
-                    l: D.l,
+                    h: M.h * 360,
+                    s: M.s,
+                    l: M.l,
                     a: this._a
                 }
             },
             toHslString: function() {
-                var D = y(this._r, this._g, this._b),
-                    H = o(D.h * 360),
-                    O = o(D.s * 100),
-                    X = o(D.l * 100);
+                var M = y(this._r, this._g, this._b),
+                    H = o(M.h * 360),
+                    O = o(M.s * 100),
+                    X = o(M.l * 100);
                 return this._a == 1 ? "hsl(" + H + ", " + O + "%, " + X + "%)" : "hsla(" + H + ", " + O + "%, " + X + "%, " + this._roundA + ")"
             },
-            toHex: function(D) {
-                return A(this._r, this._g, this._b, D)
+            toHex: function(M) {
+                return A(this._r, this._g, this._b, M)
             },
-            toHexString: function(D) {
-                return "#" + this.toHex(D)
+            toHexString: function(M) {
+                return "#" + this.toHex(M)
             },
-            toHex8: function(D) {
-                return _(this._r, this._g, this._b, this._a, D)
+            toHex8: function(M) {
+                return w(this._r, this._g, this._b, this._a, M)
             },
-            toHex8String: function(D) {
-                return "#" + this.toHex8(D)
+            toHex8String: function(M) {
+                return "#" + this.toHex8(M)
             },
             toRgb: function() {
                 return {
                     r: o(this._r),
                     g: o(this._g),
                     b: o(this._b),
                     a: this._a
@@ -18871,62 +18871,62 @@
             },
             toPercentageRgbString: function() {
                 return this._a == 1 ? "rgb(" + o(Oe(this._r, 255) * 100) + "%, " + o(Oe(this._g, 255) * 100) + "%, " + o(Oe(this._b, 255) * 100) + "%)" : "rgba(" + o(Oe(this._r, 255) * 100) + "%, " + o(Oe(this._g, 255) * 100) + "%, " + o(Oe(this._b, 255) * 100) + "%, " + this._roundA + ")"
             },
             toName: function() {
                 return this._a === 0 ? "transparent" : this._a < 1 ? !1 : Ye[A(this._r, this._g, this._b, !0)] || !1
             },
-            toFilter: function(D) {
-                var H = "#" + C(this._r, this._g, this._b, this._a),
+            toFilter: function(M) {
+                var H = "#" + k(this._r, this._g, this._b, this._a),
                     O = H,
                     X = this._gradientType ? "GradientType = 1, " : "";
-                if (D) {
-                    var re = c(D);
-                    O = "#" + C(re._r, re._g, re._b, re._a)
+                if (M) {
+                    var re = c(M);
+                    O = "#" + k(re._r, re._g, re._b, re._a)
                 }
                 return "progid:DXImageTransform.Microsoft.gradient(" + X + "startColorstr=" + H + ",endColorstr=" + O + ")"
             },
-            toString: function(D) {
-                var H = !!D;
-                D = D || this._format;
+            toString: function(M) {
+                var H = !!M;
+                M = M || this._format;
                 var O = !1,
                     X = this._a < 1 && this._a >= 0,
-                    re = !H && X && (D === "hex" || D === "hex6" || D === "hex3" || D === "hex4" || D === "hex8" || D === "name");
-                return re ? D === "name" && this._a === 0 ? this.toName() : this.toRgbString() : (D === "rgb" && (O = this.toRgbString()), D === "prgb" && (O = this.toPercentageRgbString()), (D === "hex" || D === "hex6") && (O = this.toHexString()), D === "hex3" && (O = this.toHexString(!0)), D === "hex4" && (O = this.toHex8String(!0)), D === "hex8" && (O = this.toHex8String()), D === "name" && (O = this.toName()), D === "hsl" && (O = this.toHslString()), D === "hsv" && (O = this.toHsvString()), O || this.toHexString())
+                    re = !H && X && (M === "hex" || M === "hex6" || M === "hex3" || M === "hex4" || M === "hex8" || M === "name");
+                return re ? M === "name" && this._a === 0 ? this.toName() : this.toRgbString() : (M === "rgb" && (O = this.toRgbString()), M === "prgb" && (O = this.toPercentageRgbString()), (M === "hex" || M === "hex6") && (O = this.toHexString()), M === "hex3" && (O = this.toHexString(!0)), M === "hex4" && (O = this.toHex8String(!0)), M === "hex8" && (O = this.toHex8String()), M === "name" && (O = this.toName()), M === "hsl" && (O = this.toHslString()), M === "hsv" && (O = this.toHsvString()), O || this.toHexString())
             },
             clone: function() {
                 return c(this.toString())
             },
-            _applyModification: function(D, H) {
-                var O = D.apply(null, [this].concat([].slice.call(H)));
+            _applyModification: function(M, H) {
+                var O = M.apply(null, [this].concat([].slice.call(H)));
                 return this._r = O._r, this._g = O._g, this._b = O._b, this.setAlpha(O._a), this
             },
             lighten: function() {
                 return this._applyModification(h, arguments)
             },
             brighten: function() {
-                return this._applyModification(Y, arguments)
+                return this._applyModification($, arguments)
             },
             darken: function() {
-                return this._applyModification(V, arguments)
+                return this._applyModification(Y, arguments)
             },
             desaturate: function() {
-                return this._applyModification(M, arguments)
+                return this._applyModification(P, arguments)
             },
             saturate: function() {
                 return this._applyModification(z, arguments)
             },
             greyscale: function() {
                 return this._applyModification(F, arguments)
             },
             spin: function() {
-                return this._applyModification(te, arguments)
+                return this._applyModification(ne, arguments)
             },
-            _applyCombination: function(D, H) {
-                return D.apply(null, [this].concat([].slice.call(H)))
+            _applyCombination: function(M, H) {
+                return M.apply(null, [this].concat([].slice.call(H)))
             },
             analogous: function() {
                 return this._applyCombination(Ze, arguments)
             },
             complement: function() {
                 return this._applyCombination(ie, arguments)
             },
@@ -18938,322 +18938,322 @@
             },
             triad: function() {
                 return this._applyCombination(ce, arguments)
             },
             tetrad: function() {
                 return this._applyCombination(he, arguments)
             }
-        }, c.fromRatio = function(D, H) {
-            if (typeof D == "object") {
+        }, c.fromRatio = function(M, H) {
+            if (typeof M == "object") {
                 var O = {};
-                for (var X in D) D.hasOwnProperty(X) && (X === "a" ? O[X] = D[X] : O[X] = je(D[X]));
-                D = O
+                for (var X in M) M.hasOwnProperty(X) && (X === "a" ? O[X] = M[X] : O[X] = je(M[X]));
+                M = O
             }
-            return c(D, H)
+            return c(M, H)
         };
 
-        function d(D) {
+        function d(M) {
             var H = {
                     r: 0,
                     g: 0,
                     b: 0
                 },
                 O = 1,
                 X = null,
                 re = null,
                 le = null,
-                Pe = !1,
-                Me = !1;
-            return typeof D == "string" && (D = Di(D)), typeof D == "object" && (Yt(D.r) && Yt(D.g) && Yt(D.b) ? (H = g(D.r, D.g, D.b), Pe = !0, Me = String(D.r).substr(-1) === "%" ? "prgb" : "rgb") : Yt(D.h) && Yt(D.s) && Yt(D.v) ? (X = je(D.s), re = je(D.v), H = S(D.h, X, re), Pe = !0, Me = "hsv") : Yt(D.h) && Yt(D.s) && Yt(D.l) && (X = je(D.s), le = je(D.l), H = x(D.h, X, le), Pe = !0, Me = "hsl"), D.hasOwnProperty("a") && (O = D.a)), O = lt(O), {
-                ok: Pe,
-                format: D.format || Me,
+                De = !1,
+                Pe = !1;
+            return typeof M == "string" && (M = Mi(M)), typeof M == "object" && (Yt(M.r) && Yt(M.g) && Yt(M.b) ? (H = g(M.r, M.g, M.b), De = !0, Pe = String(M.r).substr(-1) === "%" ? "prgb" : "rgb") : Yt(M.h) && Yt(M.s) && Yt(M.v) ? (X = je(M.s), re = je(M.v), H = C(M.h, X, re), De = !0, Pe = "hsv") : Yt(M.h) && Yt(M.s) && Yt(M.l) && (X = je(M.s), le = je(M.l), H = x(M.h, X, le), De = !0, Pe = "hsl"), M.hasOwnProperty("a") && (O = M.a)), O = lt(O), {
+                ok: De,
+                format: M.format || Pe,
                 r: s(255, a(H.r, 0)),
                 g: s(255, a(H.g, 0)),
                 b: s(255, a(H.b, 0)),
                 a: O
             }
         }
 
-        function g(D, H, O) {
+        function g(M, H, O) {
             return {
-                r: Oe(D, 255) * 255,
+                r: Oe(M, 255) * 255,
                 g: Oe(H, 255) * 255,
                 b: Oe(O, 255) * 255
             }
         }
 
-        function y(D, H, O) {
-            D = Oe(D, 255), H = Oe(H, 255), O = Oe(O, 255);
-            var X = a(D, H, O),
-                re = s(D, H, O),
-                le, Pe, Me = (X + re) / 2;
-            if (X == re) le = Pe = 0;
+        function y(M, H, O) {
+            M = Oe(M, 255), H = Oe(H, 255), O = Oe(O, 255);
+            var X = a(M, H, O),
+                re = s(M, H, O),
+                le, De, Pe = (X + re) / 2;
+            if (X == re) le = De = 0;
             else {
-                var Qe = X - re;
-                switch (Pe = Me > .5 ? Qe / (2 - X - re) : Qe / (X + re), X) {
-                    case D:
-                        le = (H - O) / Qe + (H < O ? 6 : 0);
+                var Ge = X - re;
+                switch (De = Pe > .5 ? Ge / (2 - X - re) : Ge / (X + re), X) {
+                    case M:
+                        le = (H - O) / Ge + (H < O ? 6 : 0);
                         break;
                     case H:
-                        le = (O - D) / Qe + 2;
+                        le = (O - M) / Ge + 2;
                         break;
                     case O:
-                        le = (D - H) / Qe + 4;
+                        le = (M - H) / Ge + 4;
                         break
                 }
                 le /= 6
             }
             return {
                 h: le,
-                s: Pe,
-                l: Me
+                s: De,
+                l: Pe
             }
         }
 
-        function x(D, H, O) {
+        function x(M, H, O) {
             var X, re, le;
-            D = Oe(D, 360), H = Oe(H, 100), O = Oe(O, 100);
+            M = Oe(M, 360), H = Oe(H, 100), O = Oe(O, 100);
 
-            function Pe(Ft, Sn, ut) {
-                return ut < 0 && (ut += 1), ut > 1 && (ut -= 1), ut < 1 / 6 ? Ft + (Sn - Ft) * 6 * ut : ut < 1 / 2 ? Sn : ut < 2 / 3 ? Ft + (Sn - Ft) * (2 / 3 - ut) * 6 : Ft
+            function De(Ft, kn, ut) {
+                return ut < 0 && (ut += 1), ut > 1 && (ut -= 1), ut < 1 / 6 ? Ft + (kn - Ft) * 6 * ut : ut < 1 / 2 ? kn : ut < 2 / 3 ? Ft + (kn - Ft) * (2 / 3 - ut) * 6 : Ft
             }
             if (H === 0) X = re = le = O;
             else {
-                var Me = O < .5 ? O * (1 + H) : O + H - O * H,
-                    Qe = 2 * O - Me;
-                X = Pe(Qe, Me, D + 1 / 3), re = Pe(Qe, Me, D), le = Pe(Qe, Me, D - 1 / 3)
+                var Pe = O < .5 ? O * (1 + H) : O + H - O * H,
+                    Ge = 2 * O - Pe;
+                X = De(Ge, Pe, M + 1 / 3), re = De(Ge, Pe, M), le = De(Ge, Pe, M - 1 / 3)
             }
             return {
                 r: X * 255,
                 g: re * 255,
                 b: le * 255
             }
         }
 
-        function w(D, H, O) {
-            D = Oe(D, 255), H = Oe(H, 255), O = Oe(O, 255);
-            var X = a(D, H, O),
-                re = s(D, H, O),
-                le, Pe, Me = X,
-                Qe = X - re;
-            if (Pe = X === 0 ? 0 : Qe / X, X == re) le = 0;
+        function _(M, H, O) {
+            M = Oe(M, 255), H = Oe(H, 255), O = Oe(O, 255);
+            var X = a(M, H, O),
+                re = s(M, H, O),
+                le, De, Pe = X,
+                Ge = X - re;
+            if (De = X === 0 ? 0 : Ge / X, X == re) le = 0;
             else {
                 switch (X) {
-                    case D:
-                        le = (H - O) / Qe + (H < O ? 6 : 0);
+                    case M:
+                        le = (H - O) / Ge + (H < O ? 6 : 0);
                         break;
                     case H:
-                        le = (O - D) / Qe + 2;
+                        le = (O - M) / Ge + 2;
                         break;
                     case O:
-                        le = (D - H) / Qe + 4;
+                        le = (M - H) / Ge + 4;
                         break
                 }
                 le /= 6
             }
             return {
                 h: le,
-                s: Pe,
-                v: Me
+                s: De,
+                v: Pe
             }
         }
 
-        function S(D, H, O) {
-            D = Oe(D, 360) * 6, H = Oe(H, 100), O = Oe(O, 100);
-            var X = e.floor(D),
-                re = D - X,
+        function C(M, H, O) {
+            M = Oe(M, 360) * 6, H = Oe(H, 100), O = Oe(O, 100);
+            var X = e.floor(M),
+                re = M - X,
                 le = O * (1 - H),
-                Pe = O * (1 - re * H),
-                Me = O * (1 - (1 - re) * H),
-                Qe = X % 6,
-                Ft = [O, Pe, le, le, Me, O][Qe],
-                Sn = [Me, O, O, Pe, le, le][Qe],
-                ut = [le, le, Me, O, O, Pe][Qe];
+                De = O * (1 - re * H),
+                Pe = O * (1 - (1 - re) * H),
+                Ge = X % 6,
+                Ft = [O, De, le, le, Pe, O][Ge],
+                kn = [Pe, O, O, De, le, le][Ge],
+                ut = [le, le, Pe, O, O, De][Ge];
             return {
                 r: Ft * 255,
-                g: Sn * 255,
+                g: kn * 255,
                 b: ut * 255
             }
         }
 
-        function A(D, H, O, X) {
-            var re = [mt(o(D).toString(16)), mt(o(H).toString(16)), mt(o(O).toString(16))];
+        function A(M, H, O, X) {
+            var re = [mt(o(M).toString(16)), mt(o(H).toString(16)), mt(o(O).toString(16))];
             return X && re[0].charAt(0) == re[0].charAt(1) && re[1].charAt(0) == re[1].charAt(1) && re[2].charAt(0) == re[2].charAt(1) ? re[0].charAt(0) + re[1].charAt(0) + re[2].charAt(0) : re.join("")
         }
 
-        function _(D, H, O, X, re) {
-            var le = [mt(o(D).toString(16)), mt(o(H).toString(16)), mt(o(O).toString(16)), mt(ln(X))];
+        function w(M, H, O, X, re) {
+            var le = [mt(o(M).toString(16)), mt(o(H).toString(16)), mt(o(O).toString(16)), mt(ln(X))];
             return re && le[0].charAt(0) == le[0].charAt(1) && le[1].charAt(0) == le[1].charAt(1) && le[2].charAt(0) == le[2].charAt(1) && le[3].charAt(0) == le[3].charAt(1) ? le[0].charAt(0) + le[1].charAt(0) + le[2].charAt(0) + le[3].charAt(0) : le.join("")
         }
 
-        function C(D, H, O, X) {
-            var re = [mt(ln(X)), mt(o(D).toString(16)), mt(o(H).toString(16)), mt(o(O).toString(16))];
+        function k(M, H, O, X) {
+            var re = [mt(ln(X)), mt(o(M).toString(16)), mt(o(H).toString(16)), mt(o(O).toString(16))];
             return re.join("")
         }
-        c.equals = function(D, H) {
-            return !D || !H ? !1 : c(D).toRgbString() == c(H).toRgbString()
+        c.equals = function(M, H) {
+            return !M || !H ? !1 : c(M).toRgbString() == c(H).toRgbString()
         }, c.random = function() {
             return c.fromRatio({
                 r: l(),
                 g: l(),
                 b: l()
             })
         };
 
-        function M(D, H) {
+        function P(M, H) {
             H = H === 0 ? 0 : H || 10;
-            var O = c(D).toHsl();
-            return O.s -= H / 100, O.s = Ge(O.s), c(O)
+            var O = c(M).toHsl();
+            return O.s -= H / 100, O.s = Ke(O.s), c(O)
         }
 
-        function z(D, H) {
+        function z(M, H) {
             H = H === 0 ? 0 : H || 10;
-            var O = c(D).toHsl();
-            return O.s += H / 100, O.s = Ge(O.s), c(O)
+            var O = c(M).toHsl();
+            return O.s += H / 100, O.s = Ke(O.s), c(O)
         }
 
-        function F(D) {
-            return c(D).desaturate(100)
+        function F(M) {
+            return c(M).desaturate(100)
         }
 
-        function h(D, H) {
+        function h(M, H) {
             H = H === 0 ? 0 : H || 10;
-            var O = c(D).toHsl();
-            return O.l += H / 100, O.l = Ge(O.l), c(O)
+            var O = c(M).toHsl();
+            return O.l += H / 100, O.l = Ke(O.l), c(O)
         }
 
-        function Y(D, H) {
+        function $(M, H) {
             H = H === 0 ? 0 : H || 10;
-            var O = c(D).toRgb();
+            var O = c(M).toRgb();
             return O.r = a(0, s(255, O.r - o(255 * -(H / 100)))), O.g = a(0, s(255, O.g - o(255 * -(H / 100)))), O.b = a(0, s(255, O.b - o(255 * -(H / 100)))), c(O)
         }
 
-        function V(D, H) {
+        function Y(M, H) {
             H = H === 0 ? 0 : H || 10;
-            var O = c(D).toHsl();
-            return O.l -= H / 100, O.l = Ge(O.l), c(O)
+            var O = c(M).toHsl();
+            return O.l -= H / 100, O.l = Ke(O.l), c(O)
         }
 
-        function te(D, H) {
-            var O = c(D).toHsl(),
+        function ne(M, H) {
+            var O = c(M).toHsl(),
                 X = (O.h + H) % 360;
             return O.h = X < 0 ? 360 + X : X, c(O)
         }
 
-        function ie(D) {
-            var H = c(D).toHsl();
+        function ie(M) {
+            var H = c(M).toHsl();
             return H.h = (H.h + 180) % 360, c(H)
         }
 
-        function ce(D) {
-            var H = c(D).toHsl(),
+        function ce(M) {
+            var H = c(M).toHsl(),
                 O = H.h;
-            return [c(D), c({
+            return [c(M), c({
                 h: (O + 120) % 360,
                 s: H.s,
                 l: H.l
             }), c({
                 h: (O + 240) % 360,
                 s: H.s,
                 l: H.l
             })]
         }
 
-        function he(D) {
-            var H = c(D).toHsl(),
+        function he(M) {
+            var H = c(M).toHsl(),
                 O = H.h;
-            return [c(D), c({
+            return [c(M), c({
                 h: (O + 90) % 360,
                 s: H.s,
                 l: H.l
             }), c({
                 h: (O + 180) % 360,
                 s: H.s,
                 l: H.l
             }), c({
                 h: (O + 270) % 360,
                 s: H.s,
                 l: H.l
             })]
         }
 
-        function Fe(D) {
-            var H = c(D).toHsl(),
+        function Fe(M) {
+            var H = c(M).toHsl(),
                 O = H.h;
-            return [c(D), c({
+            return [c(M), c({
                 h: (O + 72) % 360,
                 s: H.s,
                 l: H.l
             }), c({
                 h: (O + 216) % 360,
                 s: H.s,
                 l: H.l
             })]
         }
 
-        function Ze(D, H, O) {
+        function Ze(M, H, O) {
             H = H || 6, O = O || 30;
-            var X = c(D).toHsl(),
+            var X = c(M).toHsl(),
                 re = 360 / O,
-                le = [c(D)];
+                le = [c(M)];
             for (X.h = (X.h - (re * H >> 1) + 720) % 360; --H;) X.h = (X.h + re) % 360, le.push(c(X));
             return le
         }
 
-        function Ee(D, H) {
+        function Ee(M, H) {
             H = H || 6;
-            for (var O = c(D).toHsv(), X = O.h, re = O.s, le = O.v, Pe = [], Me = 1 / H; H--;) Pe.push(c({
+            for (var O = c(M).toHsv(), X = O.h, re = O.s, le = O.v, De = [], Pe = 1 / H; H--;) De.push(c({
                 h: X,
                 s: re,
                 v: le
-            })), le = (le + Me) % 1;
-            return Pe
+            })), le = (le + Pe) % 1;
+            return De
         }
-        c.mix = function(D, H, O) {
+        c.mix = function(M, H, O) {
             O = O === 0 ? 0 : O || 50;
-            var X = c(D).toRgb(),
+            var X = c(M).toRgb(),
                 re = c(H).toRgb(),
                 le = O / 100,
-                Pe = {
+                De = {
                     r: (re.r - X.r) * le + X.r,
                     g: (re.g - X.g) * le + X.g,
                     b: (re.b - X.b) * le + X.b,
                     a: (re.a - X.a) * le + X.a
                 };
-            return c(Pe)
-        }, c.readability = function(D, H) {
-            var O = c(D),
+            return c(De)
+        }, c.readability = function(M, H) {
+            var O = c(M),
                 X = c(H);
             return (e.max(O.getLuminance(), X.getLuminance()) + .05) / (e.min(O.getLuminance(), X.getLuminance()) + .05)
-        }, c.isReadable = function(D, H, O) {
-            var X = c.readability(D, H),
+        }, c.isReadable = function(M, H, O) {
+            var X = c.readability(M, H),
                 re, le;
             switch (le = !1, re = Oi(O), re.level + re.size) {
                 case "AAsmall":
                 case "AAAlarge":
                     le = X >= 4.5;
                     break;
                 case "AAlarge":
                     le = X >= 3;
                     break;
                 case "AAAsmall":
                     le = X >= 7;
                     break
             }
             return le
-        }, c.mostReadable = function(D, H, O) {
+        }, c.mostReadable = function(M, H, O) {
             var X = null,
                 re = 0,
-                le, Pe, Me, Qe;
-            O = O || {}, Pe = O.includeFallbackColors, Me = O.level, Qe = O.size;
-            for (var Ft = 0; Ft < H.length; Ft++) le = c.readability(D, H[Ft]), le > re && (re = le, X = c(H[Ft]));
-            return c.isReadable(D, X, {
-                level: Me,
-                size: Qe
-            }) || !Pe ? X : (O.includeFallbackColors = !1, c.mostReadable(D, ["#fff", "#000"], O))
+                le, De, Pe, Ge;
+            O = O || {}, De = O.includeFallbackColors, Pe = O.level, Ge = O.size;
+            for (var Ft = 0; Ft < H.length; Ft++) le = c.readability(M, H[Ft]), le > re && (re = le, X = c(H[Ft]));
+            return c.isReadable(M, X, {
+                level: Pe,
+                size: Ge
+            }) || !De ? X : (O.includeFallbackColors = !1, c.mostReadable(M, ["#fff", "#000"], O))
         };
         var Te = c.names = {
                 aliceblue: "f0f8ff",
                 antiquewhite: "faebd7",
                 aqua: "0ff",
                 aquamarine: "7fffd4",
                 azure: "f0ffff",
@@ -19400,65 +19400,65 @@
                 white: "fff",
                 whitesmoke: "f5f5f5",
                 yellow: "ff0",
                 yellowgreen: "9acd32"
             },
             Ye = c.hexNames = Ot(Te);
 
-        function Ot(D) {
+        function Ot(M) {
             var H = {};
-            for (var O in D) D.hasOwnProperty(O) && (H[D[O]] = O);
+            for (var O in M) M.hasOwnProperty(O) && (H[M[O]] = O);
             return H
         }
 
-        function lt(D) {
-            return D = parseFloat(D), (isNaN(D) || D < 0 || D > 1) && (D = 1), D
+        function lt(M) {
+            return M = parseFloat(M), (isNaN(M) || M < 0 || M > 1) && (M = 1), M
         }
 
-        function Oe(D, H) {
-            At(D) && (D = "100%");
-            var O = $t(D);
-            return D = s(H, a(0, parseFloat(D))), O && (D = parseInt(D * H, 10) / 100), e.abs(D - H) < 1e-6 ? 1 : D % H / parseFloat(H)
+        function Oe(M, H) {
+            At(M) && (M = "100%");
+            var O = $t(M);
+            return M = s(H, a(0, parseFloat(M))), O && (M = parseInt(M * H, 10) / 100), e.abs(M - H) < 1e-6 ? 1 : M % H / parseFloat(H)
         }
 
-        function Ge(D) {
-            return s(1, a(0, D))
+        function Ke(M) {
+            return s(1, a(0, M))
         }
 
-        function ot(D) {
-            return parseInt(D, 16)
+        function ot(M) {
+            return parseInt(M, 16)
         }
 
-        function At(D) {
-            return typeof D == "string" && D.indexOf(".") != -1 && parseFloat(D) === 1
+        function At(M) {
+            return typeof M == "string" && M.indexOf(".") != -1 && parseFloat(M) === 1
         }
 
-        function $t(D) {
-            return typeof D == "string" && D.indexOf("%") != -1
+        function $t(M) {
+            return typeof M == "string" && M.indexOf("%") != -1
         }
 
-        function mt(D) {
-            return D.length == 1 ? "0" + D : "" + D
+        function mt(M) {
+            return M.length == 1 ? "0" + M : "" + M
         }
 
-        function je(D) {
-            return D <= 1 && (D = D * 100 + "%"), D
+        function je(M) {
+            return M <= 1 && (M = M * 100 + "%"), M
         }
 
-        function ln(D) {
-            return e.round(parseFloat(D) * 255).toString(16)
+        function ln(M) {
+            return e.round(parseFloat(M) * 255).toString(16)
         }
 
-        function Ve(D) {
-            return ot(D) / 255
+        function Ve(M) {
+            return ot(M) / 255
         }
         var Ae = function() {
-            var D = "[-\\+]?\\d+%?",
+            var M = "[-\\+]?\\d+%?",
                 H = "[-\\+]?\\d*\\.\\d+%?",
-                O = "(?:" + H + ")|(?:" + D + ")",
+                O = "(?:" + H + ")|(?:" + M + ")",
                 X = "[\\s|\\(]+(" + O + ")[,|\\s]+(" + O + ")[,|\\s]+(" + O + ")\\s*\\)?",
                 re = "[\\s|\\(]+(" + O + ")[,|\\s]+(" + O + ")[,|\\s]+(" + O + ")[,|\\s]+(" + O + ")\\s*\\)?";
             return {
                 CSS_UNIT: new RegExp(O),
                 rgb: new RegExp("rgb" + X),
                 rgba: new RegExp("rgba" + re),
                 hsl: new RegExp("hsl" + X),
@@ -19468,99 +19468,99 @@
                 hex3: /^#?([0-9a-fA-F]{1})([0-9a-fA-F]{1})([0-9a-fA-F]{1})$/,
                 hex6: /^#?([0-9a-fA-F]{2})([0-9a-fA-F]{2})([0-9a-fA-F]{2})$/,
                 hex4: /^#?([0-9a-fA-F]{1})([0-9a-fA-F]{1})([0-9a-fA-F]{1})([0-9a-fA-F]{1})$/,
                 hex8: /^#?([0-9a-fA-F]{2})([0-9a-fA-F]{2})([0-9a-fA-F]{2})([0-9a-fA-F]{2})$/
             }
         }();
 
-        function Yt(D) {
-            return !!Ae.CSS_UNIT.exec(D)
+        function Yt(M) {
+            return !!Ae.CSS_UNIT.exec(M)
         }
 
-        function Di(D) {
-            D = D.replace(n, "").replace(i, "").toLowerCase();
+        function Mi(M) {
+            M = M.replace(n, "").replace(i, "").toLowerCase();
             var H = !1;
-            if (Te[D]) D = Te[D], H = !0;
-            else if (D == "transparent") return {
+            if (Te[M]) M = Te[M], H = !0;
+            else if (M == "transparent") return {
                 r: 0,
                 g: 0,
                 b: 0,
                 a: 0,
                 format: "name"
             };
             var O;
-            return (O = Ae.rgb.exec(D)) ? {
+            return (O = Ae.rgb.exec(M)) ? {
                 r: O[1],
                 g: O[2],
                 b: O[3]
-            } : (O = Ae.rgba.exec(D)) ? {
+            } : (O = Ae.rgba.exec(M)) ? {
                 r: O[1],
                 g: O[2],
                 b: O[3],
                 a: O[4]
-            } : (O = Ae.hsl.exec(D)) ? {
+            } : (O = Ae.hsl.exec(M)) ? {
                 h: O[1],
                 s: O[2],
                 l: O[3]
-            } : (O = Ae.hsla.exec(D)) ? {
+            } : (O = Ae.hsla.exec(M)) ? {
                 h: O[1],
                 s: O[2],
                 l: O[3],
                 a: O[4]
-            } : (O = Ae.hsv.exec(D)) ? {
+            } : (O = Ae.hsv.exec(M)) ? {
                 h: O[1],
                 s: O[2],
                 v: O[3]
-            } : (O = Ae.hsva.exec(D)) ? {
+            } : (O = Ae.hsva.exec(M)) ? {
                 h: O[1],
                 s: O[2],
                 v: O[3],
                 a: O[4]
-            } : (O = Ae.hex8.exec(D)) ? {
+            } : (O = Ae.hex8.exec(M)) ? {
                 r: ot(O[1]),
                 g: ot(O[2]),
                 b: ot(O[3]),
                 a: Ve(O[4]),
                 format: H ? "name" : "hex8"
-            } : (O = Ae.hex6.exec(D)) ? {
+            } : (O = Ae.hex6.exec(M)) ? {
                 r: ot(O[1]),
                 g: ot(O[2]),
                 b: ot(O[3]),
                 format: H ? "name" : "hex"
-            } : (O = Ae.hex4.exec(D)) ? {
+            } : (O = Ae.hex4.exec(M)) ? {
                 r: ot(O[1] + "" + O[1]),
                 g: ot(O[2] + "" + O[2]),
                 b: ot(O[3] + "" + O[3]),
                 a: Ve(O[4] + "" + O[4]),
                 format: H ? "name" : "hex8"
-            } : (O = Ae.hex3.exec(D)) ? {
+            } : (O = Ae.hex3.exec(M)) ? {
                 r: ot(O[1] + "" + O[1]),
                 g: ot(O[2] + "" + O[2]),
                 b: ot(O[3] + "" + O[3]),
                 format: H ? "name" : "hex"
             } : !1
         }
 
-        function Oi(D) {
+        function Oi(M) {
             var H, O;
-            return D = D || {
+            return M = M || {
                 level: "AA",
                 size: "small"
-            }, H = (D.level || "AA").toUpperCase(), O = (D.size || "small").toLowerCase(), H !== "AA" && H !== "AAA" && (H = "AA"), O !== "small" && O !== "large" && (O = "small"), {
+            }, H = (M.level || "AA").toUpperCase(), O = (M.size || "small").toLowerCase(), H !== "AA" && H !== "AAA" && (H = "AA"), O !== "small" && O !== "large" && (O = "small"), {
                 level: H,
                 size: O
             }
         }
         t.exports ? t.exports = c : window.tinycolor = c
     })(Math)
 })(c1);
 var N2 = c1.exports,
     Hs = l1(N2);
-var Og = {},
-    _f = {},
+var Mg = {},
+    Og = {},
     Yr = [],
     Ag = function() {
         var t = [].slice.call(arguments),
             e = t.length === 0 ? [] : t.reduce(function(n, i) {
                 return n.length < i.length ? n : i
             });
         return e.map(function(n, i) {
@@ -19600,20 +19600,20 @@
         i.hasOwnProperty("paths") && i.paths.forEach(function(r) {
             e.push(r.from), e.push(r.to)
         })
     });
     var n = Array.from(new Set(e));
     return n.sort(), n
 }
-var mi = function(t, e, n, i, r) {
-    this.divID = t, this.allData = [], this.dosData = {}, this.allSeries = [], this.dosSeries = [], this.allColorInfo = [], this.dosColorInfo = [], this.dosBackgroundColorInfo = [], this.currentPath = [], this.bandFermiEnergy = null, this.dosFermiEnergy = null, this.showFermi = e, this.showLegend = n, this.yLimit = i, this.dosRange = r, this.yLabel = "", typeof this.myChart < "u" && this.myChart.destroy()
+var mi = function(t, e, n, i) {
+    this.divID = t, this.allData = [], this.dosData = {}, this.allSeries = [], this.dosSeries = [], this.allColorInfo = [], this.dosColorInfo = [], this.dosBackgroundColorInfo = [], this.currentPath = [], this.bandFermiEnergy = null, this.dosFermiEnergy = null, this.energyRange = e ?? [null, null], this.dosRange = n ?? [null, null], this.yLabel = "", this.formatSettings = i ?? {}, this.showFermi = this.formatSettings.showFermi ?? !0, this.showLegend = this.formatSettings.showLegend ?? !0, typeof this.myChart < "u" && this.myChart.destroy()
 };
 mi.prototype.addBandStructure = function(t, e) {
     var n = ["#333333", "#e41a1c", "#377eb8", "#4daf4a", "#984ea3", "#ff7f00"];
-    if (typeof e > "u") {
+    if (!e) {
         var i = this.allColorInfo.length,
             r = Hs(n[i % n.length]);
         e = [r.toHexString(), r.darken(20).toHexString(), r.brighten(20).toHexString()]
     }
     this.allColorInfo.push(e), this.allData.push(t), this.bandFermiEnergy = t.fermi_level
 };
 mi.prototype.addDos = function(t) {
@@ -19626,23 +19626,23 @@
         var r = Hs(n[o % n.length]);
         r.setAlpha(.4), this.dosBackgroundColorInfo.push(r)
     }
     this.dosFermiEnergy = t.fermi_energy
 };
 mi.prototype.initChart = function(t) {
     var e = this;
-    this.showFermi === !1 ? Og = {} : Og = {
+    this.showFermi === !1 ? Mg = {} : Mg = {
         type: "line",
         id: "band-fermi",
         scaleID: "y",
         mode: "horizontal",
         value: 0,
         borderColor: "red",
         borderWidth: 2
-    }, console.log("ticksData", t), console.log("bandPlotObject", e);
+    };
     var n = {
         type: "scatter",
         data: {
             datasets: this.allSeries
         },
         options: {
             parsing: !1,
@@ -19718,19 +19718,19 @@
                     },
                     ticks: {
                         display: !1
                     }
                 }
             },
             annotation: {
-                annotations: [Og]
+                annotations: [Mg]
             }
         }
     };
-    e.yLimit && (n.options.scales.y.min = e.yLimit.ymin, n.options.scales.y.max = e.yLimit.ymax), e.xLimit && (n.options.scales.x.min = e.xLimit.xmin, n.options.scales.x.max = e.xLimit.xmax), e.yLabel && (n.options.scales.y.title.text = e.yLabel);
+    e.energyRange && (n.options.scales.y.min = e.energyRange[0], n.options.scales.y.max = e.energyRange[1]), e.xLimit && (n.options.scales.x.min = e.xLimit.xmin, n.options.scales.x.max = e.xLimit.xmax), e.yLabel && (n.options.scales.y.title.text = e.yLabel);
     var i = document.getElementById(this.divID).getContext("2d");
     e.myChart = new Fn(i, n), e.myChart.options.plugins.zoom.pan.enabled = !1
 };
 mi.prototype.initDosChart = function(t = "vertical") {
     var e = this,
         n = {};
     t === "vertical" ? (n.zeroLine = {
@@ -19749,15 +19749,15 @@
         borderWidth: 1,
         label: {
             display: !0,
             position: "end",
             content: "Fermi",
             xAdjust: 4
         }
-    }), _f = {
+    }), Og = {
         type: "scatter",
         data: {
             datasets: this.dosSeries
         },
         options: {
             indexAxis: "y",
             animation: !1,
@@ -19817,16 +19817,16 @@
                     grid: {
                         display: !0,
                         drawBorder: !0
                     },
                     border: {
                         display: !0
                     },
-                    min: e.yLimit.ymin,
-                    max: e.yLimit.ymax,
+                    min: e.energyRange[0],
+                    max: e.energyRange[1],
                     ticks: {
                         callback: function(r, o, s) {
                             if (o !== 0 && o != s.length - 1) return r
                         }
                     },
                     title: {
                         display: !0,
@@ -19868,15 +19868,15 @@
         borderColor: "red",
         borderWidth: 1,
         label: {
             display: !0,
             position: "start",
             content: "Fermi"
         }
-    }), _f = {
+    }), Og = {
         type: "scatter",
         data: {
             datasets: this.dosSeries
         },
         options: {
             animation: !1,
             plugins: {
@@ -19933,34 +19933,34 @@
                     display: !0,
                     position: "right",
                     grid: {
                         display: !0
                     },
                     title: {
                         display: !0,
-                        text: "E-Ef (eV)"
+                        text: "E - Ef (eV)"
                     },
-                    min: e.yLimit.ymin,
-                    max: e.yLimit.ymax,
+                    min: e.energyRange[0],
+                    max: e.energyRange[1],
                     ticks: {
                         callback: function(r, o, s) {
                             if (o !== 0 && o != s.length - 1) return r
                         }
                     }
                 }
             },
             elements: {
                 point: {
                     radius: 0
                 }
             }
         }
-    }), console.log("dosOptions", _f);
+    });
     var i = document.getElementById(this.divID + "-dos").getContext("2d");
-    e.myDos = new Fn(i, _f), e.myDos.options.plugins.zoom.pan.enabled = !1
+    e.myDos = new Fn(i, Og), e.myDos.options.plugins.zoom.pan.enabled = !1
 };
 mi.prototype.getDefaultPath = function() {
     if (this.allData.length > 0) {
         var t = this.allData[0].path;
         return t
     } else return []
 };
@@ -19973,93 +19973,92 @@
     var o = !1;
     if (n.currentPath.length != i.length ? o = !0 : Ag(n.currentPath, i).forEach(function(g) {
             g[0][0] != g[1][0] && (o = !0), g[0][1] != g[1][1] && (o = !0)
         }), !(!o && !e)) {
         n.currentPath = i;
         var s = function(g, y) {
                 for (var x = 0; x < y.length; x++) {
-                    var w = y[x];
-                    if (w.from == g[0] && w.to == g[1]) return {
-                        segment: w,
+                    var _ = y[x];
+                    if (_.from == g[0] && _.to == g[1]) return {
+                        segment: _,
                         reverse: !1
                     };
-                    if (w.from == g[1] && w.to == g[0]) return {
-                        segment: w,
+                    if (_.from == g[1] && _.to == g[0]) return {
+                        segment: _,
                         reverse: !0
                     }
                 }
                 return null
             },
             a = 0,
             l = [];
         n.allSeries = [], i.forEach(function(g, y) {
             l.length === 0 ? l.push([a, g[0]]) : l[l.length - 1][1] != g[0] && (l[l.length - 1][1] += "|" + g[0]);
             var x = !1,
-                w = null,
-                S;
-            n.allData.forEach(function(A, _) {
-                var C = s(g, A.paths);
-                if (C) {
+                _ = null,
+                C;
+            n.allData.forEach(function(A, w) {
+                var k = s(g, A.paths);
+                if (k) {
                     x = !0;
-                    var M = [],
-                        z = C.segment.x.length;
-                    if (C.reverse)
-                        for (S = C.segment.x.length - 1; S >= 0; S--) M.push(C.segment.x[z - 1] - C.segment.x[S]);
+                    var P = [],
+                        z = k.segment.x.length;
+                    if (k.reverse)
+                        for (C = k.segment.x.length - 1; C >= 0; C--) P.push(k.segment.x[z - 1] - k.segment.x[C]);
                     else
-                        for (S = 0; S < z; S++) M.push(C.segment.x[S] - C.segment.x[0]);
-                    var F = C.segment.two_band_types || !1,
-                        h = C.segment.values.length;
-                    w === null && (w = M[M.length - 1]);
-                    var Y = 1;
-                    if (M[M.length - 1] > 0)
-                        for (Y = w / M[M.length - 1], S = 0; S < M.length; S++) M[S] *= Y;
-                    w > 0 && C.segment.values.forEach(function(V, te) {
+                        for (C = 0; C < z; C++) P.push(k.segment.x[C] - k.segment.x[0]);
+                    var F = k.segment.two_band_types || !1,
+                        h = k.segment.values.length;
+                    _ === null && (_ = P[P.length - 1]);
+                    var $ = 1;
+                    if (P[P.length - 1] > 0)
+                        for ($ = _ / P[P.length - 1], C = 0; C < P.length; C++) P[C] *= $;
+                    _ > 0 && k.segment.values.forEach(function(Y, ne) {
                         var ie = [],
                             ce;
-                        if (C.reverse ? ce = V.slice().reverse() : ce = V, n.bandFermiEnergy) {
+                        if (k.reverse ? ce = Y.slice().reverse() : ce = Y, n.bandFermiEnergy) {
                             var he = ce.map(function(Te) {
                                 return Te - n.bandFermiEnergy
                             });
                             ce = he
                         }
-                        Ag(M, ce).forEach(function(Te) {
+                        Ag(P, ce).forEach(function(Te) {
                             ie.push({
                                 x: Te[0] + a,
                                 y: Te[1]
                             })
                         });
-                        var Fe = n.allColorInfo[_],
+                        var Fe = n.allColorInfo[w],
                             Ze = null;
-                        F ? te * 2 < h ? Ze = Fe[1] : Ze = Fe[2] : Ze = Fe[0];
+                        F ? ne * 2 < h ? Ze = Fe[1] : Ze = Fe[2] : Ze = Fe[0];
                         var Ee = {
-                            label: g[0] + "-" + g[1] + "." + te,
+                            label: g[0] + "-" + g[1] + "." + ne,
                             borderColor: Ze,
                             borderWidth: 2,
                             data: ie,
                             fill: !1,
                             showLine: !0,
                             pointRadius: 0
                         };
-                        F && te * 2 >= h && (Ee.borderDash = [10, 5]), n.allSeries.length < 1e4 && n.allSeries.push(Ee)
+                        F && ne * 2 >= h && (Ee.borderDash = [10, 5]), n.allSeries.length < 1e4 && n.allSeries.push(Ee)
                     })
                 }
-            }), x && w > 0 ? a += w : a += r, l.push([a, g[1]])
+            }), x && _ > 0 ? a += _ : a += r, l.push([a, g[1]])
         });
-        var c = n.updateTicks(l);
-        console.log("HIGH-SYM-ticks", l);
-        var d = c.map(function(g, y) {
-            return {
-                value: g[0],
-                label: g[1]
-            }
-        });
-        console.log("ticksData", d), n.xLimit = {
+        var c = n.updateTicks(l),
+            d = c.map(function(g, y) {
+                return {
+                    value: g[0],
+                    label: g[1]
+                }
+            });
+        n.xLimit = {
             xmin: 0,
             xmax: a
-        }, n.yLabel = n.allData[0].Y_label, n.yLabel === void 0 && (n.yLabel = "E - Ef (eV)"), n.myChart === void 0 ? n.initChart(d) : (n.myChart.options.scales.x.customTicks = d, n.myChart.data.datasets = n.allSeries, n.myChart.options.scales.x.max = a, n.myChart.update())
+        }, n.yLabel = n.allData[0].Y_label, n.yLabel === void 0 && (n.yLabel = this.formatSettings.bandsYlabel || "E - Ef (eV)"), n.myChart === void 0 ? n.initChart(d) : (n.myChart.options.scales.x.customTicks = d, n.myChart.data.datasets = n.allSeries, n.myChart.options.scales.x.max = a, n.myChart.update())
     }
 };
 mi.prototype.updateDosPlot = function(t = "vertical") {
     var e = this;
     e.dosSeries = [], Yr = [];
     var n = e.dosData.dos[0].x,
         i = e.dosData.dos[0].y;
@@ -20111,28 +20110,28 @@
         };
         e.dosData.dos[a].lineStyle === "dash" && (s.borderDash = [10, 5]), e.dosSeries.push(s)
     }
     e.myDos === void 0 && e.initDosChart(t), e.myDos.update()
 };
 mi.prototype.resBandZoom = function() {
     var t = this;
-    t.myChart.resetZoom(), t.myChart.options.scales.x.min = t.xLimit.xmin, t.myChart.options.scales.x.max = t.xLimit.xmax, t.myChart.options.scales.y.min = t.yLimit.ymin, t.myChart.options.scales.y.max = t.yLimit.ymax, t.myChart.update()
+    t.myChart.resetZoom(), t.myChart.options.scales.x.min = t.xLimit.xmin, t.myChart.options.scales.x.max = t.xLimit.xmax, t.energyRange && (t.myChart.options.scales.y.min = t.energyRange[0], t.myChart.options.scales.y.max = t.energyRange[1]), t.myChart.update()
 };
 mi.prototype.resDosZoom = function(t = "vertical") {
     var e = this;
-    e.myDos.resetZoom(), t === "vertical" ? (e.myDos.options.scales.y.min = e.yLimit.ymin, e.myDos.options.scales.y.max = e.yLimit.ymax) : (e.myDos.options.scales.x.min = e.yLimit.ymin, e.myDos.options.scales.x.max = e.yLimit.ymax), e.myDos.update()
+    e.myDos.resetZoom(), t === "vertical" ? (e.myDos.options.scales.y.min = e.energyRange[0], e.myDos.options.scales.y.max = e.energyRange[1]) : (e.myDos.options.scales.x.min = e.energyRange[0], e.myDos.options.scales.x.max = e.energyRange[1]), e.myDos.update()
 };
 mi.prototype.updateTicks = function(t) {
     var e = this,
         n, i = function(o, s) {
             var a = {};
             for (n = 0; n < s.length; n++) a[s[n][0]] = s[n][1];
             var l = function(x) {
-                    return x = x.replace(/GAMMA/gi, "\u0393"), x = x.replace(/DELTA/gi, "\u0394"), x = x.replace(/SIGMA/gi, "\u03A3"), x = x.replace(/LAMBDA/gi, "\u039B"), x = x.replace(/\-/gi, "\u2014"), x = x.replace(/_(.)/gi, function(w, S, A, _) {
-                        switch (S) {
+                    return x = x.replace(/GAMMA/gi, "\u0393"), x = x.replace(/DELTA/gi, "\u0394"), x = x.replace(/SIGMA/gi, "\u03A3"), x = x.replace(/LAMBDA/gi, "\u039B"), x = x.replace(/\-/gi, "\u2014"), x = x.replace(/_(.)/gi, function(_, C, A, w) {
+                        switch (C) {
                             case "0":
                                 return "\u2080";
                             case "1":
                                 return "\u2081";
                             case "2":
                                 return "\u2082";
                             case "3":
@@ -20146,20 +20145,20 @@
                             case "7":
                                 return "\u2087";
                             case "8":
                                 return "\u2088";
                             case "9":
                                 return "\u2089"
                         }
-                        return S
+                        return C
                     }), x
                 },
                 c = function(x) {
-                    return x == "G" && (x = "\u0393"), x = x.replace(/\-/gi, "\u2014"), x = x.replace(/(\d)/gi, function(w, S, A, _) {
-                        switch (S) {
+                    return x == "G" && (x = "\u0393"), x = x.replace(/\-/gi, "\u2014"), x = x.replace(/(\d)/gi, function(_, C, A, w) {
+                        switch (C) {
                             case "0":
                                 return "\u2080";
                             case "1":
                                 return "\u2081";
                             case "2":
                                 return "\u2082";
                             case "3":
@@ -20173,30 +20172,30 @@
                             case "7":
                                 return "\u2087";
                             case "8":
                                 return "\u2088";
                             case "9":
                                 return "\u2089"
                         }
-                        return S
+                        return C
                     }), x
                 },
                 d = f1([o]),
                 g = !1;
             d.findIndex(function(x) {
                 return x == "GAMMA"
             }) != -1 ? g = !1 : d.findIndex(function(x) {
                 return x == "G"
             }) != -1 ? g = !0 : g = !1;
             var y;
             return g ? y = c : y = l,
                 function(x) {
                     if (typeof x > "u") return x;
-                    var w = y(x);
-                    return w
+                    var _ = y(x);
+                    return _
                 }
         },
         r = i(e.allData, t);
     return t.map(function(o) {
         return [o[0], r(o[1])]
     })
 };
@@ -20221,34 +20220,34 @@
             a = i.push,
             l = i.indexOf,
             c = {},
             d = c.toString,
             g = c.hasOwnProperty,
             y = g.toString,
             x = y.call(Object),
-            w = {},
-            S = function(u) {
+            _ = {},
+            C = function(u) {
                 return typeof u == "function" && typeof u.nodeType != "number"
             },
             A = function(u) {
                 return u != null && u === u.window
             },
-            _ = e.document,
-            C = {
+            w = e.document,
+            k = {
                 type: !0,
                 src: !0,
                 nonce: !0,
                 noModule: !0
             };
 
-        function M(u, f, p) {
-            p = p || _;
+        function P(u, f, p) {
+            p = p || w;
             var m, v, b = p.createElement("script");
             if (b.text = u, f)
-                for (m in C) v = f[m] || f.getAttribute && f.getAttribute(m), v && b.setAttribute(m, v);
+                for (m in k) v = f[m] || f.getAttribute && f.getAttribute(m), v && b.setAttribute(m, v);
             p.head.appendChild(b).parentNode.removeChild(b)
         }
 
         function z(u) {
             return u == null ? u + "" : typeof u == "object" || typeof u == "function" ? c[d.call(u)] || "object" : typeof u
         }
         var F = "3.5.1",
@@ -20308,15 +20307,15 @@
             sort: i.sort,
             splice: i.splice
         }, h.extend = h.fn.extend = function() {
             var u, f, p, m, v, b, E = arguments[0] || {},
                 L = 1,
                 I = arguments.length,
                 B = !1;
-            for (typeof E == "boolean" && (B = E, E = arguments[L] || {}, L++), typeof E != "object" && !S(E) && (E = {}), L === I && (E = this, L--); L < I; L++)
+            for (typeof E == "boolean" && (B = E, E = arguments[L] || {}, L++), typeof E != "object" && !C(E) && (E = {}), L === I && (E = this, L--); L < I; L++)
                 if ((u = arguments[L]) != null)
                     for (f in u) m = u[f], !(f === "__proto__" || E === m) && (B && m && (h.isPlainObject(m) || (v = Array.isArray(m))) ? (p = E[f], v && !Array.isArray(p) ? b = [] : !v && !h.isPlainObject(p) ? b = {} : b = p, v = !1, E[f] = h.extend(B, b, m)) : m !== void 0 && (E[f] = m));
             return E
         }, h.extend({
             expando: "jQuery" + (F + Math.random()).replace(/\D/g, ""),
             isReady: !0,
             error: function(u) {
@@ -20329,30 +20328,30 @@
             },
             isEmptyObject: function(u) {
                 var f;
                 for (f in u) return !1;
                 return !0
             },
             globalEval: function(u, f, p) {
-                M(u, {
+                P(u, {
                     nonce: f && f.nonce
                 }, p)
             },
             each: function(u, f) {
                 var p, m = 0;
-                if (Y(u))
+                if ($(u))
                     for (p = u.length; m < p && f.call(u[m], m, u[m]) !== !1; m++);
                 else
                     for (m in u)
                         if (f.call(u[m], m, u[m]) === !1) break;
                 return u
             },
             makeArray: function(u, f) {
                 var p = f || [];
-                return u != null && (Y(Object(u)) ? h.merge(p, typeof u == "string" ? [u] : u) : a.call(p, u)), p
+                return u != null && ($(Object(u)) ? h.merge(p, typeof u == "string" ? [u] : u) : a.call(p, u)), p
             },
             inArray: function(u, f, p) {
                 return f == null ? -1 : l.call(f, u, p)
             },
             merge: function(u, f) {
                 for (var p = +f.length, m = 0, v = u.length; m < p; m++) u[v++] = f[m];
                 return u.length = v, u
@@ -20360,150 +20359,150 @@
             grep: function(u, f, p) {
                 for (var m, v = [], b = 0, E = u.length, L = !p; b < E; b++) m = !f(u[b], b), m !== L && v.push(u[b]);
                 return v
             },
             map: function(u, f, p) {
                 var m, v, b = 0,
                     E = [];
-                if (Y(u))
+                if ($(u))
                     for (m = u.length; b < m; b++) v = f(u[b], b, p), v != null && E.push(v);
                 else
                     for (b in u) v = f(u[b], b, p), v != null && E.push(v);
                 return s(E)
             },
             guid: 1,
-            support: w
+            support: _
         }), typeof Symbol == "function" && (h.fn[Symbol.iterator] = i[Symbol.iterator]), h.each("Boolean Number String Function Array Date RegExp Object Error Symbol".split(" "), function(u, f) {
             c["[object " + f + "]"] = f.toLowerCase()
         });
 
-        function Y(u) {
+        function $(u) {
             var f = !!u && "length" in u && u.length,
                 p = z(u);
-            return S(u) || A(u) ? !1 : p === "array" || f === 0 || typeof f == "number" && f > 0 && f - 1 in u
+            return C(u) || A(u) ? !1 : p === "array" || f === 0 || typeof f == "number" && f > 0 && f - 1 in u
         }
-        var V = function(u) {
-            var f, p, m, v, b, E, L, I, B, q, ee, U, Z, fe, _e, de, Tt, wt, Tn, Ue = "sizzle" + 1 * new Date,
+        var Y = function(u) {
+            var f, p, m, v, b, E, L, I, B, q, ee, V, Z, fe, _e, de, Tt, wt, Tn, Ue = "sizzle" + 1 * new Date,
                 be = u.document,
                 dn = 0,
                 ze = 0,
                 ct = Gl(),
-                aa = Gl(),
-                Xl = Gl(),
-                Pn = Gl(),
+                la = Gl(),
+                ql = Gl(),
+                Dn = Gl(),
                 oo = function(T, R) {
                     return T === R && (ee = !0), 0
                 },
                 so = {}.hasOwnProperty,
                 hn = [],
                 pr = hn.pop,
                 Wn = hn.push,
                 gr = hn.push,
                 cm = hn.slice,
                 ao = function(T, R) {
-                    for (var j = 0, G = T.length; j < G; j++)
+                    for (var j = 0, K = T.length; j < K; j++)
                         if (T[j] === R) return j;
                     return -1
                 },
-                Uf = "checked|selected|async|autofocus|autoplay|controls|defer|disabled|hidden|ismap|loop|multiple|open|readonly|required|scoped",
+                Vf = "checked|selected|async|autofocus|autoplay|controls|defer|disabled|hidden|ismap|loop|multiple|open|readonly|required|scoped",
                 He = "[\\x20\\t\\r\\n\\f]",
                 lo = "(?:\\\\[\\da-fA-F]{1,6}" + He + "?|\\\\[^\\r\\n\\f]|[\\w-]|[^\0-\\x7f])+",
                 fm = "\\[" + He + "*(" + lo + ")(?:" + He + "*([*^$|!~]?=)" + He + `*(?:'((?:\\\\.|[^\\\\'])*)'|"((?:\\\\.|[^\\\\"])*)"|(` + lo + "))|)" + He + "*\\]",
-                $f = ":(" + lo + `)(?:\\((('((?:\\\\.|[^\\\\'])*)'|"((?:\\\\.|[^\\\\"])*)")|((?:\\\\.|[^\\\\()[\\]]|` + fm + ")*)|.*)\\)|)",
+                Uf = ":(" + lo + `)(?:\\((('((?:\\\\.|[^\\\\'])*)'|"((?:\\\\.|[^\\\\"])*)")|((?:\\\\.|[^\\\\()[\\]]|` + fm + ")*)|.*)\\)|)",
                 L_ = new RegExp(He + "+", "g"),
-                ql = new RegExp("^" + He + "+|((?:^|[^\\\\])(?:\\\\.)*)" + He + "+$", "g"),
+                Zl = new RegExp("^" + He + "+|((?:^|[^\\\\])(?:\\\\.)*)" + He + "+$", "g"),
                 R_ = new RegExp("^" + He + "*," + He + "*"),
                 dm = new RegExp("^" + He + "*([>+~]|" + He + ")" + He + "*"),
                 I_ = new RegExp(He + "|>"),
-                N_ = new RegExp($f),
+                N_ = new RegExp(Uf),
                 z_ = new RegExp("^" + lo + "$"),
-                Zl = {
+                Kl = {
                     ID: new RegExp("^#(" + lo + ")"),
                     CLASS: new RegExp("^\\.(" + lo + ")"),
                     TAG: new RegExp("^(" + lo + "|[*])"),
                     ATTR: new RegExp("^" + fm),
-                    PSEUDO: new RegExp("^" + $f),
+                    PSEUDO: new RegExp("^" + Uf),
                     CHILD: new RegExp("^:(only|first|last|nth|nth-last)-(child|of-type)(?:\\(" + He + "*(even|odd|(([+-]|)(\\d*)n|)" + He + "*(?:([+-]|)" + He + "*(\\d+)|))" + He + "*\\)|)", "i"),
-                    bool: new RegExp("^(?:" + Uf + ")$", "i"),
+                    bool: new RegExp("^(?:" + Vf + ")$", "i"),
                     needsContext: new RegExp("^" + He + "*[>+~]|:(even|odd|eq|gt|lt|nth|first|last)(?:\\(" + He + "*((?:-\\d)?\\d*)" + He + "*\\)|)(?=[^-]|$)", "i")
                 },
                 F_ = /HTML$/i,
                 j_ = /^(?:input|select|textarea|button)$/i,
                 H_ = /^h\d$/i,
-                la = /^[^{]+\{\s*\[native \w/,
+                ua = /^[^{]+\{\s*\[native \w/,
                 B_ = /^(?:#([\w-]+)|(\w+)|\.([\w-]+))$/,
-                Yf = /[+~]/,
+                $f = /[+~]/,
                 Bi = new RegExp("\\\\[\\da-fA-F]{1,6}" + He + "?|\\\\([^\\r\\n\\f])", "g"),
                 Wi = function(T, R) {
                     var j = "0x" + T.slice(1) - 65536;
                     return R || (j < 0 ? String.fromCharCode(j + 65536) : String.fromCharCode(j >> 10 | 55296, j & 1023 | 56320))
                 },
                 hm = /([\0-\x1f\x7f]|^-?\d)|^-$|[^\0-\x1f\x7f-\uFFFF\w-]/g,
                 pm = function(T, R) {
                     return R ? T === "\0" ? "\uFFFD" : T.slice(0, -1) + "\\" + T.charCodeAt(T.length - 1).toString(16) + " " : "\\" + T
                 },
                 gm = function() {
-                    U()
+                    V()
                 },
-                W_ = Kl(function(T) {
+                W_ = Jl(function(T) {
                     return T.disabled === !0 && T.nodeName.toLowerCase() === "fieldset"
                 }, {
                     dir: "parentNode",
                     next: "legend"
                 });
             try {
                 gr.apply(hn = cm.call(be.childNodes), be.childNodes), hn[be.childNodes.length].nodeType
             } catch {
                 gr = {
                     apply: hn.length ? function(T, R) {
                         Wn.apply(T, cm.call(R))
                     } : function(T, R) {
-                        for (var j = T.length, G = 0; T[j++] = R[G++];);
+                        for (var j = T.length, K = 0; T[j++] = R[K++];);
                         T.length = j - 1
                     }
                 }
             }
 
-            function Xe(T, R, j, G) {
-                var W, Q, K, oe, ae, me, ge, xe = R && R.ownerDocument,
-                    De = R ? R.nodeType : 9;
-                if (j = j || [], typeof T != "string" || !T || De !== 1 && De !== 9 && De !== 11) return j;
-                if (!G && (U(R), R = R || Z, _e)) {
-                    if (De !== 11 && (ae = B_.exec(T)))
+            function Xe(T, R, j, K) {
+                var W, G, Q, oe, ae, me, ge, xe = R && R.ownerDocument,
+                    Me = R ? R.nodeType : 9;
+                if (j = j || [], typeof T != "string" || !T || Me !== 1 && Me !== 9 && Me !== 11) return j;
+                if (!K && (V(R), R = R || Z, _e)) {
+                    if (Me !== 11 && (ae = B_.exec(T)))
                         if (W = ae[1]) {
-                            if (De === 9)
-                                if (K = R.getElementById(W)) {
-                                    if (K.id === W) return j.push(K), j
+                            if (Me === 9)
+                                if (Q = R.getElementById(W)) {
+                                    if (Q.id === W) return j.push(Q), j
                                 } else return j;
-                            else if (xe && (K = xe.getElementById(W)) && Tn(R, K) && K.id === W) return j.push(K), j
+                            else if (xe && (Q = xe.getElementById(W)) && Tn(R, Q) && Q.id === W) return j.push(Q), j
                         } else {
                             if (ae[2]) return gr.apply(j, R.getElementsByTagName(T)), j;
                             if ((W = ae[3]) && p.getElementsByClassName && R.getElementsByClassName) return gr.apply(j, R.getElementsByClassName(W)), j
-                        } if (p.qsa && !Pn[T + " "] && (!de || !de.test(T)) && (De !== 1 || R.nodeName.toLowerCase() !== "object")) {
-                        if (ge = T, xe = R, De === 1 && (I_.test(T) || dm.test(T))) {
-                            for (xe = Yf.test(T) && qf(R.parentNode) || R, (xe !== R || !p.scope) && ((oe = R.getAttribute("id")) ? oe = oe.replace(hm, pm) : R.setAttribute("id", oe = Ue)), me = E(T), Q = me.length; Q--;) me[Q] = (oe ? "#" + oe : ":scope") + " " + Ql(me[Q]);
+                        } if (p.qsa && !Dn[T + " "] && (!de || !de.test(T)) && (Me !== 1 || R.nodeName.toLowerCase() !== "object")) {
+                        if (ge = T, xe = R, Me === 1 && (I_.test(T) || dm.test(T))) {
+                            for (xe = $f.test(T) && Xf(R.parentNode) || R, (xe !== R || !p.scope) && ((oe = R.getAttribute("id")) ? oe = oe.replace(hm, pm) : R.setAttribute("id", oe = Ue)), me = E(T), G = me.length; G--;) me[G] = (oe ? "#" + oe : ":scope") + " " + Ql(me[G]);
                             ge = me.join(",")
                         }
                         try {
                             return gr.apply(j, xe.querySelectorAll(ge)), j
                         } catch {
-                            Pn(T, !0)
+                            Dn(T, !0)
                         } finally {
                             oe === Ue && R.removeAttribute("id")
                         }
                     }
                 }
-                return I(T.replace(ql, "$1"), R, j, G)
+                return I(T.replace(Zl, "$1"), R, j, K)
             }
 
             function Gl() {
                 var T = [];
 
-                function R(j, G) {
-                    return T.push(j + " ") > m.cacheLength && delete R[T.shift()], R[j + " "] = G
+                function R(j, K) {
+                    return T.push(j + " ") > m.cacheLength && delete R[T.shift()], R[j + " "] = K
                 }
                 return R
             }
 
             function Jn(T) {
                 return T[Ue] = !0, T
             }
@@ -20515,22 +20514,22 @@
                 } catch {
                     return !1
                 } finally {
                     R.parentNode && R.parentNode.removeChild(R), R = null
                 }
             }
 
-            function Xf(T, R) {
-                for (var j = T.split("|"), G = j.length; G--;) m.attrHandle[j[G]] = R
+            function Yf(T, R) {
+                for (var j = T.split("|"), K = j.length; K--;) m.attrHandle[j[K]] = R
             }
 
             function mm(T, R) {
                 var j = R && T,
-                    G = j && T.nodeType === 1 && R.nodeType === 1 && T.sourceIndex - R.sourceIndex;
-                if (G) return G;
+                    K = j && T.nodeType === 1 && R.nodeType === 1 && T.sourceIndex - R.sourceIndex;
+                if (K) return K;
                 if (j) {
                     for (; j = j.nextSibling;)
                         if (j === R) return -1
                 }
                 return T ? 1 : -1
             }
 
@@ -20552,160 +20551,160 @@
                 return function(R) {
                     return "form" in R ? R.parentNode && R.disabled === !1 ? "label" in R ? "label" in R.parentNode ? R.parentNode.disabled === T : R.disabled === T : R.isDisabled === T || R.isDisabled !== !T && W_(R) === T : R.disabled === T : "label" in R ? R.disabled === T : !1
                 }
             }
 
             function uo(T) {
                 return Jn(function(R) {
-                    return R = +R, Jn(function(j, G) {
-                        for (var W, Q = T([], j.length, R), K = Q.length; K--;) j[W = Q[K]] && (j[W] = !(G[W] = j[W]))
+                    return R = +R, Jn(function(j, K) {
+                        for (var W, G = T([], j.length, R), Q = G.length; Q--;) j[W = G[Q]] && (j[W] = !(K[W] = j[W]))
                     })
                 })
             }
 
-            function qf(T) {
+            function Xf(T) {
                 return T && typeof T.getElementsByTagName < "u" && T
             }
             p = Xe.support = {}, b = Xe.isXML = function(T) {
                 var R = T.namespaceURI,
                     j = (T.ownerDocument || T).documentElement;
                 return !F_.test(R || j && j.nodeName || "HTML")
-            }, U = Xe.setDocument = function(T) {
-                var R, j, G = T ? T.ownerDocument || T : be;
-                return G == Z || G.nodeType !== 9 || !G.documentElement || (Z = G, fe = Z.documentElement, _e = !b(Z), be != Z && (j = Z.defaultView) && j.top !== j && (j.addEventListener ? j.addEventListener("unload", gm, !1) : j.attachEvent && j.attachEvent("onunload", gm)), p.scope = ei(function(W) {
+            }, V = Xe.setDocument = function(T) {
+                var R, j, K = T ? T.ownerDocument || T : be;
+                return K == Z || K.nodeType !== 9 || !K.documentElement || (Z = K, fe = Z.documentElement, _e = !b(Z), be != Z && (j = Z.defaultView) && j.top !== j && (j.addEventListener ? j.addEventListener("unload", gm, !1) : j.attachEvent && j.attachEvent("onunload", gm)), p.scope = ei(function(W) {
                     return fe.appendChild(W).appendChild(Z.createElement("div")), typeof W.querySelectorAll < "u" && !W.querySelectorAll(":scope fieldset div").length
                 }), p.attributes = ei(function(W) {
                     return W.className = "i", !W.getAttribute("className")
                 }), p.getElementsByTagName = ei(function(W) {
                     return W.appendChild(Z.createComment("")), !W.getElementsByTagName("*").length
-                }), p.getElementsByClassName = la.test(Z.getElementsByClassName), p.getById = ei(function(W) {
+                }), p.getElementsByClassName = ua.test(Z.getElementsByClassName), p.getById = ei(function(W) {
                     return fe.appendChild(W).id = Ue, !Z.getElementsByName || !Z.getElementsByName(Ue).length
                 }), p.getById ? (m.filter.ID = function(W) {
-                    var Q = W.replace(Bi, Wi);
-                    return function(K) {
-                        return K.getAttribute("id") === Q
-                    }
-                }, m.find.ID = function(W, Q) {
-                    if (typeof Q.getElementById < "u" && _e) {
-                        var K = Q.getElementById(W);
-                        return K ? [K] : []
+                    var G = W.replace(Bi, Wi);
+                    return function(Q) {
+                        return Q.getAttribute("id") === G
+                    }
+                }, m.find.ID = function(W, G) {
+                    if (typeof G.getElementById < "u" && _e) {
+                        var Q = G.getElementById(W);
+                        return Q ? [Q] : []
                     }
                 }) : (m.filter.ID = function(W) {
-                    var Q = W.replace(Bi, Wi);
-                    return function(K) {
-                        var oe = typeof K.getAttributeNode < "u" && K.getAttributeNode("id");
-                        return oe && oe.value === Q
-                    }
-                }, m.find.ID = function(W, Q) {
-                    if (typeof Q.getElementById < "u" && _e) {
-                        var K, oe, ae, me = Q.getElementById(W);
+                    var G = W.replace(Bi, Wi);
+                    return function(Q) {
+                        var oe = typeof Q.getAttributeNode < "u" && Q.getAttributeNode("id");
+                        return oe && oe.value === G
+                    }
+                }, m.find.ID = function(W, G) {
+                    if (typeof G.getElementById < "u" && _e) {
+                        var Q, oe, ae, me = G.getElementById(W);
                         if (me) {
-                            if (K = me.getAttributeNode("id"), K && K.value === W) return [me];
-                            for (ae = Q.getElementsByName(W), oe = 0; me = ae[oe++];)
-                                if (K = me.getAttributeNode("id"), K && K.value === W) return [me]
+                            if (Q = me.getAttributeNode("id"), Q && Q.value === W) return [me];
+                            for (ae = G.getElementsByName(W), oe = 0; me = ae[oe++];)
+                                if (Q = me.getAttributeNode("id"), Q && Q.value === W) return [me]
                         }
                         return []
                     }
-                }), m.find.TAG = p.getElementsByTagName ? function(W, Q) {
-                    if (typeof Q.getElementsByTagName < "u") return Q.getElementsByTagName(W);
-                    if (p.qsa) return Q.querySelectorAll(W)
-                } : function(W, Q) {
-                    var K, oe = [],
+                }), m.find.TAG = p.getElementsByTagName ? function(W, G) {
+                    if (typeof G.getElementsByTagName < "u") return G.getElementsByTagName(W);
+                    if (p.qsa) return G.querySelectorAll(W)
+                } : function(W, G) {
+                    var Q, oe = [],
                         ae = 0,
-                        me = Q.getElementsByTagName(W);
+                        me = G.getElementsByTagName(W);
                     if (W === "*") {
-                        for (; K = me[ae++];) K.nodeType === 1 && oe.push(K);
+                        for (; Q = me[ae++];) Q.nodeType === 1 && oe.push(Q);
                         return oe
                     }
                     return me
-                }, m.find.CLASS = p.getElementsByClassName && function(W, Q) {
-                    if (typeof Q.getElementsByClassName < "u" && _e) return Q.getElementsByClassName(W)
-                }, Tt = [], de = [], (p.qsa = la.test(Z.querySelectorAll)) && (ei(function(W) {
-                    var Q;
-                    fe.appendChild(W).innerHTML = "<a id='" + Ue + "'></a><select id='" + Ue + "-\r\\' msallowcapture=''><option selected=''></option></select>", W.querySelectorAll("[msallowcapture^='']").length && de.push("[*^$]=" + He + `*(?:''|"")`), W.querySelectorAll("[selected]").length || de.push("\\[" + He + "*(?:value|" + Uf + ")"), W.querySelectorAll("[id~=" + Ue + "-]").length || de.push("~="), Q = Z.createElement("input"), Q.setAttribute("name", ""), W.appendChild(Q), W.querySelectorAll("[name='']").length || de.push("\\[" + He + "*name" + He + "*=" + He + `*(?:''|"")`), W.querySelectorAll(":checked").length || de.push(":checked"), W.querySelectorAll("a#" + Ue + "+*").length || de.push(".#.+[+~]"), W.querySelectorAll("\\\f"), de.push("[\\r\\n\\f]")
+                }, m.find.CLASS = p.getElementsByClassName && function(W, G) {
+                    if (typeof G.getElementsByClassName < "u" && _e) return G.getElementsByClassName(W)
+                }, Tt = [], de = [], (p.qsa = ua.test(Z.querySelectorAll)) && (ei(function(W) {
+                    var G;
+                    fe.appendChild(W).innerHTML = "<a id='" + Ue + "'></a><select id='" + Ue + "-\r\\' msallowcapture=''><option selected=''></option></select>", W.querySelectorAll("[msallowcapture^='']").length && de.push("[*^$]=" + He + `*(?:''|"")`), W.querySelectorAll("[selected]").length || de.push("\\[" + He + "*(?:value|" + Vf + ")"), W.querySelectorAll("[id~=" + Ue + "-]").length || de.push("~="), G = Z.createElement("input"), G.setAttribute("name", ""), W.appendChild(G), W.querySelectorAll("[name='']").length || de.push("\\[" + He + "*name" + He + "*=" + He + `*(?:''|"")`), W.querySelectorAll(":checked").length || de.push(":checked"), W.querySelectorAll("a#" + Ue + "+*").length || de.push(".#.+[+~]"), W.querySelectorAll("\\\f"), de.push("[\\r\\n\\f]")
                 }), ei(function(W) {
                     W.innerHTML = "<a href='' disabled='disabled'></a><select disabled='disabled'><option/></select>";
-                    var Q = Z.createElement("input");
-                    Q.setAttribute("type", "hidden"), W.appendChild(Q).setAttribute("name", "D"), W.querySelectorAll("[name=d]").length && de.push("name" + He + "*[*^$|!~]?="), W.querySelectorAll(":enabled").length !== 2 && de.push(":enabled", ":disabled"), fe.appendChild(W).disabled = !0, W.querySelectorAll(":disabled").length !== 2 && de.push(":enabled", ":disabled"), W.querySelectorAll("*,:x"), de.push(",.*:")
-                })), (p.matchesSelector = la.test(wt = fe.matches || fe.webkitMatchesSelector || fe.mozMatchesSelector || fe.oMatchesSelector || fe.msMatchesSelector)) && ei(function(W) {
-                    p.disconnectedMatch = wt.call(W, "*"), wt.call(W, "[s!='']:x"), Tt.push("!=", $f)
-                }), de = de.length && new RegExp(de.join("|")), Tt = Tt.length && new RegExp(Tt.join("|")), R = la.test(fe.compareDocumentPosition), Tn = R || la.test(fe.contains) ? function(W, Q) {
-                    var K = W.nodeType === 9 ? W.documentElement : W,
-                        oe = Q && Q.parentNode;
-                    return W === oe || !!(oe && oe.nodeType === 1 && (K.contains ? K.contains(oe) : W.compareDocumentPosition && W.compareDocumentPosition(oe) & 16))
-                } : function(W, Q) {
-                    if (Q) {
-                        for (; Q = Q.parentNode;)
-                            if (Q === W) return !0
+                    var G = Z.createElement("input");
+                    G.setAttribute("type", "hidden"), W.appendChild(G).setAttribute("name", "D"), W.querySelectorAll("[name=d]").length && de.push("name" + He + "*[*^$|!~]?="), W.querySelectorAll(":enabled").length !== 2 && de.push(":enabled", ":disabled"), fe.appendChild(W).disabled = !0, W.querySelectorAll(":disabled").length !== 2 && de.push(":enabled", ":disabled"), W.querySelectorAll("*,:x"), de.push(",.*:")
+                })), (p.matchesSelector = ua.test(wt = fe.matches || fe.webkitMatchesSelector || fe.mozMatchesSelector || fe.oMatchesSelector || fe.msMatchesSelector)) && ei(function(W) {
+                    p.disconnectedMatch = wt.call(W, "*"), wt.call(W, "[s!='']:x"), Tt.push("!=", Uf)
+                }), de = de.length && new RegExp(de.join("|")), Tt = Tt.length && new RegExp(Tt.join("|")), R = ua.test(fe.compareDocumentPosition), Tn = R || ua.test(fe.contains) ? function(W, G) {
+                    var Q = W.nodeType === 9 ? W.documentElement : W,
+                        oe = G && G.parentNode;
+                    return W === oe || !!(oe && oe.nodeType === 1 && (Q.contains ? Q.contains(oe) : W.compareDocumentPosition && W.compareDocumentPosition(oe) & 16))
+                } : function(W, G) {
+                    if (G) {
+                        for (; G = G.parentNode;)
+                            if (G === W) return !0
                     }
                     return !1
-                }, oo = R ? function(W, Q) {
-                    if (W === Q) return ee = !0, 0;
-                    var K = !W.compareDocumentPosition - !Q.compareDocumentPosition;
-                    return K || (K = (W.ownerDocument || W) == (Q.ownerDocument || Q) ? W.compareDocumentPosition(Q) : 1, K & 1 || !p.sortDetached && Q.compareDocumentPosition(W) === K ? W == Z || W.ownerDocument == be && Tn(be, W) ? -1 : Q == Z || Q.ownerDocument == be && Tn(be, Q) ? 1 : q ? ao(q, W) - ao(q, Q) : 0 : K & 4 ? -1 : 1)
-                } : function(W, Q) {
-                    if (W === Q) return ee = !0, 0;
-                    var K, oe = 0,
+                }, oo = R ? function(W, G) {
+                    if (W === G) return ee = !0, 0;
+                    var Q = !W.compareDocumentPosition - !G.compareDocumentPosition;
+                    return Q || (Q = (W.ownerDocument || W) == (G.ownerDocument || G) ? W.compareDocumentPosition(G) : 1, Q & 1 || !p.sortDetached && G.compareDocumentPosition(W) === Q ? W == Z || W.ownerDocument == be && Tn(be, W) ? -1 : G == Z || G.ownerDocument == be && Tn(be, G) ? 1 : q ? ao(q, W) - ao(q, G) : 0 : Q & 4 ? -1 : 1)
+                } : function(W, G) {
+                    if (W === G) return ee = !0, 0;
+                    var Q, oe = 0,
                         ae = W.parentNode,
-                        me = Q.parentNode,
+                        me = G.parentNode,
                         ge = [W],
-                        xe = [Q];
-                    if (!ae || !me) return W == Z ? -1 : Q == Z ? 1 : ae ? -1 : me ? 1 : q ? ao(q, W) - ao(q, Q) : 0;
-                    if (ae === me) return mm(W, Q);
-                    for (K = W; K = K.parentNode;) ge.unshift(K);
-                    for (K = Q; K = K.parentNode;) xe.unshift(K);
+                        xe = [G];
+                    if (!ae || !me) return W == Z ? -1 : G == Z ? 1 : ae ? -1 : me ? 1 : q ? ao(q, W) - ao(q, G) : 0;
+                    if (ae === me) return mm(W, G);
+                    for (Q = W; Q = Q.parentNode;) ge.unshift(Q);
+                    for (Q = G; Q = Q.parentNode;) xe.unshift(Q);
                     for (; ge[oe] === xe[oe];) oe++;
                     return oe ? mm(ge[oe], xe[oe]) : ge[oe] == be ? -1 : xe[oe] == be ? 1 : 0
                 }), Z
             }, Xe.matches = function(T, R) {
                 return Xe(T, null, null, R)
             }, Xe.matchesSelector = function(T, R) {
-                if (U(T), p.matchesSelector && _e && !Pn[R + " "] && (!Tt || !Tt.test(R)) && (!de || !de.test(R))) try {
+                if (V(T), p.matchesSelector && _e && !Dn[R + " "] && (!Tt || !Tt.test(R)) && (!de || !de.test(R))) try {
                     var j = wt.call(T, R);
                     if (j || p.disconnectedMatch || T.document && T.document.nodeType !== 11) return j
                 } catch {
-                    Pn(R, !0)
+                    Dn(R, !0)
                 }
                 return Xe(R, Z, null, [T]).length > 0
             }, Xe.contains = function(T, R) {
-                return (T.ownerDocument || T) != Z && U(T), Tn(T, R)
+                return (T.ownerDocument || T) != Z && V(T), Tn(T, R)
             }, Xe.attr = function(T, R) {
-                (T.ownerDocument || T) != Z && U(T);
+                (T.ownerDocument || T) != Z && V(T);
                 var j = m.attrHandle[R.toLowerCase()],
-                    G = j && so.call(m.attrHandle, R.toLowerCase()) ? j(T, R, !_e) : void 0;
-                return G !== void 0 ? G : p.attributes || !_e ? T.getAttribute(R) : (G = T.getAttributeNode(R)) && G.specified ? G.value : null
+                    K = j && so.call(m.attrHandle, R.toLowerCase()) ? j(T, R, !_e) : void 0;
+                return K !== void 0 ? K : p.attributes || !_e ? T.getAttribute(R) : (K = T.getAttributeNode(R)) && K.specified ? K.value : null
             }, Xe.escape = function(T) {
                 return (T + "").replace(hm, pm)
             }, Xe.error = function(T) {
                 throw new Error("Syntax error, unrecognized expression: " + T)
             }, Xe.uniqueSort = function(T) {
                 var R, j = [],
-                    G = 0,
+                    K = 0,
                     W = 0;
                 if (ee = !p.detectDuplicates, q = !p.sortStable && T.slice(0), T.sort(oo), ee) {
-                    for (; R = T[W++];) R === T[W] && (G = j.push(W));
-                    for (; G--;) T.splice(j[G], 1)
+                    for (; R = T[W++];) R === T[W] && (K = j.push(W));
+                    for (; K--;) T.splice(j[K], 1)
                 }
                 return q = null, T
             }, v = Xe.getText = function(T) {
                 var R, j = "",
-                    G = 0,
+                    K = 0,
                     W = T.nodeType;
                 if (W) {
                     if (W === 1 || W === 9 || W === 11) {
                         if (typeof T.textContent == "string") return T.textContent;
                         for (T = T.firstChild; T; T = T.nextSibling) j += v(T)
                     } else if (W === 3 || W === 4) return T.nodeValue
                 } else
-                    for (; R = T[G++];) j += v(R);
+                    for (; R = T[K++];) j += v(R);
                 return j
             }, m = Xe.selectors = {
                 cacheLength: 50,
                 createPseudo: Jn,
-                match: Zl,
+                match: Kl,
                 attrHandle: {},
                 find: {},
                 relative: {
                     ">": {
                         dir: "parentNode",
                         first: !0
                     },
@@ -20725,15 +20724,15 @@
                         return T[1] = T[1].replace(Bi, Wi), T[3] = (T[3] || T[4] || T[5] || "").replace(Bi, Wi), T[2] === "~=" && (T[3] = " " + T[3] + " "), T.slice(0, 4)
                     },
                     CHILD: function(T) {
                         return T[1] = T[1].toLowerCase(), T[1].slice(0, 3) === "nth" ? (T[3] || Xe.error(T[0]), T[4] = +(T[4] ? T[5] + (T[6] || 1) : 2 * (T[3] === "even" || T[3] === "odd")), T[5] = +(T[7] + T[8] || T[3] === "odd")) : T[3] && Xe.error(T[0]), T
                     },
                     PSEUDO: function(T) {
                         var R, j = !T[6] && T[2];
-                        return Zl.CHILD.test(T[0]) ? null : (T[3] ? T[2] = T[4] || T[5] || "" : j && N_.test(j) && (R = E(j, !0)) && (R = j.indexOf(")", j.length - R) - j.length) && (T[0] = T[0].slice(0, R), T[2] = j.slice(0, R)), T.slice(0, 3))
+                        return Kl.CHILD.test(T[0]) ? null : (T[3] ? T[2] = T[4] || T[5] || "" : j && N_.test(j) && (R = E(j, !0)) && (R = j.indexOf(")", j.length - R) - j.length) && (T[0] = T[0].slice(0, R), T[2] = j.slice(0, R)), T.slice(0, 3))
                     }
                 },
                 filter: {
                     TAG: function(T) {
                         var R = T.replace(Bi, Wi).toLowerCase();
                         return T === "*" ? function() {
                             return !0
@@ -20744,71 +20743,71 @@
                     CLASS: function(T) {
                         var R = ct[T + " "];
                         return R || (R = new RegExp("(^|" + He + ")" + T + "(" + He + "|$)")) && ct(T, function(j) {
                             return R.test(typeof j.className == "string" && j.className || typeof j.getAttribute < "u" && j.getAttribute("class") || "")
                         })
                     },
                     ATTR: function(T, R, j) {
-                        return function(G) {
-                            var W = Xe.attr(G, T);
+                        return function(K) {
+                            var W = Xe.attr(K, T);
                             return W == null ? R === "!=" : R ? (W += "", R === "=" ? W === j : R === "!=" ? W !== j : R === "^=" ? j && W.indexOf(j) === 0 : R === "*=" ? j && W.indexOf(j) > -1 : R === "$=" ? j && W.slice(-j.length) === j : R === "~=" ? (" " + W.replace(L_, " ") + " ").indexOf(j) > -1 : R === "|=" ? W === j || W.slice(0, j.length + 1) === j + "-" : !1) : !0
                         }
                     },
-                    CHILD: function(T, R, j, G, W) {
-                        var Q = T.slice(0, 3) !== "nth",
-                            K = T.slice(-4) !== "last",
+                    CHILD: function(T, R, j, K, W) {
+                        var G = T.slice(0, 3) !== "nth",
+                            Q = T.slice(-4) !== "last",
                             oe = R === "of-type";
-                        return G === 1 && W === 0 ? function(ae) {
+                        return K === 1 && W === 0 ? function(ae) {
                             return !!ae.parentNode
                         } : function(ae, me, ge) {
-                            var xe, De, Ke, ye, Pt, Xt, Mn = Q !== K ? "nextSibling" : "previousSibling",
+                            var xe, Me, Qe, ye, Dt, Xt, Pn = G !== Q ? "nextSibling" : "previousSibling",
                                 st = ae.parentNode,
-                                ua = oe && ae.nodeName.toLowerCase(),
-                                ca = !ge && !oe,
-                                Dn = !1;
+                                ca = oe && ae.nodeName.toLowerCase(),
+                                fa = !ge && !oe,
+                                Mn = !1;
                             if (st) {
-                                if (Q) {
-                                    for (; Mn;) {
-                                        for (ye = ae; ye = ye[Mn];)
-                                            if (oe ? ye.nodeName.toLowerCase() === ua : ye.nodeType === 1) return !1;
-                                        Xt = Mn = T === "only" && !Xt && "nextSibling"
+                                if (G) {
+                                    for (; Pn;) {
+                                        for (ye = ae; ye = ye[Pn];)
+                                            if (oe ? ye.nodeName.toLowerCase() === ca : ye.nodeType === 1) return !1;
+                                        Xt = Pn = T === "only" && !Xt && "nextSibling"
                                     }
                                     return !0
                                 }
-                                if (Xt = [K ? st.firstChild : st.lastChild], K && ca) {
-                                    for (ye = st, Ke = ye[Ue] || (ye[Ue] = {}), De = Ke[ye.uniqueID] || (Ke[ye.uniqueID] = {}), xe = De[T] || [], Pt = xe[0] === dn && xe[1], Dn = Pt && xe[2], ye = Pt && st.childNodes[Pt]; ye = ++Pt && ye && ye[Mn] || (Dn = Pt = 0) || Xt.pop();)
-                                        if (ye.nodeType === 1 && ++Dn && ye === ae) {
-                                            De[T] = [dn, Pt, Dn];
+                                if (Xt = [Q ? st.firstChild : st.lastChild], Q && fa) {
+                                    for (ye = st, Qe = ye[Ue] || (ye[Ue] = {}), Me = Qe[ye.uniqueID] || (Qe[ye.uniqueID] = {}), xe = Me[T] || [], Dt = xe[0] === dn && xe[1], Mn = Dt && xe[2], ye = Dt && st.childNodes[Dt]; ye = ++Dt && ye && ye[Pn] || (Mn = Dt = 0) || Xt.pop();)
+                                        if (ye.nodeType === 1 && ++Mn && ye === ae) {
+                                            Me[T] = [dn, Dt, Mn];
                                             break
                                         }
-                                } else if (ca && (ye = ae, Ke = ye[Ue] || (ye[Ue] = {}), De = Ke[ye.uniqueID] || (Ke[ye.uniqueID] = {}), xe = De[T] || [], Pt = xe[0] === dn && xe[1], Dn = Pt), Dn === !1)
+                                } else if (fa && (ye = ae, Qe = ye[Ue] || (ye[Ue] = {}), Me = Qe[ye.uniqueID] || (Qe[ye.uniqueID] = {}), xe = Me[T] || [], Dt = xe[0] === dn && xe[1], Mn = Dt), Mn === !1)
                                     for (;
-                                        (ye = ++Pt && ye && ye[Mn] || (Dn = Pt = 0) || Xt.pop()) && !((oe ? ye.nodeName.toLowerCase() === ua : ye.nodeType === 1) && ++Dn && (ca && (Ke = ye[Ue] || (ye[Ue] = {}), De = Ke[ye.uniqueID] || (Ke[ye.uniqueID] = {}), De[T] = [dn, Dn]), ye === ae)););
-                                return Dn -= W, Dn === G || Dn % G === 0 && Dn / G >= 0
+                                        (ye = ++Dt && ye && ye[Pn] || (Mn = Dt = 0) || Xt.pop()) && !((oe ? ye.nodeName.toLowerCase() === ca : ye.nodeType === 1) && ++Mn && (fa && (Qe = ye[Ue] || (ye[Ue] = {}), Me = Qe[ye.uniqueID] || (Qe[ye.uniqueID] = {}), Me[T] = [dn, Mn]), ye === ae)););
+                                return Mn -= W, Mn === K || Mn % K === 0 && Mn / K >= 0
                             }
                         }
                     },
                     PSEUDO: function(T, R) {
-                        var j, G = m.pseudos[T] || m.setFilters[T.toLowerCase()] || Xe.error("unsupported pseudo: " + T);
-                        return G[Ue] ? G(R) : G.length > 1 ? (j = [T, T, "", R], m.setFilters.hasOwnProperty(T.toLowerCase()) ? Jn(function(W, Q) {
-                            for (var K, oe = G(W, R), ae = oe.length; ae--;) K = ao(W, oe[ae]), W[K] = !(Q[K] = oe[ae])
+                        var j, K = m.pseudos[T] || m.setFilters[T.toLowerCase()] || Xe.error("unsupported pseudo: " + T);
+                        return K[Ue] ? K(R) : K.length > 1 ? (j = [T, T, "", R], m.setFilters.hasOwnProperty(T.toLowerCase()) ? Jn(function(W, G) {
+                            for (var Q, oe = K(W, R), ae = oe.length; ae--;) Q = ao(W, oe[ae]), W[Q] = !(G[Q] = oe[ae])
                         }) : function(W) {
-                            return G(W, 0, j)
-                        }) : G
+                            return K(W, 0, j)
+                        }) : K
                     }
                 },
                 pseudos: {
                     not: Jn(function(T) {
                         var R = [],
                             j = [],
-                            G = L(T.replace(ql, "$1"));
-                        return G[Ue] ? Jn(function(W, Q, K, oe) {
-                            for (var ae, me = G(W, null, oe, []), ge = W.length; ge--;)(ae = me[ge]) && (W[ge] = !(Q[ge] = ae))
-                        }) : function(W, Q, K) {
-                            return R[0] = W, G(R, null, K, j), R[0] = null, !j.pop()
+                            K = L(T.replace(Zl, "$1"));
+                        return K[Ue] ? Jn(function(W, G, Q, oe) {
+                            for (var ae, me = K(W, null, oe, []), ge = W.length; ge--;)(ae = me[ge]) && (W[ge] = !(G[ge] = ae))
+                        }) : function(W, G, Q) {
+                            return R[0] = W, K(R, null, Q, j), R[0] = null, !j.pop()
                         }
                     }),
                     has: Jn(function(T) {
                         return function(R) {
                             return Xe(T, R).length > 0
                         }
                     }),
@@ -20882,19 +20881,19 @@
                         return T
                     }),
                     odd: uo(function(T, R) {
                         for (var j = 1; j < R; j += 2) T.push(j);
                         return T
                     }),
                     lt: uo(function(T, R, j) {
-                        for (var G = j < 0 ? j + R : j > R ? R : j; --G >= 0;) T.push(G);
+                        for (var K = j < 0 ? j + R : j > R ? R : j; --K >= 0;) T.push(K);
                         return T
                     }),
                     gt: uo(function(T, R, j) {
-                        for (var G = j < 0 ? j + R : j; ++G < R;) T.push(G);
+                        for (var K = j < 0 ? j + R : j; ++K < R;) T.push(K);
                         return T
                     })
                 }
             }, m.pseudos.nth = m.pseudos.eq;
             for (f in {
                     radio: !0,
                     checkbox: !0,
@@ -20905,202 +20904,202 @@
             for (f in {
                     submit: !0,
                     reset: !0
                 }) m.pseudos[f] = U_(f);
 
             function vm() {}
             vm.prototype = m.filters = m.pseudos, m.setFilters = new vm, E = Xe.tokenize = function(T, R) {
-                var j, G, W, Q, K, oe, ae, me = aa[T + " "];
+                var j, K, W, G, Q, oe, ae, me = la[T + " "];
                 if (me) return R ? 0 : me.slice(0);
-                for (K = T, oe = [], ae = m.preFilter; K;) {
-                    (!j || (G = R_.exec(K))) && (G && (K = K.slice(G[0].length) || K), oe.push(W = [])), j = !1, (G = dm.exec(K)) && (j = G.shift(), W.push({
+                for (Q = T, oe = [], ae = m.preFilter; Q;) {
+                    (!j || (K = R_.exec(Q))) && (K && (Q = Q.slice(K[0].length) || Q), oe.push(W = [])), j = !1, (K = dm.exec(Q)) && (j = K.shift(), W.push({
                         value: j,
-                        type: G[0].replace(ql, " ")
-                    }), K = K.slice(j.length));
-                    for (Q in m.filter)(G = Zl[Q].exec(K)) && (!ae[Q] || (G = ae[Q](G))) && (j = G.shift(), W.push({
+                        type: K[0].replace(Zl, " ")
+                    }), Q = Q.slice(j.length));
+                    for (G in m.filter)(K = Kl[G].exec(Q)) && (!ae[G] || (K = ae[G](K))) && (j = K.shift(), W.push({
                         value: j,
-                        type: Q,
-                        matches: G
-                    }), K = K.slice(j.length));
+                        type: G,
+                        matches: K
+                    }), Q = Q.slice(j.length));
                     if (!j) break
                 }
-                return R ? K.length : K ? Xe.error(T) : aa(T, oe).slice(0)
+                return R ? Q.length : Q ? Xe.error(T) : la(T, oe).slice(0)
             };
 
             function Ql(T) {
-                for (var R = 0, j = T.length, G = ""; R < j; R++) G += T[R].value;
-                return G
+                for (var R = 0, j = T.length, K = ""; R < j; R++) K += T[R].value;
+                return K
             }
 
-            function Kl(T, R, j) {
-                var G = R.dir,
+            function Jl(T, R, j) {
+                var K = R.dir,
                     W = R.next,
-                    Q = W || G,
-                    K = j && Q === "parentNode",
+                    G = W || K,
+                    Q = j && G === "parentNode",
                     oe = ze++;
                 return R.first ? function(ae, me, ge) {
-                    for (; ae = ae[G];)
-                        if (ae.nodeType === 1 || K) return T(ae, me, ge);
+                    for (; ae = ae[K];)
+                        if (ae.nodeType === 1 || Q) return T(ae, me, ge);
                     return !1
                 } : function(ae, me, ge) {
-                    var xe, De, Ke, ye = [dn, oe];
+                    var xe, Me, Qe, ye = [dn, oe];
                     if (ge) {
-                        for (; ae = ae[G];)
-                            if ((ae.nodeType === 1 || K) && T(ae, me, ge)) return !0
+                        for (; ae = ae[K];)
+                            if ((ae.nodeType === 1 || Q) && T(ae, me, ge)) return !0
                     } else
-                        for (; ae = ae[G];)
-                            if (ae.nodeType === 1 || K)
-                                if (Ke = ae[Ue] || (ae[Ue] = {}), De = Ke[ae.uniqueID] || (Ke[ae.uniqueID] = {}), W && W === ae.nodeName.toLowerCase()) ae = ae[G] || ae;
+                        for (; ae = ae[K];)
+                            if (ae.nodeType === 1 || Q)
+                                if (Qe = ae[Ue] || (ae[Ue] = {}), Me = Qe[ae.uniqueID] || (Qe[ae.uniqueID] = {}), W && W === ae.nodeName.toLowerCase()) ae = ae[K] || ae;
                                 else {
-                                    if ((xe = De[Q]) && xe[0] === dn && xe[1] === oe) return ye[2] = xe[2];
-                                    if (De[Q] = ye, ye[2] = T(ae, me, ge)) return !0
+                                    if ((xe = Me[G]) && xe[0] === dn && xe[1] === oe) return ye[2] = xe[2];
+                                    if (Me[G] = ye, ye[2] = T(ae, me, ge)) return !0
                                 } return !1
                 }
             }
 
-            function Zf(T) {
-                return T.length > 1 ? function(R, j, G) {
+            function qf(T) {
+                return T.length > 1 ? function(R, j, K) {
                     for (var W = T.length; W--;)
-                        if (!T[W](R, j, G)) return !1;
+                        if (!T[W](R, j, K)) return !1;
                     return !0
                 } : T[0]
             }
 
             function $_(T, R, j) {
-                for (var G = 0, W = R.length; G < W; G++) Xe(T, R[G], j);
+                for (var K = 0, W = R.length; K < W; K++) Xe(T, R[K], j);
                 return j
             }
 
-            function Jl(T, R, j, G, W) {
-                for (var Q, K = [], oe = 0, ae = T.length, me = R != null; oe < ae; oe++)(Q = T[oe]) && (!j || j(Q, G, W)) && (K.push(Q), me && R.push(oe));
-                return K
+            function eu(T, R, j, K, W) {
+                for (var G, Q = [], oe = 0, ae = T.length, me = R != null; oe < ae; oe++)(G = T[oe]) && (!j || j(G, K, W)) && (Q.push(G), me && R.push(oe));
+                return Q
             }
 
-            function Gf(T, R, j, G, W, Q) {
-                return G && !G[Ue] && (G = Gf(G)), W && !W[Ue] && (W = Gf(W, Q)), Jn(function(K, oe, ae, me) {
-                    var ge, xe, De, Ke = [],
+            function Zf(T, R, j, K, W, G) {
+                return K && !K[Ue] && (K = Zf(K)), W && !W[Ue] && (W = Zf(W, G)), Jn(function(Q, oe, ae, me) {
+                    var ge, xe, Me, Qe = [],
                         ye = [],
-                        Pt = oe.length,
-                        Xt = K || $_(R || "*", ae.nodeType ? [ae] : ae, []),
-                        Mn = T && (K || !R) ? Jl(Xt, Ke, T, ae, me) : Xt,
-                        st = j ? W || (K ? T : Pt || G) ? [] : oe : Mn;
-                    if (j && j(Mn, st, ae, me), G)
-                        for (ge = Jl(st, ye), G(ge, [], ae, me), xe = ge.length; xe--;)(De = ge[xe]) && (st[ye[xe]] = !(Mn[ye[xe]] = De));
-                    if (K) {
+                        Dt = oe.length,
+                        Xt = Q || $_(R || "*", ae.nodeType ? [ae] : ae, []),
+                        Pn = T && (Q || !R) ? eu(Xt, Qe, T, ae, me) : Xt,
+                        st = j ? W || (Q ? T : Dt || K) ? [] : oe : Pn;
+                    if (j && j(Pn, st, ae, me), K)
+                        for (ge = eu(st, ye), K(ge, [], ae, me), xe = ge.length; xe--;)(Me = ge[xe]) && (st[ye[xe]] = !(Pn[ye[xe]] = Me));
+                    if (Q) {
                         if (W || T) {
                             if (W) {
-                                for (ge = [], xe = st.length; xe--;)(De = st[xe]) && ge.push(Mn[xe] = De);
+                                for (ge = [], xe = st.length; xe--;)(Me = st[xe]) && ge.push(Pn[xe] = Me);
                                 W(null, st = [], ge, me)
                             }
-                            for (xe = st.length; xe--;)(De = st[xe]) && (ge = W ? ao(K, De) : Ke[xe]) > -1 && (K[ge] = !(oe[ge] = De))
+                            for (xe = st.length; xe--;)(Me = st[xe]) && (ge = W ? ao(Q, Me) : Qe[xe]) > -1 && (Q[ge] = !(oe[ge] = Me))
                         }
-                    } else st = Jl(st === oe ? st.splice(Pt, st.length) : st), W ? W(null, oe, st, me) : gr.apply(oe, st)
+                    } else st = eu(st === oe ? st.splice(Dt, st.length) : st), W ? W(null, oe, st, me) : gr.apply(oe, st)
                 })
             }
 
-            function Qf(T) {
-                for (var R, j, G, W = T.length, Q = m.relative[T[0].type], K = Q || m.relative[" "], oe = Q ? 1 : 0, ae = Kl(function(xe) {
+            function Kf(T) {
+                for (var R, j, K, W = T.length, G = m.relative[T[0].type], Q = G || m.relative[" "], oe = G ? 1 : 0, ae = Jl(function(xe) {
                         return xe === R
-                    }, K, !0), me = Kl(function(xe) {
+                    }, Q, !0), me = Jl(function(xe) {
                         return ao(R, xe) > -1
-                    }, K, !0), ge = [function(xe, De, Ke) {
-                        var ye = !Q && (Ke || De !== B) || ((R = De).nodeType ? ae(xe, De, Ke) : me(xe, De, Ke));
+                    }, Q, !0), ge = [function(xe, Me, Qe) {
+                        var ye = !G && (Qe || Me !== B) || ((R = Me).nodeType ? ae(xe, Me, Qe) : me(xe, Me, Qe));
                         return R = null, ye
                     }]; oe < W; oe++)
-                    if (j = m.relative[T[oe].type]) ge = [Kl(Zf(ge), j)];
+                    if (j = m.relative[T[oe].type]) ge = [Jl(qf(ge), j)];
                     else {
                         if (j = m.filter[T[oe].type].apply(null, T[oe].matches), j[Ue]) {
-                            for (G = ++oe; G < W && !m.relative[T[G].type]; G++);
-                            return Gf(oe > 1 && Zf(ge), oe > 1 && Ql(T.slice(0, oe - 1).concat({
+                            for (K = ++oe; K < W && !m.relative[T[K].type]; K++);
+                            return Zf(oe > 1 && qf(ge), oe > 1 && Ql(T.slice(0, oe - 1).concat({
                                 value: T[oe - 2].type === " " ? "*" : ""
-                            })).replace(ql, "$1"), j, oe < G && Qf(T.slice(oe, G)), G < W && Qf(T = T.slice(G)), G < W && Ql(T))
+                            })).replace(Zl, "$1"), j, oe < K && Kf(T.slice(oe, K)), K < W && Kf(T = T.slice(K)), K < W && Ql(T))
                         }
                         ge.push(j)
-                    } return Zf(ge)
+                    } return qf(ge)
             }
 
             function Y_(T, R) {
                 var j = R.length > 0,
-                    G = T.length > 0,
-                    W = function(Q, K, oe, ae, me) {
-                        var ge, xe, De, Ke = 0,
+                    K = T.length > 0,
+                    W = function(G, Q, oe, ae, me) {
+                        var ge, xe, Me, Qe = 0,
                             ye = "0",
-                            Pt = Q && [],
+                            Dt = G && [],
                             Xt = [],
-                            Mn = B,
-                            st = Q || G && m.find.TAG("*", me),
-                            ua = dn += Mn == null ? 1 : Math.random() || .1,
-                            ca = st.length;
-                        for (me && (B = K == Z || K || me); ye !== ca && (ge = st[ye]) != null; ye++) {
-                            if (G && ge) {
-                                for (xe = 0, !K && ge.ownerDocument != Z && (U(ge), oe = !_e); De = T[xe++];)
-                                    if (De(ge, K || Z, oe)) {
+                            Pn = B,
+                            st = G || K && m.find.TAG("*", me),
+                            ca = dn += Pn == null ? 1 : Math.random() || .1,
+                            fa = st.length;
+                        for (me && (B = Q == Z || Q || me); ye !== fa && (ge = st[ye]) != null; ye++) {
+                            if (K && ge) {
+                                for (xe = 0, !Q && ge.ownerDocument != Z && (V(ge), oe = !_e); Me = T[xe++];)
+                                    if (Me(ge, Q || Z, oe)) {
                                         ae.push(ge);
                                         break
-                                    } me && (dn = ua)
+                                    } me && (dn = ca)
                             }
-                            j && ((ge = !De && ge) && Ke--, Q && Pt.push(ge))
+                            j && ((ge = !Me && ge) && Qe--, G && Dt.push(ge))
                         }
-                        if (Ke += ye, j && ye !== Ke) {
-                            for (xe = 0; De = R[xe++];) De(Pt, Xt, K, oe);
-                            if (Q) {
-                                if (Ke > 0)
-                                    for (; ye--;) Pt[ye] || Xt[ye] || (Xt[ye] = pr.call(ae));
-                                Xt = Jl(Xt)
+                        if (Qe += ye, j && ye !== Qe) {
+                            for (xe = 0; Me = R[xe++];) Me(Dt, Xt, Q, oe);
+                            if (G) {
+                                if (Qe > 0)
+                                    for (; ye--;) Dt[ye] || Xt[ye] || (Xt[ye] = pr.call(ae));
+                                Xt = eu(Xt)
                             }
-                            gr.apply(ae, Xt), me && !Q && Xt.length > 0 && Ke + R.length > 1 && Xe.uniqueSort(ae)
+                            gr.apply(ae, Xt), me && !G && Xt.length > 0 && Qe + R.length > 1 && Xe.uniqueSort(ae)
                         }
-                        return me && (dn = ua, B = Mn), Pt
+                        return me && (dn = ca, B = Pn), Dt
                     };
                 return j ? Jn(W) : W
             }
             return L = Xe.compile = function(T, R) {
-                var j, G = [],
+                var j, K = [],
                     W = [],
-                    Q = Xl[T + " "];
-                if (!Q) {
-                    for (R || (R = E(T)), j = R.length; j--;) Q = Qf(R[j]), Q[Ue] ? G.push(Q) : W.push(Q);
-                    Q = Xl(T, Y_(W, G)), Q.selector = T
+                    G = ql[T + " "];
+                if (!G) {
+                    for (R || (R = E(T)), j = R.length; j--;) G = Kf(R[j]), G[Ue] ? K.push(G) : W.push(G);
+                    G = ql(T, Y_(W, K)), G.selector = T
                 }
-                return Q
-            }, I = Xe.select = function(T, R, j, G) {
-                var W, Q, K, oe, ae, me = typeof T == "function" && T,
-                    ge = !G && E(T = me.selector || T);
+                return G
+            }, I = Xe.select = function(T, R, j, K) {
+                var W, G, Q, oe, ae, me = typeof T == "function" && T,
+                    ge = !K && E(T = me.selector || T);
                 if (j = j || [], ge.length === 1) {
-                    if (Q = ge[0] = ge[0].slice(0), Q.length > 2 && (K = Q[0]).type === "ID" && R.nodeType === 9 && _e && m.relative[Q[1].type]) {
-                        if (R = (m.find.ID(K.matches[0].replace(Bi, Wi), R) || [])[0], R) me && (R = R.parentNode);
+                    if (G = ge[0] = ge[0].slice(0), G.length > 2 && (Q = G[0]).type === "ID" && R.nodeType === 9 && _e && m.relative[G[1].type]) {
+                        if (R = (m.find.ID(Q.matches[0].replace(Bi, Wi), R) || [])[0], R) me && (R = R.parentNode);
                         else return j;
-                        T = T.slice(Q.shift().value.length)
+                        T = T.slice(G.shift().value.length)
                     }
-                    for (W = Zl.needsContext.test(T) ? 0 : Q.length; W-- && (K = Q[W], !m.relative[oe = K.type]);)
-                        if ((ae = m.find[oe]) && (G = ae(K.matches[0].replace(Bi, Wi), Yf.test(Q[0].type) && qf(R.parentNode) || R))) {
-                            if (Q.splice(W, 1), T = G.length && Ql(Q), !T) return gr.apply(j, G), j;
+                    for (W = Kl.needsContext.test(T) ? 0 : G.length; W-- && (Q = G[W], !m.relative[oe = Q.type]);)
+                        if ((ae = m.find[oe]) && (K = ae(Q.matches[0].replace(Bi, Wi), $f.test(G[0].type) && Xf(R.parentNode) || R))) {
+                            if (G.splice(W, 1), T = K.length && Ql(G), !T) return gr.apply(j, K), j;
                             break
                         }
                 }
-                return (me || L(T, ge))(G, R, !_e, j, !R || Yf.test(T) && qf(R.parentNode) || R), j
-            }, p.sortStable = Ue.split("").sort(oo).join("") === Ue, p.detectDuplicates = !!ee, U(), p.sortDetached = ei(function(T) {
+                return (me || L(T, ge))(K, R, !_e, j, !R || $f.test(T) && Xf(R.parentNode) || R), j
+            }, p.sortStable = Ue.split("").sort(oo).join("") === Ue, p.detectDuplicates = !!ee, V(), p.sortDetached = ei(function(T) {
                 return T.compareDocumentPosition(Z.createElement("fieldset")) & 1
             }), ei(function(T) {
                 return T.innerHTML = "<a href='#'></a>", T.firstChild.getAttribute("href") === "#"
-            }) || Xf("type|href|height|width", function(T, R, j) {
+            }) || Yf("type|href|height|width", function(T, R, j) {
                 if (!j) return T.getAttribute(R, R.toLowerCase() === "type" ? 1 : 2)
             }), (!p.attributes || !ei(function(T) {
                 return T.innerHTML = "<input/>", T.firstChild.setAttribute("value", ""), T.firstChild.getAttribute("value") === ""
-            })) && Xf("value", function(T, R, j) {
+            })) && Yf("value", function(T, R, j) {
                 if (!j && T.nodeName.toLowerCase() === "input") return T.defaultValue
             }), ei(function(T) {
                 return T.getAttribute("disabled") == null
-            }) || Xf(Uf, function(T, R, j) {
-                var G;
-                if (!j) return T[R] === !0 ? R.toLowerCase() : (G = T.getAttributeNode(R)) && G.specified ? G.value : null
+            }) || Yf(Vf, function(T, R, j) {
+                var K;
+                if (!j) return T[R] === !0 ? R.toLowerCase() : (K = T.getAttributeNode(R)) && K.specified ? K.value : null
             }), Xe
         }(e);
-        h.find = V, h.expr = V.selectors, h.expr[":"] = h.expr.pseudos, h.uniqueSort = h.unique = V.uniqueSort, h.text = V.getText, h.isXMLDoc = V.isXML, h.contains = V.contains, h.escapeSelector = V.escape;
-        var te = function(u, f, p) {
+        h.find = Y, h.expr = Y.selectors, h.expr[":"] = h.expr.pseudos, h.uniqueSort = h.unique = Y.uniqueSort, h.text = Y.getText, h.isXMLDoc = Y.isXML, h.contains = Y.contains, h.escapeSelector = Y.escape;
+        var ne = function(u, f, p) {
                 for (var m = [], v = p !== void 0;
                     (u = u[f]) && u.nodeType !== 9;)
                     if (u.nodeType === 1) {
                         if (v && h(u).is(p)) break;
                         m.push(u)
                     } return m
             },
@@ -21112,15 +21111,15 @@
 
         function he(u, f) {
             return u.nodeName && u.nodeName.toLowerCase() === f.toLowerCase()
         }
         var Fe = /^<([a-z][^\/\0>:\x20\t\r\n\f]*)[\x20\t\r\n\f]*\/?>(?:<\/\1>|)$/i;
 
         function Ze(u, f, p) {
-            return S(f) ? h.grep(u, function(m, v) {
+            return C(f) ? h.grep(u, function(m, v) {
                 return !!f.call(m, v, m) !== p
             }) : f.nodeType ? h.grep(u, function(m) {
                 return m === f !== p
             }) : typeof f != "string" ? h.grep(u, function(m) {
                 return l.call(f, m) > -1 !== p
             }) : h.filter(f, u, p)
         }
@@ -21153,26 +21152,26 @@
         var Ee, Te = /^(?:\s*(<[\w\W]+>)[^>]*|#([\w-]+))$/,
             Ye = h.fn.init = function(u, f, p) {
                 var m, v;
                 if (!u) return this;
                 if (p = p || Ee, typeof u == "string")
                     if (u[0] === "<" && u[u.length - 1] === ">" && u.length >= 3 ? m = [null, u, null] : m = Te.exec(u), m && (m[1] || !f))
                         if (m[1]) {
-                            if (f = f instanceof h ? f[0] : f, h.merge(this, h.parseHTML(m[1], f && f.nodeType ? f.ownerDocument || f : _, !0)), Fe.test(m[1]) && h.isPlainObject(f))
-                                for (m in f) S(this[m]) ? this[m](f[m]) : this.attr(m, f[m]);
+                            if (f = f instanceof h ? f[0] : f, h.merge(this, h.parseHTML(m[1], f && f.nodeType ? f.ownerDocument || f : w, !0)), Fe.test(m[1]) && h.isPlainObject(f))
+                                for (m in f) C(this[m]) ? this[m](f[m]) : this.attr(m, f[m]);
                             return this
-                        } else return v = _.getElementById(m[2]), v && (this[0] = v, this.length = 1), this;
+                        } else return v = w.getElementById(m[2]), v && (this[0] = v, this.length = 1), this;
                 else return !f || f.jquery ? (f || p).find(u) : this.constructor(f).find(u);
                 else {
                     if (u.nodeType) return this[0] = u, this.length = 1, this;
-                    if (S(u)) return p.ready !== void 0 ? p.ready(u) : u(h)
+                    if (C(u)) return p.ready !== void 0 ? p.ready(u) : u(h)
                 }
                 return h.makeArray(u, this)
             };
-        Ye.prototype = h.fn, Ee = h(_);
+        Ye.prototype = h.fn, Ee = h(w);
         var Ot = /^(?:parents|prev(?:Until|All))/,
             lt = {
                 children: !0,
                 contents: !0,
                 next: !0,
                 prev: !0
             };
@@ -21218,36 +21217,36 @@
         }
         h.each({
             parent: function(u) {
                 var f = u.parentNode;
                 return f && f.nodeType !== 11 ? f : null
             },
             parents: function(u) {
-                return te(u, "parentNode")
+                return ne(u, "parentNode")
             },
             parentsUntil: function(u, f, p) {
-                return te(u, "parentNode", p)
+                return ne(u, "parentNode", p)
             },
             next: function(u) {
                 return Oe(u, "nextSibling")
             },
             prev: function(u) {
                 return Oe(u, "previousSibling")
             },
             nextAll: function(u) {
-                return te(u, "nextSibling")
+                return ne(u, "nextSibling")
             },
             prevAll: function(u) {
-                return te(u, "previousSibling")
+                return ne(u, "previousSibling")
             },
             nextUntil: function(u, f, p) {
-                return te(u, "nextSibling", p)
+                return ne(u, "nextSibling", p)
             },
             prevUntil: function(u, f, p) {
-                return te(u, "previousSibling", p)
+                return ne(u, "previousSibling", p)
             },
             siblings: function(u) {
                 return ie((u.parentNode || {}).firstChild, u)
             },
             children: function(u) {
                 return ie(u.firstChild)
             },
@@ -21256,19 +21255,19 @@
             }
         }, function(u, f) {
             h.fn[u] = function(p, m) {
                 var v = h.map(this, f, p);
                 return u.slice(-5) !== "Until" && (m = p), m && typeof m == "string" && (v = h.filter(m, v)), this.length > 1 && (lt[u] || h.uniqueSort(v), Ot.test(u) && v.reverse()), this.pushStack(v)
             }
         });
-        var Ge = /[^\x20\t\r\n\f]+/g;
+        var Ke = /[^\x20\t\r\n\f]+/g;
 
         function ot(u) {
             var f = {};
-            return h.each(u.match(Ge) || [], function(p, m) {
+            return h.each(u.match(Ke) || [], function(p, m) {
                 f[m] = !0
             }), f
         }
         h.Callbacks = function(u) {
             u = typeof u == "string" ? ot(u) : h.extend({}, u);
             var f, p, m, v, b = [],
                 E = [],
@@ -21277,23 +21276,23 @@
                     for (v = v || u.once, m = f = !0; E.length; L = -1)
                         for (p = E.shift(); ++L < b.length;) b[L].apply(p[0], p[1]) === !1 && u.stopOnFalse && (L = b.length, p = !1);
                     u.memory || (p = !1), f = !1, v && (p ? b = [] : b = "")
                 },
                 B = {
                     add: function() {
                         return b && (p && !f && (L = b.length - 1, E.push(p)), function q(ee) {
-                            h.each(ee, function(U, Z) {
-                                S(Z) ? (!u.unique || !B.has(Z)) && b.push(Z) : Z && Z.length && z(Z) !== "string" && q(Z)
+                            h.each(ee, function(V, Z) {
+                                C(Z) ? (!u.unique || !B.has(Z)) && b.push(Z) : Z && Z.length && z(Z) !== "string" && q(Z)
                             })
                         }(arguments), p && !f && I()), this
                     },
                     remove: function() {
                         return h.each(arguments, function(q, ee) {
-                            for (var U;
-                                (U = h.inArray(ee, b, U)) > -1;) b.splice(U, 1), U <= L && L--
+                            for (var V;
+                                (V = h.inArray(ee, b, V)) > -1;) b.splice(V, 1), V <= L && L--
                         }), this
                     },
                     has: function(q) {
                         return q ? h.inArray(q, b) > -1 : b.length > 0
                     },
                     empty: function() {
                         return b && (b = []), this
@@ -21330,15 +21329,15 @@
         function $t(u) {
             throw u
         }
 
         function mt(u, f, p, m) {
             var v;
             try {
-                u && S(v = u.promise) ? v.call(u).done(f).fail(p) : u && S(v = u.then) ? v.call(u, f, p) : f.apply(void 0, [u].slice(m))
+                u && C(v = u.promise) ? v.call(u).done(f).fail(p) : u && C(v = u.then) ? v.call(u, f, p) : f.apply(void 0, [u].slice(m))
             } catch (b) {
                 p.apply(void 0, [b])
             }
         }
         h.extend({
             Deferred: function(u) {
                 var f = [
@@ -21357,48 +21356,48 @@
                         catch: function(b) {
                             return m.then(null, b)
                         },
                         pipe: function() {
                             var b = arguments;
                             return h.Deferred(function(E) {
                                 h.each(f, function(L, I) {
-                                    var B = S(b[I[4]]) && b[I[4]];
+                                    var B = C(b[I[4]]) && b[I[4]];
                                     v[I[1]](function() {
                                         var q = B && B.apply(this, arguments);
-                                        q && S(q.promise) ? q.promise().progress(E.notify).done(E.resolve).fail(E.reject) : E[I[0] + "With"](this, B ? [q] : arguments)
+                                        q && C(q.promise) ? q.promise().progress(E.notify).done(E.resolve).fail(E.reject) : E[I[0] + "With"](this, B ? [q] : arguments)
                                     })
                                 }), b = null
                             }).promise()
                         },
                         then: function(b, E, L) {
                             var I = 0;
 
-                            function B(q, ee, U, Z) {
+                            function B(q, ee, V, Z) {
                                 return function() {
                                     var fe = this,
                                         _e = arguments,
                                         de = function() {
                                             var wt, Tn;
                                             if (!(q < I)) {
-                                                if (wt = U.apply(fe, _e), wt === ee.promise()) throw new TypeError("Thenable self-resolution");
-                                                Tn = wt && (typeof wt == "object" || typeof wt == "function") && wt.then, S(Tn) ? Z ? Tn.call(wt, B(I, ee, At, Z), B(I, ee, $t, Z)) : (I++, Tn.call(wt, B(I, ee, At, Z), B(I, ee, $t, Z), B(I, ee, At, ee.notifyWith))) : (U !== At && (fe = void 0, _e = [wt]), (Z || ee.resolveWith)(fe, _e))
+                                                if (wt = V.apply(fe, _e), wt === ee.promise()) throw new TypeError("Thenable self-resolution");
+                                                Tn = wt && (typeof wt == "object" || typeof wt == "function") && wt.then, C(Tn) ? Z ? Tn.call(wt, B(I, ee, At, Z), B(I, ee, $t, Z)) : (I++, Tn.call(wt, B(I, ee, At, Z), B(I, ee, $t, Z), B(I, ee, At, ee.notifyWith))) : (V !== At && (fe = void 0, _e = [wt]), (Z || ee.resolveWith)(fe, _e))
                                             }
                                         },
                                         Tt = Z ? de : function() {
                                             try {
                                                 de()
                                             } catch (wt) {
-                                                h.Deferred.exceptionHook && h.Deferred.exceptionHook(wt, Tt.stackTrace), q + 1 >= I && (U !== $t && (fe = void 0, _e = [wt]), ee.rejectWith(fe, _e))
+                                                h.Deferred.exceptionHook && h.Deferred.exceptionHook(wt, Tt.stackTrace), q + 1 >= I && (V !== $t && (fe = void 0, _e = [wt]), ee.rejectWith(fe, _e))
                                             }
                                         };
                                     q ? Tt() : (h.Deferred.getStackHook && (Tt.stackTrace = h.Deferred.getStackHook()), e.setTimeout(Tt))
                                 }
                             }
                             return h.Deferred(function(q) {
-                                f[0][3].add(B(0, q, S(L) ? L : At, q.notifyWith)), f[1][3].add(B(0, q, S(b) ? b : At)), f[2][3].add(B(0, q, S(E) ? E : $t))
+                                f[0][3].add(B(0, q, C(L) ? L : At, q.notifyWith)), f[1][3].add(B(0, q, C(b) ? b : At)), f[2][3].add(B(0, q, C(E) ? E : $t))
                             }).promise()
                         },
                         promise: function(b) {
                             return b != null ? h.extend(b, m) : m
                         }
                     },
                     v = {};
@@ -21419,15 +21418,15 @@
                     v = o.call(arguments),
                     b = h.Deferred(),
                     E = function(L) {
                         return function(I) {
                             m[L] = this, v[L] = arguments.length > 1 ? o.call(arguments) : I, --f || b.resolveWith(m, v)
                         }
                     };
-                if (f <= 1 && (mt(u, b.done(E(p)).resolve, b.reject, !f), b.state() === "pending" || S(v[p] && v[p].then))) return b.then();
+                if (f <= 1 && (mt(u, b.done(E(p)).resolve, b.reject, !f), b.state() === "pending" || C(v[p] && v[p].then))) return b.then();
                 for (; p--;) mt(v[p], E(p), b.reject);
                 return b.promise()
             }
         });
         var je = /^(Eval|Internal|Range|Reference|Syntax|Type|URI)Error$/;
         h.Deferred.exceptionHook = function(u, f) {
             e.console && e.console.warn && u && je.test(u.name) && e.console.warn("jQuery.Deferred exception: " + u.message, u.stack, f)
@@ -21441,44 +21440,44 @@
             return ln.then(u).catch(function(f) {
                 h.readyException(f)
             }), this
         }, h.extend({
             isReady: !1,
             readyWait: 1,
             ready: function(u) {
-                (u === !0 ? --h.readyWait : h.isReady) || (h.isReady = !0, !(u !== !0 && --h.readyWait > 0) && ln.resolveWith(_, [h]))
+                (u === !0 ? --h.readyWait : h.isReady) || (h.isReady = !0, !(u !== !0 && --h.readyWait > 0) && ln.resolveWith(w, [h]))
             }
         }), h.ready.then = ln.then;
 
         function Ve() {
-            _.removeEventListener("DOMContentLoaded", Ve), e.removeEventListener("load", Ve), h.ready()
+            w.removeEventListener("DOMContentLoaded", Ve), e.removeEventListener("load", Ve), h.ready()
         }
-        _.readyState === "complete" || _.readyState !== "loading" && !_.documentElement.doScroll ? e.setTimeout(h.ready) : (_.addEventListener("DOMContentLoaded", Ve), e.addEventListener("load", Ve));
+        w.readyState === "complete" || w.readyState !== "loading" && !w.documentElement.doScroll ? e.setTimeout(h.ready) : (w.addEventListener("DOMContentLoaded", Ve), e.addEventListener("load", Ve));
         var Ae = function(u, f, p, m, v, b, E) {
                 var L = 0,
                     I = u.length,
                     B = p == null;
                 if (z(p) === "object") {
                     v = !0;
                     for (L in p) Ae(u, f, L, p[L], !0, b, E)
-                } else if (m !== void 0 && (v = !0, S(m) || (E = !0), B && (E ? (f.call(u, m), f = null) : (B = f, f = function(q, ee, U) {
-                        return B.call(h(q), U)
+                } else if (m !== void 0 && (v = !0, C(m) || (E = !0), B && (E ? (f.call(u, m), f = null) : (B = f, f = function(q, ee, V) {
+                        return B.call(h(q), V)
                     })), f))
                     for (; L < I; L++) f(u[L], p, E ? m : m.call(u[L], L, f(u[L], p)));
                 return v ? u : B ? f.call(u) : I ? f(u[0], p) : b
             },
             Yt = /^-ms-/,
-            Di = /-([a-z])/g;
+            Mi = /-([a-z])/g;
 
         function Oi(u, f) {
             return f.toUpperCase()
         }
 
-        function D(u) {
-            return u.replace(Yt, "ms-").replace(Di, Oi)
+        function M(u) {
+            return u.replace(Yt, "ms-").replace(Mi, Oi)
         }
         var H = function(u) {
             return u.nodeType === 1 || u.nodeType === 9 || !+u.nodeType
         };
 
         function O() {
             this.expando = h.expando + O.uid++
@@ -21489,53 +21488,53 @@
                 return f || (f = {}, H(u) && (u.nodeType ? u[this.expando] = f : Object.defineProperty(u, this.expando, {
                     value: f,
                     configurable: !0
                 }))), f
             },
             set: function(u, f, p) {
                 var m, v = this.cache(u);
-                if (typeof f == "string") v[D(f)] = p;
+                if (typeof f == "string") v[M(f)] = p;
                 else
-                    for (m in f) v[D(m)] = f[m];
+                    for (m in f) v[M(m)] = f[m];
                 return v
             },
             get: function(u, f) {
-                return f === void 0 ? this.cache(u) : u[this.expando] && u[this.expando][D(f)]
+                return f === void 0 ? this.cache(u) : u[this.expando] && u[this.expando][M(f)]
             },
             access: function(u, f, p) {
                 return f === void 0 || f && typeof f == "string" && p === void 0 ? this.get(u, f) : (this.set(u, f, p), p !== void 0 ? p : f)
             },
             remove: function(u, f) {
                 var p, m = u[this.expando];
                 if (m !== void 0) {
                     if (f !== void 0)
-                        for (Array.isArray(f) ? f = f.map(D) : (f = D(f), f = f in m ? [f] : f.match(Ge) || []), p = f.length; p--;) delete m[f[p]];
+                        for (Array.isArray(f) ? f = f.map(M) : (f = M(f), f = f in m ? [f] : f.match(Ke) || []), p = f.length; p--;) delete m[f[p]];
                     (f === void 0 || h.isEmptyObject(m)) && (u.nodeType ? u[this.expando] = void 0 : delete u[this.expando])
                 }
             },
             hasData: function(u) {
                 var f = u[this.expando];
                 return f !== void 0 && !h.isEmptyObject(f)
             }
         };
         var X = new O,
             re = new O,
             le = /^(?:\{[\w\W]*\}|\[[\w\W]*\])$/,
-            Pe = /[A-Z]/g;
+            De = /[A-Z]/g;
 
-        function Me(u) {
+        function Pe(u) {
             return u === "true" ? !0 : u === "false" ? !1 : u === "null" ? null : u === +u + "" ? +u : le.test(u) ? JSON.parse(u) : u
         }
 
-        function Qe(u, f, p) {
+        function Ge(u, f, p) {
             var m;
             if (p === void 0 && u.nodeType === 1)
-                if (m = "data-" + f.replace(Pe, "-$&").toLowerCase(), p = u.getAttribute(m), typeof p == "string") {
+                if (m = "data-" + f.replace(De, "-$&").toLowerCase(), p = u.getAttribute(m), typeof p == "string") {
                     try {
-                        p = Me(p)
+                        p = Pe(p)
                     } catch {}
                     re.set(u, f, p)
                 } else p = void 0;
             return p
         }
         h.extend({
             hasData: function(u) {
@@ -21555,24 +21554,24 @@
             }
         }), h.fn.extend({
             data: function(u, f) {
                 var p, m, v, b = this[0],
                     E = b && b.attributes;
                 if (u === void 0) {
                     if (this.length && (v = re.get(b), b.nodeType === 1 && !X.get(b, "hasDataAttrs"))) {
-                        for (p = E.length; p--;) E[p] && (m = E[p].name, m.indexOf("data-") === 0 && (m = D(m.slice(5)), Qe(b, m, v[m])));
+                        for (p = E.length; p--;) E[p] && (m = E[p].name, m.indexOf("data-") === 0 && (m = M(m.slice(5)), Ge(b, m, v[m])));
                         X.set(b, "hasDataAttrs", !0)
                     }
                     return v
                 }
                 return typeof u == "object" ? this.each(function() {
                     re.set(this, u)
                 }) : Ae(this, function(L) {
                     var I;
-                    if (b && L === void 0) return I = re.get(b, u), I !== void 0 || (I = Qe(b, u), I !== void 0) ? I : void 0;
+                    if (b && L === void 0) return I = re.get(b, u), I !== void 0 || (I = Ge(b, u), I !== void 0) ? I : void 0;
                     this.each(function() {
                         re.set(this, u, L)
                     })
                 }, null, f, arguments.length > 1, null, !0)
             },
             removeData: function(u) {
                 return this.each(function() {
@@ -21628,40 +21627,40 @@
                         --m || v.resolveWith(b, [b])
                     };
                 for (typeof u != "string" && (f = u, u = void 0), u = u || "fx"; E--;) p = X.get(b[E], u + "queueHooks"), p && p.empty && (m++, p.empty.add(L));
                 return L(), v.promise(f)
             }
         });
         var Ft = /[+-]?(?:\d*\.|)\d+(?:[eE][+-]?\d+|)/.source,
-            Sn = new RegExp("^(?:([+-])=|)(" + Ft + ")([a-z%]*)$", "i"),
+            kn = new RegExp("^(?:([+-])=|)(" + Ft + ")([a-z%]*)$", "i"),
             ut = ["Top", "Right", "Bottom", "Left"],
-            Ai = _.documentElement,
+            Ai = w.documentElement,
             Li = function(u) {
                 return h.contains(u.ownerDocument, u)
             },
-            jl = {
+            Hl = {
                 composed: !0
             };
         Ai.getRootNode && (Li = function(u) {
-            return h.contains(u.ownerDocument, u) || u.getRootNode(jl) === u.ownerDocument
+            return h.contains(u.ownerDocument, u) || u.getRootNode(Hl) === u.ownerDocument
         });
         var Jr = function(u, f) {
             return u = f || u, u.style.display === "none" || u.style.display === "" && Li(u) && h.css(u, "display") === "none"
         };
 
-        function Zs(u, f, p, m) {
+        function Ks(u, f, p, m) {
             var v, b, E = 20,
                 L = m ? function() {
                     return m.cur()
                 } : function() {
                     return h.css(u, f, "")
                 },
                 I = L(),
                 B = p && p[3] || (h.cssNumber[f] ? "" : "px"),
-                q = u.nodeType && (h.cssNumber[f] || B !== "px" && +I) && Sn.exec(h.css(u, f));
+                q = u.nodeType && (h.cssNumber[f] || B !== "px" && +I) && kn.exec(h.css(u, f));
             if (q && q[3] !== B) {
                 for (I = I / 2, B = B || q[3], q = +I || 1; E--;) h.style(u, f, q + B), (1 - b) * (1 - (b = L() / I || .5)) <= 0 && (E = 0), q = q / b;
                 q = q * 2, h.style(u, f, q + B), p = p || []
             }
             return p && (q = +q || +I || 0, v = p[1] ? q + (p[1] + 1) * p[2] : +p[2], m && (m.unit = B, m.start = q, m.end = v)), v
         }
         var eo = {};
@@ -21688,125 +21687,125 @@
             toggle: function(u) {
                 return typeof u == "boolean" ? u ? this.show() : this.hide() : this.each(function() {
                     Jr(this) ? h(this).show() : h(this).hide()
                 })
             }
         });
         var to = /^(?:checkbox|radio)$/i,
-            Hl = /<([a-z][^\/\0>\x20\t\r\n\f]*)/i,
-            Bl = /^$|^module$|\/(?:java|ecma)script/i;
+            Bl = /<([a-z][^\/\0>\x20\t\r\n\f]*)/i,
+            Wl = /^$|^module$|\/(?:java|ecma)script/i;
         (function() {
-            var u = _.createDocumentFragment(),
-                f = u.appendChild(_.createElement("div")),
-                p = _.createElement("input");
-            p.setAttribute("type", "radio"), p.setAttribute("checked", "checked"), p.setAttribute("name", "t"), f.appendChild(p), w.checkClone = f.cloneNode(!0).cloneNode(!0).lastChild.checked, f.innerHTML = "<textarea>x</textarea>", w.noCloneChecked = !!f.cloneNode(!0).lastChild.defaultValue, f.innerHTML = "<option></option>", w.option = !!f.lastChild
+            var u = w.createDocumentFragment(),
+                f = u.appendChild(w.createElement("div")),
+                p = w.createElement("input");
+            p.setAttribute("type", "radio"), p.setAttribute("checked", "checked"), p.setAttribute("name", "t"), f.appendChild(p), _.checkClone = f.cloneNode(!0).cloneNode(!0).lastChild.checked, f.innerHTML = "<textarea>x</textarea>", _.noCloneChecked = !!f.cloneNode(!0).lastChild.defaultValue, f.innerHTML = "<option></option>", _.option = !!f.lastChild
         })();
         var un = {
             thead: [1, "<table>", "</table>"],
             col: [2, "<table><colgroup>", "</colgroup></table>"],
             tr: [2, "<table><tbody>", "</tbody></table>"],
             td: [3, "<table><tbody><tr>", "</tr></tbody></table>"],
             _default: [0, "", ""]
         };
-        un.tbody = un.tfoot = un.colgroup = un.caption = un.thead, un.th = un.td, w.option || (un.optgroup = un.option = [1, "<select multiple='multiple'>", "</select>"]);
+        un.tbody = un.tfoot = un.colgroup = un.caption = un.thead, un.th = un.td, _.option || (un.optgroup = un.option = [1, "<select multiple='multiple'>", "</select>"]);
 
         function Ct(u, f) {
             var p;
             return typeof u.getElementsByTagName < "u" ? p = u.getElementsByTagName(f || "*") : typeof u.querySelectorAll < "u" ? p = u.querySelectorAll(f || "*") : p = [], f === void 0 || f && he(u, f) ? h.merge([u], p) : p
         }
 
         function Qs(u, f) {
             for (var p = 0, m = u.length; p < m; p++) X.set(u[p], "globalEval", !f || X.get(f[p], "globalEval"))
         }
-        var Of = /<|&#?\w+;/;
+        var Mf = /<|&#?\w+;/;
 
-        function Ks(u, f, p, m, v) {
-            for (var b, E, L, I, B, q, ee = f.createDocumentFragment(), U = [], Z = 0, fe = u.length; Z < fe; Z++)
+        function Js(u, f, p, m, v) {
+            for (var b, E, L, I, B, q, ee = f.createDocumentFragment(), V = [], Z = 0, fe = u.length; Z < fe; Z++)
                 if (b = u[Z], b || b === 0)
-                    if (z(b) === "object") h.merge(U, b.nodeType ? [b] : b);
-                    else if (!Of.test(b)) U.push(f.createTextNode(b));
+                    if (z(b) === "object") h.merge(V, b.nodeType ? [b] : b);
+                    else if (!Mf.test(b)) V.push(f.createTextNode(b));
             else {
-                for (E = E || ee.appendChild(f.createElement("div")), L = (Hl.exec(b) || ["", ""])[1].toLowerCase(), I = un[L] || un._default, E.innerHTML = I[1] + h.htmlPrefilter(b) + I[2], q = I[0]; q--;) E = E.lastChild;
-                h.merge(U, E.childNodes), E = ee.firstChild, E.textContent = ""
+                for (E = E || ee.appendChild(f.createElement("div")), L = (Bl.exec(b) || ["", ""])[1].toLowerCase(), I = un[L] || un._default, E.innerHTML = I[1] + h.htmlPrefilter(b) + I[2], q = I[0]; q--;) E = E.lastChild;
+                h.merge(V, E.childNodes), E = ee.firstChild, E.textContent = ""
             }
-            for (ee.textContent = "", Z = 0; b = U[Z++];) {
+            for (ee.textContent = "", Z = 0; b = V[Z++];) {
                 if (m && h.inArray(b, m) > -1) {
                     v && v.push(b);
                     continue
                 }
                 if (B = Li(b), E = Ct(ee.appendChild(b), "script"), B && Qs(E), p)
-                    for (q = 0; b = E[q++];) Bl.test(b.type || "") && p.push(b)
+                    for (q = 0; b = E[q++];) Wl.test(b.type || "") && p.push(b)
             }
             return ee
         }
-        var Wl = /^key/,
-            Js = /^(?:mouse|pointer|contextmenu|drag|drop)|click/,
-            Vl = /^([^.]*)(?:\.(.+)|)/;
+        var Vl = /^key/,
+            ea = /^(?:mouse|pointer|contextmenu|drag|drop)|click/,
+            Ul = /^([^.]*)(?:\.(.+)|)/;
 
         function lr() {
             return !0
         }
 
         function ur() {
             return !1
         }
 
-        function Ul(u, f) {
-            return u === Af() == (f === "focus")
+        function $l(u, f) {
+            return u === Of() == (f === "focus")
         }
 
-        function Af() {
+        function Of() {
             try {
-                return _.activeElement
+                return w.activeElement
             } catch {}
         }
 
-        function ea(u, f, p, m, v, b) {
+        function ta(u, f, p, m, v, b) {
             var E, L;
             if (typeof f == "object") {
                 typeof p != "string" && (m = m || p, p = void 0);
-                for (L in f) ea(u, L, p, m, f[L], b);
+                for (L in f) ta(u, L, p, m, f[L], b);
                 return u
             }
             if (m == null && v == null ? (v = p, m = p = void 0) : v == null && (typeof p == "string" ? (v = m, m = void 0) : (v = m, m = p, p = void 0)), v === !1) v = ur;
             else if (!v) return u;
             return b === 1 && (E = v, v = function(I) {
                 return h().off(I), E.apply(this, arguments)
             }, v.guid = E.guid || (E.guid = h.guid++)), u.each(function() {
                 h.event.add(this, f, v, m, p)
             })
         }
         h.event = {
             global: {},
             add: function(u, f, p, m, v) {
-                var b, E, L, I, B, q, ee, U, Z, fe, _e, de = X.get(u);
+                var b, E, L, I, B, q, ee, V, Z, fe, _e, de = X.get(u);
                 if (H(u))
                     for (p.handler && (b = p, p = b.handler, v = b.selector), v && h.find.matchesSelector(Ai, v), p.guid || (p.guid = h.guid++), (I = de.events) || (I = de.events = Object.create(null)), (E = de.handle) || (E = de.handle = function(Tt) {
                             return typeof h < "u" && h.event.triggered !== Tt.type ? h.event.dispatch.apply(u, arguments) : void 0
-                        }), f = (f || "").match(Ge) || [""], B = f.length; B--;) L = Vl.exec(f[B]) || [], Z = _e = L[1], fe = (L[2] || "").split(".").sort(), Z && (ee = h.event.special[Z] || {}, Z = (v ? ee.delegateType : ee.bindType) || Z, ee = h.event.special[Z] || {}, q = h.extend({
+                        }), f = (f || "").match(Ke) || [""], B = f.length; B--;) L = Ul.exec(f[B]) || [], Z = _e = L[1], fe = (L[2] || "").split(".").sort(), Z && (ee = h.event.special[Z] || {}, Z = (v ? ee.delegateType : ee.bindType) || Z, ee = h.event.special[Z] || {}, q = h.extend({
                         type: Z,
                         origType: _e,
                         data: m,
                         handler: p,
                         guid: p.guid,
                         selector: v,
                         needsContext: v && h.expr.match.needsContext.test(v),
                         namespace: fe.join(".")
-                    }, b), (U = I[Z]) || (U = I[Z] = [], U.delegateCount = 0, (!ee.setup || ee.setup.call(u, m, fe, E) === !1) && u.addEventListener && u.addEventListener(Z, E)), ee.add && (ee.add.call(u, q), q.handler.guid || (q.handler.guid = p.guid)), v ? U.splice(U.delegateCount++, 0, q) : U.push(q), h.event.global[Z] = !0)
+                    }, b), (V = I[Z]) || (V = I[Z] = [], V.delegateCount = 0, (!ee.setup || ee.setup.call(u, m, fe, E) === !1) && u.addEventListener && u.addEventListener(Z, E)), ee.add && (ee.add.call(u, q), q.handler.guid || (q.handler.guid = p.guid)), v ? V.splice(V.delegateCount++, 0, q) : V.push(q), h.event.global[Z] = !0)
             },
             remove: function(u, f, p, m, v) {
-                var b, E, L, I, B, q, ee, U, Z, fe, _e, de = X.hasData(u) && X.get(u);
+                var b, E, L, I, B, q, ee, V, Z, fe, _e, de = X.hasData(u) && X.get(u);
                 if (!(!de || !(I = de.events))) {
-                    for (f = (f || "").match(Ge) || [""], B = f.length; B--;) {
-                        if (L = Vl.exec(f[B]) || [], Z = _e = L[1], fe = (L[2] || "").split(".").sort(), !Z) {
+                    for (f = (f || "").match(Ke) || [""], B = f.length; B--;) {
+                        if (L = Ul.exec(f[B]) || [], Z = _e = L[1], fe = (L[2] || "").split(".").sort(), !Z) {
                             for (Z in I) h.event.remove(u, Z + f[B], p, m, !0);
                             continue
                         }
-                        for (ee = h.event.special[Z] || {}, Z = (m ? ee.delegateType : ee.bindType) || Z, U = I[Z] || [], L = L[2] && new RegExp("(^|\\.)" + fe.join("\\.(?:.*\\.|)") + "(\\.|$)"), E = b = U.length; b--;) q = U[b], (v || _e === q.origType) && (!p || p.guid === q.guid) && (!L || L.test(q.namespace)) && (!m || m === q.selector || m === "**" && q.selector) && (U.splice(b, 1), q.selector && U.delegateCount--, ee.remove && ee.remove.call(u, q));
-                        E && !U.length && ((!ee.teardown || ee.teardown.call(u, fe, de.handle) === !1) && h.removeEvent(u, Z, de.handle), delete I[Z])
+                        for (ee = h.event.special[Z] || {}, Z = (m ? ee.delegateType : ee.bindType) || Z, V = I[Z] || [], L = L[2] && new RegExp("(^|\\.)" + fe.join("\\.(?:.*\\.|)") + "(\\.|$)"), E = b = V.length; b--;) q = V[b], (v || _e === q.origType) && (!p || p.guid === q.guid) && (!L || L.test(q.namespace)) && (!m || m === q.selector || m === "**" && q.selector) && (V.splice(b, 1), q.selector && V.delegateCount--, ee.remove && ee.remove.call(u, q));
+                        E && !V.length && ((!ee.teardown || ee.teardown.call(u, fe, de.handle) === !1) && h.removeEvent(u, Z, de.handle), delete I[Z])
                     }
                     h.isEmptyObject(I) && X.remove(u, "handle events")
                 }
             },
             dispatch: function(u) {
                 var f, p, m, v, b, E, L = new Array(arguments.length),
                     I = h.event.fix(u),
@@ -21840,15 +21839,15 @@
                     handlers: f.slice(I)
                 }), L
             },
             addProp: function(u, f) {
                 Object.defineProperty(h.Event.prototype, u, {
                     enumerable: !0,
                     configurable: !0,
-                    get: S(f) ? function() {
+                    get: C(f) ? function() {
                         if (this.originalEvent) return f(this.originalEvent)
                     } : function() {
                         if (this.originalEvent) return this.originalEvent[u]
                     },
                     set: function(p) {
                         Object.defineProperty(this, u, {
                             enumerable: !0,
@@ -21958,23 +21957,23 @@
             screenX: !0,
             screenY: !0,
             targetTouches: !0,
             toElement: !0,
             touches: !0,
             which: function(u) {
                 var f = u.button;
-                return u.which == null && Wl.test(u.type) ? u.charCode != null ? u.charCode : u.keyCode : !u.which && f !== void 0 && Js.test(u.type) ? f & 1 ? 1 : f & 2 ? 3 : f & 4 ? 2 : 0 : u.which
+                return u.which == null && Vl.test(u.type) ? u.charCode != null ? u.charCode : u.keyCode : !u.which && f !== void 0 && ea.test(u.type) ? f & 1 ? 1 : f & 2 ? 3 : f & 4 ? 2 : 0 : u.which
             }
         }, h.event.addProp), h.each({
             focus: "focusin",
             blur: "focusout"
         }, function(u, f) {
             h.event.special[u] = {
                 setup: function() {
-                    return $o(this, u, Ul), !1
+                    return $o(this, u, $l), !1
                 },
                 trigger: function() {
                     return $o(this, u), !0
                 },
                 delegateType: f
             }
         }), h.each({
@@ -21991,103 +21990,103 @@
                         b = p.relatedTarget,
                         E = p.handleObj;
                     return (!b || b !== v && !h.contains(v, b)) && (p.type = E.origType, m = E.handler.apply(this, arguments), p.type = f), m
                 }
             }
         }), h.fn.extend({
             on: function(u, f, p, m) {
-                return ea(this, u, f, p, m)
+                return ta(this, u, f, p, m)
             },
             one: function(u, f, p, m) {
-                return ea(this, u, f, p, m, 1)
+                return ta(this, u, f, p, m, 1)
             },
             off: function(u, f, p) {
                 var m, v;
                 if (u && u.preventDefault && u.handleObj) return m = u.handleObj, h(u.delegateTarget).off(m.namespace ? m.origType + "." + m.namespace : m.origType, m.selector, m.handler), this;
                 if (typeof u == "object") {
                     for (v in u) this.off(v, f, u[v]);
                     return this
                 }
                 return (f === !1 || typeof f == "function") && (p = f, f = void 0), p === !1 && (p = ur), this.each(function() {
                     h.event.remove(this, u, p, f)
                 })
             }
         });
         var Yo = /<script|<style|<link/i,
-            Lf = /checked\s*(?:[^=]|=\s*.checked.)/i,
-            Rf = /^\s*<!(?:\[CDATA\[|--)|(?:\]\]|--)>\s*$/g;
+            Af = /checked\s*(?:[^=]|=\s*.checked.)/i,
+            Lf = /^\s*<!(?:\[CDATA\[|--)|(?:\]\]|--)>\s*$/g;
 
-        function ta(u, f) {
+        function na(u, f) {
             return he(u, "table") && he(f.nodeType !== 11 ? f : f.firstChild, "tr") && h(u).children("tbody")[0] || u
         }
 
-        function na(u) {
+        function ia(u) {
             return u.type = (u.getAttribute("type") !== null) + "/" + u.type, u
         }
 
-        function If(u) {
+        function Rf(u) {
             return (u.type || "").slice(0, 5) === "true/" ? u.type = u.type.slice(5) : u.removeAttribute("type"), u
         }
 
-        function ia(u, f) {
+        function ra(u, f) {
             var p, m, v, b, E, L, I;
             if (f.nodeType === 1) {
                 if (X.hasData(u) && (b = X.get(u), I = b.events, I)) {
                     X.remove(f, "handle events");
                     for (v in I)
                         for (p = 0, m = I[v].length; p < m; p++) h.event.add(f, v, I[v][p])
                 }
                 re.hasData(u) && (E = re.access(u), L = h.extend({}, E), re.set(f, L))
             }
         }
 
-        function Nf(u, f) {
+        function If(u, f) {
             var p = f.nodeName.toLowerCase();
             p === "input" && to.test(u.type) ? f.checked = u.checked : (p === "input" || p === "textarea") && (f.defaultValue = u.defaultValue)
         }
 
         function Ri(u, f, p, m) {
             f = s(f);
             var v, b, E, L, I, B, q = 0,
                 ee = u.length,
-                U = ee - 1,
+                V = ee - 1,
                 Z = f[0],
-                fe = S(Z);
-            if (fe || ee > 1 && typeof Z == "string" && !w.checkClone && Lf.test(Z)) return u.each(function(_e) {
+                fe = C(Z);
+            if (fe || ee > 1 && typeof Z == "string" && !_.checkClone && Af.test(Z)) return u.each(function(_e) {
                 var de = u.eq(_e);
                 fe && (f[0] = Z.call(this, _e, de.html())), Ri(de, f, p, m)
             });
-            if (ee && (v = Ks(f, u[0].ownerDocument, !1, u, m), b = v.firstChild, v.childNodes.length === 1 && (v = b), b || m)) {
-                for (E = h.map(Ct(v, "script"), na), L = E.length; q < ee; q++) I = v, q !== U && (I = h.clone(I, !0, !0), L && h.merge(E, Ct(I, "script"))), p.call(u[q], I, q);
+            if (ee && (v = Js(f, u[0].ownerDocument, !1, u, m), b = v.firstChild, v.childNodes.length === 1 && (v = b), b || m)) {
+                for (E = h.map(Ct(v, "script"), ia), L = E.length; q < ee; q++) I = v, q !== V && (I = h.clone(I, !0, !0), L && h.merge(E, Ct(I, "script"))), p.call(u[q], I, q);
                 if (L)
-                    for (B = E[E.length - 1].ownerDocument, h.map(E, If), q = 0; q < L; q++) I = E[q], Bl.test(I.type || "") && !X.access(I, "globalEval") && h.contains(B, I) && (I.src && (I.type || "").toLowerCase() !== "module" ? h._evalUrl && !I.noModule && h._evalUrl(I.src, {
+                    for (B = E[E.length - 1].ownerDocument, h.map(E, Rf), q = 0; q < L; q++) I = E[q], Wl.test(I.type || "") && !X.access(I, "globalEval") && h.contains(B, I) && (I.src && (I.type || "").toLowerCase() !== "module" ? h._evalUrl && !I.noModule && h._evalUrl(I.src, {
                         nonce: I.nonce || I.getAttribute("nonce")
-                    }, B) : M(I.textContent.replace(Rf, ""), I, B))
+                    }, B) : P(I.textContent.replace(Lf, ""), I, B))
             }
             return u
         }
 
-        function ra(u, f, p) {
+        function oa(u, f, p) {
             for (var m, v = f ? h.filter(f, u) : u, b = 0;
                 (m = v[b]) != null; b++) !p && m.nodeType === 1 && h.cleanData(Ct(m)), m.parentNode && (p && Li(m) && Qs(Ct(m, "script")), m.parentNode.removeChild(m));
             return u
         }
         h.extend({
             htmlPrefilter: function(u) {
                 return u
             },
             clone: function(u, f, p) {
                 var m, v, b, E, L = u.cloneNode(!0),
                     I = Li(u);
-                if (!w.noCloneChecked && (u.nodeType === 1 || u.nodeType === 11) && !h.isXMLDoc(u))
-                    for (E = Ct(L), b = Ct(u), m = 0, v = b.length; m < v; m++) Nf(b[m], E[m]);
+                if (!_.noCloneChecked && (u.nodeType === 1 || u.nodeType === 11) && !h.isXMLDoc(u))
+                    for (E = Ct(L), b = Ct(u), m = 0, v = b.length; m < v; m++) If(b[m], E[m]);
                 if (f)
                     if (p)
-                        for (b = b || Ct(u), E = E || Ct(L), m = 0, v = b.length; m < v; m++) ia(b[m], E[m]);
-                    else ia(u, L);
+                        for (b = b || Ct(u), E = E || Ct(L), m = 0, v = b.length; m < v; m++) ra(b[m], E[m]);
+                    else ra(u, L);
                 return E = Ct(L, "script"), E.length > 0 && Qs(E, !I && Ct(u, "script")), L
             },
             cleanData: function(u) {
                 for (var f, p, m, v = h.event.special, b = 0;
                     (p = u[b]) !== void 0; b++)
                     if (H(p)) {
                         if (f = p[X.expando]) {
@@ -22096,38 +22095,38 @@
                             p[X.expando] = void 0
                         }
                         p[re.expando] && (p[re.expando] = void 0)
                     }
             }
         }), h.fn.extend({
             detach: function(u) {
-                return ra(this, u, !0)
+                return oa(this, u, !0)
             },
             remove: function(u) {
-                return ra(this, u)
+                return oa(this, u)
             },
             text: function(u) {
                 return Ae(this, function(f) {
                     return f === void 0 ? h.text(this) : this.empty().each(function() {
                         (this.nodeType === 1 || this.nodeType === 11 || this.nodeType === 9) && (this.textContent = f)
                     })
                 }, null, u, arguments.length)
             },
             append: function() {
                 return Ri(this, arguments, function(u) {
                     if (this.nodeType === 1 || this.nodeType === 11 || this.nodeType === 9) {
-                        var f = ta(this, u);
+                        var f = na(this, u);
                         f.appendChild(u)
                     }
                 })
             },
             prepend: function() {
                 return Ri(this, arguments, function(u) {
                     if (this.nodeType === 1 || this.nodeType === 11 || this.nodeType === 9) {
-                        var f = ta(this, u);
+                        var f = na(this, u);
                         f.insertBefore(u, f.firstChild)
                     }
                 })
             },
             before: function() {
                 return Ri(this, arguments, function(u) {
                     this.parentNode && this.parentNode.insertBefore(u, this)
@@ -22150,15 +22149,15 @@
             },
             html: function(u) {
                 return Ae(this, function(f) {
                     var p = this[0] || {},
                         m = 0,
                         v = this.length;
                     if (f === void 0 && p.nodeType === 1) return p.innerHTML;
-                    if (typeof f == "string" && !Yo.test(f) && !un[(Hl.exec(f) || ["", ""])[1].toLowerCase()]) {
+                    if (typeof f == "string" && !Yo.test(f) && !un[(Bl.exec(f) || ["", ""])[1].toLowerCase()]) {
                         f = h.htmlPrefilter(f);
                         try {
                             for (; m < v; m++) p = this[m] || {}, p.nodeType === 1 && (h.cleanData(Ct(p, !1)), p.innerHTML = f);
                             p = 0
                         } catch {}
                     }
                     p && this.empty().append(f)
@@ -22204,17 +22203,17 @@
                     p = q.top !== "1%", L = f(q.marginLeft) === 12, B.style.right = "60%", b = f(q.right) === 36, m = f(q.width) === 36, B.style.position = "absolute", v = f(B.offsetWidth / 3) === 12, Ai.removeChild(I), B = null
                 }
             }
 
             function f(q) {
                 return Math.round(parseFloat(q))
             }
-            var p, m, v, b, E, L, I = _.createElement("div"),
-                B = _.createElement("div");
-            B.style && (B.style.backgroundClip = "content-box", B.cloneNode(!0).style.backgroundClip = "", w.clearCloneStyle = B.style.backgroundClip === "content-box", h.extend(w, {
+            var p, m, v, b, E, L, I = w.createElement("div"),
+                B = w.createElement("div");
+            B.style && (B.style.backgroundClip = "content-box", B.cloneNode(!0).style.backgroundClip = "", _.clearCloneStyle = B.style.backgroundClip === "content-box", h.extend(_, {
                 boxSizingReliable: function() {
                     return u(), m
                 },
                 pixelBoxStyles: function() {
                     return u(), b
                 },
                 pixelPosition: function() {
@@ -22223,94 +22222,94 @@
                 reliableMarginLeft: function() {
                     return u(), L
                 },
                 scrollboxSize: function() {
                     return u(), v
                 },
                 reliableTrDimensions: function() {
-                    var q, ee, U, Z;
-                    return E == null && (q = _.createElement("table"), ee = _.createElement("tr"), U = _.createElement("div"), q.style.cssText = "position:absolute;left:-11111px", ee.style.height = "1px", U.style.height = "9px", Ai.appendChild(q).appendChild(ee).appendChild(U), Z = e.getComputedStyle(ee), E = parseInt(Z.height) > 3, Ai.removeChild(q)), E
+                    var q, ee, V, Z;
+                    return E == null && (q = w.createElement("table"), ee = w.createElement("tr"), V = w.createElement("div"), q.style.cssText = "position:absolute;left:-11111px", ee.style.height = "1px", V.style.height = "9px", Ai.appendChild(q).appendChild(ee).appendChild(V), Z = e.getComputedStyle(ee), E = parseInt(Z.height) > 3, Ai.removeChild(q)), E
                 }
             }))
         })();
 
-        function Qn(u, f, p) {
+        function Gn(u, f, p) {
             var m, v, b, E, L = u.style;
-            return p = p || no(u), p && (E = p.getPropertyValue(f) || p[f], E === "" && !Li(u) && (E = h.style(u, f)), !w.pixelBoxStyles() && Xo.test(E) && Ii.test(f) && (m = L.width, v = L.minWidth, b = L.maxWidth, L.minWidth = L.maxWidth = L.width = E, E = p.width, L.width = m, L.minWidth = v, L.maxWidth = b)), E !== void 0 ? E + "" : E
+            return p = p || no(u), p && (E = p.getPropertyValue(f) || p[f], E === "" && !Li(u) && (E = h.style(u, f)), !_.pixelBoxStyles() && Xo.test(E) && Ii.test(f) && (m = L.width, v = L.minWidth, b = L.maxWidth, L.minWidth = L.maxWidth = L.width = E, E = p.width, L.width = m, L.minWidth = v, L.maxWidth = b)), E !== void 0 ? E + "" : E
         }
 
         function cr(u, f) {
             return {
                 get: function() {
                     if (u()) {
                         delete this.get;
                         return
                     }
                     return (this.get = f).apply(this, arguments)
                 }
             }
         }
         var io = ["Webkit", "Moz", "ms"],
-            Zo = _.createElement("div").style,
-            $l = {};
+            Zo = w.createElement("div").style,
+            Yl = {};
 
-        function zf(u) {
+        function Nf(u) {
             for (var f = u[0].toUpperCase() + u.slice(1), p = io.length; p--;)
                 if (u = io[p] + f, u in Zo) return u
         }
 
         function fr(u) {
-            var f = h.cssProps[u] || $l[u];
-            return f || (u in Zo ? u : $l[u] = zf(u) || u)
+            var f = h.cssProps[u] || Yl[u];
+            return f || (u in Zo ? u : Yl[u] = Nf(u) || u)
         }
         var cn = /^(none|table(?!-c[ea]).+)/,
             Ni = /^--/,
             yi = {
                 position: "absolute",
                 visibility: "hidden",
                 display: "block"
             },
             jn = {
                 letterSpacing: "0",
                 fontWeight: "400"
             };
 
         function dr(u, f, p) {
-            var m = Sn.exec(f);
+            var m = kn.exec(f);
             return m ? Math.max(0, m[2] - (p || 0)) + (m[3] || "px") : f
         }
 
         function fn(u, f, p, m, v, b) {
             var E = f === "width" ? 1 : 0,
                 L = 0,
                 I = 0;
             if (p === (m ? "border" : "content")) return 0;
             for (; E < 4; E += 2) p === "margin" && (I += h.css(u, p + ut[E], !0, v)), m ? (p === "content" && (I -= h.css(u, "padding" + ut[E], !0, v)), p !== "margin" && (I -= h.css(u, "border" + ut[E] + "Width", !0, v))) : (I += h.css(u, "padding" + ut[E], !0, v), p !== "padding" ? I += h.css(u, "border" + ut[E] + "Width", !0, v) : L += h.css(u, "border" + ut[E] + "Width", !0, v));
             return !m && b >= 0 && (I += Math.max(0, Math.ceil(u["offset" + f[0].toUpperCase() + f.slice(1)] - b - I - L - .5)) || 0), I
         }
 
         function Hn(u, f, p) {
             var m = no(u),
-                v = !w.boxSizingReliable() || p,
+                v = !_.boxSizingReliable() || p,
                 b = v && h.css(u, "boxSizing", !1, m) === "border-box",
                 E = b,
-                L = Qn(u, f, m),
+                L = Gn(u, f, m),
                 I = "offset" + f[0].toUpperCase() + f.slice(1);
             if (Xo.test(L)) {
                 if (!p) return L;
                 L = "auto"
             }
-            return (!w.boxSizingReliable() && b || !w.reliableTrDimensions() && he(u, "tr") || L === "auto" || !parseFloat(L) && h.css(u, "display", !1, m) === "inline") && u.getClientRects().length && (b = h.css(u, "boxSizing", !1, m) === "border-box", E = I in u, E && (L = u[I])), L = parseFloat(L) || 0, L + fn(u, f, p || (b ? "border" : "content"), E, m, L) + "px"
+            return (!_.boxSizingReliable() && b || !_.reliableTrDimensions() && he(u, "tr") || L === "auto" || !parseFloat(L) && h.css(u, "display", !1, m) === "inline") && u.getClientRects().length && (b = h.css(u, "boxSizing", !1, m) === "border-box", E = I in u, E && (L = u[I])), L = parseFloat(L) || 0, L + fn(u, f, p || (b ? "border" : "content"), E, m, L) + "px"
         }
         h.extend({
             cssHooks: {
                 opacity: {
                     get: function(u, f) {
                         if (f) {
-                            var p = Qn(u, "opacity");
+                            var p = Gn(u, "opacity");
                             return p === "" ? "1" : p
                         }
                     }
                 }
             },
             cssNumber: {
                 animationIterationCount: !0,
@@ -22333,46 +22332,46 @@
                 widows: !0,
                 zIndex: !0,
                 zoom: !0
             },
             cssProps: {},
             style: function(u, f, p, m) {
                 if (!(!u || u.nodeType === 3 || u.nodeType === 8 || !u.style)) {
-                    var v, b, E, L = D(f),
+                    var v, b, E, L = M(f),
                         I = Ni.test(f),
                         B = u.style;
                     if (I || (f = fr(L)), E = h.cssHooks[f] || h.cssHooks[L], p !== void 0) {
-                        if (b = typeof p, b === "string" && (v = Sn.exec(p)) && v[1] && (p = Zs(u, f, v), b = "number"), p == null || p !== p) return;
-                        b === "number" && !I && (p += v && v[3] || (h.cssNumber[L] ? "" : "px")), !w.clearCloneStyle && p === "" && f.indexOf("background") === 0 && (B[f] = "inherit"), (!E || !("set" in E) || (p = E.set(u, p, m)) !== void 0) && (I ? B.setProperty(f, p) : B[f] = p)
+                        if (b = typeof p, b === "string" && (v = kn.exec(p)) && v[1] && (p = Ks(u, f, v), b = "number"), p == null || p !== p) return;
+                        b === "number" && !I && (p += v && v[3] || (h.cssNumber[L] ? "" : "px")), !_.clearCloneStyle && p === "" && f.indexOf("background") === 0 && (B[f] = "inherit"), (!E || !("set" in E) || (p = E.set(u, p, m)) !== void 0) && (I ? B.setProperty(f, p) : B[f] = p)
                     } else return E && "get" in E && (v = E.get(u, !1, m)) !== void 0 ? v : B[f]
                 }
             },
             css: function(u, f, p, m) {
-                var v, b, E, L = D(f),
+                var v, b, E, L = M(f),
                     I = Ni.test(f);
-                return I || (f = fr(L)), E = h.cssHooks[f] || h.cssHooks[L], E && "get" in E && (v = E.get(u, !0, p)), v === void 0 && (v = Qn(u, f, m)), v === "normal" && f in jn && (v = jn[f]), p === "" || p ? (b = parseFloat(v), p === !0 || isFinite(b) ? b || 0 : v) : v
+                return I || (f = fr(L)), E = h.cssHooks[f] || h.cssHooks[L], E && "get" in E && (v = E.get(u, !0, p)), v === void 0 && (v = Gn(u, f, m)), v === "normal" && f in jn && (v = jn[f]), p === "" || p ? (b = parseFloat(v), p === !0 || isFinite(b) ? b || 0 : v) : v
             }
         }), h.each(["height", "width"], function(u, f) {
             h.cssHooks[f] = {
                 get: function(p, m, v) {
                     if (m) return cn.test(h.css(p, "display")) && (!p.getClientRects().length || !p.getBoundingClientRect().width) ? qo(p, yi, function() {
                         return Hn(p, f, v)
                     }) : Hn(p, f, v)
                 },
                 set: function(p, m, v) {
                     var b, E = no(p),
-                        L = !w.scrollboxSize() && E.position === "absolute",
+                        L = !_.scrollboxSize() && E.position === "absolute",
                         I = L || v,
                         B = I && h.css(p, "boxSizing", !1, E) === "border-box",
                         q = v ? fn(p, f, v, B, E) : 0;
-                    return B && L && (q -= Math.ceil(p["offset" + f[0].toUpperCase() + f.slice(1)] - parseFloat(E[f]) - fn(p, f, "border", !1, E) - .5)), q && (b = Sn.exec(m)) && (b[3] || "px") !== "px" && (p.style[f] = m, m = h.css(p, f)), dr(p, m, q)
+                    return B && L && (q -= Math.ceil(p["offset" + f[0].toUpperCase() + f.slice(1)] - parseFloat(E[f]) - fn(p, f, "border", !1, E) - .5)), q && (b = kn.exec(m)) && (b[3] || "px") !== "px" && (p.style[f] = m, m = h.css(p, f)), dr(p, m, q)
                 }
             }
-        }), h.cssHooks.marginLeft = cr(w.reliableMarginLeft, function(u, f) {
-            if (f) return (parseFloat(Qn(u, "marginLeft")) || u.getBoundingClientRect().left - qo(u, {
+        }), h.cssHooks.marginLeft = cr(_.reliableMarginLeft, function(u, f) {
+            if (f) return (parseFloat(Gn(u, "marginLeft")) || u.getBoundingClientRect().left - qo(u, {
                 marginLeft: 0
             }, function() {
                 return u.getBoundingClientRect().left
             })) + "px"
         }), h.each({
             margin: "",
             padding: "",
@@ -22434,151 +22433,151 @@
             },
             swing: function(u) {
                 return .5 - Math.cos(u * Math.PI) / 2
             },
             _default: "swing"
         }, h.fx = jt.prototype.init, h.fx.step = {};
         var zi, Fi, Cn = /^(?:toggle|show|hide)$/,
-            Go = /queueHooks$/;
+            Ko = /queueHooks$/;
 
         function ro() {
-            Fi && (_.hidden === !1 && e.requestAnimationFrame ? e.requestAnimationFrame(ro) : e.setTimeout(ro, h.fx.interval), h.fx.tick())
+            Fi && (w.hidden === !1 && e.requestAnimationFrame ? e.requestAnimationFrame(ro) : e.setTimeout(ro, h.fx.interval), h.fx.tick())
         }
 
-        function Qo() {
+        function Go() {
             return e.setTimeout(function() {
                 zi = void 0
             }), zi = Date.now()
         }
 
         function hr(u, f) {
             var p, m = 0,
                 v = {
                     height: u
                 };
             for (f = f ? 1 : 0; m < 4; m += 2 - f) p = ut[m], v["margin" + p] = v["padding" + p] = u;
             return f && (v.opacity = v.width = u), v
         }
 
-        function Ko(u, f, p) {
+        function Qo(u, f, p) {
             for (var m, v = (En.tweeners[f] || []).concat(En.tweeners["*"]), b = 0, E = v.length; b < E; b++)
                 if (m = v[b].call(p, f, u)) return m
         }
 
         function Jo(u, f, p) {
             var m, v, b, E, L, I, B, q, ee = "width" in f || "height" in f,
-                U = this,
+                V = this,
                 Z = {},
                 fe = u.style,
                 _e = u.nodeType && Jr(u),
                 de = X.get(u, "fxshow");
             p.queue || (E = h._queueHooks(u, "fx"), E.unqueued == null && (E.unqueued = 0, L = E.empty.fire, E.empty.fire = function() {
                 E.unqueued || L()
-            }), E.unqueued++, U.always(function() {
-                U.always(function() {
+            }), E.unqueued++, V.always(function() {
+                V.always(function() {
                     E.unqueued--, h.queue(u, "fx").length || E.empty.fire()
                 })
             }));
             for (m in f)
                 if (v = f[m], Cn.test(v)) {
                     if (delete f[m], b = b || v === "toggle", v === (_e ? "hide" : "show"))
                         if (v === "show" && de && de[m] !== void 0) _e = !0;
                         else continue;
                     Z[m] = de && de[m] || h.style(u, m)
                 } if (I = !h.isEmptyObject(f), !(!I && h.isEmptyObject(Z))) {
-                ee && u.nodeType === 1 && (p.overflow = [fe.overflow, fe.overflowX, fe.overflowY], B = de && de.display, B == null && (B = X.get(u, "display")), q = h.css(u, "display"), q === "none" && (B ? q = B : (ar([u], !0), B = u.style.display || B, q = h.css(u, "display"), ar([u]))), (q === "inline" || q === "inline-block" && B != null) && h.css(u, "float") === "none" && (I || (U.done(function() {
+                ee && u.nodeType === 1 && (p.overflow = [fe.overflow, fe.overflowX, fe.overflowY], B = de && de.display, B == null && (B = X.get(u, "display")), q = h.css(u, "display"), q === "none" && (B ? q = B : (ar([u], !0), B = u.style.display || B, q = h.css(u, "display"), ar([u]))), (q === "inline" || q === "inline-block" && B != null) && h.css(u, "float") === "none" && (I || (V.done(function() {
                     fe.display = B
-                }), B == null && (q = fe.display, B = q === "none" ? "" : q)), fe.display = "inline-block")), p.overflow && (fe.overflow = "hidden", U.always(function() {
+                }), B == null && (q = fe.display, B = q === "none" ? "" : q)), fe.display = "inline-block")), p.overflow && (fe.overflow = "hidden", V.always(function() {
                     fe.overflow = p.overflow[0], fe.overflowX = p.overflow[1], fe.overflowY = p.overflow[2]
                 })), I = !1;
                 for (m in Z) I || (de ? "hidden" in de && (_e = de.hidden) : de = X.access(u, "fxshow", {
                     display: B
-                }), b && (de.hidden = !_e), _e && ar([u], !0), U.done(function() {
+                }), b && (de.hidden = !_e), _e && ar([u], !0), V.done(function() {
                     _e || ar([u]), X.remove(u, "fxshow");
                     for (m in Z) h.style(u, m, Z[m])
-                })), I = Ko(_e ? de[m] : 0, m, U), m in de || (de[m] = I.start, _e && (I.end = I.start, I.start = 0))
+                })), I = Qo(_e ? de[m] : 0, m, V), m in de || (de[m] = I.start, _e && (I.end = I.start, I.start = 0))
             }
         }
 
-        function Kn(u, f) {
+        function Qn(u, f) {
             var p, m, v, b, E;
             for (p in u)
-                if (m = D(p), v = f[m], b = u[p], Array.isArray(b) && (v = b[1], b = u[p] = b[0]), p !== m && (u[m] = b, delete u[p]), E = h.cssHooks[m], E && "expand" in E) {
+                if (m = M(p), v = f[m], b = u[p], Array.isArray(b) && (v = b[1], b = u[p] = b[0]), p !== m && (u[m] = b, delete u[p]), E = h.cssHooks[m], E && "expand" in E) {
                     b = E.expand(b), delete u[m];
                     for (p in b) p in u || (u[p] = b[p], f[p] = v)
                 } else f[m] = v
         }
 
         function En(u, f, p) {
             var m, v, b = 0,
                 E = En.prefilters.length,
                 L = h.Deferred().always(function() {
                     delete I.elem
                 }),
                 I = function() {
                     if (v) return !1;
-                    for (var ee = zi || Qo(), U = Math.max(0, B.startTime + B.duration - ee), Z = U / B.duration || 0, fe = 1 - Z, _e = 0, de = B.tweens.length; _e < de; _e++) B.tweens[_e].run(fe);
-                    return L.notifyWith(u, [B, fe, U]), fe < 1 && de ? U : (de || L.notifyWith(u, [B, 1, 0]), L.resolveWith(u, [B]), !1)
+                    for (var ee = zi || Go(), V = Math.max(0, B.startTime + B.duration - ee), Z = V / B.duration || 0, fe = 1 - Z, _e = 0, de = B.tweens.length; _e < de; _e++) B.tweens[_e].run(fe);
+                    return L.notifyWith(u, [B, fe, V]), fe < 1 && de ? V : (de || L.notifyWith(u, [B, 1, 0]), L.resolveWith(u, [B]), !1)
                 },
                 B = L.promise({
                     elem: u,
                     props: h.extend({}, f),
                     opts: h.extend(!0, {
                         specialEasing: {},
                         easing: h.easing._default
                     }, p),
                     originalProperties: f,
                     originalOptions: p,
-                    startTime: zi || Qo(),
+                    startTime: zi || Go(),
                     duration: p.duration,
                     tweens: [],
-                    createTween: function(ee, U) {
-                        var Z = h.Tween(u, B.opts, ee, U, B.opts.specialEasing[ee] || B.opts.easing);
+                    createTween: function(ee, V) {
+                        var Z = h.Tween(u, B.opts, ee, V, B.opts.specialEasing[ee] || B.opts.easing);
                         return B.tweens.push(Z), Z
                     },
                     stop: function(ee) {
-                        var U = 0,
+                        var V = 0,
                             Z = ee ? B.tweens.length : 0;
                         if (v) return this;
-                        for (v = !0; U < Z; U++) B.tweens[U].run(1);
+                        for (v = !0; V < Z; V++) B.tweens[V].run(1);
                         return ee ? (L.notifyWith(u, [B, 1, 0]), L.resolveWith(u, [B, ee])) : L.rejectWith(u, [B, ee]), this
                     }
                 }),
                 q = B.props;
-            for (Kn(q, B.opts.specialEasing); b < E; b++)
-                if (m = En.prefilters[b].call(B, u, q, B.opts), m) return S(m.stop) && (h._queueHooks(B.elem, B.opts.queue).stop = m.stop.bind(m)), m;
-            return h.map(q, Ko, B), S(B.opts.start) && B.opts.start.call(u, B), B.progress(B.opts.progress).done(B.opts.done, B.opts.complete).fail(B.opts.fail).always(B.opts.always), h.fx.timer(h.extend(I, {
+            for (Qn(q, B.opts.specialEasing); b < E; b++)
+                if (m = En.prefilters[b].call(B, u, q, B.opts), m) return C(m.stop) && (h._queueHooks(B.elem, B.opts.queue).stop = m.stop.bind(m)), m;
+            return h.map(q, Qo, B), C(B.opts.start) && B.opts.start.call(u, B), B.progress(B.opts.progress).done(B.opts.done, B.opts.complete).fail(B.opts.fail).always(B.opts.always), h.fx.timer(h.extend(I, {
                 elem: u,
                 anim: B,
                 queue: B.opts.queue
             })), B
         }
         h.Animation = h.extend(En, {
                 tweeners: {
                     "*": [function(u, f) {
                         var p = this.createTween(u, f);
-                        return Zs(p.elem, u, Sn.exec(f), p), p
+                        return Ks(p.elem, u, kn.exec(f), p), p
                     }]
                 },
                 tweener: function(u, f) {
-                    S(u) ? (f = u, u = ["*"]) : u = u.match(Ge);
+                    C(u) ? (f = u, u = ["*"]) : u = u.match(Ke);
                     for (var p, m = 0, v = u.length; m < v; m++) p = u[m], En.tweeners[p] = En.tweeners[p] || [], En.tweeners[p].unshift(f)
                 },
                 prefilters: [Jo],
                 prefilter: function(u, f) {
                     f ? En.prefilters.unshift(u) : En.prefilters.push(u)
                 }
             }), h.speed = function(u, f, p) {
                 var m = u && typeof u == "object" ? h.extend({}, u) : {
-                    complete: p || !p && f || S(u) && u,
+                    complete: p || !p && f || C(u) && u,
                     duration: u,
-                    easing: p && f || f && !S(f) && f
+                    easing: p && f || f && !C(f) && f
                 };
                 return h.fx.off ? m.duration = 0 : typeof m.duration != "number" && (m.duration in h.fx.speeds ? m.duration = h.fx.speeds[m.duration] : m.duration = h.fx.speeds._default), (m.queue == null || m.queue === !0) && (m.queue = "fx"), m.old = m.complete, m.complete = function() {
-                    S(m.old) && m.old.call(this), m.queue && h.dequeue(this, m.queue)
+                    C(m.old) && m.old.call(this), m.queue && h.dequeue(this, m.queue)
                 }, m
             }, h.fn.extend({
                 fadeTo: function(u, f, p, m) {
                     return this.filter(Jr).css("opacity", 0).show().end().animate({
                         opacity: f
                     }, u, p, m)
                 },
@@ -22599,15 +22598,15 @@
                     return typeof u != "string" && (p = f, f = u, u = void 0), f && this.queue(u || "fx", []), this.each(function() {
                         var v = !0,
                             b = u != null && u + "queueHooks",
                             E = h.timers,
                             L = X.get(this);
                         if (b) L[b] && L[b].stop && m(L[b]);
                         else
-                            for (b in L) L[b] && L[b].stop && Go.test(b) && m(L[b]);
+                            for (b in L) L[b] && L[b].stop && Ko.test(b) && m(L[b]);
                         for (b = E.length; b--;) E[b].elem === this && (u == null || E[b].queue === u) && (E[b].anim.stop(p), v = !1, E.splice(b, 1));
                         (v || !p) && h.dequeue(this, u)
                     })
                 },
                 finish: function(u) {
                     return u !== !1 && (u = u || "fx"), this.each(function() {
                         var f, p = X.get(this),
@@ -22662,73 +22661,73 @@
                     var v = e.setTimeout(p, u);
                     m.stop = function() {
                         e.clearTimeout(v)
                     }
                 })
             },
             function() {
-                var u = _.createElement("input"),
-                    f = _.createElement("select"),
-                    p = f.appendChild(_.createElement("option"));
-                u.type = "checkbox", w.checkOn = u.value !== "", w.optSelected = p.selected, u = _.createElement("input"), u.value = "t", u.type = "radio", w.radioValue = u.value === "t"
+                var u = w.createElement("input"),
+                    f = w.createElement("select"),
+                    p = f.appendChild(w.createElement("option"));
+                u.type = "checkbox", _.checkOn = u.value !== "", _.optSelected = p.selected, u = w.createElement("input"), u.value = "t", u.type = "radio", _.radioValue = u.value === "t"
             }();
-        var oa, ji = h.expr.attrHandle;
+        var sa, ji = h.expr.attrHandle;
         h.fn.extend({
             attr: function(u, f) {
                 return Ae(this, h.attr, u, f, arguments.length > 1)
             },
             removeAttr: function(u) {
                 return this.each(function() {
                     h.removeAttr(this, u)
                 })
             }
         }), h.extend({
             attr: function(u, f, p) {
                 var m, v, b = u.nodeType;
                 if (!(b === 3 || b === 8 || b === 2)) {
                     if (typeof u.getAttribute > "u") return h.prop(u, f, p);
-                    if ((b !== 1 || !h.isXMLDoc(u)) && (v = h.attrHooks[f.toLowerCase()] || (h.expr.match.bool.test(f) ? oa : void 0)), p !== void 0) {
+                    if ((b !== 1 || !h.isXMLDoc(u)) && (v = h.attrHooks[f.toLowerCase()] || (h.expr.match.bool.test(f) ? sa : void 0)), p !== void 0) {
                         if (p === null) {
                             h.removeAttr(u, f);
                             return
                         }
                         return v && "set" in v && (m = v.set(u, p, f)) !== void 0 ? m : (u.setAttribute(f, p + ""), p)
                     }
                     return v && "get" in v && (m = v.get(u, f)) !== null ? m : (m = h.find.attr(u, f), m ?? void 0)
                 }
             },
             attrHooks: {
                 type: {
                     set: function(u, f) {
-                        if (!w.radioValue && f === "radio" && he(u, "input")) {
+                        if (!_.radioValue && f === "radio" && he(u, "input")) {
                             var p = u.value;
                             return u.setAttribute("type", f), p && (u.value = p), f
                         }
                     }
                 }
             },
             removeAttr: function(u, f) {
                 var p, m = 0,
-                    v = f && f.match(Ge);
+                    v = f && f.match(Ke);
                 if (v && u.nodeType === 1)
                     for (; p = v[m++];) u.removeAttribute(p)
             }
-        }), oa = {
+        }), sa = {
             set: function(u, f, p) {
                 return f === !1 ? h.removeAttr(u, p) : u.setAttribute(p, p), p
             }
         }, h.each(h.expr.match.bool.source.match(/\w+/g), function(u, f) {
             var p = ji[f] || h.find.attr;
             ji[f] = function(m, v, b) {
                 var E, L, I = v.toLowerCase();
                 return b || (L = ji[I], ji[I] = E, E = p(m, v, b) != null ? I : null, ji[I] = L), E
             }
         });
-        var Yl = /^(?:input|select|textarea|button)$/i,
-            Ff = /^(?:a|area)$/i;
+        var Xl = /^(?:input|select|textarea|button)$/i,
+            zf = /^(?:a|area)$/i;
         h.fn.extend({
             prop: function(u, f) {
                 return Ae(this, h.prop, u, f, arguments.length > 1)
             },
             removeProp: function(u) {
                 return this.each(function() {
                     delete this[h.propFix[u] || u]
@@ -22739,102 +22738,102 @@
                 var m, v, b = u.nodeType;
                 if (!(b === 3 || b === 8 || b === 2)) return (b !== 1 || !h.isXMLDoc(u)) && (f = h.propFix[f] || f, v = h.propHooks[f]), p !== void 0 ? v && "set" in v && (m = v.set(u, p, f)) !== void 0 ? m : u[f] = p : v && "get" in v && (m = v.get(u, f)) !== null ? m : u[f]
             },
             propHooks: {
                 tabIndex: {
                     get: function(u) {
                         var f = h.find.attr(u, "tabindex");
-                        return f ? parseInt(f, 10) : Yl.test(u.nodeName) || Ff.test(u.nodeName) && u.href ? 0 : -1
+                        return f ? parseInt(f, 10) : Xl.test(u.nodeName) || zf.test(u.nodeName) && u.href ? 0 : -1
                     }
                 }
             },
             propFix: {
                 for: "htmlFor",
                 class: "className"
             }
-        }), w.optSelected || (h.propHooks.selected = {
+        }), _.optSelected || (h.propHooks.selected = {
             get: function(u) {
                 var f = u.parentNode;
                 return f && f.parentNode && f.parentNode.selectedIndex, null
             },
             set: function(u) {
                 var f = u.parentNode;
                 f && (f.selectedIndex, f.parentNode && f.parentNode.selectedIndex)
             }
         }), h.each(["tabIndex", "readOnly", "maxLength", "cellSpacing", "cellPadding", "rowSpan", "colSpan", "useMap", "frameBorder", "contentEditable"], function() {
             h.propFix[this.toLowerCase()] = this
         });
 
         function Hi(u) {
-            var f = u.match(Ge) || [];
+            var f = u.match(Ke) || [];
             return f.join(" ")
         }
 
-        function k(u) {
+        function S(u) {
             return u.getAttribute && u.getAttribute("class") || ""
         }
 
-        function P(u) {
-            return Array.isArray(u) ? u : typeof u == "string" ? u.match(Ge) || [] : []
+        function D(u) {
+            return Array.isArray(u) ? u : typeof u == "string" ? u.match(Ke) || [] : []
         }
         h.fn.extend({
             addClass: function(u) {
                 var f, p, m, v, b, E, L, I = 0;
-                if (S(u)) return this.each(function(B) {
-                    h(this).addClass(u.call(this, B, k(this)))
+                if (C(u)) return this.each(function(B) {
+                    h(this).addClass(u.call(this, B, S(this)))
                 });
-                if (f = P(u), f.length) {
+                if (f = D(u), f.length) {
                     for (; p = this[I++];)
-                        if (v = k(p), m = p.nodeType === 1 && " " + Hi(v) + " ", m) {
+                        if (v = S(p), m = p.nodeType === 1 && " " + Hi(v) + " ", m) {
                             for (E = 0; b = f[E++];) m.indexOf(" " + b + " ") < 0 && (m += b + " ");
                             L = Hi(m), v !== L && p.setAttribute("class", L)
                         }
                 }
                 return this
             },
             removeClass: function(u) {
                 var f, p, m, v, b, E, L, I = 0;
-                if (S(u)) return this.each(function(B) {
-                    h(this).removeClass(u.call(this, B, k(this)))
+                if (C(u)) return this.each(function(B) {
+                    h(this).removeClass(u.call(this, B, S(this)))
                 });
                 if (!arguments.length) return this.attr("class", "");
-                if (f = P(u), f.length) {
+                if (f = D(u), f.length) {
                     for (; p = this[I++];)
-                        if (v = k(p), m = p.nodeType === 1 && " " + Hi(v) + " ", m) {
+                        if (v = S(p), m = p.nodeType === 1 && " " + Hi(v) + " ", m) {
                             for (E = 0; b = f[E++];)
                                 for (; m.indexOf(" " + b + " ") > -1;) m = m.replace(" " + b + " ", " ");
                             L = Hi(m), v !== L && p.setAttribute("class", L)
                         }
                 }
                 return this
             },
             toggleClass: function(u, f) {
                 var p = typeof u,
                     m = p === "string" || Array.isArray(u);
-                return typeof f == "boolean" && m ? f ? this.addClass(u) : this.removeClass(u) : S(u) ? this.each(function(v) {
-                    h(this).toggleClass(u.call(this, v, k(this), f), f)
+                return typeof f == "boolean" && m ? f ? this.addClass(u) : this.removeClass(u) : C(u) ? this.each(function(v) {
+                    h(this).toggleClass(u.call(this, v, S(this), f), f)
                 }) : this.each(function() {
                     var v, b, E, L;
                     if (m)
-                        for (b = 0, E = h(this), L = P(u); v = L[b++];) E.hasClass(v) ? E.removeClass(v) : E.addClass(v);
-                    else(u === void 0 || p === "boolean") && (v = k(this), v && X.set(this, "__className__", v), this.setAttribute && this.setAttribute("class", v || u === !1 ? "" : X.get(this, "__className__") || ""))
+                        for (b = 0, E = h(this), L = D(u); v = L[b++];) E.hasClass(v) ? E.removeClass(v) : E.addClass(v);
+                    else(u === void 0 || p === "boolean") && (v = S(this), v && X.set(this, "__className__", v), this.setAttribute && this.setAttribute("class", v || u === !1 ? "" : X.get(this, "__className__") || ""))
                 })
             },
             hasClass: function(u) {
                 var f, p, m = 0;
                 for (f = " " + u + " "; p = this[m++];)
-                    if (p.nodeType === 1 && (" " + Hi(k(p)) + " ").indexOf(f) > -1) return !0;
+                    if (p.nodeType === 1 && (" " + Hi(S(p)) + " ").indexOf(f) > -1) return !0;
                 return !1
             }
         });
         var N = /\r/g;
         h.fn.extend({
             val: function(u) {
                 var f, p, m, v = this[0];
-                return arguments.length ? (m = S(u), this.each(function(b) {
+                return arguments.length ? (m = C(u), this.each(function(b) {
                     var E;
                     this.nodeType === 1 && (m ? E = u.call(this, b, h(this).val()) : E = u, E == null ? E = "" : typeof E == "number" ? E += "" : Array.isArray(E) && (E = h.map(E, function(L) {
                         return L == null ? "" : L + ""
                     })), f = h.valHooks[this.type] || h.valHooks[this.nodeName.toLowerCase()], (!f || !("set" in f) || f.set(this, E, "value") === void 0) && (this.value = E))
                 })) : v ? (f = h.valHooks[v.type] || h.valHooks[v.nodeName.toLowerCase()], f && "get" in f && (p = f.get(v, "value")) !== void 0 ? p : (p = v.value, typeof p == "string" ? p.replace(N, "") : p ?? "")) : void 0
             }
         }), h.extend({
@@ -22865,35 +22864,35 @@
                 }
             }
         }), h.each(["radio", "checkbox"], function() {
             h.valHooks[this] = {
                 set: function(u, f) {
                     if (Array.isArray(f)) return u.checked = h.inArray(h(u).val(), f) > -1
                 }
-            }, w.checkOn || (h.valHooks[this].get = function(u) {
+            }, _.checkOn || (h.valHooks[this].get = function(u) {
                 return u.getAttribute("value") === null ? "on" : u.value
             })
-        }), w.focusin = "onfocusin" in e;
-        var $ = /^(?:focusinfocus|focusoutblur)$/,
+        }), _.focusin = "onfocusin" in e;
+        var U = /^(?:focusinfocus|focusoutblur)$/,
             J = function(u) {
                 u.stopPropagation()
             };
         h.extend(h.event, {
             trigger: function(u, f, p, m) {
-                var v, b, E, L, I, B, q, ee, U = [p || _],
+                var v, b, E, L, I, B, q, ee, V = [p || w],
                     Z = g.call(u, "type") ? u.type : u,
                     fe = g.call(u, "namespace") ? u.namespace.split(".") : [];
-                if (b = ee = E = p = p || _, !(p.nodeType === 3 || p.nodeType === 8) && !$.test(Z + h.event.triggered) && (Z.indexOf(".") > -1 && (fe = Z.split("."), Z = fe.shift(), fe.sort()), I = Z.indexOf(":") < 0 && "on" + Z, u = u[h.expando] ? u : new h.Event(Z, typeof u == "object" && u), u.isTrigger = m ? 2 : 3, u.namespace = fe.join("."), u.rnamespace = u.namespace ? new RegExp("(^|\\.)" + fe.join("\\.(?:.*\\.|)") + "(\\.|$)") : null, u.result = void 0, u.target || (u.target = p), f = f == null ? [u] : h.makeArray(f, [u]), q = h.event.special[Z] || {}, !(!m && q.trigger && q.trigger.apply(p, f) === !1))) {
+                if (b = ee = E = p = p || w, !(p.nodeType === 3 || p.nodeType === 8) && !U.test(Z + h.event.triggered) && (Z.indexOf(".") > -1 && (fe = Z.split("."), Z = fe.shift(), fe.sort()), I = Z.indexOf(":") < 0 && "on" + Z, u = u[h.expando] ? u : new h.Event(Z, typeof u == "object" && u), u.isTrigger = m ? 2 : 3, u.namespace = fe.join("."), u.rnamespace = u.namespace ? new RegExp("(^|\\.)" + fe.join("\\.(?:.*\\.|)") + "(\\.|$)") : null, u.result = void 0, u.target || (u.target = p), f = f == null ? [u] : h.makeArray(f, [u]), q = h.event.special[Z] || {}, !(!m && q.trigger && q.trigger.apply(p, f) === !1))) {
                     if (!m && !q.noBubble && !A(p)) {
-                        for (L = q.delegateType || Z, $.test(L + Z) || (b = b.parentNode); b; b = b.parentNode) U.push(b), E = b;
-                        E === (p.ownerDocument || _) && U.push(E.defaultView || E.parentWindow || e)
+                        for (L = q.delegateType || Z, U.test(L + Z) || (b = b.parentNode); b; b = b.parentNode) V.push(b), E = b;
+                        E === (p.ownerDocument || w) && V.push(E.defaultView || E.parentWindow || e)
                     }
                     for (v = 0;
-                        (b = U[v++]) && !u.isPropagationStopped();) ee = b, u.type = v > 1 ? L : q.bindType || Z, B = (X.get(b, "events") || Object.create(null))[u.type] && X.get(b, "handle"), B && B.apply(b, f), B = I && b[I], B && B.apply && H(b) && (u.result = B.apply(b, f), u.result === !1 && u.preventDefault());
-                    return u.type = Z, !m && !u.isDefaultPrevented() && (!q._default || q._default.apply(U.pop(), f) === !1) && H(p) && I && S(p[Z]) && !A(p) && (E = p[I], E && (p[I] = null), h.event.triggered = Z, u.isPropagationStopped() && ee.addEventListener(Z, J), p[Z](), u.isPropagationStopped() && ee.removeEventListener(Z, J), h.event.triggered = void 0, E && (p[I] = E)), u.result
+                        (b = V[v++]) && !u.isPropagationStopped();) ee = b, u.type = v > 1 ? L : q.bindType || Z, B = (X.get(b, "events") || Object.create(null))[u.type] && X.get(b, "handle"), B && B.apply(b, f), B = I && b[I], B && B.apply && H(b) && (u.result = B.apply(b, f), u.result === !1 && u.preventDefault());
+                    return u.type = Z, !m && !u.isDefaultPrevented() && (!q._default || q._default.apply(V.pop(), f) === !1) && H(p) && I && C(p[Z]) && !A(p) && (E = p[I], E && (p[I] = null), h.event.triggered = Z, u.isPropagationStopped() && ee.addEventListener(Z, J), p[Z](), u.isPropagationStopped() && ee.removeEventListener(Z, J), h.event.triggered = void 0, E && (p[I] = E)), u.result
                 }
             },
             simulate: function(u, f, p) {
                 var m = h.extend(new h.Event, p, {
                     type: u,
                     isSimulated: !0
                 });
@@ -22905,15 +22904,15 @@
                     h.event.trigger(u, f, this)
                 })
             },
             triggerHandler: function(u, f) {
                 var p = this[0];
                 if (p) return h.event.trigger(u, f, p, !0)
             }
-        }), w.focusin || h.each({
+        }), _.focusin || h.each({
             focus: "focusin",
             blur: "focusout"
         }, function(u, f) {
             var p = function(m) {
                 h.event.simulate(f, m.target, h.event.fix(m))
             };
             h.event.special[f] = {
@@ -22926,15 +22925,15 @@
                     var m = this.ownerDocument || this.document || this,
                         v = X.access(m, f) - 1;
                     v ? X.access(m, f, v) : (m.removeEventListener(u, p, !0), X.remove(m, f))
                 }
             }
         });
         var se = e.location,
-            ke = {
+            Se = {
                 guid: Date.now()
             },
             yt = /\?/;
         h.parseXML = function(u) {
             var f;
             if (!u || typeof u != "string") return null;
             try {
@@ -22945,35 +22944,35 @@
             return (!f || f.getElementsByTagName("parsererror").length) && h.error("Invalid XML: " + u), f
         };
         var Et = /\[\]$/,
             Lt = /\r?\n/g,
             Bn = /^(?:submit|button|image|reset|file)$/i,
             x_ = /^(?:input|select|textarea|keygen)/i;
 
-        function jf(u, f, p, m) {
+        function Ff(u, f, p, m) {
             var v;
             if (Array.isArray(f)) h.each(f, function(b, E) {
-                p || Et.test(u) ? m(u, E) : jf(u + "[" + (typeof E == "object" && E != null ? b : "") + "]", E, p, m)
+                p || Et.test(u) ? m(u, E) : Ff(u + "[" + (typeof E == "object" && E != null ? b : "") + "]", E, p, m)
             });
             else if (!p && z(f) === "object")
-                for (v in f) jf(u + "[" + v + "]", f[v], p, m);
+                for (v in f) Ff(u + "[" + v + "]", f[v], p, m);
             else m(u, f)
         }
         h.param = function(u, f) {
             var p, m = [],
                 v = function(b, E) {
-                    var L = S(E) ? E() : E;
+                    var L = C(E) ? E() : E;
                     m[m.length] = encodeURIComponent(b) + "=" + encodeURIComponent(L ?? "")
                 };
             if (u == null) return "";
             if (Array.isArray(u) || u.jquery && !h.isPlainObject(u)) h.each(u, function() {
                 v(this.name, this.value)
             });
             else
-                for (p in u) jf(p, u[p], f, v);
+                for (p in u) Ff(p, u[p], f, v);
             return m.join("&")
         }, h.fn.extend({
             serialize: function() {
                 return h.param(this.serializeArray())
             },
             serializeArray: function() {
                 return this.map(function() {
@@ -22997,50 +22996,50 @@
                     }
                 }).get()
             }
         });
         var b_ = /%20/g,
             __ = /#.*$/,
             w_ = /([?&])_=[^&]*/,
-            k_ = /^(.*?):[ \t]*([^\r\n]*)$/mg,
-            S_ = /^(?:about|app|app-storage|.+-extension|file|res|widget):$/,
+            S_ = /^(.*?):[ \t]*([^\r\n]*)$/mg,
+            k_ = /^(?:about|app|app-storage|.+-extension|file|res|widget):$/,
             C_ = /^(?:GET|HEAD)$/,
             E_ = /^\/\//,
             om = {},
-            Hf = {},
+            jf = {},
             sm = "*/".concat("*"),
-            Bf = _.createElement("a");
-        Bf.href = se.href;
+            Hf = w.createElement("a");
+        Hf.href = se.href;
 
         function am(u) {
             return function(f, p) {
                 typeof f != "string" && (p = f, f = "*");
                 var m, v = 0,
-                    b = f.toLowerCase().match(Ge) || [];
-                if (S(p))
+                    b = f.toLowerCase().match(Ke) || [];
+                if (C(p))
                     for (; m = b[v++];) m[0] === "+" ? (m = m.slice(1) || "*", (u[m] = u[m] || []).unshift(p)) : (u[m] = u[m] || []).push(p)
             }
         }
 
         function lm(u, f, p, m) {
             var v = {},
-                b = u === Hf;
+                b = u === jf;
 
             function E(L) {
                 var I;
                 return v[L] = !0, h.each(u[L] || [], function(B, q) {
                     var ee = q(f, p, m);
                     if (typeof ee == "string" && !b && !v[ee]) return f.dataTypes.unshift(ee), E(ee), !1;
                     if (b) return !(I = ee)
                 }), I
             }
             return E(f.dataTypes[0]) || !v["*"] && E("*")
         }
 
-        function Wf(u, f) {
+        function Bf(u, f) {
             var p, m, v = h.ajaxSettings.flatOptions || {};
             for (p in f) f[p] !== void 0 && ((v[p] ? u : m || (m = {}))[p] = f[p]);
             return m && h.extend(!0, u, m), u
         }
 
         function T_(u, f, p) {
             for (var m, v, b, E, L = u.contents, I = u.dataTypes; I[0] === "*";) I.shift(), m === void 0 && (m = u.mimeType || f.getResponseHeader("Content-Type"));
@@ -23061,15 +23060,15 @@
                     E || (E = v)
                 }
                 b = b || E
             }
             if (b) return b !== I[0] && I.unshift(b), p[b]
         }
 
-        function P_(u, f, p, m) {
+        function D_(u, f, p, m) {
             var v, b, E, L, I, B = {},
                 q = u.dataTypes.slice();
             if (q[1])
                 for (E in u.converters) B[E.toLowerCase()] = u.converters[E];
             for (b = q.shift(); b;)
                 if (u.responseFields[b] && (p[u.responseFields[b]] = f), !I && m && u.dataFilter && (f = u.dataFilter(f, u.dataType)), I = b, b = q.shift(), b) {
                     if (b === "*") b = I;
@@ -23100,15 +23099,15 @@
         h.extend({
             active: 0,
             lastModified: {},
             etag: {},
             ajaxSettings: {
                 url: se.href,
                 type: "GET",
-                isLocal: S_.test(se.protocol),
+                isLocal: k_.test(se.protocol),
                 global: !0,
                 processData: !0,
                 async: !0,
                 contentType: "application/x-www-form-urlencoded; charset=UTF-8",
                 accepts: {
                     "*": sm,
                     text: "text/plain",
@@ -23134,103 +23133,103 @@
                 },
                 flatOptions: {
                     url: !0,
                     context: !0
                 }
             },
             ajaxSetup: function(u, f) {
-                return f ? Wf(Wf(u, h.ajaxSettings), f) : Wf(h.ajaxSettings, u)
+                return f ? Bf(Bf(u, h.ajaxSettings), f) : Bf(h.ajaxSettings, u)
             },
             ajaxPrefilter: am(om),
-            ajaxTransport: am(Hf),
+            ajaxTransport: am(jf),
             ajax: function(u, f) {
                 typeof u == "object" && (f = u, u = void 0), f = f || {};
-                var p, m, v, b, E, L, I, B, q, ee, U = h.ajaxSetup({}, f),
-                    Z = U.context || U,
-                    fe = U.context && (Z.nodeType || Z.jquery) ? h(Z) : h.event,
+                var p, m, v, b, E, L, I, B, q, ee, V = h.ajaxSetup({}, f),
+                    Z = V.context || V,
+                    fe = V.context && (Z.nodeType || Z.jquery) ? h(Z) : h.event,
                     _e = h.Deferred(),
                     de = h.Callbacks("once memory"),
-                    Tt = U.statusCode || {},
+                    Tt = V.statusCode || {},
                     wt = {},
                     Tn = {},
                     Ue = "canceled",
                     be = {
                         readyState: 0,
                         getResponseHeader: function(ze) {
                             var ct;
                             if (I) {
                                 if (!b)
-                                    for (b = {}; ct = k_.exec(v);) b[ct[1].toLowerCase() + " "] = (b[ct[1].toLowerCase() + " "] || []).concat(ct[2]);
+                                    for (b = {}; ct = S_.exec(v);) b[ct[1].toLowerCase() + " "] = (b[ct[1].toLowerCase() + " "] || []).concat(ct[2]);
                                 ct = b[ze.toLowerCase() + " "]
                             }
                             return ct == null ? null : ct.join(", ")
                         },
                         getAllResponseHeaders: function() {
                             return I ? v : null
                         },
                         setRequestHeader: function(ze, ct) {
                             return I == null && (ze = Tn[ze.toLowerCase()] = Tn[ze.toLowerCase()] || ze, wt[ze] = ct), this
                         },
                         overrideMimeType: function(ze) {
-                            return I == null && (U.mimeType = ze), this
+                            return I == null && (V.mimeType = ze), this
                         },
                         statusCode: function(ze) {
                             var ct;
                             if (ze)
                                 if (I) be.always(ze[be.status]);
                                 else
                                     for (ct in ze) Tt[ct] = [Tt[ct], ze[ct]];
                             return this
                         },
                         abort: function(ze) {
                             var ct = ze || Ue;
                             return p && p.abort(ct), dn(0, ct), this
                         }
                     };
-                if (_e.promise(be), U.url = ((u || U.url || se.href) + "").replace(E_, se.protocol + "//"), U.type = f.method || f.type || U.method || U.type, U.dataTypes = (U.dataType || "*").toLowerCase().match(Ge) || [""], U.crossDomain == null) {
-                    L = _.createElement("a");
+                if (_e.promise(be), V.url = ((u || V.url || se.href) + "").replace(E_, se.protocol + "//"), V.type = f.method || f.type || V.method || V.type, V.dataTypes = (V.dataType || "*").toLowerCase().match(Ke) || [""], V.crossDomain == null) {
+                    L = w.createElement("a");
                     try {
-                        L.href = U.url, L.href = L.href, U.crossDomain = Bf.protocol + "//" + Bf.host != L.protocol + "//" + L.host
+                        L.href = V.url, L.href = L.href, V.crossDomain = Hf.protocol + "//" + Hf.host != L.protocol + "//" + L.host
                     } catch {
-                        U.crossDomain = !0
+                        V.crossDomain = !0
                     }
                 }
-                if (U.data && U.processData && typeof U.data != "string" && (U.data = h.param(U.data, U.traditional)), lm(om, U, f, be), I) return be;
-                B = h.event && U.global, B && h.active++ === 0 && h.event.trigger("ajaxStart"), U.type = U.type.toUpperCase(), U.hasContent = !C_.test(U.type), m = U.url.replace(__, ""), U.hasContent ? U.data && U.processData && (U.contentType || "").indexOf("application/x-www-form-urlencoded") === 0 && (U.data = U.data.replace(b_, "+")) : (ee = U.url.slice(m.length), U.data && (U.processData || typeof U.data == "string") && (m += (yt.test(m) ? "&" : "?") + U.data, delete U.data), U.cache === !1 && (m = m.replace(w_, "$1"), ee = (yt.test(m) ? "&" : "?") + "_=" + ke.guid++ + ee), U.url = m + ee), U.ifModified && (h.lastModified[m] && be.setRequestHeader("If-Modified-Since", h.lastModified[m]), h.etag[m] && be.setRequestHeader("If-None-Match", h.etag[m])), (U.data && U.hasContent && U.contentType !== !1 || f.contentType) && be.setRequestHeader("Content-Type", U.contentType), be.setRequestHeader("Accept", U.dataTypes[0] && U.accepts[U.dataTypes[0]] ? U.accepts[U.dataTypes[0]] + (U.dataTypes[0] !== "*" ? ", " + sm + "; q=0.01" : "") : U.accepts["*"]);
-                for (q in U.headers) be.setRequestHeader(q, U.headers[q]);
-                if (U.beforeSend && (U.beforeSend.call(Z, be, U) === !1 || I)) return be.abort();
-                if (Ue = "abort", de.add(U.complete), be.done(U.success), be.fail(U.error), p = lm(Hf, U, f, be), !p) dn(-1, "No Transport");
+                if (V.data && V.processData && typeof V.data != "string" && (V.data = h.param(V.data, V.traditional)), lm(om, V, f, be), I) return be;
+                B = h.event && V.global, B && h.active++ === 0 && h.event.trigger("ajaxStart"), V.type = V.type.toUpperCase(), V.hasContent = !C_.test(V.type), m = V.url.replace(__, ""), V.hasContent ? V.data && V.processData && (V.contentType || "").indexOf("application/x-www-form-urlencoded") === 0 && (V.data = V.data.replace(b_, "+")) : (ee = V.url.slice(m.length), V.data && (V.processData || typeof V.data == "string") && (m += (yt.test(m) ? "&" : "?") + V.data, delete V.data), V.cache === !1 && (m = m.replace(w_, "$1"), ee = (yt.test(m) ? "&" : "?") + "_=" + Se.guid++ + ee), V.url = m + ee), V.ifModified && (h.lastModified[m] && be.setRequestHeader("If-Modified-Since", h.lastModified[m]), h.etag[m] && be.setRequestHeader("If-None-Match", h.etag[m])), (V.data && V.hasContent && V.contentType !== !1 || f.contentType) && be.setRequestHeader("Content-Type", V.contentType), be.setRequestHeader("Accept", V.dataTypes[0] && V.accepts[V.dataTypes[0]] ? V.accepts[V.dataTypes[0]] + (V.dataTypes[0] !== "*" ? ", " + sm + "; q=0.01" : "") : V.accepts["*"]);
+                for (q in V.headers) be.setRequestHeader(q, V.headers[q]);
+                if (V.beforeSend && (V.beforeSend.call(Z, be, V) === !1 || I)) return be.abort();
+                if (Ue = "abort", de.add(V.complete), be.done(V.success), be.fail(V.error), p = lm(jf, V, f, be), !p) dn(-1, "No Transport");
                 else {
-                    if (be.readyState = 1, B && fe.trigger("ajaxSend", [be, U]), I) return be;
-                    U.async && U.timeout > 0 && (E = e.setTimeout(function() {
+                    if (be.readyState = 1, B && fe.trigger("ajaxSend", [be, V]), I) return be;
+                    V.async && V.timeout > 0 && (E = e.setTimeout(function() {
                         be.abort("timeout")
-                    }, U.timeout));
+                    }, V.timeout));
                     try {
                         I = !1, p.send(wt, dn)
                     } catch (ze) {
                         if (I) throw ze;
                         dn(-1, ze)
                     }
                 }
 
-                function dn(ze, ct, aa, Xl) {
-                    var Pn, oo, so, hn, pr, Wn = ct;
-                    I || (I = !0, E && e.clearTimeout(E), p = void 0, v = Xl || "", be.readyState = ze > 0 ? 4 : 0, Pn = ze >= 200 && ze < 300 || ze === 304, aa && (hn = T_(U, be, aa)), !Pn && h.inArray("script", U.dataTypes) > -1 && (U.converters["text script"] = function() {}), hn = P_(U, hn, be, Pn), Pn ? (U.ifModified && (pr = be.getResponseHeader("Last-Modified"), pr && (h.lastModified[m] = pr), pr = be.getResponseHeader("etag"), pr && (h.etag[m] = pr)), ze === 204 || U.type === "HEAD" ? Wn = "nocontent" : ze === 304 ? Wn = "notmodified" : (Wn = hn.state, oo = hn.data, so = hn.error, Pn = !so)) : (so = Wn, (ze || !Wn) && (Wn = "error", ze < 0 && (ze = 0))), be.status = ze, be.statusText = (ct || Wn) + "", Pn ? _e.resolveWith(Z, [oo, Wn, be]) : _e.rejectWith(Z, [be, Wn, so]), be.statusCode(Tt), Tt = void 0, B && fe.trigger(Pn ? "ajaxSuccess" : "ajaxError", [be, U, Pn ? oo : so]), de.fireWith(Z, [be, Wn]), B && (fe.trigger("ajaxComplete", [be, U]), --h.active || h.event.trigger("ajaxStop")))
+                function dn(ze, ct, la, ql) {
+                    var Dn, oo, so, hn, pr, Wn = ct;
+                    I || (I = !0, E && e.clearTimeout(E), p = void 0, v = ql || "", be.readyState = ze > 0 ? 4 : 0, Dn = ze >= 200 && ze < 300 || ze === 304, la && (hn = T_(V, be, la)), !Dn && h.inArray("script", V.dataTypes) > -1 && (V.converters["text script"] = function() {}), hn = D_(V, hn, be, Dn), Dn ? (V.ifModified && (pr = be.getResponseHeader("Last-Modified"), pr && (h.lastModified[m] = pr), pr = be.getResponseHeader("etag"), pr && (h.etag[m] = pr)), ze === 204 || V.type === "HEAD" ? Wn = "nocontent" : ze === 304 ? Wn = "notmodified" : (Wn = hn.state, oo = hn.data, so = hn.error, Dn = !so)) : (so = Wn, (ze || !Wn) && (Wn = "error", ze < 0 && (ze = 0))), be.status = ze, be.statusText = (ct || Wn) + "", Dn ? _e.resolveWith(Z, [oo, Wn, be]) : _e.rejectWith(Z, [be, Wn, so]), be.statusCode(Tt), Tt = void 0, B && fe.trigger(Dn ? "ajaxSuccess" : "ajaxError", [be, V, Dn ? oo : so]), de.fireWith(Z, [be, Wn]), B && (fe.trigger("ajaxComplete", [be, V]), --h.active || h.event.trigger("ajaxStop")))
                 }
                 return be
             },
             getJSON: function(u, f, p) {
                 return h.get(u, f, p, "json")
             },
             getScript: function(u, f) {
                 return h.get(u, void 0, f, "script")
             }
         }), h.each(["get", "post"], function(u, f) {
             h[f] = function(p, m, v, b) {
-                return S(m) && (b = b || v, v = m, m = void 0), h.ajax(h.extend({
+                return C(m) && (b = b || v, v = m, m = void 0), h.ajax(h.extend({
                     url: p,
                     type: f,
                     dataType: b,
                     data: m,
                     success: v
                 }, h.isPlainObject(p) && p))
             }
@@ -23251,30 +23250,30 @@
                 dataFilter: function(m) {
                     h.globalEval(m, f, p)
                 }
             })
         }, h.fn.extend({
             wrapAll: function(u) {
                 var f;
-                return this[0] && (S(u) && (u = u.call(this[0])), f = h(u, this[0].ownerDocument).eq(0).clone(!0), this[0].parentNode && f.insertBefore(this[0]), f.map(function() {
+                return this[0] && (C(u) && (u = u.call(this[0])), f = h(u, this[0].ownerDocument).eq(0).clone(!0), this[0].parentNode && f.insertBefore(this[0]), f.map(function() {
                     for (var p = this; p.firstElementChild;) p = p.firstElementChild;
                     return p
                 }).append(this)), this
             },
             wrapInner: function(u) {
-                return S(u) ? this.each(function(f) {
+                return C(u) ? this.each(function(f) {
                     h(this).wrapInner(u.call(this, f))
                 }) : this.each(function() {
                     var f = h(this),
                         p = f.contents();
                     p.length ? p.wrapAll(u) : f.append(u)
                 })
             },
             wrap: function(u) {
-                var f = S(u);
+                var f = C(u);
                 return this.each(function(p) {
                     h(this).wrapAll(f ? u.call(this, p) : u)
                 })
             },
             unwrap: function(u) {
                 return this.parent(u).not("body").each(function() {
                     h(this).replaceWith(this.childNodes)
@@ -23285,31 +23284,31 @@
         }, h.expr.pseudos.visible = function(u) {
             return !!(u.offsetWidth || u.offsetHeight || u.getClientRects().length)
         }, h.ajaxSettings.xhr = function() {
             try {
                 return new e.XMLHttpRequest
             } catch {}
         };
-        var M_ = {
+        var P_ = {
                 0: 200,
                 1223: 204
             },
-            sa = h.ajaxSettings.xhr();
-        w.cors = !!sa && "withCredentials" in sa, w.ajax = sa = !!sa, h.ajaxTransport(function(u) {
+            aa = h.ajaxSettings.xhr();
+        _.cors = !!aa && "withCredentials" in aa, _.ajax = aa = !!aa, h.ajaxTransport(function(u) {
             var f, p;
-            if (w.cors || sa && !u.crossDomain) return {
+            if (_.cors || aa && !u.crossDomain) return {
                 send: function(m, v) {
                     var b, E = u.xhr();
                     if (E.open(u.type, u.url, u.async, u.username, u.password), u.xhrFields)
                         for (b in u.xhrFields) E[b] = u.xhrFields[b];
                     u.mimeType && E.overrideMimeType && E.overrideMimeType(u.mimeType), !u.crossDomain && !m["X-Requested-With"] && (m["X-Requested-With"] = "XMLHttpRequest");
                     for (b in m) E.setRequestHeader(b, m[b]);
                     f = function(L) {
                         return function() {
-                            f && (f = p = E.onload = E.onerror = E.onabort = E.ontimeout = E.onreadystatechange = null, L === "abort" ? E.abort() : L === "error" ? typeof E.status != "number" ? v(0, "error") : v(E.status, E.statusText) : v(M_[E.status] || E.status, E.statusText, (E.responseType || "text") !== "text" || typeof E.responseText != "string" ? {
+                            f && (f = p = E.onload = E.onerror = E.onabort = E.ontimeout = E.onreadystatechange = null, L === "abort" ? E.abort() : L === "error" ? typeof E.status != "number" ? v(0, "error") : v(E.status, E.statusText) : v(P_[E.status] || E.status, E.statusText, (E.responseType || "text") !== "text" || typeof E.responseText != "string" ? {
                                 binary: E.response
                             } : {
                                 text: E.responseText
                             }, E.getAllResponseHeaders()))
                         }
                     }, E.onload = f(), p = E.onerror = E.ontimeout = f("error"), E.onabort !== void 0 ? E.onabort = p : E.onreadystatechange = function() {
                         E.readyState === 4 && e.setTimeout(function() {
@@ -23348,51 +23347,51 @@
                 return {
                     send: function(m, v) {
                         f = h("<script>").attr(u.scriptAttrs || {}).prop({
                             charset: u.scriptCharset,
                             src: u.url
                         }).on("load error", p = function(b) {
                             f.remove(), p = null, b && v(b.type === "error" ? 404 : 200, b.type)
-                        }), _.head.appendChild(f[0])
+                        }), w.head.appendChild(f[0])
                     },
                     abort: function() {
                         p && p()
                     }
                 }
             }
         });
         var um = [],
-            Vf = /(=)\?(?=&|$)|\?\?/;
+            Wf = /(=)\?(?=&|$)|\?\?/;
         h.ajaxSetup({
             jsonp: "callback",
             jsonpCallback: function() {
-                var u = um.pop() || h.expando + "_" + ke.guid++;
+                var u = um.pop() || h.expando + "_" + Se.guid++;
                 return this[u] = !0, u
             }
         }), h.ajaxPrefilter("json jsonp", function(u, f, p) {
-            var m, v, b, E = u.jsonp !== !1 && (Vf.test(u.url) ? "url" : typeof u.data == "string" && (u.contentType || "").indexOf("application/x-www-form-urlencoded") === 0 && Vf.test(u.data) && "data");
-            if (E || u.dataTypes[0] === "jsonp") return m = u.jsonpCallback = S(u.jsonpCallback) ? u.jsonpCallback() : u.jsonpCallback, E ? u[E] = u[E].replace(Vf, "$1" + m) : u.jsonp !== !1 && (u.url += (yt.test(u.url) ? "&" : "?") + u.jsonp + "=" + m), u.converters["script json"] = function() {
+            var m, v, b, E = u.jsonp !== !1 && (Wf.test(u.url) ? "url" : typeof u.data == "string" && (u.contentType || "").indexOf("application/x-www-form-urlencoded") === 0 && Wf.test(u.data) && "data");
+            if (E || u.dataTypes[0] === "jsonp") return m = u.jsonpCallback = C(u.jsonpCallback) ? u.jsonpCallback() : u.jsonpCallback, E ? u[E] = u[E].replace(Wf, "$1" + m) : u.jsonp !== !1 && (u.url += (yt.test(u.url) ? "&" : "?") + u.jsonp + "=" + m), u.converters["script json"] = function() {
                 return b || h.error(m + " was not called"), b[0]
             }, u.dataTypes[0] = "json", v = e[m], e[m] = function() {
                 b = arguments
             }, p.always(function() {
-                v === void 0 ? h(e).removeProp(m) : e[m] = v, u[m] && (u.jsonpCallback = f.jsonpCallback, um.push(m)), b && S(v) && v(b[0]), b = v = void 0
+                v === void 0 ? h(e).removeProp(m) : e[m] = v, u[m] && (u.jsonpCallback = f.jsonpCallback, um.push(m)), b && C(v) && v(b[0]), b = v = void 0
             }), "script"
-        }), w.createHTMLDocument = function() {
-            var u = _.implementation.createHTMLDocument("").body;
+        }), _.createHTMLDocument = function() {
+            var u = w.implementation.createHTMLDocument("").body;
             return u.innerHTML = "<form></form><form></form>", u.childNodes.length === 2
         }(), h.parseHTML = function(u, f, p) {
             if (typeof u != "string") return [];
             typeof f == "boolean" && (p = f, f = !1);
             var m, v, b;
-            return f || (w.createHTMLDocument ? (f = _.implementation.createHTMLDocument(""), m = f.createElement("base"), m.href = _.location.href, f.head.appendChild(m)) : f = _), v = Fe.exec(u), b = !p && [], v ? [f.createElement(v[1])] : (v = Ks([u], f, b), b && b.length && h(b).remove(), h.merge([], v.childNodes))
+            return f || (_.createHTMLDocument ? (f = w.implementation.createHTMLDocument(""), m = f.createElement("base"), m.href = w.location.href, f.head.appendChild(m)) : f = w), v = Fe.exec(u), b = !p && [], v ? [f.createElement(v[1])] : (v = Js([u], f, b), b && b.length && h(b).remove(), h.merge([], v.childNodes))
         }, h.fn.load = function(u, f, p) {
             var m, v, b, E = this,
                 L = u.indexOf(" ");
-            return L > -1 && (m = Hi(u.slice(L)), u = u.slice(0, L)), S(f) ? (p = f, f = void 0) : f && typeof f == "object" && (v = "POST"), E.length > 0 && h.ajax({
+            return L > -1 && (m = Hi(u.slice(L)), u = u.slice(0, L)), C(f) ? (p = f, f = void 0) : f && typeof f == "object" && (v = "POST"), E.length > 0 && h.ajax({
                 url: u,
                 type: v || "GET",
                 dataType: "html",
                 data: f
             }).done(function(I) {
                 b = arguments, E.html(m ? h("<div>").append(h.parseHTML(I)).find(m) : I)
             }).always(p && function(I, B) {
@@ -23404,16 +23403,16 @@
             return h.grep(h.timers, function(f) {
                 return u === f.elem
             }).length
         }, h.offset = {
             setOffset: function(u, f, p) {
                 var m, v, b, E, L, I, B, q = h.css(u, "position"),
                     ee = h(u),
-                    U = {};
-                q === "static" && (u.style.position = "relative"), L = ee.offset(), b = h.css(u, "top"), I = h.css(u, "left"), B = (q === "absolute" || q === "fixed") && (b + I).indexOf("auto") > -1, B ? (m = ee.position(), E = m.top, v = m.left) : (E = parseFloat(b) || 0, v = parseFloat(I) || 0), S(f) && (f = f.call(u, p, h.extend({}, L))), f.top != null && (U.top = f.top - L.top + E), f.left != null && (U.left = f.left - L.left + v), "using" in f ? f.using.call(u, U) : (typeof U.top == "number" && (U.top += "px"), typeof U.left == "number" && (U.left += "px"), ee.css(U))
+                    V = {};
+                q === "static" && (u.style.position = "relative"), L = ee.offset(), b = h.css(u, "top"), I = h.css(u, "left"), B = (q === "absolute" || q === "fixed") && (b + I).indexOf("auto") > -1, B ? (m = ee.position(), E = m.top, v = m.left) : (E = parseFloat(b) || 0, v = parseFloat(I) || 0), C(f) && (f = f.call(u, p, h.extend({}, L))), f.top != null && (V.top = f.top - L.top + E), f.left != null && (V.left = f.left - L.left + v), "using" in f ? f.using.call(u, V) : (typeof V.top == "number" && (V.top += "px"), typeof V.left == "number" && (V.left += "px"), ee.css(V))
             }
         }, h.fn.extend({
             offset: function(u) {
                 if (arguments.length) return u === void 0 ? this : this.each(function(v) {
                     h.offset.setOffset(this, u, v)
                 });
                 var f, p, m = this[0];
@@ -23458,16 +23457,16 @@
                 return Ae(this, function(v, b, E) {
                     var L;
                     if (A(v) ? L = v : v.nodeType === 9 && (L = v.defaultView), E === void 0) return L ? L[f] : v[b];
                     L ? L.scrollTo(p ? L.pageXOffset : E, p ? E : L.pageYOffset) : v[b] = E
                 }, u, m, arguments.length)
             }
         }), h.each(["top", "left"], function(u, f) {
-            h.cssHooks[f] = cr(w.pixelPosition, function(p, m) {
-                if (m) return m = Qn(p, f), Xo.test(m) ? h(p).position()[f] + "px" : m
+            h.cssHooks[f] = cr(_.pixelPosition, function(p, m) {
+                if (m) return m = Gn(p, f), Xo.test(m) ? h(p).position()[f] + "px" : m
             })
         }), h.each({
             Height: "height",
             Width: "width"
         }, function(u, f) {
             h.each({
                 padding: "inner" + u,
@@ -23504,27 +23503,27 @@
                 return this.mouseenter(u).mouseleave(f || u)
             }
         }), h.each("blur focus focusin focusout resize scroll click dblclick mousedown mouseup mousemove mouseover mouseout mouseenter mouseleave change select submit keydown keypress keyup contextmenu".split(" "), function(u, f) {
             h.fn[f] = function(p, m) {
                 return arguments.length > 0 ? this.on(f, null, p, m) : this.trigger(f)
             }
         });
-        var D_ = /^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g;
+        var M_ = /^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g;
         h.proxy = function(u, f) {
             var p, m, v;
-            if (typeof f == "string" && (p = u[f], f = u, u = p), !!S(u)) return m = o.call(arguments, 2), v = function() {
+            if (typeof f == "string" && (p = u[f], f = u, u = p), !!C(u)) return m = o.call(arguments, 2), v = function() {
                 return u.apply(f || this, m.concat(o.call(arguments)))
             }, v.guid = u.guid = u.guid || h.guid++, v
         }, h.holdReady = function(u) {
             u ? h.readyWait++ : h.ready(!0)
-        }, h.isArray = Array.isArray, h.parseJSON = JSON.parse, h.nodeName = he, h.isFunction = S, h.isWindow = A, h.camelCase = D, h.type = z, h.now = Date.now, h.isNumeric = function(u) {
+        }, h.isArray = Array.isArray, h.parseJSON = JSON.parse, h.nodeName = he, h.isFunction = C, h.isWindow = A, h.camelCase = M, h.type = z, h.now = Date.now, h.isNumeric = function(u) {
             var f = h.type(u);
             return (f === "number" || f === "string") && !isNaN(u - parseFloat(u))
         }, h.trim = function(u) {
-            return u == null ? "" : (u + "").replace(D_, "")
+            return u == null ? "" : (u + "").replace(M_, "")
         };
         var O_ = e.jQuery,
             A_ = e.$;
         return h.noConflict = function(u) {
             return e.$ === h && (e.$ = A_), u && e.jQuery === h && (e.jQuery = O_), h
         }, typeof n > "u" && (e.jQuery = e.$ = h), h
     })
@@ -23536,120 +23535,118 @@
         e.length && (t.myChart.options.plugins.zoom.pan.enabled = !1, t.myChart.options.plugins.zoom.zoom.drag.enabled = !0, t.myChart.update("none")), gi.isEmptyObject(n) || (t.myDos.options.plugins.zoom.pan.enabled = !1, t.myDos.options.plugins.zoom.zoom.drag.enabled = !0, t.myDos.update("none"))
     };
 
 function H2(t, e, n) {
     e.length && (t.myChart.options.plugins.zoom.pan.enabled = !0, t.myChart.options.plugins.zoom.zoom.drag.enabled = !1, t.myChart.update("none")), gi.isEmptyObject(n) || (t.myDos.options.plugins.zoom.pan.enabled = !0, t.myDos.options.plugins.zoom.zoom.drag.enabled = !1, t.myDos.update("none"))
 }
 
-function B2(t, e, n, i, r, o, s, a, l) {
-    a1[t] = {};
-    var c = window.performance.now();
-    console.log("start time: plotting band plot: current time => ", t, c);
-    var d = new mi(t, r, o, s, a);
+function B2(t, e, n, i, r, o, s, a) {
+    a1[t] = {}, window.performance.now();
+    var l = new mi(t, r, o, a);
     if (n.length) {
-        n.forEach(function(F, h) {
-            var Y;
-            if (l !== void 0)
-                if (typeof l[h] == "object") {
-                    var V = Hs("red");
-                    Y = [V, l[h][0], l[h][1]]
-                } else if (typeof l[h] == "string") {
-                var V = Hs(l[h]);
-                Y = [V.toHexString(), V.darken(20).toHexString(), V.brighten(20).toHexString()]
+        n.forEach(function(P, z) {
+            var F;
+            if (s !== void 0)
+                if (typeof s[z] == "object") {
+                    var h = Hs("black");
+                    F = [h, s[z][0], s[z][1]]
+                } else if (typeof s[z] == "string") {
+                var h = Hs(s[z]);
+                F = [h.toHexString(), h.darken(20).toHexString(), h.brighten(20).toHexString()]
             } else {
-                var V = Hs("red");
-                Y = [V.toHexString(), V.darken(20).toHexString(), V.brighten(20).toHexString()]
+                var h = Hs("black");
+                F = [h.toHexString(), h.darken(20).toHexString(), h.brighten(20).toHexString()]
             }
-            d.addBandStructure(F, Y)
-        }), d.updateBandPlot();
-        var g = document.getElementById(e);
-        g.value = s1(d.getDefaultPath()), g.onkeyup = function() {
-            var F = document.getElementById(e),
-                h = F.value,
-                Y = z2(h);
-            d.updateBandPlot(Y)
+            l.addBandStructure(P, F)
+        }), l.updateBandPlot();
+        var c = document.getElementById(e);
+        c.value = s1(l.getDefaultPath()), c.onkeyup = function() {
+            var P = document.getElementById(e),
+                z = P.value,
+                F = z2(z);
+            l.updateBandPlot(F)
         };
-        var y = "Use - to define a segment<br>Use | to split the path.<br>Valid point names:<br>",
-            x = f1(d.allData);
-        y += x.join(", ");
-        var w = document.getElementById(t + "bt-reset");
-        w.onclick = function() {
-            var F = document.getElementById(e);
-            F.value = s1(d.getDefaultPath()), d.updateBandPlot(d.getDefaultPath(), !0)
+        var d = "Use - to define a segment<br>Use | to split the path.<br>Valid point names:<br>",
+            g = f1(l.allData);
+        d += g.join(", ");
+        var y = document.getElementById(t + "bt-reset");
+        y.onclick = function() {
+            var P = document.getElementById(e);
+            P.value = s1(l.getDefaultPath()), l.updateBandPlot(l.getDefaultPath(), !0)
         };
-        var S = document.getElementById(t + "bt-downloadFigure");
-        S.onclick = function() {
+        var x = document.getElementById(t + "bt-downloadFigure");
+        x.onclick = function() {
             if (gi.isEmptyObject(i)) {
-                var F = document.createElement("a");
-                F.href = d.myChart.toBase64Image("bandstructure.png", 1), F.download = "bandstructure.png", F.click()
+                var P = document.createElement("a");
+                P.href = l.myChart.toBase64Image("bandstructure.png", 1), P.download = "bandstructure.png", P.click()
             }
         };
-        var A = document.getElementById(t + "bt-downloadJson");
-        A.onclick = function() {
+        var _ = document.getElementById(t + "bt-downloadJson");
+        _.onclick = function() {
             if (gi.isEmptyObject(i)) {
-                var F = document.createElement("a");
-                n.length && n.forEach(function(h, Y) {
-                    F.href = "data:text/json;charset=utf-8," + encodeURIComponent(JSON.stringify(h)), F.download = "bandData" + Y + ".json", F.click()
+                var P = document.createElement("a");
+                n.length && n.forEach(function(z, F) {
+                    P.href = "data:text/json;charset=utf-8," + encodeURIComponent(JSON.stringify(z)), P.download = "bandData" + F + ".json", P.click()
                 })
             }
         }
     }
     if (!gi.isEmptyObject(i)) {
-        let F = function(V) {
-            d.dosSeries.forEach((te, ie) => {
-                te.label.toLowerCase().includes("total") || te.label.toLowerCase().includes("y axis") || (V ? d.myDos.hide(ie) : d.myDos.show(ie))
+        let P = function(h) {
+            l.dosSeries.forEach(($, Y) => {
+                $.label.toLowerCase().includes("total") || $.label.toLowerCase().includes("y axis") || (h ? l.myDos.hide(Y) : l.myDos.show(Y))
             })
         };
-        d.addDos(i), n.length ? d.updateDosPlot("vertical") : d.updateDosPlot("horizontal");
-        var _ = document.getElementById(t + "bt-togglePdos");
-        _.onclick = function() {
-            _.classList.contains("button") ? (gi("#" + t + "bt-togglePdos").addClass("button-white"), gi("#" + t + "bt-togglePdos").removeClass("button"), F(!0)) : (gi("#" + t + "bt-togglePdos").addClass("button"), gi("#" + t + "bt-togglePdos").removeClass("button-white"), F(!1)), d.myDos.update()
+        l.addDos(i), n.length ? l.updateDosPlot("vertical") : l.updateDosPlot("horizontal");
+        var C = document.getElementById(t + "bt-togglePdos");
+        C.onclick = function() {
+            C.classList.contains("button") ? (gi("#" + t + "bt-togglePdos").addClass("button-white"), gi("#" + t + "bt-togglePdos").removeClass("button"), P(!0)) : (gi("#" + t + "bt-togglePdos").addClass("button"), gi("#" + t + "bt-togglePdos").removeClass("button-white"), P(!1)), l.myDos.update()
         };
-        var S = document.getElementById(t + "bt-downloadFigure");
-        S.onclick = function() {
-            var V = document.createElement("a");
+        var x = document.getElementById(t + "bt-downloadFigure");
+        x.onclick = function() {
+            var h = document.createElement("a");
             if (n.length) {
-                var te = document.createElement("a");
-                V.href = d.myDos.toBase64Image("dos.png", 1), te.href = d.myChart.toBase64Image("bandstructure.png", 1), V.download = "dos.png", te.download = "bandstructure.png", te.click()
-            } else V.href = d.myDos.toBase64Image("dos.png", 1), V.download = "dos.png";
-            V.click()
+                var $ = document.createElement("a");
+                h.href = l.myDos.toBase64Image("dos.png", 1), $.href = l.myChart.toBase64Image("bandstructure.png", 1), h.download = "dos.png", $.download = "bandstructure.png", $.click()
+            } else h.href = l.myDos.toBase64Image("dos.png", 1), h.download = "dos.png";
+            h.click()
         };
-        var A = document.getElementById(t + "bt-downloadJson");
-        A.onclick = function() {
-            var V = document.createElement("a");
-            n.length ? (n.forEach(function(te, ie) {
-                V.href = "data:text/json;charset=utf-8," + encodeURIComponent(JSON.stringify(te)), V.download = "bandData" + ie + ".json", V.click()
-            }), V.href = "data:text/json;charset=utf-8," + encodeURIComponent(JSON.stringify(i)), V.download = "dosData.json", V.click()) : (V.href = "data:text/json;charset=utf-8," + encodeURIComponent(JSON.stringify(i)), V.download = "dosData.json", V.click())
-        }
-    }
-    a1[t].plotObj = d;
-    var C = document.getElementById(t + "bt-resetZoom");
-    C.onclick = function() {
-        n.length && d.resBandZoom(), !gi.isEmptyObject(i) && n.length && d.resDosZoom("vertical"), !gi.isEmptyObject(i) && !n.length && d.resDosZoom("horizontal"), console.log(d)
-    };
-    var M = document.getElementById(t + "bt-dragPan");
-    M.onclick = function() {
-        H2(d, n, i)
-    };
-    var z = document.getElementById(t + "bt-dragZoom");
-    return z.onclick = function() {
-        j2(d, n, i)
-    }, console.log("end time: plotting band plot: current time, total time => ", t, window.performance.now(), window.performance.now() - c), d
+        var _ = document.getElementById(t + "bt-downloadJson");
+        _.onclick = function() {
+            var h = document.createElement("a");
+            n.length ? (n.forEach(function($, Y) {
+                h.href = "data:text/json;charset=utf-8," + encodeURIComponent(JSON.stringify($)), h.download = "bandData" + Y + ".json", h.click()
+            }), h.href = "data:text/json;charset=utf-8," + encodeURIComponent(JSON.stringify(i)), h.download = "dosData.json", h.click()) : (h.href = "data:text/json;charset=utf-8," + encodeURIComponent(JSON.stringify(i)), h.download = "dosData.json", h.click())
+        }
+    }
+    a1[t].plotObj = l;
+    var A = document.getElementById(t + "bt-resetZoom");
+    A.onclick = function() {
+        n.length && l.resBandZoom(), !gi.isEmptyObject(i) && n.length && l.resDosZoom("vertical"), !gi.isEmptyObject(i) && !n.length && l.resDosZoom("horizontal")
+    };
+    var w = document.getElementById(t + "bt-dragPan");
+    w.onclick = function() {
+        H2(l, n, i)
+    };
+    var k = document.getElementById(t + "bt-dragZoom");
+    return k.onclick = function() {
+        j2(l, n, i)
+    }, l
 }
 
 function h1(t) {
     var e = Math.random().toString(16).slice(2),
         n = Math.random().toString(16).slice(2),
-        i = null,
-        r = t.bandsDataList.length > 0,
-        o = t.dosData != null || t.dosData != null,
+        i = (0, Bs.useRef)(null),
+        r = !(!t.bandsDataList || t.bandsDataList.length == 0),
+        o = !(!t.dosData || Object.keys(t.dosData).length === 0),
         s = r && o;
-    (0, wf.useEffect)(() => (i = B2(e, n, t.bandsDataList, t.dosData, t.showFermi, t.showLegend, t.yLimit, t.dosRange, t.colorInfo), () => {
+    (0, Bs.useEffect)(() => (i = B2(e, n, r ? t.bandsDataList : [], t.dosData, t.energyRange, t.dosRange, t.bandsColorInfo, t.formatSettings), () => {
         r && i.myChart.destroy(), o && i.myDos.destroy()
-    }), []);
+    }), [t]);
     var a = null,
         l = null,
         c = null,
         d = null,
         g = null;
     return r && (a = bt.jsx("div", {
         id: `bandsplot-${e}-div`,
@@ -23728,16 +23725,16 @@
                 children: "Download json"
             })]
         })]
     })
 }
 Fn.register(...r1);
 var Lg = Fn;
-var Bs = fa(p1());
-var Nl = t => t && t.enabled && t.modifierKey,
+var Ws = da(p1());
+var zl = t => t && t.enabled && t.modifierKey,
     w1 = (t, e) => t && e[t + "Key"],
     Hg = (t, e) => t && !e[t + "Key"];
 
 function Xr(t, e, n) {
     return t === void 0 ? !0 : typeof t == "string" ? t.indexOf(e) !== -1 : typeof t == "function" ? t({
         chart: n
     }).indexOf(e) !== -1 : !1
@@ -23771,27 +23768,27 @@
     for (let o = 0; o < r.length; o++) {
         let s = i[r[o]];
         if (e >= s.top && e <= s.bottom && t >= s.left && t <= s.right) return s
     }
     return null
 }
 
-function k1(t, e, n) {
+function S1(t, e, n) {
     let {
         mode: i = "xy",
         scaleMode: r,
         overScaleMode: o
     } = t || {}, s = V2(e, n), a = Rg(i, n), l = Rg(r, n);
     if (o) {
         let d = Rg(o, n);
         for (let g of ["x", "y"]) d[g] && (l[g] = a[g], a[g] = !1)
     }
     if (s && l[s.axis]) return [s];
     let c = [];
-    return Se(n.scales, function(d) {
+    return ke(n.scales, function(d) {
         a[d.axis] && c.push(d)
     }), c
 }
 var Ig = new WeakMap;
 
 function _t(t) {
     let e = Ig.get(t);
@@ -23803,15 +23800,15 @@
     }, Ig.set(t, e)), e
 }
 
 function U2(t) {
     Ig.delete(t)
 }
 
-function S1(t, e, n) {
+function k1(t, e, n) {
     let i = t.max - t.min,
         r = i * (e - 1),
         o = t.isHorizontal() ? n.x : n.y,
         s = Math.max(0, Math.min(1, (t.getValueForPixel(o) - t.min) / i || 0)),
         a = 1 - s;
     return {
         min: r * s,
@@ -23833,15 +23830,15 @@
         r = t.getValueForPixel(n);
     return {
         min: Math.min(i, r),
         max: Math.max(i, r)
     }
 }
 
-function Ws(t, {
+function Vs(t, {
     min: e,
     max: n
 }, i, r = !1) {
     let o = _t(t.chart),
         {
             id: s,
             axis: a,
@@ -23850,70 +23847,70 @@
         c = i && (i[s] || i[a]) || {},
         {
             minRange: d = 0
         } = c,
         g = g1(o, t, c, "min", -1 / 0),
         y = g1(o, t, c, "max", 1 / 0),
         x = r ? Math.max(n - e, d) : t.max - t.min,
-        w = (x - n + e) / 2;
-    return e -= w, n += w, e < g ? (e = g, n = Math.min(g + x, y)) : n > y && (n = y, e = Math.max(y - x, g)), l.min = e, l.max = n, o.updatedScaleLimits[t.id] = {
+        _ = (x - n + e) / 2;
+    return e -= _, n += _, e < g ? (e = g, n = Math.min(g + x, y)) : n > y && (n = y, e = Math.max(y - x, g)), l.min = e, l.max = n, o.updatedScaleLimits[t.id] = {
         min: e,
         max: n
     }, t.parse(e) !== t.min || t.parse(n) !== t.max
 }
 
 function Y2(t, e, n, i) {
-    let r = S1(t, e, n),
+    let r = k1(t, e, n),
         o = {
             min: t.min + r.min,
             max: t.max - r.max
         };
-    return Ws(t, o, i, !0)
+    return Vs(t, o, i, !0)
 }
 
 function X2(t, e, n, i) {
-    Ws(t, $2(t, e, n), i, !0)
+    Vs(t, $2(t, e, n), i, !0)
 }
 var m1 = t => t === 0 || isNaN(t) ? 0 : t < 0 ? Math.min(Math.round(t), -1) : Math.max(Math.round(t), 1);
 
 function q2(t) {
     let n = t.getLabels().length - 1;
     t.min > 0 && (t.min -= 1), t.max < n && (t.max += 1)
 }
 
 function Z2(t, e, n, i) {
-    let r = S1(t, e, n);
+    let r = k1(t, e, n);
     t.min === t.max && e < 1 && q2(t);
     let o = {
         min: t.min + m1(r.min),
         max: t.max - m1(r.max)
     };
-    return Ws(t, o, i, !0)
+    return Vs(t, o, i, !0)
 }
 
-function G2(t) {
+function K2(t) {
     return t.isHorizontal() ? t.width : t.height
 }
 
-function Q2(t, e, n) {
+function G2(t, e, n) {
     let r = t.getLabels().length - 1,
         {
             min: o,
             max: s
         } = t,
         a = Math.max(s - o, 1),
-        l = Math.round(G2(t) / Math.max(a, 10)),
+        l = Math.round(K2(t) / Math.max(a, 10)),
         c = Math.round(Math.abs(e / l)),
         d;
-    return e < -l ? (s = Math.min(s + c, r), o = a === 1 ? s : s - a, d = s === r) : e > l && (o = Math.max(0, o - c), s = a === 1 ? o : o + a, d = o === 0), Ws(t, {
+    return e < -l ? (s = Math.min(s + c, r), o = a === 1 ? s : s - a, d = s === r) : e > l && (o = Math.max(0, o - c), s = a === 1 ? o : o + a, d = o === 0), Vs(t, {
         min: o,
         max: s
     }, n) || d
 }
-var K2 = {
+var Q2 = {
     second: 500,
     minute: 30 * 1e3,
     hour: 30 * 60 * 1e3,
     day: 12 * 60 * 60 * 1e3,
     week: 3.5 * 24 * 60 * 60 * 1e3,
     month: 15 * 24 * 60 * 60 * 1e3,
     quarter: 60 * 24 * 60 * 60 * 1e3,
@@ -23921,19 +23918,19 @@
 };
 
 function C1(t, e, n, i = !1) {
     let {
         min: r,
         max: o,
         options: s
-    } = t, a = s.time && s.time.round, l = K2[a] || 0, c = t.getValueForPixel(t.getPixelForValue(r + l) - e), d = t.getValueForPixel(t.getPixelForValue(o + l) - e), {
+    } = t, a = s.time && s.time.round, l = Q2[a] || 0, c = t.getValueForPixel(t.getPixelForValue(r + l) - e), d = t.getValueForPixel(t.getPixelForValue(o + l) - e), {
         min: g = -1 / 0,
         max: y = 1 / 0
     } = i && n && n[t.axis] || {};
-    return isNaN(c) || isNaN(d) || c < g || d > y ? !0 : Ws(t, {
+    return isNaN(c) || isNaN(d) || c < g || d > y ? !0 : Vs(t, {
         min: c,
         max: d
     }, n, i)
 }
 
 function y1(t, e, n) {
     return C1(t, e, n, !0)
@@ -23942,15 +23939,15 @@
         category: Z2,
         default: Y2
     },
     zg = {
         default: X2
     },
     Fg = {
-        category: Q2,
+        category: G2,
         default: C1,
         logarithmic: y1,
         timeseries: y1
     };
 
 function J2(t, e, n) {
     let {
@@ -23962,27 +23959,27 @@
     } = t;
     if (!e[i] || !n[i]) return !0;
     let s = n[i];
     return s.min !== r || s.max !== o
 }
 
 function v1(t, e) {
-    Se(t, (n, i) => {
+    ke(t, (n, i) => {
         e[i] || delete t[i]
     })
 }
 
-function Vs(t, e) {
+function Us(t, e) {
     let {
         scales: n
     } = t, {
         originalScaleLimits: i,
         updatedScaleLimits: r
     } = e;
-    return Se(n, function(o) {
+    return ke(n, function(o) {
         J2(o, i, r) && (i[o.id] = {
             min: {
                 scale: o.min,
                 options: o.options.min
             },
             max: {
                 scale: o.max,
@@ -23998,41 +23995,41 @@
 }
 
 function b1(t, e, n, i, r) {
     let o = zg[t.type] || zg.default;
     ve(o, [t, e, n, i, r])
 }
 
-function eP(t) {
+function eD(t) {
     let e = t.chartArea;
     return {
         x: (e.left + e.right) / 2,
         y: (e.top + e.bottom) / 2
     }
 }
 
 function Bg(t, e, n = "none") {
     let {
         x: i = 1,
         y: r = 1,
-        focalPoint: o = eP(t)
+        focalPoint: o = eD(t)
     } = typeof e == "number" ? {
         x: e,
         y: e
     } : e, s = _t(t), {
         options: {
             limits: a,
             zoom: l
         }
     } = s;
-    Vs(t, s);
+    Us(t, s);
     let c = i !== 1,
         d = r !== 1,
-        g = k1(l, o, t);
-    Se(g || t.scales, function(y) {
+        g = S1(l, o, t);
+    ke(g || t.scales, function(y) {
         y.isHorizontal() && c ? x1(y, i, o, a) : !y.isHorizontal() && d && x1(y, r, o, a)
     }), t.update(n), ve(l.onZoom, [{
         chart: t
     }])
 }
 
 function E1(t, e, n, i = "none") {
@@ -24042,57 +24039,57 @@
                 limits: o,
                 zoom: s
             }
         } = r,
         {
             mode: a = "xy"
         } = s;
-    Vs(t, r);
+    Us(t, r);
     let l = Xr(a, "x", t),
         c = Xr(a, "y", t);
-    Se(t.scales, function(d) {
+    ke(t.scales, function(d) {
         d.isHorizontal() && l ? b1(d, e.x, n.x, o) : !d.isHorizontal() && c && b1(d, e.y, n.y, o)
     }), t.update(i), ve(s.onZoom, [{
         chart: t
     }])
 }
 
-function tP(t, e, n, i = "none") {
-    Vs(t, _t(t));
+function tD(t, e, n, i = "none") {
+    Us(t, _t(t));
     let r = t.scales[e];
-    Ws(r, n, void 0, !0), t.update(i)
+    Vs(r, n, void 0, !0), t.update(i)
 }
 
-function nP(t, e = "default") {
+function nD(t, e = "default") {
     let n = _t(t),
-        i = Vs(t, n);
-    Se(t.scales, function(r) {
+        i = Us(t, n);
+    ke(t.scales, function(r) {
         let o = r.options;
         i[r.id] ? (o.min = i[r.id].min.options, o.max = i[r.id].max.options) : (delete o.min, delete o.max)
     }), t.update(e), ve(n.options.zoom.onZoomComplete, [{
         chart: t
     }])
 }
 
-function iP(t, e) {
+function iD(t, e) {
     let n = t.originalScaleLimits[e];
     if (!n) return;
     let {
         min: i,
         max: r
     } = n;
     return pe(r.options, r.scale) - pe(i.options, i.scale)
 }
 
-function rP(t) {
+function rD(t) {
     let e = _t(t),
         n = 1,
         i = 1;
-    return Se(t.scales, function(r) {
-        let o = iP(e, r.id);
+    return ke(t.scales, function(r) {
+        let o = iD(e, r.id);
         if (o) {
             let s = Math.round(o / (r.max - r.min) * 100) / 100;
             n = Math.min(n, s), i = Math.max(i, s)
         }
     }), n < 1 ? n : i
 }
 
@@ -24116,27 +24113,27 @@
         options: {
             pan: a,
             limits: l
         }
     } = s, {
         onPan: c
     } = a || {};
-    Vs(t, s);
+    Us(t, s);
     let d = r !== 0,
         g = o !== 0;
-    Se(n || t.scales, function(y) {
+    ke(n || t.scales, function(y) {
         y.isHorizontal() && d ? _1(y, r, l, s) : !y.isHorizontal() && g && _1(y, o, l, s)
     }), t.update(i), ve(c, [{
         chart: t
     }])
 }
 
-function P1(t) {
+function D1(t) {
     let e = _t(t);
-    Vs(t, e);
+    Us(t, e);
     let n = {};
     for (let i of Object.keys(t.scales)) {
         let {
             min: r,
             max: o
         } = e.originalScaleLimits[i] || {
             min: {},
@@ -24146,52 +24143,52 @@
             min: r.scale,
             max: o.scale
         }
     }
     return n
 }
 
-function oP(t) {
-    let e = P1(t);
+function oD(t) {
+    let e = D1(t);
     for (let n of Object.keys(t.scales)) {
         let {
             min: i,
             max: r
         } = e[n];
         if (i !== void 0 && t.scales[n].min !== i || r !== void 0 && t.scales[n].max !== r) return !0
     }
     return !1
 }
 
-function kn(t, e) {
+function Sn(t, e) {
     let {
         handlers: n
     } = _t(t), i = n[e];
     i && i.target && (i.target.removeEventListener(e, i), delete n[e])
 }
 
-function Il(t, e, n, i) {
+function Nl(t, e, n, i) {
     let {
         handlers: r,
         options: o
     } = _t(t), s = r[n];
-    s && s.target === e || (kn(t, n), r[n] = a => i(t, a, o), r[n].target = e, e.addEventListener(n, r[n]))
+    s && s.target === e || (Sn(t, n), r[n] = a => i(t, a, o), r[n].target = e, e.addEventListener(n, r[n]))
 }
 
-function sP(t, e) {
+function sD(t, e) {
     let n = _t(t);
     n.dragStart && (n.dragging = !0, n.dragEnd = e, t.update("none"))
 }
 
-function aP(t, e) {
+function aD(t, e) {
     let n = _t(t);
-    !n.dragStart || e.key !== "Escape" || (kn(t, "keydown"), n.dragging = !1, n.dragStart = n.dragEnd = null, t.update("none"))
+    !n.dragStart || e.key !== "Escape" || (Sn(t, "keydown"), n.dragging = !1, n.dragStart = n.dragEnd = null, t.update("none"))
 }
 
-function M1(t, e, n) {
+function P1(t, e, n) {
     let {
         onZoomStart: i,
         onZoomRejected: r
     } = n;
     if (i) {
         let o = zn(e, t);
         if (ve(i, [{
@@ -24201,66 +24198,66 @@
             }]) === !1) return ve(r, [{
             chart: t,
             event: e
         }]), !1
     }
 }
 
-function lP(t, e) {
+function lD(t, e) {
     let n = _t(t),
         {
             pan: i,
             zoom: r = {}
         } = n.options;
-    if (e.button !== 0 || w1(Nl(i), e) || Hg(Nl(r.drag), e)) return ve(r.onZoomRejected, [{
+    if (e.button !== 0 || w1(zl(i), e) || Hg(zl(r.drag), e)) return ve(r.onZoomRejected, [{
         chart: t,
         event: e
     }]);
-    M1(t, e, r) !== !1 && (n.dragStart = e, Il(t, t.canvas, "mousemove", sP), Il(t, window.document, "keydown", aP))
+    P1(t, e, r) !== !1 && (n.dragStart = e, Nl(t, t.canvas, "mousemove", sD), Nl(t, window.document, "keydown", aD))
 }
 
-function D1(t, e, n, i) {
+function M1(t, e, n, i) {
     let r = Xr(e, "x", t),
         o = Xr(e, "y", t),
         {
             top: s,
             left: a,
             right: l,
             bottom: c,
             width: d,
             height: g
         } = t.chartArea,
         y = zn(n, t),
         x = zn(i, t);
     r && (a = Math.min(y.x, x.x), l = Math.max(y.x, x.x)), o && (s = Math.min(y.y, x.y), c = Math.max(y.y, x.y));
-    let w = l - a,
-        S = c - s;
+    let _ = l - a,
+        C = c - s;
     return {
         left: a,
         top: s,
         right: l,
         bottom: c,
-        width: w,
-        height: S,
-        zoomX: r && w ? 1 + (d - w) / d : 1,
-        zoomY: o && S ? 1 + (g - S) / g : 1
+        width: _,
+        height: C,
+        zoomX: r && _ ? 1 + (d - _) / d : 1,
+        zoomY: o && C ? 1 + (g - C) / g : 1
     }
 }
 
-function uP(t, e) {
+function uD(t, e) {
     let n = _t(t);
     if (!n.dragStart) return;
-    kn(t, "mousemove");
+    Sn(t, "mousemove");
     let {
         mode: i,
         onZoomComplete: r,
         drag: {
             threshold: o = 0
         }
-    } = n.options.zoom, s = D1(t, i, n.dragStart, e), a = Xr(i, "x", t) ? s.width : 0, l = Xr(i, "y", t) ? s.height : 0, c = Math.sqrt(a * a + l * l);
+    } = n.options.zoom, s = M1(t, i, n.dragStart, e), a = Xr(i, "x", t) ? s.width : 0, l = Xr(i, "y", t) ? s.height : 0, c = Math.sqrt(a * a + l * l);
     if (n.dragStart = n.dragEnd = null, c <= o) {
         n.dragging = !1, t.update("none");
         return
     }
     E1(t, {
         x: s.left,
         y: s.top
@@ -24268,84 +24265,84 @@
         x: s.right,
         y: s.bottom
     }, "zoom"), setTimeout(() => n.dragging = !1, 500), ve(r, [{
         chart: t
     }])
 }
 
-function cP(t, e, n) {
-    if (Hg(Nl(n.wheel), e)) {
+function cD(t, e, n) {
+    if (Hg(zl(n.wheel), e)) {
         ve(n.onZoomRejected, [{
             chart: t,
             event: e
         }]);
         return
     }
-    if (M1(t, e, n) !== !1 && (e.cancelable && e.preventDefault(), e.deltaY !== void 0)) return !0
+    if (P1(t, e, n) !== !1 && (e.cancelable && e.preventDefault(), e.deltaY !== void 0)) return !0
 }
 
-function fP(t, e) {
+function fD(t, e) {
     let {
         handlers: {
             onZoomComplete: n
         },
         options: {
             zoom: i
         }
     } = _t(t);
-    if (!cP(t, e, i)) return;
+    if (!cD(t, e, i)) return;
     let r = e.target.getBoundingClientRect(),
         o = 1 + (e.deltaY >= 0 ? -i.wheel.speed : i.wheel.speed),
         s = {
             x: o,
             y: o,
             focalPoint: {
                 x: e.clientX - r.left,
                 y: e.clientY - r.top
             }
         };
     Bg(t, s), n && n()
 }
 
-function dP(t, e, n, i) {
+function dD(t, e, n, i) {
     n && (_t(t).handlers[e] = W2(() => ve(n, [{
         chart: t
     }]), i))
 }
 
-function hP(t, e) {
+function hD(t, e) {
     let n = t.canvas,
         {
             wheel: i,
             drag: r,
             onZoomComplete: o
         } = e.zoom;
-    i.enabled ? (Il(t, n, "wheel", fP), dP(t, "onZoomComplete", o, 250)) : kn(t, "wheel"), r.enabled ? (Il(t, n, "mousedown", lP), Il(t, n.ownerDocument, "mouseup", uP)) : (kn(t, "mousedown"), kn(t, "mousemove"), kn(t, "mouseup"), kn(t, "keydown"))
+    i.enabled ? (Nl(t, n, "wheel", fD), dD(t, "onZoomComplete", o, 250)) : Sn(t, "wheel"), r.enabled ? (Nl(t, n, "mousedown", lD), Nl(t, n.ownerDocument, "mouseup", uD)) : (Sn(t, "mousedown"), Sn(t, "mousemove"), Sn(t, "mouseup"), Sn(t, "keydown"))
 }
 
-function pP(t) {
-    kn(t, "mousedown"), kn(t, "mousemove"), kn(t, "mouseup"), kn(t, "wheel"), kn(t, "click"), kn(t, "keydown")
+function pD(t) {
+    Sn(t, "mousedown"), Sn(t, "mousemove"), Sn(t, "mouseup"), Sn(t, "wheel"), Sn(t, "click"), Sn(t, "keydown")
 }
 
-function gP(t, e) {
+function gD(t, e) {
     return function(n, i) {
         let {
             pan: r,
             zoom: o = {}
         } = e.options;
         if (!r || !r.enabled) return !1;
         let s = i && i.srcEvent;
-        return s && !e.panning && i.pointerType === "mouse" && (Hg(Nl(r), s) || w1(Nl(o.drag), s)) ? (ve(r.onPanRejected, [{
+        return s && !e.panning && i.pointerType === "mouse" && (Hg(zl(r), s) || w1(zl(o.drag), s)) ? (ve(r.onPanRejected, [{
             chart: t,
             event: i
         }]), !1) : !0
     }
 }
 
-function mP(t, e) {
+function mD(t, e) {
     let n = Math.abs(t.clientX - e.clientX),
         i = Math.abs(t.clientY - e.clientY),
         r = n / i,
         o, s;
     return r > .3 && r < 1.7 ? o = s = !0 : n > i ? o = !0 : s = !0, {
         x: o,
         y: s
@@ -24353,31 +24350,31 @@
 }
 
 function O1(t, e, n) {
     if (e.scale) {
         let {
             center: i,
             pointers: r
-        } = n, o = 1 / e.scale * n.scale, s = n.target.getBoundingClientRect(), a = mP(r[0], r[1]), l = e.options.zoom.mode, c = {
+        } = n, o = 1 / e.scale * n.scale, s = n.target.getBoundingClientRect(), a = mD(r[0], r[1]), l = e.options.zoom.mode, c = {
             x: a.x && Xr(l, "x", t) ? o : 1,
             y: a.y && Xr(l, "y", t) ? o : 1,
             focalPoint: {
                 x: i.x - s.left,
                 y: i.y - s.top
             }
         };
         Bg(t, c), e.scale = n.scale
     }
 }
 
-function yP(t, e) {
+function yD(t, e) {
     e.options.zoom.pinch.enabled && (e.scale = 1)
 }
 
-function vP(t, e, n) {
+function vD(t, e, n) {
     e.scale && (O1(t, e, n), e.scale = null, ve(e.options.zoom.onZoomComplete, [{
         chart: t
     }]))
 }
 
 function A1(t, e, n) {
     let i = e.delta;
@@ -24386,15 +24383,15 @@
         y: n.deltaY - i.y
     }, e.panScales), e.delta = {
         x: n.deltaX,
         y: n.deltaY
     })
 }
 
-function xP(t, e, n) {
+function xD(t, e, n) {
     let {
         enabled: i,
         onPanStart: r,
         onPanRejected: o
     } = e.options.pan;
     if (!i) return;
     let s = n.target.getBoundingClientRect(),
@@ -24406,65 +24403,65 @@
             chart: t,
             event: n,
             point: a
         }]) === !1) return ve(o, [{
         chart: t,
         event: n
     }]);
-    e.panScales = k1(e.options.pan, a, t), e.delta = {
+    e.panScales = S1(e.options.pan, a, t), e.delta = {
         x: 0,
         y: 0
     }, clearTimeout(e.panEndTimeout), A1(t, e, n)
 }
 
-function bP(t, e) {
+function bD(t, e) {
     e.delta = null, e.panning && (e.panEndTimeout = setTimeout(() => e.panning = !1, 500), ve(e.options.pan.onPanComplete, [{
         chart: t
     }]))
 }
 var jg = new WeakMap;
 
-function _P(t, e) {
+function _D(t, e) {
     let n = _t(t),
         i = t.canvas,
         {
             pan: r,
             zoom: o
         } = e,
-        s = new Bs.default.Manager(i);
-    o && o.pinch.enabled && (s.add(new Bs.default.Pinch), s.on("pinchstart", () => yP(t, n)), s.on("pinch", a => O1(t, n, a)), s.on("pinchend", a => vP(t, n, a))), r && r.enabled && (s.add(new Bs.default.Pan({
+        s = new Ws.default.Manager(i);
+    o && o.pinch.enabled && (s.add(new Ws.default.Pinch), s.on("pinchstart", () => yD(t, n)), s.on("pinch", a => O1(t, n, a)), s.on("pinchend", a => vD(t, n, a))), r && r.enabled && (s.add(new Ws.default.Pan({
         threshold: r.threshold,
-        enable: gP(t, n)
-    })), s.on("panstart", a => xP(t, n, a)), s.on("panmove", a => A1(t, n, a)), s.on("panend", () => bP(t, n))), jg.set(t, s)
+        enable: gD(t, n)
+    })), s.on("panstart", a => xD(t, n, a)), s.on("panmove", a => A1(t, n, a)), s.on("panend", () => bD(t, n))), jg.set(t, s)
 }
 
-function wP(t) {
+function wD(t) {
     let e = jg.get(t);
     e && (e.remove("pinchstart"), e.remove("pinch"), e.remove("pinchend"), e.remove("panstart"), e.remove("pan"), e.remove("panend"), e.destroy(), jg.delete(t))
 }
-var kP = "2.0.1";
+var SD = "2.0.1";
 
 function Sf(t, e, n) {
     let i = n.zoom.drag,
         {
             dragStart: r,
             dragEnd: o
         } = _t(t);
     if (i.drawTime !== e || !o) return;
     let {
         left: s,
         top: a,
         width: l,
         height: c
-    } = D1(t, n.zoom.mode, r, o), d = t.ctx;
+    } = M1(t, n.zoom.mode, r, o), d = t.ctx;
     d.save(), d.beginPath(), d.fillStyle = i.backgroundColor || "rgba(225,225,225,0.3)", d.fillRect(s, a, l, c), i.borderWidth > 0 && (d.lineWidth = i.borderWidth, d.strokeStyle = i.borderColor || "rgba(225,225,225)", d.strokeRect(s, a, l, c)), d.restore()
 }
 var L1 = {
     id: "zoom",
-    version: kP,
+    version: SD,
     defaults: {
         pan: {
             enabled: !1,
             mode: "xy",
             threshold: 10,
             modifierKey: null
         },
@@ -24483,109 +24480,109 @@
                 enabled: !1
             },
             mode: "xy"
         }
     },
     start: function(t, e, n) {
         let i = _t(t);
-        i.options = n, Object.prototype.hasOwnProperty.call(n.zoom, "enabled") && console.warn("The option `zoom.enabled` is no longer supported. Please use `zoom.wheel.enabled`, `zoom.drag.enabled`, or `zoom.pinch.enabled`."), (Object.prototype.hasOwnProperty.call(n.zoom, "overScaleMode") || Object.prototype.hasOwnProperty.call(n.pan, "overScaleMode")) && console.warn("The option `overScaleMode` is deprecated. Please use `scaleMode` instead (and update `mode` as desired)."), Bs.default && _P(t, n), t.pan = (r, o, s) => T1(t, r, o, s), t.zoom = (r, o) => Bg(t, r, o), t.zoomRect = (r, o, s) => E1(t, r, o, s), t.zoomScale = (r, o, s) => tP(t, r, o, s), t.resetZoom = r => nP(t, r), t.getZoomLevel = () => rP(t), t.getInitialScaleBounds = () => P1(t), t.isZoomedOrPanned = () => oP(t)
+        i.options = n, Object.prototype.hasOwnProperty.call(n.zoom, "enabled") && console.warn("The option `zoom.enabled` is no longer supported. Please use `zoom.wheel.enabled`, `zoom.drag.enabled`, or `zoom.pinch.enabled`."), (Object.prototype.hasOwnProperty.call(n.zoom, "overScaleMode") || Object.prototype.hasOwnProperty.call(n.pan, "overScaleMode")) && console.warn("The option `overScaleMode` is deprecated. Please use `scaleMode` instead (and update `mode` as desired)."), Ws.default && _D(t, n), t.pan = (r, o, s) => T1(t, r, o, s), t.zoom = (r, o) => Bg(t, r, o), t.zoomRect = (r, o, s) => E1(t, r, o, s), t.zoomScale = (r, o, s) => tD(t, r, o, s), t.resetZoom = r => nD(t, r), t.getZoomLevel = () => rD(t), t.getInitialScaleBounds = () => D1(t), t.isZoomedOrPanned = () => oD(t)
     },
     beforeEvent(t) {
         let e = _t(t);
         if (e.panning || e.dragging) return !1
     },
     beforeUpdate: function(t, e, n) {
         let i = _t(t);
-        i.options = n, hP(t, n)
+        i.options = n, hD(t, n)
     },
     beforeDatasetsDraw(t, e, n) {
         Sf(t, "beforeDatasetsDraw", n)
     },
     afterDatasetsDraw(t, e, n) {
         Sf(t, "afterDatasetsDraw", n)
     },
     beforeDraw(t, e, n) {
         Sf(t, "beforeDraw", n)
     },
     afterDraw(t, e, n) {
         Sf(t, "afterDraw", n)
     },
     stop: function(t) {
-        pP(t), Bs.default && wP(t), U2(t)
+        pD(t), Ws.default && wD(t), U2(t)
     },
     panFunctions: Fg,
     zoomFunctions: Ng,
     zoomRectFunctions: zg
 };
 var R1 = {
     modes: {
         point(t, e) {
-            return Tf(t, e, {
+            return Ef(t, e, {
                 intersect: !0
             })
         },
         nearest(t, e, n) {
-            return EP(t, e, n)
+            return ED(t, e, n)
         },
         x(t, e, n) {
-            return Tf(t, e, {
+            return Ef(t, e, {
                 intersect: n.intersect,
                 axis: "x"
             })
         },
         y(t, e, n) {
-            return Tf(t, e, {
+            return Ef(t, e, {
                 intersect: n.intersect,
                 axis: "y"
             })
         }
     }
 };
 
-function Gg(t, e, n) {
+function Kg(t, e, n) {
     return (R1.modes[n.mode] || R1.modes.nearest)(t, e, n)
 }
 
-function SP(t, e, n) {
+function kD(t, e, n) {
     return n !== "x" && n !== "y" ? t.inRange(e.x, e.y, "x", !0) || t.inRange(e.x, e.y, "y", !0) : t.inRange(e.x, e.y, n, !0)
 }
 
-function CP(t, e, n) {
+function CD(t, e, n) {
     return n === "x" ? {
         x: t.x,
         y: e.y
     } : n === "y" ? {
         x: e.x,
         y: t.y
     } : e
 }
 
-function Tf(t, e, n) {
-    return t.visibleElements.filter(i => n.intersect ? i.inRange(e.x, e.y) : SP(i, e, n.axis))
+function Ef(t, e, n) {
+    return t.visibleElements.filter(i => n.intersect ? i.inRange(e.x, e.y) : kD(i, e, n.axis))
 }
 
-function EP(t, e, n) {
+function ED(t, e, n) {
     let i = Number.POSITIVE_INFINITY;
-    return Tf(t, e, n).reduce((r, o) => {
+    return Ef(t, e, n).reduce((r, o) => {
         let s = o.getCenterPoint(),
-            a = CP(e, s, n.axis),
+            a = CD(e, s, n.axis),
             l = tr(e, a);
         return l < i ? (r = [o], i = l) : l === i && r.push(o), r
     }, []).sort((r, o) => r._index - o._index).slice(0, 1)
 }
-var TP = (t, e) => e > t || t.length > e.length && t.slice(0, e.length) === e,
+var TD = (t, e) => e > t || t.length > e.length && t.slice(0, e.length) === e,
     jo = .001,
-    Mf = (t, e, n) => Math.min(n, Math.max(e, t));
+    Df = (t, e, n) => Math.min(n, Math.max(e, t));
 
-function PP(t, e, n) {
-    for (let i of Object.keys(t)) t[i] = Mf(t[i], e, n);
+function DD(t, e, n) {
+    for (let i of Object.keys(t)) t[i] = Df(t[i], e, n);
     return t
 }
 
-function MP(t, e, n, i) {
+function PD(t, e, n, i) {
     if (!t || !e || n <= 0) return !1;
     let r = i / 2;
     return Math.pow(t.x - e.x, 2) + Math.pow(t.y - e.y, 2) <= Math.pow(n + r, 2)
 }
 
 function J1(t, {
     x: e,
@@ -24595,238 +24592,238 @@
 }, o, s) {
     let a = s / 2,
         l = t.x >= e - a - jo && t.x <= i + a + jo,
         c = t.y >= n - a - jo && t.y <= r + a + jo;
     return o === "x" ? l : (o === "y" || l) && c
 }
 
-function Xs(t, e) {
+function qs(t, e) {
     let {
         centerX: n,
         centerY: i
     } = t.getProps(["centerX", "centerY"], e);
     return {
         x: n,
         y: i
     }
 }
 
-function DP(t, e, n, i = !0) {
+function MD(t, e, n, i = !0) {
     let r = n.split("."),
         o = 0;
     for (let s of e.split(".")) {
         let a = r[o++];
         if (parseInt(s, 10) < parseInt(a, 10)) break;
-        if (TP(a, s)) {
+        if (TD(a, s)) {
             if (i) throw new Error(`${t} v${n} is not supported. v${e} or newer is required.`);
             return !1
         }
     }
     return !0
 }
 var e_ = t => typeof t == "string" && t.endsWith("%"),
     t_ = t => parseFloat(t) / 100,
-    n_ = t => Mf(t_(t), 0, 1),
-    Cf = (t, e) => ({
+    n_ = t => Df(t_(t), 0, 1),
+    kf = (t, e) => ({
         x: t,
         y: e,
         x2: t,
         y2: e,
         width: 0,
         height: 0
     }),
-    OP = {
-        box: t => Cf(t.centerX, t.centerY),
+    OD = {
+        box: t => kf(t.centerX, t.centerY),
         ellipse: t => ({
             centerX: t.centerX,
             centerY: t.centerX,
             radius: 0,
             width: 0,
             height: 0
         }),
-        label: t => Cf(t.centerX, t.centerY),
-        line: t => Cf(t.x, t.y),
+        label: t => kf(t.centerX, t.centerY),
+        line: t => kf(t.x, t.y),
         point: t => ({
             centerX: t.centerX,
             centerY: t.centerY,
             radius: 0,
             width: 0,
             height: 0
         }),
-        polygon: t => Cf(t.centerX, t.centerY)
+        polygon: t => kf(t.centerX, t.centerY)
     };
 
-function Qg(t, e) {
+function Gg(t, e) {
     return e === "start" ? 0 : e === "end" ? t : e_(e) ? n_(e) * t : t / 2
 }
 
-function Gr(t, e, n = !0) {
+function Kr(t, e, n = !0) {
     return typeof e == "number" ? e : e_(e) ? (n ? n_(e) : t_(e)) * t : t
 }
 
-function AP(t, e) {
+function AD(t, e) {
     let {
         x: n,
         width: i
     } = t, r = e.textAlign;
     return r === "center" ? n + i / 2 : r === "end" || r === "right" ? n + i : n
 }
 
-function Kg(t, e = "center") {
+function Qg(t, e = "center") {
     return we(t) ? {
         x: pe(t.x, e),
         y: pe(t.y, e)
     } : (t = pe(t, e), {
         x: t,
         y: t
     })
 }
 
 function i_(t) {
     return t && (Ut(t.xValue) || Ut(t.yValue))
 }
 
-function Fl(t, e, n) {
+function jl(t, e, n) {
     let i = n.init;
     if (i) {
         if (i === !0) return o_(e, n)
     } else return;
-    return LP(t, e, n)
+    return LD(t, e, n)
 }
 
 function r_(t, e, n) {
     let i = !1;
     return e.forEach(r => {
         Vt(t[r]) ? (i = !0, n[r] = t[r]) : Ut(n[r]) && delete n[r]
     }), i
 }
 
 function o_(t, e) {
     let n = e.type || "line";
-    return OP[n](t)
+    return OD[n](t)
 }
 
-function LP(t, e, n) {
+function LD(t, e, n) {
     let i = ve(n.init, [{
         chart: t,
         properties: e,
         options: n
     }]);
     if (i === !0) return o_(e, n);
     if (we(i)) return i
 }
 var Wg = new Map,
-    RP = t => isNaN(t) || t <= 0,
-    IP = t => t.reduce(function(e, n) {
+    RD = t => isNaN(t) || t <= 0,
+    ID = t => t.reduce(function(e, n) {
         return e += n.string, e
     }, "");
 
-function Df(t) {
+function Pf(t) {
     if (t && typeof t == "object") {
         let e = t.toString();
         return e === "[object HTMLImageElement]" || e === "[object HTMLCanvasElement]"
     }
 }
 
 function Jg(t, {
     x: e,
     y: n
 }, i) {
     i && (t.translate(e, n), t.rotate(pt(i)), t.translate(-e, -n))
 }
 
-function Qr(t, e) {
+function Gr(t, e) {
     if (e && e.borderWidth) return t.lineCap = e.borderCapStyle, t.setLineDash(e.borderDash), t.lineDashOffset = e.borderDashOffset, t.lineJoin = e.borderJoinStyle, t.lineWidth = e.borderWidth, t.strokeStyle = e.borderColor, !0
 }
 
-function qs(t, e) {
+function Zs(t, e) {
     t.shadowColor = e.backgroundShadowColor, t.shadowBlur = e.shadowBlur, t.shadowOffsetX = e.shadowOffsetX, t.shadowOffsetY = e.shadowOffsetY
 }
 
 function em(t, e) {
     let n = e.content;
-    if (Df(n)) return {
-        width: Gr(n.width, e.width),
-        height: Gr(n.height, e.height)
+    if (Pf(n)) return {
+        width: Kr(n.width, e.width),
+        height: Kr(n.height, e.height)
     };
     let i = e.font,
         r = Re(i) ? i.map(l => tt(l)) : [tt(i)],
         o = e.textStrokeWidth,
         s = Re(n) ? n : [n],
-        a = s.join() + IP(r) + o + (t._measureText ? "-spriting" : "");
-    return Wg.has(a) || Wg.set(a, HP(t, s, r, o)), Wg.get(a)
+        a = s.join() + ID(r) + o + (t._measureText ? "-spriting" : "");
+    return Wg.has(a) || Wg.set(a, HD(t, s, r, o)), Wg.get(a)
 }
 
 function s_(t, e, n) {
     let {
         x: i,
         y: r,
         width: o,
         height: s
     } = e;
-    t.save(), qs(t, n);
-    let a = Qr(t, n);
+    t.save(), Zs(t, n);
+    let a = Gr(t, n);
     t.fillStyle = n.backgroundColor, t.beginPath(), rr(t, {
         x: i,
         y: r,
         w: o,
         h: s,
-        radius: PP(pi(n.borderRadius), 0, Math.min(o, s) / 2)
+        radius: DD(pi(n.borderRadius), 0, Math.min(o, s) / 2)
     }), t.closePath(), t.fill(), a && (t.shadowColor = n.borderShadowColor, t.stroke()), t.restore()
 }
 
-function NP(t, e, n) {
+function ND(t, e, n) {
     let i = n.content;
-    if (Df(i)) {
-        t.save(), t.globalAlpha = VP(n.opacity, i.style.opacity), t.drawImage(i, e.x, e.y, e.width, e.height), t.restore();
+    if (Pf(i)) {
+        t.save(), t.globalAlpha = VD(n.opacity, i.style.opacity), t.drawImage(i, e.x, e.y, e.width, e.height), t.restore();
         return
     }
     let r = Re(i) ? i : [i],
         o = n.font,
         s = Re(o) ? o.map(g => tt(g)) : [tt(o)],
         a = n.color,
         l = Re(a) ? a : [a],
-        c = AP(e, n),
+        c = AD(e, n),
         d = e.y + n.textStrokeWidth / 2;
-    t.save(), t.textBaseline = "middle", t.textAlign = n.textAlign, zP(t, n) && BP(t, {
+    t.save(), t.textBaseline = "middle", t.textAlign = n.textAlign, zD(t, n) && BD(t, {
         x: c,
         y: d
-    }, r, s), WP(t, {
+    }, r, s), WD(t, {
         x: c,
         y: d
     }, r, {
         fonts: s,
         colors: l
     }), t.restore()
 }
 
-function zP(t, e) {
+function zD(t, e) {
     if (e.textStrokeWidth > 0) return t.lineJoin = "round", t.miterLimit = 2, t.lineWidth = e.textStrokeWidth, t.strokeStyle = e.textStrokeColor, !0
 }
 
-function FP(t, e, n, i) {
+function FD(t, e, n, i) {
     let {
         radius: r,
         options: o
-    } = e, s = o.pointStyle, a = o.rotation, l = (a || 0) * dl;
-    if (Df(s)) {
+    } = e, s = o.pointStyle, a = o.rotation, l = (a || 0) * hl;
+    if (Pf(s)) {
         t.save(), t.translate(n, i), t.rotate(l), t.drawImage(s, -s.width / 2, -s.height / 2, s.width, s.height), t.restore();
         return
     }
-    RP(r) || jP(t, {
+    RD(r) || jD(t, {
         x: n,
         y: i,
         radius: r,
         rotation: a,
         style: s,
         rad: l
     })
 }
 
-function jP(t, {
+function jD(t, {
     x: e,
     y: n,
     radius: i,
     rotation: r,
     style: o,
     rad: s
 }) {
@@ -24864,15 +24861,15 @@
         case "dash":
             t.moveTo(e, n), t.lineTo(e + Math.cos(s) * i, n + Math.sin(s) * i);
             break
     }
     t.fill()
 }
 
-function HP(t, e, n, i) {
+function HD(t, e, n, i) {
     t.save();
     let r = e.length,
         o = 0,
         s = i;
     for (let a = 0; a < r; a++) {
         let l = n[Math.min(a, n.length - 1)];
         t.font = l.string;
@@ -24881,28 +24878,28 @@
     }
     return t.restore(), {
         width: o,
         height: s
     }
 }
 
-function BP(t, {
+function BD(t, {
     x: e,
     y: n
 }, i, r) {
     t.beginPath();
     let o = 0;
     i.forEach(function(s, a) {
         let l = r[Math.min(a, r.length - 1)],
             c = l.lineHeight;
         t.font = l.string, t.strokeText(s, e, n + c / 2 + o), o += c
     }), t.stroke()
 }
 
-function WP(t, {
+function WD(t, {
     x: e,
     y: n
 }, i, {
     fonts: r,
     colors: o
 }) {
     let s = 0;
@@ -24910,17 +24907,17 @@
         let c = o[Math.min(l, o.length - 1)],
             d = r[Math.min(l, r.length - 1)],
             g = d.lineHeight;
         t.beginPath(), t.font = d.string, t.fillStyle = c, t.fillText(a, e, n + g / 2 + s), s += g, t.fill()
     })
 }
 
-function VP(t, e) {
+function VD(t, e) {
     let n = di(t) ? t : e;
-    return di(n) ? Mf(n, 0, 1) : 1
+    return di(n) ? Df(n, 0, 1) : 1
 }
 var I1 = {
     xScaleID: {
         min: "xMin",
         max: "xMax",
         start: "left",
         end: "right",
@@ -24933,44 +24930,44 @@
         start: "bottom",
         end: "top",
         startProp: "y",
         endProp: "y2"
     }
 };
 
-function Us(t, e, n) {
+function $s(t, e, n) {
     return e = typeof e == "number" ? e : t.parse(e), qe(e) ? t.getPixelForValue(e) : n
 }
 
 function Ho(t, e, n) {
     let i = e[n];
     if (i || n === "scaleID") return i;
     let r = n.charAt(0),
         o = Object.values(t).filter(s => s.axis && s.axis === r);
     return o.length ? o[0].id : r
 }
 
 function a_(t, e) {
     if (t) {
         let n = t.options.reverse,
-            i = Us(t, e.min, n ? e.end : e.start),
-            r = Us(t, e.max, n ? e.start : e.end);
+            i = $s(t, e.min, n ? e.end : e.start),
+            r = $s(t, e.max, n ? e.start : e.end);
         return {
             start: i,
             end: r
         }
     }
 }
 
 function l_(t, e) {
     let {
         chartArea: n,
         scales: i
     } = t, r = i[Ho(i, e, "xScaleID")], o = i[Ho(i, e, "yScaleID")], s = n.width / 2, a = n.height / 2;
-    return r && (s = Us(r, e.xValue, r.left + r.width / 2)), o && (a = Us(o, e.yValue, o.top + o.height / 2)), {
+    return r && (s = $s(r, e.xValue, r.left + r.width / 2)), o && (a = $s(o, e.yValue, o.top + o.height / 2)), {
         x: s,
         y: a
     }
 }
 
 function tm(t, e) {
     let n = t.scales,
@@ -25024,41 +25021,41 @@
             centerX: o,
             centerY: s,
             width: r,
             height: r,
             radius: i
         }
     }
-    return $P(t, e)
+    return $D(t, e)
 }
 
-function UP(t, e) {
+function UD(t, e) {
     let {
         scales: n,
         chartArea: i
     } = t, r = n[e.scaleID], o = {
         x: i.left,
         y: i.top,
         x2: i.right,
         y2: i.bottom
     };
-    return r ? YP(r, o, e) : XP(n, o, e), o
+    return r ? YD(r, o, e) : XD(n, o, e), o
 }
 
 function c_(t, e) {
     let n = tm(t, e);
-    return n.initProperties = Fl(t, n, e), n.elements = [{
+    return n.initProperties = jl(t, n, e), n.elements = [{
         type: "label",
         optionScope: "label",
-        properties: GP(t, n, e),
+        properties: KD(t, n, e),
         initProperties: n.initProperties
     }], n
 }
 
-function $P(t, e) {
+function $D(t, e) {
     let n = l_(t, e),
         i = e.radius * 2;
     return {
         x: n.x - e.radius + e.xAdjust,
         y: n.y - e.radius + e.yAdjust,
         x2: n.x + e.radius + e.xAdjust,
         y2: n.y + e.radius + e.yAdjust,
@@ -25074,21 +25071,21 @@
     let n = a_(t, e) || e;
     return {
         start: Math.min(n.start, n.end),
         end: Math.max(n.start, n.end)
     }
 }
 
-function YP(t, e, n) {
-    let i = Us(t, n.value, NaN),
-        r = Us(t, n.endValue, i);
+function YD(t, e, n) {
+    let i = $s(t, n.value, NaN),
+        r = $s(t, n.endValue, i);
     t.isHorizontal() ? (e.x = i, e.x2 = r) : (e.y = i, e.y2 = r)
 }
 
-function XP(t, e, n) {
+function XD(t, e, n) {
     for (let i of Object.keys(I1)) {
         let r = t[Ho(t, n, i)];
         if (r) {
             let {
                 min: o,
                 max: s,
                 start: a,
@@ -25102,15 +25099,15 @@
                 end: r[l]
             });
             e[c] = g.start, e[d] = g.end
         }
     }
 }
 
-function qP({
+function qD({
     properties: t,
     options: e
 }, n, i, r) {
     let {
         x: o,
         x2: s,
         width: a
@@ -25127,15 +25124,15 @@
             end: r.right
         },
         adjust: e.label.xAdjust,
         size: n.width
     })
 }
 
-function ZP({
+function ZD({
     properties: t,
     options: e
 }, n, i, r) {
     let {
         y: o,
         y2: s,
         height: a
@@ -25165,28 +25162,28 @@
         position: o,
         padding: {
             start: s,
             end: a
         },
         adjust: l
     } = e, c = i - r - n - s - a - e.size;
-    return n + r / 2 + l + Qg(c, o)
+    return n + r / 2 + l + Gg(c, o)
 }
 
-function GP(t, e, n) {
+function KD(t, e, n) {
     let i = n.label;
     i.backgroundColor = "transparent", i.callout.display = !1;
-    let r = Kg(i.position),
+    let r = Qg(i.position),
         o = gt(i.padding),
         s = em(t.ctx, i),
-        a = qP({
+        a = qD({
             properties: e,
             options: n
         }, s, r, o),
-        l = ZP({
+        l = ZD({
             properties: e,
             options: n
         }, s, r, o),
         c = s.width + o.width,
         d = s.height + o.height;
     return {
         x: a,
@@ -25210,38 +25207,38 @@
         x: o + i * (t.x - o) - r * (t.y - s),
         y: s + r * (t.x - o) + i * (t.y - s)
     }
 }
 var Vg = ["enter", "leave"],
     nm = Vg.concat("click");
 
-function QP(t, e, n) {
-    e.listened = r_(n, nm, e.listeners), e.moveListened = !1, e._getElements = Gg, Vg.forEach(i => {
+function GD(t, e, n) {
+    e.listened = r_(n, nm, e.listeners), e.moveListened = !1, e._getElements = Kg, Vg.forEach(i => {
         Vt(n[i]) && (e.moveListened = !0)
     }), (!e.listened || !e.moveListened) && e.annotations.forEach(i => {
         !e.listened && Vt(i.click) && (e.listened = !0), e.moveListened || Vg.forEach(r => {
             Vt(i[r]) && (e.listened = !0, e.moveListened = !0)
         })
     })
 }
 
-function KP(t, e, n) {
+function QD(t, e, n) {
     if (t.listened) switch (e.type) {
         case "mousemove":
         case "mouseout":
-            return JP(t, e, n);
+            return JD(t, e, n);
         case "click":
-            return eM(t, e, n)
+            return eP(t, e, n)
     }
 }
 
-function JP(t, e, n) {
+function JD(t, e, n) {
     if (!t.moveListened) return;
     let i;
-    e.type === "mousemove" ? i = Gg(t, e, n.interaction) : i = [];
+    e.type === "mousemove" ? i = Kg(t, e, n.interaction) : i = [];
     let r = t.hovered;
     t.hovered = i;
     let o = {
             state: t,
             event: e
         },
         s = z1(o, "leave", r, i);
@@ -25253,80 +25250,80 @@
     event: e
 }, n, i, r) {
     let o;
     for (let s of i) r.indexOf(s) < 0 && (o = d_(s.options[n] || t.listeners[n], s, e) || o);
     return o
 }
 
-function eM(t, e, n) {
+function eP(t, e, n) {
     let i = t.listeners,
-        r = Gg(t, e, n.interaction),
+        r = Kg(t, e, n.interaction),
         o;
     for (let s of r) o = d_(s.options.click || i.click, s, e) || o;
     return o
 }
 
 function d_(t, e, n) {
     return ve(t, [e.$context, n]) === !0
 }
-var Pf = ["afterDraw", "beforeDraw"];
+var Tf = ["afterDraw", "beforeDraw"];
 
-function tM(t, e, n) {
+function tP(t, e, n) {
     let i = e.visibleElements;
-    e.hooked = r_(n, Pf, e.hooks), e.hooked || i.forEach(r => {
-        e.hooked || Pf.forEach(o => {
+    e.hooked = r_(n, Tf, e.hooks), e.hooked || i.forEach(r => {
+        e.hooked || Tf.forEach(o => {
             Vt(r.options[o]) && (e.hooked = !0)
         })
     })
 }
 
 function F1(t, e, n) {
     if (t.hooked) {
         let i = e.options[n] || t.hooks[n];
         return ve(i, [e.$context])
     }
 }
 
-function nM(t, e, n) {
-    let i = aM(t.scales, e, n),
+function nP(t, e, n) {
+    let i = aP(t.scales, e, n),
         r = j1(e, i, "min", "suggestedMin");
     r = j1(e, i, "max", "suggestedMax") || r, r && Vt(e.handleTickRangeOptions) && e.handleTickRangeOptions()
 }
 
-function iM(t, e) {
-    for (let n of t) oM(n, e)
+function iP(t, e) {
+    for (let n of t) oP(n, e)
 }
 
 function j1(t, e, n, i) {
-    if (qe(e[n]) && !rM(t.options, n, i)) {
+    if (qe(e[n]) && !rP(t.options, n, i)) {
         let r = t[n] !== e[n];
         return t[n] = e[n], r
     }
 }
 
-function rM(t, e, n) {
+function rP(t, e, n) {
     return Ut(t[e]) || Ut(t[n])
 }
 
-function oM(t, e) {
+function oP(t, e) {
     for (let n of ["scaleID", "xScaleID", "yScaleID"]) {
         let i = Ho(e, t, n);
-        i && !e[i] && sM(t, n) && console.warn(`No scale found with id '${i}' for annotation '${t.id}'`)
+        i && !e[i] && sP(t, n) && console.warn(`No scale found with id '${i}' for annotation '${t.id}'`)
     }
 }
 
-function sM(t, e) {
+function sP(t, e) {
     if (e === "scaleID") return !0;
     let n = e.charAt(0);
     for (let i of ["Min", "Max", "Value"])
         if (Ut(t[n + i])) return !0;
     return !1
 }
 
-function aM(t, e, n) {
+function aP(t, e, n) {
     let i = e.axis,
         r = e.id,
         o = i + "ScaleID",
         s = {
             min: pe(e.min, Number.NEGATIVE_INFINITY),
             max: pe(e.max, Number.POSITIVE_INFINITY)
         };
@@ -25339,43 +25336,43 @@
         let o = t[r];
         if (Ut(o)) {
             let s = e.parse(o);
             i.min = Math.min(i.min, s), i.max = Math.max(i.max, s)
         }
     }
 }
-var Kr = class extends zt {
+var Qr = class extends zt {
     inRange(e, n, i, r) {
         let {
             x: o,
             y: s
         } = Uo({
             x: e,
             y: n
         }, this.getCenterPoint(r), pt(-this.options.rotation));
         return J1({
             x: o,
             y: s
         }, this.getProps(["x", "y", "x2", "y2"], r), i, this.options.borderWidth)
     }
     getCenterPoint(e) {
-        return Xs(this, e)
+        return qs(this, e)
     }
     draw(e) {
         e.save(), Jg(e, this.getCenterPoint(), this.options.rotation), s_(e, this, this.options), e.restore()
     }
     get label() {
         return this.elements && this.elements[0]
     }
     resolveElementProperties(e, n) {
         return c_(e, n)
     }
 };
-Kr.id = "boxAnnotation";
-Kr.defaults = {
+Qr.id = "boxAnnotation";
+Qr.defaults = {
     adjustScaleRange: !0,
     backgroundShadowColor: "transparent",
     borderCapStyle: "butt",
     borderDash: [],
     borderDashOffset: 0,
     borderJoinStyle: "miter",
     borderRadius: 0,
@@ -25421,19 +25418,19 @@
     xMin: void 0,
     xScaleID: void 0,
     yMax: void 0,
     yMin: void 0,
     yScaleID: void 0,
     z: 0
 };
-Kr.defaultRoutes = {
+Qr.defaultRoutes = {
     borderColor: "color",
     backgroundColor: "color"
 };
-Kr.descriptors = {
+Qr.descriptors = {
     label: {
         _fallback: !0
     }
 };
 var h_ = ["left", "bottom", "top", "right"],
     Bo = class extends zt {
         inRange(e, n, i, r) {
@@ -25446,20 +25443,20 @@
             }, this.getCenterPoint(r), pt(-this.rotation));
             return J1({
                 x: o,
                 y: s
             }, this.getProps(["x", "y", "x2", "y2"], r), i, this.options.borderWidth)
         }
         getCenterPoint(e) {
-            return Xs(this, e)
+            return qs(this, e)
         }
         draw(e) {
             let n = this.options,
                 i = !Ut(this._visible) || this._visible;
-            !n.display || !n.content || !i || (e.save(), Jg(e, this.getCenterPoint(), this.rotation), uM(e, this), s_(e, this, n), NP(e, mM(this), n), e.restore())
+            !n.display || !n.content || !i || (e.save(), Jg(e, this.getCenterPoint(), this.rotation), uP(e, this), s_(e, this, n), ND(e, mP(this), n), e.restore())
         }
         resolveElementProperties(e, n) {
             let i;
             if (i_(n)) i = l_(e, n);
             else {
                 let {
                     centerX: a,
@@ -25468,17 +25465,17 @@
                 i = {
                     x: a,
                     y: l
                 }
             }
             let r = gt(n.padding),
                 o = em(e.ctx, n),
-                s = lM(i, o, n, r);
+                s = lP(i, o, n, r);
             return {
-                initProperties: Fl(e, s, n),
+                initProperties: jl(e, s, n),
                 pointX: i.x,
                 pointY: i.y,
                 ...s,
                 rotation: n.rotation
             }
         }
     };
@@ -25542,18 +25539,18 @@
     yValue: void 0,
     z: 0
 };
 Bo.defaultRoutes = {
     borderColor: "color"
 };
 
-function lM(t, e, n, i) {
+function lP(t, e, n, i) {
     let r = e.width + i.width + n.borderWidth,
         o = e.height + i.height + n.borderWidth,
-        s = Kg(n.position, "center"),
+        s = Qg(n.position, "center"),
         a = B1(t.x, r, n.xAdjust, s.x),
         l = B1(t.y, o, n.yAdjust, s.y);
     return {
         x: a,
         y: l,
         x2: a + r,
         y2: l + o,
@@ -25561,47 +25558,47 @@
         height: o,
         centerX: a + r / 2,
         centerY: l + o / 2
     }
 }
 
 function B1(t, e, n = 0, i) {
-    return t - Qg(e, i) + n
+    return t - Gg(e, i) + n
 }
 
-function uM(t, e) {
+function uP(t, e) {
     let {
         pointX: n,
         pointY: i,
         options: r
-    } = e, o = r.callout, s = o && o.display && pM(e, o);
-    if (!s || yM(e, o, s)) return;
-    if (t.save(), t.beginPath(), !Qr(t, o)) return t.restore();
+    } = e, o = r.callout, s = o && o.display && pP(e, o);
+    if (!s || yP(e, o, s)) return;
+    if (t.save(), t.beginPath(), !Gr(t, o)) return t.restore();
     let {
         separatorStart: l,
         separatorEnd: c
-    } = cM(e, s), {
+    } = cP(e, s), {
         sideStart: d,
         sideEnd: g
-    } = dM(e, s, l);
+    } = dP(e, s, l);
     (o.margin > 0 || r.borderWidth === 0) && (t.moveTo(l.x, l.y), t.lineTo(c.x, c.y)), t.moveTo(d.x, d.y), t.lineTo(g.x, g.y);
     let y = Uo({
         x: n,
         y: i
     }, e.getCenterPoint(), pt(-e.rotation));
     t.lineTo(y.x, y.y), t.stroke(), t.restore()
 }
 
-function cM(t, e) {
+function cP(t, e) {
     let {
         x: n,
         y: i,
         x2: r,
         y2: o
-    } = t, s = fM(t, e), a, l;
+    } = t, s = fP(t, e), a, l;
     return e === "left" || e === "right" ? (a = {
         x: n + s,
         y: i
     }, l = {
         x: a.x,
         y: o
     }) : (a = {
@@ -25612,59 +25609,59 @@
         y: a.y
     }), {
         separatorStart: a,
         separatorEnd: l
     }
 }
 
-function fM(t, e) {
+function fP(t, e) {
     let {
         width: n,
         height: i,
         options: r
     } = t, o = r.callout.margin + r.borderWidth / 2;
     return e === "right" ? n + o : e === "bottom" ? i + o : -o
 }
 
-function dM(t, e, n) {
+function dP(t, e, n) {
     let {
         y: i,
         width: r,
         height: o,
         options: s
-    } = t, a = s.callout.start, l = hM(e, s.callout), c, d;
+    } = t, a = s.callout.start, l = hP(e, s.callout), c, d;
     return e === "left" || e === "right" ? (c = {
         x: n.x,
-        y: i + Gr(o, a)
+        y: i + Kr(o, a)
     }, d = {
         x: c.x + l,
         y: c.y
     }) : (c = {
-        x: n.x + Gr(r, a),
+        x: n.x + Kr(r, a),
         y: n.y
     }, d = {
         x: c.x,
         y: c.y + l
     }), {
         sideStart: c,
         sideEnd: d
     }
 }
 
-function hM(t, e) {
+function hP(t, e) {
     let n = e.side;
     return t === "left" || t === "top" ? -n : n
 }
 
-function pM(t, e) {
+function pP(t, e) {
     let n = e.position;
-    return h_.includes(n) ? n : gM(t, e)
+    return h_.includes(n) ? n : gP(t, e)
 }
 
-function gM(t, e) {
+function gP(t, e) {
     let {
         x: n,
         y: i,
         x2: r,
         y2: o,
         width: s,
         height: a,
@@ -25672,32 +25669,32 @@
         pointY: c,
         centerX: d,
         centerY: g,
         rotation: y
     } = t, x = {
         x: d,
         y: g
-    }, w = e.start, S = Gr(s, w), A = Gr(a, w), _ = [n, n + S, n + S, r], C = [i + A, o, i, o], M = [];
+    }, _ = e.start, C = Kr(s, _), A = Kr(a, _), w = [n, n + C, n + C, r], k = [i + A, o, i, o], P = [];
     for (let z = 0; z < 4; z++) {
         let F = Uo({
-            x: _[z],
-            y: C[z]
+            x: w[z],
+            y: k[z]
         }, x, pt(y));
-        M.push({
+        P.push({
             position: h_[z],
             distance: tr(F, {
                 x: l,
                 y: c
             })
         })
     }
-    return M.sort((z, F) => z.distance - F.distance)[0].position
+    return P.sort((z, F) => z.distance - F.distance)[0].position
 }
 
-function mM({
+function mP({
     x: t,
     y: e,
     width: n,
     height: i,
     options: r
 }) {
     let o = r.borderWidth / 2,
@@ -25706,29 +25703,29 @@
         x: t + s.left + o,
         y: e + s.top + o,
         width: n - s.left - s.right - r.borderWidth,
         height: i - s.top - s.bottom - r.borderWidth
     }
 }
 
-function yM(t, e, n) {
+function yP(t, e, n) {
     let {
         pointX: i,
         pointY: r
     } = t, o = e.margin, s = i, a = r;
     return n === "left" ? s += o : n === "right" ? s -= o : n === "top" ? a += o : n === "bottom" && (a -= o), t.inRange(s, a)
 }
 var im = (t, e, n) => ({
         x: t.x + n * (e.x - t.x),
         y: t.y + n * (e.y - t.y)
     }),
     Ug = (t, e, n) => im(e, n, Math.abs((t - e.y) / (n.y - e.y))).x,
     W1 = (t, e, n) => im(e, n, Math.abs((t - e.x) / (n.x - e.x))).y,
-    zl = t => t * t,
-    vM = (t, e, {
+    Fl = t => t * t,
+    vP = (t, e, {
         x: n,
         y: i,
         x2: r,
         y2: o
     }, s) => s === "y" ? {
         start: Math.min(i, o),
         end: Math.max(i, o),
@@ -25754,93 +25751,93 @@
                         mouseY: n
                     },
                     {
                         path: a,
                         ctx: l
                     } = this;
                 if (a) {
-                    Qr(l, this.options);
+                    Gr(l, this.options);
                     let {
                         chart: d
                     } = this.$context, g = e * d.currentDevicePixelRatio, y = n * d.currentDevicePixelRatio, x = l.isPointInStroke(a, g, y) || Yg(this, s, r);
                     return l.restore(), x
                 }
-                let c = zl(o);
-                return wM(this, s, c, r) || Yg(this, s, r)
+                let c = Fl(o);
+                return wP(this, s, c, r) || Yg(this, s, r)
             }
-            return xM(this, {
+            return xP(this, {
                 mouseX: e,
                 mouseY: n
             }, i, {
                 hBorderWidth: o,
                 useFinalPosition: r
             })
         }
         getCenterPoint(e) {
-            return Xs(this, e)
+            return qs(this, e)
         }
         draw(e) {
             let {
                 x: n,
                 y: i,
                 x2: r,
                 y2: o,
                 cp: s,
                 options: a
             } = this;
-            if (e.save(), !Qr(e, a)) return e.restore();
-            qs(e, a);
+            if (e.save(), !Gr(e, a)) return e.restore();
+            Zs(e, a);
             let l = Math.sqrt(Math.pow(r - n, 2) + Math.pow(o - i, 2));
-            if (a.curve && s) return DM(e, this, s, l), e.restore();
+            if (a.curve && s) return MP(e, this, s, l), e.restore();
             let {
                 startOpts: c,
                 endOpts: d,
                 startAdjust: g,
                 endAdjust: y
             } = p_(this), x = Math.atan2(o - i, r - n);
             e.translate(n, i), e.rotate(x), e.beginPath(), e.moveTo(0 + g, 0), e.lineTo(l - y, 0), e.shadowColor = a.borderShadowColor, e.stroke(), Xg(e, 0, g, c), Xg(e, l, -y, d), e.restore()
         }
         get label() {
             return this.elements && this.elements[0]
         }
         resolveElementProperties(e, n) {
-            let i = UP(e, n),
+            let i = UD(e, n),
                 {
                     x: r,
                     y: o,
                     x2: s,
                     y2: a
                 } = i,
-                l = bM(i, e.chartArea),
-                c = l ? _M({
+                l = bP(i, e.chartArea),
+                c = l ? _P({
                     x: r,
                     y: o
                 }, {
                     x: s,
                     y: a
                 }, e.chartArea) : {
                     x: r,
                     y: o,
                     x2: s,
                     y2: a,
                     width: Math.abs(s - r),
                     height: Math.abs(a - o)
                 };
-            if (c.centerX = (s + r) / 2, c.centerY = (a + o) / 2, c.initProperties = Fl(e, c, n), n.curve) {
+            if (c.centerX = (s + r) / 2, c.centerY = (a + o) / 2, c.initProperties = jl(e, c, n), n.curve) {
                 let g = {
                         x: c.x,
                         y: c.y
                     },
                     y = {
                         x: c.x2,
                         y: c.y2
                     };
-                c.cp = MM(c, n, tr(g, y))
+                c.cp = PP(c, n, tr(g, y))
             }
-            let d = kM(e, c, n.label);
+            let d = SP(e, c, n.label);
             return d._visible = l, c.elements = [{
                 type: "label",
                 optionScope: "label",
                 properties: d,
                 initProperties: c.initProperties
             }], c
         }
@@ -25946,29 +25943,29 @@
         _fallback: !0
     }
 };
 Wo.defaultRoutes = {
     borderColor: "color"
 };
 
-function xM(t, {
+function xP(t, {
     mouseX: e,
     mouseY: n
 }, i, {
     hBorderWidth: r,
     useFinalPosition: o
 }) {
-    let s = vM(e, n, t.getProps(["x", "y", "x2", "y2"], o), i);
+    let s = vP(e, n, t.getProps(["x", "y", "x2", "y2"], o), i);
     return s.value >= s.start - r && s.value <= s.end + r || Yg(t, {
         mouseX: e,
         mouseY: n
     }, o, i)
 }
 
-function bM({
+function bP({
     x: t,
     y: e,
     x2: n,
     y2: i
 }, {
     top: r,
     right: o,
@@ -26001,15 +25998,15 @@
         y: e
     }, n), e = o), {
         x: t,
         y: e
     }
 }
 
-function _M(t, e, n) {
+function _P(t, e, n) {
     let {
         x: i,
         y: r
     } = X1(t, e, n), {
         x: o,
         y: s
     } = X1(e, t, n);
@@ -26019,130 +26016,130 @@
         x2: o,
         y2: s,
         width: Math.abs(o - i),
         height: Math.abs(s - r)
     }
 }
 
-function wM(t, {
+function wP(t, {
     mouseX: e,
     mouseY: n
 }, i = jo, r) {
     let {
         x: o,
         y: s,
         x2: a,
         y2: l
-    } = t.getProps(["x", "y", "x2", "y2"], r), c = a - o, d = l - s, g = zl(c) + zl(d), y = g === 0 ? -1 : ((e - o) * c + (n - s) * d) / g, x, w;
-    return y < 0 ? (x = o, w = s) : y > 1 ? (x = a, w = l) : (x = o + y * c, w = s + y * d), zl(e - x) + zl(n - w) <= i
+    } = t.getProps(["x", "y", "x2", "y2"], r), c = a - o, d = l - s, g = Fl(c) + Fl(d), y = g === 0 ? -1 : ((e - o) * c + (n - s) * d) / g, x, _;
+    return y < 0 ? (x = o, _ = s) : y > 1 ? (x = a, _ = l) : (x = o + y * c, _ = s + y * d), Fl(e - x) + Fl(n - _) <= i
 }
 
 function Yg(t, {
     mouseX: e,
     mouseY: n
 }, i, r) {
     let o = t.label;
     return o.options.display && o.inRange(e, n, r, i)
 }
 
-function kM(t, e, n) {
+function SP(t, e, n) {
     let i = n.borderWidth,
         r = gt(n.padding),
         o = em(t.ctx, n),
         s = o.width + r.width + i,
         a = o.height + r.height + i;
-    return CM(e, n, {
+    return CP(e, n, {
         width: s,
         height: a,
         padding: r
     }, t.chartArea)
 }
 
-function SM(t) {
+function kP(t) {
     let {
         x: e,
         y: n,
         x2: i,
         y2: r
     } = t, o = Math.atan2(r - n, i - e);
     return o > Ce / 2 ? o - Ce : o < Ce / -2 ? o + Ce : o
 }
 
-function CM(t, e, n, i) {
+function CP(t, e, n, i) {
     let {
         width: r,
         height: o,
         padding: s
     } = n, {
         xAdjust: a,
         yAdjust: l
     } = e, c = {
         x: t.x,
         y: t.y
     }, d = {
         x: t.x2,
         y: t.y2
-    }, g = e.rotation === "auto" ? SM(t) : pt(e.rotation), y = EM(r, o, g), x = TM(t, e, {
+    }, g = e.rotation === "auto" ? kP(t) : pt(e.rotation), y = EP(r, o, g), x = TP(t, e, {
         labelSize: y,
         padding: s
-    }, i), w = t.cp ? $g(c, t.cp, d, x) : im(c, d, x), S = {
+    }, i), _ = t.cp ? $g(c, t.cp, d, x) : im(c, d, x), C = {
         size: y.w,
         min: i.left,
         max: i.right,
         padding: s.left
     }, A = {
         size: y.h,
         min: i.top,
         max: i.bottom,
         padding: s.top
-    }, _ = Z1(w.x, S) + a, C = Z1(w.y, A) + l;
+    }, w = Z1(_.x, C) + a, k = Z1(_.y, A) + l;
     return {
-        x: _ - r / 2,
-        y: C - o / 2,
-        x2: _ + r / 2,
-        y2: C + o / 2,
-        centerX: _,
-        centerY: C,
-        pointX: w.x,
-        pointY: w.y,
+        x: w - r / 2,
+        y: k - o / 2,
+        x2: w + r / 2,
+        y2: k + o / 2,
+        centerX: w,
+        centerY: k,
+        pointX: _.x,
+        pointY: _.y,
         width: r,
         height: o,
         rotation: Ao(g)
     }
 }
 
-function EM(t, e, n) {
+function EP(t, e, n) {
     let i = Math.cos(n),
         r = Math.sin(n);
     return {
         w: Math.abs(t * i) + Math.abs(e * r),
         h: Math.abs(t * r) + Math.abs(e * i)
     }
 }
 
-function TM(t, e, n, i) {
-    let r, o = PM(t, i);
+function TP(t, e, n, i) {
+    let r, o = DP(t, i);
     return e.position === "start" ? r = q1({
         w: t.x2 - t.x,
         h: t.y2 - t.y
     }, n, e, o) : e.position === "end" ? r = 1 - q1({
         w: t.x - t.x2,
         h: t.y - t.y2
-    }, n, e, o) : r = Qg(1, e.position), r
+    }, n, e, o) : r = Gg(1, e.position), r
 }
 
 function q1(t, e, n, i) {
     let {
         labelSize: r,
         padding: o
     } = e, s = t.w * i.dx, a = t.h * i.dy, l = s > 0 && (r.w / 2 + o.left - i.x) / s, c = a > 0 && (r.h / 2 + o.top - i.y) / a;
-    return Mf(Math.max(l, c), 0, .25)
+    return Df(Math.max(l, c), 0, .25)
 }
 
-function PM(t, e) {
+function DP(t, e) {
     let {
         x: n,
         x2: i,
         y: r,
         y2: o
     } = t, s = Math.min(r, o) - e.top, a = Math.min(n, i) - e.left, l = e.bottom - Math.max(r, o), c = e.right - Math.max(n, i);
     return {
@@ -26166,20 +26163,20 @@
 function p_(t) {
     let e = t.options,
         n = e.arrowHeads && e.arrowHeads.start,
         i = e.arrowHeads && e.arrowHeads.end;
     return {
         startOpts: n,
         endOpts: i,
-        startAdjust: G1(t, n),
-        endAdjust: G1(t, i)
+        startAdjust: K1(t, n),
+        endAdjust: K1(t, i)
     }
 }
 
-function G1(t, e) {
+function K1(t, e) {
     if (!e || !e.display) return 0;
     let {
         length: n,
         width: i
     } = e, r = t.options.borderWidth / 2, o = {
         x: n,
         y: i + r
@@ -26195,77 +26192,77 @@
     let {
         length: r,
         width: o,
         fill: s,
         backgroundColor: a,
         borderColor: l
     } = i, c = Math.abs(e - r) + n;
-    t.beginPath(), qs(t, i), Qr(t, i), t.moveTo(c, -o), t.lineTo(e + n, 0), t.lineTo(c, o), s === !0 ? (t.fillStyle = a || l, t.closePath(), t.fill(), t.shadowColor = "transparent") : t.shadowColor = i.borderShadowColor, t.stroke()
+    t.beginPath(), Zs(t, i), Gr(t, i), t.moveTo(c, -o), t.lineTo(e + n, 0), t.lineTo(c, o), s === !0 ? (t.fillStyle = a || l, t.closePath(), t.fill(), t.shadowColor = "transparent") : t.shadowColor = i.borderShadowColor, t.stroke()
 }
 
-function MM(t, e, n) {
+function PP(t, e, n) {
     let {
         x: i,
         y: r,
         x2: o,
         y2: s,
         centerX: a,
         centerY: l
-    } = t, c = Math.atan2(s - r, o - i), d = Kg(e.controlPoint, 0), g = {
-        x: a + Gr(n, d.x, !1),
-        y: l + Gr(n, d.y, !1)
+    } = t, c = Math.atan2(s - r, o - i), d = Qg(e.controlPoint, 0), g = {
+        x: a + Kr(n, d.x, !1),
+        y: l + Kr(n, d.y, !1)
     };
     return Uo(g, {
         x: a,
         y: l
     }, c)
 }
 
-function Q1(t, {
+function G1(t, {
     x: e,
     y: n
 }, {
     angle: i,
     adjust: r
 }, o) {
     !o || !o.display || (t.save(), t.translate(e, n), t.rotate(i), Xg(t, 0, -r, o), t.restore())
 }
 
-function DM(t, e, n, i) {
+function MP(t, e, n, i) {
     let {
         x: r,
         y: o,
         x2: s,
         y2: a,
         options: l
     } = e, {
         startOpts: c,
         endOpts: d,
         startAdjust: g,
         endAdjust: y
     } = p_(e), x = {
         x: r,
         y: o
-    }, w = {
+    }, _ = {
         x: s,
         y: a
-    }, S = $1(x, n, w, 0), A = $1(x, n, w, 1) - Ce, _ = $g(x, n, w, g / i), C = $g(x, n, w, 1 - y / i), M = new Path2D;
-    t.beginPath(), M.moveTo(_.x, _.y), M.quadraticCurveTo(n.x, n.y, C.x, C.y), t.shadowColor = l.borderShadowColor, t.stroke(M), e.path = M, e.ctx = t, Q1(t, _, {
-        angle: S,
+    }, C = $1(x, n, _, 0), A = $1(x, n, _, 1) - Ce, w = $g(x, n, _, g / i), k = $g(x, n, _, 1 - y / i), P = new Path2D;
+    t.beginPath(), P.moveTo(w.x, w.y), P.quadraticCurveTo(n.x, n.y, k.x, k.y), t.shadowColor = l.borderShadowColor, t.stroke(P), e.path = P, e.ctx = t, G1(t, w, {
+        angle: C,
         adjust: g
-    }, c), Q1(t, C, {
+    }, c), G1(t, k, {
         angle: A,
         adjust: y
     }, d)
 }
 var Vo = class extends zt {
     inRange(e, n, i, r) {
         let o = this.options.rotation,
             s = this.options.borderWidth;
-        if (i !== "x" && i !== "y") return OM({
+        if (i !== "x" && i !== "y") return OP({
             x: e,
             y: n
         }, this.getProps(["width", "height", "centerX", "centerY"], r), o, s);
         let {
             x: a,
             y: l,
             x2: c,
@@ -26279,26 +26276,26 @@
         }, x = Uo({
             x: e,
             y: n
         }, this.getCenterPoint(r), pt(-o));
         return x[i] >= y.start - g - jo && x[i] <= y.end + g + jo
     }
     getCenterPoint(e) {
-        return Xs(this, e)
+        return qs(this, e)
     }
     draw(e) {
         let {
             width: n,
             height: i,
             centerX: r,
             centerY: o,
             options: s
         } = this;
-        e.save(), Jg(e, this.getCenterPoint(), s.rotation), qs(e, this.options), e.beginPath(), e.fillStyle = s.backgroundColor;
-        let a = Qr(e, s);
+        e.save(), Jg(e, this.getCenterPoint(), s.rotation), Zs(e, this.options), e.beginPath(), e.fillStyle = s.backgroundColor;
+        let a = Gr(e, s);
         e.ellipse(r, o, i / 2, n / 2, Ce / 2, 0, 2 * Ce), e.fill(), a && (e.shadowColor = s.borderShadowColor, e.stroke()), e.restore()
     }
     get label() {
         return this.elements && this.elements[0]
     }
     resolveElementProperties(e, n) {
         return c_(e, n)
@@ -26310,15 +26307,15 @@
     backgroundShadowColor: "transparent",
     borderDash: [],
     borderDashOffset: 0,
     borderShadowColor: "transparent",
     borderWidth: 1,
     display: !0,
     init: void 0,
-    label: Object.assign({}, Kr.defaults.label),
+    label: Object.assign({}, Qr.defaults.label),
     rotation: 0,
     shadowBlur: 0,
     shadowOffsetX: 0,
     shadowOffsetY: 0,
     xMax: void 0,
     xMin: void 0,
     xScaleID: void 0,
@@ -26333,40 +26330,40 @@
 };
 Vo.descriptors = {
     label: {
         _fallback: !0
     }
 };
 
-function OM(t, e, n, i) {
+function OP(t, e, n, i) {
     let {
         width: r,
         height: o,
         centerX: s,
         centerY: a
     } = e, l = r / 2, c = o / 2;
     if (l <= 0 || c <= 0) return !1;
     let d = pt(n || 0),
         g = i / 2 || 0,
         y = Math.cos(d),
         x = Math.sin(d),
-        w = Math.pow(y * (t.x - s) + x * (t.y - a), 2),
-        S = Math.pow(x * (t.x - s) - y * (t.y - a), 2);
-    return w / Math.pow(l + g, 2) + S / Math.pow(c + g, 2) <= 1.0001
+        _ = Math.pow(y * (t.x - s) + x * (t.y - a), 2),
+        C = Math.pow(x * (t.x - s) - y * (t.y - a), 2);
+    return _ / Math.pow(l + g, 2) + C / Math.pow(c + g, 2) <= 1.0001
 }
-var $s = class extends zt {
+var Ys = class extends zt {
     inRange(e, n, i, r) {
         let {
             x: o,
             y: s,
             x2: a,
             y2: l,
             width: c
         } = this.getProps(["x", "y", "x2", "y2", "width"], r), d = this.options.borderWidth;
-        if (i !== "x" && i !== "y") return MP({
+        if (i !== "x" && i !== "y") return PD({
             x: e,
             y: n
         }, this.getCenterPoint(r), c / 2, d);
         let g = d / 2,
             y = i === "y" ? {
                 start: s,
                 end: l,
@@ -26375,31 +26372,31 @@
                 start: o,
                 end: a,
                 value: e
             };
         return y.value >= y.start - g && y.value <= y.end + g
     }
     getCenterPoint(e) {
-        return Xs(this, e)
+        return qs(this, e)
     }
     draw(e) {
         let n = this.options,
             i = n.borderWidth;
         if (n.radius < .1) return;
-        e.save(), e.fillStyle = n.backgroundColor, qs(e, n);
-        let r = Qr(e, n);
-        FP(e, this, this.centerX, this.centerY), r && !Df(n.pointStyle) && (e.shadowColor = n.borderShadowColor, e.stroke()), e.restore(), n.borderWidth = i
+        e.save(), e.fillStyle = n.backgroundColor, Zs(e, n);
+        let r = Gr(e, n);
+        FD(e, this, this.centerX, this.centerY), r && !Pf(n.pointStyle) && (e.shadowColor = n.borderShadowColor, e.stroke()), e.restore(), n.borderWidth = i
     }
     resolveElementProperties(e, n) {
         let i = u_(e, n);
-        return i.initProperties = Fl(e, i, n), i
+        return i.initProperties = jl(e, i, n), i
     }
 };
-$s.id = "pointAnnotation";
-$s.defaults = {
+Ys.id = "pointAnnotation";
+Ys.defaults = {
     adjustScaleRange: !0,
     backgroundShadowColor: "transparent",
     borderDash: [],
     borderDashOffset: 0,
     borderShadowColor: "transparent",
     borderWidth: 1,
     display: !0,
@@ -26418,62 +26415,62 @@
     yAdjust: 0,
     yMax: void 0,
     yMin: void 0,
     yScaleID: void 0,
     yValue: void 0,
     z: 0
 };
-$s.defaultRoutes = {
+Ys.defaultRoutes = {
     borderColor: "color",
     backgroundColor: "color"
 };
-var Ys = class extends zt {
+var Xs = class extends zt {
     inRange(e, n, i, r) {
-        if (i !== "x" && i !== "y") return this.options.radius >= .1 && this.elements.length > 1 && LM(this.elements, e, n, r);
+        if (i !== "x" && i !== "y") return this.options.radius >= .1 && this.elements.length > 1 && LP(this.elements, e, n, r);
         let o = Uo({
                 x: e,
                 y: n
             }, this.getCenterPoint(r), pt(-this.options.rotation)),
             s = this.elements.map(c => i === "y" ? c.bY : c.bX),
             a = Math.min(...s),
             l = Math.max(...s);
         return o[i] >= a && o[i] <= l
     }
     getCenterPoint(e) {
-        return Xs(this, e)
+        return qs(this, e)
     }
     draw(e) {
         let {
             elements: n,
             options: i
         } = this;
-        e.save(), e.beginPath(), e.fillStyle = i.backgroundColor, qs(e, i);
-        let r = Qr(e, i),
+        e.save(), e.beginPath(), e.fillStyle = i.backgroundColor, Zs(e, i);
+        let r = Gr(e, i),
             o = !0;
         for (let s of n) o ? (e.moveTo(s.x, s.y), o = !1) : e.lineTo(s.x, s.y);
         e.closePath(), e.fill(), r && (e.shadowColor = i.borderShadowColor, e.stroke()), e.restore()
     }
     resolveElementProperties(e, n) {
         let i = u_(e, n),
             {
                 sides: r,
                 rotation: o
             } = n,
             s = [],
             a = 2 * Ce / r,
-            l = o * dl;
+            l = o * hl;
         for (let c = 0; c < r; c++, l += a) {
-            let d = AM(i, n, l);
-            d.initProperties = Fl(e, i, n), s.push(d)
+            let d = AP(i, n, l);
+            d.initProperties = jl(e, i, n), s.push(d)
         }
         return i.elements = s, i
     }
 };
-Ys.id = "polygonAnnotation";
-Ys.defaults = {
+Xs.id = "polygonAnnotation";
+Xs.defaults = {
     adjustScaleRange: !0,
     backgroundShadowColor: "transparent",
     borderCapStyle: "butt",
     borderDash: [],
     borderDashOffset: 0,
     borderJoinStyle: "miter",
     borderShadowColor: "transparent",
@@ -26497,20 +26494,20 @@
     yAdjust: 0,
     yMax: void 0,
     yMin: void 0,
     yScaleID: void 0,
     yValue: void 0,
     z: 0
 };
-Ys.defaultRoutes = {
+Xs.defaultRoutes = {
     borderColor: "color",
     backgroundColor: "color"
 };
 
-function AM({
+function AP({
     centerX: t,
     centerY: e
 }, {
     radius: n,
     borderWidth: i
 }, r) {
     let o = i / 2,
@@ -26530,69 +26527,69 @@
             centerY: l.y,
             bX: t + s * (n + o),
             bY: e - a * (n + o)
         }
     }
 }
 
-function LM(t, e, n, i) {
+function LP(t, e, n, i) {
     let r = !1,
         o = t[t.length - 1].getProps(["bX", "bY"], i);
     for (let s of t) {
         let a = s.getProps(["bX", "bY"], i);
         a.bY > n != o.bY > n && e < (o.bX - a.bX) * (n - a.bY) / (o.bY - a.bY) + a.bX && (r = !r), o = a
     }
     return r
 }
 var Zr = {
-    box: Kr,
+    box: Qr,
     ellipse: Vo,
     label: Bo,
     line: Wo,
-    point: $s,
-    polygon: Ys
+    point: Ys,
+    polygon: Xs
 };
 Object.keys(Zr).forEach(t => {
     rt.describe(`elements.${Zr[t].id}`, {
         _fallback: "plugins.annotation.common"
     })
 });
-var RM = {
+var RP = {
         update: Object.assign
     },
-    IM = nm.concat(Pf),
-    K1 = (t, e) => we(e) ? Zg(t, e) : t,
+    IP = nm.concat(Tf),
+    Q1 = (t, e) => we(e) ? Zg(t, e) : t,
     qg = t => t === "color" || t === "font";
 
 function rm(t = "line") {
     return Zr[t] ? t : (console.warn(`Unknown annotation type: '${t}', defaulting to 'line'`), "line")
 }
 
-function NM(t, e, n, i) {
-    let r = FM(t, n.animations, i),
+function NP(t, e, n, i) {
+    let r = FP(t, n.animations, i),
         o = e.annotations,
-        s = BM(e.elements, o);
+        s = BP(e.elements, o);
     for (let a = 0; a < o.length; a++) {
         let l = o[a],
             c = g_(s, a, l.type),
-            d = l.setContext(HM(t, c, l)),
+            d = l.setContext(HP(t, c, l)),
             g = c.resolveElementProperties(t, d);
-        g.skip = zM(g), "elements" in g && (jM(c, g.elements, d, r), delete g.elements), Ut(c.x) || Object.assign(c, g), Object.assign(c, g.initProperties), g.options = m_(d), r.update(c, g)
+        g.skip = zP(g), "elements" in g && (jP(c, g.elements, d, r), delete g.elements), Ut(c.x) || Object.assign(c, g), Object.assign(c, g.initProperties), g.options = m_(d), r.update(c, g)
     }
 }
 
-function zM(t) {
+function zP(t) {
     return isNaN(t.x) || isNaN(t.y)
 }
 
-function FM(t, e, n) {
-    return n === "reset" || n === "none" || n === "resize" ? RM : new zs(t, e)
+function FP(t, e, n) {
+    return n === "reset" || n === "none" || n === "resize" ? RP : new zs(t, e)
 }
 
-function jM(t, e, n, i) {
+function jP(t, e, n, i) {
     let r = t.elements || (t.elements = []);
     r.length = e.length;
     for (let o = 0; o < e.length; o++) {
         let s = e[o],
             a = s.properties,
             l = g_(r, o, s.type, s.initProperties),
             c = n[s.optionScope].override(s);
@@ -26606,53 +26603,53 @@
     return (!o || !(o instanceof r)) && (o = t[e] = new r, Object.assign(o, i)), o
 }
 
 function m_(t) {
     let e = Zr[rm(t.type)],
         n = {};
     n.id = t.id, n.type = t.type, n.drawTime = t.drawTime, Object.assign(n, Zg(t, e.defaults), Zg(t, e.defaultRoutes));
-    for (let i of IM) n[i] = t[i];
+    for (let i of IP) n[i] = t[i];
     return n
 }
 
 function Zg(t, e) {
     let n = {};
     for (let i of Object.keys(e)) {
         let r = e[i],
             o = t[i];
-        qg(i) && Re(o) ? n[i] = o.map(s => K1(s, r)) : n[i] = K1(o, r)
+        qg(i) && Re(o) ? n[i] = o.map(s => Q1(s, r)) : n[i] = Q1(o, r)
     }
     return n
 }
 
-function HM(t, e, n) {
+function HP(t, e, n) {
     return e.$context || (e.$context = Object.assign(Object.create(t.getContext()), {
         element: e,
         id: n.id,
         type: "annotation"
     }))
 }
 
-function BM(t, e) {
+function BP(t, e) {
     let n = e.length,
         i = t.length;
     if (i < n) {
         let r = n - i;
         t.splice(i, 0, ...new Array(r))
     } else i > n && t.splice(n, i - n);
     return t
 }
-var WM = "3.0.1",
+var WP = "3.0.1",
     qr = new Map,
-    VM = nm.concat(Pf),
+    VP = nm.concat(Tf),
     y_ = {
         id: "annotation",
-        version: WM,
+        version: WP,
         beforeRegister() {
-            DP("chart.js", "4.0", Fn.version)
+            MD("chart.js", "4.0", Fn.version)
         },
         afterRegister() {
             Fn.register(Zr)
         },
         afterUnregister() {
             Fn.unregister(Zr)
         },
@@ -26672,39 +26669,39 @@
         beforeUpdate(t, e, n) {
             let i = qr.get(t),
                 r = i.annotations = [],
                 o = n.annotations;
             we(o) ? Object.keys(o).forEach(s => {
                 let a = o[s];
                 we(a) && (a.id = s, r.push(a))
-            }) : Re(o) && r.push(...o), iM(r, t.scales)
+            }) : Re(o) && r.push(...o), iP(r, t.scales)
         },
         afterDataLimits(t, e) {
             let n = qr.get(t);
-            nM(t, e.scale, n.annotations.filter(i => i.display && i.adjustScaleRange))
+            nP(t, e.scale, n.annotations.filter(i => i.display && i.adjustScaleRange))
         },
         afterUpdate(t, e, n) {
             let i = qr.get(t);
-            QP(t, i, n), NM(t, i, n, e.mode), i.visibleElements = i.elements.filter(r => !r.skip && r.options.display), tM(t, i, n)
+            GD(t, i, n), NP(t, i, n, e.mode), i.visibleElements = i.elements.filter(r => !r.skip && r.options.display), tP(t, i, n)
         },
         beforeDatasetsDraw(t, e, n) {
-            Ef(t, "beforeDatasetsDraw", n.clip)
+            Cf(t, "beforeDatasetsDraw", n.clip)
         },
         afterDatasetsDraw(t, e, n) {
-            Ef(t, "afterDatasetsDraw", n.clip)
+            Cf(t, "afterDatasetsDraw", n.clip)
         },
         beforeDraw(t, e, n) {
-            Ef(t, "beforeDraw", n.clip)
+            Cf(t, "beforeDraw", n.clip)
         },
         afterDraw(t, e, n) {
-            Ef(t, "afterDraw", n.clip)
+            Cf(t, "afterDraw", n.clip)
         },
         beforeEvent(t, e, n) {
             let i = qr.get(t);
-            KP(i, e.event, n) && (e.changed = !0)
+            QD(i, e.event, n) && (e.changed = !0)
         },
         afterDestroy(t) {
             qr.delete(t)
         },
         _getState(t) {
             return qr.get(t)
         },
@@ -26725,15 +26722,15 @@
                 drawTime: "afterDatasetsDraw",
                 init: !1,
                 label: {}
             }
         },
         descriptors: {
             _indexable: !1,
-            _scriptable: t => !VM.includes(t) && t !== "init",
+            _scriptable: t => !VP.includes(t) && t !== "init",
             annotations: {
                 _allKeys: !1,
                 _fallback: (t, e) => `elements.${Zr[rm(e.type)].id}`
             },
             interaction: {
                 _fallback: !0
             },
@@ -26744,69 +26741,60 @@
                 },
                 _indexable: qg
             }
         },
         additionalOptionScopes: [""]
     };
 
-function Ef(t, e, n) {
+function Cf(t, e, n) {
     let {
         ctx: i,
         chartArea: r
     } = t, o = qr.get(t);
     n && Wr(i, r);
-    let s = UM(o.visibleElements, e).sort((a, l) => a.element.options.z - l.element.options.z);
-    for (let a of s) $M(i, r, o, a);
+    let s = UP(o.visibleElements, e).sort((a, l) => a.element.options.z - l.element.options.z);
+    for (let a of s) $P(i, r, o, a);
     n && Vr(i)
 }
 
-function UM(t, e) {
+function UP(t, e) {
     let n = [];
     for (let i of t)
         if (i.options.drawTime === e && n.push({
                 element: i,
                 main: !0
             }), i.elements && i.elements.length)
             for (let r of i.elements) r.options.display && r.options.drawTime === e && n.push({
                 element: r
             });
     return n
 }
 
-function $M(t, e, n, i) {
+function $P(t, e, n, i) {
     let r = i.element;
     i.main ? (F1(n, r, "beforeDraw"), r.draw(t, e), F1(n, r, "afterDraw")) : r.draw(t, e)
 }
 Lg.register(L1);
 Lg.register(y_);
-
-function YM(t) {
-    return typeof t == "object" && t !== null && Object.keys(t).length === 0
-}
-
-function XM(t) {
-    return !t.length
-}
-var qM = ix(() => {
-        let [t, e] = Eo("bands"), [n, i] = Eo("dos"), [r, o] = Eo("plot_fermilevel"), [s, a] = Eo("show_legend"), [l, c] = Eo("energy_range"), [d, g] = Eo("bands_color");
+var YP = ix(() => {
+        let [t, e] = Eo("bands"), [n, i] = Eo("dos"), [r, o] = Eo("energy_range"), [s, a] = Eo("dos_range"), [l, c] = Eo("bands_color"), [d, g] = Eo("format_settings");
         return v_.createElement(h1, {
             bandsDataList: t,
-            dosData: YM(n) ? void 0 : n,
-            showFermi: r,
-            showLegend: s,
-            yLimit: l,
-            dosRange: [],
-            colorInfo: XM(d) ? void 0 : d
+            dosData: n,
+            energyRange: r,
+            dosRange: s,
+            bandsColorInfo: l,
+            formatSettings: d
         })
     }),
-    ID = {
-        render: qM
+    LM = {
+        render: YP
     };
 export {
-    ID as
+    LM as
     default
 };
 /*! Bundled license information:
 
 react/cjs/react.production.min.js:
   (**
    * @license React
```

### Comparing `widget_bandsplot-0.6.4/pyproject.toml` & `widget_bandsplot-0.7.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "widget-bandsplot"
-version = "0.6.4"
+version = "0.7.0"
 dependencies = [
   "anywidget~=0.9.3"
 ]
 readme = "README.md"
 
 [project.optional-dependencies]
 dev = [
@@ -33,15 +33,15 @@
 dependencies = ["hatch-jupyter-builder>=0.5.0"]
 
 [tool.hatch.build.hooks.jupyter-builder.build-kwargs]
 npm = "npm"
 build_cmd = "build"
 
 [tool.bumpver]
-current_version = "v0.6.4"
+current_version = "v0.7.0"
 version_pattern = "vMAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `widget_bandsplot-0.6.4/PKG-INFO` & `widget_bandsplot-0.7.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.3
-Name: widget-bandsplot
-Version: 0.6.4
-Requires-Dist: anywidget~=0.9.3
-Provides-Extra: dev
-Requires-Dist: bumpver==2023.1129; extra == 'dev'
-Requires-Dist: jupyterlab; extra == 'dev'
-Requires-Dist: watchfiles; extra == 'dev'
-Description-Content-Type: text/markdown
-
 # Jupyter widget: Band structure visualizer
 
 [![PyPI version](https://badge.fury.io/py/widget-bandsplot.svg)](https://badge.fury.io/py/widget-bandsplot)
 
 A Jupyter widget to plot band structures and density of states. The widget is using the [mc-react-bands](https://github.com/materialscloud-org/mc-react-bands) Javascript package and is turned into a Jupyter widget with [anywidget](https://anywidget.dev/).
 
 ## Installation & usage
@@ -35,12 +25,25 @@
 ```sh
 npm install
 npm run dev
 ```
 
 Open `examples/example.ipynb` in Jupyter notebook or lab to start developing. Changes made in `js/` will be reflected in the notebook.
 
+### Releasing and publishing a new version
+
+In order to make a new release of the library and publish to PYPI, run
+
+```bash
+bumpver update --major/--minor/--patch
+```
+
+This will
+
+- update version numbers, make a corresponding `git commit` and a `git tag`;
+- push this commit and tag to Github, which triggers the Github Action that makes a new Github Release and publishes the package to PYPI.
+
 ## Acknowledgements
 
 We acknowledge support from the EPFL Open Science Fund via the [OSSCAR](http://www.osscar.org) project.
 
 <img src='https://www.osscar.org/_images/logos.png' width='700'>
```

