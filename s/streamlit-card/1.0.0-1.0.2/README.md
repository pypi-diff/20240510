# Comparing `tmp/streamlit-card-1.0.0.tar.gz` & `tmp/streamlit_card-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-card-1.0.0.tar", last modified: Thu Dec  7 11:31:01 2023, max compression
+gzip compressed data, was "streamlit_card-1.0.2.tar", last modified: Fri May 10 14:03:54 2024, max compression
```

## Comparing `streamlit-card-1.0.0.tar` & `streamlit_card-1.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 11:31:01.086346 streamlit-card-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-12-07 11:30:16.000000 streamlit-card-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-12-07 11:30:16.000000 streamlit-card-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3970 2023-12-07 11:31:01.086346 streamlit-card-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2023-12-07 11:30:16.000000 streamlit-card-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-07 11:31:01.086346 streamlit-card-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      963 2023-12-07 11:30:16.000000 streamlit-card-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 11:31:01.078346 streamlit-card-1.0.0/streamlit_card/
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2023-12-07 11:30:16.000000 streamlit-card-1.0.0/streamlit_card/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 11:31:01.078346 streamlit-card-1.0.0/streamlit_card/frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 11:31:01.082346 streamlit-card-1.0.0/streamlit_card/frontend/build/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2023-12-07 11:30:51.000000 streamlit-card-1.0.0/streamlit_card/frontend/build/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)   197459 2023-12-07 11:30:38.000000 streamlit-card-1.0.0/streamlit_card/frontend/build/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   646432 2023-12-07 11:30:38.000000 streamlit-card-1.0.0/streamlit_card/frontend/build/bootstrap.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2023-12-07 11:30:51.000000 streamlit-card-1.0.0/streamlit_card/frontend/build/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      406 2023-12-07 11:30:51.000000 streamlit-card-1.0.0/streamlit_card/frontend/build/precache-manifest.bfe10d1366557df1b3182a591c32005f.js
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2023-12-07 11:30:51.000000 streamlit-card-1.0.0/streamlit_card/frontend/build/service-worker.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 11:31:01.078346 streamlit-card-1.0.0/streamlit_card/frontend/build/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 11:31:01.086346 streamlit-card-1.0.0/streamlit_card/frontend/build/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)   498410 2023-12-07 11:30:51.000000 streamlit-card-1.0.0/streamlit_card/frontend/build/static/js/2.f9e75198.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  2066554 2023-12-07 11:30:51.000000 streamlit-card-1.0.0/streamlit_card/frontend/build/static/js/2.f9e75198.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2023-12-07 11:30:51.000000 streamlit-card-1.0.0/streamlit_card/frontend/build/static/js/main.e9936605.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     6452 2023-12-07 11:30:51.000000 streamlit-card-1.0.0/streamlit_card/frontend/build/static/js/main.e9936605.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2023-12-07 11:30:51.000000 streamlit-card-1.0.0/streamlit_card/frontend/build/static/js/runtime~main.d653cc00.js
--rw-r--r--   0 runner    (1001) docker     (127)     7997 2023-12-07 11:30:51.000000 streamlit-card-1.0.0/streamlit_card/frontend/build/static/js/runtime~main.d653cc00.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 11:31:01.086346 streamlit-card-1.0.0/streamlit_card.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3970 2023-12-07 11:31:01.000000 streamlit-card-1.0.0/streamlit_card.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      965 2023-12-07 11:31:01.000000 streamlit-card-1.0.0/streamlit_card.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-07 11:31:01.000000 streamlit-card-1.0.0/streamlit_card.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-07 11:31:01.000000 streamlit-card-1.0.0/streamlit_card.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-07 11:31:01.000000 streamlit-card-1.0.0/streamlit_card.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:03:54.990958 streamlit_card-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-10 14:03:13.000000 streamlit_card-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-10 14:03:13.000000 streamlit_card-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-05-10 14:03:54.990958 streamlit_card-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-10 14:03:13.000000 streamlit_card-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 14:03:54.990958 streamlit_card-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-10 14:03:13.000000 streamlit_card-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:03:54.982958 streamlit_card-1.0.2/streamlit_card/
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-10 14:03:13.000000 streamlit_card-1.0.2/streamlit_card/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:03:54.982958 streamlit_card-1.0.2/streamlit_card/frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:03:54.986958 streamlit_card-1.0.2/streamlit_card/frontend/build/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-10 14:03:50.000000 streamlit_card-1.0.2/streamlit_card/frontend/build/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)   197459 2024-05-10 14:03:37.000000 streamlit_card-1.0.2/streamlit_card/frontend/build/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   646432 2024-05-10 14:03:37.000000 streamlit_card-1.0.2/streamlit_card/frontend/build/bootstrap.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-10 14:03:50.000000 streamlit_card-1.0.2/streamlit_card/frontend/build/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-10 14:03:50.000000 streamlit_card-1.0.2/streamlit_card/frontend/build/precache-manifest.75bb9f3585c81fa1fdeb8616b6e03916.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-10 14:03:50.000000 streamlit_card-1.0.2/streamlit_card/frontend/build/service-worker.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:03:54.982958 streamlit_card-1.0.2/streamlit_card/frontend/build/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:03:54.990958 streamlit_card-1.0.2/streamlit_card/frontend/build/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   498410 2024-05-10 14:03:50.000000 streamlit_card-1.0.2/streamlit_card/frontend/build/static/js/2.f9e75198.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  2066554 2024-05-10 14:03:50.000000 streamlit_card-1.0.2/streamlit_card/frontend/build/static/js/2.f9e75198.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-10 14:03:50.000000 streamlit_card-1.0.2/streamlit_card/frontend/build/static/js/main.80cd56d8.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-05-10 14:03:50.000000 streamlit_card-1.0.2/streamlit_card/frontend/build/static/js/main.80cd56d8.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-10 14:03:50.000000 streamlit_card-1.0.2/streamlit_card/frontend/build/static/js/runtime~main.d653cc00.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-05-10 14:03:50.000000 streamlit_card-1.0.2/streamlit_card/frontend/build/static/js/runtime~main.d653cc00.js.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:03:54.990958 streamlit_card-1.0.2/streamlit_card.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-05-10 14:03:54.000000 streamlit_card-1.0.2/streamlit_card.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-10 14:03:54.000000 streamlit_card-1.0.2/streamlit_card.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 14:03:54.000000 streamlit_card-1.0.2/streamlit_card.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-10 14:03:54.000000 streamlit_card-1.0.2/streamlit_card.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-10 14:03:54.000000 streamlit_card-1.0.2/streamlit_card.egg-info/top_level.txt
```

### Comparing `streamlit-card-1.0.0/LICENSE` & `streamlit_card-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-card-1.0.0/PKG-INFO` & `streamlit_card-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-card
-Version: 1.0.0
+Version: 1.0.2
 Summary: A streamlit component, to make UI cards
 Home-page: https://github.com/gamcoh/st-card
 Author: gamcoh
 Author-email: cohengamliel8@gmail.com
 Keywords: card streamlit streamlit-component
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `streamlit-card-1.0.0/README.md` & `streamlit_card-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-card-1.0.0/setup.py` & `streamlit_card-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md") as readme_file:
     readme = readme_file.read()
 
 
 setuptools.setup(
     name="streamlit-card",
-    version="1.0.0",
+    version="1.0.2",
     author="gamcoh",
     author_email="cohengamliel8@gmail.com",
     description="A streamlit component, to make UI cards",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/gamcoh/st-card",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit-card-1.0.0/streamlit_card/__init__.py` & `streamlit_card-1.0.2/streamlit_card/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-card-1.0.0/streamlit_card/frontend/build/bootstrap.min.css` & `streamlit_card-1.0.2/streamlit_card/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit-card-1.0.0/streamlit_card/frontend/build/bootstrap.min.css.map` & `streamlit_card-1.0.2/streamlit_card/frontend/build/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-card-1.0.0/streamlit_card/frontend/build/index.html` & `streamlit_card-1.0.2/streamlit_card/frontend/build/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(l){function e(e){for(var r,t,n=e[0],o=e[1],u=e[2],f=0,i=[];f<n.length;f++)t=n[f],p[t]&&i.push(p[t][0]),p[t]=0;for(r in o)Object.prototype.hasOwnProperty.call(o,r)&&(l[r]=o[r]);for(s&&s(e);i.length;)i.shift()();return c.push.apply(c,u||[]),a()}function a(){for(var e,r=0;r<c.length;r++){for(var t=c[r],n=!0,o=1;o<t.length;o++){var u=t[o];0!==p[u]&&(n=!1)}n&&(c.splice(r--,1),e=f(f.s=t[0]))}return e}var t={},p={1:0},c=[];function f(e){if(t[e])return t[e].exports;var r=t[e]={i:e,l:!1,exports:{}};return l[e].call(r.exports,r,r.exports,f),r.l=!0,r.exports}f.m=l,f.c=t,f.d=function(e,r,t){f.o(e,r)||Object.defineProperty(e,r,{enumerable:!0,get:t})},f.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},f.t=function(r,e){if(1&e&&(r=f(r)),8&e)return r;if(4&e&&"object"==typeof r&&r&&r.__esModule)return r;var t=Object.create(null);if(f.r(t),Object.defineProperty(t,"default",{enumerable:!0,value:r}),2&e&&"string"!=typeof r)for(var n in r)f.d(t,n,function(e){return r[e]}.bind(null,n));return t},f.n=function(e){var r=e&&e.__esModule?function(){return e.default}:function(){return e};return f.d(r,"a",r),r},f.o=function(e,r){return Object.prototype.hasOwnProperty.call(e,r)},f.p="./";var r=window.webpackJsonp=window.webpackJsonp||[],n=r.push.bind(r);r.push=e,r=r.slice();for(var o=0;o<r.length;o++)e(r[o]);var s=n;a()}([])</script><script src="./static/js/2.f9e75198.chunk.js"></script><script src="./static/js/main.e9936605.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(l){function e(e){for(var r,t,n=e[0],o=e[1],u=e[2],f=0,i=[];f<n.length;f++)t=n[f],p[t]&&i.push(p[t][0]),p[t]=0;for(r in o)Object.prototype.hasOwnProperty.call(o,r)&&(l[r]=o[r]);for(s&&s(e);i.length;)i.shift()();return c.push.apply(c,u||[]),a()}function a(){for(var e,r=0;r<c.length;r++){for(var t=c[r],n=!0,o=1;o<t.length;o++){var u=t[o];0!==p[u]&&(n=!1)}n&&(c.splice(r--,1),e=f(f.s=t[0]))}return e}var t={},p={1:0},c=[];function f(e){if(t[e])return t[e].exports;var r=t[e]={i:e,l:!1,exports:{}};return l[e].call(r.exports,r,r.exports,f),r.l=!0,r.exports}f.m=l,f.c=t,f.d=function(e,r,t){f.o(e,r)||Object.defineProperty(e,r,{enumerable:!0,get:t})},f.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},f.t=function(r,e){if(1&e&&(r=f(r)),8&e)return r;if(4&e&&"object"==typeof r&&r&&r.__esModule)return r;var t=Object.create(null);if(f.r(t),Object.defineProperty(t,"default",{enumerable:!0,value:r}),2&e&&"string"!=typeof r)for(var n in r)f.d(t,n,function(e){return r[e]}.bind(null,n));return t},f.n=function(e){var r=e&&e.__esModule?function(){return e.default}:function(){return e};return f.d(r,"a",r),r},f.o=function(e,r){return Object.prototype.hasOwnProperty.call(e,r)},f.p="./";var r=window.webpackJsonp=window.webpackJsonp||[],n=r.push.bind(r);r.push=e,r=r.slice();for(var o=0;o<r.length;o++)e(r[o]);var s=n;a()}([])</script><script src="./static/js/2.f9e75198.chunk.js"></script><script src="./static/js/main.80cd56d8.chunk.js"></script></body></html>
```

