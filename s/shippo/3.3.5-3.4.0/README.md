# Comparing `tmp/shippo-3.3.5.tar.gz` & `tmp/shippo-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shippo-3.3.5.tar", last modified: Wed May  8 01:22:00 2024, max compression
+gzip compressed data, was "shippo-3.4.0.tar", last modified: Fri May 10 18:30:52 2024, max compression
```

## Comparing `shippo-3.3.5.tar` & `shippo-3.4.0.tar`

### file list

```diff
@@ -1,257 +1,258 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:22:00.455736 shippo-3.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)    17808 2024-05-08 01:22:00.455736 shippo-3.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-05-08 01:21:51.000000 shippo-3.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 01:22:00.455736 shippo-3.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-08 01:21:51.000000 shippo-3.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:22:00.415736 shippo-3.3.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:22:00.419736 shippo-3.3.5/src/shippo/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:22:00.423736 shippo-3.3.5/src/shippo/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/_hooks/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    14213 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/addresses.py
--rw-r--r--   0 runner    (1001) docker     (127)    19824 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/batches.py
--rw-r--r--   0 runner    (1001) docker     (127)    28485 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/carrier_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8402 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/carrier_parcel_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    11175 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/customs_declarations.py
--rw-r--r--   0 runner    (1001) docker     (127)    10952 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/customs_items.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)    11114 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/manifests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:22:00.423736 shippo-3.3.5/src/shippo/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:22:00.443736 shippo-3.3.5/src/shippo/models/components/
--rw-r--r--   0 runner    (1001) docker     (127)    10928 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/addresscompletecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/addresscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/addressimporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/addresspaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/addressvalidationresults.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/addressvalidationresultsmessage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/alcohol.py
--rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/batchcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/batchshipment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/batchshipmentbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/batchshipmentpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/billing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountchronopostcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountcolissimocreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountcorreoscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountdpddecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountdpdukcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountfedexcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccounthermesukcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountmondialrelaycreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountregistrationstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountservicelevel.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountupscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountupscreaterequestparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountuspscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountwithextrainfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrierparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carriersenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/cod.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/connectexistingownaccountrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/customerreference.py
--rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/customsdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/customsdeclarationb13afilingoptionenum.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/customsdeclarationcontentstypeenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/customsdeclarationcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/customsdeclarationeelpfcenum.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/customsdeclarationincotermenum.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/customsdeclarationnondeliveryoptionenum.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/customsdeclarationpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/customsexporteridentification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/customsinvoicedcharges.py
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/customsitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/customsitemcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/customsitempaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/customstaxidentification.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/dangerousgoodslithiumbatteries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/dangerousgoodsobject.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/defaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/defaultparceltemplateupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/departmentnumber.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/distanceunitenum.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/dryice.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/errormessage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/fedexconnectexistingownaccountparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/instanttransactioncreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/instanttransactioncreateresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/instanttransactionrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/insurance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/invoicenumber.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/labelfiletypeenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/lineitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/lineitembase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/liverate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/liveratecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/liveratepaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/manifestcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/manifestpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/objectstateenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/ordercreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/orderpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/orderstatusenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/parcelcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/parcelextra.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/parcelinsurance.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/parcelpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/parcelrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)    10259 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/parceltemplateenumset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5867 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/pickup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/pickupbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/ponumber.py
--rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/rate.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/ratemessage.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/ratepaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/refund.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/refundpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/refundrequestbody.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/rmanumber.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/servicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/servicegroupaccountandservicelevel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/servicegroupcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/servicegrouptypeenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/servicegroupupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/servicelevel.py
--rw-r--r--   0 runner    (1001) docker     (127)    42151 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/servicelevelenumset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/shipment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/shipmentcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)    13950 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/shipmentextra.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/shipmentpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/shippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/shippoaccountpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/shippoaccountupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/track.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/trackingstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/trackingstatusenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/trackingstatuslocationbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/trackingstatussubstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/tracksrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6858 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/transactioncreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/transactionpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/transactionstatusenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/upsconnectexistingownaccountparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/userparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/userparceltemplateupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/weightunitenum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:22:00.443736 shippo-3.3.5/src/shippo/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/errors/initiateoauth2signin.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:22:00.443736 shippo-3.3.5/src/shippo/models/internal/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/internal/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:22:00.451736 shippo-3.3.5/src/shippo/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/addshipmentstobatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/createaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/createbatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/createcarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/createcustomsdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/createcustomsitem.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/createliverate.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/createmanifest.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/createorder.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/createparcel.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/createpickup.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/createrefund.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/createservicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/createshipment.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/createshippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/createtrack.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/createtransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/createuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/deletedefaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/deleteservicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/deleteuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/getaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/getbatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/getcarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/getcarrierparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/getcarrierregistrationstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/getcustomsdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/getcustomsitem.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/getdefaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/getmanifest.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/getorder.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/getparcel.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/getrate.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/getrefund.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/getshipment.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/getshippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/gettrack.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/gettransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/getuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/initiateoauth2signin.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/listaddresses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/listcarrieraccounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/listcarrierparceltemplates.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/listcustomsdeclarations.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/listcustomsitems.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/listmanifests.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/listorders.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/listparcels.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/listrefunds.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/listservicegroups.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/listshipmentrates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/listshipmentratesbycurrencycode.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/listshipments.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/listshippoaccounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/listtransactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/listuserparceltemplates.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/purchasebatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/registercarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/removeshipmentsfrombatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/updatecarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/updatedefaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/updateservicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/updateshippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/updateuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/validateaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)    11426 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/orders.py
--rw-r--r--   0 runner    (1001) docker     (127)    11043 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/pickups.py
--rw-r--r--   0 runner    (1001) docker     (127)    11708 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/rates.py
--rw-r--r--   0 runner    (1001) docker     (127)    15562 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/rates_at_checkout.py
--rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/refunds.py
--rw-r--r--   0 runner    (1001) docker     (127)    15308 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/sdkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14022 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/service_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    12041 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/shipments.py
--rw-r--r--   0 runner    (1001) docker     (127)    15058 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/shippo_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8835 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/tracking_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    11272 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19025 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/user_parcel_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:22:00.455736 shippo-3.3.5/src/shippo/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    32651 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:22:00.423736 shippo-3.3.5/src/shippo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17808 2024-05-08 01:22:00.000000 shippo-3.3.5/src/shippo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11865 2024-05-08 01:22:00.000000 shippo-3.3.5/src/shippo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 01:22:00.000000 shippo-3.3.5/src/shippo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-08 01:22:00.000000 shippo-3.3.5/src/shippo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 01:22:00.000000 shippo-3.3.5/src/shippo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:30:52.044443 shippo-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-10 18:30:42.000000 shippo-3.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17812 2024-05-10 18:30:52.040443 shippo-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-05-10 18:30:42.000000 shippo-3.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 18:30:52.044443 shippo-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-10 18:30:42.000000 shippo-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:30:52.008443 shippo-3.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:30:52.012443 shippo-3.4.0/src/shippo/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:30:52.012443 shippo-3.4.0/src/shippo/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/_hooks/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14213 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19824 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/batches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28485 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/carrier_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8402 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/carrier_parcel_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11175 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/customs_declarations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10952 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/customs_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11114 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/manifests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:30:52.012443 shippo-3.4.0/src/shippo/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:30:52.032443 shippo-3.4.0/src/shippo/models/components/
+-rw-r--r--   0 runner    (1001) docker     (127)    10886 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/addresscompletecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/addresscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/addressimporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/addresspaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/addressvalidationresults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/addressvalidationresultsmessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/alcohol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/batchcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/batchshipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/batchshipmentbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/batchshipmenterrormessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/batchshipmentpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/carrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/carrieraccountbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/carrieraccountchronopostcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/carrieraccountcolissimocreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/carrieraccountcorreoscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/carrieraccountdpddecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/carrieraccountdpdukcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/carrieraccountfedexcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/carrieraccounthermesukcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/carrieraccountmondialrelaycreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/carrieraccountpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/carrieraccountregistrationstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/carrieraccountservicelevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/carrieraccountupscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/carrieraccountupscreaterequestparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/carrieraccountuspscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/carrieraccountwithextrainfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/carrierparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/carriersenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/cod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/connectexistingownaccountrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/customerreference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/customsdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/customsdeclarationb13afilingoptionenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/customsdeclarationcontentstypeenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/customsdeclarationcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/customsdeclarationeelpfcenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/customsdeclarationincotermenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/customsdeclarationnondeliveryoptionenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/customsdeclarationpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/customsexporteridentification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/customsinvoicedcharges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/customsitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/customsitemcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/customsitempaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/customstaxidentification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/dangerousgoodslithiumbatteries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/dangerousgoodsobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/defaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/defaultparceltemplateupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/departmentnumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/distanceunitenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/dryice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/fedexconnectexistingownaccountparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/instanttransactioncreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/instanttransactioncreateresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/instanttransactionrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/insurance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/invoicenumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/labelfiletypeenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/lineitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/lineitembase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/liverate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/liveratecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/liveratepaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/manifestcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/manifestpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/objectstateenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/ordercreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/orderpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/orderstatusenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/parcelcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/parcelextra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/parcelinsurance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/parcelpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/parcelrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10259 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/parceltemplateenumset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5867 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/pickup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/pickupbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/ponumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6549 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/ratepaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/refund.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/refundpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/refundrequestbody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/responsemessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/rmanumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/servicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/servicegroupaccountandservicelevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/servicegroupcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/servicegrouptypeenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/servicegroupupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/servicelevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42151 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/servicelevelenumset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6062 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/shipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/shipmentcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13950 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/shipmentextra.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/shipmentpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/shippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/shippoaccountpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/shippoaccountupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/track.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/trackingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/trackingstatusenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/trackingstatuslocationbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/trackingstatussubstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/tracksrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/transactioncreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/transactionpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/transactionstatusenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/upsconnectexistingownaccountparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/userparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/userparceltemplateupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/components/weightunitenum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:30:52.032443 shippo-3.4.0/src/shippo/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/errors/initiateoauth2signin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:30:52.032443 shippo-3.4.0/src/shippo/models/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/internal/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:30:52.040443 shippo-3.4.0/src/shippo/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/addshipmentstobatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/createaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/createbatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/createcarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/createcustomsdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/createcustomsitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/createliverate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/createmanifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/createorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/createparcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/createpickup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/createrefund.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/createservicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/createshipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/createshippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/createtrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/createtransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/createuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/deletedefaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/deleteservicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/deleteuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/getaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/getbatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/getcarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/getcarrierparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/getcarrierregistrationstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/getcustomsdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/getcustomsitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/getdefaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/getmanifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/getorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/getparcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/getrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/getrefund.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/getshipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/getshippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/gettrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/gettransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/getuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/initiateoauth2signin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/listaddresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/listcarrieraccounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/listcarrierparceltemplates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/listcustomsdeclarations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/listcustomsitems.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/listmanifests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/listorders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/listparcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/listrefunds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/listservicegroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/listshipmentrates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/listshipmentratesbycurrencycode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/listshipments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/listshippoaccounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/listtransactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/listuserparceltemplates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/purchasebatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/registercarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/removeshipmentsfrombatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/updatecarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/updatedefaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/updateservicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/updateshippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/updateuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/models/operations/validateaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11426 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11043 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/pickups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11708 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/rates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15562 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/rates_at_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/refunds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15308 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/sdkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14029 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/service_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12041 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/shipments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15058 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/shippo_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8835 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/tracking_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11272 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19025 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/user_parcel_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:30:52.040443 shippo-3.4.0/src/shippo/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32651 2024-05-10 18:30:42.000000 shippo-3.4.0/src/shippo/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:30:52.012443 shippo-3.4.0/src/shippo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17812 2024-05-10 18:30:51.000000 shippo-3.4.0/src/shippo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-05-10 18:30:51.000000 shippo-3.4.0/src/shippo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 18:30:51.000000 shippo-3.4.0/src/shippo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-10 18:30:51.000000 shippo-3.4.0/src/shippo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 18:30:51.000000 shippo-3.4.0/src/shippo.egg-info/top_level.txt
```

### Comparing `shippo-3.3.5/PKG-INFO` & `shippo-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: shippo
-Version: 3.3.5
+Version: 3.4.0
 Summary: Shipping API Python library (USPS, FedEx, UPS and more)
 Home-page: https://github.com/goshippo/shippo-python-sdk.git
 Author: Shippo
