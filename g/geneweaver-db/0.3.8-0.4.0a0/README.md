# Comparing `tmp/geneweaver_db-0.3.8.tar.gz` & `tmp/geneweaver_db-0.4.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geneweaver_db-0.3.8.tar", max compression
+gzip compressed data, was "geneweaver_db-0.4.0a0.tar", max compression
```

## Comparing `geneweaver_db-0.3.8.tar` & `geneweaver_db-0.4.0a0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    11356 2024-05-10 15:31:00.208494 geneweaver_db-0.3.8/LICENSE
--rw-r--r--   0        0        0     2162 2024-05-10 15:31:00.208494 geneweaver_db-0.3.8/README.md
--rw-r--r--   0        0        0      953 2024-05-10 15:31:00.208494 geneweaver_db-0.3.8/pyproject.toml
--rw-r--r--   0        0        0      156 2024-05-10 15:31:00.208494 geneweaver_db-0.3.8/src/geneweaver/db/__init__.py
--rw-r--r--   0        0        0      132 2024-05-10 15:31:00.208494 geneweaver_db-0.3.8/src/geneweaver/db/aio/__init__.py
--rw-r--r--   0        0        0     3134 2024-05-10 15:31:00.208494 geneweaver_db-0.3.8/src/geneweaver/db/aio/gene.py
--rw-r--r--   0        0        0     4802 2024-05-10 15:31:00.208494 geneweaver_db-0.3.8/src/geneweaver/db/aio/geneset.py
--rw-r--r--   0        0        0     2189 2024-05-10 15:31:00.208494 geneweaver_db-0.3.8/src/geneweaver/db/aio/publication.py
--rw-r--r--   0        0        0     1310 2024-05-10 15:31:00.208494 geneweaver_db-0.3.8/src/geneweaver/db/aio/species.py
--rw-r--r--   0        0        0      809 2024-05-10 15:31:00.208494 geneweaver_db-0.3.8/src/geneweaver/db/aio/threshold.py
--rw-r--r--   0        0        0       56 2024-05-10 15:31:00.208494 geneweaver_db-0.3.8/src/geneweaver/db/core/__init__.py
--rw-r--r--   0        0        0      845 2024-05-10 15:31:00.208494 geneweaver_db-0.3.8/src/geneweaver/db/core/cursor.py
--rw-r--r--   0        0        0      145 2024-05-10 15:31:00.208494 geneweaver_db-0.3.8/src/geneweaver/db/core/settings.py
--rw-r--r--   0        0        0     1769 2024-05-10 15:31:00.208494 geneweaver_db-0.3.8/src/geneweaver/db/core/settings_class.py
--rw-r--r--   0        0        0      438 2024-05-10 15:31:00.208494 geneweaver_db-0.3.8/src/geneweaver/db/exceptions.py
--rw-r--r--   0        0        0    10316 2024-05-10 15:31:00.208494 geneweaver_db-0.3.8/src/geneweaver/db/gene.py
--rw-r--r--   0        0        0     8651 2024-05-10 15:31:00.208494 geneweaver_db-0.3.8/src/geneweaver/db/geneset.py
--rw-r--r--   0        0        0     7887 2024-05-10 15:31:00.208494 geneweaver_db-0.3.8/src/geneweaver/db/geneset_value.py
--rw-r--r--   0        0        0     2063 2024-05-10 15:31:00.208494 geneweaver_db-0.3.8/src/geneweaver/db/publication.py
--rw-r--r--   0        0        0       42 2024-05-10 15:31:00.208494 geneweaver_db-0.3.8/src/geneweaver/db/query/__init__.py
--rw-r--r--   0        0        0     5410 2024-05-10 15:31:00.208494 geneweaver_db-0.3.8/src/geneweaver/db/query/gene.py
--rw-r--r--   0        0        0      364 2024-05-10 15:31:00.208494 geneweaver_db-0.3.8/src/geneweaver/db/query/geneset/__init__.py
--rw-r--r--   0        0        0     1351 2024-05-10 15:31:00.208494 geneweaver_db-0.3.8/src/geneweaver/db/query/geneset/const.py
--rw-r--r--   0        0        0     4814 2024-05-10 15:31:00.208494 geneweaver_db-0.3.8/src/geneweaver/db/query/geneset/read.py
--rw-r--r--   0        0        0     3928 2024-05-10 15:31:00.208494 geneweaver_db-0.3.8/src/geneweaver/db/query/geneset/utils.py
--rw-r--r--   0        0        0     4014 2024-05-10 15:31:00.208494 geneweaver_db-0.3.8/src/geneweaver/db/query/geneset/write.py
--rw-r--r--   0        0        0      982 2024-05-10 15:31:00.208494 geneweaver_db-0.3.8/src/geneweaver/db/query/project.py
--rw-r--r--   0        0        0     4683 2024-05-10 15:31:00.208494 geneweaver_db-0.3.8/src/geneweaver/db/query/publication.py
--rw-r--r--   0        0        0       60 2024-05-10 15:31:00.208494 geneweaver_db-0.3.8/src/geneweaver/db/query/search/__init__.py
--rw-r--r--   0        0        0       50 2024-05-10 15:31:00.208494 geneweaver_db-0.3.8/src/geneweaver/db/query/search/search.py
--rw-r--r--   0        0        0     1571 2024-05-10 15:31:00.208494 geneweaver_db-0.3.8/src/geneweaver/db/query/search/utils.py
--rw-r--r--   0        0        0     1603 2024-05-10 15:31:00.208494 geneweaver_db-0.3.8/src/geneweaver/db/query/species.py
--rw-r--r--   0        0        0     2900 2024-05-10 15:31:00.208494 geneweaver_db-0.3.8/src/geneweaver/db/query/threshold.py
--rw-r--r--   0        0        0     1776 2024-05-10 15:31:00.208494 geneweaver_db-0.3.8/src/geneweaver/db/query/utils.py
--rw-r--r--   0        0        0     1249 2024-05-10 15:31:00.208494 geneweaver_db-0.3.8/src/geneweaver/db/species.py
--rw-r--r--   0        0        0      775 2024-05-10 15:31:00.208494 geneweaver_db-0.3.8/src/geneweaver/db/threshold.py
--rw-r--r--   0        0        0     6887 2024-05-10 15:31:00.208494 geneweaver_db-0.3.8/src/geneweaver/db/user.py
--rw-r--r--   0        0        0     3085 2024-05-10 15:31:00.208494 geneweaver_db-0.3.8/src/geneweaver/db/utils.py
--rw-r--r--   0        0        0     2982 1970-01-01 00:00:00.000000 geneweaver_db-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-05-10 16:39:57.138310 geneweaver_db-0.4.0a0/LICENSE
+-rw-r--r--   0        0        0     2162 2024-05-10 16:39:57.138310 geneweaver_db-0.4.0a0/README.md
+-rw-r--r--   0        0        0      955 2024-05-10 16:39:57.138310 geneweaver_db-0.4.0a0/pyproject.toml
+-rw-r--r--   0        0        0      156 2024-05-10 16:39:57.138310 geneweaver_db-0.4.0a0/src/geneweaver/db/__init__.py
+-rw-r--r--   0        0        0      132 2024-05-10 16:39:57.138310 geneweaver_db-0.4.0a0/src/geneweaver/db/aio/__init__.py
+-rw-r--r--   0        0        0     3134 2024-05-10 16:39:57.138310 geneweaver_db-0.4.0a0/src/geneweaver/db/aio/gene.py
+-rw-r--r--   0        0        0     4964 2024-05-10 16:39:57.138310 geneweaver_db-0.4.0a0/src/geneweaver/db/aio/geneset.py
+-rw-r--r--   0        0        0     2189 2024-05-10 16:39:57.138310 geneweaver_db-0.4.0a0/src/geneweaver/db/aio/publication.py
+-rw-r--r--   0        0        0     1310 2024-05-10 16:39:57.138310 geneweaver_db-0.4.0a0/src/geneweaver/db/aio/species.py
+-rw-r--r--   0        0        0      809 2024-05-10 16:39:57.138310 geneweaver_db-0.4.0a0/src/geneweaver/db/aio/threshold.py
+-rw-r--r--   0        0        0       56 2024-05-10 16:39:57.138310 geneweaver_db-0.4.0a0/src/geneweaver/db/core/__init__.py
+-rw-r--r--   0        0        0      845 2024-05-10 16:39:57.138310 geneweaver_db-0.4.0a0/src/geneweaver/db/core/cursor.py
+-rw-r--r--   0        0        0      145 2024-05-10 16:39:57.138310 geneweaver_db-0.4.0a0/src/geneweaver/db/core/settings.py
+-rw-r--r--   0        0        0     1769 2024-05-10 16:39:57.138310 geneweaver_db-0.4.0a0/src/geneweaver/db/core/settings_class.py
+-rw-r--r--   0        0        0      438 2024-05-10 16:39:57.138310 geneweaver_db-0.4.0a0/src/geneweaver/db/exceptions.py
+-rw-r--r--   0        0        0    10316 2024-05-10 16:39:57.138310 geneweaver_db-0.4.0a0/src/geneweaver/db/gene.py
+-rw-r--r--   0        0        0     8813 2024-05-10 16:39:57.138310 geneweaver_db-0.4.0a0/src/geneweaver/db/geneset.py
+-rw-r--r--   0        0        0     7887 2024-05-10 16:39:57.138310 geneweaver_db-0.4.0a0/src/geneweaver/db/geneset_value.py
+-rw-r--r--   0        0        0     2063 2024-05-10 16:39:57.138310 geneweaver_db-0.4.0a0/src/geneweaver/db/publication.py
+-rw-r--r--   0        0        0       42 2024-05-10 16:39:57.138310 geneweaver_db-0.4.0a0/src/geneweaver/db/query/__init__.py
+-rw-r--r--   0        0        0     5410 2024-05-10 16:39:57.138310 geneweaver_db-0.4.0a0/src/geneweaver/db/query/gene.py
+-rw-r--r--   0        0        0      364 2024-05-10 16:39:57.138310 geneweaver_db-0.4.0a0/src/geneweaver/db/query/geneset/__init__.py
+-rw-r--r--   0        0        0     1351 2024-05-10 16:39:57.138310 geneweaver_db-0.4.0a0/src/geneweaver/db/query/geneset/const.py
+-rw-r--r--   0        0        0     5291 2024-05-10 16:39:57.138310 geneweaver_db-0.4.0a0/src/geneweaver/db/query/geneset/read.py
+-rw-r--r--   0        0        0     4844 2024-05-10 16:39:57.138310 geneweaver_db-0.4.0a0/src/geneweaver/db/query/geneset/utils.py
+-rw-r--r--   0        0        0     4014 2024-05-10 16:39:57.138310 geneweaver_db-0.4.0a0/src/geneweaver/db/query/geneset/write.py
+-rw-r--r--   0        0        0      982 2024-05-10 16:39:57.138310 geneweaver_db-0.4.0a0/src/geneweaver/db/query/project.py
+-rw-r--r--   0        0        0     4683 2024-05-10 16:39:57.138310 geneweaver_db-0.4.0a0/src/geneweaver/db/query/publication.py
+-rw-r--r--   0        0        0       60 2024-05-10 16:39:57.138310 geneweaver_db-0.4.0a0/src/geneweaver/db/query/search/__init__.py
+-rw-r--r--   0        0        0       50 2024-05-10 16:39:57.138310 geneweaver_db-0.4.0a0/src/geneweaver/db/query/search/search.py
+-rw-r--r--   0        0        0     1571 2024-05-10 16:39:57.138310 geneweaver_db-0.4.0a0/src/geneweaver/db/query/search/utils.py
+-rw-r--r--   0        0        0     1603 2024-05-10 16:39:57.138310 geneweaver_db-0.4.0a0/src/geneweaver/db/query/species.py
+-rw-r--r--   0        0        0     2900 2024-05-10 16:39:57.138310 geneweaver_db-0.4.0a0/src/geneweaver/db/query/threshold.py
+-rw-r--r--   0        0        0     1776 2024-05-10 16:39:57.138310 geneweaver_db-0.4.0a0/src/geneweaver/db/query/utils.py
+-rw-r--r--   0        0        0     1249 2024-05-10 16:39:57.138310 geneweaver_db-0.4.0a0/src/geneweaver/db/species.py
+-rw-r--r--   0        0        0      775 2024-05-10 16:39:57.138310 geneweaver_db-0.4.0a0/src/geneweaver/db/threshold.py
+-rw-r--r--   0        0        0     6887 2024-05-10 16:39:57.138310 geneweaver_db-0.4.0a0/src/geneweaver/db/user.py
+-rw-r--r--   0        0        0     3085 2024-05-10 16:39:57.138310 geneweaver_db-0.4.0a0/src/geneweaver/db/utils.py
+-rw-r--r--   0        0        0     2984 1970-01-01 00:00:00.000000 geneweaver_db-0.4.0a0/PKG-INFO
```

### Comparing `geneweaver_db-0.3.8/LICENSE` & `geneweaver_db-0.4.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.8/README.md` & `geneweaver_db-0.4.0a0/README.md`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.8/pyproject.toml` & `geneweaver_db-0.4.0a0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geneweaver-db"
-version = "0.3.8"
+version = "0.4.0a0"
 description = "Database Interaction Services for GeneWeaver"
 authors = ["Jax Computational Sciences <cssc@jax.org>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://thejacksonlaboratory.github.io/geneweaver-docs/"
 repository = "https://github.com/TheJacksonLaboratory/geneweaver-db"
 packages = [
```

