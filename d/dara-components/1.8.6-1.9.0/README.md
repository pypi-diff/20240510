# Comparing `tmp/dara_components-1.8.6-py3-none-any.whl.zip` & `tmp/dara_components-1.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3081755 bytes, number of entries: 86
+Zip file size: 3081751 bytes, number of entries: 86
 -rw-r--r--  2.0 unx      808 b- defN 80-Jan-01 00:00 dara/components/__init__.py
 -rw-r--r--  2.0 unx     3866 b- defN 80-Jan-01 00:00 dara/components/common/__init__.py
 -rw-r--r--  2.0 unx     9487 b- defN 80-Jan-01 00:00 dara/components/common/accordion.py
 -rw-r--r--  2.0 unx     2869 b- defN 80-Jan-01 00:00 dara/components/common/anchor.py
 -rw-r--r--  2.0 unx     4707 b- defN 80-Jan-01 00:00 dara/components/common/base_component.py
 -rw-r--r--  2.0 unx     1433 b- defN 80-Jan-01 00:00 dara/components/common/bullet_list.py
 -rw-r--r--  2.0 unx     4549 b- defN 80-Jan-01 00:00 dara/components/common/button.py
@@ -75,14 +75,14 @@
 -rw-r--r--  2.0 unx     4120 b- defN 80-Jan-01 00:00 dara/components/smart/data_slicer/data_slicer_modal.py
 -rw-r--r--  2.0 unx     1616 b- defN 80-Jan-01 00:00 dara/components/smart/data_slicer/extension/data_slicer_filter.py
 -rw-r--r--  2.0 unx     1345 b- defN 80-Jan-01 00:00 dara/components/smart/data_slicer/extension/filter_status_button.py
 -rw-r--r--  2.0 unx     8656 b- defN 80-Jan-01 00:00 dara/components/smart/data_slicer/utils/core.py
 -rw-r--r--  2.0 unx     1722 b- defN 80-Jan-01 00:00 dara/components/smart/data_slicer/utils/data_preview.py
 -rw-r--r--  2.0 unx     3313 b- defN 80-Jan-01 00:00 dara/components/smart/data_slicer/utils/plotting.py
 -rw-r--r--  2.0 unx     2877 b- defN 80-Jan-01 00:00 dara/components/smart/hierarchy.py
--rw-r--r--  2.0 unx 17002704 b- defN 80-Jan-01 00:00 dara/components/umd/dara.components.umd.js
+-rw-r--r--  2.0 unx 17002703 b- defN 80-Jan-01 00:00 dara/components/umd/dara.components.umd.js
 -rw-r--r--  2.0 unx    23576 b- defN 80-Jan-01 00:00 dara/components/umd/style.css
--rw-r--r--  2.0 unx    10944 b- defN 80-Jan-01 00:00 dara_components-1.8.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     2710 b- defN 80-Jan-01 00:00 dara_components-1.8.6.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 dara_components-1.8.6.dist-info/WHEEL
-?rw-r--r--  2.0 unx     8152 b- defN 16-Jan-01 00:00 dara_components-1.8.6.dist-info/RECORD
-86 files, 17332366 bytes uncompressed, 3068581 bytes compressed:  82.3%
+-rw-r--r--  2.0 unx    10944 b- defN 80-Jan-01 00:00 dara_components-1.9.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2710 b- defN 80-Jan-01 00:00 dara_components-1.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 dara_components-1.9.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     8152 b- defN 16-Jan-01 00:00 dara_components-1.9.0.dist-info/RECORD
+86 files, 17332365 bytes uncompressed, 3068577 bytes compressed:  82.3%
```

## zipnote {}

```diff
@@ -240,20 +240,20 @@
 
 Filename: dara/components/umd/dara.components.umd.js
 Comment: 
 
 Filename: dara/components/umd/style.css
 Comment: 
 
-Filename: dara_components-1.8.6.dist-info/LICENSE
+Filename: dara_components-1.9.0.dist-info/LICENSE
 Comment: 
 
