# Comparing `tmp/hstream-0.0.9.tar.gz` & `tmp/hstream-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hstream-0.0.9.tar", last modified: Thu Nov 10 08:17:21 2022, max compression
+gzip compressed data, was "hstream-0.1.0.tar", max compression
```

## Comparing `hstream-0.0.9.tar` & `hstream-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,15 @@
-drwxr-xr-x   0 conrad     (501) staff       (20)        0 2022-11-10 08:17:21.510389 hstream-0.0.9/
--rw-r--r--   0 conrad     (501) staff       (20)     2069 2022-11-10 08:17:21.510231 hstream-0.0.9/PKG-INFO
--rw-r--r--   0 conrad     (501) staff       (20)     1650 2022-11-10 08:17:04.000000 hstream-0.0.9/README
-drwxr-xr-x   0 conrad     (501) staff       (20)        0 2022-11-10 08:17:21.507982 hstream-0.0.9/hstream.egg-info/
--rw-r--r--   0 conrad     (501) staff       (20)     2069 2022-11-10 08:17:21.000000 hstream-0.0.9/hstream.egg-info/PKG-INFO
--rw-r--r--   0 conrad     (501) staff       (20)      413 2022-11-10 08:17:21.000000 hstream-0.0.9/hstream.egg-info/SOURCES.txt
--rw-r--r--   0 conrad     (501) staff       (20)        1 2022-11-10 08:17:21.000000 hstream-0.0.9/hstream.egg-info/dependency_links.txt
--rw-r--r--   0 conrad     (501) staff       (20)       51 2022-11-10 08:17:21.000000 hstream-0.0.9/hstream.egg-info/entry_points.txt
--rw-r--r--   0 conrad     (501) staff       (20)      126 2022-11-10 08:17:21.000000 hstream-0.0.9/hstream.egg-info/requires.txt
--rw-r--r--   0 conrad     (501) staff       (20)       12 2022-11-10 08:17:21.000000 hstream-0.0.9/hstream.egg-info/top_level.txt
-drwxr-xr-x   0 conrad     (501) staff       (20)        0 2022-11-10 08:17:21.509493 hstream-0.0.9/hyperstream/
--rw-r--r--   0 conrad     (501) staff       (20)       28 2022-11-10 06:45:33.000000 hstream-0.0.9/hyperstream/__init__.py
--rw-r--r--   0 conrad     (501) staff       (20)       61 2022-11-10 06:58:34.000000 hstream-0.0.9/hyperstream/__main__.py
--rw-r--r--   0 conrad     (501) staff       (20)    12112 2022-11-10 05:45:41.000000 hstream-0.0.9/hyperstream/components.py
--rw-r--r--   0 conrad     (501) staff       (20)     1799 2022-11-09 12:51:35.000000 hstream-0.0.9/hyperstream/hstag.py
--rw-r--r--   0 conrad     (501) staff       (20)    15375 2022-11-10 07:38:29.000000 hstream-0.0.9/hyperstream/hyperstream.py
--rw-r--r--   0 conrad     (501) staff       (20)      457 2022-11-10 06:49:13.000000 hstream-0.0.9/hyperstream/runner.py
-drwxr-xr-x   0 conrad     (501) staff       (20)        0 2022-11-10 08:17:21.509942 hstream-0.0.9/hyperstream/templates/
--rw-r--r--   0 conrad     (501) staff       (20)      498 2022-11-10 05:07:06.000000 hstream-0.0.9/hyperstream/templates/header.html
--rw-r--r--   0 conrad     (501) staff       (20)      797 2022-11-10 03:39:04.000000 hstream-0.0.9/hyperstream/templates/main.html
--rw-r--r--   0 conrad     (501) staff       (20)       38 2022-11-10 08:17:21.510425 hstream-0.0.9/setup.cfg
--rw-r--r--   0 conrad     (501) staff       (20)     1146 2022-11-10 08:17:10.000000 hstream-0.0.9/setup.py
+-rw-r--r--   0        0        0     3173 2024-05-09 12:48:28.492108 hstream-0.1.0/README.md
+-rw-r--r--   0        0        0     6874 2024-05-09 04:53:45.070019 hstream-0.1.0/hstream/HSServer.py
+-rw-r--r--   0        0        0       53 2024-05-09 04:53:45.070344 hstream-0.1.0/hstream/__init__.py
+-rw-r--r--   0        0        0      142 2024-05-09 12:06:39.049619 hstream-0.1.0/hstream/__main__.py
+-rw-r--r--   0        0        0     1030 2024-05-09 12:15:26.028596 hstream-0.1.0/hstream/cli.py
+-rw-r--r--   0        0        0    16577 2024-05-09 05:42:06.854007 hstream-0.1.0/hstream/components/components.py
+-rw-r--r--   0        0        0     4633 2024-05-09 04:53:45.071931 hstream-0.1.0/hstream/components/styling_components.py
+-rw-r--r--   0        0        0      766 2024-05-09 04:53:45.072204 hstream-0.1.0/hstream/hs.py
+-rw-r--r--   0        0        0      761 2024-05-09 12:16:49.253594 hstream-0.1.0/hstream/run.py
+-rw-r--r--   0        0        0      394 2024-05-09 04:53:45.072863 hstream-0.1.0/hstream/template.py
+-rw-r--r--   0        0        0      161 2024-05-09 04:53:45.073202 hstream-0.1.0/hstream/templates/error_html.html
+-rw-r--r--   0        0        0     2453 2024-05-09 04:53:45.073487 hstream-0.1.0/hstream/templates/format_html.html
+-rw-r--r--   0        0        0     2659 2024-05-09 04:53:45.073769 hstream-0.1.0/hstream/utils.py
+-rw-r--r--   0        0        0      526 2024-05-09 11:55:23.058055 hstream-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3798 1970-01-01 00:00:00.000000 hstream-0.1.0/PKG-INFO
```

### Comparing `hstream-0.0.9/hyperstream/components.py` & `hstream-0.1.0/hstream/components/components.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,287 +1,354 @@
-from yattag import Doc
-from yattag.simpledoc import SimpleDoc
-from typing import Literal, OrderedDict
+from typing import List, Literal, Tuple
 from functools import wraps
 from pathlib import Path
 from inspect import getframeinfo, stack
