# Comparing `tmp/pyobs_core-1.8.0.tar.gz` & `tmp/pyobs_core-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobs_core-1.8.0.tar", max compression
+gzip compressed data, was "pyobs_core-1.9.0.tar", max compression
```

## Comparing `pyobs_core-1.8.0.tar` & `pyobs_core-1.9.0.tar`

### file list

```diff
@@ -1,314 +1,314 @@
--rw-r--r--   0        0        0     1099 2023-12-20 10:06:00.473063 pyobs_core-1.8.0/LICENSE
--rw-r--r--   0        0        0       80 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/__init__.py
--rw-r--r--   0        0        0     6651 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/application.py
--rw-r--r--   0        0        0        0 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/cli/__init__.py
--rwxr-xr-x   0        0        0     2559 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/cli/pyobs.py
--rwxr-xr-x   0        0        0     8257 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/cli/pyobsd.py
--rw-r--r--   0        0        0      299 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/cli/pyobsw.py
--rw-r--r--   0        0        0     1568 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/comm/__init__.py
--rw-r--r--   0        0        0    15114 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/comm/comm.py
--rw-r--r--   0        0        0      995 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/comm/commlogging.py
--rw-r--r--   0        0        0       31 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/comm/dbus/__init__.py
--rw-r--r--   0        0        0    19668 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/comm/dbus/dbuscomm.py
--rw-r--r--   0        0        0     4091 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/comm/dbus/patch.py
--rw-r--r--   0        0        0       33 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/comm/dummy/__init__.py
--rw-r--r--   0        0        0     1409 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/comm/dummy/dummycomm.py
--rw-r--r--   0        0        0       72 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/comm/local/__init__.py
--rw-r--r--   0        0        0     2969 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/comm/local/localcomm.py
--rw-r--r--   0        0        0      851 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/comm/local/localnetwork.py
--rw-r--r--   0        0        0     4525 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/comm/proxy.py
--rw-r--r--   0        0        0       55 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/comm/xmpp/__init__.py
--rw-r--r--   0        0        0     8696 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/comm/xmpp/rpc.py
--rw-r--r--   0        0        0      102 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/comm/xmpp/xep_0009/__init__.py
--rw-r--r--   0        0        0     6010 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/comm/xmpp/xep_0009/binding.py
--rw-r--r--   0        0        0     1607 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/comm/xmpp/xep_0009/rpc.py
--rw-r--r--   0        0        0      174 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/comm/xmpp/xep_0009_timeout/__init__.py
--rw-r--r--   0        0        0     2131 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/comm/xmpp/xep_0009_timeout/rpc.py
--rw-r--r--   0        0        0      467 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/comm/xmpp/xep_0009_timeout/stanza/RPC.py
--rw-r--r--   0        0        0      231 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/comm/xmpp/xep_0009_timeout/stanza/__init__.py
--rw-r--r--   0        0        0     3626 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/comm/xmpp/xmppclient.py
--rw-r--r--   0        0        0    18283 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/comm/xmpp/xmppcomm.py
--rw-r--r--   0        0        0     6818 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/environment.py
--rw-r--r--   0        0        0      924 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/events/__init__.py
--rw-r--r--   0        0        0      165 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/events/badweather.py
--rw-r--r--   0        0        0     2420 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/events/event.py
--rw-r--r--   0        0        0     1511 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/events/exposurestatuschanged.py
--rw-r--r--   0        0        0      528 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/events/filterchanged.py
--rw-r--r--   0        0        0      904 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/events/focusfound.py
--rw-r--r--   0        0        0     1090 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/events/goodweather.py
--rw-r--r--   0        0        0     1243 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/events/log.py
--rw-r--r--   0        0        0      196 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/events/moduleclosed.py
--rw-r--r--   0        0        0      196 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/events/moduleopened.py
--rw-r--r--   0        0        0     1601 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/events/motionstatuschanged.py
--rw-r--r--   0        0        0     1269 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/events/move.py
--rw-r--r--   0        0        0     2052 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/events/newimage.py
--rw-r--r--   0        0        0     1003 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/events/newspectrum.py
--rw-r--r--   0        0        0     1331 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/events/offsets.py
--rw-r--r--   0        0        0      181 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/events/roofclosing.py
--rw-r--r--   0        0        0      185 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/events/roofopened.py
--rw-r--r--   0        0        0      778 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/events/taskfailed.py
--rw-r--r--   0        0        0      786 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/events/taskfinished.py
--rw-r--r--   0        0        0     1689 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/events/taskstarted.py
--rw-r--r--   0        0        0      415 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/events/testevent.py
--rw-r--r--   0        0        0      138 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/images/__init__.py
--rw-r--r--   0        0        0    10868 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/images/image.py
--rw-r--r--   0        0        0      221 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/images/meta/__init__.py
--rw-r--r--   0        0        0      154 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/images/meta/altazoffsets.py
--rw-r--r--   0        0        0      110 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/images/meta/exptime.py
--rw-r--r--   0        0        0      165 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/images/meta/onskydistance.py
--rw-r--r--   0        0        0      145 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/images/meta/pixeloffsets.py
--rw-r--r--   0        0        0      154 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/images/meta/radecoffsets.py
--rw-r--r--   0        0        0     1731 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/images/meta/skyoffsets.py
--rw-r--r--   0        0        0      626 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/images/processor.py
--rw-r--r--   0        0        0       94 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/images/processors/__init__.py
--rw-r--r--   0        0        0     1196 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/images/processors/_daobackgroundremover.py
--rw-r--r--   0        0        0      102 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/images/processors/astrometry/__init__.py
--rw-r--r--   0        0        0     1647 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/images/processors/astrometry/_dotnet_request.py
--rw-r--r--   0        0        0     2383 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/images/processors/astrometry/_dotnet_request_builder.py
--rw-r--r--   0        0        0     1673 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/images/processors/astrometry/_dotnet_request_logger.py
--rw-r--r--   0        0        0     1892 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/images/processors/astrometry/_dotnet_response_saver.py
--rw-r--r--   0        0        0      547 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/images/processors/astrometry/astrometry.py
--rw-r--r--   0        0        0     2338 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/images/processors/astrometry/dotnet.py
--rw-r--r--   0        0        0      248 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/images/processors/detection/__init__.py
--rw-r--r--   0        0        0     3101 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/images/processors/detection/_pysep_stats_calculator.py
--rw-r--r--   0        0        0     1526 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/images/processors/detection/_source_catalog.py
--rw-r--r--   0        0        0     2785 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/images/processors/detection/daophot.py
--rw-r--r--   0        0        0     4995 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/images/processors/detection/pysep.py
--rw-r--r--   0        0        0      571 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/images/processors/detection/sourcedetection.py
--rw-r--r--   0        0        0      135 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/images/processors/exptime/__init__.py
--rw-r--r--   0        0        0     1658 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/images/processors/exptime/exptime.py
--rw-r--r--   0        0        0     3391 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/images/processors/exptime/star.py
--rw-r--r--   0        0        0      276 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/images/processors/misc/__init__.py
--rw-r--r--   0        0        0     2195 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/images/processors/misc/addmask.py
--rw-r--r--   0        0        0     1384 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/images/processors/misc/broadcast.py
--rw-r--r--   0        0        0        0 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/images/processors/misc/calibration/__init__.py
--rw-r--r--   0        0        0     1632 2023-12-20 10:06:00.481063 pyobs_core-1.8.0/pyobs/images/processors/misc/calibration/_calibration_cache.py
--rw-r--r--   0        0        0     1739 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/images/processors/misc/calibration/_ccddata_calibrator.py
--rw-r--r--   0        0        0     6261 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/images/processors/misc/calibration/calibration.py
--rw-r--r--   0        0        0     1228 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/images/processors/misc/createfilename.py
--rw-r--r--   0        0        0     1269 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/images/processors/misc/removebackground.py
--rw-r--r--   0        0        0     1846 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/images/processors/misc/smooth.py
--rw-r--r--   0        0        0     2205 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/images/processors/misc/softbin.py
--rw-r--r--   0        0        0      469 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/images/processors/offsets/__init__.py
--rw-r--r--   0        0        0     1883 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/images/processors/offsets/astrometry.py
--rw-r--r--   0        0        0     1873 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/images/processors/offsets/brighteststar.py
--rw-r--r--   0        0        0      518 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/images/processors/offsets/dummyoffsets.py
--rw-r--r--   0        0        0     1149 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/images/processors/offsets/fitsheader.py
--rw-r--r--   0        0        0    15073 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/images/processors/offsets/nstar.py
--rw-r--r--   0        0        0     1597 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/images/processors/offsets/offsets.py
--rw-r--r--   0        0        0     5673 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/images/processors/offsets/projected.py
--rw-r--r--   0        0        0      222 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/images/processors/photometry/__init__.py
--rw-r--r--   0        0        0      584 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/images/processors/photometry/photometry.py
--rw-r--r--   0        0        0     3856 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/images/processors/photometry/photutil.py
--rw-r--r--   0        0        0     4775 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/images/processors/photometry/pysep.py
--rw-r--r--   0        0        0      377 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IAbortable.py
--rw-r--r--   0        0        0      862 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IAcquisition.py
--rw-r--r--   0        0        0     1407 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IAutoFocus.py
--rw-r--r--   0        0        0      282 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IAutoGuiding.py
--rw-r--r--   0        0        0      272 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IAutonomous.py
--rw-r--r--   0        0        0     1041 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IBinning.py
--rw-r--r--   0        0        0      379 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/ICalibrate.py
--rw-r--r--   0        0        0      247 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/ICamera.py
--rw-r--r--   0        0        0     1776 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IConfig.py
--rw-r--r--   0        0        0     1086 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/ICooling.py
--rw-r--r--   0        0        0      660 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IData.py
--rw-r--r--   0        0        0      318 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IDome.py
--rw-r--r--   0        0        0      827 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IExposure.py
--rw-r--r--   0        0        0     1117 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IExposureTime.py
--rw-r--r--   0        0        0     1000 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IFilters.py
--rw-r--r--   0        0        0      809 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IFitsHeaderAfter.py
--rw-r--r--   0        0        0      815 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IFitsHeaderBefore.py
--rw-r--r--   0        0        0      586 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IFlatField.py
--rw-r--r--   0        0        0      570 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IFocusModel.py
--rw-r--r--   0        0        0     1262 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IFocuser.py
--rw-r--r--   0        0        0      751 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IGain.py
--rw-r--r--   0        0        0     1073 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IImageFormat.py
--rw-r--r--   0        0        0      774 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IImageType.py
--rw-r--r--   0        0        0      977 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/ILatLon.py
--rw-r--r--   0        0        0      965 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IMode.py
--rw-r--r--   0        0        0      998 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IModule.py
--rw-r--r--   0        0        0     1281 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IMotion.py
--rw-r--r--   0        0        0      935 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IOffsetsAltAz.py
--rw-r--r--   0        0        0      925 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IOffsetsRaDec.py
--rw-r--r--   0        0        0      888 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IPointingAltAz.py
--rw-r--r--   0        0        0      925 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IPointingHGS.py
--rw-r--r--   0        0        0      946 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IPointingHelioprojective.py
--rw-r--r--   0        0        0      894 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IPointingRaDec.py
--rw-r--r--   0        0        0      892 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IPointingSeries.py
--rw-r--r--   0        0        0      545 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IReady.py
--rw-r--r--   0        0        0      203 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IRoof.py
--rw-r--r--   0        0        0      558 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IRotation.py
--rw-r--r--   0        0        0      394 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IRunnable.py
--rw-r--r--   0        0        0      376 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IRunning.py
--rw-r--r--   0        0        0      456 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IScriptRunner.py
--rw-r--r--   0        0        0      259 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/ISpectrograph.py
--rw-r--r--   0        0        0      485 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IStartStop.py
--rw-r--r--   0        0        0      493 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/ISyncTarget.py
--rw-r--r--   0        0        0      336 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/ITelescope.py
--rw-r--r--   0        0        0      532 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/ITemperatures.py
--rw-r--r--   0        0        0      424 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IVideo.py
--rw-r--r--   0        0        0     1469 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IWeather.py
--rw-r--r--   0        0        0     1196 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/IWindow.py
--rw-r--r--   0        0        0     2150 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/__init__.py
--rw-r--r--   0        0        0      208 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/interfaces/interface.py
--rw-r--r--   0        0        0      476 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/mixins/__init__.py
--rw-r--r--   0        0        0     2372 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/mixins/camerasettings.py
--rw-r--r--   0        0        0    15027 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/mixins/fitsheader.py
--rw-r--r--   0        0        0     2723 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/mixins/fitsnamespace.py
--rw-r--r--   0        0        0     5869 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/mixins/follow.py
--rw-r--r--   0        0        0     4397 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/mixins/motionstatus.py
--rw-r--r--   0        0        0     1439 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/mixins/pipeline.py
--rw-r--r--   0        0        0     2796 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/mixins/waitformotion.py
--rw-r--r--   0        0        0     4998 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/mixins/weatheraware.py
--rw-r--r--   0        0        0     2430 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/modules/__init__.py
--rw-r--r--   0        0        0      264 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/modules/camera/__init__.py
--rw-r--r--   0        0        0    13978 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/modules/camera/adaptive.py
--rw-r--r--   0        0        0    15982 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/modules/camera/basecamera.py
--rw-r--r--   0        0        0     7025 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/modules/camera/basespectrograph.py
--rw-r--r--   0        0        0    15416 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/modules/camera/basevideo.py
--rw-r--r--   0        0        0     9507 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/modules/camera/dummycamera.py
--rw-r--r--   0        0        0     2610 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/modules/camera/dummyspectrograph.py
--rw-r--r--   0        0        0      202 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/modules/flatfield/__init__.py
--rw-r--r--   0        0        0     9085 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/modules/flatfield/flatfield.py
--rw-r--r--   0        0        0     1505 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/modules/flatfield/pointing.py
--rw-r--r--   0        0        0     4397 2023-12-20 10:06:00.485063 pyobs_core-1.8.0/pyobs/modules/flatfield/scheduler.py
--rw-r--r--   0        0        0      154 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/focus/__init__.py
--rw-r--r--   0        0        0    18119 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/focus/focusmodel.py
--rw-r--r--   0        0        0     9638 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/focus/focusseries.py
--rw-r--r--   0        0        0      189 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/image/__init__.py
--rw-r--r--   0        0        0     8221 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/image/imagewatcher.py
--rw-r--r--   0        0        0     2935 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/image/imagewriter.py
--rw-r--r--   0        0        0     3630 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/image/seeing.py
--rw-r--r--   0        0        0    17819 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/module.py
--rw-r--r--   0        0        0      348 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/pointing/__init__.py
--rw-r--r--   0        0        0     2488 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/pointing/_base.py
--rw-r--r--   0        0        0    13742 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/pointing/_baseguiding.py
--rw-r--r--   0        0        0     7339 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/pointing/acquisition.py
--rw-r--r--   0        0        0     4127 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/pointing/autoguiding.py
--rw-r--r--   0        0        0     1531 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/pointing/dummyacquisition.py
--rw-r--r--   0        0        0      828 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/pointing/dummyguiding.py
--rw-r--r--   0        0        0     3145 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/pointing/scienceframeguiding.py
--rw-r--r--   0        0        0      222 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/robotic/__init__.py
--rw-r--r--   0        0        0     5649 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/robotic/mastermind.py
--rw-r--r--   0        0        0     6840 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/robotic/pointing.py
--rw-r--r--   0        0        0    17505 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/robotic/scheduler.py
--rw-r--r--   0        0        0     1301 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/robotic/scriptrunner.py
--rw-r--r--   0        0        0      159 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/roof/__init__.py
--rw-r--r--   0        0        0     1311 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/roof/basedome.py
--rw-r--r--   0        0        0     2102 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/roof/baseroof.py
--rw-r--r--   0        0        0     3967 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/roof/dummyroof.py
--rw-r--r--   0        0        0      158 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/telescope/__init__.py
--rw-r--r--   0        0        0    11418 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/telescope/basetelescope.py
--rw-r--r--   0        0        0    10625 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/telescope/dummytelescope.py
--rw-r--r--   0        0        0      101 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/test/__init__.py
--rw-r--r--   0        0        0     1050 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/test/standalone.py
--rw-r--r--   0        0        0      279 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/utils/__init__.py
--rw-r--r--   0        0        0     4945 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/utils/autonomouswarning.py
--rw-r--r--   0        0        0     1663 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/utils/fluentlogger.py
--rw-r--r--   0        0        0     3304 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/utils/httpfilecache.py
--rw-r--r--   0        0        0     4728 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/utils/kiosk.py
--rw-r--r--   0        0        0     3700 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/utils/stellarium.py
--rw-r--r--   0        0        0    19787 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/utils/telegram.py
--rw-r--r--   0        0        0     2980 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/utils/trigger.py
--rw-r--r--   0        0        0       93 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/weather/__init__.py
--rw-r--r--   0        0        0     8180 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/modules/weather/weather.py
--rw-r--r--   0        0        0    18099 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/object.py
--rw-r--r--   0        0        0      134 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/robotic/__init__.py
--rw-r--r--   0        0        0      160 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/robotic/lco/__init__.py
--rw-r--r--   0        0        0     3766 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/robotic/lco/dummytaskschedule.py
--rw-r--r--   0        0        0     2628 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/robotic/lco/portal.py
--rw-r--r--   0        0        0      110 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/robotic/lco/scripts/__init__.py
--rw-r--r--   0        0        0     5651 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/robotic/lco/scripts/autofocus.py
--rw-r--r--   0        0        0    11915 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/robotic/lco/scripts/default.py
--rw-r--r--   0        0        0     2064 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/robotic/lco/scripts/script.py
--rw-r--r--   0        0        0    10145 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/robotic/lco/task.py
--rw-r--r--   0        0        0     5045 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/robotic/lco/taskarchive.py
--rw-r--r--   0        0        0    13522 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/robotic/lco/taskschedule.py
--rw-r--r--   0        0        0      247 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/robotic/scripts/__init__.py
--rw-r--r--   0        0        0     1607 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/robotic/scripts/conditional.py
--rw-r--r--   0        0        0     3168 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/robotic/scripts/darkbias.py
--rw-r--r--   0        0        0       31 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/robotic/scripts/flatfield/__init__.py
--rw-r--r--   0        0        0     2023 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/robotic/scripts/flatfield/pointing.py
--rw-r--r--   0        0        0     1210 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/robotic/scripts/parallel.py
--rw-r--r--   0        0        0     1540 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/robotic/scripts/script.py
--rw-r--r--   0        0        0     1871 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/robotic/scripts/selector.py
--rw-r--r--   0        0        0     1120 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/robotic/scripts/sequential.py
--rw-r--r--   0        0        0     4545 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/robotic/scripts/skyflats.py
--rw-r--r--   0        0        0     2326 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/robotic/task.py
--rw-r--r--   0        0        0      702 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/robotic/taskarchive.py
--rw-r--r--   0        0        0     1362 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/robotic/taskrunner.py
--rw-r--r--   0        0        0     1501 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/robotic/taskschedule.py
--rw-r--r--   0        0        0        0 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/utils/__init__.py
--rw-r--r--   0        0        0      174 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/utils/archive/__init__.py
--rw-r--r--   0        0        0     3221 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/utils/archive/archive.py
--rw-r--r--   0        0        0     7764 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/utils/archive/local_archive.py
--rw-r--r--   0        0        0     8971 2023-12-20 10:06:00.489063 pyobs_core-1.8.0/pyobs/utils/archive/pyobs_archive.py
--rw-r--r--   0        0        0     1381 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/average.py
--rw-r--r--   0        0        0     2844 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/cache.py
--rw-r--r--   0        0        0     3554 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/config.py
--rw-r--r--   0        0        0     1025 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/coordinates.py
--rw-r--r--   0        0        0      802 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/curvefit.py
--rw-r--r--   0        0        0     3676 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/enums.py
--rw-r--r--   0        0        0     7528 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/exceptions.py
--rw-r--r--   0        0        0     8317 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/fits.py
--rw-r--r--   0        0        0      175 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/focusseries/__init__.py
--rw-r--r--   0        0        0      779 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/focusseries/base.py
--rw-r--r--   0        0        0     2768 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/focusseries/photometry.py
--rw-r--r--   0        0        0     6503 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/focusseries/projection.py
--rw-r--r--   0        0        0     2800 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/grids.py
--rw-r--r--   0        0        0     1099 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/http.py
--rw-r--r--   0        0        0      671 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/logger.py
--rw-r--r--   0        0        0     1485 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/modulegui.py
--rw-r--r--   0        0        0      137 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/offsets/__init__.py
--rw-r--r--   0        0        0     3734 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/offsets/applyaltazoffsets.py
--rw-r--r--   0        0        0     3658 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/offsets/applyoffsets.py
--rw-r--r--   0        0        0     3486 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/offsets/applyradecoffsets.py
--rw-r--r--   0        0        0     3324 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/parallel.py
--rw-r--r--   0        0        0     1669 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/pid.py
--rw-r--r--   0        0        0       56 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/pipeline/__init__.py
--rw-r--r--   0        0        0    10047 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/pipeline/night.py
--rw-r--r--   0        0        0     7003 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/pipeline/pipeline.py
--rw-r--r--   0        0        0      159 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/publisher/__init__.py
--rw-r--r--   0        0        0     1335 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/publisher/csv.py
--rw-r--r--   0        0        0     3097 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/publisher/http.py
--rw-r--r--   0        0        0      852 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/publisher/log.py
--rw-r--r--   0        0        0      963 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/publisher/multi.py
--rw-r--r--   0        0        0      360 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/publisher/publisher.py
--rw-r--r--   0        0        0      146 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/simulation/__init__.py
--rw-r--r--   0        0        0     9339 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/simulation/camera.py
--rw-r--r--   0        0        0     7294 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/simulation/telescope.py
--rw-r--r--   0        0        0     3024 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/simulation/world.py
--rw-r--r--   0        0        0      120 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/skyflats/__init__.py
--rw-r--r--   0        0        0     7619 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/skyflats/exptimeeval.py
--rw-r--r--   0        0        0    19967 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/skyflats/flatfielder.py
--rw-r--r--   0        0        0      204 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/skyflats/pointing/__init__.py
--rw-r--r--   0        0        0      607 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/skyflats/pointing/base.py
--rw-r--r--   0        0        0     1899 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/skyflats/pointing/static.py
--rw-r--r--   0        0        0      184 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/skyflats/priorities/__init__.py
--rw-r--r--   0        0        0     2149 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/skyflats/priorities/archive.py
--rw-r--r--   0        0        0      283 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/skyflats/priorities/base.py
--rw-r--r--   0        0        0      543 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/skyflats/priorities/const.py
--rw-r--r--   0        0        0     6567 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/skyflats/scheduler.py
--rw-r--r--   0        0        0      117 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/threads/__init__.py
--rw-r--r--   0        0        0      577 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/threads/checkabort.py
--rw-r--r--   0        0        0     1410 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/threads/lockwithabort.py
--rw-r--r--   0        0        0     1115 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/threads/threadwithreturnvalue.py
--rw-r--r--   0        0        0     2020 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/time.py
--rw-r--r--   0        0        0     8107 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/utils/types.py
--rw-r--r--   0        0        0      257 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/version.py
--rw-r--r--   0        0        0     3401 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/vfs/__init__.py
--rw-r--r--   0        0        0     2402 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/vfs/archivefile.py
--rw-r--r--   0        0        0     2042 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/vfs/file.py
--rw-r--r--   0        0        0       68 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/vfs/filelists/__init__.py
--rw-r--r--   0        0        0      185 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/vfs/filelists/filelist.py
--rw-r--r--   0        0        0      396 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/vfs/filelists/testing.py
--rw-r--r--   0        0        0     5417 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/vfs/httpfile.py
--rw-r--r--   0        0        0     4591 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/vfs/localfile.py
--rw-r--r--   0        0        0     1794 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/vfs/memfile.py
--rw-r--r--   0        0        0     3687 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/vfs/sftpfile.py
--rw-r--r--   0        0        0     3789 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/vfs/smbfile.py
--rw-r--r--   0        0        0     4924 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/vfs/sshfile.py
--rw-r--r--   0        0        0     2682 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/vfs/tempfile.py
--rw-r--r--   0        0        0     9206 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyobs/vfs/vfs.py
--rw-r--r--   0        0        0     2006 2023-12-20 10:06:00.493063 pyobs_core-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     1797 1970-01-01 00:00:00.000000 pyobs_core-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-12-23 10:57:57.605576 pyobs_core-1.9.0/LICENSE
+-rw-r--r--   0        0        0       80 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/__init__.py
+-rw-r--r--   0        0        0     6685 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/application.py
+-rw-r--r--   0        0        0        0 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/cli/__init__.py
+-rwxr-xr-x   0        0        0     2730 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/cli/pyobs.py
+-rwxr-xr-x   0        0        0     8257 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/cli/pyobsd.py
+-rw-r--r--   0        0        0      307 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/cli/pyobsw.py
+-rw-r--r--   0        0        0     1568 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/comm/__init__.py
+-rw-r--r--   0        0        0    15114 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/comm/comm.py
+-rw-r--r--   0        0        0      995 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/comm/commlogging.py
+-rw-r--r--   0        0        0       31 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/comm/dbus/__init__.py
+-rw-r--r--   0        0        0    19668 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/comm/dbus/dbuscomm.py
+-rw-r--r--   0        0        0     4099 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/comm/dbus/patch.py
+-rw-r--r--   0        0        0       33 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/comm/dummy/__init__.py
+-rw-r--r--   0        0        0     1698 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/comm/dummy/dummycomm.py
+-rw-r--r--   0        0        0       72 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/comm/local/__init__.py
+-rw-r--r--   0        0        0     3063 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/comm/local/localcomm.py
+-rw-r--r--   0        0        0      913 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/comm/local/localnetwork.py
+-rw-r--r--   0        0        0     4525 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/comm/proxy.py
+-rw-r--r--   0        0        0       55 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/comm/xmpp/__init__.py
+-rw-r--r--   0        0        0     8696 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/comm/xmpp/rpc.py
+-rw-r--r--   0        0        0      102 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/comm/xmpp/xep_0009/__init__.py
+-rw-r--r--   0        0        0     6010 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/comm/xmpp/xep_0009/binding.py
+-rw-r--r--   0        0        0     1607 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/comm/xmpp/xep_0009/rpc.py
+-rw-r--r--   0        0        0      174 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/comm/xmpp/xep_0009_timeout/__init__.py
+-rw-r--r--   0        0        0     2131 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/comm/xmpp/xep_0009_timeout/rpc.py
+-rw-r--r--   0        0        0      467 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/comm/xmpp/xep_0009_timeout/stanza/RPC.py
+-rw-r--r--   0        0        0      231 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/comm/xmpp/xep_0009_timeout/stanza/__init__.py
+-rw-r--r--   0        0        0     3626 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/comm/xmpp/xmppclient.py
+-rw-r--r--   0        0        0    18283 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/comm/xmpp/xmppcomm.py
+-rw-r--r--   0        0        0     6818 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/environment.py
+-rw-r--r--   0        0        0      924 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/events/__init__.py
+-rw-r--r--   0        0        0      165 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/events/badweather.py
+-rw-r--r--   0        0        0     2420 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/events/event.py
+-rw-r--r--   0        0        0     1511 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/events/exposurestatuschanged.py
+-rw-r--r--   0        0        0      528 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/events/filterchanged.py
+-rw-r--r--   0        0        0      904 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/events/focusfound.py
+-rw-r--r--   0        0        0     1090 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/events/goodweather.py
+-rw-r--r--   0        0        0     1243 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/events/log.py
+-rw-r--r--   0        0        0      196 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/events/moduleclosed.py
+-rw-r--r--   0        0        0      196 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/events/moduleopened.py
+-rw-r--r--   0        0        0     1601 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/events/motionstatuschanged.py
+-rw-r--r--   0        0        0     1269 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/events/move.py
+-rw-r--r--   0        0        0     2052 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/events/newimage.py
+-rw-r--r--   0        0        0     1003 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/events/newspectrum.py
+-rw-r--r--   0        0        0     1331 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/events/offsets.py
+-rw-r--r--   0        0        0      181 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/events/roofclosing.py
+-rw-r--r--   0        0        0      185 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/events/roofopened.py
+-rw-r--r--   0        0        0      778 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/events/taskfailed.py
+-rw-r--r--   0        0        0      786 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/events/taskfinished.py
+-rw-r--r--   0        0        0     1689 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/events/taskstarted.py
+-rw-r--r--   0        0        0      415 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/events/testevent.py
+-rw-r--r--   0        0        0      138 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/images/__init__.py
+-rw-r--r--   0        0        0    13421 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/images/image.py
+-rw-r--r--   0        0        0      221 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/images/meta/__init__.py
+-rw-r--r--   0        0        0      154 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/images/meta/altazoffsets.py
+-rw-r--r--   0        0        0      110 2023-12-23 10:57:57.609576 pyobs_core-1.9.0/pyobs/images/meta/exptime.py
+-rw-r--r--   0        0        0      165 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/meta/onskydistance.py
+-rw-r--r--   0        0        0      145 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/meta/pixeloffsets.py
+-rw-r--r--   0        0        0      154 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/meta/radecoffsets.py
+-rw-r--r--   0        0        0     1731 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/meta/skyoffsets.py
+-rw-r--r--   0        0        0      626 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processor.py
+-rw-r--r--   0        0        0       94 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/__init__.py
+-rw-r--r--   0        0        0     1307 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/_daobackgroundremover.py
+-rw-r--r--   0        0        0      102 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/astrometry/__init__.py
+-rw-r--r--   0        0        0     1818 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/astrometry/_dotnet_request.py
+-rw-r--r--   0        0        0     2463 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/astrometry/_dotnet_request_builder.py
+-rw-r--r--   0        0        0     1690 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/astrometry/_dotnet_request_logger.py
+-rw-r--r--   0        0        0     2149 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/astrometry/_dotnet_response_saver.py
+-rw-r--r--   0        0        0      547 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/astrometry/astrometry.py
+-rw-r--r--   0        0        0     2338 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/astrometry/dotnet.py
+-rw-r--r--   0        0        0      248 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/detection/__init__.py
+-rw-r--r--   0        0        0     3101 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/detection/_pysep_stats_calculator.py
+-rw-r--r--   0        0        0     1526 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/detection/_source_catalog.py
+-rw-r--r--   0        0        0     2790 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/detection/daophot.py
+-rw-r--r--   0        0        0     5053 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/detection/pysep.py
+-rw-r--r--   0        0        0      571 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/detection/sourcedetection.py
+-rw-r--r--   0        0        0      135 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/exptime/__init__.py
+-rw-r--r--   0        0        0     1658 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/exptime/exptime.py
+-rw-r--r--   0        0        0     3396 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/exptime/star.py
+-rw-r--r--   0        0        0      276 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/misc/__init__.py
+-rw-r--r--   0        0        0     2195 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/misc/addmask.py
+-rw-r--r--   0        0        0     1384 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/misc/broadcast.py
+-rw-r--r--   0        0        0        0 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/misc/calibration/__init__.py
+-rw-r--r--   0        0        0     1632 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/misc/calibration/_calibration_cache.py
+-rw-r--r--   0        0        0     1739 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/misc/calibration/_ccddata_calibrator.py
+-rw-r--r--   0        0        0     6261 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/misc/calibration/calibration.py
+-rw-r--r--   0        0        0     1228 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/misc/createfilename.py
+-rw-r--r--   0        0        0     1269 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/misc/removebackground.py
+-rw-r--r--   0        0        0     1851 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/misc/smooth.py
+-rw-r--r--   0        0        0     2215 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/misc/softbin.py
+-rw-r--r--   0        0        0      469 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/offsets/__init__.py
+-rw-r--r--   0        0        0     1883 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/offsets/astrometry.py
+-rw-r--r--   0        0        0     1878 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/offsets/brighteststar.py
+-rw-r--r--   0        0        0      518 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/offsets/dummyoffsets.py
+-rw-r--r--   0        0        0     1149 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/offsets/fitsheader.py
+-rw-r--r--   0        0        0    14868 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/offsets/nstar.py
+-rw-r--r--   0        0        0     1597 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/offsets/offsets.py
+-rw-r--r--   0        0        0     5572 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/offsets/projected.py
+-rw-r--r--   0        0        0      222 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/photometry/__init__.py
+-rw-r--r--   0        0        0      584 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/photometry/photometry.py
+-rw-r--r--   0        0        0     3888 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/photometry/photutil.py
+-rw-r--r--   0        0        0     4812 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/images/processors/photometry/pysep.py
+-rw-r--r--   0        0        0      377 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IAbortable.py
+-rw-r--r--   0        0        0      862 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IAcquisition.py
+-rw-r--r--   0        0        0     1407 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IAutoFocus.py
+-rw-r--r--   0        0        0      282 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IAutoGuiding.py
+-rw-r--r--   0        0        0      272 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IAutonomous.py
+-rw-r--r--   0        0        0     1041 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IBinning.py
+-rw-r--r--   0        0        0      379 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/ICalibrate.py
+-rw-r--r--   0        0        0      247 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/ICamera.py
+-rw-r--r--   0        0        0     1776 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IConfig.py
+-rw-r--r--   0        0        0     1086 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/ICooling.py
+-rw-r--r--   0        0        0      660 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IData.py
+-rw-r--r--   0        0        0      318 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IDome.py
+-rw-r--r--   0        0        0      827 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IExposure.py
+-rw-r--r--   0        0        0     1117 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IExposureTime.py
+-rw-r--r--   0        0        0     1000 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IFilters.py
+-rw-r--r--   0        0        0      809 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IFitsHeaderAfter.py
+-rw-r--r--   0        0        0      815 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IFitsHeaderBefore.py
+-rw-r--r--   0        0        0      586 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IFlatField.py
+-rw-r--r--   0        0        0      570 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IFocusModel.py
+-rw-r--r--   0        0        0     1262 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IFocuser.py
+-rw-r--r--   0        0        0      751 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IGain.py
+-rw-r--r--   0        0        0     1073 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IImageFormat.py
+-rw-r--r--   0        0        0      774 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IImageType.py
+-rw-r--r--   0        0        0      977 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/ILatLon.py
+-rw-r--r--   0        0        0      965 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IMode.py
+-rw-r--r--   0        0        0      998 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IModule.py
+-rw-r--r--   0        0        0     1281 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IMotion.py
+-rw-r--r--   0        0        0      935 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IOffsetsAltAz.py
+-rw-r--r--   0        0        0      925 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IOffsetsRaDec.py
+-rw-r--r--   0        0        0      888 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IPointingAltAz.py
+-rw-r--r--   0        0        0      925 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IPointingHGS.py
+-rw-r--r--   0        0        0      946 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IPointingHelioprojective.py
+-rw-r--r--   0        0        0      894 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IPointingRaDec.py
+-rw-r--r--   0        0        0      892 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IPointingSeries.py
+-rw-r--r--   0        0        0      545 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IReady.py
+-rw-r--r--   0        0        0      203 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IRoof.py
+-rw-r--r--   0        0        0      558 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IRotation.py
+-rw-r--r--   0        0        0      394 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IRunnable.py
+-rw-r--r--   0        0        0      376 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IRunning.py
+-rw-r--r--   0        0        0      456 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IScriptRunner.py
+-rw-r--r--   0        0        0      259 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/ISpectrograph.py
+-rw-r--r--   0        0        0      485 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IStartStop.py
+-rw-r--r--   0        0        0      493 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/ISyncTarget.py
+-rw-r--r--   0        0        0      336 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/ITelescope.py
+-rw-r--r--   0        0        0      532 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/ITemperatures.py
+-rw-r--r--   0        0        0      424 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IVideo.py
+-rw-r--r--   0        0        0     1469 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IWeather.py
+-rw-r--r--   0        0        0     1196 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/IWindow.py
+-rw-r--r--   0        0        0     2150 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/__init__.py
+-rw-r--r--   0        0        0      208 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/interfaces/interface.py
+-rw-r--r--   0        0        0      476 2023-12-23 10:57:57.613576 pyobs_core-1.9.0/pyobs/mixins/__init__.py
+-rw-r--r--   0        0        0     2372 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/mixins/camerasettings.py
+-rw-r--r--   0        0        0    15027 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/mixins/fitsheader.py
+-rw-r--r--   0        0        0     2723 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/mixins/fitsnamespace.py
+-rw-r--r--   0        0        0     5869 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/mixins/follow.py
+-rw-r--r--   0        0        0     4397 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/mixins/motionstatus.py
+-rw-r--r--   0        0        0     1439 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/mixins/pipeline.py
+-rw-r--r--   0        0        0     2796 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/mixins/waitformotion.py
+-rw-r--r--   0        0        0     4998 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/mixins/weatheraware.py
+-rw-r--r--   0        0        0     2430 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/__init__.py
+-rw-r--r--   0        0        0      264 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/camera/__init__.py
+-rw-r--r--   0        0        0    13978 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/camera/adaptive.py
+-rw-r--r--   0        0        0    15987 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/camera/basecamera.py
+-rw-r--r--   0        0        0     7025 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/camera/basespectrograph.py
+-rw-r--r--   0        0        0    15416 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/camera/basevideo.py
+-rw-r--r--   0        0        0     9507 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/camera/dummycamera.py
+-rw-r--r--   0        0        0     2610 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/camera/dummyspectrograph.py
+-rw-r--r--   0        0        0      202 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/flatfield/__init__.py
+-rw-r--r--   0        0        0     9085 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/flatfield/flatfield.py
+-rw-r--r--   0        0        0     1505 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/flatfield/pointing.py
+-rw-r--r--   0        0        0     4397 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/flatfield/scheduler.py
+-rw-r--r--   0        0        0      154 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/focus/__init__.py
+-rw-r--r--   0        0        0    18119 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/focus/focusmodel.py
+-rw-r--r--   0        0        0     9638 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/focus/focusseries.py
+-rw-r--r--   0        0        0      189 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/image/__init__.py
+-rw-r--r--   0        0        0     8221 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/image/imagewatcher.py
+-rw-r--r--   0        0        0     2935 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/image/imagewriter.py
+-rw-r--r--   0        0        0     3635 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/image/seeing.py
+-rw-r--r--   0        0        0    17819 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/module.py
+-rw-r--r--   0        0        0      348 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/pointing/__init__.py
+-rw-r--r--   0        0        0     2488 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/pointing/_base.py
+-rw-r--r--   0        0        0    13742 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/pointing/_baseguiding.py
+-rw-r--r--   0        0        0     7339 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/pointing/acquisition.py
+-rw-r--r--   0        0        0     4127 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/pointing/autoguiding.py
+-rw-r--r--   0        0        0     1531 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/pointing/dummyacquisition.py
+-rw-r--r--   0        0        0      828 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/pointing/dummyguiding.py
+-rw-r--r--   0        0        0     3145 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/pointing/scienceframeguiding.py
+-rw-r--r--   0        0        0      222 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/robotic/__init__.py
+-rw-r--r--   0        0        0     5649 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/robotic/mastermind.py
+-rw-r--r--   0        0        0     6840 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/robotic/pointing.py
+-rw-r--r--   0        0        0    17505 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/robotic/scheduler.py
+-rw-r--r--   0        0        0     1301 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/robotic/scriptrunner.py
+-rw-r--r--   0        0        0      159 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/roof/__init__.py
+-rw-r--r--   0        0        0     1311 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/roof/basedome.py
+-rw-r--r--   0        0        0     2102 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/roof/baseroof.py
+-rw-r--r--   0        0        0     3967 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/roof/dummyroof.py
+-rw-r--r--   0        0        0      158 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/telescope/__init__.py
+-rw-r--r--   0        0        0    11418 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/telescope/basetelescope.py
+-rw-r--r--   0        0        0    10625 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/telescope/dummytelescope.py
+-rw-r--r--   0        0        0      101 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/test/__init__.py
+-rw-r--r--   0        0        0     1050 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/test/standalone.py
+-rw-r--r--   0        0        0      279 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/utils/__init__.py
+-rw-r--r--   0        0        0     4945 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/utils/autonomouswarning.py
+-rw-r--r--   0        0        0     1663 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/utils/fluentlogger.py
+-rw-r--r--   0        0        0     3304 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/utils/httpfilecache.py
+-rw-r--r--   0        0        0     4728 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/utils/kiosk.py
+-rw-r--r--   0        0        0     3700 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/utils/stellarium.py
+-rw-r--r--   0        0        0    19787 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/utils/telegram.py
+-rw-r--r--   0        0        0     2980 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/utils/trigger.py
+-rw-r--r--   0        0        0       93 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/weather/__init__.py
+-rw-r--r--   0        0        0     8180 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/modules/weather/weather.py
+-rw-r--r--   0        0        0    18099 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/object.py
+-rw-r--r--   0        0        0      134 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/robotic/__init__.py
+-rw-r--r--   0        0        0      160 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/robotic/lco/__init__.py
+-rw-r--r--   0        0        0     3766 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/robotic/lco/dummytaskschedule.py
+-rw-r--r--   0        0        0     2628 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/robotic/lco/portal.py
+-rw-r--r--   0        0        0      110 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/robotic/lco/scripts/__init__.py
+-rw-r--r--   0        0        0     5651 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/robotic/lco/scripts/autofocus.py
+-rw-r--r--   0        0        0    11915 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/robotic/lco/scripts/default.py
+-rw-r--r--   0        0        0     2064 2023-12-23 10:57:57.617576 pyobs_core-1.9.0/pyobs/robotic/lco/scripts/script.py
+-rw-r--r--   0        0        0    10145 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/robotic/lco/task.py
+-rw-r--r--   0        0        0     5045 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/robotic/lco/taskarchive.py
+-rw-r--r--   0        0        0    13522 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/robotic/lco/taskschedule.py
+-rw-r--r--   0        0        0      247 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/robotic/scripts/__init__.py
+-rw-r--r--   0        0        0     1607 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/robotic/scripts/conditional.py
+-rw-r--r--   0        0        0     3168 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/robotic/scripts/darkbias.py
+-rw-r--r--   0        0        0       31 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/robotic/scripts/flatfield/__init__.py
+-rw-r--r--   0        0        0     2023 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/robotic/scripts/flatfield/pointing.py
+-rw-r--r--   0        0        0     1458 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/robotic/scripts/parallel.py
+-rw-r--r--   0        0        0     1540 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/robotic/scripts/script.py
+-rw-r--r--   0        0        0     1871 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/robotic/scripts/selector.py
+-rw-r--r--   0        0        0     1411 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/robotic/scripts/sequential.py
+-rw-r--r--   0        0        0     4545 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/robotic/scripts/skyflats.py
+-rw-r--r--   0        0        0     2326 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/robotic/task.py
+-rw-r--r--   0        0        0      702 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/robotic/taskarchive.py
+-rw-r--r--   0        0        0     1362 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/robotic/taskrunner.py
+-rw-r--r--   0        0        0     1501 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/robotic/taskschedule.py
+-rw-r--r--   0        0        0        0 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/__init__.py
+-rw-r--r--   0        0        0      174 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/archive/__init__.py
+-rw-r--r--   0        0        0     3221 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/archive/archive.py
+-rw-r--r--   0        0        0     7764 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/archive/local_archive.py
+-rw-r--r--   0        0        0     8971 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/archive/pyobs_archive.py
+-rw-r--r--   0        0        0     1381 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/average.py
+-rw-r--r--   0        0        0     2844 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/cache.py
+-rw-r--r--   0        0        0     3554 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/config.py
+-rw-r--r--   0        0        0     1025 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/coordinates.py
+-rw-r--r--   0        0        0      802 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/curvefit.py
+-rw-r--r--   0        0        0     3676 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/enums.py
+-rw-r--r--   0        0        0     7528 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/exceptions.py
+-rw-r--r--   0        0        0     8317 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/fits.py
+-rw-r--r--   0        0        0      175 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/focusseries/__init__.py
+-rw-r--r--   0        0        0      779 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/focusseries/base.py
+-rw-r--r--   0        0        0     2773 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/focusseries/photometry.py
+-rw-r--r--   0        0        0     6508 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/focusseries/projection.py
+-rw-r--r--   0        0        0     2800 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/grids.py
+-rw-r--r--   0        0        0     1099 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/http.py
+-rw-r--r--   0        0        0      671 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/logger.py
+-rw-r--r--   0        0        0     1485 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/modulegui.py
+-rw-r--r--   0        0        0      137 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/offsets/__init__.py
+-rw-r--r--   0        0        0     3734 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/offsets/applyaltazoffsets.py
+-rw-r--r--   0        0        0     3658 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/offsets/applyoffsets.py
+-rw-r--r--   0        0        0     3486 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/offsets/applyradecoffsets.py
+-rw-r--r--   0        0        0     3324 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/parallel.py
+-rw-r--r--   0        0        0     1669 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/pid.py
+-rw-r--r--   0        0        0       56 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/pipeline/__init__.py
+-rw-r--r--   0        0        0    10047 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/pipeline/night.py
+-rw-r--r--   0        0        0     7003 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/pipeline/pipeline.py
+-rw-r--r--   0        0        0      159 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/publisher/__init__.py
+-rw-r--r--   0        0        0     1335 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/publisher/csv.py
+-rw-r--r--   0        0        0     3097 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/publisher/http.py
+-rw-r--r--   0        0        0      852 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/publisher/log.py
+-rw-r--r--   0        0        0      963 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/publisher/multi.py
+-rw-r--r--   0        0        0      360 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/publisher/publisher.py
+-rw-r--r--   0        0        0      146 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/simulation/__init__.py
+-rw-r--r--   0        0        0     9339 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/simulation/camera.py
+-rw-r--r--   0        0        0     7294 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/simulation/telescope.py
+-rw-r--r--   0        0        0     3024 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/simulation/world.py
+-rw-r--r--   0        0        0      120 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/skyflats/__init__.py
+-rw-r--r--   0        0        0     7619 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/skyflats/exptimeeval.py
+-rw-r--r--   0        0        0    19967 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/skyflats/flatfielder.py
+-rw-r--r--   0        0        0      204 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/skyflats/pointing/__init__.py
+-rw-r--r--   0        0        0      607 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/skyflats/pointing/base.py
+-rw-r--r--   0        0        0     1899 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/skyflats/pointing/static.py
+-rw-r--r--   0        0        0      184 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/skyflats/priorities/__init__.py
+-rw-r--r--   0        0        0     2149 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/skyflats/priorities/archive.py
+-rw-r--r--   0        0        0      283 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/skyflats/priorities/base.py
+-rw-r--r--   0        0        0      543 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/skyflats/priorities/const.py
+-rw-r--r--   0        0        0     6567 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/skyflats/scheduler.py
+-rw-r--r--   0        0        0      117 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/threads/__init__.py
+-rw-r--r--   0        0        0      577 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/threads/checkabort.py
+-rw-r--r--   0        0        0     1410 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/threads/lockwithabort.py
+-rw-r--r--   0        0        0     1115 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/threads/threadwithreturnvalue.py
+-rw-r--r--   0        0        0     2020 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/time.py
+-rw-r--r--   0        0        0     8107 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/utils/types.py
+-rw-r--r--   0        0        0      257 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/version.py
+-rw-r--r--   0        0        0     3401 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/vfs/__init__.py
+-rw-r--r--   0        0        0     2402 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/vfs/archivefile.py
+-rw-r--r--   0        0        0     2042 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/vfs/file.py
+-rw-r--r--   0        0        0       68 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/vfs/filelists/__init__.py
+-rw-r--r--   0        0        0      185 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/vfs/filelists/filelist.py
+-rw-r--r--   0        0        0      396 2023-12-23 10:57:57.621576 pyobs_core-1.9.0/pyobs/vfs/filelists/testing.py
+-rw-r--r--   0        0        0     5417 2023-12-23 10:57:57.625576 pyobs_core-1.9.0/pyobs/vfs/httpfile.py
+-rw-r--r--   0        0        0     4591 2023-12-23 10:57:57.625576 pyobs_core-1.9.0/pyobs/vfs/localfile.py
+-rw-r--r--   0        0        0     1794 2023-12-23 10:57:57.625576 pyobs_core-1.9.0/pyobs/vfs/memfile.py
+-rw-r--r--   0        0        0     3687 2023-12-23 10:57:57.625576 pyobs_core-1.9.0/pyobs/vfs/sftpfile.py
+-rw-r--r--   0        0        0     3789 2023-12-23 10:57:57.625576 pyobs_core-1.9.0/pyobs/vfs/smbfile.py
+-rw-r--r--   0        0        0     4924 2023-12-23 10:57:57.625576 pyobs_core-1.9.0/pyobs/vfs/sshfile.py
+-rw-r--r--   0        0        0     2682 2023-12-23 10:57:57.625576 pyobs_core-1.9.0/pyobs/vfs/tempfile.py
+-rw-r--r--   0        0        0     9206 2023-12-23 10:57:57.625576 pyobs_core-1.9.0/pyobs/vfs/vfs.py
+-rw-r--r--   0        0        0     2006 2023-12-23 10:57:57.625576 pyobs_core-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1797 1970-01-01 00:00:00.000000 pyobs_core-1.9.0/PKG-INFO
```

### Comparing `pyobs_core-1.8.0/LICENSE` & `pyobs_core-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/application.py` & `pyobs_core-1.9.0/pyobs/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 import platform
 import signal
 import warnings
 import threading
 from io import StringIO
 from logging.handlers import TimedRotatingFileHandler