-License: UNKNOWN
+License: MIT License
 Description: # <img src="https://docs.goshippo.com/images/Logo.png" width="30" alt="Shippo logo"> Shippo Python SDK 
         
         Shippo is a shipping API that connects you with [multiple shipping carriers](https://goshippo.com/carriers) (such as USPS, UPS, DHL, Canada Post, Australia Post, and many others) through one interface.
         
         You must register for a [Shippo account](https://apps.goshippo.com/join) to use our API. It's free to sign up. Only pay to print a live label, test labels are free.
         
         To use the API, you must generate an [API Token](https://docs.goshippo.com/docs/guides_general/authentication/). In the following examples, replace `<YOUR_API_KEY_HERE>` with your own token.
```

### Comparing `shippo-3.3.5/README.md` & `shippo-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/setup.py` & `shippo-3.4.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,17 +15,18 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='shippo',
-    version='3.3.5',
+    version='3.4.0',
     author='Shippo',
     description='Shipping API Python library (USPS, FedEx, UPS and more)',
+    license = 'MIT License',
     url='https://github.com/goshippo/shippo-python-sdk.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
         "certifi>=2023.7.22",
         "charset-normalizer>=3.2.0",
```

### Comparing `shippo-3.3.5/src/shippo/_hooks/registration.py` & `shippo-3.4.0/src/shippo/_hooks/registration.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/_hooks/sdkhooks.py` & `shippo-3.4.0/src/shippo/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/_hooks/types.py` & `shippo-3.4.0/src/shippo/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/addresses.py` & `shippo-3.4.0/src/shippo/addresses.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/batches.py` & `shippo-3.4.0/src/shippo/batches.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/carrier_accounts.py` & `shippo-3.4.0/src/shippo/carrier_accounts.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/carrier_parcel_templates.py` & `shippo-3.4.0/src/shippo/carrier_parcel_templates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/customs_declarations.py` & `shippo-3.4.0/src/shippo/customs_declarations.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/customs_items.py` & `shippo-3.4.0/src/shippo/customs_items.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/debug.py` & `shippo-3.4.0/src/shippo/debug.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/manifests.py` & `shippo-3.4.0/src/shippo/manifests.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/__init__.py` & `shippo-3.4.0/src/shippo/models/components/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from .addressvalidationresults import *
 from .addressvalidationresultsmessage import *
 from .alcohol import *
 from .batch import *
 from .batchcreaterequest import *
 from .batchshipment import *
 from .batchshipmentbase import *
+from .batchshipmenterrormessage import *
 from .batchshipmentpaginatedlist import *
 from .billing import *
 from .carrieraccount import *
 from .carrieraccountbase import *
 from .carrieraccountcanadapostcreateparameters import *
 from .carrieraccountcanadapostcreaterequest import *
 from .carrieraccountchronopostcreaterequest import *
@@ -60,15 +61,14 @@
 from .dangerousgoodslithiumbatteries import *
 from .dangerousgoodsobject import *
 from .defaultparceltemplate import *
 from .defaultparceltemplateupdaterequest import *
 from .departmentnumber import *
 from .distanceunitenum import *
 from .dryice import *
-from .errormessage import *
 from .fedexconnectexistingownaccountparameters import *
 from .instanttransactioncreaterequest import *
 from .instanttransactioncreateresponse import *
 from .instanttransactionrate import *
 from .insurance import *
 from .invoicenumber import *
 from .labelfiletypeenum import *
@@ -93,19 +93,19 @@
 from .parcelpaginatedlist import *
 from .parcelrequest import *
 from .parceltemplateenumset import *
 from .pickup import *
 from .pickupbase import *
 from .ponumber import *
 from .rate import *
-from .ratemessage import *
 from .ratepaginatedlist import *
 from .refund import *
 from .refundpaginatedlist import *
 from .refundrequestbody import *
+from .responsemessage import *
 from .rmanumber import *
 from .security import *
 from .servicegroup import *
 from .servicegroupaccountandservicelevel import *
 from .servicegroupcreaterequest import *
 from .servicegrouptypeenum import *
 from .servicegroupupdaterequest import *
@@ -131,8 +131,8 @@
 from .upsconnectexistingownaccountparameters import *
 from .userparceltemplate import *
 from .userparceltemplateupdaterequest import *
 from .userparceltemplatewithcarriertemplatecreaterequest import *
 from .userparceltemplatewithoutcarriertemplatecreaterequest import *
 from .weightunitenum import *
 
-__all__ = ["Address","AddressCompleteCreateRequest","AddressCreateRequest","AddressImporter","AddressPaginatedList","AddressValidationResults","AddressValidationResultsMessage","Alcohol","AncillaryEndorsement","Attributes","Authentication","Batch","BatchCreateRequest","BatchShipment","BatchShipmentBase","BatchShipmentPaginatedList","BatchStatus","Billing","BuildingLocationType","BuildingType","CarrierAccount","CarrierAccountBase","CarrierAccountCanadaPostCreateParameters","CarrierAccountCanadaPostCreateRequest","CarrierAccountChronopostCreateRequest","CarrierAccountChronopostCreateRequestParameters","CarrierAccountColissimoCreateRequest","CarrierAccountColissimoCreateRequestParameters","CarrierAccountCorreosCreateRequest","CarrierAccountCorreosCreateRequestParameters","CarrierAccountDHLExpressCreateRequest","CarrierAccountDHLExpressCreateRequestParameters","CarrierAccountDPDUKCreateRequest","CarrierAccountDPDUKCreateRequestParameters","CarrierAccountDeutschePostCreateRequest","CarrierAccountDeutschePostCreateRequestParameters","CarrierAccountDpdDeCreateRequest","CarrierAccountDpdDeCreateRequestParameters","CarrierAccountFedExCreateRequest","CarrierAccountFedExCreateRequestParameters","CarrierAccountHermesUKCreateRequest","CarrierAccountHermesUKCreateRequestParameters","CarrierAccountMondialRelayCreateRequest","CarrierAccountMondialRelayCreateRequestParameters","CarrierAccountPaginatedList","CarrierAccountPosteItalianeCreateRequest","CarrierAccountPosteItalianeCreateRequestParameters","CarrierAccountRegistrationStatus","CarrierAccountServiceLevel","CarrierAccountUPSCreateRequest","CarrierAccountUPSCreateRequestParameters","CarrierAccountUSPSCreateRequest","CarrierAccountUSPSCreateRequestParameters","CarrierAccountWithExtraInfo","CarrierAccountWithExtraInfoStatus","CarrierAccountWithExtraInfoType","CarrierParcelTemplate","CarriersEnum","Cod","Code","ConnectExistingOwnAccountRequest","CustomerReference","CustomsDeclaration","CustomsDeclarationAddressImporter","CustomsDeclarationB13AFilingOptionEnum","CustomsDeclarationContentsTypeEnum","CustomsDeclarationCreateRequest","CustomsDeclarationEelPfcEnum","CustomsDeclarationIncotermEnum","CustomsDeclarationNonDeliveryOptionEnum","CustomsDeclarationPaginatedList","CustomsExporterIdentification","CustomsInvoicedCharges","CustomsItem","CustomsItemCreateRequest","CustomsItemPaginatedList","CustomsTaxIdentification","CustomsTaxIdentificationType","DangerousGoodsBiologicalMaterial","DangerousGoodsCode","DangerousGoodsLithiumBatteries","DangerousGoodsObject","DefaultParcelTemplate","DefaultParcelTemplateUpdateRequest","DepartmentNumber","DistanceUnitEnum","DryIce","ErrorMessage","FedExConnectExistingOwnAccountParameters","InstantTransactionCreateRequest","InstantTransactionCreateResponse","InstantTransactionCreateResponseMessages","InstantTransactionCreateResponseResponseType","InstantTransactionRate","Insurance","InvoiceNumber","LabelFileType","LabelFileTypeEnum","LasershipAttrs","LineItem","LineItemBase","LiveRate","LiveRateCreateRequest","LiveRatePaginatedList","Location","Manifest","ManifestCreateRequest","ManifestPaginatedList","ManifestStatus","Messages","ObjectInfo","ObjectResults","ObjectState","ObjectStateEnum","Order","OrderCreateRequest","OrderPaginatedList","OrderStatusEnum","Parcel","ParcelCreateRequest","ParcelExtra","ParcelInsurance","ParcelInsuranceProvider","ParcelPaginatedList","ParcelRequest","ParcelTemplateAramexAustraliaEnum","ParcelTemplateCouriersPleaseEnum","ParcelTemplateDHLeCommerceEnum","ParcelTemplateDPDUKEnum","ParcelTemplateFedExEnum","ParcelTemplateUPSEnum","ParcelTemplateUSPSEnum","PaymentMethod","Pickup","PickupBase","PickupStatus","PoNumber","PreferredDeliveryTimeframe","Provider","Rate","RateMessage","RatePaginatedList","RecipientType","Refund","RefundPaginatedList","RefundRequestBody","RefundStatus","ResponseType","ReturnServiceType","RmaNumber","Security","ServiceGroup","ServiceGroupAccountAndServiceLevel","ServiceGroupCreateRequest","ServiceGroupTypeEnum","ServiceGroupUpdateRequest","ServiceLevel","ServiceLevelAPCPostalEnum","ServiceLevelAPGEnum","ServiceLevelAirterraEnum","ServiceLevelAramexAustraliaEnum","ServiceLevelAsendiaEnum","ServiceLevelAustraliaPostEnum","ServiceLevelAxleHireEnum","ServiceLevelBetterTrucksEnum","ServiceLevelCDLEnum","ServiceLevelCanadaPostEnum","ServiceLevelChronopostEnum","ServiceLevelColissimoEnum","ServiceLevelCorreosEspanaEnum","ServiceLevelCouriersPleaseEnum","ServiceLevelDHLExpressEnum","ServiceLevelDHLGermanyEnum","ServiceLevelDHLeCommerceEnum","ServiceLevelDPDDEEnum","ServiceLevelDPDUKEnum","ServiceLevelDeutschePostEnum","ServiceLevelEvriUKEnum","ServiceLevelFedExEnum","ServiceLevelGLSUSEnum","ServiceLevelGlobegisticsEnum","ServiceLevelLSOEnum","ServiceLevelLasershipEnum","ServiceLevelMaergoEnum","ServiceLevelMondialRelayEnum","ServiceLevelOnTracEnum","ServiceLevelParcelforceEnum","ServiceLevelPostItalianeEnum","ServiceLevelPurolatorEnum","ServiceLevelRoyalMailEnum","ServiceLevelSendleEnum","ServiceLevelSwyftEnum","ServiceLevelUDSEnum","ServiceLevelUPSEnum","ServiceLevelUSPSEnum","ServiceLevelVehoEnum","ServiceLevelePostGlobalEnum","Shipment","ShipmentCreateRequest","ShipmentExtra","ShipmentPaginatedList","ShipmentStatus","ShippoAccount","ShippoAccountPaginatedList","ShippoAccountUpdateRequest","ShopApp","SignatureConfirmation","Source","Status","Track","TrackingStatus","TrackingStatusEnum","TrackingStatusLocationBase","TrackingStatusSubstatus","TracksRequest","Transaction","TransactionCreateRequest","TransactionMessages","TransactionPaginatedList","TransactionStatusEnum","Type","UPSConnectExistingOwnAccountParameters","UserParcelTemplate","UserParcelTemplateUpdateRequest","UserParcelTemplateWithCarrierTemplateCreateRequest","UserParcelTemplateWithoutCarrierTemplateCreateRequest","WeightUnitEnum"]
+__all__ = ["Address","AddressCompleteCreateRequest","AddressCreateRequest","AddressImporter","AddressPaginatedList","AddressValidationResults","AddressValidationResultsMessage","Alcohol","AncillaryEndorsement","Attributes","Authentication","Batch","BatchCreateRequest","BatchShipment","BatchShipmentBase","BatchShipmentErrorMessage","BatchShipmentPaginatedList","BatchStatus","Billing","BuildingLocationType","BuildingType","CarrierAccount","CarrierAccountBase","CarrierAccountCanadaPostCreateParameters","CarrierAccountCanadaPostCreateRequest","CarrierAccountChronopostCreateRequest","CarrierAccountChronopostCreateRequestParameters","CarrierAccountColissimoCreateRequest","CarrierAccountColissimoCreateRequestParameters","CarrierAccountCorreosCreateRequest","CarrierAccountCorreosCreateRequestParameters","CarrierAccountDHLExpressCreateRequest","CarrierAccountDHLExpressCreateRequestParameters","CarrierAccountDPDUKCreateRequest","CarrierAccountDPDUKCreateRequestParameters","CarrierAccountDeutschePostCreateRequest","CarrierAccountDeutschePostCreateRequestParameters","CarrierAccountDpdDeCreateRequest","CarrierAccountDpdDeCreateRequestParameters","CarrierAccountFedExCreateRequest","CarrierAccountFedExCreateRequestParameters","CarrierAccountHermesUKCreateRequest","CarrierAccountHermesUKCreateRequestParameters","CarrierAccountMondialRelayCreateRequest","CarrierAccountMondialRelayCreateRequestParameters","CarrierAccountPaginatedList","CarrierAccountPosteItalianeCreateRequest","CarrierAccountPosteItalianeCreateRequestParameters","CarrierAccountRegistrationStatus","CarrierAccountServiceLevel","CarrierAccountUPSCreateRequest","CarrierAccountUPSCreateRequestParameters","CarrierAccountUSPSCreateRequest","CarrierAccountUSPSCreateRequestParameters","CarrierAccountWithExtraInfo","CarrierAccountWithExtraInfoStatus","CarrierAccountWithExtraInfoType","CarrierParcelTemplate","CarriersEnum","Cod","Code","ConnectExistingOwnAccountRequest","CustomerReference","CustomsDeclaration","CustomsDeclarationAddressImporter","CustomsDeclarationB13AFilingOptionEnum","CustomsDeclarationContentsTypeEnum","CustomsDeclarationCreateRequest","CustomsDeclarationEelPfcEnum","CustomsDeclarationIncotermEnum","CustomsDeclarationNonDeliveryOptionEnum","CustomsDeclarationPaginatedList","CustomsExporterIdentification","CustomsInvoicedCharges","CustomsItem","CustomsItemCreateRequest","CustomsItemPaginatedList","CustomsTaxIdentification","CustomsTaxIdentificationType","DangerousGoodsBiologicalMaterial","DangerousGoodsCode","DangerousGoodsLithiumBatteries","DangerousGoodsObject","DefaultParcelTemplate","DefaultParcelTemplateUpdateRequest","DepartmentNumber","DistanceUnitEnum","DryIce","FedExConnectExistingOwnAccountParameters","InstantTransactionCreateRequest","InstantTransactionCreateResponse","InstantTransactionCreateResponseResponseType","InstantTransactionRate","Insurance","InvoiceNumber","LabelFileType","LabelFileTypeEnum","LasershipAttrs","LineItem","LineItemBase","LiveRate","LiveRateCreateRequest","LiveRatePaginatedList","Location","Manifest","ManifestCreateRequest","ManifestPaginatedList","ManifestStatus","ObjectInfo","ObjectResults","ObjectState","ObjectStateEnum","Order","OrderCreateRequest","OrderPaginatedList","OrderStatusEnum","Parcel","ParcelCreateRequest","ParcelExtra","ParcelInsurance","ParcelInsuranceProvider","ParcelPaginatedList","ParcelRequest","ParcelTemplateAramexAustraliaEnum","ParcelTemplateCouriersPleaseEnum","ParcelTemplateDHLeCommerceEnum","ParcelTemplateDPDUKEnum","ParcelTemplateFedExEnum","ParcelTemplateUPSEnum","ParcelTemplateUSPSEnum","PaymentMethod","Pickup","PickupBase","PickupStatus","PoNumber","PreferredDeliveryTimeframe","Provider","Rate","RatePaginatedList","RecipientType","Refund","RefundPaginatedList","RefundRequestBody","RefundStatus","ResponseMessage","ResponseType","ReturnServiceType","RmaNumber","Security","ServiceGroup","ServiceGroupAccountAndServiceLevel","ServiceGroupCreateRequest","ServiceGroupTypeEnum","ServiceGroupUpdateRequest","ServiceLevel","ServiceLevelAPCPostalEnum","ServiceLevelAPGEnum","ServiceLevelAirterraEnum","ServiceLevelAramexAustraliaEnum","ServiceLevelAsendiaEnum","ServiceLevelAustraliaPostEnum","ServiceLevelAxleHireEnum","ServiceLevelBetterTrucksEnum","ServiceLevelCDLEnum","ServiceLevelCanadaPostEnum","ServiceLevelChronopostEnum","ServiceLevelColissimoEnum","ServiceLevelCorreosEspanaEnum","ServiceLevelCouriersPleaseEnum","ServiceLevelDHLExpressEnum","ServiceLevelDHLGermanyEnum","ServiceLevelDHLeCommerceEnum","ServiceLevelDPDDEEnum","ServiceLevelDPDUKEnum","ServiceLevelDeutschePostEnum","ServiceLevelEvriUKEnum","ServiceLevelFedExEnum","ServiceLevelGLSUSEnum","ServiceLevelGlobegisticsEnum","ServiceLevelLSOEnum","ServiceLevelLasershipEnum","ServiceLevelMaergoEnum","ServiceLevelMondialRelayEnum","ServiceLevelOnTracEnum","ServiceLevelParcelforceEnum","ServiceLevelPostItalianeEnum","ServiceLevelPurolatorEnum","ServiceLevelRoyalMailEnum","ServiceLevelSendleEnum","ServiceLevelSwyftEnum","ServiceLevelUDSEnum","ServiceLevelUPSEnum","ServiceLevelUSPSEnum","ServiceLevelVehoEnum","ServiceLevelePostGlobalEnum","Shipment","ShipmentCreateRequest","ShipmentExtra","ShipmentPaginatedList","ShipmentStatus","ShippoAccount","ShippoAccountPaginatedList","ShippoAccountUpdateRequest","ShopApp","SignatureConfirmation","Source","Status","Track","TrackingStatus","TrackingStatusEnum","TrackingStatusLocationBase","TrackingStatusSubstatus","TracksRequest","Transaction","TransactionCreateRequest","TransactionPaginatedList","TransactionStatusEnum","Type","UPSConnectExistingOwnAccountParameters","UserParcelTemplate","UserParcelTemplateUpdateRequest","UserParcelTemplateWithCarrierTemplateCreateRequest","UserParcelTemplateWithoutCarrierTemplateCreateRequest","WeightUnitEnum"]
```

### Comparing `shippo-3.3.5/src/shippo/models/components/address.py` & `shippo-3.4.0/src/shippo/models/components/address.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/addresscompletecreaterequest.py` & `shippo-3.4.0/src/shippo/models/components/addresscompletecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/addresscreaterequest.py` & `shippo-3.4.0/src/shippo/models/components/addresscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/addressimporter.py` & `shippo-3.4.0/src/shippo/models/components/addressimporter.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/addresspaginatedlist.py` & `shippo-3.4.0/src/shippo/models/components/addresspaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/addressvalidationresults.py` & `shippo-3.4.0/src/shippo/models/components/addressvalidationresults.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/addressvalidationresultsmessage.py` & `shippo-3.4.0/src/shippo/models/components/addressvalidationresultsmessage.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/alcohol.py` & `shippo-3.4.0/src/shippo/models/components/alcohol.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/batch.py` & `shippo-3.4.0/src/shippo/models/components/batch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/batchcreaterequest.py` & `shippo-3.4.0/src/shippo/models/components/batchcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/batchshipment.py` & `shippo-3.4.0/src/shippo/models/components/batchshipment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from .errormessage import ErrorMessage
+from .batchshipmenterrormessage import BatchShipmentErrorMessage
 from .shipmentcreaterequest import ShipmentCreateRequest
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from shippo import utils
 from typing import List, Optional
 
 class Status(str, Enum):
@@ -40,13 +40,13 @@
     to attach to the object.
     """
     servicelevel_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('servicelevel_token'), 'exclude': lambda f: f is None }})
     r"""A token that sets the shipping method for the batch, overriding the batch default.
     Servicelevel tokens can be found <a href=\"#tag/Service-Levels\">in this list</a> 
     or <a href=\"#operation/ListCarrierAccounts\">at this endpoint</a>.
     """
-    messages: Optional[List[ErrorMessage]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('messages'), 'exclude': lambda f: f is None }})
+    messages: Optional[List[BatchShipmentErrorMessage]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('messages'), 'exclude': lambda f: f is None }})
     r"""List of Shipment and Transaction error messages."""
     transaction: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transaction'), 'exclude': lambda f: f is None }})
     r"""Object ID of the transaction object created for this batch shipment."""
```

### Comparing `shippo-3.3.5/src/shippo/models/components/batchshipmentbase.py` & `shippo-3.4.0/src/shippo/models/components/batchshipmentbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/batchshipmentpaginatedlist.py` & `shippo-3.4.0/src/shippo/models/components/batchshipmentpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/billing.py` & `shippo-3.4.0/src/shippo/models/components/billing.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/carrieraccount.py` & `shippo-3.4.0/src/shippo/models/components/carrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/carrieraccountbase.py` & `shippo-3.4.0/src/shippo/models/components/carrieraccountbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py` & `shippo-3.4.0/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py` & `shippo-3.4.0/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/carrieraccountchronopostcreaterequest.py` & `shippo-3.4.0/src/shippo/models/components/carrieraccountchronopostcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/carrieraccountcolissimocreaterequest.py` & `shippo-3.4.0/src/shippo/models/components/carrieraccountcolissimocreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/carrieraccountcorreoscreaterequest.py` & `shippo-3.4.0/src/shippo/models/components/carrieraccountcorreoscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py` & `shippo-3.4.0/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py` & `shippo-3.4.0/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py` & `shippo-3.4.0/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/carrieraccountdpddecreaterequest.py` & `shippo-3.4.0/src/shippo/models/components/carrieraccountdpddecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/carrieraccountdpdukcreaterequest.py` & `shippo-3.4.0/src/shippo/models/components/carrieraccountdpdukcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/carrieraccountfedexcreaterequest.py` & `shippo-3.4.0/src/shippo/models/components/carrieraccountfedexcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/carrieraccounthermesukcreaterequest.py` & `shippo-3.4.0/src/shippo/models/components/carrieraccounthermesukcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/carrieraccountmondialrelaycreaterequest.py` & `shippo-3.4.0/src/shippo/models/components/carrieraccountmondialrelaycreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/carrieraccountpaginatedlist.py` & `shippo-3.4.0/src/shippo/models/components/carrieraccountpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py` & `shippo-3.4.0/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/carrieraccountregistrationstatus.py` & `shippo-3.4.0/src/shippo/models/components/carrieraccountregistrationstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/carrieraccountservicelevel.py` & `shippo-3.4.0/src/shippo/models/components/carrieraccountservicelevel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/carrieraccountupscreaterequest.py` & `shippo-3.4.0/src/shippo/models/components/carrieraccountupscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/carrieraccountupscreaterequestparameters.py` & `shippo-3.4.0/src/shippo/models/components/carrieraccountupscreaterequestparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/carrieraccountuspscreaterequest.py` & `shippo-3.4.0/src/shippo/models/components/carrieraccountuspscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/carrieraccountwithextrainfo.py` & `shippo-3.4.0/src/shippo/models/components/carrieraccountwithextrainfo.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/carrierparceltemplate.py` & `shippo-3.4.0/src/shippo/models/components/carrierparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/carriersenum.py` & `shippo-3.4.0/src/shippo/models/components/carriersenum.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/cod.py` & `shippo-3.4.0/src/shippo/models/components/cod.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/connectexistingownaccountrequest.py` & `shippo-3.4.0/src/shippo/models/components/connectexistingownaccountrequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/customerreference.py` & `shippo-3.4.0/src/shippo/models/components/customerreference.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/customsdeclaration.py` & `shippo-3.4.0/src/shippo/models/components/customsdeclaration.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/customsdeclarationb13afilingoptionenum.py` & `shippo-3.4.0/src/shippo/models/components/customsdeclarationb13afilingoptionenum.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/customsdeclarationcreaterequest.py` & `shippo-3.4.0/src/shippo/models/components/customsdeclarationcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/customsdeclarationeelpfcenum.py` & `shippo-3.4.0/src/shippo/models/components/customsdeclarationeelpfcenum.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/customsdeclarationincotermenum.py` & `shippo-3.4.0/src/shippo/models/components/customsdeclarationincotermenum.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/customsdeclarationpaginatedlist.py` & `shippo-3.4.0/src/shippo/models/components/customsdeclarationpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/customsexporteridentification.py` & `shippo-3.4.0/src/shippo/models/components/customsexporteridentification.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/customsinvoicedcharges.py` & `shippo-3.4.0/src/shippo/models/components/customsinvoicedcharges.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/customsitem.py` & `shippo-3.4.0/src/shippo/models/components/customsitem.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/customsitemcreaterequest.py` & `shippo-3.4.0/src/shippo/models/components/customsitemcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/customsitempaginatedlist.py` & `shippo-3.4.0/src/shippo/models/components/customsitempaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/customstaxidentification.py` & `shippo-3.4.0/src/shippo/models/components/customstaxidentification.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py` & `shippo-3.4.0/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/dangerousgoodslithiumbatteries.py` & `shippo-3.4.0/src/shippo/models/components/dangerousgoodslithiumbatteries.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/dangerousgoodsobject.py` & `shippo-3.4.0/src/shippo/models/components/dangerousgoodsobject.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/defaultparceltemplate.py` & `shippo-3.4.0/src/shippo/models/components/defaultparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/defaultparceltemplateupdaterequest.py` & `shippo-3.4.0/src/shippo/models/components/defaultparceltemplateupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/departmentnumber.py` & `shippo-3.4.0/src/shippo/models/components/departmentnumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/dryice.py` & `shippo-3.4.0/src/shippo/models/components/dryice.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/errormessage.py` & `shippo-3.4.0/src/shippo/models/components/tracksrequest.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
-from typing import Dict, List, Optional
+from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class ErrorMessage:
-    shipment: Optional[List[Dict[str, List[str]]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('shipment'), 'exclude': lambda f: f is None }})
+class TracksRequest:
+    carrier: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('carrier') }})
+    r"""Name of the carrier of the shipment to track."""
+    tracking_number: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tracking_number') }})
+    r"""Tracking number to track."""
+    metadata: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
+    r"""A string of up to 100 characters that can be filled with any additional information you want to attach to the object."""
```

### Comparing `shippo-3.3.5/src/shippo/models/components/fedexconnectexistingownaccountparameters.py` & `shippo-3.4.0/src/shippo/models/components/fedexconnectexistingownaccountparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/instanttransactioncreaterequest.py` & `shippo-3.4.0/src/shippo/models/components/instanttransactioncreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/instanttransactioncreateresponse.py` & `shippo-3.4.0/src/shippo/models/components/transaction.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,54 +1,45 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
-from .instanttransactionrate import InstantTransactionRate
 from .labelfiletypeenum import LabelFileTypeEnum
 from .objectstateenum import ObjectStateEnum
+from .responsemessage import ResponseMessage
 from .trackingstatusenum import TrackingStatusEnum
 from .transactionstatusenum import TransactionStatusEnum
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from shippo import utils
 from typing import List, Optional
 
-
-@dataclasses.dataclass
-class InstantTransactionCreateResponseMessages:
-    pass
-
-class InstantTransactionCreateResponseResponseType(str, Enum):
-    INSTANT = 'instant'
+class ResponseType(str, Enum):
+    STANDARD = 'standard'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class InstantTransactionCreateResponse:
+class Transaction:
     commercial_invoice_url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('commercial_invoice_url'), 'exclude': lambda f: f is None }})
     r"""A URL pointing to the commercial invoice as a 8.5x11 inch PDF file.
     A value will only be returned if the Transactions has been processed successfully and if the shipment is international.
     """
     eta: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eta'), 'exclude': lambda f: f is None }})
     r"""The estimated time of arrival according to the carrier."""
     label_file_type: Optional[LabelFileTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('label_file_type'), 'exclude': lambda f: f is None }})
     r"""Print format of the <a href=\\"https://docs.goshippo.com/docs/shipments/shippinglabelsizes/\\">label</a>. If empty, will use the default format set from
     <a href=\"https://apps.goshippo.com/settings/labels\">the Shippo dashboard.</a>
     """
     label_url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('label_url'), 'exclude': lambda f: f is None }})
     r"""A URL pointing directly to the label in the format you've set in your settings.
     A value will only be returned if the Transactions has been processed successfully.
     """
-    messages: Optional[List[InstantTransactionCreateResponseMessages]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('messages'), 'exclude': lambda f: f is None }})
-    r"""An array containing elements of the following schema:<br>
-    `code` (string): an identifier for the corresponding message (not always available)<br>
-    `message` (string): a publishable message containing further information.
-    """
+    messages: Optional[List[ResponseMessage]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('messages'), 'exclude': lambda f: f is None }})
     metadata: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
     r"""A string of up to 100 characters that can be filled with any additional information you want to
     attach to the object.
     """
     object_created: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_created'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
     r"""Date and time of Transaction creation."""
     object_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_id'), 'exclude': lambda f: f is None }})
@@ -73,11 +64,14 @@
     """
     tracking_status: Optional[TrackingStatusEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tracking_status'), 'exclude': lambda f: f is None }})
     r"""Indicates the high level status of the shipment."""
     tracking_url_provider: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tracking_url_provider'), 'exclude': lambda f: f is None }})
     r"""A link to track this item on the carrier-provided tracking website.
     A value will only be returned if tracking is available and the carrier provides such a service.
     """
-    rate: Optional[InstantTransactionRate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('rate'), 'exclude': lambda f: f is None }})
-    response_type: Optional[InstantTransactionCreateResponseResponseType] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('responseType'), 'exclude': lambda f: f is None }})
+    rate: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('rate'), 'exclude': lambda f: f is None }})
+    r"""ID of the Rate object for which a Label has to be obtained.
+    Please note that only rates that are not older than 7 days can be purchased in order to ensure up-to-date pricing.
+    """
+    response_type: Optional[ResponseType] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('responseType'), 'exclude': lambda f: f is None }})
```

### Comparing `shippo-3.3.5/src/shippo/models/components/instanttransactionrate.py` & `shippo-3.4.0/src/shippo/models/components/instanttransactionrate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/insurance.py` & `shippo-3.4.0/src/shippo/models/components/insurance.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/invoicenumber.py` & `shippo-3.4.0/src/shippo/models/components/invoicenumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/labelfiletypeenum.py` & `shippo-3.4.0/src/shippo/models/components/labelfiletypeenum.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/lineitem.py` & `shippo-3.4.0/src/shippo/models/components/lineitem.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/lineitembase.py` & `shippo-3.4.0/src/shippo/models/components/lineitembase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/liverate.py` & `shippo-3.4.0/src/shippo/models/components/liverate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/liveratecreaterequest.py` & `shippo-3.4.0/src/shippo/models/components/liveratecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/liveratepaginatedlist.py` & `shippo-3.4.0/src/shippo/models/components/liveratepaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/location.py` & `shippo-3.4.0/src/shippo/models/components/location.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/manifest.py` & `shippo-3.4.0/src/shippo/models/components/manifest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/manifestcreaterequest.py` & `shippo-3.4.0/src/shippo/models/components/manifestcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/manifestpaginatedlist.py` & `shippo-3.4.0/src/shippo/models/components/manifestpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/order.py` & `shippo-3.4.0/src/shippo/models/components/order.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/ordercreaterequest.py` & `shippo-3.4.0/src/shippo/models/components/ordercreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/orderpaginatedlist.py` & `shippo-3.4.0/src/shippo/models/components/orderpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/orderstatusenum.py` & `shippo-3.4.0/src/shippo/models/components/orderstatusenum.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/parcel.py` & `shippo-3.4.0/src/shippo/models/components/parcel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/parcelcreaterequest.py` & `shippo-3.4.0/src/shippo/models/components/parcelcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/parcelextra.py` & `shippo-3.4.0/src/shippo/models/components/parcelextra.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/parcelinsurance.py` & `shippo-3.4.0/src/shippo/models/components/parcelinsurance.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/parcelpaginatedlist.py` & `shippo-3.4.0/src/shippo/models/components/parcelpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/parcelrequest.py` & `shippo-3.4.0/src/shippo/models/components/parcelrequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/parceltemplateenumset.py` & `shippo-3.4.0/src/shippo/models/components/parceltemplateenumset.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/pickup.py` & `shippo-3.4.0/src/shippo/models/components/pickup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/pickupbase.py` & `shippo-3.4.0/src/shippo/models/components/pickupbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/ponumber.py` & `shippo-3.4.0/src/shippo/models/components/ponumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/rate.py` & `shippo-3.4.0/src/shippo/models/components/rate.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
-from .ratemessage import RateMessage
+from .responsemessage import ResponseMessage
 from .servicelevel import ServiceLevel
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from shippo import utils
 from typing import List, Optional
 