+import cherrypy
 
 
-class Components:
-    def __init__(self) -> None:
-        self.return_old_doc_and_init_new()
-        # self.doc, self.tag, self.text = Doc().tagtext()
+def component_wrapper(component_fucntion):
+    @wraps(component_fucntion)
+    def wrapped_component_function(self, *method_args, **method_kwargs):
+        # if we arn't provided a key let make one
+        key = method_kwargs.get("key", False)
+        if not key:
+            key = self.get_key_based_on_call(method_args)
+            method_kwargs["key"] = key
+        value = self.component_value(
+            default_value=method_kwargs.get("default_value", None),
+            key=method_kwargs["key"],
+        )
+        method_kwargs["value"] = value
+        with self.tag(
+            "div",
+            ("id", f"container_for_{method_kwargs['key']}"),
+            ("hx-trigger", f"none"),
+        ):
+            # each component should return a function that formats the user value stored in the session
+            # after sent back by htmx
+            user_input_formatting_fn = component_fucntion(
+                self, *method_args, **method_kwargs
+            )
+        # if there is no current value let subsitute the default value
+
+        if user_input_formatting_fn != None:
+            return user_input_formatting_fn(value)
+        else:
+            # temporary while we get all components to return a function
+            return value
+
+    return wrapped_component_function
 
+
+class ComponentsGeneric:
     def get_key_based_on_call(self, message):
         """
         Get the concat the functions call line and arguments to get a key
 
-        * Gothca * : f-strings are evaluated before we get to inspect them so they'll
-                     cause double-ups and might need explicit keys assigned
-
+        * Gothca * : loop will be on the same line and therefor get the same key,
+                     we need the user to specify a key in that case
+                     this case is not checked for atm
         """
         for i in range(20):