-from typing import Optional, Any, Dict
+from typing import Optional, Any, Dict, List
 import yaml
 
 from pyobs.object import get_object, get_class_from_string
 from pyobs.modules import Module
 from pyobs.utils.config import pre_process_yaml
 
 # just init logger with something here, will be overwritten in __init__
@@ -31,15 +31,15 @@
         """
 
         # get config name without path and extension
         self._config = config
 
         # formatter for logging, and list of logging handlers
         formatter = logging.Formatter("%(asctime)s [%(levelname)s] %(filename)s:%(lineno)d %(message)s")
-        handlers = []
+        handlers: List[logging.Handler] = []
 
         # create stdout logging handler
         stream_handler = logging.StreamHandler()
         stream_handler.setFormatter(formatter)
         handlers.append(stream_handler)
 
         # create file logging handler, if log file is given
@@ -106,15 +106,15 @@
         group = asyncio.gather(*tasks, return_exceptions=True)
         self._loop.run_until_complete(group)
 
         # finished
         log.info("Closing loop...")
         self._loop.close()
 
-    def _signal_handler(self, sig) -> None:
+    def _signal_handler(self, sig: int) -> None:
         """React to signals and quit module."""
 
         # stop loop
         # loop = asyncio.get_running_loop()
         # loop.stop()
         self._module.quit()
```

### Comparing `pyobs_core-1.8.0/pyobs/cli/pyobs.py` & `pyobs_core-1.9.0/pyobs/cli/pyobs.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import argparse
 import os
-from typing import Type, Any
+from typing import Type, Any, Optional, TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from pyobs.application import Application
 
 from pyobs import version
 
 
-def init_cli():
+def init_cli() -> argparse.ArgumentParser:
     # init argument parsing
     # for all command line parameters we set the default to an environment variable,
     # so they can also be specified that way
     parser = argparse.ArgumentParser()
 
     # config
     parser.add_argument("config", type=str, help="Configuration file")
@@ -26,15 +29,15 @@
     # version
     parser.add_argument("-v", "--version", action="version", version=version())
 
     # return it
     return parser
 
 
-def parse_cli(parser: argparse.ArgumentParser):
+def parse_cli(parser: argparse.ArgumentParser) -> dict[str, Any]:
     from pyobs.utils.time import Time
 
     # parse args
     args = parser.parse_args()
 
     # set debug time now
     if args.debug_time is not None:
@@ -46,15 +49,15 @@
     if args.config:
         args.config = os.path.abspath(args.config)
 
     # finished
     return vars(args)
 
 
-def start_daemon(app_class, pid_file=None, **kwargs: Any) -> None:
+def start_daemon(app_class: Type["Application"], pid_file: str, **kwargs: Any) -> None:
     """Start process as a daemon.
 
     Args:
         app_class: Class to create app from
         pid_file: Name of PID file.
     """
     import daemon
@@ -66,15 +69,15 @@
     # This launches the daemon in its context
     with daemon.DaemonContext(
         working_directory=run_dir, umask=0o002, pidfile=pidfile.TimeoutPIDLockFile(pid_file)
     ) as context:
         run(app_class, **kwargs)
 
 
-def run(app_class: Type, **kwargs: Any) -> None:
+def run(app_class: Type["Application"], **kwargs: Any) -> None:
     """Run a pyobs application with the given options.
 
     Args:
         app_class: Class to create app from
     """
 
     # create app and run it
```

### Comparing `pyobs_core-1.8.0/pyobs/cli/pyobsd.py` & `pyobs_core-1.9.0/pyobs/cli/pyobsd.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/comm/__init__.py` & `pyobs_core-1.9.0/pyobs/comm/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/comm/comm.py` & `pyobs_core-1.9.0/pyobs/comm/comm.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/comm/commlogging.py` & `pyobs_core-1.9.0/pyobs/comm/commlogging.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/comm/dbus/dbuscomm.py` & `pyobs_core-1.9.0/pyobs/comm/dbus/dbuscomm.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/comm/dbus/patch.py` & `pyobs_core-1.9.0/pyobs/comm/dbus/patch.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from dbus_next.service import ServiceInterface
 from dbus_next.aio import MessageBus
 from dbus_next.message_bus import BaseMessageBus
 import dbus_next.service
 from dbus_next import introspection as intr
 
 
-def patch():
+def patch() -> None:
     """
     Patches dbus-next to allow for a providing the sender name. Probably a bad idea, but better than using
     a fork of the project.
     """
     MessageBus._make_method_handler = _aio_make_method_handler
     BaseMessageBus._make_method_handler = _make_method_handler
     dbus_next.service._Method.__init__ = _method__init__
```

### Comparing `pyobs_core-1.8.0/pyobs/comm/local/localcomm.py` & `pyobs_core-1.9.0/pyobs/comm/local/localcomm.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,24 +5,23 @@
 from pyobs.comm import Comm
 from pyobs.events import Event
 from pyobs.interfaces import Interface
 from pyobs.utils.types import cast_response_to_real
 
 
 class LocalComm(Comm):
-    def __init__(self, name: str, *args, **kwargs):
-
+    def __init__(self, name: str, *args: Any, **kwargs: Any):
         Comm.__init__(self, *args, **kwargs)
 
         self._name = name
         self._network = pyobs.comm.local.LocalNetwork()
         self._network.connect_client(self)
 
     @property
-    def name(self) -> Optional[str]:
+    def name(self) -> str:
         """Name of this client."""
         return self._name
 
     @property
     def clients(self) -> List[str]:
         """Returns list of currently connected clients.
 