-Filename: dara_components-1.8.6.dist-info/METADATA
+Filename: dara_components-1.9.0.dist-info/METADATA
 Comment: 
 
-Filename: dara_components-1.8.6.dist-info/WHEEL
+Filename: dara_components-1.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: dara_components-1.8.6.dist-info/RECORD
+Filename: dara_components-1.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dara/components/umd/dara.components.umd.js

### js-beautify {}

```diff
@@ -61437,15 +61437,15 @@
             component: item.content
         });
     };
 
     function Accordion(props) {
         const [style2, css2] = core$2.useComponentStyles(props);
         const [value, setValue] = core$2.useVariable(props.value);
-        const [onCarouselAction] = core$2.useAction(props.onchange);
+        const onCarouselAction = core$2.useAction(props.onchange);
 
         function handleChange(val) {
             setValue(val);
             onCarouselAction(val);
         }
         return /* @__PURE__ */ React__default.default.createElement(
             StyledAccordion, {
@@ -61613,15 +61613,16 @@
     const StyledButton$1 = core$2.injectCss(styled__default.default(Button$3)`
     flex: ${(props) => props.isSimpleButton ? void 0 : "1 1 100%"};
 `);
 
     function Button(props) {
         var _a3, _b, _c, _d;
         const [style2, css2] = core$2.useComponentStyles(props);
-        const [onClick, loading] = core$2.useAction(props.onclick);
+        const onClick = core$2.useAction(props.onclick);
+        const loading = core$2.useActionIsLoading(props.onclick);
         const disabled2 = useConditionOrVariable(props.disabled);
         const Icon2 = props.icon ? core$2.getIcon(props.icon) : null;
         const iconColor = Array.isArray(props.children) ? ((_c = (_b = (_a3 = props.children) == null ? void 0 : _a3[0]) == null ? void 0 : _b.props) == null ? void 0 : _c.color) || "inherit" : "inherit";
         return /* @__PURE__ */ React__default.default.createElement(
             StyledButton$1, {
                 $rawCss: css2,
                 className: props.className,
@@ -61687,15 +61688,15 @@
     }
     const StyledButtonBar = core$2.injectCss(ButtonBar$1);
 
     function ButtonBar(props) {
         const formCtx2 = useFormContext(props);
         const [style2, css2] = core$2.useComponentStyles(props);
         const [value, setValue] = core$2.useVariable(formCtx2.resolveInitialValue(props.items[0].value));
-        const [onChangeAction] = core$2.useAction(props.onchange);
+        const onChangeAction = core$2.useAction(props.onchange);
         const onSelect = React.useCallback(
             (item) => {
                 setValue(item.value);
                 onChangeAction(item.value);
                 formCtx2.updateForm(item.value);
             },
             [setValue, onChangeAction]
@@ -62273,15 +62274,15 @@
         ));
     }
     const StyledCarousel = core$2.injectCss(Carousel$1);
 
     function Carousel(props) {
         const [items] = core$2.useVariable(props.items);
         const [value, setValue] = core$2.useVariable(props.value);
-        const [onCarouselAction] = core$2.useAction(props.onchange);
+        const onCarouselAction = core$2.useAction(props.onchange);
 
         function handleChange(val) {
             setValue(val);
             onCarouselAction(val);
         }
         const remappedItems = React.useMemo(
             () => items.map((item) => {
@@ -62358,15 +62359,15 @@
     const StyledCheckbox = core$2.injectCss(CheckboxGroup$1);
 
     function CheckboxGroup(props) {
         const formCtx2 = useFormContext(props);
         const [items] = core$2.useVariable(props.items);
         const [value, setValue] = core$2.useVariable(formCtx2.resolveInitialValue([]));
         const [style2, css2] = core$2.useComponentStyles(props);
-        const [onChangeAction] = core$2.useAction(props.onchange);
+        const onChangeAction = core$2.useAction(props.onchange);
         const onChange2 = React.useCallback(
             (values) => {
                 let newValues;
                 if (Array.isArray(values)) {
                     newValues = values.map((item) => item.value);
                 } else {
                     newValues = values.value;
@@ -65749,15 +65750,15 @@
         ));
     }
     const StyledComponentSelectList = core$2.injectCss(ComponentSelectList$1);
 
     function ComponentSelectList(props) {
         const [style2, css2] = core$2.useComponentStyles(props);
         const [selectedItems, setSelectedItems] = core$2.useVariable(props.selected_items);
-        const [onSelect] = core$2.useAction(props.on_select);
+        const onSelect = core$2.useAction(props.on_select);
         const updateSelectedItems2 = React.useCallback(
             (items) => {
                 const newSelectedItems = props.multi_select ? items : items[0] || null;
                 setSelectedItems == null ? void 0 : setSelectedItems(newSelectedItems);
                 onSelect == null ? void 0 : onSelect(newSelectedItems);
             },
             [onSelect, props.multi_select, setSelectedItems]
@@ -65803,15 +65804,15 @@
         return parsed;
     }
 
     function Datepicker(props) {
         const formCtx2 = useFormContext(props);
         const [style2, css2] = core$2.useComponentStyles(props);
         const [value, setValue] = core$2.useVariable(formCtx2.resolveInitialValue());
-        const [onChangeAction] = core$2.useAction(props.onchange);
+        const onChangeAction = core$2.useAction(props.onchange);
         const isFirstRender = React.useRef(true);
         const onChange2 = (date) => {
             if (!isFirstRender.current && (!Array.isArray(date) && date || Array.isArray(date) && date[0] && date[1])) {
                 let newDate;
                 if (Array.isArray(date)) {
                     newDate = [formatISO(date[0]), formatISO(date[1])];
                 } else {
@@ -65891,15 +65892,15 @@
     const StyledCenter = core$2.injectCss(core$2.Center);
 
     function UploadDropzone(props) {
         const theme2 = useClTheme();
         const [style2, css2] = core$2.useComponentStyles(props);
         const [currentStatus, setCurrentStatus] = React.useState(status.INITIALIZED);
         const [errorMessage, setErrorMessage] = React.useState();
-        const [onFileDrop] = core$2.useAction(props.on_drop);
+        const onFileDrop = core$2.useAction(props.on_drop);
         const extras = core$2.useRequestExtras();
         const onDrop = async (acceptedFiles) => {
             var _a3;
             if (acceptedFiles.length === 1) {
                 setCurrentStatus(status.LOADING);
                 try {
                     const {
@@ -66073,15 +66074,15 @@
     flex-direction: column;
     gap: 0.75rem;
 `;
     const StyledForm = core$2.injectCss("div");
 
     function Form(props) {
         const [formState, setFormState] = core$2.useVariable(props.value);
-        const [onSubmit] = core$2.useAction(props.onsubmit);
+        const onSubmit = core$2.useAction(props.onsubmit);
         const [style2, css2] = core$2.useComponentStyles(props);
         const updateForm = React.useCallback(
             (value, id2) => {
                 setFormState((oldFormState) => ({
                     ...oldFormState,
                     [id2]: value
                 }));
@@ -66208,15 +66209,15 @@
     }
 
     function Input(props) {
         const formCtx2 = useFormContext(props);
         const [style2, css2] = core$2.useComponentStyles(props);
         const [value, setValue] = core$2.useVariable(formCtx2.resolveInitialValue());
         const [internalValue, setInternalValue] = React.useState(value);
-        const [onInputAction] = core$2.useAction(props.onchange);
+        const onInputAction = core$2.useAction(props.onchange);
         const debouncedAction = React.useMemo(() => debounce_1$1(onInputAction, 500), [onInputAction]);
         const debouncedSetValue = React.useMemo(() => debounce_1$1(setValue, 500), [setValue]);
         const debouncedUpdateForm = React.useMemo(() => debounce_1$1(formCtx2.updateForm, 500), [formCtx2.updateForm]);
 
         function handleChange(val) {
             let newValue = val;
             if (props.type === "number") {
@@ -75052,15 +75053,15 @@
 
     function RadioGroup(props) {
         var _a3;
         const formCtx2 = useFormContext(props);
         const [items] = core$2.useVariable(props.items);
         const [value, setValue] = core$2.useVariable(formCtx2.resolveInitialValue([]));
         const [style2, css2] = core$2.useComponentStyles(props);
-        const [onChangeAction] = core$2.useAction(props.onchange);
+        const onChangeAction = core$2.useAction(props.onchange);
         const onChange2 = React.useCallback(
             (values) => {
                 setValue(values.value);
                 onChangeAction(values.value);
                 formCtx2.updateForm(values.value);
             },
             [setValue]
@@ -75131,15 +75132,15 @@
                 return matchingItem;
             }
             return typeof val === "string" || typeof val === "number" ? {
                 label: String(val),
                 val
             } : val;
         };
-        const [onChangeAction] = core$2.useAction(props.onchange);
+        const onChangeAction = core$2.useAction(props.onchange);
         const itemHasListSection = React.useRef(null);
         if (itemHasListSection.current === null) {
             itemHasListSection.current = hasListSection(formattedItems);
         }
         React.useEffect(() => {
             if (props.multiselect && value !== void 0 && !Array.isArray(value)) {
                 throw new Error("Value for multiselect should be a Variable instance of an array");
@@ -75253,15 +75254,15 @@
     }
     const StyledSlider = core$2.injectCss(Slider$1);
 
     function Slider(props) {
         const formCtx2 = useFormContext(props);
         const [style2, css2] = core$2.useComponentStyles(props);
         const [value, setValue] = core$2.useVariable(formCtx2.resolveInitialValue(props.domain[0]));
-        const [onTrack] = core$2.useAction(props.onchange);
+        const onTrack = core$2.useAction(props.onchange);
         const debouncedSetValue = React.useMemo(() => debounce_1$1(setValue, 300), [setValue]);
         const debouncedOnTrack = React.useMemo(() => debounce_1$1(onTrack, 300), [onTrack]);
         const debouncedUpdateForm = React.useMemo(() => debounce_1$1(formCtx2.updateForm, 300), [formCtx2.updateForm]);
         const isOutputNumber = typeof value === "number";
 
         function onChange2(values) {
             let serialisedValues = values;
@@ -75398,15 +75399,15 @@
 `;
     const SwitchDiv = core$2.injectCss(_SwitchDiv);
 
     function Switch(props) {
         const formCtx2 = useFormContext(props);
         const [style2, css2] = core$2.useComponentStyles(props);
         const [value, setValue] = core$2.useVariable(formCtx2.resolveInitialValue());
-        const [onChangeAction] = core$2.useAction(props.onchange);
+        const onChangeAction = core$2.useAction(props.onchange);
 
         function onChange2(enabled) {
             setValue(enabled);
             onChangeAction(enabled);
             formCtx2.updateForm(enabled);
         }
         return /* @__PURE__ */ React__default.default.createElement(SwitchDiv, {
@@ -75942,15 +75943,15 @@
             }
             return extraDataCache.current[idx];
         }
         React.useEffect(() => {
             extraDataCache.current = {};
         }, [getData]);
         const [style2, css2] = core$2.useComponentStyles(props);
-        const [onClickRow] = core$2.useAction(props.onclick_row);
+        const onClickRow = core$2.useAction(props.onclick_row);
         const columns = React.useMemo(() => {
             const mappedCols = mapColumns(resolvedColumns);
             if (props.show_checkboxes && props.onclick_row || props.selected_indices) {
                 mappedCols == null ? void 0 : mappedCols.unshift(Table$1.ActionColumn([Table$1.Actions.SELECT], "select_box_col", "left", true));
             }
             return mappedCols;
         }, [resolvedColumns, props.onclick_row]);
@@ -76125,15 +76126,15 @@
     const StyledTextarea = core$2.injectCss(TextArea);
 
     function Textarea(props) {
         const formCtx2 = useFormContext(props);
         const [style2, css2] = core$2.useComponentStyles(props);
         const [value, setValue] = core$2.useVariable(formCtx2.resolveInitialValue());
         const [internalValue, setInternalValue] = React.useState(value);
-        const [onInputAction] = core$2.useAction(props.onchange);
+        const onInputAction = core$2.useAction(props.onchange);
         const debouncedAction = React.useMemo(() => debounce_1$1(onInputAction, 500), [onInputAction]);
         const debouncedSetValue = React.useMemo(() => debounce_1$1(setValue, 500), [setValue]);
         const debouncedUpdateForm = React.useMemo(() => debounce_1$1(formCtx2.updateForm, 500), [formCtx2.updateForm]);
 
         function handleChange(val) {
             setInternalValue(val);
             debouncedSetValue(val);
@@ -76235,15 +76236,15 @@
                 libraries.forEach((url2) => {
                     loadBokehLibrary(url2, bokehVersion);
                 });
             }
             events2.forEach(([ev, handler]) => {
                 document.removeEventListener(ev, handler);
             });
-            eventActions.forEach(([name2, [action]]) => {
+            eventActions.forEach(([name2, action]) => {
                 const handler = (e3) => {
                     action(e3.detail);
                 };
                 const evtName = createEventName(name2, docJson.roots[0].id);
                 document.addEventListener(evtName, handler);
                 events2.push([evtName, handler]);
             });
@@ -314596,15 +314597,15 @@
         const [figure, setFigure] = React.useState(() => JSON.parse(props.figure));
         const eventActions = /* @__PURE__ */ new Map();
         if (props.events) {
             props.events.forEach((event2) => {
                 var _a3;
                 const actions = new Array();
                 event2 == null ? void 0 : event2.actions.forEach((action) => {
-                    const [actionHandler] = core$2.useAction(action);
+                    const actionHandler = core$2.useAction(action);
                     actions.push({
                         custom_js: event2.custom_js,
                         handler: actionHandler
                     });
                 });
                 const currentActions = (_a3 = eventActions.get(event2.event_name)) != null ? _a3 : [];
                 eventActions.set(event2.event_name, [...currentActions, ...actions]);
@@ -315500,15 +315501,15 @@
     :hover {
         transform: none;
     }
 `;
 
     function FilterStatusButton(props) {
         const [filterStats] = core$2.useVariable(props.filter_stats);
-        const [onClick] = core$2.useAction(props.on_click);
+        const onClick = core$2.useAction(props.on_click);
 
         function clickHandler() {
             onClick(null);
         }
         return ReactDOM__default.default.createPortal(
             /* @__PURE__ */
             React__namespace.createElement(
@@ -319669,15 +319670,15 @@
         });
     }
     const StyledHierarchyViewer = core$2.injectCss(HierarchyViewer$1);
 
     function HierarchyViewer(props) {
         const [style2, css2] = core$2.useComponentStyles(props);
         const hierarchy2 = core$2.useVariable(props.hierarchy)[0];
-        const [onClick] = core$2.useAction(props.on_click_node);
+        const onClick = core$2.useAction(props.on_click_node);
         return /* @__PURE__ */ React__default.default.createElement(
             StyledHierarchyViewer, {
                 $rawCss: css2,
                 allowLeafClick: props.allow_leaf_click,
                 allowParentClick: props.allow_parent_click,
                 data: hierarchy2,
                 onClick,
@@ -432587,17 +432588,17 @@
     function CausalGraphViewer(props) {
         const {
             pushNotification
         } = core$2.Notifications.useNotifications();
         const [style2, css2] = core$2.useComponentStyles(props);
         const theme2 = useClTheme();
         const [graphData, setCausalGraphVariable] = core$2.useVariable(props.causal_graph);
-        const [onClickNode] = core$2.useAction(props.on_click_node);
-        const [onClickEdge] = core$2.useAction(props.on_click_edge);
-        const [onUpdate] = core$2.useAction(props.on_update);
+        const onClickNode = core$2.useAction(props.on_click_node);
+        const onClickEdge = core$2.useAction(props.on_click_edge);
+        const onUpdate = core$2.useAction(props.on_update);
         const graphLayout = React.useMemo(() => parseLayoutDefinition(props.graph_layout), [props.graph_layout]);
         const formattedDefaultLegends = React.useMemo(() => {
             return Object.fromEntries(
                 Object.entries(props.default_legends).map(([editorMode, defaultLegends]) => {
                     return [editorMode, defaultLegends.map((legend) => transformLegendColor(theme2, legend))];
                 })
             );
@@ -432643,15 +432644,15 @@
     }
     const StyledHierarchyBuilder = core$2.injectCss(NodeHierarchyBuilder$1);
 
     function NodeHierarchyBuilder(props) {
         const [style2, css2] = core$2.useComponentStyles(props);
         const mounted = React.useRef(false);
         const [nodes, setNodes] = core$2.useVariable(props.nodes);
-        const [updateHandler] = core$2.useAction(props.on_update);
+        const updateHandler = core$2.useAction(props.on_update);
         if (mounted.current === false) {
             if (!(Array.isArray(nodes) && nodes.every(
                     (layer) => Array.isArray(layer) && layer.every((node2) => typeof node2 === "string" || typeof node2 === "object")
                 ))) {
                 throw new Error('NodeHierarchyBuilder expects "nodes" to be a list of lists of strings or Node objects');
             }
             mounted.current = true;
@@ -432718,17 +432719,17 @@
         const [style2, css2] = core$2.useComponentStyles(props);
         const [nodes] = core$2.useVariable(props.nodes);
         const parsedNodes = React.useMemo(() => parseNodes(nodes), [nodes]);
         const theme2 = useClTheme();
         const [initialConstraints] = core$2.useVariable(props.initial_constraints);
         const parsedConstraints = React.useMemo(() => parseConstraints(initialConstraints), [initialConstraints]);
         const graphLayout = React.useMemo(() => parseLayoutDefinition(props.graph_layout), []);
-        const [onClickEdge] = core$2.useAction(props.on_click_edge);
-        const [onClickNode] = core$2.useAction(props.on_click_node);
-        const [onUpdate] = core$2.useAction(props.on_update);
+        const onClickEdge = core$2.useAction(props.on_click_edge);
+        const onClickNode = core$2.useAction(props.on_click_node);
+        const onUpdate = core$2.useAction(props.on_update);
         const formattedDefaultLegends = React.useMemo(() => {
             return Object.fromEntries(
                 Object.entries(props.default_legends).map(([editorMode, defaultLegends]) => {
                     return [editorMode, defaultLegends.map((legend) => transformLegendColor(theme2, legend))];
                 })
             );
         }, [props.default_legends, theme2]);
```

## Comparing `dara_components-1.8.6.dist-info/LICENSE` & `dara_components-1.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dara_components-1.8.6.dist-info/METADATA` & `dara_components-1.9.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: dara-components
-Version: 1.8.6
+Version: 1.9.0
 Summary: Components for the Dara Framework
 Home-page: https://dara.causalens.com/
 License: Apache-2.0
 Author: Patricia Jacob
 Author-email: patricia@causalens.com
 Requires-Python: >=3.8.0,<3.12.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bokeh (>=3.1.0,<3.2.0)
 Requires-Dist: cai-causal-graph (>=0.3.6)
-Requires-Dist: dara-core (==1.8.6)
+Requires-Dist: dara-core (==1.9.0)
 Requires-Dist: dill (>=0.3.0,<0.4.0)
 Requires-Dist: matplotlib (>=2.0.0)
 Requires-Dist: pandas (>=1.1.0,<3.0.0)
 Requires-Dist: plotly (>=5.14.0,<5.15.0)
 Requires-Dist: scipy
 Requires-Dist: seaborn (>=0.11.0)
 Project-URL: Repository, https://github.com/causalens/dara
 Description-Content-Type: text/markdown
 
 # Dara Components
 
-<img src="https://github.com/causalens/dara/blob/VERSION-1.8.6/img/dara_light.svg?raw=true">
+<img src="https://github.com/causalens/dara/blob/VERSION-1.9.0/img/dara_light.svg?raw=true">
 
 ![Master tests](https://github.com/causalens/dara/actions/workflows/tests.yml/badge.svg?branch=master)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
 [![PyPI](https://img.shields.io/pypi/v/dara-components.svg?color=dark-green)](https://pypi.org/project/dara-components/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dara-components.svg?color=dark-green)](https://pypi.org/project/dara-components/)
 [![NPM](https://img.shields.io/npm/v/@darajs/components.svg?color=dark-green)](https://www.npmjs.com/package/@darajs/components)
```

## Comparing `dara_components-1.8.6.dist-info/RECORD` & `dara_components-1.9.0.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -74,13 +74,13 @@
 dara/components/smart/data_slicer/data_slicer_modal.py,sha256=t7NywA5DiFiUiUnuFQbTAAVm6PM7Qjd6LGzd9OWA0QE,4120
 dara/components/smart/data_slicer/extension/data_slicer_filter.py,sha256=2wdWn3gcrewrhUZ4tGNwAh1JURpcLmeDKIP7c5j9_sI,1616
 dara/components/smart/data_slicer/extension/filter_status_button.py,sha256=02CgqHEBgkZg1E9v9HGrnRYvEiMNhYpajyOwGuPNV1M,1345
 dara/components/smart/data_slicer/utils/core.py,sha256=6BrmG-iwQCuwUAKQ-y9zFKLeinnzhXIaUOB58UxCYbc,8656
 dara/components/smart/data_slicer/utils/data_preview.py,sha256=OAphjMrm3F76XmJ09X7sZSeOeKqGJFwN5ooo3qcyrG4,1722
 dara/components/smart/data_slicer/utils/plotting.py,sha256=JYzdQLXdAD0A8k2W-764xUr7zN0Ri5nf3OQ2Nb_iuiY,3313
 dara/components/smart/hierarchy.py,sha256=STkgyZiVB1c6KJtcKnn1r8lnjZAIrWkTCpZ_WCyCI1c,2877
-dara/components/umd/dara.components.umd.js,sha256=fMV3CmhpXhtfwoHtFCjvi9lUbCH8KknqjsH3HW0nuuc,17002704
+dara/components/umd/dara.components.umd.js,sha256=7a0IhPt-swT52ZyvJeyVh7khAn6oUZm4ClPLlZs3rDI,17002703
 dara/components/umd/style.css,sha256=cvNU48TRRp73QxBrE9awB-zm3YURFnFlASafeLTNa_U,23576
-dara_components-1.8.6.dist-info/LICENSE,sha256=r9u1w2RvpLMV6YjuXHIKXRBKzia3fx_roPwboGcLqCc,10944
-dara_components-1.8.6.dist-info/METADATA,sha256=JtPknx-gyz0Uw2-wYKmXlQb44RSYoP8dm-thT6MEgNg,2710
-dara_components-1.8.6.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-dara_components-1.8.6.dist-info/RECORD,,
+dara_components-1.9.0.dist-info/LICENSE,sha256=r9u1w2RvpLMV6YjuXHIKXRBKzia3fx_roPwboGcLqCc,10944
+dara_components-1.9.0.dist-info/METADATA,sha256=x8KtEfxQKaB1UK5FQDmJyTTR_lq6AQbB0Q_O4NMrjik,2710
+dara_components-1.9.0.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+dara_components-1.9.0.dist-info/RECORD,,
```

