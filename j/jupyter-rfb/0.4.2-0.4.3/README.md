# Comparing `tmp/jupyter_rfb-0.4.2.tar.gz` & `tmp/jupyter_rfb-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter_rfb-0.4.2.tar", last modified: Tue Nov  7 10:14:58 2023, max compression
+gzip compressed data, was "jupyter_rfb-0.4.3.tar", last modified: Fri May 10 07:45:19 2024, max compression
```

## Comparing `jupyter_rfb-0.4.2.tar` & `jupyter_rfb-0.4.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-11-07 10:14:58.150674 jupyter_rfb-0.4.2/
--rw-r--r--   0 almar      (501) staff       (20)     1062 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.2/LICENSE
--rw-r--r--   0 almar      (501) staff       (20)      386 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.2/MANIFEST.in
--rw-r--r--   0 almar      (501) staff       (20)      824 2023-11-07 10:14:58.150759 jupyter_rfb-0.4.2/PKG-INFO
--rw-r--r--   0 almar      (501) staff       (20)     1880 2023-06-09 13:12:17.000000 jupyter_rfb-0.4.2/README.md
--rw-r--r--   0 almar      (501) staff       (20)      182 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.2/install.json
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-11-07 10:14:58.133401 jupyter_rfb-0.4.2/js/
--rw-r--r--   0 almar      (501) staff       (20)      455 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.2/js/.eslintrc.json
--rw-r--r--   0 almar      (501) staff       (20)      157 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.2/js/README.md
--rw-r--r--   0 almar      (501) staff       (20)      647 2023-02-20 11:47:49.000000 jupyter_rfb-0.4.2/js/amd-public-path.js
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-11-07 10:14:58.135179 jupyter_rfb-0.4.2/js/dist/
--rw-r--r--   0 almar      (501) staff       (20)     8404 2023-11-07 10:14:51.000000 jupyter_rfb-0.4.2/js/dist/index.js
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-11-07 10:14:58.137882 jupyter_rfb-0.4.2/js/lib/
--rw-r--r--   0 almar      (501) staff       (20)      459 2023-02-20 11:47:49.000000 jupyter_rfb-0.4.2/js/lib/extension.js
--rw-r--r--   0 almar      (501) staff       (20)      185 2023-02-20 11:47:49.000000 jupyter_rfb-0.4.2/js/lib/index.js
--rw-r--r--   0 almar      (501) staff       (20)      522 2023-02-20 11:47:49.000000 jupyter_rfb-0.4.2/js/lib/labplugin.js
--rw-r--r--   0 almar      (501) staff       (20)    18506 2023-11-07 10:12:10.000000 jupyter_rfb-0.4.2/js/lib/widget.js
--rw-r--r--   0 almar      (501) staff       (20)     1456 2023-02-20 11:47:49.000000 jupyter_rfb-0.4.2/js/package.json
--rw-r--r--   0 almar      (501) staff       (20)     2828 2023-02-20 11:47:49.000000 jupyter_rfb-0.4.2/js/webpack.config.js
--rw-r--r--   0 almar      (501) staff       (20)   182106 2023-02-24 11:06:22.000000 jupyter_rfb-0.4.2/js/yarn.lock
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-11-07 10:14:58.140531 jupyter_rfb-0.4.2/jupyter_rfb/
--rw-r--r--   0 almar      (501) staff       (20)     1842 2023-02-24 11:04:02.000000 jupyter_rfb-0.4.2/jupyter_rfb/__init__.py
--rw-r--r--   0 almar      (501) staff       (20)     3552 2023-02-17 06:37:49.000000 jupyter_rfb-0.4.2/jupyter_rfb/_jpg.py
--rw-r--r--   0 almar      (501) staff       (20)     2416 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.2/jupyter_rfb/_png.py
--rw-r--r--   0 almar      (501) staff       (20)     4922 2023-11-07 10:12:10.000000 jupyter_rfb-0.4.2/jupyter_rfb/_utils.py
--rw-r--r--   0 almar      (501) staff       (20)      421 2023-11-07 10:14:37.000000 jupyter_rfb-0.4.2/jupyter_rfb/_version.py
--rw-r--r--   0 almar      (501) staff       (20)     5088 2023-10-25 20:55:24.000000 jupyter_rfb-0.4.2/jupyter_rfb/events.py
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-11-07 10:14:58.146351 jupyter_rfb-0.4.2/jupyter_rfb/labextension/
--rw-r--r--   0 almar      (501) staff       (20)     1572 2023-11-07 10:14:57.000000 jupyter_rfb-0.4.2/jupyter_rfb/labextension/package.json
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-11-07 10:14:58.148474 jupyter_rfb-0.4.2/jupyter_rfb/labextension/static/
--rw-r--r--   0 almar      (501) staff       (20)     8036 2023-11-07 10:14:57.000000 jupyter_rfb-0.4.2/jupyter_rfb/labextension/static/261.9ef272ff509129a4e555.js
--rw-r--r--   0 almar      (501) staff       (20)     7667 2023-11-07 10:14:57.000000 jupyter_rfb-0.4.2/jupyter_rfb/labextension/static/920.68e3589cd1cc5ef32304.js
--rw-r--r--   0 almar      (501) staff       (20)     6441 2023-11-07 10:14:57.000000 jupyter_rfb-0.4.2/jupyter_rfb/labextension/static/remoteEntry.f201b0f18d69b7610789.js
--rw-r--r--   0 almar      (501) staff       (20)      118 2023-11-07 10:14:57.000000 jupyter_rfb-0.4.2/jupyter_rfb/labextension/static/style.js
--rw-r--r--   0 almar      (501) staff       (20)       20 2023-11-07 10:14:57.000000 jupyter_rfb-0.4.2/jupyter_rfb/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-11-07 10:14:58.149128 jupyter_rfb-0.4.2/jupyter_rfb/nbextension/
--rw-r--r--   0 almar      (501) staff       (20)      531 2023-11-07 10:14:51.000000 jupyter_rfb-0.4.2/jupyter_rfb/nbextension/extension.js
--rw-r--r--   0 almar      (501) staff       (20)     8404 2023-11-07 10:14:51.000000 jupyter_rfb-0.4.2/jupyter_rfb/nbextension/index.js
--rw-r--r--   0 almar      (501) staff       (20)    16687 2023-11-07 10:12:10.000000 jupyter_rfb-0.4.2/jupyter_rfb/widget.py
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-11-07 10:14:58.146124 jupyter_rfb-0.4.2/jupyter_rfb.egg-info/
--rw-r--r--   0 almar      (501) staff       (20)      824 2023-11-07 10:14:57.000000 jupyter_rfb-0.4.2/jupyter_rfb.egg-info/PKG-INFO
--rw-r--r--   0 almar      (501) staff       (20)     1120 2023-11-07 10:14:57.000000 jupyter_rfb-0.4.2/jupyter_rfb.egg-info/SOURCES.txt
--rw-r--r--   0 almar      (501) staff       (20)        1 2023-11-07 10:14:57.000000 jupyter_rfb-0.4.2/jupyter_rfb.egg-info/dependency_links.txt
--rw-r--r--   0 almar      (501) staff       (20)        1 2022-02-04 09:25:53.000000 jupyter_rfb-0.4.2/jupyter_rfb.egg-info/not-zip-safe
--rw-r--r--   0 almar      (501) staff       (20)       46 2023-11-07 10:14:57.000000 jupyter_rfb-0.4.2/jupyter_rfb.egg-info/requires.txt
--rw-r--r--   0 almar      (501) staff       (20)       12 2023-11-07 10:14:57.000000 jupyter_rfb-0.4.2/jupyter_rfb.egg-info/top_level.txt
--rw-r--r--   0 almar      (501) staff       (20)       65 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.2/jupyter_rfb.json
--rw-r--r--   0 almar      (501) staff       (20)      153 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.2/pyproject.toml
--rw-r--r--   0 almar      (501) staff       (20)      460 2023-11-07 10:14:58.151360 jupyter_rfb-0.4.2/setup.cfg
--rw-r--r--   0 almar      (501) staff       (20)     2525 2023-04-30 21:11:03.000000 jupyter_rfb-0.4.2/setup.py
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-11-07 10:14:58.150400 jupyter_rfb-0.4.2/tests/
--rw-r--r--   0 almar      (501) staff       (20)     3443 2023-02-17 06:37:49.000000 jupyter_rfb-0.4.2/tests/test_jpg.py
--rw-r--r--   0 almar      (501) staff       (20)     2614 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.2/tests/test_png.py
--rw-r--r--   0 almar      (501) staff       (20)     3670 2023-02-17 06:37:49.000000 jupyter_rfb-0.4.2/tests/test_utils.py
--rw-r--r--   0 almar      (501) staff       (20)     8312 2023-11-07 10:12:10.000000 jupyter_rfb-0.4.2/tests/test_widget.py
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-05-10 07:45:19.084814 jupyter_rfb-0.4.3/
+-rw-r--r--   0 almar      (501) staff       (20)     1062 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.3/LICENSE
+-rw-r--r--   0 almar      (501) staff       (20)      386 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.3/MANIFEST.in
+-rw-r--r--   0 almar      (501) staff       (20)      824 2024-05-10 07:45:19.084887 jupyter_rfb-0.4.3/PKG-INFO
+-rw-r--r--   0 almar      (501) staff       (20)     1880 2023-06-09 13:12:17.000000 jupyter_rfb-0.4.3/README.md
+-rw-r--r--   0 almar      (501) staff       (20)      182 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.3/install.json
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-05-10 07:45:19.078490 jupyter_rfb-0.4.3/js/
+-rw-r--r--   0 almar      (501) staff       (20)      455 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.3/js/.eslintrc.json
+-rw-r--r--   0 almar      (501) staff       (20)      157 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.3/js/README.md
+-rw-r--r--   0 almar      (501) staff       (20)      647 2023-02-20 11:47:49.000000 jupyter_rfb-0.4.3/js/amd-public-path.js
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-05-10 07:45:19.078709 jupyter_rfb-0.4.3/js/dist/
+-rw-r--r--   0 almar      (501) staff       (20)     8563 2024-05-10 07:45:10.000000 jupyter_rfb-0.4.3/js/dist/index.js
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-05-10 07:45:19.079274 jupyter_rfb-0.4.3/js/lib/
+-rw-r--r--   0 almar      (501) staff       (20)      459 2023-02-20 11:47:49.000000 jupyter_rfb-0.4.3/js/lib/extension.js
+-rw-r--r--   0 almar      (501) staff       (20)      185 2024-05-10 07:44:48.000000 jupyter_rfb-0.4.3/js/lib/index.js
+-rw-r--r--   0 almar      (501) staff       (20)      522 2023-02-20 11:47:49.000000 jupyter_rfb-0.4.3/js/lib/labplugin.js
+-rw-r--r--   0 almar      (501) staff       (20)    18725 2024-04-16 11:03:12.000000 jupyter_rfb-0.4.3/js/lib/widget.js
+-rw-r--r--   0 almar      (501) staff       (20)     1505 2024-05-10 07:45:09.000000 jupyter_rfb-0.4.3/js/package.json
+-rw-r--r--   0 almar      (501) staff       (20)     2828 2023-02-20 11:47:49.000000 jupyter_rfb-0.4.3/js/webpack.config.js
+-rw-r--r--   0 almar      (501) staff       (20)    94847 2024-05-10 07:45:09.000000 jupyter_rfb-0.4.3/js/yarn.lock
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-05-10 07:45:19.080896 jupyter_rfb-0.4.3/jupyter_rfb/
+-rw-r--r--   0 almar      (501) staff       (20)     1842 2023-02-24 11:04:02.000000 jupyter_rfb-0.4.3/jupyter_rfb/__init__.py
+-rw-r--r--   0 almar      (501) staff       (20)     3552 2023-02-17 06:37:49.000000 jupyter_rfb-0.4.3/jupyter_rfb/_jpg.py
+-rw-r--r--   0 almar      (501) staff       (20)     2416 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.3/jupyter_rfb/_png.py
+-rw-r--r--   0 almar      (501) staff       (20)     4922 2023-11-07 10:12:10.000000 jupyter_rfb-0.4.3/jupyter_rfb/_utils.py
+-rw-r--r--   0 almar      (501) staff       (20)      445 2024-05-10 07:34:08.000000 jupyter_rfb-0.4.3/jupyter_rfb/_version.py
+-rw-r--r--   0 almar      (501) staff       (20)     5093 2024-05-10 07:32:58.000000 jupyter_rfb-0.4.3/jupyter_rfb/events.py
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-05-10 07:45:19.082365 jupyter_rfb-0.4.3/jupyter_rfb/labextension/
+-rw-r--r--   0 almar      (501) staff       (20)     1621 2024-05-10 07:45:18.000000 jupyter_rfb-0.4.3/jupyter_rfb/labextension/package.json
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-05-10 07:45:19.083216 jupyter_rfb-0.4.3/jupyter_rfb/labextension/static/
+-rw-r--r--   0 almar      (501) staff       (20)     8187 2024-05-10 07:45:18.000000 jupyter_rfb-0.4.3/jupyter_rfb/labextension/static/493.cb43b5d572b2f6b10c8e.js
+-rw-r--r--   0 almar      (501) staff       (20)     7826 2024-05-10 07:45:18.000000 jupyter_rfb-0.4.3/jupyter_rfb/labextension/static/678.c748912b15ffb2656a49.js
+-rw-r--r--   0 almar      (501) staff       (20)     6480 2024-05-10 07:45:18.000000 jupyter_rfb-0.4.3/jupyter_rfb/labextension/static/remoteEntry.0d5a3b6ccc7e17c1ed27.js
+-rw-r--r--   0 almar      (501) staff       (20)      118 2024-05-10 07:45:18.000000 jupyter_rfb-0.4.3/jupyter_rfb/labextension/static/style.js
+-rw-r--r--   0 almar      (501) staff       (20)       20 2024-05-10 07:45:18.000000 jupyter_rfb-0.4.3/jupyter_rfb/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-05-10 07:45:19.083576 jupyter_rfb-0.4.3/jupyter_rfb/nbextension/
+-rw-r--r--   0 almar      (501) staff       (20)      531 2024-05-10 07:45:10.000000 jupyter_rfb-0.4.3/jupyter_rfb/nbextension/extension.js
+-rw-r--r--   0 almar      (501) staff       (20)     8563 2024-05-10 07:45:10.000000 jupyter_rfb-0.4.3/jupyter_rfb/nbextension/index.js
+-rw-r--r--   0 almar      (501) staff       (20)    17152 2024-05-10 07:32:58.000000 jupyter_rfb-0.4.3/jupyter_rfb/widget.py
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-05-10 07:45:19.082211 jupyter_rfb-0.4.3/jupyter_rfb.egg-info/
+-rw-r--r--   0 almar      (501) staff       (20)      824 2024-05-10 07:45:18.000000 jupyter_rfb-0.4.3/jupyter_rfb.egg-info/PKG-INFO
+-rw-r--r--   0 almar      (501) staff       (20)     1120 2024-05-10 07:45:19.000000 jupyter_rfb-0.4.3/jupyter_rfb.egg-info/SOURCES.txt
+-rw-r--r--   0 almar      (501) staff       (20)        1 2024-05-10 07:45:18.000000 jupyter_rfb-0.4.3/jupyter_rfb.egg-info/dependency_links.txt
+-rw-r--r--   0 almar      (501) staff       (20)        1 2022-02-04 09:25:53.000000 jupyter_rfb-0.4.3/jupyter_rfb.egg-info/not-zip-safe
+-rw-r--r--   0 almar      (501) staff       (20)       46 2024-05-10 07:45:18.000000 jupyter_rfb-0.4.3/jupyter_rfb.egg-info/requires.txt
+-rw-r--r--   0 almar      (501) staff       (20)       12 2024-05-10 07:45:18.000000 jupyter_rfb-0.4.3/jupyter_rfb.egg-info/top_level.txt
+-rw-r--r--   0 almar      (501) staff       (20)       65 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.3/jupyter_rfb.json
+-rw-r--r--   0 almar      (501) staff       (20)      153 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.3/pyproject.toml
+-rw-r--r--   0 almar      (501) staff       (20)      460 2024-05-10 07:45:19.085186 jupyter_rfb-0.4.3/setup.cfg
+-rw-r--r--   0 almar      (501) staff       (20)     2525 2023-04-30 21:11:03.000000 jupyter_rfb-0.4.3/setup.py
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-05-10 07:45:19.084570 jupyter_rfb-0.4.3/tests/
+-rw-r--r--   0 almar      (501) staff       (20)     3443 2023-02-17 06:37:49.000000 jupyter_rfb-0.4.3/tests/test_jpg.py
+-rw-r--r--   0 almar      (501) staff       (20)     2614 2022-02-04 09:25:28.000000 jupyter_rfb-0.4.3/tests/test_png.py
+-rw-r--r--   0 almar      (501) staff       (20)     3670 2023-02-17 06:37:49.000000 jupyter_rfb-0.4.3/tests/test_utils.py
+-rw-r--r--   0 almar      (501) staff       (20)     8346 2024-04-16 11:03:12.000000 jupyter_rfb-0.4.3/tests/test_widget.py
```

### Comparing `jupyter_rfb-0.4.2/LICENSE` & `jupyter_rfb-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.4.2/README.md` & `jupyter_rfb-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.4.2/js/amd-public-path.js` & `jupyter_rfb-0.4.3/js/amd-public-path.js`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.4.2/js/dist/index.js` & `jupyter_rfb-0.4.3/js/dist/index.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -5,15 +5,15 @@
                 var s = i(325);
                 const n = new URL(s.uri, document.location);
                 n.pathname = n.pathname.slice(0, n.pathname.lastIndexOf("/") + 1), i.p = `${n.origin}${n.pathname}`
             },
             681: (e, t, i) => {
                 i.r(t), i.d(t, {
                     RemoteFrameBufferModel: () => n,
-                    RemoteFrameBufferView: () => l,
+                    RemoteFrameBufferView: () => o,
                     version: () => _.i8
                 });
                 var s = i(146);
                 class n extends s.DOMWidgetModel {
                     defaults() {
                         return {
                             ...super.defaults(),
@@ -23,15 +23,16 @@
                             _view_module: "jupyter_rfb",
                             _model_module_version: "0.1.0",
                             _view_module_version: "0.1.0",
                             frame_feedback: {},
                             css_width: "500px",
                             css_height: "300px",
                             resizable: !0,
-                            has_visible_views: !1
+                            has_visible_views: !1,
+                            cursor: "default"
                         }
                     }
                     initialize() {
                         super.initialize.apply(this, arguments), this.img_elements = [], this._intersection_observer = new IntersectionObserver(this._intersection_callback.bind(this)), window.setInterval(this.collect_view_img_elements.bind(this), 5e3), this.frames = [], this.on("msg:custom", this.on_msg, this), this.last_frame = {
                             src: "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAIAAACQd1PeAAAADElEQVR42mOor68HAAL+AX6E2KOJAAAAAElFTkSuQmCC",
                             index: 0,
                             timestamp: 0
@@ -93,15 +94,15 @@
                     close() {
                         this.send({
                             event_type: "close",
                             time_stamp: a()
                         }), super.close.apply(this, arguments)
                     }
                 }
-                class l extends s.DOMWidgetView {
+                class o extends s.DOMWidgetView {
                     render() {
                         var e = this;
 
                         function t() {
                             let t = e._wheel_state.e,
                                 i = e.img.getBoundingClientRect(),
                                 s = {
@@ -117,23 +118,25 @@
                             e._wheel_state.dx = 0, e._wheel_state.dy = 0, e._wheel_state.pending = !1, e.send(s)
                         }
 
                         function i(t) {
                             if (null === e.el.offsetParent) return;
                             let i = {
                                 event_type: "key_" + t.type.slice(3),
-                                key: o[t.key] || t.key,
+                                key: l[t.key] || t.key,
                                 modifiers: r(t),
                                 time_stamp: a()
                             };
                             t.repeat || e.send(i), t.stopPropagation(), t.preventDefault()
                         }
                         this.focus_el = document.createElement("a"), this.focus_el.href = "#", this.focus_el.style.position = "absolute", this.focus_el.style.width = "1px", this.focus_el.style.height = "1px", this.focus_el.style.padding = "0", this.focus_el.style.zIndex = "-99", this.el.appendChild(this.focus_el), this.img = new Image, this.img.decoding = "sync", this.img.loading = "eager", this.img.style.touchAction = "none", this.img.ondragstart = () => !1, this.img.tabIndex = -1, this.img.oncontextmenu = function(e) {
                             if (!e.shiftKey) return e.preventDefault(), e.stopPropagation(), !1
-                        }, this.img.src = this.model.last_frame.src, this.el.appendChild(this.img), this.model.collect_view_img_elements(), this._throttlers = {}, this.img.style.width = "100%", this.img.style.height = "100%", this.el.style.width = this.model.get("css_width"), this.el.style.height = this.model.get("css_height"), this.el.style.resize = this.model.get("resizable") ? "both" : "none", this.model.on("change:css_width", (function() {
+                        }, this.img.src = this.model.last_frame.src, this.el.appendChild(this.img), this.model.collect_view_img_elements(), this.el.style.cursor = this.model.get("cursor"), this.model.on("change:cursor", (function() {
+                            this.el.style.cursor = this.model.get("cursor")
+                        }), this), this._throttlers = {}, this.img.style.width = "100%", this.img.style.height = "100%", this.el.style.width = this.model.get("css_width"), this.el.style.height = this.model.get("css_height"), this.el.style.resize = this.model.get("resizable") ? "both" : "none", this.model.on("change:css_width", (function() {
                             this.el.style.width = this.model.get("css_width")
                         }), this), this.model.on("change:css_height", (function() {
                             this.el.style.height = this.model.get("css_height")
                         }), this), this.model.on("change:resizable", (function() {
                             this.el.style.resize = this.model.get("resizable") ? "both" : "none"
                         }), this), this._current_size = [0, 0, 1], this._resizeObserver = new ResizeObserver(this._check_resize.bind(e)), this._resizeObserver.observe(this.img), window.addEventListener("resize", this._check_resize.bind(this)), this._pointers = {}, this._last_buttons = [], this.img.addEventListener("pointerdown", (function(t) {
                             e.focus_el.focus(), e.img.setPointerCapture(t.pointerId), e._pointers[t.pointerId] = t;
@@ -176,49 +179,49 @@
                             time_stamp: a()
                         }, 200))
                     }
                     send_throttled(e, t) {
                         let i = e.event_type || "",
                             s = this._throttlers[i];
                         void 0 === s && (s = function(e, t) {
-                            var i, s, n, l = null,
-                                o = 0,
+                            var i, s, n, o = null,
+                                l = 0,
                                 r = function() {
-                                    o = Date.now(), l = null, n = e.apply(i, s), l || (i = s = null)
+                                    l = Date.now(), o = null, n = e.apply(i, s), o || (i = s = null)
                                 };
                             return function() {
                                 var h = Date.now(),
-                                    a = t - (h - o);
-                                return i = this, s = arguments, a <= 0 || a > t ? (l && (clearTimeout(l), l = null), o = h, n = e.apply(i, s), l || (i = s = null)) : l || (l = setTimeout(r, a)), n
+                                    a = t - (h - l);
+                                return i = this, s = arguments, a <= 0 || a > t ? (o && (clearTimeout(o), o = null), l = h, n = e.apply(i, s), o || (i = s = null)) : o || (o = setTimeout(r, a)), n
                             }
                         }(this.send, t || 50), this._throttlers[i] = s), s.call(this, e)
                     }
                 }
-                var o = {
+                var l = {
                     Ctrl: "Control",
                     Del: "Delete",
                     Esc: "Escape"
                 };
 
                 function r(e) {
-                    return ["Alt", "Shift", "Ctrl", "Meta"].filter((t => e[t.toLowerCase() + "Key"])).map((e => o[e] || e))
+                    return ["Alt", "Shift", "Ctrl", "Meta"].filter((t => e[t.toLowerCase() + "Key"])).map((e => l[e] || e))
                 }
 
                 function h(e, t, i, s) {
                     let n = e.getBoundingClientRect(),
-                        l = [n.left, n.top],
-                        o = Number(t.clientX - l[0]),
-                        h = Number(t.clientY - l[1]),
+                        o = [n.left, n.top],
+                        l = Number(t.clientX - o[0]),
+                        h = Number(t.clientY - o[1]),
                         _ = {},
                         d = 0;
                     for (let e in i) {
                         let t = i[e],
                             s = {
-                                x: Number(t.clientX - l[0]),
-                                y: Number(t.clientY - l[1]),
+                                x: Number(t.clientX - o[0]),
+                                y: Number(t.clientY - o[1]),
                                 pressure: t.pressure
                             };
                         _[t.pointerId] = s, d += 1
                     }
                     var m = {
                             0: 1,
                             1: 3,
@@ -227,48 +230,48 @@
                             4: 5,
                             5: 6
                         } [t.button] || 0,
                         u = [];
                     for (let e of [0, 1, 2, 3, 4, 5]) 1 << e & t.buttons && u.push(e + 1);
                     return {
                         event_type: s,
-                        x: o,
+                        x: l,
                         y: h,
                         button: m,
                         buttons: u,
                         modifiers: r(t),
                         ntouches: d,
                         touches: _,
                         time_stamp: a()
                     }
                 }
 
                 function a() {
                     return Date.now() / 1e3
                 }
                 const _ = {
-                    i8: "0.1.0"
+                    i8: "0.4.3"
                 }
             },
             146: e => {
                 e.exports = t
             },
             325: t => {
                 t.exports = e
             }
         },
         s = {};
 
     function n(e) {
         var t = s[e];
         if (void 0 !== t) return t.exports;
-        var l = s[e] = {
+        var o = s[e] = {
             exports: {}
         };
-        return i[e](l, l.exports, n), l.exports
+        return i[e](o, o.exports, n), o.exports
     }
     return n.n = e => {
         var t = e && e.__esModule ? () => e.default : () => e;
         return n.d(t, {
             a: t
         }), t
     }, n.d = (e, t) => {
```

