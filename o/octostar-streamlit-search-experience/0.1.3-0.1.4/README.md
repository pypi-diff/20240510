# Comparing `tmp/octostar_streamlit_search_experience-0.1.3.tar.gz` & `tmp/octostar_streamlit_search_experience-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octostar_streamlit_search_experience-0.1.3.tar", max compression
+gzip compressed data, was "octostar_streamlit_search_experience-0.1.4.tar", max compression
```

## Comparing `octostar_streamlit_search_experience-0.1.3.tar` & `octostar_streamlit_search_experience-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      769 2024-05-06 21:21:27.822014 octostar_streamlit_search_experience-0.1.3/README.md
--rw-r--r--   0        0        0     3018 2024-05-10 18:50:09.062335 octostar_streamlit_search_experience-0.1.3/octostar_streamlit_search_experience/__init__.py
--rw-r--r--   0        0        0      436 2024-05-06 19:56:14.704927 octostar_streamlit_search_experience-0.1.3/octostar_streamlit_search_experience/frontend/.eslintrc.cjs
--rw-r--r--   0        0        0      253 2024-05-06 19:56:14.705546 octostar_streamlit_search_experience-0.1.3/octostar_streamlit_search_experience/frontend/.gitignore
--rw-r--r--   0        0        0     1300 2024-05-06 19:56:14.705182 octostar_streamlit_search_experience-0.1.3/octostar_streamlit_search_experience/frontend/README.md
--rw-r--r--   0        0        0      429 2024-05-10 21:00:07.222361 octostar_streamlit_search_experience-0.1.3/octostar_streamlit_search_experience/frontend/dist/assets/index-B12znyeL.css
--rw-r--r--   0        0        0   368139 2024-05-10 21:00:07.222430 octostar_streamlit_search_experience-0.1.3/octostar_streamlit_search_experience/frontend/dist/assets/index-DJ3f7eVh.js
--rw-r--r--   0        0        0      466 2024-05-10 21:00:07.222278 octostar_streamlit_search_experience-0.1.3/octostar_streamlit_search_experience/frontend/dist/index.html
--rw-r--r--   0        0        0      366 2024-05-06 19:56:14.705921 octostar_streamlit_search_experience-0.1.3/octostar_streamlit_search_experience/frontend/index.html
--rw-r--r--   0        0        0   131747 2024-05-10 18:26:12.852367 octostar_streamlit_search_experience-0.1.3/octostar_streamlit_search_experience/frontend/package-lock.json
--rw-r--r--   0        0        0      882 2024-05-10 18:26:12.803858 octostar_streamlit_search_experience-0.1.3/octostar_streamlit_search_experience/frontend/package.json
--rw-r--r--   0        0        0     1916 2024-05-10 20:55:21.697320 octostar_streamlit_search_experience-0.1.3/octostar_streamlit_search_experience/frontend/src/App.tsx
--rw-r--r--   0        0        0      472 2024-05-10 20:37:49.870464 octostar_streamlit_search_experience-0.1.3/octostar_streamlit_search_experience/frontend/src/components/Dropzone/Dropzone.module.css
--rw-r--r--   0        0        0     6742 2024-05-10 21:00:04.083424 octostar_streamlit_search_experience-0.1.3/octostar_streamlit_search_experience/frontend/src/components/Dropzone/Dropzone.tsx
--rw-r--r--   0        0        0       33 2024-05-10 02:16:57.058643 octostar_streamlit_search_experience-0.1.3/octostar_streamlit_search_experience/frontend/src/components/SearchExperienceButton/SearchExperienceButton.module.css
--rw-r--r--   0        0        0      716 2024-05-10 02:17:50.306372 octostar_streamlit_search_experience-0.1.3/octostar_streamlit_search_experience/frontend/src/components/SearchExperienceButton/SearchExperienceButton.tsx
--rw-r--r--   0        0        0      215 2024-05-06 20:48:31.521496 octostar_streamlit_search_experience-0.1.3/octostar_streamlit_search_experience/frontend/src/main.tsx
--rw-r--r--   0        0        0      297 2024-05-10 18:41:03.922126 octostar_streamlit_search_experience-0.1.3/octostar_streamlit_search_experience/frontend/src/types.ts
--rw-r--r--   0        0        0       38 2024-05-06 19:56:14.708711 octostar_streamlit_search_experience-0.1.3/octostar_streamlit_search_experience/frontend/src/vite-env.d.ts
--rw-r--r--   0        0        0      605 2024-05-06 19:56:14.709077 octostar_streamlit_search_experience-0.1.3/octostar_streamlit_search_experience/frontend/tsconfig.json
--rw-r--r--   0        0        0      233 2024-05-06 19:56:14.709733 octostar_streamlit_search_experience-0.1.3/octostar_streamlit_search_experience/frontend/tsconfig.node.json
--rw-r--r--   0        0        0      178 2024-05-08 17:55:47.277413 octostar_streamlit_search_experience-0.1.3/octostar_streamlit_search_experience/frontend/vite.config.ts
--rw-r--r--   0        0        0      486 2024-05-10 21:00:35.187679 octostar_streamlit_search_experience-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1522 1970-01-01 00:00:00.000000 octostar_streamlit_search_experience-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      769 2024-05-06 21:21:27.822014 octostar_streamlit_search_experience-0.1.4/README.md
+-rw-r--r--   0        0        0     3018 2024-05-10 18:50:09.062335 octostar_streamlit_search_experience-0.1.4/octostar_streamlit_search_experience/__init__.py
+-rw-r--r--   0        0        0      436 2024-05-06 19:56:14.704927 octostar_streamlit_search_experience-0.1.4/octostar_streamlit_search_experience/frontend/.eslintrc.cjs
+-rw-r--r--   0        0        0      253 2024-05-06 19:56:14.705546 octostar_streamlit_search_experience-0.1.4/octostar_streamlit_search_experience/frontend/.gitignore
+-rw-r--r--   0        0        0     1300 2024-05-06 19:56:14.705182 octostar_streamlit_search_experience-0.1.4/octostar_streamlit_search_experience/frontend/README.md
+-rw-r--r--   0        0        0      429 2024-05-10 21:00:07.222361 octostar_streamlit_search_experience-0.1.4/octostar_streamlit_search_experience/frontend/dist/assets/index-B12znyeL.css
+-rw-r--r--   0        0        0   368139 2024-05-10 21:00:07.222430 octostar_streamlit_search_experience-0.1.4/octostar_streamlit_search_experience/frontend/dist/assets/index-DJ3f7eVh.js
+-rw-r--r--   0        0        0      466 2024-05-10 21:00:07.222278 octostar_streamlit_search_experience-0.1.4/octostar_streamlit_search_experience/frontend/dist/index.html
+-rw-r--r--   0        0        0      366 2024-05-06 19:56:14.705921 octostar_streamlit_search_experience-0.1.4/octostar_streamlit_search_experience/frontend/index.html
+-rw-r--r--   0        0        0   131747 2024-05-10 18:26:12.852367 octostar_streamlit_search_experience-0.1.4/octostar_streamlit_search_experience/frontend/package-lock.json
+-rw-r--r--   0        0        0      882 2024-05-10 18:26:12.803858 octostar_streamlit_search_experience-0.1.4/octostar_streamlit_search_experience/frontend/package.json
+-rw-r--r--   0        0        0     1916 2024-05-10 20:55:21.697320 octostar_streamlit_search_experience-0.1.4/octostar_streamlit_search_experience/frontend/src/App.tsx
+-rw-r--r--   0        0        0      472 2024-05-10 20:37:49.870464 octostar_streamlit_search_experience-0.1.4/octostar_streamlit_search_experience/frontend/src/components/Dropzone/Dropzone.module.css
+-rw-r--r--   0        0        0     6742 2024-05-10 21:00:04.083424 octostar_streamlit_search_experience-0.1.4/octostar_streamlit_search_experience/frontend/src/components/Dropzone/Dropzone.tsx
+-rw-r--r--   0        0        0       33 2024-05-10 02:16:57.058643 octostar_streamlit_search_experience-0.1.4/octostar_streamlit_search_experience/frontend/src/components/SearchExperienceButton/SearchExperienceButton.module.css
+-rw-r--r--   0        0        0      716 2024-05-10 02:17:50.306372 octostar_streamlit_search_experience-0.1.4/octostar_streamlit_search_experience/frontend/src/components/SearchExperienceButton/SearchExperienceButton.tsx
+-rw-r--r--   0        0        0      215 2024-05-06 20:48:31.521496 octostar_streamlit_search_experience-0.1.4/octostar_streamlit_search_experience/frontend/src/main.tsx
+-rw-r--r--   0        0        0      297 2024-05-10 18:41:03.922126 octostar_streamlit_search_experience-0.1.4/octostar_streamlit_search_experience/frontend/src/types.ts
+-rw-r--r--   0        0        0       38 2024-05-06 19:56:14.708711 octostar_streamlit_search_experience-0.1.4/octostar_streamlit_search_experience/frontend/src/vite-env.d.ts
+-rw-r--r--   0        0        0      605 2024-05-06 19:56:14.709077 octostar_streamlit_search_experience-0.1.4/octostar_streamlit_search_experience/frontend/tsconfig.json
+-rw-r--r--   0        0        0      233 2024-05-06 19:56:14.709733 octostar_streamlit_search_experience-0.1.4/octostar_streamlit_search_experience/frontend/tsconfig.node.json
+-rw-r--r--   0        0        0      178 2024-05-08 17:55:47.277413 octostar_streamlit_search_experience-0.1.4/octostar_streamlit_search_experience/frontend/vite.config.ts
+-rw-r--r--   0        0        0      486 2024-05-10 21:00:57.136179 octostar_streamlit_search_experience-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1522 1970-01-01 00:00:00.000000 octostar_streamlit_search_experience-0.1.4/PKG-INFO
```

### Comparing `octostar_streamlit_search_experience-0.1.3/README.md` & `octostar_streamlit_search_experience-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `octostar_streamlit_search_experience-0.1.3/octostar_streamlit_search_experience/__init__.py` & `octostar_streamlit_search_experience-0.1.4/octostar_streamlit_search_experience/__init__.py`

 * *Files identical despite different names*