@@ -61,20 +61,15 @@
     Shippo is not able to guarantee any transit times.
     """
     included_insurance_price: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('included_insurance_price'), 'exclude': lambda f: f is None }})
     r"""Cost to the user to insure the Rate for the requested amount of coverage, if insurance coverage was requested.
     Expressed in the currency used in the sender's country. Will be null if no insurance coverage was requested, or if insurance is requested from a non-standard insurance provider. 
     Please note this price is already included in the `amount` and `amount_local` fields on the Rate. Do not add this field to them.
     """
-    messages: Optional[List[RateMessage]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('messages'), 'exclude': lambda f: f is None }})
-    r"""An array containing elements of the following schema: <br>
-    `source`(string): the name of the carrier sending the message. <br>
-    `code` (string): carrier specific identifier code for the corresponding message (not always available).<br>
-    `text` (string): a publishable message containing further information (not always available).
-    """
+    messages: Optional[List[ResponseMessage]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('messages'), 'exclude': lambda f: f is None }})
     provider_image_75: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('provider_image_75'), 'exclude': lambda f: f is None }})
     r"""URL to the provider logo with max. dimensions of 75*75px.
     Please refer to the provider's Logo Usage Guidelines before using the logo.
     """
     provider_image_200: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('provider_image_200'), 'exclude': lambda f: f is None }})
     r"""URL to the provider logo with max. dimensions of 200*200px.
     Please refer to the provider's Logo Usage Guidelines before using the logo.