-            
-            caller = getframeinfo(stack()[i][0])
-            if str(self.path_to_user_script) in caller.filename:
-                # breakpoint()
-                call_signiture = f"{Path(caller.filename).stem}, {caller.lineno}"
+            # import ipdb; ipdb.set_trace()
+            inspect_caller = getframeinfo(stack()[i][0])
+            if "HS_STREAM_USER_FILE" in inspect_caller.filename:
+                call_signiture = (
+                    f"{Path(inspect_caller.filename).stem}, {inspect_caller.lineno}"
+                )
                 key = "".join(x for x in call_signiture if x.isalpha() or x.isnumeric())
                 return key
 
-    def build_component(
-        self, component_type, label=None, default_value=None, key=None, **kwargs
-    ):
+    def component_value(self, default_value=None, key=None, **kwargs):
         """Writes a component to the SH front end
 
         Args:
-            label (_type_, optional): Must be ubique within the app. Content to write to the web front end. Defaults to None.
+            label (_type_, optional): Must be unique within the app. Content to write to the web front end. Defaults to None.
             default_value (_type_, optional): default value the component returns before use enters value - will always be null for text or component where user doesn't input. Defaults to None.
         """
+        return cherrypy.session.get(key, default_value)
 
-        # to support user's use of `with hs.tag` we first need to exit out of the context manager
-        # while 'yattag.simpledoc.SimpleDoc.DocumentRoot' not in str(type(self.doc.current_tag)):
-
-        component_key = key
-
-        assert (
-            not "_" in component_key
-        ), "please don't use underscores in keys"  # we use headers to update compoennts by key but headers don't like underscores
-        components = self.get_components()
-        if not components.get(component_key, False):
-            # if we don't have this component stored initialise it
-            components[component_key] = {
-                # these values shouldn't change between reruns so we set them here on initialisation
-                "current_value": default_value,
-                "component_key": component_key,
-                "component_type": component_type,
-            }
-
-        components[component_key].update(
-            {
-                # these values can change between reruns (i.e. text input is outputted to a write component)
-                "label": label,
-            }
-        )
-
-        if kwargs:
-            components[component_key].update(kwargs)
-        try:
-            self.write_components(
-                components,
-            )
-        except Exception as e:
-            print("error ", e)
-
-        return components[component_key]["current_value"]
-
-    def component_wrapper(component_fucntion):
-        @wraps(component_fucntion)
-        def wrapped_component_function(self, *method_args, **method_kwargs):
-            # if we arn't provided a key let make one
-            if not method_kwargs.get("key", False):
-                method_kwargs["key"] = self.get_key_based_on_call(method_args)
-
-            # if there is no current value let subsitute the default value
-            value = self.build_component(
-                **component_fucntion(self, *method_args, **method_kwargs)
-            )
-            return value
-
-        return wrapped_component_function
-
-    def return_old_doc_and_init_new(self):
-        old_doc = ""
-        if getattr(self, "doc", False):
-            #
-            # to support user's use of `with hs.tag` we first need to exit out of the context manager
-            # untill we reach the root (in case we are nested deep within `with's`)
-            while "yattag.simpledoc.SimpleDoc.DocumentRoot" not in str(
-                type(self.doc.current_tag)
-            ):
-                self.doc.current_tag.__exit__(False, value=None, traceback=False)
-            old_doc = str(self.doc.getvalue())
-
-        # Refresh the doc to blank for the next element
-        self.doc, self.tag, self.text = Doc().tagtext()
-        return old_doc
 
+class Components(ComponentsGeneric):
     @component_wrapper
-    def markdown(self, text: str, *, key: str = False) -> None:
+    def markdown(self, text: str, key: str = False, **kwargs) -> None:
         import markdown
 
