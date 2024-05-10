# Comparing `tmp/vigilant_kit-1.4.3.tar.gz` & `tmp/vigilant_kit-1.4.4.tar.gz`

## Comparing `vigilant_kit-1.4.3.tar` & `vigilant_kit-1.4.4.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 vigilant_kit-1.4.3/CHANGELOG.md
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 vigilant_kit-1.4.3/vgl_config.yaml.example
--rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 vigilant_kit-1.4.3/bin/doc_generator.py
--rw-r--r--   0        0        0    31729 2020-02-02 00:00:00.000000 vigilant_kit-1.4.3/docs/actions.md
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 vigilant_kit-1.4.3/docs/browser_options.md
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 vigilant_kit-1.4.3/docs/changelog_logic.md
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 vigilant_kit-1.4.3/docs/configuration.md
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 vigilant_kit-1.4.3/docs/native_selenium.md
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 vigilant_kit-1.4.3/docs/selenium_install.md
--rw-r--r--   0        0        0    11059 2020-02-02 00:00:00.000000 vigilant_kit-1.4.3/docs/tutorial_pytest.md
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 vigilant_kit-1.4.3/docs/vigilant_pytest.md
--rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 vigilant_kit-1.4.3/docs/vigilant_unittest.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.4.3/src/vigilant/__init__.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vigilant_kit-1.4.3/src/vigilant/logger.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.4.3/src/vigilant/actions/__init__.py
--rw-r--r--   0        0        0     6495 2020-02-02 00:00:00.000000 vigilant_kit-1.4.3/src/vigilant/actions/assertions.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 vigilant_kit-1.4.3/src/vigilant/actions/data_saver.py
--rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 vigilant_kit-1.4.3/src/vigilant/actions/finder.py
--rw-r--r--   0        0        0    15038 2020-02-02 00:00:00.000000 vigilant_kit-1.4.3/src/vigilant/actions/vigilant_actions.py
--rw-r--r--   0        0        0     5064 2020-02-02 00:00:00.000000 vigilant_kit-1.4.3/src/vigilant/actions/waiter.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 vigilant_kit-1.4.3/src/vigilant/driver/__init__.py
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 vigilant_kit-1.4.3/src/vigilant/driver/vigilant_driver.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vigilant_kit-1.4.3/.gitignore
--rw-r--r--   0        0        0    35125 2020-02-02 00:00:00.000000 vigilant_kit-1.4.3/LICENSE
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 vigilant_kit-1.4.3/README.md
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 vigilant_kit-1.4.3/pyproject.toml
--rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 vigilant_kit-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/CHANGELOG.md
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/vgl_config.yaml.example
+-rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/bin/doc_generator.py
+-rw-r--r--   0        0        0    31729 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/docs/actions.md
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/docs/browser_options.md
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/docs/changelog_logic.md
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/docs/configuration.md
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/docs/native_selenium.md
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/docs/selenium_install.md
+-rw-r--r--   0        0        0    11059 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/docs/tutorial_pytest.md
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/docs/vigilant_pytest.md
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/docs/vigilant_unittest.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/src/vigilant/__init__.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/src/vigilant/logger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/src/vigilant/actions/__init__.py
+-rw-r--r--   0        0        0     6495 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/src/vigilant/actions/assertions.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/src/vigilant/actions/data_saver.py
+-rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/src/vigilant/actions/finder.py
+-rw-r--r--   0        0        0    15142 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/src/vigilant/actions/vigilant_actions.py
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/src/vigilant/actions/vigilant_pdf.py
+-rw-r--r--   0        0        0     5064 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/src/vigilant/actions/waiter.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/src/vigilant/driver/__init__.py
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/src/vigilant/driver/vigilant_driver.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/.gitignore
+-rw-r--r--   0        0        0    35125 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/LICENSE
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/README.md
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/pyproject.toml
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/PKG-INFO
```

### Comparing `vigilant_kit-1.4.3/bin/doc_generator.py` & `vigilant_kit-1.4.4/bin/doc_generator.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.4.3/docs/actions.md` & `vigilant_kit-1.4.4/docs/actions.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.4.3/docs/browser_options.md` & `vigilant_kit-1.4.4/docs/browser_options.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.4.3/docs/changelog_logic.md` & `vigilant_kit-1.4.4/docs/changelog_logic.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.4.3/docs/configuration.md` & `vigilant_kit-1.4.4/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.4.3/docs/native_selenium.md` & `vigilant_kit-1.4.4/docs/native_selenium.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.4.3/docs/selenium_install.md` & `vigilant_kit-1.4.4/docs/selenium_install.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.4.3/docs/tutorial_pytest.md` & `vigilant_kit-1.4.4/docs/tutorial_pytest.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.4.3/docs/vigilant_pytest.md` & `vigilant_kit-1.4.4/docs/vigilant_pytest.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.4.3/docs/vigilant_unittest.md` & `vigilant_kit-1.4.4/docs/vigilant_unittest.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.4.3/src/vigilant/actions/assertions.py` & `vigilant_kit-1.4.4/src/vigilant/actions/assertions.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.4.3/src/vigilant/actions/finder.py` & `vigilant_kit-1.4.4/src/vigilant/actions/finder.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.4.3/src/vigilant/actions/vigilant_actions.py` & `vigilant_kit-1.4.4/src/vigilant/actions/vigilant_actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.common.by import By
 
 from vigilant.actions.assertions import Assertions
 from vigilant.actions.finder import Finder
 from vigilant.actions.waiter import Waiter
 from vigilant.actions.data_saver import DataSaver
