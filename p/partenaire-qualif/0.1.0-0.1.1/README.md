# Comparing `tmp/partenaire-qualif-0.1.0.tar.gz` & `tmp/partenaire-qualif-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "partenaire-qualif-0.1.0.tar", last modified: Fri May 10 13:56:54 2024, max compression
+gzip compressed data, was "partenaire-qualif-0.1.1.tar", last modified: Fri May 10 14:18:00 2024, max compression
```

## Comparing `partenaire-qualif-0.1.0.tar` & `partenaire-qualif-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 13:56:54.939002 partenaire-qualif-0.1.0/
--rw-rw-rw-   0        0        0     1087 2024-05-09 03:19:27.000000 partenaire-qualif-0.1.0/LICENSE
--rw-rw-rw-   0        0        0       30 2024-05-09 04:51:13.000000 partenaire-qualif-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2778 2024-05-10 13:56:54.939002 partenaire-qualif-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2255 2024-05-09 05:01:41.000000 partenaire-qualif-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 13:56:54.905764 partenaire-qualif-0.1.0/partenaire_qualif.egg-info/
--rw-rw-rw-   0        0        0     2778 2024-05-10 13:56:54.000000 partenaire-qualif-0.1.0/partenaire_qualif.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      379 2024-05-10 13:56:54.000000 partenaire-qualif-0.1.0/partenaire_qualif.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 13:56:54.000000 partenaire-qualif-0.1.0/partenaire_qualif.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2024-05-10 13:56:54.000000 partenaire-qualif-0.1.0/partenaire_qualif.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-10 13:56:54.000000 partenaire-qualif-0.1.0/partenaire_qualif.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-10 13:56:54.933407 partenaire-qualif-0.1.0/qualif/
--rw-rw-rw-   0        0        0      101 2024-05-09 04:06:13.000000 partenaire-qualif-0.1.0/qualif/__init__.py
--rw-rw-rw-   0        0        0     8719 2024-05-10 13:50:58.000000 partenaire-qualif-0.1.0/qualif/qualif.py
-drwxrwxrwx   0        0        0        0 2024-05-10 13:56:54.937700 partenaire-qualif-0.1.0/qualif/templates/
--rw-rw-rw-   0        0        0     2182 2024-05-09 06:03:24.000000 partenaire-qualif-0.1.0/qualif/templates/prompt_find_website_template.txt
--rw-rw-rw-   0        0        0     1745 2024-05-10 13:48:49.000000 partenaire-qualif-0.1.0/qualif/templates/prompt_qualification_template.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 13:56:54.939974 partenaire-qualif-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      943 2024-05-10 13:56:43.000000 partenaire-qualif-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 14:18:00.928979 partenaire-qualif-0.1.1/
+-rw-rw-rw-   0        0        0     1087 2024-05-09 03:19:27.000000 partenaire-qualif-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0       30 2024-05-09 04:51:13.000000 partenaire-qualif-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2778 2024-05-10 14:18:00.928979 partenaire-qualif-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2255 2024-05-09 05:01:41.000000 partenaire-qualif-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 14:18:00.897593 partenaire-qualif-0.1.1/partenaire_qualif.egg-info/
+-rw-rw-rw-   0        0        0     2778 2024-05-10 14:18:00.000000 partenaire-qualif-0.1.1/partenaire_qualif.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      379 2024-05-10 14:18:00.000000 partenaire-qualif-0.1.1/partenaire_qualif.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 14:18:00.000000 partenaire-qualif-0.1.1/partenaire_qualif.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2024-05-10 14:18:00.000000 partenaire-qualif-0.1.1/partenaire_qualif.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-10 14:18:00.000000 partenaire-qualif-0.1.1/partenaire_qualif.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 14:18:00.928979 partenaire-qualif-0.1.1/qualif/
+-rw-rw-rw-   0        0        0      101 2024-05-09 04:06:13.000000 partenaire-qualif-0.1.1/qualif/__init__.py
+-rw-rw-rw-   0        0        0     9159 2024-05-10 14:16:58.000000 partenaire-qualif-0.1.1/qualif/qualif.py
+drwxrwxrwx   0        0        0        0 2024-05-10 14:18:00.928979 partenaire-qualif-0.1.1/qualif/templates/
+-rw-rw-rw-   0        0        0     2182 2024-05-09 06:03:24.000000 partenaire-qualif-0.1.1/qualif/templates/prompt_find_website_template.txt
+-rw-rw-rw-   0        0        0     1745 2024-05-10 13:48:49.000000 partenaire-qualif-0.1.1/qualif/templates/prompt_qualification_template.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 14:18:00.928979 partenaire-qualif-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      943 2024-05-10 14:17:47.000000 partenaire-qualif-0.1.1/setup.py
```

### Comparing `partenaire-qualif-0.1.0/LICENSE` & `partenaire-qualif-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `partenaire-qualif-0.1.0/PKG-INFO` & `partenaire-qualif-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: partenaire-qualif
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple tool that automates the qualification of a partner(reseller/integrator/editor) by finding its website, industries, business functions and services.
 Home-page: https://github.com/ymurong/partenaire-qualif.git
 Author: Yanchao MURONG
 Author-email: yanchao.murong@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `partenaire-qualif-0.1.0/README.md` & `partenaire-qualif-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `partenaire-qualif-0.1.0/partenaire_qualif.egg-info/PKG-INFO` & `partenaire-qualif-0.1.1/partenaire_qualif.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: partenaire-qualif
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple tool that automates the qualification of a partner(reseller/integrator/editor) by finding its website, industries, business functions and services.
 Home-page: https://github.com/ymurong/partenaire-qualif.git
 Author: Yanchao MURONG
 Author-email: yanchao.murong@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `partenaire-qualif-0.1.0/qualif/qualif.py` & `partenaire-qualif-0.1.1/qualif/qualif.py`

 * *Files 5% similar despite different names*

```diff
@@ -127,27 +127,44 @@
                 {"role": "system", "content": "Tu es un expert dans la qualification des partenaires indirectes"},
                 {"role": "user", "content": cur_prompt}
             ]
             website = self.complete(messages=messages)
 
         if validators.url(website):
             return website
