# Comparing `tmp/docmesh-0.0.2.tar.gz` & `tmp/docmesh-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docmesh-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "docmesh-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `docmesh-0.0.2.tar` & `docmesh-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0       10 2024-05-09 08:25:56.266488 docmesh-0.0.2/README.md
--rw-r--r--   0        0        0       22 2024-05-09 09:53:55.978803 docmesh-0.0.2/docmesh/__init__.py
--rw-r--r--   0        0        0      882 2024-05-09 09:23:16.324316 docmesh-0.0.2/docmesh/db/__init__.py
--rw-r--r--   0        0        0     1397 2024-05-09 04:35:40.368345 docmesh-0.0.2/docmesh/db/auth.py
--rw-r--r--   0        0        0     7451 2024-05-09 09:23:16.330585 docmesh-0.0.2/docmesh/db/neo.py
--rw-r--r--   0        0        0     3237 2024-05-09 09:42:14.197261 docmesh-0.0.2/docmesh/main.py
--rw-r--r--   0        0        0       88 2024-05-09 01:46:53.997886 docmesh-0.0.2/docmesh/parser/__init__.py
--rw-r--r--   0        0        0      788 2024-05-09 01:46:54.001608 docmesh-0.0.2/docmesh/parser/output_parser.py
--rw-r--r--   0        0        0      857 2024-05-09 01:46:54.056241 docmesh-0.0.2/docmesh/prompt.py
--rw-r--r--   0        0        0      186 2024-05-09 09:39:35.901101 docmesh-0.0.2/docmesh/toolkit/__init__.py
--rw-r--r--   0        0        0      507 2024-05-09 08:25:56.296406 docmesh-0.0.2/docmesh/toolkit/entity.py
--rw-r--r--   0        0        0      653 2024-05-09 09:23:16.347369 docmesh-0.0.2/docmesh/toolkit/paper.py
--rw-r--r--   0        0        0      431 2024-05-09 09:39:29.458383 docmesh-0.0.2/docmesh/toolkit/recommend.py
--rw-r--r--   0        0        0      569 2024-05-09 09:38:29.753379 docmesh-0.0.2/docmesh/tools/__init__.py
--rw-r--r--   0        0        0      859 2024-05-09 08:25:56.312152 docmesh-0.0.2/docmesh/tools/base.py
--rw-r--r--   0        0        0     2192 2024-05-09 08:25:56.316922 docmesh-0.0.2/docmesh/tools/entity.py
--rw-r--r--   0        0        0     3895 2024-05-09 09:44:23.645514 docmesh-0.0.2/docmesh/tools/graph_tools.py
--rw-r--r--   0        0        0     4001 2024-05-09 09:23:16.357311 docmesh-0.0.2/docmesh/tools/paper.py
--rw-r--r--   0        0        0     2275 2024-05-09 09:37:40.948496 docmesh-0.0.2/docmesh/tools/recommend.py
--rw-r--r--   0        0        0      276 2024-05-09 09:23:16.362731 docmesh-0.0.2/docmesh/utils/__init__.py
--rw-r--r--   0        0        0      269 2024-05-09 01:46:54.041643 docmesh-0.0.2/docmesh/utils/graph_utils.py
--rw-r--r--   0        0        0     3148 2024-05-09 09:23:16.368077 docmesh-0.0.2/docmesh/utils/semantic_scholar.py
--rw-r--r--   0        0        0      885 2024-05-09 10:15:34.124067 docmesh-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      863 1970-01-01 00:00:00.000000 docmesh-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       10 2024-05-09 08:25:56.000000 docmesh-0.0.3/README.md
+-rw-r--r--   0        0        0       22 2024-05-09 14:16:38.605821 docmesh-0.0.3/docmesh/__init__.py
+-rw-r--r--   0        0        0      882 2024-05-09 09:23:16.000000 docmesh-0.0.3/docmesh/db/__init__.py
+-rw-r--r--   0        0        0     1397 2024-05-09 04:35:40.000000 docmesh-0.0.3/docmesh/db/auth.py
+-rw-r--r--   0        0        0     7451 2024-05-09 09:23:16.000000 docmesh-0.0.3/docmesh/db/neo.py
+-rw-r--r--   0        0        0     3242 2024-05-09 13:51:24.046692 docmesh-0.0.3/docmesh/main.py
+-rw-r--r--   0        0        0       88 2024-05-09 01:46:53.000000 docmesh-0.0.3/docmesh/parser/__init__.py
+-rw-r--r--   0        0        0      788 2024-05-09 01:46:54.000000 docmesh-0.0.3/docmesh/parser/output_parser.py
+-rw-r--r--   0        0        0      857 2024-05-09 11:18:10.000000 docmesh-0.0.3/docmesh/prompt.py
+-rw-r--r--   0        0        0      186 2024-05-09 09:39:35.000000 docmesh-0.0.3/docmesh/toolkit/__init__.py
+-rw-r--r--   0        0        0      507 2024-05-09 08:25:56.000000 docmesh-0.0.3/docmesh/toolkit/entity.py
+-rw-r--r--   0        0        0      653 2024-05-09 09:23:16.000000 docmesh-0.0.3/docmesh/toolkit/paper.py
+-rw-r--r--   0        0        0      431 2024-05-09 09:39:29.000000 docmesh-0.0.3/docmesh/toolkit/recommend.py
+-rw-r--r--   0        0        0      569 2024-05-09 09:38:29.000000 docmesh-0.0.3/docmesh/tools/__init__.py
+-rw-r--r--   0        0        0     1104 2024-05-09 11:22:53.000000 docmesh-0.0.3/docmesh/tools/base.py
+-rw-r--r--   0        0        0     2274 2024-05-09 11:40:01.000000 docmesh-0.0.3/docmesh/tools/entity.py
+-rw-r--r--   0        0        0     3895 2024-05-09 09:44:23.000000 docmesh-0.0.3/docmesh/tools/graph_tools.py
+-rw-r--r--   0        0        0     4235 2024-05-09 11:39:28.000000 docmesh-0.0.3/docmesh/tools/paper.py
+-rw-r--r--   0        0        0     2367 2024-05-09 11:15:26.000000 docmesh-0.0.3/docmesh/tools/recommend.py
+-rw-r--r--   0        0        0      276 2024-05-09 09:23:16.000000 docmesh-0.0.3/docmesh/utils/__init__.py
+-rw-r--r--   0        0        0      269 2024-05-09 01:46:54.000000 docmesh-0.0.3/docmesh/utils/graph_utils.py
+-rw-r--r--   0        0        0     3148 2024-05-09 09:23:16.000000 docmesh-0.0.3/docmesh/utils/semantic_scholar.py
+-rw-r--r--   0        0        0      885 2024-05-09 10:22:13.000000 docmesh-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      863 1970-01-01 00:00:00.000000 docmesh-0.0.3/PKG-INFO
```

### Comparing `docmesh-0.0.2/docmesh/db/__init__.py` & `docmesh-0.0.3/docmesh/db/__init__.py`

 * *Files identical despite different names*

### Comparing `docmesh-0.0.2/docmesh/db/auth.py` & `docmesh-0.0.3/docmesh/db/auth.py`

 * *Files identical despite different names*

### Comparing `docmesh-0.0.2/docmesh/db/neo.py` & `docmesh-0.0.3/docmesh/db/neo.py`

 * *Files identical despite different names*

### Comparing `docmesh-0.0.2/docmesh/main.py` & `docmesh-0.0.3/docmesh/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     return {"data": data}
 
 
 def _execute_agent(entity_name: str, query: str, session_id: str) -> str:
     # setup react prompt
     prompt = MEMORY_REACT_PROMPT
     # setup llm
