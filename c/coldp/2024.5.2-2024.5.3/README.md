# Comparing `tmp/coldp-2024.5.2.tar.gz` & `tmp/coldp-2024.5.3.tar.gz`

## Comparing `coldp-2024.5.2.tar` & `coldp-2024.5.3.tar`

### file list

```diff
@@ -1,53 +1,103 @@
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 coldp-2024.5.2/.gitattributes
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 coldp-2024.5.2/VERSION
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 coldp-2024.5.2/makefile
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 coldp-2024.5.2/version.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/Makefile
--rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/make.bat
--rw-r--r--   0        0        0    97590 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/coldp.html
--rw-r--r--   0        0        0    25588 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/genindex.html
--rw-r--r--   0        0        0     4743 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/index.html
--rw-r--r--   0        0        0    13217 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/name-bundle.html
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/objects.inv
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/search.html
--rw-r--r--   0        0        0    21036 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/searchindex.js
--rw-r--r--   0        0        0    11850 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/_static/alabaster.css
--rw-r--r--   0        0        0    16020 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/_static/basic.css
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/_static/custom.css
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/_static/doctools.js
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/_static/file.png
--rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/_static/plus.png
--rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/_static/pygments.css
--rw-r--r--   0        0        0    20731 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/_static/searchtools.js
--rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/_static/sphinx_highlight.js
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/build/html/_static/sphinx_paramlinks.css
--rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/source/coldp.rst
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/source/conf.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/source/index.rst
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 coldp-2024.5.2/docs/source/name-bundle.rst
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 coldp-2024.5.2/src/coldp/__init__.py
--rw-r--r--   0        0        0   100701 2020-02-02 00:00:00.000000 coldp-2024.5.2/src/coldp/coldp.py
--rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 coldp-2024.5.2/src/coldp/coldp_coldp.svg
--rw-r--r--   0        0        0    10909 2020-02-02 00:00:00.000000 coldp-2024.5.2/src/coldp/coldp_distribution.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 coldp-2024.5.2/src/coldp/testit.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 coldp-2024.5.2/test/input/Tonzidae/Distribution.tsv
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 coldp-2024.5.2/test/input/Tonzidae/Media.tsv
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 coldp-2024.5.2/test/input/Tonzidae/NameRelation.tsv
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 coldp-2024.5.2/test/input/Tonzidae/NameUsage.tsv
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 coldp-2024.5.2/test/input/Tonzidae/Reference.tsv
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 coldp-2024.5.2/test/input/Tonzidae/SpeciesEstimate.tsv
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 coldp-2024.5.2/test/input/Tonzidae/SpeciesInteraction.tsv
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 coldp-2024.5.2/test/input/Tonzidae/TaxonConceptRelation.tsv
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 coldp-2024.5.2/test/input/Tonzidae/TypeMaterial.tsv
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 coldp-2024.5.2/test/input/Tonzidae/VernacularName.tsv
--rw-r--r--   0        0        0   697219 2020-02-02 00:00:00.000000 coldp-2024.5.2/test/input/Tonzidae/logo.png
--rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 coldp-2024.5.2/test/input/Tonzidae/metadata.yaml
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 coldp-2024.5.2/test/input/Tonzidae/reference.json
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 coldp-2024.5.2/.gitignore
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 coldp-2024.5.2/LICENSE
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 coldp-2024.5.2/README.md
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 coldp-2024.5.2/pyproject.toml
--rw-r--r--   0        0        0     4222 2020-02-02 00:00:00.000000 coldp-2024.5.2/PKG-INFO
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 coldp-2024.5.3/.gitattributes
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 coldp-2024.5.3/VERSION
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 coldp-2024.5.3/makefile
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 coldp-2024.5.3/version.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/Makefile
+-rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/make.bat
+-rw-r--r--   0        0        0   118424 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/coldp.html
+-rw-r--r--   0        0        0    30155 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/genindex.html
+-rw-r--r--   0        0        0     8209 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/index.html
+-rw-r--r--   0        0        0    13606 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/name-bundle.html
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/objects.inv
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/search.html
+-rw-r--r--   0        0        0    26118 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/searchindex.js
+-rw-r--r--   0        0        0    21622 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/usage.html
+-rw-r--r--   0        0        0    11850 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/_static/alabaster.css
+-rw-r--r--   0        0        0    16020 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/_static/basic.css
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/_static/custom.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/_static/doctools.js
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/_static/file.png
+-rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/_static/plus.png
+-rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/_static/pygments.css
+-rw-r--r--   0        0        0    20731 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/html/_static/sphinx_paramlinks.css
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/.buildinfo
+-rw-r--r--   0        0        0   215766 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/COLDP.pdf
+-rw-r--r--   0        0        0   258568 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/index.html
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/objects.inv
+-rw-r--r--   0        0        0    16018 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/basic.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/doctools.js
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/file.png
+-rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/language_data.js
+-rw-r--r--   0        0        0    27326 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/main.css
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/plus.png
+-rw-r--r--   0        0        0     5003 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/pygments.css
+-rw-r--r--   0        0        0    20731 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/searchtools.js
+-rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0   201708 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/fonts/FiraMono-Bold.ttf
+-rw-r--r--   0        0        0   169056 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/fonts/FiraMono-Medium.ttf
+-rw-r--r--   0        0        0   170204 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/fonts/FiraMono-Regular.ttf
+-rw-r--r--   0        0        0   521796 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/fonts/FiraSans-Bold.otf
+-rw-r--r--   0        0        0   524840 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/fonts/FiraSans-Italic.otf
+-rw-r--r--   0        0        0   505308 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/fonts/FiraSans-Light.otf
+-rw-r--r--   0        0        0   522236 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/fonts/FiraSans-LightItalic.otf
+-rw-r--r--   0        0        0   507828 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/fonts/FiraSans-Regular.otf
+-rw-r--r--   0        0        0   192304 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/fonts/WorkSans-Bold.ttf
+-rw-r--r--   0        0        0   191916 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/fonts/WorkSans-Regular.ttf
+-rw-r--r--   0        0        0   192372 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/fonts/WorkSans-SemiBold.ttf
+-rw-r--r--   0        0        0   194078 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/fonts/fa-solid-900.eot
+-rw-r--r--   0        0        0   849240 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/fonts/fa-solid-900.svg
+-rw-r--r--   0        0        0   193792 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/fonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0    99004 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/fonts/fa-solid-900.woff
+-rw-r--r--   0        0        0    76120 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/fonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_admonition.scss
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_alerts.scss
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_api.scss
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_back-cover.scss
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_blocks.scss
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_code.scss
+-rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_cover.scss
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_fonts.scss
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_lists.scss
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_needs.scss
+-rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_pages.scss
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_tables.scss
+-rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_text.scss
+-rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_toc.scss
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/_variables.scss
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/build/simplepdf/_static/styles/sources/main.scss
+-rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/source/coldp.rst
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/source/conf.py
+-rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/source/index.pdf
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/source/index.rst
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/source/name-bundle.rst
+-rw-r--r--   0        0        0     6565 2020-02-02 00:00:00.000000 coldp-2024.5.3/docs/source/usage.rst
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 coldp-2024.5.3/src/coldp/__init__.py
+-rw-r--r--   0        0        0   113448 2020-02-02 00:00:00.000000 coldp-2024.5.3/src/coldp/coldp.py
+-rw-r--r--   0        0        0    10909 2020-02-02 00:00:00.000000 coldp-2024.5.3/src/coldp/coldp_distribution.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 coldp-2024.5.3/src/coldp/testit.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 coldp-2024.5.3/test/test_coldp.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 coldp-2024.5.3/test/input/Tonzidae/Distribution.tsv
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 coldp-2024.5.3/test/input/Tonzidae/Media.tsv
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 coldp-2024.5.3/test/input/Tonzidae/NameRelation.tsv
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 coldp-2024.5.3/test/input/Tonzidae/NameUsage.tsv
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 coldp-2024.5.3/test/input/Tonzidae/Reference.tsv
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 coldp-2024.5.3/test/input/Tonzidae/SpeciesEstimate.tsv
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 coldp-2024.5.3/test/input/Tonzidae/SpeciesInteraction.tsv
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 coldp-2024.5.3/test/input/Tonzidae/TaxonConceptRelation.tsv
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 coldp-2024.5.3/test/input/Tonzidae/TypeMaterial.tsv
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 coldp-2024.5.3/test/input/Tonzidae/VernacularName.tsv
+-rw-r--r--   0        0        0   697219 2020-02-02 00:00:00.000000 coldp-2024.5.3/test/input/Tonzidae/logo.png
+-rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 coldp-2024.5.3/test/input/Tonzidae/metadata.yaml
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 coldp-2024.5.3/test/input/Tonzidae/reference.json
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 coldp-2024.5.3/.gitignore
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 coldp-2024.5.3/LICENSE
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 coldp-2024.5.3/README.md
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 coldp-2024.5.3/pyproject.toml
+-rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 coldp-2024.5.3/PKG-INFO
```

### Comparing `coldp-2024.5.2/version.py` & `coldp-2024.5.3/version.py`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.2/docs/Makefile` & `coldp-2024.5.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.2/docs/make.bat` & `coldp-2024.5.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.2/docs/build/html/coldp.html` & `coldp-2024.5.3/docs/build/html/coldp.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>coldp.COLDP &#8212; COLDP 2024.5.2 documentation</title>
+    <title>coldp.COLDP &#8212; COLDP 2024.5.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
-    <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css?v=dd72e65a" />
-    <script src="_static/documentation_options.js?v=1723c9d4"></script>
+    <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
+    <script src="_static/documentation_options.js?v=b35b4dcd"></script>
     <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="coldp.NameBundle" href="name-bundle.html" />
-    <link rel="prev" title="COLDP" href="index.html" />
+    <link rel="prev" title="coldp" href="index.html" />
    
   <link rel="stylesheet" href="_static/custom.css" type="text/css" />
   
 
   
   
 
@@ -33,17 +33,17 @@
 
           <div class="body" role="main">
             
   <section id="coldp-coldp">
 <h1>coldp.COLDP<a class="headerlink" href="#coldp-coldp" title="Link to this heading">¶</a></h1>
 <section id="class">
 <h2>Class<a class="headerlink" href="#class" title="Link to this heading">¶</a></h2>
-<dl class="py class">
-<dt class="sig sig-object py">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">coldp.</span></span><span class="sig-name descname"><span class="pre">COLDP</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">name</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">folder</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'.'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">code</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'ICZN'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">default_taxon_record</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">insert_species_for_trinomials</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">create_subspecies_for_infrasubspecifics</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">create_synonyms_without_subgenus</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">basionyms_from_synonyms</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">classification_from_parents</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">allow_repeated_binomials</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">create_taxa_for_not_established</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">issues_to_stdout</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">context</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span></dt>
+<dl class="py method">
+<dt class="sig sig-object py" id="coldp.COLDP.__init__">
+<span class="sig-prename descclassname"><span class="pre">COLDP.</span></span><span class="sig-name descname"><span class="pre">__init__</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">name</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">folder</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'.'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">code</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'ICZN'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">default_taxon_record</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">insert_species_for_trinomials</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">create_subspecies_for_infrasubspecifics</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">create_synonyms_without_subgenus</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">basionyms_from_synonyms</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">classification_from_parents</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">allow_repeated_binomials</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">create_taxa_for_not_established</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">issues_to_stdout</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">context</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#coldp.COLDP.__init__" title="Link to this definition">¶</a></dt>
 <dd><p>Class to manage a set of Pandas dataframes for CSV tables in Catalogue
 of Life Data Package.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="coldp.COLDP.params.name"></span><strong>name</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.params.name">¶</a> – The name for the COLDP package. If a folder of this name exists inside the folder specied by the folder parameter, this COLDP instance will be initialised with the contents of any COLDP-compliant CSV or TSV files in the named folder.</p></li>
 <li><p><span class="target" id="coldp.COLDP.params.folder"></span><strong>folder</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.params.folder">¶</a> – Name of folder that may contain the named COLDP source folder from which source files should be read (name specified via the name parameter) and that is the default folder in which a COLDP folder will be written when the COLDP instance is saved. This is not the folder in which the CSV files are written. It is the folder which will contain the subfolder holding CSV files.</p></li>
@@ -137,15 +137,29 @@
 
 </section>
 <section id="add-or-modify-records">
 <h3>Add or modify records<a class="headerlink" href="#add-or-modify-records" title="Link to this heading">¶</a></h3>
 <dl class="py method">
 <dt class="sig sig-object py" id="coldp.COLDP.start_name_bundle">
 <span class="sig-prename descclassname"><span class="pre">COLDP.</span></span><span class="sig-name descname"><span class="pre">start_name_bundle</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">accepted</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">incertae_sedis</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sic</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#coldp.COLDP.start_name_bundle" title="Link to this definition">¶</a></dt>
-<dd></dd></dl>
+<dd><p>Return a NameBundle object based on the supplied accepted name and referencing this COLDP instance</p>
+<dl class="field-list simple">
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><ul class="simple">
+<li><p><span class="target" id="coldp.COLDP.start_name_bundle.params.accepted"></span><strong>accepted</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.start_name_bundle.params.accepted">¶</a> – Dictionary containing COLDP Name record for accepted name</p></li>
+<li><p><span class="target" id="coldp.COLDP.start_name_bundle.params.incertae_sedis"></span><strong>incertae_sedis</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.start_name_bundle.params.incertae_sedis">¶</a> – If True, the associated COLDP Taxon Record will be flagged as <em>incertae sedis</em></p></li>
+<li><p><span class="target" id="coldp.COLDP.start_name_bundle.params.sic"></span><strong>sic</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.start_name_bundle.params.sic">¶</a> – If True, issues will not be reported if the name is not properly code-compliant</p></li>
+</ul>
+</dd>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
+<dd class="field-even"><p>NameBundle instance initialised with supplied parameters</p>
+</dd>
+</dl>
+<p>This is the normal way to construct a new NameBundle object.</p>
+</dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="coldp.COLDP.add_names">
 <span class="sig-prename descclassname"><span class="pre">COLDP.</span></span><span class="sig-name descname"><span class="pre">add_names</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">bundle</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">parent</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#coldp.COLDP.add_names" title="Link to this definition">¶</a></dt>
 <dd><p>Ensure one or more names are included in names dataframe and update
 taxa and synonyms dataframes as necessary</p>
 <dl class="field-list simple">
@@ -166,17 +180,17 @@
 additional synonyms may be created to represent subspecies-rank versions
 of infrasubspecific trinomials and subgenus-free versions of combinations
 including a subgenus name.</p>
 <p>If a matching name already exists in the COLDP instance, no new name will
 normally be added. Instead, the name record in the bundle will be updated
 with the ID (and basionymID where applicable) from the existing name. This
 allows for additional synonyms to be added to an existing taxon. The
-behaviour can be over-ridden with the <code class="xref py py-paramref docutils literal notranslate"><span class="pre">allow_repeated_binomials</span></code>
+behaviour can be over-ridden with the <a class="reference internal" href="#coldp.COLDP.__init__.params.allow_repeated_binomials" title="coldp.COLDP.__init__"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">allow_repeated_binomials</span></code></a>
 option, in which case any number of matching names can be added.</p>
-<p>If the <code class="xref py py-paramref docutils literal notranslate"><span class="pre">insert_species_for_trinomials</span></code> option is
+<p>If the <a class="reference internal" href="#coldp.COLDP.__init__.params.insert_species_for_trinomials" title="coldp.COLDP.__init__"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">insert_species_for_trinomials</span></code></a> option is
 set, a new species will be created if required before adding the
 trinomial as its child. In this case the bundle will contain the id
 for the species taxon as a species_taxon_id property.</p>
 <p>Name records in the bundle are all updated with existing or new IDs and
 basionymIDs, which are inferred automatically for zoological names by
 associating combinations with and without parentheses around the
 authorship.</p>
@@ -325,25 +339,36 @@
 </section>
 <section id="save">
 <h3>Save<a class="headerlink" href="#save" title="Link to this heading">¶</a></h3>
 <dl class="py method">
 <dt class="sig sig-object py" id="coldp.COLDP.save">
 <span class="sig-prename descclassname"><span class="pre">COLDP.</span></span><span class="sig-name descname"><span class="pre">save</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">destination</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">name</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#coldp.COLDP.save" title="Link to this definition">¶</a></dt>
 <dd><p>Write dataframes as COLDP CSV files</p>
-<p>Behaviour:
-Ensure that &lt;folder&gt;/&lt;name&gt;/ exists and write all dataframes as CSV.</p>
+<dl class="field-list simple">
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><ul class="simple">
+<li><p><span class="target" id="coldp.COLDP.save.params.destination"></span><strong>destination</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.save.params.destination">¶</a> – Path to folder in which package should be saved. Defaults to destination supplied to constructor, which defaults to “.”</p></li>
+<li><p><span class="target" id="coldp.COLDP.save.params.name"></span><strong>name</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.save.params.name">¶</a> – Name for COLDP package (subfolder name). Defaults to name supplied to constructor, which defaults to None. If no name provided, save will fail.</p></li>
+</ul>
+</dd>
+</dl>
+<p>If necessary creates subfolder with name <a class="reference internal" href="#coldp.COLDP.save.params.name" title="coldp.COLDP.save"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">name</span></code></a>
+in <a class="reference internal" href="#coldp.COLDP.save.params.destination" title="coldp.COLDP.save"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">destination</span></code></a>, and then writes CSV file
+representations for all DataFrames in the folder. Empty columns are dropped.
+Any numpy NAN elements are replaced with an empty string.</p>
 </dd></dl>
 
 </section>
 <section id="find-or-get-records">
 <h3>Find or get records<a class="headerlink" href="#find-or-get-records" title="Link to this heading">¶</a></h3>
 <dl class="py method">
 <dt class="sig sig-object py" id="coldp.COLDP.find_name_record">
 <span class="sig-prename descclassname"><span class="pre">COLDP.</span></span><span class="sig-name descname"><span class="pre">find_name_record</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">name</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#coldp.COLDP.find_name_record" title="Link to this definition">¶</a></dt>
-<dd><p>Return record from names DataFrame matching key fields in supplied record</p>
+<dd><p>Return record from names DataFrame matching key fields (scientificName,
+authorship and rank) in supplied record</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="coldp.COLDP.find_name_record.params.name"></span><strong>name</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.find_name_record.params.name">¶</a> – Dictionary containing Name properties</p>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>Dictionary containing matching record if found</p>
 </dd>
@@ -352,20 +377,63 @@
 supplied scientificName, authorship and rank and returns it as a
 COLDP Name properties dictionary, or None if no match is found.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="coldp.COLDP.find_names">
 <span class="sig-prename descclassname"><span class="pre">COLDP.</span></span><span class="sig-name descname"><span class="pre">find_names</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">properties</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">to_dict</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#coldp.COLDP.find_names" title="Link to this definition">¶</a></dt>
-<dd></dd></dl>
+<dd><p>Get all COLDP Name records matching all the supplied properties</p>
+<dl class="field-list simple">
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><ul class="simple">
+<li><p><span class="target" id="coldp.COLDP.find_names.params.properties"></span><strong>properties</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.find_names.params.properties">¶</a> – Dictionary of property values to serve as filter</p></li>
+<li><p><span class="target" id="coldp.COLDP.find_names.params.to_dict"></span><strong>to_dict</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.find_names.params.to_dict">¶</a> – True if records should be converted from Pandas format to dictionary records, False (default) otherwise.</p></li>
+</ul>
+</dd>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
+<dd class="field-even"><p>Set of COLDP Name records either as DataFrame or list of dictionaries</p>
+</dd>
+</dl>
+<p>Returns all matching records as Pandas DataFrame or list of dictionaries. If no matches, None is returned.</p>
+</dd></dl>
+
+<dl class="py method">
+<dt class="sig sig-object py" id="coldp.COLDP.find_distribution">
+<span class="sig-prename descclassname"><span class="pre">COLDP.</span></span><span class="sig-name descname"><span class="pre">find_distribution</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">distribution</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#coldp.COLDP.find_distribution" title="Link to this definition">¶</a></dt>
+<dd><p>Locate existing COLDP distribution record exactly matching all major
+fields in <a class="reference internal" href="#coldp.COLDP.find_distribution.params.distribution" title="coldp.COLDP.find_distribution"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">distribution</span></code></a></p>
+<dl class="field-list simple">
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><p><span class="target" id="coldp.COLDP.find_distribution.params.distribution"></span><strong>distribution</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.find_distribution.params.distribution">¶</a> – Dictionary of COLDP distribution properties representing a record to be found</p>
+</dd>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
+<dd class="field-even"><p>DataFrame with one COLDP distribution record if found, else None</p>
+</dd>
+</dl>
+<p>Only returns a record that exactly matches the values supplied in
+<a class="reference internal" href="#coldp.COLDP.find_distribution.params.distribution" title="coldp.COLDP.find_distribution"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">distribution</span></code></a> for all of
+taxonID, area, gazetteer, status, referenceID.</p>
+</dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="coldp.COLDP.get_name">
 <span class="sig-prename descclassname"><span class="pre">COLDP.</span></span><span class="sig-name descname"><span class="pre">get_name</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">id</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#coldp.COLDP.get_name" title="Link to this definition">¶</a></dt>
-<dd></dd></dl>
+<dd><p>Return record from names DataFrame with supplied ID</p>
+<dl class="field-list simple">
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><p><span class="target" id="coldp.COLDP.get_name.params.id"></span><strong>id</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.get_name.params.id">¶</a> – String ID for COLDP Name record</p>
+</dd>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
+<dd class="field-even"><p>Pandas DataFrame containing matching record if found</p>
+</dd>
+</dl>
+<p>Locates any existing record in the names DataFrame with the supplied
+ID, or None if no match is found. If multiple matches are found, logs
+an issue and returns the first.</p>
+</dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="coldp.COLDP.get_reference">
 <span class="sig-prename descclassname"><span class="pre">COLDP.</span></span><span class="sig-name descname"><span class="pre">get_reference</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">id</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#coldp.COLDP.get_reference" title="Link to this definition">¶</a></dt>
 <dd><p>Get reference record as dictionary from ID string</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
@@ -378,30 +446,81 @@
 <p>Returns None if no matching reference. If multiple records exist with
 the given id, a warning is logged and the first match is returned.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="coldp.COLDP.get_taxon">
 <span class="sig-prename descclassname"><span class="pre">COLDP.</span></span><span class="sig-name descname"><span class="pre">get_taxon</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">id</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#coldp.COLDP.get_taxon" title="Link to this definition">¶</a></dt>
-<dd></dd></dl>
+<dd><p>Return a COLDP Taxon record matching the supplied ID</p>
+<dl class="field-list simple">
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><p><span class="target" id="coldp.COLDP.get_taxon.params.id"></span><strong>id</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.get_taxon.params.id">¶</a> – String ID value</p>
+</dd>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
+<dd class="field-even"><p>Dictionary representation of COLDP Taxon record</p>
+</dd>
+</dl>
+<p>Logs a warning if more than one match and returns the first such match.</p>
+</dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="coldp.COLDP.get_synonyms">
 <span class="sig-prename descclassname"><span class="pre">COLDP.</span></span><span class="sig-name descname"><span class="pre">get_synonyms</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">taxonID</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">to_dict</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#coldp.COLDP.get_synonyms" title="Link to this definition">¶</a></dt>
-<dd></dd></dl>
+<dd><p>Get all COLDP Synonym records for the supplied taxon ID</p>
+<dl class="field-list simple">
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><ul class="simple">
+<li><p><span class="target" id="coldp.COLDP.get_synonyms.params.taxonID"></span><strong>taxonID</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.get_synonyms.params.taxonID">¶</a> – String taxonID value</p></li>
+<li><p><span class="target" id="coldp.COLDP.get_synonyms.params.to_dict"></span><strong>to_dict</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.get_synonyms.params.to_dict">¶</a> – True if records should be converted from Pandas format to dictionary records, False (default) otherwise.</p></li>
+</ul>
+</dd>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
+<dd class="field-even"><p>Set of COLDP Synonym records for taxon either as DataFrame or list of dictionaries</p>
+</dd>
+</dl>
+<p>Returns all matching records as Pandas DataFrame or list of dictionaries. If no matches, None is returned.</p>
+</dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="coldp.COLDP.get_synonymy">
 <span class="sig-prename descclassname"><span class="pre">COLDP.</span></span><span class="sig-name descname"><span class="pre">get_synonymy</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">nameID</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">to_dict</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#coldp.COLDP.get_synonymy" title="Link to this definition">¶</a></dt>
-<dd></dd></dl>
+<dd><p>Get accepted COLDP Name record and all synonym COLDP Name records for the supplied name ID</p>
+<dl class="field-list simple">
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><ul class="simple">
+<li><p><span class="target" id="coldp.COLDP.get_synonymy.params.taxonID"></span><strong>taxonID</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.get_synonymy.params.taxonID">¶</a> – String nameID value</p></li>
+<li><p><span class="target" id="coldp.COLDP.get_synonymy.params.to_dict"></span><strong>to_dict</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.get_synonymy.params.to_dict">¶</a> – True if records should be converted from Pandas format to dictionary records, False (default) otherwise</p></li>
+</ul>
+</dd>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
+<dd class="field-even"><p>Tuple containing COLDP Name record for accepted name and a DataFrame or list of dictionaries representing all synonym Name records</p>
+</dd>
+</dl>
+<p>Maps the name indicated by the provided nameID to the accepted taxon and
+returns its name and the names for all synonyms for the taxon. These may
+all be returned either as Pandas DataFrames or in dictionary representations.</p>
+</dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="coldp.COLDP.get_children">
 <span class="sig-prename descclassname"><span class="pre">COLDP.</span></span><span class="sig-name descname"><span class="pre">get_children</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">taxonID</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">to_dict</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#coldp.COLDP.get_children" title="Link to this definition">¶</a></dt>
-<dd></dd></dl>
+<dd><p>Get all child taxa for the COLDP Taxon associated with the supplied taxonID</p>
+<dl class="field-list simple">
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><ul class="simple">
+<li><p><span class="target" id="coldp.COLDP.get_children.params.taxonID"></span><strong>taxonID</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.get_children.params.taxonID">¶</a> – String ID for COLDP Taxon record</p></li>
+<li><p><span class="target" id="coldp.COLDP.get_children.params.to_dict"></span><strong>to_dict</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.get_children.params.to_dict">¶</a> – True if records should be converted from Pandas format to dictionary records, False (default) otherwise.</p></li>
+</ul>
+</dd>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
+<dd class="field-even"><p>Set of COLDP Taxon records for children of identified taxon either as DataFrame or list of dictionaries</p>
+</dd>
+</dl>
+<p>Returns all matching records as Pandas DataFrame or list of dictionaries. If no matches, None is returned.</p>
+</dd></dl>
 
 </section>
 <section id="tidy-package">
 <h3>Tidy package<a class="headerlink" href="#tidy-package" title="Link to this heading">¶</a></h3>
 <dl class="py method">
 <dt class="sig sig-object py" id="coldp.COLDP.fix_basionyms">
 <span class="sig-prename descclassname"><span class="pre">COLDP.</span></span><span class="sig-name descname"><span class="pre">fix_basionyms</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">names</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">synonyms</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#coldp.COLDP.fix_basionyms" title="Link to this definition">¶</a></dt>
@@ -615,16 +734,32 @@
 </dl>
 <p>This method is used to extract and rename a subset of columns from a
 COLDP NameUsage table.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="coldp.COLDP.insert_taxon">
-<span class="sig-prename descclassname"><span class="pre">COLDP.</span></span><span class="sig-name descname"><span class="pre">insert_taxon</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">name</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">parent</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">incertae_sedis</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#coldp.COLDP.insert_taxon" title="Link to this definition">¶</a></dt>
-<dd></dd></dl>
+<span class="sig-prename descclassname"><span class="pre">COLDP.</span></span><span class="sig-name descname"><span class="pre">insert_taxon</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">name</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">parentID</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">incertae_sedis</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#coldp.COLDP.insert_taxon" title="Link to this definition">¶</a></dt>
+<dd><p>Insert COLDP Taxon record as child of identified parent - creates or moves record as necessary</p>
+<dl class="field-list simple">
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><ul class="simple">
+<li><p><span class="target" id="coldp.COLDP.insert_taxon.params.name"></span><strong>name</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.insert_taxon.params.name">¶</a> – COLDP Name record to be used as accepted name for new taxon</p></li>
+<li><p><span class="target" id="coldp.COLDP.insert_taxon.params.parentID"></span><strong>parentID</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.insert_taxon.params.parentID">¶</a> – String identifier for parent taxon</p></li>
+</ul>
+</dd>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
+<dd class="field-even"><p>Dictionary containing taxon record</p>
+</dd>
+</dl>
+<p>If a taxon record already exists for the name, any parenthood change is
+made as required and the record is returned as a dictionary. Otherwise
+a new record is created and returned. Default values are taken from the
+<a class="reference internal" href="#coldp.COLDP.__init__.params.default_taxon_record" title="coldp.COLDP.__init__"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">default_taxon_record</span></code></a> dictionary.</p>
+</dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="coldp.COLDP.insert_synonym">
 <span class="sig-prename descclassname"><span class="pre">COLDP.</span></span><span class="sig-name descname"><span class="pre">insert_synonym</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">taxon_id</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">name_id</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#coldp.COLDP.insert_synonym" title="Link to this definition">¶</a></dt>
 <dd><p>Add basic COLDP Synonym record to COLDP instance</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
