# Comparing `tmp/GnDocTrans-0.0.3.tar.gz` & `tmp/GnDocTrans-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GnDocTrans-0.0.3.tar", last modified: Wed May  8 07:56:25 2024, max compression
+gzip compressed data, was "GnDocTrans-0.0.4.tar", last modified: Fri May 10 03:01:27 2024, max compression
```

## Comparing `GnDocTrans-0.0.3.tar` & `GnDocTrans-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 fusen     (1000) fusen     (1000)        0 2024-05-08 07:56:25.277210 GnDocTrans-0.0.3/
-drwxrwxr-x   0 fusen     (1000) fusen     (1000)        0 2024-05-08 07:56:25.277210 GnDocTrans-0.0.3/GnDocTrans/
--rw-rw-r--   0 fusen     (1000) fusen     (1000)       30 2024-05-07 06:57:19.000000 GnDocTrans-0.0.3/GnDocTrans/__init__.py
--rw-rw-r--   0 fusen     (1000) fusen     (1000)    23662 2024-05-08 07:55:47.000000 GnDocTrans-0.0.3/GnDocTrans/tri_derive_tile.py
-drwxrwxr-x   0 fusen     (1000) fusen     (1000)        0 2024-05-08 07:56:25.277210 GnDocTrans-0.0.3/GnDocTrans.egg-info/
--rw-rw-r--   0 fusen     (1000) fusen     (1000)      354 2024-05-08 07:56:25.000000 GnDocTrans-0.0.3/GnDocTrans.egg-info/PKG-INFO
--rw-rw-r--   0 fusen     (1000) fusen     (1000)      230 2024-05-08 07:56:25.000000 GnDocTrans-0.0.3/GnDocTrans.egg-info/SOURCES.txt
--rw-rw-r--   0 fusen     (1000) fusen     (1000)        1 2024-05-08 07:56:25.000000 GnDocTrans-0.0.3/GnDocTrans.egg-info/dependency_links.txt
--rw-rw-r--   0 fusen     (1000) fusen     (1000)       20 2024-05-08 07:56:25.000000 GnDocTrans-0.0.3/GnDocTrans.egg-info/requires.txt
--rw-rw-r--   0 fusen     (1000) fusen     (1000)       11 2024-05-08 07:56:25.000000 GnDocTrans-0.0.3/GnDocTrans.egg-info/top_level.txt
--rw-rw-r--   0 fusen     (1000) fusen     (1000)      354 2024-05-08 07:56:25.277210 GnDocTrans-0.0.3/PKG-INFO
--rw-rw-r--   0 fusen     (1000) fusen     (1000)       38 2024-05-08 07:56:25.277210 GnDocTrans-0.0.3/setup.cfg
--rw-rw-r--   0 fusen     (1000) fusen     (1000)      501 2024-05-08 07:56:15.000000 GnDocTrans-0.0.3/setup.py
+drwxrwxr-x   0 fusen     (1000) fusen     (1000)        0 2024-05-10 03:01:27.825815 GnDocTrans-0.0.4/
+drwxrwxr-x   0 fusen     (1000) fusen     (1000)        0 2024-05-10 03:01:27.825815 GnDocTrans-0.0.4/GnDocTrans/
+-rw-rw-r--   0 fusen     (1000) fusen     (1000)       30 2024-05-07 06:57:19.000000 GnDocTrans-0.0.4/GnDocTrans/__init__.py
+-rw-rw-r--   0 fusen     (1000) fusen     (1000)    23925 2024-05-10 03:00:34.000000 GnDocTrans-0.0.4/GnDocTrans/tri_derive_tile.py
+drwxrwxr-x   0 fusen     (1000) fusen     (1000)        0 2024-05-10 03:01:27.825815 GnDocTrans-0.0.4/GnDocTrans.egg-info/
+-rw-rw-r--   0 fusen     (1000) fusen     (1000)      354 2024-05-10 03:01:27.000000 GnDocTrans-0.0.4/GnDocTrans.egg-info/PKG-INFO
+-rw-rw-r--   0 fusen     (1000) fusen     (1000)      230 2024-05-10 03:01:27.000000 GnDocTrans-0.0.4/GnDocTrans.egg-info/SOURCES.txt
+-rw-rw-r--   0 fusen     (1000) fusen     (1000)        1 2024-05-10 03:01:27.000000 GnDocTrans-0.0.4/GnDocTrans.egg-info/dependency_links.txt
+-rw-rw-r--   0 fusen     (1000) fusen     (1000)       20 2024-05-10 03:01:27.000000 GnDocTrans-0.0.4/GnDocTrans.egg-info/requires.txt
+-rw-rw-r--   0 fusen     (1000) fusen     (1000)       11 2024-05-10 03:01:27.000000 GnDocTrans-0.0.4/GnDocTrans.egg-info/top_level.txt
+-rw-rw-r--   0 fusen     (1000) fusen     (1000)      354 2024-05-10 03:01:27.825815 GnDocTrans-0.0.4/PKG-INFO
+-rw-rw-r--   0 fusen     (1000) fusen     (1000)       38 2024-05-10 03:01:27.825815 GnDocTrans-0.0.4/setup.cfg
+-rw-rw-r--   0 fusen     (1000) fusen     (1000)      501 2024-05-10 03:00:49.000000 GnDocTrans-0.0.4/setup.py
```

### Comparing `GnDocTrans-0.0.3/GnDocTrans/tri_derive_tile.py` & `GnDocTrans-0.0.4/GnDocTrans/tri_derive_tile.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,15 +163,15 @@
     boxes_of_random: list[list] = []
     flags_dict: dict[str, list[bool]] = {
         'islet': [False]*len(exist_boxes['islet'])
     }
     for row in range(rows):
         col_shift = half_cell_w if row%2 else 0
         for col in range(cols+(row%2)):
