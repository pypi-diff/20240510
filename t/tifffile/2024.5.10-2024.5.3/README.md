# Comparing `tmp/tifffile-2024.5.10.tar.gz` & `tmp/tifffile-2024.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tifffile-2024.5.10.tar", last modified: Fri May 10 05:18:31 2024, max compression
+gzip compressed data, was "tifffile-2024.5.3.tar", last modified: Sat May  4 00:45:36 2024, max compression
```

## Comparing `tifffile-2024.5.10.tar` & `tifffile-2024.5.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 05:18:31.015422 tifffile-2024.5.10/
--rw-rw-rw-   0        0        0      324 2019-07-10 16:43:27.000000 tifffile-2024.5.10/ACKNOWLEDGEMENTS.rst
--rw-rw-rw-   0        0        0    38254 2024-05-10 05:18:29.000000 tifffile-2024.5.10/CHANGES.rst
--rw-rw-rw-   0        0        0     1559 2024-05-10 05:18:29.000000 tifffile-2024.5.10/LICENSE
--rw-rw-rw-   0        0        0      569 2023-08-11 02:48:51.000000 tifffile-2024.5.10/MANIFEST.in
--rw-rw-rw-   0        0        0    32037 2024-05-10 05:18:31.014422 tifffile-2024.5.10/PKG-INFO
--rw-rw-rw-   0        0        0    30795 2024-05-10 05:18:29.000000 tifffile-2024.5.10/README.rst
-drwxrwxrwx   0        0        0        0 2024-05-10 05:18:31.005924 tifffile-2024.5.10/docs/
-drwxrwxrwx   0        0        0        0 2024-05-10 05:18:31.005924 tifffile-2024.5.10/docs/_static/
--rw-rw-rw-   0        0        0      127 2022-05-28 19:33:31.000000 tifffile-2024.5.10/docs/_static/custom.css
--rw-rw-rw-   0        0        0     1098 2023-12-25 06:05:35.000000 tifffile-2024.5.10/docs/conf.py
--rw-rw-rw-   0        0        0     3644 2023-08-12 18:29:44.000000 tifffile-2024.5.10/docs/make.py
-drwxrwxrwx   0        0        0        0 2024-05-10 05:18:31.006915 tifffile-2024.5.10/examples/
--rw-rw-rw-   0        0        0    15113 2024-02-12 18:46:43.000000 tifffile-2024.5.10/examples/earthbigdata.py
--rw-rw-rw-   0        0        0     2542 2024-01-28 18:02:54.000000 tifffile-2024.5.10/examples/issue125.py
--rw-rw-rw-   0        0        0       42 2024-05-10 05:18:31.015422 tifffile-2024.5.10/setup.cfg
--rw-rw-rw-   0        0        0     3936 2023-10-18 16:48:53.000000 tifffile-2024.5.10/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-10 05:18:31.006915 tifffile-2024.5.10/tests/
--rw-rw-rw-   0        0        0     1591 2024-05-04 00:43:50.000000 tifffile-2024.5.10/tests/conftest.py
--rw-rw-rw-   0        0        0   753978 2024-05-10 04:36:24.000000 tifffile-2024.5.10/tests/test_tifffile.py
-drwxrwxrwx   0        0        0        0 2024-05-10 05:18:31.011422 tifffile-2024.5.10/tifffile/
--rw-rw-rw-   0        0        0      110 2024-01-28 01:29:32.000000 tifffile-2024.5.10/tifffile/__init__.py
--rw-rw-rw-   0        0        0      135 2020-01-01 02:31:36.000000 tifffile-2024.5.10/tifffile/__main__.py
--rw-rw-rw-   0        0        0    11863 2024-05-10 05:11:16.000000 tifffile-2024.5.10/tifffile/_imagecodecs.py
--rw-rw-rw-   0        0        0    61794 2023-07-03 00:17:39.000000 tifffile-2024.5.10/tifffile/geodb.py
--rw-rw-rw-   0        0        0      680 2023-07-03 00:17:47.000000 tifffile-2024.5.10/tifffile/lsm2bin.py
--rw-rw-rw-   0        0        0     5904 2024-01-29 17:41:17.000000 tifffile-2024.5.10/tifffile/numcodecs.py
--rw-rw-rw-   0        0        0        0 2023-08-11 00:10:50.000000 tifffile-2024.5.10/tifffile/py.typed
--rw-rw-rw-   0        0        0     2410 2023-07-03 00:18:03.000000 tifffile-2024.5.10/tifffile/tiff2fsspec.py
--rw-rw-rw-   0        0        0     1437 2023-07-03 00:18:11.000000 tifffile-2024.5.10/tifffile/tiffcomment.py
--rw-rw-rw-   0        0        0   891047 2024-05-10 05:16:14.000000 tifffile-2024.5.10/tifffile/tifffile.py
-drwxrwxrwx   0        0        0        0 2024-05-10 05:18:31.014422 tifffile-2024.5.10/tifffile.egg-info/
--rw-rw-rw-   0        0        0    32037 2024-05-10 05:18:30.000000 tifffile-2024.5.10/tifffile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      617 2024-05-10 05:18:30.000000 tifffile-2024.5.10/tifffile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 05:18:30.000000 tifffile-2024.5.10/tifffile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      155 2024-05-10 05:18:30.000000 tifffile-2024.5.10/tifffile.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       75 2024-05-10 05:18:30.000000 tifffile-2024.5.10/tifffile.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-10 05:18:30.000000 tifffile-2024.5.10/tifffile.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 00:45:36.153592 tifffile-2024.5.3/
+-rw-rw-rw-   0        0        0      324 2019-07-10 16:43:27.000000 tifffile-2024.5.3/ACKNOWLEDGEMENTS.rst
+-rw-rw-rw-   0        0        0    38141 2024-05-04 00:45:34.000000 tifffile-2024.5.3/CHANGES.rst
+-rw-rw-rw-   0        0        0     1559 2024-05-04 00:45:34.000000 tifffile-2024.5.3/LICENSE
+-rw-rw-rw-   0        0        0      569 2023-08-11 02:48:51.000000 tifffile-2024.5.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    31893 2024-05-04 00:45:36.153592 tifffile-2024.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0    30652 2024-05-04 00:45:34.000000 tifffile-2024.5.3/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-04 00:45:36.153592 tifffile-2024.5.3/docs/
+drwxrwxrwx   0        0        0        0 2024-05-04 00:45:36.153592 tifffile-2024.5.3/docs/_static/
+-rw-rw-rw-   0        0        0      127 2022-05-28 19:33:31.000000 tifffile-2024.5.3/docs/_static/custom.css
+-rw-rw-rw-   0        0        0     1098 2023-12-25 06:05:35.000000 tifffile-2024.5.3/docs/conf.py
+-rw-rw-rw-   0        0        0     3644 2023-08-12 18:29:44.000000 tifffile-2024.5.3/docs/make.py
+drwxrwxrwx   0        0        0        0 2024-05-04 00:45:36.153592 tifffile-2024.5.3/examples/
+-rw-rw-rw-   0        0        0    15113 2024-02-12 18:46:43.000000 tifffile-2024.5.3/examples/earthbigdata.py
+-rw-rw-rw-   0        0        0     2542 2024-01-28 18:02:54.000000 tifffile-2024.5.3/examples/issue125.py
+-rw-rw-rw-   0        0        0       42 2024-05-04 00:45:36.153592 tifffile-2024.5.3/setup.cfg
+-rw-rw-rw-   0        0        0     3936 2023-10-18 16:48:53.000000 tifffile-2024.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 00:45:36.153592 tifffile-2024.5.3/tests/
+-rw-rw-rw-   0        0        0     1591 2024-05-04 00:43:50.000000 tifffile-2024.5.3/tests/conftest.py
+-rw-rw-rw-   0        0        0   751633 2024-05-04 00:13:02.000000 tifffile-2024.5.3/tests/test_tifffile.py
+drwxrwxrwx   0        0        0        0 2024-05-04 00:45:36.153592 tifffile-2024.5.3/tifffile/
+-rw-rw-rw-   0        0        0      110 2024-01-28 01:29:32.000000 tifffile-2024.5.3/tifffile/__init__.py
+-rw-rw-rw-   0        0        0      135 2020-01-01 02:31:36.000000 tifffile-2024.5.3/tifffile/__main__.py
+-rw-rw-rw-   0        0        0    11865 2024-04-25 00:49:56.000000 tifffile-2024.5.3/tifffile/_imagecodecs.py
+-rw-rw-rw-   0        0        0    61794 2023-07-03 00:17:39.000000 tifffile-2024.5.3/tifffile/geodb.py
+-rw-rw-rw-   0        0        0      680 2023-07-03 00:17:47.000000 tifffile-2024.5.3/tifffile/lsm2bin.py
+-rw-rw-rw-   0        0        0     5904 2024-01-29 17:41:17.000000 tifffile-2024.5.3/tifffile/numcodecs.py
+-rw-rw-rw-   0        0        0        0 2023-08-11 00:10:50.000000 tifffile-2024.5.3/tifffile/py.typed
+-rw-rw-rw-   0        0        0     2410 2023-07-03 00:18:03.000000 tifffile-2024.5.3/tifffile/tiff2fsspec.py
+-rw-rw-rw-   0        0        0     1437 2023-07-03 00:18:11.000000 tifffile-2024.5.3/tifffile/tiffcomment.py
+-rw-rw-rw-   0        0        0   890009 2024-05-04 00:45:12.000000 tifffile-2024.5.3/tifffile/tifffile.py
+drwxrwxrwx   0        0        0        0 2024-05-04 00:45:36.153592 tifffile-2024.5.3/tifffile.egg-info/
+-rw-rw-rw-   0        0        0    31893 2024-05-04 00:45:35.000000 tifffile-2024.5.3/tifffile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      617 2024-05-04 00:45:36.000000 tifffile-2024.5.3/tifffile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 00:45:35.000000 tifffile-2024.5.3/tifffile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      155 2024-05-04 00:45:35.000000 tifffile-2024.5.3/tifffile.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       75 2024-05-04 00:45:35.000000 tifffile-2024.5.3/tifffile.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-04 00:45:35.000000 tifffile-2024.5.3/tifffile.egg-info/top_level.txt
```

### Comparing `tifffile-2024.5.10/CHANGES.rst` & `tifffile-2024.5.3/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 Revisions
 ---------
 
-2024.5.10
-
-- Pass 5082 tests.
-- Support reading JPEGXL compression in DNG 1.7.
-- Read invalid TIFF created by IDEAS software.
-
 2024.5.3
 