+        # loop at least
         return None
 
+    def find_website_loop(self, partner_name: str, max_loop=3) -> str | None:
+        """
+        Try to find website for max_loop times, return website if found, otherwise return None.
+        :param partner_name:
+        :param max_loop:
+        :return:
+        """
+        cur_loop = 1
+        website = None
+        while cur_loop <= max_loop:
+            website = self.find_website(partner_name)
+            if website is not None:
+                break
+            cur_loop += 1
+        return website
+
     def qualify(self, partner_name: str) -> json:
         final_result = {}
 
         cur_prompt = self.prompt_qualification.replace('{{Entreprise}}', partner_name)
         messages = [
             {"role": "system", "content": "Tu es un expert dans la qualification des partenaires indirectes"},
             {"role": "user", "content": cur_prompt}
         ]
 
         if self.browsing:
-            website = self.find_website(partner_name)
+            website = self.find_website_loop(partner_name)
             final_result["site_web"] = website
             web_content = None
             try:
                 web_content = Scrapper(url=website).scrape_first_level_content()
             except Exception as e:
                 final_result["site_web"] = "Information non disponible"
 
@@ -183,14 +200,15 @@
                 row["secteurs"] = json_response["Secteur_d_Activite"]
                 row["metier"] = json_response["Metier"]
                 row["offres"] = json_response["Offres"]
                 df_row = row.to_frame().T
                 final_df = pd.concat([final_df, df_row], ignore_index=True)
         return final_df
 
+
 if __name__ == '__main__':
     # Load Data
     df_partenaires = pd.read_excel("../partners_conseil_informatique_6202.xlsx")
     df_partenaires_sample = df_partenaires.sample(n=10, random_state=52)
     df_partenaires_sample
 
     azure_endpoint = "https://chatgpt-dp-innovation-dev.openai.azure.com/"
@@ -202,9 +220,9 @@
     client = AzureOpenAI(
         azure_endpoint=azure_endpoint,
         api_key=apikey,
         api_version=apiversion,
     )
 
     tool = CompanyQualificationTool(client=client, model=model, temperature=0, browsing=True, browsing_key=browsing_key)
-    final_df = tool.batch(df_partners=df_partenaires_sample, col_name_partner="Raison Sociale")
-    final_df.to_excel("../Partenaires_sample_docaposte_with_browsing_integrateurs.xlsx")
+    result = final_df = tool.qualify("APITECH")
+    print(result)
```

### Comparing `partenaire-qualif-0.1.0/qualif/templates/prompt_find_website_template.txt` & `partenaire-qualif-0.1.1/qualif/templates/prompt_find_website_template.txt`

 * *Files identical despite different names*

### Comparing `partenaire-qualif-0.1.0/qualif/templates/prompt_qualification_template.txt` & `partenaire-qualif-0.1.1/qualif/templates/prompt_qualification_template.txt`

 * *Files identical despite different names*

### Comparing `partenaire-qualif-0.1.0/setup.py` & `partenaire-qualif-0.1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="partenaire-qualif",
-    version="0.1.0",
+    version="0.1.1",
     author="Yanchao MURONG",
     author_email="yanchao.murong@gmail.com",
     description="A simple tool that automates the qualification of a partner(reseller/integrator/editor) by finding its website, industries, business functions and services.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ymurong/partenaire-qualif.git",
     packages=setuptools.find_packages(),
```