### Comparing `octostar_streamlit_search_experience-0.1.3/octostar_streamlit_search_experience/frontend/README.md` & `octostar_streamlit_search_experience-0.1.4/octostar_streamlit_search_experience/frontend/README.md`

 * *Files identical despite different names*

### Comparing `octostar_streamlit_search_experience-0.1.3/octostar_streamlit_search_experience/frontend/dist/assets/index-DJ3f7eVh.js` & `octostar_streamlit_search_experience-0.1.4/octostar_streamlit_search_experience/frontend/dist/assets/index-DJ3f7eVh.js`

 * *Files identical despite different names*

### Comparing `octostar_streamlit_search_experience-0.1.3/octostar_streamlit_search_experience/frontend/package-lock.json` & `octostar_streamlit_search_experience-0.1.4/octostar_streamlit_search_experience/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `octostar_streamlit_search_experience-0.1.3/octostar_streamlit_search_experience/frontend/package.json` & `octostar_streamlit_search_experience-0.1.4/octostar_streamlit_search_experience/frontend/package.json`

 * *Files identical despite different names*

### Comparing `octostar_streamlit_search_experience-0.1.3/octostar_streamlit_search_experience/frontend/src/App.tsx` & `octostar_streamlit_search_experience-0.1.4/octostar_streamlit_search_experience/frontend/src/App.tsx`

 * *Files identical despite different names*

### Comparing `octostar_streamlit_search_experience-0.1.3/octostar_streamlit_search_experience/frontend/src/components/Dropzone/Dropzone.tsx` & `octostar_streamlit_search_experience-0.1.4/octostar_streamlit_search_experience/frontend/src/components/Dropzone/Dropzone.tsx`

 * *Files identical despite different names*

### Comparing `octostar_streamlit_search_experience-0.1.3/octostar_streamlit_search_experience/frontend/src/components/SearchExperienceButton/SearchExperienceButton.tsx` & `octostar_streamlit_search_experience-0.1.4/octostar_streamlit_search_experience/frontend/src/components/SearchExperienceButton/SearchExperienceButton.tsx`

 * *Files identical despite different names*

### Comparing `octostar_streamlit_search_experience-0.1.3/octostar_streamlit_search_experience/frontend/tsconfig.json` & `octostar_streamlit_search_experience-0.1.4/octostar_streamlit_search_experience/frontend/tsconfig.json`

 * *Files identical despite different names*

### Comparing `octostar_streamlit_search_experience-0.1.3/PKG-INFO` & `octostar_streamlit_search_experience-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octostar-streamlit-search-experience
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

