# Comparing `tmp/value_nlp-0.1.3.tar.gz` & `tmp/value_nlp-0.1.4.tar.gz`

## Comparing `value_nlp-0.1.3.tar` & `value_nlp-0.1.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 value_nlp-0.1.3/multivalue/resources/adv_adj_degree_modifier.json
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 value_nlp-0.1.3/multivalue/resources/adv_adj_flat.json
--rw-r--r--   0        0        0    49239 2020-02-02 00:00:00.000000 value_nlp-0.1.3/multivalue/resources/attestation_vectors.csv
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 value_nlp-0.1.3/multivalue/resources/benefactive_verbs.txt
--rw-r--r--   0        0        0 10445514 2020-02-02 00:00:00.000000 value_nlp-0.1.3/multivalue/resources/concreteness.csv
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 value_nlp-0.1.3/multivalue/resources/det_plural.json
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 value_nlp-0.1.3/multivalue/resources/det_possessive_obj.json
--rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 value_nlp-0.1.3/multivalue/resources/ditransitive_dobj_verbs.txt
--rw-r--r--   0        0        0  1965318 2020-02-02 00:00:00.000000 value_nlp-0.1.3/multivalue/resources/ewave.csv
--rw-r--r--   0        0        0     5491 2020-02-02 00:00:00.000000 value_nlp-0.1.3/multivalue/resources/feature_id_to_function_name.json
--rw-r--r--   0        0        0    13515 2020-02-02 00:00:00.000000 value_nlp-0.1.3/multivalue/resources/mass_nouns.txt
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 value_nlp-0.1.3/multivalue/resources/modals_past.json
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 value_nlp-0.1.3/multivalue/resources/negatives.json
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 value_nlp-0.1.3/multivalue/resources/negatives_no_more.json
--rw-r--r--   0        0        0   523529 2020-02-02 00:00:00.000000 value_nlp-0.1.3/multivalue/resources/noun_concreteness.json
--rw-r--r--   0        0        0    54083 2020-02-02 00:00:00.000000 value_nlp-0.1.3/multivalue/resources/people_terms.csv
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 value_nlp-0.1.3/multivalue/resources/possessives.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 value_nlp-0.1.3/multivalue/resources/pron_obj_to_subj.json
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 value_nlp-0.1.3/multivalue/resources/reflexives_aave.json
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 value_nlp-0.1.3/multivalue/resources/reflexives_emphatic.json
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 value_nlp-0.1.3/multivalue/resources/reflexives_number_swap.json
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 value_nlp-0.1.3/multivalue/resources/reflexives_obj_pron.json
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 value_nlp-0.1.3/multivalue/resources/reflexives_regularized.json
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 value_nlp-0.1.3/multivalue/resources/reflexives_subj.json
--rw-r--r--   0        0        0    12559 2020-02-02 00:00:00.000000 value_nlp-0.1.3/multivalue/resources/transitive_dobj_verbs.txt
--rw-r--r--   0        0        0    36250 2020-02-02 00:00:00.000000 value_nlp-0.1.3/multivalue/resources/unittests.json
--rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 value_nlp-0.1.3/multivalue/resources/varieties.csv
--rw-r--r--   0        0        0  1296370 2020-02-02 00:00:00.000000 value_nlp-0.1.3/multivalue/resources/verb_transitivity.tsv
--rw-r--r--   0        0        0   148032 2020-02-02 00:00:00.000000 value_nlp-0.1.3/multivalue/BaseDialect.py
--rw-r--r--   0        0        0    13205 2020-02-02 00:00:00.000000 value_nlp-0.1.3/multivalue/Dialects.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 value_nlp-0.1.3/multivalue/__init__.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 value_nlp-0.1.3/multivalue/build_attestation_vectors.py
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 value_nlp-0.1.3/multivalue/build_benefactive_ditransitive_verb_list.py
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 value_nlp-0.1.3/multivalue/build_coqa_value.py
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 value_nlp-0.1.3/multivalue/build_hit_csv.py
--rw-r--r--   0        0        0     6684 2020-02-02 00:00:00.000000 value_nlp-0.1.3/multivalue/build_value.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 value_nlp-0.1.3/multivalue/inflect/__init__.py
--rw-r--r--   0        0        0     6594 2020-02-02 00:00:00.000000 value_nlp-0.1.3/multivalue/inflect/base.py
--rw-r--r--   0        0        0     5561 2020-02-02 00:00:00.000000 value_nlp-0.1.3/multivalue/inflect/english.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 value_nlp-0.1.3/LICENSE
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 value_nlp-0.1.3/README.md
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 value_nlp-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 value_nlp-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 value_nlp-0.1.4/multivalue/resources/adv_adj_degree_modifier.json
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 value_nlp-0.1.4/multivalue/resources/adv_adj_flat.json
+-rw-r--r--   0        0        0    49239 2020-02-02 00:00:00.000000 value_nlp-0.1.4/multivalue/resources/attestation_vectors.csv
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 value_nlp-0.1.4/multivalue/resources/benefactive_verbs.txt
+-rw-r--r--   0        0        0 10445514 2020-02-02 00:00:00.000000 value_nlp-0.1.4/multivalue/resources/concreteness.csv
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 value_nlp-0.1.4/multivalue/resources/det_plural.json
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 value_nlp-0.1.4/multivalue/resources/det_possessive_obj.json
+-rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 value_nlp-0.1.4/multivalue/resources/ditransitive_dobj_verbs.txt
+-rw-r--r--   0        0        0  1965318 2020-02-02 00:00:00.000000 value_nlp-0.1.4/multivalue/resources/ewave.csv
+-rw-r--r--   0        0        0     5491 2020-02-02 00:00:00.000000 value_nlp-0.1.4/multivalue/resources/feature_id_to_function_name.json
+-rw-r--r--   0        0        0    13515 2020-02-02 00:00:00.000000 value_nlp-0.1.4/multivalue/resources/mass_nouns.txt
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 value_nlp-0.1.4/multivalue/resources/modals_past.json
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 value_nlp-0.1.4/multivalue/resources/negatives.json
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 value_nlp-0.1.4/multivalue/resources/negatives_no_more.json
+-rw-r--r--   0        0        0   523529 2020-02-02 00:00:00.000000 value_nlp-0.1.4/multivalue/resources/noun_concreteness.json
+-rw-r--r--   0        0        0    54083 2020-02-02 00:00:00.000000 value_nlp-0.1.4/multivalue/resources/people_terms.csv
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 value_nlp-0.1.4/multivalue/resources/possessives.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 value_nlp-0.1.4/multivalue/resources/pron_obj_to_subj.json
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 value_nlp-0.1.4/multivalue/resources/reflexives_aave.json
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 value_nlp-0.1.4/multivalue/resources/reflexives_emphatic.json
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 value_nlp-0.1.4/multivalue/resources/reflexives_number_swap.json
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 value_nlp-0.1.4/multivalue/resources/reflexives_obj_pron.json
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 value_nlp-0.1.4/multivalue/resources/reflexives_regularized.json
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 value_nlp-0.1.4/multivalue/resources/reflexives_subj.json
+-rw-r--r--   0        0        0    12559 2020-02-02 00:00:00.000000 value_nlp-0.1.4/multivalue/resources/transitive_dobj_verbs.txt
+-rw-r--r--   0        0        0    36250 2020-02-02 00:00:00.000000 value_nlp-0.1.4/multivalue/resources/unittests.json
+-rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 value_nlp-0.1.4/multivalue/resources/varieties.csv
+-rw-r--r--   0        0        0  1296370 2020-02-02 00:00:00.000000 value_nlp-0.1.4/multivalue/resources/verb_transitivity.tsv
+-rw-r--r--   0        0        0   148032 2020-02-02 00:00:00.000000 value_nlp-0.1.4/multivalue/BaseDialect.py
+-rw-r--r--   0        0        0    13205 2020-02-02 00:00:00.000000 value_nlp-0.1.4/multivalue/Dialects.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 value_nlp-0.1.4/multivalue/__init__.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 value_nlp-0.1.4/multivalue/build_attestation_vectors.py
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 value_nlp-0.1.4/multivalue/build_benefactive_ditransitive_verb_list.py
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 value_nlp-0.1.4/multivalue/build_coqa_value.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 value_nlp-0.1.4/multivalue/build_hit_csv.py
+-rw-r--r--   0        0        0     6684 2020-02-02 00:00:00.000000 value_nlp-0.1.4/multivalue/build_value.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 value_nlp-0.1.4/multivalue/inflect/__init__.py
+-rw-r--r--   0        0        0     6594 2020-02-02 00:00:00.000000 value_nlp-0.1.4/multivalue/inflect/base.py
+-rw-r--r--   0        0        0     5561 2020-02-02 00:00:00.000000 value_nlp-0.1.4/multivalue/inflect/english.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 value_nlp-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 value_nlp-0.1.4/README.md
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 value_nlp-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 value_nlp-0.1.4/PKG-INFO
```

### Comparing `value_nlp-0.1.3/multivalue/resources/adv_adj_flat.json` & `value_nlp-0.1.4/multivalue/resources/adv_adj_flat.json`

 * *Files identical despite different names*

### Comparing `value_nlp-0.1.3/multivalue/resources/attestation_vectors.csv` & `value_nlp-0.1.4/multivalue/resources/attestation_vectors.csv`

 * *Files identical despite different names*

### Comparing `value_nlp-0.1.3/multivalue/resources/benefactive_verbs.txt` & `value_nlp-0.1.4/multivalue/resources/benefactive_verbs.txt`

 * *Files identical despite different names*

### Comparing `value_nlp-0.1.3/multivalue/resources/concreteness.csv` & `value_nlp-0.1.4/multivalue/resources/concreteness.csv`

 * *Files identical despite different names*

### Comparing `value_nlp-0.1.3/multivalue/resources/ditransitive_dobj_verbs.txt` & `value_nlp-0.1.4/multivalue/resources/ditransitive_dobj_verbs.txt`

 * *Files identical despite different names*

### Comparing `value_nlp-0.1.3/multivalue/resources/ewave.csv` & `value_nlp-0.1.4/multivalue/resources/ewave.csv`

 * *Files identical despite different names*

### Comparing `value_nlp-0.1.3/multivalue/resources/feature_id_to_function_name.json` & `value_nlp-0.1.4/multivalue/resources/feature_id_to_function_name.json`

 * *Files identical despite different names*

### Comparing `value_nlp-0.1.3/multivalue/resources/mass_nouns.txt` & `value_nlp-0.1.4/multivalue/resources/mass_nouns.txt`

 * *Files identical despite different names*

### Comparing `value_nlp-0.1.3/multivalue/resources/noun_concreteness.json` & `value_nlp-0.1.4/multivalue/resources/noun_concreteness.json`

 * *Files identical despite different names*

### Comparing `value_nlp-0.1.3/multivalue/resources/people_terms.csv` & `value_nlp-0.1.4/multivalue/resources/people_terms.csv`

 * *Files identical despite different names*

### Comparing `value_nlp-0.1.3/multivalue/resources/transitive_dobj_verbs.txt` & `value_nlp-0.1.4/multivalue/resources/transitive_dobj_verbs.txt`

 * *Files identical despite different names*

### Comparing `value_nlp-0.1.3/multivalue/resources/unittests.json` & `value_nlp-0.1.4/multivalue/resources/unittests.json`

 * *Files identical despite different names*

### Comparing `value_nlp-0.1.3/multivalue/resources/varieties.csv` & `value_nlp-0.1.4/multivalue/resources/varieties.csv`

 * *Files identical despite different names*

### Comparing `value_nlp-0.1.3/multivalue/resources/verb_transitivity.tsv` & `value_nlp-0.1.4/multivalue/resources/verb_transitivity.tsv`

 * *Files identical despite different names*

### Comparing `value_nlp-0.1.3/multivalue/BaseDialect.py` & `value_nlp-0.1.4/multivalue/BaseDialect.py`

 * *Files identical despite different names*

### Comparing `value_nlp-0.1.3/multivalue/Dialects.py` & `value_nlp-0.1.4/multivalue/Dialects.py`

 * *Files identical despite different names*

### Comparing `value_nlp-0.1.3/multivalue/build_attestation_vectors.py` & `value_nlp-0.1.4/multivalue/build_attestation_vectors.py`

 * *Files identical despite different names*

### Comparing `value_nlp-0.1.3/multivalue/build_benefactive_ditransitive_verb_list.py` & `value_nlp-0.1.4/multivalue/build_benefactive_ditransitive_verb_list.py`

 * *Files identical despite different names*

### Comparing `value_nlp-0.1.3/multivalue/build_coqa_value.py` & `value_nlp-0.1.4/multivalue/build_coqa_value.py`

 * *Files identical despite different names*

### Comparing `value_nlp-0.1.3/multivalue/build_hit_csv.py` & `value_nlp-0.1.4/multivalue/build_hit_csv.py`

 * *Files identical despite different names*

### Comparing `value_nlp-0.1.3/multivalue/build_value.py` & `value_nlp-0.1.4/multivalue/build_value.py`

 * *Files identical despite different names*

### Comparing `value_nlp-0.1.3/multivalue/inflect/base.py` & `value_nlp-0.1.4/multivalue/inflect/base.py`

 * *Files identical despite different names*

### Comparing `value_nlp-0.1.3/multivalue/inflect/english.py` & `value_nlp-0.1.4/multivalue/inflect/english.py`

 * *Files identical despite different names*

### Comparing `value_nlp-0.1.3/LICENSE` & `value_nlp-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `value_nlp-0.1.3/pyproject.toml` & `value_nlp-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "value-nlp"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   {name="Will Held", email="wheld3@gatech.edu"},
   {name="Caleb Ziems", email="cjziems@stanford.edu"}
 ]
 description = "A Framework for Cross-Dialectal NLP"
 readme = "README.md"
 requires-python = ">=3.10"
```