@@ -708,17 +843,17 @@
 <span class="sig-prename descclassname"><span class="pre">COLDP.</span></span><span class="sig-name descname"><span class="pre">prepare_bundle</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">bundle</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#coldp.COLDP.prepare_bundle" title="Link to this definition">¶</a></dt>
 <dd><p>Add extra names to <code class="xref py py-class docutils literal notranslate"><span class="pre">NameBundle</span></code> if required based on current options</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="coldp.COLDP.prepare_bundle.params.bundle"></span><strong>bundle</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.prepare_bundle.params.bundle">¶</a> – NameBundle to be processed</p>
 </dd>
 </dl>
-<p>If <code class="xref py py-paramref docutils literal notranslate"><span class="pre">insert_species_for_trinomials</span></code> is True, ensure that the implied binomial exists for any new trinomials.</p>
-<p>If <code class="xref py py-paramref docutils literal notranslate"><span class="pre">create_subspecies_for_infrasubspecifics</span></code> is True, add a subspecies-rank synonym to the bundle for each infrasubspecific name.</p>
-<p>If <code class="xref py py-paramref docutils literal notranslate"><span class="pre">create_synonyms_without_subgenus</span></code> is True, add a subgenus-free synonym to the bundle for each name containing a subgenus.</p>
+<p>If <a class="reference internal" href="#coldp.COLDP.__init__.params.insert_species_for_trinomials" title="coldp.COLDP.__init__"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">insert_species_for_trinomials</span></code></a> is True, ensure that the implied binomial exists for any new trinomials.</p>
+<p>If <a class="reference internal" href="#coldp.COLDP.__init__.params.create_subspecies_for_infrasubspecifics" title="coldp.COLDP.__init__"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">create_subspecies_for_infrasubspecifics</span></code></a> is True, add a subspecies-rank synonym to the bundle for each infrasubspecific name.</p>
+<p>If <a class="reference internal" href="#coldp.COLDP.__init__.params.create_synonyms_without_subgenus" title="coldp.COLDP.__init__"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">create_synonyms_without_subgenus</span></code></a> is True, add a subgenus-free synonym to the bundle for each name containing a subgenus.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="coldp.COLDP.validate_record">
 <span class="sig-prename descclassname"><span class="pre">COLDP.</span></span><span class="sig-name descname"><span class="pre">validate_record</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">record_type</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">record</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#coldp.COLDP.validate_record" title="Link to this definition">¶</a></dt>
 <dd><p>Verify whether all ID values used as forign keys in <a class="reference internal" href="#coldp.COLDP.validate_record.params.record" title="coldp.COLDP.validate_record"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">record</span></code></a> correspond with existing records in the relevant tables</p>
 <dl class="field-list simple">
@@ -742,14 +877,21 @@
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="coldp.COLDP.identify_name.params.name"></span><strong>name</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.identify_name.params.name">¶</a> – Dictionary containing COLDP Name properties</p>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>Currently stored version of the name record in question</p>
 </dd>
 </dl>
+<p>If a COLDP Name record for this name already exists
+(based on <a class="reference internal" href="#coldp.COLDP.find_name_record" title="coldp.COLDP.find_name_record"><code class="xref py py-func docutils literal notranslate"><span class="pre">find_name_record()</span></code></a>), return the existing
+name, unless this is a species name and the
+<a class="reference internal" href="#coldp.COLDP.__init__.params.allow_repeated_binomials" title="coldp.COLDP.__init__"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">allow_repeated_binomials</span></code></a> option has been set,
+in which case a new record will be created.</p>
+<p>If the name is missing, create a new record with the next unused ID
+value and return the record with the ID.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="coldp.COLDP.same_basionym">
 <span class="sig-prename descclassname"><span class="pre">COLDP.</span></span><span class="sig-name descname"><span class="pre">same_basionym</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">a</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">b</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#coldp.COLDP.same_basionym" title="Link to this definition">¶</a></dt>
 <dd><p>Validates whether two name records share the same basionym (i.e. are different combinations for the same original name)
 :param _sphinx_paramlinks_coldp.COLDP.same_basionym.a: Dictionary with parameters representing a COLDP Name record
@@ -786,15 +928,29 @@
 </dl>
 <p>Relevant only for zoological names</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="coldp.COLDP.epithet_and_authorship_match">
 <span class="sig-prename descclassname"><span class="pre">COLDP.</span></span><span class="sig-name descname"><span class="pre">epithet_and_authorship_match</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">name</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">epithet</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">authorship</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#coldp.COLDP.epithet_and_authorship_match" title="Link to this definition">¶</a></dt>
-<dd></dd></dl>
+<dd><p>Check whether a name record matches the supplied epithet and authorship</p>
+<dl class="field-list simple">
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><ul class="simple">
+<li><p><span class="target" id="coldp.COLDP.epithet_and_authorship_match.params.name"></span><strong>name</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.epithet_and_authorship_match.params.name">¶</a> – Dictionary containing COLDP Name record</p></li>
+<li><p><span class="target" id="coldp.COLDP.epithet_and_authorship_match.params.epithet"></span><strong>epithet</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.epithet_and_authorship_match.params.epithet">¶</a> – Specific or infraspecific epithet</p></li>
+<li><p><span class="target" id="coldp.COLDP.epithet_and_authorship_match.params.authorship"></span><strong>authorship</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.epithet_and_authorship_match.params.authorship">¶</a> – Authorship string</p></li>
+</ul>
+</dd>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
+<dd class="field-even"><p>True if the <a class="reference internal" href="#coldp.COLDP.epithet_and_authorship_match.params.epithet" title="coldp.COLDP.epithet_and_authorship_match"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">epithet</span></code></a> matches the lowest-ranked epithet and <a class="reference internal" href="#coldp.COLDP.epithet_and_authorship_match.params.authorship" title="coldp.COLDP.epithet_and_authorship_match"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">authorship</span></code></a> matches the authorship in the name record</p>
+</dd>
+</dl>
+<p>Comparison ignores epithet gender endings.</p>
+</dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="coldp.COLDP.set_basionymid">
 <span class="sig-prename descclassname"><span class="pre">COLDP.</span></span><span class="sig-name descname"><span class="pre">set_basionymid</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">name</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">basionymid</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#coldp.COLDP.set_basionymid" title="Link to this definition">¶</a></dt>
 <dd><p>Set basionymID on Name record in names DataFrame</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
@@ -805,25 +961,71 @@
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="coldp.COLDP.fix_basionymid">
 <span class="sig-prename descclassname"><span class="pre">COLDP.</span></span><span class="sig-name descname"><span class="pre">fix_basionymid</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">name</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">synonyms</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#coldp.COLDP.fix_basionymid" title="Link to this definition">¶</a></dt>
-<dd></dd></dl>
+<dd><p>Update name so its basionymID references the original combination in a list of synonyms</p>
+<dl class="field-list simple">
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><ul class="simple">
+<li><p><span class="target" id="coldp.COLDP.fix_basionymid.params.name"></span><strong>name</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.fix_basionymid.params.name">¶</a> – Dictionary containing COLDP Name record for which basionymID is to be fixed</p></li>
+<li><p><span class="target" id="coldp.COLDP.fix_basionymid.params.synonyms"></span><strong>synonyms</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.fix_basionymid.params.synonyms">¶</a> – List of COLDP Name records that may contain basionym</p></li>
+</ul>
+</dd>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
+<dd class="field-even"><p></p>
+</dd>
+</dl>
+<p>Returns name following any updates.</p>
+</dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="coldp.COLDP.find_name">
 <span class="sig-prename descclassname"><span class="pre">COLDP.</span></span><span class="sig-name descname"><span class="pre">find_name</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">scientificName</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">authorship</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">rank</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#coldp.COLDP.find_name" title="Link to this definition">¶</a></dt>
-<dd></dd></dl>
+<dd><p>Return record from names DataFrame matching supplied scientificName,
+authorship and rank</p>
+<dl class="field-list simple">
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><ul class="simple">
+<li><p><span class="target" id="coldp.COLDP.find_name.params.scientificName"></span><strong>scientificName</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.find_name.params.scientificName">¶</a> – Scientific name in canonical format</p></li>
+<li><p><span class="target" id="coldp.COLDP.find_name.params.authorship"></span><strong>authorship</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.find_name.params.authorship">¶</a> – Authorship string</p></li>
+<li><p><span class="target" id="coldp.COLDP.find_name.params.rank"></span><strong>rank</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.find_name.params.rank">¶</a> – Rank name string</p></li>
+</ul>
+</dd>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
+<dd class="field-even"><p>Dictionary containing matching record if found</p>
+</dd>
+</dl>
+<p>Locates any existing record in the names DataFrame that matches the
+supplied scientificName, authorship and rank and returns it as a
+COLDP Name properties dictionary, or None if no match is found.</p>
+<p>If <a class="reference internal" href="#coldp.COLDP.find_name.params.authorship" title="coldp.COLDP.find_name"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">authorship</span></code></a> is None, returns a
+name based only on scientificName and rank.</p>
+</dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="coldp.COLDP.find_taxon">
 <span class="sig-prename descclassname"><span class="pre">COLDP.</span></span><span class="sig-name descname"><span class="pre">find_taxon</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">scientificName</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">authorship</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">rank</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#coldp.COLDP.find_taxon" title="Link to this definition">¶</a></dt>
-<dd></dd></dl>
+<dd><p>Get COLDP Taxon record (as Pandas dataframe) with accepted name matching supplied scientificName, authorship and rank values</p>
+<dl class="field-list simple">
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><ul class="simple">
+<li><p><span class="target" id="coldp.COLDP.find_taxon.params.scientificName"></span><strong>scientificName</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.find_taxon.params.scientificName">¶</a> – Scientific name in canonical format</p></li>
+<li><p><span class="target" id="coldp.COLDP.find_taxon.params.authorship"></span><strong>authorship</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.find_taxon.params.authorship">¶</a> – Authorship string</p></li>
+<li><p><span class="target" id="coldp.COLDP.find_taxon.params.rank"></span><strong>rank</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.find_taxon.params.rank">¶</a> – Rank name string</p></li>
+</ul>
+</dd>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
+<dd class="field-even"><p>COLDP Taxon record matching supplied parameters</p>
+</dd>
+</dl>
+<p>Logs a warning issue if multiple taxon records exist for a matching name and returns the first such match. Returns None if no match.</p>
+</dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="coldp.COLDP.construct_species_rank_name">
 <span class="sig-prename descclassname"><span class="pre">COLDP.</span></span><span class="sig-name descname"><span class="pre">construct_species_rank_name</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">g</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sg</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">s</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ss</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">marker</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#coldp.COLDP.construct_species_rank_name" title="Link to this definition">¶</a></dt>
 <dd><p>Consistently construct a species or infraspecific name from the included epithets and optional rank marker</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
@@ -899,15 +1101,27 @@
 </dl>
 <p>Simply checks if the supplied rank is one of those below the subspecies.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="coldp.COLDP.issue">
 <span class="sig-prename descclassname"><span class="pre">COLDP.</span></span><span class="sig-name descname"><span class="pre">issue</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">message</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#coldp.COLDP.issue" title="Link to this definition">¶</a></dt>
-<dd></dd></dl>
+<dd><p>Log issue with data provided through methods</p>
+<dl class="field-list simple">
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><p><span class="target" id="coldp.COLDP.issue.params.message"></span><strong>message</strong><a class="paramlink headerlink reference internal" href="#coldp.COLDP.issue.params.message">¶</a> – Text to be saved as body of issue</p>
+</dd>
+</dl>
+<p>Creates a new record in an issues DataFrame that will be included in the
+COLDP export when <a class="reference internal" href="#coldp.COLDP.save" title="coldp.COLDP.save"><code class="xref py py-func docutils literal notranslate"><span class="pre">save()</span></code></a> is called. This record includes
+the message and the context string supplied on the most recent call to
+<a class="reference internal" href="#coldp.COLDP.set_context" title="coldp.COLDP.set_context"><code class="xref py py-func docutils literal notranslate"><span class="pre">set_context()</span></code></a>.</p>
+<p>If <a class="reference internal" href="#coldp.COLDP.__init__.params.issues_to_stdout" title="coldp.COLDP.__init__"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">issues_to_stdout</span></code></a> is True, the context and message
+are also output as an error via logging.</p>
+</dd></dl>
 
 </section>
 <section id="index-and-search">
 <h2>Index and search<a class="headerlink" href="#index-and-search" title="Link to this heading">¶</a></h2>
 <ul class="simple">
 <li><p><a class="reference internal" href="genindex.html"><span class="std std-ref">Index</span></a></p></li>
 <li><p><a class="reference internal" href="search.html"><span class="std std-ref">Search Page</span></a></p></li>
@@ -928,32 +1142,34 @@
 
 
 
 
 
 
 <h3>Navigation</h3>
-<p class="caption" role="heading"><span class="caption-text">Contents:</span></p>
 <ul class="current">
 <li class="toctree-l1 current"><a class="current reference internal" href="#">coldp.COLDP</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="#class">Class</a></li>
 <li class="toctree-l2"><a class="reference internal" href="#methods">Methods</a></li>
 <li class="toctree-l2"><a class="reference internal" href="#constants">Constants</a></li>
 <li class="toctree-l2"><a class="reference internal" href="#internal-methods">Internal methods</a></li>
 <li class="toctree-l2"><a class="reference internal" href="#index-and-search">Index and search</a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="name-bundle.html">coldp.NameBundle</a></li>
 </ul>
+<ul>
+<li class="toctree-l1"><a class="reference internal" href="usage.html">Usage</a></li>
+</ul>
 
 <div class="relations">
 <h3>Related Topics</h3>
 <ul>
   <li><a href="index.html">Documentation overview</a><ul>
-      <li>Previous: <a href="index.html" title="previous chapter">COLDP</a></li>
+      <li>Previous: <a href="index.html" title="previous chapter">coldp</a></li>
       <li>Next: <a href="name-bundle.html" title="next chapter">coldp.NameBundle</a></li>
   </ul></li>
 </ul>
 </div>
 <search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 ************ ccoollddpp..CCOOLLDDPP_?¶ ************
 ********** CCllaassss_?¶ **********
-  ccllaassss coldp.COLDP(nnaammee, ffoollddeerr==''..'', ccooddee==''IICCZZNN'', ddeeffaauulltt__ttaaxxoonn__rreeccoorrdd==NNoonnee,
+  COLDP.__init__(nnaammee, ffoollddeerr==''..'', ccooddee==''IICCZZNN'', ddeeffaauulltt__ttaaxxoonn__rreeccoorrdd==NNoonnee,
   iinnsseerrtt__ssppeecciieess__ffoorr__ttrriinnoommiiaallss==FFaallssee,
   ccrreeaattee__ssuubbssppeecciieess__ffoorr__iinnffrraassuubbssppeecciiffiiccss==FFaallssee,
   ccrreeaattee__ssyynnoonnyymmss__wwiitthhoouutt__ssuubbggeennuuss==FFaallssee, bbaassiioonnyymmss__ffrroomm__ssyynnoonnyymmss==FFaallssee,
   ccllaassssiiffiiccaattiioonn__ffrroomm__ppaarreennttss==FFaallssee, aallllooww__rreeppeeaatteedd__bbiinnoommiiaallss==FFaallssee,
-  ccrreeaattee__ttaaxxaa__ffoorr__nnoott__eessttaabblliisshheedd==FFaallssee, iissssuueess__ttoo__ssttddoouutt==FFaallssee, ccoonntteexxtt==NNoonnee)
+  ccrreeaattee__ttaaxxaa__ffoorr__nnoott__eessttaabblliisshheedd==FFaallssee, iissssuueess__ttoo__ssttddoouutt==FFaallssee, ccoonntteexxtt==NNoonnee)_¶
       Class to manage a set of Pandas dataframes for CSV tables in Catalogue of
       Life Data Package.
         Parameters:
                 * nnaammee_¶ – The name for the COLDP package. If a folder of this
                   name exists inside the folder specied by the folder
                   parameter, this COLDP instance will be initialised with the
                   contents of any COLDP-compliant CSV or TSV files in the named
@@ -128,14 +128,26 @@
       to the instance. The context variable provides an external mechanism for
       the user to label these issues as they occur. For example, if the user is
       processing a spreadsheet of species names, they can call set_context with
       a string identifying the row from the source spreadsheet. This value will
       be included in the context column in the issue.csv output.
 ******** AAdddd oorr mmooddiiffyy rreeccoorrddss_?¶ ********
   COLDP.start_name_bundle(aacccceepptteedd, iinncceerrttaaee__sseeddiiss==FFaallssee, ssiicc==FFaallssee)_¶
+      Return a NameBundle object based on the supplied accepted name and
+      referencing this COLDP instance
+        Parameters:
+                * aacccceepptteedd_¶ – Dictionary containing COLDP Name record for
+                  accepted name
+                * iinncceerrttaaee__sseeddiiss_¶ – If True, the associated COLDP Taxon Record
+                  will be flagged as iinncceerrttaaee sseeddiiss
+                * ssiicc_¶ – If True, issues will not be reported if the name is
+                  not properly code-compliant
+        Returns:
+            NameBundle instance initialised with supplied parameters
+      This is the normal way to construct a new NameBundle object.
   COLDP.add_names(bbuunnddllee, ppaarreenntt==NNoonnee)_¶
       Ensure one or more names are included in names dataframe and update taxa
       and synonyms dataframes as necessary
         Parameters:
                 * bbuunnddllee_¶ – NameBundle object with set of associated taxon
                   names
                 * ppaarreenntt_¶ – ID for taxon record for which the accepted taxon in
@@ -150,17 +162,17 @@
       synonyms may be created to represent subspecies-rank versions of
       infrasubspecific trinomials and subgenus-free versions of combinations
       including a subgenus name.
       If a matching name already exists in the COLDP instance, no new name will
       normally be added. Instead, the name record in the bundle will be updated
       with the ID (and basionymID where applicable) from the existing name.
       This allows for additional synonyms to be added to an existing taxon. The
-      behaviour can be over-ridden with the allow_repeated_binomials option, in
+      behaviour can be over-ridden with the _a_l_l_o_w___r_e_p_e_a_t_e_d___b_i_n_o_m_i_a_l_s option, in
       which case any number of matching names can be added.
-      If the insert_species_for_trinomials option is set, a new species will be
+      If the _i_n_s_e_r_t___s_p_e_c_i_e_s___f_o_r___t_r_i_n_o_m_i_a_l_s option is set, a new species will be
       created if required before adding the trinomial as its child. In this
       case the bundle will contain the id for the species taxon as a
       species_taxon_id property.
       Name records in the bundle are all updated with existing or new IDs and
       basionymIDs, which are inferred automatically for zoological names by
       associating combinations with and without parentheses around the
       authorship.
@@ -249,40 +261,120 @@
                 * pprrooppeerrttiieess_¶ – Dictionary of COLDP Taxon properties to be set
                   for the identified record
       If a taxon record exists with the given ID, set all properties in the
       dictionary.
 ******** SSaavvee_?¶ ********
   COLDP.save(ddeessttiinnaattiioonn==NNoonnee, nnaammee==NNoonnee)_¶
       Write dataframes as COLDP CSV files
-      Behaviour: Ensure that <folder>/<name>/ exists and write all dataframes
-      as CSV.
+        Parameters:
+                * ddeessttiinnaattiioonn_¶ – Path to folder in which package should be
+                  saved. Defaults to destination supplied to constructor, which
+                  defaults to “.”
+                * nnaammee_¶ – Name for COLDP package (subfolder name). Defaults to
+                  name supplied to constructor, which defaults to None. If no
+                  name provided, save will fail.
+      If necessary creates subfolder with name _n_a_m_e in _d_e_s_t_i_n_a_t_i_o_n, and then
+      writes CSV file representations for all DataFrames in the folder. Empty
+      columns are dropped. Any numpy NAN elements are replaced with an empty
+      string.
 ******** FFiinndd oorr ggeett rreeccoorrddss_?¶ ********
   COLDP.find_name_record(nnaammee)_¶
-      Return record from names DataFrame matching key fields in supplied record
+      Return record from names DataFrame matching key fields (scientificName,
+      authorship and rank) in supplied record
         Parameters:
             nnaammee_¶ – Dictionary containing Name properties
         Returns:
             Dictionary containing matching record if found
       Locates any existing record in the names DataFrame that matches the
       supplied scientificName, authorship and rank and returns it as a COLDP
       Name properties dictionary, or None if no match is found.
   COLDP.find_names(pprrooppeerrttiieess, ttoo__ddiicctt==FFaallssee)_¶
+      Get all COLDP Name records matching all the supplied properties
+        Parameters:
+                * pprrooppeerrttiieess_¶ – Dictionary of property values to serve as
+                  filter
+                * ttoo__ddiicctt_¶ – True if records should be converted from Pandas
+                  format to dictionary records, False (default) otherwise.
+        Returns:
+            Set of COLDP Name records either as DataFrame or list of
+            dictionaries
+      Returns all matching records as Pandas DataFrame or list of dictionaries.
+      If no matches, None is returned.
+  COLDP.find_distribution(ddiissttrriibbuuttiioonn)_¶
+      Locate existing COLDP distribution record exactly matching all major
+      fields in _d_i_s_t_r_i_b_u_t_i_o_n
+        Parameters:
+            ddiissttrriibbuuttiioonn_¶ – Dictionary of COLDP distribution properties
+            representing a record to be found
+        Returns:
+            DataFrame with one COLDP distribution record if found, else None
+      Only returns a record that exactly matches the values supplied in
+      _d_i_s_t_r_i_b_u_t_i_o_n for all of taxonID, area, gazetteer, status, referenceID.
   COLDP.get_name(iidd)_¶
+      Return record from names DataFrame with supplied ID
+        Parameters:
+            iidd_¶ – String ID for COLDP Name record
+        Returns:
+            Pandas DataFrame containing matching record if found
+      Locates any existing record in the names DataFrame with the supplied ID,
+      or None if no match is found. If multiple matches are found, logs an
+      issue and returns the first.
   COLDP.get_reference(iidd)_¶
       Get reference record as dictionary from ID string
         Parameters:
             iidd_¶ – ID string for requested COLDP reference record
         Returns:
             Dictionary of COLDP reference properties for requested ID
       Returns None if no matching reference. If multiple records exist with the
       given id, a warning is logged and the first match is returned.
   COLDP.get_taxon(iidd)_¶
+      Return a COLDP Taxon record matching the supplied ID
+        Parameters:
+            iidd_¶ – String ID value
+        Returns:
+            Dictionary representation of COLDP Taxon record
+      Logs a warning if more than one match and returns the first such match.
   COLDP.get_synonyms(ttaaxxoonnIIDD, ttoo__ddiicctt==FFaallssee)_¶
+      Get all COLDP Synonym records for the supplied taxon ID
+        Parameters:
+                * ttaaxxoonnIIDD_¶ – String taxonID value
+                * ttoo__ddiicctt_¶ – True if records should be converted from Pandas
+                  format to dictionary records, False (default) otherwise.
+        Returns:
+            Set of COLDP Synonym records for taxon either as DataFrame or list
+            of dictionaries
+      Returns all matching records as Pandas DataFrame or list of dictionaries.
+      If no matches, None is returned.
   COLDP.get_synonymy(nnaammeeIIDD, ttoo__ddiicctt==FFaallssee)_¶
+      Get accepted COLDP Name record and all synonym COLDP Name records for the
+      supplied name ID
+        Parameters:
+                * ttaaxxoonnIIDD_¶ – String nameID value
+                * ttoo__ddiicctt_¶ – True if records should be converted from Pandas
+                  format to dictionary records, False (default) otherwise
+        Returns:
+            Tuple containing COLDP Name record for accepted name and a
+            DataFrame or list of dictionaries representing all synonym Name
+            records
+      Maps the name indicated by the provided nameID to the accepted taxon and
+      returns its name and the names for all synonyms for the taxon. These may
+      all be returned either as Pandas DataFrames or in dictionary
+      representations.
   COLDP.get_children(ttaaxxoonnIIDD, ttoo__ddiicctt==FFaallssee)_¶
+      Get all child taxa for the COLDP Taxon associated with the supplied
+      taxonID
+        Parameters:
+                * ttaaxxoonnIIDD_¶ – String ID for COLDP Taxon record
+                * ttoo__ddiicctt_¶ – True if records should be converted from Pandas
+                  format to dictionary records, False (default) otherwise.
+        Returns:
+            Set of COLDP Taxon records for children of identified taxon either
+            as DataFrame or list of dictionaries
+      Returns all matching records as Pandas DataFrame or list of dictionaries.
+      If no matches, None is returned.
 ******** TTiiddyy ppaacckkaaggee_?¶ ********
   COLDP.fix_basionyms(nnaammeess, ssyynnoonnyymmss)_¶
       Update dataframe of name records so that subsequent combination names
       refer to the original basionym record where present
         Parameters:
                 * nnaammeess_¶ – Dataframe containing COLDP name records to be
                   updated
@@ -413,15 +505,27 @@
                 * hheeaaddiinnggss_¶ – List of column headings for destination dataframe
                 * mmaappppiinnggss_¶ – Dictionary mapping destination column names to
                   source column names
         Returns:
             New Dataframe based on supplied mappings
       This method is used to extract and rename a subset of columns from a
       COLDP NameUsage table.
-  COLDP.insert_taxon(nnaammee, ppaarreenntt, iinncceerrttaaee__sseeddiiss==FFaallssee)_¶
+  COLDP.insert_taxon(nnaammee, ppaarreennttIIDD, iinncceerrttaaee__sseeddiiss==FFaallssee)_¶
+      Insert COLDP Taxon record as child of identified parent - creates or
+      moves record as necessary
+        Parameters:
+                * nnaammee_¶ – COLDP Name record to be used as accepted name for new
+                  taxon
+                * ppaarreennttIIDD_¶ – String identifier for parent taxon
+        Returns:
+            Dictionary containing taxon record
+      If a taxon record already exists for the name, any parenthood change is
+      made as required and the record is returned as a dictionary. Otherwise a
+      new record is created and returned. Default values are taken from the
+      _d_e_f_a_u_l_t___t_a_x_o_n___r_e_c_o_r_d dictionary.
   COLDP.insert_synonym(ttaaxxoonn__iidd, nnaammee__iidd)_¶
       Add basic COLDP Synonym record to COLDP instance
         Parameters:
                 * ttaaxxoonn__iidd_¶ – String ID for taxon for which synonym is being
                   registered
                 * nnaammee__iidd_¶ – String ID for name which is being registered as a
                   synonym
@@ -471,19 +575,19 @@
       Appends next taxon ID to the list along with a value guaranteed to be
       higher than the one added on the previous execution of this method.
       Recursively add IDs for children.
   COLDP.prepare_bundle(bbuunnddllee)_¶
       Add extra names to NameBundle if required based on current options
         Parameters:
             bbuunnddllee_¶ – NameBundle to be processed
-      If insert_species_for_trinomials is True, ensure that the implied
+      If _i_n_s_e_r_t___s_p_e_c_i_e_s___f_o_r___t_r_i_n_o_m_i_a_l_s is True, ensure that the implied
       binomial exists for any new trinomials.
-      If create_subspecies_for_infrasubspecifics is True, add a subspecies-rank
+      If _c_r_e_a_t_e___s_u_b_s_p_e_c_i_e_s___f_o_r___i_n_f_r_a_s_u_b_s_p_e_c_i_f_i_c_s is True, add a subspecies-rank
       synonym to the bundle for each infrasubspecific name.
-      If create_synonyms_without_subgenus is True, add a subgenus-free synonym
+      If _c_r_e_a_t_e___s_y_n_o_n_y_m_s___w_i_t_h_o_u_t___s_u_b_g_e_n_u_s is True, add a subgenus-free synonym
       to the bundle for each name containing a subgenus.
   COLDP.validate_record(rreeccoorrdd__ttyyppee, rreeccoorrdd)_¶
       Verify whether all ID values used as forign keys in _r_e_c_o_r_d correspond
       with existing records in the relevant tables
         Parameters:
                 * rreeccoorrdd__ttyyppee_¶ – Name for the data class to which this record
                   should below