### Comparing `geneweaver_db-0.3.8/src/geneweaver/db/aio/gene.py` & `geneweaver_db-0.4.0a0/src/geneweaver/db/aio/gene.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.8/src/geneweaver/db/aio/geneset.py` & `geneweaver_db-0.4.0a0/src/geneweaver/db/aio/geneset.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     pubmed_id: Optional[int] = None,
     gene_id_type: Optional[GeneIdentifier] = None,
     search_text: Optional[str] = None,
     limit: Optional[int] = None,
     offset: Optional[int] = None,
     is_readable_by: Optional[int] = None,
     with_publication_info: bool = True,
+    ontology_term: Optional[str] = None,
 ) -> List[Row]:
     """Get genesets from the database.
 
     :param cursor: An async database cursor.
     :param gs_id: Show only results with this geneset ID.
     :param owner_id: Show only results owned by this user ID.
     :param curation_tier: Show only results of this curation tier.
@@ -39,14 +40,15 @@
     :param gene_id_type: Show only results with this gene ID type.
     :param search_text: Return genesets that match this search text (using PostgreSQL
                         full-text search).
     :param limit: Limit the number of results.
     :param offset: Offset the results.
     :param is_readable_by: A user ID to check if the user can read the results.
     :param with_publication_info: Include publication info in the return.
+    :param ontology_term: Show only results associated with this ontology term.
 
     :return: list of results using `.fetchall()`
     """
     await cursor.execute(
         *geneset_query.get(
             is_readable_by=is_readable_by,
             gs_id=gs_id,
@@ -58,14 +60,15 @@
             publication_id=publication_id,
             pubmed_id=pubmed_id,
             gene_id_type=gene_id_type,
             search_text=search_text,
             limit=limit,
             offset=offset,
             with_publication_info=with_publication_info,
+            ontology_term=ontology_term,
         )
     )
 
     return await cursor.fetchall()
 
 
 async def by_id(
```

### Comparing `geneweaver_db-0.3.8/src/geneweaver/db/aio/publication.py` & `geneweaver_db-0.4.0a0/src/geneweaver/db/aio/publication.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.8/src/geneweaver/db/aio/species.py` & `geneweaver_db-0.4.0a0/src/geneweaver/db/aio/species.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.8/src/geneweaver/db/aio/threshold.py` & `geneweaver_db-0.4.0a0/src/geneweaver/db/aio/threshold.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.8/src/geneweaver/db/core/cursor.py` & `geneweaver_db-0.4.0a0/src/geneweaver/db/core/cursor.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.8/src/geneweaver/db/core/settings_class.py` & `geneweaver_db-0.4.0a0/src/geneweaver/db/core/settings_class.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.8/src/geneweaver/db/gene.py` & `geneweaver_db-0.4.0a0/src/geneweaver/db/gene.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.8/src/geneweaver/db/geneset.py` & `geneweaver_db-0.4.0a0/src/geneweaver/db/geneset.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     publication_id: Optional[int] = None,
     pubmed_id: Optional[int] = None,
     gene_id_type: Optional[GeneIdentifier] = None,
     search_text: Optional[str] = None,
     limit: Optional[int] = None,
     offset: Optional[int] = None,
     with_publication_info: bool = True,
+    ontology_term: Optional[str] = None,
 ) -> List[Row]:
     """Get genesets from the database.
 
     :param cursor: An async database cursor.
     :param is_readable_by: A user ID to check if the user can read the results.
     :param gs_id: Show only results with this geneset ID.
     :param owner_id: Show only results owned by this user ID.
@@ -40,14 +41,15 @@
     :param pubmed_id: Show only results with this PubMed ID.
     :param gene_id_type: Show only results with this gene ID type.
     :param search_text: Return genesets that match this search text (using PostgreSQL
                         full-text search).
     :param limit: Limit the number of results.
     :param offset: Offset the results.
     :param with_publication_info: Include publication info in the return.
+    :param ontology_term: Show only results associated with this ontology term.
 
     :return: list of results using `.fetchall()`
     """
     cursor.execute(
         *geneset_query.get(
             is_readable_by=is_readable_by,
             gs_id=gs_id,
@@ -59,14 +61,15 @@
             publication_id=publication_id,
             pubmed_id=pubmed_id,
             gene_id_type=gene_id_type,
             search_text=search_text,
             limit=limit,
             offset=offset,
             with_publication_info=with_publication_info,
+            ontology_term=ontology_term,
         )
     )
 
     return cursor.fetchall()
 
 
 def by_id(
```

### Comparing `geneweaver_db-0.3.8/src/geneweaver/db/geneset_value.py` & `geneweaver_db-0.4.0a0/src/geneweaver/db/geneset_value.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.8/src/geneweaver/db/publication.py` & `geneweaver_db-0.4.0a0/src/geneweaver/db/publication.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.8/src/geneweaver/db/query/gene.py` & `geneweaver_db-0.4.0a0/src/geneweaver/db/query/gene.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.8/src/geneweaver/db/query/geneset/const.py` & `geneweaver_db-0.4.0a0/src/geneweaver/db/query/geneset/const.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.8/src/geneweaver/db/query/geneset/read.py` & `geneweaver_db-0.4.0a0/src/geneweaver/db/query/geneset/read.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """SQL query generation code for reading genesets."""
 
 from typing import Optional, Tuple
 
 from geneweaver.core.enum import GeneIdentifier, Species
 from geneweaver.db.query.geneset.utils import (
     GenesetTierOrTiers,
+    add_ontology_parameter,
+    add_ontology_query,
     format_select_query,
     is_readable,
     restrict_tier,
     search,
 )
 from geneweaver.db.query.utils import construct_filters
 from geneweaver.db.utils import limit_and_offset
@@ -27,14 +29,15 @@
     gene_id_type: Optional[GeneIdentifier] = None,
     search_text: Optional[str] = None,
     status: Optional[str] = "normal",
     limit: Optional[int] = None,
     offset: Optional[int] = None,
     is_readable_by: Optional[int] = None,
     with_publication_info: bool = True,
+    ontology_term: Optional[str] = None,
 ) -> Tuple[Composed, dict]:
     """Get genesets.
 
     :param gs_id: Show only results with this geneset ID.
     :param owner_id: Show only results owned by this user ID.
     :param curation_tier: Show only results of this curation tier.
     :param species: Show only results associated with this species.
@@ -46,22 +49,32 @@
     :param search_text: Return genesets that match this search text (using PostgreSQL
                         full-text search).
     :param status: Show only results with this status. Default is "normal".
     :param limit: Limit the number of results.
     :param offset: Offset the results.
     :param is_readable_by: A user ID to check if the user can read the results.
     :param with_publication_info: Include publication info in the return.
+    :param ontology_term: Show only results associated with this ontology term.
     """
     params = {}
     filtering = []
     query = format_select_query(
         with_publication_info=with_publication_info,
         with_publication_join=pubmed_id is not None,
     )
 