### Comparing `jupyter_rfb-0.4.2/js/lib/labplugin.js` & `jupyter_rfb-0.4.3/js/lib/labplugin.js`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.4.2/js/lib/widget.js` & `jupyter_rfb-0.4.3/js/lib/widget.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -34,15 +34,16 @@
             _view_module_version: '0.1.0',
             // For the frames
             frame_feedback: {},
             // For the widget
             css_width: '500px',
             css_height: '300px',
             resizable: true,
-            has_visible_views: false
+            has_visible_views: false,
+            cursor: 'default'
         };
     }
     initialize() {
         super.initialize.apply(this, arguments);
         // Keep a list if img elements.
         this.img_elements = [];
         // Observer that will check whether the img elements are within the viewport.
@@ -225,14 +226,20 @@
         };
 
         // Initialize the image
         this.img.src = this.model.last_frame.src;
         this.el.appendChild(this.img);
         this.model.collect_view_img_elements();
 
+        // Cursor
+        this.el.style.cursor = this.model.get('cursor');
+        this.model.on('change:cursor', function() {
+            this.el.style.cursor = this.model.get('cursor');
+        }, this);
+
         // Set of throttler functions to send events at a friendly pace
         this._throttlers = {};
 
         // Initialize sizing.
         // Setting the this.el's size right now has no effect. We also set it in _check_size() below.
         this.img.style.width = '100%';
         this.img.style.height = '100%';