@@ -494,14 +598,20 @@
   COLDP.identify_name(nnaammee)_¶
       Ensure COLDP Name record is present and return a copy containing the
       current ID and basionymID
         Parameters:
             nnaammee_¶ – Dictionary containing COLDP Name properties
         Returns:
             Currently stored version of the name record in question
+      If a COLDP Name record for this name already exists (based on
+      _f_i_n_d___n_a_m_e___r_e_c_o_r_d_(_)), return the existing name, unless this is a species
+      name and the _a_l_l_o_w___r_e_p_e_a_t_e_d___b_i_n_o_m_i_a_l_s option has been set, in which case
+      a new record will be created.
+      If the name is missing, create a new record with the next unused ID value
+      and return the record with the ID.
   COLDP.same_basionym(aa, bb)_¶
       Validates whether two name records share the same basionym (i.e. are
       different combinations for the same original name) :param
       _sphinx_paramlinks_coldp.COLDP.same_basionym.a: Dictionary with
       parameters representing a COLDP Name record :param
       _sphinx_paramlinks_coldp.COLDP.same_basionym.b: Dictionary with
       parameters representing a COLDP Name record :return: True if the
@@ -518,22 +628,63 @@
       Return authorship string without enclosing parentheses
         Parameters:
             aauutthhoorrsshhiipp_¶ – Authorship string
         Returns:
             Authorship stripped of enclosing parentheses
       Relevant only for zoological names
   COLDP.epithet_and_authorship_match(nnaammee, eeppiitthheett, aauutthhoorrsshhiipp)_¶
+      Check whether a name record matches the supplied epithet and authorship
+        Parameters:
+                * nnaammee_¶ – Dictionary containing COLDP Name record
+                * eeppiitthheett_¶ – Specific or infraspecific epithet
+                * aauutthhoorrsshhiipp_¶ – Authorship string
+        Returns:
+            True if the _e_p_i_t_h_e_t matches the lowest-ranked epithet and
+            _a_u_t_h_o_r_s_h_i_p matches the authorship in the name record
+      Comparison ignores epithet gender endings.
   COLDP.set_basionymid(nnaammee, bbaassiioonnyymmiidd)_¶
       Set basionymID on Name record in names DataFrame
         Parameters:
                 * nnaammee_¶ – Name record as dictionary of COLDP properties
                 * bbaassiioonnyymmiidd_¶ – String ID of associated basionyn record
   COLDP.fix_basionymid(nnaammee, ssyynnoonnyymmss)_¶
+      Update name so its basionymID references the original combination in a
+      list of synonyms
+        Parameters:
+                * nnaammee_¶ – Dictionary containing COLDP Name record for which
+                  basionymID is to be fixed
+                * ssyynnoonnyymmss_¶ – List of COLDP Name records that may contain
+                  basionym
+        Returns:
+      Returns name following any updates.
   COLDP.find_name(sscciieennttiiffiiccNNaammee, aauutthhoorrsshhiipp, rraannkk)_¶
+      Return record from names DataFrame matching supplied scientificName,
+      authorship and rank
+        Parameters:
+                * sscciieennttiiffiiccNNaammee_¶ – Scientific name in canonical format
+                * aauutthhoorrsshhiipp_¶ – Authorship string
+                * rraannkk_¶ – Rank name string
+        Returns:
+            Dictionary containing matching record if found
+      Locates any existing record in the names DataFrame that matches the
+      supplied scientificName, authorship and rank and returns it as a COLDP
+      Name properties dictionary, or None if no match is found.
+      If _a_u_t_h_o_r_s_h_i_p is None, returns a name based only on scientificName and
+      rank.
   COLDP.find_taxon(sscciieennttiiffiiccNNaammee, aauutthhoorrsshhiipp, rraannkk)_¶
+      Get COLDP Taxon record (as Pandas dataframe) with accepted name matching
+      supplied scientificName, authorship and rank values
+        Parameters:
+                * sscciieennttiiffiiccNNaammee_¶ – Scientific name in canonical format
+                * aauutthhoorrsshhiipp_¶ – Authorship string
+                * rraannkk_¶ – Rank name string
+        Returns:
+            COLDP Taxon record matching supplied parameters
+      Logs a warning issue if multiple taxon records exist for a matching name
+      and returns the first such match. Returns None if no match.
   COLDP.construct_species_rank_name(gg, ssgg, ss, ssss, mmaarrkkeerr)_¶
       Consistently construct a species or infraspecific name from the included
       epithets and optional rank marker
         Parameters:
                 * gg_¶ – Genus name
                 * ssgg_¶ – Subgenus name
                 * ss_¶ – Specific epithet
@@ -575,28 +726,36 @@
       Check whether name is in for a rank below the subspecies
         Parameters:
             nnaammee_¶ – Dictionary representing a COLDP Name record
         Returns:
             True if the name is infraspecific
       Simply checks if the supplied rank is one of those below the subspecies.
   COLDP.issue(mmeessssaaggee)_¶
+      Log issue with data provided through methods
+        Parameters:
+            mmeessssaaggee_¶ – Text to be saved as body of issue
+      Creates a new record in an issues DataFrame that will be included in the
+      COLDP export when _s_a_v_e_(_) is called. This record includes the message and
+      the context string supplied on the most recent call to _s_e_t___c_o_n_t_e_x_t_(_).
+      If _i_s_s_u_e_s___t_o___s_t_d_o_u_t is True, the context and message are also output as
+      an error via logging.
 ********** IInnddeexx aanndd sseeaarrcchh_?¶ **********
     * _I_n_d_e_x
     * _S_e_a_r_c_h_ _P_a_g_e
 ************ _CC_OO_LL_DD_PP ************
 ******** NNaavviiggaattiioonn ********
-Contents:
     * _c_o_l_d_p_._C_O_L_D_P
           o _C_l_a_s_s
           o _M_e_t_h_o_d_s
           o _C_o_n_s_t_a_n_t_s
           o _I_n_t_e_r_n_a_l_ _m_e_t_h_o_d_s
           o _I_n_d_e_x_ _a_n_d_ _s_e_a_r_c_h
     * _c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e
+    * _U_s_a_g_e
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
-          o Previous: _C_O_L_D_P
+          o Previous: _c_o_l_d_p
           o Next: _c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
 ©2024, Donald Hobern. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r_ _0_._7_._1_6 | _P_a_g_e
 _s_o_u_r_c_e
```

### Comparing `coldp-2024.5.2/docs/build/html/genindex.html` & `coldp-2024.5.3/docs/build/html/genindex.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Index &#8212; COLDP 2024.5.2 documentation</title>
+    <title>Index &#8212; COLDP 2024.5.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
-    <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css?v=dd72e65a" />
-    <script src="_static/documentation_options.js?v=1723c9d4"></script>
+    <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
+    <script src="_static/documentation_options.js?v=b35b4dcd"></script>
     <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="#" />
     <link rel="search" title="Search" href="search.html" />
    
   <link rel="stylesheet" href="_static/custom.css" type="text/css" />
   
@@ -30,15 +30,16 @@
 
           <div class="body" role="main">
             
 
 <h1 id="index">Index</h1>
 
 <div class="genindex-jumpbox">
- <a href="#A"><strong>A</strong></a>
+ <a href="#_"><strong>_</strong></a>
+ | <a href="#A"><strong>A</strong></a>
  | <a href="#B"><strong>B</strong></a>
  | <a href="#C"><strong>C</strong></a>
  | <a href="#D"><strong>D</strong></a>
  | <a href="#E"><strong>E</strong></a>
  | <a href="#F"><strong>F</strong></a>
  | <a href="#G"><strong>G</strong></a>
  | <a href="#H"><strong>H</strong></a>
@@ -50,49 +51,73 @@
  | <a href="#R"><strong>R</strong></a>
  | <a href="#S"><strong>S</strong></a>
  | <a href="#T"><strong>T</strong></a>
  | <a href="#V"><strong>V</strong></a>
  | <a href="#Y"><strong>Y</strong></a>
  
 </div>
+<h2 id="_">_</h2>
+<table style="width: 100%" class="indextable genindextable"><tr>
+  <td style="width: 33%; vertical-align: top;"><ul>
+      <li><a href="coldp.html#coldp.COLDP.__init__">__init__() (coldp.COLDP method)</a>
+
+      <ul>
+        <li><a href="name-bundle.html#coldp.NameBundle.__init__">(coldp.NameBundle method)</a>
+</li>
+      </ul></li>
+  </ul></td>
+</tr></table>
+
 <h2 id="A">A</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="coldp.html#coldp.COLDP.construct_authorship.params.a">a (coldp.COLDP.construct_authorship parameter)</a>
 
       <ul>
         <li><a href="coldp.html#coldp.COLDP.same_basionym.params.a">(coldp.COLDP.same_basionym parameter)</a>
 </li>
       </ul></li>
-      <li><a href="name-bundle.html#coldp.NameBundle.params.accepted">accepted (coldp.NameBundle parameter)</a>
+      <li><a href="coldp.html#coldp.COLDP.start_name_bundle.params.accepted">accepted (coldp.COLDP.start_name_bundle parameter)</a>
+
+      <ul>
+        <li><a href="name-bundle.html#coldp.NameBundle.params.accepted">(coldp.NameBundle parameter)</a>
 </li>
+      </ul></li>
       <li><a href="coldp.html#coldp.COLDP.add_distribution">add_distribution() (coldp.COLDP method)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.add_name_relation">add_name_relation() (coldp.COLDP method)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.add_names">add_names() (coldp.COLDP method)</a>
 </li>
-  </ul></td>
-  <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="coldp.html#coldp.COLDP.add_references">add_references() (coldp.COLDP method)</a>
 </li>
+  </ul></td>
+  <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="coldp.html#coldp.COLDP.add_species_interaction">add_species_interaction() (coldp.COLDP method)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.add_synonym">add_synonym() (coldp.COLDP method)</a>
 
       <ul>
         <li><a href="name-bundle.html#coldp.NameBundle.add_synonym">(coldp.NameBundle method)</a>
 </li>
       </ul></li>
       <li><a href="coldp.html#coldp.COLDP.add_type_material">add_type_material() (coldp.COLDP method)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.params.allow_repeated_binomials">allow_repeated_binomials (coldp.COLDP parameter)</a>
 </li>
-      <li><a href="coldp.html#coldp.COLDP.get_original_authorship.params.authorship">authorship (coldp.COLDP.get_original_authorship parameter)</a>
+      <li><a href="coldp.html#coldp.COLDP.epithet_and_authorship_match.params.authorship">authorship (coldp.COLDP.epithet_and_authorship_match parameter)</a>
+
+      <ul>
+        <li><a href="coldp.html#coldp.COLDP.find_name.params.authorship">(coldp.COLDP.find_name parameter)</a>
+</li>
+        <li><a href="coldp.html#coldp.COLDP.find_taxon.params.authorship">(coldp.COLDP.find_taxon parameter)</a>
 </li>
+        <li><a href="coldp.html#coldp.COLDP.get_original_authorship.params.authorship">(coldp.COLDP.get_original_authorship parameter)</a>
+</li>
+      </ul></li>
   </ul></td>
 </tr></table>
 
 <h2 id="B">B</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="coldp.html#coldp.COLDP.same_basionym.params.b">b (coldp.COLDP.same_basionym parameter)</a>
@@ -151,46 +176,58 @@
 </li>
       <li><a href="coldp.html#coldp.COLDP.params.default_taxon_record">default_taxon_record (coldp.COLDP parameter)</a>
 
       <ul>
         <li><a href="coldp.html#coldp.COLDP.set_default_taxon_record.params.default_taxon_record">(coldp.COLDP.set_default_taxon_record parameter)</a>
 </li>
       </ul></li>
+      <li><a href="name-bundle.html#coldp.NameBundle.derive_name">derive_name() (coldp.NameBundle method)</a>
+</li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
-      <li><a href="name-bundle.html#coldp.NameBundle.derive_name">derive_name() (coldp.NameBundle method)</a>
+      <li><a href="coldp.html#coldp.COLDP.save.params.destination">destination (coldp.COLDP.save parameter)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.extract_table.params.df">df (coldp.COLDP.extract_table parameter)</a>
 
       <ul>
         <li><a href="coldp.html#coldp.COLDP.sort_taxa_recursive.params.df">(coldp.COLDP.sort_taxa_recursive parameter)</a>
 </li>
       </ul></li>
       <li><a href="coldp.html#coldp.COLDP.add_distribution.params.distribution">distribution (coldp.COLDP.add_distribution parameter)</a>
+
+      <ul>
+        <li><a href="coldp.html#coldp.COLDP.find_distribution.params.distribution">(coldp.COLDP.find_distribution parameter)</a>
 </li>
+      </ul></li>
   </ul></td>
 </tr></table>
 
 <h2 id="E">E</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
-      <li><a href="coldp.html#coldp.COLDP.remove_gender.params.epithet">epithet (coldp.COLDP.remove_gender parameter)</a>
+      <li><a href="coldp.html#coldp.COLDP.epithet_and_authorship_match.params.epithet">epithet (coldp.COLDP.epithet_and_authorship_match parameter)</a>
+
+      <ul>
+        <li><a href="coldp.html#coldp.COLDP.remove_gender.params.epithet">(coldp.COLDP.remove_gender parameter)</a>
 </li>
+      </ul></li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="coldp.html#coldp.COLDP.epithet_and_authorship_match">epithet_and_authorship_match() (coldp.COLDP method)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.extract_table">extract_table() (coldp.COLDP method)</a>
 </li>
   </ul></td>
 </tr></table>
 
 <h2 id="F">F</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
+      <li><a href="coldp.html#coldp.COLDP.find_distribution">find_distribution() (coldp.COLDP method)</a>
+</li>
       <li><a href="coldp.html#coldp.COLDP.find_name">find_name() (coldp.COLDP method)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.find_name_record">find_name_record() (coldp.COLDP method)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.find_names">find_names() (coldp.COLDP method)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.find_reference">find_reference() (coldp.COLDP method)</a>
@@ -247,36 +284,44 @@
 </li>
   </ul></td>
 </tr></table>
 
 <h2 id="I">I</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
-      <li><a href="coldp.html#coldp.COLDP.get_reference.params.id">id (coldp.COLDP.get_reference parameter)</a>
+      <li><a href="coldp.html#coldp.COLDP.get_name.params.id">id (coldp.COLDP.get_name parameter)</a>
 
       <ul>
+        <li><a href="coldp.html#coldp.COLDP.get_reference.params.id">(coldp.COLDP.get_reference parameter)</a>
+</li>
+        <li><a href="coldp.html#coldp.COLDP.get_taxon.params.id">(coldp.COLDP.get_taxon parameter)</a>
+</li>
         <li><a href="coldp.html#coldp.COLDP.sort_taxa_recursive.params.id">(coldp.COLDP.sort_taxa_recursive parameter)</a>
 </li>
       </ul></li>
       <li><a href="coldp.html#coldp.id_mappings">id_mappings (in module coldp)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.identify_name">identify_name() (coldp.COLDP method)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.sort_taxa_recursive.params.ids">ids (coldp.COLDP.sort_taxa_recursive parameter)</a>
 </li>
-      <li><a href="name-bundle.html#coldp.NameBundle.params.incertae_sedis">incertae_sedis (coldp.NameBundle parameter)</a>
+      <li><a href="coldp.html#coldp.COLDP.start_name_bundle.params.incertae_sedis">incertae_sedis (coldp.COLDP.start_name_bundle parameter)</a>
+
+      <ul>
+        <li><a href="name-bundle.html#coldp.NameBundle.params.incertae_sedis">(coldp.NameBundle parameter)</a>
 </li>
+      </ul></li>
       <li><a href="coldp.html#coldp.COLDP.get_text_tree.params.indent">indent (coldp.COLDP.get_text_tree parameter)</a>
 </li>
+  </ul></td>
+  <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="coldp.html#coldp.COLDP.get_text_tree.params.initial_prefix">initial_prefix (coldp.COLDP.get_text_tree parameter)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.initialise_dataframe">initialise_dataframe() (coldp.COLDP method)</a>
 </li>
-  </ul></td>
-  <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="coldp.html#coldp.COLDP.params.insert_species_for_trinomials">insert_species_for_trinomials (coldp.COLDP parameter)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.insert_synonym">insert_synonym() (coldp.COLDP method)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.insert_taxon">insert_taxon() (coldp.COLDP method)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.add_species_interaction.params.interaction">interaction (coldp.COLDP.add_species_interaction parameter)</a>
@@ -299,39 +344,49 @@
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="coldp.html#coldp.COLDP.extract_table.params.mappings">mappings (coldp.COLDP.extract_table parameter)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.construct_species_rank_name.params.marker">marker (coldp.COLDP.construct_species_rank_name parameter)</a>
 </li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
+      <li><a href="coldp.html#coldp.COLDP.issue.params.message">message (coldp.COLDP.issue parameter)</a>
+</li>
       <li><a href="coldp.html#coldp.COLDP.modify_name">modify_name() (coldp.COLDP method)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.modify_taxon">modify_taxon() (coldp.COLDP method)</a>
 </li>
   </ul></td>
 </tr></table>
 
 <h2 id="N">N</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="coldp.html#coldp.COLDP.params.name">name (coldp.COLDP parameter)</a>
 
       <ul>
+        <li><a href="coldp.html#coldp.COLDP.epithet_and_authorship_match.params.name">(coldp.COLDP.epithet_and_authorship_match parameter)</a>
+</li>
         <li><a href="coldp.html#coldp.COLDP.find_name_record.params.name">(coldp.COLDP.find_name_record parameter)</a>
 </li>
+        <li><a href="coldp.html#coldp.COLDP.fix_basionymid.params.name">(coldp.COLDP.fix_basionymid parameter)</a>
+</li>
         <li><a href="coldp.html#coldp.COLDP.identify_name.params.name">(coldp.COLDP.identify_name parameter)</a>
 </li>
         <li><a href="coldp.html#coldp.COLDP.initialise_dataframe.params.name">(coldp.COLDP.initialise_dataframe parameter)</a>
 </li>
+        <li><a href="coldp.html#coldp.COLDP.insert_taxon.params.name">(coldp.COLDP.insert_taxon parameter)</a>
+</li>
         <li><a href="coldp.html#coldp.COLDP.is_infrasubspecific.params.name">(coldp.COLDP.is_infrasubspecific parameter)</a>
 </li>
         <li><a href="coldp.html#coldp.COLDP.is_species_group.params.name">(coldp.COLDP.is_species_group parameter)</a>
 </li>
         <li><a href="coldp.html#coldp.COLDP.reset_ids.params.name">(coldp.COLDP.reset_ids parameter)</a>
 </li>
+        <li><a href="coldp.html#coldp.COLDP.save.params.name">(coldp.COLDP.save parameter)</a>
+</li>
         <li><a href="coldp.html#coldp.COLDP.set_basionymid.params.name">(coldp.COLDP.set_basionymid parameter)</a>
 </li>
         <li><a href="coldp.html#coldp.COLDP.table_by_name.params.name">(coldp.COLDP.table_by_name parameter)</a>
 </li>
         <li><a href="name-bundle.html#coldp.NameBundle.derive_name.params.name">(coldp.NameBundle.derive_name parameter)</a>
 </li>
         <li><a href="name-bundle.html#coldp.NameBundle.normalise_name.params.name">(coldp.NameBundle.normalise_name parameter)</a>
@@ -365,40 +420,50 @@
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="coldp.html#coldp.COLDP.add_names.params.parent">parent (coldp.COLDP.add_names parameter)</a>
 
       <ul>
         <li><a href="coldp.html#coldp.COLDP.fix_classification_recursive.params.parent">(coldp.COLDP.fix_classification_recursive parameter)</a>
 </li>
       </ul></li>
+      <li><a href="coldp.html#coldp.COLDP.insert_taxon.params.parentID">parentID (coldp.COLDP.insert_taxon parameter)</a>
+</li>
       <li><a href="coldp.html#coldp.COLDP.reset_ids.params.prefix">prefix (coldp.COLDP.reset_ids parameter)</a>
 </li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="coldp.html#coldp.COLDP.prepare_bundle">prepare_bundle() (coldp.COLDP method)</a>
 </li>
-      <li><a href="coldp.html#coldp.COLDP.modify_name.params.properties">properties (coldp.COLDP.modify_name parameter)</a>
+      <li><a href="coldp.html#coldp.COLDP.find_names.params.properties">properties (coldp.COLDP.find_names parameter)</a>
 
       <ul>
+        <li><a href="coldp.html#coldp.COLDP.modify_name.params.properties">(coldp.COLDP.modify_name parameter)</a>
+</li>
         <li><a href="coldp.html#coldp.COLDP.modify_taxon.params.properties">(coldp.COLDP.modify_taxon parameter)</a>
 </li>
       </ul></li>
   </ul></td>
 </tr></table>
 
 <h2 id="R">R</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
+      <li><a href="coldp.html#coldp.COLDP.find_name.params.rank">rank (coldp.COLDP.find_name parameter)</a>
+
+      <ul>
+        <li><a href="coldp.html#coldp.COLDP.find_taxon.params.rank">(coldp.COLDP.find_taxon parameter)</a>
+</li>
+      </ul></li>
       <li><a href="coldp.html#coldp.COLDP.fix_classification_recursive.params.ranks">ranks (coldp.COLDP.fix_classification_recursive parameter)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.validate_record.params.record">record (coldp.COLDP.validate_record parameter)</a>
 </li>
-      <li><a href="coldp.html#coldp.COLDP.validate_record.params.record_type">record_type (coldp.COLDP.validate_record parameter)</a>
-</li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
+      <li><a href="coldp.html#coldp.COLDP.validate_record.params.record_type">record_type (coldp.COLDP.validate_record parameter)</a>
+</li>
       <li><a href="coldp.html#coldp.COLDP.find_reference.params.reference">reference (coldp.COLDP.find_reference parameter)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.add_references.params.reference_list">reference_list (coldp.COLDP.add_references parameter)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.remove_gender">remove_gender() (coldp.COLDP method)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.reset_ids">reset_ids() (coldp.COLDP method)</a>
@@ -411,27 +476,35 @@
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="coldp.html#coldp.COLDP.construct_species_rank_name.params.s">s (coldp.COLDP.construct_species_rank_name parameter)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.same_basionym">same_basionym() (coldp.COLDP method)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.save">save() (coldp.COLDP method)</a>
 </li>
+      <li><a href="coldp.html#coldp.COLDP.find_name.params.scientificName">scientificName (coldp.COLDP.find_name parameter)</a>
+
+      <ul>
+        <li><a href="coldp.html#coldp.COLDP.find_taxon.params.scientificName">(coldp.COLDP.find_taxon parameter)</a>
+</li>
+      </ul></li>
       <li><a href="coldp.html#coldp.COLDP.set_basionymid">set_basionymid() (coldp.COLDP method)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.set_context">set_context() (coldp.COLDP method)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.set_default_taxon_record">set_default_taxon_record() (coldp.COLDP method)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.set_options">set_options() (coldp.COLDP method)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.construct_species_rank_name.params.sg">sg (coldp.COLDP.construct_species_rank_name parameter)</a>
 </li>
-      <li><a href="name-bundle.html#coldp.NameBundle.params.sic">sic (coldp.NameBundle parameter)</a>
+      <li><a href="coldp.html#coldp.COLDP.start_name_bundle.params.sic">sic (coldp.COLDP.start_name_bundle parameter)</a>
 
       <ul>
+        <li><a href="name-bundle.html#coldp.NameBundle.params.sic">(coldp.NameBundle parameter)</a>
+</li>
         <li><a href="name-bundle.html#coldp.NameBundle.add_synonym.params.sic">(coldp.NameBundle.add_synonym parameter)</a>
 </li>
         <li><a href="name-bundle.html#coldp.NameBundle.normalise_name.params.sic">(coldp.NameBundle.normalise_name parameter)</a>
 </li>
       </ul></li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
@@ -451,16 +524,20 @@
         <li><a href="name-bundle.html#coldp.NameBundle.add_synonym.params.synonym">(coldp.NameBundle.add_synonym parameter)</a>
 </li>
       </ul></li>
       <li><a href="coldp.html#coldp.synonym_from_nameusage">synonym_from_nameusage (in module coldp)</a>
 </li>
       <li><a href="coldp.html#coldp.COLDP.get_text_tree.params.synonym_prefix">synonym_prefix (coldp.COLDP.get_text_tree parameter)</a>
 </li>
-      <li><a href="coldp.html#coldp.COLDP.fix_basionyms.params.synonyms">synonyms (coldp.COLDP.fix_basionyms parameter)</a>
+      <li><a href="coldp.html#coldp.COLDP.fix_basionymid.params.synonyms">synonyms (coldp.COLDP.fix_basionymid parameter)</a>
+
+      <ul>
+        <li><a href="coldp.html#coldp.COLDP.fix_basionyms.params.synonyms">(coldp.COLDP.fix_basionyms parameter)</a>
 </li>
+      </ul></li>
   </ul></td>
 </tr></table>
 
 <h2 id="T">T</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="coldp.html#coldp.COLDP.table_by_name">table_by_name() (coldp.COLDP method)</a>
@@ -473,18 +550,36 @@
 
       <ul>
         <li><a href="coldp.html#coldp.COLDP.modify_name.params.taxon_id">(coldp.COLDP.modify_name parameter)</a>
 </li>
         <li><a href="coldp.html#coldp.COLDP.modify_taxon.params.taxon_id">(coldp.COLDP.modify_taxon parameter)</a>
 </li>
       </ul></li>
+      <li><a href="coldp.html#coldp.COLDP.get_children.params.taxonID">taxonID (coldp.COLDP.get_children parameter)</a>
+
+      <ul>
+        <li><a href="coldp.html#coldp.COLDP.get_synonyms.params.taxonID">(coldp.COLDP.get_synonyms parameter)</a>
+</li>
+        <li><a href="coldp.html#coldp.COLDP.get_synonymy.params.taxonID">(coldp.COLDP.get_synonymy parameter)</a>
+</li>
+        <li><a href="coldp.html#coldp.COLDP.get_text_tree.params.taxonID">(coldp.COLDP.get_text_tree parameter)</a>
+</li>
+      </ul></li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
-      <li><a href="coldp.html#coldp.COLDP.get_text_tree.params.taxonID">taxonID (coldp.COLDP.get_text_tree parameter)</a>
+      <li><a href="coldp.html#coldp.COLDP.find_names.params.to_dict">to_dict (coldp.COLDP.find_names parameter)</a>
+
+      <ul>
+        <li><a href="coldp.html#coldp.COLDP.get_children.params.to_dict">(coldp.COLDP.get_children parameter)</a>
+</li>
+        <li><a href="coldp.html#coldp.COLDP.get_synonyms.params.to_dict">(coldp.COLDP.get_synonyms parameter)</a>
 </li>
+        <li><a href="coldp.html#coldp.COLDP.get_synonymy.params.to_dict">(coldp.COLDP.get_synonymy parameter)</a>
+</li>
+      </ul></li>
       <li><a href="coldp.html#coldp.COLDP.add_type_material.params.type_material">type_material (coldp.COLDP.add_type_material parameter)</a>
 </li>
   </ul></td>
 </tr></table>
 
 <h2 id="V">V</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
@@ -520,19 +615,21 @@
 
 
 
 
 
 
 <h3>Navigation</h3>
-<p class="caption" role="heading"><span class="caption-text">Contents:</span></p>
 <ul>
 <li class="toctree-l1"><a class="reference internal" href="coldp.html">coldp.COLDP</a></li>
 <li class="toctree-l1"><a class="reference internal" href="name-bundle.html">coldp.NameBundle</a></li>
 </ul>
+<ul>
+<li class="toctree-l1"><a class="reference internal" href="usage.html">Usage</a></li>
+</ul>
 
 <div class="relations">
 <h3>Related Topics</h3>
 <ul>
   <li><a href="index.html">Documentation overview</a><ul>
   </ul></li>
 </ul>
```

#### html2text {}

```diff
@@ -1,23 +1,30 @@
 ************ IInnddeexx ************
-_AA | _BB | _CC | _DD | _EE | _FF | _GG | _HH | _II | _MM | _NN | _OO | _PP | _RR | _SS | _TT | _VV | _YY
+___ | _AA | _BB | _CC | _DD | _EE | _FF | _GG | _HH | _II | _MM | _NN | _OO | _PP | _RR | _SS | _TT | _VV | _YY
+********** __ **********
+    * _____i_n_i_t_____(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
+          o _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e_ _m_e_t_h_o_d_)
 ********** AA **********
-    * _a_                                     * _a_d_d___r_e_f_e_r_e_n_c_e_s_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
+    * _a_                                     * _a_d_d___s_p_e_c_i_e_s___i_n_t_e_r_a_c_t_i_o_n_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
       _(_c_o_l_d_p_._C_O_L_D_P_._c_o_n_s_t_r_u_c_t___a_u_t_h_o_r_s_h_i_p       _m_e_t_h_o_d_)