@@ -41,28 +40,28 @@
             List of supported interfaces.
 
         Raises:
             IndexError: If client cannot be found.
         """
 
         remote_client: LocalComm = self._network.get_client(client)
-        return remote_client.module.interfaces
+        return [] if remote_client.module is None else remote_client.module.interfaces
 
     async def _supports_interface(self, client: str, interface: Type[Interface]) -> bool:
         """Checks, whether the given client supports the given interface.
 
         Args:
             client: Client to check.
             interface: Interface to check.
 
         Returns:
-            Whether or not interface is supported.
+            Whether interface is supported.
         """
         interfaces = await self.get_interfaces(client)
-        return interfaces in interfaces
+        return interface in interfaces
 
     async def execute(self, client: str, method: str, annotation: Dict[str, Any], *args: Any) -> Any:
         """Execute a given method on a remote client.
 
         Args:
             client (str): ID of client.
             method (str): Method to call.
@@ -70,18 +69,20 @@
             *args: List of parameters for given method.
 
         Returns:
             Passes through return from method call.
         """
 
         remote_client = self._network.get_client(client)
+        if remote_client.module is None:
+            raise ValueError
         simple_results = await remote_client.module.execute(method, *args)
         real_results = cast_response_to_real(
-                simple_results, annotation["return"], self.cast_to_real_pre, self.cast_to_real_post
-            )
+            simple_results, annotation["return"], self.cast_to_real_pre, self.cast_to_real_post
+        )
         return real_results
 
     async def send_event(self, event: Event) -> None:
         """Send an event to other clients.
 
         Args:
             event (Event): Event to send