-        html = markdown.markdown(text)
-        with self.tag("div"):
+        # import ipdb; ipdb.set_trace()
+        html = markdown.markdown(str(text))
+        with self.tag(
+            "div",
+        ):
             self.doc.asis(html)
-        display_html = self.return_old_doc_and_init_new()
-        return dict(
-            label=display_html,
-            component_type="Markdown",
-            key=key,
-        )
 
     @component_wrapper
-    def text_input(self, label: str, *, default_value: str = '', key: str = None) -> str:
+    def text_input(
+        self,
+        label: str,
+        default_value: str = "",
+        key: str = None,
+        placeholder: str = False,
+        **kwargs,
+    ) -> str:
         """Displays text input for user to input text
 
         Args:
             text (str): label to display to user describing the text input
             default_value (str): value innitially entered into text box
         Returns:
             str: text inputted by user
         """
-        component_attr = self.get_components().get(key, OrderedDict())
         with self.tag("label"):
             self.text(label)
         with self.tag(
             "input",
-            ("name", key),
-            ("hx-post", f"/value_changed/{key}"),
-            ("hx-trigger", "focusout"),
+            ("hx-ext", "debug"),
+            ("name", "new_value"),
+            ("hx-post", f"/set_component_value?component_id={key}"),
+            ("hx-swap", "none"),
             ("type", "text"),
         ):
-            pass
-        html = self.return_old_doc_and_init_new()
-        return dict(
-            label=html, component_type="TextInput", default_value=default_value, key=key
-        )
+            if kwargs["value"]:
+                self.doc.attr(value=str(kwargs["value"]))
+            elif placeholder:
+                self.doc.attr(placeholder=placeholder)
+        return lambda x: str(x)
+
+    def html(self, *args, **kwargs):
+        return self.tag(*args, **kwargs)
 
     @component_wrapper
-    def number_input(self, label: str, *, default_value: int = 0, key: str = None) -> str:
+    def number_input(
+        self, label: str, default_value: int = 0, key: str = None, **kwargs
+    ) -> str:
         """Displays text input for user to input text
-
         Args:
             text (str): label to display to user describing the text input
             default_value (str): value innitially entered into text box
         Returns:
             str: text inputted by user
         """
-        component_attr = self.get_components().get(key, OrderedDict())
         with self.tag("label"):
             self.text(label)
         with self.tag(
             "input",
-            ("name", key),
-            ("hx-post", f"/value_changed/{key}"),
+            ("name", "new_value"),
+            ("hx-post", f"/set_component_value?component_id={key}"),
             ("hx-trigger", "focusout"),
             ("type", "number"),
+            ("value", str(kwargs["value"])),
         ):
             pass
-        html = self.return_old_doc_and_init_new()
-        return dict(
-            label=html, component_type="TextInput", default_value=default_value, key=key
-        )
 
     @component_wrapper
-    def select_box(self, label: list[str], default_value: str = False, key: str = None) -> str:
+    def select_box(
+        self, label: List[str], default_value: str = None, key: str = None, **kwargs
+    ) -> str:
+        """
+        Dropdown component for user to select from a list of options
+
+        Args:
+            label (List[str]): Options to display to user
+            default_value (str, optional): Value to select when component load the first time. Defaults to False.
+            key (str, optional): Unique key - default is set based on label (options) so set this if there are multiple inputs with same label argument. Defaults to None.
+
+        Returns:
+            str: Selected value
+        """
+        # HStream developer note: The default value logic is handled by the `@component_wrapper`
         with self.doc.select(
-            ("name", key),
-            ("hx-post", f"/value_changed/{key}"),
-            # multiple = "multiple"
+            ("name", "new_value"),
+            ("hx-post", f"/set_component_value?component_id={key}"),
         ):
             for value in label:
                 with self.tag(
                     "option",
                     ("value", value),
                 ):