-      _p_a_r_a_m_e_t_e_r_)                            * _a_d_d___s_p_e_c_i_e_s___i_n_t_e_r_a_c_t_i_o_n_(_)_ 
-          o _(_c_o_l_d_p_._C_O_L_D_P_._s_a_m_e___b_a_s_i_o_n_y_m        _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
-            _p_a_r_a_m_e_t_e_r_)                      * _a_d_d___s_y_n_o_n_y_m_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
-    * _a_c_c_e_p_t_e_d_ _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e                  o _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e_ _m_e_t_h_o_d_)
-      _p_a_r_a_m_e_t_e_r_)                            * _a_d_d___t_y_p_e___m_a_t_e_r_i_a_l_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
-    * _a_d_d___d_i_s_t_r_i_b_u_t_i_o_n_(_)_ _(_c_o_l_d_p_._C_O_L_D_P         _m_e_t_h_o_d_)
-      _m_e_t_h_o_d_)                               * _a_l_l_o_w___r_e_p_e_a_t_e_d___b_i_n_o_m_i_a_l_s_ 
-    * _a_d_d___n_a_m_e___r_e_l_a_t_i_o_n_(_)_ _(_c_o_l_d_p_._C_O_L_D_P        _(_c_o_l_d_p_._C_O_L_D_P_ _p_a_r_a_m_e_t_e_r_)
-      _m_e_t_h_o_d_)                               * _a_u_t_h_o_r_s_h_i_p_ 
-    * _a_d_d___n_a_m_e_s_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)        _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___o_r_i_g_i_n_a_l___a_u_t_h_o_r_s_h_i_p
-                                              _p_a_r_a_m_e_t_e_r_)
+      _p_a_r_a_m_e_t_e_r_)                            * _a_d_d___s_y_n_o_n_y_m_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
+          o _(_c_o_l_d_p_._C_O_L_D_P_._s_a_m_e___b_a_s_i_o_n_y_m            o _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e_ _m_e_t_h_o_d_)
+            _p_a_r_a_m_e_t_e_r_)                      * _a_d_d___t_y_p_e___m_a_t_e_r_i_a_l_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
+    * _a_c_c_e_p_t_e_d_                              * _a_l_l_o_w___r_e_p_e_a_t_e_d___b_i_n_o_m_i_a_l_s_ _(_c_o_l_d_p_._C_O_L_D_P
+      _(_c_o_l_d_p_._C_O_L_D_P_._s_t_a_r_t___n_a_m_e___b_u_n_d_l_e          _p_a_r_a_m_e_t_e_r_)
+      _p_a_r_a_m_e_t_e_r_)                            * _a_u_t_h_o_r_s_h_i_p_ 
+          o _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e                 _(_c_o_l_d_p_._C_O_L_D_P_._e_p_i_t_h_e_t___a_n_d___a_u_t_h_o_r_s_h_i_p___m_a_t_c_h
+            _p_a_r_a_m_e_t_e_r_)                        _p_a_r_a_m_e_t_e_r_)
+    * _a_d_d___d_i_s_t_r_i_b_u_t_i_o_n_(_)_ _(_c_o_l_d_p_._C_O_L_D_P             o _(_c_o_l_d_p_._C_O_L_D_P_._f_i_n_d___n_a_m_e_ _p_a_r_a_m_e_t_e_r_)
+      _m_e_t_h_o_d_)                                     o _(_c_o_l_d_p_._C_O_L_D_P_._f_i_n_d___t_a_x_o_n_ _p_a_r_a_m_e_t_e_r_)
+    * _a_d_d___n_a_m_e___r_e_l_a_t_i_o_n_(_)_ _(_c_o_l_d_p_._C_O_L_D_P            o _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___o_r_i_g_i_n_a_l___a_u_t_h_o_r_s_h_i_p
+      _m_e_t_h_o_d_)                                       _p_a_r_a_m_e_t_e_r_)
+    * _a_d_d___n_a_m_e_s_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
+    * _a_d_d___r_e_f_e_r_e_n_c_e_s_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
+      _m_e_t_h_o_d_)
 ********** BB **********
     * _b_ _(_c_o_l_d_p_._C_O_L_D_P_._s_a_m_e___b_a_s_i_o_n_y_m     * _b_a_s_i_o_n_y_m_s___f_r_o_m___s_y_n_o_n_y_m_s_ _(_c_o_l_d_p_._C_O_L_D_P
       _p_a_r_a_m_e_t_e_r_)                         _p_a_r_a_m_e_t_e_r_)
     * _b_a_s_i_o_n_y_m_i_d_                       * _b_u_n_d_l_e_ _(_c_o_l_d_p_._C_O_L_D_P_._a_d_d___n_a_m_e_s
       _(_c_o_l_d_p_._C_O_L_D_P_._s_e_t___b_a_s_i_o_n_y_m_i_d        _p_a_r_a_m_e_t_e_r_)
       _p_a_r_a_m_e_t_e_r_)                             o _(_c_o_l_d_p_._C_O_L_D_P_._p_r_e_p_a_r_e___b_u_n_d_l_e
                                                _p_a_r_a_m_e_t_e_r_)
@@ -29,38 +36,41 @@
     * _c_o_l_d_p_ _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e           _(_c_o_l_d_p_._C_O_L_D_P_ _p_a_r_a_m_e_t_e_r_)
       _p_a_r_a_m_e_t_e_r_)                      * _c_r_e_a_t_e___s_y_n_o_n_y_m_s___w_i_t_h_o_u_t___s_u_b_g_e_n_u_s_ 
     * _c_o_n_s_t_r_u_c_t___a_u_t_h_o_r_s_h_i_p_(_)_            _(_c_o_l_d_p_._C_O_L_D_P_ _p_a_r_a_m_e_t_e_r_)
       _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)            * _c_r_e_a_t_e___t_a_x_a___f_o_r___n_o_t___e_s_t_a_b_l_i_s_h_e_d_ 
     * _c_o_n_s_t_r_u_c_t___s_p_e_c_i_e_s___r_a_n_k___n_a_m_e       _(_c_o_l_d_p_._C_O_L_D_P_ _p_a_r_a_m_e_t_e_r_)
       _(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)         * _c_s_v___e_x_t_e_n_s_i_o_n_s_ _(_i_n_ _m_o_d_u_l_e_ _c_o_l_d_p_)
 ********** DD **********
-    * _d_e_f_a_u_l_t___h_e_a_d_i_n_g_s_                                * _d_e_r_i_v_e___n_a_m_e_(_)_ _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e
-      _(_c_o_l_d_p_._C_O_L_D_P_._i_n_i_t_i_a_l_i_s_e___d_a_t_a_f_r_a_m_e                 _m_e_t_h_o_d_)
+    * _d_e_f_a_u_l_t___h_e_a_d_i_n_g_s_                                * _d_e_s_t_i_n_a_t_i_o_n_ _(_c_o_l_d_p_._C_O_L_D_P_._s_a_v_e
+      _(_c_o_l_d_p_._C_O_L_D_P_._i_n_i_t_i_a_l_i_s_e___d_a_t_a_f_r_a_m_e                 _p_a_r_a_m_e_t_e_r_)
       _p_a_r_a_m_e_t_e_r_)                                      * _d_f_ _(_c_o_l_d_p_._C_O_L_D_P_._e_x_t_r_a_c_t___t_a_b_l_e
     * _d_e_f_a_u_l_t___t_a_x_o_n___r_e_c_o_r_d_ _(_c_o_l_d_p_._C_O_L_D_P                 _p_a_r_a_m_e_t_e_r_)
       _p_a_r_a_m_e_t_e_r_)                                            o _(_c_o_l_d_p_._C_O_L_D_P_._s_o_r_t___t_a_x_a___r_e_c_u_r_s_i_v_e
           o _(_c_o_l_d_p_._C_O_L_D_P_._s_e_t___d_e_f_a_u_l_t___t_a_x_o_n___r_e_c_o_r_d             _p_a_r_a_m_e_t_e_r_)
             _p_a_r_a_m_e_t_e_r_)                                * _d_i_s_t_r_i_b_u_t_i_o_n_ 
-                                                        _(_c_o_l_d_p_._C_O_L_D_P_._a_d_d___d_i_s_t_r_i_b_u_t_i_o_n
+    * _d_e_r_i_v_e___n_a_m_e_(_)_ _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e_ _m_e_t_h_o_d_)           _(_c_o_l_d_p_._C_O_L_D_P_._a_d_d___d_i_s_t_r_i_b_u_t_i_o_n
                                                         _p_a_r_a_m_e_t_e_r_)
+                                                            o _(_c_o_l_d_p_._C_O_L_D_P_._f_i_n_d___d_i_s_t_r_i_b_u_t_i_o_n
+                                                              _p_a_r_a_m_e_t_e_r_)
 ********** EE **********
-    * _e_p_i_t_h_e_t_ _(_c_o_l_d_p_._C_O_L_D_P_._r_e_m_o_v_e___g_e_n_d_e_r     * _e_p_i_t_h_e_t___a_n_d___a_u_t_h_o_r_s_h_i_p___m_a_t_c_h_(_)_ 
-      _p_a_r_a_m_e_t_e_r_)                               _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
-                                             * _e_x_t_r_a_c_t___t_a_b_l_e_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
-                                               _m_e_t_h_o_d_)
+    * _e_p_i_t_h_e_t_                                       * _e_p_i_t_h_e_t___a_n_d___a_u_t_h_o_r_s_h_i_p___m_a_t_c_h
+      _(_c_o_l_d_p_._C_O_L_D_P_._e_p_i_t_h_e_t___a_n_d___a_u_t_h_o_r_s_h_i_p___m_a_t_c_h       _(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
+      _p_a_r_a_m_e_t_e_r_)                                    * _e_x_t_r_a_c_t___t_a_b_l_e_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
+          o _(_c_o_l_d_p_._C_O_L_D_P_._r_e_m_o_v_e___g_e_n_d_e_r                _m_e_t_h_o_d_)
+            _p_a_r_a_m_e_t_e_r_)
 ********** FF **********
-    * _f_i_n_d___n_a_m_e_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)      * _f_i_x___b_a_s_i_o_n_y_m_i_d_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
+    * _f_i_n_d___d_i_s_t_r_i_b_u_t_i_o_n_(_)_ _(_c_o_l_d_p_._C_O_L_D_P      * _f_i_x___b_a_s_i_o_n_y_m_i_d_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
+      _m_e_t_h_o_d_)                                 _m_e_t_h_o_d_)
+    * _f_i_n_d___n_a_m_e_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)      * _f_i_x___b_a_s_i_o_n_y_m_s_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
     * _f_i_n_d___n_a_m_e___r_e_c_o_r_d_(_)_ _(_c_o_l_d_p_._C_O_L_D_P         _m_e_t_h_o_d_)
-      _m_e_t_h_o_d_)                               * _f_i_x___b_a_s_i_o_n_y_m_s_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
+      _m_e_t_h_o_d_)                               * _f_i_x___c_l_a_s_s_i_f_i_c_a_t_i_o_n_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
     * _f_i_n_d___n_a_m_e_s_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)       _m_e_t_h_o_d_)
-    * _f_i_n_d___r_e_f_e_r_e_n_c_e_(_)_ _(_c_o_l_d_p_._C_O_L_D_P         * _f_i_x___c_l_a_s_s_i_f_i_c_a_t_i_o_n_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
-      _m_e_t_h_o_d_)                                 _m_e_t_h_o_d_)
-    * _f_i_n_d___t_a_x_o_n_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)     * _f_i_x___c_l_a_s_s_i_f_i_c_a_t_i_o_n___r_e_c_u_r_s_i_v_e_(_)_ 
-                                              _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
-                                            * _f_o_l_d_e_r_ _(_c_o_l_d_p_._C_O_L_D_P_ _p_a_r_a_m_e_t_e_r_)
+    * _f_i_n_d___r_e_f_e_r_e_n_c_e_(_)_ _(_c_o_l_d_p_._C_O_L_D_P         * _f_i_x___c_l_a_s_s_i_f_i_c_a_t_i_o_n___r_e_c_u_r_s_i_v_e_(_)_ 
+      _m_e_t_h_o_d_)                                 _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
+    * _f_i_n_d___t_a_x_o_n_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)     * _f_o_l_d_e_r_ _(_c_o_l_d_p_._C_O_L_D_P_ _p_a_r_a_m_e_t_e_r_)
                                             * _f_o_l_d_e_r_n_a_m_e_ 
                                               _(_c_o_l_d_p_._C_O_L_D_P_._i_n_i_t_i_a_l_i_s_e___d_a_t_a_f_r_a_m_e
                                               _p_a_r_a_m_e_t_e_r_)
 ********** GG **********
     * _g_                                            * _g_e_t___r_e_f_e_r_e_n_c_e_(_)_ 
       _(_c_o_l_d_p_._C_O_L_D_P_._c_o_n_s_t_r_u_c_t___s_p_e_c_i_e_s___r_a_n_k___n_a_m_e       _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
       _p_a_r_a_m_e_t_e_r_)                                   * _g_e_t___s_y_n_o_n_y_m_s_(_)_ 
@@ -70,118 +80,141 @@
       _m_e_t_h_o_d_)                                      * _g_e_t___t_a_x_o_n_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
                                                      _m_e_t_h_o_d_)
                                                    * _g_e_t___t_e_x_t___t_r_e_e_(_)_ 
                                                      _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
 ********** HH **********
     * _h_e_a_d_i_n_g_s_ _(_c_o_l_d_p_._C_O_L_D_P_._e_x_t_r_a_c_t___t_a_b_l_e_ _p_a_r_a_m_e_t_e_r_)
 ********** II **********
-    * _i_d_ _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___r_e_f_e_r_e_n_c_e              * _i_n_s_e_r_t___s_p_e_c_i_e_s___f_o_r___t_r_i_n_o_m_i_a_l_s_ 
-      _p_a_r_a_m_e_t_e_r_)                                   _(_c_o_l_d_p_._C_O_L_D_P_ _p_a_r_a_m_e_t_e_r_)
-          o _(_c_o_l_d_p_._C_O_L_D_P_._s_o_r_t___t_a_x_a___r_e_c_u_r_s_i_v_e     * _i_n_s_e_r_t___s_y_n_o_n_y_m_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
+    * _i_d_ _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___n_a_m_e_ _p_a_r_a_m_e_t_e_r_)        * _i_n_i_t_i_a_l___p_r_e_f_i_x_ 
+          o _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___r_e_f_e_r_e_n_c_e             _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___t_e_x_t___t_r_e_e
+            _p_a_r_a_m_e_t_e_r_)                             _p_a_r_a_m_e_t_e_r_)
+          o _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___t_a_x_o_n               * _i_n_i_t_i_a_l_i_s_e___d_a_t_a_f_r_a_m_e_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
             _p_a_r_a_m_e_t_e_r_)                             _m_e_t_h_o_d_)
-    * _i_d___m_a_p_p_i_n_g_s_ _(_i_n_ _m_o_d_u_l_e_ _c_o_l_d_p_)              * _i_n_s_e_r_t___t_a_x_o_n_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
-    * _i_d_e_n_t_i_f_y___n_a_m_e_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)       * _i_n_t_e_r_a_c_t_i_o_n_ 
-    * _i_d_s_ _(_c_o_l_d_p_._C_O_L_D_P_._s_o_r_t___t_a_x_a___r_e_c_u_r_s_i_v_e         _(_c_o_l_d_p_._C_O_L_D_P_._a_d_d___s_p_e_c_i_e_s___i_n_t_e_r_a_c_t_i_o_n
-      _p_a_r_a_m_e_t_e_r_)                                   _p_a_r_a_m_e_t_e_r_)
-    * _i_n_c_e_r_t_a_e___s_e_d_i_s_ _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e           * _i_s___b_a_s_i_o_n_y_m_ 
-      _p_a_r_a_m_e_t_e_r_)                                   _(_c_o_l_d_p_._C_O_L_D_P_._c_o_n_s_t_r_u_c_t___a_u_t_h_o_r_s_h_i_p
+          o _(_c_o_l_d_p_._C_O_L_D_P_._s_o_r_t___t_a_x_a___r_e_c_u_r_s_i_v_e     * _i_n_s_e_r_t___s_p_e_c_i_e_s___f_o_r___t_r_i_n_o_m_i_a_l_s_ 
+            _p_a_r_a_m_e_t_e_r_)                             _(_c_o_l_d_p_._C_O_L_D_P_ _p_a_r_a_m_e_t_e_r_)
+    * _i_d___m_a_p_p_i_n_g_s_ _(_i_n_ _m_o_d_u_l_e_ _c_o_l_d_p_)              * _i_n_s_e_r_t___s_y_n_o_n_y_m_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
+    * _i_d_e_n_t_i_f_y___n_a_m_e_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)         _m_e_t_h_o_d_)
+    * _i_d_s_ _(_c_o_l_d_p_._C_O_L_D_P_._s_o_r_t___t_a_x_a___r_e_c_u_r_s_i_v_e       * _i_n_s_e_r_t___t_a_x_o_n_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
+      _p_a_r_a_m_e_t_e_r_)                                 * _i_n_t_e_r_a_c_t_i_o_n_ 
+    * _i_n_c_e_r_t_a_e___s_e_d_i_s_                               _(_c_o_l_d_p_._C_O_L_D_P_._a_d_d___s_p_e_c_i_e_s___i_n_t_e_r_a_c_t_i_o_n
+      _(_c_o_l_d_p_._C_O_L_D_P_._s_t_a_r_t___n_a_m_e___b_u_n_d_l_e               _p_a_r_a_m_e_t_e_r_)
+      _p_a_r_a_m_e_t_e_r_)                                 * _i_s___b_a_s_i_o_n_y_m_ 
+          o _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e_ _p_a_r_a_m_e_t_e_r_)           _(_c_o_l_d_p_._C_O_L_D_P_._c_o_n_s_t_r_u_c_t___a_u_t_h_o_r_s_h_i_p
     * _i_n_d_e_n_t_ _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___t_e_x_t___t_r_e_e            _p_a_r_a_m_e_t_e_r_)
       _p_a_r_a_m_e_t_e_r_)                                 * _i_s___i_n_f_r_a_s_u_b_s_p_e_c_i_f_i_c_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
-    * _i_n_i_t_i_a_l___p_r_e_f_i_x_                               _m_e_t_h_o_d_)
-      _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___t_e_x_t___t_r_e_e_ _p_a_r_a_m_e_t_e_r_)      * _i_s___s_p_e_c_i_e_s___g_r_o_u_p_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
-    * _i_n_i_t_i_a_l_i_s_e___d_a_t_a_f_r_a_m_e_(_)_ _(_c_o_l_d_p_._C_O_L_D_P          _m_e_t_h_o_d_)
-      _m_e_t_h_o_d_)                                    * _i_s_s_u_e_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
+                                                   _m_e_t_h_o_d_)
+                                                 * _i_s___s_p_e_c_i_e_s___g_r_o_u_p_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
+                                                   _m_e_t_h_o_d_)
+                                                 * _i_s_s_u_e_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
                                                  * _i_s_s_u_e_s___t_o___s_t_d_o_u_t_ _(_c_o_l_d_p_._C_O_L_D_P
                                                    _p_a_r_a_m_e_t_e_r_)
 ********** MM **********
-    * _m_a_p_p_i_n_g_s_ _(_c_o_l_d_p_._C_O_L_D_P_._e_x_t_r_a_c_t___t_a_b_l_e          * _m_o_d_i_f_y___n_a_m_e_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
-      _p_a_r_a_m_e_t_e_r_)                                     _m_e_t_h_o_d_)
-    * _m_a_r_k_e_r_                                       * _m_o_d_i_f_y___t_a_x_o_n_(_)_ 
-      _(_c_o_l_d_p_._C_O_L_D_P_._c_o_n_s_t_r_u_c_t___s_p_e_c_i_e_s___r_a_n_k___n_a_m_e       _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
-      _p_a_r_a_m_e_t_e_r_)
+    * _m_a_p_p_i_n_g_s_ _(_c_o_l_d_p_._C_O_L_D_P_._e_x_t_r_a_c_t___t_a_b_l_e          * _m_e_s_s_a_g_e_ _(_c_o_l_d_p_._C_O_L_D_P_._i_s_s_u_e
+      _p_a_r_a_m_e_t_e_r_)                                     _p_a_r_a_m_e_t_e_r_)
+    * _m_a_r_k_e_r_                                       * _m_o_d_i_f_y___n_a_m_e_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
+      _(_c_o_l_d_p_._C_O_L_D_P_._c_o_n_s_t_r_u_c_t___s_p_e_c_i_e_s___r_a_n_k___n_a_m_e       _m_e_t_h_o_d_)
+      _p_a_r_a_m_e_t_e_r_)                                   * _m_o_d_i_f_y___t_a_x_o_n_(_)_ 
+                                                     _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
 ********** NN **********
-    * _n_a_m_e_ _(_c_o_l_d_p_._C_O_L_D_P_ _p_a_r_a_m_e_t_e_r_)                * _n_a_m_e___f_r_o_m___n_a_m_e_u_s_a_g_e_ _(_i_n_ _m_o_d_u_l_e
-          o _(_c_o_l_d_p_._C_O_L_D_P_._f_i_n_d___n_a_m_e___r_e_c_o_r_d           _c_o_l_d_p_)
-            _p_a_r_a_m_e_t_e_r_)                            * _n_a_m_e___i_d_ 
-          o _(_c_o_l_d_p_._C_O_L_D_P_._i_d_e_n_t_i_f_y___n_a_m_e              _(_c_o_l_d_p_._C_O_L_D_P_._i_n_s_e_r_t___s_y_n_o_n_y_m
-            _p_a_r_a_m_e_t_e_r_)                              _p_a_r_a_m_e_t_e_r_)
-          o _(_c_o_l_d_p_._C_O_L_D_P_._i_n_i_t_i_a_l_i_s_e___d_a_t_a_f_r_a_m_e     * _n_a_m_e___r_e_l_a_t_i_o_n_ 
-            _p_a_r_a_m_e_t_e_r_)                              _(_c_o_l_d_p_._C_O_L_D_P_._a_d_d___n_a_m_e___r_e_l_a_t_i_o_n
-          o _(_c_o_l_d_p_._C_O_L_D_P_._i_s___i_n_f_r_a_s_u_b_s_p_e_c_i_f_i_c        _p_a_r_a_m_e_t_e_r_)
-            _p_a_r_a_m_e_t_e_r_)                            * _n_a_m_e_s_ 
-          o _(_c_o_l_d_p_._C_O_L_D_P_._i_s___s_p_e_c_i_e_s___g_r_o_u_p           _(_c_o_l_d_p_._C_O_L_D_P_._f_i_x___b_a_s_i_o_n_y_m_s
-            _p_a_r_a_m_e_t_e_r_)                              _p_a_r_a_m_e_t_e_r_)
-          o _(_c_o_l_d_p_._C_O_L_D_P_._r_e_s_e_t___i_d_s_ _p_a_r_a_m_e_t_e_r_)     * _n_o_r_m_a_l_i_s_e___n_a_m_e_(_)_ 
-          o _(_c_o_l_d_p_._C_O_L_D_P_._s_e_t___b_a_s_i_o_n_y_m_i_d             _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e_ _m_e_t_h_o_d_)
-            _p_a_r_a_m_e_t_e_r_)
-          o _(_c_o_l_d_p_._C_O_L_D_P_._t_a_b_l_e___b_y___n_a_m_e
-            _p_a_r_a_m_e_t_e_r_)
-          o _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e_._d_e_r_i_v_e___n_a_m_e
-            _p_a_r_a_m_e_t_e_r_)
+    * _n_a_m_e_ _(_c_o_l_d_p_._C_O_L_D_P_ _p_a_r_a_m_e_t_e_r_)                        * _n_a_m_e___f_r_o_m___n_a_m_e_u_s_a_g_e_ _(_i_n_ _m_o_d_u_l_e
+          o _(_c_o_l_d_p_._C_O_L_D_P_._e_p_i_t_h_e_t___a_n_d___a_u_t_h_o_r_s_h_i_p___m_a_t_c_h       _c_o_l_d_p_)
+            _p_a_r_a_m_e_t_e_r_)                                    * _n_a_m_e___i_d_ 
+          o _(_c_o_l_d_p_._C_O_L_D_P_._f_i_n_d___n_a_m_e___r_e_c_o_r_d_ _p_a_r_a_m_e_t_e_r_)        _(_c_o_l_d_p_._C_O_L_D_P_._i_n_s_e_r_t___s_y_n_o_n_y_m
+          o _(_c_o_l_d_p_._C_O_L_D_P_._f_i_x___b_a_s_i_o_n_y_m_i_d_ _p_a_r_a_m_e_t_e_r_)          _p_a_r_a_m_e_t_e_r_)
+          o _(_c_o_l_d_p_._C_O_L_D_P_._i_d_e_n_t_i_f_y___n_a_m_e_ _p_a_r_a_m_e_t_e_r_)         * _n_a_m_e___r_e_l_a_t_i_o_n_ 
+          o _(_c_o_l_d_p_._C_O_L_D_P_._i_n_i_t_i_a_l_i_s_e___d_a_t_a_f_r_a_m_e               _(_c_o_l_d_p_._C_O_L_D_P_._a_d_d___n_a_m_e___r_e_l_a_t_i_o_n
+            _p_a_r_a_m_e_t_e_r_)                                      _p_a_r_a_m_e_t_e_r_)
+          o _(_c_o_l_d_p_._C_O_L_D_P_._i_n_s_e_r_t___t_a_x_o_n_ _p_a_r_a_m_e_t_e_r_)          * _n_a_m_e_s_ 
+          o _(_c_o_l_d_p_._C_O_L_D_P_._i_s___i_n_f_r_a_s_u_b_s_p_e_c_i_f_i_c                _(_c_o_l_d_p_._C_O_L_D_P_._f_i_x___b_a_s_i_o_n_y_m_s
+            _p_a_r_a_m_e_t_e_r_)                                      _p_a_r_a_m_e_t_e_r_)
+          o _(_c_o_l_d_p_._C_O_L_D_P_._i_s___s_p_e_c_i_e_s___g_r_o_u_p_ _p_a_r_a_m_e_t_e_r_)      * _n_o_r_m_a_l_i_s_e___n_a_m_e_(_)_ 
+          o _(_c_o_l_d_p_._C_O_L_D_P_._r_e_s_e_t___i_d_s_ _p_a_r_a_m_e_t_e_r_)               _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e_ _m_e_t_h_o_d_)
+          o _(_c_o_l_d_p_._C_O_L_D_P_._s_a_v_e_ _p_a_r_a_m_e_t_e_r_)
+          o _(_c_o_l_d_p_._C_O_L_D_P_._s_e_t___b_a_s_i_o_n_y_m_i_d_ _p_a_r_a_m_e_t_e_r_)
+          o _(_c_o_l_d_p_._C_O_L_D_P_._t_a_b_l_e___b_y___n_a_m_e_ _p_a_r_a_m_e_t_e_r_)
+          o _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e_._d_e_r_i_v_e___n_a_m_e_ _p_a_r_a_m_e_t_e_r_)
           o _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e_._n_o_r_m_a_l_i_s_e___n_a_m_e
             _p_a_r_a_m_e_t_e_r_)
 ********** OO **********
     * _o_p_t_i_o_n_s_ _(_c_o_l_d_p_._C_O_L_D_P_._s_e_t___o_p_t_i_o_n_s_ _p_a_r_a_m_e_t_e_r_)
 ********** PP **********
     * _p_a_r_e_n_t_ _(_c_o_l_d_p_._C_O_L_D_P_._a_d_d___n_a_m_e_s_ _p_a_r_a_m_e_t_e_r_)            * _p_r_e_p_a_r_e___b_u_n_d_l_e_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
           o _(_c_o_l_d_p_._C_O_L_D_P_._f_i_x___c_l_a_s_s_i_f_i_c_a_t_i_o_n___r_e_c_u_r_s_i_v_e       _m_e_t_h_o_d_)
             _p_a_r_a_m_e_t_e_r_)                                    * _p_r_o_p_e_r_t_i_e_s_ 
-    * _p_r_e_f_i_x_ _(_c_o_l_d_p_._C_O_L_D_P_._r_e_s_e_t___i_d_s_ _p_a_r_a_m_e_t_e_r_)              _(_c_o_l_d_p_._C_O_L_D_P_._m_o_d_i_f_y___n_a_m_e
-                                                            _p_a_r_a_m_e_t_e_r_)
+    * _p_a_r_e_n_t_I_D_ _(_c_o_l_d_p_._C_O_L_D_P_._i_n_s_e_r_t___t_a_x_o_n_ _p_a_r_a_m_e_t_e_r_)         _(_c_o_l_d_p_._C_O_L_D_P_._f_i_n_d___n_a_m_e_s
+    * _p_r_e_f_i_x_ _(_c_o_l_d_p_._C_O_L_D_P_._r_e_s_e_t___i_d_s_ _p_a_r_a_m_e_t_e_r_)              _p_a_r_a_m_e_t_e_r_)
+                                                                o _(_c_o_l_d_p_._C_O_L_D_P_._m_o_d_i_f_y___n_a_m_e
+                                                                  _p_a_r_a_m_e_t_e_r_)
                                                                 o _(_c_o_l_d_p_._C_O_L_D_P_._m_o_d_i_f_y___t_a_x_o_n
                                                                   _p_a_r_a_m_e_t_e_r_)
 ********** RR **********