```

### Comparing `jupyter_rfb-0.4.2/js/package.json` & `jupyter_rfb-0.4.3/js/package.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8701923076923077%*

 * *Differences: {"'devDependencies'": "{'@jupyterlab/builder': '^4.1.3', 'webpack-cli': '^5.1.4'}",*

 * * "'license'": "'MIT'",*

 * * "'version'": "'0.4.3'"}*

```diff
@@ -2,17 +2,18 @@
     "author": "Almar Klein",
     "dependencies": {
         "@jupyter-widgets/base": "^1.1 || ^2 || ^3 || ^4 || ^5 || ^6",
         "lodash": "^4.17.4"
     },
     "description": "Remote Frame Buffer for Jupyter",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.0.0",
+        "@jupyterlab/builder": "^4.1.3",
         "rimraf": "^2.6.1",
-        "webpack": "^5"
+        "webpack": "^5",
+        "webpack-cli": "^5.1.4"
     },
     "files": [
         "lib/**/*.js",
         "dist/*.js"
     ],
     "jupyterlab": {
         "extension": "lib/labplugin",
@@ -27,14 +28,15 @@
     "keywords": [
         "jupyter",
         "widgets",
         "ipython",
         "ipywidgets",
         "jupyterlab-extension"
     ],
+    "license": "MIT",
     "main": "lib/index.js",
     "name": "jupyter_rfb",
     "repository": {
         "type": "git",
         "url": "https://github.com/vispy/jupyter_rfb.git"
     },
     "scripts": {
@@ -43,9 +45,9 @@
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:prod": "webpack --mode=production && yarn run build:labextension",
         "clean": "rimraf dist/ && rimraf ../jupyter_rfb/labextension/ && rimraf ../jupyter_rfb/nbextension",
         "prepublish": "yarn run clean && yarn run build:prod",
         "test": "echo \"Error: no test specified\" && exit 1",
         "watch": "webpack --watch --mode=development"
     },
-    "version": "0.1.0"
+    "version": "0.4.3"
 }
```