@@ -90,8 +91,8 @@
         remote_clients = self._network.get_clients()
         for client in remote_clients:
             client._send_event_to_module(event, self.name)
 
     async def _register_events(
         self, events: List[Type[Event]], handler: Optional[Callable[[Event, str], Coroutine[Any, Any, bool]]] = None
     ) -> None:
-        pass
+        pass
```

### Comparing `pyobs_core-1.8.0/pyobs/comm/local/localnetwork.py` & `pyobs_core-1.9.0/pyobs/comm/local/localnetwork.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from __future__ import annotations
 
-from typing import Dict, List
+from typing import Dict, List, Optional
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     import pyobs.comm
 
 
 class LocalNetwork:
-    _instance = None
+    _instance: Optional["LocalNetwork"] = None
 
-    def __new__(cls):
+    def __new__(cls) -> "LocalNetwork":
         if cls._instance is None:
-            print('Creating the object')
+            print("Creating the object")
             cls._instance = super(LocalNetwork, cls).__new__(cls)
 
             cls._clients: Dict[str, pyobs.comm.local.LocalComm] = {}
 
         return cls._instance
 
-    def connect_client(self, comm: pyobs.comm.local.LocalComm):
+    def connect_client(self, comm: pyobs.comm.local.LocalComm) -> None:
         self._clients[comm.name] = comm
 
     def get_client(self, name: str) -> pyobs.comm.local.LocalComm:
         return self._clients[name]
 
     def get_clients(self) -> List[pyobs.comm.local.LocalComm]:
         return list(self._clients.values())
