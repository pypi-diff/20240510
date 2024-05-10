# Comparing `tmp/grabberlib-0.1.4.tar.gz` & `tmp/grabberlib-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grabberlib-0.1.4.tar", max compression
+gzip compressed data, was "grabberlib-0.1.5.tar", max compression
```

## Comparing `grabberlib-0.1.4.tar` & `grabberlib-0.1.5.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0        0 2024-05-03 14:50:36.715508 grabberlib-0.1.4/README.md
--rw-r--r--   0        0        0        1 2024-05-03 14:50:36.716140 grabberlib-0.1.4/assets/pages.txt
--rw-r--r--   0        0        0        0 2024-05-03 14:50:36.718507 grabberlib-0.1.4/grabber/__init__.py
--rw-r--r--   0        0        0     1690 2024-05-03 14:50:36.718702 grabberlib-0.1.4/grabber/__main__.py
--rw-r--r--   0        0        0        0 2024-05-03 14:50:36.718877 grabberlib-0.1.4/grabber/controllers/__init__.py
--rw-r--r--   0        0        0     5057 2024-05-08 12:59:24.763016 grabberlib-0.1.4/grabber/controllers/base.py
--rw-r--r--   0        0        0        0 2024-05-03 14:50:36.719286 grabberlib-0.1.4/grabber/core/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 14:50:36.719467 grabberlib-0.1.4/grabber/core/bot/__init__.py
--rw-r--r--   0        0        0      997 2024-05-08 13:00:46.779103 grabberlib-0.1.4/grabber/core/bot/core.py
--rw-r--r--   0        0        0       65 2024-05-03 14:50:36.719818 grabberlib-0.1.4/grabber/core/exc.py
--rw-r--r--   0        0        0      772 2024-05-08 11:57:16.753731 grabberlib-0.1.4/grabber/core/settings.py
--rw-r--r--   0        0        0        0 2024-05-03 14:50:36.720132 grabberlib-0.1.4/grabber/core/sources/__init__.py
--rw-r--r--   0        0        0     3708 2024-05-08 14:40:24.957649 grabberlib-0.1.4/grabber/core/sources/everia.py
--rw-r--r--   0        0        0     2666 2024-05-08 12:55:29.819062 grabberlib-0.1.4/grabber/core/sources/graph.py
--rw-r--r--   0        0        0     3061 2024-05-08 12:05:40.276104 grabberlib-0.1.4/grabber/core/sources/khd.py
--rw-r--r--   0        0        0     2445 2024-05-08 12:59:24.762443 grabberlib-0.1.4/grabber/core/sources/nudecosplay.py
--rw-r--r--   0        0        0     2818 2024-05-08 12:08:31.466179 grabberlib-0.1.4/grabber/core/sources/xasiat.py
--rw-r--r--   0        0        0     3143 2024-05-08 12:49:26.255753 grabberlib-0.1.4/grabber/core/sources/xiuren.py
--rw-r--r--   0        0        0        1 2024-05-03 14:50:36.721312 grabberlib-0.1.4/grabber/core/sources/yellow.py
--rw-r--r--   0        0        0    19079 2024-05-08 14:40:42.519056 grabberlib-0.1.4/grabber/core/utils.py
--rw-r--r--   0        0        0      175 2024-05-08 14:35:16.922182 grabberlib-0.1.4/grabber/core/version.py
--rw-r--r--   0        0        0        0 2024-05-03 14:50:36.721870 grabberlib-0.1.4/grabber/templates/__init__.py
--rw-r--r--   0        0        0     1036 2024-05-08 14:35:21.539925 grabberlib-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1348 1970-01-01 00:00:00.000000 grabberlib-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.755675 grabberlib-0.1.5/README.md
+-rw-r--r--   0        0        0        1 2024-04-20 14:47:15.755675 grabberlib-0.1.5/assets/pages.txt
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.1.5/grabber/__init__.py
+-rw-r--r--   0        0        0     1690 2024-04-20 14:47:15.759675 grabberlib-0.1.5/grabber/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.1.5/grabber/controllers/__init__.py
+-rw-r--r--   0        0        0     5270 2024-05-10 14:48:30.795989 grabberlib-0.1.5/grabber/controllers/base.py
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.1.5/grabber/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-22 14:35:12.060596 grabberlib-0.1.5/grabber/core/bot/__init__.py
+-rw-r--r--   0        0        0     1287 2024-05-10 12:20:10.885923 grabberlib-0.1.5/grabber/core/bot/core.py
+-rw-r--r--   0        0        0       65 2024-04-20 14:47:15.759675 grabberlib-0.1.5/grabber/core/exc.py
+-rw-r--r--   0        0        0      772 2024-05-09 12:59:39.317729 grabberlib-0.1.5/grabber/core/settings.py
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.1.5/grabber/core/sources/__init__.py
+-rw-r--r--   0        0        0     3320 2024-05-10 14:42:57.044880 grabberlib-0.1.5/grabber/core/sources/common.py
+-rw-r--r--   0        0        0     3653 2024-05-09 13:30:04.157477 grabberlib-0.1.5/grabber/core/sources/everia.py
+-rw-r--r--   0        0        0     2698 2024-05-10 12:33:08.173014 grabberlib-0.1.5/grabber/core/sources/graph.py
+-rw-r--r--   0        0        0     3218 2024-05-10 12:29:42.290554 grabberlib-0.1.5/grabber/core/sources/khd.py
+-rw-r--r--   0        0        0     2857 2024-05-10 12:22:23.770346 grabberlib-0.1.5/grabber/core/sources/nudecosplay.py
+-rw-r--r--   0        0        0     2818 2024-05-09 12:59:39.317729 grabberlib-0.1.5/grabber/core/sources/xasiat.py
+-rw-r--r--   0        0        0     2950 2024-05-10 12:23:01.737325 grabberlib-0.1.5/grabber/core/sources/xiuren.py
+-rw-r--r--   0        0        0        1 2024-04-20 14:47:15.759675 grabberlib-0.1.5/grabber/core/sources/yellow.py
+-rw-r--r--   0        0        0    19128 2024-05-10 14:47:30.689591 grabberlib-0.1.5/grabber/core/utils.py
+-rw-r--r--   0        0        0      175 2024-05-10 14:59:26.762508 grabberlib-0.1.5/grabber/core/version.py
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.1.5/grabber/templates/__init__.py
+-rw-r--r--   0        0        0     1036 2024-05-10 14:59:34.322306 grabberlib-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1348 1970-01-01 00:00:00.000000 grabberlib-0.1.5/PKG-INFO
```

### Comparing `grabberlib-0.1.4/grabber/__main__.py` & `grabberlib-0.1.5/grabber/__main__.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.4/grabber/controllers/base.py` & `grabberlib-0.1.5/grabber/controllers/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from cement import Controller, ex
 from telegraph import Telegraph
 
 from grabber.core.settings import TELEGRAPH_TOKEN
