# Comparing `tmp/pytest_splunk_addon_ui_smartx-3.1.0.tar.gz` & `tmp/pytest_splunk_addon_ui_smartx-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_splunk_addon_ui_smartx-3.1.0.tar", max compression
+gzip compressed data, was "pytest_splunk_addon_ui_smartx-3.1.1.tar", max compression
```

## Comparing `pytest_splunk_addon_ui_smartx-3.1.0.tar` & `pytest_splunk_addon_ui_smartx-3.1.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0    11341 2024-05-09 10:47:43.832617 pytest_splunk_addon_ui_smartx-3.1.0/LICENSE
--rw-r--r--   0        0        0     1782 2024-05-09 10:48:15.605106 pytest_splunk_addon_ui_smartx-3.1.0/pyproject.toml
--rw-r--r--   0        0        0      668 2024-05-09 10:48:15.601106 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/__init__.py
--rw-r--r--   0        0        0     2984 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/__init__.py
--rw-r--r--   0        0        0      579 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/__init__.py
--rw-r--r--   0        0        0     6774 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/account_select.py
--rw-r--r--   0        0        0     1766 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/action_controls.py
--rw-r--r--   0        0        0    10881 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/alert_base_component.py
--rw-r--r--   0        0        0     1971 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/alert_base_control.py
--rw-r--r--   0        0        0     1194 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/button.py
--rw-r--r--   0        0        0     3054 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/checkbox.py
--rw-r--r--   0        0        0     3000 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/dropdown.py
--rw-r--r--   0        0        0     1572 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/searchbox.py
--rw-r--r--   0        0        0     1753 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/single_select.py
--rw-r--r--   0        0        0    19489 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/table.py
--rw-r--r--   0        0        0     2808 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/textbox.py
--rw-r--r--   0        0        0     1688 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/toggle.py
--rw-r--r--   0        0        0     7200 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/backend_confs.py
--rw-r--r--   0        0        0    23257 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/base_test.py
--rw-r--r--   0        0        0      579 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/__init__.py
--rw-r--r--   0        0        0    10944 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/base_component.py
--rw-r--r--   0        0        0      816 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/conf_table.py
--rw-r--r--   0        0        0      579 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/__init__.py
--rw-r--r--   0        0        0     2537 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/base_control.py
--rw-r--r--   0        0        0     1179 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/button.py
--rw-r--r--   0        0        0     3217 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/checkbox.py
--rw-r--r--   0        0        0     3012 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/learn_more.py
--rw-r--r--   0        0        0     1979 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/message.py
--rw-r--r--   0        0        0     7094 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/multi_select.py
--rw-r--r--   0        0        0     3079 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/oauth_select.py
--rw-r--r--   0        0        0    13813 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/single_select.py
--rw-r--r--   0        0        0     2718 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/textarea.py
--rw-r--r--   0        0        0     3119 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/textbox.py
--rw-r--r--   0        0        0     2547 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/toggle.py
--rw-r--r--   0        0        0     8201 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/dropdown.py
--rw-r--r--   0        0        0     4941 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/entity.py
--rw-r--r--   0        0        0     3678 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/input_table.py
--rw-r--r--   0        0        0     1887 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/login.py
--rw-r--r--   0        0        0     5142 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/message_tray.py
--rw-r--r--   0        0        0    23658 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/table.py
--rw-r--r--   0        0        0     1673 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/tabs.py
--rw-r--r--   0        0        0      579 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/pages/__init__.py
--rw-r--r--   0        0        0     2824 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/pages/logging.py
--rw-r--r--   0        0        0     1075 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/pages/login.py
--rw-r--r--   0        0        0     1633 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/pages/page.py
--rw-r--r--   0        0        0     4659 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/pages/proxy.py
--rw-r--r--   0        0        0    10257 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/plugin.py
--rw-r--r--   0        0        0     1156 2024-05-09 10:47:43.836617 pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/utils.py
--rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 pytest_splunk_addon_ui_smartx-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11341 2024-05-09 14:13:38.538713 pytest_splunk_addon_ui_smartx-3.1.1/LICENSE
+-rw-r--r--   0        0        0     1782 2024-05-09 14:14:18.162517 pytest_splunk_addon_ui_smartx-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0      668 2024-05-09 14:14:18.158517 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/__init__.py
+-rw-r--r--   0        0        0     2984 2024-05-09 14:13:38.542713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/alert_actions/__init__.py
+-rw-r--r--   0        0        0      579 2024-05-09 14:13:38.542713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/alert_actions/components/__init__.py
+-rw-r--r--   0        0        0     6774 2024-05-09 14:13:38.542713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/alert_actions/components/account_select.py
+-rw-r--r--   0        0        0     1766 2024-05-09 14:13:38.542713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/alert_actions/components/action_controls.py
+-rw-r--r--   0        0        0    10881 2024-05-09 14:13:38.542713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/alert_actions/components/alert_base_component.py
+-rw-r--r--   0        0        0     1971 2024-05-09 14:13:38.542713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/alert_actions/components/alert_base_control.py
+-rw-r--r--   0        0        0     1194 2024-05-09 14:13:38.542713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/alert_actions/components/button.py
+-rw-r--r--   0        0        0     3054 2024-05-09 14:13:38.542713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/alert_actions/components/checkbox.py
+-rw-r--r--   0        0        0     3000 2024-05-09 14:13:38.542713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/alert_actions/components/dropdown.py
+-rw-r--r--   0        0        0     1572 2024-05-09 14:13:38.542713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/alert_actions/components/searchbox.py
+-rw-r--r--   0        0        0     1753 2024-05-09 14:13:38.542713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/alert_actions/components/single_select.py
+-rw-r--r--   0        0        0    19489 2024-05-09 14:13:38.546713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/alert_actions/components/table.py
+-rw-r--r--   0        0        0     2808 2024-05-09 14:13:38.546713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/alert_actions/components/textbox.py
+-rw-r--r--   0        0        0     1688 2024-05-09 14:13:38.546713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/alert_actions/components/toggle.py
+-rw-r--r--   0        0        0     7200 2024-05-09 14:13:38.546713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/backend_confs.py
+-rw-r--r--   0        0        0    23257 2024-05-09 14:13:38.546713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/base_test.py
+-rw-r--r--   0        0        0      579 2024-05-09 14:13:38.546713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/__init__.py
+-rw-r--r--   0        0        0    10944 2024-05-09 14:13:38.546713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/base_component.py
+-rw-r--r--   0        0        0      816 2024-05-09 14:13:38.546713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/conf_table.py
+-rw-r--r--   0        0        0      579 2024-05-09 14:13:38.546713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/controls/__init__.py
+-rw-r--r--   0        0        0     2537 2024-05-09 14:13:38.546713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/controls/base_control.py
+-rw-r--r--   0        0        0     1179 2024-05-09 14:13:38.546713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/controls/button.py
+-rw-r--r--   0        0        0     3217 2024-05-09 14:13:38.546713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/controls/checkbox.py
+-rw-r--r--   0        0        0     3012 2024-05-09 14:13:38.546713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/controls/learn_more.py
+-rw-r--r--   0        0        0     2112 2024-05-09 14:13:38.546713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/controls/message.py
+-rw-r--r--   0        0        0     7288 2024-05-09 14:13:38.546713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/controls/multi_select.py
+-rw-r--r--   0        0        0     3079 2024-05-09 14:13:38.546713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/controls/oauth_select.py
+-rw-r--r--   0        0        0    13813 2024-05-09 14:13:38.546713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/controls/single_select.py
+-rw-r--r--   0        0        0     2718 2024-05-09 14:13:38.546713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/controls/textarea.py
+-rw-r--r--   0        0        0     3119 2024-05-09 14:13:38.546713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/controls/textbox.py
+-rw-r--r--   0        0        0     2547 2024-05-09 14:13:38.546713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/controls/toggle.py
+-rw-r--r--   0        0        0     8201 2024-05-09 14:13:38.546713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/dropdown.py
+-rw-r--r--   0        0        0     4941 2024-05-09 14:13:38.546713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/entity.py
+-rw-r--r--   0        0        0     3678 2024-05-09 14:13:38.546713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/input_table.py
+-rw-r--r--   0        0        0     1887 2024-05-09 14:13:38.546713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/login.py
+-rw-r--r--   0        0        0     5142 2024-05-09 14:13:38.546713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/message_tray.py
+-rw-r--r--   0        0        0    23658 2024-05-09 14:13:38.546713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/table.py
+-rw-r--r--   0        0        0     1673 2024-05-09 14:13:38.546713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/tabs.py
+-rw-r--r--   0        0        0      579 2024-05-09 14:13:38.546713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/pages/__init__.py
+-rw-r--r--   0        0        0     2824 2024-05-09 14:13:38.546713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/pages/logging.py
+-rw-r--r--   0        0        0     1075 2024-05-09 14:13:38.546713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/pages/login.py
+-rw-r--r--   0        0        0     1633 2024-05-09 14:13:38.546713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/pages/page.py
+-rw-r--r--   0        0        0     4659 2024-05-09 14:13:38.546713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/pages/proxy.py
+-rw-r--r--   0        0        0    10257 2024-05-09 14:13:38.546713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/plugin.py
+-rw-r--r--   0        0        0     1156 2024-05-09 14:13:38.546713 pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/utils.py
+-rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 pytest_splunk_addon_ui_smartx-3.1.1/PKG-INFO
```

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/LICENSE` & `pytest_splunk_addon_ui_smartx-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pyproject.toml` & `pytest_splunk_addon_ui_smartx-3.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         "Programming Language :: Python :: 3.7",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: Apache Software License",
 ]
 packages = [
         {include = "pytest_splunk_addon_ui_smartx/**/*.py"},
 ]
-version = "3.1.0"
+version = "3.1.1"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 pytest-html = "*"
 urllib3 = "^1.21.1"
 selenium = "*"
 webdriver-manager = "*"
```

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/__init__.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 from . import components, pages
 from .components import controls
 