```

### Comparing `pyobs_core-1.8.0/pyobs/comm/proxy.py` & `pyobs_core-1.9.0/pyobs/comm/proxy.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/comm/xmpp/rpc.py` & `pyobs_core-1.9.0/pyobs/comm/xmpp/rpc.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/comm/xmpp/xep_0009/binding.py` & `pyobs_core-1.9.0/pyobs/comm/xmpp/xep_0009/binding.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/comm/xmpp/xep_0009/rpc.py` & `pyobs_core-1.9.0/pyobs/comm/xmpp/xep_0009/rpc.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/comm/xmpp/xep_0009_timeout/rpc.py` & `pyobs_core-1.9.0/pyobs/comm/xmpp/xep_0009_timeout/rpc.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/comm/xmpp/xmppclient.py` & `pyobs_core-1.9.0/pyobs/comm/xmpp/xmppclient.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/comm/xmpp/xmppcomm.py` & `pyobs_core-1.9.0/pyobs/comm/xmpp/xmppcomm.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/environment.py` & `pyobs_core-1.9.0/pyobs/environment.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/events/__init__.py` & `pyobs_core-1.9.0/pyobs/events/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/events/event.py` & `pyobs_core-1.9.0/pyobs/events/event.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/events/exposurestatuschanged.py` & `pyobs_core-1.9.0/pyobs/events/exposurestatuschanged.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/events/filterchanged.py` & `pyobs_core-1.9.0/pyobs/events/filterchanged.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/events/focusfound.py` & `pyobs_core-1.9.0/pyobs/events/focusfound.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/events/goodweather.py` & `pyobs_core-1.9.0/pyobs/events/goodweather.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/events/log.py` & `pyobs_core-1.9.0/pyobs/events/log.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/events/motionstatuschanged.py` & `pyobs_core-1.9.0/pyobs/events/motionstatuschanged.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/events/move.py` & `pyobs_core-1.9.0/pyobs/events/move.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/events/newimage.py` & `pyobs_core-1.9.0/pyobs/events/newimage.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/events/newspectrum.py` & `pyobs_core-1.9.0/pyobs/events/newspectrum.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/events/offsets.py` & `pyobs_core-1.9.0/pyobs/events/offsets.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/events/taskfailed.py` & `pyobs_core-1.9.0/pyobs/events/taskfailed.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/events/taskfinished.py` & `pyobs_core-1.9.0/pyobs/events/taskfinished.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/events/taskstarted.py` & `pyobs_core-1.9.0/pyobs/events/taskstarted.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/images/image.py` & `pyobs_core-1.9.0/pyobs/images/image.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from astropy.io import fits
 from astropy.io.fits import table_to_hdu, ImageHDU
 from astropy.table import Table
 from astropy.nddata import CCDData, StdDevUncertainty
 from numpy.typing import NDArray
 
 from pyobs.utils.fits import FilenameFormatter
+import pyobs.utils.exceptions as exc
 
 MetaClass = TypeVar("MetaClass")
 
 
 class Image:
     """Image class."""
 
@@ -41,24 +42,24 @@
             uncertainty: Uncertainty image.
             catalog: Catalog table.
             raw: If image is calibrated, this should be the raw image.
             meta: Dictionary with meta information (note: not preserved in I/O operations!).
         """
 
         # store
-        self.data = data
-        self.header = fits.Header() if header is None else header.copy()
-        self.mask = None if mask is None else mask.copy()
-        self.uncertainty = None if uncertainty is None else uncertainty.copy()
-        self.catalog = None if catalog is None else catalog.copy()
-        self.raw = None if raw is None else raw.copy()
-        self.meta = {} if meta is None else copy.deepcopy(meta)
+        self._data = data
+        self._header = fits.Header() if header is None else header.copy()
+        self._mask = None if mask is None else mask.copy()
+        self._uncertainty = None if uncertainty is None else uncertainty.copy()
+        self._catalog = None if catalog is None else catalog.copy()
+        self._raw = None if raw is None else raw.copy()
+        self._meta = {} if meta is None else copy.deepcopy(meta)
 
         # add basic header stuff
-        if data is not None:
+        if data is not None and self._header is not None:
             self.header["NAXIS1"] = data.shape[1]
             self.header["NAXIS2"] = data.shape[0]
 
     @classmethod
     def from_bytes(cls, data: bytes) -> Image:
         """Create Image from a bytes array containing a FITS file.
 
@@ -68,18 +69,18 @@
         Returns:
             The new image.
         """
 
         # create hdu
         with io.BytesIO(data) as bio:
             # read whole file
-            data = fits.open(bio, memmap=False, lazy_load_hdus=False)
+            d = fits.open(bio, memmap=False, lazy_load_hdus=False)
 
             # load image
-            return cls._from_hdu_list(data)
+            return cls._from_hdu_list(d)
 
     @classmethod
     def from_file(cls, filename: str) -> Image:
         """Create image from FITS file.
 
         Args:
             filename: Name of file to load image from.
@@ -124,43 +125,45 @@
 
         # create image
         image = cls()
 
         # find HDU with image data
         for hdu in data:
             if (
-                isinstance(hdu, fits.PrimaryHDU) and hdu.header["NAXIS"] > 0
-                or isinstance(hdu, fits.ImageHDU) and hdu.name == "SCI"
+                isinstance(hdu, fits.PrimaryHDU)
+                and hdu.header["NAXIS"] > 0
+                or isinstance(hdu, fits.ImageHDU)
+                and hdu.name == "SCI"
                 or isinstance(hdu, fits.CompImageHDU)
             ):
                 # found image HDU
                 image_hdu = hdu
                 break
         else:
             raise ValueError("Could not find HDU with main image.")
 
         # get data
         image.data = image_hdu.data
         image.header = image_hdu.header
 
         # mask
         if "MASK" in data:
-            image.mask = data["MASK"].data
+            image._mask = data["MASK"].data
 
         # uncertainties
         if "UNCERT" in data:
-            image.uncertainty = data["UNCERT"].data
+            image._uncertainty = data["UNCERT"].data
 
         # catalog
         if "CAT" in data:
-            image.catalog = Table(data["CAT"].data)
+            image._catalog = Table(data["CAT"].data)
 
         # raw
         if "RAW" in data:
-            image.raw = data["RAW"].data
+            image._raw = data["RAW"].data
 
         # finished
         return image
 
     @property
     def unit(self) -> str:
         """Returns units of pixels in image."""
@@ -172,29 +175,29 @@
     def __deepcopy__(self) -> Image:
         """Returns a shallow copy of this image."""
         return self.copy()
 
     def copy(self) -> Image:
         """Returns a copy of this image."""
         return Image(
-            data=self.data,
-            header=self.header,
-            mask=self.mask,
-            uncertainty=self.uncertainty,
-            catalog=self.catalog,
-            raw=self.raw,
-            meta=self.meta,
+            data=self._data,
+            header=self._header,
+            mask=self._mask,
+            uncertainty=self._uncertainty,
+            catalog=self._catalog,
+            raw=self._raw,
+            meta=self._meta,
         )
 
     def __truediv__(self, other: Image) -> Image:
         """Divides this image by other."""
         img = self.copy()
-        if img.data is None or other.data is None:
+        if img._data is None or other._data is None:
             raise ValueError("One image in division is None.")
-        img.data /= other.data
+        img._data /= other._data
         return img
 
     def writeto(self, f: Any, *args: Any, **kwargs: Any) -> None:
         """Write image as FITS to given file object.
 
         Args:
             f: File object to write to.
@@ -204,91 +207,91 @@
         hdu_list = fits.HDUList([])
 
         # create image HDU
         hdu = fits.PrimaryHDU(self.data, header=self.header)
         hdu_list.append(hdu)
 
         # catalog?
-        if self.catalog is not None:
-            hdu = table_to_hdu(self.catalog)
+        if self._catalog is not None:
+            hdu = table_to_hdu(self._catalog)
             hdu.name = "CAT"
             hdu_list.append(hdu)
 
         # mask?
-        if self.mask is not None:
-            hdu = ImageHDU(self.mask.astype(np.uint8))
+        if self._mask is not None:
+            hdu = ImageHDU(self._mask.astype(np.uint8))
             hdu.name = "MASK"
             hdu_list.append(hdu)
 
         # errors?
-        if self.uncertainty is not None:
-            hdu = ImageHDU(self.uncertainty.data)
+        if self._uncertainty is not None:
+            hdu = ImageHDU(self._uncertainty.data)
             hdu.name = "UNCERT"
             hdu_list.append(hdu)
 
         # raw?
-        if self.raw is not None:
-            hdu = ImageHDU(self.raw.data)
+        if self._raw is not None:
+            hdu = ImageHDU(self._raw.data)
             hdu.name = "RAW"
             hdu_list.append(hdu)
 
         # write it
         hdu_list.writeto(f, *args, **kwargs)
 
     def to_bytes(self) -> bytes:
         """Write to a bytes array and return it."""
         with io.BytesIO() as bio:
             self.writeto(bio)
             return bio.getvalue()
 
     def write_catalog(self, f: Any, *args: Any, **kwargs: Any) -> None:
         """Write catalog to file object."""
-        if self.catalog is None:
+        if self._catalog is None:
             return
 
-        hdu = table_to_hdu(self.catalog)
+        hdu = table_to_hdu(self._catalog)
         hdu.writeto(f, *args, **kwargs)
 
     def to_ccddata(self) -> CCDData:
         """Convert Image to CCDData"""
         return CCDData(
-            data=self.data,
-            meta=self.header,
-            mask=None if self.mask is None else self.mask,
-            uncertainty=None if self.uncertainty is None else StdDevUncertainty(self.uncertainty),
+            data=self._data,
+            meta=self._header,
+            mask=self._mask,
+            uncertainty=None if self._uncertainty is None else StdDevUncertainty(self._uncertainty),
             unit="adu",
         )
 
     def format_filename(self, formatter: FilenameFormatter) -> str:
         """Format filename with given formatter."""
-        self.header["FNAME"] = formatter(self.header)
-        return str(self.header["FNAME"])
+        self._header["FNAME"] = formatter(self._header)
+        return str(self._header["FNAME"])
 
     @property
     def pixel_scale(self) -> Optional[float]:
         """Returns pixel scale in arcsec/pixel."""
-        if "CD1_1" in self.header:
-            return abs(float(self.header["CD1_1"])) * 3600.0
-        elif "CDELT1" in self.header:
-            return abs(float(self.header["CDELT1"])) * 3600.0
+        if "CD1_1" in self._header:
+            return abs(float(self._header["CD1_1"])) * 3600.0
+        elif "CDELT1" in self._header:
+            return abs(float(self._header["CDELT1"])) * 3600.0
         else:
             return None
 
     def to_jpeg(self, vmin: Optional[float] = None, vmax: Optional[float] = None) -> bytes:
         """Returns a JPEG image created from this image.
 
         Returns:
             The image.
         """
 
         # import PIL Image
         import PIL.Image
 
         # copy data
-        data: NDArray[Any] = np.copy(self.data)  # type: ignore
+        data: NDArray[Any] = np.copy(self._data)  # type: ignore
         if data is None:
             raise ValueError("No data in image.")
 
         # no vmin/vmax?
         if vmin is None or vmax is None:
             flattened = sorted(data.flatten())
             vmin = flattened[int(0.05 * len(flattened))]
@@ -323,43 +326,137 @@
         set_meta/get_meta only for class-based data.
 
         Args:
             meta: Meta information to store.
         """
 
         # store it
-        self.meta[meta.__class__] = meta
+        self._meta[meta.__class__] = meta
 
     def has_meta(self, meta_class: Type[MetaClass]) -> bool:
         """Whether meta exists."""
-        return meta_class in self.meta
+        return meta_class in self._meta
 
     def get_meta(self, meta_class: Type[MetaClass]) -> MetaClass:
         """Returns meta information, assuming that it is stored under the class of the object.
 
         Args:
             meta_class: Class to return meta information for.
 
         Returns:
             Meta information of the given class.
         """
         # return default?
-        if meta_class not in self.meta:
+        if meta_class not in self._meta:
             raise ValueError("Meta value not found.")
 
         # correct type?
-        if not isinstance(self.meta[meta_class], meta_class):
+        if not isinstance(self._meta[meta_class], meta_class):
             raise ValueError("Stored meta information is of wrong type.")
 
         # return it
-        return cast(MetaClass, self.meta[meta_class])
+        return cast(MetaClass, self._meta[meta_class])
 
     def get_meta_safe(self, meta_class: Type[MetaClass], default: Optional[MetaClass] = None) -> Optional[MetaClass]:
         """Calls get_meta in a safe way and returns default value in case of an exception."""
 
         try:
             return self.get_meta(meta_class)
         except:
             return default
 
+    @property
+    def data(self) -> NDArray[Any]:
+        if self._data is None:
+            raise exc.ImageError("No data found in image.")
+        return self._data
+
+    @property
+    def safe_data(self) -> Optional[NDArray[Any]]:
+        return self._data
+
+    @data.setter
+    def data(self, val: Optional[NDArray[Any]]):
+        self._data = val
+
+    @property
+    def header(self) -> fits.Header:
+        if self._header is None:
+            raise exc.ImageError("No header found in image.")
+        return self._header
+
+    @property
+    def safe_header(self) -> Optional[fits.Header]:
+        return self._header
+
+    @header.setter
+    def header(self, val: Optional[fits.Header]):
+        self._header = val
+
+    @property
+    def mask(self) -> NDArray[Any]:
+        if self._mask is None:
+            raise exc.ImageError("No mask found in image.")
+        return self._mask
+
+    @property
+    def safe_mask(self) -> Optional[NDArray[Any]]:
+        return self._mask
+
+    @mask.setter
+    def mask(self, val: Optional[NDArray[Any]]):
+        self._mask = val
+
+    @property
+    def uncertainty(self) -> NDArray[Any]:
+        if self._uncertainty is None:
+            raise exc.ImageError("No uncertainties found in image.")
+        return self._uncertainty
+
+    @property
+    def safe_uncertainty(self) -> Optional[NDArray[Any]]:
+        return self._uncertainty
+
+    @uncertainty.setter
+    def uncertainty(self, val: Optional[NDArray[Any]]):
+        self._uncertainty = val
+
+    @property
+    def catalog(self) -> Table:
+        if self._catalog is None:
+            raise exc.ImageError("No catalog found in image.")
+        return self._catalog
+
+    @property
+    def safe_catalog(self) -> Optional[Table]:
+        return self._catalog
+
+    @catalog.setter
+    def catalog(self, val: Optional[Table]):
+        self._catalog = val
+
+    @property
+    def raw(self) -> NDArray[Any]:
+        if self._raw is None:
+            raise exc.ImageError("No raw data found in image.")
+        return self._raw
+
+    @property
+    def safe_raw(self) -> Optional[NDArray[Any]]:
+        return self._raw
+
+    @raw.setter
+    def raw(self, val: Optional[NDArray[Any]]):
+        self._raw = val
+
+    @property
+    def meta(self) -> Dict[Any, Any]:
+        if self._meta is None:
+            self._meta: Dict[Any, Any] = {}
+        return self._meta
+
+    @meta.setter
+    def meta(self, val: Optional[Dict[Any, Any]]):
+        self._meta = val
+
 
 __all__ = ["Image"]
```

### Comparing `pyobs_core-1.8.0/pyobs/images/meta/skyoffsets.py` & `pyobs_core-1.9.0/pyobs/images/meta/skyoffsets.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/images/processor.py` & `pyobs_core-1.9.0/pyobs/images/processor.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/images/processors/astrometry/_dotnet_request.py` & `pyobs_core-1.9.0/pyobs/images/processors/astrometry/_dotnet_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,53 @@
-from typing import Dict, Optional
-
+from typing import Dict, Optional, Any
 import aiohttp
 
 import pyobs.utils.exceptions as exc
 
 
 class _DotNetRequest:
-    def __init__(self, request_data: Dict[str, any]):
+    def __init__(self, request_data: Dict[str, Any]):
         self._request_data = request_data
 
-        self._response_data: Optional[Dict[str, any]] = None
+        self._response_data: Optional[Dict[str, Any]] = None
         self._status_code: Optional[int] = None
 
-    async def _send_request(self, url: str, timeout: int):
+    async def _send_request(self, url: str, timeout: int) -> None:
         async with aiohttp.ClientSession() as session:
             async with session.post(url, json=self._request_data, timeout=timeout) as response:
                 self._status_code = response.status
                 self._response_data = await response.json()
 
     def _generate_request_error_msg(self) -> str:
-        if "error" not in self._response_data:
+        if self._response_data is None or "error" not in self._response_data:
             return "Could not connect to astrometry service."
 
         if self._response_data["error"] == "Could not find WCS file.":
             return "Could not determine WCS."
 
         return f"Received error from astrometry service: {self._response_data['error']}"
 
-    def _handle_request_error(self):
+    def _handle_request_error(self) -> None:
         error_msg = self._generate_request_error_msg()
         raise exc.ImageError(error_msg)
 
-    def _is_request_successful(self) -> bool:
-        return self._status_code != 200 or "error" in self._response_data
+    def _has_request_error(self) -> bool:
+        return (
+            self._status_code is None
+            or self._response_data is None
+            or self._status_code != 200
+            or "error" in self._response_data
+        )
 
-    async def send(self, url: str, timeout: int):
+    async def send(self, url: str, timeout: int) -> None:
         await self._send_request(url, timeout)
 
-        if self._is_request_successful():
+        if self._has_request_error():
             self._handle_request_error()
 
     @property
-    def request_data(self) -> Dict[str, any]:
+    def request_data(self) -> Dict[str, Any]:
         return self._request_data
 
     @property
-    def response_data(self) -> Optional[Dict[str, any]]:
+    def response_data(self) -> Optional[Dict[str, Any]]:
         return self._response_data
```

### Comparing `pyobs_core-1.8.0/pyobs/images/processors/astrometry/_dotnet_request_builder.py` & `pyobs_core-1.9.0/pyobs/images/processors/astrometry/_dotnet_request_builder.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,45 @@
-from typing import Optional
+from typing import Optional, Any, Dict
 
 import pandas as pd
 from astropy.io.fits import Header
 
 from pyobs.images import Image
 import pyobs.utils.exceptions as exc
 from pyobs.images.processors.astrometry._dotnet_request import _DotNetRequest
 
 
 class _DotNetRequestBuilder:
     def __init__(self, source_count: int, radius: float):
         self._source_count = source_count
         self._radius = radius
 
-        self._request_data = {}
+        self._request_data: Dict[str, Any] = {}
         self._catalog = pd.DataFrame()
         self._header: Optional[Header] = None
 
-    def _filter_catalog(self):
+    def _filter_catalog(self) -> None:
         self._catalog = self._catalog.dropna(how="any")
         self._catalog = self._catalog[self._catalog["peak"] < 60000]
 
-    def _validate_catalog(self):
+    def _validate_catalog(self) -> None:
         if self._catalog is None or len(self._catalog) < 3:
             raise exc.ImageError("Not enough sources for astrometry.")
 
-    def _select_brightest_stars(self):
+    def _select_brightest_stars(self) -> None:
         self._catalog = self._catalog.sort_values("flux", ascending=False)
         self._catalog = self._catalog[: self._source_count]
 
-    def _validate_header(self):
-        if "CDELT1" not in self._header:
+    def _validate_header(self) -> None:
+        if self._header is None or "CDELT1" not in self._header:
             raise exc.ImageError("No CDELT1 found in header.")
 
-    def _build_request_data(self):
+    def _build_request_data(self) -> None:
+        if self._header is None:
+            raise exc.ImageError("No header found.")
         scale = abs(self._header["CDELT1"]) * 3600
         self._request_data = {
             "ra": self._header["TEL-RA"],
             "dec": self._header["TEL-DEC"],
             "scale_low": scale * 0.9,
             "scale_high": scale * 1.1,
             "radius": self._radius,
@@ -48,16 +50,14 @@
             "x": self._catalog["x"].tolist(),
             "y": self._catalog["y"].tolist(),
             "flux": self._catalog["flux"].tolist(),
         }
 
     def __call__(self, image: Image) -> _DotNetRequest:
         # set catalog and header
-        if image.catalog is None:
-            raise exc.ImageError("No catalog found in image.")
         self._catalog = image.catalog[["x", "y", "flux", "peak"]].to_pandas()
         self._header = image.header
 
         # select stars
         self._filter_catalog()
         self._validate_catalog()
         self._select_brightest_stars()
```

### Comparing `pyobs_core-1.8.0/pyobs/images/processors/astrometry/_dotnet_request_logger.py` & `pyobs_core-1.9.0/pyobs/images/processors/astrometry/_dotnet_request_logger.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,35 +10,35 @@
 
 class _RequestLogger:
     def __init__(self, logger: logging.Logger, image: Image, request_data: Dict[str, Any]):
         self._logger = logger
         self._image = image
         self._request_data = request_data
 
-    def log_request_data(self):
+    def log_request_data(self) -> None:
         ra_dec = SkyCoord(ra=self._request_data["ra"] * u.deg, dec=self._request_data["dec"] * u.deg, frame="icrs")
         center_x, center_y = self._image.header["CRPIX1"], self._image.header["CRPIX2"]
 
         self._logger.info(
             "Found original RA=%s (%.4f), Dec=%s (%.4f) at pixel %.2f,%.2f.",
             ra_dec.ra.to_string(sep=":", unit=u.hour, pad=True),
             self._request_data["ra"],
             ra_dec.dec.to_string(sep=":", unit=u.deg, pad=True),
             self._request_data["dec"],
             center_x,
             center_y,
         )
 
-    def log_request_result(self, image_wcs: WCS):
+    def log_request_result(self, image_wcs: WCS) -> None:
         center_x, center_y = self._image.header["CRPIX1"], self._image.header["CRPIX2"]
         final_ra, final_dec = image_wcs.all_pix2world(center_x, center_y, 0)
         final_ra_dec = SkyCoord(ra=final_ra * u.deg, dec=final_dec * u.deg, frame="icrs")
 
         self._logger.info(
             "Found final RA=%s (%.4f), Dec=%s (%.4f) at pixel %.2f,%.2f.",
             final_ra_dec.ra.to_string(sep=":", unit=u.hour, pad=True),
             self._request_data["ra"],
             final_ra_dec.dec.to_string(sep=":", unit=u.deg, pad=True),
             self._request_data["dec"],
             center_x,
             center_y,
-        )
+        )
```

### Comparing `pyobs_core-1.8.0/pyobs/images/processors/astrometry/_dotnet_response_saver.py` & `pyobs_core-1.9.0/pyobs/images/processors/astrometry/_dotnet_response_saver.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,71 @@
 from copy import copy
 from typing import Dict, Any, Optional
 
 from astropy.wcs import WCS
 
 from pyobs.images import Image
+import pyobs.utils.exceptions as exc
 
 
 class _ResponseImageWriter:
     def __init__(self, response_data: Dict[str, Any], image: Image):
         self._response_data = response_data
         self._image = copy(image)
 
         self._image_wcs: Optional[WCS] = None
 
     @property
-    def response_data(self):
+    def response_data(self) -> Dict[str, Any]:
         return self._response_data
 
     @property
-    def image(self):
+    def image(self) -> Image:
         return self._image
 
     @property
-    def image_wcs(self):
+    def image_wcs(self) -> WCS:
         return self._image_wcs
 
-    def _write_response_into_header(self):
+    def _write_response_into_header(self) -> None:
         header_keywords_to_update = [
-            "CTYPE1", "CTYPE2",
-            "CRPIX1", "CRPIX2",
-            "CRVAL1", "CRVAL2",
-            "CD1_1", "CD1_2",
-            "CD2_1", "CD2_2",
+            "CTYPE1",
+            "CTYPE2",
+            "CRPIX1",
+            "CRPIX2",
+            "CRVAL1",
+            "CRVAL2",
+            "CD1_1",
+            "CD1_2",
+            "CD2_1",
+            "CD2_2",
         ]
 
         for keyword in header_keywords_to_update:
             self._image.header[keyword] = self._response_data[keyword]
 
-    def _delete_old_wcs_data(self):
+    def _delete_old_wcs_data(self) -> None:
         """
         astrometry.net gives a CD matrix, so we have to delete the PC matrix and the CDELT* parameters
         """
         for keyword in ["PC1_1", "PC1_2", "PC2_1", "PC2_2", "CDELT1", "CDELT2"]:
             del self._image.header[keyword]
 
-    def _generate_image_wcs(self):
+    def _generate_image_wcs(self) -> None:
         self._image_wcs = WCS(self._image.header)
 
-    def _add_plate_solution_to_catalog(self):
+    def _add_plate_solution_to_catalog(self) -> None:
+        if self._image_wcs is None:
+            raise exc.ImageError("No WCS found.")
         ras, decs = self._image_wcs.all_pix2world(self._image.catalog["x"], self._image.catalog["y"], 1)
 
         self._image.catalog["ra"] = ras
         self._image.catalog["dec"] = decs
 
-    def _add_wcs_err_success(self):
+    def _add_wcs_err_success(self) -> None:
         self._image.header["WCSERR"] = 0
 
     def __call__(self, *args, **kwargs) -> Image:
         self._write_response_into_header()
         self._delete_old_wcs_data()
         self._generate_image_wcs()
         self._add_plate_solution_to_catalog()
```

### Comparing `pyobs_core-1.8.0/pyobs/images/processors/astrometry/astrometry.py` & `pyobs_core-1.9.0/pyobs/images/processors/astrometry/astrometry.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/images/processors/astrometry/dotnet.py` & `pyobs_core-1.9.0/pyobs/images/processors/astrometry/dotnet.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/images/processors/detection/_pysep_stats_calculator.py` & `pyobs_core-1.9.0/pyobs/images/processors/detection/_pysep_stats_calculator.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/images/processors/detection/_source_catalog.py` & `pyobs_core-1.9.0/pyobs/images/processors/detection/_source_catalog.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/images/processors/detection/daophot.py` & `pyobs_core-1.9.0/pyobs/images/processors/detection/daophot.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         Args:
             image: Image to find stars in.
 
         Returns:
             Image with attached catalog.
         """
 
-        if image.data is None:
+        if image.safe_data is None:
             log.warning("No data found in image.")
             return image
 
         background_corrected_image = self._background_remover(image)
         background_corrected_data = background_corrected_image.data.astype(float)
 
         _, median, std = sigma_clipped_stats(background_corrected_data, sigma=3.0)
```

### Comparing `pyobs_core-1.8.0/pyobs/images/processors/detection/pysep.py` & `pyobs_core-1.9.0/pyobs/images/processors/detection/pysep.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,24 +19,30 @@
 
 class SepSourceDetection(SourceDetection):
     """Detect sources using SEP."""
 
     __module__ = "pyobs.images.processors.detection"
 
     _CATALOG_KEYS = [
-        "x", "y",
+        "x",
+        "y",
         "peak",
         "flux",
         "fwhm",
-        "a", "b", "theta",
+        "a",
+        "b",
+        "theta",
         "ellipticity",
         "tnpix",
         "kronrad",
-        "fluxrad25", "fluxrad50", "fluxrad75",
-        "xwin", "ywin",
+        "fluxrad25",
+        "fluxrad50",
+        "fluxrad75",
+        "xwin",
+        "ywin",
     ]
 
     def __init__(
         self,
         threshold: float = 1.5,
         minarea: int = 5,
         deblend_nthresh: int = 32,
@@ -73,15 +79,15 @@
         Args:
             image: Image to find stars in.
 
         Returns:
             Image with attached catalog.
         """
 
-        if image.data is None:
+        if image.safe_data is None:
             log.warning("No data found in image.")
             return image
 
         mask = self._get_mask_or_default(image)
 
         data, background = self.remove_background(image.data, mask)
 
@@ -100,15 +106,15 @@
         source_catalog.apply_fits_origin_convention()
 
         output_image = source_catalog.save_to_image(image, self._CATALOG_KEYS)
         return output_image
 
     @staticmethod
     def _get_mask_or_default(image: Image) -> np.ndarray:
-        if image.mask is not None:
+        if image.safe_mask is not None:
             return image.mask
 
         return np.zeros(image.data.shape, dtype=bool)
 
     @staticmethod
     def _get_gain_or_default(image: Image) -> Optional[float]:
         if "DET-GAIN" in image.header:
```

### Comparing `pyobs_core-1.8.0/pyobs/images/processors/detection/sourcedetection.py` & `pyobs_core-1.9.0/pyobs/images/processors/detection/sourcedetection.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/images/processors/exptime/exptime.py` & `pyobs_core-1.9.0/pyobs/images/processors/exptime/exptime.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/images/processors/exptime/star.py` & `pyobs_core-1.9.0/pyobs/images/processors/exptime/star.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         Args:
             image: Image to process.
         """
 
         self._image = copy(image)
         last_exp_time = image.header["EXPTIME"]
 
-        if self._image.catalog is None:
+        if self._image.safe_catalog is None:
             log.info("No catalog found in image.")
             return last_exp_time
 
         saturation = self._calc_saturation_level_or_default()
         self._filter_saturated_stars(saturation)
         self._filter_edge_stars()
         brightest_star = self._find_brightest_star()
```

### Comparing `pyobs_core-1.8.0/pyobs/images/processors/misc/addmask.py` & `pyobs_core-1.9.0/pyobs/images/processors/misc/addmask.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/images/processors/misc/broadcast.py` & `pyobs_core-1.9.0/pyobs/images/processors/misc/broadcast.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/images/processors/misc/calibration/_calibration_cache.py` & `pyobs_core-1.9.0/pyobs/images/processors/misc/calibration/_calibration_cache.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/images/processors/misc/calibration/_ccddata_calibrator.py` & `pyobs_core-1.9.0/pyobs/images/processors/misc/calibration/_ccddata_calibrator.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/images/processors/misc/calibration/calibration.py` & `pyobs_core-1.9.0/pyobs/images/processors/misc/calibration/calibration.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/images/processors/misc/createfilename.py` & `pyobs_core-1.9.0/pyobs/images/processors/misc/createfilename.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/images/processors/misc/removebackground.py` & `pyobs_core-1.9.0/pyobs/images/processors/misc/removebackground.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/images/processors/misc/smooth.py` & `pyobs_core-1.9.0/pyobs/images/processors/misc/smooth.py`

 * *Files 12% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             image: Image to smooth.
 
         Returns:
             Smoothed image.
         """
 
         output_image = image.copy()
