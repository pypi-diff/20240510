# Comparing `tmp/pydboat-1.0.1.tar.gz` & `tmp/pydboat-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydboat-1.0.1.tar", last modified: Thu May  9 06:03:26 2024, max compression
+gzip compressed data, was "pydboat-1.0.2.tar", last modified: Fri May 10 02:01:13 2024, max compression
```

## Comparing `pydboat-1.0.1.tar` & `pydboat-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 06:03:26.102625 pydboat-1.0.1/
--rw-rw-rw-   0        0        0     1060 2024-05-09 03:50:44.000000 pydboat-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     1038 2024-05-09 06:03:26.100067 pydboat-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        8 2024-05-08 11:09:53.000000 pydboat-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 06:03:26.099067 pydboat-1.0.1/pydboat.egg-info/
--rw-rw-rw-   0        0        0     1038 2024-05-09 06:03:25.000000 pydboat-1.0.1/pydboat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2024-05-09 06:03:26.000000 pydboat-1.0.1/pydboat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 06:03:25.000000 pydboat-1.0.1/pydboat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2024-05-09 06:03:25.000000 pydboat-1.0.1/pydboat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 06:03:26.102625 pydboat-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     4659 2024-05-09 06:03:11.000000 pydboat-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-09 06:03:26.099067 pydboat-1.0.1/src/
--rw-rw-rw-   0        0        0        0 2024-05-09 05:07:49.000000 pydboat-1.0.1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 06:03:26.100067 pydboat-1.0.1/src/resource/
--rw-rw-rw-   0        0        0        0 2024-05-09 05:03:57.000000 pydboat-1.0.1/src/resource/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 02:01:13.790476 pydboat-1.0.2/
+-rw-rw-rw-   0        0        0     1060 2024-05-09 03:50:44.000000 pydboat-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1038 2024-05-10 02:01:13.787997 pydboat-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        8 2024-05-08 11:09:53.000000 pydboat-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 02:01:13.786993 pydboat-1.0.2/pydboat.egg-info/
+-rw-rw-rw-   0        0        0     1038 2024-05-10 02:01:13.000000 pydboat-1.0.2/pydboat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2024-05-10 02:01:13.000000 pydboat-1.0.2/pydboat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 02:01:13.000000 pydboat-1.0.2/pydboat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2024-05-10 02:01:13.000000 pydboat-1.0.2/pydboat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 02:01:13.790476 pydboat-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     4649 2024-05-10 02:01:03.000000 pydboat-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 02:01:13.786993 pydboat-1.0.2/src/
+-rw-rw-rw-   0        0        0        0 2024-05-09 05:07:49.000000 pydboat-1.0.2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 02:01:13.787997 pydboat-1.0.2/src/resource/
+-rw-rw-rw-   0        0        0        0 2024-05-09 05:03:57.000000 pydboat-1.0.2/src/resource/__init__.py
```

### Comparing `pydboat-1.0.1/LICENSE` & `pydboat-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydboat-1.0.1/PKG-INFO` & `pydboat-1.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydboat
-Version: 1.0.1
+Version: 1.0.2
 Summary: This is a project template.
 Home-page: https://github.com/dangfugui/pyboat
 Author: fg
 Author-email: dangfugui@163.com
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pydboat-1.0.1/pydboat.egg-info/PKG-INFO` & `pydboat-1.0.2/pydboat.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydboat
-Version: 1.0.1
+Version: 1.0.2
 Summary: This is a project template.
 Home-page: https://github.com/dangfugui/pyboat
 Author: fg
 Author-email: dangfugui@163.com
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pydboat-1.0.1/setup.py` & `pydboat-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         "Natural Language :: English",
         "Natural Language :: Chinese (Simplified)",
 
     ],
 
     # 如果上传时出现ERROR：The user '' isn't allowed to upload to project ''，换个名字，长一点无所谓，不能跟别人重复
     name="pydboat",
-    version="1.0.1",
+    version="1.0.2",
     author="fg",
     author_email="dangfugui@163.com",
     description="This is a project template.",
     long_description=my_long_description,
 
     # 存放源码的地址，填入gitee的源码网址即可
     url="https://github.com/dangfugui/pyboat",
@@ -79,15 +79,15 @@
     packages=find_packages(),
 
     # README.md文本的格式，如果希望使用markdown语言就需要下面这句话
     long_description_content_type="text/markdown",
 
     # 安装过程中，需要安装的静态文件，如配置文件、service文件、图片等
     data_files=[
-         ("", ["D:\\_File\\code\\github\\pyboat\\src\\resource\\jeecgboot-vue3.zip"]),
+         ("", ["D:\\_File\\code\\github\\pyboat\\src\\resource\\dist.zip"]),
          # ("/usr/lib/systemd/system", ["bin/*.service"]),
                ],
 
     # 希望被打包的文件
     # package_data={
     #     "":["*.txt"],
     #     "bandwidth_reporter":["*.txt"]
```