### Comparing `jupyter_rfb-0.4.2/js/webpack.config.js` & `jupyter_rfb-0.4.3/js/webpack.config.js`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.4.2/jupyter_rfb/__init__.py` & `jupyter_rfb-0.4.3/jupyter_rfb/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.4.2/jupyter_rfb/_jpg.py` & `jupyter_rfb-0.4.3/jupyter_rfb/_jpg.py`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.4.2/jupyter_rfb/_png.py` & `jupyter_rfb-0.4.3/jupyter_rfb/_png.py`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.4.2/jupyter_rfb/_utils.py` & `jupyter_rfb-0.4.3/jupyter_rfb/_utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.4.2/jupyter_rfb/events.py` & `jupyter_rfb-0.4.3/jupyter_rfb/events.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 
 * **pointer_down**: emitted when the user interacts with mouse,
   touch or other pointer devices, by pressing it down.
 
     * *x*: horizontal position of the pointer within the widget.
     * *y*: vertical position of the pointer within the widget.
     * *button*: the button to which this event applies. See section below for details.
-    * *buttons*: a list of buttons being pressed down.
-    * *modifiers*: a list of modifier keys being pressed down. See section below for details.
+    * *buttons*: a tuple of buttons being pressed down.
+    * *modifiers*: a tuple of modifier keys being pressed down. See section below for details.
     * *ntouches*: the number of simultaneous pointers being down.
     * *touches*: a dict with int keys (pointer id's), and values that are dicts
       that contain "x", "y", and "pressure".
     * *time_stamp*: a timestamp in seconds.
 
 * **pointer_up**: emitted when the user releases a pointer.
   This event has the same keys as the pointer down event.
@@ -59,22 +59,22 @@
   scrolling. In applications where the scroll dimension does not matter,
   it is therefore recommended to use `delta = event['dy'] or event['dx']`.
 
     * *dx*: the horizontal scroll delta (positive means scroll right).
     * *dy*: the vertical scroll delta (positive means scroll down or zoom out).
     * *x*: the mouse horizontal position during the scroll.
     * *y*: the mouse vertical position during the scroll.
-    * *buttons*: a list of buttons being pressed down.
-    * *modifiers*: a list of modifier keys being pressed down.
+    * *buttons*: a tuple of buttons being pressed down.
+    * *modifiers*: a tuple of modifier keys being pressed down.
     * *time_stamp*: a timestamp in seconds.
 
 * **key_down**: emitted when a key is pressed down.
 
     * *key*: the key being pressed as a string. See section below for details.
-    * *modifiers*: a list of modifier keys being pressed down.
+    * *modifiers*: a tuple of modifier keys being pressed down.
     * *time_stamp*: a timestamp in seconds.
 
 * **key_up**: emitted when a key is released.
   This event has the same keys as the key down event.
 
 
 Time stamps
```

### Comparing `jupyter_rfb-0.4.2/jupyter_rfb/labextension/package.json` & `jupyter_rfb-0.4.3/jupyter_rfb/labextension/package.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8689903846153846%*

 * *Differences: {"'devDependencies'": "{'@jupyterlab/builder': '^4.1.3', 'webpack-cli': '^5.1.4'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.0d5a3b6ccc7e17c1ed27.js'}}",*

 * * "'license'": "'MIT'",*

 * * "'version'": "'0.4.3'"}*

```diff
@@ -2,26 +2,27 @@
     "author": "Almar Klein",
     "dependencies": {
         "@jupyter-widgets/base": "^1.1 || ^2 || ^3 || ^4 || ^5 || ^6",
         "lodash": "^4.17.4"
     },
     "description": "Remote Frame Buffer for Jupyter",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.0.0",
+        "@jupyterlab/builder": "^4.1.3",
         "rimraf": "^2.6.1",
-        "webpack": "^5"
+        "webpack": "^5",
+        "webpack-cli": "^5.1.4"
     },
     "files": [
         "lib/**/*.js",
         "dist/*.js"
     ],
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.f201b0f18d69b7610789.js"
+            "load": "static/remoteEntry.0d5a3b6ccc7e17c1ed27.js"
         },
         "extension": "lib/labplugin",
         "outputDir": "../jupyter_rfb/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -31,14 +32,15 @@
     "keywords": [
         "jupyter",
         "widgets",
         "ipython",
         "ipywidgets",
         "jupyterlab-extension"
     ],
+    "license": "MIT",
     "main": "lib/index.js",
     "name": "jupyter_rfb",
     "repository": {
         "type": "git",
         "url": "https://github.com/vispy/jupyter_rfb.git"
     },
     "scripts": {
@@ -47,9 +49,9 @@
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:prod": "webpack --mode=production && yarn run build:labextension",
         "clean": "rimraf dist/ && rimraf ../jupyter_rfb/labextension/ && rimraf ../jupyter_rfb/nbextension",
         "prepublish": "yarn run clean && yarn run build:prod",
         "test": "echo \"Error: no test specified\" && exit 1",
         "watch": "webpack --watch --mode=development"
     },
-    "version": "0.1.0"
+    "version": "0.4.3"
 }
```

### Comparing `jupyter_rfb-0.4.2/jupyter_rfb/labextension/static/261.9ef272ff509129a4e555.js` & `jupyter_rfb-0.4.3/jupyter_rfb/labextension/static/493.cb43b5d572b2f6b10c8e.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,32 +1,33 @@
 "use strict";
 (self.webpackChunkjupyter_rfb = self.webpackChunkjupyter_rfb || []).push([
-    [261, 920], {
-        920: (e, t, i) => {
+    [493], {
+        678: (e, t, i) => {
             i.r(t), i.d(t, {
                 RemoteFrameBufferModel: () => n,
-                RemoteFrameBufferView: () => l,
-                version: () => a.i8
+                RemoteFrameBufferView: () => r,
+                version: () => a.rE
             });
-            var s = i(382);
+            var s = i(4);
             class n extends s.DOMWidgetModel {
                 defaults() {
                     return {
                         ...super.defaults(),
                         _model_name: "RemoteFrameBufferModel",
                         _view_name: "RemoteFrameBufferView",
                         _model_module: "jupyter_rfb",
                         _view_module: "jupyter_rfb",
                         _model_module_version: "0.1.0",
                         _view_module_version: "0.1.0",
                         frame_feedback: {},
                         css_width: "500px",
                         css_height: "300px",
                         resizable: !0,
-                        has_visible_views: !1
+                        has_visible_views: !1,
+                        cursor: "default"
                     }
                 }
                 initialize() {
                     super.initialize.apply(this, arguments), this.img_elements = [], this._intersection_observer = new IntersectionObserver(this._intersection_callback.bind(this)), window.setInterval(this.collect_view_img_elements.bind(this), 5e3), this.frames = [], this.on("msg:custom", this.on_msg, this), this.last_frame = {
                         src: "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAIAAACQd1PeAAAADElEQVR42mOor68HAAL+AX6E2KOJAAAAAElFTkSuQmCC",
                         index: 0,
                         timestamp: 0
@@ -88,15 +89,15 @@
                 close() {
                     this.send({
                         event_type: "close",
                         time_stamp: _()
                     }), super.close.apply(this, arguments)
                 }
             }
-            class l extends s.DOMWidgetView {
+            class r extends s.DOMWidgetView {
                 render() {
                     var e = this;
 
                     function t() {
                         let t = e._wheel_state.e,
                             i = e.img.getBoundingClientRect(),
                             s = {
@@ -112,23 +113,25 @@
                         e._wheel_state.dx = 0, e._wheel_state.dy = 0, e._wheel_state.pending = !1, e.send(s)
                     }
 
                     function i(t) {
                         if (null === e.el.offsetParent) return;
                         let i = {
                             event_type: "key_" + t.type.slice(3),
-                            key: r[t.key] || t.key,
+                            key: l[t.key] || t.key,
                             modifiers: o(t),
                             time_stamp: _()
                         };
                         t.repeat || e.send(i), t.stopPropagation(), t.preventDefault()
                     }
                     this.focus_el = document.createElement("a"), this.focus_el.href = "#", this.focus_el.style.position = "absolute", this.focus_el.style.width = "1px", this.focus_el.style.height = "1px", this.focus_el.style.padding = "0", this.focus_el.style.zIndex = "-99", this.el.appendChild(this.focus_el), this.img = new Image, this.img.decoding = "sync", this.img.loading = "eager", this.img.style.touchAction = "none", this.img.ondragstart = () => !1, this.img.tabIndex = -1, this.img.oncontextmenu = function(e) {
                         if (!e.shiftKey) return e.preventDefault(), e.stopPropagation(), !1
-                    }, this.img.src = this.model.last_frame.src, this.el.appendChild(this.img), this.model.collect_view_img_elements(), this._throttlers = {}, this.img.style.width = "100%", this.img.style.height = "100%", this.el.style.width = this.model.get("css_width"), this.el.style.height = this.model.get("css_height"), this.el.style.resize = this.model.get("resizable") ? "both" : "none", this.model.on("change:css_width", (function() {
+                    }, this.img.src = this.model.last_frame.src, this.el.appendChild(this.img), this.model.collect_view_img_elements(), this.el.style.cursor = this.model.get("cursor"), this.model.on("change:cursor", (function() {
+                        this.el.style.cursor = this.model.get("cursor")
+                    }), this), this._throttlers = {}, this.img.style.width = "100%", this.img.style.height = "100%", this.el.style.width = this.model.get("css_width"), this.el.style.height = this.model.get("css_height"), this.el.style.resize = this.model.get("resizable") ? "both" : "none", this.model.on("change:css_width", (function() {
                         this.el.style.width = this.model.get("css_width")
                     }), this), this.model.on("change:css_height", (function() {
                         this.el.style.height = this.model.get("css_height")
                     }), this), this.model.on("change:resizable", (function() {
                         this.el.style.resize = this.model.get("resizable") ? "both" : "none"
                     }), this), this._current_size = [0, 0, 1], this._resizeObserver = new ResizeObserver(this._check_resize.bind(e)), this._resizeObserver.observe(this.img), window.addEventListener("resize", this._check_resize.bind(this)), this._pointers = {}, this._last_buttons = [], this.img.addEventListener("pointerdown", (function(t) {
                         e.focus_el.focus(), e.img.setPointerCapture(t.pointerId), e._pointers[t.pointerId] = t;
@@ -171,49 +174,49 @@
                         time_stamp: _()
                     }, 200))
                 }
                 send_throttled(e, t) {
                     let i = e.event_type || "",
                         s = this._throttlers[i];
                     void 0 === s && (s = function(e, t) {
-                        var i, s, n, l = null,
-                            r = 0,
+                        var i, s, n, r = null,
+                            l = 0,
                             o = function() {
-                                r = Date.now(), l = null, n = e.apply(i, s), l || (i = s = null)
+                                l = Date.now(), r = null, n = e.apply(i, s), r || (i = s = null)
                             };
                         return function() {
                             var h = Date.now(),
-                                _ = t - (h - r);
-                            return i = this, s = arguments, _ <= 0 || _ > t ? (l && (clearTimeout(l), l = null), r = h, n = e.apply(i, s), l || (i = s = null)) : l || (l = setTimeout(o, _)), n
+                                _ = t - (h - l);
+                            return i = this, s = arguments, _ <= 0 || _ > t ? (r && (clearTimeout(r), r = null), l = h, n = e.apply(i, s), r || (i = s = null)) : r || (r = setTimeout(o, _)), n
                         }
                     }(this.send, t || 50), this._throttlers[i] = s), s.call(this, e)
                 }
             }
-            var r = {
+            var l = {
                 Ctrl: "Control",
                 Del: "Delete",
                 Esc: "Escape"
             };
 
             function o(e) {
-                return ["Alt", "Shift", "Ctrl", "Meta"].filter((t => e[t.toLowerCase() + "Key"])).map((e => r[e] || e))
+                return ["Alt", "Shift", "Ctrl", "Meta"].filter((t => e[t.toLowerCase() + "Key"])).map((e => l[e] || e))
             }
 
             function h(e, t, i, s) {
                 let n = e.getBoundingClientRect(),
-                    l = [n.left, n.top],
-                    r = Number(t.clientX - l[0]),
-                    h = Number(t.clientY - l[1]),
+                    r = [n.left, n.top],
+                    l = Number(t.clientX - r[0]),
+                    h = Number(t.clientY - r[1]),
                     a = {},
                     d = 0;
                 for (let e in i) {
                     let t = i[e],
                         s = {
-                            x: Number(t.clientX - l[0]),
-                            y: Number(t.clientY - l[1]),
+                            x: Number(t.clientX - r[0]),
+                            y: Number(t.clientY - r[1]),
                             pressure: t.pressure
                         };
                     a[t.pointerId] = s, d += 1
                 }
                 var m = {
                         0: 1,
                         1: 3,
@@ -222,50 +225,50 @@
                         4: 5,
                         5: 6
                     } [t.button] || 0,
                     u = [];
                 for (let e of [0, 1, 2, 3, 4, 5]) 1 << e & t.buttons && u.push(e + 1);
                 return {
                     event_type: s,
-                    x: r,
+                    x: l,
                     y: h,
                     button: m,
                     buttons: u,
                     modifiers: o(t),
                     ntouches: d,
                     touches: a,
                     time_stamp: _()
                 }
             }
 
             function _() {
                 return Date.now() / 1e3
             }
             const a = {
-                i8: "0.1.0"
+                rE: "0.4.3"
             }
         },
-        261: (e, t, i) => {
+        493: (e, t, i) => {
             i.r(t), i.d(t, {
-                remoteFrameBufferPlugin: () => n,
-                default: () => l
+                default: () => r,
+                remoteFrameBufferPlugin: () => n
             });
-            var s = i(920);
+            var s = i(678);
             const n = {
                     id: "jupyter_rfb:plugin",
-                    requires: [i(382).IJupyterWidgetRegistry],
+                    requires: [i(4).IJupyterWidgetRegistry],
                     activate: function(e, t) {
                         t.registerWidget({
                             name: "jupyter_rfb",
                             version: s.version,
                             exports: {
                                 RemoteFrameBufferModel: s.RemoteFrameBufferModel,
                                 RemoteFrameBufferView: s.RemoteFrameBufferView
                             }
                         })
                     },
                     autoStart: !0
                 },
-                l = n
+                r = n
         }
     }
 ]);
```

### Comparing `jupyter_rfb-0.4.2/jupyter_rfb/labextension/static/920.68e3589cd1cc5ef32304.js` & `jupyter_rfb-0.4.3/jupyter_rfb/labextension/static/678.c748912b15ffb2656a49.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,32 +1,33 @@
 "use strict";
 (self.webpackChunkjupyter_rfb = self.webpackChunkjupyter_rfb || []).push([
-    [920], {
-        920: (e, t, i) => {
+    [678, 4], {
+        678: (e, t, i) => {
             i.r(t), i.d(t, {
                 RemoteFrameBufferModel: () => n,
                 RemoteFrameBufferView: () => l,
-                version: () => a.i8
+                version: () => a.rE
             });
-            var s = i(382);
+            var s = i(4);
             class n extends s.DOMWidgetModel {
                 defaults() {
                     return {
                         ...super.defaults(),
                         _model_name: "RemoteFrameBufferModel",
                         _view_name: "RemoteFrameBufferView",
                         _model_module: "jupyter_rfb",
                         _view_module: "jupyter_rfb",
                         _model_module_version: "0.1.0",
                         _view_module_version: "0.1.0",
                         frame_feedback: {},
                         css_width: "500px",
                         css_height: "300px",
                         resizable: !0,
-                        has_visible_views: !1
+                        has_visible_views: !1,
+                        cursor: "default"
                     }
                 }
                 initialize() {
                     super.initialize.apply(this, arguments), this.img_elements = [], this._intersection_observer = new IntersectionObserver(this._intersection_callback.bind(this)), window.setInterval(this.collect_view_img_elements.bind(this), 5e3), this.frames = [], this.on("msg:custom", this.on_msg, this), this.last_frame = {
                         src: "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAIAAACQd1PeAAAADElEQVR42mOor68HAAL+AX6E2KOJAAAAAElFTkSuQmCC",
                         index: 0,
                         timestamp: 0
@@ -102,51 +103,53 @@
                             s = {
                                 event_type: "wheel",
                                 x: Number(t.clientX - i.left),
                                 y: Number(t.clientY - i.top),
                                 dx: e._wheel_state.dx,
                                 dy: e._wheel_state.dy,
                                 buttons: e._last_buttons,
-                                modifiers: h(t),
+                                modifiers: r(t),
                                 time_stamp: _()
                             };
                         e._wheel_state.dx = 0, e._wheel_state.dy = 0, e._wheel_state.pending = !1, e.send(s)
                     }
 
                     function i(t) {
                         if (null === e.el.offsetParent) return;
                         let i = {
                             event_type: "key_" + t.type.slice(3),
                             key: o[t.key] || t.key,
-                            modifiers: h(t),
+                            modifiers: r(t),
                             time_stamp: _()
                         };
                         t.repeat || e.send(i), t.stopPropagation(), t.preventDefault()
                     }
                     this.focus_el = document.createElement("a"), this.focus_el.href = "#", this.focus_el.style.position = "absolute", this.focus_el.style.width = "1px", this.focus_el.style.height = "1px", this.focus_el.style.padding = "0", this.focus_el.style.zIndex = "-99", this.el.appendChild(this.focus_el), this.img = new Image, this.img.decoding = "sync", this.img.loading = "eager", this.img.style.touchAction = "none", this.img.ondragstart = () => !1, this.img.tabIndex = -1, this.img.oncontextmenu = function(e) {
                         if (!e.shiftKey) return e.preventDefault(), e.stopPropagation(), !1
-                    }, this.img.src = this.model.last_frame.src, this.el.appendChild(this.img), this.model.collect_view_img_elements(), this._throttlers = {}, this.img.style.width = "100%", this.img.style.height = "100%", this.el.style.width = this.model.get("css_width"), this.el.style.height = this.model.get("css_height"), this.el.style.resize = this.model.get("resizable") ? "both" : "none", this.model.on("change:css_width", (function() {
+                    }, this.img.src = this.model.last_frame.src, this.el.appendChild(this.img), this.model.collect_view_img_elements(), this.el.style.cursor = this.model.get("cursor"), this.model.on("change:cursor", (function() {
+                        this.el.style.cursor = this.model.get("cursor")
+                    }), this), this._throttlers = {}, this.img.style.width = "100%", this.img.style.height = "100%", this.el.style.width = this.model.get("css_width"), this.el.style.height = this.model.get("css_height"), this.el.style.resize = this.model.get("resizable") ? "both" : "none", this.model.on("change:css_width", (function() {
                         this.el.style.width = this.model.get("css_width")
                     }), this), this.model.on("change:css_height", (function() {
                         this.el.style.height = this.model.get("css_height")
                     }), this), this.model.on("change:resizable", (function() {
                         this.el.style.resize = this.model.get("resizable") ? "both" : "none"
                     }), this), this._current_size = [0, 0, 1], this._resizeObserver = new ResizeObserver(this._check_resize.bind(e)), this._resizeObserver.observe(this.img), window.addEventListener("resize", this._check_resize.bind(this)), this._pointers = {}, this._last_buttons = [], this.img.addEventListener("pointerdown", (function(t) {
                         e.focus_el.focus(), e.img.setPointerCapture(t.pointerId), e._pointers[t.pointerId] = t;
-                        let i = r(e.img, t, e._pointers, "pointer_down");
+                        let i = h(e.img, t, e._pointers, "pointer_down");
                         e._last_buttons = i.buttons, e.send(i), t.altKey || t.preventDefault()
                     })), this.img.addEventListener("lostpointercapture", (function(t) {
-                        let i = r(e.img, t, e._pointers, "pointer_up");
+                        let i = h(e.img, t, e._pointers, "pointer_up");
                         delete e._pointers[t.pointerId], e._last_buttons = i.buttons, e.send(i)
                     })), this.img.addEventListener("pointermove", (function(t) {
                         if (void 0 === e._pointers[t.pointerId] && Object.keys(e._pointers).length > 0) return;
-                        let i = r(e.img, t, e._pointers, "pointer_move");
+                        let i = h(e.img, t, e._pointers, "pointer_move");
                         e.send_throttled(i, 20)
                     })), this.img.addEventListener("dblclick", (function(t) {
-                        let i = r(e.img, t, {}, "double_click");
+                        let i = h(e.img, t, {}, "double_click");
                         delete i.touches, delete i.ntouches, e.send(i), t.altKey || t.preventDefault()
                     })), this._wheel_state = {
                         dx: 0,
                         dy: 0,
                         e: null,
                         pending: !1
                     }, this.img.addEventListener("wheel", (function(i) {
@@ -173,40 +176,40 @@
                 }
                 send_throttled(e, t) {
                     let i = e.event_type || "",
                         s = this._throttlers[i];
                     void 0 === s && (s = function(e, t) {
                         var i, s, n, l = null,
                             o = 0,
-                            h = function() {
+                            r = function() {
                                 o = Date.now(), l = null, n = e.apply(i, s), l || (i = s = null)
                             };
                         return function() {
-                            var r = Date.now(),
-                                _ = t - (r - o);
-                            return i = this, s = arguments, _ <= 0 || _ > t ? (l && (clearTimeout(l), l = null), o = r, n = e.apply(i, s), l || (i = s = null)) : l || (l = setTimeout(h, _)), n
+                            var h = Date.now(),
+                                _ = t - (h - o);
+                            return i = this, s = arguments, _ <= 0 || _ > t ? (l && (clearTimeout(l), l = null), o = h, n = e.apply(i, s), l || (i = s = null)) : l || (l = setTimeout(r, _)), n
                         }
                     }(this.send, t || 50), this._throttlers[i] = s), s.call(this, e)
                 }
             }
             var o = {
                 Ctrl: "Control",
                 Del: "Delete",
                 Esc: "Escape"
             };
 
-            function h(e) {
+            function r(e) {
                 return ["Alt", "Shift", "Ctrl", "Meta"].filter((t => e[t.toLowerCase() + "Key"])).map((e => o[e] || e))
             }
 
-            function r(e, t, i, s) {
+            function h(e, t, i, s) {
                 let n = e.getBoundingClientRect(),
                     l = [n.left, n.top],
                     o = Number(t.clientX - l[0]),
-                    r = Number(t.clientY - l[1]),
+                    h = Number(t.clientY - l[1]),
                     a = {},
                     d = 0;
                 for (let e in i) {
                     let t = i[e],
                         s = {
                             x: Number(t.clientX - l[0]),
                             y: Number(t.clientY - l[1]),
@@ -223,26 +226,26 @@
                         5: 6
                     } [t.button] || 0,
                     u = [];
                 for (let e of [0, 1, 2, 3, 4, 5]) 1 << e & t.buttons && u.push(e + 1);
                 return {
                     event_type: s,
                     x: o,
-                    y: r,
+                    y: h,
                     button: m,
                     buttons: u,
-                    modifiers: h(t),
+                    modifiers: r(t),
                     ntouches: d,
                     touches: a,
                     time_stamp: _()
                 }
             }
 
             function _() {
                 return Date.now() / 1e3
             }
             const a = {
-                i8: "0.1.0"
+                rE: "0.4.3"
             }
         }
     }
 ]);
```

### Comparing `jupyter_rfb-0.4.2/jupyter_rfb/labextension/static/remoteEntry.f201b0f18d69b7610789.js` & `jupyter_rfb-0.4.3/jupyter_rfb/labextension/static/remoteEntry.0d5a3b6ccc7e17c1ed27.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, f, s, d, p, c, h, v = {
-            176: (e, r, t) => {
+    var e, r, t, n, o, a, i, u, f, l, s, d, p, c, h, v, b, g = {
+            784: (e, r, t) => {
                 var n = {
-                        "./index": () => Promise.all([t.e(382), t.e(920)]).then((() => () => t(920))),
-                        "./extension": () => Promise.all([t.e(382), t.e(261)]).then((() => () => t(261)))
+                        "./index": () => t.e(678).then((() => () => t(678))),
+                        "./extension": () => Promise.all([t.e(4), t.e(493)]).then((() => () => t(493)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     a = (e, r) => {
                         if (t.S) {
                             var n = "default",
@@ -20,113 +20,114 @@
                     };
                 t.d(r, {
                     get: () => o,
                     init: () => a
                 })
             }
         },
-        b = {};
+        m = {};
 
-    function g(e) {
-        var r = b[e];
+    function y(e) {
+        var r = m[e];
         if (void 0 !== r) return r.exports;
-        var t = b[e] = {
+        var t = m[e] = {
             exports: {}
         };
-        return v[e](t, t.exports, g), t.exports
+        return g[e](t, t.exports, y), t.exports
     }
-    g.m = v, g.c = b, g.n = e => {
+    y.m = g, y.c = m, y.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
-        return g.d(r, {
+        return y.d(r, {
             a: r
         }), r
-    }, g.d = (e, r) => {
-        for (var t in r) g.o(r, t) && !g.o(e, t) && Object.defineProperty(e, t, {
+    }, y.d = (e, r) => {
+        for (var t in r) y.o(r, t) && !y.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, g.f = {}, g.e = e => Promise.all(Object.keys(g.f).reduce(((r, t) => (g.f[t](e, r), r)), [])), g.u = e => e + "." + {
-        261: "9ef272ff509129a4e555",
-        382: "1f3c426f14b6845534ba",
-        920: "68e3589cd1cc5ef32304"
+    }, y.f = {}, y.e = e => Promise.all(Object.keys(y.f).reduce(((r, t) => (y.f[t](e, r), r)), [])), y.u = e => e + "." + {
+        4: "8c0b9e46657bfc157d84",
+        493: "cb43b5d572b2f6b10c8e",
+        678: "c748912b15ffb2656a49"
     } [e] + ".js?v=" + {
-        261: "9ef272ff509129a4e555",
-        382: "1f3c426f14b6845534ba",
-        920: "68e3589cd1cc5ef32304"
-    } [e], g.g = function() {
+        4: "8c0b9e46657bfc157d84",
+        493: "cb43b5d572b2f6b10c8e",
+        678: "c748912b15ffb2656a49"
+    } [e], y.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), g.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "jupyter_rfb:", g.l = (t, n, o, a) => {
+    }(), y.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "jupyter_rfb:", y.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== o)
-                for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
-                    var s = l[f];
+                for (var f = document.getElementsByTagName("script"), l = 0; l < f.length; l++) {
+                    var s = f[l];
                     if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
                         i = s;
                         break
                     }
                 }
-            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, g.nc && i.setAttribute("nonce", g.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
+            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, y.nc && i.setAttribute("nonce", y.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
             var d = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(p);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
                 p = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
             i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
         }
-    }, g.r = e => {
+    }, y.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
-        g.S = {};
+        y.S = {};
         var e = {},
             r = {};
-        g.I = (t, n) => {
+        y.I = (t, n) => {
             n || (n = []);
             var o = r[t];
             if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
                 if (n.push(o), e[t]) return e[t];
-                g.o(g.S, t) || (g.S[t] = {});
-                var a = g.S[t],
+                y.o(y.S, t) || (y.S[t] = {});
+                var a = y.S[t],
                     i = "jupyter_rfb",
                     u = [];
                 return "default" === t && ((e, r, t, n) => {
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
-                        get: () => Promise.all([g.e(382), g.e(920)]).then((() => () => g(920))),
+                        get: () => y.e(678).then((() => () => y(678))),
                         from: i,
                         eager: !1
                     })
-                })("jupyter_rfb", "0.1.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("jupyter_rfb", "0.4.3"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        g.g.importScripts && (e = g.g.location + "");
-        var r = g.g.document;
+        y.g.importScripts && (e = y.g.location + "");
+        var r = y.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
-            t.length && (e = t[t.length - 1].src)
+            if (t.length)
+                for (var n = t.length - 1; n > -1 && (!e || !/^http(s?):/.test(e));) e = t[n--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), g.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), y.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
@@ -149,129 +150,135 @@
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
             for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(u = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
             return t
         }
         var i = [];
         for (a = 1; a < e.length; a++) {
             var u = e[a];
-            i.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? i.pop() + " " + i.pop() : o(u))
+            i.push(0 === u ? "not(" + f() + ")" : 1 === u ? "(" + f() + " || " + f() + ")" : 2 === u ? i.pop() + " " + i.pop() : o(u))
         }
-        return l();
+        return f();
 
-        function l() {
+        function f() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
-            for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var f, s, d = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !l || ("u" == d ? u > n && !o : "" == d != o);
+            for (var i = 0, u = 1, f = !0;; u++, i++) {
+                var l, s, d = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(l = r[i]))[0])) return !f || ("u" == d ? u > n && !o : "" == d != o);
                 if ("u" == s) {
-                    if (!l || "u" != d) return !1
-                } else if (l)
+                    if (!f || "u" != d) return !1
+                } else if (f)
                     if (d == s)
                         if (u <= n) {
-                            if (f != e[u]) return !1
+                            if (l != e[u]) return !1
                         } else {
-                            if (o ? f > e[u] : f < e[u]) return !1;
-                            f != e[u] && (l = !1)
+                            if (o ? l > e[u] : l < e[u]) return !1;
+                            l != e[u] && (f = !1)
                         }
                 else if ("s" != d && "n" != d) {
                     if (o || u <= n) return !1;
-                    l = !1, u--
+                    f = !1, u--
                 } else {
                     if (u <= n || s < d != o) return !1;
-                    l = !1
-                } else "s" != d && "n" != d && (l = !1, u--)
+                    f = !1
+                } else "s" != d && "n" != d && (f = !1, u--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
         }
         return !!c()
     }, i = (e, r) => {
-        var t = g.S[e];
-        if (!t || !g.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        var t = y.S[e];
+        if (!t || !y.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
+    }, f = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", l = (e, r, t, n) => {
         var o = u(e, t);
-        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(l(e, t, o, n)), s(e[t][o])
-    }, s = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, o) {
-        var a = g.I(r);
-        return a && a.then ? a.then(e.bind(e, r, g.S[r], t, n, o)) : e(r, g.S[r], t, n)
-    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), p = {}, c = {
-        382: () => d("default", "@jupyter-widgets/base", [, [1, 6],
+        return a(n, o) || s(f(e, t, o, n)), d(e[t][o])
+    }, s = e => {
+        "undefined" != typeof console && console.warn && console.warn(e)
+    }, d = e => (e.loaded = 1, e.get()), p = (e => function(r, t, n, o) {
+        var a = y.I(r);
+        return a && a.then ? a.then(e.bind(e, r, y.S[r], t, n, o)) : e(r, y.S[r], t, n)
+    })(((e, r, t, n) => (i(e, t), l(r, 0, t, n)))), c = {}, h = {
+        4: () => p("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 5],
             [1, 4],
             [1, 3],
             [1, 2],
             [1, 1, 1], 1, 1, 1, 1, 1
         ])
-    }, h = {
-        382: [382]
-    }, g.f.consumes = (e, r) => {
-        g.o(h, e) && h[e].forEach((e => {
-            if (g.o(p, e)) return r.push(p[e]);
-            var t = r => {
-                    p[e] = 0, g.m[e] = t => {
-                        delete g.c[e], t.exports = r()
+    }, v = {
+        4: [4],
+        678: [4]
+    }, b = {}, y.f.consumes = (e, r) => {
+        y.o(v, e) && v[e].forEach((e => {
+            if (y.o(c, e)) return r.push(c[e]);
+            if (!b[e]) {
+                var t = r => {
+                    c[e] = 0, y.m[e] = t => {
+                        delete y.c[e], t.exports = r()
                     }
-                },
-                n = r => {
-                    delete p[e], g.m[e] = t => {
-                        throw delete g.c[e], r
+                };
+                b[e] = !0;
+                var n = r => {
+                    delete c[e], y.m[e] = t => {
+                        throw delete y.c[e], r
                     }
                 };
-            try {
-                var o = c[e]();
-                o.then ? r.push(p[e] = o.then(t).catch(n)) : t(o)
-            } catch (e) {
-                n(e)
+                try {
+                    var o = h[e]();
+                    o.then ? r.push(c[e] = o.then(t).catch(n)) : t(o)
+                } catch (e) {
+                    n(e)
+                }
             }
         }))
     }, (() => {
         var e = {
-            909: 0
+            533: 0
         };
-        g.f.j = (r, t) => {
-            var n = g.o(e, r) ? e[r] : void 0;
+        y.f.j = (r, t) => {
+            var n = y.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
-                else if (382 != r) {
+                else if (4 != r) {
                 var o = new Promise(((t, o) => n = e[r] = [t, o]));
                 t.push(n[2] = o);
-                var a = g.p + g.u(r),
+                var a = y.p + y.u(r),
                     i = new Error;
-                g.l(a, (t => {
-                    if (g.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
+                y.l(a, (t => {
+                    if (y.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
                         var o = t && ("load" === t.type ? "missing" : t.type),
                             a = t && t.target && t.target.src;
                         i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
                     }
                 }), "chunk-" + r, r)
             } else e[r] = 0
         };
         var r = (r, t) => {
                 var n, o, [a, i, u] = t,
-                    l = 0;
+                    f = 0;
                 if (a.some((r => 0 !== e[r]))) {
-                    for (n in i) g.o(i, n) && (g.m[n] = i[n]);
-                    u && u(g)
+                    for (n in i) y.o(i, n) && (y.m[n] = i[n]);
+                    u && u(y)
                 }
-                for (r && r(t); l < a.length; l++) o = a[l], g.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); f < a.length; f++) o = a[f], y.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkjupyter_rfb = self.webpackChunkjupyter_rfb || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
-    var m = g(176);
-    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).jupyter_rfb = m
+    var w = y(784);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).jupyter_rfb = w
 })();
```

### Comparing `jupyter_rfb-0.4.2/jupyter_rfb/nbextension/extension.js` & `jupyter_rfb-0.4.3/jupyter_rfb/nbextension/extension.js`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.4.2/jupyter_rfb/nbextension/index.js` & `jupyter_rfb-0.4.3/jupyter_rfb/nbextension/index.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -5,15 +5,15 @@
                 var s = i(325);
                 const n = new URL(s.uri, document.location);
                 n.pathname = n.pathname.slice(0, n.pathname.lastIndexOf("/") + 1), i.p = `${n.origin}${n.pathname}`
             },
             681: (e, t, i) => {
                 i.r(t), i.d(t, {
                     RemoteFrameBufferModel: () => n,
-                    RemoteFrameBufferView: () => l,
+                    RemoteFrameBufferView: () => o,
                     version: () => _.i8
                 });
                 var s = i(146);
                 class n extends s.DOMWidgetModel {
                     defaults() {
                         return {
                             ...super.defaults(),
@@ -23,15 +23,16 @@
                             _view_module: "jupyter_rfb",
                             _model_module_version: "0.1.0",
                             _view_module_version: "0.1.0",
                             frame_feedback: {},
                             css_width: "500px",
                             css_height: "300px",
                             resizable: !0,
-                            has_visible_views: !1
+                            has_visible_views: !1,
+                            cursor: "default"
                         }
                     }
                     initialize() {
                         super.initialize.apply(this, arguments), this.img_elements = [], this._intersection_observer = new IntersectionObserver(this._intersection_callback.bind(this)), window.setInterval(this.collect_view_img_elements.bind(this), 5e3), this.frames = [], this.on("msg:custom", this.on_msg, this), this.last_frame = {
                             src: "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAIAAACQd1PeAAAADElEQVR42mOor68HAAL+AX6E2KOJAAAAAElFTkSuQmCC",
                             index: 0,
                             timestamp: 0
@@ -93,15 +94,15 @@
                     close() {
                         this.send({
                             event_type: "close",
                             time_stamp: a()
                         }), super.close.apply(this, arguments)
                     }
                 }
-                class l extends s.DOMWidgetView {
+                class o extends s.DOMWidgetView {
                     render() {
                         var e = this;
 
                         function t() {
                             let t = e._wheel_state.e,
                                 i = e.img.getBoundingClientRect(),
                                 s = {
@@ -117,23 +118,25 @@
                             e._wheel_state.dx = 0, e._wheel_state.dy = 0, e._wheel_state.pending = !1, e.send(s)
                         }
 
                         function i(t) {
                             if (null === e.el.offsetParent) return;
                             let i = {
                                 event_type: "key_" + t.type.slice(3),
-                                key: o[t.key] || t.key,
+                                key: l[t.key] || t.key,
                                 modifiers: r(t),
                                 time_stamp: a()
                             };
                             t.repeat || e.send(i), t.stopPropagation(), t.preventDefault()
                         }
                         this.focus_el = document.createElement("a"), this.focus_el.href = "#", this.focus_el.style.position = "absolute", this.focus_el.style.width = "1px", this.focus_el.style.height = "1px", this.focus_el.style.padding = "0", this.focus_el.style.zIndex = "-99", this.el.appendChild(this.focus_el), this.img = new Image, this.img.decoding = "sync", this.img.loading = "eager", this.img.style.touchAction = "none", this.img.ondragstart = () => !1, this.img.tabIndex = -1, this.img.oncontextmenu = function(e) {
                             if (!e.shiftKey) return e.preventDefault(), e.stopPropagation(), !1
-                        }, this.img.src = this.model.last_frame.src, this.el.appendChild(this.img), this.model.collect_view_img_elements(), this._throttlers = {}, this.img.style.width = "100%", this.img.style.height = "100%", this.el.style.width = this.model.get("css_width"), this.el.style.height = this.model.get("css_height"), this.el.style.resize = this.model.get("resizable") ? "both" : "none", this.model.on("change:css_width", (function() {
+                        }, this.img.src = this.model.last_frame.src, this.el.appendChild(this.img), this.model.collect_view_img_elements(), this.el.style.cursor = this.model.get("cursor"), this.model.on("change:cursor", (function() {
+                            this.el.style.cursor = this.model.get("cursor")
+                        }), this), this._throttlers = {}, this.img.style.width = "100%", this.img.style.height = "100%", this.el.style.width = this.model.get("css_width"), this.el.style.height = this.model.get("css_height"), this.el.style.resize = this.model.get("resizable") ? "both" : "none", this.model.on("change:css_width", (function() {
                             this.el.style.width = this.model.get("css_width")
                         }), this), this.model.on("change:css_height", (function() {
                             this.el.style.height = this.model.get("css_height")
                         }), this), this.model.on("change:resizable", (function() {
                             this.el.style.resize = this.model.get("resizable") ? "both" : "none"
                         }), this), this._current_size = [0, 0, 1], this._resizeObserver = new ResizeObserver(this._check_resize.bind(e)), this._resizeObserver.observe(this.img), window.addEventListener("resize", this._check_resize.bind(this)), this._pointers = {}, this._last_buttons = [], this.img.addEventListener("pointerdown", (function(t) {
                             e.focus_el.focus(), e.img.setPointerCapture(t.pointerId), e._pointers[t.pointerId] = t;
@@ -176,49 +179,49 @@
                             time_stamp: a()
                         }, 200))
                     }
                     send_throttled(e, t) {
                         let i = e.event_type || "",
                             s = this._throttlers[i];
                         void 0 === s && (s = function(e, t) {
-                            var i, s, n, l = null,
-                                o = 0,
+                            var i, s, n, o = null,
+                                l = 0,
                                 r = function() {
-                                    o = Date.now(), l = null, n = e.apply(i, s), l || (i = s = null)
+                                    l = Date.now(), o = null, n = e.apply(i, s), o || (i = s = null)
                                 };
                             return function() {
                                 var h = Date.now(),
-                                    a = t - (h - o);
-                                return i = this, s = arguments, a <= 0 || a > t ? (l && (clearTimeout(l), l = null), o = h, n = e.apply(i, s), l || (i = s = null)) : l || (l = setTimeout(r, a)), n
+                                    a = t - (h - l);
+                                return i = this, s = arguments, a <= 0 || a > t ? (o && (clearTimeout(o), o = null), l = h, n = e.apply(i, s), o || (i = s = null)) : o || (o = setTimeout(r, a)), n
                             }
                         }(this.send, t || 50), this._throttlers[i] = s), s.call(this, e)
                     }
                 }
-                var o = {
+                var l = {
                     Ctrl: "Control",
                     Del: "Delete",
                     Esc: "Escape"
                 };
 
                 function r(e) {
-                    return ["Alt", "Shift", "Ctrl", "Meta"].filter((t => e[t.toLowerCase() + "Key"])).map((e => o[e] || e))
+                    return ["Alt", "Shift", "Ctrl", "Meta"].filter((t => e[t.toLowerCase() + "Key"])).map((e => l[e] || e))
                 }
 
                 function h(e, t, i, s) {
                     let n = e.getBoundingClientRect(),
-                        l = [n.left, n.top],
-                        o = Number(t.clientX - l[0]),
-                        h = Number(t.clientY - l[1]),
+                        o = [n.left, n.top],
+                        l = Number(t.clientX - o[0]),
+                        h = Number(t.clientY - o[1]),
                         _ = {},
                         d = 0;
                     for (let e in i) {
                         let t = i[e],
                             s = {
-                                x: Number(t.clientX - l[0]),
-                                y: Number(t.clientY - l[1]),
+                                x: Number(t.clientX - o[0]),
+                                y: Number(t.clientY - o[1]),
                                 pressure: t.pressure
                             };
                         _[t.pointerId] = s, d += 1
                     }
                     var m = {
                             0: 1,
                             1: 3,
@@ -227,48 +230,48 @@
                             4: 5,
                             5: 6
                         } [t.button] || 0,
                         u = [];
                     for (let e of [0, 1, 2, 3, 4, 5]) 1 << e & t.buttons && u.push(e + 1);
                     return {
                         event_type: s,
-                        x: o,
+                        x: l,
                         y: h,
                         button: m,
                         buttons: u,
                         modifiers: r(t),
                         ntouches: d,
                         touches: _,
                         time_stamp: a()
                     }
                 }
 
                 function a() {
                     return Date.now() / 1e3
                 }
                 const _ = {
-                    i8: "0.1.0"
+                    i8: "0.4.3"
                 }
             },
             146: e => {
                 e.exports = t
             },
             325: t => {
                 t.exports = e
             }
         },
         s = {};
 
     function n(e) {
         var t = s[e];
         if (void 0 !== t) return t.exports;
-        var l = s[e] = {
+        var o = s[e] = {
             exports: {}
         };
-        return i[e](l, l.exports, n), l.exports
+        return i[e](o, o.exports, n), o.exports
     }
     return n.n = e => {
         var t = e && e.__esModule ? () => e.default : () => e;
         return n.d(t, {
             a: t
         }), t
     }, n.d = (e, t) => {
```

### Comparing `jupyter_rfb-0.4.2/jupyter_rfb/widget.py` & `jupyter_rfb-0.4.3/jupyter_rfb/widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,16 @@
       as a number between 1 and 100. Default 80. Set to lower numbers for more
       performance on slow connections. Note that each interaction is ended with a
       lossless image (PNG). If set to 100 or if JPEG encoding isn't possible (missing
       pillow or simplejpeg dependencies), then lossless PNGs will always be sent.
     * *max_buffered_frames*: the number of frames that is allowed to be "in-flight",
       i.e. sent, but not yet confirmed by the client. Default 2. Higher values
       may result in a higher FPS at the cost of introducing lag.
+    * *cursor*: the cursor style, ex: "crosshair", "grab". Valid cursors:
+      https://developer.mozilla.org/en-US/docs/Web/CSS/cursor#keyword
 
     """
 
     # Name of the widget view class in front-end
     _view_name = Unicode("RemoteFrameBufferView").tag(sync=True)
 
     # Name of the widget model class in front-end
@@ -71,14 +73,15 @@
     frame_feedback = Dict({}).tag(sync=True)
     has_visible_views = Bool(False).tag(sync=True)
     max_buffered_frames = Int(2, min=1)
     quality = Int(80, min=1, max=100)
     css_width = Unicode("500px").tag(sync=True)
     css_height = Unicode("300px").tag(sync=True)
     resizable = Bool(True).tag(sync=True)
+    cursor = Unicode("default").tag(sync=True)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._ipython_display_ = None  # we use _repr_mimebundle_ instread
         # Setup an output widget, so that any errors in our callbacks
         # are actually shown. We display the output in the cell-output
         # corresponding to the cell that instantiates the widget.
@@ -152,14 +155,19 @@
         if "event_type" in content:
             # We have some builtin handling
             if content["event_type"] == "resize":
                 self._rfb_last_resize_event = content
                 self.request_draw()
             elif content["event_type"] == "close":
                 self._repr_mimebundle_ = None
+            # Turn lists into tuples (js/json does not have tuples)
+            if "buttons" in content:
+                content["buttons"] = tuple(content["buttons"])
+            if "modifiers" in content:
+                content["modifiers"] = tuple(content["modifiers"])
             # Let the subclass handle the event
             with self._output_context:
                 self.handle_event(content)
 
     # ---- drawing
 
     def snapshot(self, pixel_ratio=None, _initial=False):
```

### Comparing `jupyter_rfb-0.4.2/jupyter_rfb.egg-info/PKG-INFO` & `jupyter_rfb-0.4.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: jupyter-rfb
-Version: 0.4.2
+Name: jupyter_rfb
+Version: 0.4.3
 Summary: Remote Frame Buffer for Jupyter
 Home-page: https://github.com/vispy/jupyter_rfb
 Author: Almar Klein
 Author-email: almar@almarklein.org
 License: MIT
 Keywords: ipython,jupyter,widgets,visualization,remote frame buffer
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jupyter_rfb-0.4.2/jupyter_rfb.egg-info/SOURCES.txt` & `jupyter_rfb-0.4.3/jupyter_rfb.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 jupyter_rfb.egg-info/PKG-INFO
 jupyter_rfb.egg-info/SOURCES.txt
 jupyter_rfb.egg-info/dependency_links.txt
 jupyter_rfb.egg-info/not-zip-safe
 jupyter_rfb.egg-info/requires.txt
 jupyter_rfb.egg-info/top_level.txt
 jupyter_rfb/labextension/package.json
-jupyter_rfb/labextension/static/261.9ef272ff509129a4e555.js
-jupyter_rfb/labextension/static/920.68e3589cd1cc5ef32304.js
-jupyter_rfb/labextension/static/remoteEntry.f201b0f18d69b7610789.js
+jupyter_rfb/labextension/static/493.cb43b5d572b2f6b10c8e.js
+jupyter_rfb/labextension/static/678.c748912b15ffb2656a49.js
+jupyter_rfb/labextension/static/remoteEntry.0d5a3b6ccc7e17c1ed27.js
 jupyter_rfb/labextension/static/style.js
 jupyter_rfb/labextension/static/third-party-licenses.json
 jupyter_rfb/nbextension/extension.js
 jupyter_rfb/nbextension/index.js
 tests/test_jpg.py
 tests/test_png.py
 tests/test_utils.py
```

### Comparing `jupyter_rfb-0.4.2/setup.py` & `jupyter_rfb-0.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.4.2/tests/test_jpg.py` & `jupyter_rfb-0.4.3/tests/test_jpg.py`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.4.2/tests/test_png.py` & `jupyter_rfb-0.4.3/tests/test_png.py`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.4.2/tests/test_utils.py` & `jupyter_rfb-0.4.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_rfb-0.4.2/tests/test_widget.py` & `jupyter_rfb-0.4.3/tests/test_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import time
 
 import numpy as np
 from pytest import raises
 from jupyter_rfb import RemoteFrameBuffer
 from jupyter_rfb._utils import Snapshot
+from traitlets import TraitError
 
 
 class MyRFB(RemoteFrameBuffer):
     """RFB class to use in the tests."""
 
     max_buffered_frames = 1
 
@@ -207,15 +208,15 @@
     w = RemoteFrameBuffer()
 
     assert w.frame_feedback == {}
 
     assert w.max_buffered_frames == 2
     w.max_buffered_frames = 99
     w.max_buffered_frames = 1
-    with raises(Exception):  # TraitError -> min 1
+    with raises(TraitError):  # TraitError -> min 1
         w.max_buffered_frames = 0
 
     assert w.css_width.endswith("px")
     assert w.css_height.endswith("px")
 
     assert w.resizable
```