+from vigilant.actions.vigilant_pdf import VigilantPDF
 from vigilant.logger import logger as log
 
 
 def get_base_url() -> str:
     """
     Get the base URL from the environment variable 'BASE_URL'.
 
@@ -31,14 +32,15 @@
 
     def __init__(self, driver):
         self.driver: Remote = driver
         self.assertions: Assertions = Assertions(self.driver)
         self.finder: Finder = Finder(self.driver)
         self.waiter: Waiter = Waiter(self.driver, self.finder)
         self.data_saver: DataSaver = DataSaver()
+        self.vgl_pdf: VigilantPDF = VigilantPDF()
 
     def get_relative_page(self, url):
         """
         Opens the page by the URL relative to the one set in the BASE_URL configuration variable.
 
         :param url: A path to the page relative to the BASE_URL
         :return: self
```

### Comparing `vigilant_kit-1.4.3/src/vigilant/actions/waiter.py` & `vigilant_kit-1.4.4/src/vigilant/actions/waiter.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.4.3/src/vigilant/driver/__init__.py` & `vigilant_kit-1.4.4/src/vigilant/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.4.3/src/vigilant/driver/vigilant_driver.py` & `vigilant_kit-1.4.4/src/vigilant/driver/vigilant_driver.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.4.3/.gitignore` & `vigilant_kit-1.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.4.3/LICENSE` & `vigilant_kit-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.4.3/README.md` & `vigilant_kit-1.4.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 
 
 ## What included?
 _Wait for condition, Act by Interaction, Assert the result._
 
 
 ### **Actions** 
-   - `click()` - click on element when it visible and scrolled in to the view;
-   - `scroll_to()` - easy scroll to the element when necessary;
-   - `fill_form()` - fill form with many fields without repetitive;
-   - `switch_to_window()` - work with multiply browser windows without any issues;
+   - `click()`
+   - `scroll_to()`
+   - `fill_form()`
+   - `switch_to_window()`
    - ...
 
 ### **Waiters for condition** 
 
    - `wait_for_element_to_be_visible()`
    - `wait_for_element_to_be_clickable()`
    - `wait_for_text_to_be_present_in_element()`
@@ -43,14 +43,22 @@
 ### **Scrappers**
 Minimal required methods for scrapping some data:
   - `get_text_from_element()`
   - `get_attribute_from_element()`
   - `get_cookie()`
   - `save_data_to_txt()`
 