+from grabber.core.sources.common import get_sources_for_common
 from grabber.core.sources.everia import get_sources_for_everia
 from grabber.core.sources.graph import get_for_telegraph
 from grabber.core.sources.khd import get_sources_for_4khd
 from grabber.core.sources.nudecosplay import get_sources_for_nudecosplay
 from grabber.core.sources.xiuren import get_sources_for_xiuren
 from grabber.core.utils import upload_folders_to_telegraph
 
@@ -129,27 +130,30 @@
             "4khd": get_sources_for_4khd,
             "telegraph": get_for_telegraph,
             "xiuren": get_sources_for_xiuren,
             "nudecosplay": get_sources_for_nudecosplay,
             "nudebird": get_sources_for_nudecosplay,
             "hotgirl": get_sources_for_nudecosplay,
             "everia": get_sources_for_everia,
+            "bestgirlsexy": get_sources_for_common,
+            "asigirl": get_sources_for_common,
+            "cosplaytele": get_sources_for_common,
         }
 
         if upload:
             upload_folders_to_telegraph(
                 folder_name=folder,
                 limit=limit,
                 send_to_channel=send_to_telegram,
                 telegraph_client=telegraph_client,
             )
         else:
             getter_images = getter_mapping.get(entity, get_for_telegraph)
             getter_images(
                 sources=sources,
                 entity=entity,
+                telegraph_client=telegraph_client,
                 final_dest=folder,
                 save_to_telegraph=publish,
                 is_tag=is_tag,
                 limit=limit,
-                telegraph_client=telegraph_client,
             )
```

### Comparing `grabberlib-0.1.4/grabber/core/settings.py` & `grabberlib-0.1.5/grabber/core/settings.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.4/grabber/core/sources/everia.py` & `grabberlib-0.1.5/grabber/core/sources/everia.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,16 +93,14 @@
         if final_dest:
             folder_name = page_title
             title_dest = final_dest / folder_name
             if not title_dest.exists():
                 title_dest.mkdir(parents=True, exist_ok=True)
             title_folder_mapping[page_title] = (unique_img_urls, title_dest)
 