-__version__ = "3.1.0"
+__version__ = "3.1.1"
```

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/__init__.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/alert_actions/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/__init__.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/alert_actions/components/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/account_select.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/alert_actions/components/account_select.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/action_controls.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/alert_actions/components/action_controls.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/alert_base_component.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/alert_actions/components/alert_base_component.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/alert_base_control.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/alert_actions/components/alert_base_control.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/button.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/alert_actions/components/button.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/checkbox.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/alert_actions/components/checkbox.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/dropdown.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/alert_actions/components/dropdown.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/searchbox.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/alert_actions/components/searchbox.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/single_select.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/alert_actions/components/single_select.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/table.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/alert_actions/components/table.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/textbox.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/alert_actions/components/textbox.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/alert_actions/components/toggle.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/alert_actions/components/toggle.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/backend_confs.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/backend_confs.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/base_test.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/base_test.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/__init__.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/base_component.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/base_component.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/conf_table.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/conf_table.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/__init__.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/controls/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/base_control.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/controls/base_control.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/button.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/controls/button.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/checkbox.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/controls/checkbox.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/learn_more.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/controls/learn_more.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/message.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/controls/message.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,19 @@
         """
         :param browser: The selenium webdriver
         :param container: The locator of the container where the control is located in.
         """
         super().__init__(browser, container)
         self.elements.update(
             {
-                "msg_text": Selector(select=container.select + '[data-test="message"]'),
+                # changes w.r.t. splunk-ui 4.30.0
+                "msg_text": Selector(
+                    select=container.select
+                    + '[data-test="message"] div[data-test="content"]'
+                ),
             }
         )
 
     def get_msg(self):
         """
         Returns the error message
             :return: Str error message
```

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/multi_select.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/controls/multi_select.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,21 +37,25 @@
 
         root_selector = container.select + ' [data-test="multiselect"]'
         self.elements.update({"root": Selector(select=root_selector)})
 
         self.elements.update(
             {
                 "selected": Selector(
-                    select=root_selector + ' [data-test="selected-option"]'
+                    # changes w.r.t. splunk-ui 4.30.0
+                    select=root_selector
+                    + ' [data-test="selected-option"] div[data-test="label"]'
                 ),
                 """
                 Click on selected element deselects it
                 """
                 "deselect": Selector(
-                    select=root_selector + ' [data-test="selected-option"]'
+                    # changes w.r.t. splunk-ui 4.30.0
+                    select=root_selector
+                    + ' [data-test="selected-option"] div[data-test="label"]'
                 ),
                 "input": Selector(select=root_selector + ' [data-test="textbox"]'),
             }
         )
 
     def search(self, value):
         """
```

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/oauth_select.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/controls/oauth_select.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/single_select.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/controls/single_select.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/textarea.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/controls/textarea.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/textbox.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/controls/textbox.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/controls/toggle.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/controls/toggle.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/dropdown.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/dropdown.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/entity.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/entity.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/input_table.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/input_table.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/login.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/login.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/message_tray.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/message_tray.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/table.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/table.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/components/tabs.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/components/tabs.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/pages/__init__.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/pages/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/pages/logging.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/pages/logging.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/pages/login.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/pages/login.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/pages/page.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/pages/page.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/pages/proxy.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/pages/proxy.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/plugin.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/pytest_splunk_addon_ui_smartx/utils.py` & `pytest_splunk_addon_ui_smartx-3.1.1/pytest_splunk_addon_ui_smartx/utils.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon_ui_smartx-3.1.0/PKG-INFO` & `pytest_splunk_addon_ui_smartx-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-splunk-addon-ui-smartx
-Version: 3.1.0
+Version: 3.1.1
 Summary: Library to support testing Splunk Add-on UX
 License: Apache-2.0
 Author: Splunk
 Author-email: addonfactory@splunk.com
 Requires-Python: >=3.7,<4.0
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
```