-            if random.random() < probability:
+            if random.random() <= probability:
                 tl_x = col*cell_w - col_shift
                 tl_y = row*cell_h
                 center_x = tl_x + cell_w / 2
                 center_y = tl_y + cell_h / 2
                 is_in_box: bool = False
                 for name, flag_list in flags_dict.items():
                     for index, flag in enumerate(flag_list):
@@ -179,14 +179,16 @@
                             continue
                         is_in_box = (exist_boxes[name][index][0] < center_x and center_x < exist_boxes[name][index][0]+exist_boxes[name][index][2]) and \
                             (exist_boxes[name][index][1] < center_y and center_y < exist_boxes[name][index][1]+exist_boxes[name][index][3])
                         if is_in_box:
                             break
                     if is_in_box:
                         break
+                if is_in_box:
+                    print(f'It has hit the existed box: ["name":{name}, "index":{index}], location: ["row":{row}, "col":{col}]')
                 if not is_in_box:
                     boxes_of_random.append([tl_x, tl_y, cell_w, cell_h])
     return {
         'random': boxes_of_random
     }
     
 
@@ -323,14 +325,19 @@
         cv2.rectangle(canvas, (box[0], box[1]), (box[2], box[3]), 255, -1)
     if 0 < element_extend:
         elem = cv2.getStructuringElement(cv2.MORPH_RECT, (element_extend*2+1, element_extend*2+1))
         canvas = cv2.morphologyEx(canvas, cv2.MORPH_CLOSE, elem)
     # if inverse:
     canvas = cv2.bitwise_not(canvas)
     contours, hierarchy = cv2.findContours(canvas, cv2.RETR_CCOMP, cv2.CHAIN_APPROX_SIMPLE)
+    if len(contours) == 0:
+        return {
+            'parent': [],
+            'childs': []
+        }
     hierarchy = hierarchy[0]
     output_parent: list[list[list]] = []
     output_childs: list[list[list[list]]] = []
     index = 0
     while -1 != index:
         output_parent.append(np.squeeze(contours[index], axis=1).tolist())
         # for point in output_parent[-1]:
@@ -365,19 +372,19 @@
 def pathsToSVG(paths: list[list[list]]) -> str:
     # print(paths)
     # print(len(paths))
     return ' '.join([pathToSVG(path) for path in paths])
 
 
 
-def pathsToSVGs(paths: list[list[list]]) -> list[str]:
+def pathsToSVGs_old(paths: list[list[list]]) -> list[str]:
     return [pathToSVG(path)+' Z' for path in paths]
 
 
-def pathsToSVGs2(parent: list[list[list]], childs: list[list[list[list]]]) -> list[str]:
+def pathsToSVGs(parent: list[list[list]], childs: list[list[list[list]]]) -> list[str]:
     str_list: list[str] = []
     for par, chi in zip(parent, childs):
         parts = [pathToSVG(par)]
         for box in chi:
             parts.append(pathToSVG(box))
         parts.append('Z')
         str_list.append(' '.join(parts))
@@ -449,19 +456,19 @@
         else:
             shift_x = int(math.ceil(sandbox_width * reference_cx))
         shift_x = shift_x // cell_width * cell_width
     boxes_raw = shiftBoxes(boxes_raw, shift_x, shift_y)
     boxes_rand = randBoxes(cell_width, cell_height, cell_rows, cell_cols, probability, boxes_raw)
     boxes_all = copy.deepcopy(boxes_raw)
     boxes_all.update(copy.deepcopy(boxes_rand))
-    ocean_patch_list = pathsToSVGs2(**boxesToPathsInvGlobal(boxes_all, sandbox_width, sandbox_height, element_extend=2))
+    ocean_patch_list = pathsToSVGs(**boxesToPathsInvGlobal(boxes_all, sandbox_width, sandbox_height, element_extend=2))
     # boxes_str = pathsToSVG(boxesToPaths(boxes_all, element_extend=2))
     boxes_patch = copy.deepcopy(boxes_rand)
     boxes_patch['sector'] = copy.deepcopy(boxes_raw['sector'])
-    derive_patch_list = pathsToSVGs2(**boxesToPaths(boxes_patch, element_extend=2))
+    derive_patch_list = pathsToSVGs(**boxesToPaths(boxes_patch, element_extend=2))
     # patch_str_list = pathsToSVGs(boxesToPaths(boxes_patch, element_extend=2))
     viewbox_x = 0 if 'left' == direction else sandbox_width - canvas_width
     viewbox_x = (sandbox_width - canvas_width) / 2
     viewbox_y = (sandbox_height - canvas_height) / 2
     if reference_cx < 0.3333:
         viewbox_x = 0
     elif reference_cx < 0.6667:
@@ -624,18 +631,18 @@
         resolution_width=1024, resolution_height=1024,
         canvas_width=1024, canvas_height=1024,
         original_img_str=img_str, derive1_img_str=bin_str, derive2_img_str=con_str,
         structure='2-1',
         direction='right',
         location='islet',
         shift='3',
-        probability=0.5,
+        probability=1,
         reference_cx=0.5, reference_cy=0.4,
         image_width=image_width, image_height=image_height,
         space_width=image_width//10, space_height=image_width//12,
     )
-    with open('2-1-0.5.svg', 'w') as fp:
+    with open('result.svg', 'w') as fp:
         fp.write(svg_str)
 
 
 if '__main__' == __name__:
     test()
```