-    llm = ChatOpenAI(model="gpt-4-0125-preview")
+    llm = ChatOpenAI(model=os.getenv("OPENAI_MODEL"))
     # set up all tools
     tools = [
         *EntityToolkit(entity_name=entity_name).get_tools(),
         *PaperToolkit(entity_name=entity_name).get_tools(),
         *RecommendToolkit(entity_name=entity_name).get_tools(),
     ]
     # setup ReAct agent
```

### Comparing `docmesh-0.0.2/docmesh/parser/output_parser.py` & `docmesh-0.0.3/docmesh/parser/output_parser.py`

 * *Files identical despite different names*

### Comparing `docmesh-0.0.2/docmesh/prompt.py` & `docmesh-0.0.3/docmesh/prompt.py`

 * *Files identical despite different names*

### Comparing `docmesh-0.0.2/docmesh/toolkit/paper.py` & `docmesh-0.0.3/docmesh/toolkit/paper.py`

 * *Files identical despite different names*

### Comparing `docmesh-0.0.2/docmesh/tools/__init__.py` & `docmesh-0.0.3/docmesh/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `docmesh-0.0.2/docmesh/tools/base.py` & `docmesh-0.0.3/docmesh/tools/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,20 @@
 from langchain_core.tools import BaseTool
 from langchain_core.tools import ToolException
 
 
 class BaseAgentTool(BaseTool):
     entity_name: str
 
+    def _preporcess_input(self, s: str) -> str:
+        # in some rare case, input may include the keyword
+        # `Observation` in prompt.
+        s = s.strip().replace("Observation:", "").replace("Observation", "").strip()
+        return s
+
     def _raise_tool_error(self, err_msg: str) -> None:
         raise ToolException(err_msg)
 
     def _dataframe_to_msg(self, df: DataFrame) -> str:
         columns = df.columns.to_list()
 
         def _row_to_msg(row: Series) -> str:
```

### Comparing `docmesh-0.0.2/docmesh/tools/entity.py` & `docmesh-0.0.3/docmesh/tools/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     handle_tool_error: bool = True
 
     def _run(
         self,
         name: str,
         run_manager: Optional[CallbackManagerForToolRun] = None,
     ) -> str:
+        name = self._preporcess_input(name)
         follow_entity(self.entity_name, name)
         return f"\nSuccessfully follow entity {name}\n"
 
 
 class ListFollowsTool(BaseAgentNoInputTool):
     name: str = "list_follows"
     description: str = "useful when you need to list all you follows"