-    * _r_a_n_k_s_                                         * _r_e_f_e_r_e_n_c_e_ 
-      _(_c_o_l_d_p_._C_O_L_D_P_._f_i_x___c_l_a_s_s_i_f_i_c_a_t_i_o_n___r_e_c_u_r_s_i_v_e       _(_c_o_l_d_p_._C_O_L_D_P_._f_i_n_d___r_e_f_e_r_e_n_c_e
-      _p_a_r_a_m_e_t_e_r_)                                      _p_a_r_a_m_e_t_e_r_)
-    * _r_e_c_o_r_d_ _(_c_o_l_d_p_._C_O_L_D_P_._v_a_l_i_d_a_t_e___r_e_c_o_r_d           * _r_e_f_e_r_e_n_c_e___l_i_s_t_ 
-      _p_a_r_a_m_e_t_e_r_)                                      _(_c_o_l_d_p_._C_O_L_D_P_._a_d_d___r_e_f_e_r_e_n_c_e_s
-    * _r_e_c_o_r_d___t_y_p_e_ _(_c_o_l_d_p_._C_O_L_D_P_._v_a_l_i_d_a_t_e___r_e_c_o_r_d        _p_a_r_a_m_e_t_e_r_)
-      _p_a_r_a_m_e_t_e_r_)                                    * _r_e_m_o_v_e___g_e_n_d_e_r_(_)_ 
-                                                      _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
+    * _r_a_n_k_ _(_c_o_l_d_p_._C_O_L_D_P_._f_i_n_d___n_a_m_e_ _p_a_r_a_m_e_t_e_r_)        * _r_e_c_o_r_d___t_y_p_e_ 
+          o _(_c_o_l_d_p_._C_O_L_D_P_._f_i_n_d___t_a_x_o_n_ _p_a_r_a_m_e_t_e_r_)        _(_c_o_l_d_p_._C_O_L_D_P_._v_a_l_i_d_a_t_e___r_e_c_o_r_d
+    * _r_a_n_k_s_                                           _p_a_r_a_m_e_t_e_r_)
+      _(_c_o_l_d_p_._C_O_L_D_P_._f_i_x___c_l_a_s_s_i_f_i_c_a_t_i_o_n___r_e_c_u_r_s_i_v_e     * _r_e_f_e_r_e_n_c_e_ 
+      _p_a_r_a_m_e_t_e_r_)                                      _(_c_o_l_d_p_._C_O_L_D_P_._f_i_n_d___r_e_f_e_r_e_n_c_e
+    * _r_e_c_o_r_d_ _(_c_o_l_d_p_._C_O_L_D_P_._v_a_l_i_d_a_t_e___r_e_c_o_r_d             _p_a_r_a_m_e_t_e_r_)
+      _p_a_r_a_m_e_t_e_r_)                                    * _r_e_f_e_r_e_n_c_e___l_i_s_t_ 
+                                                      _(_c_o_l_d_p_._C_O_L_D_P_._a_d_d___r_e_f_e_r_e_n_c_e_s
+                                                      _p_a_r_a_m_e_t_e_r_)
+                                                    * _r_e_m_o_v_e___g_e_n_d_e_r_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
+                                                      _m_e_t_h_o_d_)
                                                     * _r_e_s_e_t___i_d_s_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
                                                       _m_e_t_h_o_d_)
 ********** SS **********
     * _s_                                            * _s_o_r_t___n_a_m_e_s_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
       _(_c_o_l_d_p_._C_O_L_D_P_._c_o_n_s_t_r_u_c_t___s_p_e_c_i_e_s___r_a_n_k___n_a_m_e     * _s_o_r_t___t_a_x_a_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
       _p_a_r_a_m_e_t_e_r_)                                   * _s_o_r_t___t_a_x_a___r_e_c_u_r_s_i_v_e_(_)_ _(_c_o_l_d_p_._C_O_L_D_P
     * _s_a_m_e___b_a_s_i_o_n_y_m_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)           _m_e_t_h_o_d_)
     * _s_a_v_e_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)                  * _s_s_ 
-    * _s_e_t___b_a_s_i_o_n_y_m_i_d_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)          _(_c_o_l_d_p_._C_O_L_D_P_._c_o_n_s_t_r_u_c_t___s_p_e_c_i_e_s___r_a_n_k___n_a_m_e
+    * _s_c_i_e_n_t_i_f_i_c_N_a_m_e_ _(_c_o_l_d_p_._C_O_L_D_P_._f_i_n_d___n_a_m_e          _(_c_o_l_d_p_._C_O_L_D_P_._c_o_n_s_t_r_u_c_t___s_p_e_c_i_e_s___r_a_n_k___n_a_m_e
+      _p_a_r_a_m_e_t_e_r_)                                     _p_a_r_a_m_e_t_e_r_)
+          o _(_c_o_l_d_p_._C_O_L_D_P_._f_i_n_d___t_a_x_o_n_ _p_a_r_a_m_e_t_e_r_)     * _s_t_a_r_t___n_a_m_e___b_u_n_d_l_e_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
+    * _s_e_t___b_a_s_i_o_n_y_m_i_d_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)        * _s_y_n_o_n_y_m_ _(_c_o_l_d_p_._C_O_L_D_P_._a_d_d___s_y_n_o_n_y_m
     * _s_e_t___c_o_n_t_e_x_t_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)             _p_a_r_a_m_e_t_e_r_)
-    * _s_e_t___d_e_f_a_u_l_t___t_a_x_o_n___r_e_c_o_r_d_(_)_ _(_c_o_l_d_p_._C_O_L_D_P      * _s_t_a_r_t___n_a_m_e___b_u_n_d_l_e_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)
-      _m_e_t_h_o_d_)                                      * _s_y_n_o_n_y_m_ _(_c_o_l_d_p_._C_O_L_D_P_._a_d_d___s_y_n_o_n_y_m
-    * _s_e_t___o_p_t_i_o_n_s_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)             _p_a_r_a_m_e_t_e_r_)
-    * _s_g_                                                 o _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e_._a_d_d___s_y_n_o_n_y_m
-      _(_c_o_l_d_p_._C_O_L_D_P_._c_o_n_s_t_r_u_c_t___s_p_e_c_i_e_s___r_a_n_k___n_a_m_e             _p_a_r_a_m_e_t_e_r_)
-      _p_a_r_a_m_e_t_e_r_)                                   * _s_y_n_o_n_y_m___f_r_o_m___n_a_m_e_u_s_a_g_e_ _(_i_n_ _m_o_d_u_l_e_ _c_o_l_d_p_)
-    * _s_i_c_ _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e_ _p_a_r_a_m_e_t_e_r_)             * _s_y_n_o_n_y_m___p_r_e_f_i_x_ 
-          o _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e_._a_d_d___s_y_n_o_n_y_m            _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___t_e_x_t___t_r_e_e_ _p_a_r_a_m_e_t_e_r_)
-            _p_a_r_a_m_e_t_e_r_)                             * _s_y_n_o_n_y_m_s_ _(_c_o_l_d_p_._C_O_L_D_P_._f_i_x___b_a_s_i_o_n_y_m_s
-          o _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e_._n_o_r_m_a_l_i_s_e___n_a_m_e         _p_a_r_a_m_e_t_e_r_)
+    * _s_e_t___d_e_f_a_u_l_t___t_a_x_o_n___r_e_c_o_r_d_(_)_ _(_c_o_l_d_p_._C_O_L_D_P            o _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e_._a_d_d___s_y_n_o_n_y_m
+      _m_e_t_h_o_d_)                                              _p_a_r_a_m_e_t_e_r_)
+    * _s_e_t___o_p_t_i_o_n_s_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)           * _s_y_n_o_n_y_m___f_r_o_m___n_a_m_e_u_s_a_g_e_ _(_i_n_ _m_o_d_u_l_e_ _c_o_l_d_p_)
+    * _s_g_                                           * _s_y_n_o_n_y_m___p_r_e_f_i_x_ 
+      _(_c_o_l_d_p_._C_O_L_D_P_._c_o_n_s_t_r_u_c_t___s_p_e_c_i_e_s___r_a_n_k___n_a_m_e       _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___t_e_x_t___t_r_e_e_ _p_a_r_a_m_e_t_e_r_)
+      _p_a_r_a_m_e_t_e_r_)                                   * _s_y_n_o_n_y_m_s_ _(_c_o_l_d_p_._C_O_L_D_P_._f_i_x___b_a_s_i_o_n_y_m_i_d
+    * _s_i_c_ _(_c_o_l_d_p_._C_O_L_D_P_._s_t_a_r_t___n_a_m_e___b_u_n_d_l_e             _p_a_r_a_m_e_t_e_r_)
+      _p_a_r_a_m_e_t_e_r_)                                         o _(_c_o_l_d_p_._C_O_L_D_P_._f_i_x___b_a_s_i_o_n_y_m_s
+          o _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e_ _p_a_r_a_m_e_t_e_r_)                   _p_a_r_a_m_e_t_e_r_)
+          o _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e_._a_d_d___s_y_n_o_n_y_m
+            _p_a_r_a_m_e_t_e_r_)
+          o _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e_._n_o_r_m_a_l_i_s_e___n_a_m_e
             _p_a_r_a_m_e_t_e_r_)
 ********** TT **********
-    * _t_a_b_l_e___b_y___n_a_m_e_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)          * _t_a_x_o_n_I_D_ 
-    * _t_a_x_a_                                            _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___t_e_x_t___t_r_e_e
-      _(_c_o_l_d_p_._C_O_L_D_P_._f_i_x___c_l_a_s_s_i_f_i_c_a_t_i_o_n___r_e_c_u_r_s_i_v_e       _p_a_r_a_m_e_t_e_r_)
-      _p_a_r_a_m_e_t_e_r_)                                    * _t_y_p_e___m_a_t_e_r_i_a_l_ 
-    * _t_a_x_o_n___f_r_o_m___n_a_m_e_u_s_a_g_e_ _(_i_n_ _m_o_d_u_l_e_ _c_o_l_d_p_)          _(_c_o_l_d_p_._C_O_L_D_P_._a_d_d___t_y_p_e___m_a_t_e_r_i_a_l
-    * _t_a_x_o_n___i_d_ _(_c_o_l_d_p_._C_O_L_D_P_._i_n_s_e_r_t___s_y_n_o_n_y_m            _p_a_r_a_m_e_t_e_r_)
+    * _t_a_b_l_e___b_y___n_a_m_e_(_)_ _(_c_o_l_d_p_._C_O_L_D_P_ _m_e_t_h_o_d_)          * _t_o___d_i_c_t_ _(_c_o_l_d_p_._C_O_L_D_P_._f_i_n_d___n_a_m_e_s
+    * _t_a_x_a_                                            _p_a_r_a_m_e_t_e_r_)
+      _(_c_o_l_d_p_._C_O_L_D_P_._f_i_x___c_l_a_s_s_i_f_i_c_a_t_i_o_n___r_e_c_u_r_s_i_v_e           o _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___c_h_i_l_d_r_e_n
+      _p_a_r_a_m_e_t_e_r_)                                            _p_a_r_a_m_e_t_e_r_)
+    * _t_a_x_o_n___f_r_o_m___n_a_m_e_u_s_a_g_e_ _(_i_n_ _m_o_d_u_l_e_ _c_o_l_d_p_)              o _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___s_y_n_o_n_y_m_s
+    * _t_a_x_o_n___i_d_ _(_c_o_l_d_p_._C_O_L_D_P_._i_n_s_e_r_t___s_y_n_o_n_y_m                  _p_a_r_a_m_e_t_e_r_)
+      _p_a_r_a_m_e_t_e_r_)                                          o _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___s_y_n_o_n_y_m_y
+          o _(_c_o_l_d_p_._C_O_L_D_P_._m_o_d_i_f_y___n_a_m_e_ _p_a_r_a_m_e_t_e_r_)             _p_a_r_a_m_e_t_e_r_)
+          o _(_c_o_l_d_p_._C_O_L_D_P_._m_o_d_i_f_y___t_a_x_o_n               * _t_y_p_e___m_a_t_e_r_i_a_l_ 
+            _p_a_r_a_m_e_t_e_r_)                                _(_c_o_l_d_p_._C_O_L_D_P_._a_d_d___t_y_p_e___m_a_t_e_r_i_a_l
+    * _t_a_x_o_n_I_D_ _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___c_h_i_l_d_r_e_n               _p_a_r_a_m_e_t_e_r_)
       _p_a_r_a_m_e_t_e_r_)
-          o _(_c_o_l_d_p_._C_O_L_D_P_._m_o_d_i_f_y___n_a_m_e_ _p_a_r_a_m_e_t_e_r_)
-          o _(_c_o_l_d_p_._C_O_L_D_P_._m_o_d_i_f_y___t_a_x_o_n
+          o _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___s_y_n_o_n_y_m_s
+            _p_a_r_a_m_e_t_e_r_)
+          o _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___s_y_n_o_n_y_m_y
+            _p_a_r_a_m_e_t_e_r_)
+          o _(_c_o_l_d_p_._C_O_L_D_P_._g_e_t___t_e_x_t___t_r_e_e
             _p_a_r_a_m_e_t_e_r_)
 ********** VV **********
     * _v_a_l_i_d_a_t_e___r_e_c_o_r_d_(_)_ _(_c_o_l_d_p_._C_O_L_D_P     * _v_a_l_u_e_s_ _(_c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e_._d_e_r_i_v_e___n_a_m_e
       _m_e_t_h_o_d_)                              _p_a_r_a_m_e_t_e_r_)
 ********** YY **********
     * _y_ _(_c_o_l_d_p_._C_O_L_D_P_._c_o_n_s_t_r_u_c_t___a_u_t_h_o_r_s_h_i_p_ _p_a_r_a_m_e_t_e_r_)
 ************ _CC_OO_LL_DD_PP ************
 ******** NNaavviiggaattiioonn ********
-Contents:
     * _c_o_l_d_p_._C_O_L_D_P
     * _c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e
+    * _U_s_a_g_e
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
 ©2024, Donald Hobern. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r_ _0_._7_._1_6
```

### Comparing `coldp-2024.5.2/docs/build/html/name-bundle.html` & `coldp-2024.5.3/docs/build/html/name-bundle.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>coldp.NameBundle &#8212; COLDP 2024.5.2 documentation</title>
+    <title>coldp.NameBundle &#8212; COLDP 2024.5.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
-    <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css?v=dd72e65a" />
-    <script src="_static/documentation_options.js?v=1723c9d4"></script>
+    <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
+    <script src="_static/documentation_options.js?v=b35b4dcd"></script>
     <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
+    <link rel="next" title="Usage" href="usage.html" />
     <link rel="prev" title="coldp.COLDP" href="coldp.html" />
    
   <link rel="stylesheet" href="_static/custom.css" type="text/css" />
   
 
   
   
@@ -32,17 +33,17 @@
 
           <div class="body" role="main">
             
   <section id="coldp-namebundle">
 <h1>coldp.NameBundle<a class="headerlink" href="#coldp-namebundle" title="Link to this heading">¶</a></h1>
 <section id="class">
 <h2>Class<a class="headerlink" href="#class" title="Link to this heading">¶</a></h2>
-<dl class="py class">
-<dt class="sig sig-object py">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">coldp.</span></span><span class="sig-name descname"><span class="pre">NameBundle</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">coldp</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">accepted</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">incertae_sedis</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sic</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span></dt>
+<dl class="py method">
+<dt class="sig sig-object py" id="coldp.NameBundle.__init__">
+<span class="sig-prename descclassname"><span class="pre">NameBundle.</span></span><span class="sig-name descname"><span class="pre">__init__</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">coldp</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">accepted</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">incertae_sedis</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sic</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#coldp.NameBundle.__init__" title="Link to this definition">¶</a></dt>
 <dd><p>Wrapper class to manage set of associated names, normally an accepted name
 and one or more synonyms. The bundle handles the logic of associated name
 variations.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="coldp.NameBundle.params.coldp"></span><strong>coldp</strong><a class="paramlink headerlink reference internal" href="#coldp.NameBundle.params.coldp">¶</a> – <code class="xref py py-class docutils literal notranslate"><span class="pre">COLDP</span></code> object to handle logging of any issues and normalise name records</p></li>
@@ -52,15 +53,15 @@
 </ul>
 </dd>
 </dl>
 <p>The minimal usage is to create a new bundle with an accepted name. One
 or more synonyms can also be supplied using the <a class="reference internal" href="#coldp.NameBundle.add_synonym" title="coldp.NameBundle.add_synonym"><code class="xref py py-func docutils literal notranslate"><span class="pre">add_synonym()</span></code></a> method.
 The bundle is then submitted to the <a class="reference internal" href="coldp.html#coldp.COLDP.add_names" title="coldp.COLDP.add_names"><code class="xref py py-func docutils literal notranslate"><span class="pre">coldp.COLDP.add_names()</span></code></a> method for
 processing.</p>
-<p>NameBundle objects should not be created directly. Use the :py:punc`coldp.COLDP.start_name_bundle` method instead.</p>
+<p>NameBundle objects should not be created directly. Use the <a class="reference internal" href="coldp.html#coldp.COLDP.start_name_bundle" title="coldp.COLDP.start_name_bundle"><code class="xref py py-func docutils literal notranslate"><span class="pre">coldp.COLDP.start_name_bundle()</span></code></a> method instead.</p>
 <p>accepted should contain a dictionary with keys that match property names from the <a class="reference external" href="https://github.com/CatalogueOfLife/coldp?tab=readme-ov-file#name">COLDP Name class</a></p>
 </dd></dl>
 
 </section>
 <section id="methods">
 <h2>Methods<a class="headerlink" href="#methods" title="Link to this heading">¶</a></h2>
 <dl class="py method">
@@ -135,30 +136,33 @@
 
 
 
 
 
 
 <h3>Navigation</h3>
-<p class="caption" role="heading"><span class="caption-text">Contents:</span></p>
 <ul class="current">
 <li class="toctree-l1"><a class="reference internal" href="coldp.html">coldp.COLDP</a></li>
 <li class="toctree-l1 current"><a class="current reference internal" href="#">coldp.NameBundle</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="#class">Class</a></li>
 <li class="toctree-l2"><a class="reference internal" href="#methods">Methods</a></li>
 <li class="toctree-l2"><a class="reference internal" href="#index-and-search">Index and search</a></li>
 </ul>
 </li>
 </ul>
+<ul>
+<li class="toctree-l1"><a class="reference internal" href="usage.html">Usage</a></li>
+</ul>
 
 <div class="relations">
 <h3>Related Topics</h3>
 <ul>
   <li><a href="index.html">Documentation overview</a><ul>
       <li>Previous: <a href="coldp.html" title="previous chapter">coldp.COLDP</a></li>
+      <li>Next: <a href="usage.html" title="next chapter">Usage</a></li>
   </ul></li>
 </ul>
 </div>
 <search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="search.html" method="get">
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 ************ ccoollddpp..NNaammeeBBuunnddllee_?¶ ************
 ********** CCllaassss_?¶ **********
-  ccllaassss coldp.NameBundle(ccoollddpp, aacccceepptteedd, iinncceerrttaaee__sseeddiiss==FFaallssee, ssiicc==FFaallssee)
+  NameBundle.__init__(ccoollddpp, aacccceepptteedd, iinncceerrttaaee__sseeddiiss==FFaallssee, ssiicc==FFaallssee)_¶
       Wrapper class to manage set of associated names, normally an accepted
       name and one or more synonyms. The bundle handles the logic of associated
       name variations.
         Parameters:
                 * ccoollddpp_¶ – COLDP object to handle logging of any issues and
                   normalise name records
                 * aacccceepptteedd_¶ – Dictionary mapping COLDP name elements to values
@@ -14,16 +14,16 @@
                   record should be marked “incertae sedis”
                 * ssiicc_¶ – Flag to indicate if the accepted name should be
                   processed without reporting issues for invalid format
       The minimal usage is to create a new bundle with an accepted name. One or
       more synonyms can also be supplied using the _a_d_d___s_y_n_o_n_y_m_(_) method. The
       bundle is then submitted to the _c_o_l_d_p_._C_O_L_D_P_._a_d_d___n_a_m_e_s_(_) method for
       processing.
-      NameBundle objects should not be created directly. Use the :py:
-      punc`coldp.COLDP.start_name_bundle` method instead.
+      NameBundle objects should not be created directly. Use the
+      _c_o_l_d_p_._C_O_L_D_P_._s_t_a_r_t___n_a_m_e___b_u_n_d_l_e_(_) method instead.
       accepted should contain a dictionary with keys that match property names
       from the _C_O_L_D_P_ _N_a_m_e_ _c_l_a_s_s
 ********** MMeetthhooddss_?¶ **********
   NameBundle.add_synonym(ssyynnoonnyymm, ssiicc==FFaallssee)_¶
       Register an additional name as a synonym for the accepted name
       synonym should contain a dictionary with keys that match property names
       from the _C_O_L_D_P_ _N_a_m_e_ _c_l_a_s_s
@@ -54,20 +54,21 @@
         Returns:
             Name dictionary with supplied values supplemented from name
 ********** IInnddeexx aanndd sseeaarrcchh_?¶ **********
     * _I_n_d_e_x
     * _S_e_a_r_c_h_ _P_a_g_e
 ************ _CC_OO_LL_DD_PP ************
 ******** NNaavviiggaattiioonn ********
-Contents:
     * _c_o_l_d_p_._C_O_L_D_P
     * _c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e
           o _C_l_a_s_s
           o _M_e_t_h_o_d_s
           o _I_n_d_e_x_ _a_n_d_ _s_e_a_r_c_h
+    * _U_s_a_g_e
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
           o Previous: _c_o_l_d_p_._C_O_L_D_P
+          o Next: _U_s_a_g_e
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
 ©2024, Donald Hobern. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r_ _0_._7_._1_6 | _P_a_g_e
 _s_o_u_r_c_e
```

### Comparing `coldp-2024.5.2/docs/build/html/search.html` & `coldp-2024.5.3/docs/build/html/search.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Search &#8212; COLDP 2024.5.2 documentation</title>
+    <title>Search &#8212; COLDP 2024.5.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
-    <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css?v=dd72e65a" />
+    <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     
-    <script src="_static/documentation_options.js?v=1723c9d4"></script>
+    <script src="_static/documentation_options.js?v=b35b4dcd"></script>
     <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <script src="_static/searchtools.js"></script>
     <script src="_static/language_data.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="#" />
     <script src="searchindex.js" defer="defer"></script>
@@ -77,19 +77,21 @@
 
 
 
 
 
 
 <h3>Navigation</h3>
-<p class="caption" role="heading"><span class="caption-text">Contents:</span></p>
 <ul>
 <li class="toctree-l1"><a class="reference internal" href="coldp.html">coldp.COLDP</a></li>
 <li class="toctree-l1"><a class="reference internal" href="name-bundle.html">coldp.NameBundle</a></li>
 </ul>
+<ul>
+<li class="toctree-l1"><a class="reference internal" href="usage.html">Usage</a></li>
+</ul>
 
 <div class="relations">
 <h3>Related Topics</h3>
 <ul>
   <li><a href="index.html">Documentation overview</a><ul>
   </ul></li>
 </ul>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 ************ SSeeaarrcchh ************
 Please activate JavaScript to enable the search functionality.
 Searching for multiple words only shows matches that contain all words.
 [q                   ][search]
 ************ _CC_OO_LL_DD_PP ************
 ******** NNaavviiggaattiioonn ********
-Contents:
     * _c_o_l_d_p_._C_O_L_D_P
     * _c_o_l_d_p_._N_a_m_e_B_u_n_d_l_e
+    * _U_s_a_g_e
 ******** RReellaatteedd TTooppiiccss ********
     * _D_o_c_u_m_e_n_t_a_t_i_o_n_ _o_v_e_r_v_i_e_w
 ©2024, Donald Hobern. | Powered by _S_p_h_i_n_x_ _7_._3_._7 & _A_l_a_b_a_s_t_e_r_ _0_._7_._1_6
```

### Comparing `coldp-2024.5.2/docs/build/html/searchindex.js` & `coldp-2024.5.3/docs/build/html/searchindex.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -2,78 +2,94 @@
     "alltitles": {
         "Access to DataFrames": [
             [0, "access-to-dataframes"]
         ],
         "Add or modify records": [
             [0, "add-or-modify-records"]
         ],
-        "COLDP": [
-            [1, "coldp"]
-        ],
         "Class": [
             [0, "class"],
             [2, "class"]
         ],
+        "Classes": [
+            [1, "classes"]
+        ],
         "Constants": [
             [0, "constants"]
         ],
-        "Contents:": [
-            [1, null]
-        ],
         "Control behaviour": [
             [0, "control-behaviour"]
         ],
         "Find or get records": [
             [0, "find-or-get-records"]
         ],
         "Index and search": [
             [0, "index-and-search"],
             [1, "index-and-search"],
             [2, "index-and-search"]
         ],
+        "Installation": [
+            [1, "installation"]
+        ],
         "Internal methods": [
             [0, "internal-methods"]
         ],
         "Methods": [
             [0, "methods"],
             [2, "methods"]
         ],
+        "Overview": [
+            [1, "overview"]
+        ],
         "Save": [
             [0, "save"]
         ],
         "Tidy package": [
             [0, "tidy-package"]
         ],
+        "Usage": [
+            [1, "usage"],
+            [3, "usage"]
+        ],
         "Utilities": [
             [0, "utilities"]
         ],
+        "coldp": [
+            [1, "coldp"]
+        ],
         "coldp.COLDP": [
             [0, "coldp-coldp"]
         ],
         "coldp.NameBundle": [
             [2, "coldp-namebundle"]
         ]
     },
-    "docnames": ["coldp", "index", "name-bundle"],
+    "docnames": ["coldp", "index", "name-bundle", "usage"],
     "envversion": {
         "sphinx": 61,
         "sphinx.domains.c": 3,
         "sphinx.domains.changeset": 1,
         "sphinx.domains.citation": 1,
         "sphinx.domains.cpp": 9,
         "sphinx.domains.index": 1,
         "sphinx.domains.javascript": 3,
         "sphinx.domains.math": 2,
         "sphinx.domains.python": 4,
         "sphinx.domains.rst": 2,
         "sphinx.domains.std": 2,
         "sphinx.ext.intersphinx": 1
     },