+                    if kwargs["value"] == value:
+                        self.doc.attr(selected="")
+
+                    self.text(str(value))
+
+    @component_wrapper
+    def multiselect(
+        self, label: List[str], default_value: List[int] = [], key: str = None, **kwargs
+    ) -> List[int]:
+        """
+        Dropdown component for user to select multiple options from a list and returns a comma separated string of the  of selected options
+
+        Args:
+            label (List[str]): Options to display to user
+            default_value (str, optional): Value to select when component load the first time. Defaults to False.
+            key (str, optional): Unique key - default is set based on label (options) so set this if there are multiple inputs with same label argument. Defaults to None.
+
+        Returns:
+            str: Selected value
+        """
+
+        assert type(label) == type([]) and type(default_value) == type(
+            []
+        ), "multiselect requires a list of options and a list of default values"
+
+        # HStream developer note: The default value logic is handled by the `@component_wrapper`
+        if type(kwargs["value"]) == type(""):
+            # the frontend returns the value as a string of comma seperated values
+            currently_selected_values = kwargs["value"].split(",")
+        elif type(kwargs["value"]) == type([]):
+            currently_selected_values = kwargs["value"]
+        else:
+            raise "multi select current value seems corrupted"
+
+        with self.doc.select(
+            ("name", "new_value"),
+            ("id", key),
+            ("hx-post", f"/set_component_value?component_id={key}"),
+            ("multiple", ""),
+            # transform the multiselect value into a list of selected indexes like "1,2,7"
+            # ("hx-vals", "js:{"+key+" : "+js_to_get_all_select_values+"}"),
+            ("hx-trigger", "focusout"),
+        ):
+            for value in label:
+                assert not "," in value, "multiselect options can't contain commas"
+                with self.tag(
+                    "option",
+                    ("value", value),
+                    ("selected", "") if value in currently_selected_values else "",
+                ):
                     self.text(value)
-        html = self.return_old_doc_and_init_new()
-        return dict(
-            label=html, component_type="TextInput", default_value=default_value, key=key
-        )
+
+        return lambda x: [x] if type(x) == type("") else x
+
+    @component_wrapper
+    def multi_dropdown(
+        self, label: List[str], default_value: List[int] = [], key: str = None, **kwargs
+    ) -> List[int]:
+        with self.tag(
+            "form",
+            ("id", key),
+            ("hx-post", f"/set_component_value?component_id={key}"),
+            # ("hx-trigger", "click from:input[type=checkbox]"),
+        ):
+            with self.tag(
+                "details",
+                ("class", "dropdown"),
+                ("name", "new_value"),
+                ("multiple", ""),
+            ):
+                with self.tag("summary", ("style", "overflow:hidden;")):
+                    for v in kwargs["value"]:
+                        with self.tag("kbd"):
+                            self.text(v)
+                with self.tag("ul"):
+                    with self.tag("li"):
+                        for option in label:
+                            with self.tag("label"):
+                                checked = (
+                                    ("checked", "")
+                                    if option in kwargs["value"]
+                                    else ("not_checked", "")
+                                )
+                                self.doc.input(
+                                    ("name", option),
+                                    ("type", "checkbox"),
+                                    ("value", option),
+                                    checked,
+                                )
+                                self.text(option)
+                    with self.tag("button", ("type", "submit")):
+                        self.text("submit")
+        return lambda x: list(x.keys()) if type(x) == type({}) else x
 
     @component_wrapper
     def slider(
         self,
         label: str,
         minValue: int,
         maxValue: int,
-        default_value: int,
+        default_value: int = None,
         key: str = None,
+        **kwargs,
     ) -> str:
         """ """