-        if output_image.data is None:
+        if output_image.safe_data is None:
             log.warning("No data found in image.")
             return image
 
         output_image.data = scipy.ndimage.gaussian_filter(
             output_image.data, self.sigma, order=self.order, mode=self.mode, cval=self.cval, truncate=self.truncate
         )
```

### Comparing `pyobs_core-1.8.0/pyobs/images/processors/misc/softbin.py` & `pyobs_core-1.9.0/pyobs/images/processors/misc/softbin.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,20 +33,20 @@
             image: Image to bin.
 
         Returns:
             Binned image.
         """
 
         output_image = image.copy()
-        if output_image.data is None:
+        if output_image.safe_data is None:
             log.warning("No data found in image.")
             return image
 
         output_image.data = self._reshape_image(output_image.data)
-        if output_image.data is None:
+        if output_image.safe_data is None:
             log.warning("No data found in image after reshaping.")
             return image
 
         self._update_header(output_image)
 
         return output_image
```

### Comparing `pyobs_core-1.8.0/pyobs/images/processors/offsets/astrometry.py` & `pyobs_core-1.9.0/pyobs/images/processors/offsets/astrometry.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/images/processors/offsets/brighteststar.py` & `pyobs_core-1.9.0/pyobs/images/processors/offsets/brighteststar.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             Original image.
 
         Raises:
             ValueError: If offset could not be found.
         """
 
         # get catalog and sort by flux
-        cat = image.catalog
+        cat = image.safe_catalog
         if cat is None or len(cat) < 1:
             log.warning("No catalog found in image.")
             return image
         cat.sort("flux", reverse=True)
 
         # get first X/Y coordinates
         x, y = cat["x"][0], cat["y"][0]
```

### Comparing `pyobs_core-1.8.0/pyobs/images/processors/offsets/dummyoffsets.py` & `pyobs_core-1.9.0/pyobs/images/processors/offsets/dummyoffsets.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/images/processors/offsets/fitsheader.py` & `pyobs_core-1.9.0/pyobs/images/processors/offsets/fitsheader.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/images/processors/offsets/nstar.py` & `pyobs_core-1.9.0/pyobs/images/processors/offsets/nstar.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,20 +124,14 @@
         Raises:
             ValueError if not at least max(self.min_required_sources_in_image, self.N_stars) in filtered list of sources
         """
 
         # run pipeline on 1st image
         img = await self.run_pipeline(image)
 
-        # check data and catalog
-        if img.data is None:
-            raise ValueError("No data found in image.")
-        if img.catalog is None:
-            raise ValueError("No catalog found in image.")
-
         # do photometry and get catalog
         sources = self._fits2numpy(img.catalog)
 
         # filter sources
         sources = self.remove_sources_close_to_border(sources, img.data.shape, star_box_size // 2 + 1)
         sources = self.remove_bad_sources(sources)
         self._check_sources_count(sources)
@@ -269,15 +263,15 @@
             image: Image to calculate offset for.
 
         Returns:
             Offset tuple.
         """
 
         # data?
-        if image.data is None:
+        if image.safe_data is None:
             return None, None
 
         # calculate offset for each star
         offsets = []
         for box in self.ref_boxes:
             # get box dimensions
             box_ymin, box_ymax = box.origin[1], box.origin[1] + box.data.shape[0]
```

### Comparing `pyobs_core-1.8.0/pyobs/images/processors/offsets/offsets.py` & `pyobs_core-1.9.0/pyobs/images/processors/offsets/offsets.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/images/processors/offsets/projected.py` & `pyobs_core-1.9.0/pyobs/images/processors/offsets/projected.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,18 +78,14 @@
         Returns:
             Projected images.
         """
 
         # get image data and header
         data, hdr = image.data, image.header
 
-        # no data?
-        if data is None:
-            raise ValueError("Image contains no data.")
-
         # trimsec
         if "TRIMSEC" in hdr:
             m = re.match(r"\[([0-9]+):([0-9]+),([0-9]+):([0-9]+)\]", hdr["TRIMSEC"])
             if m is None:
                 raise ValueError("Invalid trimsec.")
             x0, x1, y0, y1 = [int(f) for f in m.groups()]
             data = data[y0 - 1 : y1, x0 - 1 : x1]
```

### Comparing `pyobs_core-1.8.0/pyobs/images/processors/photometry/photometry.py` & `pyobs_core-1.9.0/pyobs/images/processors/photometry/photometry.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/images/processors/photometry/photutil.py` & `pyobs_core-1.9.0/pyobs/images/processors/photometry/photutil.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
         # no pixel scale given?
         if image.pixel_scale is None:
             log.warning("No pixel scale provided by image.")
             return image
 
         # fetch catalog
-        if image.catalog is None:
+        if image.safe_catalog is None:
             log.warning("No catalog in image.")
             return image
         sources = image.catalog.copy()
 
         # get positions
         positions = [(x - 1, y - 1) for x, y in sources.iterrows("x", "y")]
 
@@ -92,15 +92,16 @@
                 annulus_data = m.multiply(image.data)
                 annulus_data_1d = annulus_data[m.data > 0]
                 _, median_sigclip, _ = sigma_clipped_stats(annulus_data_1d)
                 bkg_median.append(median_sigclip)
 
             # do photometry
             phot = await loop.run_in_executor(
-                None, partial(aperture_photometry, image.data, aperture, mask=image.mask, error=image.uncertainty)
+                None,
+                partial(aperture_photometry, image.data, aperture, mask=image.safe_mask, error=image.safe_uncertainty),
             )
 
             # calc flux
             bkg_median_np = np.array(bkg_median)
             aper_bkg = bkg_median_np * aperture.area
             sources["fluxaper%d" % diameter] = phot["aperture_sum"] - aper_bkg
             if "aperture_sum_err" in phot.columns:
```

### Comparing `pyobs_core-1.8.0/pyobs/images/processors/photometry/pysep.py` & `pyobs_core-1.9.0/pyobs/images/processors/photometry/pysep.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,41 +63,44 @@
 
     @staticmethod
     def _photometry(image: Image) -> Image:
         import sep
         from pyobs.images.processors.detection import SepSourceDetection
 
         # check data
-        if image.data is None:
+        if image.safe_data is None:
             log.warning("No data found in image.")
             return image
-        if image.catalog is None:
+        if image.safe_catalog is None:
             log.warning("No catalog found in image.")
             return image
 
-        # no mask?
-        mask = image.mask if image.mask is not None else np.ones(image.data.shape, dtype=bool)
-
         # remove background
-        data, bkg = SepSourceDetection.remove_background(image.data, mask)
+        data, bkg = SepSourceDetection.remove_background(image.data, image.safe_mask)
 
         # fetch catalog
         sources = image.catalog.copy()
 
         # match SEP conventions
         x, y = sources["x"] - 1, sources["y"] - 1
 
         # get gain
         gain = image.header["DET-GAIN"] if "DET-GAIN" in image.header else None
 
         # perform aperture photometry for diameters of 1" to 8"
         for diameter in [1, 2, 3, 4, 5, 6, 7, 8]:
             if image.pixel_scale is not None:
                 flux, fluxerr, flag = sep.sum_circle(
-                    data, x, y, diameter / 2.0 / image.pixel_scale, mask=image.mask, err=image.uncertainty, gain=gain
+                    data,
+                    x,
+                    y,
+                    diameter / 2.0 / image.pixel_scale,
+                    mask=image.safe_mask,
+                    err=image.safe_uncertainty,
+                    gain=gain,
                 )
                 sources["fluxaper{0}".format(diameter)] = flux
                 sources["fluxerr{0}".format(diameter)] = fluxerr
 
             else:
                 sources["fluxaper{0}".format(diameter)] = 0
                 sources["fluxerr{0}".format(diameter)] = 0
```

### Comparing `pyobs_core-1.8.0/pyobs/interfaces/IAcquisition.py` & `pyobs_core-1.9.0/pyobs/interfaces/IAcquisition.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/interfaces/IAutoFocus.py` & `pyobs_core-1.9.0/pyobs/interfaces/IAutoFocus.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/interfaces/IBinning.py` & `pyobs_core-1.9.0/pyobs/interfaces/IBinning.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/interfaces/IConfig.py` & `pyobs_core-1.9.0/pyobs/interfaces/IConfig.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/interfaces/ICooling.py` & `pyobs_core-1.9.0/pyobs/interfaces/ICooling.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/interfaces/IData.py` & `pyobs_core-1.9.0/pyobs/interfaces/IData.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/interfaces/IExposure.py` & `pyobs_core-1.9.0/pyobs/interfaces/IExposure.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/interfaces/IExposureTime.py` & `pyobs_core-1.9.0/pyobs/interfaces/IExposureTime.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/interfaces/IFilters.py` & `pyobs_core-1.9.0/pyobs/interfaces/IFilters.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/interfaces/IFitsHeaderAfter.py` & `pyobs_core-1.9.0/pyobs/interfaces/IFitsHeaderAfter.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/interfaces/IFitsHeaderBefore.py` & `pyobs_core-1.9.0/pyobs/interfaces/IFitsHeaderBefore.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/interfaces/IFlatField.py` & `pyobs_core-1.9.0/pyobs/interfaces/IFlatField.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/interfaces/IFocusModel.py` & `pyobs_core-1.9.0/pyobs/interfaces/IFocusModel.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/interfaces/IFocuser.py` & `pyobs_core-1.9.0/pyobs/interfaces/IFocuser.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/interfaces/IGain.py` & `pyobs_core-1.9.0/pyobs/interfaces/IGain.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/interfaces/IImageFormat.py` & `pyobs_core-1.9.0/pyobs/interfaces/IImageFormat.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/interfaces/IImageType.py` & `pyobs_core-1.9.0/pyobs/interfaces/IImageType.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/interfaces/ILatLon.py` & `pyobs_core-1.9.0/pyobs/interfaces/ILatLon.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/interfaces/IMode.py` & `pyobs_core-1.9.0/pyobs/interfaces/IMode.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/interfaces/IModule.py` & `pyobs_core-1.9.0/pyobs/interfaces/IModule.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/interfaces/IMotion.py` & `pyobs_core-1.9.0/pyobs/interfaces/IMotion.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/interfaces/IOffsetsAltAz.py` & `pyobs_core-1.9.0/pyobs/interfaces/IOffsetsAltAz.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/interfaces/IOffsetsRaDec.py` & `pyobs_core-1.9.0/pyobs/interfaces/IOffsetsRaDec.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/interfaces/IPointingAltAz.py` & `pyobs_core-1.9.0/pyobs/interfaces/IPointingAltAz.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/interfaces/IPointingHGS.py` & `pyobs_core-1.9.0/pyobs/interfaces/IPointingHGS.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/interfaces/IPointingHelioprojective.py` & `pyobs_core-1.9.0/pyobs/interfaces/IPointingHelioprojective.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/interfaces/IPointingRaDec.py` & `pyobs_core-1.9.0/pyobs/interfaces/IPointingRaDec.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/interfaces/IPointingSeries.py` & `pyobs_core-1.9.0/pyobs/interfaces/IPointingSeries.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/interfaces/IReady.py` & `pyobs_core-1.9.0/pyobs/interfaces/IReady.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/interfaces/IRotation.py` & `pyobs_core-1.9.0/pyobs/interfaces/IRotation.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/interfaces/ITemperatures.py` & `pyobs_core-1.9.0/pyobs/interfaces/ITemperatures.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/interfaces/IWeather.py` & `pyobs_core-1.9.0/pyobs/interfaces/IWeather.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/interfaces/IWindow.py` & `pyobs_core-1.9.0/pyobs/interfaces/IWindow.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/interfaces/__init__.py` & `pyobs_core-1.9.0/pyobs/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/mixins/camerasettings.py` & `pyobs_core-1.9.0/pyobs/mixins/camerasettings.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/mixins/fitsheader.py` & `pyobs_core-1.9.0/pyobs/mixins/fitsheader.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/mixins/fitsnamespace.py` & `pyobs_core-1.9.0/pyobs/mixins/fitsnamespace.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/mixins/follow.py` & `pyobs_core-1.9.0/pyobs/mixins/follow.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/mixins/motionstatus.py` & `pyobs_core-1.9.0/pyobs/mixins/motionstatus.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/mixins/pipeline.py` & `pyobs_core-1.9.0/pyobs/mixins/pipeline.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/mixins/waitformotion.py` & `pyobs_core-1.9.0/pyobs/mixins/waitformotion.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/mixins/weatheraware.py` & `pyobs_core-1.9.0/pyobs/mixins/weatheraware.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/modules/__init__.py` & `pyobs_core-1.9.0/pyobs/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/modules/camera/adaptive.py` & `pyobs_core-1.9.0/pyobs/modules/camera/adaptive.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/modules/camera/basecamera.py` & `pyobs_core-1.9.0/pyobs/modules/camera/basecamera.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,15 +242,15 @@
         # reset abort event
         self.expose_abort.clear()
 
         # do the exposure
         self._exposure = ExposureInfo(start=datetime.datetime.utcnow(), exposure_time=exposure_time)
         try:
             image = await self._expose(exposure_time, open_shutter, abort_event=self.expose_abort)
-            if image is None or image.data is None:
+            if image is None or image.safe_data is None:
                 raise exc.GrabImageError("Could not take image.")
 
         except exc.PyObsError:
             # exposure was not successful (aborted?), so reset everything and re-raise
             self._exposure = None
             raise
```

### Comparing `pyobs_core-1.8.0/pyobs/modules/camera/basespectrograph.py` & `pyobs_core-1.9.0/pyobs/modules/camera/basespectrograph.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/modules/camera/basevideo.py` & `pyobs_core-1.9.0/pyobs/modules/camera/basevideo.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/modules/camera/dummycamera.py` & `pyobs_core-1.9.0/pyobs/modules/camera/dummycamera.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/modules/camera/dummyspectrograph.py` & `pyobs_core-1.9.0/pyobs/modules/camera/dummyspectrograph.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/modules/flatfield/flatfield.py` & `pyobs_core-1.9.0/pyobs/modules/flatfield/flatfield.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/modules/flatfield/pointing.py` & `pyobs_core-1.9.0/pyobs/modules/flatfield/pointing.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/modules/flatfield/scheduler.py` & `pyobs_core-1.9.0/pyobs/modules/flatfield/scheduler.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/modules/focus/focusmodel.py` & `pyobs_core-1.9.0/pyobs/modules/focus/focusmodel.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/modules/focus/focusseries.py` & `pyobs_core-1.9.0/pyobs/modules/focus/focusseries.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/modules/image/imagewatcher.py` & `pyobs_core-1.9.0/pyobs/modules/image/imagewatcher.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/modules/image/imagewriter.py` & `pyobs_core-1.9.0/pyobs/modules/image/imagewriter.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/modules/image/seeing.py` & `pyobs_core-1.9.0/pyobs/modules/image/seeing.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             image = await self.vfs.read_image(event.filename)
 
         except FileNotFoundError:
             log.error("Could not download image.")
             return False
 
         # get catalog
-        cat = image.catalog
+        cat = image.safe_catalog
         if cat is None:
             # no catalog found in file
             return False
 
         # filter by ellipticity
         cat = cat[cat["ellipticity"] < self._max_ellipticity]
```

### Comparing `pyobs_core-1.8.0/pyobs/modules/module.py` & `pyobs_core-1.9.0/pyobs/modules/module.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/modules/pointing/_base.py` & `pyobs_core-1.9.0/pyobs/modules/pointing/_base.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/modules/pointing/_baseguiding.py` & `pyobs_core-1.9.0/pyobs/modules/pointing/_baseguiding.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/modules/pointing/acquisition.py` & `pyobs_core-1.9.0/pyobs/modules/pointing/acquisition.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/modules/pointing/autoguiding.py` & `pyobs_core-1.9.0/pyobs/modules/pointing/autoguiding.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/modules/pointing/dummyacquisition.py` & `pyobs_core-1.9.0/pyobs/modules/pointing/dummyacquisition.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/modules/pointing/dummyguiding.py` & `pyobs_core-1.9.0/pyobs/modules/pointing/dummyguiding.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/modules/pointing/scienceframeguiding.py` & `pyobs_core-1.9.0/pyobs/modules/pointing/scienceframeguiding.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/modules/robotic/mastermind.py` & `pyobs_core-1.9.0/pyobs/modules/robotic/mastermind.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/modules/robotic/pointing.py` & `pyobs_core-1.9.0/pyobs/modules/robotic/pointing.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/modules/robotic/scheduler.py` & `pyobs_core-1.9.0/pyobs/modules/robotic/scheduler.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/modules/robotic/scriptrunner.py` & `pyobs_core-1.9.0/pyobs/modules/robotic/scriptrunner.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/modules/roof/basedome.py` & `pyobs_core-1.9.0/pyobs/modules/roof/basedome.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/modules/roof/baseroof.py` & `pyobs_core-1.9.0/pyobs/modules/roof/baseroof.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/modules/roof/dummyroof.py` & `pyobs_core-1.9.0/pyobs/modules/roof/dummyroof.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/modules/telescope/basetelescope.py` & `pyobs_core-1.9.0/pyobs/modules/telescope/basetelescope.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/modules/telescope/dummytelescope.py` & `pyobs_core-1.9.0/pyobs/modules/telescope/dummytelescope.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/modules/test/standalone.py` & `pyobs_core-1.9.0/pyobs/modules/test/standalone.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/modules/utils/autonomouswarning.py` & `pyobs_core-1.9.0/pyobs/modules/utils/autonomouswarning.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/modules/utils/fluentlogger.py` & `pyobs_core-1.9.0/pyobs/modules/utils/fluentlogger.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/modules/utils/httpfilecache.py` & `pyobs_core-1.9.0/pyobs/modules/utils/httpfilecache.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/modules/utils/kiosk.py` & `pyobs_core-1.9.0/pyobs/modules/utils/kiosk.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/modules/utils/stellarium.py` & `pyobs_core-1.9.0/pyobs/modules/utils/stellarium.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/modules/utils/telegram.py` & `pyobs_core-1.9.0/pyobs/modules/utils/telegram.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/modules/utils/trigger.py` & `pyobs_core-1.9.0/pyobs/modules/utils/trigger.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/modules/weather/weather.py` & `pyobs_core-1.9.0/pyobs/modules/weather/weather.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/object.py` & `pyobs_core-1.9.0/pyobs/object.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/robotic/lco/dummytaskschedule.py` & `pyobs_core-1.9.0/pyobs/robotic/lco/dummytaskschedule.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/robotic/lco/portal.py` & `pyobs_core-1.9.0/pyobs/robotic/lco/portal.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/robotic/lco/scripts/autofocus.py` & `pyobs_core-1.9.0/pyobs/robotic/lco/scripts/autofocus.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/robotic/lco/scripts/default.py` & `pyobs_core-1.9.0/pyobs/robotic/lco/scripts/default.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/robotic/lco/scripts/script.py` & `pyobs_core-1.9.0/pyobs/robotic/lco/scripts/script.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/robotic/lco/task.py` & `pyobs_core-1.9.0/pyobs/robotic/lco/task.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/robotic/lco/taskarchive.py` & `pyobs_core-1.9.0/pyobs/robotic/lco/taskarchive.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/robotic/lco/taskschedule.py` & `pyobs_core-1.9.0/pyobs/robotic/lco/taskschedule.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/robotic/scripts/conditional.py` & `pyobs_core-1.9.0/pyobs/robotic/scripts/conditional.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/robotic/scripts/darkbias.py` & `pyobs_core-1.9.0/pyobs/robotic/scripts/darkbias.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/robotic/scripts/flatfield/pointing.py` & `pyobs_core-1.9.0/pyobs/robotic/scripts/flatfield/pointing.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/robotic/scripts/parallel.py` & `pyobs_core-1.9.0/pyobs/robotic/scripts/sequential.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 from __future__ import annotations
-import asyncio
 import logging
 from typing import Any, Dict, Optional, List, TYPE_CHECKING
 
 if TYPE_CHECKING:
     from pyobs.robotic import TaskRunner, TaskSchedule, TaskArchive
 from pyobs.robotic.scripts import Script
 
-
 log = logging.getLogger(__name__)
 
 
-class ParallelRunner(Script):
-    """Script for running other scripts in parallel."""
+class SequentialRunner(Script):
+    """Script for running a sequence of other scripts."""
 
     __module__ = "pyobs.modules.robotic"
 
     def __init__(
         self,
         scripts: List[Dict[str, Any]],
+        check_all_can_run: bool = True,
         **kwargs: Any,
     ):
-        """Initialize a new ParallelRunner.
+        """Initialize a new SequentialRunner.
 
         Args:
-            scripts: list or dict of scripts to run in parallel.
+            script: list or dict of scripts to run in a sequence.
         """
         Script.__init__(self, **kwargs)
         self.scripts = scripts