-    "filenames": ["coldp.rst", "index.rst", "name-bundle.rst"],
+    "filenames": ["coldp.rst", "index.rst", "name-bundle.rst", "usage.rst"],
     "indexentries": {
+        "__init__() (coldp.coldp method)": [
+            [0, "coldp.COLDP.__init__", false]
+        ],
+        "__init__() (coldp.namebundle method)": [
+            [2, "coldp.NameBundle.__init__", false]
+        ],
         "add_distribution() (coldp.coldp method)": [
             [0, "coldp.COLDP.add_distribution", false]
         ],
         "add_name_relation() (coldp.coldp method)": [
             [0, "coldp.COLDP.add_name_relation", false]
         ],
         "add_names() (coldp.coldp method)": [
@@ -108,14 +124,17 @@
         ],
         "epithet_and_authorship_match() (coldp.coldp method)": [
             [0, "coldp.COLDP.epithet_and_authorship_match", false]
         ],
         "extract_table() (coldp.coldp method)": [
             [0, "coldp.COLDP.extract_table", false]
         ],
+        "find_distribution() (coldp.coldp method)": [
+            [0, "coldp.COLDP.find_distribution", false]
+        ],
         "find_name() (coldp.coldp method)": [
             [0, "coldp.COLDP.find_name", false]
         ],
         "find_name_record() (coldp.coldp method)": [
             [0, "coldp.COLDP.find_name_record", false]
         ],
         "find_names() (coldp.coldp method)": [
@@ -256,25 +275,27 @@
             [0, 2, 1, "", "csv_extensions"],
             [0, 2, 1, "", "id_mappings"],
             [0, 2, 1, "", "name_from_nameusage"],
             [0, 2, 1, "", "synonym_from_nameusage"],
             [0, 2, 1, "", "taxon_from_nameusage"]
         ],
         "coldp.COLDP": [
+            [0, 0, 1, "", "__init__"],
             [0, 0, 1, "", "add_distribution"],
             [0, 0, 1, "", "add_name_relation"],
             [0, 0, 1, "", "add_names"],
             [0, 0, 1, "", "add_references"],
             [0, 0, 1, "", "add_species_interaction"],
             [0, 0, 1, "", "add_synonym"],
             [0, 0, 1, "", "add_type_material"],
             [0, 0, 1, "", "construct_authorship"],
             [0, 0, 1, "", "construct_species_rank_name"],
             [0, 0, 1, "", "epithet_and_authorship_match"],
             [0, 0, 1, "", "extract_table"],
+            [0, 0, 1, "", "find_distribution"],
             [0, 0, 1, "", "find_name"],
             [0, 0, 1, "", "find_name_record"],
             [0, 0, 1, "", "find_names"],
             [0, 0, 1, "", "find_reference"],
             [0, 0, 1, "", "find_taxon"],
             [0, 0, 1, "", "fix_basionymid"],
             [0, 0, 1, "", "fix_basionyms"],
@@ -343,40 +364,84 @@
         "coldp.COLDP.construct_species_rank_name.params": [
             [0, 1, 1, "", "g"],
             [0, 1, 1, "", "marker"],
             [0, 1, 1, "", "s"],
             [0, 1, 1, "", "sg"],
             [0, 1, 1, "", "ss"]
         ],
+        "coldp.COLDP.epithet_and_authorship_match.params": [
+            [0, 1, 1, "", "authorship"],
+            [0, 1, 1, "", "epithet"],
+            [0, 1, 1, "", "name"]
+        ],
         "coldp.COLDP.extract_table.params": [
             [0, 1, 1, "", "df"],
             [0, 1, 1, "", "headings"],
             [0, 1, 1, "", "mappings"]
         ],
+        "coldp.COLDP.find_distribution.params": [
+            [0, 1, 1, "", "distribution"]
+        ],
+        "coldp.COLDP.find_name.params": [
+            [0, 1, 1, "", "authorship"],
+            [0, 1, 1, "", "rank"],
+            [0, 1, 1, "", "scientificName"]
+        ],
         "coldp.COLDP.find_name_record.params": [
             [0, 1, 1, "", "name"]
         ],
+        "coldp.COLDP.find_names.params": [
+            [0, 1, 1, "", "properties"],
+            [0, 1, 1, "", "to_dict"]
+        ],
         "coldp.COLDP.find_reference.params": [
             [0, 1, 1, "", "reference"]
         ],
+        "coldp.COLDP.find_taxon.params": [
+            [0, 1, 1, "", "authorship"],
+            [0, 1, 1, "", "rank"],
+            [0, 1, 1, "", "scientificName"]
+        ],
+        "coldp.COLDP.fix_basionymid.params": [
+            [0, 1, 1, "", "name"],
+            [0, 1, 1, "", "synonyms"]
+        ],
         "coldp.COLDP.fix_basionyms.params": [
             [0, 1, 1, "", "names"],
             [0, 1, 1, "", "synonyms"]
         ],
         "coldp.COLDP.fix_classification_recursive.params": [
             [0, 1, 1, "", "parent"],
             [0, 1, 1, "", "ranks"],
             [0, 1, 1, "", "taxa"]
         ],
+        "coldp.COLDP.get_children.params": [
+            [0, 1, 1, "", "taxonID"],
+            [0, 1, 1, "", "to_dict"]
+        ],
+        "coldp.COLDP.get_name.params": [
+            [0, 1, 1, "", "id"]
+        ],
         "coldp.COLDP.get_original_authorship.params": [
             [0, 1, 1, "", "authorship"]
         ],
         "coldp.COLDP.get_reference.params": [
             [0, 1, 1, "", "id"]
         ],
+        "coldp.COLDP.get_synonyms.params": [
+            [0, 1, 1, "", "taxonID"],
+            [0, 1, 1, "", "to_dict"]
+        ],
+        "coldp.COLDP.get_synonymy.params": [
+            [0, 1, 1, "", "taxonID"],
+            [0, 1, 1, "", "to_dict"]
+        ],
+        "coldp.COLDP.get_taxon.params": [
+            [0, 1, 1, "", "id"]
+        ],
         "coldp.COLDP.get_text_tree.params": [
             [0, 1, 1, "", "indent"],
             [0, 1, 1, "", "initial_prefix"],
             [0, 1, 1, "", "synonym_prefix"],
             [0, 1, 1, "", "taxonID"]
         ],
         "coldp.COLDP.identify_name.params": [
@@ -387,20 +452,27 @@
             [0, 1, 1, "", "foldername"],
             [0, 1, 1, "", "name"]
         ],
         "coldp.COLDP.insert_synonym.params": [
             [0, 1, 1, "", "name_id"],
             [0, 1, 1, "", "taxon_id"]
         ],
+        "coldp.COLDP.insert_taxon.params": [
+            [0, 1, 1, "", "name"],
+            [0, 1, 1, "", "parentID"]
+        ],
         "coldp.COLDP.is_infrasubspecific.params": [
             [0, 1, 1, "", "name"]
         ],
         "coldp.COLDP.is_species_group.params": [
             [0, 1, 1, "", "name"]
         ],
+        "coldp.COLDP.issue.params": [
+            [0, 1, 1, "", "message"]
+        ],
         "coldp.COLDP.modify_name.params": [
             [0, 1, 1, "", "properties"],
             [0, 1, 1, "", "taxon_id"]
         ],
         "coldp.COLDP.modify_taxon.params": [
             [0, 1, 1, "", "properties"],
             [0, 1, 1, "", "taxon_id"]
@@ -430,14 +502,18 @@
             [0, 1, 1, "", "name"],
             [0, 1, 1, "", "prefix"]
         ],
         "coldp.COLDP.same_basionym.params": [
             [0, 1, 1, "", "a"],
             [0, 1, 1, "", "b"]
         ],
+        "coldp.COLDP.save.params": [
+            [0, 1, 1, "", "destination"],
+            [0, 1, 1, "", "name"]
+        ],
         "coldp.COLDP.set_basionymid.params": [
             [0, 1, 1, "", "basionymid"],
             [0, 1, 1, "", "name"]
         ],
         "coldp.COLDP.set_context.params": [
             [0, 1, 1, "", "context"]
         ],
@@ -448,22 +524,28 @@
             [0, 1, 1, "", "options"]
         ],
         "coldp.COLDP.sort_taxa_recursive.params": [
             [0, 1, 1, "", "df"],
             [0, 1, 1, "", "id"],
             [0, 1, 1, "", "ids"]
         ],
+        "coldp.COLDP.start_name_bundle.params": [
+            [0, 1, 1, "", "accepted"],
+            [0, 1, 1, "", "incertae_sedis"],
+            [0, 1, 1, "", "sic"]
+        ],
         "coldp.COLDP.table_by_name.params": [
             [0, 1, 1, "", "name"]
         ],
         "coldp.COLDP.validate_record.params": [
             [0, 1, 1, "", "record"],
             [0, 1, 1, "", "record_type"]
         ],
         "coldp.NameBundle": [
+            [2, 0, 1, "", "__init__"],
             [2, 0, 1, "", "add_synonym"],
             [2, 0, 1, "", "derive_name"],
             [2, 0, 1, "", "normalise_name"]
         ],
         "coldp.NameBundle.add_synonym.params": [
             [2, 1, 1, "", "sic"],
             [2, 1, 1, "", "synonym"]
@@ -492,589 +574,775 @@
         "0": "py:method",
         "1": "py:parameter",
         "2": "py:data"
     },
     "terms": {
         "": 0,
         "1": 0,
+        "10": 3,
+        "1111": 3,
+        "115": 3,
+        "12129": 3,
+        "127": 3,
+        "147": 3,
+        "150": 3,
+        "153": 3,
         "1831": 0,
         "1832": 0,
         "1838": 0,
-        "2": 0,
-        "A": 0,
+        "1923": 3,
+        "1978": 3,
+        "2": [0, 3],
+        "2014": 3,
+        "2015": 3,
+        "2019": 3,
+        "25077087": 3,
+        "27259": 3,
+        "3897": 3,
+        "4": 3,
+        "40": 3,
+        "463": 3,
+        "49": 3,
+        "505": 3,
+        "54": 3,
+        "56100973": 3,
+        "671": 3,
+        "697": 3,
+        "704": 3,
+        "819": 3,
+        "A": [0, 1, 3],
+        "At": 1,
         "For": 0,
         "If": 0,
-        "In": 0,
-        "It": 0,
+        "In": [0, 3],
+        "It": [0, 3],
         "One": [0, 2],
-        "The": [0, 2],
+        "The": [0, 1, 2, 3],
         "Then": 0,
+        "These": 0,
+        "__init__": [0, 2],
         "_sphinx_paramlinks_coldp": 0,
-        "ab": 0,
+        "ab": [0, 3],
         "absent": 0,
-        "accept": [0, 2],
-        "accepted_taxon_id": 0,
-        "ad": [0, 2],
-        "add_distribut": 0,
-        "add_nam": [0, 2],
+        "accept": [0, 1, 2, 3],
+        "accepted_taxon_id": [0, 3],
+        "ad": [0, 1, 2, 3],
+        "add": [1, 3],
+        "add_distribut": [0, 3],
+        "add_nam": [0, 1, 2, 3],
         "add_name_rel": 0,
-        "add_refer": 0,
+        "add_refer": [0, 3],
         "add_species_interact": 0,
-        "add_synonym": [0, 2],
+        "add_synonym": [0, 2, 3],
         "add_type_materi": 0,
         "add_typemateri": 0,
-        "addit": [0, 2],
+        "addit": [0, 1, 2, 3],
         "after": 0,
-        "all": [0, 2],
+        "all": [0, 1, 2, 3],
         "allow": 0,
         "allow_repeated_binomi": 0,
         "along": 0,
         "alphabet": 0,
-        "alreadi": 0,
+        "alreadi": [0, 3],
         "also": [0, 2],
         "alter": 0,
-        "altern": 0,
+        "altern": [0, 1],
+        "american": 3,
         "among": 0,
-        "an": [0, 2],
+        "an": [0, 1, 2, 3],
         "ancestri": 0,
-        "ani": [0, 2],
+        "ani": [0, 1, 2],
+        "animalia": 3,
         "annot": 0,
-        "anoth": 0,
+        "anoth": [0, 1],
         "appear": 0,
         "append": 0,
         "applic": 0,
         "appropri": [0, 2],
-        "ar": 0,
+        "ar": [0, 1, 3],
+        "area": [0, 3],
         "argument": 0,
         "around": 0,
+        "arthropoda": 3,
         "assist": 0,
-        "associ": [0, 2],
+        "associ": [0, 1, 2, 3],
         "asterisk": 0,
         "atom": 0,
-        "author": 0,
-        "authorship": 0,
-        "automat": 0,
-        "b": 0,
+        "author": [0, 3],
+        "authorship": [0, 3],
+        "automat": [0, 1],
+        "b": [0, 3],
         "back": 0,
         "base": [0, 2],
-        "basic": 0,
+        "basic": [0, 3],
         "basionym": 0,
-        "basionymid": 0,
+        "basionymid": [0, 1, 3],
         "basionyms_from_synonym": 0,
         "basionyn": 0,
+        "bc": 3,
         "becom": 0,
         "been": 0,
         "befor": 0,
         "being": 0,
         "below": 0,
         "between": 0,
         "binomi": 0,
+        "biodiversitylibrari": 3,
+        "bodi": 0,
         "boolean": 0,
-        "both": 0,
-        "bundl": [0, 2],
+        "both": [0, 3],
+        "braun": 3,
+        "braun_1923": 3,
+        "bring": 1,
+        "bundl": [0, 2, 3],
+        "c": 3,
+        "ca": 3,
         "call": 0,
-        "can": [0, 2],
+        "can": [0, 1, 2],
+        "canada": 3,
+        "canon": 0,
         "case": 0,
-        "catalogu": 0,
+        "catalogu": [0, 1],
         "chang": 0,
         "check": 0,
-        "child": 0,
+        "checklist": 1,
+        "child": [0, 3],
         "children": 0,
         "citat": 0,
-        "class": 1,
-        "classif": 0,
+        "class": 3,
+        "classif": [0, 3],
         "classification_from_par": 0,
-        "code": [0, 2],
+        "code": [0, 2, 3],
+        "col": 1,
+        "coldp": 3,
         "column": 0,
-        "combin": 0,
+        "combin": [0, 1, 3],
         "comma": 0,
+        "compar": 3,
+        "comparison": 0,
         "complet": 0,
-        "compliant": [0, 2],
+        "compliant": [0, 1, 2],
         "compon": 0,
         "compos": 0,
         "concept": 0,
         "consecut": 0,
         "consist": 0,
         "constant": 1,
         "construct": 0,
         "construct_authorship": 0,
         "construct_species_rank_nam": 0,
-        "contain": [0, 2],
-        "containertitl": 0,
-        "content": 0,
+        "constructor": 0,
+        "contain": [0, 1, 2],
+        "containertitl": [0, 3],
+        "content": [0, 1, 3],
         "context": 0,
         "continu": 0,
         "conveni": 0,
+        "convert": 0,
         "copi": [0, 2],
         "correct": 0,
         "correctli": 0,
         "correspond": 0,
-        "creat": [0, 2],
+        "creat": [0, 1, 2, 3],
         "create_subspecies_for_infrasubspecif": 0,
         "create_synonyms_without_subgenu": 0,
         "create_taxa_for_not_establish": 0,
+        "creation": 1,
         "cross": 0,
-        "csv": 0,
+        "csv": [0, 1],
         "csv_extens": 0,
-        "current": 0,
-        "data": 0,
+        "cum": 3,
+        "curent": 3,
+        "current": [0, 3],
+        "d": 3,
+        "data": [0, 1, 3],
         "databas": 0,
+        "datafram": [1, 3],
         "dataset": 0,
-        "default": 0,
+        "davi": 3,
+        "davis_1978": 3,
+        "default": [0, 3],
         "default_head": 0,
-        "default_taxon_record": 0,
-        "delimit": 0,
+        "default_taxon_record": [0, 3],
+        "delimit": [0, 1],
         "depend": 0,
         "derive_nam": 2,
         "descend": 0,
         "destin": 0,
+        "dewaard": 3,
         "df": 0,
-        "dictionari": [0, 2],
+        "dictionari": [0, 1, 2],
         "differ": 0,
         "directli": 2,
-        "distribut": 0,
+        "displai": 3,
+        "distribut": [0, 3],
         "doe": [0, 2],
+        "doi": 3,
+        "drop": 0,
         "e": 0,
-        "each": 0,
+        "each": [0, 3],
         "easi": 0,
+        "edit": 1,
         "editor": 0,
         "either": 0,
-        "element": [0, 2],
+        "element": [0, 2, 3],
         "els": 0,
-        "empti": 0,
+        "empti": [0, 1],
+        "enabl": 3,
         "enclos": 0,
         "end": 0,
         "ensur": [0, 2],
+        "entomolog": 3,
+        "entomologi": 3,
+        "entomologist": 3,
         "epithet": 0,
         "epithet_and_authorship_match": 0,
         "equal": 0,
         "error": 0,
-        "establish": 0,
+        "establish": [0, 3],
         "etc": 0,
         "even": 0,
+        "evolut": 3,
         "exactli": 0,
-        "exampl": 0,
+        "exampl": [0, 3],
         "execut": 0,
-        "exist": [0, 2],
+        "exist": [0, 1, 2, 3],
+        "expand": 1,
         "expect": [0, 2],
+        "export": 0,
+        "extant": 3,
         "extens": 0,
         "extern": 0,
         "extra": [0, 2],
         "extract": 0,
         "extract_t": 0,
-        "f": 0,
+        "f": [0, 3],
+        "facilit": 1,
+        "fail": 0,
         "fals": [0, 2],
-        "famili": 0,
+        "famili": [0, 3],
+        "family_id": 3,
         "field": 0,
-        "file": 0,
+        "file": [0, 1],
         "fill": 0,
+        "filter": 0,
+        "final": 3,
+        "find_distribut": 0,
         "find_nam": 0,
         "find_name_record": 0,
         "find_refer": 0,
         "find_taxon": 0,
         "first": 0,
         "fix": 0,
         "fix_basionym": 0,
         "fix_basionymid": 0,
         "fix_classif": 0,
         "fix_classification_recurs": 0,
         "flag": [0, 2],
-        "folder": 0,
+        "folder": [0, 1, 3],
         "foldernam": 0,
-        "follow": [0, 2],
+        "follow": [0, 2, 3],
         "foreign": 0,
         "forign": 0,
         "form": 0,
-        "format": [0, 2],
+        "format": [0, 1, 2, 3],
         "forward": 0,
         "found": 0,
-        "four": 0,
+        "four": [0, 3],
         "frame": 0,
         "free": 0,
-        "from": [0, 2],
-        "g": 0,
+        "from": [0, 1, 2, 3],
+        "fuscoleuca": 3,
+        "g": [0, 3],
+        "gazett": [0, 3],
         "gender": 0,
-        "gener": 0,
-        "genu": 0,
+        "gener": [0, 3],
+        "genera": 3,
+        "genu": [0, 3],
+        "genus_id": 3,
+        "get": 3,
         "get_children": 0,
         "get_nam": 0,
         "get_original_authorship": 0,
         "get_refer": 0,
         "get_synonym": 0,
         "get_synonymi": 0,
         "get_taxon": 0,
-        "get_text_tre": 0,
+        "get_text_tre": [0, 3],
         "given": 0,
         "greek": 0,
         "group": 0,
         "guarante": 0,
         "ha": 0,
         "handl": [0, 2],
+        "harrison": 3,
         "head": 0,
+        "helper": 1,
         "hierarch": 0,
         "hierarchi": 0,
         "higher": 0,
         "highest": 0,
-        "hold": 0,
+        "histori": 3,
+        "hold": [0, 1],
         "housekeep": 0,
-        "i": [0, 2],
+        "http": 3,
+        "i": [0, 1, 2, 3],
         "icbn": 0,
         "iczn": 0,
-        "id": 0,
+        "id": [0, 3],
         "id_map": 0,
         "ident": 0,
-        "identifi": 0,
+        "identifi": [0, 1],
         "identify_nam": 0,
+        "ignor": 0,
+        "illustr": 3,
         "immedi": 0,
         "impli": 0,
-        "import": 0,
-        "incerta": 2,
+        "implic": 3,
+        "implicit": 1,
+        "import": [0, 3],
+        "incerta": [0, 2],
         "incertae_sedi": [0, 2],
-        "includ": 0,
+        "includ": [0, 1, 3],
+        "incurvariida": 3,
+        "incurvariin": 3,
         "inde": 0,
         "indent": 0,
         "indic": [0, 2],
         "infer": 0,
         "infraspecif": 0,
         "infrasubspecif": 0,
         "initalis": 0,
         "initial_prefix": 0,
-        "initialis": 0,
+        "initialis": [0, 1],
         "initialise_datafram": 0,
+        "insecta": 3,
         "insensit": 0,
-        "insert": 0,
+        "insert": [0, 1],
         "insert_species_for_trinomi": 0,
         "insert_synonym": 0,
         "insert_taxon": 0,
         "insid": 0,
-        "instanc": 0,
+        "instanc": [0, 1, 3],
+        "instanti": 1,
         "instead": [0, 2],
         "integ": 0,
         "intend": 0,
         "interact": 0,
         "intern": 1,
         "invalid": 2,
         "is_basionym": 0,
         "is_infrasubspecif": 0,
         "is_species_group": 0,
-        "issu": [0, 2],
+        "iso": 3,
+        "issu": [0, 2, 3],
         "issues_to_stdout": 0,
         "ital": 0,
-        "its": 0,
+        "item": 3,
+        "its": [0, 1],
+        "j": 3,
+        "jstor": 3,
         "just": 0,
+        "k": 3,
         "kei": [0, 2],
         "keyword": 0,
-        "kingdom": 0,
+        "kingdom": [0, 3],
+        "l": 3,
         "label": 0,
         "lack": 0,
+        "lampronia": 3,
+        "landri": 3,
+        "latest": 1,
         "latin": 0,
         "least": 0,
+        "leav": 3,
+        "lepidoptera": 3,
         "level": 0,
-        "life": 0,
+        "life": [0, 1, 3],
         "like": 0,
+        "lineag": 3,
+        "link": 3,
         "list": 0,
-        "load": 0,
-        "locat": 0,
+        "load": [0, 1, 3],
+        "locat": [0, 3],
         "log": [0, 2],
         "logic": 2,
         "lower": 0,
         "lowest": 0,
-        "mai": 0,
+        "m": 3,
+        "made": 0,
+        "mai": [0, 1],
+        "main": 1,
         "major": 0,
-        "manag": [0, 2],
+        "manag": [0, 1, 2, 3],
+        "mani": 1,
+        "manipul": 1,
         "map": [0, 2],
         "mark": 2,
         "marker": 0,
         "match": [0, 2],
         "mechan": 0,
+        "memori": 1,
         "messag": 0,
         "method": 1,
+        "microlepidoptera": 3,
         "minim": 2,
-        "miss": 2,
+        "minimum": 1,
+        "miss": [0, 2],
+        "mitter": 3,
+        "mixtur": 3,
         "modify_nam": 0,
         "modify_taxon": 0,
+        "molecular": 3,
+        "monotyp": 3,
         "more": [0, 2],
+        "morphologi": 3,
         "most": 0,
+        "moth": 3,
+        "move": 0,
         "multilin": 0,
         "multipl": 0,
         "must": 0,
-        "name": [0, 2],
+        "name": [0, 1, 2, 3],
         "name_from_nameusag": 0,
         "name_id": 0,
         "name_rel": 0,
         "nameand": 0,
-        "namebundl": [0, 1],
+        "namebundl": [0, 1, 3],
         "nameid": 0,
-        "namerel": 0,
+        "namerel": [0, 3],
         "nameusag": 0,
+        "nan": 0,
+        "nativ": 3,
         "necessari": [0, 2],
         "need": 0,
         "nest": 0,
-        "new": [0, 2],
+        "new": [0, 1, 2, 3],
         "next": 0,
         "node": 0,
         "nomenclatur": 0,
+        "nonditrysian": 3,
         "none": 0,
-        "normal": [0, 2],
+        "normal": [0, 1, 2],
         "normalis": [0, 2],
         "normalise_nam": 2,
+        "north": 3,
+        "note": 3,
         "number": 0,
+        "numpi": 0,
         "o": 0,
-        "object": [0, 2],
+        "object": [0, 1, 2, 3],
         "occur": 0,
         "often": 0,
+        "oldest": 3,
         "omit": 0,
-        "onc": 0,
-        "one": [0, 2],
-        "onli": 0,
-        "option": 0,
-        "order": 0,
-        "origin": 0,
-        "other": 0,
+        "onc": [0, 1],
+        "one": [0, 1, 2],
+        "onli": [0, 3],
+        "option": [0, 1],
+        "order": [0, 3],
+        "org": 3,
+        "organis": 1,
+        "origin": [0, 3],
+        "other": [0, 1, 3],
         "otherwis": 0,
         "output": 0,
         "over": 0,
         "overrid": 2,
         "own": 0,
-        "packag": 2,
-        "page": [0, 1, 2],
-        "panda": 0,
+        "p": 3,
+        "pacif": 3,
+        "packag": [1, 2],
+        "page": [0, 1, 2, 3],
+        "pan": 3,
+        "panda": [0, 1],
         "param": 0,
         "paramet": [0, 2],
         "parent": 0,
         "parenthensi": 0,
         "parenthes": 0,
+        "parenthood": 0,
         "parentid": 0,
+        "pars": 3,
         "part": 0,
         "pass": 0,
         "path": 0,
+        "pattern": 3,
         "per": 0,
-        "phylum": 0,
+        "phylogeni": 3,
+        "phylum": [0, 3],
+        "pip": 1,
+        "pohl": 3,
+        "pohl_et_al_2019": 3,
         "point": 0,
         "posit": 0,
         "possibl": 0,
         "potenti": 0,
         "prece": 0,
         "preced": 0,
         "prefer": 0,
         "prefix": 0,
         "prepar": 0,
         "prepare_bundl": 0,
         "prepend": 0,
         "present": 0,
         "preserv": 0,
         "previou": 0,
-        "print": 0,
+        "print": [0, 3],
         "problem": 0,
         "process": [0, 2],
         "produc": 0,
-        "properti": [0, 2],
-        "provid": 0,
+        "properli": 0,
+        "properti": [0, 2, 3],
+        "provid": [0, 3],
         "public": 0,
-        "punc": 2,
-        "py": 2,
+        "publishedinpag": 3,
+        "publishedinyear": 3,
+        "py": 1,
+        "pypi": 1,
+        "python": 1,
+        "queri": 1,
         "question": 0,
-        "rank": 0,
+        "r": 3,
+        "rank": [0, 3],
         "read": 0,
+        "recent": 0,
         "recognis": 0,
-        "record": 2,
+        "record": [1, 2, 3],
         "record_typ": 0,
         "recurs": 0,
-        "refer": 0,
+        "refer": [0, 3],
         "referenc": 0,
         "reference_head": 0,
         "reference_list": 0,
-        "referenceid": 0,
+        "referenceid": [0, 3],
+        "regier": 3,
+        "regier_et_al_2014": 3,
         "regist": [0, 2],
         "reject": 0,
         "relatednameid": 0,
-        "relationship": 0,
-        "relev": 0,
+        "relationship": [0, 1],
+        "relev": [0, 3],
         "remov": 0,
         "remove_gend": 0,
         "renam": 0,
-        "report": 2,
-        "repres": 0,
+        "replac": 0,
+        "report": [0, 2],
+        "repres": [0, 1],
         "represent": 0,
         "request": 0,
         "requir": 0,
         "reset": 0,
         "reset_id": 0,
         "resolv": 0,
         "result": [0, 2],
         "return": [0, 2],
         "review": 0,
         "ridden": 0,
         "root": 0,
         "row": 0,
         "rule": 2,
+        "run": 3,
         "s_": 0,
-        "same": 0,
+        "same": [0, 3],
         "same_basionym": 0,
         "satisfi": 0,
-        "scientif": 0,
-        "scientificnam": 0,
-        "second": 0,
+        "save": [1, 3],
+        "schmidt": 3,
+        "scientif": [0, 1],
+        "scientificnam": [0, 3],
+        "second": [0, 3],
         "section": 0,
-        "sedi": 2,
+        "sedi": [0, 2],
         "see": 0,
         "select": 0,
         "separ": 0,
         "sequenc": 0,
-        "serialis": 0,
-        "set": [0, 2],
+        "serialis": [0, 1],
+        "serv": 0,
+        "set": [0, 1, 2],
         "set_basionymid": 0,
         "set_context": 0,
         "set_default_taxon_record": 0,
         "set_opt": 0,
         "sg": 0,
         "share": 0,
-        "should": [0, 2],
-        "show": 0,
+        "should": [0, 1, 2],
+        "show": [0, 3],
         "sibl": 0,
         "sic": [0, 2],
         "side": 0,
         "sign": 0,
         "simpli": 0,
-        "simplifi": 0,
-        "sinc": 0,
-        "so": 0,
+        "simplifi": [0, 1],
+        "sinc": [0, 3],
+        "singl": 3,
+        "so": [0, 1],
+        "societi": 3,
+        "sohn": 3,
         "sort": 0,
         "sort_nam": 0,
         "sort_taxa": 0,
         "sort_taxa_recurs": 0,
         "sourc": 0,
         "space": 0,
-        "speci": 0,
+        "speci": [0, 1, 3],
+        "species_id": 3,
         "species_interact": 0,
         "species_taxon_id": 0,
-        "speciesinteract": 0,
+        "speciesinteract": [0, 3],
         "specif": 0,
         "specifi": 0,
-        "specificepithet": 0,
+        "specificepithet": [0, 3],
         "spreadsheet": 0,
         "ss": 0,
-        "start_name_bundl": [0, 2],
+        "stabl": 3,
+        "start_name_bundl": [0, 1, 2, 3],
+        "statu": [0, 3],
         "stdout": 0,
         "step": 0,
         "store": 0,
-        "string": 0,
+        "string": [0, 3],
         "strip": 0,
         "subclass": 0,
         "subfamili": 0,
-        "subfold": 0,
+        "subfold": [0, 3],
         "subgener": 0,
         "subgenu": 0,
         "submit": 2,
         "subord": 0,
         "subphylum": 0,
         "subsequ": 0,
         "subset": 0,
         "subspeci": 0,
         "subspecif": 0,
         "subtrib": 0,
         "subvar": 0,
         "superfamili": 0,
         "supplement": 2,
-        "suppli": [0, 2],
+        "suppli": [0, 1, 2],
         "support": 0,
-        "synonym": [0, 2],
+        "syen": 3,
+        "synonym": [0, 1, 2, 3],
         "synonym_from_nameusag": 0,
         "synonym_prefix": 0,
         "synonymis": 0,
-        "tab": 0,
-        "tabl": 0,
+        "systemat": 3,
+        "t": 3,
+        "tab": [0, 1],
+        "tabl": [0, 3],
         "table_by_nam": 0,
+        "taken": 0,
         "target": 0,
-        "taxa": 0,
-        "taxon": [0, 2],
+        "taxa": [0, 1, 3],
+        "taxon": [0, 1, 2, 3],
+        "taxon_default": 3,
         "taxon_from_nameusag": 0,
         "taxon_id": 0,
-        "taxonid": 0,
-        "taxonom": 0,
+        "taxonid": [0, 3],
+        "taxonom": [0, 1],
+        "tee": 3,
         "term": 0,
-        "text": 0,
+        "text": [0, 3],
         "than": 0,
         "thei": 0,
-        "thi": [0, 2],
+        "thi": [0, 1, 2, 3],
         "those": 0,
-        "time": 0,
-        "titl": 0,
+        "three": 3,
+        "through": 0,
+        "time": [0, 3],
+        "titl": [0, 3],
         "to_dict": 0,
-        "tool": 0,
+        "togeth": 1,
+        "tool": [0, 1],
         "top": 0,
+        "transact": 3,
         "tree": 0,
         "tribe": 0,
+        "tridentaforma": 3,
+        "tridentaformida": 3,
+        "trigger": 1,
         "trinomi": 0,
         "true": 0,
         "tsv": 0,
         "tupl": 0,
-        "two": 0,
+        "two": [0, 1, 3],
         "txt": 0,
         "type": 0,
         "type_materi": 0,
-        "typemateri": 0,
-        "u": 0,
+        "typemateri": [0, 3],
+        "u": [0, 3],
         "um": 0,
-        "unchang": 0,
+        "unchang": [0, 3],
+        "uninomi": 3,
+        "unless": 0,
         "unus": 0,
         "updat": [0, 2],
         "upon": 0,
-        "us": [0, 2],
+        "us": [0, 1, 2],
         "usag": 2,
         "user": 0,
-        "valid": 0,
+        "valid": [0, 3],
         "validate_record": 0,
-        "valu": [0, 2],
+        "valu": [0, 1, 2],
         "var": 0,
         "variabl": 0,
+        "variant": 1,
         "variat": 2,
         "varieti": 0,
         "verifi": 0,
-        "version": 0,
-        "via": 0,
+        "version": [0, 1],
+        "via": [0, 1],
         "view": 0,
-        "volum": 0,
+        "volum": [0, 3],
+        "wai": 0,
         "warn": 0,
         "well": 0,
-        "when": 0,
+        "when": [0, 3],
         "whenev": 0,
         "where": 0,
         "whether": 0,
         "which": [0, 2],
         "whole": 0,
         "within": 0,
         "without": [0, 2],
         "word": 0,
+        "work": 1,
+        "would": 3,
         "wrapper": 2,
         "write": 0,
         "written": 0,
+        "www": 3,
         "y": 0,
         "year": 0,
-        "zoolog": 0
+        "zookei": 3,
+        "zoolog": 0,
+        "zwick": 3
     },
-    "titles": ["coldp.COLDP", "COLDP", "coldp.NameBundle"],
+    "titles": ["coldp.COLDP", "coldp", "coldp.NameBundle", "Usage"],
     "titleterms": {
         "access": 0,
         "add": 0,
         "behaviour": 0,
-        "class": [0, 2],
+        "class": [0, 1, 2],
         "coldp": [0, 1, 2],
         "constant": 0,
-        "content": 1,
         "control": 0,
         "datafram": 0,
         "find": 0,
         "get": 0,
         "index": [0, 1, 2],
+        "instal": 1,
         "intern": 0,
         "method": [0, 2],
         "modifi": 0,
         "namebundl": 2,
+        "overview": 1,
         "packag": 0,
         "record": 0,
         "save": 0,
         "search": [0, 1, 2],
         "tidi": 0,
+        "usag": [1, 3],
         "util": 0
     }
 })