+### **Test PDF**
+You're testing some eCommerce project, and you need to check your PDF invoice file? No problem!
+   - `find_pdf_file()`,
+   - `assert_strings_in_pdf()`,
+   - `assert_strings_not_in_pdf()`,
+   - `find_file_and_assert_strings_are_in()`,
+   - ...
+
 And much more! Check list of all available - [Actions](docs/actions.md)
 
 
 ## Extending Functionality
 If you need something that is not covered in this library, you still have access to all native `Selenium WebDriver` 
 methods. You can create your own methods or use native `WebDriver` methods and share them on one browser session.
```

### Comparing `vigilant_kit-1.4.3/pyproject.toml` & `vigilant_kit-1.4.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "vigilant_kit"
-version = "1.4.3"
+version = "1.4.4"
 authors = [
   { name="Pelykh Ivan", email="ivan.pelykh@protonmail.com" },
 ]
 description = "Library that makes functional testing with Selenium WebDriver fast and easy. "
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
     "selenium",
-    "python-dotenv",
-    "requests",
-    "psutil",
-    "pyyaml"
+    "pyyaml",
+    "PyMuPDF"
 ]
 
 keywords = ["testing", "selenium", "webdriver", "pytest", "unittest", "bdd", "tdd", "functional", "functional-testing"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/vigilant"]
```

### Comparing `vigilant_kit-1.4.3/PKG-INFO` & `vigilant_kit-1.4.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.3
 Name: vigilant_kit
-Version: 1.4.3
+Version: 1.4.4
 Summary: Library that makes functional testing with Selenium WebDriver fast and easy. 
 Project-URL: Homepage, https://github.com/ivpel/vigilant
 Project-URL: Bug Tracker, https://github.com/ivpel/vigilant/issues
 Author-email: Pelykh Ivan <ivan.pelykh@protonmail.com>
 License-File: LICENSE
 Keywords: bdd,functional,functional-testing,pytest,selenium,tdd,testing,unittest,webdriver
 Requires-Python: >=3.7
-Requires-Dist: psutil
-Requires-Dist: python-dotenv
+Requires-Dist: pymupdf
 Requires-Dist: pyyaml
-Requires-Dist: requests
 Requires-Dist: selenium
 Description-Content-Type: text/markdown
 
 # Vigilant Kit
 **Vigilant** is a set of tools designed to help write and run robust functional tests using Selenium WebDriver. With 
 **Vigilant**, you can start writing complex test cases in a minute.
 
@@ -28,18 +26,18 @@
 
 
 ## What included?
 _Wait for condition, Act by Interaction, Assert the result._
 
 
 ### **Actions** 
-   - `click()` - click on element when it visible and scrolled in to the view;
-   - `scroll_to()` - easy scroll to the element when necessary;
-   - `fill_form()` - fill form with many fields without repetitive;
-   - `switch_to_window()` - work with multiply browser windows without any issues;
+   - `click()`
+   - `scroll_to()`
+   - `fill_form()`
+   - `switch_to_window()`
    - ...
 
 ### **Waiters for condition** 
 
    - `wait_for_element_to_be_visible()`
    - `wait_for_element_to_be_clickable()`
    - `wait_for_text_to_be_present_in_element()`
@@ -60,14 +58,22 @@
 ### **Scrappers**
 Minimal required methods for scrapping some data:
   - `get_text_from_element()`
   - `get_attribute_from_element()`
   - `get_cookie()`
   - `save_data_to_txt()`
 
+### **Test PDF**
+You're testing some eCommerce project, and you need to check your PDF invoice file? No problem!
+   - `find_pdf_file()`,
+   - `assert_strings_in_pdf()`,
+   - `assert_strings_not_in_pdf()`,
+   - `find_file_and_assert_strings_are_in()`,
+   - ...
+
 And much more! Check list of all available - [Actions](docs/actions.md)
 
 
 ## Extending Functionality
 If you need something that is not covered in this library, you still have access to all native `Selenium WebDriver` 
 methods. You can create your own methods or use native `WebDriver` methods and share them on one browser session.
```