@@ -52,14 +53,15 @@
     handle_tool_error: bool = True
 
     def _run(
         self,
         n: str,
         run_manager: Optional[CallbackManagerForToolRun] = None,
     ) -> str:
+        n = self._preporcess_input(n)
         try:
             n = int(n)
         except Exception:
             self._raise_tool_error(
                 "Input argument `n` should be an integer, please check your input. "
                 "Pay attention that you MUST ONLY input the number, like 1, 3, 5.\n"
             )
```

### Comparing `docmesh-0.0.2/docmesh/tools/graph_tools.py` & `docmesh-0.0.3/docmesh/tools/graph_tools.py`

 * *Files identical despite different names*

### Comparing `docmesh-0.0.2/docmesh/tools/paper.py` & `docmesh-0.0.3/docmesh/tools/paper.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     handle_tool_error: bool = True
 
     def _run(
         self,
         title: str,
         run_manager: Optional[CallbackManagerForToolRun] = None,
     ) -> str:
+        title = self._preporcess_input(title)
         try:
             paper = add_paper(title)
         except PaperIdNotFound:
             self._raise_tool_error(f"Cannot find paper id for paper {title}, you may end execution.")
 
         msg = f"Successfully add paper {title} with id {paper.paper_id} into neo4j database."
         return f"\n{msg}\n"
@@ -49,14 +50,15 @@
     handle_tool_error: bool = True
 
     def _run(
         self,
         title: str,
         run_manager: Optional[CallbackManagerForToolRun] = None,
     ) -> str:
+        title = self._preporcess_input(title)
         paper_id = get_paper_from_title(title=title).paper_id
         msg = f"Successfully find paper id {paper_id} for {title}."
         return f"\n{msg}\n"
 
 
 class MarkPaperReadToolInput(BaseModel):
     paper_id: str = Field(description="paper id")
@@ -69,14 +71,15 @@
     handle_tool_error: bool = True
 
     def _run(
         self,
         paper_id: str,
         run_manager: Optional[CallbackManagerForToolRun] = None,
     ) -> str:
+        paper_id = self._preporcess_input(paper_id)
         read_paper(entity_name=self.entity_name, paper_id=paper_id)
         msg = f"Successfully mark paper {paper_id} read."
         return f"\n{msg}\n"
 
 
 class PaperSummaryToolInput(BaseModel):
     paper_id: str = Field(description="paper id")
@@ -91,14 +94,15 @@
     handle_tool_error: bool = True
 
     def _run(
         self,
         paper_id: str,
         run_manager: Optional[CallbackManagerForToolRun] = None,
     ) -> str:
+        paper_id = self._preporcess_input(paper_id)
         paper = get_paper_from_id(paper_id=paper_id)
         msg = paper.summary
         return f"\n{msg}\n"
 
 
 class ListLatestPaperToolInput(BaseModel):
     n: str = Field(description="number of papers")
@@ -114,14 +118,15 @@
     handle_tool_error: bool = True
 
     def _run(
         self,
         n: str,
         run_manager: Optional[CallbackManagerForToolRun] = None,
     ) -> str:
+        n = self._preporcess_input(n)
         try:
             n = int(n)
         except Exception:
             self._raise_tool_error(
                 "Input argument `n` should be an integer, please check your inputt. "
                 "Pay attention that you MUST ONLY input the number, like 1, 3, 5.\n"
             )
```

### Comparing `docmesh-0.0.2/docmesh/tools/recommend.py` & `docmesh-0.0.3/docmesh/tools/recommend.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     handle_tool_error: bool = True
 
     def _run(
         self,
         n: str,
         run_manager: Optional[CallbackManagerForToolRun] = None,
     ) -> str:
+        n = self._preporcess_input(n)
         try:
             n = int(n)
         except Exception:
             self._raise_tool_error(
                 "Input argument `n` should be an integer, please check your inputt. "
                 "Pay attention that you MUST ONLY input the number, like 1, 3, 5.\n"
             )
@@ -50,14 +51,15 @@
     handle_tool_error: bool = True
 
     def _run(
         self,
         date_time: str,
         run_manager: Optional[CallbackManagerForToolRun] = None,
     ) -> str:
+        date_time = self._preporcess_input(date_time)
         try:
             datetime.strptime(date_time, "%Y-%m-%d")
         except Exception:
             self._raise_tool_error(
                 "Input argument `date_time` should be written in format `YYYY-MM-DD`, "
                 "please check your input, valid input can be 1995-03-01, 2024-01-01.\n"
             )
```

### Comparing `docmesh-0.0.2/docmesh/utils/semantic_scholar.py` & `docmesh-0.0.3/docmesh/utils/semantic_scholar.py`

 * *Files identical despite different names*

### Comparing `docmesh-0.0.2/pyproject.toml` & `docmesh-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `docmesh-0.0.2/PKG-INFO` & `docmesh-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docmesh
-Version: 0.0.2
+Version: 0.0.3
 Summary: Agent helps you dig the paper connection!
 Author-email: Zhengkai Yang <kyle.yang1995@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

