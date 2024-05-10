# Comparing `tmp/md2api-0.4.2.tar.gz` & `tmp/md2api-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "md2api-0.4.2.tar", max compression
+gzip compressed data, was "md2api-0.5.0.tar", max compression
```

## Comparing `md2api-0.4.2.tar` & `md2api-0.5.0.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0     1065 2021-08-22 10:43:12.503115 md2api-0.4.2/LICENSE
--rw-r--r--   0        0        0      377 2022-05-29 11:58:16.502648 md2api-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     4596 2022-05-29 11:57:44.943329 md2api-0.4.2/src/md2api/run.py
--rw-r--r--   0        0        0      772 2022-05-29 11:58:42.843025 md2api-0.4.2/setup.py
--rw-r--r--   0        0        0      438 2022-05-29 11:58:42.843221 md2api-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-10 15:57:04.155006 md2api-0.5.0/LICENSE
+-rw-r--r--   0        0        0      376 2024-05-10 21:30:41.532184 md2api-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6111 2024-05-10 21:29:06.364181 md2api-0.5.0/src/md2api/run.py
+-rw-r--r--   0        0        0      436 1970-01-01 00:00:00.000000 md2api-0.5.0/PKG-INFO
```

### Comparing `md2api-0.4.2/LICENSE` & `md2api-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `md2api-0.4.2/src/md2api/run.py` & `md2api-0.5.0/src/md2api/run.py`

 * *Files 22% similar despite different names*

```diff
@@ -95,14 +95,49 @@
             description=extract_description(document.html_text),
             published_at=document.published_at
         )for document in documents
     ]
     document_path = index_path / Path('index.html')
     document_path.write_text(json.dumps(sorted([index._asdict() for index in indices], key=lambda i: i.get('published_at'))))
 
+def create_category_index(output_path: Path, documents: list[Document]):
+    index_path = output_path / Path('posts')
+
+    indices: list[Index] = [
+        Index(
+            title=document.title,
+            heading=document.heading,
+            path='/' + str(Path('posts') / document.path),
+            description=extract_description(document.html_text),
+            published_at=document.published_at
+        )for document in documents
+    ]
+
+    category_names = dict()
+
+    for document in documents:
+        category_name = document.path.split('/')[0]
+        postIndex = Index(
+            title=document.title,
+            heading=document.heading,
+            path='/' + str(Path('posts') / document.path),
+            description=extract_description(document.html_text),
+            published_at=document.published_at
+        )
+
+        if category_name not in category_names.keys():
+            category_names[category_name] = [postIndex]
+        else: 
+            category_names[category_name] = category_names[category_name].append(postIndex)
+    
+    for category, posts in category_names.items():
+        document_path = index_path / Path(category) / Path('index.html')
+        document_path.write_text(json.dumps(sorted([post._asdict() for post in posts], key=lambda i: i.get('published_at'))))
+        # print(json.dumps(sorted([index._asdict() for category_name in category_names], key=lambda i: i.get('published_at'))))
+
 
 def create_sitemap_xml(output_path: Path, site_url: str, post_dir: str, pages: list[Document]) -> str:
     urlset = ElementTree.Element('urlset')
     urlset.set("xmlns", "http://www.sitemaps.org/schemas/sitemap/0.9")
     tree = ElementTree.ElementTree(element=urlset)
 
     # for top-page
@@ -143,12 +178,13 @@
             html_text=convert_markdown_to_html(markdown.read_text()),
             published_at=get_lastcommit_date(markdown)
         ) for markdown in markdown_files if get_lastcommit_date(markdown)
     ]
 
     create_posts(output_path=output_path, documents=documents)
     create_posts_index(output_path=output_path, documents=documents)
+    create_category_index(output_path=output_path, documents=documents)
     create_sitemap_xml(output_path=output_path, site_url=site_url, post_dir=post_dir, pages=documents)
 
 
 if __name__ == '__main__':
     main()
```