```

### Comparing `shippo-3.3.5/src/shippo/models/components/ratemessage.py` & `shippo-3.4.0/src/shippo/models/components/transactionpaginatedlist.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from .transaction import Transaction
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
-from typing import Optional
+from typing import List, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class RateMessage:
-    source: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('source'), 'exclude': lambda f: f is None }})
-    code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('code'), 'exclude': lambda f: f is None }})
-    text: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('text'), 'exclude': lambda f: f is None }})
+class TransactionPaginatedList:
+    next: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})
+    previous: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
+    results: Optional[List[Transaction]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})
```

### Comparing `shippo-3.3.5/src/shippo/models/components/ratepaginatedlist.py` & `shippo-3.4.0/src/shippo/models/components/ratepaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/refund.py` & `shippo-3.4.0/src/shippo/models/components/refund.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/refundpaginatedlist.py` & `shippo-3.4.0/src/shippo/models/components/refundpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/refundrequestbody.py` & `shippo-3.4.0/src/shippo/models/components/refundrequestbody.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/rmanumber.py` & `shippo-3.4.0/src/shippo/models/components/rmanumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/servicegroup.py` & `shippo-3.4.0/src/shippo/models/components/servicegroup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/servicegroupaccountandservicelevel.py` & `shippo-3.4.0/src/shippo/models/components/servicegroupaccountandservicelevel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/servicegroupcreaterequest.py` & `shippo-3.4.0/src/shippo/models/components/servicegroupcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/servicegrouptypeenum.py` & `shippo-3.4.0/src/shippo/models/components/servicegrouptypeenum.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/servicegroupupdaterequest.py` & `shippo-3.4.0/src/shippo/models/components/servicegroupupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/servicelevel.py` & `shippo-3.4.0/src/shippo/models/components/servicelevel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/servicelevelenumset.py` & `shippo-3.4.0/src/shippo/models/components/servicelevelenumset.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/shipment.py` & `shippo-3.4.0/src/shippo/models/components/shipment.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,24 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
 from .address import Address
