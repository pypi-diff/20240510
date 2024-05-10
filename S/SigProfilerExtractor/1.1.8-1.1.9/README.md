# Comparing `tmp/SigProfilerExtractor-1.1.8.tar.gz` & `tmp/SigProfilerExtractor-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SigProfilerExtractor-1.1.8.tar", last modified: Fri Jul  8 22:01:57 2022, max compression
+gzip compressed data, was "dist/SigProfilerExtractor-1.1.9.tar", last modified: Wed Jul 27 21:40:43 2022, max compression
```

## Comparing `SigProfilerExtractor-1.1.8.tar` & `SigProfilerExtractor-1.1.9.tar`

### file list

```diff
@@ -1,141 +1,82 @@
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2022-07-08 22:01:57.000000 SigProfilerExtractor-1.1.8/
--rw-r--r--   0 mbarnes    (501) staff       (20)     1809 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/.gitignore
--rw-r--r--   0 mbarnes    (501) staff       (20)      102 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/.travis.yml
--rw-r--r--   0 mbarnes    (501) staff       (20)     1351 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/LICENSE.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)      533 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/MANIFEST.in
--rw-r--r--   0 mbarnes    (501) staff       (20)    19468 2022-07-08 22:01:57.000000 SigProfilerExtractor-1.1.8/PKG-INFO
--rw-r--r--   0 mbarnes    (501) staff       (20)    17025 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/README.md
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2022-07-08 22:01:57.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/
--rw-r--r--   0 mbarnes    (501) staff       (20)    15956 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/PlotDecomposition.py
--rw-r--r--   0 mbarnes    (501) staff       (20)    14727 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/PlotDecomposition_CNV48.py
--rw-r--r--   0 mbarnes    (501) staff       (20)    13918 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/PlotDecomposition_DBS78.py
--rw-r--r--   0 mbarnes    (501) staff       (20)    14143 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/PlotDecomposition_ID83.py
--rw-r--r--   0 mbarnes    (501) staff       (20)    14267 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/PlotDecomposition_SBS1536.py
--rw-r--r--   0 mbarnes    (501) staff       (20)    14375 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/PlotDecomposition_SBS288.py
--rw-r--r--   0 mbarnes    (501) staff       (20)    14304 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/PlotDecomposition_SBS96.py
--rw-r--r--   0 mbarnes    (501) staff       (20)   148277 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/SigProfilerPlottingMatrix.py
--rw-r--r--   0 mbarnes    (501) staff       (20)       49 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/__init__.py
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2022-07-08 22:01:57.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/
--rwxr-xr-x   0 mbarnes    (501) staff       (20)     3342 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/21_breast_WGS_substitutions.mat
--rw-r--r--   0 mbarnes    (501) staff       (20)     4864 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Accolade_fermante.png
--rw-r--r--   0 mbarnes    (501) staff       (20)      803 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/CNV_features.tsv
--rw-r--r--   0 mbarnes    (501) staff       (20)    15995 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/CNV_signatures.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)     1641 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/CN_classes_dictionary.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   128402 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/DBS_signatures_genome_builds.xlsx
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2022-07-08 22:01:57.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2022-07-08 22:01:57.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/GRCh37/
--rw-r--r--   0 mbarnes    (501) staff       (20)    14328 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/GRCh37/COSMIC_v1_SBS_GRCh37.txt
--rwxr-xr-x   0 mbarnes    (501) staff       (20)    36586 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/GRCh37/COSMIC_v2_SBS_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17758 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/GRCh37/COSMIC_v3.1_DBS_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    29489 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/GRCh37/COSMIC_v3.1_ID_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   137506 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/GRCh37/COSMIC_v3.1_SBS_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17758 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/GRCh37/COSMIC_v3.2_DBS_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    29489 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/GRCh37/COSMIC_v3.2_ID_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   109467 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/GRCh37/COSMIC_v3.2_SBS288_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   148966 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/GRCh37/COSMIC_v3.2_SBS_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17757 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/GRCh37/COSMIC_v3_DBS_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    28686 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/GRCh37/COSMIC_v3_ID_GRCh37.txt
--rwxr-xr-x   0 mbarnes    (501) staff       (20)   128501 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/GRCh37/COSMIC_v3_SBS_GRCh37.txt
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2022-07-08 22:01:57.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/GRCh38/
--rw-r--r--   0 mbarnes    (501) staff       (20)    39244 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/GRCh38/COSMIC_v1_SBS_GRCh38.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    53205 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/GRCh38/COSMIC_v2_SBS_GRCh38.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17833 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/GRCh38/COSMIC_v3.1_DBS_GRCh38.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   138534 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/GRCh38/COSMIC_v3.1_SBS_GRCh38.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17833 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/GRCh38/COSMIC_v3.2_DBS_GRCh38.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   150027 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/GRCh38/COSMIC_v3.2_SBS_GRCh38.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17829 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/GRCh38/COSMIC_v3_DBS_GRCh38.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   129685 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/GRCh38/COSMIC_v3_SBS_GRCh38.txt
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2022-07-08 22:01:57.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/mm10/
--rw-r--r--   0 mbarnes    (501) staff       (20)    39213 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/mm10/COSMIC_v1_SBS_mm10.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    53208 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/mm10/COSMIC_v2_SBS_mm10.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17834 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/mm10/COSMIC_v3.1_DBS_mm10.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   138625 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/mm10/COSMIC_v3.1_SBS_mm10.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17834 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/mm10/COSMIC_v3.2_DBS_mm10.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   150107 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/mm10/COSMIC_v3.2_SBS_mm10.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17836 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/mm10/COSMIC_v3_DBS_mm10.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   129718 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/mm10/COSMIC_v3_SBS_mm10.txt
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2022-07-08 22:01:57.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/mm9/
--rw-r--r--   0 mbarnes    (501) staff       (20)    39213 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/mm9/COSMIC_v1_SBS_mm9.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    53199 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/mm9/COSMIC_v2_SBS_mm9.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17839 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/mm9/COSMIC_v3.1_DBS_mm9.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   138548 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/mm9/COSMIC_v3.1_SBS_mm9.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17839 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/mm9/COSMIC_v3.2_DBS_mm9.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   150036 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/mm9/COSMIC_v3.2_SBS_mm9.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17837 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/mm9/COSMIC_v3_DBS_mm9.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   129655 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/mm9/COSMIC_v3_SBS_mm9.txt
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2022-07-08 22:01:57.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/rn6/
--rw-r--r--   0 mbarnes    (501) staff       (20)    39230 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/rn6/COSMIC_v1_SBS_rn6.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    53187 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/rn6/COSMIC_v2_SBS_rn6.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17837 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/rn6/COSMIC_v3.1_DBS_rn6.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   138524 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/rn6/COSMIC_v3.1_SBS_rn6.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17837 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/rn6/COSMIC_v3.2_DBS_rn6.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   150001 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/rn6/COSMIC_v3.2_SBS_rn6.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17840 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/rn6/COSMIC_v3_DBS_rn6.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   129663 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Reference_Signatures/rn6/COSMIC_v3_SBS_rn6.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   380152 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/SBS_signatures_genome_builds.xlsx
--rw-r--r--   0 mbarnes    (501) staff       (20)     7124 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Samples.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)     3851 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/csvexample.csv
--rwxr-xr-x   0 mbarnes    (501) staff       (20)     8338 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/sigProfiler_DBS_signatures.csv
--rw-r--r--   0 mbarnes    (501) staff       (20)    16970 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/sigProfiler_ID_signatures.csv
--rwxr-xr-x   0 mbarnes    (501) staff       (20)    57422 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/sigProfiler_SBS_signatures_2018_03_28.csv
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2022-07-08 22:01:57.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/
--rw-r--r--   0 mbarnes    (501) staff       (20)    42134 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD3851a.vcf
--rw-r--r--   0 mbarnes    (501) staff       (20)   144692 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD3890a.vcf
--rw-r--r--   0 mbarnes    (501) staff       (20)   132516 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD3904a.vcf
--rw-r--r--   0 mbarnes    (501) staff       (20)   108261 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD3905a.vcf
--rw-r--r--   0 mbarnes    (501) staff       (20)   243267 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD3945a.vcf
--rw-r--r--   0 mbarnes    (501) staff       (20)   144314 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD4005a.vcf
--rw-r--r--   0 mbarnes    (501) staff       (20)   217281 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD4006a.vcf
--rw-r--r--   0 mbarnes    (501) staff       (20)    63094 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD4085a.vcf
--rw-r--r--   0 mbarnes    (501) staff       (20)    51960 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD4086a.vcf
--rw-r--r--   0 mbarnes    (501) staff       (20)    40304 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD4088a.vcf
--rw-r--r--   0 mbarnes    (501) staff       (20)   126650 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD4103a.vcf
--rw-r--r--   0 mbarnes    (501) staff       (20)   243377 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD4107a.vcf
--rw-r--r--   0 mbarnes    (501) staff       (20)   233696 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD4109a.vcf
--rw-r--r--   0 mbarnes    (501) staff       (20)   235200 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD4115a.vcf
--rw-r--r--   0 mbarnes    (501) staff       (20)   189909 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD4116a.vcf
--rw-r--r--   0 mbarnes    (501) staff       (20)  1672536 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD4120a.vcf
--rw-r--r--   0 mbarnes    (501) staff       (20)    92642 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD4192a.vcf
--rw-r--r--   0 mbarnes    (501) staff       (20)    35093 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD4194a.vcf
--rw-r--r--   0 mbarnes    (501) staff       (20)   107668 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD4198a.vcf
--rw-r--r--   0 mbarnes    (501) staff       (20)   164069 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD4199a.vcf
--rw-r--r--   0 mbarnes    (501) staff       (20)    59915 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD4248a.vcf
--rw-r--r--   0 mbarnes    (501) staff       (20)     7721 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/decomposition.py
--rw-r--r--   0 mbarnes    (501) staff       (20)     3860 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/estimate_best_solution.py
--rw-r--r--   0 mbarnes    (501) staff       (20)     9307 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/nmf_cpu.py
--rw-r--r--   0 mbarnes    (501) staff       (20)     9273 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/nmf_gpu.py
--rw-r--r--   0 mbarnes    (501) staff       (20)     6292 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/plotActivity.py
--rw-r--r--   0 mbarnes    (501) staff       (20)    42699 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/sigpro.py
--rw-r--r--   0 mbarnes    (501) staff       (20)    35383 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/single_sample.py
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2022-07-08 22:01:57.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/src/
--rw-r--r--   0 mbarnes    (501) staff       (20)    12535 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/src/Accolade_fermante.png
--rw-r--r--   0 mbarnes    (501) staff       (20)      165 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/src/CREDIT.md
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2022-07-08 22:01:57.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/src/Fonts/
--rw-r--r--   0 mbarnes    (501) staff       (20)   750984 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/src/Fonts/Arial Bold.ttf
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2022-07-08 22:01:57.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/src/FormatFiles/
--rw-r--r--   0 mbarnes    (501) staff       (20)    13740 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/src/FormatFiles/Sample_Files.DBS1248.all
--rw-r--r--   0 mbarnes    (501) staff       (20)     1686 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/src/FormatFiles/Sample_Files.DBS186.all
--rw-r--r--   0 mbarnes    (501) staff       (20)    38700 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/src/FormatFiles/Sample_Files.DBS2976.all
--rw-r--r--   0 mbarnes    (501) staff       (20)      558 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/src/FormatFiles/Sample_Files.DBS78.all
--rw-r--r--   0 mbarnes    (501) staff       (20)      309 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/src/FormatFiles/Sample_Files.ID28.all
--rw-r--r--   0 mbarnes    (501) staff       (20)     5407 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/src/FormatFiles/Sample_Files.ID415.all
--rw-r--r--   0 mbarnes    (501) staff       (20)      926 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/src/FormatFiles/Sample_Files.ID83.all
--rw-r--r--   0 mbarnes    (501) staff       (20)    16908 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/src/FormatFiles/Sample_Files.SBS1536.all
--rw-r--r--   0 mbarnes    (501) staff       (20)      180 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/src/FormatFiles/Sample_Files.SBS24.all
--rw-r--r--   0 mbarnes    (501) staff       (20)     4236 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/src/FormatFiles/Sample_Files.SBS384.all
--rw-r--r--   0 mbarnes    (501) staff       (20)       42 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/src/FormatFiles/Sample_Files.SBS6.all
--rw-r--r--   0 mbarnes    (501) staff       (20)    79884 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/src/FormatFiles/Sample_Files.SBS6144.all
--rw-r--r--   0 mbarnes    (501) staff       (20)      876 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/src/FormatFiles/Sample_Files.SBS96.all
--rw-r--r--   0 mbarnes    (501) staff       (20)    99476 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/subroutines.py
--rw-r--r--   0 mbarnes    (501) staff       (20)     4669 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/tmbplot.py
--rw-r--r--   0 mbarnes    (501) staff       (20)      236 2022-07-08 22:01:56.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor/version.py
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2022-07-08 22:01:57.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor.egg-info/
--rw-r--r--   0 mbarnes    (501) staff       (20)    19468 2022-07-08 22:01:57.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor.egg-info/PKG-INFO
--rw-r--r--   0 mbarnes    (501) staff       (20)     7006 2022-07-08 22:01:57.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor.egg-info/SOURCES.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)        1 2022-07-08 22:01:57.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor.egg-info/dependency_links.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)        1 2022-07-08 22:00:55.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor.egg-info/not-zip-safe
--rw-r--r--   0 mbarnes    (501) staff       (20)      279 2022-07-08 22:01:57.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor.egg-info/requires.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)       21 2022-07-08 22:01:57.000000 SigProfilerExtractor-1.1.8/SigProfilerExtractor.egg-info/top_level.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)       38 2022-07-08 22:01:57.000000 SigProfilerExtractor-1.1.8/setup.cfg
--rw-r--r--   0 mbarnes    (501) staff       (20)     2910 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/setup.py
--rw-r--r--   0 mbarnes    (501) staff       (20)      374 2022-07-08 22:00:34.000000 SigProfilerExtractor-1.1.8/test.py
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2022-07-27 21:40:43.000000 SigProfilerExtractor-1.1.9/
+-rw-r--r--   0 mbarnes    (501) staff       (20)     1842 2022-07-27 21:40:38.000000 SigProfilerExtractor-1.1.9/.gitignore
+-rw-r--r--   0 mbarnes    (501) staff       (20)      102 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/.travis.yml
+-rw-r--r--   0 mbarnes    (501) staff       (20)     1351 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/LICENSE.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)      221 2022-07-27 21:40:38.000000 SigProfilerExtractor-1.1.9/MANIFEST.in
+-rw-r--r--   0 mbarnes    (501) staff       (20)    19468 2022-07-27 21:40:43.000000 SigProfilerExtractor-1.1.9/PKG-INFO
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17025 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/README.md
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2022-07-27 21:40:42.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/
+-rw-r--r--   0 mbarnes    (501) staff       (20)    15956 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/PlotDecomposition.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)    14727 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/PlotDecomposition_CNV48.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)    13918 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/PlotDecomposition_DBS78.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)    14143 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/PlotDecomposition_ID83.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)    14267 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/PlotDecomposition_SBS1536.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)    14375 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/PlotDecomposition_SBS288.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)    14304 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/PlotDecomposition_SBS96.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)   148277 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/SigProfilerPlottingMatrix.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)       49 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/__init__.py
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2022-07-27 21:40:42.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/
+-rwxr-xr-x   0 mbarnes    (501) staff       (20)     3342 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/21_breast_WGS_substitutions.mat
+-rw-r--r--   0 mbarnes    (501) staff       (20)      803 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/CNV_features.tsv
+-rw-r--r--   0 mbarnes    (501) staff       (20)     1641 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/CN_classes_dictionary.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)     7124 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/Samples.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)     3851 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/csvexample.csv
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2022-07-27 21:40:43.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/
+-rw-r--r--   0 mbarnes    (501) staff       (20)    42134 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD3851a.vcf
+-rw-r--r--   0 mbarnes    (501) staff       (20)   144692 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD3890a.vcf
+-rw-r--r--   0 mbarnes    (501) staff       (20)   132516 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD3904a.vcf
+-rw-r--r--   0 mbarnes    (501) staff       (20)   108261 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD3905a.vcf
+-rw-r--r--   0 mbarnes    (501) staff       (20)   243267 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD3945a.vcf
+-rw-r--r--   0 mbarnes    (501) staff       (20)   144314 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD4005a.vcf
+-rw-r--r--   0 mbarnes    (501) staff       (20)   217281 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD4006a.vcf
+-rw-r--r--   0 mbarnes    (501) staff       (20)    63094 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD4085a.vcf
+-rw-r--r--   0 mbarnes    (501) staff       (20)    51960 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD4086a.vcf
+-rw-r--r--   0 mbarnes    (501) staff       (20)    40304 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD4088a.vcf
+-rw-r--r--   0 mbarnes    (501) staff       (20)   126650 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD4103a.vcf
+-rw-r--r--   0 mbarnes    (501) staff       (20)   243377 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD4107a.vcf
+-rw-r--r--   0 mbarnes    (501) staff       (20)   233696 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD4109a.vcf
+-rw-r--r--   0 mbarnes    (501) staff       (20)   235200 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD4115a.vcf
+-rw-r--r--   0 mbarnes    (501) staff       (20)   189909 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD4116a.vcf
+-rw-r--r--   0 mbarnes    (501) staff       (20)  1672536 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD4120a.vcf
+-rw-r--r--   0 mbarnes    (501) staff       (20)    92642 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD4192a.vcf
+-rw-r--r--   0 mbarnes    (501) staff       (20)    35093 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD4194a.vcf
+-rw-r--r--   0 mbarnes    (501) staff       (20)   107668 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD4198a.vcf
+-rw-r--r--   0 mbarnes    (501) staff       (20)   164069 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD4199a.vcf
+-rw-r--r--   0 mbarnes    (501) staff       (20)    59915 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD4248a.vcf
+-rw-r--r--   0 mbarnes    (501) staff       (20)     3860 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/estimate_best_solution.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)     9307 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/nmf_cpu.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)     9273 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/nmf_gpu.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)     6292 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/plotActivity.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)    42799 2022-07-27 21:40:38.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/sigpro.py
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2022-07-27 21:40:43.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/src/
+-rw-r--r--   0 mbarnes    (501) staff       (20)    12535 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/src/Accolade_fermante.png
+-rw-r--r--   0 mbarnes    (501) staff       (20)      165 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/src/CREDIT.md
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2022-07-27 21:40:43.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/src/Fonts/
+-rw-r--r--   0 mbarnes    (501) staff       (20)   750984 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/src/Fonts/Arial Bold.ttf
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2022-07-27 21:40:43.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/src/FormatFiles/
+-rw-r--r--   0 mbarnes    (501) staff       (20)    13740 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/src/FormatFiles/Sample_Files.DBS1248.all
+-rw-r--r--   0 mbarnes    (501) staff       (20)     1686 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/src/FormatFiles/Sample_Files.DBS186.all
+-rw-r--r--   0 mbarnes    (501) staff       (20)    38700 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/src/FormatFiles/Sample_Files.DBS2976.all
+-rw-r--r--   0 mbarnes    (501) staff       (20)      558 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/src/FormatFiles/Sample_Files.DBS78.all
+-rw-r--r--   0 mbarnes    (501) staff       (20)      309 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/src/FormatFiles/Sample_Files.ID28.all
+-rw-r--r--   0 mbarnes    (501) staff       (20)     5407 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/src/FormatFiles/Sample_Files.ID415.all
+-rw-r--r--   0 mbarnes    (501) staff       (20)      925 2022-07-27 21:40:38.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/src/FormatFiles/Sample_Files.ID83.all
+-rw-r--r--   0 mbarnes    (501) staff       (20)    16908 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/src/FormatFiles/Sample_Files.SBS1536.all
+-rw-r--r--   0 mbarnes    (501) staff       (20)      180 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/src/FormatFiles/Sample_Files.SBS24.all
+-rw-r--r--   0 mbarnes    (501) staff       (20)     4236 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/src/FormatFiles/Sample_Files.SBS384.all
+-rw-r--r--   0 mbarnes    (501) staff       (20)       42 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/src/FormatFiles/Sample_Files.SBS6.all
+-rw-r--r--   0 mbarnes    (501) staff       (20)    79884 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/src/FormatFiles/Sample_Files.SBS6144.all
+-rw-r--r--   0 mbarnes    (501) staff       (20)      876 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/src/FormatFiles/Sample_Files.SBS96.all
+-rw-r--r--   0 mbarnes    (501) staff       (20)    63492 2022-07-27 21:40:38.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/subroutines.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)     4669 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/tmbplot.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)      185 2022-07-27 21:40:42.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor/version.py
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2022-07-27 21:40:42.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor.egg-info/
+-rw-r--r--   0 mbarnes    (501) staff       (20)    19468 2022-07-27 21:40:42.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor.egg-info/PKG-INFO
+-rw-r--r--   0 mbarnes    (501) staff       (20)     3142 2022-07-27 21:40:42.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor.egg-info/SOURCES.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)        1 2022-07-27 21:40:42.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor.egg-info/dependency_links.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)        1 2022-07-27 21:40:42.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor.egg-info/not-zip-safe
+-rw-r--r--   0 mbarnes    (501) staff       (20)      277 2022-07-27 21:40:42.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor.egg-info/requires.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)       21 2022-07-27 21:40:42.000000 SigProfilerExtractor-1.1.9/SigProfilerExtractor.egg-info/top_level.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)       38 2022-07-27 21:40:43.000000 SigProfilerExtractor-1.1.9/setup.cfg
+-rw-r--r--   0 mbarnes    (501) staff       (20)     2857 2022-07-27 21:40:38.000000 SigProfilerExtractor-1.1.9/setup.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)      374 2022-07-27 20:44:00.000000 SigProfilerExtractor-1.1.9/test.py
```

### Comparing `SigProfilerExtractor-1.1.8/.gitignore` & `SigProfilerExtractor-1.1.9/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 wheels/
 pip-wheel-metadata/
 share/python-wheels/
 *.egg-info/
 .installed.cfg
 *.egg
 MANIFEST
