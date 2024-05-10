# Comparing `tmp/ipymolstar-0.0.4.tar.gz` & `tmp/ipymolstar-0.0.5.tar.gz`

## Comparing `ipymolstar-0.0.4.tar` & `ipymolstar-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ipymolstar-0.0.4/src/ipymolstar/__init__.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 ipymolstar-0.0.4/src/ipymolstar/pdbe-dark.css
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ipymolstar-0.0.4/src/ipymolstar/pdbe-light.css
--rw-r--r--   0        0        0     7959 2020-02-02 00:00:00.000000 ipymolstar-0.0.4/src/ipymolstar/widget.js
--rw-r--r--   0        0        0     6103 2020-02-02 00:00:00.000000 ipymolstar-0.0.4/src/ipymolstar/widget.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ipymolstar-0.0.4/.gitignore
--rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 ipymolstar-0.0.4/README.md
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 ipymolstar-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 ipymolstar-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ipymolstar-0.0.5/src/ipymolstar/__init__.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 ipymolstar-0.0.5/src/ipymolstar/pdbe-dark.css
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ipymolstar-0.0.5/src/ipymolstar/pdbe-light.css
+-rw-r--r--   0        0        0     6949 2020-02-02 00:00:00.000000 ipymolstar-0.0.5/src/ipymolstar/widget.js
+-rw-r--r--   0        0        0     8454 2020-02-02 00:00:00.000000 ipymolstar-0.0.5/src/ipymolstar/widget.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ipymolstar-0.0.5/.gitignore
+-rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 ipymolstar-0.0.5/README.md
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 ipymolstar-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 ipymolstar-0.0.5/PKG-INFO
```

### Comparing `ipymolstar-0.0.4/src/ipymolstar/widget.js` & `ipymolstar-0.0.5/src/ipymolstar/widget.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,9 +1,8 @@
-import * as myModule from "https://www.ebi.ac.uk/pdbe/pdb-component-library/js/pdbe-molstar-plugin-3.1.3.js";
-// import * as myModule from "https://cdn.jsdelivr.net/npm/pdbe-molstar@latest/build/pdbe-molstar-plugin.js"
+import * as myModule from "https://cdn.jsdelivr.net/npm/pdbe-molstar@3.2.0/build/pdbe-molstar-plugin.js"
 
 function standardize_color(str) {
     var ctx = document.createElement("canvas").getContext("2d");
     ctx.fillStyle = str;
     return ctx.fillStyle;
 }
 
@@ -178,32 +177,47 @@
         },
         "change:color_data": () => {
             const selectValue = model.get("color_data");
             if (selectValue !== null) {
                 viewerInstance.visual.select(selectValue);
             }
         },
+        "change:tooltips": () => {
+            const tooltipValue = model.get("tooltips");
+            if (tooltipValue !== null) {
+                viewerInstance.visual.tooltips(tooltipValue);
+            }
+        },
     };
 
     let otherCallbacks = {
         "change:molecule_id": () => {
             viewerInstance.visual.update(getOptions(model), true);
         },
         "change:custom_data": () => {
             viewerInstance.visual.update(getOptions(model), true);
         },
+        "change:visual_style": () => {
+            viewerInstance.visual.update(getOptions(model), true);
+        },
+        // "change:lighting": () => {
+        //   viewerInstance.visual.update(getOptions(model), true);
+        // },
         "change:bg_color": () => {
             viewerInstance.canvas.setBgColor(toRgb(model.get("bg_color")));
         },
         "change:_reset": () => {
             const resetValue = model.get("_reset");
             if (resetValue !== null) {
                 viewerInstance.visual.reset(resetValue);
             }
         },
+        "change:_clear_tooltips": () => {
+            viewerInstance.visual.clearTooltips();
+        }
     };
 
     let combinedCallbacks = Object.assign({},
         callbacksLoadComplete,
         otherCallbacks
     );
 
@@ -219,58 +233,14 @@
 
     document.addEventListener("PDB.molstar.mouseover", (e) => {
         const eventData = e.eventData;
         model.set("mouseover_event", eventData);
         model.save_changes();
     });
 
-    // TODO return unsubscribe
-
-    // these require re-render
-    // model.on("change:visual_style", () => {
-    //     viewerInstance.visual.update({visualStyle: model.get('visual_style')});
-    //     console.log(model.get('visual_style'));
-    // });
-
-    // model.on("change:lighting", () => {
-    //     viewerInstance.visual.update({lighting: model.get('lighting')});
-    // });
-
-    // model.on("change:_focus", () => {
-    //   const focusValue = model.get("_focus");
-    //   if (focusValue !== null) {
-    //     viewerInstance.visual.focus(focusValue);
-    //   }
-    // });
-    // model.on("change:_highlight", () => {
-    //   const highlightValue = model.get("_highlight");
-    //   if (highlightValue !== null) {
-    //     viewerInstance.visual.highlight(highlightValue);
-    //   }
-    // });
-    // model.on("change:_clear_highlight", () => {
-    //   1;
-    //   viewerInstance.visual.clearHighlight();
-    // });
-    // model.on("change:_clear_selection", () => {
-    //   viewerInstance.visual.clearSelection(model.get("_args")["number"]);
-    // });
-    // });
-    // model.on("change:_update", () => {
-    //   const updateValue = model.get("_update");
-    //   if (updateValue !== null) {
-    //     viewerInstance.visual.update(updateValue);
-    //   }
-
-    // });
-    // model.on("change:hide_coarse", () => {
-    //   viewerInstance.visual.visibility({ water: !model.get("hide_coarse") });
-    // });
-
-    // this could be a loop?
     return () => {
         unsubscribes.forEach((unsubscribe) => unsubscribe());
     };
 }
 
 export default {
     render
```

### Comparing `ipymolstar-0.0.4/README.md` & `ipymolstar-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ipymolstar-0.0.4/PKG-INFO` & `ipymolstar-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ipymolstar
-Version: 0.0.4
+Version: 0.0.5
 Requires-Dist: anywidget
 Provides-Extra: dev
 Requires-Dist: jupyterlab; extra == 'dev'
 Requires-Dist: watchfiles; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # ipymolstar
```

