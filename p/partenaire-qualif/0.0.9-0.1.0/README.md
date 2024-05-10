# Comparing `tmp/partenaire-qualif-0.0.9.tar.gz` & `tmp/partenaire-qualif-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "partenaire-qualif-0.0.9.tar", last modified: Thu May  9 06:11:48 2024, max compression
+gzip compressed data, was "partenaire-qualif-0.1.0.tar", last modified: Fri May 10 13:56:54 2024, max compression
```

## Comparing `partenaire-qualif-0.0.9.tar` & `partenaire-qualif-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 06:11:48.654535 partenaire-qualif-0.0.9/
--rw-rw-rw-   0        0        0     1087 2024-05-09 03:19:27.000000 partenaire-qualif-0.0.9/LICENSE
--rw-rw-rw-   0        0        0       30 2024-05-09 04:51:13.000000 partenaire-qualif-0.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0     2778 2024-05-09 06:11:48.654535 partenaire-qualif-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     2255 2024-05-09 05:01:41.000000 partenaire-qualif-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 06:11:48.622097 partenaire-qualif-0.0.9/partenaire_qualif.egg-info/
--rw-rw-rw-   0        0        0     2778 2024-05-09 06:11:48.000000 partenaire-qualif-0.0.9/partenaire_qualif.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      379 2024-05-09 06:11:48.000000 partenaire-qualif-0.0.9/partenaire_qualif.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 06:11:48.000000 partenaire-qualif-0.0.9/partenaire_qualif.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2024-05-09 06:11:48.000000 partenaire-qualif-0.0.9/partenaire_qualif.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-09 06:11:48.000000 partenaire-qualif-0.0.9/partenaire_qualif.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-09 06:11:48.649804 partenaire-qualif-0.0.9/qualif/
--rw-rw-rw-   0        0        0      101 2024-05-09 04:06:13.000000 partenaire-qualif-0.0.9/qualif/__init__.py
--rw-rw-rw-   0        0        0     7809 2024-05-09 06:07:58.000000 partenaire-qualif-0.0.9/qualif/qualif.py
-drwxrwxrwx   0        0        0        0 2024-05-09 06:11:48.652455 partenaire-qualif-0.0.9/qualif/templates/
--rw-rw-rw-   0        0        0     2182 2024-05-09 06:03:24.000000 partenaire-qualif-0.0.9/qualif/templates/prompt_find_website_template.txt
--rw-rw-rw-   0        0        0     1747 2024-05-09 03:11:23.000000 partenaire-qualif-0.0.9/qualif/templates/prompt_qualification_template.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 06:11:48.655461 partenaire-qualif-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      943 2024-05-09 06:10:46.000000 partenaire-qualif-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:56:54.939002 partenaire-qualif-0.1.0/
+-rw-rw-rw-   0        0        0     1087 2024-05-09 03:19:27.000000 partenaire-qualif-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0       30 2024-05-09 04:51:13.000000 partenaire-qualif-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2778 2024-05-10 13:56:54.939002 partenaire-qualif-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2255 2024-05-09 05:01:41.000000 partenaire-qualif-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 13:56:54.905764 partenaire-qualif-0.1.0/partenaire_qualif.egg-info/
+-rw-rw-rw-   0        0        0     2778 2024-05-10 13:56:54.000000 partenaire-qualif-0.1.0/partenaire_qualif.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      379 2024-05-10 13:56:54.000000 partenaire-qualif-0.1.0/partenaire_qualif.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 13:56:54.000000 partenaire-qualif-0.1.0/partenaire_qualif.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2024-05-10 13:56:54.000000 partenaire-qualif-0.1.0/partenaire_qualif.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-10 13:56:54.000000 partenaire-qualif-0.1.0/partenaire_qualif.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 13:56:54.933407 partenaire-qualif-0.1.0/qualif/
+-rw-rw-rw-   0        0        0      101 2024-05-09 04:06:13.000000 partenaire-qualif-0.1.0/qualif/__init__.py
+-rw-rw-rw-   0        0        0     8719 2024-05-10 13:50:58.000000 partenaire-qualif-0.1.0/qualif/qualif.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:56:54.937700 partenaire-qualif-0.1.0/qualif/templates/
+-rw-rw-rw-   0        0        0     2182 2024-05-09 06:03:24.000000 partenaire-qualif-0.1.0/qualif/templates/prompt_find_website_template.txt
+-rw-rw-rw-   0        0        0     1745 2024-05-10 13:48:49.000000 partenaire-qualif-0.1.0/qualif/templates/prompt_qualification_template.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 13:56:54.939974 partenaire-qualif-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      943 2024-05-10 13:56:43.000000 partenaire-qualif-0.1.0/setup.py
```

### Comparing `partenaire-qualif-0.0.9/LICENSE` & `partenaire-qualif-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `partenaire-qualif-0.0.9/PKG-INFO` & `partenaire-qualif-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: partenaire-qualif
-Version: 0.0.9
+Version: 0.1.0
 Summary: A simple tool that automates the qualification of a partner(reseller/integrator/editor) by finding its website, industries, business functions and services.
 Home-page: https://github.com/ymurong/partenaire-qualif.git
 Author: Yanchao MURONG
 Author-email: yanchao.murong@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `partenaire-qualif-0.0.9/README.md` & `partenaire-qualif-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `partenaire-qualif-0.0.9/partenaire_qualif.egg-info/PKG-INFO` & `partenaire-qualif-0.1.0/partenaire_qualif.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: partenaire-qualif
-Version: 0.0.9
+Version: 0.1.0
 Summary: A simple tool that automates the qualification of a partner(reseller/integrator/editor) by finding its website, industries, business functions and services.
 Home-page: https://github.com/ymurong/partenaire-qualif.git
 Author: Yanchao MURONG
 Author-email: yanchao.murong@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `partenaire-qualif-0.0.9/qualif/qualif.py` & `partenaire-qualif-0.1.0/qualif/qualif.py`

 * *Files 14% similar despite different names*

```diff
@@ -164,25 +164,47 @@
             return final_result
         return response
 
     def batch(self, df_partners: pd.DataFrame, col_name_partner: str) -> pd.DataFrame:
         """
         :param df_partenaires: original panda dataframe that should contain at least a column of partner names
         :param col_name: the column name of the partner name
-        :return: final_df: enriched panda dataframe that will contain site_web, secteurs, metier, services
+        :return: final_df: enriched panda dataframe that will contain site_web, secteurs, metier, Offres
         """
         # Initialize an empty DataFrame
         start_time = time.time()
         final_df = pd.DataFrame()
         for index, row in tqdm.tqdm(df_partners.iterrows()):
             partner = row[col_name_partner]
             json_response = self.qualify(partner_name=partner)
             if json_response is not None:
                 logger.info(f"--- {time.time() - start_time} seconds --- {partner} ok")
                 if self.browsing:
                     row["site_web"] = json_response["site_web"]
                 row["secteurs"] = json_response["Secteur_d_Activite"]
                 row["metier"] = json_response["Metier"]