+SigProfilerExtractor/version.py 
 
 # PyInstaller
 #  Usually these files are written by a python script from a template
 #  before PyInstaller builds the exe, so as to inject date/other infos into it.
 *.manifest
 *.spec
```

### Comparing `SigProfilerExtractor-1.1.8/LICENSE.txt` & `SigProfilerExtractor-1.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/PKG-INFO` & `SigProfilerExtractor-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SigProfilerExtractor
-Version: 1.1.8
+Version: 1.1.9
 Summary: Extracts mutational signatures from mutational catalogues
 Home-page: https://github.com/AlexandrovLab/SigProfilerExtractor.git
 Author: S Mishu Ashiqul Islam
 Author-email: m0islam@ucsd.edu
 License: UCSD
 Description: [![Docs](https://img.shields.io/badge/docs-latest-blue.svg)](https://osf.io/t6j7u/wiki/home/) 
         [![License](https://img.shields.io/badge/License-BSD\%202--Clause-orange.svg)](https://opensource.org/licenses/BSD-2-Clause)
```

### Comparing `SigProfilerExtractor-1.1.8/README.md` & `SigProfilerExtractor-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/PlotDecomposition.py` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/PlotDecomposition.py`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/PlotDecomposition_CNV48.py` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/PlotDecomposition_CNV48.py`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/PlotDecomposition_DBS78.py` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/PlotDecomposition_DBS78.py`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/PlotDecomposition_ID83.py` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/PlotDecomposition_ID83.py`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/PlotDecomposition_SBS1536.py` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/PlotDecomposition_SBS1536.py`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/PlotDecomposition_SBS288.py` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/PlotDecomposition_SBS288.py`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/PlotDecomposition_SBS96.py` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/PlotDecomposition_SBS96.py`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/SigProfilerPlottingMatrix.py` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/SigProfilerPlottingMatrix.py`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/21_breast_WGS_substitutions.mat` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/21_breast_WGS_substitutions.mat`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/CNV_features.tsv` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/CNV_features.tsv`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/CN_classes_dictionary.txt` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/CN_classes_dictionary.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/Samples.txt` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/Samples.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/csvexample.csv` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/csvexample.csv`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD3851a.vcf` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD3851a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD3890a.vcf` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD3890a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD3904a.vcf` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD3904a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD3905a.vcf` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD3905a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD3945a.vcf` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD3945a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD4005a.vcf` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD4005a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD4006a.vcf` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD4006a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD4085a.vcf` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD4085a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD4086a.vcf` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD4086a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD4088a.vcf` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD4088a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD4103a.vcf` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD4103a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD4107a.vcf` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD4107a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD4109a.vcf` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD4109a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD4115a.vcf` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD4115a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD4116a.vcf` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD4116a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD4120a.vcf` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD4120a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD4192a.vcf` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD4192a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD4194a.vcf` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD4194a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD4198a.vcf` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD4198a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD4199a.vcf` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD4199a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/data/vcftest/PD4248a.vcf` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/data/vcftest/PD4248a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/estimate_best_solution.py` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/estimate_best_solution.py`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/nmf_cpu.py` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/nmf_cpu.py`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/nmf_gpu.py` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/nmf_gpu.py`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/plotActivity.py` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/plotActivity.py`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/sigpro.py` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/sigpro.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,19 +39,21 @@
 import sigProfilerPlotting 
 import multiprocessing
 from SigProfilerExtractor import subroutines as sub
 import SigProfilerMatrixGenerator
 from SigProfilerMatrixGenerator.scripts import SigProfilerMatrixGeneratorFunc as datadump   
 import multiprocessing as mp
 import SigProfilerExtractor as cosmic
-from SigProfilerExtractor import single_sample as ss
+# from SigProfilerExtractor import single_sample as ss
 import SigProfilerAssignment as spa
+from SigProfilerAssignment import single_sample as spasub
 from SigProfilerAssignment import decomposition as decomp
-from SigProfilerAssignment import Analyzer as Analyze
+# from SigProfilerAssignment import Analyzer as Analyze
 from numpy.random import SeedSequence
+# from scipy.optimize import nnls
 
 def memory_usage():
     pid = os.getpid()
     py = psutil.Process(pid)
     memoryUse1 = py.memory_info()[0]/2.**30  # memory use in GB...I think
     print('\n************** Reported Current Memory Use: '+ str(round(memoryUse1,2))+" GB *****************\n")
 
@@ -725,15 +727,15 @@
             # remove signatures only if the process stability is above a thresh-hold of 0.85
             if  avgSilhouetteCoefficients> -1.0:   
                 stic = time.time() 
                 if cpu > 0:
                     pool = mp.Pool(processes=cpu)
                 else:
                     pool = mp.Pool()
-                results = [pool.apply_async(ss.fit_signatures_pool, args=(genomes,processAvg,x,)) for x in range(genomes.shape[1])]
+                results = [pool.apply_async(spasub.fit_signatures_pool, args=(genomes,processAvg,x,)) for x in range(genomes.shape[1])]
                 pooloutput = [p.get() for p in results]
                 pool.close()
                                     
                 for i in range(len(pooloutput)):
                     exposureAvg[:,i]=pooloutput[i][0] 
                 stoc = time.time()
                 print ("Optimization time is {} seconds".format(stoc-stic))
```

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/src/Accolade_fermante.png` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/src/Accolade_fermante.png`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/src/Fonts/Arial Bold.ttf` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/src/Fonts/Arial Bold.ttf`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/src/FormatFiles/Sample_Files.DBS1248.all` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/src/FormatFiles/Sample_Files.DBS1248.all`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/src/FormatFiles/Sample_Files.DBS186.all` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/src/FormatFiles/Sample_Files.DBS186.all`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/src/FormatFiles/Sample_Files.DBS2976.all` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/src/FormatFiles/Sample_Files.DBS2976.all`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/src/FormatFiles/Sample_Files.DBS78.all` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/src/FormatFiles/Sample_Files.DBS78.all`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/src/FormatFiles/Sample_Files.ID415.all` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/src/FormatFiles/Sample_Files.ID415.all`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/src/FormatFiles/Sample_Files.ID83.all` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/src/FormatFiles/Sample_Files.ID83.all`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-MutationsType
+MutationType
 1:Del:C:0
 1:Del:C:1
 1:Del:C:2
 1:Del:C:3
 1:Del:C:4
 1:Del:C:5
 1:Del:T:0
```

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/src/FormatFiles/Sample_Files.SBS1536.all` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/src/FormatFiles/Sample_Files.SBS1536.all`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/src/FormatFiles/Sample_Files.SBS384.all` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/src/FormatFiles/Sample_Files.SBS384.all`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/src/FormatFiles/Sample_Files.SBS6144.all` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/src/FormatFiles/Sample_Files.SBS6144.all`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/src/FormatFiles/Sample_Files.SBS96.all` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/src/FormatFiles/Sample_Files.SBS96.all`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor/tmbplot.py` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor/tmbplot.py`

 * *Files identical despite different names*

### Comparing `SigProfilerExtractor-1.1.8/SigProfilerExtractor.egg-info/PKG-INFO` & `SigProfilerExtractor-1.1.9/SigProfilerExtractor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SigProfilerExtractor
-Version: 1.1.8
+Version: 1.1.9
 Summary: Extracts mutational signatures from mutational catalogues
 Home-page: https://github.com/AlexandrovLab/SigProfilerExtractor.git
 Author: S Mishu Ashiqul Islam
 Author-email: m0islam@ucsd.edu
 License: UCSD
 Description: [![Docs](https://img.shields.io/badge/docs-latest-blue.svg)](https://osf.io/t6j7u/wiki/home/) 
         [![License](https://img.shields.io/badge/License-BSD\%202--Clause-orange.svg)](https://opensource.org/licenses/BSD-2-Clause)
```

### Comparing `SigProfilerExtractor-1.1.8/setup.py` & `SigProfilerExtractor-1.1.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,42 +4,42 @@
 import sys
 import subprocess
 
 #remove the dist folder first if exists
 if os.path.exists("dist"):
     shutil.rmtree("dist")
 
-VERSION = '1.1.8'
+VERSION = '1.1.9'
 
 
 with open('README.md') as f:
 	long_description = f.read()
 
 def write_version_py(filename='SigProfilerExtractor/version.py'):
     # Copied from numpy setup.py
     cnt = """
 # THIS FILE IS GENERATED FROM SIGPROFILEREXTRACTOR SETUP.PY
 short_version = '%(version)s'
 version = '%(version)s'
-Update = 'Adding SigProfilerAssignment version to Job Metadata file; Updating "opportunity_genome" parameter passed to SPA'
+Update = 'Fix typos, requirements, and remove legacy decomposition code'
     
     """
     fh = open(filename, 'w')
     fh.write(cnt % {'version': VERSION,})
     fh.close()
 requirements=[
           'matplotlib>=3.4.2,<=3.4.3',
           'scipy>=1.6.3',
           'torch>=1.8.1',
           'numpy>=1.21.2',
           'pandas>=1.2.4', 
           'nimfa>=1.1.0', 
-          'SigProfilerMatrixGenerator>=1.1.30', 
-          'sigProfilerPlotting>=1.1.15', 
-          'SigProfilerAssignment>=0.0.5',
+          'SigProfilerMatrixGenerator>=1.2.8', 
+          'sigProfilerPlotting>=1.2.2', 
+          'SigProfilerAssignment>=0.0.8',
           'pillow',
           'statsmodels>=0.9.0',
           'scikit-learn>=0.24.2',
           'psutil>=5.6.1',
           'reportlab>=3.5.42',
           'PyPDF2>=1.26.0'
            ]
```