+from .customsdeclaration import CustomsDeclaration
 from .parcel import Parcel
 from .rate import Rate
+from .responsemessage import ResponseMessage
 from .shipmentextra import ShipmentExtra
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from shippo import utils
 from typing import List, Optional
 
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class Messages:
-    code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('code'), 'exclude': lambda f: f is None }})
-    source: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('source'), 'exclude': lambda f: f is None }})
-    text: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('text'), 'exclude': lambda f: f is None }})
-    
-
-
 class ShipmentStatus(str, Enum):
     r"""`Waiting` shipments have been successfully submitted but not yet been processed.
     `Queued` shipments are currently being processed. 
     `Success` shipments have been processed successfully, meaning that rate generation has concluded. 
     `Error` does not occur currently and is reserved for future use.
     """
     ERROR = 'ERROR'
@@ -46,18 +38,15 @@
     address_to: Address = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address_to') }})
     r"""<a href=\\"#tag/Addresses\\">Address</a> object of the recipient / buyer. Will be returned expanded by default."""
     carrier_accounts: List[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('carrier_accounts') }})
     r"""An array of object_ids of the carrier account objects to be used for getting shipping rates for this shipment.
     If no carrier account object_ids are set in this field, Shippo will attempt to generate rates using all the 
     carrier accounts that have the `active` field set.
     """
