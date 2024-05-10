# Comparing `tmp/opensr-test-0.2.0.tar.gz` & `tmp/opensr-test-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensr-test-0.2.0.tar", last modified: Sun Mar 24 14:03:21 2024, max compression
+gzip compressed data, was "opensr-test-0.2.1.tar", last modified: Wed Mar 27 16:40:04 2024, max compression
```

## Comparing `opensr-test-0.2.0.tar` & `opensr-test-0.2.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 cesar     (1002) cesar     (1002)        0 2024-03-24 14:03:21.844764 opensr-test-0.2.0/
--rw-rw-r--   0 cesar     (1002) cesar     (1002)     1077 2024-02-09 11:36:31.000000 opensr-test-0.2.0/LICENSE
--rw-rw-r--   0 cesar     (1002) cesar     (1002)    10532 2024-03-24 14:03:21.844764 opensr-test-0.2.0/PKG-INFO
--rw-rw-r--   0 cesar     (1002) cesar     (1002)     9814 2024-03-24 14:01:31.000000 opensr-test-0.2.0/README.md
-drwxrwxr-x   0 cesar     (1002) cesar     (1002)        0 2024-03-24 14:03:21.844764 opensr-test-0.2.0/opensr_test/
--rw-rw-r--   0 cesar     (1002) cesar     (1002)      137 2024-03-23 10:42:07.000000 opensr-test-0.2.0/opensr_test/__init__.py
--rw-rw-r--   0 cesar     (1002) cesar     (1002)     9265 2024-03-24 10:15:54.000000 opensr-test-0.2.0/opensr_test/config.py
--rw-rw-r--   0 cesar     (1002) cesar     (1002)    17034 2024-03-23 10:42:07.000000 opensr-test-0.2.0/opensr_test/distance.py
--rw-rw-r--   0 cesar     (1002) cesar     (1002)     3421 2024-03-23 10:42:07.000000 opensr-test-0.2.0/opensr_test/download.py
--rw-rw-r--   0 cesar     (1002) cesar     (1002)     3998 2024-03-23 10:42:07.000000 opensr-test-0.2.0/opensr_test/hallucinations.py
--rw-rw-r--   0 cesar     (1002) cesar     (1002)    11223 2024-03-24 10:13:37.000000 opensr-test-0.2.0/opensr_test/kernels.py
-drwxrwxr-x   0 cesar     (1002) cesar     (1002)        0 2024-03-24 14:03:21.844764 opensr-test-0.2.0/opensr_test/lightglue/
--rw-rw-r--   0 cesar     (1002) cesar     (1002)      263 2024-02-07 08:14:13.000000 opensr-test-0.2.0/opensr_test/lightglue/__init__.py
--rw-rw-r--   0 cesar     (1002) cesar     (1002)    26763 2024-02-07 08:14:13.000000 opensr-test-0.2.0/opensr_test/lightglue/aliked.py
--rw-rw-r--   0 cesar     (1002) cesar     (1002)     1751 2024-02-07 08:14:13.000000 opensr-test-0.2.0/opensr_test/lightglue/disk.py
--rw-rw-r--   0 cesar     (1002) cesar     (1002)     1500 2024-02-07 08:14:13.000000 opensr-test-0.2.0/opensr_test/lightglue/dog_hardnet.py
--rw-rw-r--   0 cesar     (1002) cesar     (1002)    25998 2024-03-23 10:42:07.000000 opensr-test-0.2.0/opensr_test/lightglue/lightglue.py
--rw-rw-r--   0 cesar     (1002) cesar     (1002)     8194 2024-02-07 08:14:13.000000 opensr-test-0.2.0/opensr_test/lightglue/sift.py
--rw-rw-r--   0 cesar     (1002) cesar     (1002)     8618 2024-02-07 08:14:13.000000 opensr-test-0.2.0/opensr_test/lightglue/superpoint.py
--rw-rw-r--   0 cesar     (1002) cesar     (1002)     5511 2024-03-23 10:42:07.000000 opensr-test-0.2.0/opensr_test/lightglue/utils.py
--rw-rw-r--   0 cesar     (1002) cesar     (1002)     5919 2024-02-09 11:46:15.000000 opensr-test-0.2.0/opensr_test/lightglue/viz2d.py
--rw-rw-r--   0 cesar     (1002) cesar     (1002)    21719 2024-03-24 10:55:17.000000 opensr-test-0.2.0/opensr_test/main.py
--rw-rw-r--   0 cesar     (1002) cesar     (1002)    15630 2024-03-23 18:34:25.000000 opensr-test-0.2.0/opensr_test/plot.py
--rw-rw-r--   0 cesar     (1002) cesar     (1002)      916 2024-02-09 11:36:31.000000 opensr-test-0.2.0/opensr_test/reflectance.py
--rw-rw-r--   0 cesar     (1002) cesar     (1002)    20856 2024-03-23 10:42:07.000000 opensr-test-0.2.0/opensr_test/spatial.py
--rw-rw-r--   0 cesar     (1002) cesar     (1002)      918 2024-02-09 11:36:31.000000 opensr-test-0.2.0/opensr_test/spectral.py
--rw-rw-r--   0 cesar     (1002) cesar     (1002)     8499 2024-03-23 10:42:07.000000 opensr-test-0.2.0/opensr_test/utils.py
-drwxrwxr-x   0 cesar     (1002) cesar     (1002)        0 2024-03-24 14:03:21.844764 opensr-test-0.2.0/opensr_test.egg-info/
--rw-rw-r--   0 cesar     (1002) cesar     (1002)    10532 2024-03-24 14:03:21.000000 opensr-test-0.2.0/opensr_test.egg-info/PKG-INFO
--rw-rw-r--   0 cesar     (1002) cesar     (1002)      778 2024-03-24 14:03:21.000000 opensr-test-0.2.0/opensr_test.egg-info/SOURCES.txt
--rw-rw-r--   0 cesar     (1002) cesar     (1002)        1 2024-03-24 14:03:21.000000 opensr-test-0.2.0/opensr_test.egg-info/dependency_links.txt
--rw-rw-r--   0 cesar     (1002) cesar     (1002)      131 2024-03-24 14:03:21.000000 opensr-test-0.2.0/opensr_test.egg-info/requires.txt
--rw-rw-r--   0 cesar     (1002) cesar     (1002)       12 2024-03-24 14:03:21.000000 opensr-test-0.2.0/opensr_test.egg-info/top_level.txt
--rw-rw-r--   0 cesar     (1002) cesar     (1002)       38 2024-03-24 14:03:21.844764 opensr-test-0.2.0/setup.cfg
--rw-rw-r--   0 cesar     (1002) cesar     (1002)     1490 2024-03-24 14:02:51.000000 opensr-test-0.2.0/setup.py
+drwxrwxr-x   0 cesar     (1002) cesar     (1002)        0 2024-03-27 16:40:04.256873 opensr-test-0.2.1/
+-rw-rw-r--   0 cesar     (1002) cesar     (1002)     1077 2024-02-09 11:36:31.000000 opensr-test-0.2.1/LICENSE
+-rw-rw-r--   0 cesar     (1002) cesar     (1002)    10581 2024-03-27 16:40:04.256873 opensr-test-0.2.1/PKG-INFO
+-rw-rw-r--   0 cesar     (1002) cesar     (1002)     9863 2024-03-24 14:19:46.000000 opensr-test-0.2.1/README.md
+drwxrwxr-x   0 cesar     (1002) cesar     (1002)        0 2024-03-27 16:40:04.256873 opensr-test-0.2.1/opensr_test/
+-rw-rw-r--   0 cesar     (1002) cesar     (1002)      137 2024-03-23 10:42:07.000000 opensr-test-0.2.1/opensr_test/__init__.py
+-rw-rw-r--   0 cesar     (1002) cesar     (1002)     9265 2024-03-24 10:15:54.000000 opensr-test-0.2.1/opensr_test/config.py
+-rw-rw-r--   0 cesar     (1002) cesar     (1002)    17034 2024-03-23 10:42:07.000000 opensr-test-0.2.1/opensr_test/distance.py
+-rw-rw-r--   0 cesar     (1002) cesar     (1002)     3421 2024-03-23 10:42:07.000000 opensr-test-0.2.1/opensr_test/download.py
+-rw-rw-r--   0 cesar     (1002) cesar     (1002)     3998 2024-03-23 10:42:07.000000 opensr-test-0.2.1/opensr_test/hallucinations.py
+-rw-rw-r--   0 cesar     (1002) cesar     (1002)    11223 2024-03-24 10:13:37.000000 opensr-test-0.2.1/opensr_test/kernels.py
+drwxrwxr-x   0 cesar     (1002) cesar     (1002)        0 2024-03-27 16:40:04.256873 opensr-test-0.2.1/opensr_test/lightglue/
+-rw-rw-r--   0 cesar     (1002) cesar     (1002)      263 2024-02-07 08:14:13.000000 opensr-test-0.2.1/opensr_test/lightglue/__init__.py
+-rw-rw-r--   0 cesar     (1002) cesar     (1002)    26763 2024-02-07 08:14:13.000000 opensr-test-0.2.1/opensr_test/lightglue/aliked.py
+-rw-rw-r--   0 cesar     (1002) cesar     (1002)     1751 2024-02-07 08:14:13.000000 opensr-test-0.2.1/opensr_test/lightglue/disk.py
+-rw-rw-r--   0 cesar     (1002) cesar     (1002)     1500 2024-02-07 08:14:13.000000 opensr-test-0.2.1/opensr_test/lightglue/dog_hardnet.py
+-rw-rw-r--   0 cesar     (1002) cesar     (1002)    25998 2024-03-23 10:42:07.000000 opensr-test-0.2.1/opensr_test/lightglue/lightglue.py
+-rw-rw-r--   0 cesar     (1002) cesar     (1002)     8194 2024-02-07 08:14:13.000000 opensr-test-0.2.1/opensr_test/lightglue/sift.py
+-rw-rw-r--   0 cesar     (1002) cesar     (1002)     8618 2024-02-07 08:14:13.000000 opensr-test-0.2.1/opensr_test/lightglue/superpoint.py
+-rw-rw-r--   0 cesar     (1002) cesar     (1002)     5511 2024-03-23 10:42:07.000000 opensr-test-0.2.1/opensr_test/lightglue/utils.py
+-rw-rw-r--   0 cesar     (1002) cesar     (1002)     5919 2024-02-09 11:46:15.000000 opensr-test-0.2.1/opensr_test/lightglue/viz2d.py
+-rw-rw-r--   0 cesar     (1002) cesar     (1002)    21719 2024-03-24 10:55:17.000000 opensr-test-0.2.1/opensr_test/main.py
+-rw-rw-r--   0 cesar     (1002) cesar     (1002)    15630 2024-03-23 18:34:25.000000 opensr-test-0.2.1/opensr_test/plot.py
+-rw-rw-r--   0 cesar     (1002) cesar     (1002)      916 2024-02-09 11:36:31.000000 opensr-test-0.2.1/opensr_test/reflectance.py
+-rw-rw-r--   0 cesar     (1002) cesar     (1002)    20856 2024-03-23 10:42:07.000000 opensr-test-0.2.1/opensr_test/spatial.py
+-rw-rw-r--   0 cesar     (1002) cesar     (1002)      918 2024-02-09 11:36:31.000000 opensr-test-0.2.1/opensr_test/spectral.py
+-rw-rw-r--   0 cesar     (1002) cesar     (1002)     8499 2024-03-23 10:42:07.000000 opensr-test-0.2.1/opensr_test/utils.py
+drwxrwxr-x   0 cesar     (1002) cesar     (1002)        0 2024-03-27 16:40:04.256873 opensr-test-0.2.1/opensr_test.egg-info/
+-rw-rw-r--   0 cesar     (1002) cesar     (1002)    10581 2024-03-27 16:40:04.000000 opensr-test-0.2.1/opensr_test.egg-info/PKG-INFO
+-rw-rw-r--   0 cesar     (1002) cesar     (1002)      778 2024-03-27 16:40:04.000000 opensr-test-0.2.1/opensr_test.egg-info/SOURCES.txt
+-rw-rw-r--   0 cesar     (1002) cesar     (1002)        1 2024-03-27 16:40:04.000000 opensr-test-0.2.1/opensr_test.egg-info/dependency_links.txt
+-rw-rw-r--   0 cesar     (1002) cesar     (1002)      143 2024-03-27 16:40:04.000000 opensr-test-0.2.1/opensr_test.egg-info/requires.txt
+-rw-rw-r--   0 cesar     (1002) cesar     (1002)       12 2024-03-27 16:40:04.000000 opensr-test-0.2.1/opensr_test.egg-info/top_level.txt
+-rw-rw-r--   0 cesar     (1002) cesar     (1002)       38 2024-03-27 16:40:04.256873 opensr-test-0.2.1/setup.cfg
+-rw-rw-r--   0 cesar     (1002) cesar     (1002)     1513 2024-03-27 16:39:41.000000 opensr-test-0.2.1/setup.py
```

### Comparing `opensr-test-0.2.0/LICENSE` & `opensr-test-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opensr-test-0.2.0/PKG-INFO` & `opensr-test-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensr-test
-Version: 0.2.0
+Version: 0.2.1
 Summary: A comprehensive benchmark for real-world Sentinel-2 imagery super-resolution
 Home-page: https://github.com/ESAOpenSR/opensr-test
 Author: Cesar Aybar Camacho
 Author-email: csaybar@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -45,15 +45,15 @@
 </a>
 </p>
 
 ---
 
 **GitHub**: [https://github.com/ESAOpenSR/opensr-test](https://github.com/ESAOpenSR/opensr-test)
 
-**Documentation**: [https://opensr-test.readthedocs.io/](https://opensr-test.readthedocs.io/)
+**Documentation**: [https://esaopensr.github.io/opensr-test](https://esaopensr.github.io/opensr-test)
 
 **PyPI**: [https://pypi.org/project/opensr-test/](https://pypi.org/project/opensr-test/)
 
 **Paper**: Coming soon!
 
 ---
 
@@ -319,15 +319,15 @@
 
 <p align="center">
   <img src="docs/images/example05.png">
 </p>
 
 ## Deeper understanding
 
-Explore the [API](/docs/API/model_parameters.md) section for more details about personalizing your benchmark experiments.
+Explore the [API](https://esaopensr.github.io/opensr-test/docs/API/config_pydantic.html) section for more details about personalizing your benchmark experiments.
 
 <p align="center">
     <a href="/docs/api.md"><img src="docs/images/image02.png" alt="opensr-test" width="30%"></a>
 </p>
 
 ## Citation
 
@@ -337,7 +337,8 @@
 Coming soon!
 ```
 
 ## Acknowledgements
 
 This work was make with the support of the European Space Agency (ESA) under the project “Explainable AI: application to trustworthy super-resolution (OpenSR)”. Cesar Aybar acknowledges support by the National Council of Science, Technology, and Technological Innovation (CONCYTEC, Peru) through the “PROYECTOS DE INVESTIGACIÓN BÁSICA – 2023-01” program with contract number PE501083135-2023-PROCIENCIA. Luis Gómez-Chova acknowledges support from the Spanish Ministry of Science and Innovation (project PID2019-109026RB-I00 funded by MCIN/AEI/10.13039/501100011033).
 
+
```

#### html2text {}

```diff
@@ -1,43 +1,44 @@
-Metadata-Version: 2.1 Name: opensr-test Version: 0.2.0 Summary: A comprehensive
+Metadata-Version: 2.1 Name: opensr-test Version: 0.2.1 Summary: A comprehensive
 benchmark for real-world Sentinel-2 imagery super-resolution Home-page: https:/
 /github.com/ESAOpenSR/opensr-test Author: Cesar Aybar Camacho Author-email:
 csaybar@gmail.com License: MIT Platform: UNKNOWN Classifier: Development Status
 :: 2 - Pre-Alpha Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python ::
 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown Provides-Extra: perceptual License-
 File: LICENSE
                                    _[_h_e_a_d_e_r_]
  AA ccoommpprreehheennssiivvee bbeenncchhmmaarrkk ffoorr rreeaall--wwoorrlldd SSeennttiinneell--22 iimmaaggeerryy ssuuppeerr--rreessoolluuttiioonn
               _[_P_y_P_I_]_[_L_i_c_e_n_s_e_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_B_l_a_c_k_]_[_i_s_o_r_t_]
 --- **GitHub**: [https://github.com/ESAOpenSR/opensr-test](https://github.com/
-ESAOpenSR/opensr-test) **Documentation**: [https://opensr-test.readthedocs.io/]
-(https://opensr-test.readthedocs.io/) **PyPI**: [https://pypi.org/project/
-opensr-test/](https://pypi.org/project/opensr-test/) **Paper**: Coming soon! --
-- # ## Overview In remote sensing, Image Super-Resolution (ISR) goal is to
-improve the ground sampling distance. However, two problems are common in the
-literature. First, most models are **tested on synthetic data**, raising doubts
-about their real-world applicability and performance. Second, traditional
-evaluation metrics such as PSNR, LPIPS, and SSIM are not designed for assessing
-ISR performance. These metrics fall short, especially in conditions involving
-changes in luminance or spatial misalignments - scenarios that are frequently
-encountered in remote sensing imagery. To address these challenges, 'opensr-
-test' provides a fair approach for ISR benchmark. We provide **three datasets**
-that were carefully crafted to minimize spatial and spectral misalignment.
-Besides, 'opensr-test' precisely assesses ISR algorithm performance across
-**three independent metrics groups** that measure *consistency*, *synthesis*,
-and *correctness*. ## How to use The example below shows how to use `opensr-
-test` to benchmark your SR model. ```python import torch import opensr_test lr
-= torch.rand(4, 64, 64) hr = torch.rand(4, 256, 256) sr = torch.rand(4, 256,
-256) metrics = opensr_test.Metrics() metrics.compute(lr=lr, sr=sr, hr=hr) ```
-## Benchmark Benchmark comparison of SR models. Downward arrows (â) denote
-metrics in which lower values are preferable, and upward arrows (â) indicate
-metrics in which higher values reflect better performance.
+ESAOpenSR/opensr-test) **Documentation**: [https://esaopensr.github.io/opensr-
+test](https://esaopensr.github.io/opensr-test) **PyPI**: [https://pypi.org/
+project/opensr-test/](https://pypi.org/project/opensr-test/) **Paper**: Coming
+soon! --- # ## Overview In remote sensing, Image Super-Resolution (ISR) goal is
+to improve the ground sampling distance. However, two problems are common in
+the literature. First, most models are **tested on synthetic data**, raising
+doubts about their real-world applicability and performance. Second,
+traditional evaluation metrics such as PSNR, LPIPS, and SSIM are not designed
+for assessing ISR performance. These metrics fall short, especially in
+conditions involving changes in luminance or spatial misalignments - scenarios
+that are frequently encountered in remote sensing imagery. To address these
+challenges, 'opensr-test' provides a fair approach for ISR benchmark. We
+provide **three datasets** that were carefully crafted to minimize spatial and
+spectral misalignment. Besides, 'opensr-test' precisely assesses ISR algorithm
+performance across **three independent metrics groups** that measure
+*consistency*, *synthesis*, and *correctness*. ## How to use The example below
+shows how to use `opensr-test` to benchmark your SR model. ```python import
+torch import opensr_test lr = torch.rand(4, 64, 64) hr = torch.rand(4, 256,
+256) sr = torch.rand(4, 256, 256) metrics = opensr_test.Metrics()
+metrics.compute(lr=lr, sr=sr, hr=hr) ``` ## Benchmark Benchmark comparison of
+SR models. Downward arrows (â) denote metrics in which lower values are
+preferable, and upward arrows (â) indicate metrics in which higher values
+reflect better performance.
  _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
 |_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_CC_oo_nn_ss_ii_ss_tt_ee_nn_cc_yy_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_SS_yy_nn_tt_hh_ee_ss_ii_ss_|_CC_oo_rr_rr_ee_cc_tt_nn_ee_ss_ss_ _ _ _ _ _ _ _ _ |
 |                 |rreefflleeccttaannccee|ssppeeccttrraall|ssppaattiiaall|hhiigghh--    |      |      |      |
 |                 |?â??        |?â??     |?â??    |ffrreeqquueennccyy|hhaa ?â??|oomm ?â??|iimm ?â??|
 |_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _|_?â_?_?_ _ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ |
 |      |_SS_uu_pp_ee_rr_II_mm_aa_gg_ee_|_00_.._00_00_88_ _ _ _ _ _ _|_77_.._22_88_66_ _ _ _|_00_.._11_33_11_ _ _|_0_._0_0_3_ _ _ _ _|_00_.._11_11_77_ _|_00_.._77_88_44_ _|_00_.._00_99_88_ |
 |NNAAIIPP  |_SS_RR_44_RR_SS_ _ _ _ _ _|_0_._0_1_6_ _ _ _ _ _ _|_33_.._44_77_11_ _ _ _|_1_._1_5_6_ _ _|_0_._0_1_0_ _ _ _ _|_0_._8_6_9_ _|_0_._0_7_7_ _|_0_._0_5_4_ |
@@ -85,16 +86,17 @@
 Display the matching points between the LR and SR images: ```python
 metrics.plot_spatial_matches() ```
                           [docs/images/example03.png]
 Display a summary of all the metrics: ```python metrics.plot_summary() ```
                           [docs/images/example04.png]
 Display the correctness of the SR image: ```python metrics.plot_tc() ```
                           [docs/images/example05.png]
-## Deeper understanding Explore the [API](/docs/API/model_parameters.md)
-section for more details about personalizing your benchmark experiments.
+## Deeper understanding Explore the [API](https://esaopensr.github.io/opensr-
+test/docs/API/config_pydantic.html) section for more details about
+personalizing your benchmark experiments.
                                  _[_o_p_e_n_s_r_-_t_e_s_t_]
 ## Citation If you use `opensr-test` in your research, please cite our paper:
 ``` Coming soon! ``` ## Acknowledgements This work was make with the support of
 the European Space Agency (ESA) under the project âExplainable AI:
 application to trustworthy super-resolution (OpenSR)â. Cesar Aybar
 acknowledges support by the National Council of Science, Technology, and
 Technological Innovation (CONCYTEC, Peru) through the âPROYECTOS DE
```

### Comparing `opensr-test-0.2.0/README.md` & `opensr-test-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 </a>
 </p>
 
 ---
 
 **GitHub**: [https://github.com/ESAOpenSR/opensr-test](https://github.com/ESAOpenSR/opensr-test)
 
-**Documentation**: [https://opensr-test.readthedocs.io/](https://opensr-test.readthedocs.io/)
+**Documentation**: [https://esaopensr.github.io/opensr-test](https://esaopensr.github.io/opensr-test)
 
 **PyPI**: [https://pypi.org/project/opensr-test/](https://pypi.org/project/opensr-test/)
 
 **Paper**: Coming soon!
 
 ---
 
@@ -299,15 +299,15 @@
 
 <p align="center">
   <img src="docs/images/example05.png">
 </p>
 
 ## Deeper understanding
 
-Explore the [API](/docs/API/model_parameters.md) section for more details about personalizing your benchmark experiments.
+Explore the [API](https://esaopensr.github.io/opensr-test/docs/API/config_pydantic.html) section for more details about personalizing your benchmark experiments.
 
 <p align="center">
     <a href="/docs/api.md"><img src="docs/images/image02.png" alt="opensr-test" width="30%"></a>
 </p>
 
 ## Citation
 
@@ -315,8 +315,8 @@
 
 ```
 Coming soon!
 ```
 
 ## Acknowledgements
 
-This work was make with the support of the European Space Agency (ESA) under the project “Explainable AI: application to trustworthy super-resolution (OpenSR)”. Cesar Aybar acknowledges support by the National Council of Science, Technology, and Technological Innovation (CONCYTEC, Peru) through the “PROYECTOS DE INVESTIGACIÓN BÁSICA – 2023-01” program with contract number PE501083135-2023-PROCIENCIA. Luis Gómez-Chova acknowledges support from the Spanish Ministry of Science and Innovation (project PID2019-109026RB-I00 funded by MCIN/AEI/10.13039/501100011033).
+This work was make with the support of the European Space Agency (ESA) under the project “Explainable AI: application to trustworthy super-resolution (OpenSR)”. Cesar Aybar acknowledges support by the National Council of Science, Technology, and Technological Innovation (CONCYTEC, Peru) through the “PROYECTOS DE INVESTIGACIÓN BÁSICA – 2023-01” program with contract number PE501083135-2023-PROCIENCIA. Luis Gómez-Chova acknowledges support from the Spanish Ministry of Science and Innovation (project PID2019-109026RB-I00 funded by MCIN/AEI/10.13039/501100011033).
```

#### html2text {}

```diff
@@ -1,33 +1,34 @@
                                    _[_h_e_a_d_e_r_]
  AA ccoommpprreehheennssiivvee bbeenncchhmmaarrkk ffoorr rreeaall--wwoorrlldd SSeennttiinneell--22 iimmaaggeerryy ssuuppeerr--rreessoolluuttiioonn
               _[_P_y_P_I_]_[_L_i_c_e_n_s_e_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_B_l_a_c_k_]_[_i_s_o_r_t_]
 --- **GitHub**: [https://github.com/ESAOpenSR/opensr-test](https://github.com/
-ESAOpenSR/opensr-test) **Documentation**: [https://opensr-test.readthedocs.io/]
-(https://opensr-test.readthedocs.io/) **PyPI**: [https://pypi.org/project/
-opensr-test/](https://pypi.org/project/opensr-test/) **Paper**: Coming soon! --
-- # ## Overview In remote sensing, Image Super-Resolution (ISR) goal is to
-improve the ground sampling distance. However, two problems are common in the
-literature. First, most models are **tested on synthetic data**, raising doubts
-about their real-world applicability and performance. Second, traditional
-evaluation metrics such as PSNR, LPIPS, and SSIM are not designed for assessing
-ISR performance. These metrics fall short, especially in conditions involving
-changes in luminance or spatial misalignments - scenarios that are frequently
-encountered in remote sensing imagery. To address these challenges, 'opensr-
-test' provides a fair approach for ISR benchmark. We provide **three datasets**
-that were carefully crafted to minimize spatial and spectral misalignment.
-Besides, 'opensr-test' precisely assesses ISR algorithm performance across
-**three independent metrics groups** that measure *consistency*, *synthesis*,
-and *correctness*. ## How to use The example below shows how to use `opensr-
-test` to benchmark your SR model. ```python import torch import opensr_test lr
-= torch.rand(4, 64, 64) hr = torch.rand(4, 256, 256) sr = torch.rand(4, 256,
-256) metrics = opensr_test.Metrics() metrics.compute(lr=lr, sr=sr, hr=hr) ```
-## Benchmark Benchmark comparison of SR models. Downward arrows (â) denote
-metrics in which lower values are preferable, and upward arrows (â) indicate
-metrics in which higher values reflect better performance.
+ESAOpenSR/opensr-test) **Documentation**: [https://esaopensr.github.io/opensr-
+test](https://esaopensr.github.io/opensr-test) **PyPI**: [https://pypi.org/
+project/opensr-test/](https://pypi.org/project/opensr-test/) **Paper**: Coming
+soon! --- # ## Overview In remote sensing, Image Super-Resolution (ISR) goal is
+to improve the ground sampling distance. However, two problems are common in
+the literature. First, most models are **tested on synthetic data**, raising
+doubts about their real-world applicability and performance. Second,
+traditional evaluation metrics such as PSNR, LPIPS, and SSIM are not designed
+for assessing ISR performance. These metrics fall short, especially in
+conditions involving changes in luminance or spatial misalignments - scenarios
+that are frequently encountered in remote sensing imagery. To address these
+challenges, 'opensr-test' provides a fair approach for ISR benchmark. We
+provide **three datasets** that were carefully crafted to minimize spatial and
+spectral misalignment. Besides, 'opensr-test' precisely assesses ISR algorithm
+performance across **three independent metrics groups** that measure
+*consistency*, *synthesis*, and *correctness*. ## How to use The example below
+shows how to use `opensr-test` to benchmark your SR model. ```python import
+torch import opensr_test lr = torch.rand(4, 64, 64) hr = torch.rand(4, 256,
+256) sr = torch.rand(4, 256, 256) metrics = opensr_test.Metrics()
+metrics.compute(lr=lr, sr=sr, hr=hr) ``` ## Benchmark Benchmark comparison of
+SR models. Downward arrows (â) denote metrics in which lower values are
+preferable, and upward arrows (â) indicate metrics in which higher values
+reflect better performance.
  _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
 |_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_CC_oo_nn_ss_ii_ss_tt_ee_nn_cc_yy_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_SS_yy_nn_tt_hh_ee_ss_ii_ss_|_CC_oo_rr_rr_ee_cc_tt_nn_ee_ss_ss_ _ _ _ _ _ _ _ _ |
 |                 |rreefflleeccttaannccee|ssppeeccttrraall|ssppaattiiaall|hhiigghh--    |      |      |      |
 |                 |?â??        |?â??     |?â??    |ffrreeqquueennccyy|hhaa ?â??|oomm ?â??|iimm ?â??|
 |_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _|_?â_?_?_ _ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ |
 |      |_SS_uu_pp_ee_rr_II_mm_aa_gg_ee_|_00_.._00_00_88_ _ _ _ _ _ _|_77_.._22_88_66_ _ _ _|_00_.._11_33_11_ _ _|_0_._0_0_3_ _ _ _ _|_00_.._11_11_77_ _|_00_.._77_88_44_ _|_00_.._00_99_88_ |
 |NNAAIIPP  |_SS_RR_44_RR_SS_ _ _ _ _ _|_0_._0_1_6_ _ _ _ _ _ _|_33_.._44_77_11_ _ _ _|_1_._1_5_6_ _ _|_0_._0_1_0_ _ _ _ _|_0_._8_6_9_ _|_0_._0_7_7_ _|_0_._0_5_4_ |
@@ -75,16 +76,17 @@
 Display the matching points between the LR and SR images: ```python
 metrics.plot_spatial_matches() ```
                           [docs/images/example03.png]
 Display a summary of all the metrics: ```python metrics.plot_summary() ```
                           [docs/images/example04.png]
 Display the correctness of the SR image: ```python metrics.plot_tc() ```
                           [docs/images/example05.png]
-## Deeper understanding Explore the [API](/docs/API/model_parameters.md)
-section for more details about personalizing your benchmark experiments.
+## Deeper understanding Explore the [API](https://esaopensr.github.io/opensr-
+test/docs/API/config_pydantic.html) section for more details about
+personalizing your benchmark experiments.
                                  _[_o_p_e_n_s_r_-_t_e_s_t_]
 ## Citation If you use `opensr-test` in your research, please cite our paper:
 ``` Coming soon! ``` ## Acknowledgements This work was make with the support of
 the European Space Agency (ESA) under the project âExplainable AI:
 application to trustworthy super-resolution (OpenSR)â. Cesar Aybar
 acknowledges support by the National Council of Science, Technology, and
 Technological Innovation (CONCYTEC, Peru) through the âPROYECTOS DE
```

### Comparing `opensr-test-0.2.0/opensr_test/config.py` & `opensr-test-0.2.1/opensr_test/config.py`

 * *Files identical despite different names*

### Comparing `opensr-test-0.2.0/opensr_test/distance.py` & `opensr-test-0.2.1/opensr_test/distance.py`

 * *Files identical despite different names*

### Comparing `opensr-test-0.2.0/opensr_test/download.py` & `opensr-test-0.2.1/opensr_test/download.py`

 * *Files identical despite different names*

### Comparing `opensr-test-0.2.0/opensr_test/hallucinations.py` & `opensr-test-0.2.1/opensr_test/hallucinations.py`

 * *Files identical despite different names*

### Comparing `opensr-test-0.2.0/opensr_test/kernels.py` & `opensr-test-0.2.1/opensr_test/kernels.py`

 * *Files identical despite different names*

### Comparing `opensr-test-0.2.0/opensr_test/lightglue/aliked.py` & `opensr-test-0.2.1/opensr_test/lightglue/aliked.py`

 * *Files identical despite different names*

### Comparing `opensr-test-0.2.0/opensr_test/lightglue/disk.py` & `opensr-test-0.2.1/opensr_test/lightglue/disk.py`

 * *Files identical despite different names*

### Comparing `opensr-test-0.2.0/opensr_test/lightglue/dog_hardnet.py` & `opensr-test-0.2.1/opensr_test/lightglue/dog_hardnet.py`

 * *Files identical despite different names*

### Comparing `opensr-test-0.2.0/opensr_test/lightglue/lightglue.py` & `opensr-test-0.2.1/opensr_test/lightglue/lightglue.py`

 * *Files identical despite different names*

### Comparing `opensr-test-0.2.0/opensr_test/lightglue/sift.py` & `opensr-test-0.2.1/opensr_test/lightglue/sift.py`

 * *Files identical despite different names*

### Comparing `opensr-test-0.2.0/opensr_test/lightglue/superpoint.py` & `opensr-test-0.2.1/opensr_test/lightglue/superpoint.py`

 * *Files identical despite different names*

### Comparing `opensr-test-0.2.0/opensr_test/lightglue/utils.py` & `opensr-test-0.2.1/opensr_test/lightglue/utils.py`

 * *Files identical despite different names*

### Comparing `opensr-test-0.2.0/opensr_test/lightglue/viz2d.py` & `opensr-test-0.2.1/opensr_test/lightglue/viz2d.py`

 * *Files identical despite different names*

### Comparing `opensr-test-0.2.0/opensr_test/main.py` & `opensr-test-0.2.1/opensr_test/main.py`

 * *Files identical despite different names*

### Comparing `opensr-test-0.2.0/opensr_test/plot.py` & `opensr-test-0.2.1/opensr_test/plot.py`

 * *Files identical despite different names*

### Comparing `opensr-test-0.2.0/opensr_test/reflectance.py` & `opensr-test-0.2.1/opensr_test/reflectance.py`

 * *Files identical despite different names*

### Comparing `opensr-test-0.2.0/opensr_test/spatial.py` & `opensr-test-0.2.1/opensr_test/spatial.py`

 * *Files identical despite different names*

### Comparing `opensr-test-0.2.0/opensr_test/spectral.py` & `opensr-test-0.2.1/opensr_test/spectral.py`

 * *Files identical despite different names*

### Comparing `opensr-test-0.2.0/opensr_test/utils.py` & `opensr-test-0.2.1/opensr_test/utils.py`

 * *Files identical despite different names*

### Comparing `opensr-test-0.2.0/opensr_test.egg-info/PKG-INFO` & `opensr-test-0.2.1/opensr_test.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensr-test
-Version: 0.2.0
+Version: 0.2.1
 Summary: A comprehensive benchmark for real-world Sentinel-2 imagery super-resolution
 Home-page: https://github.com/ESAOpenSR/opensr-test
 Author: Cesar Aybar Camacho
 Author-email: csaybar@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -45,15 +45,15 @@
 </a>
 </p>
 
 ---
 
 **GitHub**: [https://github.com/ESAOpenSR/opensr-test](https://github.com/ESAOpenSR/opensr-test)
 
-**Documentation**: [https://opensr-test.readthedocs.io/](https://opensr-test.readthedocs.io/)
+**Documentation**: [https://esaopensr.github.io/opensr-test](https://esaopensr.github.io/opensr-test)
 
 **PyPI**: [https://pypi.org/project/opensr-test/](https://pypi.org/project/opensr-test/)
 
 **Paper**: Coming soon!
 
 ---
 
@@ -319,15 +319,15 @@
 
 <p align="center">
   <img src="docs/images/example05.png">
 </p>
 
 ## Deeper understanding
 
-Explore the [API](/docs/API/model_parameters.md) section for more details about personalizing your benchmark experiments.
+Explore the [API](https://esaopensr.github.io/opensr-test/docs/API/config_pydantic.html) section for more details about personalizing your benchmark experiments.
 
 <p align="center">
     <a href="/docs/api.md"><img src="docs/images/image02.png" alt="opensr-test" width="30%"></a>
 </p>
 
 ## Citation
 
@@ -337,7 +337,8 @@
 Coming soon!
 ```
 
 ## Acknowledgements
 
 This work was make with the support of the European Space Agency (ESA) under the project “Explainable AI: application to trustworthy super-resolution (OpenSR)”. Cesar Aybar acknowledges support by the National Council of Science, Technology, and Technological Innovation (CONCYTEC, Peru) through the “PROYECTOS DE INVESTIGACIÓN BÁSICA – 2023-01” program with contract number PE501083135-2023-PROCIENCIA. Luis Gómez-Chova acknowledges support from the Spanish Ministry of Science and Innovation (project PID2019-109026RB-I00 funded by MCIN/AEI/10.13039/501100011033).
 
+
```

#### html2text {}

```diff
@@ -1,43 +1,44 @@
-Metadata-Version: 2.1 Name: opensr-test Version: 0.2.0 Summary: A comprehensive
+Metadata-Version: 2.1 Name: opensr-test Version: 0.2.1 Summary: A comprehensive
 benchmark for real-world Sentinel-2 imagery super-resolution Home-page: https:/
 /github.com/ESAOpenSR/opensr-test Author: Cesar Aybar Camacho Author-email:
 csaybar@gmail.com License: MIT Platform: UNKNOWN Classifier: Development Status
 :: 2 - Pre-Alpha Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python ::
 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown Provides-Extra: perceptual License-
 File: LICENSE
                                    _[_h_e_a_d_e_r_]
  AA ccoommpprreehheennssiivvee bbeenncchhmmaarrkk ffoorr rreeaall--wwoorrlldd SSeennttiinneell--22 iimmaaggeerryy ssuuppeerr--rreessoolluuttiioonn
               _[_P_y_P_I_]_[_L_i_c_e_n_s_e_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_B_l_a_c_k_]_[_i_s_o_r_t_]
 --- **GitHub**: [https://github.com/ESAOpenSR/opensr-test](https://github.com/
-ESAOpenSR/opensr-test) **Documentation**: [https://opensr-test.readthedocs.io/]
-(https://opensr-test.readthedocs.io/) **PyPI**: [https://pypi.org/project/
-opensr-test/](https://pypi.org/project/opensr-test/) **Paper**: Coming soon! --
-- # ## Overview In remote sensing, Image Super-Resolution (ISR) goal is to
-improve the ground sampling distance. However, two problems are common in the
-literature. First, most models are **tested on synthetic data**, raising doubts
-about their real-world applicability and performance. Second, traditional
-evaluation metrics such as PSNR, LPIPS, and SSIM are not designed for assessing
-ISR performance. These metrics fall short, especially in conditions involving
-changes in luminance or spatial misalignments - scenarios that are frequently
-encountered in remote sensing imagery. To address these challenges, 'opensr-
-test' provides a fair approach for ISR benchmark. We provide **three datasets**
-that were carefully crafted to minimize spatial and spectral misalignment.
-Besides, 'opensr-test' precisely assesses ISR algorithm performance across
-**three independent metrics groups** that measure *consistency*, *synthesis*,
-and *correctness*. ## How to use The example below shows how to use `opensr-
-test` to benchmark your SR model. ```python import torch import opensr_test lr
-= torch.rand(4, 64, 64) hr = torch.rand(4, 256, 256) sr = torch.rand(4, 256,
-256) metrics = opensr_test.Metrics() metrics.compute(lr=lr, sr=sr, hr=hr) ```
-## Benchmark Benchmark comparison of SR models. Downward arrows (â) denote
-metrics in which lower values are preferable, and upward arrows (â) indicate
-metrics in which higher values reflect better performance.
+ESAOpenSR/opensr-test) **Documentation**: [https://esaopensr.github.io/opensr-
+test](https://esaopensr.github.io/opensr-test) **PyPI**: [https://pypi.org/
+project/opensr-test/](https://pypi.org/project/opensr-test/) **Paper**: Coming
+soon! --- # ## Overview In remote sensing, Image Super-Resolution (ISR) goal is
+to improve the ground sampling distance. However, two problems are common in
+the literature. First, most models are **tested on synthetic data**, raising
+doubts about their real-world applicability and performance. Second,
+traditional evaluation metrics such as PSNR, LPIPS, and SSIM are not designed
+for assessing ISR performance. These metrics fall short, especially in
+conditions involving changes in luminance or spatial misalignments - scenarios
+that are frequently encountered in remote sensing imagery. To address these
+challenges, 'opensr-test' provides a fair approach for ISR benchmark. We
+provide **three datasets** that were carefully crafted to minimize spatial and
+spectral misalignment. Besides, 'opensr-test' precisely assesses ISR algorithm
+performance across **three independent metrics groups** that measure
+*consistency*, *synthesis*, and *correctness*. ## How to use The example below
+shows how to use `opensr-test` to benchmark your SR model. ```python import
+torch import opensr_test lr = torch.rand(4, 64, 64) hr = torch.rand(4, 256,
+256) sr = torch.rand(4, 256, 256) metrics = opensr_test.Metrics()
+metrics.compute(lr=lr, sr=sr, hr=hr) ``` ## Benchmark Benchmark comparison of
+SR models. Downward arrows (â) denote metrics in which lower values are
+preferable, and upward arrows (â) indicate metrics in which higher values
+reflect better performance.
  _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
 |_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_CC_oo_nn_ss_ii_ss_tt_ee_nn_cc_yy_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_SS_yy_nn_tt_hh_ee_ss_ii_ss_|_CC_oo_rr_rr_ee_cc_tt_nn_ee_ss_ss_ _ _ _ _ _ _ _ _ |
 |                 |rreefflleeccttaannccee|ssppeeccttrraall|ssppaattiiaall|hhiigghh--    |      |      |      |
 |                 |?â??        |?â??     |?â??    |ffrreeqquueennccyy|hhaa ?â??|oomm ?â??|iimm ?â??|
 |_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _|_?â_?_?_ _ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ _|_ _ _ _ _ _ |
 |      |_SS_uu_pp_ee_rr_II_mm_aa_gg_ee_|_00_.._00_00_88_ _ _ _ _ _ _|_77_.._22_88_66_ _ _ _|_00_.._11_33_11_ _ _|_0_._0_0_3_ _ _ _ _|_00_.._11_11_77_ _|_00_.._77_88_44_ _|_00_.._00_99_88_ |
 |NNAAIIPP  |_SS_RR_44_RR_SS_ _ _ _ _ _|_0_._0_1_6_ _ _ _ _ _ _|_33_.._44_77_11_ _ _ _|_1_._1_5_6_ _ _|_0_._0_1_0_ _ _ _ _|_0_._8_6_9_ _|_0_._0_7_7_ _|_0_._0_5_4_ |
@@ -85,16 +86,17 @@
 Display the matching points between the LR and SR images: ```python
 metrics.plot_spatial_matches() ```
                           [docs/images/example03.png]
 Display a summary of all the metrics: ```python metrics.plot_summary() ```
                           [docs/images/example04.png]
 Display the correctness of the SR image: ```python metrics.plot_tc() ```
                           [docs/images/example05.png]
-## Deeper understanding Explore the [API](/docs/API/model_parameters.md)
-section for more details about personalizing your benchmark experiments.
+## Deeper understanding Explore the [API](https://esaopensr.github.io/opensr-
+test/docs/API/config_pydantic.html) section for more details about
+personalizing your benchmark experiments.
                                  _[_o_p_e_n_s_r_-_t_e_s_t_]
 ## Citation If you use `opensr-test` in your research, please cite our paper:
 ``` Coming soon! ``` ## Acknowledgements This work was make with the support of
 the European Space Agency (ESA) under the project âExplainable AI:
 application to trustworthy super-resolution (OpenSR)â. Cesar Aybar
 acknowledges support by the National Council of Science, Technology, and
 Technological Innovation (CONCYTEC, Peru) through the âPROYECTOS DE
```

### Comparing `opensr-test-0.2.0/opensr_test.egg-info/SOURCES.txt` & `opensr-test-0.2.1/opensr_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opensr-test-0.2.0/setup.py` & `opensr-test-0.2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,29 +10,30 @@
     text_type = type("")
     with io.open(filename, mode="r", encoding="utf-8") as fd:
         return re.sub(text_type(r":[a-z]+:`~?(.*?)`"), text_type(r"``\1``"), fd.read())
 
 
 setup(
     name="opensr-test",
-    version="0.2.0",
+    version="0.2.1",
     url="https://github.com/ESAOpenSR/opensr-test",
     license="MIT",
     author="Cesar Aybar Camacho",
     author_email="csaybar@gmail.com",
     description="A comprehensive benchmark for real-world Sentinel-2 imagery super-resolution",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     packages=find_packages(
         exclude=("tests",), include=["opensr_test", "opensr_test.*"]
     ),
     install_requires=[
         "torch>=1.9.0",
         "numpy",
         "matplotlib",
+        "torchvision",
         "scikit-image",
         "scikit-learn",
         "requests",
         "kornia",
         "pydantic",
         "opencv-python",
     ],
```