-        final_dest.mkdir(parents=True, exist_ok=True)
-
         if save_to_telegraph:
             telegraph_uploader(
                 unique_img_urls=unique_img_urls,
                 page_title=page_title,
                 posts_sent_counter=posts_sent_counter,
                 telegraph_client=telegraph_client,
             )
```

### Comparing `grabberlib-0.1.4/grabber/core/sources/graph.py` & `grabberlib-0.1.5/grabber/core/sources/graph.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,76 +18,74 @@
     sources: List[str],
     entity: str,
     telegraph_client: Telegraph,
     final_dest: str | pathlib.Path = "",
     save_to_telegraph: bool | None = False,
     **kwargs,
 ) -> None:
-    posts_sent_counter = 0
-    titles = set()
     tqdm_sources_iterable = tqdm(
         enumerate(sources),
         total=len(sources),
+        desc="Retrieving URLs...",
     )
     query, src_attr = query_mapping[entity]
     headers = headers_mapping.get(entity, None)
-    folders = set()
-    titles_and_folders = set()
+    page_title = None
     title_folder_mapping = {}
+    posts_sent_counter = 0
+    titles = []
 
     if final_dest:
-        final_dest = pathlib.Path(final_dest)
-        if not final_dest.exists():
-            final_dest.mkdir(parents=True, exist_ok=True)
-    else:
-        final_dest = get_media_root()
+        final_dest_folder = get_media_root() / final_dest
+        if not final_dest_folder.exists():
+            final_dest_folder.mkdir(parents=True, exist_ok=True)
+            final_dest = final_dest_folder
 
     for idx, source_url in tqdm_sources_iterable:
         folder_name = ""
         tags, soup = get_tags(
             source_url,
             headers=headers,
             query=query,
         )
 
-        title_tag = soup.select("title")[0]  # type: ignore
-        folder_name = title_tag.get_text().strip().rstrip()
-        page_title = folder_name
-        titles.add(page_title)
-        titles_and_folders.add((page_title, folder_name))
+        if page_title is None:
+            page_title = soup.find("title").get_text(strip=True)
 
-        final_dest = final_dest / folder_name
+        folder_name = page_title
 
-        if not final_dest.exists():
-            final_dest.mkdir(parents=True, exist_ok=True)
-
-        folders.add(final_dest)
         unique_img_urls = set()
-
         for idx, img_tag in enumerate(tags or []):
             img_src = img_tag.attrs[src_attr]
             img_name: str = img_src.split("/")[-1]
             img_name = img_name.strip().rstrip()
             if "images.hotgirl.asia" not in img_src:
                 unique_img_urls.add(
                     (f"{idx + 1}-{img_name}", f"https://telegra.ph{img_src}")
                 )
             else:
                 unique_img_urls.add((f"{idx + 1}-{img_name}", img_src))
 
-        title_folder_mapping[page_title] = (unique_img_urls, final_dest)
+        if final_dest:
+            folder_name = page_title
+            title_dest = final_dest / folder_name
+            if not title_dest.exists():
+                title_dest.mkdir(parents=True, exist_ok=True)
+            title_folder_mapping[page_title] = (unique_img_urls, title_dest)
 
         if save_to_telegraph:
             telegraph_uploader(
                 unique_img_urls=unique_img_urls,
                 page_title=page_title,
                 posts_sent_counter=posts_sent_counter,
                 telegraph_client=telegraph_client,
+                tqdm_iterable=tqdm_sources_iterable,
             )
             posts_sent_counter += 1
+        page_title = None
 
     if final_dest:
         downloader(
             titles=titles,
             title_folder_mapping=title_folder_mapping,
             headers=headers,
         )
```

### Comparing `grabberlib-0.1.4/grabber/core/sources/khd.py` & `grabberlib-0.1.5/grabber/core/sources/xasiat.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,98 +1,92 @@
 import pathlib
-from typing import List, Optional
+from typing import List
 
 from telegraph import Telegraph
 from tqdm import tqdm
 
 from grabber.core.settings import get_media_root
 from grabber.core.utils import (
     downloader,
     query_mapping,
     headers_mapping,
     get_tags,
     telegraph_uploader,
 )
 
 