```

### Comparing `coldp-2024.5.2/docs/build/html/_static/alabaster.css` & `coldp-2024.5.3/docs/build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.2/docs/build/html/_static/basic.css` & `coldp-2024.5.3/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.2/docs/build/html/_static/doctools.js` & `coldp-2024.5.3/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.2/docs/build/html/_static/language_data.js` & `coldp-2024.5.3/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.2/docs/build/html/_static/pygments.css` & `coldp-2024.5.3/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.2/docs/build/html/_static/searchtools.js` & `coldp-2024.5.3/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.2/docs/build/html/_static/sphinx_highlight.js` & `coldp-2024.5.3/docs/build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.2/docs/source/coldp.rst` & `coldp-2024.5.3/docs/source/coldp.rst`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 ===========
 
 .. currentmodule:: coldp
 
 Class
 ~~~~~
 
-.. autoclass:: COLDP
-    :no-index:
+.. automethod:: coldp.COLDP.__init__
 
 Methods
 ~~~~~~~
 
 Control behaviour
 ^^^^^^^^^^^^^^^^^
 .. automethod:: coldp.COLDP.set_options
@@ -36,14 +35,15 @@
 ^^^^
 .. automethod:: coldp.COLDP.save
 
 Find or get records
 ^^^^^^^^^^^^^^^^^^^
 .. automethod:: coldp.COLDP.find_name_record
 .. automethod:: coldp.COLDP.find_names
+.. automethod:: coldp.COLDP.find_distribution
 .. automethod:: coldp.COLDP.get_name
 .. automethod:: coldp.COLDP.get_reference
 .. automethod:: coldp.COLDP.get_taxon
 .. automethod:: coldp.COLDP.get_synonyms
 .. automethod:: coldp.COLDP.get_synonymy
 .. automethod:: coldp.COLDP.get_children
```

### Comparing `coldp-2024.5.2/docs/source/conf.py` & `coldp-2024.5.3/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,25 +11,26 @@
 import sys
 
 sys.path.insert(0, os.path.abspath("../../src/coldp"))
 
 project = "COLDP"
 copyright = "2024, Donald Hobern"
 author = "Donald Hobern"
-release = "2024.5.2"
+release = "2024.5.3"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.doctest",
     "sphinx.ext.intersphinx",
     "sphinx.ext.autosummary",
     "sphinx_paramlinks",
+    "sphinx_simplepdf",
 ]
 
 
 autosummary_generate = True
 autodoc_typehints = "none"
 
 templates_path = ["_templates"]
```

### Comparing `coldp-2024.5.2/src/coldp/coldp.py` & `coldp-2024.5.3/src/coldp/coldp.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # version ='2024.0.2'
 # ---------------------------------------------------------------------------
 """ 
 COLDP is a Python class for creating or loading, manipulating and serialising 
 Catalogue of Life Data Package (COLDP) files, the preferred format within 
 Catalogue of Life for organising taxonomic checklist datasets. 
 
-See: https://github.com/CatalogueOfLife/coldp 
+See: `COL Data Package (ColDP) Specification <https://github.com/CatalogueOfLife/coldp>`_
 """
 # ---------------------------------------------------------------------------
 # Imports
 # ---------------------------------------------------------------------------
 import pandas as pd
 import numpy as np
 import logging
@@ -306,61 +306,110 @@
 dictionary that includes the key "namerelation" with a list containing 
 "nameID" and "relatedNameID" as its value.
 
 This is a map of the foreign-key relationships that need to be validated 
 and preserved between the COLDP data tables.
 """
 
-# ---------------------------------------------------------------------------
+# -----------------------------------------------------------------------------
+# Required properties for tables
+#
+# Properties expected by COLDP methods when processing or finding records in
+# each table
+# -----------------------------------------------------------------------------
+required_properties = {
+    "reference": [
+        "ID",
+        "author",
+        "title",
+        "issued",
+        "containerTitle",
+        "volume",
+        "issue",
+        "page",
+        "citation",
+    ],
+    "name": [
+        "uninomial",
+        "genus",
+        "infragenericEpithet",
+        "specificEpithet",
+        "infraspecificEpithet",
+        "authorship",
+        "rank",
+        "basionymID",
+        "scientificName",
+        "code",
+        "status",
+    ],
+    "distribution": [
+        "taxonID",
+        "area",
+        "gazetteer",
+        "status",
+        "referenceID",
+    ],
+}
+"""
+Dictionary mapping table names to list of properties (columns) required by
+COLDP in a loaded dataframe.
+
+:py:func:`~coldp.COLDP.initialise_dataframe` will ensure that all listed columns
+are present.
+"""
+
+# ----------------------------------------------------------------------------
 # Recognised file extensions and their associated separator characters
-# ---------------------------------------------------------------------------
+# ----------------------------------------------------------------------------
 csv_extensions = {"csv": ",", "tsv": "\t", "txt": "\t"}
 """
 Dictionary mapping supported CSV/TSV file extensions to the expected delimiter.
 
 Supported extensions are .csv for comma-separated data files and .tsv or .txt for tab-delimited data files.
 """
 
 # ---------------------------------------------------------------------------
 # Regular expression patterns for uninomial and species-rank epithets and a
 # superset expression including both
 # ---------------------------------------------------------------------------
 uninomial_pattern = re.compile("^[A-Z][a-z]+$")
 epithet_pattern = re.compile("^[a-z]-?[a-z]+$")
 name_pattern = re.compile("^[A-Za-z]-?[a-z]+$")
+scientific_name_pattern = re.compile(
+    r"^([A-Z][a-z]+)( ([A-Z][a-z]+))?( ([a-z]-?[a-z]+))?( [abfrpsuv]+\.)?( ([a-z]-?[a-z]+))?$"
+)
 
 
 class NameBundle:
-    """
-    Wrapper class to manage set of associated names, normally an accepted name
-    and one or more synonyms. The bundle handles the logic of associated name
-    variations.
-
-    :param coldp: :py:class:`~coldp.COLDP` object to handle logging of any issues and normalise name records
-    :param accepted: Dictionary mapping COLDP name elements to values for the accepted name - a name record and a taxon record will be added to the COLDP package for the accepted name
-    :param incertae_sedis: Flag to indicate if the resulting taxon record should be marked "incertae sedis"
-    :param sic: Flag to indicate if the accepted name should be processed without reporting issues for invalid format
-
-    The minimal usage is to create a new bundle with an accepted name. One
-    or more synonyms can also be supplied using the :py:func:`~coldp.NameBundle.add_synonym` method.
-    The bundle is then submitted to the :py:func:`coldp.COLDP.add_names` method for
-    processing.
-
-    NameBundle objects should not be created directly. Use the :py:punc`coldp.COLDP.start_name_bundle` method instead.
-
-    accepted should contain a dictionary with keys that match property names from the `COLDP Name class <https://github.com/CatalogueOfLife/coldp?tab=readme-ov-file#name>`_
-    """
-
     def __init__(
         self,
         coldp,
         accepted: dict[str:str],
         incertae_sedis: bool = False,
         sic: bool = False,
     ) -> None:
+        """
+        Wrapper class to manage set of associated names, normally an accepted name
+        and one or more synonyms. The bundle handles the logic of associated name
+        variations.
+
+        :param coldp: :py:class:`~coldp.COLDP` object to handle logging of any issues and normalise name records
+        :param accepted: Dictionary mapping COLDP name elements to values for the accepted name - a name record and a taxon record will be added to the COLDP package for the accepted name
+        :param incertae_sedis: Flag to indicate if the resulting taxon record should be marked "incertae sedis"
+        :param sic: Flag to indicate if the accepted name should be processed without reporting issues for invalid format
+
+        The minimal usage is to create a new bundle with an accepted name. One
+        or more synonyms can also be supplied using the :py:func:`~coldp.NameBundle.add_synonym` method.
+        The bundle is then submitted to the :py:func:`coldp.COLDP.add_names` method for
+        processing.
+
+        NameBundle objects should not be created directly. Use the :py:func:`coldp.COLDP.start_name_bundle` method instead.
+
+        accepted should contain a dictionary with keys that match property names from the `COLDP Name class <https://github.com/CatalogueOfLife/coldp?tab=readme-ov-file#name>`_
+        """
 
         self.coldp = coldp
         if "rank" not in accepted:
             self.coldp.issue(
                 "Accepted name missing rank, assume species: " + str(accepted)
             )
             accepted["rank"] = "species"
@@ -393,40 +442,34 @@
                         normalised["authorship"] is None
                         or s["authorship"] is None
                         or normalised["authorship"] == s["authorship"]
                     ):
                         present = True
                         break
         if not present:
-            self.synonyms.append(self.normalise_name(synonym, sic))
+            self.synonyms.append(normalised)
 
     def normalise_name(self, name: dict[str:str], sic: bool = False) -> dict:
         """
         Ensure that a name record dictionary contains all necessary/appropriate elements
 
         :param name: Dictionary containing name to be normalised
         :param sic: Flag to indicate that the name does not follow expected formatting rules for a code-compliant name and that no issues should be logged for this
         :return: Name dictionary updated with extra values
         """
 
         # Ensure main elements are present in dictionary
-        for k in [
-            "uninomial",
-            "genus",
-            "infragenericEpithet",
-            "specificEpithet",
-            "infraspecificEpithet",
-            "authorship",
-            "rank",
-            "basionymID",
-            "scientificName",
-        ]:
+        for k in required_properties["name"]:
             if k not in name:
                 name[k] = ""
 
+        # If code is missing, use value from COLDP
+        if "code" not in name or name["code"] == "":
+            name["code"] = self.coldp.code
+
         # Skip processing if sic
         if not sic:
             # Check uninomials for formatting - log issues and fix case
             for k in ["uninomial", "genus", "infragenericEpithet"]:
                 if len(name[k]) > 0:
                     if not name_pattern.match(name[k]):
                         self.coldp.issue(
@@ -447,16 +490,41 @@
                         self.coldp.issue("Invalid pattern for epithet: " + name[k])
                     elif name[k][0].isupper():
                         self.coldp.issue(
                             "Uppercase initial letter for epithet: " + name[k]
                         )
                         name[k] = name[k][0].lower() + name[k][1:]
 
+        # If scientificName is present, make sure all parts are
+        # also completed.
+        if name["scientificName"]:
+            match = scientific_name_pattern.match(name["scientificName"])
+            if match is not None:
+                # Handle any name with a specificEpithet
+                if match.group(5):
+                    if not name["genus"]:
+                        name["genus"] = match.group(1)
+                    if not name["infragenericEpithet"] and match.group(3):
+                        name["infragenericEpithet"] = match.group(3)
+                    if not name["specificEpithet"] and match.group(5):
+                        name["specificEpithet"] = match.group(5)
+                    if not name["infraspecificEpithet"] and match.group(8):
+                        name["infraspecificEpithet"] = match.group(8)
+                elif name["rank"] == "subgenus":
+                    if not name["genus"]:
+                        name["genus"] = match.group(1)
+                    if not name["uninomial"] and match.group(3):
+                        name["uninomial"] = match.group(3)
+                else:
+                    if not name["uninomial"]:
+                        name["uninomial"] = match.group(1)
+
+        # Generate properly formatted scientific name unless sic is True.
+        # If sic is True but scientificName is empty, generate anyway.
         if not sic or not name["scientificName"]:
-            # Generate properly formatted scientific name
             if self.coldp.is_species_group(name):
                 (
                     name["scientificName"],
                     name["rank"],
                 ) = self.coldp.construct_species_rank_name(
                     name["genus"],
                     name["infragenericEpithet"],
@@ -485,81 +553,21 @@
             "authorship" not in values
             and "authorship" in name
             and not name["authorship"].startswith("(")
         ):
             if "genus" in values or "specificEpithet" in values:
                 values["authorship"] = "(" + name["authorship"] + ")"
 
-        for k in [
-            "basionymID",
-            "authorship",
-            "rank",
-            "uninomial",
-            "genus",
-            "infragenericEpithet",
-            "specificEpithet",
-            "infraspecificEpithet",
-            "code",
-            "status",
-        ]:
+        for k in required_properties["name"]:
             if k in name and k not in values:
                 values[k] = name[k]
         return self.normalise_name(values, sic)
 
 
 class COLDP:
-    """
-    Class to manage a set of Pandas dataframes for CSV tables in Catalogue
-    of Life Data Package.
-
-    :param name: The name for the COLDP package. If a folder of this name exists inside the folder specied by the folder parameter, this COLDP instance will be initialised with the contents of any COLDP-compliant CSV or TSV files in the named folder.
-    :param folder: Name of folder that may contain the named COLDP source folder from which source files should be read (name specified via the name parameter) and that is the default folder in which a COLDP folder will be written when the COLDP instance is saved. This is not the folder in which the CSV files are written. It is the folder which will contain the subfolder holding CSV files.
-    :param code: ICZN or ICBN to indicate the nomenclatural code for name formatting. ICZN is the default.
-    :param default_taxon_record: Any values in the dictionary are automatically used as default values in taxon records added to the COLDP instance. In other words, the dictionary becomes the base into which other taxon record properties are then inserted.
-    :param insert_species_for_trinomials: If true, insert species (taxon and name) if trinomials are provided without the associated species. This can be convenient when mapping source data that only lists infraspecific taxa for species with subspecies, varieties or forms.
-    :param create_subspecies_for_infrasubspecifics: If true, automatically add a trinomial at subspecific rank as a synonym whenever an infrasubspecific name is added. This may be useful if the resulting dataset is intended to provide easy mapping of strings to taxon concepts, since versions of the trinomial lacking the rank marker will often be found in source data.
-    :param create_synonyms_without_subgenus: If true, automatically add a binomial or trinomial without an included subgenus name as a synonym whenever a name including a subgenus is added. This may be useful if the resulting dataset is intended to provide easy mapping of strings to taxon concepts, since versions of lacking the subgeneric component will often be found in source data.
-    :param basionyms_from_synonyms: If true, basionym associations are automatically created from synonyms within a loaded COLDP dataset. If an accepted name includes parentheses around the authorship, and if a name with the same epithet and authorship but no parentheses is included in the synonyms, the ID value for the synonym will be used for the basionymID element in the accepted name. This is normally a housekeeping step when first loading a new COLDP dataset. This option is only used when the dataset is first loaded. Addition of basionym relationships is automatic for names added as part of the same NameBundle.
-    :param classification_from_parents: If true, insert names for higher ranks into relevant elements in each taxon record based on the parent and higher ancestry for the taxon.
-    :param allow_repeated_binomials: If true, omit checks rejecting the addition of the same binomial more than once to the COLDP name dataframe.
-    :param create_taxa_for_not_established: If true, generate taxon records even if the associated name is flagged as not established (i.e. not satisfying the relevant nomenclatural code)
-    :param issues_to_stdout: If true, print any issue messages (see :py:func:`~coldp.COLDP.issue`) to stdout as well as inserting then in the issue dataframe.
-    :param context: Value to be used in labeling issue records (see :py:func:`~coldp.COLDP.issue`). This value is more normally set using :py:func:`~coldp.COLDP.set_context`.
-
-    A COLDP object is initalised with a source/destination folder, COLDP package
-    name and other options.
-
-    If a subfolder exists with the supplied name in the supplied folder, it
-    will be initialised with data from any CSV/TSV files it contains with any
-    of the following base names: name, taxon, synonym, reference,
-    distribution, speciesinteraction, namerelation, typematerial or nameusage,
-    and with a file extension recognised via :py:data:`~coldp.COLDP.csv_extensions`.
-    File names are case insensitive.
-
-    Files with the base name nameusage are loaded only if the name, taxon or
-    synonym file is absent, in which case the contents of the nameusage file
-    are mapped internally to the more normalised COLDP format with separate
-    name + taxon + synonym tables.
-
-    If no folder exists with the supplied name, an empty instance is created.
-    Pandas dataframes are created as required for the COLDP data types as
-    data are inserted into the instance.
-
-    The :py:func:`~coldp.COLDP.start_name_bundle` method produces a :py:class:`~coldp.COLDP.NameBundle` object for preparing an
-    accepted name and associated synonyms to pass to the :py:func:`~coldp.COLDP.add_names` method
-    which creates name, taxon and synonym records as a set of cross-referenced
-    objects.
-
-    Other data is added using the :py:func:`~coldp.COLDP.add_references, :py:func:`~coldp.COLDP.add_names`, :py:func:`~coldp.COLDP.add_name_relation`,
-    :py:func:`~coldp.COLDP.add_typematerial`, :py:func:`~coldp.COLDP.add_distribution`, :py:func:`~coldp.COLDP.add_species_interaction` and
-    :py:func:`~coldp.COLDP.modify_taxon` methods.
-
-    The :py:func:`~coldp.COLDP.save` method writes the data back to the same or another folder.
-    """
-
     def __init__(
         self,
         name: str,
         folder: str = ".",
         code: str = "ICZN",
         default_taxon_record: dict[str:str] = None,
         insert_species_for_trinomials: bool = False,
@@ -568,22 +576,71 @@
         basionyms_from_synonyms: bool = False,
         classification_from_parents: bool = False,
         allow_repeated_binomials: bool = False,
         create_taxa_for_not_established: bool = False,
         issues_to_stdout: bool = False,
         context: str = None,
     ) -> None:
+        """
+        Class to manage a set of Pandas dataframes for CSV tables in Catalogue
+        of Life Data Package.
+
+        :param name: The name for the COLDP package. If a folder of this name exists inside the folder specied by the folder parameter, this COLDP instance will be initialised with the contents of any COLDP-compliant CSV or TSV files in the named folder.
+        :param folder: Name of folder that may contain the named COLDP source folder from which source files should be read (name specified via the name parameter) and that is the default folder in which a COLDP folder will be written when the COLDP instance is saved. This is not the folder in which the CSV files are written. It is the folder which will contain the subfolder holding CSV files.
+        :param code: ICZN or ICBN to indicate the nomenclatural code for name formatting. ICZN is the default.
+        :param default_taxon_record: Any values in the dictionary are automatically used as default values in taxon records added to the COLDP instance. In other words, the dictionary becomes the base into which other taxon record properties are then inserted.
+        :param insert_species_for_trinomials: If true, insert species (taxon and name) if trinomials are provided without the associated species. This can be convenient when mapping source data that only lists infraspecific taxa for species with subspecies, varieties or forms.
+        :param create_subspecies_for_infrasubspecifics: If true, automatically add a trinomial at subspecific rank as a synonym whenever an infrasubspecific name is added. This may be useful if the resulting dataset is intended to provide easy mapping of strings to taxon concepts, since versions of the trinomial lacking the rank marker will often be found in source data.
+        :param create_synonyms_without_subgenus: If true, automatically add a binomial or trinomial without an included subgenus name as a synonym whenever a name including a subgenus is added. This may be useful if the resulting dataset is intended to provide easy mapping of strings to taxon concepts, since versions of lacking the subgeneric component will often be found in source data.
+        :param basionyms_from_synonyms: If true, basionym associations are automatically created from synonyms within a loaded COLDP dataset. If an accepted name includes parentheses around the authorship, and if a name with the same epithet and authorship but no parentheses is included in the synonyms, the ID value for the synonym will be used for the basionymID element in the accepted name. This is normally a housekeeping step when first loading a new COLDP dataset. This option is only used when the dataset is first loaded. Addition of basionym relationships is automatic for names added as part of the same NameBundle.
+        :param classification_from_parents: If true, insert names for higher ranks into relevant elements in each taxon record based on the parent and higher ancestry for the taxon.
+        :param allow_repeated_binomials: If true, omit checks rejecting the addition of the same binomial more than once to the COLDP name dataframe.
+        :param create_taxa_for_not_established: If true, generate taxon records even if the associated name is flagged as not established (i.e. not satisfying the relevant nomenclatural code)
+        :param issues_to_stdout: If true, print any issue messages (see :py:func:`~coldp.COLDP.issue`) to stdout as well as inserting then in the issue dataframe.
+        :param context: Value to be used in labeling issue records (see :py:func:`~coldp.COLDP.issue`). This value is more normally set using :py:func:`~coldp.COLDP.set_context`.
+
+        A COLDP object is initalised with a source/destination folder, COLDP package
+        name and other options.
+
+        If a subfolder exists with the supplied name in the supplied folder, it
+        will be initialised with data from any CSV/TSV files it contains with any
+        of the following base names: name, taxon, synonym, reference,
+        distribution, speciesinteraction, namerelation, typematerial or nameusage,
+        and with a file extension recognised via :py:data:`~coldp.COLDP.csv_extensions`.
+        File names are case insensitive.
+
+        Files with the base name nameusage are loaded only if the name, taxon or
+        synonym file is absent, in which case the contents of the nameusage file
+        are mapped internally to the more normalised COLDP format with separate
+        name + taxon + synonym tables.
+
+        If no folder exists with the supplied name, an empty instance is created.
+        Pandas dataframes are created as required for the COLDP data types as
+        data are inserted into the instance.
+
+        The :py:func:`~coldp.COLDP.start_name_bundle` method produces a :py:class:`~coldp.COLDP.NameBundle` object for preparing an
+        accepted name and associated synonyms to pass to the :py:func:`~coldp.COLDP.add_names` method
+        which creates name, taxon and synonym records as a set of cross-referenced
+        objects.
+
+        Other data is added using the :py:func:`~coldp.COLDP.add_references, :py:func:`~coldp.COLDP.add_names`, :py:func:`~coldp.COLDP.add_name_relation`,
+        :py:func:`~coldp.COLDP.add_typematerial`, :py:func:`~coldp.COLDP.add_distribution`, :py:func:`~coldp.COLDP.add_species_interaction` and
+        :py:func:`~coldp.COLDP.modify_taxon` methods.
+
+        The :py:func:`~coldp.COLDP.save` method writes the data back to the same or another folder.
+        """
 
         self.default_taxon = {
             "provisional": "false",
             "extinct": "false",
             "temporalRangeEnd": "Holocene",
         }
-        self.default_taxon_record = default_taxon_record
-        self.code = "ICZN"
+        if default_taxon_record is not None:
+            self.default_taxon.update(default_taxon_record)
+        self.code = code
         self.species_from_trinomials = insert_species_for_trinomials
         self.subspecies_from_trinomials = create_subspecies_for_infrasubspecifics
         self.subgenus_free_synonyms = create_synonyms_without_subgenus
         self.basionyms_from_synonyms = basionyms_from_synonyms
         self.classification_from_parents = classification_from_parents
         self.allow_repeated_binomials = allow_repeated_binomials
         self.create_taxa_for_not_established = create_taxa_for_not_established
@@ -771,14 +828,20 @@
                         taxon_from_nameusage,
                     )
 
         # Empty dataframe by default
         if df is None and default_headings is not None:
             df = pd.DataFrame(columns=default_headings)
 
+        # Ensure essential columns are present
+        if name in required_properties:
+            for column in required_properties[name]:
+                if column not in df.columns:
+                    df[column] = ""
+
         return df
 
     def extract_table(
         self, df: pd.DataFrame, headings: list[str], mappings: dict[str:str]
     ) -> pd.DataFrame:
         """
         Extract a set of columns from a dataframe using a dictionary that maps
@@ -1212,25 +1275,15 @@
         :return: DataFrame with one COLDP reference record if found, else None
 
         Only returns a record that exactly matches the values supplied in
         :py:paramref:`~coldp.COLDP.find_reference.reference` for all of
         author, title, issued, containerTitle, volume, issue, page and citation.
         """
 
-        for k in [
-            "ID",
-            "author",
-            "title",
-            "issued",
-            "containerTitle",
-            "volume",
-            "issue",
-            "page",
-            "citation",
-        ]:
+        for k in required_properties["reference"]:
             if k not in reference:
                 reference[k] = ""
 
         match = self.references[
             (self.references["author"] == reference["author"])
             & (self.references["title"] == reference["title"])
             & (self.references["issued"] == reference["issued"])
@@ -1241,15 +1294,27 @@
             & (self.references["citation"] == reference["citation"])
         ]
 
         if len(match) == 0:
             return None
         return match.iloc[0]
 
-    def start_name_bundle(self, accepted, incertae_sedis=False, sic=False):
+    def start_name_bundle(
+        self, accepted: dict[str:str], incertae_sedis: bool = False, sic: bool = False
+    ) -> NameBundle:
+        """
+        Return a NameBundle object based on the supplied accepted name and referencing this COLDP instance
+
+        :param accepted: Dictionary containing COLDP Name record for accepted name
+        :param incertae_sedis: If True, the associated COLDP Taxon Record will be flagged as *incertae sedis*
+        :param sic: If True, issues will not be reported if the name is not properly code-compliant
+        :return: NameBundle instance initialised with supplied parameters
+
+        This is the normal way to construct a new NameBundle object.
+        """
         return NameBundle(self, accepted, incertae_sedis, sic)
 
     def add_names(self, bundle: NameBundle, parent: str = None) -> None:
         """
         Ensure one or more names are included in names dataframe and update
         taxa and synonyms dataframes as necessary
 