-    messages: List[Messages] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('messages') }})
-    r"""An array containing elements of the following schema:<br>`code` (string): an identifier for the corresponding message
-    (not always available)<br>`message` (string): a publishable message containing further information.
-    """
+    messages: List[ResponseMessage] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('messages') }})
     object_created: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_created'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse }})
     r"""Date and time of Shipment creation."""
     object_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_id') }})
     r"""Unique identifier of the given Shipment object."""
     object_owner: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_owner') }})
     r"""Username of the user who created the Shipment object."""
     object_updated: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_updated'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse }})
@@ -71,25 +60,24 @@
     """
     status: ShipmentStatus = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
     r"""`Waiting` shipments have been successfully submitted but not yet been processed.
     `Queued` shipments are currently being processed. 
     `Success` shipments have been processed successfully, meaning that rate generation has concluded. 
     `Error` does not occur currently and is reserved for future use.
     """
-    customs_declaration: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customs_declaration'), 'exclude': lambda f: f is None }})
-    r"""ID of the Customs Declarations object for an international shipment."""
     extra: Optional[ShipmentExtra] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('extra'), 'exclude': lambda f: f is None }})
     r"""An object holding optional extra services to be requested."""
     shipment_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('shipment_date'), 'exclude': lambda f: f is None }})
     r"""Date the shipment will be tendered to the carrier. Must be in the format `2014-01-18T00:35:03.463Z`.
     Defaults to current date and time if no value is provided. Please note that some carriers require this value to
     be in the future, on a working day, or similar.
     """
     address_return: Optional[Address] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address_return'), 'exclude': lambda f: f is None }})
     r"""ID of the Address object where the shipment will be sent back to if it is not delivered
     (Only available for UPS, USPS, and Fedex shipments). <br/> 
     If this field is not set, your shipments will be returned to the address_from.
     """
+    customs_declaration: Optional[CustomsDeclaration] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customs_declaration'), 'exclude': lambda f: f is None }})
     test: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('test'), 'exclude': lambda f: f is None }})
     r"""Indicates whether the object has been created in test mode."""
```

### Comparing `shippo-3.3.5/src/shippo/models/components/shipmentcreaterequest.py` & `shippo-3.4.0/src/shippo/models/components/shipmentcreaterequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from .addresscreaterequest import AddressCreateRequest
+from .customsdeclarationcreaterequest import CustomsDeclarationCreateRequest
 from .parcelcreaterequest import ParcelCreateRequest
 from .shipmentextra import ShipmentExtra
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
 from typing import List, Optional, Union
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ShipmentCreateRequest:
     address_from: Union[AddressCreateRequest, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address_from') }})
     address_to: Union[AddressCreateRequest, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address_to') }})
     parcels: List[Union[ParcelCreateRequest, str]] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parcels') }})
-    customs_declaration: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customs_declaration'), 'exclude': lambda f: f is None }})
-    r"""ID of the Customs Declarations object for an international shipment."""
     extra: Optional[ShipmentExtra] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('extra'), 'exclude': lambda f: f is None }})
     r"""An object holding optional extra services to be requested."""
     metadata: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
     r"""A string of up to 100 characters that can be filled with any additional information you want to attach to the object."""
     shipment_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('shipment_date'), 'exclude': lambda f: f is None }})
     r"""Date the shipment will be tendered to the carrier. Must be in the format `2014-01-18T00:35:03.463Z`.
     Defaults to current date and time if no value is provided. Please note that some carriers require this value to
     be in the future, on a working day, or similar.
     """
     address_return: Optional[Union[AddressCreateRequest, str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address_return'), 'exclude': lambda f: f is None }})
+    customs_declaration: Optional[Union[CustomsDeclarationCreateRequest, str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customs_declaration'), 'exclude': lambda f: f is None }})
     async_: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('async'), 'exclude': lambda f: f is None }})
     carrier_accounts: Optional[List[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('carrier_accounts'), 'exclude': lambda f: f is None }})
     r"""List of <a href=\\"#tag/Carrier-Accounts/\\">Carrier Accounts</a> `object_id`s used to filter
     the returned rates.  If set, only rates from these carriers will be returned.
     """
```

### Comparing `shippo-3.3.5/src/shippo/models/components/shipmentextra.py` & `shippo-3.4.0/src/shippo/models/components/shipmentextra.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/shipmentpaginatedlist.py` & `shippo-3.4.0/src/shippo/models/components/shipmentpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/shippoaccount.py` & `shippo-3.4.0/src/shippo/models/components/shippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/shippoaccountpaginatedlist.py` & `shippo-3.4.0/src/shippo/models/components/shippoaccountpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/shippoaccountupdaterequest.py` & `shippo-3.4.0/src/shippo/models/components/shippoaccountupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/track.py` & `shippo-3.4.0/src/shippo/models/components/track.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/trackingstatus.py` & `shippo-3.4.0/src/shippo/models/components/trackingstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/trackingstatuslocationbase.py` & `shippo-3.4.0/src/shippo/models/components/trackingstatuslocationbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/trackingstatussubstatus.py` & `shippo-3.4.0/src/shippo/models/components/trackingstatussubstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/transaction.py` & `shippo-3.4.0/src/shippo/models/components/instanttransactioncreateresponse.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,46 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
+from .instanttransactionrate import InstantTransactionRate
 from .labelfiletypeenum import LabelFileTypeEnum
 from .objectstateenum import ObjectStateEnum
+from .responsemessage import ResponseMessage
 from .trackingstatusenum import TrackingStatusEnum
 from .transactionstatusenum import TransactionStatusEnum
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from shippo import utils
 from typing import List, Optional
 
-
-@dataclasses.dataclass
-class TransactionMessages:
-    pass
-
-class ResponseType(str, Enum):
-    STANDARD = 'standard'
+class InstantTransactionCreateResponseResponseType(str, Enum):
+    INSTANT = 'instant'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Transaction:
+class InstantTransactionCreateResponse:
     commercial_invoice_url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('commercial_invoice_url'), 'exclude': lambda f: f is None }})
     r"""A URL pointing to the commercial invoice as a 8.5x11 inch PDF file.
     A value will only be returned if the Transactions has been processed successfully and if the shipment is international.
     """
     eta: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eta'), 'exclude': lambda f: f is None }})
     r"""The estimated time of arrival according to the carrier."""
     label_file_type: Optional[LabelFileTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('label_file_type'), 'exclude': lambda f: f is None }})
     r"""Print format of the <a href=\\"https://docs.goshippo.com/docs/shipments/shippinglabelsizes/\\">label</a>. If empty, will use the default format set from
     <a href=\"https://apps.goshippo.com/settings/labels\">the Shippo dashboard.</a>
     """
     label_url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('label_url'), 'exclude': lambda f: f is None }})
     r"""A URL pointing directly to the label in the format you've set in your settings.
     A value will only be returned if the Transactions has been processed successfully.
     """
-    messages: Optional[List[TransactionMessages]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('messages'), 'exclude': lambda f: f is None }})
-    r"""An array containing elements of the following schema:<br>
-    `code` (string): an identifier for the corresponding message (not always available)<br>
-    `message` (string): a publishable message containing further information.
-    """
+    messages: Optional[List[ResponseMessage]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('messages'), 'exclude': lambda f: f is None }})
     metadata: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
     r"""A string of up to 100 characters that can be filled with any additional information you want to
     attach to the object.
     """
     object_created: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_created'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
     r"""Date and time of Transaction creation."""
     object_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_id'), 'exclude': lambda f: f is None }})
@@ -72,14 +65,11 @@
     """
     tracking_status: Optional[TrackingStatusEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tracking_status'), 'exclude': lambda f: f is None }})
     r"""Indicates the high level status of the shipment."""
     tracking_url_provider: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tracking_url_provider'), 'exclude': lambda f: f is None }})
     r"""A link to track this item on the carrier-provided tracking website.
     A value will only be returned if tracking is available and the carrier provides such a service.
     """
-    rate: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('rate'), 'exclude': lambda f: f is None }})
-    r"""ID of the Rate object for which a Label has to be obtained.
-    Please note that only rates that are not older than 7 days can be purchased in order to ensure up-to-date pricing.
-    """
-    response_type: Optional[ResponseType] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('responseType'), 'exclude': lambda f: f is None }})
+    rate: Optional[InstantTransactionRate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('rate'), 'exclude': lambda f: f is None }})
+    response_type: Optional[InstantTransactionCreateResponseResponseType] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('responseType'), 'exclude': lambda f: f is None }})
```

### Comparing `shippo-3.3.5/src/shippo/models/components/transactioncreaterequest.py` & `shippo-3.4.0/src/shippo/models/components/transactioncreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/transactionpaginatedlist.py` & `shippo-3.4.0/src/shippo/models/components/responsemessage.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from .transaction import Transaction
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
-from typing import List, Optional
+from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class TransactionPaginatedList:
-    next: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})
-    previous: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
-    results: Optional[List[Transaction]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})
+class ResponseMessage:
+    r"""Message returned with supporting information from a request. In some cases this can be an error message,
+    for example a timeout from a carrier. If available, the origin of the message is displayed in `source`.
+    """
+    source: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('source'), 'exclude': lambda f: f is None }})
+    r"""Origin of message"""
+    code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('code'), 'exclude': lambda f: f is None }})
+    r"""Classification of message"""
+    text: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('text'), 'exclude': lambda f: f is None }})
+    r"""Message content"""
```

### Comparing `shippo-3.3.5/src/shippo/models/components/upsconnectexistingownaccountparameters.py` & `shippo-3.4.0/src/shippo/models/components/upsconnectexistingownaccountparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/userparceltemplate.py` & `shippo-3.4.0/src/shippo/models/components/userparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/userparceltemplateupdaterequest.py` & `shippo-3.4.0/src/shippo/models/components/userparceltemplateupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py` & `shippo-3.4.0/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py` & `shippo-3.4.0/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/errors/initiateoauth2signin.py` & `shippo-3.4.0/src/shippo/models/errors/initiateoauth2signin.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/errors/sdkerror.py` & `shippo-3.4.0/src/shippo/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/__init__.py` & `shippo-3.4.0/src/shippo/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/addshipmentstobatch.py` & `shippo-3.4.0/src/shippo/models/operations/addshipmentstobatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/deletedefaultparceltemplate.py` & `shippo-3.4.0/src/shippo/models/operations/deletedefaultparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/deleteservicegroup.py` & `shippo-3.4.0/src/shippo/models/operations/deleteservicegroup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/deleteuserparceltemplate.py` & `shippo-3.4.0/src/shippo/models/operations/deleteuserparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/getaddress.py` & `shippo-3.4.0/src/shippo/models/operations/getaddress.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/getbatch.py` & `shippo-3.4.0/src/shippo/models/operations/getbatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/getcarrieraccount.py` & `shippo-3.4.0/src/shippo/models/operations/getcarrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/getcarrierparceltemplate.py` & `shippo-3.4.0/src/shippo/models/operations/getcarrierparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/getcarrierregistrationstatus.py` & `shippo-3.4.0/src/shippo/models/operations/getcarrierregistrationstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/getcustomsdeclaration.py` & `shippo-3.4.0/src/shippo/models/operations/getcustomsdeclaration.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/getcustomsitem.py` & `shippo-3.4.0/src/shippo/models/operations/getcustomsitem.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/getdefaultparceltemplate.py` & `shippo-3.4.0/src/shippo/models/operations/getdefaultparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/getmanifest.py` & `shippo-3.4.0/src/shippo/models/operations/getmanifest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/getorder.py` & `shippo-3.4.0/src/shippo/models/operations/getorder.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/getparcel.py` & `shippo-3.4.0/src/shippo/models/operations/getparcel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/getrate.py` & `shippo-3.4.0/src/shippo/models/operations/getrate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/getrefund.py` & `shippo-3.4.0/src/shippo/models/operations/getrefund.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/getshipment.py` & `shippo-3.4.0/src/shippo/models/operations/getshipment.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/getshippoaccount.py` & `shippo-3.4.0/src/shippo/models/operations/getshippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/gettrack.py` & `shippo-3.4.0/src/shippo/models/operations/gettrack.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/gettransaction.py` & `shippo-3.4.0/src/shippo/models/operations/gettransaction.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/getuserparceltemplate.py` & `shippo-3.4.0/src/shippo/models/operations/getuserparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/initiateoauth2signin.py` & `shippo-3.4.0/src/shippo/models/operations/initiateoauth2signin.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/listaddresses.py` & `shippo-3.4.0/src/shippo/models/operations/listaddresses.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/listcarrieraccounts.py` & `shippo-3.4.0/src/shippo/models/operations/listcarrieraccounts.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/listcarrierparceltemplates.py` & `shippo-3.4.0/src/shippo/models/operations/listcarrierparceltemplates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/listcustomsdeclarations.py` & `shippo-3.4.0/src/shippo/models/operations/listcustomsdeclarations.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/listcustomsitems.py` & `shippo-3.4.0/src/shippo/models/operations/listcustomsitems.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/listmanifests.py` & `shippo-3.4.0/src/shippo/models/operations/listmanifests.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/listorders.py` & `shippo-3.4.0/src/shippo/models/operations/listorders.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/listparcels.py` & `shippo-3.4.0/src/shippo/models/operations/listparcels.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/listservicegroups.py` & `shippo-3.4.0/src/shippo/models/operations/listservicegroups.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/listshipmentrates.py` & `shippo-3.4.0/src/shippo/models/operations/listshipmentrates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/listshipmentratesbycurrencycode.py` & `shippo-3.4.0/src/shippo/models/operations/listshipmentratesbycurrencycode.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/listshipments.py` & `shippo-3.4.0/src/shippo/models/operations/listshipments.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/listshippoaccounts.py` & `shippo-3.4.0/src/shippo/models/operations/listshippoaccounts.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/listtransactions.py` & `shippo-3.4.0/src/shippo/models/operations/listtransactions.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/listuserparceltemplates.py` & `shippo-3.4.0/src/shippo/models/operations/listuserparceltemplates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/purchasebatch.py` & `shippo-3.4.0/src/shippo/models/operations/purchasebatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/removeshipmentsfrombatch.py` & `shippo-3.4.0/src/shippo/models/operations/removeshipmentsfrombatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/updatecarrieraccount.py` & `shippo-3.4.0/src/shippo/models/operations/updatecarrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/updateshippoaccount.py` & `shippo-3.4.0/src/shippo/models/operations/updateshippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/updateuserparceltemplate.py` & `shippo-3.4.0/src/shippo/models/operations/updateuserparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/models/operations/validateaddress.py` & `shippo-3.4.0/src/shippo/models/operations/validateaddress.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/orders.py` & `shippo-3.4.0/src/shippo/orders.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/parcels.py` & `shippo-3.4.0/src/shippo/parcels.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/pickups.py` & `shippo-3.4.0/src/shippo/pickups.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/rates.py` & `shippo-3.4.0/src/shippo/rates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/rates_at_checkout.py` & `shippo-3.4.0/src/shippo/rates_at_checkout.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/refunds.py` & `shippo-3.4.0/src/shippo/refunds.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/sdk.py` & `shippo-3.4.0/src/shippo/sdk.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/sdkconfiguration.py` & `shippo-3.4.0/src/shippo/sdkconfiguration.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
     client: requests_http.Session
     globals: internal.Globals
     security: Union[components.Security,Callable[[], components.Security]] = None
     server_url: Optional[str] = ''
     server_idx: Optional[int] = 0
     language: str = 'python'
     openapi_doc_version: str = '2018-02-08'