-        if not key:
-            key = label
-
-        kwargs = {
-            "minValue": minValue,
-            "maxValue": maxValue,
-        }
-
-        component_attr = self.get_components().get(key, OrderedDict())
-        component_key = key
+        with self.tag("label", ("for", key)):
+            self.text(label)
         with self.tag(
             "input",
-            ("name", component_key),
+            ("name", "new_value"),
+            ("id", key),
             ("type", "range"),
-            ("value", component_attr.get("current_value", "")),
-            ("min", component_attr.get("minValue", 0)),
-            ("max", component_attr.get("maxValue", 100)),
-            ("hx-post", f"/value_changed/{component_key}"),
-        ):
-            self.text("")
-        html = self.return_old_doc_and_init_new()
-        return dict(
-            label=html,
-            component_type="Slider",
-            default_value=default_value,
-            key=key,
-            **kwargs,
-        )
+            ("value", str(kwargs["value"])),
+            ("min", minValue),
+            ("max", maxValue),
+            ("hx-post", f"/set_component_value?component_id={key}"),
+        ):
+            pass
 
     @component_wrapper
     def nav(
         self,
-        label: list[str],
-        default_value,
+        label: List[str],
         key,
+        default_value=None,
+        **kwargs,
     ):
-        if not key:
-            key = label
-        kwargs = {}
-        component_attr = self.get_components().get(key, OrderedDict())
-        component_value = component_attr.get('current_value', False)
-        component_key = key
-        with self.tag("ul"):
-            for item in label:
-                color = "grey" if component_value == item else ""
-                with self.tag(
-                    "li",
-                ):
-                    with self.tag(
-                        "a",
-                        ("href", "#"),
-                        ('test', item),
-                        ('style', f'color:{color}'),
-                        # changing nav is currently not supported because the label isn' part of the refresh check
-                        (
-                            "hx-post",
-                            f"/value_changed/{component_key}?{component_key}={item}",
-                        ),
-                    ):
-                        self.text(str(item))
-        html = self.return_old_doc_and_init_new()
-        return dict(
-            label=html,
-            component_type="Nav",
-            default_value=default_value,
-            key=key,
-            **kwargs,
-        )
+        hyperscript = f"""
+        on load log #hs-nav then 
+        if #nav-content in #hs-nav exists
+            remove #nav-content in #hs-nav
+        end then
+        remove @_ from #nav-content
+        put me into #hs-nav then
+        set @style to display:block
+                """
+
+        with self.tag(
+            "header",
+            ("id", "nav-content"),
+            ("_", hyperscript),
+            (
+                "style",
+                "display:none",
+            ),  # so when this is first inserted the visitors screen doesn't jump
+            ("visibility", "hidden"),
+        ):
+            with self.tag(
+                "nav",
+            ):
+                with self.tag("ul"):
+                    for item in label:
+                        if type(item) == type(lambda x: x):
+                            # handle functions
+                            item()
+
+                        elif type(item) == type(""):
+                            # handle string navs
+                            color = "grey" if kwargs["value"] == item else ""
+                            with self.tag(
+                                "li",
+                                ("hx-trigger", "click"),
+                                (
+                                    "hx-post",
+                                    f"/set_component_value/?component_id={key}&new_value={item}",
+                                ),
+                                ("hx-swap", "none"),
+                            ):
+                                with self.tag(
+                                    "a",
+                                    # ("style", f"color:{color}"),
+                                ):
+                                    self.text(str(item))
 
     @component_wrapper