@@ -1268,18 +1333,18 @@
         of infrasubspecific trinomials and subgenus-free versions of combinations
         including a subgenus name.
 
         If a matching name already exists in the COLDP instance, no new name will
         normally be added. Instead, the name record in the bundle will be updated
         with the ID (and basionymID where applicable) from the existing name. This
         allows for additional synonyms to be added to an existing taxon. The
-        behaviour can be over-ridden with the :paramref:`~coldp.COLDP.allow_repeated_binomials`
+        behaviour can be over-ridden with the :paramref:`~coldp.COLDP.__init__.allow_repeated_binomials`
         option, in which case any number of matching names can be added.
 
-        If the :paramref:`~coldp.COLDP.insert_species_for_trinomials` option is
+        If the :paramref:`~coldp.COLDP.__init__.insert_species_for_trinomials` option is
         set, a new species will be created if required before adding the
         trinomial as its child. In this case the bundle will contain the id
         for the species taxon as a species_taxon_id property.
 
         Name records in the bundle are all updated with existing or new IDs and
         basionymIDs, which are inferred automatically for zoological names by
         associating combinations with and without parentheses around the
@@ -1344,15 +1409,15 @@
 
         if bundle.accepted["basionymID"] != bundle.accepted["ID"]:
             self.names.loc[
                 self.names["basionymID"] == bundle.accepted["ID"], ["basionymID"]
             ] = bundle.accepted["basionymID"]
 
         if (
-            "status" not in bundle.accepted
+            not bundle.accepted["status"]
             or bundle.accepted["status"] == "established"
             or self.create_taxa_for_not_established
         ):
             if bundle.species:
                 taxon = self.insert_taxon(bundle.species, parent)
                 parent = taxon["ID"]
                 bundle.species_taxon_id = parent
@@ -1485,20 +1550,54 @@
             or distribution["taxonID"] not in self.taxa["ID"].values
         ):
             self.issue(
                 f"Distribution must be associated with a valid taxon ID ({distribution['taxonID'] if 'taxonID' in distribution else 'None'}) supplied"
             )
             return None
 
+        dist = self.find_distribution(distribution)
+        if dist is not None:
+            logging.debug("Matched distribution")
+            return dist.to_dict()
+
         self.distributions = pd.concat(
             (self.distributions, pd.DataFrame.from_records([distribution])),
             ignore_index=True,
         )
         return distribution
 
+    def find_distribution(self, distribution: dict[str:str]) -> pd.DataFrame:
+        """
+        Locate existing COLDP distribution record exactly matching all major
+        fields in :py:paramref:`~coldp.COLDP.find_distribution.distribution`
+
+        :param distribution: Dictionary of COLDP distribution properties representing a record to be found
+        :return: DataFrame with one COLDP distribution record if found, else None
+
+        Only returns a record that exactly matches the values supplied in
+        :py:paramref:`~coldp.COLDP.find_distribution.distribution` for all of
+        taxonID, area, gazetteer, status, referenceID.
+        """
+
+        for k in required_properties["distribution"]:
+            if k not in distribution:
+                distribution[k] = ""
+
+        match = self.distributions[
+            (self.distributions["taxonID"] == distribution["taxonID"])
+            & (self.distributions["area"] == distribution["area"])
+            & (self.distributions["gazetteer"] == distribution["gazetteer"])
+            & (self.distributions["status"] == distribution["status"])
+            & (self.distributions["referenceID"] == distribution["referenceID"])
+        ]
+
+        if len(match) == 0:
+            return None
+        return match.iloc[0]
+
     def add_species_interaction(self, interaction: dict[str:str]) -> dict[str:str]:
         """
         Add COLDP SpeciesInteraction record to COLDP instance
 
         :param interaction: COLDP SpeciesInteraction record represented as dictionary of properties
         :return: SpeciesInteraction record returned unchanged
 
@@ -1528,19 +1627,19 @@
 
     def prepare_bundle(self, bundle):
         """
         Add extra names to :py:class:`~coldp.NameBundle` if required based on current options
 
         :param bundle: NameBundle to be processed
 
-        If :paramref:`~coldp.COLDP.insert_species_for_trinomials` is True, ensure that the implied binomial exists for any new trinomials.
+        If :paramref:`~coldp.COLDP.__init__.insert_species_for_trinomials` is True, ensure that the implied binomial exists for any new trinomials.
 
-        If :paramref:`~coldp.COLDP.create_subspecies_for_infrasubspecifics` is True, add a subspecies-rank synonym to the bundle for each infrasubspecific name.
+        If :paramref:`~coldp.COLDP.__init__.create_subspecies_for_infrasubspecifics` is True, add a subspecies-rank synonym to the bundle for each infrasubspecific name.
 
-        If :paramref:`~coldp.COLDP.create_synonyms_without_subgenus` is True, add a subgenus-free synonym to the bundle for each name containing a subgenus.
+        If :paramref:`~coldp.COLDP.__init__.create_synonyms_without_subgenus` is True, add a subgenus-free synonym to the bundle for each name containing a subgenus.
         """
 
         # Identify the species that should exist to allow the accepted name to be grafted. E.g. Aus bus cus --> Aus bus
         if self.species_from_trinomials:
             if bundle.accepted["infraspecificEpithet"]:
                 bundle.species = bundle.derive_name(
                     bundle.accepted,
@@ -1655,17 +1754,29 @@
                         self.issue(
                             f"Record {record_type} {record} includes unrecognised {property}: {record[property]}"
                         )
                         valid = False
 
         return valid
 
-    def insert_taxon(self, name, parent, incertae_sedis=False):
+    def insert_taxon(
+        self, name: dict[str:str], parentID: str, incertae_sedis: bool = False
+    ) -> dict[str:str]:
+        """
+        Insert COLDP Taxon record as child of identified parent - creates or moves record as necessary
 
-        print(f"Name: {name}\nParent: {parent}")
+        :param name: COLDP Name record to be used as accepted name for new taxon
+        :param parentID: String identifier for parent taxon
+        :return: Dictionary containing taxon record
+
+        If a taxon record already exists for the name, any parenthood change is
+        made as required and the record is returned as a dictionary. Otherwise
+        a new record is created and returned. Default values are taken from the
+        :paramref:`~coldp.COLDP.__init__.default_taxon_record` dictionary.
+        """
         match = self.taxa[self.taxa["nameID"] == name["ID"]]
         if len(match) > 0:
             if len(match) > 1:
                 self.issue("More than one taxon matches name " + name["ID"])
             match = match.iloc[0]
             if match["uninomial"] != name["uninomial"]:
                 self.issue(
@@ -1688,20 +1799,20 @@
                     + name["scientificName"]
                     + ") for taxon id "
                     + match["ID"]
                 )
             if (
                 "parentID" in match
                 and match["parentID"]
-                and parent
-                and match["parentID"] != parent
+                and parentID
+                and match["parentID"] != parentID
             ):
                 match = self.taxa[self.taxa["ID"] == match["parentID"]].iloc[0]
                 parentA = self.names[self.names["ID"] == match["nameID"]].iloc[0]
-                match = self.taxa[self.taxa["ID"] == parent].iloc[0]
+                match = self.taxa[self.taxa["ID"] == parentID].iloc[0]
                 parentB = self.names[self.names["ID"] == match["nameID"]].iloc[0]
                 self.issue(
                     "Parent mismatch for "
                     + name["rank"]
                     + " "
                     + name["scientificName"]
                     + " "
@@ -1711,34 +1822,34 @@
                     + " "
                     + parentA["authorship"]
                     + ", now: "
                     + parentB["scientificName"]
                     + " "
                     + parentB["authorship"]
                 )
-            return match
+            return match.to_dict()
         else:
             parent_rank = ""
             parent_name = ""
-            if parent:
-                match = self.taxa[self.taxa["ID"] == parent]
+            if parentID:
+                match = self.taxa[self.taxa["ID"] == parentID]
                 if len(match) == 0:
-                    self.issue("Parent taxon not found " + parent)
+                    self.issue("Parent taxon not found " + parentID)
                     taxon_row = self.default_taxon
                 else:
                     taxon_row = match.iloc[0].copy()
                     parent_name_row = self.names[
                         self.names["ID"] == taxon_row["nameID"]
                     ]
                     parent_rank = parent_name_row.iloc[0]["rank"]
                     parent_name = parent_name_row.iloc[0]["scientificName"]
             else:
                 taxon_row = self.default_taxon
             taxon_row["ID"] = str(len(self.taxa) + 1)
-            taxon_row["parentID"] = parent if parent else ""
+            taxon_row["parentID"] = parentID if parentID else ""
             taxon_row["nameID"] = name["ID"]
             if parent_rank in [
                 "kingdom",
                 "phylum",
                 "class",
                 "order",
                 "superfamily",
@@ -1806,14 +1917,23 @@
 
     def identify_name(self, name: dict[str:str]) -> dict[str:str]:
         """
         Ensure COLDP Name record is present and return a copy containing the current ID and basionymID
 
         :param name: Dictionary containing COLDP Name properties
         :return: Currently stored version of the name record in question
+
+        If a COLDP Name record for this name already exists
+        (based on :py:func:`~coldp.COLDP.find_name_record`), return the existing
+        name, unless this is a species name and the
+        :paramref:`~coldp.COLDP.__init__.allow_repeated_binomials` option has been set,
+        in which case a new record will be created.
+
+        If the name is missing, create a new record with the next unused ID
+        value and return the record with the ID.
         """
         match = None
 
         if name["rank"] != "species" or not self.allow_repeated_binomials:
             match = self.find_name_record(name)
         if match is not None:
             return match
@@ -1871,15 +1991,27 @@
 
         Relevant only for zoological names
         """
         if authorship.startswith("(") and ")" in authorship:
             return authorship[1 : authorship.index(")")]
         return authorship
 
-    def epithet_and_authorship_match(self, name, epithet, authorship):
+    def epithet_and_authorship_match(
+        self, name: dict[str:str], epithet: str, authorship: str
+    ) -> bool:
+        """
+        Check whether a name record matches the supplied epithet and authorship
+
+        :param name: Dictionary containing COLDP Name record
+        :param epithet: Specific or infraspecific epithet
+        :param authorship: Authorship string
+        :return: True if the :paramref:`~coldp.COLDP.epithet_and_authorship_match.epithet` matches the lowest-ranked epithet and :paramref:`~coldp.COLDP.epithet_and_authorship_match.authorship` matches the authorship in the name record
+
+        Comparison ignores epithet gender endings.
+        """
         epithet = self.remove_gender(epithet)
         return name["authorship"] == authorship and (
             self.remove_gender(name["infraspecificEpithet"]) == epithet
             or (
                 self.remove_gender(name["specificEpithet"]) == epithet
                 and not name["infraspecificEpithet"]
             )
@@ -1899,14 +2031,23 @@
             self.names.loc[self.names["ID"] == name["ID"], ["basionymID"]] = basionymid
             name["basionymID"] = basionymid
         return name
 
     def fix_basionymid(
         self, name: dict[str:str], synonyms: list[dict[str:str]]
     ) -> dict[str:str]:
+        """
+        Update name so its basionymID references the original combination in a list of synonyms
+
+        :param name: Dictionary containing COLDP Name record for which basionymID is to be fixed
+        :param synonyms: List of COLDP Name records that may contain basionym
+        :return:
+
+        Returns name following any updates.
+        """
         original_authorship = self.get_original_authorship(name["authorship"])
         if name["authorship"] != original_authorship:
             epithet = (
                 name["infraspecificEpithet"]
                 if name["infraspecificEpithet"]
                 else name["specificEpithet"]
             )
@@ -1918,37 +2059,66 @@
                     break
         else:
             name = self.set_basionymid(name, name["ID"])
         return name
 
     def find_name_record(self, name: dict[str:str]) -> dict[str:str]:
         """
-        Return record from names DataFrame matching key fields in supplied record
+        Return record from names DataFrame matching key fields (scientificName,
+        authorship and rank) in supplied record
 
         :param name: Dictionary containing Name properties
         :return: Dictionary containing matching record if found
 
         Locates any existing record in the names DataFrame that matches the
         supplied scientificName, authorship and rank and returns it as a
         COLDP Name properties dictionary, or None if no match is found.
         """
         record = self.find_name(
             name["scientificName"], name["authorship"], name["rank"]
         )
         return None if record is None else record.to_dict()
 
-    def get_name(self, id: str):
+    def get_name(self, id: str) -> pd.DataFrame:
+        """
+        Return record from names DataFrame with supplied ID
+
+        :param id: String ID for COLDP Name record
+        :return: Pandas DataFrame containing matching record if found
+
+        Locates any existing record in the names DataFrame with the supplied
+        ID, or None if no match is found. If multiple matches are found, logs
+        an issue and returns the first.
+        """
         match = self.names[self.names["ID"] == id]
         if len(match) == 0:
             return None
         if len(match) > 1:
             logging.warn(f"Multiple matches for name ID: {id}")
         return match.to_dict("records")[0]
 
-    def find_name(self, scientificName, authorship, rank):
+    def find_name(
+        self, scientificName: str, authorship: str, rank: str
+    ) -> pd.DataFrame:
+        """
+        Return record from names DataFrame matching supplied scientificName,
+        authorship and rank
+
+        :param scientificName: Scientific name in canonical format
+        :param authorship: Authorship string
+        :param rank: Rank name string
+        :return: Dictionary containing matching record if found
+
+        Locates any existing record in the names DataFrame that matches the
+        supplied scientificName, authorship and rank and returns it as a
+        COLDP Name properties dictionary, or None if no match is found.
+
+        If :paramref:`~coldp.COLDP.find_name.authorship` is None, returns a
+        name based only on scientificName and rank.
+        """
         if authorship is None:
             match = self.names[
                 (self.names["scientificName"] == scientificName)
                 & (self.names["rank"] == rank)
             ]
         else:
             match = self.names[
@@ -1961,25 +2131,48 @@
                 "Multiple name records for "
                 + f"{rank} {scientificName} {str(authorship)}"
             )
         if len(match) == 1:
             return match.iloc[0]
         return None
 
-    def find_taxon(self, scientificName, authorship, rank):
+    def find_taxon(
+        self, scientificName: str, authorship: str, rank: str
+    ) -> pd.DataFrame:
+        """
+        Get COLDP Taxon record (as Pandas dataframe) with accepted name matching supplied scientificName, authorship and rank values
+
+        :param scientificName: Scientific name in canonical format
+        :param authorship: Authorship string
+        :param rank: Rank name string
+        :return: COLDP Taxon record matching supplied parameters
+
+        Logs a warning issue if multiple taxon records exist for a matching name and returns the first such match. Returns None if no match.
+        """
         name = self.find_name(scientificName, authorship, rank)
         if name is not None:
             match = self.taxa[self.taxa["nameID"] == name["ID"]]
             if len(match) > 1:
                 self.issue("Multiple taxa for name " + str(name))
             if len(match) > 0:
                 return match.iloc[0]
         return None
 
-    def find_names(self, properties, to_dict=False):
+    def find_names(
+        self, properties: dict[str:str], to_dict: bool = False
+    ) -> pd.DataFrame | list[dict[str:str]]:
+        """
+        Get all COLDP Name records matching all the supplied properties
+
+        :param properties: Dictionary of property values to serve as filter
+        :param to_dict: True if records should be converted from Pandas format to dictionary records, False (default) otherwise.
+        :return: Set of COLDP Name records either as DataFrame or list of dictionaries
+
+        Returns all matching records as Pandas DataFrame or list of dictionaries. If no matches, None is returned.
+        """
         for k in properties.keys():
             if k not in self.names.columns:
                 self.issue(f"Unknown name property: {k}")
                 return None
 
         names = self.names
         for k in properties.keys():
@@ -1987,31 +2180,63 @@
             if len(names) == 0:
                 return None
 
         if to_dict:
             return names.to_dict("records")
         return names
 
-    def get_taxon(self, id):
+    def get_taxon(self, id: str) -> dict[str:str]:
+        """
+        Return a COLDP Taxon record matching the supplied ID
+
+        :param id: String ID value
+        :return: Dictionary representation of COLDP Taxon record
+
+        Logs a warning if more than one match and returns the first such match.
+        """
         match = self.taxa[self.taxa["ID"] == id]
         if match.empty:
             return None
         if len(match.index) > 1:
             logging.warn(f"Multiple matches for taxon ID: {id}")
         return match.to_dict("records")[0]
 
-    def get_synonyms(self, taxonID, to_dict=False):
+    def get_synonyms(
+        self, taxonID: str, to_dict: bool = False
+    ) -> pd.DataFrame | list[dict[str:str]]:
+        """
+        Get all COLDP Synonym records for the supplied taxon ID
+
+        :param taxonID: String taxonID value
+        :param to_dict: True if records should be converted from Pandas format to dictionary records, False (default) otherwise.
+        :return: Set of COLDP Synonym records for taxon either as DataFrame or list of dictionaries
+
+        Returns all matching records as Pandas DataFrame or list of dictionaries. If no matches, None is returned.
+        """
         match = self.synonyms[self.synonyms["taxonID"] == taxonID]
         if match.empty:
             return None
         if to_dict:
             return match.to_dict("records")
         return match
 
-    def get_synonymy(self, nameID, to_dict=False):
+    def get_synonymy(
+        self, nameID: str, to_dict: bool = False
+    ) -> tuple[pd.DataFrame | dict[str:str], pd.DataFrame | list[dict[str:str]]]:
+        """
+        Get accepted COLDP Name record and all synonym COLDP Name records for the supplied name ID
+
+        :param taxonID: String nameID value
+        :param to_dict: True if records should be converted from Pandas format to dictionary records, False (default) otherwise
+        :return: Tuple containing COLDP Name record for accepted name and a DataFrame or list of dictionaries representing all synonym Name records
+
+        Maps the name indicated by the provided nameID to the accepted taxon and
+        returns its name and the names for all synonyms for the taxon. These may
+        all be returned either as Pandas DataFrames or in dictionary representations.
+        """
         match = self.taxa[self.taxa["nameID"] == nameID]
         if match.empty:
             match = self.synonyms[self.synonyms["nameID"] == nameID]
             if match.empty:
                 return None, None
             if len(match.index) > 1:
                 logging.warn(f"Multiple synonyms for name {nameID}")
@@ -2044,15 +2269,26 @@
         else:
             synonymy = self.names[self.names["ID"].isin(synonyms["nameID"])]
             if to_dict:
                 synonymy = synonymy.to_dict("records")
 
         return accepted, synonymy
 
-    def get_children(self, taxonID, to_dict=False):
+    def get_children(
+        self, taxonID: str, to_dict: bool = False
+    ) -> pd.DataFrame | list[dict[str:str]]:
+        """
+        Get all child taxa for the COLDP Taxon associated with the supplied taxonID
+
+        :param taxonID: String ID for COLDP Taxon record
+        :param to_dict: True if records should be converted from Pandas format to dictionary records, False (default) otherwise.
+        :return: Set of COLDP Taxon records for children of identified taxon either as DataFrame or list of dictionaries
+
+        Returns all matching records as Pandas DataFrame or list of dictionaries. If no matches, None is returned.
+        """
         match = self.taxa[self.taxa["parentID"] == taxonID]
         if match.empty:
             return None
         if to_dict:
             return match.to_dict("records")
         return match
 
@@ -2245,20 +2481,25 @@
         return "rank" in name and name["rank"] in [
             "variety",
             "subvariety",
             "form",
             "aberration",
         ]
 
-    def save(self, destination=None, name=None):
+    def save(self, destination: str = None, name: str = None) -> None:
         """
         Write dataframes as COLDP CSV files
 
-        Behaviour:
-        Ensure that <folder>/<name>/ exists and write all dataframes as CSV.
+        :param destination: Path to folder in which package should be saved. Defaults to destination supplied to constructor, which defaults to "."
+        :param name: Name for COLDP package (subfolder name). Defaults to name supplied to constructor, which defaults to None. If no name provided, save will fail.
+
+        If necessary creates subfolder with name :paramref:`~coldp.COLDP.save.name`
+        in :paramref:`~coldp.COLDP.save.destination`, and then writes CSV file
+        representations for all DataFrames in the folder. Empty columns are dropped.
+        Any numpy NAN elements are replaced with an empty string.
         """
 
         if destination is None:
             destination = self.folder
         if destination is None or not os.path.exists(destination):
             logging.critical(
                 f"Can't save package. Folder does not exist: {destination}"
@@ -2286,15 +2527,28 @@
                 value.dropna(how="all", axis=1, inplace=True)
                 value.replace(np.nan, "", inplace=True)
                 file_name = os.path.join(coldp_folder, item + ".csv")
                 value.to_csv(file_name, index=False)
         logging.info("COLDP saved to " + coldp_folder)
         return
 
-    def issue(self, message):
+    def issue(self, message: str) -> None:
+        """
+        Log issue with data provided through methods
+
+        :param message: Text to be saved as body of issue
+
+        Creates a new record in an issues DataFrame that will be included in the
+        COLDP export when :py:func:`~coldp.COLDP.save` is called. This record includes
+        the message and the context string supplied on the most recent call to
+        :py:func:`~coldp.COLDP.set_context`.
+
+        If :paramref:`~coldp.COLDP.__init__.issues_to_stdout` is True, the context and message
+        are also output as an error via logging.
+        """
         if self.issues is None:
             self.issues = pd.DataFrame(columns=issues_headings)
 
         context = self.context if self.context else ""
         issue_record = {"issue": message, "context": context}
 
         if self.issues_to_stdout:
```

### Comparing `coldp-2024.5.2/src/coldp/coldp_distribution.py` & `coldp-2024.5.3/src/coldp/coldp_distribution.py`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.2/src/coldp/testit.py` & `coldp-2024.5.3/src/coldp/testit.py`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.2/test/input/Tonzidae/NameUsage.tsv` & `coldp-2024.5.3/test/input/Tonzidae/NameUsage.tsv`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.2/test/input/Tonzidae/Reference.tsv` & `coldp-2024.5.3/test/input/Tonzidae/Reference.tsv`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.2/test/input/Tonzidae/logo.png` & `coldp-2024.5.3/test/input/Tonzidae/logo.png`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.2/test/input/Tonzidae/metadata.yaml` & `coldp-2024.5.3/test/input/Tonzidae/metadata.yaml`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.2/LICENSE` & `coldp-2024.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `coldp-2024.5.2/README.md` & `coldp-2024.5.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 # py-coldp
  Python tools for working with taxonomic checklists organised as Catalogue of Life Data Package (COLDP) format
 
 # Overview
 py-coldp is a Python package to facilitate creation, manipulation, editing and serialisation of taxonomic checklists in the [Catalogue of Life Data Package](https://github.com/CatalogueOfLife/coldp ) format.
 
 The package includes two classes:
-* **[COLDP](#class-coldp)** - A COLDP package loaded as a set of Pandas dataframes
-* **[NameBundle](#class-namebundle)** - A helper class to simplify addition of taxon names with sets of associated synonyms to a COLDP instance
+* **COLDP** - A COLDP package loaded as a set of Pandas dataframes
+* **NameBundle** - A helper class to simplify addition of taxon names with sets of associated synonyms to a COLDP instance
 
 # Class: COLDP
 The main **COLDP** class instantiates a COLDP package in memory as a set of Pandas dataframes. An instance may be initialised from the contents of a folder containing a set of COLDP-compliant CSV or tab-delimited data files or alternatively can be initialised as an empty instance in memory. The class includes many methods for inserting new data, editing existing records and querying the contents of the package. The instance can then be saved as a set of CSV files in a named folder .
 
 # Class: NameBundle
 
 The **NameBundle** class brings together a scientific name and its synonyms so that these can be added together and the COLDP package can automatically manage their relationships NameBundle objects are normally created using the COLDP.**start_name_bundle()** method. 
 
 At minimum a NameBundle is initialised with a dictionary holding a set of COLDP name record values. The scientific name represented by this dictionary should be the accepted name for a species or other taxon. Synonyms may then be added to the NameBundle. 
 
 Once all names are included, the NameBundle can be added to the COLDP object via the COLDP.**add_names()** method. This adds name, taxon and synonym records for the set of names supplied. COLDP options may expand the set of added synonyms to include variant formats or may trigger the addition of one or taxa that are implicit in the accepted name. 
 
-The COLDP object will automatically manage record identifiers and the basionymID for any name records that are combinations of another name in the set.
+The COLDP object will automatically manage record identifiers and the basionymID for any name records that are combinations of another name in the set.
+
+# Installation
+```console
+pip install py-coldp
+```
+
+# Documentation
+[Browsable documentation for COLDP version: 2024.5.3](https://html-preview.github.io/?url=https://github.com/dhobern/py-coldp/blob/main/docs/build/html/index.html)
+
+[PDF documentation for COLDP version: 2024.5.3](https://github.com/dhobern/py-coldp/blob/main/docs/build/simplepdf/COLDP.pdf)
```

### Comparing `coldp-2024.5.2/pyproject.toml` & `coldp-2024.5.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "coldp"
-version = "2024.5.2"
+version = "2024.5.3"
 authors = [
   { name="Donald Hobern", email="dhobern@gmail.com" },
 ]
 description = "Python tools for working with taxonomic checklists organised as Catalogue of Life Data Package (COLDP) format"
 keywords = ["Catalogue of Life", "COLDP", "taxonomic checklist"]
 readme = "README.md"
 requires-python = ">=3.8"
@@ -28,10 +28,13 @@
 Homepage = "https://github.com/dhobern/py-coldp"
 Issues = "https://github.com/dhobern/py-coldp/issues"
 
 [project.optional-dependencies]
 doc = [
     "sphinx", "sphinx-paramlinks"
 ]
+test = [
+    "pytest"
+]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/coldp"]
```

### Comparing `coldp-2024.5.2/PKG-INFO` & `coldp-2024.5.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: coldp
-Version: 2024.5.2
+Version: 2024.5.3
 Summary: Python tools for working with taxonomic checklists organised as Catalogue of Life Data Package (COLDP) format
 Project-URL: Homepage, https://github.com/dhobern/py-coldp
 Project-URL: Issues, https://github.com/dhobern/py-coldp/issues
 Author-email: Donald Hobern <dhobern@gmail.com>
 License: MIT License
         
         Copyright (c) [2024] [Donald Hobern]
@@ -34,31 +34,43 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: numpy
 Requires-Dist: pandas
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == 'doc'
 Requires-Dist: sphinx-paramlinks; extra == 'doc'
+Provides-Extra: test
+Requires-Dist: pytest; extra == 'test'
 Description-Content-Type: text/markdown
 
 # py-coldp
  Python tools for working with taxonomic checklists organised as Catalogue of Life Data Package (COLDP) format
 
 # Overview
 py-coldp is a Python package to facilitate creation, manipulation, editing and serialisation of taxonomic checklists in the [Catalogue of Life Data Package](https://github.com/CatalogueOfLife/coldp ) format.
 
 The package includes two classes:
-* **[COLDP](#class-coldp)** - A COLDP package loaded as a set of Pandas dataframes
-* **[NameBundle](#class-namebundle)** - A helper class to simplify addition of taxon names with sets of associated synonyms to a COLDP instance
+* **COLDP** - A COLDP package loaded as a set of Pandas dataframes
+* **NameBundle** - A helper class to simplify addition of taxon names with sets of associated synonyms to a COLDP instance
 
 # Class: COLDP
 The main **COLDP** class instantiates a COLDP package in memory as a set of Pandas dataframes. An instance may be initialised from the contents of a folder containing a set of COLDP-compliant CSV or tab-delimited data files or alternatively can be initialised as an empty instance in memory. The class includes many methods for inserting new data, editing existing records and querying the contents of the package. The instance can then be saved as a set of CSV files in a named folder .
 
 # Class: NameBundle
 
 The **NameBundle** class brings together a scientific name and its synonyms so that these can be added together and the COLDP package can automatically manage their relationships NameBundle objects are normally created using the COLDP.**start_name_bundle()** method. 
 
 At minimum a NameBundle is initialised with a dictionary holding a set of COLDP name record values. The scientific name represented by this dictionary should be the accepted name for a species or other taxon. Synonyms may then be added to the NameBundle. 
 
 Once all names are included, the NameBundle can be added to the COLDP object via the COLDP.**add_names()** method. This adds name, taxon and synonym records for the set of names supplied. COLDP options may expand the set of added synonyms to include variant formats or may trigger the addition of one or taxa that are implicit in the accepted name. 
 
-The COLDP object will automatically manage record identifiers and the basionymID for any name records that are combinations of another name in the set.
+The COLDP object will automatically manage record identifiers and the basionymID for any name records that are combinations of another name in the set.
+
+# Installation
+```console
+pip install py-coldp
+```
+
+# Documentation
+[Browsable documentation for COLDP version: 2024.5.3](https://html-preview.github.io/?url=https://github.com/dhobern/py-coldp/blob/main/docs/build/html/index.html)
+
+[PDF documentation for COLDP version: 2024.5.3](https://github.com/dhobern/py-coldp/blob/main/docs/build/simplepdf/COLDP.pdf)
```

