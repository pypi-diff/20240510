# Comparing `tmp/marker_pdf-0.2.2.tar.gz` & `tmp/marker_pdf-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marker_pdf-0.2.2.tar", max compression
+gzip compressed data, was "marker_pdf-0.2.4.tar", max compression
```

## Comparing `marker_pdf-0.2.2.tar` & `marker_pdf-0.2.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0    35101 2023-11-16 20:09:42.311962 marker_pdf-0.2.2/LICENSE
--rw-r--r--   0        0        0    13302 2024-05-09 18:42:22.504099 marker_pdf-0.2.2/README.md
--rwxr-xr-x   0        0        0      541 2023-12-19 21:40:35.305844 marker_pdf-0.2.2/chunk_convert.py
--rwxr-xr-x   0        0        0     1151 2024-05-09 16:07:14.765161 marker_pdf-0.2.2/chunk_convert.sh
--rwxr-xr-x   0        0        0     4852 2024-05-09 19:04:27.934570 marker_pdf-0.2.2/convert.py
--rwxr-xr-x   0        0        0     1246 2024-05-08 19:28:45.549038 marker_pdf-0.2.2/convert_single.py
--rw-r--r--   0        0        0     1376 2024-05-09 14:37:06.538810 marker_pdf-0.2.2/marker/benchmark/scoring.py
--rw-r--r--   0        0        0      231 2023-11-13 21:39:41.829455 marker_pdf-0.2.2/marker/cleaners/bullets.py
--rw-r--r--   0        0        0     4405 2024-05-08 17:44:54.251299 marker_pdf-0.2.2/marker/cleaners/code.py
--rw-r--r--   0        0        0      950 2024-05-07 20:26:01.091879 marker_pdf-0.2.2/marker/cleaners/fontstyle.py
--rw-r--r--   0        0        0     2766 2024-05-07 20:26:12.412431 marker_pdf-0.2.2/marker/cleaners/headers.py
--rw-r--r--   0        0        0     2456 2024-05-07 19:20:29.345524 marker_pdf-0.2.2/marker/cleaners/headings.py
--rw-r--r--   0        0        0      248 2024-05-03 21:25:54.927963 marker_pdf-0.2.2/marker/cleaners/text.py
--rw-r--r--   0        0        0     5164 2024-05-09 18:04:24.927228 marker_pdf-0.2.2/marker/convert.py
--rw-r--r--   0        0        0     2450 2024-04-30 19:24:46.032856 marker_pdf-0.2.2/marker/debug/data.py
--rw-r--r--   0        0        0     7884 2024-05-08 19:28:39.435042 marker_pdf-0.2.2/marker/equations/equations.py
--rw-r--r--   0        0        0     1549 2024-05-08 19:28:39.424935 marker_pdf-0.2.2/marker/equations/inference.py
--rw-r--r--   0        0        0     2594 2024-05-07 20:51:37.990183 marker_pdf-0.2.2/marker/images/extract.py
--rw-r--r--   0        0        0      473 2024-05-07 17:35:52.062308 marker_pdf-0.2.2/marker/images/save.py
--rw-r--r--   0        0        0     1928 2024-05-09 17:56:48.915437 marker_pdf-0.2.2/marker/layout/layout.py
--rw-r--r--   0        0        0     2516 2024-05-09 18:50:44.232751 marker_pdf-0.2.2/marker/layout/order.py
--rw-r--r--   0        0        0      396 2024-05-01 20:56:02.059168 marker_pdf-0.2.2/marker/logger.py
--rw-r--r--   0        0        0     2178 2024-05-09 18:19:52.086803 marker_pdf-0.2.2/marker/models.py
--rw-r--r--   0        0        0      888 2024-05-09 17:56:54.611918 marker_pdf-0.2.2/marker/ocr/detection.py
--rw-r--r--   0        0        0     2468 2024-05-07 05:37:29.807989 marker_pdf-0.2.2/marker/ocr/heuristics.py
--rw-r--r--   0        0        0     1223 2024-05-09 18:28:58.770602 marker_pdf-0.2.2/marker/ocr/lang.py
--rw-r--r--   0        0        0     5742 2024-05-09 18:45:41.515716 marker_pdf-0.2.2/marker/ocr/recognition.py
--rw-r--r--   0        0        0     2180 2024-05-01 20:19:00.486329 marker_pdf-0.2.2/marker/ocr/tesseract.py
--rw-r--r--   0        0        0      258 2024-05-02 23:16:18.893143 marker_pdf-0.2.2/marker/ocr/utils.py
--rw-r--r--   0        0        0     1265 2024-05-07 18:48:43.948534 marker_pdf-0.2.2/marker/output.py
--rw-r--r--   0        0        0     3932 2024-05-07 19:36:28.635033 marker_pdf-0.2.2/marker/pdf/extract_text.py
--rw-r--r--   0        0        0      817 2024-05-07 02:48:52.757068 marker_pdf-0.2.2/marker/pdf/images.py
--rw-r--r--   0        0        0     2339 2024-05-07 19:21:25.071249 marker_pdf-0.2.2/marker/pdf/utils.py
--rw-r--r--   0        0        0     3904 2024-05-08 19:28:39.432619 marker_pdf-0.2.2/marker/postprocessors/editor.py
--rw-r--r--   0        0        0     7103 2024-05-09 16:45:38.707953 marker_pdf-0.2.2/marker/postprocessors/markdown.py
--rw-r--r--   0        0        0     4977 2024-05-07 20:27:15.110937 marker_pdf-0.2.2/marker/postprocessors/t5.py
--rw-r--r--   0        0        0     2849 2024-05-03 13:40:49.822158 marker_pdf-0.2.2/marker/schema/bbox.py
--rw-r--r--   0        0        0     3259 2024-05-08 16:58:04.155413 marker_pdf-0.2.2/marker/schema/block.py
--rw-r--r--   0        0        0      502 2024-05-02 20:26:11.294687 marker_pdf-0.2.2/marker/schema/merged.py
--rw-r--r--   0        0        0     1618 2024-05-08 17:45:07.502133 marker_pdf-0.2.2/marker/schema/page.py
--rw-r--r--   0        0        0     4236 2024-05-09 18:50:32.918877 marker_pdf-0.2.2/marker/settings.py
--rw-r--r--   0        0        0     3384 2024-05-07 19:20:29.343760 marker_pdf-0.2.2/marker/tables/cells.py
--rw-r--r--   0        0        0     7178 2024-05-08 02:12:14.849108 marker_pdf-0.2.2/marker/tables/table.py
--rw-r--r--   0        0        0     1128 2024-05-07 05:24:59.879003 marker_pdf-0.2.2/marker/tables/utils.py
--rw-r--r--   0        0        0      156 2024-05-09 17:43:20.364396 marker_pdf-0.2.2/marker/utils.py
--rw-r--r--   0        0        0     1319 2024-05-09 18:02:48.805156 marker_pdf-0.2.2/pyproject.toml
--rw-r--r--   0        0        0    14833 1970-01-01 00:00:00.000000 marker_pdf-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35101 2023-11-16 20:09:42.311962 marker_pdf-0.2.4/LICENSE
+-rw-r--r--   0        0        0    13304 2024-05-09 20:17:26.733428 marker_pdf-0.2.4/README.md
+-rwxr-xr-x   0        0        0      638 2024-05-09 20:17:26.734062 marker_pdf-0.2.4/chunk_convert.py
+-rwxr-xr-x   0        0        0     1151 2024-05-09 20:17:26.734330 marker_pdf-0.2.4/chunk_convert.sh
+-rwxr-xr-x   0        0        0     4853 2024-05-09 20:17:26.734670 marker_pdf-0.2.4/convert.py
+-rwxr-xr-x   0        0        0     1246 2024-05-09 20:17:26.735061 marker_pdf-0.2.4/convert_single.py
+-rw-r--r--   0        0        0     1376 2024-05-09 20:17:26.742233 marker_pdf-0.2.4/marker/benchmark/scoring.py
+-rw-r--r--   0        0        0      231 2023-11-13 21:39:41.829455 marker_pdf-0.2.4/marker/cleaners/bullets.py
+-rw-r--r--   0        0        0     4457 2024-05-09 20:17:26.742423 marker_pdf-0.2.4/marker/cleaners/code.py
+-rw-r--r--   0        0        0      950 2024-05-09 20:17:26.742652 marker_pdf-0.2.4/marker/cleaners/fontstyle.py
+-rw-r--r--   0        0        0     2766 2024-05-09 20:17:26.742873 marker_pdf-0.2.4/marker/cleaners/headers.py
+-rw-r--r--   0        0        0     2456 2024-05-09 20:17:26.743108 marker_pdf-0.2.4/marker/cleaners/headings.py
+-rw-r--r--   0        0        0      248 2024-05-09 20:17:26.743362 marker_pdf-0.2.4/marker/cleaners/text.py
+-rw-r--r--   0        0        0     5164 2024-05-09 20:17:26.743631 marker_pdf-0.2.4/marker/convert.py
+-rw-r--r--   0        0        0     2450 2024-05-09 20:17:26.744114 marker_pdf-0.2.4/marker/debug/data.py
+-rw-r--r--   0        0        0     7884 2024-05-09 20:17:26.744427 marker_pdf-0.2.4/marker/equations/equations.py
+-rw-r--r--   0        0        0     1549 2024-05-09 20:17:26.744703 marker_pdf-0.2.4/marker/equations/inference.py
+-rw-r--r--   0        0        0     2594 2024-05-09 20:17:26.745380 marker_pdf-0.2.4/marker/images/extract.py
+-rw-r--r--   0        0        0      473 2024-05-09 20:17:26.745752 marker_pdf-0.2.4/marker/images/save.py
+-rw-r--r--   0        0        0     1928 2024-05-09 20:17:26.745936 marker_pdf-0.2.4/marker/layout/layout.py
+-rw-r--r--   0        0        0     2516 2024-05-09 20:17:26.746215 marker_pdf-0.2.4/marker/layout/order.py
+-rw-r--r--   0        0        0      396 2024-05-09 20:17:26.746551 marker_pdf-0.2.4/marker/logger.py
+-rw-r--r--   0        0        0     2178 2024-05-09 20:17:26.746894 marker_pdf-0.2.4/marker/models.py
+-rw-r--r--   0        0        0      888 2024-05-09 20:17:26.747116 marker_pdf-0.2.4/marker/ocr/detection.py
+-rw-r--r--   0        0        0     2468 2024-05-09 20:17:26.747490 marker_pdf-0.2.4/marker/ocr/heuristics.py
+-rw-r--r--   0        0        0     1223 2024-05-09 20:17:26.747721 marker_pdf-0.2.4/marker/ocr/lang.py
+-rw-r--r--   0        0        0     5742 2024-05-09 20:17:26.747923 marker_pdf-0.2.4/marker/ocr/recognition.py
+-rw-r--r--   0        0        0     2180 2024-05-09 20:17:26.748160 marker_pdf-0.2.4/marker/ocr/tesseract.py
+-rw-r--r--   0        0        0      258 2024-05-09 20:17:26.748548 marker_pdf-0.2.4/marker/ocr/utils.py
+-rw-r--r--   0        0        0     1266 2024-05-09 20:17:26.748771 marker_pdf-0.2.4/marker/output.py
+-rw-r--r--   0        0        0     3932 2024-05-09 20:17:26.748932 marker_pdf-0.2.4/marker/pdf/extract_text.py
+-rw-r--r--   0        0        0      817 2024-05-09 20:17:26.749637 marker_pdf-0.2.4/marker/pdf/images.py
+-rw-r--r--   0        0        0     2442 2024-05-09 20:17:26.749816 marker_pdf-0.2.4/marker/pdf/utils.py
+-rw-r--r--   0        0        0     3904 2024-05-09 20:17:26.750026 marker_pdf-0.2.4/marker/postprocessors/editor.py
+-rw-r--r--   0        0        0     7226 2024-05-09 20:17:26.750172 marker_pdf-0.2.4/marker/postprocessors/markdown.py
+-rw-r--r--   0        0        0     4977 2024-05-09 20:17:26.750386 marker_pdf-0.2.4/marker/postprocessors/t5.py
+-rw-r--r--   0        0        0     2849 2024-05-09 20:17:26.750639 marker_pdf-0.2.4/marker/schema/bbox.py
+-rw-r--r--   0        0        0     3259 2024-05-09 20:17:26.751094 marker_pdf-0.2.4/marker/schema/block.py
+-rw-r--r--   0        0        0      502 2024-05-09 20:17:26.751365 marker_pdf-0.2.4/marker/schema/merged.py
+-rw-r--r--   0        0        0     1618 2024-05-09 20:17:26.751528 marker_pdf-0.2.4/marker/schema/page.py
+-rw-r--r--   0        0        0     4238 2024-05-09 20:17:26.751699 marker_pdf-0.2.4/marker/settings.py
+-rw-r--r--   0        0        0     3384 2024-05-09 20:17:26.751922 marker_pdf-0.2.4/marker/tables/cells.py
+-rw-r--r--   0        0        0     7178 2024-05-09 20:17:26.752162 marker_pdf-0.2.4/marker/tables/table.py
+-rw-r--r--   0        0        0     1128 2024-05-09 20:17:26.752402 marker_pdf-0.2.4/marker/tables/utils.py
+-rw-r--r--   0        0        0      156 2024-05-09 20:17:26.752684 marker_pdf-0.2.4/marker/utils.py
+-rw-r--r--   0        0        0     1338 2024-05-09 20:17:26.754195 marker_pdf-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0    14875 1970-01-01 00:00:00.000000 marker_pdf-0.2.4/PKG-INFO
```

### Comparing `marker_pdf-0.2.2/LICENSE` & `marker_pdf-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.2/README.md` & `marker_pdf-0.2.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 | [Multi-column CNN](https://arxiv.org/pdf/1804.07821.pdf)              | arXiv paper | [View](https://github.com/VikParuchuri/marker/blob/master/data/examples/marker/multicolcnn.md)         | [View](https://github.com/VikParuchuri/marker/blob/master/data/examples/nougat/multicolcnn.md)         |
 
 
 ## Performance
 
 ![Benchmark overall](data/images/overall.png)
 
-The above results are with marker and nougat setup so they each take ~3GB of VRAM on an A6000.
+The above results are with marker and nougat setup so they each take ~4GB of VRAM on an A6000.
 
 See [below](#benchmarks) for detailed speed and accuracy benchmarks, and instructions on how to run your own benchmarks.
 
 # Community
 
 [Discord](https://discord.gg//KuZwXNGnfH) is where we discuss future development.
 
@@ -174,15 +174,15 @@
 | marker | 0.536176        | 0.516833         | 0.70515         | 0.710657    | 0.690042     | 0.523467  |
 | nougat | 0.44009         | 0.588973         | 0.322706        | 0.401342    | 0.160842     | 0.525663  |
 
 Peak GPU memory usage during the benchmark is `4.2GB` for nougat, and `4.1GB` for marker.  Benchmarks were run on an A6000 Ada.
 
 **Throughput**
 
-Marker takes about 4GB of VRAM on average per task, so you can convert 12 documents in parallel on an A6000.
+Marker takes about 4.5GB of VRAM on average per task, so you can convert 10 documents in parallel on an A6000.
 
 ![Benchmark results](data/images/per_doc.png)
 
 ## Running your own benchmarks
 
 You can benchmark the performance of marker on your machine. Install marker manually with:
```

### Comparing `marker_pdf-0.2.2/chunk_convert.sh` & `marker_pdf-0.2.4/chunk_convert.sh`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.2/convert.py` & `marker_pdf-0.2.4/convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 
 @ray.remote(num_cpus=settings.RAY_CORES_PER_WORKER, num_gpus=.05 if settings.CUDA else 0)
 def process_single_pdf(filepath: str, out_folder: str, model_refs, metadata: Optional[Dict] = None, min_length: Optional[int] = None):
     fname = os.path.basename(filepath)
     if markdown_exists(out_folder, fname):
         return
+
     try:
         # Skip trying to convert files that don't have a lot of embedded text
         # This can indicate that they were scanned, and not OCRed properly
         # Usually these files are not recent/high-quality
         if min_length:
             filetype = find_filetype(filepath)
             if filetype == "other":
```

### Comparing `marker_pdf-0.2.2/convert_single.py` & `marker_pdf-0.2.4/convert_single.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.2/marker/benchmark/scoring.py` & `marker_pdf-0.2.4/marker/benchmark/scoring.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.2/marker/cleaners/code.py` & `marker_pdf-0.2.4/marker/cleaners/code.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,21 +63,21 @@
 
                 is_indent.append(line.bbox[0] > min_start)
 
             comment_lines = comment_count([line.prelim_text for line in block.lines])
             is_code = [
                 len(block.lines) > 3,
                 is_code_linelen(block.lines),
-                sum(is_indent) + comment_lines > len(block.lines) * .3,
+                sum(is_indent) + comment_lines > len(block.lines) * .7, # Indentation and comments are a majority
             ]
 
             if avg_font_size is not None:
                 font_checks = [
-                    mean(line_font_sizes) <= avg_font_size, # Lower than average font size and line height
-                    mean(block_line_heights) < avg_line_height
+                    mean(line_font_sizes) <= avg_font_size * .8, # Lower than average font size and line height
+                    mean(block_line_heights) < avg_line_height * .8
                 ]
                 is_code += font_checks
 
             if all(is_code):
                 code_block_count += 1
                 block.block_type = "Code"
```

### Comparing `marker_pdf-0.2.2/marker/cleaners/fontstyle.py` & `marker_pdf-0.2.4/marker/cleaners/fontstyle.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.2/marker/cleaners/headers.py` & `marker_pdf-0.2.4/marker/cleaners/headers.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.2/marker/cleaners/headings.py` & `marker_pdf-0.2.4/marker/cleaners/headings.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.2/marker/convert.py` & `marker_pdf-0.2.4/marker/convert.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.2/marker/debug/data.py` & `marker_pdf-0.2.4/marker/debug/data.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.2/marker/equations/equations.py` & `marker_pdf-0.2.4/marker/equations/equations.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.2/marker/equations/inference.py` & `marker_pdf-0.2.4/marker/equations/inference.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.2/marker/images/extract.py` & `marker_pdf-0.2.4/marker/images/extract.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.2/marker/layout/layout.py` & `marker_pdf-0.2.4/marker/layout/layout.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.2/marker/layout/order.py` & `marker_pdf-0.2.4/marker/layout/order.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.2/marker/models.py` & `marker_pdf-0.2.4/marker/models.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.2/marker/ocr/detection.py` & `marker_pdf-0.2.4/marker/ocr/detection.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.2/marker/ocr/heuristics.py` & `marker_pdf-0.2.4/marker/ocr/heuristics.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.2/marker/ocr/lang.py` & `marker_pdf-0.2.4/marker/ocr/lang.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.2/marker/ocr/recognition.py` & `marker_pdf-0.2.4/marker/ocr/recognition.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.2/marker/ocr/tesseract.py` & `marker_pdf-0.2.4/marker/ocr/tesseract.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.2/marker/output.py` & `marker_pdf-0.2.4/marker/output.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 import json
 
 
 def get_subfolder_path(out_folder, fname):
     subfolder_name = fname.split(".")[0]
     subfolder_path = os.path.join(out_folder, subfolder_name)
-    os.makedirs(subfolder_path, exist_ok=True)
     return subfolder_path
 
 
 def get_markdown_filepath(out_folder, fname):
     subfolder_path = get_subfolder_path(out_folder, fname)
     out_filename = fname.rsplit(".", 1)[0] + ".md"
     out_filename = os.path.join(subfolder_path, out_filename)
@@ -19,14 +18,16 @@
 def markdown_exists(out_folder, fname):
     out_filename = get_markdown_filepath(out_folder, fname)
     return os.path.exists(out_filename)
 
 
 def save_markdown(out_folder, fname, full_text, images, out_metadata):
     subfolder_path = get_subfolder_path(out_folder, fname)
+    os.makedirs(subfolder_path, exist_ok=True)
+
     markdown_filepath = get_markdown_filepath(out_folder, fname)
     out_meta_filepath = markdown_filepath.rsplit(".", 1)[0] + "_meta.json"
 
     with open(markdown_filepath, "w+", encoding='utf-8') as f:
         f.write(full_text)
     with open(out_meta_filepath, "w+") as f:
         f.write(json.dumps(out_metadata, indent=4))
```

### Comparing `marker_pdf-0.2.2/marker/pdf/extract_text.py` & `marker_pdf-0.2.4/marker/pdf/extract_text.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.2/marker/pdf/images.py` & `marker_pdf-0.2.4/marker/pdf/images.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.2/marker/pdf/utils.py` & `marker_pdf-0.2.4/marker/pdf/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 import filetype
 
 from marker.settings import settings
 
 
 def find_filetype(fpath):
     kind = filetype.guess(fpath)
+    if kind is None:
+        print(f"Could not determine filetype for {fpath}")
+        return "other"
 
     mimetype = kind.mime
 
     # Get extensions from mimetype
     # The mimetype is not always consistent, so use in to check the most common formats
     if "pdf" in mimetype:
         return "pdf"
```

### Comparing `marker_pdf-0.2.2/marker/postprocessors/editor.py` & `marker_pdf-0.2.4/marker/postprocessors/editor.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.2/marker/postprocessors/markdown.py` & `marker_pdf-0.2.4/marker/postprocessors/markdown.py`

 * *Files 6% similar despite different names*

```diff
@@ -92,37 +92,39 @@
             text = "\n" + text + "\n"
     return text
 
 
 def line_separator(line1, line2, block_type, is_continuation=False):
     # Should cover latin-derived languages and russian
     lowercase_letters = r'\p{Lo}|\p{Ll}|\d'
+    hyphens = r'-—¬'
     # Remove hyphen in current line if next line and current line appear to be joined
-    hyphen_pattern = regex.compile(rf'.*[{lowercase_letters}][-]\s?$', regex.DOTALL)
+    hyphen_pattern = regex.compile(rf'.*[{lowercase_letters}][{hyphens}]\s?$', regex.DOTALL)
     if line1 and hyphen_pattern.match(line1) and regex.match(rf"^\s?[{lowercase_letters}]", line2):
         # Split on — or - from the right
-        line1 = regex.split(r"[-—]\s?$", line1)[0]
+        line1 = regex.split(rf"[{hyphens}]\s?$", line1)[0]
         return line1.rstrip() + line2.lstrip()
 
     all_letters = r'\p{L}|\d'
-    sentence_continuations = r',;\(\—\"\''
+    sentence_continuations = r',;\(\—\"\'\*'
     sentence_ends = r'。ๆ\.?!'
     line_end_pattern = regex.compile(rf'.*[{lowercase_letters}][{sentence_continuations}]?\s?$', regex.DOTALL)
     line_start_pattern = regex.compile(rf'^\s?[{all_letters}]', regex.DOTALL)
     sentence_end_pattern = regex.compile(rf'.*[{sentence_ends}]\s?$', regex.DOTALL)
 
+    text_blocks = ["Text", "List-item", "Footnote", "Caption", "Figure"]
     if block_type in ["Title", "Section-header"]:
         return line1.rstrip() + " " + line2.lstrip()
     elif block_type == "Formula":
         return line1 + "\n" + line2
-    elif line_end_pattern.match(line1) and line_start_pattern.match(line2) and block_type == "Text":
+    elif line_end_pattern.match(line1) and line_start_pattern.match(line2) and block_type in text_blocks:
         return line1.rstrip() + " " + line2.lstrip()
     elif is_continuation:
         return line1.rstrip() + " " + line2.lstrip()
-    elif block_type == "Text" and sentence_end_pattern.match(line1):
+    elif block_type in text_blocks and sentence_end_pattern.match(line1):
         return line1 + "\n\n" + line2
     elif block_type == "Table":
         return line1 + "\n\n" + line2
     else:
         return line1 + "\n" + line2
```

### Comparing `marker_pdf-0.2.2/marker/postprocessors/t5.py` & `marker_pdf-0.2.4/marker/postprocessors/t5.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.2/marker/schema/bbox.py` & `marker_pdf-0.2.4/marker/schema/bbox.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.2/marker/schema/block.py` & `marker_pdf-0.2.4/marker/schema/block.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.2/marker/schema/page.py` & `marker_pdf-0.2.4/marker/schema/page.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.2/marker/settings.py` & `marker_pdf-0.2.4/marker/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
         if torch.backends.mps.is_available():
             return "mps"
 
         return "cpu"
 
     INFERENCE_RAM: int = 40 # How much VRAM each GPU has (in GB).
-    VRAM_PER_TASK: float = 4 # How much VRAM to allocate per task (in GB).  Peak marker VRAM usage is around 5GB, but avg across workers is lower.
+    VRAM_PER_TASK: float = 4.5 # How much VRAM to allocate per task (in GB).  Peak marker VRAM usage is around 5GB, but avg across workers is lower.
     DEFAULT_LANG: str = "English" # Default language we assume files to be in, should be one of the keys in TESSERACT_LANGUAGES
 
     SUPPORTED_FILETYPES: Dict = {
         "application/pdf": "pdf",
     }
 
     # Text line Detection
```

### Comparing `marker_pdf-0.2.2/marker/tables/cells.py` & `marker_pdf-0.2.4/marker/tables/cells.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.2/marker/tables/table.py` & `marker_pdf-0.2.4/marker/tables/table.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.2/marker/tables/utils.py` & `marker_pdf-0.2.4/marker/tables/utils.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.2/pyproject.toml` & `marker_pdf-0.2.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "marker-pdf"
-version = "0.2.2"
+version = "0.2.4"
 description = "Convert PDF to markdown with high speed and accuracy."
 authors = ["Vik Paruchuri <github@vikas.sh>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 repository = "https://github.com/VikParuchuri/marker"
 keywords = ["pdf", "markdown", "ocr", "nlp"]
 packages = [
@@ -33,14 +33,15 @@
 ftfy = "^6.1.1"
 texify = "^0.1.8"
 rapidfuzz = "^3.8.1"
 surya-ocr = "^0.4.3"
 filetype = "^1.2.0"
 regex = "^2024.4.28"
 pdftext = "^0.3.7"
+grpcio = "^1.63.0"
 
 [tool.poetry.group.dev.dependencies]
 jupyter = "^1.0.0"
 
 [tool.poetry.scripts]
 marker = "convert:main"
 marker_single = "convert_single:main"
```

### Comparing `marker_pdf-0.2.2/PKG-INFO` & `marker_pdf-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marker-pdf
-Version: 0.2.2
+Version: 0.2.4
 Summary: Convert PDF to markdown with high speed and accuracy.
 Home-page: https://github.com/VikParuchuri/marker
 License: GPL-3.0-or-later
 Keywords: pdf,markdown,ocr,nlp
 Author: Vik Paruchuri
 Author-email: github@vikas.sh
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pillow (>=10.1.0,<11.0.0)
 Requires-Dist: filetype (>=1.2.0,<2.0.0)
 Requires-Dist: ftfy (>=6.1.1,<7.0.0)
+Requires-Dist: grpcio (>=1.63.0,<2.0.0)
 Requires-Dist: numpy (>=1.26.1,<2.0.0)
 Requires-Dist: pdftext (>=0.3.7,<0.4.0)
 Requires-Dist: pydantic (>=2.4.2,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.0.3,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: rapidfuzz (>=3.8.1,<4.0.0)
 Requires-Dist: ray (>=2.20.0,<3.0.0)
@@ -67,15 +68,15 @@
 | [Multi-column CNN](https://arxiv.org/pdf/1804.07821.pdf)              | arXiv paper | [View](https://github.com/VikParuchuri/marker/blob/master/data/examples/marker/multicolcnn.md)         | [View](https://github.com/VikParuchuri/marker/blob/master/data/examples/nougat/multicolcnn.md)         |
 
 
 ## Performance
 
 ![Benchmark overall](data/images/overall.png)
 
-The above results are with marker and nougat setup so they each take ~3GB of VRAM on an A6000.
+The above results are with marker and nougat setup so they each take ~4GB of VRAM on an A6000.
 
 See [below](#benchmarks) for detailed speed and accuracy benchmarks, and instructions on how to run your own benchmarks.
 
 # Community
 
 [Discord](https://discord.gg//KuZwXNGnfH) is where we discuss future development.
 
@@ -210,15 +211,15 @@
 | marker | 0.536176        | 0.516833         | 0.70515         | 0.710657    | 0.690042     | 0.523467  |
 | nougat | 0.44009         | 0.588973         | 0.322706        | 0.401342    | 0.160842     | 0.525663  |
 
 Peak GPU memory usage during the benchmark is `4.2GB` for nougat, and `4.1GB` for marker.  Benchmarks were run on an A6000 Ada.
 
 **Throughput**
 
-Marker takes about 4GB of VRAM on average per task, so you can convert 12 documents in parallel on an A6000.
+Marker takes about 4.5GB of VRAM on average per task, so you can convert 10 documents in parallel on an A6000.
 
 ![Benchmark results](data/images/per_doc.png)
 
 ## Running your own benchmarks
 
 You can benchmark the performance of marker on your machine. Install marker manually with:
```