+    # expand query to include ontology term if needed
+    if ontology_term:
+        query = add_ontology_query(query=query)
+        filtering, params = add_ontology_parameter(
+            existing_filters=filtering,
+            existing_params=params,
+            ontology_term=ontology_term,
+        )
+
     filtering, params = is_readable(filtering, params, is_readable_by)
     filtering, params = search(filtering, params, search_text)
     filtering, params = restrict_tier(filtering, params, curation_tier)
 
     filtering, params = construct_filters(
         filtering,
         params,
```

### Comparing `geneweaver_db-0.3.8/src/geneweaver/db/query/geneset/utils.py` & `geneweaver_db-0.4.0a0/src/geneweaver/db/query/geneset/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -55,14 +55,42 @@
             + SQL("ON geneset.pub_id = publication.pub_id")
         )
     else:
         query = query + SQL(",").join(GENESET_FIELDS) + SQL("FROM geneset")
     return query
 
 
+def add_ontology_query(query: Composed) -> Composed:
+    """Expand geneset query with join to ontology.
+
+    :param query: geneset base query
+    """
+    ontology_query = (
+        query
+        + SQL("JOIN geneset_ontology ON geneset.gs_id = geneset_ontology.gs_id")
+        + SQL("JOIN ontology ON geneset_ontology.ont_id = ontology.ont_id")
+    )
+
+    return ontology_query
+
+
+def add_ontology_parameter(
+    existing_filters: SQLList, existing_params: ParamDict, ontology_term: str
+) -> Tuple[SQLList, ParamDict]:
+    """Add the ontology term filter to the query.
+
+    :param existing_filters: The existing filters.
+    :param existing_params: The existing parameters.
+    :param ontology_term: The ontology term to filter by.
+    """
+    existing_filters.append(SQL("ontology.ont_ref_id IN(%(ontology_term)s)"))
+    existing_params["ontology_term"] = ontology_term
+    return existing_filters, existing_params
+
+
 def is_readable(
     existing_filters: SQLList,
     existing_params: ParamDict,
     is_readable_by: Optional[int] = None,
 ) -> Tuple[SQLList, ParamDict]:
     """Add the is_readable filter to the query.
```

### Comparing `geneweaver_db-0.3.8/src/geneweaver/db/query/geneset/write.py` & `geneweaver_db-0.4.0a0/src/geneweaver/db/query/geneset/write.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.8/src/geneweaver/db/query/project.py` & `geneweaver_db-0.4.0a0/src/geneweaver/db/query/project.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.8/src/geneweaver/db/query/publication.py` & `geneweaver_db-0.4.0a0/src/geneweaver/db/query/publication.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.8/src/geneweaver/db/query/search/utils.py` & `geneweaver_db-0.4.0a0/src/geneweaver/db/query/search/utils.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.8/src/geneweaver/db/query/species.py` & `geneweaver_db-0.4.0a0/src/geneweaver/db/query/species.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.8/src/geneweaver/db/query/threshold.py` & `geneweaver_db-0.4.0a0/src/geneweaver/db/query/threshold.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.8/src/geneweaver/db/query/utils.py` & `geneweaver_db-0.4.0a0/src/geneweaver/db/query/utils.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.8/src/geneweaver/db/species.py` & `geneweaver_db-0.4.0a0/src/geneweaver/db/species.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.8/src/geneweaver/db/threshold.py` & `geneweaver_db-0.4.0a0/src/geneweaver/db/threshold.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.8/src/geneweaver/db/user.py` & `geneweaver_db-0.4.0a0/src/geneweaver/db/user.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.8/src/geneweaver/db/utils.py` & `geneweaver_db-0.4.0a0/src/geneweaver/db/utils.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.8/PKG-INFO` & `geneweaver_db-0.4.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geneweaver-db
-Version: 0.3.8
+Version: 0.4.0a0
 Summary: Database Interaction Services for GeneWeaver
 Home-page: https://thejacksonlaboratory.github.io/geneweaver-docs/
 License: Apache-2.0
 Author: Jax Computational Sciences
 Author-email: cssc@jax.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