-    def pyplot(self, fig, key: str = None) -> None:
+    def pyplot(self, fig, height="200px", key: str = None, **kwargs) -> None:
         """Displays matplotlib plot to user
-
         Args:
             fig (matplotlib.figure.Figure): label to display to user describing the text input
         Returns:
             str: text inputted by user
-
-
         Example:
             import matplotlib.pyplot as plt
             import numpy as np
             x = np.arange(0,4*np.pi,0.1)   # start,stop,step
             y = np.sin(x) * float(sine_height)
             fig, ax = plt.subplots()
             ax.plot(x,y)
@@ -297,51 +364,92 @@
         base64_data = b64encode(stringIObytes.read())
         base64_data = base64_data.decode("utf-8")
 
         with self.tag(
             "img",
             ("src", f"data:image/png;base64,{base64_data}"),
             ("alt", "Graph"),
+            (
+                "height",
+                height,
+            ),  # we set the height manually so swapping images doesn't cause a page jump (due to size 100 -> 0 -> 100)
         ):
-            self.text("")
-        html = self.return_old_doc_and_init_new()
-        return dict(label=html, component_type="Image", default_value=None, key=key)
+            pass
 
     @component_wrapper
     def checkbox(
         self,
         label: str,
         default_value: bool = False,
         key: str = None,
+        **kwargs,
     ) -> str:
         """ """
-        if not key:
-            key = label
-
-        component_attr = self.get_components().get(key, OrderedDict())
-        component_value = component_attr.get('current_value', default_value)
-        component_key = key
-        with self.tag("label",
-            ('for', component_key)
+        bool_checker_fromat_fn = (
+            lambda user_checkbox_value: user_checkbox_value == "True"
+        )
+        value = bool_checker_fromat_fn(kwargs["value"])
+        with self.tag("label", ("for", key)):
+            with self.tag(
+                "input",
+                ("id", key),
+                ("type", "checkbox"),
+                (
+                    "checked" if value else "notchecked",
+                    "",
+                ),
+                # annoyingly a blank checkbox is not sent back in a submit event,
+                # so we attach the state of the checkbox here
+                # https://htmx.org/attributes/hx-vals/, https://github.com/bigskysoftware/htmx/issues/894
+                # ("hx-vals", "js:{" + key + ": event.srcElement.checked}"),
+                # ("hx-post", f"/set_component_value?component_id={key}"),
+                (
+                    "hx-post",
+                    f"/set_component_value/?component_id={key}&new_value={not value}",
+                ),
             ):
+                pass
+            self.text(label)
+        return bool_checker_fromat_fn
+
+    @component_wrapper
+    def button(
+        self,
+        label: str,
+        default_value: bool = False,
+        key: str = None,
+        full_width: bool = False,
+        **kwargs,
+    ) -> bool:
+        """ """
+        with self.tag(
+            "button",
+            ("id", key),
+            ("type", "submit") if full_width else ("type", "button"),
+            ("hx-trigger", "click"),
+            ("hx-post", f"/set_component_value/?component_id={key}&new_value=true"),
+            ("hx-swap", "none"),
+        ):
             self.text(label)
-        print('component_value ', component_value)
+        cherrypy.session[key] = False
+        return lambda s: True if s in ["True", "true", True] else False
+
+    def grid(self, *args, **kwargs):
+        return self.tag("div", ("class", "grid"), *args, **kwargs)
+
+    def write_dataframe(self, df, key, striped=False, **kwargs) -> None:
+        """Writes a dataframe to the
+
+        Args:
+            df (pd.DataFrame): Dataframe to write to the web front end
+            key (str): Must be unique within the app. Used to reference the dataframe in the front end
+        """
         with self.tag(
-            "input",
-            ("id",component_key ),
-            # ("name", component_key),
-            ("type", "checkbox"),
-            ( 'checked' if component_value in ["true", True, 1, "1"] else 'notchecked', ''),
-            # annoyingly a blank checkbox is not sent back in a submit event, 
-            # so we attach the state of the checkbox here
-            # https://htmx.org/attributes/hx-vals/, https://github.com/bigskysoftware/htmx/issues/894
-            ("hx-vals", 'js:{'+component_key+': event.srcElement.checked}'),
-            ("hx-post", f"/value_changed/{component_key}"),
-        ):
-            self.text("")
-        html = self.return_old_doc_and_init_new()
-        return dict(
-            label=html,
-            component_type="Slider",
-            default_value=default_value,
-            key=key,
-        )
+            "div",
+            klass="overflow-auto",
+        ):
+            html = (
+                df.to_html(classes="", border="", justify="unset")
+                .replace('style="text-align: unset;"', "")
+                .replace('class="dataframe"', f'class="{striped}"')
+            )
+            self.doc.asis(html)
```