### Comparing `streamlit-card-1.0.0/streamlit_card/frontend/build/service-worker.js` & `streamlit_card-1.0.2/streamlit_card/frontend/build/service-worker.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -10,15 +10,15 @@
  * and re-run your build process.
  * See https://goo.gl/2aRDsh
  */
 
 importScripts("https://storage.googleapis.com/workbox-cdn/releases/3.6.3/workbox-sw.js");
 
 importScripts(
-    "./precache-manifest.bfe10d1366557df1b3182a591c32005f.js"
+    "./precache-manifest.75bb9f3585c81fa1fdeb8616b6e03916.js"
 );
 
 workbox.clientsClaim();
 
 /**
  * The workboxSW.precacheAndRoute() method efficiently caches and responds to
  * requests for URLs in the manifest.
```

### Comparing `streamlit-card-1.0.0/streamlit_card/frontend/build/static/js/2.f9e75198.chunk.js` & `streamlit_card-1.0.2/streamlit_card/frontend/build/static/js/2.f9e75198.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-card-1.0.0/streamlit_card/frontend/build/static/js/2.f9e75198.chunk.js.map` & `streamlit_card-1.0.2/streamlit_card/frontend/build/static/js/2.f9e75198.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-card-1.0.0/streamlit_card/frontend/build/static/js/main.e9936605.chunk.js` & `streamlit_card-1.0.2/streamlit_card/frontend/build/static/js/main.80cd56d8.chunk.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -35,15 +35,15 @@
                                 u = g.a.div(Object(c.a)({
                                     display: "flex",
                                     cursor: "pointer",
                                     fontFamily: "".concat(l.font, ", 'Segoe UI', 'Roboto', sans-serif"),
                                     height: "".concat(250, "px"),
                                     borderRadius: "20px",
                                     overflow: "hidden",
-                                    backgroundImage: "url(".concat(r, ")"),
+                                    backgroundImage: r ? "url(".concat(r, ")") : "none",
                                     backgroundPosition: "center",
                                     backgroundSize: "cover",
                                     backgroundRepeat: "no-repeat",
                                     boxShadow: "0px 0px 40px rgba(0, 0, 0, 0.2)",
                                     margin: "".concat(s, "px"),
                                     marginLeft: "auto",
                                     marginRight: "auto",
@@ -110,8 +110,8 @@
             i.a.render(o.a.createElement(o.a.StrictMode, null, o.a.createElement(b, null)), document.getElementById("root"))
         }
     },
     [
         [17, 1, 2]
     ]
 ]);
-//# sourceMappingURL=main.e9936605.chunk.js.map
+//# sourceMappingURL=main.80cd56d8.chunk.js.map
```

### Comparing `streamlit-card-1.0.0/streamlit_card/frontend/build/static/js/main.e9936605.chunk.js.map` & `streamlit_card-1.0.2/streamlit_card/frontend/build/static/js/main.80cd56d8.chunk.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8095238095238095%*

 * *Differences: {"'file'": "'static/js/main.80cd56d8.chunk.js'",*

 * * "'mappings'": "'mOAQMA,6MASGC,OAAS,WAAiB,IAAAC,EACMC,EAAKC,MAAMC,KAA1CC,EADyBJ,EACzBI,MAAOC,EADkBL,EAClBK,KAAMC,EADYN,EACZM,MAAOC,EADKP,EACLO,OAKlBC,EAAUP,EAAKC,MAAfM,MAIR,IAAKA,EACH,OAAOC,EAAAC,EAAAC,cAAA,kEAGT,IAEMC,EAASL,EAAOM,KAAKD,QAAU,GAE/Bd,EAAOgB,IAAOC,IAAPC,OAAAC,EAAA,EAAAD,CAAA,CAETE,QAAS,OACTC,OAAQ,UACRC,WAAU,GAAAC,OAAKb,EAAMc,KAAX,sCACVC,OAAM,GAAAF,OATK,IASL,MACNG,aAAc,OACdC,SAAU,SACVC,gBAAiBpB,EAAK,OAAAe,OAAUf,EAAV,KAAqB,OAC3CqB,mBAAoB,SACpBC,eA […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.e9936605.chunk.js",
-    "mappings": "mOAQMA,6MASGC,OAAS,WAAiB,IAAAC,EACMC,EAAKC,MAAMC,KAA1CC,EADyBJ,EACzBI,MAAOC,EADkBL,EAClBK,KAAMC,EADYN,EACZM,MAAOC,EADKP,EACLO,OAKlBC,EAAUP,EAAKC,MAAfM,MAIR,IAAKA,EACH,OAAOC,EAAAC,EAAAC,cAAA,kEAGT,IAEMC,EAASL,EAAOM,KAAKD,QAAU,GAE/Bd,EAAOgB,IAAOC,IAAPC,OAAAC,EAAA,EAAAD,CAAA,CAETE,QAAS,OACTC,OAAQ,UACRC,WAAU,GAAAC,OAAKb,EAAMc,KAAX,sCACVC,OAAM,GAAAF,OATK,IASL,MACNG,aAAc,OACdC,SAAU,SACVC,gBAAe,OAAAL,OAASf,EAAT,KACfqB,mBAAoB,SACpBC,eAAgB,QAChBC,iBAAkB,YAClBC,UAAW,kCACXlB,OAAM,GAAAS,OAAKT,EAAL,MACNmB,WAAY,OACZC,YAAa,OACbC,cAAe,SACfC,eAAgB,SAChBC,WAAY,SACZC,UAAW,SACXC,MAAO7B,EAAM8B,UACbC,MAAK,GAAAlB,OAxBK,IAwBL,MACLmB,SAAU,WACVC,WAAY,wBACTlC,EAAOM,MAxBD,qLAuCP6B,EAAS5B,IAAOC,IAAPC,OAAAC,EAAA,EAAAD,CAAA,CACb2B,QAAS/B,EACT2B,MAAO,QACJhC,EAAOQ,MAGN6B,EAAQ9B,IAAO+B,GAAP7B,OAAAC,EAAA,EAAAD,CAAA,CACZqB,MAAO,QACPS,OAAQ,IACRC,SAAU,MACVC,WAAY,UACTzC,EAAOH,QAGN6C,EAAOnC,IAAOoC,EAAPlC,OAAAC,EAAA,EAAAD,CAAA,CACXqB,MAAO,QACPW,WAAY,SACZF,OAAQ,IACRC,SAAU,MACVnC,OAAQ,KACLL,EAAOF,OAGN8C,EAASrC,IAAOC,IAAPC,OAAAC,EAAA,EAAAD,CAAA,CACboC,gBAAiB,qBACjB7B,OAAQ,OACRgB,MAAO,OACPC,SAAU,WACVa,IAAK,IACLC,KAAM,IACNR,OAAQ,KACLvC,EAAOgD,SAIQ,kBAATlD,IACTA,EAAO,CAACA,IAIV,IADA,IAAImD,EAAQ,GACHC,EAAI,EAAGA,EAAIpD,EAAKqD,OAAQD,IAAK,CACpC,IAAME,EAAItD,EAAKoD,GACfD,EAAMI,KAAKnD,EAAAC,EAAAC,cAACsC,EAAD,KAAOU,IAGpB,OACElD,EAAAC,EAAAC,cAAC+B,EAAD,KACEjC,EAAAC,EAAAC,cAACb,EAAD,CAAM+D,QAAS5D,EAAK4D,SAClBpD,EAAAC,EAAAC,cAACwC,EAAD,MACA1C,EAAAC,EAAAC,cAACiC,EAAD,KAAQxC,GACPoD,OAMDK,QAAU,WACZ5D,EAAKC,MAAMC,KAAK2D,KAClBC,OAAOC,KAAK/D,EAAKC,MAAMC,KAAK2D,IAAK,UAEnCG,IAAUC,mBAAkB,wFA5H5BD,IAAUE,6DAIVF,IAAUE,wBANKC,KAkIJC,cAAwBvE,GCtIvCwE,IAASvE,OACPU,EAAAC,EAAAC,cAACF,EAAAC,EAAM6D,WAAP,KACE9D,EAAAC,EAAAC,cAAC6D,EAAD,OAEFC,SAASC,eAAe",
+    "file": "static/js/main.80cd56d8.chunk.js",
+    "mappings": "mOAQMA,6MASGC,OAAS,WAAiB,IAAAC,EACMC,EAAKC,MAAMC,KAA1CC,EADyBJ,EACzBI,MAAOC,EADkBL,EAClBK,KAAMC,EADYN,EACZM,MAAOC,EADKP,EACLO,OAKlBC,EAAUP,EAAKC,MAAfM,MAIR,IAAKA,EACH,OAAOC,EAAAC,EAAAC,cAAA,kEAGT,IAEMC,EAASL,EAAOM,KAAKD,QAAU,GAE/Bd,EAAOgB,IAAOC,IAAPC,OAAAC,EAAA,EAAAD,CAAA,CAETE,QAAS,OACTC,OAAQ,UACRC,WAAU,GAAAC,OAAKb,EAAMc,KAAX,sCACVC,OAAM,GAAAF,OATK,IASL,MACNG,aAAc,OACdC,SAAU,SACVC,gBAAiBpB,EAAK,OAAAe,OAAUf,EAAV,KAAqB,OAC3CqB,mBAAoB,SACpBC,eAAgB,QAChBC,iBAAkB,YAClBC,UAAW,kCACXlB,OAAM,GAAAS,OAAKT,EAAL,MACNmB,WAAY,OACZC,YAAa,OACbC,cAAe,SACfC,eAAgB,SAChBC,WAAY,SACZC,UAAW,SACXC,MAAO7B,EAAM8B,UACbC,MAAK,GAAAlB,OAxBK,IAwBL,MACLmB,SAAU,WACVC,WAAY,wBACTlC,EAAOM,MAxBD,qLAuCP6B,EAAS5B,IAAOC,IAAPC,OAAAC,EAAA,EAAAD,CAAA,CACb2B,QAAS/B,EACT2B,MAAO,QACJhC,EAAOQ,MAGN6B,EAAQ9B,IAAO+B,GAAP7B,OAAAC,EAAA,EAAAD,CAAA,CACZqB,MAAO,QACPS,OAAQ,IACRC,SAAU,MACVC,WAAY,UACTzC,EAAOH,QAGN6C,EAAOnC,IAAOoC,EAAPlC,OAAAC,EAAA,EAAAD,CAAA,CACXqB,MAAO,QACPW,WAAY,SACZF,OAAQ,IACRC,SAAU,MACVnC,OAAQ,KACLL,EAAOF,OAGN8C,EAASrC,IAAOC,IAAPC,OAAAC,EAAA,EAAAD,CAAA,CACboC,gBAAiB,qBACjB7B,OAAQ,OACRgB,MAAO,OACPC,SAAU,WACVa,IAAK,IACLC,KAAM,IACNR,OAAQ,KACLvC,EAAOgD,SAIQ,kBAATlD,IACTA,EAAO,CAACA,IAIV,IADA,IAAImD,EAAQ,GACHC,EAAI,EAAGA,EAAIpD,EAAKqD,OAAQD,IAAK,CACpC,IAAME,EAAItD,EAAKoD,GACfD,EAAMI,KAAKnD,EAAAC,EAAAC,cAACsC,EAAD,KAAOU,IAGpB,OACElD,EAAAC,EAAAC,cAAC+B,EAAD,KACEjC,EAAAC,EAAAC,cAACb,EAAD,CAAM+D,QAAS5D,EAAK4D,SAClBpD,EAAAC,EAAAC,cAACwC,EAAD,MACA1C,EAAAC,EAAAC,cAACiC,EAAD,KAAQxC,GACPoD,OAMDK,QAAU,WACZ5D,EAAKC,MAAMC,KAAK2D,KAClBC,OAAOC,KAAK/D,EAAKC,MAAMC,KAAK2D,IAAK,UAEnCG,IAAUC,mBAAkB,wFA5H5BD,IAAUE,6DAIVF,IAAUE,wBANKC,KAkIJC,cAAwBvE,GCtIvCwE,IAASvE,OACPU,EAAAC,EAAAC,cAACF,EAAAC,EAAM6D,WAAP,KACE9D,EAAAC,EAAAC,cAAC6D,EAAD,OAEFC,SAASC,eAAe",
     "names": [
         "Card",
         "render",
         "_this$props$args",
         "_this",
         "props",
         "args",
@@ -82,12 +82,12 @@
     ],
     "sourceRoot": "",
     "sources": [
         "stCard.tsx",
         "index.tsx"
     ],
     "sourcesContent": [
-        "import {\n  Streamlit,\n  StreamlitComponentBase,\n  withStreamlitConnection,\n} from \"streamlit-component-lib\";\nimport React, { ReactNode } from \"react\";\nimport styled from \"@emotion/styled\";\n\nclass Card extends StreamlitComponentBase {\n  public componentDidUpdate(): void {\n    Streamlit.setFrameHeight();\n  }\n\n  public componentDidMount(): void {\n    Streamlit.setFrameHeight();\n  }\n\n  public render = (): ReactNode => {\n    let { title, text, image, styles } = this.props.args;\n\n    // Streamlit sends us a theme object via props that we can use to ensure\n    // that our component has visuals that match the active theme in a\n    // streamlit app.\n    const { theme } = this.props;\n\n    // Maintain compatibility with older versions of Streamlit that don't send\n    // a theme object.\n    if (!theme) {\n      return <div>Theme is undefined, please check streamlit version.</div>;\n    }\n\n    const height = 250;\n    const width = 300;\n    const margin = styles.card.margin || 40;\n\n    const Card = styled.div(\n      {\n        display: \"flex\",\n        cursor: \"pointer\",\n        fontFamily: `${theme.font}, 'Segoe UI', 'Roboto', sans-serif`,\n        height: `${height}px`,\n        borderRadius: \"20px\",\n        overflow: \"hidden\",\n        backgroundImage: `url(${image})`,\n        backgroundPosition: \"center\",\n        backgroundSize: \"cover\",\n        backgroundRepeat: \"no-repeat\",\n        boxShadow: \"0px 0px 40px rgba(0, 0, 0, 0.2)\",\n        margin: `${margin}px`,\n        marginLeft: \"auto\",\n        marginRight: \"auto\",\n        flexDirection: \"column\",\n        justifyContent: \"center\",\n        alignItems: \"center\",\n        textAlign: \"center\",\n        color: theme.textColor,\n        width: `${width}px`,\n        position: \"relative\",\n        transition: \"all 0.3s ease-in-out\",\n        ...styles.card,\n      },\n      `\n      & {\n        transform: scale(0.95);\n      }\n      &:hover {\n        transform: scale(1);\n      }\n      &:active {\n        transform: scale(0.95);\n      }\n      `\n    );\n\n    const Parent = styled.div({\n      padding: margin,\n      width: \"100%\",\n      ...styles.div,\n    });\n\n    const Title = styled.h2({\n      color: \"white\",\n      zIndex: \"2\",\n      fontSize: \"2em\",\n      fontWeight: \"bolder\",\n      ...styles.title,\n    });\n\n    const Text = styled.p({\n      color: \"white\",\n      fontWeight: \"bolder\",\n      zIndex: \"2\",\n      fontSize: \"1em\",\n      margin: \"0\",\n      ...styles.text,\n    });\n\n    const Filter = styled.div({\n      backgroundColor: \"rgba(0, 0, 0, 0.5)\",\n      height: \"100%\",\n      width: \"100%\",\n      position: \"absolute\",\n      top: \"0\",\n      left: \"0\",\n      zIndex: \"1\",\n      ...styles.filter,\n    });\n\n    // if the text is a string, convert it to an array\n    if (typeof text === \"string\") {\n      text = [text];\n    }\n\n    let texts = [];\n    for (let i = 0; i < text.length; i++) {\n      const t = text[i];\n      texts.push(<Text>{t}</Text>);\n    }\n\n    return (\n      <Parent>\n        <Card onClick={this.onClick}>\n          <Filter />\n          <Title>{title}</Title>\n          {texts}\n        </Card>\n      </Parent>\n    );\n  };\n\n  private onClick = (): void => {\n    if (this.props.args.url) {\n      window.open(this.props.args.url, \"_blank\");\n    }\n    Streamlit.setComponentValue(true);\n  };\n}\n\nexport default withStreamlitConnection(Card);\n",
+        "import {\n  Streamlit,\n  StreamlitComponentBase,\n  withStreamlitConnection,\n} from \"streamlit-component-lib\";\nimport React, { ReactNode } from \"react\";\nimport styled from \"@emotion/styled\";\n\nclass Card extends StreamlitComponentBase {\n  public componentDidUpdate(): void {\n    Streamlit.setFrameHeight();\n  }\n\n  public componentDidMount(): void {\n    Streamlit.setFrameHeight();\n  }\n\n  public render = (): ReactNode => {\n    let { title, text, image, styles } = this.props.args;\n\n    // Streamlit sends us a theme object via props that we can use to ensure\n    // that our component has visuals that match the active theme in a\n    // streamlit app.\n    const { theme } = this.props;\n\n    // Maintain compatibility with older versions of Streamlit that don't send\n    // a theme object.\n    if (!theme) {\n      return <div>Theme is undefined, please check streamlit version.</div>;\n    }\n\n    const height = 250;\n    const width = 300;\n    const margin = styles.card.margin || 40;\n\n    const Card = styled.div(\n      {\n        display: \"flex\",\n        cursor: \"pointer\",\n        fontFamily: `${theme.font}, 'Segoe UI', 'Roboto', sans-serif`,\n        height: `${height}px`,\n        borderRadius: \"20px\",\n        overflow: \"hidden\",\n        backgroundImage: image ? `url(${image})` : \"none\",\n        backgroundPosition: \"center\",\n        backgroundSize: \"cover\",\n        backgroundRepeat: \"no-repeat\",\n        boxShadow: \"0px 0px 40px rgba(0, 0, 0, 0.2)\",\n        margin: `${margin}px`,\n        marginLeft: \"auto\",\n        marginRight: \"auto\",\n        flexDirection: \"column\",\n        justifyContent: \"center\",\n        alignItems: \"center\",\n        textAlign: \"center\",\n        color: theme.textColor,\n        width: `${width}px`,\n        position: \"relative\",\n        transition: \"all 0.3s ease-in-out\",\n        ...styles.card,\n      },\n      `\n      & {\n        transform: scale(0.95);\n      }\n      &:hover {\n        transform: scale(1);\n      }\n      &:active {\n        transform: scale(0.95);\n      }\n      `\n    );\n\n    const Parent = styled.div({\n      padding: margin,\n      width: \"100%\",\n      ...styles.div,\n    });\n\n    const Title = styled.h2({\n      color: \"white\",\n      zIndex: \"2\",\n      fontSize: \"2em\",\n      fontWeight: \"bolder\",\n      ...styles.title,\n    });\n\n    const Text = styled.p({\n      color: \"white\",\n      fontWeight: \"bolder\",\n      zIndex: \"2\",\n      fontSize: \"1em\",\n      margin: \"0\",\n      ...styles.text,\n    });\n\n    const Filter = styled.div({\n      backgroundColor: \"rgba(0, 0, 0, 0.5)\",\n      height: \"100%\",\n      width: \"100%\",\n      position: \"absolute\",\n      top: \"0\",\n      left: \"0\",\n      zIndex: \"1\",\n      ...styles.filter,\n    });\n\n    // if the text is a string, convert it to an array\n    if (typeof text === \"string\") {\n      text = [text];\n    }\n\n    let texts = [];\n    for (let i = 0; i < text.length; i++) {\n      const t = text[i];\n      texts.push(<Text>{t}</Text>);\n    }\n\n    return (\n      <Parent>\n        <Card onClick={this.onClick}>\n          <Filter />\n          <Title>{title}</Title>\n          {texts}\n        </Card>\n      </Parent>\n    );\n  };\n\n  private onClick = (): void => {\n    if (this.props.args.url) {\n      window.open(this.props.args.url, \"_blank\");\n    }\n    Streamlit.setComponentValue(true);\n  };\n}\n\nexport default withStreamlitConnection(Card);\n",
         "import React from \"react\"\nimport ReactDOM from \"react-dom\"\nimport Card from \"./stCard\"\n\nReactDOM.render(\n  <React.StrictMode>\n    <Card />\n  </React.StrictMode>,\n  document.getElementById(\"root\")\n)\n"
     ],
     "version": 3
 }
```

### Comparing `streamlit-card-1.0.0/streamlit_card/frontend/build/static/js/runtime~main.d653cc00.js` & `streamlit_card-1.0.2/streamlit_card/frontend/build/static/js/runtime~main.d653cc00.js`

 * *Files identical despite different names*

### Comparing `streamlit-card-1.0.0/streamlit_card/frontend/build/static/js/runtime~main.d653cc00.js.map` & `streamlit_card-1.0.2/streamlit_card/frontend/build/static/js/runtime~main.d653cc00.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-card-1.0.0/streamlit_card.egg-info/PKG-INFO` & `streamlit_card-1.0.2/streamlit_card.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-card
-Version: 1.0.0
+Version: 1.0.2
 Summary: A streamlit component, to make UI cards
 Home-page: https://github.com/gamcoh/st-card
 Author: gamcoh
 Author-email: cohengamliel8@gmail.com
 Keywords: card streamlit streamlit-component
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `streamlit-card-1.0.0/streamlit_card.egg-info/SOURCES.txt` & `streamlit_card-1.0.2/streamlit_card.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 streamlit_card.egg-info/dependency_links.txt
 streamlit_card.egg-info/requires.txt
 streamlit_card.egg-info/top_level.txt
 streamlit_card/frontend/build/asset-manifest.json
 streamlit_card/frontend/build/bootstrap.min.css
 streamlit_card/frontend/build/bootstrap.min.css.map
 streamlit_card/frontend/build/index.html
-streamlit_card/frontend/build/precache-manifest.bfe10d1366557df1b3182a591c32005f.js
+streamlit_card/frontend/build/precache-manifest.75bb9f3585c81fa1fdeb8616b6e03916.js
 streamlit_card/frontend/build/service-worker.js
 streamlit_card/frontend/build/static/js/2.f9e75198.chunk.js
 streamlit_card/frontend/build/static/js/2.f9e75198.chunk.js.map
-streamlit_card/frontend/build/static/js/main.e9936605.chunk.js
-streamlit_card/frontend/build/static/js/main.e9936605.chunk.js.map
+streamlit_card/frontend/build/static/js/main.80cd56d8.chunk.js
+streamlit_card/frontend/build/static/js/main.80cd56d8.chunk.js.map
 streamlit_card/frontend/build/static/js/runtime~main.d653cc00.js
 streamlit_card/frontend/build/static/js/runtime~main.d653cc00.js.map
```