-def get_images_from_pagination(url: str, headers: Optional[dict] = None) -> List[str]:
-    page_nav_query = "div.page-link-box li a.page-numbers"
-    tags, _ = get_tags(url, headers=headers, query=page_nav_query)
-    return [a.attrs["href"] for a in tags if tags]
-
-
-def get_sources_for_4khd(
+def get_for_xasiat(
     sources: List[str],
     entity: str,
     telegraph_client: Telegraph,
     final_dest: str | pathlib.Path = "",
     save_to_telegraph: bool | None = False,
     **kwargs,
 ) -> None:
     send_to_telegram = kwargs.get("send_to_telegram", False)
     titles = set()
     tqdm_sources_iterable = tqdm(
         enumerate(sources),
         total=len(sources),
-        desc="Retrieving URLs...",
     )
     query, src_attr = query_mapping[entity]
     headers = headers_mapping.get(entity, None)
     folders = set()
     titles_and_folders = set()
     title_folder_mapping = {}
 
     if final_dest:
-        final_dest = pathlib.Path(final_dest)
-        if not final_dest.exists():
-            final_dest.mkdir(parents=True, exist_ok=True)
+        final_dest_folder = get_media_root() / final_dest
+        if not final_dest_folder.exists():
+            final_dest_folder.mkdir(parents=True, exist_ok=True)
+            final_dest = final_dest_folder
 
     for idx, source_url in tqdm_sources_iterable:
-        current_folder = None
-        current_title = None
         folder_name = ""
-        urls = [
+        tqdm_sources_iterable.set_description(f"Retrieving URLs from {source_url}")
+        tags, soup = get_tags(
             source_url,
-            *get_images_from_pagination(url=source_url, headers=headers),
-        ]
-        image_tags = []
-
-        for index, url in enumerate(urls):
-            tags, soup = get_tags(
-                url,
-                headers=headers,
-                query=query,
-            )
-            image_tags.extend(tags or [])
-
-            if index == 0:
-                folder_name = soup.select("title")[0].get_text()  # type: ignore
-                title = folder_name.strip().rstrip()
-                titles.add(title)
-                titles_and_folders.add((title, folder_name))
-                current_title = title
+            headers=headers,
+            query=query,
+        )
+
+        title_tag = soup.select("title")[0]  # type: ignore
+        folder_name = title_tag.get_text().strip().rstrip()
+        title = folder_name
+        titles.add(title)
+        titles_and_folders.add((title, folder_name))
 
         if final_dest:
-            new_folder = final_dest / folder_name
+            new_folder = get_media_root() / final_dest / folder_name
         else:
             new_folder = get_media_root() / folder_name
 
         if not new_folder.exists():
             new_folder.mkdir(parents=True, exist_ok=True)
 
-        current_folder = new_folder
-        folders.add(current_folder)
+        folders.add(new_folder)
         unique_img_urls = set()
 
-        for idx, img_tag in enumerate(image_tags):
+        for idx, img_tag in enumerate(tags or []):
             img_src = img_tag.attrs[src_attr]
-            img_name: str = img_src.split("/")[-1].split("?")[0]
-            img_name = img_name.strip().rstrip()
-            unique_img_urls.add((f"{idx + 1}-{img_name}", img_src))
-        title_folder_mapping[current_title] = (unique_img_urls, new_folder)
+
+            if "xasiat" in img_src:
+                img_name: str = img_src.split("/")[-2]
+                img_name = img_name.strip().rstrip()
+                img_extension: str = img_name.split(".")[-1]
+            else:
+                img_name: str = img_src.split("/")[-1]
+                img_name = img_name.strip().rstrip()
+                img_extension: str = img_name.split(".")[-1]
+
+            unique_img_urls.add(
+                (title, f"{idx + 1}.{img_extension}", img_src),
+            )
+
+        title_folder_mapping[title] = (unique_img_urls, new_folder)
 
     downloader(title_folder_mapping, headers)
     telegraph_uploader(
         title_folder_mapping=title_folder_mapping,
         send_to_telegram=send_to_telegram,
         save_to_telegraph=save_to_telegraph,
         telegraph_client=telegraph_client,
```

### Comparing `grabberlib-0.1.4/grabber/core/sources/nudecosplay.py` & `grabberlib-0.1.5/grabber/core/sources/xiuren.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,83 +1,96 @@
 import pathlib
-from typing import List
+from typing import List, Optional
 
-from telegraph import Telegraph
+import telegraph
 from tqdm import tqdm
 
-from grabber.core.settings import get_media_root
 from grabber.core.utils import (
     downloader,
+    get_pages_from_pagination,
     query_mapping,
     headers_mapping,
     get_tags,
     telegraph_uploader,
 )
 
 
-def get_sources_for_nudecosplay(
+def get_sources_for_xiuren(
     sources: List[str],
     entity: str,
-    telegraph_client: Telegraph,
+    telegraph_client: Optional[telegraph.Telegraph] = None,
     final_dest: str | pathlib.Path = "",
     save_to_telegraph: bool | None = False,
-    **kwargs,
+    is_tag: Optional[bool] = False,
+    limit: Optional[int] = None,
 ) -> None:
-    send_to_telegram = kwargs.get("send_to_telegram", False)
-    titles = set()
+    query, src_attr = query_mapping[entity]
+    headers = headers_mapping.get(entity, None)
+    page_title = None
+    title_folder_mapping = {}
+    posts_sent_counter = 0
+    titles = []
+    titles_posted = set()
+
     tqdm_sources_iterable = tqdm(
         enumerate(sources),
         total=len(sources),
         desc="Retrieving URLs...",
     )
-    query, src_attr = query_mapping[entity]
-    headers = headers_mapping.get(entity, None)
-    folders = set()
-    titles_and_folders = set()
-    title_folder_mapping = {}
-
-    if final_dest:
-        final_dest_folder = get_media_root() / final_dest
-        if not final_dest_folder.exists():
-            final_dest_folder.mkdir(parents=True, exist_ok=True)
-            final_dest = final_dest_folder
 
     for idx, source_url in tqdm_sources_iterable:
         folder_name = ""
-        tags, soup = get_tags(
+        if is_tag:
+            urls = get_pages_from_pagination(url=source_url, target="xiuren")
+            targets = urls[:limit] if limit else urls
+            return get_sources_for_xiuren(
+                sources=targets,
+                entity=entity,
+                final_dest=final_dest,
+                save_to_telegraph=save_to_telegraph,
+                is_tag=False,
+            )
+
+        image_tags, soup = get_tags(
             source_url,
             headers=headers,
             query=query,
         )
 
-        title_tag = soup.select("title")[0]  # type: ignore
-        folder_name = title_tag.get_text().strip().rstrip()
-        title = folder_name
-        titles.add(title)
-        titles_and_folders.add((title, folder_name))
+        if page_title is None:
+            page_title = soup.find('title').get_text(strip=True).split("- Xiuren.biz")[0].strip().rstrip()
+            titles.append(page_title)
 
-        if final_dest:
-            new_folder = get_media_root() / final_dest / folder_name
-        else:
-            new_folder = get_media_root() / folder_name
-
-        if not new_folder.exists():
-            new_folder.mkdir(parents=True, exist_ok=True)
-
-        folders.add(new_folder)
         unique_img_urls = set()
-
-        for idx, img_tag in enumerate(tags or []):
+        for idx, img_tag in enumerate(image_tags):
             img_src = img_tag.attrs[src_attr]
-            img_name: str = img_src.split("/")[-1]
+            img_name: str = img_src.split("/")[-1].split("?")[0]
             img_name = img_name.strip().rstrip()
             unique_img_urls.add((f"{idx + 1}-{img_name}", img_src))
 
-        title_folder_mapping[title] = (unique_img_urls, new_folder)
+        tqdm_sources_iterable.set_description(f"Finished retrieving images for {page_title}")
 
-    downloader(title_folder_mapping, headers)
-    telegraph_uploader(
-        title_folder_mapping=title_folder_mapping,
-        send_to_telegram=send_to_telegram,
-        save_to_telegraph=save_to_telegraph,
-        telegraph_client=telegraph_client,
-    )
+        if final_dest:
+            folder_name = page_title
+            title_dest = final_dest / folder_name
+            if not title_dest.exists():
+                title_dest.mkdir(parents=True, exist_ok=True)
+            title_folder_mapping[page_title] = (unique_img_urls, title_dest)
+
+        if save_to_telegraph:
+            telegraph_uploader(
+                unique_img_urls=unique_img_urls,
+                page_title=page_title,
+                posts_sent_counter=posts_sent_counter,
+                telegraph_client=telegraph_client,
+                tqdm_iterable=tqdm_sources_iterable,
+            )
+            titles_posted.add(page_title)
+            posts_sent_counter += 1
+        page_title = None
+
+    if final_dest:
+        downloader(
+            titles=titles,
+            title_folder_mapping=title_folder_mapping,
+            headers=headers,
+        )
```

### Comparing `grabberlib-0.1.4/grabber/core/sources/xasiat.py` & `grabberlib-0.1.5/grabber/core/sources/common.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,84 +10,95 @@
     query_mapping,
     headers_mapping,
     get_tags,
     telegraph_uploader,
 )
 
 
-def get_for_xasiat(
+def get_sources_for_common(
     sources: List[str],
     entity: str,
     telegraph_client: Telegraph,
     final_dest: str | pathlib.Path = "",
     save_to_telegraph: bool | None = False,
     **kwargs,
 ) -> None:
-    send_to_telegram = kwargs.get("send_to_telegram", False)
-    titles = set()
     tqdm_sources_iterable = tqdm(
         enumerate(sources),
         total=len(sources),
+        desc="Retrieving URLs...",
     )
     query, src_attr = query_mapping[entity]
     headers = headers_mapping.get(entity, None)
-    folders = set()
-    titles_and_folders = set()
+    page_title = None
     title_folder_mapping = {}
+    posts_sent_counter = 0
+    titles = []
 
     if final_dest:
         final_dest_folder = get_media_root() / final_dest
         if not final_dest_folder.exists():
             final_dest_folder.mkdir(parents=True, exist_ok=True)
             final_dest = final_dest_folder
 
     for idx, source_url in tqdm_sources_iterable:
         folder_name = ""
-        tqdm_sources_iterable.set_description(f"Retrieving URLs from {source_url}")
-        tags, soup = get_tags(
+        image_tags, soup = get_tags(
             source_url,
             headers=headers,
             query=query,
         )
+        if not image_tags and entity == "asigirl":
+            queries_and_atrrs = [
+                ("a.gallery-item", "data-src"),
+                ("a.swipebox", "href"),
+                ("div.gallery-group a", "href"),
+                ("div.gallery-container.justified-gallery a", "href"),
+            ]
+            for query, src_attr in queries_and_atrrs:
+                image_tags, soup = get_tags(
+                    source_url,
+                    headers=headers,
+                    query=query,
+                )
+                if image_tags:
+                    break
+
+        if page_title is None:
+            page_title = soup.find('title').get_text(strip=True).rstrip()
+            if "Free Download" in page_title:
+                page_title = page_title.split("- Free Download")[0]
+            titles.append(page_title)
 
-        title_tag = soup.select("title")[0]  # type: ignore
-        folder_name = title_tag.get_text().strip().rstrip()
-        title = folder_name
-        titles.add(title)
-        titles_and_folders.add((title, folder_name))
-
-        if final_dest:
-            new_folder = get_media_root() / final_dest / folder_name
-        else:
-            new_folder = get_media_root() / folder_name
-
-        if not new_folder.exists():
-            new_folder.mkdir(parents=True, exist_ok=True)
-
-        folders.add(new_folder)
         unique_img_urls = set()
-
-        for idx, img_tag in enumerate(tags or []):
+        for idx, img_tag in enumerate(image_tags):
             img_src = img_tag.attrs[src_attr]
+            img_name: str = img_src.split("/")[-1].split("?")[0]
+            img_name = img_name.strip().rstrip()
+            unique_img_urls.add((f"{idx + 1}-{img_name}", img_src))
 
-            if "xasiat" in img_src:
-                img_name: str = img_src.split("/")[-2]
-                img_name = img_name.strip().rstrip()
-                img_extension: str = img_name.split(".")[-1]
-            else:
-                img_name: str = img_src.split("/")[-1]
-                img_name = img_name.strip().rstrip()
-                img_extension: str = img_name.split(".")[-1]
+        tqdm_sources_iterable.set_description(f"Finished retrieving images for {page_title}")
 
-            unique_img_urls.add(
-                (title, f"{idx + 1}.{img_extension}", img_src),
+        if final_dest:
+            folder_name = page_title
+            title_dest = final_dest / folder_name
+            if not title_dest.exists():
+                title_dest.mkdir(parents=True, exist_ok=True)
+            title_folder_mapping[page_title] = (unique_img_urls, title_dest)
+
+        if save_to_telegraph:
+            telegraph_uploader(
+                unique_img_urls=unique_img_urls,
+                page_title=page_title,
+                posts_sent_counter=posts_sent_counter,
+                telegraph_client=telegraph_client,
+                tqdm_iterable=tqdm_sources_iterable,
             )
+            posts_sent_counter += 1
+        page_title = None
 
-        title_folder_mapping[title] = (unique_img_urls, new_folder)
-
-    downloader(title_folder_mapping, headers)
-    telegraph_uploader(
-        title_folder_mapping=title_folder_mapping,
-        send_to_telegram=send_to_telegram,
-        save_to_telegraph=save_to_telegraph,
-        telegraph_client=telegraph_client,
-    )
+    if final_dest:
+        downloader(
+            titles=titles,
+            title_folder_mapping=title_folder_mapping,
+            headers=headers,
+        )
```

### Comparing `grabberlib-0.1.4/grabber/core/sources/xiuren.py` & `grabberlib-0.1.5/grabber/core/sources/nudecosplay.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,105 +1,92 @@
 import pathlib
 from typing import List
 
-import telegraph
+from telegraph import Telegraph
 from tqdm import tqdm
 
 from grabber.core.settings import get_media_root
 from grabber.core.utils import (
     downloader,
-    get_pages_from_pagination,
     query_mapping,
     headers_mapping,
     get_tags,
     telegraph_uploader,
 )
 
 
-def get_sources_for_xiuren(
+def get_sources_for_nudecosplay(
     sources: List[str],
     entity: str,
-    telegraph_client: telegraph.Telegraph,
+    telegraph_client: Telegraph,
     final_dest: str | pathlib.Path = "",
     save_to_telegraph: bool | None = False,
     **kwargs,
 ) -> None:
-    titles = set()
-    is_tag: bool = kwargs.get("is_tag", False)
-    limit: int = kwargs.get("limit", 0)
     tqdm_sources_iterable = tqdm(
         enumerate(sources),
         total=len(sources),
         desc="Retrieving URLs...",
     )
     query, src_attr = query_mapping[entity]
     headers = headers_mapping.get(entity, None)
-    folders = set()
-    titles_and_folders = set()
+    page_title = None
     title_folder_mapping = {}
     posts_sent_counter = 0
+    titles = []
+    split_text_mapping = {
+        'nudebird': '- Nude Bird',
+        'nudecosplay': '/nudecosplay.biz/',
+        "hotgirl": "- Hotgirl.biz"
+    }
+    split_text_with = split_text_mapping[entity]
 
     if final_dest:
         final_dest_folder = get_media_root() / final_dest
         if not final_dest_folder.exists():
             final_dest_folder.mkdir(parents=True, exist_ok=True)
             final_dest = final_dest_folder
 
     for idx, source_url in tqdm_sources_iterable:
         folder_name = ""
-
-        if is_tag:
-            urls = get_pages_from_pagination(url=source_url, target="xiuren")
-            targets = urls[:limit] if limit else urls
-            return get_sources_for_xiuren(
-                sources=targets,
-                entity=entity,
-                final_dest=final_dest,
-                save_to_telegraph=save_to_telegraph,
-                is_tag=False,
-            )
-
-        tags, soup = get_tags(
+        image_tags, soup = get_tags(
             source_url,
             headers=headers,
             query=query,
         )
+        if page_title is None:
+            page_title = soup.find('title').get_text(strip=True).split(split_text_with)[0].strip().rstrip()
+            titles.append(page_title)
 
-        title_tag = soup.select("title")[0]  # type: ignore
-        folder_name = title_tag.get_text().strip().rstrip()
-        page_title = folder_name
-        titles.add(page_title)
-        titles_and_folders.add((page_title, folder_name))
-
-        if final_dest:
-            new_folder = get_media_root() / final_dest / folder_name
-        else:
-            new_folder = get_media_root() / folder_name
-
-        if not new_folder.exists():
-            new_folder.mkdir(parents=True, exist_ok=True)
-
-        folders.add(new_folder)
         unique_img_urls = set()
-
-        for idx, img_tag in enumerate(tags or []):
+        for idx, img_tag in enumerate(image_tags):
             img_src = img_tag.attrs[src_attr]
-            img_name: str = img_src.split("/")[-1]
+            img_name: str = img_src.split("/")[-1].split("?")[0]
             img_name = img_name.strip().rstrip()
             unique_img_urls.add((f"{idx + 1}-{img_name}", img_src))
 
-        title_folder_mapping[page_title] = (unique_img_urls, new_folder)
+        tqdm_sources_iterable.set_description(f"Finished retrieving images for {page_title}")
+
+        if final_dest:
+            folder_name = page_title
+            title_dest = final_dest / folder_name
+            if not title_dest.exists():
+                title_dest.mkdir(parents=True, exist_ok=True)
+            title_folder_mapping[page_title] = (unique_img_urls, title_dest)
+
         if save_to_telegraph:
             telegraph_uploader(
                 unique_img_urls=unique_img_urls,
                 page_title=page_title,
                 posts_sent_counter=posts_sent_counter,
                 telegraph_client=telegraph_client,
+                tqdm_iterable=tqdm_sources_iterable,
             )
             posts_sent_counter += 1
+        page_title = None
 
     if final_dest:
         downloader(
             titles=titles,
             title_folder_mapping=title_folder_mapping,
             headers=headers,
         )
```

### Comparing `grabberlib-0.1.4/grabber/core/utils.py` & `grabberlib-0.1.5/grabber/core/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,16 +27,17 @@
 PAGINATION_BASE_URL_QUERY = "div.jeg_navigation.jeg_pagination a.page_number"
 POSTS_QUERY_XPATH = "/html/body/div[2]/div[5]/div/div[1]/div/div/div[2]/div/div/div[2]/div/div[1]/div/div/div/article/div/div/a"
 
 
 query_mapping = {
     "xiuren": ("div.content-inner img", "src"),
     "nudebird": ("div.thecontent a", "href"),
+    "hotgirl": ("div.thecontent a", "href"),
     "nudecosplay": (
-        "img[src^='https://static9.hentai-cosplays.com/'][alt^='PureMedia']",
+        "div.content-inner a[data-lbwps-srcsmall^='https://nudecosplay.biz'] img",
         "src",
     ),
     "v2ph": ("div.photos-list.text-center img", "src"),  # Needs to handle pagination
     "cgcosplay": ("div.gallery-icon.portrait img", "src"),
     "mitaku": ("img.msacwl-img", "data-lazy"),
     "xasiat": ("div.images a", "href"),
     "telegraph": ("img", "src"),
@@ -45,14 +46,17 @@
         "src",
     ),
     "yellow": (
         "div.elementor-widget-container a[href^='https://terabox.com']",
         "href",
     ),
     "everia": ("div.entry-content img", "src"),
+    "bestgirlsexy": ("div.elementor-widget-container p img", "data-src"),
+    "asigirl": ("a.asigirl-item", "href"),
+    "cosplaytele": ("img.attachment-full.size-full", "src"),
 }
 
 
 @dataclass(kw_only=True)
 class PaginationXPath:
     pagination_query: str
     pages_count_query: str
@@ -243,16 +247,16 @@
 
 
 def telegraph_uploader(
     unique_img_urls: Tuple[Tuple[str, str]],
     page_title: str,
     posts_sent_counter: Optional[int] = 0,
     telegraph_client: Optional[Telegraph] = None,
+    tqdm_iterable: Optional[tqdm] = None,
 ) -> None:
-    is_title_posted = False
     if telegraph_client is None:
         telegraph_client = get_new_telegraph_client()
 
     posts = []
     html_post = create_html_template(unique_img_urls)
     post_url = create_page(
         title=page_title, html_content=html_post, telegraph_client=telegraph_client
@@ -260,38 +264,30 @@
     telegraph_post = f"{page_title} - {post_url}"
     posts.append(telegraph_post)
 
     if posts_sent_counter == 10:
         sleep(10)
 
     try:
-        if not is_title_posted:
-            asyncio.run(
-                send_message(
-                    post_text=page_title,
-                    retry=True,
-                    posts_counter=posts_sent_counter,
-                )
-            )
-            is_title_posted = True
-
         asyncio.run(
             send_message(
                 post_text=telegraph_post,
                 retry=True,
                 posts_counter=posts_sent_counter,
+                tqdm_iterable=tqdm_iterable,
             )
         )
     except Exception:
         sleep(20)
         asyncio.run(
             send_message(
                 post_text=telegraph_post,
                 retry=True,
                 posts_counter=posts_sent_counter,
+                tqdm_iterable=tqdm_iterable,
             )
         )
 
         albums_dir = pathlib.Path.home() / ".albums_data"
         albums_dir.mkdir(parents=True, exist_ok=True)
         albums_file = albums_dir / "pages.txt"
```

### Comparing `grabberlib-0.1.4/pyproject.toml` & `grabberlib-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grabberlib"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["grabber"]
 readme = "README.md"
 packages = [
     { include = "grabber/**/*.py" },
     { include = "assets/pages.txt" },
 ]
```

### Comparing `grabberlib-0.1.4/PKG-INFO` & `grabberlib-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grabberlib
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: grabber
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