-    sdk_version: str = '3.3.5'
-    gen_version: str = '2.324.0'
-    user_agent: str = 'speakeasy-sdk/python 3.3.5 2.324.0 2018-02-08 shippo'
+    sdk_version: str = '3.4.0'
+    gen_version: str = '2.326.3'
+    user_agent: str = 'speakeasy-sdk/python 3.4.0 2.326.3 2018-02-08 shippo'
     retry_config: Optional[RetryConfig] = None
 
     def __post_init__(self):
         self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
```

### Comparing `shippo-3.3.5/src/shippo/service_groups.py` & `shippo-3.4.0/src/shippo/service_groups.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def update(self, request: Optional[components.ServiceGroupUpdateRequest]) -> components.ServiceGroup:
+    def update(self, request: Optional[components.ServiceGroupUpdateRequest] = None) -> components.ServiceGroup:
         r"""Update an existing service group
         Updates an existing service group object. <br>The object_id cannot be updated as it is the unique identifier for the object.
         """
         hook_ctx = HookContext(operation_id='UpdateServiceGroup', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         _globals = operations.UpdateServiceGroupGlobals(
             shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
         )
```

### Comparing `shippo-3.3.5/src/shippo/shipments.py` & `shippo-3.4.0/src/shippo/shipments.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/shippo_accounts.py` & `shippo-3.4.0/src/shippo/shippo_accounts.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/tracking_status.py` & `shippo-3.4.0/src/shippo/tracking_status.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/transactions.py` & `shippo-3.4.0/src/shippo/transactions.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/user_parcel_templates.py` & `shippo-3.4.0/src/shippo/user_parcel_templates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/utils/retries.py` & `shippo-3.4.0/src/shippo/utils/retries.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo/utils/utils.py` & `shippo-3.4.0/src/shippo/utils/utils.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.5/src/shippo.egg-info/PKG-INFO` & `shippo-3.4.0/src/shippo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: shippo
-Version: 3.3.5
+Version: 3.4.0
 Summary: Shipping API Python library (USPS, FedEx, UPS and more)
 Home-page: https://github.com/goshippo/shippo-python-sdk.git
 Author: Shippo
-License: UNKNOWN
+License: MIT License
 Description: # <img src="https://docs.goshippo.com/images/Logo.png" width="30" alt="Shippo logo"> Shippo Python SDK 
         
         Shippo is a shipping API that connects you with [multiple shipping carriers](https://goshippo.com/carriers) (such as USPS, UPS, DHL, Canada Post, Australia Post, and many others) through one interface.
         
         You must register for a [Shippo account](https://apps.goshippo.com/join) to use our API. It's free to sign up. Only pay to print a live label, test labels are free.
         
         To use the API, you must generate an [API Token](https://docs.goshippo.com/docs/guides_general/authentication/). In the following examples, replace `<YOUR_API_KEY_HERE>` with your own token.
```

### Comparing `shippo-3.3.5/src/shippo.egg-info/SOURCES.txt` & `shippo-3.4.0/src/shippo.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 src/shippo/__init__.py
 src/shippo/addresses.py
 src/shippo/batches.py
 src/shippo/carrier_accounts.py
 src/shippo/carrier_parcel_templates.py
@@ -42,14 +43,15 @@
 src/shippo/models/components/addressvalidationresults.py
 src/shippo/models/components/addressvalidationresultsmessage.py
 src/shippo/models/components/alcohol.py
 src/shippo/models/components/batch.py
 src/shippo/models/components/batchcreaterequest.py
 src/shippo/models/components/batchshipment.py
 src/shippo/models/components/batchshipmentbase.py
+src/shippo/models/components/batchshipmenterrormessage.py
 src/shippo/models/components/batchshipmentpaginatedlist.py
 src/shippo/models/components/billing.py
 src/shippo/models/components/carrieraccount.py
 src/shippo/models/components/carrieraccountbase.py
 src/shippo/models/components/carrieraccountcanadapostcreateparameters.py
 src/shippo/models/components/carrieraccountcanadapostcreaterequest.py
 src/shippo/models/components/carrieraccountchronopostcreaterequest.py
@@ -94,15 +96,14 @@
 src/shippo/models/components/dangerousgoodslithiumbatteries.py
 src/shippo/models/components/dangerousgoodsobject.py
 src/shippo/models/components/defaultparceltemplate.py
 src/shippo/models/components/defaultparceltemplateupdaterequest.py
 src/shippo/models/components/departmentnumber.py
 src/shippo/models/components/distanceunitenum.py
 src/shippo/models/components/dryice.py
-src/shippo/models/components/errormessage.py
 src/shippo/models/components/fedexconnectexistingownaccountparameters.py
 src/shippo/models/components/instanttransactioncreaterequest.py
 src/shippo/models/components/instanttransactioncreateresponse.py
 src/shippo/models/components/instanttransactionrate.py
 src/shippo/models/components/insurance.py
 src/shippo/models/components/invoicenumber.py
 src/shippo/models/components/labelfiletypeenum.py
@@ -127,19 +128,19 @@
 src/shippo/models/components/parcelpaginatedlist.py
 src/shippo/models/components/parcelrequest.py
 src/shippo/models/components/parceltemplateenumset.py
 src/shippo/models/components/pickup.py
 src/shippo/models/components/pickupbase.py
 src/shippo/models/components/ponumber.py
 src/shippo/models/components/rate.py
-src/shippo/models/components/ratemessage.py
 src/shippo/models/components/ratepaginatedlist.py
 src/shippo/models/components/refund.py
 src/shippo/models/components/refundpaginatedlist.py
 src/shippo/models/components/refundrequestbody.py
+src/shippo/models/components/responsemessage.py
 src/shippo/models/components/rmanumber.py
 src/shippo/models/components/security.py
 src/shippo/models/components/servicegroup.py
 src/shippo/models/components/servicegroupaccountandservicelevel.py
 src/shippo/models/components/servicegroupcreaterequest.py
 src/shippo/models/components/servicegrouptypeenum.py
 src/shippo/models/components/servicegroupupdaterequest.py
```