-                row["services"] = json_response["Service"]
+                row["offres"] = json_response["Offres"]
                 df_row = row.to_frame().T
                 final_df = pd.concat([final_df, df_row], ignore_index=True)
         return final_df
+
+if __name__ == '__main__':
+    # Load Data
+    df_partenaires = pd.read_excel("../partners_conseil_informatique_6202.xlsx")
+    df_partenaires_sample = df_partenaires.sample(n=10, random_state=52)
+    df_partenaires_sample
+
+    azure_endpoint = "https://chatgpt-dp-innovation-dev.openai.azure.com/"
+    apikey = "58d9c01f9ced46f480a5356bbb6d94da"
+    browsing_key = 'fb37d55b3ffc4ed49015366c0f078907'
+    apiversion = "2024-02-15-preview"
+    model = "smb"
+
+    client = AzureOpenAI(
+        azure_endpoint=azure_endpoint,
+        api_key=apikey,
+        api_version=apiversion,
+    )
+
+    tool = CompanyQualificationTool(client=client, model=model, temperature=0, browsing=True, browsing_key=browsing_key)
+    final_df = tool.batch(df_partners=df_partenaires_sample, col_name_partner="Raison Sociale")
+    final_df.to_excel("../Partenaires_sample_docaposte_with_browsing_integrateurs.xlsx")
```

### Comparing `partenaire-qualif-0.0.9/qualif/templates/prompt_find_website_template.txt` & `partenaire-qualif-0.1.0/qualif/templates/prompt_find_website_template.txt`

 * *Files identical despite different names*

### Comparing `partenaire-qualif-0.0.9/qualif/templates/prompt_qualification_template.txt` & `partenaire-qualif-0.1.0/qualif/templates/prompt_qualification_template.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Vous recevrez une entreprise qui opère en tant que revendeur, intégrateur de systèmes, ou éditeur de logiciels.
 
-Votre tâche est de qualifier l'entreprise en identifiant les secteurs d'activité dans lesquels elle opère, les fonctions d'affaires dans lesquelles elle se spécialise, et les services qu'elle offre.
+Votre tâche est de qualifier l'entreprise en identifiant les secteurs d'activité dans lesquels elle opère, les fonctions d'affaires dans lesquelles elle se spécialise, et les offres qu'elle propose.
 
 
 Voici des exemples non exhaustifs des secteurs, des métier et des services :
 
 Secteur_d_Activite : immobilier, assurance, santé, commerce de gros, telecom, etc.
 Metier : RH, Marketing, Commerce, Gestion de Projet, Gestion de Connaissance, Relation Client, Communication, Production, Conception, Finance/Comptabilité, Autre
-Service : dématérialisation de la paie, dématérialisation des factures, signature électronique, cybersécurité, etc.
+Offres : dématérialisation de la paie, dématérialisation des factures, signature électronique, cybersécurité, etc.
 
 La réponse doit être concise et fournie au format JSON. Si vous les connaissez pas, mettre information non disponible.
 
 Voici un shot d'exemple:
 
 Nom d'Entreprise: Sopra Steria
 Réponse:
@@ -29,15 +29,15 @@
     "Transport"
   ],
   "Metier": [
     "Finance et Administration",
     "RH",
     "Service Client"
   ],
-  "Service": [
+  "Offres": [
     "Conseil",
     "Intelligence Artificielle",
     "Services Technologiques",
     "Intégration de Systèmes",
     "Développement de Logiciels",
     "Services de Processus d'Affaires",
     "Gestion d'Infrastructure",
```

### Comparing `partenaire-qualif-0.0.9/setup.py` & `partenaire-qualif-0.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="partenaire-qualif",
-    version="0.0.9",
+    version="0.1.0",
     author="Yanchao MURONG",
     author_email="yanchao.murong@gmail.com",
     description="A simple tool that automates the qualification of a partner(reseller/integrator/editor) by finding its website, industries, business functions and services.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ymurong/partenaire-qualif.git",
     packages=setuptools.find_packages(),
```