+- Pass 5080 tests.
 - Fix reading incompletely written LSM.
 - Fix reading Philips DP with extra rows of tiles (#253, breaking).
 
 2024.4.24
 
 - Fix compatibility issue with numpy 2 (#252).
```

### Comparing `tifffile-2024.5.10/LICENSE` & `tifffile-2024.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tifffile-2024.5.10/MANIFEST.in` & `tifffile-2024.5.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `tifffile-2024.5.10/PKG-INFO` & `tifffile-2024.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tifffile
-Version: 2024.5.10
+Version: 2024.5.3
 Summary: Read and write TIFF files
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/tifffile/issues
 Project-URL: Source Code, https://github.com/cgohlke/tifffile
@@ -59,15 +59,15 @@
 Tifffile can also be used to inspect TIFF structures, read image data from
 multi-dimensional file sequences, write fsspec ReferenceFileSystem for
 TIFF files and image file sequences, patch TIFF tag values, and parse
 many proprietary metadata formats.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.5.10
+:Version: 2024.5.3
 :DOI: `10.5281/zenodo.6795860 <https://doi.org/10.5281/zenodo.6795860>`_
 
 Quickstart
 ----------
 
 Install the tifffile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/tifffile/>`_::
@@ -103,30 +103,25 @@
 - `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
 - `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2024.1.1
   (required for encoding or decoding LZW, JPEG, etc. compressed segments)
 - `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.4
   (required for plotting)
 - `Lxml <https://pypi.org/project/lxml/>`_ 5.2.1
   (required only for validating and printing XML)
-- `Zarr <https://pypi.org/project/zarr/>`_ 2.18.0
+- `Zarr <https://pypi.org/project/zarr/>`_ 2.17.2
   (required only for opening Zarr stores)
 - `Fsspec <https://pypi.org/project/fsspec/>`_ 2024.3.1
   (required only for opening ReferenceFileSystem files)
 
 Revisions
 ---------
 
-2024.5.10
-
-- Pass 5082 tests.
-- Support reading JPEGXL compression in DNG 1.7.
-- Read invalid TIFF created by IDEAS software.
-
 2024.5.3
 
+- Pass 5080 tests.
 - Fix reading incompletely written LSM.
 - Fix reading Philips DP with extra rows of tiles (#253, breaking).
 
 2024.4.24
 
 - Fix compatibility issue with numpy 2 (#252).
 
@@ -418,16 +413,16 @@
 - Tags for TIFF and Related Specifications. Digital Preservation.
   https://www.loc.gov/preservation/digital/formats/content/tiff_tags.shtml
 - CIPA DC-008-2016: Exchangeable image file format for digital still cameras:
   Exif Version 2.31.
   http://www.cipa.jp/std/documents/e/DC-008-Translation-2016-E.pdf
 - The EER (Electron Event Representation) file format.
   https://github.com/fei-company/EerReaderLib
-- Digital Negative (DNG) Specification. Version 1.7.1.0, September 2023.
-  https://helpx.adobe.com/content/dam/help/en/photoshop/pdf/DNG_Spec_1_7_1_0.pdf
+- Digital Negative (DNG) Specification. Version 1.5.0.0, June 2012.
+  https://www.adobe.com/content/dam/acom/en/products/photoshop/pdfs/dng_spec_1.5.0.0.pdf
 - Roche Digital Pathology. BIF image file format for digital pathology.
   https://diagnostics.roche.com/content/dam/diagnostics/Blueprint/en/pdf/rmd/Roche-Digital-Pathology-BIF-Whitepaper.pdf
 - Astro-TIFF specification. https://astro-tiff.sourceforge.io/
 - Aperio Technologies, Inc. Digital Slides and Third-Party Data Interchange.
   Aperio_Digital_Slides_and_Third-party_data_interchange.pdf
 - PerkinElmer image format.
   https://downloads.openmicroscopy.org/images/Vectra-QPTIFF/perkinelmer/PKI_Image%20Format.docx
@@ -487,15 +482,14 @@
 (18, 301, 219)
 
 Iterate over all pages in the TIFF file and successively read images:
 
 >>> with TiffFile('temp.tif') as tif:
 ...     for page in tif.pages:
 ...         image = page.asarray()
-...
 
 Get information about the image stack in the TIFF file without reading
 any image data:
 
 >>> tif = TiffFile('temp.tif')
 >>> len(tif.pages)  # number of pages in the file
 64
@@ -515,15 +509,14 @@
 'QYX'
 >>> tif.close()
 
 Inspect the "XResolution" tag from the first page in the TIFF file:
 
 >>> with TiffFile('temp.tif') as tif:
 ...     tag = tif.pages[0].tags['XResolution']
-...
 >>> tag.value
 (1, 1)
 >>> tag.name
 'XResolution'
 >>> tag.code
 282
 >>> tag.count
@@ -533,21 +526,19 @@
 
 Iterate over all tags in the TIFF file:
 
 >>> with TiffFile('temp.tif') as tif:
 ...     for page in tif.pages:
 ...         for tag in page.tags:
 ...             tag_name, tag_value = tag.name, tag.value
-...
 
 Overwrite the value of an existing tag, for example, XResolution:
 
 >>> with TiffFile('temp.tif', mode='r+') as tif:
 ...     _ = tif.pages[0].tags['XResolution'].overwrite((96000, 1000))
-...
 
 Write a 5-dimensional floating-point array using BigTIFF format, separate
 color components, tiling, Zlib compression level 8, horizontal differencing
 predictor, and additional metadata:
 
 >>> data = numpy.random.rand(2, 5, 3, 301, 219).astype('float32')
 >>> imwrite(
@@ -556,44 +547,43 @@
 ...     bigtiff=True,
 ...     photometric='rgb',
 ...     planarconfig='separate',
 ...     tile=(32, 32),
 ...     compression='zlib',
 ...     compressionargs={'level': 8},
 ...     predictor=True,
-...     metadata={'axes': 'TZCYX'},
+...     metadata={'axes': 'TZCYX'}
 ... )
 
 Write a 10 fps time series of volumes with xyz voxel size 2.6755x2.6755x3.9474
 micron^3 to an ImageJ hyperstack formatted TIFF file:
 
 >>> volume = numpy.random.randn(6, 57, 256, 256).astype('float32')
 >>> image_labels = [f'{i}' for i in range(volume.shape[0] * volume.shape[1])]
 >>> imwrite(
 ...     'temp.tif',
 ...     volume,
 ...     imagej=True,
-...     resolution=(1.0 / 2.6755, 1.0 / 2.6755),
+...     resolution=(1./2.6755, 1./2.6755),
 ...     metadata={
 ...         'spacing': 3.947368,
 ...         'unit': 'um',
-...         'finterval': 1 / 10,
+...         'finterval': 1/10,
 ...         'fps': 10.0,
 ...         'axes': 'TZYX',
 ...         'Labels': image_labels,
-...     },
+...     }
 ... )
 
 Read the volume and metadata from the ImageJ hyperstack file:
 
 >>> with TiffFile('temp.tif') as tif:
 ...     volume = tif.asarray()
 ...     axes = tif.series[0].axes
 ...     imagej_metadata = tif.imagej_metadata
-...
 >>> volume.shape
 (6, 57, 256, 256)
 >>> axes
 'TZYX'
 >>> imagej_metadata['slices']
 57
 >>> imagej_metadata['frames']
@@ -606,15 +596,18 @@
 (6, 57, 256, 256)
 >>> del memmap_volume
 
 Create a TIFF file containing an empty image and write to the memory-mapped
 NumPy array (note: this does not work with compression or tiling):
 
 >>> memmap_image = memmap(
-...     'temp.tif', shape=(256, 256, 3), dtype='float32', photometric='rgb'
+...     'temp.tif',
+...     shape=(256, 256, 3),
+...     dtype='float32',
+...     photometric='rgb'
 ... )
 >>> type(memmap_image)
 <class 'numpy.memmap'>
 >>> memmap_image[255, 255, 1] = 1.0
 >>> memmap_image.flush()
 >>> del memmap_image
 
@@ -623,127 +616,121 @@
 interoperability):
 
 >>> series0 = numpy.random.randint(0, 255, (32, 32, 3), 'uint8')
 >>> series1 = numpy.random.randint(0, 255, (4, 256, 256), 'uint16')
 >>> with TiffWriter('temp.tif') as tif:
 ...     tif.write(series0, photometric='rgb')
 ...     tif.write(series1, photometric='minisblack')
-...
 
 Read the second image series from the TIFF file:
 
 >>> series1 = imread('temp.tif', series=1)
 >>> series1.shape
 (4, 256, 256)
 
 Successively write the frames of one contiguous series to a TIFF file:
 
 >>> data = numpy.random.randint(0, 255, (30, 301, 219), 'uint8')
 >>> with TiffWriter('temp.tif') as tif:
 ...     for frame in data:
 ...         tif.write(frame, contiguous=True)
-...
 
 Append an image series to the existing TIFF file (note: this does not work
 with ImageJ hyperstack or OME-TIFF files):
 
 >>> data = numpy.random.randint(0, 255, (301, 219, 3), 'uint8')
 >>> imwrite('temp.tif', data, photometric='rgb', append=True)
 
 Create a TIFF file from a generator of tiles:
 
 >>> data = numpy.random.randint(0, 2**12, (31, 33, 3), 'uint16')
 >>> def tiles(data, tileshape):
 ...     for y in range(0, data.shape[0], tileshape[0]):
 ...         for x in range(0, data.shape[1], tileshape[1]):
 ...             yield data[y : y + tileshape[0], x : x + tileshape[1]]
-...
 >>> imwrite(
 ...     'temp.tif',
 ...     tiles(data, (16, 16)),
 ...     tile=(16, 16),
 ...     shape=data.shape,
 ...     dtype=data.dtype,
-...     photometric='rgb',
+...     photometric='rgb'
 ... )
 
 Write a multi-dimensional, multi-resolution (pyramidal), multi-series OME-TIFF
 file with metadata. Sub-resolution images are written to SubIFDs. Limit
 parallel encoding to 2 threads. Write a thumbnail image as a separate image
 series:
 
 >>> data = numpy.random.randint(0, 255, (8, 2, 512, 512, 3), 'uint8')
 >>> subresolutions = 2
 >>> pixelsize = 0.29  # micrometer
 >>> with TiffWriter('temp.ome.tif', bigtiff=True) as tif:
-...     metadata = {
+...     metadata={
 ...         'axes': 'TCYXS',
 ...         'SignificantBits': 8,
 ...         'TimeIncrement': 0.1,
 ...         'TimeIncrementUnit': 's',
 ...         'PhysicalSizeX': pixelsize,
 ...         'PhysicalSizeXUnit': 'µm',
 ...         'PhysicalSizeY': pixelsize,
 ...         'PhysicalSizeYUnit': 'µm',
 ...         'Channel': {'Name': ['Channel 1', 'Channel 2']},
-...         'Plane': {'PositionX': [0.0] * 16, 'PositionXUnit': ['µm'] * 16},
+...         'Plane': {'PositionX': [0.0] * 16, 'PositionXUnit': ['µm'] * 16}
 ...     }
 ...     options = dict(
 ...         photometric='rgb',
 ...         tile=(128, 128),
 ...         compression='jpeg',
 ...         resolutionunit='CENTIMETER',
-...         maxworkers=2,
+...         maxworkers=2
 ...     )
 ...     tif.write(
 ...         data,
 ...         subifds=subresolutions,
 ...         resolution=(1e4 / pixelsize, 1e4 / pixelsize),
 ...         metadata=metadata,
-...         **options,
+...         **options
 ...     )
 ...     # write pyramid levels to the two subifds
 ...     # in production use resampling to generate sub-resolution images
 ...     for level in range(subresolutions):
-...         mag = 2 ** (level + 1)
+...         mag = 2**(level + 1)
 ...         tif.write(
 ...             data[..., ::mag, ::mag, :],
 ...             subfiletype=1,
 ...             resolution=(1e4 / mag / pixelsize, 1e4 / mag / pixelsize),
-...             **options,
+...             **options
 ...         )
 ...     # add a thumbnail image as a separate series
 ...     # it is recognized by QuPath as an associated image
 ...     thumbnail = (data[0, 0, ::8, ::8] >> 2).astype('uint8')
 ...     tif.write(thumbnail, metadata={'Name': 'thumbnail'})
-...
 
 Access the image levels in the pyramidal OME-TIFF file:
 
 >>> baseimage = imread('temp.ome.tif')
 >>> second_level = imread('temp.ome.tif', series=0, level=1)
 >>> with TiffFile('temp.ome.tif') as tif:
 ...     baseimage = tif.series[0].asarray()
 ...     second_level = tif.series[0].levels[1].asarray()
-...
 
 Iterate over and decode single JPEG compressed tiles in the TIFF file:
 
 >>> with TiffFile('temp.ome.tif') as tif:
 ...     fh = tif.filehandle
 ...     for page in tif.pages:
 ...         for index, (offset, bytecount) in enumerate(
 ...             zip(page.dataoffsets, page.databytecounts)
 ...         ):
 ...             _ = fh.seek(offset)
 ...             data = fh.read(bytecount)
 ...             tile, indices, shape = page.decode(
 ...                 data, index, jpegtables=page.jpegtables
 ...             )
-...
 
 Use Zarr to read parts of the tiled, pyramidal images in the TIFF file:
 
 >>> import zarr
 >>> store = imread('temp.ome.tif', aszarr=True)
 >>> z = zarr.open(store, mode='r')
 >>> z
@@ -785,15 +772,15 @@
 
 >>> imwrite(
 ...     'temp.ome.tif',
 ...     shape=(8, 800, 600),
 ...     dtype='uint16',
 ...     photometric='minisblack',
 ...     tile=(128, 128),
-...     metadata={'axes': 'CYX'},
+...     metadata={'axes': 'CYX'}
 ... )
 >>> store = imread('temp.ome.tif', mode='r+', aszarr=True)
 >>> z = zarr.open(store, mode='r+')
 >>> z
 <zarr.core.Array (8, 800, 600) uint16>
 >>> z[3, 100:200, 200:300:2] = 1024
 >>> store.close()
@@ -810,15 +797,17 @@
 (2, 64, 64)
 >>> image_sequence.dtype
 dtype('float64')
 
 Read an image stack from a series of TIFF files with a file name pattern
 as NumPy or Zarr arrays:
 
->>> image_sequence = TiffSequence('temp_C0*.tif', pattern=r'_(C)(\d+)(T)(\d+)')
+>>> image_sequence = TiffSequence(
+...     'temp_C0*.tif', pattern=r'_(C)(\d+)(T)(\d+)'
+... )
 >>> image_sequence.shape
 (1, 2)
 >>> image_sequence.axes
 'CT'
 >>> data = image_sequence.asarray()
 >>> data.shape
 (1, 2, 64, 64)
```

### Comparing `tifffile-2024.5.10/README.rst` & `tifffile-2024.5.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 Tifffile can also be used to inspect TIFF structures, read image data from
 multi-dimensional file sequences, write fsspec ReferenceFileSystem for
 TIFF files and image file sequences, patch TIFF tag values, and parse
 many proprietary metadata formats.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.5.10
+:Version: 2024.5.3
 :DOI: `10.5281/zenodo.6795860 <https://doi.org/10.5281/zenodo.6795860>`_
 
 Quickstart
 ----------
 
 Install the tifffile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/tifffile/>`_::
@@ -70,30 +70,25 @@
 - `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
 - `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2024.1.1
   (required for encoding or decoding LZW, JPEG, etc. compressed segments)
 - `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.4
   (required for plotting)
 - `Lxml <https://pypi.org/project/lxml/>`_ 5.2.1
   (required only for validating and printing XML)
-- `Zarr <https://pypi.org/project/zarr/>`_ 2.18.0
+- `Zarr <https://pypi.org/project/zarr/>`_ 2.17.2
   (required only for opening Zarr stores)
 - `Fsspec <https://pypi.org/project/fsspec/>`_ 2024.3.1
   (required only for opening ReferenceFileSystem files)
 
 Revisions
 ---------
 
-2024.5.10
-
-- Pass 5082 tests.
-- Support reading JPEGXL compression in DNG 1.7.
-- Read invalid TIFF created by IDEAS software.
-
 2024.5.3
 
+- Pass 5080 tests.
 - Fix reading incompletely written LSM.
 - Fix reading Philips DP with extra rows of tiles (#253, breaking).
 
 2024.4.24
 
 - Fix compatibility issue with numpy 2 (#252).
 
@@ -385,16 +380,16 @@
 - Tags for TIFF and Related Specifications. Digital Preservation.
   https://www.loc.gov/preservation/digital/formats/content/tiff_tags.shtml
 - CIPA DC-008-2016: Exchangeable image file format for digital still cameras:
   Exif Version 2.31.
   http://www.cipa.jp/std/documents/e/DC-008-Translation-2016-E.pdf
 - The EER (Electron Event Representation) file format.
   https://github.com/fei-company/EerReaderLib
-- Digital Negative (DNG) Specification. Version 1.7.1.0, September 2023.
-  https://helpx.adobe.com/content/dam/help/en/photoshop/pdf/DNG_Spec_1_7_1_0.pdf
+- Digital Negative (DNG) Specification. Version 1.5.0.0, June 2012.
+  https://www.adobe.com/content/dam/acom/en/products/photoshop/pdfs/dng_spec_1.5.0.0.pdf
 - Roche Digital Pathology. BIF image file format for digital pathology.
   https://diagnostics.roche.com/content/dam/diagnostics/Blueprint/en/pdf/rmd/Roche-Digital-Pathology-BIF-Whitepaper.pdf
 - Astro-TIFF specification. https://astro-tiff.sourceforge.io/
 - Aperio Technologies, Inc. Digital Slides and Third-Party Data Interchange.
   Aperio_Digital_Slides_and_Third-party_data_interchange.pdf
 - PerkinElmer image format.
   https://downloads.openmicroscopy.org/images/Vectra-QPTIFF/perkinelmer/PKI_Image%20Format.docx
@@ -454,15 +449,14 @@
 (18, 301, 219)
 
 Iterate over all pages in the TIFF file and successively read images:
 
 >>> with TiffFile('temp.tif') as tif:
 ...     for page in tif.pages:
 ...         image = page.asarray()
-...
 
 Get information about the image stack in the TIFF file without reading
 any image data:
 
 >>> tif = TiffFile('temp.tif')
 >>> len(tif.pages)  # number of pages in the file
 64
@@ -482,15 +476,14 @@
 'QYX'
 >>> tif.close()
 
 Inspect the "XResolution" tag from the first page in the TIFF file:
 
 >>> with TiffFile('temp.tif') as tif:
 ...     tag = tif.pages[0].tags['XResolution']
-...
 >>> tag.value
 (1, 1)
 >>> tag.name
 'XResolution'
 >>> tag.code
 282
 >>> tag.count
@@ -500,21 +493,19 @@
 
 Iterate over all tags in the TIFF file:
 
 >>> with TiffFile('temp.tif') as tif:
 ...     for page in tif.pages:
 ...         for tag in page.tags:
 ...             tag_name, tag_value = tag.name, tag.value
-...
 
 Overwrite the value of an existing tag, for example, XResolution:
 
 >>> with TiffFile('temp.tif', mode='r+') as tif:
 ...     _ = tif.pages[0].tags['XResolution'].overwrite((96000, 1000))
-...
 
 Write a 5-dimensional floating-point array using BigTIFF format, separate
 color components, tiling, Zlib compression level 8, horizontal differencing
 predictor, and additional metadata:
 
 >>> data = numpy.random.rand(2, 5, 3, 301, 219).astype('float32')
 >>> imwrite(
@@ -523,44 +514,43 @@
 ...     bigtiff=True,
 ...     photometric='rgb',
 ...     planarconfig='separate',
 ...     tile=(32, 32),
 ...     compression='zlib',
 ...     compressionargs={'level': 8},
 ...     predictor=True,
-...     metadata={'axes': 'TZCYX'},
+...     metadata={'axes': 'TZCYX'}
 ... )
 
 Write a 10 fps time series of volumes with xyz voxel size 2.6755x2.6755x3.9474
 micron^3 to an ImageJ hyperstack formatted TIFF file:
 
 >>> volume = numpy.random.randn(6, 57, 256, 256).astype('float32')
 >>> image_labels = [f'{i}' for i in range(volume.shape[0] * volume.shape[1])]
 >>> imwrite(
 ...     'temp.tif',
 ...     volume,
 ...     imagej=True,
-...     resolution=(1.0 / 2.6755, 1.0 / 2.6755),
+...     resolution=(1./2.6755, 1./2.6755),
 ...     metadata={
 ...         'spacing': 3.947368,
 ...         'unit': 'um',
-...         'finterval': 1 / 10,
+...         'finterval': 1/10,
 ...         'fps': 10.0,
 ...         'axes': 'TZYX',
 ...         'Labels': image_labels,
-...     },
+...     }
 ... )
 
 Read the volume and metadata from the ImageJ hyperstack file:
 
 >>> with TiffFile('temp.tif') as tif:
 ...     volume = tif.asarray()
 ...     axes = tif.series[0].axes
 ...     imagej_metadata = tif.imagej_metadata
-...
 >>> volume.shape
 (6, 57, 256, 256)
 >>> axes
 'TZYX'
 >>> imagej_metadata['slices']
 57
 >>> imagej_metadata['frames']
@@ -573,15 +563,18 @@
 (6, 57, 256, 256)
 >>> del memmap_volume
 
 Create a TIFF file containing an empty image and write to the memory-mapped
 NumPy array (note: this does not work with compression or tiling):
 
 >>> memmap_image = memmap(
-...     'temp.tif', shape=(256, 256, 3), dtype='float32', photometric='rgb'
+...     'temp.tif',
+...     shape=(256, 256, 3),
+...     dtype='float32',
+...     photometric='rgb'
 ... )
 >>> type(memmap_image)
 <class 'numpy.memmap'>
 >>> memmap_image[255, 255, 1] = 1.0
 >>> memmap_image.flush()
 >>> del memmap_image
 
@@ -590,127 +583,121 @@
 interoperability):
 
 >>> series0 = numpy.random.randint(0, 255, (32, 32, 3), 'uint8')
 >>> series1 = numpy.random.randint(0, 255, (4, 256, 256), 'uint16')
 >>> with TiffWriter('temp.tif') as tif:
 ...     tif.write(series0, photometric='rgb')
 ...     tif.write(series1, photometric='minisblack')
-...
 
 Read the second image series from the TIFF file:
 
 >>> series1 = imread('temp.tif', series=1)
 >>> series1.shape
 (4, 256, 256)
 
 Successively write the frames of one contiguous series to a TIFF file:
 
 >>> data = numpy.random.randint(0, 255, (30, 301, 219), 'uint8')
 >>> with TiffWriter('temp.tif') as tif:
 ...     for frame in data:
 ...         tif.write(frame, contiguous=True)
-...
 
 Append an image series to the existing TIFF file (note: this does not work
 with ImageJ hyperstack or OME-TIFF files):
 
 >>> data = numpy.random.randint(0, 255, (301, 219, 3), 'uint8')
 >>> imwrite('temp.tif', data, photometric='rgb', append=True)
 
 Create a TIFF file from a generator of tiles:
 
 >>> data = numpy.random.randint(0, 2**12, (31, 33, 3), 'uint16')
 >>> def tiles(data, tileshape):
 ...     for y in range(0, data.shape[0], tileshape[0]):
 ...         for x in range(0, data.shape[1], tileshape[1]):
 ...             yield data[y : y + tileshape[0], x : x + tileshape[1]]
-...
 >>> imwrite(
 ...     'temp.tif',
 ...     tiles(data, (16, 16)),
 ...     tile=(16, 16),
 ...     shape=data.shape,
 ...     dtype=data.dtype,
-...     photometric='rgb',
+...     photometric='rgb'
 ... )
 
 Write a multi-dimensional, multi-resolution (pyramidal), multi-series OME-TIFF
 file with metadata. Sub-resolution images are written to SubIFDs. Limit
 parallel encoding to 2 threads. Write a thumbnail image as a separate image
 series:
 
 >>> data = numpy.random.randint(0, 255, (8, 2, 512, 512, 3), 'uint8')
 >>> subresolutions = 2
 >>> pixelsize = 0.29  # micrometer
 >>> with TiffWriter('temp.ome.tif', bigtiff=True) as tif:
-...     metadata = {
+...     metadata={
 ...         'axes': 'TCYXS',
 ...         'SignificantBits': 8,
 ...         'TimeIncrement': 0.1,
 ...         'TimeIncrementUnit': 's',
 ...         'PhysicalSizeX': pixelsize,
 ...         'PhysicalSizeXUnit': 'µm',
 ...         'PhysicalSizeY': pixelsize,
 ...         'PhysicalSizeYUnit': 'µm',
 ...         'Channel': {'Name': ['Channel 1', 'Channel 2']},
-...         'Plane': {'PositionX': [0.0] * 16, 'PositionXUnit': ['µm'] * 16},
+...         'Plane': {'PositionX': [0.0] * 16, 'PositionXUnit': ['µm'] * 16}
 ...     }
 ...     options = dict(
 ...         photometric='rgb',
 ...         tile=(128, 128),
 ...         compression='jpeg',
 ...         resolutionunit='CENTIMETER',
-...         maxworkers=2,
+...         maxworkers=2
 ...     )
 ...     tif.write(
 ...         data,
 ...         subifds=subresolutions,
 ...         resolution=(1e4 / pixelsize, 1e4 / pixelsize),
 ...         metadata=metadata,
-...         **options,
+...         **options
 ...     )
 ...     # write pyramid levels to the two subifds
 ...     # in production use resampling to generate sub-resolution images
 ...     for level in range(subresolutions):
-...         mag = 2 ** (level + 1)
+...         mag = 2**(level + 1)
 ...         tif.write(
 ...             data[..., ::mag, ::mag, :],
 ...             subfiletype=1,
 ...             resolution=(1e4 / mag / pixelsize, 1e4 / mag / pixelsize),
-...             **options,
+...             **options
 ...         )
 ...     # add a thumbnail image as a separate series
 ...     # it is recognized by QuPath as an associated image
 ...     thumbnail = (data[0, 0, ::8, ::8] >> 2).astype('uint8')
 ...     tif.write(thumbnail, metadata={'Name': 'thumbnail'})
-...
 
 Access the image levels in the pyramidal OME-TIFF file:
 
 >>> baseimage = imread('temp.ome.tif')
 >>> second_level = imread('temp.ome.tif', series=0, level=1)
 >>> with TiffFile('temp.ome.tif') as tif:
 ...     baseimage = tif.series[0].asarray()
 ...     second_level = tif.series[0].levels[1].asarray()
-...
 
 Iterate over and decode single JPEG compressed tiles in the TIFF file:
 
 >>> with TiffFile('temp.ome.tif') as tif:
 ...     fh = tif.filehandle
 ...     for page in tif.pages:
 ...         for index, (offset, bytecount) in enumerate(
 ...             zip(page.dataoffsets, page.databytecounts)
 ...         ):
 ...             _ = fh.seek(offset)
 ...             data = fh.read(bytecount)
 ...             tile, indices, shape = page.decode(
 ...                 data, index, jpegtables=page.jpegtables
 ...             )
-...
 
 Use Zarr to read parts of the tiled, pyramidal images in the TIFF file:
 
 >>> import zarr
 >>> store = imread('temp.ome.tif', aszarr=True)
 >>> z = zarr.open(store, mode='r')
 >>> z
@@ -752,15 +739,15 @@
 
 >>> imwrite(
 ...     'temp.ome.tif',
 ...     shape=(8, 800, 600),
 ...     dtype='uint16',
 ...     photometric='minisblack',
 ...     tile=(128, 128),
-...     metadata={'axes': 'CYX'},
+...     metadata={'axes': 'CYX'}
 ... )
 >>> store = imread('temp.ome.tif', mode='r+', aszarr=True)
 >>> z = zarr.open(store, mode='r+')
 >>> z
 <zarr.core.Array (8, 800, 600) uint16>
 >>> z[3, 100:200, 200:300:2] = 1024
 >>> store.close()
@@ -777,15 +764,17 @@
 (2, 64, 64)
 >>> image_sequence.dtype
 dtype('float64')
 
 Read an image stack from a series of TIFF files with a file name pattern
 as NumPy or Zarr arrays:
 
->>> image_sequence = TiffSequence('temp_C0*.tif', pattern=r'_(C)(\d+)(T)(\d+)')
+>>> image_sequence = TiffSequence(
+...     'temp_C0*.tif', pattern=r'_(C)(\d+)(T)(\d+)'
+... )
 >>> image_sequence.shape
 (1, 2)
 >>> image_sequence.axes
 'CT'
 >>> data = image_sequence.asarray()
 >>> data.shape
 (1, 2, 64, 64)
```

### Comparing `tifffile-2024.5.10/docs/conf.py` & `tifffile-2024.5.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.5.10/docs/make.py` & `tifffile-2024.5.3/docs/make.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.5.10/examples/earthbigdata.py` & `tifffile-2024.5.3/examples/earthbigdata.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.5.10/examples/issue125.py` & `tifffile-2024.5.3/examples/issue125.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.5.10/setup.py` & `tifffile-2024.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.5.10/tests/conftest.py` & `tifffile-2024.5.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.5.10/tests/test_tifffile.py` & `tifffile-2024.5.3/tests/test_tifffile.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 # mypy: check-untyped-defs=False
 
 """Unittests for the tifffile package.
 
 Public data files can be requested from the author.
 Private data files are not available due to size and copyright restrictions.
 
-:Version: 2024.5.10
+:Version: 2024.5.3
 
 """
 
 import binascii
 import datetime
 import glob
 import json
@@ -238,15 +238,14 @@
 LZMA = TIFF.COMPRESSION.LZMA
 ZSTD = TIFF.COMPRESSION.ZSTD
 WEBP = TIFF.COMPRESSION.WEBP
 PNG = TIFF.COMPRESSION.PNG
 LERC = TIFF.COMPRESSION.LERC
 JPEG2000 = TIFF.COMPRESSION.JPEG2000
 JPEGXL = TIFF.COMPRESSION.JPEGXL
-JPEGXL_DNG = TIFF.COMPRESSION.JPEGXL_DNG
 PACKBITS = TIFF.COMPRESSION.PACKBITS
 JPEG = TIFF.COMPRESSION.JPEG
 OJPEG = TIFF.COMPRESSION.OJPEG
 APERIO_JP2000_RGB = TIFF.COMPRESSION.APERIO_JP2000_RGB
 APERIO_JP2000_YCBC = TIFF.COMPRESSION.APERIO_JP2000_YCBC
 ADOBE_DEFLATE = TIFF.COMPRESSION.ADOBE_DEFLATE
 DEFLATE = TIFF.COMPRESSION.DEFLATE
@@ -2834,34 +2833,14 @@
             compression='zlib',
             **kwargs,
         )
         im = imread(fname, maxworkers=2, buffersize=buffersize)
     assert_array_equal(im, data)
 
 
-@pytest.mark.skipif(SKIP_PRIVATE, reason=REASON)
-def test_issue_ideas(caplog):
-    """Test reading invalid TIFF produced by IDEAS."""
-    # https://forum.image.sc/t/96103
-    # NewSubfileType tag is of type bytes
-    # FillOrder tag is zero
-    fname = private_file('IDEAS/IDEAS_file.ome.tif')
-    with TiffFile(fname) as tif:
-        assert '0 is not a valid FILLORDER' in caplog.text
-        assert 'invalid self.subfiletype=b' in caplog.text
-        assert tif.is_ome
-        page = tif.pages.first
-        assert page.tags['NewSubfileType'].value == b'\x02\x00'
-        assert page.tags['FillOrder'].value == 0
-        series = tif.series[0]
-        assert series.shape == (37, 29)
-        assert series.axes == 'YX'
-        assert_array_equal(page.asarray(), series.asarray())
-
-
 class TestExceptions:
     """Test various Exceptions and Warnings."""
 
     data = random_data(numpy.uint16, (5, 13, 17))
 
     @pytest.fixture(scope='class')
     def fname(self):
@@ -3655,15 +3634,15 @@
             assert 'None' not in tags
             assert None not in tags
             assert 'TiffTags' in repr(tags)
 
 
 def test_class_tifftagregistry():
     """Test TiffTagRegistry."""
-    numtags = 666
+    numtags = 657
     tags = TIFF.TAGS
     assert len(tags) == numtags
     assert tags[11] == 'ProcessingSoftware'
     assert tags['ProcessingSoftware'] == 11
     assert tags.getall(11) == ['ProcessingSoftware']
     assert tags.getall('ProcessingSoftware') == [11]
     tags.add(11, 'ProcessingSoftware')
@@ -6103,55 +6082,14 @@
                 image = page.asarray()
         else:
             image = page.asarray()
             assert_aszarr_method(page, image)
         assert__str__(tif)
 
 
-@pytest.mark.skipif(
-    SKIP_PRIVATE or SKIP_CODECS or not imagecodecs.JPEGXL, reason=REASON
-)
-def test_read_dng_jpegxl():
-    """Test read JPEGXL in DNG."""
-    fname = private_file('DNG/20240125_204051_1.dng')
-    with TiffFile(fname) as tif:
-        assert len(tif.pages) == 1
-        assert len(tif.series) == 6
-
-        page = tif.pages.first.pages[0]
-        assert not page.is_reduced
-        assert page.compression == JPEGXL_DNG
-        assert page.photometric == LINEAR_RAW
-        assert page.imagewidth == 5712
-        assert page.imagelength == 4284
-        assert page.bitspersample == 16
-        assert page.samplesperpixel == 3
-        image = page.asarray()
-        assert image.shape == (4284, 5712, 3)
-        assert image.dtype == 'uint16'
-        assert image[1024, 1024, 1] == 36
-
-        page = tif.pages.first.pages[1]
-        assert page.is_reduced
-        assert page.compression == JPEGXL_DNG
-        assert page.photometric == RGB
-        assert page.imagewidth == 1024
-        assert page.imagelength == 768
-        assert page.bitspersample == 8
-        assert page.samplesperpixel == 3
-        image = page.asarray()
-        assert image.shape == (768, 1024, 3)
-        assert image.dtype == 'uint8'
-        assert image[512, 512, 1] == 48
-        assert page.tags['JXLDistance'].value == 2.0
-        assert page.tags['JXLEffort'].value == 7
-        assert page.tags['JXLDecodeSpeed'].value == 4
-        assert__str__(tif)
-
-
 @pytest.mark.skipif(SKIP_PRIVATE, reason=REASON)
 @pytest.mark.parametrize('fname', ['sample1.orf', 'sample1.rw2'])
 def test_read_rawformats(fname, caplog):
     """Test parse unsupported RAW formats."""
     fname = private_file(f'RAWformats/{fname}')
     with TiffFile(fname) as tif:
         assert 'RAW format' in caplog.text
```

### Comparing `tifffile-2024.5.10/tifffile/_imagecodecs.py` & `tifffile-2024.5.3/tifffile/_imagecodecs.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,16 +128,16 @@
     r"""Decompress PackBits encoded byte string.
 
     >>> packbits_decode(b'\x80\x80')  # NOP
     b''
     >>> packbits_decode(b'\x02123')
     b'123'
     >>> packbits_decode(
-    ...     b'\xfe\xaa\x02\x80\x00\x2a\xfd\xaa\x03\x80\x00\x2a\x22\xf7\xaa'
-    ... )[:-5]
+    ...   b'\xfe\xaa\x02\x80\x00\x2a\xfd\xaa\x03\x80\x00\x2a\x22\xf7\xaa'
+    ...     )[:-5]
     b'\xaa\xaa\xaa\x80\x00*\xaa\xaa\xaa\xaa\x80\x00*"\xaa\xaa\xaa\xaa\xaa'
 
     """
     out = []
     out_extend = out.extend
     i = 0
     try:
```

### Comparing `tifffile-2024.5.10/tifffile/geodb.py` & `tifffile-2024.5.3/tifffile/geodb.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.5.10/tifffile/lsm2bin.py` & `tifffile-2024.5.3/tifffile/lsm2bin.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.5.10/tifffile/numcodecs.py` & `tifffile-2024.5.3/tifffile/numcodecs.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.5.10/tifffile/tiff2fsspec.py` & `tifffile-2024.5.3/tifffile/tiff2fsspec.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.5.10/tifffile/tiffcomment.py` & `tifffile-2024.5.3/tifffile/tiffcomment.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.5.10/tifffile/tifffile.py` & `tifffile-2024.5.3/tifffile/tifffile.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 Tifffile can also be used to inspect TIFF structures, read image data from
 multi-dimensional file sequences, write fsspec ReferenceFileSystem for
 TIFF files and image file sequences, patch TIFF tag values, and parse
 many proprietary metadata formats.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.5.10
+:Version: 2024.5.3
 :DOI: `10.5281/zenodo.6795860 <https://doi.org/10.5281/zenodo.6795860>`_
 
 Quickstart
 ----------
 
 Install the tifffile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/tifffile/>`_::
@@ -100,30 +100,25 @@
 - `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
 - `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2024.1.1
   (required for encoding or decoding LZW, JPEG, etc. compressed segments)
 - `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.4
   (required for plotting)
 - `Lxml <https://pypi.org/project/lxml/>`_ 5.2.1
   (required only for validating and printing XML)
-- `Zarr <https://pypi.org/project/zarr/>`_ 2.18.0
+- `Zarr <https://pypi.org/project/zarr/>`_ 2.17.2
   (required only for opening Zarr stores)
 - `Fsspec <https://pypi.org/project/fsspec/>`_ 2024.3.1
   (required only for opening ReferenceFileSystem files)
 
 Revisions
 ---------
 
-2024.5.10
-
-- Pass 5082 tests.
-- Support reading JPEGXL compression in DNG 1.7.
-- Read invalid TIFF created by IDEAS software.
-
 2024.5.3
 
+- Pass 5080 tests.
 - Fix reading incompletely written LSM.
 - Fix reading Philips DP with extra rows of tiles (#253, breaking).
 
 2024.4.24
 
 - Fix compatibility issue with numpy 2 (#252).
 
@@ -415,16 +410,16 @@
 - Tags for TIFF and Related Specifications. Digital Preservation.
   https://www.loc.gov/preservation/digital/formats/content/tiff_tags.shtml
 - CIPA DC-008-2016: Exchangeable image file format for digital still cameras:
   Exif Version 2.31.
   http://www.cipa.jp/std/documents/e/DC-008-Translation-2016-E.pdf
 - The EER (Electron Event Representation) file format.
   https://github.com/fei-company/EerReaderLib
-- Digital Negative (DNG) Specification. Version 1.7.1.0, September 2023.
-  https://helpx.adobe.com/content/dam/help/en/photoshop/pdf/DNG_Spec_1_7_1_0.pdf
+- Digital Negative (DNG) Specification. Version 1.5.0.0, June 2012.
+  https://www.adobe.com/content/dam/acom/en/products/photoshop/pdfs/dng_spec_1.5.0.0.pdf
 - Roche Digital Pathology. BIF image file format for digital pathology.
   https://diagnostics.roche.com/content/dam/diagnostics/Blueprint/en/pdf/rmd/Roche-Digital-Pathology-BIF-Whitepaper.pdf
 - Astro-TIFF specification. https://astro-tiff.sourceforge.io/
 - Aperio Technologies, Inc. Digital Slides and Third-Party Data Interchange.
   Aperio_Digital_Slides_and_Third-party_data_interchange.pdf
 - PerkinElmer image format.
   https://downloads.openmicroscopy.org/images/Vectra-QPTIFF/perkinelmer/PKI_Image%20Format.docx
@@ -484,15 +479,14 @@
 (18, 301, 219)
 
 Iterate over all pages in the TIFF file and successively read images:
 
 >>> with TiffFile('temp.tif') as tif:
 ...     for page in tif.pages:
 ...         image = page.asarray()
-...
 
 Get information about the image stack in the TIFF file without reading
 any image data:
 
 >>> tif = TiffFile('temp.tif')
 >>> len(tif.pages)  # number of pages in the file
 64
@@ -512,15 +506,14 @@
 'QYX'
 >>> tif.close()
 
 Inspect the "XResolution" tag from the first page in the TIFF file:
 
 >>> with TiffFile('temp.tif') as tif:
 ...     tag = tif.pages[0].tags['XResolution']
-...
 >>> tag.value
 (1, 1)
 >>> tag.name
 'XResolution'
 >>> tag.code
 282
 >>> tag.count
@@ -530,21 +523,19 @@
 
 Iterate over all tags in the TIFF file:
 
 >>> with TiffFile('temp.tif') as tif:
 ...     for page in tif.pages:
 ...         for tag in page.tags:
 ...             tag_name, tag_value = tag.name, tag.value
-...
 
 Overwrite the value of an existing tag, for example, XResolution:
 
 >>> with TiffFile('temp.tif', mode='r+') as tif:
 ...     _ = tif.pages[0].tags['XResolution'].overwrite((96000, 1000))
-...
 
 Write a 5-dimensional floating-point array using BigTIFF format, separate
 color components, tiling, Zlib compression level 8, horizontal differencing
 predictor, and additional metadata:
 
 >>> data = numpy.random.rand(2, 5, 3, 301, 219).astype('float32')
 >>> imwrite(
@@ -553,44 +544,43 @@
 ...     bigtiff=True,
 ...     photometric='rgb',
 ...     planarconfig='separate',
 ...     tile=(32, 32),
 ...     compression='zlib',
 ...     compressionargs={'level': 8},
 ...     predictor=True,
-...     metadata={'axes': 'TZCYX'},
+...     metadata={'axes': 'TZCYX'}
 ... )
 
 Write a 10 fps time series of volumes with xyz voxel size 2.6755x2.6755x3.9474
 micron^3 to an ImageJ hyperstack formatted TIFF file:
 
 >>> volume = numpy.random.randn(6, 57, 256, 256).astype('float32')
 >>> image_labels = [f'{i}' for i in range(volume.shape[0] * volume.shape[1])]
 >>> imwrite(
 ...     'temp.tif',
 ...     volume,
 ...     imagej=True,
-...     resolution=(1.0 / 2.6755, 1.0 / 2.6755),
+...     resolution=(1./2.6755, 1./2.6755),
 ...     metadata={
 ...         'spacing': 3.947368,
 ...         'unit': 'um',
-...         'finterval': 1 / 10,
+...         'finterval': 1/10,
 ...         'fps': 10.0,
 ...         'axes': 'TZYX',
 ...         'Labels': image_labels,
-...     },
+...     }
 ... )
 
 Read the volume and metadata from the ImageJ hyperstack file:
 
 >>> with TiffFile('temp.tif') as tif:
 ...     volume = tif.asarray()
 ...     axes = tif.series[0].axes
 ...     imagej_metadata = tif.imagej_metadata
-...
 >>> volume.shape
 (6, 57, 256, 256)
 >>> axes
 'TZYX'
 >>> imagej_metadata['slices']
 57
 >>> imagej_metadata['frames']
@@ -603,15 +593,18 @@
 (6, 57, 256, 256)
 >>> del memmap_volume
 
 Create a TIFF file containing an empty image and write to the memory-mapped
 NumPy array (note: this does not work with compression or tiling):
 
 >>> memmap_image = memmap(
-...     'temp.tif', shape=(256, 256, 3), dtype='float32', photometric='rgb'
+...     'temp.tif',
+...     shape=(256, 256, 3),
+...     dtype='float32',
+...     photometric='rgb'
 ... )
 >>> type(memmap_image)
 <class 'numpy.memmap'>
 >>> memmap_image[255, 255, 1] = 1.0
 >>> memmap_image.flush()
 >>> del memmap_image
 
@@ -620,127 +613,121 @@
 interoperability):
 
 >>> series0 = numpy.random.randint(0, 255, (32, 32, 3), 'uint8')
 >>> series1 = numpy.random.randint(0, 255, (4, 256, 256), 'uint16')
 >>> with TiffWriter('temp.tif') as tif:
 ...     tif.write(series0, photometric='rgb')
 ...     tif.write(series1, photometric='minisblack')
-...
 
 Read the second image series from the TIFF file:
 
 >>> series1 = imread('temp.tif', series=1)
 >>> series1.shape
 (4, 256, 256)
 
 Successively write the frames of one contiguous series to a TIFF file:
 
 >>> data = numpy.random.randint(0, 255, (30, 301, 219), 'uint8')
 >>> with TiffWriter('temp.tif') as tif:
 ...     for frame in data:
 ...         tif.write(frame, contiguous=True)
-...
 
 Append an image series to the existing TIFF file (note: this does not work
 with ImageJ hyperstack or OME-TIFF files):
 
 >>> data = numpy.random.randint(0, 255, (301, 219, 3), 'uint8')
 >>> imwrite('temp.tif', data, photometric='rgb', append=True)
 
 Create a TIFF file from a generator of tiles:
 
 >>> data = numpy.random.randint(0, 2**12, (31, 33, 3), 'uint16')
 >>> def tiles(data, tileshape):
 ...     for y in range(0, data.shape[0], tileshape[0]):
 ...         for x in range(0, data.shape[1], tileshape[1]):
 ...             yield data[y : y + tileshape[0], x : x + tileshape[1]]
-...
 >>> imwrite(
 ...     'temp.tif',
 ...     tiles(data, (16, 16)),
 ...     tile=(16, 16),
 ...     shape=data.shape,
 ...     dtype=data.dtype,
-...     photometric='rgb',
+...     photometric='rgb'
 ... )
 
 Write a multi-dimensional, multi-resolution (pyramidal), multi-series OME-TIFF
 file with metadata. Sub-resolution images are written to SubIFDs. Limit
 parallel encoding to 2 threads. Write a thumbnail image as a separate image
 series:
 
 >>> data = numpy.random.randint(0, 255, (8, 2, 512, 512, 3), 'uint8')
 >>> subresolutions = 2
 >>> pixelsize = 0.29  # micrometer
 >>> with TiffWriter('temp.ome.tif', bigtiff=True) as tif:
-...     metadata = {
+...     metadata={
 ...         'axes': 'TCYXS',
 ...         'SignificantBits': 8,
 ...         'TimeIncrement': 0.1,
 ...         'TimeIncrementUnit': 's',
 ...         'PhysicalSizeX': pixelsize,
 ...         'PhysicalSizeXUnit': 'µm',
 ...         'PhysicalSizeY': pixelsize,
 ...         'PhysicalSizeYUnit': 'µm',
 ...         'Channel': {'Name': ['Channel 1', 'Channel 2']},
-...         'Plane': {'PositionX': [0.0] * 16, 'PositionXUnit': ['µm'] * 16},
+...         'Plane': {'PositionX': [0.0] * 16, 'PositionXUnit': ['µm'] * 16}
 ...     }
 ...     options = dict(
 ...         photometric='rgb',
 ...         tile=(128, 128),
 ...         compression='jpeg',
 ...         resolutionunit='CENTIMETER',
-...         maxworkers=2,
+...         maxworkers=2
 ...     )
 ...     tif.write(
 ...         data,
 ...         subifds=subresolutions,
 ...         resolution=(1e4 / pixelsize, 1e4 / pixelsize),
 ...         metadata=metadata,
-...         **options,
+...         **options
 ...     )
 ...     # write pyramid levels to the two subifds
 ...     # in production use resampling to generate sub-resolution images
 ...     for level in range(subresolutions):
-...         mag = 2 ** (level + 1)
+...         mag = 2**(level + 1)
 ...         tif.write(
 ...             data[..., ::mag, ::mag, :],
 ...             subfiletype=1,
 ...             resolution=(1e4 / mag / pixelsize, 1e4 / mag / pixelsize),
-...             **options,
+...             **options
 ...         )
 ...     # add a thumbnail image as a separate series
 ...     # it is recognized by QuPath as an associated image
 ...     thumbnail = (data[0, 0, ::8, ::8] >> 2).astype('uint8')
 ...     tif.write(thumbnail, metadata={'Name': 'thumbnail'})
-...
 
 Access the image levels in the pyramidal OME-TIFF file:
 
 >>> baseimage = imread('temp.ome.tif')
 >>> second_level = imread('temp.ome.tif', series=0, level=1)
 >>> with TiffFile('temp.ome.tif') as tif:
 ...     baseimage = tif.series[0].asarray()
 ...     second_level = tif.series[0].levels[1].asarray()
-...
 
 Iterate over and decode single JPEG compressed tiles in the TIFF file:
 
 >>> with TiffFile('temp.ome.tif') as tif:
 ...     fh = tif.filehandle
 ...     for page in tif.pages:
 ...         for index, (offset, bytecount) in enumerate(
 ...             zip(page.dataoffsets, page.databytecounts)
 ...         ):
 ...             _ = fh.seek(offset)
 ...             data = fh.read(bytecount)
 ...             tile, indices, shape = page.decode(
 ...                 data, index, jpegtables=page.jpegtables
 ...             )
-...
 
 Use Zarr to read parts of the tiled, pyramidal images in the TIFF file:
 
 >>> import zarr
 >>> store = imread('temp.ome.tif', aszarr=True)
 >>> z = zarr.open(store, mode='r')
 >>> z
@@ -782,15 +769,15 @@
 
 >>> imwrite(
 ...     'temp.ome.tif',
 ...     shape=(8, 800, 600),
 ...     dtype='uint16',
 ...     photometric='minisblack',
 ...     tile=(128, 128),
-...     metadata={'axes': 'CYX'},
+...     metadata={'axes': 'CYX'}
 ... )
 >>> store = imread('temp.ome.tif', mode='r+', aszarr=True)
 >>> z = zarr.open(store, mode='r+')
 >>> z
 <zarr.core.Array (8, 800, 600) uint16>
 >>> z[3, 100:200, 200:300:2] = 1024
 >>> store.close()
@@ -807,15 +794,17 @@
 (2, 64, 64)
 >>> image_sequence.dtype
 dtype('float64')
 
 Read an image stack from a series of TIFF files with a file name pattern
 as NumPy or Zarr arrays:
 
->>> image_sequence = TiffSequence('temp_C0*.tif', pattern=r'_(C)(\d+)(T)(\d+)')
+>>> image_sequence = TiffSequence(
+...     'temp_C0*.tif', pattern=r'_(C)(\d+)(T)(\d+)'
+... )
 >>> image_sequence.shape
 (1, 2)
 >>> image_sequence.axes
 'CT'
 >>> data = image_sequence.asarray()
 >>> data.shape
 (1, 2, 64, 64)
@@ -844,15 +833,15 @@
 
     $ python -m tifffile temp.ome.tif
 
 """
 
 from __future__ import annotations
 
-__version__ = '2024.5.10'
+__version__ = '2024.5.3'
 
 __all__ = [
     'TiffFile',
     'TiffFileError',
     'TiffFrame',
     'TiffPage',
     'TiffPages',
@@ -4145,15 +4134,14 @@
             return 1
         if chunksize < 2048 and compression in {
             33003,  # JPEG2000
             33004,  # JPEG2000
             33005,  # JPEG2000
             34712,  # JPEG2000
             50002,  # JPEG XL
-            52546,  # JPEG XL DNG
         }:
             return 1
         if chunksize < 1024 and compression in {
             34925,  # LZMA
             50001,  # WebP
         }:
             return 1
@@ -8196,18 +8184,14 @@
 
         if self.subfiletype == 0:
             value = tags.valueof(255)  # SubfileType
             if value == 2:
                 self.subfiletype = 0b1  # reduced image
             elif value == 3:
                 self.subfiletype = 0b10  # multi-page
-        elif not isinstance(self.subfiletype, int):
-            # files created by IDEAS
-            logger().warning(f'{self!r} invalid {self.subfiletype=}')
-            self.subfiletype = 0
 
         # consolidate private tags; remove them from self.tags
         # if self.is_andor:
         #     self.andor_tags
         # elif self.is_epics:
         #     self.epics_tags
         # elif self.is_ndpi:
@@ -11920,15 +11904,17 @@
     Different tag codes may be registered with the same name, for example,
     37387 and 41483 are both named FlashEnergy.
 
     Parameters:
         arg: Mapping of codes to names.
 
     Examples:
-        >>> tags = TiffTagRegistry([(34853, 'GPSTag'), (34853, 'OlympusSIS2')])
+        >>> tags = TiffTagRegistry(
+        ...     [(34853, 'GPSTag'), (34853, 'OlympusSIS2')]
+        ... )
         >>> tags.add(37387, 'FlashEnergy')
         >>> tags.add(41483, 'FlashEnergy')
         >>> tags['GPSTag']
         34853
         >>> tags[34853]
         'GPSTag'
         >>> tags.getall(34853)
@@ -13002,15 +12988,14 @@
             34892: 'imagecodecs_jpeg',
             34933: 'imagecodecs_png',
             34934: 'imagecodecs_jpegxr',
             48124: 'imagecodecs_jetraw',
             50000: 'imagecodecs_zstd',  # numcodecs.zstd fails w/ unknown sizes
             50001: 'imagecodecs_webp',
             50002: 'imagecodecs_jpegxl',
-            52546: 'imagecodecs_jpegxl',
             **({} if compressors is None else compressors),
         }
 
         for series in self._data:
             errormsg = ' not supported by the fsspec ReferenceFileSystem'
             keyframe = series.keyframe
             if (
@@ -15594,15 +15579,14 @@
 
 @final
 class NullContext:
     """Null context manager. Can be used as a dummy reentrant lock.
 
     >>> with NullContext():
     ...     pass
-    ...
 
     """
 
     __slots__ = ()
 
     def __enter__(self) -> NullContext:
         return self
@@ -16030,16 +16014,15 @@
                             raise OmeXmlError('more than 3 modulo dimensions')
                 else:
                     dimorder.append(ax)
             hiaxes = ''.join(dimorder)
 
             # TODO: use user-specified start, stop, step, or labels
             moduloalong = ''.join(
-                f'<ModuloAlong{ax} Type="{axtype}" '
-                f'Start="0" End="{size - 1}"/>'
+                f'<ModuloAlong{ax} Type="{axtype}" Start="0" End="{size-1}"/>'
                 for ax, (axtype, size) in modulo.items()
             )
             annotationref = f'<AnnotationRef ID="Annotation:{index}"/>'
             annotations = (
                 f'<XMLAnnotation ID="Annotation:{index}" '
                 'Namespace="openmicroscopy.org/omero/dimension/modulo">'
                 '<Value>'
@@ -16534,15 +16517,15 @@
             elif key in {50001, 34927}:  # 34927 deprecated
                 if self._encode:
                     codec = imagecodecs.webp_encode
                 else:
                     codec = imagecodecs.webp_decode
             elif key in {65000, 65001, 65002} and not self._encode:
                 codec = imagecodecs.eer_decode
-            elif key in {50002, 52546}:
+            elif key == 50002:
                 if self._encode:
                     codec = imagecodecs.jpegxl_encode
                 else:
                     codec = imagecodecs.jpegxl_decode
             else:
                 try:
                     msg = f'{COMPRESSION(key)!r} not supported'
@@ -16804,20 +16787,18 @@
     """JPEG XR (Zoomable Image File format)."""
     JETRAW = 48124
     """Jetraw by Dotphoton."""
     ZSTD = 50000
     """Zstandard."""
     WEBP = 50001
     """WebP."""
-    JPEGXL = 50002  # GDAL
+    JPEGXL = 50002
     """JPEG XL."""
     PIXTIFF = 50013
     """ZLIB (Atalasoft)."""
-    JPEGXL_DNG = 52546
-    """JPEG XL (DNG)."""
     EER_V0 = 65000  # FIXED82 Thermo Fisher Scientific
     EER_V1 = 65001  # FIXED72 Thermo Fisher Scientific
     EER_V2 = 65002  # VARIABLE Thermo Fisher Scientific
     # KODAK_DCR = 65000
     # PENTAX_PEF = 65535
 
     def __bool__(self) -> bool:
@@ -17787,23 +17768,14 @@
                 (52530, 'CameraCalibration3'),  # DNG 1.6
                 (52538, 'ReductionMatrix3'),  # DNG 1.6
                 (52537, 'ProfileHueSatMapData3'),  # DNG 1.6
                 (52532, 'ForwardMatrix3'),  # DNG 1.6
                 (52533, 'IlluminantData1'),  # DNG 1.6
                 (52534, 'IlluminantData2'),  # DNG 1.6
                 (53535, 'IlluminantData3'),  # DNG 1.6
-                (52544, 'ProfileGainTableMap2'),  # DNG 1.7
-                (52547, 'ColumnInterleaveFactor'),  # DNG 1.7
-                (52548, 'ImageSequenceInfo'),  # DNG 1.7
-                (52550, 'ImageStats'),  # DNG 1.7
-                (52551, 'ProfileDynamicRange'),  # DNG 1.7
-                (52552, 'ProfileGroupName'),  # DNG 1.7
-                (52553, 'JXLDistance'),  # DNG 1.7
-                (52554, 'JXLEffort'),  # DNG 1.7
-                (52555, 'JXLDecodeSpeed'),  # DNG 1.7
                 (55000, 'AperioUnknown55000'),
                 (55001, 'AperioMagnification'),
                 (55002, 'AperioMPP'),
                 (55003, 'AperioScanScopeID'),
                 (55004, 'AperioDate'),
                 (59932, 'Padding'),
                 (59933, 'OffsetSchema'),
@@ -18345,15 +18317,14 @@
             34712,  # jpeg2k
             34892,  # jpeg
             34933,  # png
             34934,  # jpegxr ZIF
             48124,  # jetraw
             50001,  # webp
             50002,  # jpegxl
-            52546,  # jpegxl DNG
         }
 
     @cached_property
     def AXES_NAMES(self) -> dict[str, str]:
         """Map axes character codes to dimension names.
 
         - **X : width** (image width)
@@ -23665,18 +23636,16 @@
         other = {'big': '>', 'little': '<'}[sys.byteorder]
     return byteorder == other
 
 
 def recarray2dict(recarray: numpy.recarray, /) -> dict[str, Any]:
     """Return numpy.recarray as dictionary.
 
-    >>> r = numpy.array(
-    ...     [(1.0, 2, 'a'), (3.0, 4, 'bc')],
-    ...     dtype=[('x', '<f4'), ('y', '<i4'), ('s', 'S2')],
-    ... )
+    >>> r = numpy.array([(1., 2, 'a'), (3., 4, 'bc')],
+    ...                 dtype=[('x', '<f4'), ('y', '<i4'), ('s', 'S2')])
     >>> recarray2dict(r)
     {'x': [1.0, 3.0], 'y': [2, 4], 's': ['a', 'bc']}
     >>> recarray2dict(r[1])
     {'x': 3.0, 'y': 4, 's': 'bc'}
 
     """
     # TODO: subarrays
@@ -24205,15 +24174,15 @@
             result[key] = value
     return result
 
 
 def update_kwargs(kwargs: dict[str, Any], /, **keyvalues: Any) -> None:
     """Update dict with keys and values if keys do not already exist.
 
-    >>> kwargs = {'one': 1}
+    >>> kwargs = {'one': 1, }
     >>> update_kwargs(kwargs, one=None, two=2)
     >>> kwargs == {'one': 1, 'two': 2}
     True
 
     """
     for key, value in keyvalues.items():
         if key not in kwargs:
```

### Comparing `tifffile-2024.5.10/tifffile.egg-info/PKG-INFO` & `tifffile-2024.5.3/tifffile.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tifffile
-Version: 2024.5.10
+Version: 2024.5.3
 Summary: Read and write TIFF files
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/tifffile/issues
 Project-URL: Source Code, https://github.com/cgohlke/tifffile
@@ -59,15 +59,15 @@
 Tifffile can also be used to inspect TIFF structures, read image data from
 multi-dimensional file sequences, write fsspec ReferenceFileSystem for
 TIFF files and image file sequences, patch TIFF tag values, and parse
 many proprietary metadata formats.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.5.10
+:Version: 2024.5.3
 :DOI: `10.5281/zenodo.6795860 <https://doi.org/10.5281/zenodo.6795860>`_
 
 Quickstart
 ----------
 
 Install the tifffile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/tifffile/>`_::
@@ -103,30 +103,25 @@
 - `NumPy <https://pypi.org/project/numpy/>`_ 1.26.4
 - `Imagecodecs <https://pypi.org/project/imagecodecs/>`_ 2024.1.1
   (required for encoding or decoding LZW, JPEG, etc. compressed segments)
 - `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.8.4
   (required for plotting)
 - `Lxml <https://pypi.org/project/lxml/>`_ 5.2.1
   (required only for validating and printing XML)
-- `Zarr <https://pypi.org/project/zarr/>`_ 2.18.0
+- `Zarr <https://pypi.org/project/zarr/>`_ 2.17.2
   (required only for opening Zarr stores)
 - `Fsspec <https://pypi.org/project/fsspec/>`_ 2024.3.1
   (required only for opening ReferenceFileSystem files)
 
 Revisions
 ---------
 
-2024.5.10
-
-- Pass 5082 tests.
-- Support reading JPEGXL compression in DNG 1.7.
-- Read invalid TIFF created by IDEAS software.
-
 2024.5.3
 
+- Pass 5080 tests.
 - Fix reading incompletely written LSM.
 - Fix reading Philips DP with extra rows of tiles (#253, breaking).
 
 2024.4.24
 
 - Fix compatibility issue with numpy 2 (#252).
 
@@ -418,16 +413,16 @@
 - Tags for TIFF and Related Specifications. Digital Preservation.
   https://www.loc.gov/preservation/digital/formats/content/tiff_tags.shtml
 - CIPA DC-008-2016: Exchangeable image file format for digital still cameras:
   Exif Version 2.31.
   http://www.cipa.jp/std/documents/e/DC-008-Translation-2016-E.pdf
 - The EER (Electron Event Representation) file format.
   https://github.com/fei-company/EerReaderLib
-- Digital Negative (DNG) Specification. Version 1.7.1.0, September 2023.
-  https://helpx.adobe.com/content/dam/help/en/photoshop/pdf/DNG_Spec_1_7_1_0.pdf
+- Digital Negative (DNG) Specification. Version 1.5.0.0, June 2012.
+  https://www.adobe.com/content/dam/acom/en/products/photoshop/pdfs/dng_spec_1.5.0.0.pdf
 - Roche Digital Pathology. BIF image file format for digital pathology.
   https://diagnostics.roche.com/content/dam/diagnostics/Blueprint/en/pdf/rmd/Roche-Digital-Pathology-BIF-Whitepaper.pdf
 - Astro-TIFF specification. https://astro-tiff.sourceforge.io/
 - Aperio Technologies, Inc. Digital Slides and Third-Party Data Interchange.
   Aperio_Digital_Slides_and_Third-party_data_interchange.pdf
 - PerkinElmer image format.
   https://downloads.openmicroscopy.org/images/Vectra-QPTIFF/perkinelmer/PKI_Image%20Format.docx
@@ -487,15 +482,14 @@
 (18, 301, 219)
 
 Iterate over all pages in the TIFF file and successively read images:
 
 >>> with TiffFile('temp.tif') as tif:
 ...     for page in tif.pages:
 ...         image = page.asarray()
-...
 
 Get information about the image stack in the TIFF file without reading
 any image data:
 
 >>> tif = TiffFile('temp.tif')
 >>> len(tif.pages)  # number of pages in the file
 64
@@ -515,15 +509,14 @@
 'QYX'
 >>> tif.close()
 
 Inspect the "XResolution" tag from the first page in the TIFF file:
 
 >>> with TiffFile('temp.tif') as tif:
 ...     tag = tif.pages[0].tags['XResolution']
-...
 >>> tag.value
 (1, 1)
 >>> tag.name
 'XResolution'
 >>> tag.code
 282
 >>> tag.count
@@ -533,21 +526,19 @@
 
 Iterate over all tags in the TIFF file:
 
 >>> with TiffFile('temp.tif') as tif:
 ...     for page in tif.pages:
 ...         for tag in page.tags:
 ...             tag_name, tag_value = tag.name, tag.value
-...
 
 Overwrite the value of an existing tag, for example, XResolution:
 
 >>> with TiffFile('temp.tif', mode='r+') as tif:
 ...     _ = tif.pages[0].tags['XResolution'].overwrite((96000, 1000))
-...
 
 Write a 5-dimensional floating-point array using BigTIFF format, separate
 color components, tiling, Zlib compression level 8, horizontal differencing
 predictor, and additional metadata:
 
 >>> data = numpy.random.rand(2, 5, 3, 301, 219).astype('float32')
 >>> imwrite(
@@ -556,44 +547,43 @@
 ...     bigtiff=True,
 ...     photometric='rgb',
 ...     planarconfig='separate',
 ...     tile=(32, 32),
 ...     compression='zlib',
 ...     compressionargs={'level': 8},
 ...     predictor=True,
-...     metadata={'axes': 'TZCYX'},
+...     metadata={'axes': 'TZCYX'}
 ... )
 
 Write a 10 fps time series of volumes with xyz voxel size 2.6755x2.6755x3.9474
 micron^3 to an ImageJ hyperstack formatted TIFF file:
 
 >>> volume = numpy.random.randn(6, 57, 256, 256).astype('float32')
 >>> image_labels = [f'{i}' for i in range(volume.shape[0] * volume.shape[1])]
 >>> imwrite(
 ...     'temp.tif',
 ...     volume,
 ...     imagej=True,
-...     resolution=(1.0 / 2.6755, 1.0 / 2.6755),
+...     resolution=(1./2.6755, 1./2.6755),
 ...     metadata={
 ...         'spacing': 3.947368,
 ...         'unit': 'um',
-...         'finterval': 1 / 10,
+...         'finterval': 1/10,
 ...         'fps': 10.0,
 ...         'axes': 'TZYX',
 ...         'Labels': image_labels,
-...     },
+...     }
 ... )
 
 Read the volume and metadata from the ImageJ hyperstack file:
 
 >>> with TiffFile('temp.tif') as tif:
 ...     volume = tif.asarray()
 ...     axes = tif.series[0].axes
 ...     imagej_metadata = tif.imagej_metadata
-...
 >>> volume.shape
 (6, 57, 256, 256)
 >>> axes
 'TZYX'
 >>> imagej_metadata['slices']
 57
 >>> imagej_metadata['frames']
@@ -606,15 +596,18 @@
 (6, 57, 256, 256)
 >>> del memmap_volume
 
 Create a TIFF file containing an empty image and write to the memory-mapped
 NumPy array (note: this does not work with compression or tiling):
 
 >>> memmap_image = memmap(
-...     'temp.tif', shape=(256, 256, 3), dtype='float32', photometric='rgb'
+...     'temp.tif',
+...     shape=(256, 256, 3),
+...     dtype='float32',
+...     photometric='rgb'
 ... )
 >>> type(memmap_image)
 <class 'numpy.memmap'>
 >>> memmap_image[255, 255, 1] = 1.0
 >>> memmap_image.flush()
 >>> del memmap_image
 
@@ -623,127 +616,121 @@
 interoperability):
 
 >>> series0 = numpy.random.randint(0, 255, (32, 32, 3), 'uint8')
 >>> series1 = numpy.random.randint(0, 255, (4, 256, 256), 'uint16')
 >>> with TiffWriter('temp.tif') as tif:
 ...     tif.write(series0, photometric='rgb')
 ...     tif.write(series1, photometric='minisblack')
-...
 
 Read the second image series from the TIFF file:
 
 >>> series1 = imread('temp.tif', series=1)
 >>> series1.shape
 (4, 256, 256)
 
 Successively write the frames of one contiguous series to a TIFF file:
 
 >>> data = numpy.random.randint(0, 255, (30, 301, 219), 'uint8')
 >>> with TiffWriter('temp.tif') as tif:
 ...     for frame in data:
 ...         tif.write(frame, contiguous=True)
-...
 
 Append an image series to the existing TIFF file (note: this does not work
 with ImageJ hyperstack or OME-TIFF files):
 
 >>> data = numpy.random.randint(0, 255, (301, 219, 3), 'uint8')
 >>> imwrite('temp.tif', data, photometric='rgb', append=True)
 
 Create a TIFF file from a generator of tiles:
 
 >>> data = numpy.random.randint(0, 2**12, (31, 33, 3), 'uint16')
 >>> def tiles(data, tileshape):
 ...     for y in range(0, data.shape[0], tileshape[0]):
 ...         for x in range(0, data.shape[1], tileshape[1]):
 ...             yield data[y : y + tileshape[0], x : x + tileshape[1]]
-...
 >>> imwrite(
 ...     'temp.tif',
 ...     tiles(data, (16, 16)),
 ...     tile=(16, 16),
 ...     shape=data.shape,
 ...     dtype=data.dtype,
-...     photometric='rgb',
+...     photometric='rgb'
 ... )
 
 Write a multi-dimensional, multi-resolution (pyramidal), multi-series OME-TIFF
 file with metadata. Sub-resolution images are written to SubIFDs. Limit
 parallel encoding to 2 threads. Write a thumbnail image as a separate image
 series:
 
 >>> data = numpy.random.randint(0, 255, (8, 2, 512, 512, 3), 'uint8')
 >>> subresolutions = 2
 >>> pixelsize = 0.29  # micrometer
 >>> with TiffWriter('temp.ome.tif', bigtiff=True) as tif:
-...     metadata = {
+...     metadata={
 ...         'axes': 'TCYXS',
 ...         'SignificantBits': 8,
 ...         'TimeIncrement': 0.1,
 ...         'TimeIncrementUnit': 's',
 ...         'PhysicalSizeX': pixelsize,
 ...         'PhysicalSizeXUnit': 'µm',
 ...         'PhysicalSizeY': pixelsize,
 ...         'PhysicalSizeYUnit': 'µm',
 ...         'Channel': {'Name': ['Channel 1', 'Channel 2']},
-...         'Plane': {'PositionX': [0.0] * 16, 'PositionXUnit': ['µm'] * 16},
+...         'Plane': {'PositionX': [0.0] * 16, 'PositionXUnit': ['µm'] * 16}
 ...     }
 ...     options = dict(
 ...         photometric='rgb',
 ...         tile=(128, 128),
 ...         compression='jpeg',
 ...         resolutionunit='CENTIMETER',
-...         maxworkers=2,
+...         maxworkers=2
 ...     )
 ...     tif.write(
 ...         data,
 ...         subifds=subresolutions,
 ...         resolution=(1e4 / pixelsize, 1e4 / pixelsize),
 ...         metadata=metadata,
-...         **options,
+...         **options
 ...     )
 ...     # write pyramid levels to the two subifds
 ...     # in production use resampling to generate sub-resolution images
 ...     for level in range(subresolutions):
-...         mag = 2 ** (level + 1)
+...         mag = 2**(level + 1)
 ...         tif.write(
 ...             data[..., ::mag, ::mag, :],
 ...             subfiletype=1,
 ...             resolution=(1e4 / mag / pixelsize, 1e4 / mag / pixelsize),
-...             **options,
+...             **options
 ...         )
 ...     # add a thumbnail image as a separate series
 ...     # it is recognized by QuPath as an associated image
 ...     thumbnail = (data[0, 0, ::8, ::8] >> 2).astype('uint8')
 ...     tif.write(thumbnail, metadata={'Name': 'thumbnail'})
-...
 
 Access the image levels in the pyramidal OME-TIFF file:
 
 >>> baseimage = imread('temp.ome.tif')
 >>> second_level = imread('temp.ome.tif', series=0, level=1)
 >>> with TiffFile('temp.ome.tif') as tif:
 ...     baseimage = tif.series[0].asarray()
 ...     second_level = tif.series[0].levels[1].asarray()
-...
 
 Iterate over and decode single JPEG compressed tiles in the TIFF file:
 
 >>> with TiffFile('temp.ome.tif') as tif:
 ...     fh = tif.filehandle
 ...     for page in tif.pages:
 ...         for index, (offset, bytecount) in enumerate(
 ...             zip(page.dataoffsets, page.databytecounts)
 ...         ):
 ...             _ = fh.seek(offset)
 ...             data = fh.read(bytecount)
 ...             tile, indices, shape = page.decode(
 ...                 data, index, jpegtables=page.jpegtables
 ...             )
-...
 
 Use Zarr to read parts of the tiled, pyramidal images in the TIFF file:
 
 >>> import zarr
 >>> store = imread('temp.ome.tif', aszarr=True)
 >>> z = zarr.open(store, mode='r')
 >>> z
@@ -785,15 +772,15 @@
 
 >>> imwrite(
 ...     'temp.ome.tif',
 ...     shape=(8, 800, 600),
 ...     dtype='uint16',
 ...     photometric='minisblack',
 ...     tile=(128, 128),
-...     metadata={'axes': 'CYX'},
+...     metadata={'axes': 'CYX'}
 ... )
 >>> store = imread('temp.ome.tif', mode='r+', aszarr=True)
 >>> z = zarr.open(store, mode='r+')
 >>> z
 <zarr.core.Array (8, 800, 600) uint16>
 >>> z[3, 100:200, 200:300:2] = 1024
 >>> store.close()
@@ -810,15 +797,17 @@
 (2, 64, 64)
 >>> image_sequence.dtype
 dtype('float64')
 
 Read an image stack from a series of TIFF files with a file name pattern
 as NumPy or Zarr arrays:
 
->>> image_sequence = TiffSequence('temp_C0*.tif', pattern=r'_(C)(\d+)(T)(\d+)')
+>>> image_sequence = TiffSequence(
+...     'temp_C0*.tif', pattern=r'_(C)(\d+)(T)(\d+)'
+... )
 >>> image_sequence.shape
 (1, 2)
 >>> image_sequence.axes
 'CT'
 >>> data = image_sequence.asarray()
 >>> data.shape
 (1, 2, 64, 64)
```

### Comparing `tifffile-2024.5.10/tifffile.egg-info/SOURCES.txt` & `tifffile-2024.5.3/tifffile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