+        self.check_all_can_run = check_all_can_run
 
     async def can_run(self) -> bool:
-        return True
+        check_all = [self.get_object(s, Script).can_run() for s in self.scripts]
+        return all(check_all) if self.check_all_can_run else check_all[0]
 
     async def run(
         self,
         task_runner: TaskRunner,
         task_schedule: Optional[TaskSchedule] = None,
         task_archive: Optional[TaskArchive] = None,
     ) -> None:
-        tasks = [
-            asyncio.create_task(self.get_object(s, Script).run(task_runner, task_schedule, task_archive))
-            for s in self.scripts
-        ]
-        await asyncio.gather(*tasks)
+        for s in self.scripts:
+            script = self.get_object(s, Script)
+            if script.can_run():
+                await script.run(task_runner, task_schedule, task_archive)
 
 
-__all__ = ["ParallelRunner"]
+__all__ = ["SequentialRunner"]
```

### Comparing `pyobs_core-1.8.0/pyobs/robotic/scripts/script.py` & `pyobs_core-1.9.0/pyobs/robotic/scripts/script.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/robotic/scripts/selector.py` & `pyobs_core-1.9.0/pyobs/robotic/scripts/selector.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/robotic/scripts/skyflats.py` & `pyobs_core-1.9.0/pyobs/robotic/scripts/skyflats.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/robotic/task.py` & `pyobs_core-1.9.0/pyobs/robotic/task.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/robotic/taskarchive.py` & `pyobs_core-1.9.0/pyobs/robotic/taskarchive.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/robotic/taskrunner.py` & `pyobs_core-1.9.0/pyobs/robotic/taskrunner.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/robotic/taskschedule.py` & `pyobs_core-1.9.0/pyobs/robotic/taskschedule.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/archive/archive.py` & `pyobs_core-1.9.0/pyobs/utils/archive/archive.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/archive/local_archive.py` & `pyobs_core-1.9.0/pyobs/utils/archive/local_archive.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/archive/pyobs_archive.py` & `pyobs_core-1.9.0/pyobs/utils/archive/pyobs_archive.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/average.py` & `pyobs_core-1.9.0/pyobs/utils/average.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/cache.py` & `pyobs_core-1.9.0/pyobs/utils/cache.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/config.py` & `pyobs_core-1.9.0/pyobs/utils/config.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/coordinates.py` & `pyobs_core-1.9.0/pyobs/utils/coordinates.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/curvefit.py` & `pyobs_core-1.9.0/pyobs/utils/curvefit.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/enums.py` & `pyobs_core-1.9.0/pyobs/utils/enums.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/exceptions.py` & `pyobs_core-1.9.0/pyobs/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/fits.py` & `pyobs_core-1.9.0/pyobs/utils/fits.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/focusseries/base.py` & `pyobs_core-1.9.0/pyobs/utils/focusseries/base.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/focusseries/photometry.py` & `pyobs_core-1.9.0/pyobs/utils/focusseries/photometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             focus_value: Value to fit along, e.g. focus value or its offset
         """
 
         # do photometry
         self._source_detection(image)
 
         # filter
-        sources = image.catalog
+        sources = image.safe_catalog
         if sources is None:
             return
         sources = sources[sources["ellipticity"] < 0.1]
         sources = sources[sources["peak"] > 1000]
         sources = sources[sources["radius"] > 0]
 
         # calculate median radius
```

### Comparing `pyobs_core-1.8.0/pyobs/utils/focusseries/projection.py` & `pyobs_core-1.9.0/pyobs/utils/focusseries/projection.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
         Args:
             image: Image to analyse
             focus_value: Value to fit along, e.g. focus value or its offset
         """
 
         # clean data
-        if image.data is None:
+        if image.safe_data is None:
             return
         data = self._clean(image.data)
 
         # get projections
         xproj = np.mean(data, axis=0)
         yproj = np.mean(data, axis=1)
         nx = len(xproj)
```

### Comparing `pyobs_core-1.8.0/pyobs/utils/grids.py` & `pyobs_core-1.9.0/pyobs/utils/grids.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/http.py` & `pyobs_core-1.9.0/pyobs/utils/http.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/logger.py` & `pyobs_core-1.9.0/pyobs/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/modulegui.py` & `pyobs_core-1.9.0/pyobs/utils/modulegui.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/offsets/applyaltazoffsets.py` & `pyobs_core-1.9.0/pyobs/utils/offsets/applyaltazoffsets.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/offsets/applyoffsets.py` & `pyobs_core-1.9.0/pyobs/utils/offsets/applyoffsets.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/offsets/applyradecoffsets.py` & `pyobs_core-1.9.0/pyobs/utils/offsets/applyradecoffsets.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/parallel.py` & `pyobs_core-1.9.0/pyobs/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/pid.py` & `pyobs_core-1.9.0/pyobs/utils/pid.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/pipeline/night.py` & `pyobs_core-1.9.0/pyobs/utils/pipeline/night.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/pipeline/pipeline.py` & `pyobs_core-1.9.0/pyobs/utils/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/publisher/csv.py` & `pyobs_core-1.9.0/pyobs/utils/publisher/csv.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/publisher/http.py` & `pyobs_core-1.9.0/pyobs/utils/publisher/http.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/publisher/log.py` & `pyobs_core-1.9.0/pyobs/utils/publisher/log.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/publisher/multi.py` & `pyobs_core-1.9.0/pyobs/utils/publisher/multi.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/simulation/camera.py` & `pyobs_core-1.9.0/pyobs/utils/simulation/camera.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/simulation/telescope.py` & `pyobs_core-1.9.0/pyobs/utils/simulation/telescope.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/simulation/world.py` & `pyobs_core-1.9.0/pyobs/utils/simulation/world.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/skyflats/exptimeeval.py` & `pyobs_core-1.9.0/pyobs/utils/skyflats/exptimeeval.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/skyflats/flatfielder.py` & `pyobs_core-1.9.0/pyobs/utils/skyflats/flatfielder.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/skyflats/pointing/base.py` & `pyobs_core-1.9.0/pyobs/utils/skyflats/pointing/base.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/skyflats/pointing/static.py` & `pyobs_core-1.9.0/pyobs/utils/skyflats/pointing/static.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/skyflats/priorities/archive.py` & `pyobs_core-1.9.0/pyobs/utils/skyflats/priorities/archive.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/skyflats/priorities/const.py` & `pyobs_core-1.9.0/pyobs/utils/skyflats/priorities/const.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/skyflats/scheduler.py` & `pyobs_core-1.9.0/pyobs/utils/skyflats/scheduler.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/threads/checkabort.py` & `pyobs_core-1.9.0/pyobs/utils/threads/checkabort.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/threads/lockwithabort.py` & `pyobs_core-1.9.0/pyobs/utils/threads/lockwithabort.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/threads/threadwithreturnvalue.py` & `pyobs_core-1.9.0/pyobs/utils/threads/threadwithreturnvalue.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/time.py` & `pyobs_core-1.9.0/pyobs/utils/time.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/utils/types.py` & `pyobs_core-1.9.0/pyobs/utils/types.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/vfs/__init__.py` & `pyobs_core-1.9.0/pyobs/vfs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/vfs/archivefile.py` & `pyobs_core-1.9.0/pyobs/vfs/archivefile.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/vfs/file.py` & `pyobs_core-1.9.0/pyobs/vfs/file.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/vfs/httpfile.py` & `pyobs_core-1.9.0/pyobs/vfs/httpfile.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/vfs/localfile.py` & `pyobs_core-1.9.0/pyobs/vfs/localfile.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/vfs/memfile.py` & `pyobs_core-1.9.0/pyobs/vfs/memfile.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/vfs/sftpfile.py` & `pyobs_core-1.9.0/pyobs/vfs/sftpfile.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/vfs/smbfile.py` & `pyobs_core-1.9.0/pyobs/vfs/smbfile.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/vfs/sshfile.py` & `pyobs_core-1.9.0/pyobs/vfs/sshfile.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/vfs/tempfile.py` & `pyobs_core-1.9.0/pyobs/vfs/tempfile.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyobs/vfs/vfs.py` & `pyobs_core-1.9.0/pyobs/vfs/vfs.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.8.0/pyproject.toml` & `pyobs_core-1.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "pyobs-core"
 packages = [{ include = "pyobs" }]
-version = "1.8.0"
+version = "1.9.0"
 description = "robotic telescope software"
 authors = ["Tim-Oliver Husser <thusser@uni-goettingen.de>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 scipy = "^1.11.3"
```

### Comparing `pyobs_core-1.8.0/PKG-INFO` & `pyobs_core-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobs-core
-Version: 1.8.0
+Version: 1.9.0
 Summary: robotic telescope software
 License: MIT
 Author: Tim-Oliver Husser
 Author-email: thusser@uni-goettingen.de
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

